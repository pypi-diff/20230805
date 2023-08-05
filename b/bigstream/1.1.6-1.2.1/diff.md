# Comparing `tmp/bigstream-1.1.6.tar.gz` & `tmp/bigstream-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigstream-1.1.6.tar", last modified: Thu Aug  3 21:07:13 2023, max compression
+gzip compressed data, was "bigstream-1.2.1.tar", last modified: Sat Aug  5 00:26:47 2023, max compression
```

## Comparing `bigstream-1.1.6.tar` & `bigstream-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-03 21:07:01.677801 bigstream-1.1.6/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.6/LICENSE.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-08-03 21:07:01.676772 bigstream-1.1.6/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.6/README.md
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-03 21:07:01.651989 bigstream-1.1.6/bigstream/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/__init__.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40218 2023-07-31 23:04:13.000000 bigstream-1.1.6/bigstream/align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-25 16:20:10.000000 bigstream-1.1.6/bigstream/application_pipelines.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-31 21:53:33.000000 bigstream-1.1.6/bigstream/configure_irm.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/features.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/level_set.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/metrics.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16819 2023-07-31 22:57:06.000000 bigstream-1.1.6/bigstream/motion_correct.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22638 2023-08-03 21:05:07.000000 bigstream-1.1.6/bigstream/piecewise_align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.6/bigstream/piecewise_transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-08-01 18:43:55.000000 bigstream-1.1.6/bigstream/stitch.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14215 2023-07-31 22:47:55.000000 bigstream-1.1.6/bigstream/transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21985 2023-08-02 14:31:12.000000 bigstream-1.1.6/bigstream/utility.py
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-03 21:07:01.672164 bigstream-1.1.6/bigstream.egg-info/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-08-03 21:07:01.000000 bigstream-1.1.6/bigstream.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-08-03 21:07:01.679075 bigstream-1.1.6/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-08-03 21:06:40.000000 bigstream-1.1.6/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-05 00:26:35.268507 bigstream-1.2.1/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.2.1/LICENSE.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-08-05 00:26:35.267117 bigstream-1.2.1/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.2.1/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-05 00:26:35.244945 bigstream-1.2.1/bigstream/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.2.1/bigstream/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40218 2023-08-04 21:21:04.000000 bigstream-1.2.1/bigstream/align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-25 16:20:10.000000 bigstream-1.2.1/bigstream/application_pipelines.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-31 21:53:33.000000 bigstream-1.2.1/bigstream/configure_irm.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.2.1/bigstream/features.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.2.1/bigstream/level_set.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.2.1/bigstream/metrics.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16931 2023-08-04 23:06:59.000000 bigstream-1.2.1/bigstream/motion_correct.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22638 2023-08-04 19:57:05.000000 bigstream-1.2.1/bigstream/piecewise_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.2.1/bigstream/piecewise_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-08-01 18:43:55.000000 bigstream-1.2.1/bigstream/stitch.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14215 2023-07-31 22:47:55.000000 bigstream-1.2.1/bigstream/transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22417 2023-08-05 00:22:57.000000 bigstream-1.2.1/bigstream/utility.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-08-05 00:26:35.262526 bigstream-1.2.1/bigstream.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-08-05 00:26:34.000000 bigstream-1.2.1/bigstream.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-08-05 00:26:35.000000 bigstream-1.2.1/bigstream.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-08-05 00:26:34.000000 bigstream-1.2.1/bigstream.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-08-05 00:26:34.000000 bigstream-1.2.1/bigstream.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-08-05 00:26:34.000000 bigstream-1.2.1/bigstream.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-08-05 00:26:35.269826 bigstream-1.2.1/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-08-05 00:23:16.000000 bigstream-1.2.1/setup.py
```

### Comparing `bigstream-1.1.6/LICENSE.txt` & `bigstream-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/README.md` & `bigstream-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/align.py` & `bigstream-1.2.1/bigstream/align.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/application_pipelines.py` & `bigstream-1.2.1/bigstream/application_pipelines.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/configure_irm.py` & `bigstream-1.2.1/bigstream/configure_irm.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/features.py` & `bigstream-1.2.1/bigstream/features.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/level_set.py` & `bigstream-1.2.1/bigstream/level_set.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/metrics.py` & `bigstream-1.2.1/bigstream/metrics.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/motion_correct.py` & `bigstream-1.2.1/bigstream/motion_correct.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,25 +173,25 @@
 
     # distribute
     futures = cluster.client.map(wrapped_affine_align, mov_indices)
     params = np.array(cluster.client.gather(futures))
 
     # smooth and interpolate
     # TODO: this kind of smoothing will not work with affine transforms
-    params = gaussian_filter1d(params, sigma, axis=0)
+    params = gaussian_filter1d(params, sigma / time_stride, axis=0)
     if time_stride > 1:
         x = np.arange(total_frames) / time_stride
-        coords = np.meshgrid(x, np.mgrid[:6], indexing='ij')
-        params = map_coordinates(params, coords, mode='nearest')
+        coords = np.meshgrid(x, np.mgrid[:params.shape[1]], indexing='ij')
+        params = map_coordinates(params, coords, order=1, mode='nearest')
 
     # convert to matrices
     # TODO: again this assumes rigid transforms
-    transforms = np.empty((total_frames, 4, 4))
+    transforms = np.empty((total_frames, fix.ndim+1, fix.ndim+1))
     for i in range(params.shape[0]):
-        e = ut.parameters_to_euler_transform_3d(params[i])
+        e = ut.parameters_to_euler_transform(params[i])
         t = ut.affine_transform_to_matrix(e)
         transforms[i] = t
 
     # return all transforms
     return transforms
 
 
@@ -418,63 +418,65 @@
         if mask_sh != mov_sh:
             mask = zoom(mask, np.array(mov_sh) / mask_sh, order=0)
         np.save(temporary_directory.name + '/mask.npy', mask)
 
     # save initial deforms to location accessible to all workers
     new_list = []
     for iii, transform in enumerate(static_transform_list_before):
-        if transform.shape != (4, 4) and len(transform.shape) != 1:
+        if len(transform.shape) > 2:
             path = temporary_directory.name + f'/deform{iii}.npy'
             np.save(path, transform)
             transform = path
         new_list.append(transform)
     static_transform_list_before = new_list
 
     # save subsequent deforms to location accessible to all workers
     new_list = []
     for iii, transform in enumerate(static_transform_list_after):
-        if transform.shape != (4, 4) and len(transform.shape) != 1:
+        if len(transform.shape) > 2:
             path = temporary_directory.name + f'/deform{iii}.npy'
             np.save(path, transform)
             transform = path
         new_list.append(transform)
     static_transform_list_after = new_list
 
     # determine which frames will be resampled, ensure transforms are list
     total_frames = mov_zarr.shape[0]
     mov_indices = range(0, total_frames, time_stride)
     compute_frames = len(mov_indices)
-    transforms = list(transforms)
+    transforms = list(transforms)[::time_stride]
 
     # create an output zarr file
     output_zarr = ut.create_zarr(
         write_path,
         (compute_frames,) + mov_zarr.shape[1:],
         (1,) + mov_zarr.shape[1:],
-        np.uint16,
+        mov_zarr.dtype,
     )
 
     # wrap transform function
     def wrapped_apply_transform(
         read_index, write_index, transform,
         static_transform_list_before,
         static_transform_list_after,
     ):
 
         # read frame and mask data
         fix = np.load(temporary_directory.name + '/fix.npy')
         mov = mov_zarr[read_index]
+        mask = None
         if os.path.isfile(temporary_directory.name + '/mask.npy'):
             mask = np.load(temporary_directory.name + '/mask.npy')
 
         # format transform_list
         a = [np.load(x) if isinstance(x, str) else x for x in static_transform_list_before]
         b = [np.load(x) if isinstance(x, str) else x for x in static_transform_list_after]
         transform_list = [transform,]
         if len(transform.shape) == 1:  # affine + bspline case
+            # deformable_motion_correct not generalize to 2d yet, so this is fine
             transform_list = [transform[:16].reshape((4,4)), transform[16:]]
         transform_list = a + transform_list + b
 
         # apply transform_list
         aligned = apply_transform(
             fix, mov, fix_spacing, mov_spacing,
             transform_list=transform_list,
```

### Comparing `bigstream-1.1.6/bigstream/piecewise_align.py` & `bigstream-1.2.1/bigstream/piecewise_align.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/piecewise_transform.py` & `bigstream-1.2.1/bigstream/piecewise_transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/stitch.py` & `bigstream-1.2.1/bigstream/stitch.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/transform.py` & `bigstream-1.2.1/bigstream/transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/bigstream/utility.py` & `bigstream-1.2.1/bigstream/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     -------
     rigid_transform : sitk.Euler3DTransform object
         The same rigid transform but as a sitk object
     """
 
     ndims = matrix.shape[0] - 1
     matrix_sitk = invert_matrix_axes(matrix)
-    transform = sitk.Euler2DTransform if ndims == 2 else sitk.Euler3DTransform()
+    transform = sitk.Euler2DTransform() if ndims == 2 else sitk.Euler3DTransform()
     transform.SetMatrix(matrix_sitk[:ndims, :ndims].flatten())
     transform.SetTranslation(matrix_sitk[:ndims, -1].squeeze())
     return transform
 
 
 def euler_transform_to_parameters(transform):
     """
@@ -208,40 +208,53 @@
 
     Returns
     -------
     rigid_parameters : 1d-array, length 6
         The rigid transform parameters: (rotX, rotY, rotZ, transX, transY, transZ)
     """
 
-    return np.array((transform.GetAngleX(),
-                     transform.GetAngleY(),
-                     transform.GetAngleZ()) +
-                     transform.GetTranslation()
-    )
+    if transform.GetDimension() == 2:
+        return np.array((transform.GetAngle(),) +
+                         transform.GetTranslation(),
+        )
+
+    elif transform.GetDimension() == 3:
+        return np.array((transform.GetAngleX(),
+                         transform.GetAngleY(),
+                         transform.GetAngleZ()) +
+                         transform.GetTranslation()
+        )
 
 
-def parameters_to_euler_transform_3d(params):
+def parameters_to_euler_transform(params):
     """
     Convert rigid transform parameters to a sitk.Euler3DTransform object
 
     Parameters
     ----------
     rigid_parameters : 1d-array, length 6
         The rigid transform parameters: (rotX, rotY, rotZ, transX, transY, transZ)
 
     Returns
     -------
     transform : sitk.Euler3DTransform
         A sitk rigid transform object
     """
 
-    transform = sitk.Euler3DTransform()
-    transform.SetRotation(*params[:3])
-    transform.SetTranslation(params[3:])
-    return transform
+    if len(params) == 3:
+        transform = sitk.Euler2DTransform()
+        transform.SetAngle(params[0])
+        transform.SetTranslation(params[1:])
+        return transform
+
+    elif len(params) == 6:
+        transform = sitk.Euler3DTransform()
+        transform.SetRotation(*params[:3])
+        transform.SetTranslation(params[3:])
+        return transform
 
 
 def physical_parameters_to_affine_matrix_3d(params, center):
     """
     Convert separate affine transform parameters to an affine matrix
 
     Parameters
```

### Comparing `bigstream-1.1.6/bigstream.egg-info/SOURCES.txt` & `bigstream-1.2.1/bigstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.6/setup.py` & `bigstream-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bigstream",
-    version="1.1.6",
+    version="1.2.1",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for distributed alignment of massive images",
     url="https://github.com/GFleishman/bigstream",
     license="MIT",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

