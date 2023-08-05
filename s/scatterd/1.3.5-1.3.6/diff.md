# Comparing `tmp/scatterd-1.3.5.tar.gz` & `tmp/scatterd-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatterd-1.3.5.tar", last modified: Sun May 28 21:15:12 2023, max compression
+gzip compressed data, was "scatterd-1.3.6.tar", last modified: Sat Aug  5 18:24:35 2023, max compression
```

## Comparing `scatterd-1.3.5.tar` & `scatterd-1.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:15:12.035347 scatterd-1.3.5/
--rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.5/LICENSE
--rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4994 2023-05-28 21:15:12.036345 scatterd-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:15:12.010876 scatterd-1.3.5/scatterd/
--rw-rw-rw-   0        0        0     1831 2023-05-28 18:52:48.000000 scatterd-1.3.5/scatterd/__init__.py
--rw-rw-rw-   0        0        0     7314 2023-05-27 20:14:36.000000 scatterd-1.3.5/scatterd/examples.py
--rw-rw-rw-   0        0        0    21289 2023-05-28 20:59:17.000000 scatterd-1.3.5/scatterd/scatterd.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:15:12.034350 scatterd-1.3.5/scatterd.egg-info/
--rw-rw-rw-   0        0        0     4994 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 21:15:11.000000 scatterd-1.3.5/scatterd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2023-05-28 21:15:12.051439 scatterd-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-05-27 20:51:23.000000 scatterd-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:24:35.275741 scatterd-1.3.6/
+-rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4994 2023-08-05 18:24:35.275741 scatterd-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 18:24:35.267788 scatterd-1.3.6/scatterd/
+-rw-rw-rw-   0        0        0     1859 2023-08-05 17:58:33.000000 scatterd-1.3.6/scatterd/__init__.py
+-rw-rw-rw-   0        0        0     7410 2023-08-05 18:17:10.000000 scatterd-1.3.6/scatterd/examples.py
+-rw-rw-rw-   0        0        0    22466 2023-08-05 18:24:00.000000 scatterd-1.3.6/scatterd/scatterd.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:24:35.274742 scatterd-1.3.6/scatterd.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-08-05 18:24:35.000000 scatterd-1.3.6/scatterd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-08-05 18:24:35.000000 scatterd-1.3.6/scatterd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:24:35.000000 scatterd-1.3.6/scatterd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-08-05 18:24:35.000000 scatterd-1.3.6/scatterd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 18:24:35.000000 scatterd-1.3.6/scatterd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-08-05 18:24:35.280728 scatterd-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1420 2023-08-05 17:57:13.000000 scatterd-1.3.6/setup.py
```

### Comparing `scatterd-1.3.5/LICENSE` & `scatterd-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.5/PKG-INFO` & `scatterd-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.5
+Version: 1.3.6
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.5.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.5 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.6 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.6.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.5/README.md` & `scatterd-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.5/scatterd/__init__.py` & `scatterd-1.3.6/scatterd/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from scatterd.scatterd import scatterd, import_example, set_colors, _preprocessing, jitter_func, normalize_between_0_and_1
+from scatterd.scatterd import scatterd, set_colors, _preprocessing, jitter_func, normalize_between_0_and_1
+from datazets import get as import_example
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.3.5'
+__version__ = '1.3.6'
 
 # module level doc-string
 __doc__ = """
 scatterd
 =====================================================================
 
 Scatterd is an easy and fast way of creating beautiful scatter plots.
```

### Comparing `scatterd-1.3.5/scatterd/examples.py` & `scatterd-1.3.6/scatterd/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from scatterd import scatterd, import_example
 import numpy as np
 
 # %%
-from scatterd import scatterd
-
-# %%
-
-df = import_example()
+df = import_example(data='cancer', verbose='info')
 fig, ax = scatterd(df['tsneX'],
                    df['tsneY'],
                    labels=df['labx'],
+                   verbose='info',
                    )
 
 # %%
 from scatterd import scatterd, import_example
-df = import_example()
+df = import_example(data='cancer', verbose='warning')
 fig, ax = scatterd(df['tsneX'],
                    df['tsneY'],
                    labels=df['labx'],
                    density=True,
                    density_on_top=False,
                     # args_density={'alpha': 0.3},
                     gradient='opaque',
                     # gradient='#FFFFFF',
                    edgecolor='#000000',
                    grid=True,
                    fontweight='normal',
                    fontsize=26,
                    legend=2,
+                   verbose='info',
                    )
 
 # %%
 # X, y = make_friedman1(n_samples=100000, n_features=5, random_state=0)
 # fig, ax = scatterd(X[:,0], X[:,1], density=False, s=0)
 
 
@@ -58,16 +56,16 @@
 from sklearn import datasets
 iris = datasets.load_iris()
 X = iris.data[:, :2]  # we only take the first two features.
 labels = iris.target
 
 import colourmap
 c=colourmap.fromlist(labels)[0]
-c[0]=[0,0,0]
-c[1]=[0,0,0]
+c[0]=[0,0,0,0]
+c[1]=[0,0,0,0]
 s = (labels+1) * 200
 random_integers = np.random.randint(0, len(s), size=X.shape[0])
 alpha = np.random.rand(1, X.shape[0])[0][random_integers]
 
 # %%
 from scatterd import scatterd
 import matplotlib as mpl
```

### Comparing `scatterd-1.3.5/scatterd/scatterd.py` & `scatterd-1.3.6/scatterd/scatterd.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,24 @@
 
 # %% Libraries
 import colourmap
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
-import requests
-import os
-from urllib.parse import urlparse
+import logging
+
+logger = logging.getLogger('')
+[logger.removeHandler(handler) for handler in logger.handlers[:]]
+console = logging.StreamHandler()
+formatter = logging.Formatter('[scatterd] >%(levelname)s> %(message)s')
+console.setFormatter(formatter)
+logger.addHandler(console)
+logger = logging.getLogger(__name__)
+
 
 # %% Main
 def scatterd(x,
              y,
              z=None,
              s=150,
              c=[0, 0.1, 0.4],
@@ -38,15 +45,15 @@
              legend=None,
              jitter=None,
              xlabel='x-axis', ylabel='y-axis', title='', fontsize=24, fontcolor=None, grid=True, fontweight='normal',
              args_density = {'cmap': 'Reds', 'fill': True, 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False},
              visible=True,
              fig=None,
              ax=None,
-             verbose=3):
+             verbose='info'):
     """Make scaterplot.
 
     Parameters
     ----------
     x : numpy array
         1D Coordinates x-axis.
     y : numpy array
@@ -129,14 +136,17 @@
         'Set1'       Discrete colors
     figsize : tuple, optional
         Figure size. The default is (15,10).
     visible : Bool, default: True
         Visible status of the Figure. When False, figure is created on the background.
     args_density : dict()
         Dictionary containing arguments for kernel density plotting.
+    verbose : int, (default: 'info')
+        Print progress to screen. The default is 'info'
+        60: None, 40: error, 30: warning, 20: info, 10: debug
 
     Returns
     -------
     Fig, ax
 
     Examples
     --------
@@ -175,14 +185,17 @@
     References
     -------
     * github: https://github.com/erdogant/scatterd
     * Documentation: https://erdogant.github.io/scatterd/
     * Colormap: https://matplotlib.org/examples/color/colormaps_reference.html
 
     """
+    # Set the logger
+    set_logger(verbose=verbose)
+
     if len(x)!=len(y): raise Exception('[scatterd] >Error: input parameter x should be the same size of y.')
     if isinstance(c, str): raise Exception('[scatterd] >Error: input parameter c(olors) should be RGB of type tuple [0,0,0] .')
     if not isinstance(s, int) and len(s)!=len(x): raise Exception('[scatterd] >Error: input parameter s(ize) should be of same size of X.')
     if (z is not None) and len(x)!=len(z): raise Exception('[scatterd] >Error: input parameter z should be the same size of x and y.')
     if s is None: s=0
     if c is None: s, c = 0, [0, 0, 0]
     if isinstance(s, (int, float)) and s==0: fontsize=0
@@ -191,41 +204,44 @@
     # Defaults
     defaults_density = {'cmap': 'Reds', 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False, 'fill': True}
     args_density = {**defaults_density, **args_density}
 
     # Preprocessing
     X, labels = _preprocessing(x, y, z, labels, jitter, norm)
     # Set color
-    c_rgb, opaque = set_colors(X, labels, c, cmap, gradient=gradient, opaque_type=opaque_type, verbose=verbose)
+    c_rgb, opaque = set_colors(X, labels, c, cmap, gradient=gradient, opaque_type=opaque_type)
     # Set fontcolor
-    fontcolor = set_fontcolor(fontcolor, labels, X, cmap, verbose=2)
+    fontcolor = set_fontcolor(fontcolor, labels, X, cmap)
     # Set size
     s = set_size(X, s)
     # Set size
-    alpha = set_alpha(X, alpha, gradient, opaque, verbose)
+    alpha = set_alpha(X, alpha, gradient, opaque)
     # Set marker
     marker = set_marker(X, marker)
     # Bootup figure
     fig, ax = init_figure(ax, z, dpi, figsize, visible, fig)
     # Set figure properties
     ax = _set_figure_properties(X, labels, fontcolor, fontsize, xlabel, ylabel, title, grid, fontweight, zorder, ax)
 
     # Add density as bottom layer to the scatterplot
     if density:
+        logger.info('Add density layer')
         ax = sns.kdeplot(x=X[:, 0], y=X[:, 1], ax=ax, **args_density)
 
     # Scatter all at once
     if (labels is None) and isinstance(marker, str):
+        logger.info('Create scatterplot (fast)')
         # Do not try to plot legend.
         legend = -1
         if z is None:
             ax.scatter(X[:, 0], X[:, 1], c=c_rgb, s=s, edgecolor=edgecolor, marker=marker, alpha=alpha, zorder=zorder)
         else:
             ax.scatter(X[:, 0], X[:, 1], X[:, 2], s=s, c=c_rgb, edgecolor=edgecolor, marker=marker, alpha=alpha, zorder=zorder)
     else:
+        logger.info('Create scatterplot')
         uilabels = np.unique(labels)
         for label in uilabels:
             Iloc1 = label==labels
             # Extract the unique markers
             for m in np.unique(marker[Iloc1]):
                 Iloc2 = np.logical_and(Iloc1, m==marker)
                 if z is None:
@@ -280,38 +296,40 @@
             # if isinstance(child, matplotlib.spines.Spine):
                 # child.set_color(grid)
 
     return ax
 
 
 # %% Setup colors
-def set_colors(X, labels, c, cmap='tab20c', gradient=None, opaque_type='per_class', verbose=3):
+def set_colors(X, labels, c, cmap='tab20c', gradient=None, opaque_type='per_class', verbose=None):
     """Set colors."""
+    # Set the logger
+    if verbose is not None: set_logger(verbose=verbose)
     if c is None: return None
 
     # The default is all dots to black
     c_rgb = np.repeat([0, 0, 0], X.shape[0], axis=0).reshape(-1, 3)
     # Create opaque levels
     opaque = np.array([1.0] * X.shape[0])
 
     # Change on input c
     if len(c)==1 and isinstance(c, list): c = c[0]
     if len(c)==3 and isinstance(c[0], (int, float)):
-        if verbose>=4: print('[scatterd] >Colors are all set to %s.' %(c))
+        logger.debug('Colors are all set to %s.' %(c))
         c_rgb = np.repeat([c], X.shape[0], axis=0).reshape(-1, 3)
 
     if X.shape[0]==len(c):
-        if verbose>=4: print('[scatterd] >Colors are set to input colors defined in [c].')
+        logger.debug('Colors are set to input colors defined in [c].')
         c_rgb=c
 
     if labels is not None:
         # Create unqiue colors for labels if there are multiple classes or in case cmap and gradient is used.
-        if verbose>=4: print('[scatterd] >Colors are based on the input [labels] and on [cmap].')
+        logger.debug('Colors are based on the input [labels] and on [cmap].')
         if labels is None: labels = np.repeat(0, X.shape[0])
-        c_rgb = colourmap.fromlist(labels, X=X, cmap=cmap, scheme='rgb', method='matplotlib', gradient=gradient, opaque_type=opaque_type)[0]
+        c_rgb = colourmap.fromlist(labels, X=X, cmap=cmap, scheme='rgb', method='matplotlib', gradient=gradient, opaque_type=opaque_type, verbose=verbose)[0]
         # Add extra column with transparancy
         if gradient=='opaque' and c_rgb.shape[1]==4:
             # Set the minimum transparancy level at 0.1
             opaque = np.maximum(c_rgb[:, -1], 0.1)
             c_rgb = c_rgb[:, :3]
 
     # Return
@@ -371,37 +389,39 @@
     x_min, x_max = np.min(X, 0), np.max(X, 0)
     out = (X - x_min) / (x_max - x_min)
     out[np.isnan(out)]=1
     return out
 
 
 # %% Fontcolor
-def set_fontcolor(fontcolor, label, X, cmap, verbose=3):
-    if (fontcolor is not None) and colourmap.is_hex_color(fontcolor, verbose=0):
+def set_fontcolor(fontcolor, label, X, cmap, verbose=None):
+    # Set the logger
+    if verbose is not None: set_logger(verbose=verbose)
+    if (fontcolor is not None) and colourmap.is_hex_color(fontcolor, verbose=get_logger()):
         fontcolor = colourmap.hex2rgb(fontcolor)
 
     # Set font colors
     if (fontcolor is None) and (label is None):
         # fontcolor = {np.unique(label)[0]: [0, 0, 0]}
         pass
     elif (fontcolor is None) and (len(np.unique(label))==1):
         pass
     elif (fontcolor is not None) and (len(fontcolor)==3 or len(fontcolor)==1):
         fontcolor_dict = {}
         for lab in np.unique(label):
             fontcolor_dict[lab]=fontcolor
         fontcolor=fontcolor_dict
     elif (fontcolor is not None) and (label is None):
-        if verbose>=2: print('[scatterd] >Warning : Without label, there is no font(color) to print.')
+        logger.warning('Without label, there is no font(color) to print.')
     elif (fontcolor is None) and (label is not None):
-        _, fontcolor = colourmap.fromlist(label, cmap=cmap, method='matplotlib')
+        _, fontcolor = colourmap.fromlist(label, cmap=cmap, method='matplotlib', verbose=get_logger())
     elif (fontcolor is not None) and (label is not None) and (len(fontcolor)==X.shape[0]):
-        _, fontcolor = colourmap.fromlist(fontcolor, cmap=cmap, method='matplotlib')
+        _, fontcolor = colourmap.fromlist(fontcolor, cmap=cmap, method='matplotlib', verbose=get_logger())
     elif (fontcolor is not None) and (label is not None) and ((isinstance(fontcolor[0], int)) or (isinstance(fontcolor[0], float))):
-        _, tmpcolors = colourmap.fromlist(label, cmap=cmap, method='matplotlib')
+        _, tmpcolors = colourmap.fromlist(label, cmap=cmap, method='matplotlib', verbose=get_logger())
         # list(map(lambda x: tmpcolors.update({x: fontcolor}), [*tmpcolors.keys()]))
         fontcolor = tmpcolors
     else:
         raise Exception('[scatterd] >ERROR : fontcolor input is not correct.')
 
     return fontcolor
 
@@ -410,21 +430,23 @@
     """Set size."""
     if isinstance(s, (int, float)): s = np.repeat(s, X.shape[0])
     # Minimum size should be 0 (dots will not be showed)
     s = np.maximum(s, 0)
     return s
 
 
-def set_alpha(X, alpha, gradient, opaque, verbose):
+def set_alpha(X, alpha, gradient, opaque, verbose=None):
     """Set alpha."""
+    # Set the logger
+    if verbose is not None: set_logger(verbose=verbose)
     if alpha is None: alpha=0.8
     if isinstance(alpha, (int, float)):
         alpha = np.repeat(alpha, X.shape[0])
     if gradient=='opaque':
-        if verbose>=3: print('[scatterd]> Set alpha based on density because of the parameter: [%s]' %(gradient))
+        logger.info('Set alpha based on density because of the parameter: [%s]' %(gradient))
         alpha = opaque
     # Minimum size should be 0 (dots will not be showed)
     alpha = np.maximum(alpha, 0)
     return alpha
 
 
 def set_marker(X, marker):
@@ -459,91 +481,94 @@
 
     if fig is not None:
         fig.set_visible(visible)
 
     return fig, ax
 
 
-# %% Import example dataset from github.
-def import_example(data='cancer', url=None, sep=',', verbose=3):
-    """Import example dataset from github source.
-
-    Description
-    -----------
-    Import one of the few datasets from github source or specify your own download url link.
-
-    Parameters
-    ----------
-    data : str
-        Name of datasets: 'cancer'
-    url : str
-        url link to to dataset.
-    verbose : int, (default: 3)
-
-    Returns
-    -------
-    pd.DataFrame()
-        Dataset containing mixed features.
-
-    """
-    import pandas as pd
-
-    if url is None:
-        url='https://erdogant.github.io/datasets/cancer_dataset.zip'
+# %%
+def convert_verbose_to_new(verbose):
+    """Convert old verbosity to the new."""
+    # In case the new verbosity is used, convert to the old one.
+    if verbose is None: verbose=0
+    if not isinstance(verbose, str) and verbose<10:
+        status_map = {
+            'None': 'silent',
+            0: 'silent',
+            6: 'silent',
+            1: 'critical',
+            2: 'warning',
+            3: 'info',
+            4: 'debug',
+            5: 'debug'}
+        if verbose>=2: print('[scatterd]> WARNING use the standardized verbose status. The status [1-6] will be deprecated in future versions.')
+        return status_map.get(verbose, 0)
     else:
-        data = wget.filename_from_url(url)
+        return verbose
 
-    if url is None:
-        if verbose>=3: print('Nothing to download.')
-        return None
-
-    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    filename = os.path.basename(urlparse(url).path)
-    PATH_TO_DATA = os.path.join(curpath, filename)
-    if not os.path.isdir(curpath):
-        os.makedirs(curpath, exist_ok=True)
-
-    # Check file exists.
-    if not os.path.isfile(PATH_TO_DATA):
-        if verbose>=3: print('Downloading [%s] dataset from github source..' %(data))
-        wget(url, PATH_TO_DATA)
 
-    # Import local dataset
-    if verbose>=3: print('Import dataset [%s]' %(data))
-
-    df = pd.read_csv(PATH_TO_DATA, sep=sep)
-    # Return
-    return df
+# %%
+def get_logger():
+    return logger.getEffectiveLevel()
 
 
-# %% Download files from github source
-def wget(url, writepath):
-    """Retrieve file from url.
+# %%
+def set_logger(verbose: [str, int] = 'info'):
+    """Set the logger for verbosity messages.
 
     Parameters
     ----------
-    url : str.
-        Internet source.
-    writepath : str.
-        Directory to write the file.
+    verbose : [str, int], default is 'info' or 20
+        Set the verbose messages using string or integer values.
+        * [0, 60, None, 'silent', 'off', 'no']: No message.
+        * [10, 'debug']: Messages from debug level and higher.
+        * [20, 'info']: Messages from info level and higher.
+        * [30, 'warning']: Messages from warning level and higher.
+        * [50, 'critical']: Messages from critical level and higher.
 
     Returns
     -------
     None.
 
-    Example
-    -------
-    >>> import clustimage as cl
-    >>> images = cl.wget('https://erdogant.github.io/datasets/flower_images.zip', 'c://temp//flower_images.zip')
+    > # Set the logger to warning
+    > set_logger(verbose='warning')
+    > # Test with different messages
+    > logger.debug("Hello debug")
+    > logger.info("Hello info")
+    > logger.warning("Hello warning")
+    > logger.critical("Hello critical")
 
     """
-    r = requests.get(url, stream=True)
-    with open(writepath, "wb") as fd:
-        for chunk in r.iter_content(chunk_size=1024):
-            fd.write(chunk)
+    # Set 0 and None as no messages.
+    if (verbose==0) or (verbose is None):
+        verbose=60
+    # Convert to verbose
+    verbose = convert_verbose_to_new(verbose)
+    # Convert str to levels
+    if isinstance(verbose, str):
+        levels = {'silent': 60,
+                  'off': 60,
+                  'no': 60,
+                  'debug': 10,
+                  'info': 20,
+                  'warning': 30,
+                  'error': 50,
+                  'critical': 50}
+        verbose = levels[verbose]
+
+    # Show examples
+    logger.setLevel(verbose)
+    logger.debug('Set verbose to %s' %(verbose))
+
+
+# %%
+def disable_tqdm():
+    """Set the logger for verbosity messages."""
+    return (True if (logger.getEffectiveLevel()>=30) else False)
+
 
 # %% Density
 # def coord2density(X, kernel='gaussian', metric='euclidean', ax=None, visible=False):
 #     from sklearn.neighbors import KernelDensity
 
 #     kde = KernelDensity(kernel=kernel, metric=metric, bandwidth=0.2).fit(X)
 #     dens = kde.score_samples(X)
```

### Comparing `scatterd-1.3.5/scatterd.egg-info/PKG-INFO` & `scatterd-1.3.6/scatterd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.5
+Version: 1.3.6
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.5.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.5 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.6 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.6.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.5/setup.py` & `scatterd-1.3.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE))
 
 #--------  Create setup file    
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-     install_requires=['matplotlib','numpy','colourmap>=1.1.13','seaborn','requests'],
+     install_requires=['matplotlib','numpy','colourmap>=1.1.16','seaborn', 'datazets'],
      python_requires='>=3',
      name='scatterd',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="scatterd is an easy and fast way of creating scatter plots.",
      long_description=long_description,
```

