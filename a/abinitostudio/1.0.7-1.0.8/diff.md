# Comparing `tmp/abinitostudio-1.0.7.tar.gz` & `tmp/abinitostudio-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\abinitostudio-1.0.7.tar", last modified: Fri Aug  4 14:47:38 2023, max compression
+gzip compressed data, was "dist\abinitostudio-1.0.8.tar", last modified: Sat Aug  5 03:14:13 2023, max compression
```

## Comparing `abinitostudio-1.0.7.tar` & `abinitostudio-1.0.8.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:38.000000 abinitostudio-1.0.7/
--rw-rw-rw-   0        0        0     1084 2023-07-31 13:26:19.000000 abinitostudio-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      110 2023-08-04 14:23:19.000000 abinitostudio-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      425 2023-08-04 14:47:38.000000 abinitostudio-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2021-08-06 03:05:42.000000 abinitostudio-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.7/abinitostudio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio/calculation/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.7/abinitostudio/calculation/__init__.py
--rw-rw-rw-   0        0        0    25840 2021-08-02 00:55:16.000000 abinitostudio-1.0.7/abinitostudio/calculation/vasp_calculation.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio/images/
--rw-rw-rw-   0        0        0     7946 2021-07-08 05:28:12.000000 abinitostudio-1.0.7/abinitostudio/images/3d可视.png
--rw-rw-rw-   0        0        0     7103 2021-07-27 09:09:04.000000 abinitostudio-1.0.7/abinitostudio/images/DOS.png
--rw-rw-rw-   0        0        0     2541 2021-07-11 06:18:08.000000 abinitostudio-1.0.7/abinitostudio/images/band.png
--rw-rw-rw-   0        0        0     3332 2021-07-27 09:08:38.000000 abinitostudio-1.0.7/abinitostudio/images/band_noncal.png
--rw-rw-rw-   0        0        0     2218 2021-07-27 09:08:58.000000 abinitostudio-1.0.7/abinitostudio/images/phonin.png
--rw-rw-rw-   0        0        0     3762 2021-07-27 09:08:22.000000 abinitostudio-1.0.7/abinitostudio/images/scf.png
--rw-rw-rw-   0        0        0     2830 2021-07-27 09:08:28.000000 abinitostudio-1.0.7/abinitostudio/images/scf_noncal.png
--rw-rw-rw-   0        0        0    87766 2021-07-30 08:31:34.000000 abinitostudio-1.0.7/abinitostudio/images/startup.jpg
--rw-rw-rw-   0        0        0     6280 2021-07-10 11:22:50.000000 abinitostudio-1.0.7/abinitostudio/images/vasp.png
--rw-rw-rw-   0        0        0     2468 2021-07-27 09:09:24.000000 abinitostudio-1.0.7/abinitostudio/images/wannier.png
--rw-rw-rw-   0        0        0     5090 2021-06-28 05:59:22.000000 abinitostudio-1.0.7/abinitostudio/images/关于.png
--rw-rw-rw-   0        0        0     7333 2021-06-28 05:43:40.000000 abinitostudio-1.0.7/abinitostudio/images/关闭.png
--rw-rw-rw-   0        0        0     3636 2021-07-08 07:06:54.000000 abinitostudio-1.0.7/abinitostudio/images/层级.png
--rw-rw-rw-   0        0        0     2981 2021-06-28 07:05:38.000000 abinitostudio-1.0.7/abinitostudio/images/态密度.png
--rw-rw-rw-   0        0        0     5788 2021-07-08 06:57:38.000000 abinitostudio-1.0.7/abinitostudio/images/扩胞.png
--rw-rw-rw-   0        0        0     2034 2021-06-28 07:04:50.000000 abinitostudio-1.0.7/abinitostudio/images/投影能带.png
--rw-rw-rw-   0        0        0     6657 2021-07-10 04:25:24.000000 abinitostudio-1.0.7/abinitostudio/images/测试.png
--rw-rw-rw-   0        0        0     9896 2021-06-28 07:27:34.000000 abinitostudio-1.0.7/abinitostudio/images/结构.png
--rw-rw-rw-   0        0        0     2229 2021-06-28 07:04:44.000000 abinitostudio-1.0.7/abinitostudio/images/能带.png
--rw-rw-rw-   0        0        0    22484 2021-08-01 09:49:20.000000 abinitostudio-1.0.7/abinitostudio/images/能带图.png
--rw-rw-rw-   0        0        0     7906 2021-07-10 04:23:36.000000 abinitostudio-1.0.7/abinitostudio/images/设置.png
--rw-rw-rw-   0        0        0     2434 2021-06-28 06:32:52.000000 abinitostudio-1.0.7/abinitostudio/images/说明.png
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio/io/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.7/abinitostudio/io/__init__.py
--rw-rw-rw-   0        0        0    20951 2023-07-26 23:35:53.000000 abinitostudio-1.0.7/abinitostudio/io/vasp_io.py
--rw-rw-rw-   0        0        0    59876 2023-07-26 23:10:00.000000 abinitostudio-1.0.7/abinitostudio/myMainWindow.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio/plot/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.7/abinitostudio/plot/__init__.py
--rw-rw-rw-   0        0        0      679 2021-08-05 03:39:45.000000 abinitostudio-1.0.7/abinitostudio/plot/plot_field.py
--rw-rw-rw-   0        0        0     2330 2023-07-27 00:58:33.000000 abinitostudio-1.0.7/abinitostudio/plot/plot_vasp.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio/structure/
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.7/abinitostudio/structure/__init__.py
--rw-rw-rw-   0        0        0    35274 2023-07-26 23:37:48.000000 abinitostudio-1.0.7/abinitostudio/structure/plot_structure.py
--rw-rw-rw-   0        0        0     3343 2021-08-02 00:55:55.000000 abinitostudio-1.0.7/abinitostudio/structure/tabdialog.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio/ui/
--rw-rw-rw-   0        0        0    17348 2023-08-04 14:29:08.000000 abinitostudio-1.0.7/abinitostudio/ui/Dialog_DOS.py
--rw-rw-rw-   0        0        0    38644 2023-08-04 14:30:25.000000 abinitostudio-1.0.7/abinitostudio/ui/Dialog_PB.py
--rw-rw-rw-   0        0        0     7647 2023-08-04 14:30:24.000000 abinitostudio-1.0.7/abinitostudio/ui/Dialog_band.py
--rw-rw-rw-   0        0        0    14025 2023-08-04 14:36:48.000000 abinitostudio-1.0.7/abinitostudio/ui/UI.py
--rw-rw-rw-   0        0        0    12173 2023-08-04 14:40:14.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_setting.py
--rw-rw-rw-   0        0        0     8936 2023-08-04 14:40:18.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_test.py
--rw-rw-rw-   0        0        0    31933 2023-08-04 14:40:21.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_DOS.py
--rw-rw-rw-   0        0        0    32266 2023-08-04 14:40:19.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_band.py
--rw-rw-rw-   0        0        0    31958 2023-08-04 14:40:20.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_band_noncal.py
--rw-rw-rw-   0        0        0    25113 2023-08-04 14:40:21.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_phonon.py
--rw-rw-rw-   0        0        0    22778 2023-08-04 14:40:22.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_scf.py
--rw-rw-rw-   0        0        0    22799 2023-08-04 14:40:23.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_scf_noncal.py
--rw-rw-rw-   0        0        0     4599 2023-08-04 14:40:24.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_supercell.py
--rw-rw-rw-   0        0        0    21167 2023-08-04 14:40:25.000000 abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_wannier.py
--rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.7/abinitostudio/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio.egg-info/
--rw-rw-rw-   0        0        0      425 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2019 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-04 14:47:37.000000 abinitostudio-1.0.7/abinitostudio.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:38.000000 abinitostudio-1.0.7/doc/
--rw-rw-rw-   0        0        0   756022 2021-07-30 07:37:10.000000 abinitostudio-1.0.7/doc/说明文档.pdf
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:38.000000 abinitostudio-1.0.7/examples/
--rw-rw-rw-   0        0        0 12582333 2021-08-01 03:29:39.000000 abinitostudio-1.0.7/examples/CHGCAR
--rw-rw-rw-   0        0        0   300593 2020-07-30 07:58:04.000000 abinitostudio-1.0.7/examples/DOSCAR
--rw-rw-rw-   0        0        0   132487 2019-11-19 12:21:46.000000 abinitostudio-1.0.7/examples/EIGENVAL_CdCl
--rw-rw-rw-   0        0        0     1321 2023-04-21 12:57:23.000000 abinitostudio-1.0.7/examples/POSCAR
--rw-rw-rw-   0        0        0  2888368 2019-11-19 12:21:46.000000 abinitostudio-1.0.7/examples/PROCAR _CdCl
--rw-rw-rw-   0        0        0      291 2021-08-01 03:08:04.000000 abinitostudio-1.0.7/examples/text_ip.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 14:47:38.000000 abinitostudio-1.0.7/scripts/
--rw-rw-rw-   0        0        0      895 2023-08-04 14:32:09.000000 abinitostudio-1.0.7/scripts/appMain.py
--rw-rw-rw-   0        0        0     8707 2021-08-01 03:49:29.000000 abinitostudio-1.0.7/scripts/cal_vasp_single.py
--rw-rw-rw-   0        0        0       42 2023-08-04 14:47:38.000000 abinitostudio-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-08-04 14:47:22.000000 abinitostudio-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/
+-rw-rw-rw-   0        0        0     1084 2023-07-31 13:26:19.000000 abinitostudio-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      110 2023-08-04 14:23:19.000000 abinitostudio-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      411 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2021-08-06 03:05:42.000000 abinitostudio-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.8/abinitostudio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio/calculation/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.8/abinitostudio/calculation/__init__.py
+-rw-rw-rw-   0        0        0    25840 2021-08-02 00:55:16.000000 abinitostudio-1.0.8/abinitostudio/calculation/vasp_calculation.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/abinitostudio/images/
+-rw-rw-rw-   0        0        0     5090 2021-06-28 05:59:22.000000 abinitostudio-1.0.8/abinitostudio/images/about.png
+-rw-rw-rw-   0        0        0     2541 2021-07-11 06:18:08.000000 abinitostudio-1.0.8/abinitostudio/images/band.png
+-rw-rw-rw-   0        0        0     3332 2021-07-27 09:08:38.000000 abinitostudio-1.0.8/abinitostudio/images/band_noncal.png
+-rw-rw-rw-   0        0        0     7333 2021-06-28 05:43:40.000000 abinitostudio-1.0.8/abinitostudio/images/close.png
+-rw-rw-rw-   0        0        0     7103 2021-07-27 09:09:04.000000 abinitostudio-1.0.8/abinitostudio/images/dos.png
+-rw-rw-rw-   0        0        0     2229 2021-06-28 07:04:44.000000 abinitostudio-1.0.8/abinitostudio/images/energy_band.png
+-rw-rw-rw-   0        0        0     2218 2021-07-27 09:08:58.000000 abinitostudio-1.0.8/abinitostudio/images/phonon.png
+-rw-rw-rw-   0        0        0     2034 2021-06-28 07:04:50.000000 abinitostudio-1.0.8/abinitostudio/images/projected_bands.png
+-rw-rw-rw-   0        0        0     3762 2021-07-27 09:08:22.000000 abinitostudio-1.0.8/abinitostudio/images/scf.png
+-rw-rw-rw-   0        0        0     2830 2021-07-27 09:08:28.000000 abinitostudio-1.0.8/abinitostudio/images/scf_noncal.png
+-rw-rw-rw-   0        0        0     7906 2021-07-10 04:23:36.000000 abinitostudio-1.0.8/abinitostudio/images/setting.png
+-rw-rw-rw-   0        0        0    87766 2021-07-30 08:31:34.000000 abinitostudio-1.0.8/abinitostudio/images/startup.jpg
+-rw-rw-rw-   0        0        0     9896 2021-06-28 07:27:34.000000 abinitostudio-1.0.8/abinitostudio/images/structure.png
+-rw-rw-rw-   0        0        0     5788 2021-07-08 06:57:38.000000 abinitostudio-1.0.8/abinitostudio/images/supercell.png
+-rw-rw-rw-   0        0        0     6657 2021-07-10 04:25:24.000000 abinitostudio-1.0.8/abinitostudio/images/test.png
+-rw-rw-rw-   0        0        0     6280 2021-07-10 11:22:50.000000 abinitostudio-1.0.8/abinitostudio/images/vasp.png
+-rw-rw-rw-   0        0        0     7946 2021-07-08 05:28:12.000000 abinitostudio-1.0.8/abinitostudio/images/view_3d.png
+-rw-rw-rw-   0        0        0     2468 2021-07-27 09:09:24.000000 abinitostudio-1.0.8/abinitostudio/images/wannier.png
+-rw-rw-rw-   0        0        0     3636 2021-07-08 07:06:54.000000 abinitostudio-1.0.8/abinitostudio/images/层级.png
+-rw-rw-rw-   0        0        0    22484 2021-08-01 09:49:20.000000 abinitostudio-1.0.8/abinitostudio/images/能带图.png
+-rw-rw-rw-   0        0        0     2434 2021-06-28 06:32:52.000000 abinitostudio-1.0.8/abinitostudio/images/说明.png
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/abinitostudio/io/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.8/abinitostudio/io/__init__.py
+-rw-rw-rw-   0        0        0    20951 2023-07-26 23:35:53.000000 abinitostudio-1.0.8/abinitostudio/io/vasp_io.py
+-rw-rw-rw-   0        0        0    59876 2023-07-26 23:10:00.000000 abinitostudio-1.0.8/abinitostudio/myMainWindow.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/abinitostudio/plot/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.8/abinitostudio/plot/__init__.py
+-rw-rw-rw-   0        0        0      679 2021-08-05 03:39:45.000000 abinitostudio-1.0.8/abinitostudio/plot/plot_field.py
+-rw-rw-rw-   0        0        0     2330 2023-07-27 00:58:33.000000 abinitostudio-1.0.8/abinitostudio/plot/plot_vasp.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/abinitostudio/structure/
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.8/abinitostudio/structure/__init__.py
+-rw-rw-rw-   0        0        0    35274 2023-07-26 23:37:48.000000 abinitostudio-1.0.8/abinitostudio/structure/plot_structure.py
+-rw-rw-rw-   0        0        0     3343 2021-08-02 00:55:55.000000 abinitostudio-1.0.8/abinitostudio/structure/tabdialog.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/abinitostudio/ui/
+-rw-rw-rw-   0        0        0    17348 2023-08-04 14:29:08.000000 abinitostudio-1.0.8/abinitostudio/ui/Dialog_DOS.py
+-rw-rw-rw-   0        0        0    38644 2023-08-04 14:30:25.000000 abinitostudio-1.0.8/abinitostudio/ui/Dialog_PB.py
+-rw-rw-rw-   0        0        0     7647 2023-08-04 14:30:24.000000 abinitostudio-1.0.8/abinitostudio/ui/Dialog_band.py
+-rw-rw-rw-   0        0        0    15549 2023-08-05 00:59:36.000000 abinitostudio-1.0.8/abinitostudio/ui/UI.py
+-rw-rw-rw-   0        0        0    12173 2023-08-04 14:40:14.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_setting.py
+-rw-rw-rw-   0        0        0     8936 2023-08-04 14:40:18.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_test.py
+-rw-rw-rw-   0        0        0    31933 2023-08-04 14:40:21.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_DOS.py
+-rw-rw-rw-   0        0        0    32266 2023-08-04 14:40:19.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_band.py
+-rw-rw-rw-   0        0        0    31958 2023-08-04 14:40:20.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_band_noncal.py
+-rw-rw-rw-   0        0        0    25113 2023-08-04 14:40:21.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_phonon.py
+-rw-rw-rw-   0        0        0    22778 2023-08-04 14:40:22.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_scf.py
+-rw-rw-rw-   0        0        0    22799 2023-08-04 14:40:23.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_scf_noncal.py
+-rw-rw-rw-   0        0        0     4599 2023-08-04 14:40:24.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_supercell.py
+-rw-rw-rw-   0        0        0    21167 2023-08-04 14:40:25.000000 abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_wannier.py
+-rw-rw-rw-   0        0        0        0 2020-01-08 01:57:09.000000 abinitostudio-1.0.8/abinitostudio/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio.egg-info/
+-rw-rw-rw-   0        0        0      411 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-05 03:14:12.000000 abinitostudio-1.0.8/abinitostudio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/doc/
+-rw-rw-rw-   0        0        0   756022 2021-07-30 07:37:10.000000 abinitostudio-1.0.8/doc/说明文档.pdf
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/examples/
+-rw-rw-rw-   0        0        0 12582333 2021-08-01 03:29:39.000000 abinitostudio-1.0.8/examples/CHGCAR
+-rw-rw-rw-   0        0        0   300593 2020-07-30 07:58:04.000000 abinitostudio-1.0.8/examples/DOSCAR
+-rw-rw-rw-   0        0        0   132487 2019-11-19 12:21:46.000000 abinitostudio-1.0.8/examples/EIGENVAL_CdCl
+-rw-rw-rw-   0        0        0     1321 2023-04-21 12:57:23.000000 abinitostudio-1.0.8/examples/POSCAR
+-rw-rw-rw-   0        0        0  2888368 2019-11-19 12:21:46.000000 abinitostudio-1.0.8/examples/PROCAR _CdCl
+-rw-rw-rw-   0        0        0      291 2021-08-01 03:08:04.000000 abinitostudio-1.0.8/examples/text_ip.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/scripts/
+-rw-rw-rw-   0        0        0      895 2023-08-04 14:32:09.000000 abinitostudio-1.0.8/scripts/appMain.py
+-rw-rw-rw-   0        0        0     8707 2021-08-01 03:49:29.000000 abinitostudio-1.0.8/scripts/cal_vasp_single.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 03:14:13.000000 abinitostudio-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-08-05 03:13:51.000000 abinitostudio-1.0.8/setup.py
```

### Comparing `abinitostudio-1.0.7/LICENSE` & `abinitostudio-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/README.md` & `abinitostudio-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/calculation/vasp_calculation.py` & `abinitostudio-1.0.8/abinitostudio/calculation/vasp_calculation.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/3d可视.png` & `abinitostudio-1.0.8/abinitostudio/images/view_3d.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/DOS.png` & `abinitostudio-1.0.8/abinitostudio/images/dos.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/band.png` & `abinitostudio-1.0.8/abinitostudio/images/band.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/band_noncal.png` & `abinitostudio-1.0.8/abinitostudio/images/band_noncal.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/phonin.png` & `abinitostudio-1.0.8/abinitostudio/images/phonon.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/scf.png` & `abinitostudio-1.0.8/abinitostudio/images/scf.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/scf_noncal.png` & `abinitostudio-1.0.8/abinitostudio/images/scf_noncal.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/startup.jpg` & `abinitostudio-1.0.8/abinitostudio/images/startup.jpg`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/vasp.png` & `abinitostudio-1.0.8/abinitostudio/images/vasp.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/wannier.png` & `abinitostudio-1.0.8/abinitostudio/images/wannier.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/关于.png` & `abinitostudio-1.0.8/abinitostudio/images/about.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/关闭.png` & `abinitostudio-1.0.8/abinitostudio/images/close.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/层级.png` & `abinitostudio-1.0.8/abinitostudio/images/层级.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/扩胞.png` & `abinitostudio-1.0.8/abinitostudio/images/supercell.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/投影能带.png` & `abinitostudio-1.0.8/abinitostudio/images/projected_bands.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/测试.png` & `abinitostudio-1.0.8/abinitostudio/images/test.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/结构.png` & `abinitostudio-1.0.8/abinitostudio/images/structure.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/能带.png` & `abinitostudio-1.0.8/abinitostudio/images/energy_band.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/能带图.png` & `abinitostudio-1.0.8/abinitostudio/images/能带图.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/设置.png` & `abinitostudio-1.0.8/abinitostudio/images/setting.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/images/说明.png` & `abinitostudio-1.0.8/abinitostudio/images/说明.png`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/io/vasp_io.py` & `abinitostudio-1.0.8/abinitostudio/io/vasp_io.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/myMainWindow.py` & `abinitostudio-1.0.8/abinitostudio/myMainWindow.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/plot/plot_field.py` & `abinitostudio-1.0.8/abinitostudio/plot/plot_field.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/plot/plot_vasp.py` & `abinitostudio-1.0.8/abinitostudio/plot/plot_vasp.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/structure/plot_structure.py` & `abinitostudio-1.0.8/abinitostudio/structure/plot_structure.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/structure/tabdialog.py` & `abinitostudio-1.0.8/abinitostudio/structure/tabdialog.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/Dialog_DOS.py` & `abinitostudio-1.0.8/abinitostudio/ui/Dialog_DOS.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/Dialog_PB.py` & `abinitostudio-1.0.8/abinitostudio/ui/Dialog_PB.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/Dialog_band.py` & `abinitostudio-1.0.8/abinitostudio/ui/Dialog_band.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 # Form implementation generated from reading ui file 'UI.ui'
 #
 # Created by: PyQt5 UI code generator 5.10
 #
 # WARNING! All changes made in this file will be lost!
 
 from PyQt5 import QtCore, QtGui, QtWidgets
+import os
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.resize(553, 448)
         icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap("abinitostudio/images/结构.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        
+        script_dir = os.path.dirname(__file__) #<-- absolute dir the script is in
+        
+        rel_path = "../images/structure.png"
+        path_tmp = os.path.join(script_dir, rel_path)        
+        icon.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         MainWindow.setWindowIcon(icon)
         MainWindow.setStyleSheet("QPushButton{\ncolor:rgb(255, 0, 0);\nfont: 12pt \"宋体\";\n}\n\n"
                                  "QLabel{\ncolor:rgb(0, 85, 255);\nfont: 12pt \"宋体\";\n}\n\n"
                                  "QCheckBox{\ncolor:rgb(0, 85, 255);\nfont: 12pt \"宋体\";\n}\n\n"
                                  "QGroupBox{\ncolor:rgb(170, 85, 255);\nfont: 12pt \"宋体\";\n}\n\n"
                                  "QTextBrowser{\nfont: 12pt \"宋体\";\n}\n\n"
                                  "QLineEdit{\nfont: 12pt \"宋体\";\n}\n\n")
@@ -70,15 +76,15 @@
         self.menuHelp.setObjectName("menuHelp")
 
         self.menu = QtWidgets.QMenu(self.menubar)
         self.menu.setObjectName("menu")
 
         self.menuVASP = QtWidgets.QMenu(self.menu)
         icon1 = QtGui.QIcon()
-        icon1.addPixmap(QtGui.QPixmap("abinitostudio/images/vasp.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon1.addPixmap(QtGui.QPixmap("../images/vasp.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.menuVASP.setIcon(icon1)
         self.menuVASP.setObjectName("menuVASP")
 
         self.menu_2 = QtWidgets.QMenu(self.menubar)
         self.menu_2.setObjectName("menu_2")
 
         self.menu_4 = QtWidgets.QMenu(self.menubar)
@@ -87,117 +93,155 @@
         MainWindow.setMenuBar(self.menubar)
         self.toolBar = QtWidgets.QToolBar(MainWindow)
         self.toolBar.setObjectName("toolBar")
         MainWindow.addToolBar(QtCore.Qt.TopToolBarArea, self.toolBar)
 
         self.actionclose = QtWidgets.QAction(MainWindow)
         icon2 = QtGui.QIcon()
-        icon2.addPixmap(QtGui.QPixmap("abinitostudio/images/关闭.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        
+        rel_path = "../images/close.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon2.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionclose.setIcon(icon2)
         self.actionclose.setObjectName("actionclose")
 
         self.actionband = QtWidgets.QAction(MainWindow)
         icon3 = QtGui.QIcon()
-        icon3.addPixmap(QtGui.QPixmap("abinitostudio/images/能带.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        
+        rel_path = "../images/energy_band.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon3.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionband.setIcon(icon3)
         self.actionband.setObjectName("actionband")
 
         self.actionprojectionband = QtWidgets.QAction(MainWindow)
         icon4 = QtGui.QIcon()
-        icon4.addPixmap(QtGui.QPixmap("abinitostudio/images/态密度.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/dos.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon4.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionprojectionband.setIcon(icon4)
         self.actionprojectionband.setObjectName("actionprojectionband")
 
         self.actiondos = QtWidgets.QAction(MainWindow)
         icon5 = QtGui.QIcon()
-        icon5.addPixmap(QtGui.QPixmap("abinitostudio/images/投影能带.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/projected_bands.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon5.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actiondos.setIcon(icon5)
         self.actiondos.setObjectName("actiondos")
 
         self.actionchgcar = QtWidgets.QAction(MainWindow)
         icon5 = QtGui.QIcon()
-        icon5.addPixmap(QtGui.QPixmap("abinitostudio/images/投影能带.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/projected_bands.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon5.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionchgcar.setIcon(icon5)
         self.actionchgcar.setObjectName("actionCHGCAR")
 
         self.actioninstruction = QtWidgets.QAction(MainWindow)
         icon6 = QtGui.QIcon()
-        icon6.addPixmap(QtGui.QPixmap("abinitostudio/images/说明.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/about.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon6.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actioninstruction.setIcon(icon6)
         self.actioninstruction.setObjectName("actioninstruction")
 
         self.actionabout = QtWidgets.QAction(MainWindow)
         icon7 = QtGui.QIcon()
-        icon7.addPixmap(QtGui.QPixmap("abinitostudio/images/关于.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/about.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon7.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionabout.setIcon(icon7)
         self.actionabout.setObjectName("actionabout")
 
         self.actionsupercell = QtWidgets.QAction(MainWindow)
         icon8 = QtGui.QIcon()
-        icon8.addPixmap(QtGui.QPixmap("abinitostudio/images/扩胞.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/supercell.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon8.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionsupercell.setIcon(icon8)
         self.actionsupercell.setObjectName("actionsupercell")
 
         self.actionsetting = QtWidgets.QAction(MainWindow)
         icon9 = QtGui.QIcon()
-        icon9.addPixmap(QtGui.QPixmap("abinitostudio/images/设置.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/setting.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon9.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionsetting.setIcon(icon9)
         self.actionsetting.setObjectName("actionsetting")
 
         self.actiontest = QtWidgets.QAction(MainWindow)
         icon10 = QtGui.QIcon()
-        icon10.addPixmap(QtGui.QPixmap("abinitostudio/images/测试.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/test.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon10.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actiontest.setIcon(icon10)
         self.actiontest.setObjectName("actiontest")
 
         self.actionvisual = QtWidgets.QAction(MainWindow)
         icon11 = QtGui.QIcon()
-        icon11.addPixmap(QtGui.QPixmap("abinitostudio/images/3d可视.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/view_3d.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon11.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionvisual.setIcon(icon11)
         self.actionvisual.setObjectName("actionvisual")
 
         self.actionbands = QtWidgets.QAction(MainWindow)
         icon12 = QtGui.QIcon()
-        icon12.addPixmap(QtGui.QPixmap("abinitostudio/images/band.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/band.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon12.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionbands.setIcon(icon12)
         self.actionbands.setObjectName("actionbands")
 
         self.actionscf = QtWidgets.QAction(MainWindow)
         icon13 = QtGui.QIcon()
-        icon13.addPixmap(QtGui.QPixmap("abinitostudio/images/scf.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/scf.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon13.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionscf.setIcon(icon13)
         self.actionscf.setObjectName("actionscf")
 
         self.actionscf_noncal = QtWidgets.QAction(MainWindow)
         icon14 = QtGui.QIcon()
-        icon14.addPixmap(QtGui.QPixmap("abinitostudio/images/scf_noncal.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/scf_noncal.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon14.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionscf_noncal.setIcon(icon14)
         self.actionscf_noncal.setObjectName("actionscf_noncal")
 
         self.actionband_noncal = QtWidgets.QAction(MainWindow)
         icon15 = QtGui.QIcon()
-        icon15.addPixmap(QtGui.QPixmap("abinitostudio/images/band_noncal.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/band_noncal.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon15.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionband_noncal.setIcon(icon15)
         self.actionband_noncal.setObjectName("actionband_noncal")
 
         self.actionDOS = QtWidgets.QAction(MainWindow)
         icon16 = QtGui.QIcon()
-        icon16.addPixmap(QtGui.QPixmap("abinitostudio/images/DOS.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/dos.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon16.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionDOS.setIcon(icon16)
         self.actionDOS.setObjectName("actionDOS")
 
         self.actionphonon = QtWidgets.QAction(MainWindow)
         icon17 = QtGui.QIcon()
-        icon17.addPixmap(QtGui.QPixmap("abinitostudio/images/phonin.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/phonon.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon17.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionphonon.setIcon(icon17)
         self.actionphonon.setObjectName("actionphonon")
 
         self.actionwannier = QtWidgets.QAction(MainWindow)
         icon18 = QtGui.QIcon()
-        icon18.addPixmap(QtGui.QPixmap("abinitostudio/images/wannier.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        rel_path = "../images/wannier.png"
+        path_tmp = os.path.join(script_dir, rel_path)
+        icon18.addPixmap(QtGui.QPixmap(path_tmp), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         self.actionwannier.setIcon(icon18)
         self.actionwannier.setObjectName("actionwannier")
 
         self.menuFile.addAction(self.actionvisual)
         self.menuFile.addAction(self.actionclose)
 
         self.menuOperation.addAction(self.actionband)
```

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_setting.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_setting.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_test.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_test.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_DOS.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_DOS.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_band.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_band.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_band_noncal.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_band_noncal.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_phonon.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_phonon.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_scf.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_scf.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_scf_noncal.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_scf_noncal.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_supercell.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_supercell.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio/ui/UI_vasp_wannier.py` & `abinitostudio-1.0.8/abinitostudio/ui/UI_vasp_wannier.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/abinitostudio.egg-info/SOURCES.txt` & `abinitostudio-1.0.8/abinitostudio.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,35 +7,34 @@
 abinitostudio.egg-info/PKG-INFO
 abinitostudio.egg-info/SOURCES.txt
 abinitostudio.egg-info/dependency_links.txt
 abinitostudio.egg-info/requires.txt
 abinitostudio.egg-info/top_level.txt
 abinitostudio/calculation/__init__.py
 abinitostudio/calculation/vasp_calculation.py
-abinitostudio/images/3d可视.png
-abinitostudio/images/DOS.png
+abinitostudio/images/about.png
 abinitostudio/images/band.png
 abinitostudio/images/band_noncal.png
-abinitostudio/images/phonin.png
+abinitostudio/images/close.png
+abinitostudio/images/dos.png
+abinitostudio/images/energy_band.png
+abinitostudio/images/phonon.png
+abinitostudio/images/projected_bands.png
 abinitostudio/images/scf.png
 abinitostudio/images/scf_noncal.png
+abinitostudio/images/setting.png
 abinitostudio/images/startup.jpg
+abinitostudio/images/structure.png
+abinitostudio/images/supercell.png
+abinitostudio/images/test.png
 abinitostudio/images/vasp.png
+abinitostudio/images/view_3d.png
 abinitostudio/images/wannier.png
-abinitostudio/images/关于.png
-abinitostudio/images/关闭.png
 abinitostudio/images/层级.png
-abinitostudio/images/态密度.png
-abinitostudio/images/扩胞.png
-abinitostudio/images/投影能带.png
-abinitostudio/images/测试.png
-abinitostudio/images/结构.png
-abinitostudio/images/能带.png
 abinitostudio/images/能带图.png
-abinitostudio/images/设置.png
 abinitostudio/images/说明.png
 abinitostudio/io/__init__.py
 abinitostudio/io/vasp_io.py
 abinitostudio/plot/__init__.py
 abinitostudio/plot/plot_field.py
 abinitostudio/plot/plot_vasp.py
 abinitostudio/structure/__init__.py
```

### Comparing `abinitostudio-1.0.7/doc/说明文档.pdf` & `abinitostudio-1.0.8/doc/说明文档.pdf`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/examples/CHGCAR` & `abinitostudio-1.0.8/examples/CHGCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/examples/DOSCAR` & `abinitostudio-1.0.8/examples/DOSCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/examples/EIGENVAL_CdCl` & `abinitostudio-1.0.8/examples/EIGENVAL_CdCl`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/examples/POSCAR` & `abinitostudio-1.0.8/examples/POSCAR`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/examples/PROCAR _CdCl` & `abinitostudio-1.0.8/examples/PROCAR _CdCl`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/scripts/appMain.py` & `abinitostudio-1.0.8/scripts/appMain.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/scripts/cal_vasp_single.py` & `abinitostudio-1.0.8/scripts/cal_vasp_single.py`

 * *Files identical despite different names*

### Comparing `abinitostudio-1.0.7/setup.py` & `abinitostudio-1.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 
 setup(name="abinitostudio",
-    version="1.0.7",
+    version="1.0.8",
     description="A studio for first-principles calculations.",
     long_description="This is a long description.",
     author="Pan Zhou, Xin Lu and Li Zhongsun",
     author_email="zhoupan71234@xtu.edu.cn",
     classifiers=["Development Status :: 3 - Alpha",'Programming Language :: Python',],
 #    packages=find_packages()
     packages=['abinitostudio',
```

