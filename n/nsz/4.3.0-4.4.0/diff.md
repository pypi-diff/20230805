# Comparing `tmp/nsz-4.3.0.tar.gz` & `tmp/nsz-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsz-4.3.0.tar", last modified: Thu Jul  6 13:50:01 2023, max compression
+gzip compressed data, was "nsz-4.4.0.tar", last modified: Sat Aug  5 09:42:14 2023, max compression
```

## Comparing `nsz-4.3.0.tar` & `nsz-4.4.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.938816 nsz-4.3.0/
--rw-rw-rw-   0        0        0     1400 2020-08-11 01:14:07.000000 nsz-4.3.0/LICENSE
--rw-rw-rw-   0        0        0    14352 2023-07-06 13:50:01.937806 nsz-4.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    13770 2023-07-06 12:07:20.000000 nsz-4.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.831800 nsz-4.3.0/nsz/
--rw-rw-rw-   0        0        0    10343 2023-06-22 23:31:37.000000 nsz-4.3.0/nsz/BlockCompressor.py
--rw-rw-rw-   0        0        0     2302 2020-09-04 20:34:54.000000 nsz-4.3.0/nsz/BlockDecompressorReader.py
--rw-rw-rw-   0        0        0     2833 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/ExtractTitlekeys.py
--rw-rw-rw-   0        0        0     6804 2022-12-08 20:07:11.000000 nsz-4.3.0/nsz/FileExistingChecks.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.869791 nsz-4.3.0/nsz/Fs/
--rw-rw-rw-   0        0        0     5552 2020-09-05 17:02:35.000000 nsz-4.3.0/nsz/Fs/BaseFs.py
--rw-rw-rw-   0        0        0     7491 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Bktr.py
--rw-rw-rw-   0        0        0     2142 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Cnmt.py
--rw-rw-rw-   0        0        0    14879 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/File.py
--rw-rw-rw-   0        0        0     4699 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Hfs0.py
--rw-rw-rw-   0        0        0     1395 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Ivfc.py
--rw-rw-rw-   0        0        0    18339 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Nacp.py
--rw-rw-rw-   0        0        0     8911 2020-09-05 18:10:42.000000 nsz-4.3.0/nsz/Fs/Nca.py
--rw-rw-rw-   0        0        0    13186 2022-10-03 17:43:34.000000 nsz-4.3.0/nsz/Fs/Nsp.py
--rw-rw-rw-   0        0        0     7167 2023-07-05 16:25:07.000000 nsz-4.3.0/nsz/Fs/Pfs0.py
--rw-rw-rw-   0        0        0     1783 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Rom.py
--rw-rw-rw-   0        0        0     6443 2023-07-05 22:08:01.000000 nsz-4.3.0/nsz/Fs/Ticket.py
--rw-rw-rw-   0        0        0      552 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Type.py
--rw-rw-rw-   0        0        0     9553 2020-09-02 00:56:55.000000 nsz-4.3.0/nsz/Fs/Xci.py
--rw-rw-rw-   0        0        0      908 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/__init__.py
--rw-rw-rw-   0        0        0      743 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Header.py
--rw-rw-rw-   0        0        0     3942 2022-12-08 20:07:11.000000 nsz-4.3.0/nsz/IndependentNczDecompressor.py
--rw-rw-rw-   0        0        0    11010 2023-07-06 11:32:26.000000 nsz-4.3.0/nsz/NszDecompressor.py
--rw-rw-rw-   0        0        0     6900 2023-07-06 11:45:03.000000 nsz-4.3.0/nsz/ParseArguments.py
--rw-rw-rw-   0        0        0     1532 2022-12-08 20:07:11.000000 nsz-4.3.0/nsz/PathTools.py
--rw-rw-rw-   0        0        0      366 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/SectionFs.py
--rw-rw-rw-   0        0        0     7184 2023-06-22 23:31:37.000000 nsz-4.3.0/nsz/SolidCompressor.py
--rw-rw-rw-   0        0        0      428 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/ThreadSafeCounter.py
--rw-rw-rw-   0        0        0    12142 2023-07-06 12:27:31.000000 nsz-4.3.0/nsz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.890814 nsz-4.3.0/nsz/gui/
--rw-rw-rw-   0        0        0      940 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/AboutDialog.py
--rw-rw-rw-   0        0        0     1478 2020-08-30 22:49:38.000000 nsz-4.3.0/nsz/gui/DraggableScrollbar.py
--rw-rw-rw-   0        0        0     1602 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/FileDialogs.py
--rw-rw-rw-   0        0        0     5767 2020-12-24 23:45:55.000000 nsz-4.3.0/nsz/gui/GameList.py
--rw-rw-rw-   0        0        0      159 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/GuiPath.py
--rw-rw-rw-   0        0        0     2685 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/Hyperlink.py
--rw-rw-rw-   0        0        0     1650 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/KivyOnTop.py
--rw-rw-rw-   0        0        0     6291 2023-07-06 12:04:52.000000 nsz-4.3.0/nsz/gui/NSZ_GUI.py
--rw-rw-rw-   0        0        0     2862 2023-04-11 08:37:41.000000 nsz-4.3.0/nsz/gui/RootWidget.py
--rw-rw-rw-   0        0        0     1360 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/SettingScrollOptions.py
--rw-rw-rw-   0        0        0     1434 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/ShaderWidget.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.897798 nsz-4.3.0/nsz/gui/fonts/
--rw-rw-rw-   0        0        0  1754936 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/fonts/MPLUS1p-Medium.ttf
--rw-rw-rw-   0        0        0     4393 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/fonts/OFL.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.905801 nsz-4.3.0/nsz/gui/json/
--rw-rw-rw-   0        0        0     1859 2023-07-06 11:58:43.000000 nsz-4.3.0/nsz/gui/json/settings_advanced.json
--rw-rw-rw-   0        0        0     2112 2023-07-06 11:58:59.000000 nsz-4.3.0/nsz/gui/json/settings_basic.json
--rw-rw-rw-   0        0        0      616 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/json/settings_tools.json
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.917801 nsz-4.3.0/nsz/gui/layout/
--rw-rw-rw-   0        0        0     1763 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/AboutDialog.kv
--rw-rw-rw-   0        0        0      113 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/layout/GUI.kv
--rw-rw-rw-   0        0        0     2583 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/GameList.kv
--rw-rw-rw-   0        0        0      352 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/Hyperlink.kv
--rw-rw-rw-   0        0        0     1263 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/layout/OpenFileDialog.kv
--rw-rw-rw-   0        0        0     2365 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/RootWidget.kv
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.919813 nsz-4.3.0/nsz/gui/shaders/
--rw-rw-rw-   0        0        0      599 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/shaders/plasma.shader
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.921803 nsz-4.3.0/nsz/gui/txt/
--rw-rw-rw-   0        0        0     1574 2023-07-06 10:16:02.000000 nsz-4.3.0/nsz/gui/txt/license.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.930807 nsz-4.3.0/nsz/nut/
--rw-rw-rw-   0        0        0     1066 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/Hex.py
--rw-rw-rw-   0        0        0     6092 2023-07-06 13:10:18.000000 nsz-4.3.0/nsz/nut/Keys.py
--rw-rw-rw-   0        0        0      621 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/Print.py
--rw-rw-rw-   0        0        0     1417 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/Titles.py
--rw-rw-rw-   0        0        0    25572 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/aes128.py
--rw-rw-rw-   0        0        0     3957 2021-06-26 23:57:40.000000 nsz-4.3.0/nsz/undupe.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.935815 nsz-4.3.0/nsz.egg-info/
--rw-rw-rw-   0        0        0     1289 2023-07-06 13:50:01.000000 nsz-4.3.0/nsz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      594 2022-10-03 17:43:34.000000 nsz-4.3.0/nsz.py
--rw-rw-rw-   0        0        0       42 2023-07-06 13:50:01.938816 nsz-4.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-07-06 10:41:21.000000 nsz-4.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.259263 nsz-4.4.0/
+-rw-rw-rw-   0        0        0     1400 2020-08-11 01:14:07.000000 nsz-4.4.0/LICENSE
+-rw-rw-rw-   0        0        0    14804 2023-08-05 09:42:14.258276 nsz-4.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14222 2023-08-05 09:40:10.000000 nsz-4.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:13.943325 nsz-4.4.0/nsz/
+-rw-rw-rw-   0        0        0    10361 2023-08-05 09:40:10.000000 nsz-4.4.0/nsz/BlockCompressor.py
+-rw-rw-rw-   0        0        0     2302 2020-09-04 20:34:54.000000 nsz-4.4.0/nsz/BlockDecompressorReader.py
+-rw-rw-rw-   0        0        0     2833 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/ExtractTitlekeys.py
+-rw-rw-rw-   0        0        0     6804 2022-12-08 20:07:11.000000 nsz-4.4.0/nsz/FileExistingChecks.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.031726 nsz-4.4.0/nsz/Fs/
+-rw-rw-rw-   0        0        0     5645 2023-07-21 22:16:06.000000 nsz-4.4.0/nsz/Fs/BaseFs.py
+-rw-rw-rw-   0        0        0     7491 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Fs/Bktr.py
+-rw-rw-rw-   0        0        0     2142 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Fs/Cnmt.py
+-rw-rw-rw-   0        0        0    14936 2023-07-21 22:16:06.000000 nsz-4.4.0/nsz/Fs/File.py
+-rw-rw-rw-   0        0        0     4594 2023-08-05 09:40:10.000000 nsz-4.4.0/nsz/Fs/Hfs0.py
+-rw-rw-rw-   0        0        0     1395 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Fs/Ivfc.py
+-rw-rw-rw-   0        0        0    18339 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Fs/Nacp.py
+-rw-rw-rw-   0        0        0     8911 2020-09-05 18:10:42.000000 nsz-4.4.0/nsz/Fs/Nca.py
+-rw-rw-rw-   0        0        0    13078 2023-08-05 09:40:10.000000 nsz-4.4.0/nsz/Fs/Nsp.py
+-rw-rw-rw-   0        0        0     6890 2023-08-05 09:40:10.000000 nsz-4.4.0/nsz/Fs/Pfs0.py
+-rw-rw-rw-   0        0        0     1783 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Fs/Rom.py
+-rw-rw-rw-   0        0        0     6443 2023-07-05 22:08:01.000000 nsz-4.4.0/nsz/Fs/Ticket.py
+-rw-rw-rw-   0        0        0      552 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Fs/Type.py
+-rw-rw-rw-   0        0        0     9553 2020-09-02 00:56:55.000000 nsz-4.4.0/nsz/Fs/Xci.py
+-rw-rw-rw-   0        0        0      908 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Fs/__init__.py
+-rw-rw-rw-   0        0        0      743 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/Header.py
+-rw-rw-rw-   0        0        0     3942 2022-12-08 20:07:11.000000 nsz-4.4.0/nsz/IndependentNczDecompressor.py
+-rw-rw-rw-   0        0        0    11010 2023-07-06 11:32:26.000000 nsz-4.4.0/nsz/NszDecompressor.py
+-rw-rw-rw-   0        0        0     6900 2023-07-06 11:45:03.000000 nsz-4.4.0/nsz/ParseArguments.py
+-rw-rw-rw-   0        0        0     1532 2022-12-08 20:07:11.000000 nsz-4.4.0/nsz/PathTools.py
+-rw-rw-rw-   0        0        0      366 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/SectionFs.py
+-rw-rw-rw-   0        0        0     7184 2023-06-22 23:31:37.000000 nsz-4.4.0/nsz/SolidCompressor.py
+-rw-rw-rw-   0        0        0      410 2023-08-05 09:40:10.000000 nsz-4.4.0/nsz/ThreadSafeCounter.py
+-rw-rw-rw-   0        0        0    12194 2023-08-05 09:40:10.000000 nsz-4.4.0/nsz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.114524 nsz-4.4.0/nsz/gui/
+-rw-rw-rw-   0        0        0      940 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/AboutDialog.py
+-rw-rw-rw-   0        0        0     1478 2020-08-30 22:49:38.000000 nsz-4.4.0/nsz/gui/DraggableScrollbar.py
+-rw-rw-rw-   0        0        0     1602 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/FileDialogs.py
+-rw-rw-rw-   0        0        0     5767 2020-12-24 23:45:55.000000 nsz-4.4.0/nsz/gui/GameList.py
+-rw-rw-rw-   0        0        0      159 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/GuiPath.py
+-rw-rw-rw-   0        0        0     2685 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/Hyperlink.py
+-rw-rw-rw-   0        0        0     1650 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/KivyOnTop.py
+-rw-rw-rw-   0        0        0     6291 2023-08-05 09:40:10.000000 nsz-4.4.0/nsz/gui/NSZ_GUI.py
+-rw-rw-rw-   0        0        0     2862 2023-04-11 08:37:41.000000 nsz-4.4.0/nsz/gui/RootWidget.py
+-rw-rw-rw-   0        0        0     1360 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/SettingScrollOptions.py
+-rw-rw-rw-   0        0        0     1434 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/ShaderWidget.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.133541 nsz-4.4.0/nsz/gui/fonts/
+-rw-rw-rw-   0        0        0  1754936 2020-08-31 22:31:18.000000 nsz-4.4.0/nsz/gui/fonts/MPLUS1p-Medium.ttf
+-rw-rw-rw-   0        0        0     4393 2020-08-31 22:31:18.000000 nsz-4.4.0/nsz/gui/fonts/OFL.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.155728 nsz-4.4.0/nsz/gui/json/
+-rw-rw-rw-   0        0        0     1859 2023-07-06 11:58:43.000000 nsz-4.4.0/nsz/gui/json/settings_advanced.json
+-rw-rw-rw-   0        0        0     2112 2023-07-06 11:58:59.000000 nsz-4.4.0/nsz/gui/json/settings_basic.json
+-rw-rw-rw-   0        0        0      616 2020-08-31 22:31:18.000000 nsz-4.4.0/nsz/gui/json/settings_tools.json
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.200804 nsz-4.4.0/nsz/gui/layout/
+-rw-rw-rw-   0        0        0     1763 2020-08-31 22:31:18.000000 nsz-4.4.0/nsz/gui/layout/AboutDialog.kv
+-rw-rw-rw-   0        0        0      113 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/layout/GUI.kv
+-rw-rw-rw-   0        0        0     2583 2020-08-31 22:31:18.000000 nsz-4.4.0/nsz/gui/layout/GameList.kv
+-rw-rw-rw-   0        0        0      352 2020-08-31 22:31:18.000000 nsz-4.4.0/nsz/gui/layout/Hyperlink.kv
+-rw-rw-rw-   0        0        0     1263 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/layout/OpenFileDialog.kv
+-rw-rw-rw-   0        0        0     2365 2020-08-31 22:31:18.000000 nsz-4.4.0/nsz/gui/layout/RootWidget.kv
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.206812 nsz-4.4.0/nsz/gui/shaders/
+-rw-rw-rw-   0        0        0      599 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/gui/shaders/plasma.shader
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.214839 nsz-4.4.0/nsz/gui/txt/
+-rw-rw-rw-   0        0        0     1574 2023-07-06 10:16:02.000000 nsz-4.4.0/nsz/gui/txt/license.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.254269 nsz-4.4.0/nsz/nut/
+-rw-rw-rw-   0        0        0     1066 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/nut/Hex.py
+-rw-rw-rw-   0        0        0     6092 2023-07-06 13:10:18.000000 nsz-4.4.0/nsz/nut/Keys.py
+-rw-rw-rw-   0        0        0      621 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/nut/Print.py
+-rw-rw-rw-   0        0        0     1417 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/nut/Titles.py
+-rw-rw-rw-   0        0        0    25572 2020-08-11 01:14:07.000000 nsz-4.4.0/nsz/nut/aes128.py
+-rw-rw-rw-   0        0        0     3957 2021-06-26 23:57:40.000000 nsz-4.4.0/nsz/undupe.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:14.256276 nsz-4.4.0/nsz.egg-info/
+-rw-rw-rw-   0        0        0     1289 2023-08-05 09:42:13.000000 nsz-4.4.0/nsz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      594 2022-10-03 17:43:34.000000 nsz-4.4.0/nsz.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:42:14.259263 nsz-4.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-08-05 09:40:10.000000 nsz-4.4.0/setup.py
```

### Comparing `nsz-4.3.0/LICENSE` & `nsz-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/PKG-INFO` & `nsz-4.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsz
-Version: 4.3.0
+Version: 4.4.0
 Summary: NSZ - Homebrew compatible NSP/XCI compressor/decompressor
 Home-page: https://github.com/nicoboss/nsz
 Author: Nico Bosshard
 Author-email: nico@bosshome.ch
 Maintainer: Nico Bosshard
 Maintainer-email: nico@bosshome.ch
 Keywords: nsz,xcz,ncz,nsp,xci,nca,Switch
@@ -41,14 +41,22 @@
 ### PIP Package
 Use the following command to install the console-only version:\
 `pip3 install --upgrade nsz`
 
 Use the following command to install the GUI version:\
 `pip3 install --upgrade nsz[gui]`
 
+### Android
+1. Install "Pydroid 3" and the "Pydroid repository plugin" from the Play Store
+2. Open "Pydroid 3" and navigate to "Pip"
+3. Enter "nsz" and unselect "use prebuild" then press install
+4. Navigate to "Terminal" to use the "nsz" command
+5. The first time it will tell you where to copy your prod.keys which you should do using the "cp" command
+6. Use any command line arguments you want like "nsz -D file.nsz" to decompress your game
+
 ### Running from source
 The tool can also be run by cloning the repository, installing the requirements and then executing nsz using `python3 nsz.py`
 
 Use the following command to install the console-only versions requirements:\
 `pip3 install -r requirements.txt`
 
 Use the following command to install the GUI versions requirements:\
```

### Comparing `nsz-4.3.0/README.md` & `nsz-4.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 ### PIP Package
 Use the following command to install the console-only version:\
 `pip3 install --upgrade nsz`
 
 Use the following command to install the GUI version:\
 `pip3 install --upgrade nsz[gui]`
 
+### Android
+1. Install "Pydroid 3" and the "Pydroid repository plugin" from the Play Store
+2. Open "Pydroid 3" and navigate to "Pip"
+3. Enter "nsz" and unselect "use prebuild" then press install
+4. Navigate to "Terminal" to use the "nsz" command
+5. The first time it will tell you where to copy your prod.keys which you should do using the "cp" command
+6. Use any command line arguments you want like "nsz -D file.nsz" to decompress your game
+
 ### Running from source
 The tool can also be run by cloning the repository, installing the requirements and then executing nsz using `python3 nsz.py`
 
 Use the following command to install the console-only versions requirements:\
 `pip3 install -r requirements.txt`
 
 Use the following command to install the GUI versions requirements:\
```

### Comparing `nsz-4.3.0/nsz/BlockCompressor.py` & `nsz-4.4.0/nsz/BlockCompressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 	CHUNK_SZ = 0x100000
 	UNCOMPRESSABLE_HEADER_SIZE = 0x4000
 	if blockSizeExponent < 14 or blockSizeExponent > 32:
 		raise ValueError("Block size must be between 14 and 32")
 	blockSize = 2**blockSizeExponent
 	manager = Manager()
 	results = manager.list()
-	readyForWork = Counter(0)
-	pleaseKillYourself = Counter(0)
+	readyForWork = Counter(manager, 0)
+	pleaseKillYourself = Counter(manager, 0)
 	TasksPerChunk = 209715200//blockSize
 	for i in range(TasksPerChunk):
 		results.append(b"")
 	pool = []
 	work = manager.Queue(threads)
 	
 	for i in range(threads):
```

### Comparing `nsz-4.3.0/nsz/BlockDecompressorReader.py` & `nsz-4.4.0/nsz/BlockDecompressorReader.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/ExtractTitlekeys.py` & `nsz-4.4.0/nsz/ExtractTitlekeys.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/FileExistingChecks.py` & `nsz-4.4.0/nsz/FileExistingChecks.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/BaseFs.py` & `nsz-4.4.0/nsz/Fs/BaseFs.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 		self.buffer = buffer
 		self.sectionStart = 0
 		self.fsType = None
 		self.cryptoType = None
 		self.size = 0
 		self.cryptoCounter = None
 		self.magic = None
+		self._headerSize = None
 		self.bktrRelocation = None
 		self.bktrSubsection = None
 			
 		self.files = []
 		
 		if buffer:
 			self.buffer = buffer
@@ -147,14 +148,15 @@
 	
 	def printInfo(self, maxDepth = 3, indent = 0):
 		tabs = '\t' * indent
 		Print.info(tabs + 'magic = ' + str(self.magic))
 		Print.info(tabs + 'fsType = ' + str(self.fsType))
 		Print.info(tabs + 'cryptoType = ' + str(self.cryptoType))
 		Print.info(tabs + 'size = ' + str(self.size))
+		Print.info(tabs + 'headerSize = %s' % (str(self._headerSize)))
 		Print.info(tabs + 'offset = %s - (%s)' % (str(self.offset), str(self.sectionStart)))
 		if self.cryptoCounter:
 			Print.info(tabs + 'cryptoCounter = ' + str(hx(self.cryptoCounter)))
 			
 		if self.cryptoKey:
 			Print.info(tabs + 'cryptoKey = ' + str(hx(self.cryptoKey)))
```

### Comparing `nsz-4.3.0/nsz/Fs/Bktr.py` & `nsz-4.4.0/nsz/Fs/Bktr.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/Cnmt.py` & `nsz-4.4.0/nsz/Fs/Cnmt.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/File.py` & `nsz-4.4.0/nsz/Fs/File.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
 		return bytes(ctr)
 		
 	def printInfo(self, maxDepth = 3, indent = 0):
 		tabs = '\t' * indent
 		if self._path:
 			Print.info('%sFile Path: %s' % (tabs, self._path))
 		Print.info('%sFile Size: %s' % (tabs, self.size))
+		Print.info('%sFile Offset: %s' % (tabs, self.offset))
 
 	def sha256(self):
 		hash = hashlib.sha256()
 	
 		self.rewind()
 
 		if self.size >= 10000:
```

### Comparing `nsz-4.3.0/nsz/Fs/Hfs0.py` & `nsz-4.4.0/nsz/Fs/Hfs0.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,21 +64,19 @@
 			self.write(self.getHeader())
 			super(Hfs0Stream, self).close()
 
 	def getHeader(self):
 		stringTable = '\x00'.join(file['name'] for file in self.files)
 		
 		headerSize = 0x10 + len(self.files) * 0x40 + len(stringTable)
-		remainder = 0x10 - headerSize % 0x10
-		headerSize += remainder
 	
 		h = b''
 		h += b'HFS0'
 		h += len(self.files).to_bytes(4, byteorder='little')
-		h += (len(stringTable)+remainder).to_bytes(4, byteorder='little')
+		h += (len(stringTable)).to_bytes(4, byteorder='little')
 		h += b'\x00\x00\x00\x00'
 		
 		stringOffset = 0
 
 		for f in self.files:
 			sizeOfHashedRegion = 0x200 if 0x200 < f['size'] else f['size']
 
@@ -88,15 +86,14 @@
 			h += sizeOfHashedRegion.to_bytes(4, byteorder='little')
 			h += b'\x00' * 8
 			h += b'\x00' * 0x20 # sha256 hash of region
 			
 			stringOffset += len(f['name']) + 1
 			
 		h += stringTable.encode()
-		h += remainder * b'\x00'
 		
 		return h
 
 class Hfs0(Pfs0):
 	def __init__(self, buffer, path = None, mode = None, cryptoType = -1, cryptoKey = -1, cryptoCounter = -1):
 		super(Hfs0, self).__init__(buffer, path, mode, cryptoType, cryptoKey, cryptoCounter)
```

### Comparing `nsz-4.3.0/nsz/Fs/Ivfc.py` & `nsz-4.4.0/nsz/Fs/Ivfc.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/Nacp.py` & `nsz-4.4.0/nsz/Fs/Nacp.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/Nca.py` & `nsz-4.4.0/nsz/Fs/Nca.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/Nsp.py` & `nsz-4.4.0/nsz/Fs/Nsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,35 +403,32 @@
 		Print.info('\t\tRepacked to %s!' % outf.name)
 		outf.close()
 
 	def generateHeader(self, files):
 		filesNb = len(files)
 		stringTable = '\x00'.join(os.path.basename(file) for file in files)
 		headerSize = 0x10 + (filesNb)*0x18 + len(stringTable)
-		remainder = 0x10 - headerSize%0x10
-		headerSize += remainder
 		
 		fileSizes = [os.path.getsize(file) for file in files]
 		fileOffsets = [sum(fileSizes[:n]) for n in range(filesNb)]
 		
 		fileNamesLengths = [len(os.path.basename(file))+1 for file in files] # +1 for the \x00
 		stringTableOffsets = [sum(fileNamesLengths[:n]) for n in range(filesNb)]
 		
 		header =  b''
 		header += b'PFS0'
 		header += pk('<I', filesNb)
-		header += pk('<I', len(stringTable)+remainder)
+		header += pk('<I', len(stringTable))
 		header += b'\x00\x00\x00\x00'
 		for n in range(filesNb):
 			header += pk('<Q', fileOffsets[n])
 			header += pk('<Q', fileSizes[n])
 			header += pk('<I', stringTableOffsets[n])
 			header += b'\x00\x00\x00\x00'
 		header += stringTable.encode()
-		header += remainder * b'\x00'
 		
 		return header
 
 	def verifyKey(self, key):
 		for f in self:
 			if type(f) == Nca:
 				pass
```

### Comparing `nsz-4.3.0/nsz/Fs/Pfs0.py` & `nsz-4.4.0/nsz/Fs/Pfs0.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,45 +61,40 @@
 			self.seek(0)
 			self.write(self.getHeader())
 			super(Pfs0Stream, self).close()
 			
 	def getHeaderSize(self):
 		stringTable = '\x00'.join(file['name'] for file in self.files)
 		headerSize = 0x10 + len(self.files) * 0x18 + len(stringTable)
-		remainder = 0x10 - headerSize % 0x10
-		headerSize += remainder
 		return headerSize
 
 	def getFirstFileOffset(self):
 		return self.files[0].offset
 
 	def getHeader(self):
 		stringTable = '\x00'.join(file['name'] for file in self.files)
 		headerSize = 0x10 + len(self.files) * 0x18 + len(stringTable)
-		remainder = 0x10 - headerSize % 0x10
-		headerSize += remainder
 	
 		h = b''
 		h += b'PFS0'
 		h += len(self.files).to_bytes(4, byteorder='little')
-		h += (len(stringTable)+remainder).to_bytes(4, byteorder='little')
+		h += (len(stringTable)).to_bytes(4, byteorder='little')
 		h += b'\x00\x00\x00\x00'
 		
 		stringOffset = 0
 
 		for f in self.files:
 			h += (f['offset'] - headerSize).to_bytes(8, byteorder='little')
 			h += f['size'].to_bytes(8, byteorder='little')
 			h += stringOffset.to_bytes(4, byteorder='little')
 			h += b'\x00\x00\x00\x00'
 			
 			stringOffset += len(f['name']) + 1
 			
 		h += stringTable.encode()
-		h += remainder * b'\x00'
 		
 		return h
 
 
 class Pfs0VerifyStream():
 	def __init__(self, headerSize, mode = 'wb'):
 		self.files = []
@@ -137,35 +132,32 @@
 	def getHash(self):
 		hexHash = self.binhash.hexdigest()
 		return hexHash
 
 	def getHeaderHash(self):
 		stringTable = '\x00'.join(file['name'] for file in self.files)
 		headerSize = 0x10 + len(self.files) * 0x18 + len(stringTable)
-		remainder = 0x10 - headerSize % 0x10
-		headerSize += remainder
 	
 		h = b''
 		h += b'PFS0'
 		h += len(self.files).to_bytes(4, byteorder='little')
-		h += (len(stringTable)+remainder).to_bytes(4, byteorder='little')
+		h += (len(stringTable)).to_bytes(4, byteorder='little')
 		h += b'\x00\x00\x00\x00'
 		
 		stringOffset = 0
 		
 		for f in self.files:
 			h += (f['offset'] - headerSize).to_bytes(8, byteorder='little')
 			h += f['size'].to_bytes(8, byteorder='little')
 			h += stringOffset.to_bytes(4, byteorder='little')
 			h += b'\x00\x00\x00\x00'
 			
 			stringOffset += len(f['name']) + 1
 			
 		h += stringTable.encode()
-		h += remainder * b'\x00'
 		
 		headerBinhash = sha256()
 		headerBinhash.update(h)
 		headerHexHash = headerBinhash.hexdigest()
 		return headerHexHash
```

### Comparing `nsz-4.3.0/nsz/Fs/Rom.py` & `nsz-4.4.0/nsz/Fs/Rom.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/Ticket.py` & `nsz-4.4.0/nsz/Fs/Ticket.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/Type.py` & `nsz-4.4.0/nsz/Fs/Type.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/Xci.py` & `nsz-4.4.0/nsz/Fs/Xci.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Fs/__init__.py` & `nsz-4.4.0/nsz/Fs/__init__.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/Header.py` & `nsz-4.4.0/nsz/Header.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/IndependentNczDecompressor.py` & `nsz-4.4.0/nsz/IndependentNczDecompressor.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/NszDecompressor.py` & `nsz-4.4.0/nsz/NszDecompressor.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/ParseArguments.py` & `nsz-4.4.0/nsz/ParseArguments.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/PathTools.py` & `nsz-4.4.0/nsz/PathTools.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/SolidCompressor.py` & `nsz-4.4.0/nsz/SolidCompressor.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/__init__.py` & `nsz-4.4.0/nsz/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,33 +96,33 @@
 				argOutFolderToPharse += "/"
 			if not Path(argOutFolderToPharse).is_dir():
 				Print.error('Error: Output directory "{0}" does not exist!'.format(args.output))
 				return
 		argOutFolder = Path(argOutFolderToPharse).resolve() if args.output else None
 		
 		Print.info('')
-		Print.info('             NSZ v4.3   ,;:;;,')
+		Print.info('             NSZ v4.4   ,;:;;,')
 		Print.info('                       ;;;;;')
 		Print.info('               .=\',    ;:;;:,')
 		Print.info('              /_\', "=. \';:;:;')
 		Print.info('              @=:__,  \,;:;:\'')
 		Print.info('                _(\.=  ;:;;\'')
 		Print.info('               `"_(  _/="`')
 		Print.info('                `"\'')
 		Print.info('')
 		
 		barManager = enlighten.get_manager()
 		poolManager = Manager()
 		statusReport = poolManager.list()
-		readyForWork = Counter(0)
-		pleaseNoPrint = Counter(0)
-		pleaseKillYourself = Counter(0)
+		readyForWork = Counter(poolManager, 0)
+		pleaseNoPrint = Counter(poolManager, 0)
+		pleaseKillYourself = Counter(poolManager, 0)
 		pool = []
 		work = poolManager.Queue()
-		amountOfTastkQueued = Counter(0)
+		amountOfTastkQueued = Counter(poolManager, 0)
 		targetDictNsz = dict()
 		targetDictXcz = dict()
 		
 		if args.titlekeys:
 			extractTitlekeys(args.file)
 		
 		if args.extract:
```

### Comparing `nsz-4.3.0/nsz/gui/AboutDialog.py` & `nsz-4.4.0/nsz/gui/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/DraggableScrollbar.py` & `nsz-4.4.0/nsz/gui/DraggableScrollbar.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/FileDialogs.py` & `nsz-4.4.0/nsz/gui/FileDialogs.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/GameList.py` & `nsz-4.4.0/nsz/gui/GameList.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/Hyperlink.py` & `nsz-4.4.0/nsz/gui/Hyperlink.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/KivyOnTop.py` & `nsz-4.4.0/nsz/gui/KivyOnTop.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/NSZ_GUI.py` & `nsz-4.4.0/nsz/gui/NSZ_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		#to take effect." caused by checking if booth variables are set after setting
 		#one of them without offering any way of setting booth at the same time
 		Logger.setLevel(logging.ERROR)
 		Window.minimum_width = 800
 		Window.minimum_height = 600
 		Logger.setLevel(realLevl)
 		Builder.load_file(getGuiPath('layout/GUI.kv'))
-		self.title = 'NSZ GUI 4.3'
+		self.title = 'NSZ GUI 4.4'
 		self.icon = getGuiPath('nsZip.png')
 		root = FloatLayout()
 		with open(getGuiPath('shaders/plasma.shader')) as stream:
 			plasma_shader = stream.read()
 			root.add_widget(ShaderWidget(fs=plasma_shader))
 		gameList = GameList()
 		self.rootWidget = RootWidget(gameList)
```

### Comparing `nsz-4.3.0/nsz/gui/RootWidget.py` & `nsz-4.4.0/nsz/gui/RootWidget.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/SettingScrollOptions.py` & `nsz-4.4.0/nsz/gui/SettingScrollOptions.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/ShaderWidget.py` & `nsz-4.4.0/nsz/gui/ShaderWidget.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/fonts/MPLUS1p-Medium.ttf` & `nsz-4.4.0/nsz/gui/fonts/MPLUS1p-Medium.ttf`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/fonts/OFL.txt` & `nsz-4.4.0/nsz/gui/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/json/settings_advanced.json` & `nsz-4.4.0/nsz/gui/json/settings_advanced.json`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/json/settings_basic.json` & `nsz-4.4.0/nsz/gui/json/settings_basic.json`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/json/settings_tools.json` & `nsz-4.4.0/nsz/gui/json/settings_tools.json`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/layout/AboutDialog.kv` & `nsz-4.4.0/nsz/gui/layout/AboutDialog.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/layout/GameList.kv` & `nsz-4.4.0/nsz/gui/layout/GameList.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/layout/OpenFileDialog.kv` & `nsz-4.4.0/nsz/gui/layout/OpenFileDialog.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/layout/RootWidget.kv` & `nsz-4.4.0/nsz/gui/layout/RootWidget.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/shaders/plasma.shader` & `nsz-4.4.0/nsz/gui/shaders/plasma.shader`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/gui/txt/license.txt` & `nsz-4.4.0/nsz/gui/txt/license.txt`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/nut/Hex.py` & `nsz-4.4.0/nsz/nut/Hex.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/nut/Keys.py` & `nsz-4.4.0/nsz/nut/Keys.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/nut/Print.py` & `nsz-4.4.0/nsz/nut/Print.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/nut/Titles.py` & `nsz-4.4.0/nsz/nut/Titles.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/nut/aes128.py` & `nsz-4.4.0/nsz/nut/aes128.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz/undupe.py` & `nsz-4.4.0/nsz/undupe.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz.egg-info/SOURCES.txt` & `nsz-4.4.0/nsz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/nsz.py` & `nsz-4.4.0/nsz.py`

 * *Files identical despite different names*

### Comparing `nsz-4.3.0/setup.py` & `nsz-4.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='nsz',
-	version='4.3.0',
+	version='4.4.0',
 	script="nsz.py",
 	author="Nico Bosshard",
 	author_email="nico@bosshome.ch",
 	maintainer="Nico Bosshard",
 	maintainer_email="nico@bosshome.ch",
 	description="NSZ - Homebrew compatible NSP/XCI compressor/decompressor",
 	long_description=long_description,
```

