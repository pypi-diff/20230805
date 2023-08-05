# Comparing `tmp/opstool-0.8.3.tar.gz` & `tmp/opstool-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opstool-0.8.3.tar", last modified: Fri Jul 21 16:43:36 2023, max compression
+gzip compressed data, was "opstool-0.8.4.tar", last modified: Sat Aug  5 07:37:11 2023, max compression
```

## Comparing `opstool-0.8.3.tar` & `opstool-0.8.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.210731 opstool-0.8.3/
--rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.3/LICENCE.txt
--rw-rw-rw-   0        0        0     6424 2023-07-21 16:43:36.210731 opstool-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 16:43:36.210731 opstool-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.175592 opstool-0.8.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.179481 opstool-0.8.3/src/opstool/
--rw-rw-rw-   0        0        0     8995 2023-06-17 04:24:19.000000 opstool-0.8.3/src/opstool/EleClassTags.py
--rw-rw-rw-   0        0        0       23 2023-07-21 16:41:10.000000 opstool-0.8.3/src/opstool/__about__.py
--rw-rw-rw-   0        0        0      673 2023-05-25 13:37:11.000000 opstool-0.8.3/src/opstool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.179481 opstool-0.8.3/src/opstool/analysis/
--rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.3/src/opstool/analysis/__init__.py
--rw-rw-rw-   0        0        0    13409 2023-06-01 06:34:16.000000 opstool-0.8.3/src/opstool/analysis/_sec_analysis.py
--rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.3/src/opstool/analysis/_smart_analyze.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.195114 opstool-0.8.3/src/opstool/examples/
--rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.3/src/opstool/examples/ArchBridge.py
--rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.3/src/opstool/examples/ArchBridge2.py
--rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.3/src/opstool/examples/CableStayedBridge.py
--rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.3/src/opstool/examples/Dam.py
--rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.3/src/opstool/examples/DamBreak.py
--rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.3/src/opstool/examples/Frame3D.py
--rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.3/src/opstool/examples/Frame3D2.py
--rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.3/src/opstool/examples/GridFrame.py
--rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.3/src/opstool/examples/Igloo.py
--rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.3/src/opstool/examples/Pier.py
--rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.3/src/opstool/examples/SDOF.py
--rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.3/src/opstool/examples/SuspensionBridge.py
--rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.3/src/opstool/examples/__init__.py
--rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.3/src/opstool/examples/shell3D.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.195114 opstool-0.8.3/src/opstool/preprocessing/
--rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.3/src/opstool/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2876 2023-05-09 04:18:48.000000 opstool-0.8.3/src/opstool/preprocessing/geom_transf.py
--rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.3/src/opstool/preprocessing/load.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.195114 opstool-0.8.3/src/opstool/preprocessing/section/
--rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.3/src/opstool/preprocessing/section/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.3/src/opstool/preprocessing/section/lib_sec_mesh.py
--rw-rw-rw-   0        0        0    60702 2023-05-23 16:16:51.000000 opstool-0.8.3/src/opstool/preprocessing/section/sec_mesh.py
--rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.3/src/opstool/preprocessing/section/var_sec_mesh.py
--rw-rw-rw-   0        0        0    53581 2023-05-26 07:18:07.000000 opstool-0.8.3/src/opstool/preprocessing/tcl2py.py
--rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.3/src/opstool/preprocessing/unit_system.py
--rw-rw-rw-   0        0        0     6679 2023-06-17 05:03:00.000000 opstool-0.8.3/src/opstool/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.210731 opstool-0.8.3/src/opstool/vis/
--rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.3/src/opstool/vis/__init__.py
--rw-rw-rw-   0        0        0    32837 2023-06-17 08:35:28.000000 opstool-0.8.3/src/opstool/vis/_get_model_base.py
--rw-rw-rw-   0        0        0   108776 2023-07-21 16:38:13.000000 opstool-0.8.3/src/opstool/vis/_plotly_base.py
--rw-rw-rw-   0        0        0    68932 2023-06-23 14:36:55.000000 opstool-0.8.3/src/opstool/vis/_pyvista_base.py
--rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.3/src/opstool/vis/fiber_sec_vis.py
--rw-rw-rw-   0        0        0    33077 2023-06-17 09:08:01.000000 opstool-0.8.3/src/opstool/vis/get_model_data.py
--rw-rw-rw-   0        0        0    28645 2023-05-25 15:40:29.000000 opstool-0.8.3/src/opstool/vis/ops_vis_2d.py
--rw-rw-rw-   0        0        0    26569 2023-07-21 16:39:02.000000 opstool-0.8.3/src/opstool/vis/ops_vis_plotly.py
--rw-rw-rw-   0        0        0    26362 2023-06-19 07:13:16.000000 opstool-0.8.3/src/opstool/vis/ops_vis_pyvista.py
--rw-rw-rw-   0        0        0    10367 2023-06-17 09:08:55.000000 opstool-0.8.3/src/opstool/vis/quick_plot.py
--rw-rw-rw-   0        0        0    14099 2023-05-09 07:53:13.000000 opstool-0.8.3/src/opstool/vis/save_tikz.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.179481 opstool-0.8.3/src/opstool.egg-info/
--rw-rw-rw-   0        0        0     6424 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1758 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 16:43:36.000000 opstool-0.8.3/src/opstool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 16:43:36.210731 opstool-0.8.3/tests/
--rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.3/tests/test_dambreak.py
--rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.3/tests/test_fiber_sec_vis.py
--rw-rw-rw-   0        0        0     2995 2023-06-17 05:06:14.000000 opstool-0.8.3/tests/test_model_vis.py
--rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.3/tests/test_sec_analysis.py
--rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.3/tests/test_sec_mesh.py
--rw-rw-rw-   0        0        0      954 2023-05-09 13:39:18.000000 opstool-0.8.3/tests/test_temp.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.685456 opstool-0.8.4/
+-rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.4/LICENCE.txt
+-rw-rw-rw-   0        0        0     6424 2023-08-05 07:37:11.684456 opstool-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 07:37:11.685456 opstool-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.628529 opstool-0.8.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.635417 opstool-0.8.4/src/opstool/
+-rw-rw-rw-   0        0        0     8995 2023-06-17 04:24:19.000000 opstool-0.8.4/src/opstool/EleClassTags.py
+-rw-rw-rw-   0        0        0       23 2023-08-05 07:29:40.000000 opstool-0.8.4/src/opstool/__about__.py
+-rw-rw-rw-   0        0        0      673 2023-05-25 13:37:11.000000 opstool-0.8.4/src/opstool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.641528 opstool-0.8.4/src/opstool/analysis/
+-rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.4/src/opstool/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13409 2023-06-01 06:34:16.000000 opstool-0.8.4/src/opstool/analysis/_sec_analysis.py
+-rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.4/src/opstool/analysis/_smart_analyze.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.659527 opstool-0.8.4/src/opstool/examples/
+-rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.4/src/opstool/examples/ArchBridge.py
+-rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.4/src/opstool/examples/ArchBridge2.py
+-rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.4/src/opstool/examples/CableStayedBridge.py
+-rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.4/src/opstool/examples/Dam.py
+-rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.4/src/opstool/examples/DamBreak.py
+-rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.4/src/opstool/examples/Frame3D.py
+-rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.4/src/opstool/examples/Frame3D2.py
+-rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.4/src/opstool/examples/GridFrame.py
+-rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.4/src/opstool/examples/Igloo.py
+-rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.4/src/opstool/examples/Pier.py
+-rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.4/src/opstool/examples/SDOF.py
+-rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.4/src/opstool/examples/SuspensionBridge.py
+-rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.4/src/opstool/examples/__init__.py
+-rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.4/src/opstool/examples/shell3D.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.663528 opstool-0.8.4/src/opstool/preprocessing/
+-rw-rw-rw-   0        0        0      886 2023-08-02 11:21:29.000000 opstool-0.8.4/src/opstool/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2876 2023-05-09 04:18:48.000000 opstool-0.8.4/src/opstool/preprocessing/geom_transf.py
+-rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.4/src/opstool/preprocessing/load.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.667530 opstool-0.8.4/src/opstool/preprocessing/section/
+-rw-rw-rw-   0        0        0      547 2023-08-02 11:20:59.000000 opstool-0.8.4/src/opstool/preprocessing/section/__init__.py
+-rw-rw-rw-   0        0        0    27140 2023-08-02 12:22:34.000000 opstool-0.8.4/src/opstool/preprocessing/section/sec_lib.py
+-rw-rw-rw-   0        0        0    64747 2023-08-02 11:54:32.000000 opstool-0.8.4/src/opstool/preprocessing/section/sec_mesh.py
+-rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.4/src/opstool/preprocessing/section/var_sec_mesh.py
+-rw-rw-rw-   0        0        0    53581 2023-05-26 07:18:07.000000 opstool-0.8.4/src/opstool/preprocessing/tcl2py.py
+-rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.4/src/opstool/preprocessing/unit_system.py
+-rw-rw-rw-   0        0        0     6679 2023-06-17 05:03:00.000000 opstool-0.8.4/src/opstool/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.679532 opstool-0.8.4/src/opstool/vis/
+-rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.4/src/opstool/vis/__init__.py
+-rw-rw-rw-   0        0        0    32837 2023-07-27 16:15:24.000000 opstool-0.8.4/src/opstool/vis/_get_model_base.py
+-rw-rw-rw-   0        0        0   108776 2023-07-21 16:38:13.000000 opstool-0.8.4/src/opstool/vis/_plotly_base.py
+-rw-rw-rw-   0        0        0    68932 2023-06-23 14:36:55.000000 opstool-0.8.4/src/opstool/vis/_pyvista_base.py
+-rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.4/src/opstool/vis/fiber_sec_vis.py
+-rw-rw-rw-   0        0        0    33077 2023-06-17 09:08:01.000000 opstool-0.8.4/src/opstool/vis/get_model_data.py
+-rw-rw-rw-   0        0        0    28645 2023-05-25 15:40:29.000000 opstool-0.8.4/src/opstool/vis/ops_vis_2d.py
+-rw-rw-rw-   0        0        0    26569 2023-07-21 16:39:02.000000 opstool-0.8.4/src/opstool/vis/ops_vis_plotly.py
+-rw-rw-rw-   0        0        0    26362 2023-06-19 07:13:16.000000 opstool-0.8.4/src/opstool/vis/ops_vis_pyvista.py
+-rw-rw-rw-   0        0        0    10367 2023-06-17 09:08:55.000000 opstool-0.8.4/src/opstool/vis/quick_plot.py
+-rw-rw-rw-   0        0        0    14099 2023-05-09 07:53:13.000000 opstool-0.8.4/src/opstool/vis/save_tikz.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.639521 opstool-0.8.4/src/opstool.egg-info/
+-rw-rw-rw-   0        0        0     6424 2023-08-05 07:37:11.000000 opstool-0.8.4/src/opstool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1753 2023-08-05 07:37:11.000000 opstool-0.8.4/src/opstool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 07:37:11.000000 opstool-0.8.4/src/opstool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-08-05 07:37:11.000000 opstool-0.8.4/src/opstool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 07:37:11.000000 opstool-0.8.4/src/opstool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 07:37:11.684456 opstool-0.8.4/tests/
+-rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.4/tests/test_dambreak.py
+-rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.4/tests/test_fiber_sec_vis.py
+-rw-rw-rw-   0        0        0     2995 2023-06-17 05:06:14.000000 opstool-0.8.4/tests/test_model_vis.py
+-rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.4/tests/test_sec_analysis.py
+-rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.4/tests/test_sec_mesh.py
+-rw-rw-rw-   0        0        0      954 2023-05-09 13:39:18.000000 opstool-0.8.4/tests/test_temp.py
```

### Comparing `opstool-0.8.3/LICENCE.txt` & `opstool-0.8.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/PKG-INFO` & `opstool-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.3
+Version: 0.8.4
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.3 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.4 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.3/README.md` & `opstool-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/setup.py` & `opstool-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/EleClassTags.py` & `opstool-0.8.4/src/opstool/EleClassTags.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/__init__.py` & `opstool-0.8.4/src/opstool/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/analysis/_sec_analysis.py` & `opstool-0.8.4/src/opstool/analysis/_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/analysis/_smart_analyze.py` & `opstool-0.8.4/src/opstool/analysis/_smart_analyze.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/ArchBridge.py` & `opstool-0.8.4/src/opstool/examples/ArchBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/ArchBridge2.py` & `opstool-0.8.4/src/opstool/examples/ArchBridge2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/CableStayedBridge.py` & `opstool-0.8.4/src/opstool/examples/CableStayedBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/Dam.py` & `opstool-0.8.4/src/opstool/examples/Dam.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/DamBreak.py` & `opstool-0.8.4/src/opstool/examples/DamBreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/Frame3D.py` & `opstool-0.8.4/src/opstool/examples/Frame3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/Frame3D2.py` & `opstool-0.8.4/src/opstool/examples/Frame3D2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/GridFrame.py` & `opstool-0.8.4/src/opstool/examples/GridFrame.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/Igloo.py` & `opstool-0.8.4/src/opstool/examples/Igloo.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/Pier.py` & `opstool-0.8.4/src/opstool/examples/Pier.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/SDOF.py` & `opstool-0.8.4/src/opstool/examples/SDOF.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/SuspensionBridge.py` & `opstool-0.8.4/src/opstool/examples/SuspensionBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/examples/shell3D.py` & `opstool-0.8.4/src/opstool/examples/shell3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/preprocessing/__init__.py` & `opstool-0.8.4/src/opstool/preprocessing/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .load import gen_grav_load
 from .tcl2py import tcl2py
 from .unit_system import UnitSystem
 from .geom_transf import beam_geom_transf
 from .section import (Rebars, SecMesh, add_circle, add_material,
                       add_polygon, offset, poly_offset, line_offset, var_line_string, vis_var_sec,
-                      get_legendre_loc, get_lobatto_loc)
+                      get_legendre_loc, get_lobatto_loc, section_library)
 
 __all__ = ["gen_grav_load",
            "tcl2py",
            "UnitSystem",
            "beam_geom_transf",
            # -----------
            "SecMesh",
@@ -18,9 +18,10 @@
            "add_circle",
            "offset",
            "poly_offset",
            "line_offset",
            "var_line_string",
            "vis_var_sec",
            "get_legendre_loc",
-           "get_lobatto_loc"
+           "get_lobatto_loc",
+           "section_library"
            ]
```

### Comparing `opstool-0.8.3/src/opstool/preprocessing/geom_transf.py` & `opstool-0.8.4/src/opstool/preprocessing/geom_transf.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/preprocessing/load.py` & `opstool-0.8.4/src/opstool/preprocessing/load.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/preprocessing/section/__init__.py` & `opstool-0.8.4/src/opstool/preprocessing/section/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from .sec_mesh import (Rebars, SecMesh, add_circle, add_material,
                        add_polygon, offset, poly_offset, line_offset)
 from .var_sec_mesh import var_line_string, vis_var_sec, get_legendre_loc, get_lobatto_loc
+from .sec_lib import section_library
 
-__all__ = ["SecMesh",
-           "Rebars",
-           "add_material",
-           "add_polygon",
-           "add_circle",
-           "offset",
-           "poly_offset",
-           "line_offset",
-           "var_line_string",
-           "vis_var_sec",
-           "get_legendre_loc",
-           "get_lobatto_loc"]
+__all__ = [
+    "SecMesh",
+    "Rebars",
+    "add_material",
+    "add_polygon",
+    "add_circle",
+    "offset",
+    "poly_offset",
+    "line_offset",
+    "var_line_string",
+    "vis_var_sec",
+    "get_legendre_loc",
+    "get_lobatto_loc",
+    "section_library"
+]
```

### Comparing `opstool-0.8.3/src/opstool/preprocessing/section/sec_mesh.py` & `opstool-0.8.4/src/opstool/preprocessing/section/sec_mesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,56 +72,73 @@
         Returns
         ----------
         instance
         """
         self.group_map = group
         return self
 
-    def assign_mesh_size(self, mesh_size: dict):
+    def get_group(self,):
+        """Return the group dict for each geometry obj.
+
+        Returns
+        ----------
+        group : dict[str, any]
+        """
+        return self.group_map
+
+    def assign_mesh_size(self, mesh_size: dict = None):
         """Assign the mesh size dict for each mesh.
 
         Parameters
         ------------
-        mesh_size : dict[str, float]
+        mesh_size : dict[str, float], default=None
             A dict of name as key, mesh size as value.
             The mesh sizes describe the maximum mesh element area to be
             used in the finite-element mesh for each Geometry object.
+            If default None is used, the mesh size of each Geometry will be
+            calculate by its area / 100.
 
         Returns
         ------------
         instance
         """
         if not self.group_map:
             raise ValueError("The assign_group method should be run first!")
-        for name in mesh_size.keys():
-            if name not in self.group_map.keys():
-                raise ValueError(
-                    f"{name} is not specified in the assign_group function!"
-                )
+        if mesh_size is None:
+            mesh_size = dict()
+            for name, geom in self.group_map.items():
+                area = geom.calculate_area()
+                mesh_size[name] = area / 100
+        else:
+            for name in mesh_size.keys():
+                if name not in self.group_map.keys():
+                    raise ValueError(
+                        f"{name} is not specified in the assign_group function!"
+                    )
         self.mesh_size_map = mesh_size
         return self
 
     def assign_ops_matTag(self, mat_tag: dict):
         """Assign the mesh size dict for each mesh.
 
         Parameters
         --------------
         mat_tag : dict[str, int]
-            A dict of name as key, opensees matTag previous defined as value.
+            A dict of name as key, OpenSees matTag previous defined as value.
 
         Returns
         ----------
         instance
         """
         if not self.group_map:
             raise ValueError("The assign_group method should be run first!")
         for name in mat_tag.keys():
             if name not in self.group_map.keys():
                 raise ValueError(
-                    f"{name} is not specified in the assign_group function!"
+                    f"{name} is not specified in the assign_group method!"
                 )
         self.mat_ops_map = mat_tag
         return self
 
     def assign_group_color(self, colors: dict):
         """Assign the color dict to plot the section.
 
@@ -169,26 +186,30 @@
                     poissons_ratio=geom.material.poissons_ratio,
                     yield_strength=geom.material.yield_strength,
                     density=geom.material.density,
                     color=self.color_map[name],
                 )
             geoms.append(geom)
             mesh_sizes.append(self.mesh_size_map[name])
-        geom_obj = CompoundGeometry(geoms)
-        mesh_obj = geom_obj.create_mesh(mesh_sizes=mesh_sizes)
+        if len(geoms) > 1:
+            geom_obj = CompoundGeometry(geoms)
+            mesh_obj = geom_obj.create_mesh(mesh_sizes=mesh_sizes)
+        else:
+            geom_obj = geoms[0]
+            mesh_obj = geom_obj.create_mesh(mesh_sizes=mesh_sizes[0])
         self.section = Section(geom_obj, time_info=False)
         self.mesh_obj = mesh_obj.mesh
         self._get_mesh_data()
         if plot_mesh:
             self.section.plot_mesh(materials=True, alpha=0.90)
 
     def _get_mesh_data(self):
         # * mesh data
         vertices = self.mesh_obj["vertices"]
-        self.points = vertices
+        self.points = np.array(vertices)
         triangles = self.mesh_obj["triangles"][:, :3]
         triangle_attributes = self.mesh_obj["triangle_attributes"]
         attributes = np.unique(triangle_attributes)
         for name, attri in zip(self.group_map.keys(), attributes):
             idx = triangle_attributes == attri
             self.cells_map[name] = triangles[idx[:, 0]]
         # * fiber data
@@ -299,30 +320,32 @@
     def get_j(self):
         """Return section torsion constant.
 
         Returns
         -------
         Float
         """
-        j = 0
+        j = 10000
         if self.frame_sec_props:
             j = self.frame_sec_props["J"]
         elif self.sec_props:
             j = self.sec_props["J"]
         else:
-            raise ValueError(
-                "The Section Properties method <get_frame_props> or <get_sec_props> has not been run!"
-            )
+            self.get_frame_props()
+            j = self.frame_sec_props["J"]
         return j
 
-    def _run_sec_props(self, Eref, Gref, section):
+    def _run_sec_props(self, Eref, Gref):
+        self.section.calculate_geometric_properties()
+        self.section.calculate_warping_properties()
+        section = self.section
         # Second moments of area centroidal axis
         ixx_c, iyy_c, ixy_c = section.get_ic()
         # Elastic centroid
-        cx, cy = section.get_c()
+        cx, cy = (0.0, 0.0) if self.is_centring else section.get_c()
         # Elastic section moduli about the centroidal axis with respect to the top and bottom fibres
         zxx_plus, zxx_minus, zyy_plus, zyy_minus = section.get_z()
         # Principal bending axis angle
         phi = section.get_phi()
         # Shear area for loading about the centroidal axis
         area_sx, area_sy = section.get_As()
         # mass
@@ -378,14 +401,15 @@
         self.sec_props = sec_props
 
     def get_sec_props(
         self,
         Eref: float = 1.0,
         Gref: float = None,
         display_results: bool = False,
+        fmt: str = '8.3E',
         plot_centroids: bool = False,
     ):
         """
         Solving Section Geometry Properties by Finite Element Method, by ``sectionproperties`` pacakge.
         See `sectionproperties doc <https://sectionproperties.readthedocs.io/en/latest/rst/post.html
         #getting-specific-section-properties>`_
 
@@ -400,14 +424,16 @@
             See `sectionproperties doc <https://sectionproperties.readthedocs.io/en/latest/rst/post.html
             #how-material-properties-affect-results>`_
         Gref: float, default=None
             Reference shear modulus, useful for torsional constant calculations of composite section.
             If None, Gref = 0.5 * Eref.
         display_results : bool, default=True
             whether to display the results.
+        fmt : str, optional
+            Number formatting string when display_results=True.
         plot_centroids : bool, default=False
             whether to plot centroids
 
         Returns
         -----------
         sec_props: dict
             section props dict, including:
@@ -434,18 +460,15 @@
             Note that according to the OpenSees convention,
             the x-axis refers to the normal direction of the section,
             the y-axis refers to the abscissa,
             and the z-axis refers to the ordinate direction.
         """
         if Gref is None:
             Gref = 0.5 * Eref
-        section = self.section
-        section.calculate_geometric_properties()
-        section.calculate_warping_properties()
-        self._run_sec_props(Eref, Gref, section)
+        self._run_sec_props(Eref, Gref)
         if display_results:
             # section.display_results()
             syms = [
                 "A",
                 "Asy",
                 "Asz",
                 "centroid",
@@ -480,29 +503,33 @@
             ]
             table = Table(title="Section Properties")
             table.add_column("Symbol", style="cyan", no_wrap=True)
             table.add_column("Value", style="magenta")
             table.add_column("Definition", style="green")
             for sym_, def_ in zip(syms, defs):
                 if sym_ != "centroid":
-                    table.add_row(sym_, f"{self.sec_props[sym_]:.3E}", def_)
+                    table.add_row(sym_, f"{self.sec_props[sym_]:>{fmt}}", def_)
                 else:
                     table.add_row(
                         sym_,
-                        f"({self.sec_props[sym_][0]:.3E}, {self.sec_props[sym_][1]:.3E})",
+                        f"({self.sec_props[sym_][0]:>{fmt}}, {self.sec_props[sym_][1]:>{fmt}})",
                         def_,
                     )
             console = Console()
             console.print(table)
         if plot_centroids:
-            section.plot_centroids()
+            self.section.plot_centroids()
         return self.sec_props
 
     def get_frame_props(
-        self, Eref: float = 1.0, Gref: float = None, display_results: bool = False
+        self,
+        Eref: float = 1.0,
+        Gref: float = None,
+        display_results: bool = False,
+        fmt: str = '8.3E'
     ):
         """Calculates and returns the properties required for a frame analysis.
         See `sectionproperties doc <https://sectionproperties.readthedocs.io/en/latest/rst/api.html
         #sectionproperties.analysis.section.Section.calculate_frame_properties>`_
 
         This method is fast, but cannot calculate the shear area compared to the
         method :py:meth:`~opstool.preprocessing.SecMesh.get_sec_props`.
@@ -515,14 +542,16 @@
             See `sectionproperties doc <https://sectionproperties.readthedocs.io/en/latest/rst/post.html#
             how-material-properties-affect-results>`_
         Gref: float, default=None
             Reference shear modulus, useful for torsional constant calculations of composite section.
             If None, Gref = 0.5 * Eref.
         display_results : bool, default=True
             whether to display the results.
+        fmt : str, optional
+            Number formatting string when display_results=True.
 
         Returns
         -----------
         sec_props: dict
             section props dict, including:
 
             * Cross-sectional area (A)
@@ -550,15 +579,15 @@
         """
         if Gref is None:
             Gref = 0.5 * Eref
         # self.section.calculate_geometric_properties()
         (ea, ixx_c, iyy_c, ixy_c, j, phi) = self.section.calculate_frame_properties(
             solver_type="direct"
         )
-        cx, cy = self.section.get_c()
+        cx, cy = (0.0, 0.0) if self.is_centring else self.section.get_c()
         mass, ga = 0, 0
         for el in self.section.elements:
             (area_, _, _, _, _, _, _, g, rho) = el.geometric_properties()
             mass += area_ * rho
             ga += area_ * g
         self.section.section_props.calculate_centroidal_properties(self.section.mesh)
         zxx_plus, zxx_minus, zyy_plus, zyy_minus = self.section.get_z()
@@ -634,26 +663,42 @@
             ]
             table = Table(title="Frame Section Properties")
             table.add_column("Symbol", style="cyan", no_wrap=True)
             table.add_column("Value", style="magenta")
             table.add_column("Definition", style="green")
             for sym_, def_ in zip(syms, defs):
                 if sym_ != "centroid":
-                    table.add_row(sym_, f"{sec_props[sym_]:.3E}", def_)
+                    table.add_row(
+                        sym_,
+                        "{:>{fmt}}".format(sec_props[sym_], fmt=fmt),
+                        def_
+                    )
                 else:
                     table.add_row(
                         sym_,
-                        f"({sec_props[sym_][0]:.3E}, {sec_props[sym_][1]:.3E})",
+                        f"({sec_props[sym_][0]:>{fmt}}, {sec_props[sym_][1]:>{fmt}})",
                         def_,
                     )
             console = Console()
             console.print(table)
         self.frame_sec_props = sec_props
         return sec_props
 
+    def display_all_results(self, fmt: str = '8.6e'):
+        """Prints all results that have been calculated by ``sectionproperties`` to the terminal.
+
+        Parameters
+        ----------
+        fmt : str, optional
+            Number formatting string.
+        """
+        if not self.sec_props:
+            self._run_sec_props()
+        self.section.display_results(fmt=fmt)
+
     def get_stress(
         self,
         N: float = 0,
         Vy: float = 0,
         Vz: float = 0,
         Myy: float = 0,
         Mzz: float = 0,
@@ -986,28 +1031,40 @@
             rebar_xy = self.rebar_data[i]["rebar_xy"]
             x_rot, y_rot = sec_rotation(rebar_xy[:, 0], rebar_xy[:, 1], theta)
             (
                 self.rebar_data[i]["rebar_xy"][:, 0],
                 self.rebar_data[i]["rebar_xy"][:, 1],
             ) = (x_rot, y_rot)
 
-    def opspy_cmds(self, secTag: int, GJ: float):
+    def opspy_cmds(self, secTag: int, GJ: float = None, G: float = None):
         """Generate openseespy fiber section command.
 
         Parameters
         ------------
         secTag : int
             The section tag assigned in OpenSees.
-        GJ : float
+        GJ : float, default = None
             Torsion stiffness.
+            Note that at least one of GJ and G needs to be specified,
+            and if both, it will be calculated by GJ.
+        G : float, default = None
+            Shear modulus.The torsion constant is automatically calculated by the program.
+            Note that at least one of GJ and G needs to be specified,
+            and if both, it will be calculated by GJ.
 
         Returns
         ----------
         None
         """
+        if GJ is None:
+            if G is None:
+                raise ValueError("GJ and G need to assign at least one!")
+            else:
+                GJ = G * self.get_j()
+
         ops.section("Fiber", secTag, "-GJ", GJ)
 
         names = self.centers_map.keys()
         for name in names:
             centers = self.centers_map[name]
             areas = self.areas_map[name]
             matTag = self.mat_ops_map[name]
@@ -1018,35 +1075,47 @@
             rebar_xy = data["rebar_xy"]
             dia = data["dia"]
             matTag = data["matTag"]
             for xy in rebar_xy:
                 area = np.pi / 4 * dia**2
                 ops.fiber(xy[0], xy[1], area, matTag)
 
-    def to_file(self, output_path: str, secTag: int, GJ: float):
+    def to_file(self, output_path: str, secTag: int, GJ: float = None, G: float = None):
         """Output the opensees fiber code to file.
 
         Parameters
         -------------
         output_path : str
             The filepath to save, e.g., r"my_dir/my_section.py"
         secTag : int
             The section tag assigned in OpenSees.
-        GJ : float
+        GJ : float, default = None
             Torsion stiffness.
+            Note that at least one of GJ and G needs to be specified,
+            and if both, it will be calculated by GJ.
+        G : float, default = None
+            Shear modulus.The torsion constant is automatically calculated by the program.
+            Note that at least one of GJ and G needs to be specified,
+            and if both, it will be calculated by GJ.
 
         Returns
         ---------
         None
 
         Notes
         -----
         Notes that output_path must be endswith ``.py`` or ``.tcl``,
         function will create the file by a right style.
         """
+        if GJ is None:
+            if G is None:
+                raise ValueError("GJ and G need to assign at least one!")
+            else:
+                GJ = G * self.get_j()
+
         names = self.centers_map.keys()
         if output_path.endswith(".tcl"):
             self._to_tcl(output_path, names, secTag, GJ)
         elif output_path.endswith(".py"):
             self._to_py(output_path, names, secTag, GJ)
         else:
             raise ValueError("output_path must endwith .tcl or .py!")
@@ -1109,30 +1178,33 @@
                         f"ops.fiber({xy[0]:.8E}, {xy[1]:.8E}, {area:.8E}, {mat_tag})\n"
                     )
 
     def view(
         self,
         fill: bool = True,
         engine: str = "plotly",
-        save_html: str = "SecMesh.html",
+        save_html: str = None,
         on_notebook: bool = False,
+        show_hover: bool = False,
     ):
         """Display the section mesh.
 
         Parameters
         -----------
         fill : bool, default=True
              Whether to fill the trangles.
         engine: str, default='plotly'
             Plot engine, optional "plotly" or "matplotlib".
         save_html: str, default="SecMesh.html"
             If set, the figure will save as a html file, only useful for engine="plotly".
             If False or None, this parameter will be ignored.
         on_notebook: bool, default=False
             If True, the figure will display in a notebook.
+        show_hover: bool, default=False
+            If True, the figure will show the hover labels.
 
         Returns
         --------
         None
         """
 
         # self.section.display_mesh_info()
@@ -1140,24 +1212,27 @@
         vertices = self.points
         x = vertices[:, 0]
         y = vertices[:, 1]
         aspect_ratio = (np.max(y) - np.min(y)) / (np.max(x) - np.min(x))
         if engine.lower().startswith("m"):
             self._plot_mpl(fill, aspect_ratio)
         elif engine.lower().startswith("p"):
-            self._plot_plotly(fill, aspect_ratio, save_html, on_notebook)
+            self._plot_plotly(fill, aspect_ratio, save_html, show_hover=show_hover)
         else:
             raise ValueError(
                 f"not supported engine {engine}! optional, 'plotly' or 'matplotlib'!"
             )
 
     def _plot_mpl(self, fill, aspect_ratio):
         # matplotlib plot
-        fig, ax = plt.subplots(figsize=(8, 8 * aspect_ratio))
-        # ax.set_facecolor("#efefef")
+        if aspect_ratio <= 0.333:
+            aspect_ratio = 0.333
+        if aspect_ratio >= 3:
+            aspect_ratio = 3
+        fig, ax = plt.subplots(figsize=(8, 8))
         # view the mesh
         vertices = self.points  # the coords of each triangle vertex
         for name, faces in self.cells_map.items():
             # faces = faces.astype(np.int64)
             if not fill:
                 x = vertices[:, 0]
                 y = vertices[:, 1]
@@ -1191,29 +1266,35 @@
             rebar_coords = []
             for xy in rebar_xy:
                 rebar_coords.append(xy)
             patches = [plt.Circle((xy[0], xy[1]), dia / 2) for xy in rebar_coords]
             coll = PatchCollection(patches, facecolors=color)
             ax.add_collection(coll)
 
-        # ax.set_aspect("equal")
+        ax.set_aspect(aspect_ratio)
         ax.set_title(self.sec_name, fontsize=26, fontfamily="SimSun")
         ax.legend(
             fontsize=18,
             shadow=False,
             markerscale=3,
-            loc=10,
+            loc='center left',
             ncol=len(self.group_map),
-            bbox_to_anchor=(0.5, -0.2),
+            bbox_to_anchor=(1.01, 0.5),
             bbox_transform=ax.transAxes,
         )
+        ax.set_xlabel("y", fontsize=22)
+        ax.set_ylabel("z", fontsize=22)
         ax.tick_params(labelsize=18)
+        plt.tight_layout()
         plt.show()
 
-    def _plot_plotly(self, fill, aspect_ratio, save_html, on_notebook):
+    def _plot_plotly(
+        self, fill, aspect_ratio, save_html,
+        show_hover: bool = True
+    ):
         vertices = self.points  # the coords of each triangle vertex
         n_cells = 0
         n_cells_map = dict()
         fig = go.Figure()
         tplot = []
         for name, faces in self.cells_map.items():
             if not self.mat_ops_map:
@@ -1265,27 +1346,28 @@
                         mode="lines",
                         line=dict(color=self.color_map[name], width=1.2),
                         connectgaps=False,
                         hoverinfo="skip",
                     )
                 )
             # hover label
-            tplot.append(
-                go.Scatter(
-                    x=center_areas[:, 0],
-                    y=center_areas[:, 1],
-                    marker=dict(
-                        size=0, color=self.color_map[name], symbol="diamond-open"
-                    ),
-                    mode="markers",
-                    name=label,
-                    customdata=center_areas_labels,
-                    hovertemplate="%{customdata}",
+            if show_hover:
+                tplot.append(
+                    go.Scatter(
+                        x=center_areas[:, 0],
+                        y=center_areas[:, 1],
+                        marker=dict(
+                            size=0, color=self.color_map[name], symbol="diamond-open"
+                        ),
+                        mode="markers",
+                        name=label,
+                        customdata=center_areas_labels,
+                        hovertemplate="%{customdata}",
+                    )
                 )
-            )
         fig.add_traces(tplot)
         # rebars
         shapes = []
         for data in self.rebar_data:
             color = data["color"]
             rebar_xy = data["rebar_xy"]
             r = data["dia"] / 2
@@ -1304,32 +1386,40 @@
                     )
                 )
         # -------------------------------------
         txt = "Num. of Mesh: "
         for k, v in n_cells_map.items():
             txt += f"| {k}--{v} "
         txt += f"| total--{n_cells}"
+        if aspect_ratio <= 0.3:
+            width, height = 1600, 1600 * 0.3
+        elif aspect_ratio > 0.3 and aspect_ratio <= 1.0:
+            width, height = 1600, 1600 * aspect_ratio
+        elif aspect_ratio > 1.0 and aspect_ratio <= 3.333:
+            width, height = 900 / aspect_ratio, 900
+        else:
+            width, height = 900 / 3.333, 900
         fig.update_layout(
             shapes=shapes,
-            width=900,
-            height=900 * aspect_ratio,
+            width=width,
+            height=height,
             template="plotly",
             autosize=True,
             showlegend=False,
             scene=dict(aspectratio=dict(x=1, y=aspect_ratio), aspectmode="data"),
             title=dict(
-                font=dict(family="courier", color="black", size=16),
+                font=dict(family="courier", color="black", size=18),
                 text=f"<b>{self.sec_name}</b> <br>" + f"{txt}",
             ),
         )
         fig.update_xaxes(tickfont_size=18, ticks="outside")
         fig.update_yaxes(tickfont_size=18, ticks="outside")
         if save_html:
             pio.write_html(fig, file=save_html, auto_open=True)
-        if on_notebook:
+        else:
             fig.show()
 
 
 class Rebars:
     """
     A class to create the rebar point.
     """
@@ -1349,15 +1439,17 @@
         group_name: str = None,
     ):
         """Add rebar along a line, can be a line or polygon.
 
         Parameters
         ----------
         points: list[list[float, float]]
-            A list of rebar coords, [(x1, y1), (x2, y2),...,(xn, yn)]
+            A list of rebar coords, [(x1, y1), (x2, y2),...,(xn, yn)],
+            in which each element represents a corner point,
+            and every two corner points are divided by the arg `gap`.
         dia: float
             Rebar dia.
         gap: float, default=0.1
             Rebar space.
         n: int, default=None
             The number of rebars, if not None,
             update the Arg `gap` according to `n`.
@@ -1532,14 +1624,23 @@
     -------
     polygon obj
     """
     if material is None:
         material_ = add_material()
     else:
         material_ = material
+    # close or not
+    vec = np.array(outline[0]) - np.array(outline[-1])
+    if np.linalg.norm(vec) < 1e-8:
+        outline = outline[:-1]
+    if holes is not None:
+        for i, hole in enumerate(holes):
+            vec = np.array(hole[0]) - np.array(hole[-1])
+            if np.linalg.norm(vec) < 1e-8:
+                holes[i] = hole[:-1]
     ply = Polygon(outline, holes)
     geometry = Geometry(geom=ply, material=material_)
     return geometry
 
 
 def add_circle(
     xo: list,
```

### Comparing `opstool-0.8.3/src/opstool/preprocessing/section/var_sec_mesh.py` & `opstool-0.8.4/src/opstool/preprocessing/section/var_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/preprocessing/tcl2py.py` & `opstool-0.8.4/src/opstool/preprocessing/tcl2py.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/preprocessing/unit_system.py` & `opstool-0.8.4/src/opstool/preprocessing/unit_system.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/utils.py` & `opstool-0.8.4/src/opstool/utils.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/_get_model_base.py` & `opstool-0.8.4/src/opstool/vis/_get_model_base.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/_plotly_base.py` & `opstool-0.8.4/src/opstool/vis/_plotly_base.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/_pyvista_base.py` & `opstool-0.8.4/src/opstool/vis/_pyvista_base.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/fiber_sec_vis.py` & `opstool-0.8.4/src/opstool/vis/fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/get_model_data.py` & `opstool-0.8.4/src/opstool/vis/get_model_data.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/ops_vis_2d.py` & `opstool-0.8.4/src/opstool/vis/ops_vis_2d.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/ops_vis_plotly.py` & `opstool-0.8.4/src/opstool/vis/ops_vis_plotly.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/ops_vis_pyvista.py` & `opstool-0.8.4/src/opstool/vis/ops_vis_pyvista.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/quick_plot.py` & `opstool-0.8.4/src/opstool/vis/quick_plot.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool/vis/save_tikz.py` & `opstool-0.8.4/src/opstool/vis/save_tikz.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/src/opstool.egg-info/PKG-INFO` & `opstool-0.8.4/src/opstool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.3
+Version: 0.8.4
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.3 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.4 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.3/src/opstool.egg-info/SOURCES.txt` & `opstool-0.8.4/src/opstool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 src/opstool/examples/shell3D.py
 src/opstool/preprocessing/__init__.py
 src/opstool/preprocessing/geom_transf.py
 src/opstool/preprocessing/load.py
 src/opstool/preprocessing/tcl2py.py
 src/opstool/preprocessing/unit_system.py
 src/opstool/preprocessing/section/__init__.py
-src/opstool/preprocessing/section/lib_sec_mesh.py
+src/opstool/preprocessing/section/sec_lib.py
 src/opstool/preprocessing/section/sec_mesh.py
 src/opstool/preprocessing/section/var_sec_mesh.py
 src/opstool/vis/__init__.py
 src/opstool/vis/_get_model_base.py
 src/opstool/vis/_plotly_base.py
 src/opstool/vis/_pyvista_base.py
 src/opstool/vis/fiber_sec_vis.py
```

### Comparing `opstool-0.8.3/tests/test_dambreak.py` & `opstool-0.8.4/tests/test_dambreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/tests/test_fiber_sec_vis.py` & `opstool-0.8.4/tests/test_fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/tests/test_model_vis.py` & `opstool-0.8.4/tests/test_model_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/tests/test_sec_analysis.py` & `opstool-0.8.4/tests/test_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/tests/test_sec_mesh.py` & `opstool-0.8.4/tests/test_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.3/tests/test_temp.py` & `opstool-0.8.4/tests/test_temp.py`

 * *Files identical despite different names*

