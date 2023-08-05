# Comparing `tmp/codedapertures-0.7.1.tar.gz` & `tmp/codedapertures-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.7.1.tar", last modified: Wed Aug  2 01:31:18 2023, max compression
+gzip compressed data, was "codedapertures-0.8.tar", last modified: Sat Aug  5 01:53:44 2023, max compression
```

## Comparing `codedapertures-0.7.1.tar` & `codedapertures-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-08-02 01:31:18.275516 codedapertures-0.7.1/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.7.1/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      722 2023-08-02 01:31:18.275410 codedapertures-0.7.1/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)     2041 2023-07-29 01:49:47.000000 codedapertures-0.7.1/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-08-02 01:31:18.274504 codedapertures-0.7.1/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.7.1/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)    32071 2023-08-02 01:26:33.000000 codedapertures-0.7.1/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-08-02 01:31:18.275256 codedapertures-0.7.1/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      722 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.7.1/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       40 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-08-02 01:31:18.275550 codedapertures-0.7.1/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      925 2023-08-02 01:29:51.000000 codedapertures-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:53:44.854621 codedapertures-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-05 01:53:35.000000 codedapertures-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-05 01:53:44.854621 codedapertures-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-05 01:53:35.000000 codedapertures-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:53:44.854621 codedapertures-0.8/codedapertures/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-05 01:53:35.000000 codedapertures-0.8/codedapertures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32221 2023-08-05 01:53:35.000000 codedapertures-0.8/codedapertures/codedapertures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:53:44.854621 codedapertures-0.8/codedapertures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-05 01:53:44.000000 codedapertures-0.8/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-05 01:53:44.000000 codedapertures-0.8/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:53:44.000000 codedapertures-0.8/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:53:44.000000 codedapertures-0.8/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 01:53:44.000000 codedapertures-0.8/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 01:53:44.000000 codedapertures-0.8/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:53:44.854621 codedapertures-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-05 01:53:35.000000 codedapertures-0.8/setup.py
```

### Comparing `codedapertures-0.7.1/LICENSE` & `codedapertures-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.7.1/PKG-INFO` & `codedapertures-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.7.1
+Version: 0.8
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.7.1/README.md` & `codedapertures-0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 # CodedApertures
 #### a python package for generating coded apertures  
 
 [![Downloads](https://static.pepy.tech/personalized-badge/codedapertures?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/codedapertures)
 
 CodedApertures is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
 
-New to coded apertures? Here's a nice article: https://www.paulcarlisle.net/codedaperture/
-
-PyPI URL: https://pypi.org/project/codedapertures/
+New to coded apertures? Here's a nice article: https://www.paulcarlisle.net/codedaperture/.
 
 ### Usage
 
-Install with PIP:
+Install from [PyPI](https://pypi.org/project/codedapertures/) with PIP:
 ```
 pip install codedapertures
 ```
 
+Coded patterns that this package can generate:
+
+| class | coded aperture |
+|---|---|
+| rand1d | random array (1D) |
+| rand2d | random array (2D) |
+| ura | uniformly redundant array |
+| mura | modified uniformly redundant array |
+| pnp | pseudo-noise product array |
+| randhex | random array (hexagonal) |
+| shura | skew-hadamard uniformly redundant array |
+| hura | hexagonal uniformly redundant array |
+
+Note that for consistency with relevant decoding algorithms, we define the
+binary meaning as such
+| val | mask pixel |
+|---|---|
+| 0 | closed |
+| 1 | open |
+
 See [demo.ipynb](https://github.com/bpops/codedapertures/blob/master/demo.ipynb) for examples of use.
 
 ### Credits
 
 URA pattern: E. E. Fenimore and T. M. Cannon, "Coded aperture imaging with uniformly redundant arrays," Appl. Opt. 17, 337-347 (1978).
 
 MURA pattern:  E.E. Fenimore and S. R. Gottesman, "New family of binary arrays for coded aperture imaging" Appl. Opt. 28 (20): 4344-4352 (1989).
```

### Comparing `codedapertures-0.7.1/codedapertures/codedapertures.py` & `codedapertures-0.8/codedapertures/codedapertures.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from   commpy             import pnsequence
 import numpy              as     np
 import matplotlib.pyplot  as     plt
 from   matplotlib.patches import RegularPolygon
 import pyprimes
 import random
+from   scipy.signal       import correlate2d
 
 
 class mask_sq():
     """
     Mask
 
     Holds one of several types of square coded aperture patterns.
@@ -50,33 +51,32 @@
         -------
         A_ij : ndarrray
             the 2D boolean mask
         """
         mask = 1-self.A_ij if inverse else self.A_ij
         return mask
 
-    def add_border(self, width, empty=False):
+    def add_border(self, width):
         """
         Adds a border with the given width
 
         Parameters
         ----------
         width : int
             width of border
         """
         
         new_width  = self.width  + width*2
         new_height = self.height + width*2
         new_mask   = np.zeros((new_width, new_height))
-        if not empty: new_mask = new_mask +1
         new_mask[width:-width,width:-width] = self.A_ij
         self.A_ij  = new_mask
 
 
-class rand_1d(mask_sq):
+class rand1d(mask_sq):
     """
     Random 1-dimensional Array
 
     Parameters
     ----------
     x : int
         number of 'x' elements in the array
@@ -90,20 +90,20 @@
     
     def __init__(self, x=10, y=10, fill=0.5, quiet=False):
         self.r = x
         self.s = y
         self.fill = fill
         
         # randomly fill
-        A_ij = np.zeros([self.r, self.s])
+        A_ij = np.zeros([self.r, self.s])+1
         for i in range(self.r):
             if random.random() < self.fill:
-                A_ij[i,:] = 1
+                A_ij[i,:] = 0
         self.A_ij = A_ij
-        self.actual_fill = np.sum(A_ij[:,0])/(self.r)
+        self.actual_fill = (self.r-np.sum(A_ij[:,0]))/(self.r)
         
         # get width/height
         self.width = self.A_ij.shape[0]
         self.height = self.A_ij.shape[1]
 
         if not quiet: self.report()
         
@@ -144,21 +144,21 @@
         ----------
         inverse : bool
             if True, will invert the array before plotting
         size : int
             size of the plot (default 8)
         """
         plt.rcParams['figure.figsize'] = [size,size]
-        cmap = "binary_r" if inverse else "binary"
+        cmap = "binary" if inverse else "binary_r"
         plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
         plt.axis('off')
         plt.title("Random 1D")
         plt.show()
 
-class rand_2d(mask_sq):
+class rand2d(mask_sq):
     """
     Random 2-dimensional Array
 
     Parameters
     ----------
     x : int
         number of 'x' elements in the array
@@ -172,21 +172,21 @@
     
     def __init__(self, x=10, y=10, fill=0.5, quiet=False):
         self.r = x
         self.s = y
         self.fill = fill
         
         # randomly fill
-        A_ij = np.zeros([self.r, self.s])
+        A_ij = np.zeros([self.r, self.s])+1
         for i in range(self.r):
             for j in range(self.s):
                 if random.random() < self.fill:
-                    A_ij[i,j] = 1
+                    A_ij[i,j] = 0
         self.A_ij = A_ij
-        self.actual_fill = np.sum(A_ij)/(self.r*self.s)
+        self.actual_fill = 1-np.sum(A_ij)/(self.r*self.s)
         
         # get width/height
         self.width = self.A_ij.shape[0]
         self.height = self.A_ij.shape[1]
 
         if not quiet: self.report()
         
@@ -207,15 +207,15 @@
         ----------
         inverse : bool
             if True, will invert the array before plotting
         size : int
             size of the plot (default 8)
         """
         plt.rcParams['figure.figsize'] = [size,size]
-        cmap = "binary_r" if inverse else "binary"
+        cmap = "binary" if inverse else "binary_r"
         plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
         plt.axis('off')
         plt.title("Random 2D")
         plt.show()
 
 class ura(mask_sq):
     """
@@ -232,15 +232,15 @@
     """
 
     def __init__(self, rank=4, mult=2, quiet=False):
         self.rank = rank
         self.mult = mult
         
         # get r, s
-        r, s = self.__get_prime_pairs(self.rank)
+        s, r = self.__get_prime_pairs(self.rank)
         self.r = r
         self.s = s
         
         # generate C_r(I)
         C_r_I = np.zeros(r) - 1
         C_s_J = np.zeros(s) - 1
         for x in range(1, r):
@@ -254,23 +254,26 @@
             for J in range(s):
                 if I == 0:
                     A_IJ[I,J] = 0
                 elif J == 0:
                     A_IJ[I,J] = 1
                 elif C_r_I[I] * C_s_J[J] == 1:
                     A_IJ[I,J] = 1
+                else:
+                    A_IJ[I,J] = 0
 
         # generate A_ij
         m = self.mult
         A_ij = np.zeros([m*r,m*s])
         for i in range(m*r):
             for j in range(m*s):
                 A_ij[i,j] = A_IJ[i%r,j%s]
         A_ij = np.roll(A_ij, int((r+1)/2), axis=0)
         A_ij = np.roll(A_ij, int((s+1)/2), axis=1)
+        A_ij = np.transpose(A_ij)
         self.A_ij = A_ij
         
         # get width/height
         self.width = self.A_ij.shape[0]
         self.height = self.A_ij.shape[1]
 
         if not quiet: self.report()
@@ -321,17 +324,16 @@
         ----------
         inverse : bool
             if True, will invert the array before plotting
         size : int
             size of the plot (default 8)
         """
         plt.rcParams['figure.figsize'] = [size,size]
-        cmap = "binary_r" if inverse else "binary"
+        cmap = "binary" if inverse else "binary_r"
         plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
-        plt.axis('off')
         plt.title("URA")
         plt.show()
 
 class mura(mask_sq):
     """
     Modified Uniformly Redundant Array
 
@@ -402,15 +404,15 @@
         ----------
         inverse : bool
             if True, will invert the array before plotting
         size : int
             size of the plot (default 8)
         """
         plt.rcParams['figure.figsize'] = [size,size]
-        cmap = "binary_r" if inverse else "binary"
+        cmap = "binary" if inverse else "binary_r"
         plt.imshow(np.transpose(self.A_ij), cmap=cmap, aspect=1)
         plt.axis('off')
         plt.title("MURA")
         plt.show()
 
 class shura():
     """
@@ -459,19 +461,19 @@
         for i in range(self.rx):
             for j in range(self.ry):
                 i_idx = i - self.radius
                 j_idx = j - self.radius
                 self.l[i,j] = (i_idx + self.r*j_idx) % self.v
 
         # calculate mask
-        self.mask = np.zeros(self.l.shape, dtype=np.int16)
+        self.mask = np.zeros(self.l.shape, dtype=np.int16)+1
         for i in range(self.mask.shape[0]):
             for j in range(self.mask.shape[1]):
                 if self.l[i,j] in self.D:
-                    self.mask[i,j] = 1
+                    self.mask[i,j] = 0
 
         # map to axial matrix
         for i in range(self.diam):
             for j in range(self.diam):
                 if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
                     self.axial_matrix[i,j] = self.mask[i,j]
                 else:
@@ -548,17 +550,17 @@
 
                 # recenter
                 x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
                 y -= (self.mask.shape[1] * 1/hex_vert)/2.0 - hex_vert/2.0
 
                 # add hexagon
                 if self.mask[x_i,y_i] == 1:
-                    facecolor='k'
-                else:
                     facecolor='w'
+                else:
+                    facecolor='k'
                 hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
                               orientation=np.radians(60), 
                                facecolor=facecolor, alpha=0.6, edgecolor='k')
                 ax.add_patch(hex)
 
                 # add label
                 if labels:
@@ -590,16 +592,16 @@
         hex_vert  = (hex_width)*(2.0/np.sqrt(3))
 
         # draw hexagon array
         for y in range(self.diam):
             row_width = self.diam - abs(self.radius-y)
             start_i   = np.max((self.radius-y,0))
             for x in range(row_width):
-                facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
-                alpha     = 0.9 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                facecolor = 'w' if self.axial_matrix[x+start_i,y] == 1 else 'k'
+                alpha     = 0.3 if self.axial_matrix[x+start_i,y] == 1 else 0.9
                 label     = self.l[x+start_i,y]
                 hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
                                       ((y-self.radius)*((3/2)*hex_vert/2.0))),
                                      numVertices=6, radius=hex_vert/2.0, 
                                      orientation=np.radians(60), 
                                      facecolor=facecolor, alpha=alpha,
                                      edgecolor='k')
@@ -659,19 +661,19 @@
         for i in range(self.rx):
             for j in range(self.ry):
                 i_idx = i - self.radius
                 j_idx = j - self.radius
                 self.l[i,j] = (i_idx + self.r*j_idx) % self.v
 
         # calculate mask
-        self.mask = np.zeros(self.l.shape, dtype=np.int16)
+        self.mask = np.zeros(self.l.shape, dtype=np.int16)+1
         for i in range(self.mask.shape[0]):
             for j in range(self.mask.shape[1]):
                 if self.l[i,j] in self.D:
-                    self.mask[i,j] = 1
+                    self.mask[i,j] = 0
 
         # map to axial matrix
         for i in range(self.diam):
             for j in range(self.diam):
                 if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
                     self.axial_matrix[i,j] = self.mask[i,j]
                 else:
@@ -762,17 +764,17 @@
 
                 # recenter
                 x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
                 y -= (self.mask.shape[1] * 1/hex_vert)/2.0 - hex_vert/2.0
 
                 # add hexagon
                 if self.mask[x_i,y_i] == 1:
-                    facecolor='k'
-                else:
                     facecolor='w'
+                else:
+                    facecolor='k'
                 hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
                               orientation=np.radians(60), 
                                facecolor=facecolor, alpha=0.6, edgecolor='k')
                 ax.add_patch(hex)
 
                 # add label
                 if labels:
@@ -804,16 +806,16 @@
         hex_vert  = (hex_width)*(2.0/np.sqrt(3))
 
         # draw hexagon array
         for y in range(self.diam):
             row_width = self.diam - abs(self.radius-y)
             start_i   = np.max((self.radius-y,0))
             for x in range(row_width):
-                facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
-                alpha     = 0.9 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                facecolor = 'w' if self.axial_matrix[x+start_i,y] == 1 else 'k'
+                alpha     = 0.3 if self.axial_matrix[x+start_i,y] == 1 else 0.9
                 label     = self.l[x+start_i,y]
                 hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
                                       ((y-self.radius)*((3/2)*hex_vert/2.0))),
                                      numVertices=6, radius=hex_vert/2.0, 
                                      orientation=np.radians(60), 
                                      facecolor=facecolor, alpha=alpha,
                                      edgecolor='k')
@@ -827,15 +829,15 @@
         # set axis limits
         plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
         plt.ylim(-self.radius,self.radius)
         plt.title(f"HURA [o:{self.v}, r:{self.r}]")
         plt.show()
             
 
-class rand_hex():
+class randhex():
     """
     Random Hexagonal Array
 
     Parameters
     ----------
     radius: int
         vertex-to-vertex radius of the array, minus half the pixel width
@@ -846,29 +848,29 @@
     """
     def __init__(self, radius=3, fill=0.5, quiet=False):
 
         # get/determine mask properties
         self.radius       = radius
         self.diam         = self.radius*2+1
         self.side_width   = radius + 1
-        self.axial_matrix = np.zeros((self.diam,self.diam))
+        self.axial_matrix = np.zeros((self.diam,self.diam))+1
         self.loc_matrix   = np.zeros((2,self.diam,self.diam))
         self.fill         = fill
 
         # generate mask pattern
         for i in range(self.diam):
             for j in range(self.diam):
                 if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
                     if random.random() < self.fill:
-                        self.axial_matrix[i,j] = 1
+                        self.axial_matrix[i,j] = 0
                 else:
                     self.axial_matrix[i,j] = np.nan
 
         # determine actual fill factor
-        self.actual_fill = np.sum(self.axial_matrix == 1) / np.sum(~np.isnan(self.axial_matrix))
+        self.actual_fill = 1- (np.sum(self.axial_matrix == 1) / np.sum(~np.isnan(self.axial_matrix)))
 
         # generate locations
         for i in range(self.diam):
             for j in range(self.diam):
                 if not np.isnan(self.axial_matrix[i,j]):
                     self.loc_matrix[0,i,j] = i*np.sqrt(3) - abs(j-self.radius)/2.0
                     self.loc_matrix[1,i,j] = -i + j
@@ -898,16 +900,16 @@
         hex_vert  = (hex_width)*(2.0/np.sqrt(3))
 
         # draw hexagon array
         for y in range(self.diam):
             row_width = self.diam - abs(self.radius-y)
             start_i   = np.max((self.radius-y,0))
             for x in range(row_width):
-                facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
-                alpha     = 0.6 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                facecolor = 'w' if self.axial_matrix[x+start_i,y] == 1 else 'k'
+                alpha     = 0.3 if self.axial_matrix[x+start_i,y] == 1 else 0.9
                 hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
                                       ((y-self.radius)*((3/2)*hex_vert/2.0))),
                                      numVertices=6, radius=hex_vert/2.0, 
                                      orientation=np.radians(60), 
                                      facecolor=facecolor, alpha=alpha,
                                      edgecolor='k')
                 ax.add_patch(hex)
@@ -975,16 +977,16 @@
         ----------
         inverse : bool
             if True, will invert the array before plotting
         size : int
             size of the plot (default 8)
         """
         plt.rcParams['figure.figsize'] = [size,size]
-        cmap = "binary_r" if inverse else "binary"
-        plt.imshow(self.mask, cmap="gray", origin='lower', aspect=1)
+        cmap = "binary" if inverse else "binary_r"
+        plt.imshow(self.mask, cmap=cmap, origin='lower', aspect=1)
         plt.axis('off')
         plt.title(f"Pseudo-Noise Product Array [m: {self.m}, n: {self.n}]")
         plt.show()
         
 
 def prim_poly(m):
     """
@@ -1048,8 +1050,15 @@
     while True:
         L = 4*m + 1
         if pyprimes.isprime(L):
             this_rank += 1
         if this_rank == rank:
             break
         m += 1
-    return L
+    return L
+
+def autocorrelate(array):
+    """
+    Performs auto correlation
+    """
+
+
```

### Comparing `codedapertures-0.7.1/codedapertures.egg-info/PKG-INFO` & `codedapertures-0.8/codedapertures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.7.1
+Version: 0.8
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.7.1/setup.py` & `codedapertures-0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import setuptools
 
 setuptools.setup(name='codedapertures',
-      version='0.7.1',
+      version='0.8',
       description='a python package for generating coded apertures',
       long_description='CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
       url='https://github.com/bpops/codedapertures',
       author='bpops',
       license='MIT',
       install_requires=['pyprimes',
-                'numpy',
-                'matplotlib',
-                'scikit-commpy'],
+                        'numpy',
+                        'matplotlib',
+                        'scikit-commpy',
+                        'scipy',],
       zip_safe=False)
```

