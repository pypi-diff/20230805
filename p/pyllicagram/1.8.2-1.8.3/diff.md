# Comparing `tmp/pyllicagram-1.8.2.tar.gz` & `tmp/pyllicagram-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllicagram-1.8.2.tar", last modified: Thu Aug  3 10:53:57 2023, max compression
+gzip compressed data, was "pyllicagram-1.8.3.tar", last modified: Sat Aug  5 16:50:08 2023, max compression
```

## Comparing `pyllicagram-1.8.2.tar` & `pyllicagram-1.8.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.873826 pyllicagram-1.8.2/
--rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-08-03 10:53:57.873722 pyllicagram-1.8.2/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)     5361 2023-06-08 10:33:06.000000 pyllicagram-1.8.2/README.md
--rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-08-03 10:53:57.873861 pyllicagram-1.8.2/setup.cfg
--rw-r--r--   0 benoit2c   (501) staff       (20)      413 2023-08-03 10:52:51.000000 pyllicagram-1.8.2/setup.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.872349 pyllicagram-1.8.2/src/
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.872871 pyllicagram-1.8.2/src/pyllicagram/
--rw-r--r--   0 benoit2c   (501) staff       (20)     6083 2023-08-03 10:49:16.000000 pyllicagram-1.8.2/src/pyllicagram/__init__.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-03 10:53:57.873581 pyllicagram-1.8.2/src/pyllicagram.egg-info/
--rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/SOURCES.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/dependency_links.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/requires.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-08-03 10:53:57.000000 pyllicagram-1.8.2/src/pyllicagram.egg-info/top_level.txt
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-05 16:50:08.514620 pyllicagram-1.8.3/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-08-05 16:50:08.514512 pyllicagram-1.8.3/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)     5361 2023-06-08 10:33:06.000000 pyllicagram-1.8.3/README.md
+-rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-08-05 16:50:08.514657 pyllicagram-1.8.3/setup.cfg
+-rw-r--r--   0 benoit2c   (501) staff       (20)      413 2023-08-05 16:49:14.000000 pyllicagram-1.8.3/setup.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-05 16:50:08.513262 pyllicagram-1.8.3/src/
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-05 16:50:08.513732 pyllicagram-1.8.3/src/pyllicagram/
+-rw-r--r--   0 benoit2c   (501) staff       (20)     6084 2023-08-05 16:49:01.000000 pyllicagram-1.8.3/src/pyllicagram/__init__.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-08-05 16:50:08.514366 pyllicagram-1.8.3/src/pyllicagram.egg-info/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-08-05 16:50:08.000000 pyllicagram-1.8.3/src/pyllicagram.egg-info/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-08-05 16:50:08.000000 pyllicagram-1.8.3/src/pyllicagram.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-08-05 16:50:08.000000 pyllicagram-1.8.3/src/pyllicagram.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-08-05 16:50:08.000000 pyllicagram-1.8.3/src/pyllicagram.egg-info/requires.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-08-05 16:50:08.000000 pyllicagram-1.8.3/src/pyllicagram.egg-info/top_level.txt
```

### Comparing `pyllicagram-1.8.2/README.md` & `pyllicagram-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyllicagram-1.8.2/src/pyllicagram/__init__.py` & `pyllicagram-1.8.3/src/pyllicagram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # ------------------------
 # API CALL
 def pyllicagram(recherche,corpus="presse",debut=1789,fin=1950,resolution="default",somme=False):
         if not isinstance(recherche, str) and not isinstance(recherche, list):
             raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
         if not isinstance(recherche, list): recherche = [recherche]
-        assert corpus in ["lemonde","livres","presse","huma","paris"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
+        #assert corpus in ["lemonde","livres","presse","huma","paris"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
         assert resolution in ["default","annee","mois"], 'Vous devez choisir la résolution parmi "default", "annee" ou "mois"'
         result = []
         for gram in tqdm(recherche):
                 gram = urllib.parse.quote_plus(gram.lower()).replace("-"," ").replace("+"," ")
                 gram = gram.replace(" ","%20")
                 df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/query?corpus={corpus}&mot={gram}&from={debut}&to={fin}&resolution={resolution:}")
                 #if resolution=="mois" and corpus != "livres":
```

