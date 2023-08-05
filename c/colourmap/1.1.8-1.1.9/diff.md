# Comparing `tmp/colourmap-1.1.8.tar.gz` & `tmp/colourmap-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colourmap-1.1.8.tar", last modified: Tue Oct 18 09:31:28 2022, max compression
+gzip compressed data, was "colourmap-1.1.9.tar", last modified: Tue Oct 18 11:43:57 2022, max compression
```

## Comparing `colourmap-1.1.8.tar` & `colourmap-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-18 09:31:28.140675 colourmap-1.1.8/
--rw-rw-rw-   0        0        0     1169 2022-02-17 15:03:48.000000 colourmap-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      118 2022-02-17 15:03:48.000000 colourmap-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4049 2022-10-18 09:31:28.140675 colourmap-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3433 2022-04-03 09:21:03.000000 colourmap-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-18 09:31:28.117005 colourmap-1.1.8/colourmap/
--rw-rw-rw-   0        0        0      751 2022-10-18 09:30:58.000000 colourmap-1.1.8/colourmap/__init__.py
--rw-rw-rw-   0        0        0     9395 2022-09-02 11:38:42.000000 colourmap-1.1.8/colourmap/colourmap.py
--rw-rw-rw-   0        0        0     1254 2022-04-04 19:37:17.000000 colourmap-1.1.8/colourmap/examples.py
-drwxrwxrwx   0        0        0        0 2022-10-18 09:31:28.138681 colourmap-1.1.8/colourmap.egg-info/
--rw-rw-rw-   0        0        0     4049 2022-10-18 09:31:27.000000 colourmap-1.1.8/colourmap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2022-10-18 09:31:27.000000 colourmap-1.1.8/colourmap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 09:31:27.000000 colourmap-1.1.8/colourmap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-10-18 09:31:27.000000 colourmap-1.1.8/colourmap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-10-18 09:31:27.000000 colourmap-1.1.8/colourmap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      262 2022-10-18 09:31:28.144664 colourmap-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1365 2022-03-11 12:58:41.000000 colourmap-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-18 11:43:57.675200 colourmap-1.1.9/
+-rw-rw-rw-   0        0        0     1169 2022-02-17 15:03:48.000000 colourmap-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      118 2022-02-17 15:03:48.000000 colourmap-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4008 2022-10-18 11:43:57.675200 colourmap-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3433 2022-04-03 09:21:03.000000 colourmap-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-18 11:43:57.666196 colourmap-1.1.9/colourmap/
+-rw-rw-rw-   0        0        0      751 2022-10-18 11:43:15.000000 colourmap-1.1.9/colourmap/__init__.py
+-rw-rw-rw-   0        0        0     9782 2022-10-18 11:42:22.000000 colourmap-1.1.9/colourmap/colourmap.py
+-rw-rw-rw-   0        0        0     1254 2022-04-04 19:37:17.000000 colourmap-1.1.9/colourmap/examples.py
+drwxrwxrwx   0        0        0        0 2022-10-18 11:43:57.675200 colourmap-1.1.9/colourmap.egg-info/
+-rw-rw-rw-   0        0        0     4008 2022-10-18 11:43:57.000000 colourmap-1.1.9/colourmap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2022-10-18 11:43:57.000000 colourmap-1.1.9/colourmap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-18 11:43:57.000000 colourmap-1.1.9/colourmap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2022-10-18 11:43:57.000000 colourmap-1.1.9/colourmap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-10-18 11:43:57.000000 colourmap-1.1.9/colourmap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      262 2022-10-18 11:43:57.677167 colourmap-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2022-03-11 12:58:41.000000 colourmap-1.1.9/setup.py
```

### Comparing `colourmap-1.1.8/LICENSE` & `colourmap-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `colourmap-1.1.8/PKG-INFO` & `colourmap-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: colourmap
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python package colourmap generates an N unique colors from the specified input colormap.
 Home-page: https://erdogant.github.io/colourmap
+Download-URL: https://github.com/erdogant/colourmap/archive/1.1.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/colourmap/archive/1.1.8.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -103,9 +101,7 @@
 <hr>
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * For citations, please use the citation at the right side panel.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: colourmap Version: 1.1.8 Summary: Python package
+Metadata-Version: 2.1 Name: colourmap Version: 1.1.9 Summary: Python package
 colourmap generates an N unique colors from the specified input colormap. Home-
-page: https://erdogant.github.io/colourmap Author: Erdogan Taskesen Author-
-email: erdogant@gmail.com License: UNKNOWN Download-URL: https://github.com/
-erdogant/colourmap/archive/1.1.8.tar.gz Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # colourmap [!
-[Python](https://img.shields.io/pypi/pyversions/colourmap)](https://
-img.shields.io/pypi/pyversions/colourmap) [![PyPI Version](https://
-img.shields.io/pypi/v/colourmap)](https://pypi.org/project/colourmap/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/colourmap/blob/master/LICENSE) [![Github Forks](https://
-img.shields.io/github/forks/erdogant/colourmap.svg)](https://github.com/
-erdogant/colourmap/network) [![GitHub Open Issues](https://img.shields.io/
-github/issues/erdogant/colourmap.svg)](https://github.com/erdogant/colourmap/
-issues) [![Project Status](http://www.repostatus.org/badges/latest/active.svg)]
-(http://www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/
-colourmap/month)](https://pepy.tech/project/colourmap/month) [![Downloads]
-(https://pepy.tech/badge/colourmap)](https://pepy.tech/project/colourmap) [!
-[Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+page: https://erdogant.github.io/colourmap Download-URL: https://github.com/
+erdogant/colourmap/archive/1.1.9.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # colourmap [![Python](https://img.shields.io/pypi/
+pyversions/colourmap)](https://img.shields.io/pypi/pyversions/colourmap) [!
+[PyPI Version](https://img.shields.io/pypi/v/colourmap)](https://pypi.org/
+project/colourmap/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/colourmap/blob/master/LICENSE) [!
+[Github Forks](https://img.shields.io/github/forks/erdogant/colourmap.svg)]
+(https://github.com/erdogant/colourmap/network) [![GitHub Open Issues](https://
+img.shields.io/github/issues/erdogant/colourmap.svg)](https://github.com/
+erdogant/colourmap/issues) [![Project Status](http://www.repostatus.org/badges/
+latest/active.svg)](http://www.repostatus.org/#active) [![Downloads](https://
+pepy.tech/badge/colourmap/month)](https://pepy.tech/project/colourmap/month) [!
+[Downloads](https://pepy.tech/badge/colourmap)](https://pepy.tech/project/
+colourmap) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
 erdogant.github.io/colourmap/)   *`` Colourmap`` generates an unique lit of RGB
 and HEX colors for the specified input list. # **â­ï¸ Star this repo if you
 like it â­ï¸** # ### [Documentation pages](https://erdogant.github.io/
 colourmap/) On the [documentation pages](https://erdogant.github.io/colourmap/
 ) you can find more information about ``colourmap`` with examples. # #####
 Install colourmap from PyPI ```bash pip install colourmap # normal install pip
 install -U colourmap # update if needed ``` ### Import colourmap package
```

### Comparing `colourmap-1.1.8/README.md` & `colourmap-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `colourmap-1.1.8/colourmap/__init__.py` & `colourmap-1.1.9/colourmap/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     rgb2hex,
     hex2rgb,
     hex2rgba,
 )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 
 
 # module level doc-string
 __doc__ = """
 **colourmap**
 =====================================================================
```

### Comparing `colourmap-1.1.8/colourmap/colourmap.py` & `colourmap-1.1.9/colourmap/colourmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         Method to generate colors
         'matplotlib' (default)
         'seaborn'
     scheme : String, optional
         The output of color is in the scheme:
         'rgb'
         'hex'
+    verbose : int, optional
+        Print progress to screen. The default is 3.
+        0: None, 1: ERROR, 2: WARN, 3: INFO (default), 4: DEBUG, 5: TRACE
 
     References
     ----------
     Colormap: https://matplotlib.org/examples/color/colormaps_reference.html
 
     Returns
     -------
@@ -55,15 +58,16 @@
     else:
         listlen=3
 
     if method=='seaborn':
         sns = _check_seaborn()
         color_list = sns.color_palette(cmap, N)
     else:
-        base = plt.cm.get_cmap(cmap)
+        # base = plt.cm.get_cmap(cmap)
+        base = matplotlib.colormaps[cmap]
         color_list = base(np.linspace(0, 1, N))[:, 0:listlen].tolist()
         # If there are not enough colors in the cmap, use the seaborn method.
         uicolors = len(np.unique(rgb2hex(color_list)))
         if uicolors != N:
             if verbose>=2: print('[colourmap]> Warning: Colormap [%s] can not create [%d] unique colors! Available unique colors: [%d].' %(cmap, N, uicolors))
 
     # Set the output coloring scheme
@@ -196,15 +200,15 @@
 
     """
     # Pass 16 to the integer function for change of base
     return [int(c_hex[i:i + 2], 16) for i in range(1, 6, 2)]
 
 
 # %%
-def fromlist(y, cmap='Set1', gradient=None, method='matplotlib', scheme='rgb'):
+def fromlist(y, cmap='Set1', gradient=None, method='matplotlib', scheme='rgb', verbose=3):
     """Generate colors from input list.
 
     Description
     ------------
     This function creates unique colors based on the input list y and the cmap.
     When the gradient hex color is defined, such as '#000000', a gradient coloring space is created between two colors.
         The start color of the particular y, using the cmap and
@@ -223,14 +227,17 @@
         Method to generate colors
         'matplotlib' (default)
         'seaborn'
     scheme : String, optional
         The output of color is in the scheme:
         'rgb'
         'hex'
+    verbose : int, optional
+        Print progress to screen. The default is 3.
+        0: None, 1: ERROR, 2: WARN, 3: INFO (default), 4: DEBUG, 5: TRACE
 
     Returns
     -------
     tuple containing:
         List of colors in the same order as y.
         dict for the unique colors
 
@@ -244,15 +251,15 @@
     uiy = np.unique(y)
 
     # Get unique categories without sort
     # indexes = np.unique(y, return_index=True)[1]
     # uiy = [y[index] for index in sorted(indexes)]
 
     # Get colors
-    colors_unique = generate(len(uiy), cmap=cmap, method=method, scheme=scheme)
+    colors_unique = generate(len(uiy), cmap=cmap, method=method, scheme=scheme, verbose=verbose)
 
     # Make dict for each search
     colordict = dict(zip(uiy, colors_unique))
 
     # Color using density and the gradient.
     if gradient is not None:
         # Set the scheme
```

### Comparing `colourmap-1.1.8/colourmap/examples.py` & `colourmap-1.1.9/colourmap/examples.py`

 * *Files identical despite different names*

### Comparing `colourmap-1.1.8/colourmap.egg-info/PKG-INFO` & `colourmap-1.1.9/colourmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: colourmap
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python package colourmap generates an N unique colors from the specified input colormap.
 Home-page: https://erdogant.github.io/colourmap
+Download-URL: https://github.com/erdogant/colourmap/archive/1.1.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/colourmap/archive/1.1.8.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -103,9 +101,7 @@
 <hr>
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * For citations, please use the citation at the right side panel.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: colourmap Version: 1.1.8 Summary: Python package
+Metadata-Version: 2.1 Name: colourmap Version: 1.1.9 Summary: Python package
 colourmap generates an N unique colors from the specified input colormap. Home-
-page: https://erdogant.github.io/colourmap Author: Erdogan Taskesen Author-
-email: erdogant@gmail.com License: UNKNOWN Download-URL: https://github.com/
-erdogant/colourmap/archive/1.1.8.tar.gz Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # colourmap [!
-[Python](https://img.shields.io/pypi/pyversions/colourmap)](https://
-img.shields.io/pypi/pyversions/colourmap) [![PyPI Version](https://
-img.shields.io/pypi/v/colourmap)](https://pypi.org/project/colourmap/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/colourmap/blob/master/LICENSE) [![Github Forks](https://
-img.shields.io/github/forks/erdogant/colourmap.svg)](https://github.com/
-erdogant/colourmap/network) [![GitHub Open Issues](https://img.shields.io/
-github/issues/erdogant/colourmap.svg)](https://github.com/erdogant/colourmap/
-issues) [![Project Status](http://www.repostatus.org/badges/latest/active.svg)]
-(http://www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/
-colourmap/month)](https://pepy.tech/project/colourmap/month) [![Downloads]
-(https://pepy.tech/badge/colourmap)](https://pepy.tech/project/colourmap) [!
-[Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+page: https://erdogant.github.io/colourmap Download-URL: https://github.com/
+erdogant/colourmap/archive/1.1.9.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # colourmap [![Python](https://img.shields.io/pypi/
+pyversions/colourmap)](https://img.shields.io/pypi/pyversions/colourmap) [!
+[PyPI Version](https://img.shields.io/pypi/v/colourmap)](https://pypi.org/
+project/colourmap/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/colourmap/blob/master/LICENSE) [!
+[Github Forks](https://img.shields.io/github/forks/erdogant/colourmap.svg)]
+(https://github.com/erdogant/colourmap/network) [![GitHub Open Issues](https://
+img.shields.io/github/issues/erdogant/colourmap.svg)](https://github.com/
+erdogant/colourmap/issues) [![Project Status](http://www.repostatus.org/badges/
+latest/active.svg)](http://www.repostatus.org/#active) [![Downloads](https://
+pepy.tech/badge/colourmap/month)](https://pepy.tech/project/colourmap/month) [!
+[Downloads](https://pepy.tech/badge/colourmap)](https://pepy.tech/project/
+colourmap) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
 erdogant.github.io/colourmap/)   *`` Colourmap`` generates an unique lit of RGB
 and HEX colors for the specified input list. # **â­ï¸ Star this repo if you
 like it â­ï¸** # ### [Documentation pages](https://erdogant.github.io/
 colourmap/) On the [documentation pages](https://erdogant.github.io/colourmap/
 ) you can find more information about ``colourmap`` with examples. # #####
 Install colourmap from PyPI ```bash pip install colourmap # normal install pip
 install -U colourmap # update if needed ``` ### Import colourmap package
```

### Comparing `colourmap-1.1.8/setup.py` & `colourmap-1.1.9/setup.py`

 * *Files identical despite different names*

