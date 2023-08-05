# Comparing `tmp/MyGaiaDB-0.2.tar.gz` & `tmp/MyGaiaDB-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyGaiaDB-0.2.tar", last modified: Sat Apr  1 20:39:35 2023, max compression
+gzip compressed data, was "MyGaiaDB-0.3.tar", last modified: Sat Aug  5 20:28:14 2023, max compression
```

## Comparing `MyGaiaDB-0.2.tar` & `MyGaiaDB-0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.760006 MyGaiaDB-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.756006 MyGaiaDB-0.2/MyGaiaDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-04-01 20:39:35.000000 MyGaiaDB-0.2/MyGaiaDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-01 20:39:35.000000 MyGaiaDB-0.2/MyGaiaDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 20:39:35.000000 MyGaiaDB-0.2/MyGaiaDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-01 20:39:35.000000 MyGaiaDB-0.2/MyGaiaDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-01 20:39:35.000000 MyGaiaDB-0.2/MyGaiaDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-04-01 20:39:35.760006 MyGaiaDB-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19483 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.756006 MyGaiaDB-0.2/mygaiadb/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.756006 MyGaiaDB-0.2/mygaiadb/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33911 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/data/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/data/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.756006 MyGaiaDB-0.2/mygaiadb/ext_c/
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/ext_c/astroqlite.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.756006 MyGaiaDB-0.2/mygaiadb/query/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/query/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.756006 MyGaiaDB-0.2/mygaiadb/spec/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/mygaiadb/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 20:39:35.760006 MyGaiaDB-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:39:35.760006 MyGaiaDB-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-01 20:37:22.000000 MyGaiaDB-0.2/tests/test_mygaiadb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.376280 MyGaiaDB-0.3/MyGaiaDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-08-05 20:28:14.000000 MyGaiaDB-0.3/MyGaiaDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-05 20:28:14.000000 MyGaiaDB-0.3/MyGaiaDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 20:28:14.000000 MyGaiaDB-0.3/MyGaiaDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-05 20:28:14.000000 MyGaiaDB-0.3/MyGaiaDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 20:28:14.000000 MyGaiaDB-0.3/MyGaiaDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22398 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.376280 MyGaiaDB-0.3/mygaiadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/mygaiadb/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41270 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/data/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/data/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/mygaiadb/ext_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/ext_c/astroqlite.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/mygaiadb/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/query/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/mygaiadb/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/mygaiadb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:28:14.380280 MyGaiaDB-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/tests/test_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-05 20:26:36.000000 MyGaiaDB-0.3/tests/test_mygaiadb.py
```

### Comparing `MyGaiaDB-0.2/LICENSE` & `MyGaiaDB-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MyGaiaDB-0.2/MyGaiaDB.egg-info/PKG-INFO` & `MyGaiaDB-0.3/MyGaiaDB.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyGaiaDB
-Version: 0.2
+Version: 0.3
 Summary: Setup local serverless ESA Gaia / 2MASS / ALLWISE databases and run query locally with python
 Home-page: https://github.com/henrysky/MyGaiaDB
 Author: Henry Leung
 Author-email: henrysky.leung@utoronto.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/henrysky/MyGaiaDB/issues
 Project-URL: Documentation, https://github.com/henrysky/MyGaiaDB
@@ -21,57 +21,59 @@
 
 MyGaiaDB
 ===============
 
 *Why share when you can have the whole Gaia database on your own locally?*
 
 ``MyGaiaDB`` is simple python package with a set of scripts to help you setup a local 
-Gaia **DR3** database (also local 2MASS and ALLWISE databases too) without the need of administrator privilege 
+Gaia **DR3** database (local 2MASS, ALLWISE and CATWISE databases too) without the need of administrator privilege 
 and is compatible to all major platforms (Linux, Mac and Windows) because ``MyGaiaDB`` is **serverless** 
-and requires Python only using ``sqlite`` as long as you have enough disk space.
+which requires Python only using ``sqlite`` as long as you have enough disk space.
 
 This code is mainly to help myself managing data for my research project with Gaia DR3 XP spectra 
 and not meant to fit research usage from every aspect of Gaia's 1 billion stars. The main motivation of this 
-code is to make setting up local Gaia database with 2MASS and ALLWISE accessible to everyone. Possible use cases include 
-but not limited to make very long complex query cross-matching to multiple databases that can take a long time 
+code is to make setting up local Gaia database with 2MASS, ALLWISE and CATWISE accessible to everyone. Possible use cases include 
+but not limited to making very long complex query cross-matching to multiple databases that can take a long time 
 to finish (where the online ESA `Gaia archive`_ has timeout limitation).
 
 You are welcome to modify the code, make pull request to make this code to suit your and others need.
 
-**Part of this code will never be continuously tested properly since no way I can run this code with a few TB of gaia data on Github Actions**
+..
+
+    Part of this code will never be continuously tested properly since no way I can run this code with a few TBs of gaia data on Github Actions
 
 .. contents:: **Table of Contents**
     :depth: 3
 
 Installation and Dependencies
 -------------------------------
 
 This code requires ``python >= 3.8`` with ``numpy``, ``pandas``, ``h5py``, ``astropy`` and ``tqdm`` while only need to use 
 ``sqlite3`` bundled with your python installation without additional installation.
 Some optional functionalities require ``galpy``, ``mwdust``. Downloading functions require ``wget``.
 
 You can simply do ``pip install mygaiadb`` to install compiled ``MyGaiaDB`` wheels.
 
 Otherwise, you need to compile the code locally from source code. You need to add the folder which contains ``sqlite3ext.h`` to **INCLUDE** environment variable.
-If you are using Conda, you can do ``set INCLUDE=%CONDA_PREFIX%\Library\include;%INCLUDE%`` for Windows CMD or ``$env:INCLUDE="$env:CONDA_PREFIX\Library\include"`` for Windows PowerShell 
+If you are using Conda, you can do ``set INCLUDE=%CONDA_PREFIX%\Library\include;%INCLUDE%`` for Windows Command Prompt or ``$env:INCLUDE="$env:CONDA_PREFIX\Library\include"`` for Windows PowerShell 
 or ``export CFLAGS=-I$CONDA_PREFIX/include`` for MacOS or nothing for Linux. Then you can run ``python -m pip install .`` to install the 
 latest commits from github or ``python -m pip install -e .``  to develop ``MyGaiaDB`` locally.
 
 Folder Structure
 -------------------
 
 You need to make sure you have at least ~8TB of free disk space with fast **random read** speed for optimal query performance. 
 First set an environment variable called **MY_ASTRO_DATA** which point to a folder that (will) contains your 
 astronomical data in general. To be compatible with other python package, under **MY_ASTRO_DATA** there should be a folder called ``gaia_mirror`` that contains all 
 gaia data (i.e. **GAIA_TOOLS_DATA** environment variable from Jo Bovy's gaia_tools_).
 
 .. _apogee: https://github.com/jobovy/apogee
 .. _gaia_tools: https://github.com/jobovy/gaia_tools
 
-If you start from scratch, you only need to set **MY_ASTRO_DATA** environment variable and ``MyGaiaDB`` will populate the files and folders. 
+If you start from scratch on a clean computer, you only need to set **MY_ASTRO_DATA** environment variable and ``MyGaiaDB`` will populate the files and folders. 
 ``MyGaiaDB`` will use ``~/.mygaiadb`` folder to save user specific settings and tables.
 
 If you already have the data on your computer but in a different directory structure and you do not want or can not move them, 
 you can use symbolic link to create the required folder structure without 
 duplicating files. For Linux and MacOS, you can use ``ln -s {source-dir-or-file-path} {symbolic-dir-or-file-path}``. 
 For Windows, you can use ``mklink {symbolic-file-path} {source-file-path}`` or ``mklink /D {symbolic-dir-path} {source-dir-path}``. 
 The **case sensitive** folder structure should look something like the following chart:
@@ -122,19 +124,27 @@
     │   │   │   │   │   ├── XpSampledMeanSpectrum_000000-003111.csv.gz
     │   │   │   │   │   ├── ******
     │   │   │   │   │   └── XpSampledMeanSpectrum_786097-786431.csv.gz
     ├── 2mass_mirror/
     │   ├── psc_aaa.gz
     │   ├── ******
     │   └── xsc_baa.gz
-    └── allwise_mirror/
-        ├── wise-allwise-cat-part01.bz2
-        ├── ******
-        └── wise-allwise-cat-part48.bz2
-
+    ├── allwise_mirror/
+    │   ├── wise-allwise-cat-part01.bz2
+    │   ├── ******
+    │   └── wise-allwise-cat-part48.bz2
+    └── catwise_mirror/
+        └── 2020/
+            ├── 000/
+            │   ├── 0000m016_opt1_20191208_213403_ab_v5_cat_b0.tbl.gz
+            │   └── ******
+            ├── 001/
+            │   ├── 0015m016_opt1_20191209_054819_ab_v5_cat_b0.tbl.gz
+            │   └── ******
+            └── ******
 
 Downloading Data
 ---------------------------
 
 To download with ``MyGaiaDB``, you can do
 
 ..  code-block:: python
@@ -149,58 +159,63 @@
     download.download_2mass_best_neightbour()
     # for allwise best neightbour
     download.download_allwise_best_neightbour()
     # for 2MASS
     download.download_2mass()
     # for allwise
     download.download_allwise()
+    # for catwise
+    download.download_catwise()
     # for xp continuous
     download.download_gaia_xp_continuous()
     # for xp sampled
     download.download_gaia_xp_sampled()    
     # for rvs spectra
     download.download_gaia_rvs()
 
 
 Official data links:
 
 * Official Gaia data can be accessed here: https://cdn.gea.esac.esa.int/Gaia/
 * Official 2MASS data can be accessed here: https://irsa.ipac.caltech.edu/2MASS/download/allsky/
 * Official ALLWISE data can be accessed here: https://irsa.ipac.caltech.edu/data/download/wise-allwise/
+* Official CATWISE data can be accessed here: https://catwise.github.io/
 
 Compiling Databases
 ---------------------
 Here are functions to compile databases (each function only need to be ran once on each computer you store the data). 
 **Each function will generate large sized file(s)**. Moreover, if you are using a shared computing server, 
 only one user need to run the functions and share **MY_ASTRO_DATA** folder path to other user so
 they can setup their own environment variable **MY_ASTRO_DATA** to that folder too. Multiple users can use the SQL 
-database at the same time since ``MyGaiaDB`` will set read-only permission mission before loading databases.
+database at the same time since ``MyGaiaDB`` will set read-only permission before loading databases to prevent accidential modification.
 
 ..  code-block:: python
 
     from mygaiadb import compile
 
     # compile Gaia SQL dataset
     compile.compile_gaia_sql_db()
     # compile 2MASS SQL dataset
     compile.compile_tmass_sql_db()
     # compile ALLWISE SQL dataset
     compile.compile_allwise_sql_db()
+    # compile CATWISE SQL dataset
+    compile.compile_catwise_sql_db()
 
     # turn compressed XP coeffs files to h5, with options to save correlation matrix too
     compile.compile_xp_continuous_h5(save_correlation_matrix=False)
     # compile all XP coeffs into a single h5, partitioned batches of stars by their HEALPix
     compile.compile_xp_continuous_allinone_h5()
 
 SQL Databases Data Model
 ---------------------------
 
 Currently for Gaia DR3 in ``MyGaiaDB``, these databases are only available if you have compiled all of them: 
 ``gaiadr3.gaia_source``, ``gaiadr3.allwise_best_neighbour``, ``gaiadr3.tmasspscxsc_best_neighbour``, 
-``gaiadr3.astrophysical_parameters``, ``tmass.twomass_psc``, ``allwise.allwise``. But there are a few 
+``gaiadr3.astrophysical_parameters``, ``tmass.twomass_psc``, ``allwise.allwise``, ``catwise.catwise``. But there are a few 
 utility functions to see list of tables and table's columns. Brief description of the tables are as following:
 
 -   | ``gaiadr3.gaia_source``
     | This table mimics ``gaia_source_lite`` on `Gaia Archive`_ with addition of ``grvs_mag`` columns
     | Official description: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_main_source_catalogue/ssec_dm_gaia_source.html
 -   | ``gaiadr3.allwise_best_neighbour``
     | This table is identical to ``allwise_best_neighbour`` on `Gaia Archive`_
@@ -213,14 +228,17 @@
     | Official description: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_astrophysical_parameter_tables/ssec_dm_astrophysical_parameters.html
 -   | ``tmass.twomass_psc``
     | This table is a lite version of 2MASS Point Source Catalog (PSC) with only essential useful columns are kept
     | Official description: https://irsa.ipac.caltech.edu/2MASS/download/allsky/format_psc.html
 -   | ``allwise.allwise``
     | This table is a lite version of ALLWISE source catalog with only essential useful columns are kept
     | Official description: https://wise2.ipac.caltech.edu/docs/release/allwise/expsup/sec2_1a.html
+-   | ``catwise.catwise``
+    | This table is a lite version of CATWISE source catalog with only essential useful columns are kept
+    | Official description: https://irsa.ipac.caltech.edu/data/WISE/CatWISE/gator_docs/catwise_colDescriptions.html
 
 You can use ``list_all_tables()`` to get a list of tables excluding ``user_table``. do 
 
 ..  code-block:: python
 
     from mygaiadb.query import LocalGaiaSQL
 
@@ -274,14 +292,29 @@
         SELECT DISTANCE(179., 10., G.ra, G.dec) as ang_sep
         FROM gaiadr3.gaia_source as G
         WHERE G.source_id = 4472832130942575872
     """)
 
 and you will get the same result of 89.618118.
 
+For example the following query which utilize conventional maths function to approximate uncertainty in Gaia G magnitude
+
+..  code-block:: python
+
+    from mygaiadb.query import LocalGaiaSQL
+
+    # initialize a local Gaia SQL database instance
+    local_db = LocalGaiaSQL()
+    # CDS equation for conversion: http://vizier.cds.unistra.fr/viz-bin/VizieR-n?-source=METAnot&catid=1350&notid=63&-out=text
+    local_db.query("""
+        SELECT sqrt(power(((2.5 / log(10)) * (1 / G.phot_g_mean_flux_over_error)), 2) + power(0.0027553202, 2)) as phot_g_mean_mag_error
+        FROM gaiadr3.gaia_source as G
+        WHERE G.source_id = 3158175803069175680
+    """)
+
 Another example is the following query that works on `Gaia Archive`_ will also work in ``MyGaiaDB`` to select the first 100 gaia sources with XP coefficients
 
 ..  code-block:: sql
 
     SELECT TOP 100 * 
     FROM gaiadr3.gaia_source as G 
     WHERE (G.has_xp_continuous = 'True')
@@ -317,17 +350,27 @@
     INNER JOIN gaiadr3.allwise_best_neighbour as W on W.source_id = T.source_id
     INNER JOIN tmass.twomass_psc as TM on TM.designation = T.original_ext_source_id
     INNER JOIN allwise.allwise as AW on AW.designation = W.original_ext_source_id
     WHERE (G.has_xp_continuous = 1) AND (G.ruwe < 1.4) AND (G.ipd_frac_multi_peak <= 2) AND (G.ipd_gof_harmonic_amplitude<0.1) AND (GA.logg_gspspec < 3.0)
     """
 
     # take ~12 hours to complete
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True)
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, comments=True)
 
-As you can see for ``has_xp_continuous``, we can also use ``1`` to represent ``true`` which is used by Gaia archive but both are fine with ``MyGaiaDB``.
+As you can see for ``has_xp_continuous``, we can also use ``1`` to represent ``true`` which is used by Gaia archive but both are fine with ``MyGaiaDB``. 
+The ``overwrite=True`` means the function will save the file even if the file with the same name already exists. The ``comments=True`` means the function will 
+save the query as a comment in the csv file so you know how to reproduce the query result. To read the comments from the csv file, you can use the following code
+
+..  code-block:: python
+
+    from itertools import takewhile
+    with open("output.csv", "r") as fobj:
+        headiter = takewhile(lambda s: s.startswith("#"), fobj)
+        header = list(headiter)
+    print(" ".join(header).replace(" # ", "").replace("# ", ""))
 
 ``MyGaiaDB`` also has callbacks functionality called ``QueryCallback``, these callbacks can be used when you do query. For example, 
 you can create a callbacks to convert ``ra`` in degree to `ra_rad` in radian. So your csv file in the end will have a new column 
 called ``ra_rad``. Functions in ``QueryCallback`` must have arguments with **exact** column names in your query so ``MyGaiaDB`` knows 
 which columns to use on the fly.
 
 ..  code-block:: python
@@ -341,15 +384,15 @@
     query = """
     SELECT G.source_id, G.ra, G.dec
     FROM gaiadr3.gaia_source as G
     LIMIT 100000
     """
     ra_conversion = QueryCallback(new_col_name="ra_rad", func=lambda ra: ra / 180 * np.pi)
 
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True, callbacks=[ra_conversion])
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, callbacks=[ra_conversion], comments=True)
 
 We also have a few useful callbacks included by default to add columns like zero-point corrected parallax or extinction
 
 ..  code-block:: python
 
     from mygaiadb.query import ZeroPointCallback, DustCallback
 
@@ -360,26 +403,26 @@
     """
 
     # adding zero-point corrected parallax using official Gaia DR3 parallax zero-point python package
     zp_callback = ZeroPointCallback(new_col_name="parallax_w_zp")
     # adding SFD E(B-V) in H band filter using mwdust python package
     dust_callback = DustCallback(new_col_name="sfd_ebv", filter="H", dustmap="SFD")
 
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True, callbacks=[zp_callback, dust_callback])
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, callbacks=[zp_callback, dust_callback])
 
 User tables
 -------------
 
 ``MyGaiaDB`` support the use of user uploaded table. You can load your table first by ``pandas`` and then do
 
 ..  code-block:: python
 
     from mygaiadb.query import LocalGaiaSQL 
-    localdb = LocalGaiaSQL()  
-    localdb.upload_user_table(pd.DataFrame({"source_id": [5188146770731873152, 4611686018427432192, 5764607527332179584]}), tablename="my_table_1")
+    local_db = LocalGaiaSQL()  
+    local_db.upload_user_table(pd.DataFrame({"source_id": [5188146770731873152, 4611686018427432192, 5764607527332179584]}), tablename="my_table_1")
 
 and then carry-on doing query with ``my_table_1`` cross-matching with other tables like 
 
 ..  code-block:: python
 
     local_db.query("""SELECT * FROM gaiadr3.gaia_source as G  INNER JOIN user_table.my_table_1 as MY on MY.source_id = G.source_id""")
 
@@ -389,39 +432,48 @@
 
     local_db.list_user_tables()
 
 and you can remove a user table like ``my_table_1`` in this case by using ``remove_user_table()``
 
 ..  code-block:: python
 
-    a.remove_user_table("my_table_1")
+    local_db.remove_user_table("my_table_1")
 
-Spectroscopy Query
---------------------
+Gaia XP Spectroscopy Query
+----------------------------
 
 There can be use case where you want to run a function (e.g., a machine learning model) to a large batch of source_id with reasonable memory usage. 
 You can use ``MyGaiaDB`` to do that in batch provided you have compiled a single h5 with ``mygaiadb.compile.compile_xp_continuous_allinone_h5()``
 
 ..  code-block:: python
 
     from mygaiadb.spec import yield_xp_coeffs
 
     for i in yield_xp_coeffs(a_very_long_source_id_array):
         coeffs, idx = i
         # XP coeffs of idx from the original a_very_long_source_id_array
 
-For example you want to infer ``M_H`` with your machine learning model
+    # alternatively if you also want coeffs error
+    for i in yield_xp_coeffs(a_very_long_source_id_array, return_errors=True):
+        coeffs, idx, coeffs_err = i  # unpack
+
+    # alternatively if you want coeffs error and some other columns like bp_n_relevant_basesand rp_n_relevant_bases
+    # ref: https://gea.esac.esa.int/archive/documentation/GDR3//Gaia_archive/chap_datamodel/sec_dm_spectroscopic_tables/ssec_dm_xp_summary.html
+    for i in yield_xp_coeffs(a_very_long_source_id_array, return_errors=True, return_additional_columns=["bp_n_relevant_bases", "rp_n_relevant_bases"]):
+        coeffs, idx, coeffs_err, bp_n_relevant_bases, rp_n_relevant_bases = i  # unpack
+
+For example you want to infer ``M_H`` with your machine learning model on many XP spectra
 
 ..  code-block:: python
 
     from mygaiadb.spec import yield_xp_coeffs
 
-    m_h = np.ones(len(a_very_long_source_id_array)) * -9999.
+    m_h = np.ones(len(a_very_long_source_id_array)) * np.nan
     for i in yield_xp_coeffs(a_very_long_source_id_array):
-        coeffs, idx = i
+        coeffs, idx = i  # unpack
         m_h[idx] = your_ml_model(coeffs)
 
 Author
 -------------
 -  | **Henry Leung** - henrysky_
    | University of Toronto
    | Contact Henry: henrysky.leung [at] utoronto.ca
```

### Comparing `MyGaiaDB-0.2/PKG-INFO` & `MyGaiaDB-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyGaiaDB
-Version: 0.2
+Version: 0.3
 Summary: Setup local serverless ESA Gaia / 2MASS / ALLWISE databases and run query locally with python
 Home-page: https://github.com/henrysky/MyGaiaDB
 Author: Henry Leung
 Author-email: henrysky.leung@utoronto.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/henrysky/MyGaiaDB/issues
 Project-URL: Documentation, https://github.com/henrysky/MyGaiaDB
@@ -21,57 +21,59 @@
 
 MyGaiaDB
 ===============
 
 *Why share when you can have the whole Gaia database on your own locally?*
 
 ``MyGaiaDB`` is simple python package with a set of scripts to help you setup a local 
-Gaia **DR3** database (also local 2MASS and ALLWISE databases too) without the need of administrator privilege 
+Gaia **DR3** database (local 2MASS, ALLWISE and CATWISE databases too) without the need of administrator privilege 
 and is compatible to all major platforms (Linux, Mac and Windows) because ``MyGaiaDB`` is **serverless** 
-and requires Python only using ``sqlite`` as long as you have enough disk space.
+which requires Python only using ``sqlite`` as long as you have enough disk space.
 
 This code is mainly to help myself managing data for my research project with Gaia DR3 XP spectra 
 and not meant to fit research usage from every aspect of Gaia's 1 billion stars. The main motivation of this 
-code is to make setting up local Gaia database with 2MASS and ALLWISE accessible to everyone. Possible use cases include 
-but not limited to make very long complex query cross-matching to multiple databases that can take a long time 
+code is to make setting up local Gaia database with 2MASS, ALLWISE and CATWISE accessible to everyone. Possible use cases include 
+but not limited to making very long complex query cross-matching to multiple databases that can take a long time 
 to finish (where the online ESA `Gaia archive`_ has timeout limitation).
 
 You are welcome to modify the code, make pull request to make this code to suit your and others need.
 
-**Part of this code will never be continuously tested properly since no way I can run this code with a few TB of gaia data on Github Actions**
+..
+
+    Part of this code will never be continuously tested properly since no way I can run this code with a few TBs of gaia data on Github Actions
 
 .. contents:: **Table of Contents**
     :depth: 3
 
 Installation and Dependencies
 -------------------------------
 
 This code requires ``python >= 3.8`` with ``numpy``, ``pandas``, ``h5py``, ``astropy`` and ``tqdm`` while only need to use 
 ``sqlite3`` bundled with your python installation without additional installation.
 Some optional functionalities require ``galpy``, ``mwdust``. Downloading functions require ``wget``.
 
 You can simply do ``pip install mygaiadb`` to install compiled ``MyGaiaDB`` wheels.
 
 Otherwise, you need to compile the code locally from source code. You need to add the folder which contains ``sqlite3ext.h`` to **INCLUDE** environment variable.
-If you are using Conda, you can do ``set INCLUDE=%CONDA_PREFIX%\Library\include;%INCLUDE%`` for Windows CMD or ``$env:INCLUDE="$env:CONDA_PREFIX\Library\include"`` for Windows PowerShell 
+If you are using Conda, you can do ``set INCLUDE=%CONDA_PREFIX%\Library\include;%INCLUDE%`` for Windows Command Prompt or ``$env:INCLUDE="$env:CONDA_PREFIX\Library\include"`` for Windows PowerShell 
 or ``export CFLAGS=-I$CONDA_PREFIX/include`` for MacOS or nothing for Linux. Then you can run ``python -m pip install .`` to install the 
 latest commits from github or ``python -m pip install -e .``  to develop ``MyGaiaDB`` locally.
 
 Folder Structure
 -------------------
 
 You need to make sure you have at least ~8TB of free disk space with fast **random read** speed for optimal query performance. 
 First set an environment variable called **MY_ASTRO_DATA** which point to a folder that (will) contains your 
 astronomical data in general. To be compatible with other python package, under **MY_ASTRO_DATA** there should be a folder called ``gaia_mirror`` that contains all 
 gaia data (i.e. **GAIA_TOOLS_DATA** environment variable from Jo Bovy's gaia_tools_).
 
 .. _apogee: https://github.com/jobovy/apogee
 .. _gaia_tools: https://github.com/jobovy/gaia_tools
 
-If you start from scratch, you only need to set **MY_ASTRO_DATA** environment variable and ``MyGaiaDB`` will populate the files and folders. 
+If you start from scratch on a clean computer, you only need to set **MY_ASTRO_DATA** environment variable and ``MyGaiaDB`` will populate the files and folders. 
 ``MyGaiaDB`` will use ``~/.mygaiadb`` folder to save user specific settings and tables.
 
 If you already have the data on your computer but in a different directory structure and you do not want or can not move them, 
 you can use symbolic link to create the required folder structure without 
 duplicating files. For Linux and MacOS, you can use ``ln -s {source-dir-or-file-path} {symbolic-dir-or-file-path}``. 
 For Windows, you can use ``mklink {symbolic-file-path} {source-file-path}`` or ``mklink /D {symbolic-dir-path} {source-dir-path}``. 
 The **case sensitive** folder structure should look something like the following chart:
@@ -122,19 +124,27 @@
     │   │   │   │   │   ├── XpSampledMeanSpectrum_000000-003111.csv.gz
     │   │   │   │   │   ├── ******
     │   │   │   │   │   └── XpSampledMeanSpectrum_786097-786431.csv.gz
     ├── 2mass_mirror/
     │   ├── psc_aaa.gz
     │   ├── ******
     │   └── xsc_baa.gz
-    └── allwise_mirror/
-        ├── wise-allwise-cat-part01.bz2
-        ├── ******
-        └── wise-allwise-cat-part48.bz2
-
+    ├── allwise_mirror/
+    │   ├── wise-allwise-cat-part01.bz2
+    │   ├── ******
+    │   └── wise-allwise-cat-part48.bz2
+    └── catwise_mirror/
+        └── 2020/
+            ├── 000/
+            │   ├── 0000m016_opt1_20191208_213403_ab_v5_cat_b0.tbl.gz
+            │   └── ******
+            ├── 001/
+            │   ├── 0015m016_opt1_20191209_054819_ab_v5_cat_b0.tbl.gz
+            │   └── ******
+            └── ******
 
 Downloading Data
 ---------------------------
 
 To download with ``MyGaiaDB``, you can do
 
 ..  code-block:: python
@@ -149,58 +159,63 @@
     download.download_2mass_best_neightbour()
     # for allwise best neightbour
     download.download_allwise_best_neightbour()
     # for 2MASS
     download.download_2mass()
     # for allwise
     download.download_allwise()
+    # for catwise
+    download.download_catwise()
     # for xp continuous
     download.download_gaia_xp_continuous()
     # for xp sampled
     download.download_gaia_xp_sampled()    
     # for rvs spectra
     download.download_gaia_rvs()
 
 
 Official data links:
 
 * Official Gaia data can be accessed here: https://cdn.gea.esac.esa.int/Gaia/
 * Official 2MASS data can be accessed here: https://irsa.ipac.caltech.edu/2MASS/download/allsky/
 * Official ALLWISE data can be accessed here: https://irsa.ipac.caltech.edu/data/download/wise-allwise/
+* Official CATWISE data can be accessed here: https://catwise.github.io/
 
 Compiling Databases
 ---------------------
 Here are functions to compile databases (each function only need to be ran once on each computer you store the data). 
 **Each function will generate large sized file(s)**. Moreover, if you are using a shared computing server, 
 only one user need to run the functions and share **MY_ASTRO_DATA** folder path to other user so
 they can setup their own environment variable **MY_ASTRO_DATA** to that folder too. Multiple users can use the SQL 
-database at the same time since ``MyGaiaDB`` will set read-only permission mission before loading databases.
+database at the same time since ``MyGaiaDB`` will set read-only permission before loading databases to prevent accidential modification.
 
 ..  code-block:: python
 
     from mygaiadb import compile
 
     # compile Gaia SQL dataset
     compile.compile_gaia_sql_db()
     # compile 2MASS SQL dataset
     compile.compile_tmass_sql_db()
     # compile ALLWISE SQL dataset
     compile.compile_allwise_sql_db()
+    # compile CATWISE SQL dataset
+    compile.compile_catwise_sql_db()
 
     # turn compressed XP coeffs files to h5, with options to save correlation matrix too
     compile.compile_xp_continuous_h5(save_correlation_matrix=False)
     # compile all XP coeffs into a single h5, partitioned batches of stars by their HEALPix
     compile.compile_xp_continuous_allinone_h5()
 
 SQL Databases Data Model
 ---------------------------
 
 Currently for Gaia DR3 in ``MyGaiaDB``, these databases are only available if you have compiled all of them: 
 ``gaiadr3.gaia_source``, ``gaiadr3.allwise_best_neighbour``, ``gaiadr3.tmasspscxsc_best_neighbour``, 
-``gaiadr3.astrophysical_parameters``, ``tmass.twomass_psc``, ``allwise.allwise``. But there are a few 
+``gaiadr3.astrophysical_parameters``, ``tmass.twomass_psc``, ``allwise.allwise``, ``catwise.catwise``. But there are a few 
 utility functions to see list of tables and table's columns. Brief description of the tables are as following:
 
 -   | ``gaiadr3.gaia_source``
     | This table mimics ``gaia_source_lite`` on `Gaia Archive`_ with addition of ``grvs_mag`` columns
     | Official description: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_main_source_catalogue/ssec_dm_gaia_source.html
 -   | ``gaiadr3.allwise_best_neighbour``
     | This table is identical to ``allwise_best_neighbour`` on `Gaia Archive`_
@@ -213,14 +228,17 @@
     | Official description: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_astrophysical_parameter_tables/ssec_dm_astrophysical_parameters.html
 -   | ``tmass.twomass_psc``
     | This table is a lite version of 2MASS Point Source Catalog (PSC) with only essential useful columns are kept
     | Official description: https://irsa.ipac.caltech.edu/2MASS/download/allsky/format_psc.html
 -   | ``allwise.allwise``
     | This table is a lite version of ALLWISE source catalog with only essential useful columns are kept
     | Official description: https://wise2.ipac.caltech.edu/docs/release/allwise/expsup/sec2_1a.html
+-   | ``catwise.catwise``
+    | This table is a lite version of CATWISE source catalog with only essential useful columns are kept
+    | Official description: https://irsa.ipac.caltech.edu/data/WISE/CatWISE/gator_docs/catwise_colDescriptions.html
 
 You can use ``list_all_tables()`` to get a list of tables excluding ``user_table``. do 
 
 ..  code-block:: python
 
     from mygaiadb.query import LocalGaiaSQL
 
@@ -274,14 +292,29 @@
         SELECT DISTANCE(179., 10., G.ra, G.dec) as ang_sep
         FROM gaiadr3.gaia_source as G
         WHERE G.source_id = 4472832130942575872
     """)
 
 and you will get the same result of 89.618118.
 
+For example the following query which utilize conventional maths function to approximate uncertainty in Gaia G magnitude
+
+..  code-block:: python
+
+    from mygaiadb.query import LocalGaiaSQL
+
+    # initialize a local Gaia SQL database instance
+    local_db = LocalGaiaSQL()
+    # CDS equation for conversion: http://vizier.cds.unistra.fr/viz-bin/VizieR-n?-source=METAnot&catid=1350&notid=63&-out=text
+    local_db.query("""
+        SELECT sqrt(power(((2.5 / log(10)) * (1 / G.phot_g_mean_flux_over_error)), 2) + power(0.0027553202, 2)) as phot_g_mean_mag_error
+        FROM gaiadr3.gaia_source as G
+        WHERE G.source_id = 3158175803069175680
+    """)
+
 Another example is the following query that works on `Gaia Archive`_ will also work in ``MyGaiaDB`` to select the first 100 gaia sources with XP coefficients
 
 ..  code-block:: sql
 
     SELECT TOP 100 * 
     FROM gaiadr3.gaia_source as G 
     WHERE (G.has_xp_continuous = 'True')
@@ -317,17 +350,27 @@
     INNER JOIN gaiadr3.allwise_best_neighbour as W on W.source_id = T.source_id
     INNER JOIN tmass.twomass_psc as TM on TM.designation = T.original_ext_source_id
     INNER JOIN allwise.allwise as AW on AW.designation = W.original_ext_source_id
     WHERE (G.has_xp_continuous = 1) AND (G.ruwe < 1.4) AND (G.ipd_frac_multi_peak <= 2) AND (G.ipd_gof_harmonic_amplitude<0.1) AND (GA.logg_gspspec < 3.0)
     """
 
     # take ~12 hours to complete
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True)
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, comments=True)
 
-As you can see for ``has_xp_continuous``, we can also use ``1`` to represent ``true`` which is used by Gaia archive but both are fine with ``MyGaiaDB``.
+As you can see for ``has_xp_continuous``, we can also use ``1`` to represent ``true`` which is used by Gaia archive but both are fine with ``MyGaiaDB``. 
+The ``overwrite=True`` means the function will save the file even if the file with the same name already exists. The ``comments=True`` means the function will 
+save the query as a comment in the csv file so you know how to reproduce the query result. To read the comments from the csv file, you can use the following code
+
+..  code-block:: python
+
+    from itertools import takewhile
+    with open("output.csv", "r") as fobj:
+        headiter = takewhile(lambda s: s.startswith("#"), fobj)
+        header = list(headiter)
+    print(" ".join(header).replace(" # ", "").replace("# ", ""))
 
 ``MyGaiaDB`` also has callbacks functionality called ``QueryCallback``, these callbacks can be used when you do query. For example, 
 you can create a callbacks to convert ``ra`` in degree to `ra_rad` in radian. So your csv file in the end will have a new column 
 called ``ra_rad``. Functions in ``QueryCallback`` must have arguments with **exact** column names in your query so ``MyGaiaDB`` knows 
 which columns to use on the fly.
 
 ..  code-block:: python
@@ -341,15 +384,15 @@
     query = """
     SELECT G.source_id, G.ra, G.dec
     FROM gaiadr3.gaia_source as G
     LIMIT 100000
     """
     ra_conversion = QueryCallback(new_col_name="ra_rad", func=lambda ra: ra / 180 * np.pi)
 
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True, callbacks=[ra_conversion])
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, callbacks=[ra_conversion], comments=True)
 
 We also have a few useful callbacks included by default to add columns like zero-point corrected parallax or extinction
 
 ..  code-block:: python
 
     from mygaiadb.query import ZeroPointCallback, DustCallback
 
@@ -360,26 +403,26 @@
     """
 
     # adding zero-point corrected parallax using official Gaia DR3 parallax zero-point python package
     zp_callback = ZeroPointCallback(new_col_name="parallax_w_zp")
     # adding SFD E(B-V) in H band filter using mwdust python package
     dust_callback = DustCallback(new_col_name="sfd_ebv", filter="H", dustmap="SFD")
 
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True, callbacks=[zp_callback, dust_callback])
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, callbacks=[zp_callback, dust_callback])
 
 User tables
 -------------
 
 ``MyGaiaDB`` support the use of user uploaded table. You can load your table first by ``pandas`` and then do
 
 ..  code-block:: python
 
     from mygaiadb.query import LocalGaiaSQL 
-    localdb = LocalGaiaSQL()  
-    localdb.upload_user_table(pd.DataFrame({"source_id": [5188146770731873152, 4611686018427432192, 5764607527332179584]}), tablename="my_table_1")
+    local_db = LocalGaiaSQL()  
+    local_db.upload_user_table(pd.DataFrame({"source_id": [5188146770731873152, 4611686018427432192, 5764607527332179584]}), tablename="my_table_1")
 
 and then carry-on doing query with ``my_table_1`` cross-matching with other tables like 
 
 ..  code-block:: python
 
     local_db.query("""SELECT * FROM gaiadr3.gaia_source as G  INNER JOIN user_table.my_table_1 as MY on MY.source_id = G.source_id""")
 
@@ -389,39 +432,48 @@
 
     local_db.list_user_tables()
 
 and you can remove a user table like ``my_table_1`` in this case by using ``remove_user_table()``
 
 ..  code-block:: python
 
-    a.remove_user_table("my_table_1")
+    local_db.remove_user_table("my_table_1")
 
-Spectroscopy Query
---------------------
+Gaia XP Spectroscopy Query
+----------------------------
 
 There can be use case where you want to run a function (e.g., a machine learning model) to a large batch of source_id with reasonable memory usage. 
 You can use ``MyGaiaDB`` to do that in batch provided you have compiled a single h5 with ``mygaiadb.compile.compile_xp_continuous_allinone_h5()``
 
 ..  code-block:: python
 
     from mygaiadb.spec import yield_xp_coeffs
 
     for i in yield_xp_coeffs(a_very_long_source_id_array):
         coeffs, idx = i
         # XP coeffs of idx from the original a_very_long_source_id_array
 
-For example you want to infer ``M_H`` with your machine learning model
+    # alternatively if you also want coeffs error
+    for i in yield_xp_coeffs(a_very_long_source_id_array, return_errors=True):
+        coeffs, idx, coeffs_err = i  # unpack
+
+    # alternatively if you want coeffs error and some other columns like bp_n_relevant_basesand rp_n_relevant_bases
+    # ref: https://gea.esac.esa.int/archive/documentation/GDR3//Gaia_archive/chap_datamodel/sec_dm_spectroscopic_tables/ssec_dm_xp_summary.html
+    for i in yield_xp_coeffs(a_very_long_source_id_array, return_errors=True, return_additional_columns=["bp_n_relevant_bases", "rp_n_relevant_bases"]):
+        coeffs, idx, coeffs_err, bp_n_relevant_bases, rp_n_relevant_bases = i  # unpack
+
+For example you want to infer ``M_H`` with your machine learning model on many XP spectra
 
 ..  code-block:: python
 
     from mygaiadb.spec import yield_xp_coeffs
 
-    m_h = np.ones(len(a_very_long_source_id_array)) * -9999.
+    m_h = np.ones(len(a_very_long_source_id_array)) * np.nan
     for i in yield_xp_coeffs(a_very_long_source_id_array):
-        coeffs, idx = i
+        coeffs, idx = i  # unpack
         m_h[idx] = your_ml_model(coeffs)
 
 Author
 -------------
 -  | **Henry Leung** - henrysky_
    | University of Toronto
    | Contact Henry: henrysky.leung [at] utoronto.ca
```

### Comparing `MyGaiaDB-0.2/README.rst` & `MyGaiaDB-0.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 MyGaiaDB
 ===============
 
 *Why share when you can have the whole Gaia database on your own locally?*
 
 ``MyGaiaDB`` is simple python package with a set of scripts to help you setup a local 
-Gaia **DR3** database (also local 2MASS and ALLWISE databases too) without the need of administrator privilege 
+Gaia **DR3** database (local 2MASS, ALLWISE and CATWISE databases too) without the need of administrator privilege 
 and is compatible to all major platforms (Linux, Mac and Windows) because ``MyGaiaDB`` is **serverless** 
-and requires Python only using ``sqlite`` as long as you have enough disk space.
+which requires Python only using ``sqlite`` as long as you have enough disk space.
 
 This code is mainly to help myself managing data for my research project with Gaia DR3 XP spectra 
 and not meant to fit research usage from every aspect of Gaia's 1 billion stars. The main motivation of this 
-code is to make setting up local Gaia database with 2MASS and ALLWISE accessible to everyone. Possible use cases include 
-but not limited to make very long complex query cross-matching to multiple databases that can take a long time 
+code is to make setting up local Gaia database with 2MASS, ALLWISE and CATWISE accessible to everyone. Possible use cases include 
+but not limited to making very long complex query cross-matching to multiple databases that can take a long time 
 to finish (where the online ESA `Gaia archive`_ has timeout limitation).
 
 You are welcome to modify the code, make pull request to make this code to suit your and others need.
 
-**Part of this code will never be continuously tested properly since no way I can run this code with a few TB of gaia data on Github Actions**
+..
+
+    Part of this code will never be continuously tested properly since no way I can run this code with a few TBs of gaia data on Github Actions
 
 .. contents:: **Table of Contents**
     :depth: 3
 
 Installation and Dependencies
 -------------------------------
 
 This code requires ``python >= 3.8`` with ``numpy``, ``pandas``, ``h5py``, ``astropy`` and ``tqdm`` while only need to use 
 ``sqlite3`` bundled with your python installation without additional installation.
 Some optional functionalities require ``galpy``, ``mwdust``. Downloading functions require ``wget``.
 
 You can simply do ``pip install mygaiadb`` to install compiled ``MyGaiaDB`` wheels.
 
 Otherwise, you need to compile the code locally from source code. You need to add the folder which contains ``sqlite3ext.h`` to **INCLUDE** environment variable.
-If you are using Conda, you can do ``set INCLUDE=%CONDA_PREFIX%\Library\include;%INCLUDE%`` for Windows CMD or ``$env:INCLUDE="$env:CONDA_PREFIX\Library\include"`` for Windows PowerShell 
+If you are using Conda, you can do ``set INCLUDE=%CONDA_PREFIX%\Library\include;%INCLUDE%`` for Windows Command Prompt or ``$env:INCLUDE="$env:CONDA_PREFIX\Library\include"`` for Windows PowerShell 
 or ``export CFLAGS=-I$CONDA_PREFIX/include`` for MacOS or nothing for Linux. Then you can run ``python -m pip install .`` to install the 
 latest commits from github or ``python -m pip install -e .``  to develop ``MyGaiaDB`` locally.
 
 Folder Structure
 -------------------
 
 You need to make sure you have at least ~8TB of free disk space with fast **random read** speed for optimal query performance. 
 First set an environment variable called **MY_ASTRO_DATA** which point to a folder that (will) contains your 
 astronomical data in general. To be compatible with other python package, under **MY_ASTRO_DATA** there should be a folder called ``gaia_mirror`` that contains all 
 gaia data (i.e. **GAIA_TOOLS_DATA** environment variable from Jo Bovy's gaia_tools_).
 
 .. _apogee: https://github.com/jobovy/apogee
 .. _gaia_tools: https://github.com/jobovy/gaia_tools
 
-If you start from scratch, you only need to set **MY_ASTRO_DATA** environment variable and ``MyGaiaDB`` will populate the files and folders. 
+If you start from scratch on a clean computer, you only need to set **MY_ASTRO_DATA** environment variable and ``MyGaiaDB`` will populate the files and folders. 
 ``MyGaiaDB`` will use ``~/.mygaiadb`` folder to save user specific settings and tables.
 
 If you already have the data on your computer but in a different directory structure and you do not want or can not move them, 
 you can use symbolic link to create the required folder structure without 
 duplicating files. For Linux and MacOS, you can use ``ln -s {source-dir-or-file-path} {symbolic-dir-or-file-path}``. 
 For Windows, you can use ``mklink {symbolic-file-path} {source-file-path}`` or ``mklink /D {symbolic-dir-path} {source-dir-path}``. 
 The **case sensitive** folder structure should look something like the following chart:
@@ -101,19 +103,27 @@
     │   │   │   │   │   ├── XpSampledMeanSpectrum_000000-003111.csv.gz
     │   │   │   │   │   ├── ******
     │   │   │   │   │   └── XpSampledMeanSpectrum_786097-786431.csv.gz
     ├── 2mass_mirror/
     │   ├── psc_aaa.gz
     │   ├── ******
     │   └── xsc_baa.gz
-    └── allwise_mirror/
-        ├── wise-allwise-cat-part01.bz2
-        ├── ******
-        └── wise-allwise-cat-part48.bz2
-
+    ├── allwise_mirror/
+    │   ├── wise-allwise-cat-part01.bz2
+    │   ├── ******
+    │   └── wise-allwise-cat-part48.bz2
+    └── catwise_mirror/
+        └── 2020/
+            ├── 000/
+            │   ├── 0000m016_opt1_20191208_213403_ab_v5_cat_b0.tbl.gz
+            │   └── ******
+            ├── 001/
+            │   ├── 0015m016_opt1_20191209_054819_ab_v5_cat_b0.tbl.gz
+            │   └── ******
+            └── ******
 
 Downloading Data
 ---------------------------
 
 To download with ``MyGaiaDB``, you can do
 
 ..  code-block:: python
@@ -128,58 +138,63 @@
     download.download_2mass_best_neightbour()
     # for allwise best neightbour
     download.download_allwise_best_neightbour()
     # for 2MASS
     download.download_2mass()
     # for allwise
     download.download_allwise()
+    # for catwise
+    download.download_catwise()
     # for xp continuous
     download.download_gaia_xp_continuous()
     # for xp sampled
     download.download_gaia_xp_sampled()    
     # for rvs spectra
     download.download_gaia_rvs()
 
 
 Official data links:
 
 * Official Gaia data can be accessed here: https://cdn.gea.esac.esa.int/Gaia/
 * Official 2MASS data can be accessed here: https://irsa.ipac.caltech.edu/2MASS/download/allsky/
 * Official ALLWISE data can be accessed here: https://irsa.ipac.caltech.edu/data/download/wise-allwise/
+* Official CATWISE data can be accessed here: https://catwise.github.io/
 
 Compiling Databases
 ---------------------
 Here are functions to compile databases (each function only need to be ran once on each computer you store the data). 
 **Each function will generate large sized file(s)**. Moreover, if you are using a shared computing server, 
 only one user need to run the functions and share **MY_ASTRO_DATA** folder path to other user so
 they can setup their own environment variable **MY_ASTRO_DATA** to that folder too. Multiple users can use the SQL 
-database at the same time since ``MyGaiaDB`` will set read-only permission mission before loading databases.
+database at the same time since ``MyGaiaDB`` will set read-only permission before loading databases to prevent accidential modification.
 
 ..  code-block:: python
 
     from mygaiadb import compile
 
     # compile Gaia SQL dataset
     compile.compile_gaia_sql_db()
     # compile 2MASS SQL dataset
     compile.compile_tmass_sql_db()
     # compile ALLWISE SQL dataset
     compile.compile_allwise_sql_db()
+    # compile CATWISE SQL dataset
+    compile.compile_catwise_sql_db()
 
     # turn compressed XP coeffs files to h5, with options to save correlation matrix too
     compile.compile_xp_continuous_h5(save_correlation_matrix=False)
     # compile all XP coeffs into a single h5, partitioned batches of stars by their HEALPix
     compile.compile_xp_continuous_allinone_h5()
 
 SQL Databases Data Model
 ---------------------------
 
 Currently for Gaia DR3 in ``MyGaiaDB``, these databases are only available if you have compiled all of them: 
 ``gaiadr3.gaia_source``, ``gaiadr3.allwise_best_neighbour``, ``gaiadr3.tmasspscxsc_best_neighbour``, 
-``gaiadr3.astrophysical_parameters``, ``tmass.twomass_psc``, ``allwise.allwise``. But there are a few 
+``gaiadr3.astrophysical_parameters``, ``tmass.twomass_psc``, ``allwise.allwise``, ``catwise.catwise``. But there are a few 
 utility functions to see list of tables and table's columns. Brief description of the tables are as following:
 
 -   | ``gaiadr3.gaia_source``
     | This table mimics ``gaia_source_lite`` on `Gaia Archive`_ with addition of ``grvs_mag`` columns
     | Official description: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_main_source_catalogue/ssec_dm_gaia_source.html
 -   | ``gaiadr3.allwise_best_neighbour``
     | This table is identical to ``allwise_best_neighbour`` on `Gaia Archive`_
@@ -192,14 +207,17 @@
     | Official description: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_astrophysical_parameter_tables/ssec_dm_astrophysical_parameters.html
 -   | ``tmass.twomass_psc``
     | This table is a lite version of 2MASS Point Source Catalog (PSC) with only essential useful columns are kept
     | Official description: https://irsa.ipac.caltech.edu/2MASS/download/allsky/format_psc.html
 -   | ``allwise.allwise``
     | This table is a lite version of ALLWISE source catalog with only essential useful columns are kept
     | Official description: https://wise2.ipac.caltech.edu/docs/release/allwise/expsup/sec2_1a.html
+-   | ``catwise.catwise``
+    | This table is a lite version of CATWISE source catalog with only essential useful columns are kept
+    | Official description: https://irsa.ipac.caltech.edu/data/WISE/CatWISE/gator_docs/catwise_colDescriptions.html
 
 You can use ``list_all_tables()`` to get a list of tables excluding ``user_table``. do 
 
 ..  code-block:: python
 
     from mygaiadb.query import LocalGaiaSQL
 
@@ -253,14 +271,29 @@
         SELECT DISTANCE(179., 10., G.ra, G.dec) as ang_sep
         FROM gaiadr3.gaia_source as G
         WHERE G.source_id = 4472832130942575872
     """)
 
 and you will get the same result of 89.618118.
 
+For example the following query which utilize conventional maths function to approximate uncertainty in Gaia G magnitude
+
+..  code-block:: python
+
+    from mygaiadb.query import LocalGaiaSQL
+
+    # initialize a local Gaia SQL database instance
+    local_db = LocalGaiaSQL()
+    # CDS equation for conversion: http://vizier.cds.unistra.fr/viz-bin/VizieR-n?-source=METAnot&catid=1350&notid=63&-out=text
+    local_db.query("""
+        SELECT sqrt(power(((2.5 / log(10)) * (1 / G.phot_g_mean_flux_over_error)), 2) + power(0.0027553202, 2)) as phot_g_mean_mag_error
+        FROM gaiadr3.gaia_source as G
+        WHERE G.source_id = 3158175803069175680
+    """)
+
 Another example is the following query that works on `Gaia Archive`_ will also work in ``MyGaiaDB`` to select the first 100 gaia sources with XP coefficients
 
 ..  code-block:: sql
 
     SELECT TOP 100 * 
     FROM gaiadr3.gaia_source as G 
     WHERE (G.has_xp_continuous = 'True')
@@ -296,17 +329,27 @@
     INNER JOIN gaiadr3.allwise_best_neighbour as W on W.source_id = T.source_id
     INNER JOIN tmass.twomass_psc as TM on TM.designation = T.original_ext_source_id
     INNER JOIN allwise.allwise as AW on AW.designation = W.original_ext_source_id
     WHERE (G.has_xp_continuous = 1) AND (G.ruwe < 1.4) AND (G.ipd_frac_multi_peak <= 2) AND (G.ipd_gof_harmonic_amplitude<0.1) AND (GA.logg_gspspec < 3.0)
     """
 
     # take ~12 hours to complete
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True)
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, comments=True)
 
-As you can see for ``has_xp_continuous``, we can also use ``1`` to represent ``true`` which is used by Gaia archive but both are fine with ``MyGaiaDB``.
+As you can see for ``has_xp_continuous``, we can also use ``1`` to represent ``true`` which is used by Gaia archive but both are fine with ``MyGaiaDB``. 
+The ``overwrite=True`` means the function will save the file even if the file with the same name already exists. The ``comments=True`` means the function will 
+save the query as a comment in the csv file so you know how to reproduce the query result. To read the comments from the csv file, you can use the following code
+
+..  code-block:: python
+
+    from itertools import takewhile
+    with open("output.csv", "r") as fobj:
+        headiter = takewhile(lambda s: s.startswith("#"), fobj)
+        header = list(headiter)
+    print(" ".join(header).replace(" # ", "").replace("# ", ""))
 
 ``MyGaiaDB`` also has callbacks functionality called ``QueryCallback``, these callbacks can be used when you do query. For example, 
 you can create a callbacks to convert ``ra`` in degree to `ra_rad` in radian. So your csv file in the end will have a new column 
 called ``ra_rad``. Functions in ``QueryCallback`` must have arguments with **exact** column names in your query so ``MyGaiaDB`` knows 
 which columns to use on the fly.
 
 ..  code-block:: python
@@ -320,15 +363,15 @@
     query = """
     SELECT G.source_id, G.ra, G.dec
     FROM gaiadr3.gaia_source as G
     LIMIT 100000
     """
     ra_conversion = QueryCallback(new_col_name="ra_rad", func=lambda ra: ra / 180 * np.pi)
 
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True, callbacks=[ra_conversion])
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, callbacks=[ra_conversion], comments=True)
 
 We also have a few useful callbacks included by default to add columns like zero-point corrected parallax or extinction
 
 ..  code-block:: python
 
     from mygaiadb.query import ZeroPointCallback, DustCallback
 
@@ -339,26 +382,26 @@
     """
 
     # adding zero-point corrected parallax using official Gaia DR3 parallax zero-point python package
     zp_callback = ZeroPointCallback(new_col_name="parallax_w_zp")
     # adding SFD E(B-V) in H band filter using mwdust python package
     dust_callback = DustCallback(new_col_name="sfd_ebv", filter="H", dustmap="SFD")
 
-    local_db.save_csv(query, "output.csv", chunchsize=50000, overwrite=True, callbacks=[zp_callback, dust_callback])
+    local_db.save_csv(query, "output.csv", chunksize=50000, overwrite=True, callbacks=[zp_callback, dust_callback])
 
 User tables
 -------------
 
 ``MyGaiaDB`` support the use of user uploaded table. You can load your table first by ``pandas`` and then do
 
 ..  code-block:: python
 
     from mygaiadb.query import LocalGaiaSQL 
-    localdb = LocalGaiaSQL()  
-    localdb.upload_user_table(pd.DataFrame({"source_id": [5188146770731873152, 4611686018427432192, 5764607527332179584]}), tablename="my_table_1")
+    local_db = LocalGaiaSQL()  
+    local_db.upload_user_table(pd.DataFrame({"source_id": [5188146770731873152, 4611686018427432192, 5764607527332179584]}), tablename="my_table_1")
 
 and then carry-on doing query with ``my_table_1`` cross-matching with other tables like 
 
 ..  code-block:: python
 
     local_db.query("""SELECT * FROM gaiadr3.gaia_source as G  INNER JOIN user_table.my_table_1 as MY on MY.source_id = G.source_id""")
 
@@ -368,39 +411,48 @@
 
     local_db.list_user_tables()
 
 and you can remove a user table like ``my_table_1`` in this case by using ``remove_user_table()``
 
 ..  code-block:: python
 
-    a.remove_user_table("my_table_1")
+    local_db.remove_user_table("my_table_1")
 
-Spectroscopy Query
---------------------
+Gaia XP Spectroscopy Query
+----------------------------
 
 There can be use case where you want to run a function (e.g., a machine learning model) to a large batch of source_id with reasonable memory usage. 
 You can use ``MyGaiaDB`` to do that in batch provided you have compiled a single h5 with ``mygaiadb.compile.compile_xp_continuous_allinone_h5()``
 
 ..  code-block:: python
 
     from mygaiadb.spec import yield_xp_coeffs
 
     for i in yield_xp_coeffs(a_very_long_source_id_array):
         coeffs, idx = i
         # XP coeffs of idx from the original a_very_long_source_id_array
 
-For example you want to infer ``M_H`` with your machine learning model
+    # alternatively if you also want coeffs error
+    for i in yield_xp_coeffs(a_very_long_source_id_array, return_errors=True):
+        coeffs, idx, coeffs_err = i  # unpack
+
+    # alternatively if you want coeffs error and some other columns like bp_n_relevant_basesand rp_n_relevant_bases
+    # ref: https://gea.esac.esa.int/archive/documentation/GDR3//Gaia_archive/chap_datamodel/sec_dm_spectroscopic_tables/ssec_dm_xp_summary.html
+    for i in yield_xp_coeffs(a_very_long_source_id_array, return_errors=True, return_additional_columns=["bp_n_relevant_bases", "rp_n_relevant_bases"]):
+        coeffs, idx, coeffs_err, bp_n_relevant_bases, rp_n_relevant_bases = i  # unpack
+
+For example you want to infer ``M_H`` with your machine learning model on many XP spectra
 
 ..  code-block:: python
 
     from mygaiadb.spec import yield_xp_coeffs
 
-    m_h = np.ones(len(a_very_long_source_id_array)) * -9999.
+    m_h = np.ones(len(a_very_long_source_id_array)) * np.nan
     for i in yield_xp_coeffs(a_very_long_source_id_array):
-        coeffs, idx = i
+        coeffs, idx = i  # unpack
         m_h[idx] = your_ml_model(coeffs)
 
 Author
 -------------
 -  | **Henry Leung** - henrysky_
    | University of Toronto
    | Contact Henry: henrysky.leung [at] utoronto.ca
```

### Comparing `MyGaiaDB-0.2/mygaiadb/__init__.py` & `MyGaiaDB-0.3/mygaiadb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 mygaiadb_usertable_db.touch()
 
 gaia_sql_db_path = astro_data_path.joinpath("gaia_mirror", "gaiadr3.db")
 gaia_astro_param_sql_db_path = astro_data_path.joinpath("gaia_mirror", "gaiadr3_astrophysical_params.db")
 gaia_xp_coeff_h5_path = astro_data_path.joinpath("gaia_mirror" ,"xp_continuous_mean_spectrum_allinone.h5")
 tmass_sql_db_path = astro_data_path.joinpath("2mass_mirror", "tmass.db")
 allwise_sql_db_path = astro_data_path.joinpath("allwise_mirror", "allwise.db")
+catwise_sql_db_path = astro_data_path.joinpath("catwise_mirror", "catwise.db")
```

### Comparing `MyGaiaDB-0.2/mygaiadb/data/__init__.py` & `MyGaiaDB-0.3/mygaiadb/data/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT = _GAIA_DR3_PARENT.joinpath("cross_match", "allwise_best_neighbour")
 _GAIA_DR3_2MASS_NEIGHBOUR_PARENT = _GAIA_DR3_PARENT.joinpath("cross_match", "tmasspscxsc_best_neighbour")
 _GAIA_DR3_XP_CONTINUOUS_PARENT = _GAIA_DR3_PARENT.joinpath("Spectroscopy", "xp_continuous_mean_spectrum")
 _GAIA_DR3_XP_SAMPLED_PARENT = _GAIA_DR3_PARENT.joinpath("Spectroscopy", "xp_sampled_mean_spectrum")
 _GAIA_DR3_RVS_PARENT = _GAIA_DR3_PARENT.joinpath("Spectroscopy", "rvs_mean_spectrum")
 _2MASS_PARENT = astro_data_path.joinpath("2mass_mirror")
 _ALLWISE_PARENT = astro_data_path.joinpath("allwise_mirror")
+_CATWISE_PARENT = astro_data_path.joinpath("catwise_mirror", "2020")
 
 
 def downloader(url, fullfilename, name, test=False, session=None):
     """
     url: URL of data file
     fullfilename: full local path
     name: name of the task
```

### Comparing `MyGaiaDB-0.2/mygaiadb/data/compile.py` & `MyGaiaDB-0.3/mygaiadb/data/compile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import sqlite3
 from pathlib import Path
 import os
 import glob
 import tqdm
 import h5py
+import warnings
 import numpy as np
 import pandas as pd
 from . import (
     _GAIA_DR3_GAIASOURCE_PARENT,
     _GAIA_DR3_ASTROPHYS_PARENT,
     _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT,
     _GAIA_DR3_2MASS_NEIGHBOUR_PARENT,
     _2MASS_PARENT,
-    _ALLWISE_PARENT
+    _ALLWISE_PARENT,
+    _CATWISE_PARENT,
 )
-from .. import astro_data_path, gaia_sql_db_path, tmass_sql_db_path, allwise_sql_db_path, gaia_xp_coeff_h5_path
+from .. import astro_data_path, gaia_sql_db_path, tmass_sql_db_path, allwise_sql_db_path, gaia_xp_coeff_h5_path, catwise_sql_db_path
 
 
 def compile_xp_continuous_allinone_h5():
     base_path = astro_data_path.joinpath(
         "gaia_mirror",
         "Gaia",
         "gdr3",
@@ -291,17 +293,17 @@
 
     # we have added "grvs_mag" to the table on top of gaia_source_lite on Gaia Archive
     # will take ~11 hours to run
     if do_gaia_source_table:
         # =================== setup Gaia schema and first two tables ===================
         # this section will take ~30 minutes to run
         for schema in [
-            "gaia_source_lite_schema",
-            "allwise_best_neighbour_schema",
-            "tmasspscxsc_best_neighbour_schema",
+            "gaia_source_lite_schema.sql",
+            "allwise_best_neighbour_schema.sql",
+            "tmasspscxsc_best_neighbour_schema.sql",
         ]:
             schema_filename = os.path.join(
                 os.path.dirname(__file__), "sql_schema", f"{schema}"
             )
             with open(schema_filename) as f:
                 lines = f.read().replace("\n", "")
             c.execute(lines)
@@ -380,15 +382,15 @@
             data = pd.read_csv(
                 p, header=1, sep=",", skiprows=999, usecols=dtypes.keys(), dtype=dtypes
             )
             # write the data to a sqlite table
             data.to_sql("gaia_source", conn, if_exists="append", index=False)
 
     if do_gaia_astrophysical_table:
-        schema_filename = os.path.join(os.path.dirname(__file__), "sql_schema", "astrophysical_parameters_lite_schema")
+        schema_filename = os.path.join(os.path.dirname(__file__), "sql_schema", "astrophysical_parameters_lite_schema.sql")
 
         with open(schema_filename) as f:
             lines = f.read().replace("\n", "")
         c.execute(lines)
         # =================== populate gaia_source lite table ===================
         # we have added "grvs_mag" to the table on top of gaia_source_lite on Gaia Archive
         # will take ~11 hours to run
@@ -487,15 +489,15 @@
     """
     Path(tmass_sql_db_path).touch()
     conn = sqlite3.connect(tmass_sql_db_path)
     c = conn.cursor()
 
     # =================== 2MASS ===================
     # this section will take 1 hour to run
-    schema_filename = os.path.join(os.path.dirname(__file__), "sql_schema", "twomass_psc_lite_schema")
+    schema_filename = os.path.join(os.path.dirname(__file__), "sql_schema", "twomass_psc_lite_schema.sql")
 
     with open(schema_filename) as f:
         lines = f.read().replace("\n", "")
     c.execute(lines)
 
     # only the first part, not all actually
     # https://irsa.ipac.caltech.edu/data/2MASS/docs/releases/allsky/doc/sec2_2a.html
@@ -624,15 +626,15 @@
     This function compile allwise SQL database
     """
     Path(allwise_sql_db_path).touch()
     conn = sqlite3.connect(allwise_sql_db_path)
     c = conn.cursor()
 
     # this section will take ~16 hours to run
-    schema_filename = os.path.join(os.path.dirname(__file__), "sql_schema", "allwise_lite_schema")
+    schema_filename = os.path.join(os.path.dirname(__file__), "sql_schema", "allwise_lite_schema.sql")
 
     with open(schema_filename) as f:
         lines = f.read().replace("\n", "")
     c.execute(lines)
 
     # only the first part, not all actually
     # https://wise2.ipac.caltech.edu/docs/release/allwise/expsup/sec2_1a.html
@@ -984,20 +986,298 @@
         }
         data = pd.read_csv(
             p,
             header=None,
             sep="|",
             usecols=[allwise_allcol.index(i) for i in dtypes.keys()],
             names=dtypes.keys(),
+            dtype=dtypes
         )
-        data.astype(dtypes)
         
         # write the data to a sqlite table
         data.to_sql(f"allwise", conn, if_exists="append", index=False)
 
     # =================== indexing ===================
     if indexing:
         # 22m56s
         print("Doing Indexing")
         c.execute(
             """CREATE INDEX allwise_designation_mags ON allwise (designation, w1mpro, w2mpro, w3mpro, w4mpro, w1snr, w2snr, w3snr, w4snr, ph_qual);"""
         )
+
+
+def compile_catwise_sql_db(indexing=True):
+    """
+    This function compile allwise SQL database
+    """
+    Path(catwise_sql_db_path).touch()
+    conn = sqlite3.connect(catwise_sql_db_path)
+    c = conn.cursor()
+
+    # this section will take ~16 hours to run
+    schema_filename = os.path.join(os.path.dirname(__file__), "sql_schema", "catwise_lite_schema.sql")
+
+    with open(schema_filename) as f:
+        lines = f.read().replace("\n", "")
+    c.execute(lines)
+
+    # only the first part, not all actually
+    # https://portal.nersc.gov/project/cosmo/data/CatWISE/2020cwcat.sis20200318.txt
+    catwise_allcol = [
+        # Note that the first column in the width is occupied by a "pipe" or "bar" delimiter ("|")
+        "source_name",
+        "source_id",
+        "ra",
+        "dec",
+        "sigra",
+        "sigdec",
+        "sigradec",
+        # the following positions reflect the source xy position in the unWISE full depth coadd
+        "wx",
+        "wy",
+        # The next set of columns are aperture/annulus measurements from the unWISE epoch coadds
+        "w1sky",
+        "w1sigsk",
+        "w1conf",
+        "w2sky",
+        "w2sigsk",
+        "w2conf",
+        # WPRO epoch coadd measurements
+        "w1fitr",
+        "w2fitr",
+        "w1snr",
+        "w2snr",
+        "w1flux",
+        "w1sigflux",
+        "w2flux",
+        "w2sigflux",
+        "w1mpro",
+        "w1sigmpro",
+        "w1rchi2",
+        "w2mpro",
+        "w2sigmpro",
+        "w2rchi2",
+        "rchi2",
+        "nb",
+        "na",
+        "w1Sat",
+        "w2Sat",
+        # full depth coadd measurements: WAPPco, standard aperture w/ aperture correction;
+        # the standard (aperture corrected) aperture radius is 8.25 arcsec.
+        "w1mag",
+        "w1sigm",
+        "w1flg",
+        "w1Cov",
+        "w2mag",
+        "w2sigm",
+        "w2flg",
+        "w2Cov",
+        # full depth coadd measurements: WAPPco, circular apertures, no aperture correction is applied;
+        # radii:    5.50   8.25  11.00  13.75  16.50  19.25  22.00  24.75 arcsec
+        "w1mag_1",
+        "w1sigm_1",
+        "w1flg_1",
+        "w2mag_1",
+        "w2sigm_1",
+        "w2flg_1",
+        "w1mag_2",
+        "w1sigm_2",
+        "w1flg_2",
+        "w2mag_2",
+        "w2sigm_2",
+        "w2flg_2",
+        "w1mag_3",
+        "w1sigm_3",
+        "w1flg_3",
+        "w2mag_3",
+        "w2sigm_3",
+        "w2flg_3",
+        "w1mag_4",
+        "w1sigm_4",
+        "w1flg_4",
+        "w2mag_4",
+        "w2sigm_4",
+        "w2flg_4",
+        "w1mag_5",
+        "w1sigm_5",
+        "w1flg_5",
+        "w2mag_5",
+        "w2sigm_5",
+        "w2flg_5",
+        "w1mag_6",
+        "w1sigm_6",
+        "w1flg_6",
+        "w2mag_6",
+        "w2sigm_6",
+        "w2flg_6",
+        "w1mag_7",
+        "w1sigm_7",
+        "w1flg_7",
+        "w2mag_7",
+        "w2sigm_7",
+        "w2flg_7",
+        "w1mag_8",
+        "w1sigm_8",
+        "w1flg_8",
+        "w2mag_8",
+        "w2sigm_8",
+        "w2flg_8",
+        # the following are "N of M" counters for WPRO measurements
+        # w?M   - The number of individual epochs for band ? that are
+        #         available to make a profile-fit measurement.
+        # w?NM  - The number of individual epochs for band ? on which
+        #         WPRO extracted a flux measurement that has snr>3.
+        # w?mLQ - variability indicator mLogQ for the flux array
+        "w1NM",
+        "w1M",
+        "w1magP",
+        "w1sigP1",
+        "w1sigP2",
+        "w1k",
+        "w1Ndf",
+        "w1mLQ",
+        "w1mJDmin",
+        "w1mJDmax",
+        "w1mJDmean",
+        "w2NM",
+        "w2M",
+        "w2magP",
+        "w2sigP1",
+        "w2sigP2",
+        "w2k",
+        "w2Ndf",
+        "w2mLQ",
+        "w2mJDmin",
+        "w2mJDmax",
+        "w2mJDmean",
+        "rho12",
+        "q12",
+        "nIters",
+        "nSteps",
+        "mdetID",
+        "p1",
+        "p2",
+        "MeanObsMJD",
+        "ra_pm",
+        "dec_pm",
+        "sigra_pm",
+        "sigdec_pm",
+        "sigradec_pm",
+        "PMRA",
+        "PMDec",
+        "sigPMRA",
+        "sigPMDec",
+        "w1snr_pm",
+        "w2snr_pm",
+        "w1flux_pm",
+        "w1sigflux_pm",
+        "w2flux_pm",
+        "w2sigflux_pm",
+        "w1mpro_pm",
+        "w1sigmpro_pm",
+        "w1rchi2_pm",
+        "w2mpro_pm",
+        "w2sigmpro_pm",
+        "w2rchi2_pm",
+        "rchi2_pm",
+        "pmcode",
+        "nIters_pm",
+        "nSteps_pm",
+        "dist",
+        "dw1mag",
+        "rch2w1",
+        "dw2mag",
+        "rch2w2",
+        "elon_avg",
+        "elonSig",
+        "elat_avg",
+        "elatSig",
+        "Delon",
+        "DelonSig",
+        "Delat",
+        "DelatSig",
+        "DelonSNR",
+        "DelatSNR",
+        "chi2pmra",
+        "chi2pmdec",
+        "ka",
+        "k1",
+        "k2",
+        "km",
+        "par_pm",
+        "par_pmSig",
+        "par_stat",
+        "par_sigma",
+        "dist_x",
+        "cc_flags",
+        "w1cc_map",
+        "w1cc_map_str",
+        "w2cc_map",
+        "w2cc_map_str",
+        "n_aw",
+        "ab_flags",
+        "w1ab_map",
+        "w1ab_map_str",
+        "w2ab_map",
+        "w2ab_map_str",
+        "glon",
+        "glat",
+        "elon",
+        "elat",
+        "unwise_objid",
+    ]
+
+    for p in tqdm.tqdm(list(_CATWISE_PARENT.glob("*/*cat_b0.tbl.gz"))):
+        dtypes = {
+            "source_name": str,  # source_name does not seems to be unique, dont use it as primary key
+            "source_id": str,
+            "ra": np.float64,
+            "dec": np.float64,
+            "sigra": np.float32,
+            "sigdec": np.float32,
+            "sigradec": np.float32,
+            "w1snr": np.float32,  # 18
+            "w2snr": np.float32,  # 19
+            "w1mpro": np.float32,  # 24
+            "w1sigmpro": np.float32,  # 25
+            "w2mpro": np.float32,  # 27
+            "w2sigmpro": np.float32,  # 28
+            "nb": "Int32",  # 31
+            "na": "Int32",  # 32
+            "w1mag": np.float32,  # 35
+            "w1flg": "Int32",  # 37
+            "w2mag": np.float32,  # 39
+            "w2flg": "Int32",  # 41
+            "w1k": np.float32,  # 96
+            "w1mJDmean": np.float64,  # 101
+            "w2k": np.float32,  # 107
+            "w2mJDmean": np.float64,  # 112
+            # "cc_flags": str,
+            "w1ab_map": "Int32",
+            "w2ab_map": "Int32",
+            "unwise_objid": str,
+        }
+        try:
+            data = pd.read_table(
+                p,
+                delim_whitespace=True,
+                skiprows=19,
+                usecols=[catwise_allcol.index(i) for i in dtypes.keys()],
+                names=dtypes.keys(),
+                dtype=dtypes,
+            )
+        except ValueError:  # sometimes there are 20 rows of comments
+            data = pd.read_table(
+                p,
+                delim_whitespace=True,
+                skiprows=20,
+                usecols=[catwise_allcol.index(i) for i in dtypes.keys()],
+                names=dtypes.keys(),
+                dtype=dtypes,
+            )
+        
+        # write the data to a sqlite table
+        data.to_sql(f"catwise", conn, if_exists="append", index=False)
+
+    # =================== indexing ===================
+    if indexing:
+        warnings.warn("Indexing for CATWISE is not implemented yet")
```

### Comparing `MyGaiaDB-0.2/mygaiadb/data/download.py` & `MyGaiaDB-0.3/mygaiadb/data/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,53 +6,92 @@
     _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT,
     _GAIA_DR3_2MASS_NEIGHBOUR_PARENT,
     _GAIA_DR3_XP_CONTINUOUS_PARENT,
     _GAIA_DR3_XP_SAMPLED_PARENT,
     _GAIA_DR3_RVS_PARENT,
     _ALLWISE_PARENT,
     _2MASS_PARENT,
+    _CATWISE_PARENT,
 )
 
 
 def download_gaia_source(test=False):
     _GAIA_DR3_GAIASOURCE_PARENT.mkdir(parents=True, exist_ok=True)
     _url = "http://cdn.gea.esac.esa.int/Gaia/gdr3/gaia_source/"
     if test:
-        downloader(f"{_url}GaiaSource_000000-003111.csv.gz", _GAIA_DR3_GAIASOURCE_PARENT.joinpath("GaiaSource_000000-003111.csv.gz"), "test", test=test)
-        downloader(f"{_url}GaiaSource_003112-005263.csv.gz", _GAIA_DR3_GAIASOURCE_PARENT.joinpath("GaiaSource_003112-005263.csv.gz"), "test", test=test)
+        downloader(
+            f"{_url}GaiaSource_000000-003111.csv.gz",
+            _GAIA_DR3_GAIASOURCE_PARENT.joinpath("GaiaSource_000000-003111.csv.gz"),
+            "test",
+            test=test,
+        )
+        downloader(
+            f"{_url}GaiaSource_003112-005263.csv.gz",
+            _GAIA_DR3_GAIASOURCE_PARENT.joinpath("GaiaSource_003112-005263.csv.gz"),
+            "test",
+            test=test,
+        )
         # cmd_str = f"cd {_GAIA_DR3_GAIASOURCE_PARENT.as_posix()} && curl --no-clobber -s -O {_url}GaiaSource_000000-003111.csv.gz"
         # subprocess.run(cmd_str, shell=True)
         # cmd_str = f"cd {_GAIA_DR3_GAIASOURCE_PARENT.as_posix()} && curl --no-clobber -s -O {_url}GaiaSource_003112-005263.csv.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_GAIA_DR3_GAIASOURCE_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
 
 
 def download_gaia_astrophysical_parameters(test=False):
     _GAIA_DR3_ASTROPHYS_PARENT.mkdir(parents=True, exist_ok=True)
     _url = "http://cdn.gea.esac.esa.int/Gaia/gdr3/Astrophysical_parameters/astrophysical_parameters/"
     if test:
-        downloader(f"{_url}AstrophysicalParameters_000000-003111.csv.gz", _GAIA_DR3_ASTROPHYS_PARENT.joinpath("AstrophysicalParameters_000000-003111.csv.gz"), "test", test=test)
-        downloader(f"{_url}AstrophysicalParameters_003112-005263.csv.gz", _GAIA_DR3_ASTROPHYS_PARENT.joinpath("AstrophysicalParameters_003112-005263.csv.gz"), "test", test=test)
+        downloader(
+            f"{_url}AstrophysicalParameters_000000-003111.csv.gz",
+            _GAIA_DR3_ASTROPHYS_PARENT.joinpath(
+                "AstrophysicalParameters_000000-003111.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
+        downloader(
+            f"{_url}AstrophysicalParameters_003112-005263.csv.gz",
+            _GAIA_DR3_ASTROPHYS_PARENT.joinpath(
+                "AstrophysicalParameters_003112-005263.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
         # cmd_str = f"cd {_GAIA_DR3_ASTROPHYS_PARENT.as_posix()} && curl --no-clobber -s -O {_url}AstrophysicalParameters_000000-003111.csv.gz"
         # subprocess.run(cmd_str, shell=True)
         # cmd_str = f"cd {_GAIA_DR3_ASTROPHYS_PARENT.as_posix()} && curl --no-clobber -s -O {_url}AstrophysicalParameters_003112-005263.csv.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_GAIA_DR3_ASTROPHYS_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
 
 
 def download_allwise_best_neightbour(test=False):
     _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.mkdir(parents=True, exist_ok=True)
     _url = "http://cdn.gea.esac.esa.int/Gaia/gedr3/cross_match/allwise_best_neighbour/"
     if test:
-        downloader(f"{_url}allwiseBestNeighbour0001.csv.gz", _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.joinpath("allwiseBestNeighbour0001.csv.gz"), "test", test=test)
-        downloader(f"{_url}allwiseBestNeighbour0002.csv.gz", _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.joinpath("allwiseBestNeighbour0002.csv.gz"), "test", test=test)
+        downloader(
+            f"{_url}allwiseBestNeighbour0001.csv.gz",
+            _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.joinpath(
+                "allwiseBestNeighbour0001.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
+        downloader(
+            f"{_url}allwiseBestNeighbour0002.csv.gz",
+            _GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.joinpath(
+                "allwiseBestNeighbour0002.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
         # cmd_str = f"cd {_GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.as_posix()} && curl --no-clobber -s -O {_url}allwiseBestNeighbour0001.csv.gz"
         # subprocess.run(cmd_str, shell=True)
         # cmd_str = f"cd {_GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.as_posix()} && curl --no-clobber -s -O {_url}allwiseBestNeighbour0002.csv.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_GAIA_DR3_ALLWISE_NEIGHBOUR_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
@@ -60,32 +99,49 @@
 
 def download_2mass_best_neightbour(test=False):
     _GAIA_DR3_2MASS_NEIGHBOUR_PARENT.mkdir(parents=True, exist_ok=True)
     _url = (
         "http://cdn.gea.esac.esa.int/Gaia/gedr3/cross_match/tmasspscxsc_best_neighbour/"
     )
     if test:
-        downloader(f"{_url}tmasspscxscBestNeighbour0001.csv.gz", _GAIA_DR3_2MASS_NEIGHBOUR_PARENT.joinpath("tmasspscxscBestNeighbour0001.csv.gz"), "test", test=test)
-        downloader(f"{_url}tmasspscxscBestNeighbour0002.csv.gz", _GAIA_DR3_2MASS_NEIGHBOUR_PARENT.joinpath("tmasspscxscBestNeighbour0002.csv.gz"), "test", test=test)
+        downloader(
+            f"{_url}tmasspscxscBestNeighbour0001.csv.gz",
+            _GAIA_DR3_2MASS_NEIGHBOUR_PARENT.joinpath(
+                "tmasspscxscBestNeighbour0001.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
+        downloader(
+            f"{_url}tmasspscxscBestNeighbour0002.csv.gz",
+            _GAIA_DR3_2MASS_NEIGHBOUR_PARENT.joinpath(
+                "tmasspscxscBestNeighbour0002.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
         # cmd_str = f"cd {_GAIA_DR3_2MASS_NEIGHBOUR_PARENT.as_posix()} && curl --no-clobber -s -O {_url}tmasspscxscBestNeighbour0001.csv.gz"
         # subprocess.run(cmd_str, shell=True)
         # cmd_str = f"cd {_GAIA_DR3_2MASS_NEIGHBOUR_PARENT.as_posix()} && curl --no-clobber -s -O {_url}tmasspscxscBestNeighbour0002.csv.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_GAIA_DR3_2MASS_NEIGHBOUR_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
 
+
 def download_2mass(test=False):
     _2MASS_PARENT.mkdir(parents=True, exist_ok=True)
-    _url = (
-        "https://irsa.ipac.caltech.edu/2MASS/download/allsky/"
-    )
+    _url = "https://irsa.ipac.caltech.edu/2MASS/download/allsky/"
     if test:
-        downloader(f"{_url}psc_aaa.gz", _2MASS_PARENT.joinpath("psc_aaa.gz"), "test", test=test)
-        downloader(f"{_url}psc_aab.gz", _2MASS_PARENT.joinpath("psc_aab.gz"), "test", test=test)
+        downloader(
+            f"{_url}psc_aaa.gz", _2MASS_PARENT.joinpath("psc_aaa.gz"), "test", test=test
+        )
+        downloader(
+            f"{_url}psc_aab.gz", _2MASS_PARENT.joinpath("psc_aab.gz"), "test", test=test
+        )
         # cmd_str = f"cd {_2MASS_PARENT.as_posix()} && curl --no-clobber -s -O {_url}psc_aaa.gz"
         # subprocess.run(cmd_str, shell=True)
         # cmd_str = f"cd {_2MASS_PARENT.as_posix()} && curl --no-clobber -s -O {_url}psc_aab.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_2MASS_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
@@ -146,48 +202,93 @@
         f"wget -P {_ALLWISE_PARENT.as_posix()} --no-clobber --no-verbose --no-parent http://irsa.ipac.caltech.edu/data/download/wise-allwise/wise-allwise-cat-part45.bz2",
         f"wget -P {_ALLWISE_PARENT.as_posix()} --no-clobber --no-verbose --no-parent http://irsa.ipac.caltech.edu/data/download/wise-allwise/wise-allwise-cat-part46.bz2",
         f"wget -P {_ALLWISE_PARENT.as_posix()} --no-clobber --no-verbose --no-parent http://irsa.ipac.caltech.edu/data/download/wise-allwise/wise-allwise-cat-part47.bz2",
         f"wget -P {_ALLWISE_PARENT.as_posix()} --no-clobber --no-verbose --no-parent http://irsa.ipac.caltech.edu/data/download/wise-allwise/wise-allwise-cat-part48.bz2",
     ]
 
     if test:
-        downloader(f"http://irsa.ipac.caltech.edu/data/download/wise-allwise/wise-allwise-cat-part01.bz2", _ALLWISE_PARENT.joinpath("wise-allwise-cat-part01.bz2"), "test", test=test)
+        downloader(
+            f"http://irsa.ipac.caltech.edu/data/download/wise-allwise/wise-allwise-cat-part01.bz2",
+            _ALLWISE_PARENT.joinpath("wise-allwise-cat-part01.bz2"),
+            "test",
+            test=test,
+        )
         # subprocess.run(cmd_list[3], shell=True)
     else:
         for cmd_str in cmd_list:
             subprocess.run(cmd_str, shell=True)
 
 
 def download_gaia_xp_continuous(test=False):
     _GAIA_DR3_XP_CONTINUOUS_PARENT.mkdir(parents=True, exist_ok=True)
     _url = "http://cdn.gea.esac.esa.int/Gaia/gdr3/Spectroscopy/xp_continuous_mean_spectrum/"
     if test:
-        downloader(f"{_url}XpContinuousMeanSpectrum_000000-003111.csv.gz", _GAIA_DR3_XP_CONTINUOUS_PARENT.joinpath("XpContinuousMeanSpectrum_000000-003111.csv.gz"), "test", test=test)
+        downloader(
+            f"{_url}XpContinuousMeanSpectrum_000000-003111.csv.gz",
+            _GAIA_DR3_XP_CONTINUOUS_PARENT.joinpath(
+                "XpContinuousMeanSpectrum_000000-003111.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
         # cmd_str = f"cd {_GAIA_DR3_XP_CONTINUOUS_PARENT.as_posix()} && curl --no-clobber -s -O {_url}XpContinuousMeanSpectrum_000000-003111.csv.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_GAIA_DR3_XP_CONTINUOUS_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
 
 
 def download_gaia_xp_sampled(test=False):
     _GAIA_DR3_XP_SAMPLED_PARENT.mkdir(parents=True, exist_ok=True)
-    _url = "http://cdn.gea.esac.esa.int/Gaia/gdr3/Spectroscopy/xp_sampled_mean_spectrum/"
+    _url = (
+        "http://cdn.gea.esac.esa.int/Gaia/gdr3/Spectroscopy/xp_sampled_mean_spectrum/"
+    )
     if test:
-        downloader(f"{_url}XpSampledMeanSpectrum_000000-003111.csv.gz", _GAIA_DR3_XP_SAMPLED_PARENT.joinpath("XpSampledMeanSpectrum_000000-003111.csv.gz"), "test", test=test)
+        downloader(
+            f"{_url}XpSampledMeanSpectrum_000000-003111.csv.gz",
+            _GAIA_DR3_XP_SAMPLED_PARENT.joinpath(
+                "XpSampledMeanSpectrum_000000-003111.csv.gz"
+            ),
+            "test",
+            test=test,
+        )
         # cmd_str = f"cd {_GAIA_DR3_XP_SAMPLED_PARENT.as_posix()} && curl --no-clobber -s -O {_url}XpSampledMeanSpectrum_000000-003111.csv.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_GAIA_DR3_XP_SAMPLED_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
 
 
 def download_gaia_rvs(test=False):
     _GAIA_DR3_RVS_PARENT.mkdir(parents=True, exist_ok=True)
     _url = "http://cdn.gea.esac.esa.int/Gaia/gdr3/Spectroscopy/rvs_mean_spectrum/"
     if test:
-        downloader(f"{_url}RvsMeanSpectrum_000000-003111.csv.gz", _GAIA_DR3_RVS_PARENT.joinpath("RvsMeanSpectrum_000000-003111.csv.gz"), "test", test=test)
+        downloader(
+            f"{_url}RvsMeanSpectrum_000000-003111.csv.gz",
+            _GAIA_DR3_RVS_PARENT.joinpath("RvsMeanSpectrum_000000-003111.csv.gz"),
+            "test",
+            test=test,
+        )
         # cmd_str = f"cd {_GAIA_DR3_RVS_PARENT.as_posix()} && curl --no-clobber -s -O {_url}RvsMeanSpectrum_000000-003111.csv.gz"
         # subprocess.run(cmd_str, shell=True)
     else:
         cmd_str = f"wget -P {_GAIA_DR3_RVS_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive --level=1 --no-directories {_url}"
         subprocess.run(cmd_str, shell=True)
+
+
+def download_catwise(test=False):
+    _CATWISE_PARENT.mkdir(parents=True, exist_ok=True)
+    _url = "https://portal.nersc.gov/project/cosmo/data/CatWISE/2020/"
+    if test:
+        downloader(
+            f"{_url}000/0000m016_opt1_20191208_213403_ab_v5_cat_b0.tbl.gz",
+            _CATWISE_PARENT.joinpath(
+                "000", "0000m016_opt1_20191208_213403_ab_v5_cat_b0.tbl.gz"
+            ),
+            "test",
+            test=test,
+        )
+        # cmd_str = f"cd {_CATWISE_PARENT.as_posix()} && curl --no-clobber -s -O {_url}catwise_2020a.tbl"
+        # subprocess.run(cmd_str, shell=True)
+    else:
+        cmd_str = f"wget -P {_CATWISE_PARENT.as_posix()} --no-clobber --no-verbose --no-parent --recursive -R 'index.html*' --level=2 -e robots=off --no-host-directories --cut-dirs=5 {_url}"
+        subprocess.run(cmd_str, shell=True)
```

### Comparing `MyGaiaDB-0.2/mygaiadb/ext_c/astroqlite.c` & `MyGaiaDB-0.3/mygaiadb/ext_c/astroqlite.c`

 * *Files identical despite different names*

### Comparing `MyGaiaDB-0.2/mygaiadb/query/callbacks.py` & `MyGaiaDB-0.3/mygaiadb/query/callbacks.py`

 * *Files identical despite different names*

### Comparing `MyGaiaDB-0.2/mygaiadb/query/query.py` & `MyGaiaDB-0.3/mygaiadb/query/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from tqdm import tqdm
 from mygaiadb import (
     mygaiadb_default_db,
     mygaiadb_usertable_db,
     gaia_sql_db_path,
     tmass_sql_db_path,
     allwise_sql_db_path,
+    catwise_sql_db_path,
     __version__
 )
 
 
 class QueryCallback:
     """
     Callback to add new column to SQL query on the fly
@@ -43,14 +44,15 @@
     Class for local Gaia SQL database
     """
 
     def __init__(
         self,
         load_tmass=True,
         load_allwise=True,
+        load_catwise=True,
         load_ext=True,
         readonly_guard=True,
     ):
         """
         Parameters
         ----------
         load_tmass : bool
@@ -60,32 +62,38 @@
         load_ext : bool
             whether to load sqlite extension
         readonly_guard : bool
             whether to ensure the databases are read-only
         """
         self.load_tmass = load_tmass
         self.load_allwise = load_allwise
+        self.load_catwise = load_catwise
         self.load_ext = load_ext
         self.readonly_guard = readonly_guard
         self.attached_db_name = []
 
         # flag for windows or not
         self.win32 = sys.platform.startswith("win32")
 
         self.conn, self.cursor = self._load_db()
 
         # ipython Auto-completion
         try:
             from IPython import get_ipython
-            def name_completer(ipython, event):
+            def list_all_tables_completer(ipython, event):
                 out = self.list_all_tables()
                 out.extend(list(f"user_table.{i}" for i in self.list_user_tables().keys()))
                 return out
-            get_ipython().set_hook("complete_command", name_completer,
+            def usertable_completer(ipython, event):
+                out = self.list_user_tables()
+                return out
+            get_ipython().set_hook("complete_command", list_all_tables_completer,
                                    re_key=".*get_table_column")
+            get_ipython().set_hook("complete_command", usertable_completer,
+                                   re_key=".*remove_user_table")
         except:
             pass
 
     def _check_callbacks_header(self, headers, callbacks):
         """
         Helper function to check if all columns required by all callbacks are presented in query
 
@@ -116,15 +124,15 @@
         if self.win32:
             os.chmod(file_path, stat.S_IREAD)
         else:
             os.chmod(file_path, 0o444)
 
     def _file_exist(self, path):
         if not os.path.exists(path):
-            raise FileExistsError(f"Database at {path} does not exist")
+            raise FileNotFoundError(f"Database at {path} does not exist. You should set loading that database to False.")
 
     def preprocess_query(func):
         """
         Decoractor to preprocess query. Mostly to increase compatability with Gaia ADQL
         """
 
         def preprocess_logic(self, *args, **kwargs):
@@ -188,14 +196,20 @@
             self.attached_db_name.append("tmass")
         if self.load_allwise:
             self._file_exist(allwise_sql_db_path)
             if self.readonly_guard:
                 self._read_only(allwise_sql_db_path)  # set read-only before loading it
             c.execute(f"""ATTACH DATABASE '{allwise_sql_db_path}' AS allwise""")
             self.attached_db_name.append("allwise")
+        if self.load_catwise:
+            self._file_exist(catwise_sql_db_path)
+            if self.readonly_guard:
+                self._read_only(catwise_sql_db_path)  # set read-only before loading it
+            c.execute(f"""ATTACH DATABASE '{catwise_sql_db_path}' AS catwise""")
+            self.attached_db_name.append("catwise")
         # ======================= optional table =======================
         return conn, c
     
     @staticmethod
     def _load_sqlite3_ext(c):
         c.enable_load_extension(True)
         # Find and load the library
@@ -212,60 +226,84 @@
                     c.load_extension(_lib)
                     break
         if _lib is None:
             raise IOError("MyGaiaDB SQL C extension not found")
 
     @preprocess_query
     def save_csv(
-        self, query, filename, chunchsize=50000, overwrite=True, callbacks=None
+        self, query, filename, chunksize=50000, overwrite=True, callbacks=None, comments=True
     ):
         """
-        Given query, save the fetchall() result to csv, "chunchsize" number of rows at each time until finished
+        Given query, save the fetchall() result to csv, "chunksize" number of rows at each time until finished
 
         Parameters
         ----------
         query : string
             Query string
         filename : string
             filename (*.csv) to be saved
+        chunksize : int
+            number of rows to do in one batch
+        overwrite : bool
+            whether to overwrite csv file if it already exists
+        callbacks : list
+            list of mygaiadb callbacks
+        comments : bool
+            whether to save the query as comment lines in csv file
         Returns
         -------
         None
         """
         if callbacks is not None and not isinstance(callbacks, list):
             raise TypeError("callbacks must be a list")
 
         self.cursor.execute(query)
         if os.path.exists(filename) and not overwrite:
             raise SystemError(f"{os.path.abspath(filename)} already existed!")
+        f = open(filename, "w")
+        if comments:
+            comment_char = "# "
+            query_commented = query.replace("\n", "\n" + comment_char)
+            if "\n" in query_commented[:1]:
+                # in case the first character is new line
+                query_commented = query_commented[1:]
+            else:
+                # in case the first character is NOT new line so we need to add comment in the first line
+                query_commented = comment_char + query_commented
+            if "\n" in query_commented[-3:-2]:
+                # in case the last character is new line, so will mess up the csv header
+                query_commented = query_commented[:-2]
+            else:
+                # if not we need to add a new line so header wont be in the comment line
+                query_commented = query_commented + "\n"
+            f.write(query_commented)
         # write header rows
         header_og = [d[0] for d in self.cursor.description]
         if callbacks is not None:
             header_big = [d[0] for d in self.cursor.description]
             header_big.extend([i.new_col_name for i in callbacks])
             self._check_callbacks_header(header_og, callbacks)
         else:
             header_big = header_og
-        pd.DataFrame(columns=header_big).to_csv(filename, index=False)
-        # csv_out.writerow(header)
         first_flag = True
         with tqdm(unit=" rows") as pbar:
             pbar.set_description_str("Rows written: ")
             while True:  # looping until the end
-                results = self.cursor.fetchmany(chunchsize)
+                results = self.cursor.fetchmany(chunksize)
                 if results == []:
                     break
                 _df = pd.DataFrame(results, columns=header_og)
                 if callbacks is not None:
                     _df = self._result_after_callbacks(_df, callbacks)
                 _df.to_csv(
-                    filename,
+                    f,
                     mode="a" if not first_flag else "w",
                     index=False,
                     header=False if not first_flag else True,
+                    lineterminator="\n"
                 )
                 first_flag = False
                 pbar.update(len(_df))
         return None
 
     @preprocess_query
     def query(self, query, callbacks=None):
```

### Comparing `MyGaiaDB-0.2/mygaiadb/utils.py` & `MyGaiaDB-0.3/mygaiadb/utils.py`

 * *Files identical despite different names*

### Comparing `MyGaiaDB-0.2/setup.py` & `MyGaiaDB-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     include_dirs=[pathlib.Path("./mygaiadb/ext_c/").as_posix()],
 )
 
 ext_modules = [astroqlite_c]
 
 setup(
     name="MyGaiaDB",
-    version="0.2",
+    version="0.3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Astronomy",
         "Topic :: Database :: Database Engines/Servers",
```

### Comparing `MyGaiaDB-0.2/tests/test_ext.py` & `MyGaiaDB-0.3/tests/test_ext.py`

 * *Files identical despite different names*

