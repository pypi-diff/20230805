# Comparing `tmp/distfit-1.6.8.tar.gz` & `tmp/distfit-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distfit-1.6.8.tar", last modified: Wed Mar  8 17:52:54 2023, max compression
+gzip compressed data, was "distfit-1.6.9.tar", last modified: Tue Mar 14 21:35:41 2023, max compression
```

## Comparing `distfit-1.6.8.tar` & `distfit-1.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 17:52:54.076379 distfit-1.6.8/
--rw-rw-rw-   0        0        0     1181 2021-02-06 21:18:04.000000 distfit-1.6.8/LICENSE
--rw-rw-rw-   0        0        0        0 2021-02-06 21:18:04.000000 distfit-1.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0    11483 2023-03-08 17:52:54.074383 distfit-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0    10901 2023-02-24 20:53:14.000000 distfit-1.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-08 17:52:53.985665 distfit-1.6.8/distfit/
--rw-rw-rw-   0        0        0     2141 2023-03-08 16:18:57.000000 distfit-1.6.8/distfit/__init__.py
--rw-rw-rw-   0        0        0   116083 2023-03-07 21:42:02.000000 distfit-1.6.8/distfit/distfit.py
--rw-rw-rw-   0        0        0    21914 2023-03-08 16:16:31.000000 distfit-1.6.8/distfit/examples.py
-drwxrwxrwx   0        0        0        0 2023-03-08 17:52:54.069407 distfit-1.6.8/distfit/tests/
--rw-rw-rw-   0        0        0        0 2022-03-19 18:20:44.000000 distfit-1.6.8/distfit/tests/__init__.py
--rw-rw-rw-   0        0        0    14005 2023-02-11 20:27:35.000000 distfit-1.6.8/distfit/tests/test_distfit.py
-drwxrwxrwx   0        0        0        0 2023-03-08 17:52:54.049456 distfit-1.6.8/distfit.egg-info/
--rw-rw-rw-   0        0        0    11483 2023-03-08 17:52:52.000000 distfit-1.6.8/distfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-03-08 17:52:53.000000 distfit-1.6.8/distfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 17:52:52.000000 distfit-1.6.8/distfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-03-08 17:52:53.000000 distfit-1.6.8/distfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-08 17:52:53.000000 distfit-1.6.8/distfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-08 17:52:54.076659 distfit-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1690 2023-02-17 16:25:54.000000 distfit-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-14 21:35:41.393917 distfit-1.6.9/
+-rw-rw-rw-   0        0        0     1181 2021-02-06 21:18:04.000000 distfit-1.6.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-02-06 21:18:04.000000 distfit-1.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    11480 2023-03-14 21:35:41.392912 distfit-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10898 2023-03-14 21:35:32.000000 distfit-1.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-14 21:35:41.368076 distfit-1.6.9/distfit/
+-rw-rw-rw-   0        0        0     2141 2023-03-14 21:29:05.000000 distfit-1.6.9/distfit/__init__.py
+-rw-rw-rw-   0        0        0   115294 2023-03-14 21:25:22.000000 distfit-1.6.9/distfit/distfit.py
+-rw-rw-rw-   0        0        0    24188 2023-03-14 21:24:11.000000 distfit-1.6.9/distfit/examples.py
+drwxrwxrwx   0        0        0        0 2023-03-14 21:35:41.389854 distfit-1.6.9/distfit/tests/
+-rw-rw-rw-   0        0        0        0 2022-03-19 18:20:44.000000 distfit-1.6.9/distfit/tests/__init__.py
+-rw-rw-rw-   0        0        0    14005 2023-03-14 17:48:05.000000 distfit-1.6.9/distfit/tests/test_distfit.py
+drwxrwxrwx   0        0        0        0 2023-03-14 21:35:41.387868 distfit-1.6.9/distfit.egg-info/
+-rw-rw-rw-   0        0        0    11480 2023-03-14 21:35:40.000000 distfit-1.6.9/distfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-03-14 21:35:41.000000 distfit-1.6.9/distfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-14 21:35:40.000000 distfit-1.6.9/distfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-03-14 21:35:40.000000 distfit-1.6.9/distfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-03-14 21:35:41.000000 distfit-1.6.9/distfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-14 21:35:41.394907 distfit-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1690 2023-02-17 16:25:54.000000 distfit-1.6.9/setup.py
```

### Comparing `distfit-1.6.8/LICENSE` & `distfit-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `distfit-1.6.8/PKG-INFO` & `distfit-1.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: distfit
-Version: 1.6.8
+Version: 1.6.9
 Summary: distfit is a python library for probability density fitting.
 Home-page: https://erdogant.github.io/distfit
-Download-URL: https://github.com/erdogant/distfit/archive/1.6.8.tar.gz
+Download-URL: https://github.com/erdogant/distfit/archive/1.6.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -152,42 +152,42 @@
 # 
 
 ##### [Example: Make predictions using the fitted distribution](https://erdogant.github.io/distfit/pages/html/Examples.html#make-predictions)
 
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#make-predictions">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP1a.png" width="450" />
   </a>
 </p>
 
 
 
 # 
 
 ##### [Example: Test for one specific distributions](https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-distribution)
 
 The full list of distributions is listed here: https://erdogant.github.io/distfit/pages/html/Parametric.html
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-distribution">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP3b.png" width="450" />
   </a>
 </p>
 
 
 # 
 
 ##### [Example: Test for multiple distributions](https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-multiple-distributions)
 
 The full list of distributions is listed here: https://erdogant.github.io/distfit/pages/html/Parametric.html
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-multiple-distributions">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP2b.png" width="450" />
   </a>
 </p>
 
 
 #
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: distfit Version: 1.6.8 Summary: distfit is a python
+Metadata-Version: 2.1 Name: distfit Version: 1.6.9 Summary: distfit is a python
 library for probability density fitting. Home-page: https://erdogant.github.io/
-distfit Download-URL: https://github.com/erdogant/distfit/archive/1.6.8.tar.gz
+distfit Download-URL: https://github.com/erdogant/distfit/archive/1.6.9.tar.gz
 Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE
      [https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://
@@ -87,25 +87,25 @@
 erdogant.github.io/distfit/pages/html/Examples.html#plot-rss) After we have a
 fitted model, we can make some predictions using the theoretical distributions.
 After making some predictions, we can plot again but now the predictions are
 automatically included.
 [https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_summary.png]
 # ##### [Example: Make predictions using the fitted distribution](https://
 erdogant.github.io/distfit/pages/html/Examples.html#make-predictions)
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP1a.png]
 # ##### [Example: Test for one specific distributions](https://
 erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-
 distribution) The full list of distributions is listed here: https://
 erdogant.github.io/distfit/pages/html/Parametric.html
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP3b.png]
 # ##### [Example: Test for multiple distributions](https://erdogant.github.io/
 distfit/pages/html/Examples.html#fit-for-multiple-distributions) The full list
 of distributions is listed here: https://erdogant.github.io/distfit/pages/html/
 Parametric.html
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP2b.png]
 # ##### [Example: Fit discrete distribution](https://erdogant.github.io/
 distfit/pages/html/Discrete.html) ```python from scipy.stats import binom #
 Generate random numbers # Set parameters for the test-case n = 8 p = 0.5 #
 Generate 10000 samples of the distribution of (n, p) X = binom(n, p).rvs(10000)
 print(X) # [5 1 4 5 5 6 2 4 6 5 4 4 4 7 3 4 4 2 3 3 4 4 5 1 3 2 7 4 5 2 3 4 3 3
 2 3 5 # 4 6 7 6 2 4 3 3 5 3 5 3 4 4 4 7 5 4 5 3 4 3 3 4 3 3 6 3 3 5 4 4 2 3 2 5
 7 # 5 4 8 3 4 3 5 4 3 5 5 2 5 6 7 4 5 5 5 4 4 3 4 5 6 2...] # Import distfit
```

### Comparing `distfit-1.6.8/README.md` & `distfit-1.6.9/distfit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: distfit
+Version: 1.6.9
+Summary: distfit is a python library for probability density fitting.
+Home-page: https://erdogant.github.io/distfit
+Download-URL: https://github.com/erdogant/distfit/archive/1.6.9.tar.gz
+Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png" width="600" />
   </a>
 </p>
 
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://img.shields.io/pypi/pyversions/distfit)
@@ -135,42 +152,42 @@
 # 
 
 ##### [Example: Make predictions using the fitted distribution](https://erdogant.github.io/distfit/pages/html/Examples.html#make-predictions)
 
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#make-predictions">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP1a.png" width="450" />
   </a>
 </p>
 
 
 
 # 
 
 ##### [Example: Test for one specific distributions](https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-distribution)
 
 The full list of distributions is listed here: https://erdogant.github.io/distfit/pages/html/Parametric.html
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-distribution">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP3b.png" width="450" />
   </a>
 </p>
 
 
 # 
 
 ##### [Example: Test for multiple distributions](https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-multiple-distributions)
 
 The full list of distributions is listed here: https://erdogant.github.io/distfit/pages/html/Parametric.html
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-multiple-distributions">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP2b.png" width="450" />
   </a>
 </p>
 
 
 # 
 
 
@@ -247,7 +264,9 @@
 ### Citation
 Please cite ``distfit`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
+
+
```

#### html2text {}

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1 Name: distfit Version: 1.6.9 Summary: distfit is a python
+library for probability density fitting. Home-page: https://erdogant.github.io/
+distfit Download-URL: https://github.com/erdogant/distfit/archive/1.6.9.tar.gz
+Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE
      [https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://
 img.shields.io/pypi/pyversions/distfit) [![Pypi](https://img.shields.io/pypi/v/
 distfit)](https://pypi.org/project/distfit/) [![Docs](https://img.shields.io/
 badge/Sphinx-Docs-Green)](https://erdogant.github.io/distfit/) [![LOC](https://
 sloc.xyz/github/erdogant/distfit/?category=code)](https://github.com/erdogant/
 distfit/) [![Downloads](https://static.pepy.tech/personalized-badge/
@@ -79,25 +87,25 @@
 erdogant.github.io/distfit/pages/html/Examples.html#plot-rss) After we have a
 fitted model, we can make some predictions using the theoretical distributions.
 After making some predictions, we can plot again but now the predictions are
 automatically included.
 [https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_summary.png]
 # ##### [Example: Make predictions using the fitted distribution](https://
 erdogant.github.io/distfit/pages/html/Examples.html#make-predictions)
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP1a.png]
 # ##### [Example: Test for one specific distributions](https://
 erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-
 distribution) The full list of distributions is listed here: https://
 erdogant.github.io/distfit/pages/html/Parametric.html
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP3b.png]
 # ##### [Example: Test for multiple distributions](https://erdogant.github.io/
 distfit/pages/html/Examples.html#fit-for-multiple-distributions) The full list
 of distributions is listed here: https://erdogant.github.io/distfit/pages/html/
 Parametric.html
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP2b.png]
 # ##### [Example: Fit discrete distribution](https://erdogant.github.io/
 distfit/pages/html/Discrete.html) ```python from scipy.stats import binom #
 Generate random numbers # Set parameters for the test-case n = 8 p = 0.5 #
 Generate 10000 samples of the distribution of (n, p) X = binom(n, p).rvs(10000)
 print(X) # [5 1 4 5 5 6 2 4 6 5 4 4 4 7 3 4 4 2 3 3 4 4 5 1 3 2 7 4 5 2 3 4 3 3
 2 3 5 # 4 6 7 6 2 4 3 3 5 3 5 3 4 4 4 7 5 4 5 3 4 3 3 4 3 3 6 3 3 5 4 4 2 3 2 5
 7 # 5 4 8 3 4 3 5 4 3 5 5 2 5 6 7 4 5 5 5 4 4 3 4 5 6 2...] # Import distfit
```

### Comparing `distfit-1.6.8/distfit/__init__.py` & `distfit-1.6.9/distfit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distfit.distfit import distfit
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.6.8'
+__version__ = '1.6.9'
 
 
 # module level doc-string
 __doc__ = """
 distfit
 =====================================================================
 distfit is a python package for probability density fitting of univariate distributions for random variables.
@@ -40,18 +40,18 @@
 >>> # Plot summary
 >>> dfit.plot_summary()
 >>>
 >>> # Make prediction
 >>> results_proba = dfit.predict(y)
 >>>
 >>> # Plot PDF
->>> fig, ax = dfit.plot(chart='PDF', n_top=1)
+>>> fig, ax = dfit.plot(chart='pdf', n_top=1)
 >>>
 >>> # Add the CDF to the plot
->>> fig, ax = dfit.plot(chart='CDF', n_top=1, ax=ax)
+>>> fig, ax = dfit.plot(chart='cdf', n_top=1, ax=ax)
 >>>
 >>> # QQ-plot for top 10 fitted distributions
 >>> fig, ax = dfit.qqplot(X, n_top=10)
 >>>
 
 References
 ----------
```

### Comparing `distfit-1.6.8/distfit/distfit.py` & `distfit-1.6.9/distfit/distfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,18 @@
     >>> # PDF plot
     >>> dfit.plot()
     >>>
     >>> # Make prediction
     >>> results_proba = dfit.predict(y)
     >>>
     >>> # Plot PDF
-    >>> fig, ax = dfit.plot(chart='PDF')
+    >>> fig, ax = dfit.plot(chart='pdf')
     >>>
     >>> # Add the CDF to the plot
-    >>> fig, ax = dfit.plot(chart='CDF', n_top=1, ax=ax)
+    >>> fig, ax = dfit.plot(chart='cdf', n_top=1, ax=ax)
     >>>
     >>> # QQ-plot for top 10 fitted distributions
     >>> fig, ax = dfit.qqplot(X, n_top=10)
     >>>
     """
 
     def __init__(self,
@@ -194,18 +194,18 @@
         >>> # PDF plot
         >>> dfit.plot()
         >>>
         >>> # Make prediction
         >>> results_proba = dfit.predict(y)
         >>>
         >>> # Plot PDF
-        >>> fig, ax = dfit.plot(chart='PDF', n_top=1)
+        >>> fig, ax = dfit.plot(chart='pdf', n_top=1)
         >>>
         >>> # Add the CDF to the plot
-        >>> fig, ax = dfit.plot(chart='CDF', n_top=1, ax=ax)
+        >>> fig, ax = dfit.plot(chart='cdf', n_top=1, ax=ax)
         >>>
         >>> # QQ-plot for top 10 fitted distributions
         >>> fig, ax = dfit.qqplot(X, n_top=10)
         >>>
 
         References
         ----------
@@ -670,15 +670,15 @@
             binedges = snsout[0]
             # binedges = np.append(binedges, 10**-6)
 
         return (binedges, histvals)
 
     # Plot
     def plot(self,
-             chart='PDF',
+             chart='pdf',
              n_top=1,
              title='',
              emp_properties={'color': '#000000', 'linewidth': 3, 'linestyle': '-'},
              pdf_properties={'color': '#880808', 'linewidth': 3, 'linestyle': '-'},
              bar_properties={'color': '#607B8B', 'linewidth': 1, 'edgecolor': '#5A5A5A', 'align': 'center'},
              cii_properties={'color': '#C41E3A', 'linewidth': 3, 'linestyle': 'dashed', 'marker': 'x', 'size': 20, 'color_sign_multipletest': 'g', 'color_sign': 'g', 'color_general': 'r'},
              fontsize=16,
@@ -692,18 +692,18 @@
              grid=True,
              cmap=None,
              verbose=None):
         """Make plot.
 
         Parameters
         ----------
-        chart: str, default: 'PDF'
+        chart: str, default: 'pdf'
             Chart to plot.
-                * 'PDF': Probability density function.
-                * 'CDF': Cumulative density function.
+                * 'pdf': Probability density function.
+                * 'cdf': Cumulative density function.
         n_top : int, optional
             Show the top number of results. The default is 1.
         title : String, optional (default: '')
             Title of the plot.
         emp_properties : dict
             The line properties of the emperical line.
                 * None: Do not plot.
@@ -765,43 +765,43 @@
         >>>
         >>> # Initialize
         >>> dfit = distfit(alpha=0.01)
         >>> dfit.fit_transform(X)
         >>> dfit.predict(y)
         >>>
         >>> # Plot seperately
-        >>> fig, ax = dfit.plot(chart='PDF')
-        >>> fig, ax = dfit.plot(chart='CDF')
+        >>> fig, ax = dfit.plot(chart='pdf')
+        >>> fig, ax = dfit.plot(chart='cdf')
         >>>
         >>> # Change or remove properties of the chart.
-        >>> dfit.plot(chart='PDF', pdf_properties={'color': 'r'}, cii_properties={'color': 'g'}, emp_properties=None, bar_properties=None)
-        >>> dfit.plot(chart='CDF', pdf_properties={'color': 'r'}, cii_properties={'color': 'g'}, emp_properties=None, bar_properties=None)
+        >>> dfit.plot(chart='pdf', pdf_properties={'color': 'r'}, cii_properties={'color': 'g'}, emp_properties=None, bar_properties=None)
+        >>> dfit.plot(chart='cdf', pdf_properties={'color': 'r'}, cii_properties={'color': 'g'}, emp_properties=None, bar_properties=None)
         >>>
         >>> # Create subplot
         >>> fig, ax = plt.subplots(1,2, figsize=(25, 10))
-        >>> dfit.plot(chart='PDF', ax=ax[0])
-        >>> dfit.plot(chart='CDF', ax=ax[1])
+        >>> dfit.plot(chart='pdf', ax=ax[0])
+        >>> dfit.plot(chart='cdf', ax=ax[1])
         >>>
         >>> # Change or remove properties of the chart.
-        >>> fig, ax = dfit.plot(chart='PDF', pdf_properties={'color': 'r', 'linewidth': 3}, cii_properties={'color': 'r', 'linewidth': 3}, bar_properties={'color': '#1e3f5a'})
-        >>> dfit.plot(chart='CDF', n_top=10, pdf_properties={'color': 'r'}, cii_properties=None, bar_properties=None, ax=ax)
+        >>> fig, ax = dfit.plot(chart='pdf', pdf_properties={'color': 'r', 'linewidth': 3}, cii_properties={'color': 'r', 'linewidth': 3}, bar_properties={'color': '#1e3f5a'})
+        >>> dfit.plot(chart='cdf', n_top=10, pdf_properties={'color': 'r'}, cii_properties=None, bar_properties=None, ax=ax)
 
         """
         if verbose is not None: set_logger(verbose)
         if not hasattr(self, 'model'): raise Exception('[distfit] Error in plot: For plotting, A model is required. Try fitting first on your data using fit_transform(X)')
         properties = _get_properties(pdf_properties, emp_properties, bar_properties, cii_properties)
 
         logger.info('Create %s plot for the %s method.' %(chart, self.method))
-        if chart.upper()=='PDF' and self.method=='parametric':
+        if chart.lower()=='pdf' and self.method=='parametric':
             fig, ax = _plot_parametric(self, title=title, figsize=figsize, xlim=xlim, ylim=ylim, fig=fig, ax=ax, grid=grid, emp_properties=properties['emp'], pdf_properties=properties['pdf'], bar_properties=properties['bar'], cii_properties=properties['cii'], n_top=n_top, cmap=cmap, xlabel=xlabel, ylabel=ylabel, fontsize=fontsize)
-        elif chart.upper()=='PDF' and self.method=='discrete':
+        elif chart.lower()=='pdf' and self.method=='discrete':
             fig, ax = plot_binom(self, title=title, figsize=figsize, xlim=xlim, ylim=ylim, grid=grid, emp_properties=properties['emp'], pdf_properties=properties['pdf'], bar_properties=properties['bar'], cii_properties=properties['cii'], xlabel=xlabel, ylabel=ylabel, fontsize=fontsize)
-        elif chart.upper()=='PDF' and (self.method=='quantile') or (self.method=='percentile'):
+        elif chart.lower()=='pdf' and (self.method=='quantile') or (self.method=='percentile'):
             fig, ax = _plot_quantile(self, title=title, figsize=figsize, xlim=xlim, ylim=ylim, fig=fig, ax=ax, grid=grid, emp_properties=properties['emp'], bar_properties=properties['bar'], cii_properties=properties['cii'], xlabel=xlabel, ylabel=ylabel, fontsize=fontsize)
-        elif chart.upper()=='CDF' and (self.method=='parametric' or self.method=='discrete'):
+        elif chart.lower()=='cdf' and (self.method=='parametric' or self.method=='discrete'):
             fig, ax = self.plot_cdf(n_top=n_top, title=title, figsize=figsize, xlim=xlim, ylim=ylim, fig=fig, ax=ax, grid=grid, emp_properties=properties['emp'], cdf_properties=properties['pdf'], cii_properties=properties['cii'], cmap=cmap, xlabel=xlabel, ylabel=ylabel, fontsize=fontsize)
         else:
             logger.warning('Nothing to plot. %s not yet implemented or possible for the %s approach.' %(chart, self.method))
             fig, ax = None, None
 
         # Return
         return fig, ax
@@ -1133,23 +1133,23 @@
         >>> # Initialize
         >>> dfit = distfit()
         >>>
         >>> # Fit
         >>> dfit.fit_transform(X)
         >>>
         >>> # Make CDF plot
-        >>> fig, ax = dfit.plot(chart='CDF')
+        >>> fig, ax = dfit.plot(chart='cdf')
         >>>
         >>> # Append the PDF plot
-        >>> dfit.plot(chart='PDF', fig=fig, ax=ax)
+        >>> dfit.plot(chart='pdf', fig=fig, ax=ax)
         >>>
         >>> # Plot the CDF of the top 10 fitted distributions.
-        >>> fig, ax = dfit.plot(chart='CDF', n_top=10)
+        >>> fig, ax = dfit.plot(chart='cdf', n_top=10)
         >>> # Append the PDF plot
-        >>> dfit.plot(chart='PDF', n_top=10, fig=fig, ax=ax)
+        >>> dfit.plot(chart='pdf', n_top=10, fig=fig, ax=ax)
         >>>
         """
         logger.info('Ploting CDF')
         if verbose is not None: set_logger(verbose)
         if n_top is None: n_top = 1
         properties = _get_properties(cdf_properties, emp_properties, None, cii_properties)
 
@@ -1668,37 +1668,42 @@
     # Bootstrapping
     # the goal here is to estimate the KS statistic of the fitted distribution when the params are estimated from data.
     # 1. Resample using fitted distribution.
     # 2. Use the resampled data to fit again the distribution.
     # 3. Compare the resampled data vs. fitted PDF.
 
     bootstrap_score, bootstrap_pass = 0, None
-    if (n_boots is not None) and (n_boots>=10):
-        # Limit the number of samples to avoid memory issues.
-        n = np.minimum(10000, len(X))
-        # Kolmogorov-Smirnov (KS) statistic
-        Dn = st.kstest(X, distribution_fit.cdf)
-
-        Dns=[]
-        for i in tqdm(range(n_boots), desc="[distfit] >Bootstrapping " + distribution.name.title(), position=0, leave=False, disable=disable_tqdm()):
-            # Resample from target distribution: k
-            resamples = distribution_fit.rvs(n, random_state=random_state)
-            # Find new target parameters after resampling
-            params = distribution.fit(resamples)
-            # Create new fit: k-hat
-            fit = distribution(*params)
-            # Score the k-hat distribution vs. for the resampled data of distribution k.
-            Dn_i = st.kstest(resamples, fit.cdf)
-            # Store the test statistics
-            Dns.append(Dn_i[0])
-
-        Dn_alpha = np.quantile(Dns, 1 - alpha)
-        bootstrap_pass = False if Dn[0] > Dn_alpha else True
-        # Compute ratio correct
-        bootstrap_score = np.sum(Dns > Dn[0]) / n_boots
+    
+    try:
+        if (n_boots is not None) and (n_boots>=10):
+            # Limit the number of samples to avoid memory issues.
+            n = np.minimum(10000, len(X))
+            # Kolmogorov-Smirnov (KS) statistic
+            Dn = st.kstest(X, distribution_fit.cdf)
+    
+            Dns=[]
+            for i in tqdm(range(n_boots), desc="[distfit] >Bootstrapping " + distribution.name.title(), position=0, leave=False, disable=disable_tqdm()):
+                # Resample n times from target distribution.
+                resamples = distribution_fit.rvs(n, random_state=random_state)
+                # Find new target parameters after resampling
+                params = distribution.fit(resamples)
+                # Create new fit: k-hat
+                fit = distribution(*params)
+                # Score the k-hat distribution vs. for the resampled data of distribution k.
+                Dn_i = st.kstest(resamples, fit.cdf)
+                # Store the test statistics
+                Dns.append(Dn_i[0])
+    
+            Dn_alpha = np.quantile(Dns, 1 - alpha)
+            bootstrap_pass = False if Dn[0] > Dn_alpha else True
+            # Compute ratio correct
+            bootstrap_score = np.sum(Dns > Dn[0]) / n_boots
+    except:
+        pass
+        # logger.info('[%s] > Could not estimate fit, likely due to low sample size.' %(distr))
     # Return
     return bootstrap_score, bootstrap_pass
 
 
 # %%
 def _get_properties(pdf_properties, emp_properties, bar_properties, cii_properties):
     if cii_properties is not None: cii_properties = {**{'color': '#C41E3A', 'linewidth': 3, 'linestyle': 'dashed', 'marker': 'x', 'size': 20, 'color_sign_multipletest': 'g', 'color_sign': 'g', 'color_general': 'r', 'alpha': 1}, **cii_properties}
@@ -2097,22 +2102,15 @@
     out['random_state'] = random_state
     # Return
     return out
 
 
 # %% Compute score for each distribution
 def _compute_score_distribution(data, X, y_obs, DISTRIBUTIONS, stats, cmap='Set1', n_boots=None, random_state=None):
-    # model = {}
-    # model['name'] = st.norm
-    # model['stats'] = stats
-    # model['params'] = (0.0, 1.0)
-    best_score = np.inf
-    best_bootstrap_score = np.inf
     df = pd.DataFrame(index=range(0, len(DISTRIBUTIONS)), columns=['name', 'score', 'loc', 'scale', 'arg', 'params', 'model', 'bootstrap_score', 'bootstrap_pass'])
-    # max_name_len = np.max(list(map(lambda x: len(x.name), DISTRIBUTIONS)))
     max_name_len = np.max(list(map(lambda x: len(x.name) if isinstance(x.name, str) else len(x.name()), DISTRIBUTIONS)))
 
     # Estimate distribution parameters
     for i, distribution in enumerate(DISTRIBUTIONS):
 
         # Fit the distribution. However this can result in an error. I need the try-except.
         try:
@@ -2147,29 +2145,14 @@
                 df.values[i, 3] = scale
                 df.values[i, 4] = arg
                 df.values[i, 5] = params
                 df.values[i, 6] = distribution_fit
                 df.values[i, 7] = bootstrap_score
                 df.values[i, 8] = bootstrap_pass
 
-                # identify if this distribution is better
-                # if (best_score > score > 0) or (best_bootstrap_score > bootstrap_score > 0):
-                #     best_score = score
-                #     best_bootstrap_score = bootstrap_score
-                #     model['name'] = distr_name
-                #     model['name'] = distribution
-                #     model['model'] = distribution_fit
-                #     model['params'] = params
-                #     model['score'] = score
-                #     model['loc'] = loc
-                #     model['scale'] = scale
-                #     model['arg'] = arg
-                #     model['bootstrap_score'] = bootstrap_score
-                #     model['bootstrap_pass'] = bootstrap_pass
-
             # Setup for the logger
             spaces_1 = ' ' * (max_name_len - len(distr_name))
             scores = ('[%s: %g] [loc=%.3f scale=%.3f]' %(stats, score, loc, scale))
             time_spent = time.time() - start_time
             logger.info("[%s%s] [%.4s sec] %s" %(distr_name, spaces_1, time_spent, scores))
 
         except Exception:
```

### Comparing `distfit-1.6.8/distfit/examples.py` & `distfit-1.6.9/distfit/examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,94 @@
 from distfit import distfit
+import pandas as pd
+
+normal_distributions = ["halfgennorm", "lognorm", "powerlognorm",
+                        "gennorm", "norm", "truncnorm", "exponnorm",
+                        "powernorm", "foldnorm",  "halfnorm"]
+
+values = pd.read_pickle(r"C:\Users\playground\Downloads\repro\repro_data")
+dist_fitter = distfit(distr=normal_distributions, n_boots=10)
+dist_fitter.fit_transform(values)
+dist_fitter.plot_summary()
+dist_fitter.plot()
+dist_fitter.bootstrap(values, n_boots=10, update_model=False)
+
+# %%
+import matplotlib.pyplot as plt
+from distfit import distfit
+import seaborn as sns
+import numpy as np
+import scipy.stats as st
+np.random.seed(4)
+
+loc = 5
+scale=10
+sample_dist = st.lognorm.rvs(3, loc=loc, scale=np.exp(scale), size=10000)
+# shape, loc, scale = st.lognorm.fit(sample_dist, floc=0)
+# print(shape, loc, scale)
+# print(np.log(scale), shape) # mu and sigma
+
+dfit = distfit('parametric', todf=True, distr=["lognorm"])
+dfit.fit_transform(sample_dist)
+
+print('Estimated loc: %g, input loc: %g' %(dfit.model['loc'], loc))
+print('Estimated mu or scale: %g, input scale: %g' %(np.log(dfit.model['scale']), scale))
+
+# mu
+np.mean(np.log(sample_dist))
+
+
+mu=13.8
+loc=47.55
+x_sim = np.random.normal(loc=loc,scale=np.exp(mu), size = 10000)
+x_sim = np.append([*filter(lambda x: x<=80, x_sim)],np.random.normal(loc=90,scale=10, size = 50))
+x_sim = np.array([*filter(lambda x: x >=0,x_sim)])
+
+# shape, loc, scale = stats.lognorm.fit(sample, floc=0) # hold location to 0 while fitting
+# np.mean(x_sim)
+# np.std(np.log(x_sim))
+
+dfit = distfit(todf=True, distr=["lognorm"])
+dfit.fit_transform(x_sim)
+dfit.bootstrap(x_sim, n_boots=1)
+
+# print('Estimated loc: %g, input loc: %g' %(dfit.model['loc'], loc))
+print('Estimated mu or scale: %g, input scale: %g' %(np.log(dfit.model['scale']), mu))
+dfit.plot()
+
+np.mean(np.log(x_sim))
+np.std(np.log(x_sim))
+
+
+# sns.histplot(x,ax=ax[0])
+fig, ax = plt.subplots(1,3, figsize=(20,8))
+dfit.plot("PDF",n_top=3,fontsize=11, pdf_properties=None, cii_properties=None, emp_properties=None, ax=ax[0], bar_properties={'edgecolor': '#000000'})
+dfit.plot("PDF",n_top=3,fontsize=11,ax=ax[1])
+dfit.plot("CDF",n_top=3,fontsize=11,ax=ax[2])
+plt.show()
+
+# %%
+from distfit import distfit
 import matplotlib.pyplot as plt
 
 dfit = distfit(smooth=3, bound='up')
 df = dfit.import_example(data='tips')
 dfit.fit_transform(df['tip'], n_boots=100)
 # dfit.fit_transform(df['tip'], n_boots=0)
 dfit.lineplot(df['tip'], xlabel='Number', ylabel='Tip value', grid=True)
 
 # Plot PDF/CDF
 fig, ax = plt.subplots(1,2, figsize=(25, 10))
-dfit.plot(chart='PDF', n_top=5, ax=ax[0])
-dfit.plot(chart='CDF', n_top=5,ax=ax[1])
+dfit.plot(chart='pdf', n_top=5, ax=ax[0])
+dfit.plot(chart='cdf', n_top=5,ax=ax[1])
 # Show plot
 plt.show()
 
 fig, ax = dfit.plot()
-dfit.plot(chart='CDF', ax=ax)
+dfit.plot(chart='cdf', ax=ax)
 
 dfit.plot_summary()
 
 X = dfit.generate(100)
 # Ploy the data
 dfit.lineplot(X, xlabel='Number', ylabel='Tip value', grid=True)
 plt.figure();plt.plot(X)
@@ -172,16 +241,16 @@
 # Plot
 dfit.plot_summary()
 
 
 out = dfit.bootstrap(X, n_boots=10, n_top=None)
 dfit.plot_summary()
 
-fig, ax = dfit.plot(chart='PDF', n_top=5, cmap='Set2');
-dfit.plot(chart='CDF', n_top=10, cmap='Set2', ax=ax);
+fig, ax = dfit.plot(chart='pdf', n_top=5, cmap='Set2');
+dfit.plot(chart='cdf', n_top=10, cmap='Set2', ax=ax);
 dfit.plot_cdf()
 
 
 # %%
 from distfit import distfit
 # Set parameters for the test-case
 n = 8
@@ -194,18 +263,18 @@
 # Run distfit to and determine whether we can find the parameters from the data.
 results = dfit.fit_transform(X)
 # Get the model and best fitted parameters.
 
 y = [0, 1, 10, 11, 12]
 
 results = dfit.predict(y)
-dfit.plot(chart='PDF')
-dfit.plot(chart='PDF', pdf_properties=None)
-dfit.plot(chart='CDF', n_top=5)
-dfit.plot(chart='CDF', pdf_properties=None, n_top=2)
+dfit.plot(chart='pdf')
+dfit.plot(chart='pdf', pdf_properties=None)
+dfit.plot(chart='cdf', n_top=5)
+dfit.plot(chart='cdf', pdf_properties=None, n_top=2)
 dfit.plot_cdf()
 
 # %% QQ plot
 from distfit import distfit
 dfit = distfit(verbose=20)
 
 # Random Exponential data
@@ -215,39 +284,39 @@
 dfit = distfit(distr='popular')
 # Fit
 dfit.fit_transform(X)
 # QQplot
 dfit.qqplot(X)
 dfit.qqplot(X, n_top=11, cmap='Set1')
 
-dfit.plot(chart='PDF')
-dfit.plot(chart='PDF', pdf_properties=None)
-dfit.plot(chart='PDF', pdf_properties=None, n_top=10)
-dfit.plot(chart='CDF', n_top=10)
-dfit.plot(chart='CDF', pdf_properties=None, n_top=10)
+dfit.plot(chart='pdf')
+dfit.plot(chart='pdf', pdf_properties=None)
+dfit.plot(chart='pdf', pdf_properties=None, n_top=10)
+dfit.plot(chart='cdf', n_top=10)
+dfit.plot(chart='cdf', pdf_properties=None, n_top=10)
 
 
-# fig, ax = dfit.plot(chart='CDF', n_top=10);
-# dfit.plot(chart='PDF', n_top=10, fig=fig, ax=ax);
+# fig, ax = dfit.plot(chart='cdf', n_top=10);
+# dfit.plot(chart='pdf', n_top=10, fig=fig, ax=ax);
 # dfit.qqplot(X, n_top=10, fig=fig, ax=ax);
 
 # %% CDF plot
 from distfit import distfit
 dfit = distfit(verbose=20)
 
 # Random Exponential data
 X = np.random.exponential(0.5, 10000)
 # X = np.random.uniform(0, 1000, 10000)
 # X = np.random.normal(0, 1, 1000)
 dfit = distfit(distr='popular')
 # Fit and plot
 dfit.fit_transform(X)
 # dfit.plot_cdf(n_top=10);
-fig, ax = dfit.plot(chart='PDF', n_top=5, cmap='Set2');
-dfit.plot(chart='CDF', n_top=10, cmap='Set2', ax=ax);
+fig, ax = dfit.plot(chart='pdf', n_top=5, cmap='Set2');
+dfit.plot(chart='cdf', n_top=10, cmap='Set2', ax=ax);
 # dfit.plot_cdf()
 dfit.plot_summary(n_top=10);
 
 import scipy.stats as stats
 import pylab 
 # Calculate quantiles for a probability plot, and optionally show the plot.
 # Generates a probability plot of sample data against the quantiles of a specified theoretical distribution.
```

### Comparing `distfit-1.6.8/distfit/tests/test_distfit.py` & `distfit-1.6.9/distfit/tests/test_distfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from distfit import distfit
 import unittest
 from scipy.stats import binom
 import matplotlib.pyplot as plt
 
 def show_figures(dfit):
-    charts = ['PDF', 'CDF']
+    charts = ['pdf', 'cdf']
     n_top=[1, 10]
     for chart in charts:
         for n in n_top:
             dfit.plot(chart=chart, n_top=n)
             dfit.plot(chart=chart, n_top=n, cii_properties=None, emp_properties={}, pdf_properties={}, bar_properties={})
             dfit.plot(chart=chart, n_top=n, cii_properties={}, emp_properties=None, pdf_properties={}, bar_properties={})
             dfit.plot(chart=chart, n_top=n, cii_properties={}, emp_properties={}, pdf_properties=None, bar_properties={})
@@ -34,22 +34,22 @@
         dfit.bootstrap(X, n_boots=10)
         assert dfit.model
         assert np.all(np.isin(['name', 'score', 'loc', 'scale'], dfit.summary.columns))
         dfit.summary[['name', 'score', 'bootstrap_score', 'bootstrap_pass']]
 
         # Create subplot
         fig, ax = plt.subplots(1,2, figsize=(25, 10))
-        dfit.plot(chart='PDF', ax=ax[0])
-        dfit.plot(chart='CDF', ax=ax[1])
-        dfit.plot(chart='PDF',  emp_properties=None, bar_properties=None, pdf_properties={'color': 'r'}, cii_properties={'color': 'g'})
+        dfit.plot(chart='pdf', ax=ax[0])
+        dfit.plot(chart='cdf', ax=ax[1])
+        dfit.plot(chart='pdf',  emp_properties=None, bar_properties=None, pdf_properties={'color': 'r'}, cii_properties={'color': 'g'})
 
         # Create subplot
         fig, ax = plt.subplots(1,2, figsize=(25, 10))
-        dfit.plot(chart='PDF', n_top=11, ax=ax[0])
-        dfit.plot(chart='CDF', n_top=11, ax=ax[1])
+        dfit.plot(chart='pdf', n_top=11, ax=ax[0])
+        dfit.plot(chart='cdf', n_top=11, ax=ax[1])
 
         # Create subplot
         fig, ax = plt.subplots(1,2, figsize=(25, 10))
         dfit.qqplot(X, ax=ax[0])
         dfit.qqplot(X, n_top=11, ax=ax[1])
 
         # Load library
```

### Comparing `distfit-1.6.8/distfit.egg-info/PKG-INFO` & `distfit-1.6.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: distfit
-Version: 1.6.8
-Summary: distfit is a python library for probability density fitting.
-Home-page: https://erdogant.github.io/distfit
-Download-URL: https://github.com/erdogant/distfit/archive/1.6.8.tar.gz
-Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png" width="600" />
   </a>
 </p>
 
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://img.shields.io/pypi/pyversions/distfit)
@@ -152,42 +135,42 @@
 # 
 
 ##### [Example: Make predictions using the fitted distribution](https://erdogant.github.io/distfit/pages/html/Examples.html#make-predictions)
 
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#make-predictions">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP1a.png" width="450" />
   </a>
 </p>
 
 
 
 # 
 
 ##### [Example: Test for one specific distributions](https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-distribution)
 
 The full list of distributions is listed here: https://erdogant.github.io/distfit/pages/html/Parametric.html
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-distribution">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP3b.png" width="450" />
   </a>
 </p>
 
 
 # 
 
 ##### [Example: Test for multiple distributions](https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-multiple-distributions)
 
 The full list of distributions is listed here: https://erdogant.github.io/distfit/pages/html/Parametric.html
 
 <p align="left">
   <a href="https://erdogant.github.io/distfit/pages/html/Examples.html#fit-for-multiple-distributions">
-  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png" width="450" />
+  <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP2b.png" width="450" />
   </a>
 </p>
 
 
 # 
 
 
@@ -264,9 +247,7 @@
 ### Citation
 Please cite ``distfit`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1 Name: distfit Version: 1.6.8 Summary: distfit is a python
-library for probability density fitting. Home-page: https://erdogant.github.io/
-distfit Download-URL: https://github.com/erdogant/distfit/archive/1.6.8.tar.gz
-Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE
      [https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://
 img.shields.io/pypi/pyversions/distfit) [![Pypi](https://img.shields.io/pypi/v/
 distfit)](https://pypi.org/project/distfit/) [![Docs](https://img.shields.io/
 badge/Sphinx-Docs-Green)](https://erdogant.github.io/distfit/) [![LOC](https://
 sloc.xyz/github/erdogant/distfit/?category=code)](https://github.com/erdogant/
 distfit/) [![Downloads](https://static.pepy.tech/personalized-badge/
@@ -87,25 +79,25 @@
 erdogant.github.io/distfit/pages/html/Examples.html#plot-rss) After we have a
 fitted model, we can make some predictions using the theoretical distributions.
 After making some predictions, we can plot again but now the predictions are
 automatically included.
 [https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_summary.png]
 # ##### [Example: Make predictions using the fitted distribution](https://
 erdogant.github.io/distfit/pages/html/Examples.html#make-predictions)
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP1a.png]
 # ##### [Example: Test for one specific distributions](https://
 erdogant.github.io/distfit/pages/html/Examples.html#fit-for-one-specific-
 distribution) The full list of distributions is listed here: https://
 erdogant.github.io/distfit/pages/html/Parametric.html
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP3b.png]
 # ##### [Example: Test for multiple distributions](https://erdogant.github.io/
 distfit/pages/html/Examples.html#fit-for-multiple-distributions) The full list
 of distributions is listed here: https://erdogant.github.io/distfit/pages/html/
 Parametric.html
-[https://github.com/erdogant/distfit/blob/master/docs/figs/fig1_prediction.png]
+[https://github.com/erdogant/distfit/blob/master/docs/figs/example_figP2b.png]
 # ##### [Example: Fit discrete distribution](https://erdogant.github.io/
 distfit/pages/html/Discrete.html) ```python from scipy.stats import binom #
 Generate random numbers # Set parameters for the test-case n = 8 p = 0.5 #
 Generate 10000 samples of the distribution of (n, p) X = binom(n, p).rvs(10000)
 print(X) # [5 1 4 5 5 6 2 4 6 5 4 4 4 7 3 4 4 2 3 3 4 4 5 1 3 2 7 4 5 2 3 4 3 3
 2 3 5 # 4 6 7 6 2 4 3 3 5 3 5 3 4 4 4 7 5 4 5 3 4 3 3 4 3 3 6 3 3 5 4 4 2 3 2 5
 7 # 5 4 8 3 4 3 5 4 3 5 5 2 5 6 7 4 5 5 5 4 4 3 4 5 6 2...] # Import distfit
```

### Comparing `distfit-1.6.8/setup.py` & `distfit-1.6.9/setup.py`

 * *Files identical despite different names*

