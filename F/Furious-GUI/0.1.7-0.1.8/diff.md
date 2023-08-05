# Comparing `tmp/Furious-GUI-0.1.7.tar.gz` & `tmp/Furious-GUI-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.1.7.tar", last modified: Thu Jul 27 01:16:38 2023, max compression
+gzip compressed data, was "Furious-GUI-0.1.8.tar", last modified: Sat Aug  5 03:48:21 2023, max compression
```

## Comparing `Furious-GUI-0.1.7.tar` & `Furious-GUI-0.1.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.120968 Furious-GUI-0.1.7/Furious/
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.120968 Furious-GUI-0.1.7/Furious/Action/
--rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Connect.py
--rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/EditConfiguration.py
--rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Exit.py
--rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Export.py
--rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Import.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Language.py
--rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Routing.py
--rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Settings.py
--rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.136420 Furious-GUI-0.1.7/Furious/Core/
--rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.7/Furious/Core/Configuration.py
--rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Core/Core.py
--rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Core/Intellisense.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.105147 Furious-GUI-0.1.7/Furious/Data/
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.136420 Furious-GUI-0.1.7/Furious/Data/font/
--rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/font/CascadiaMono
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.136420 Furious-GUI-0.1.7/Furious/Data/hysteria/
--rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/hysteria/country.mmdb
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.183121 Furious-GUI-0.1.7/Furious/Data/xray/
--rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/xray/geoip.dat
--rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/xray/geosite.dat
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.214718 Furious-GUI-0.1.7/Furious/Gui/
--rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Gui/Action.py
--rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Gui/Icon.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.230103 Furious-GUI-0.1.7/Furious/Utility/
--rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.7/Furious/Utility/Constants.py
--rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Process.py
--rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Proxy.py
--rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.7/Furious/Utility/Resources.py
--rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Settings.py
--rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/StartupOnBoot.py
--rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Theme.py
--rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Translator.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Utility.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-27 01:16:05.000000 Furious-GUI-0.1.7/Furious/Version.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.230103 Furious-GUI-0.1.7/Furious/Widget/
--rw-rw-rw-   0        0        0     8709 2023-07-26 11:36:26.000000 Furious-GUI-0.1.7/Furious/Widget/Application.py
--rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/ConnectingProgressBar.py
--rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/EditConfiguration.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/ExportQRCode.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/IndentSpinBox.py
--rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/LogViewer.py
--rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/SystemTrayIcon.py
--rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/Widget.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/Furious_GUI.egg-info/
--rw-rw-rw-   0        0        0     6940 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      201 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     6940 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     5924 2023-07-26 23:53:22.000000 Furious-GUI-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1886 2023-07-27 01:16:05.000000 Furious-GUI-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.481694 Furious-GUI-0.1.8/Furious/
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.560144 Furious-GUI-0.1.8/Furious/Action/
+-rw-rw-rw-   0        0        0    25095 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Action/Connect.py
+-rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/EditConfiguration.py
+-rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Exit.py
+-rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Export.py
+-rw-rw-rw-   0        0        0    15675 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Action/Import.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Language.py
+-rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Routing.py
+-rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/Settings.py
+-rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.575730 Furious-GUI-0.1.8/Furious/Core/
+-rw-rw-rw-   0        0        0    21870 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Core/Configuration.py
+-rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Core/Core.py
+-rw-rw-rw-   0        0        0     4575 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Core/Intellisense.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.450784 Furious-GUI-0.1.8/Furious/Data/
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.591197 Furious-GUI-0.1.8/Furious/Data/font/
+-rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/font/CascadiaMono
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.606672 Furious-GUI-0.1.8/Furious/Data/hysteria/
+-rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/hysteria/country.mmdb
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.653938 Furious-GUI-0.1.8/Furious/Data/xray/
+-rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/xray/geoip.dat
+-rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/Furious/Data/xray/geosite.dat
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.669633 Furious-GUI-0.1.8/Furious/Gui/
+-rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Gui/Action.py
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Gui/Icon.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.763183 Furious-GUI-0.1.8/Furious/Utility/
+-rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.8/Furious/Utility/Constants.py
+-rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Process.py
+-rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Proxy.py
+-rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.8/Furious/Utility/Resources.py
+-rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Settings.py
+-rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/StartupOnBoot.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Theme.py
+-rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/Translator.py
+-rw-rw-rw-   0        0        0     5231 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Utility/Utility.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Utility/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/Furious/Version.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.841090 Furious-GUI-0.1.8/Furious/Widget/
+-rw-rw-rw-   0        0        0     8709 2023-07-26 11:36:26.000000 Furious-GUI-0.1.8/Furious/Widget/Application.py
+-rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/ConnectingProgressBar.py
+-rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/EditConfiguration.py
+-rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/ExportQRCode.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/IndentSpinBox.py
+-rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/LogViewer.py
+-rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/SystemTrayIcon.py
+-rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/Widget.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/Widget/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/__init__.py
+-rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.8/Furious/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/Furious_GUI.egg-info/
+-rw-rw-rw-   0        0        0    10866 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      195 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 03:48:21.000000 Furious-GUI-0.1.8/Furious_GUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0    10866 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9850 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 03:48:21.872787 Furious-GUI-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2023-08-05 03:44:20.000000 Furious-GUI-0.1.8/setup.py
```

### Comparing `Furious-GUI-0.1.7/Furious/Action/Connect.py` & `Furious-GUI-0.1.8/Furious/Action/Connect.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         self.coreText = ''
         self.coreJSON = {}
         self.coreRunning = False
         self.XrayRouting = {}
 
         self.connectingFlag = False
 
+        self.disconnectReason = ''
+
         # Note: The connection test is carried out item by item
         # from top to bottom. If any of these succeed,
         # connected action will be executed.
 
         # "Popular" sites that's been endorsed by some government.
         self.testPool = [
             # Messaging
@@ -90,53 +92,91 @@
 
         if exitcode == XrayCore.ExitCode.ConfigurationError:
             if not self.isConnecting():
                 # Protect connecting action. Mandatory
                 return self.disconnectAction(
                     f'{XrayCore.name()}: {_("Invalid server configuration")}'
                 )
+            else:
+                self.coreRunning = False
+                self.disconnectReason = (
+                    f'{XrayCore.name()}: {_("Invalid server configuration")}'
+                )
+
+                return
 
         if exitcode == XrayCore.ExitCode.ServerStartFailure:
             if not self.isConnecting():
                 # Protect connecting action. Mandatory
                 return self.disconnectAction(
                     f'{XrayCore.name()}: {_("Failed to start core")}'
                 )
+            else:
+                self.coreRunning = False
+                self.disconnectReason = (
+                    f'{XrayCore.name()}: {_("Failed to start core")}'
+                )
+
+                return
 
         if not self.isConnecting():
             # Protect connecting action. Mandatory
             self.disconnectAction(
                 f'{XrayCore.name()}: {_("Core terminated unexpectedly")}'
             )
+        else:
+            self.coreRunning = False
+            self.disconnectReason = (
+                f'{XrayCore.name()}: {_("Core terminated unexpectedly")}'
+            )
 
     def HysteriaExitCallback(self, exitcode):
         if self.coreName:
             # If core is running
             assert self.coreRunning
             assert self.coreName == Hysteria.name()
 
         if exitcode == Hysteria.ExitCode.ConfigurationError:
             if not self.isConnecting():
                 # Protect connecting action. Mandatory
                 return self.disconnectAction(
                     f'{Hysteria.name()}: {_("Invalid server configuration")}'
                 )
+            else:
+                self.coreRunning = False
+                self.disconnectReason = (
+                    f'{Hysteria.name()}: {_("Invalid server configuration")}'
+                )
+
+                return
 
         if exitcode == Hysteria.ExitCode.RemoteNetworkError:
             if not self.isConnecting():
                 # Protect connecting action. Mandatory
                 return self.disconnectAction(
                     f'{Hysteria.name()}: {_("Connection to server has been lost")}'
                 )
+            else:
+                self.coreRunning = False
+                self.disconnectReason = (
+                    f'{Hysteria.name()}: {_("Connection to server has been lost")}'
+                )
+
+                return
 
         if not self.isConnecting():
             # Protect connecting action. Mandatory
             self.disconnectAction(
                 f'{Hysteria.name()}: {_("Core terminated unexpectedly")}'
             )
+        else:
+            self.coreRunning = False
+            self.disconnectReason = (
+                f'{Hysteria.name()}: {_("Core terminated unexpectedly")}'
+            )
 
     def stopCore(self):
         # Stop any potentially running core
         self.XrayCore.stop()
         self.Hysteria.stop()
 
     def showConnectingProgressBar(self):
@@ -225,14 +265,16 @@
         self.coreJSON = {}
         self.coreRunning = False
         self.XrayRouting = {}
 
         # Accept new action
         self.setDisabledAction(False)
 
+        self.disconnectReason = ''
+
         self.connectingFlag = False
 
     @property
     def MainWidget(self):
         # Handy reference
         return QApplication.instance().MainWidget
 
@@ -513,21 +555,24 @@
             assert isinstance(self.networkReply, QNetworkReply)
 
             if self.networkReply.error() != QNetworkReply.NetworkError.NoError:
                 logger.error(
                     f'{self.coreName}: connection test failed. {self.networkReply.errorString()}'
                 )
 
-                if self.testTime < len(self.testPool):
+                if self.testTime < len(self.testPool) and self.coreRunning:
                     # Try next
                     self.startConnectionTest(showRoutingChangedMessage)
                 else:
-                    self.disconnectAction(
-                        f'{self.coreName}: {_("Connection test failed")}'
-                    )
+                    if self.disconnectReason:
+                        self.disconnectAction(self.disconnectReason)
+                    else:
+                        self.disconnectAction(
+                            f'{self.coreName}: {_("Connection test failed")}'
+                        )
             else:
                 logger.info(f'{self.coreName}: connection test success. Connected')
 
                 QApplication.instance().Connect = Switch.ON_
 
                 # Connected status
                 self.setConnectedStatus()
@@ -622,16 +667,22 @@
             # No matching core
             self.reset()
             self.errorConfiguration()
 
             return
 
         if not self.coreRunning:
-            # No valid HTTP proxy endpoint / Core has exited.
-            # reset / disconnect has been called
+            # 1. No valid HTTP proxy endpoint. reset / disconnect has been called
+
+            if self.isConnecting():
+                # 2. Core has exited. disconnectReason must not be empty
+                assert self.disconnectReason
+
+                self.disconnectAction(self.disconnectReason)
+
             return
 
         try:
             Proxy.set(self.proxyServer, PROXY_SERVER_BYPASS)
         except Exception:
             # Any non-exit exceptions
```

### Comparing `Furious-GUI-0.1.7/Furious/Action/Export.py` & `Furious-GUI-0.1.8/Furious/Action/Export.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Action/Import.py` & `Furious-GUI-0.1.8/Furious/Action/Import.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from Furious.Core.Configuration import (
     Configuration,
     XrayCoreConfiguration,
     ProxyOutboundObject,
+    ProxyOutboundObjectSS,
 )
 from Furious.Gui.Action import Action
 from Furious.Widget.Widget import Menu, MessageBox
 from Furious.Utility.Utility import (
     Base64Encoder,
+    Protocol,
     StateContext,
     Storage,
     bootstrapIcon,
     protocolRepr,
 )
 from Furious.Utility.Translator import gettext as _
 
@@ -215,15 +217,15 @@
 
             queryObject = {
                 key: value for key, value in urllib.parse.parse_qsl(parseResult.query)
             }
 
             remark = urllib.parse.unquote(parseResult.fragment)
 
-            uuid_, remote_host, remote_port = re.split(r'[@:]', parseResult.path)
+            uuid_, remote_host, remote_port = re.split(r'[@:]', parseResult.netloc)
 
             encryption = queryObject.get('encryption', 'none')
             type_ = queryObject.get('type', 'tcp')
             security = queryObject.get('security', 'none')
 
             # Remove redundant items
             queryObject.pop('encryption', '')
@@ -258,14 +260,91 @@
 
             return remark, True
         except Exception:
             # Any non-exit exceptions
 
             return '', False
 
+    @staticmethod
+    def parseShareLinkSIP002(data):
+        try:
+            result = urllib.parse.urlparse(data)
+            remark = urllib.parse.unquote(result.fragment)
+
+            try:
+                # Try pack with 3 element
+                userinfo, address, port = re.split(r'[@:]', result.netloc)
+
+                # Some old SS share link doesn't add padding
+                # in base64 encoding. Add padding to userinfo
+                method, password = (
+                    Base64Encoder.decode(userinfo + '===').decode().split(':')
+                )
+            except ValueError:
+                # Unpack error. Try pack with 4 element
+
+                method, password, address, port = re.split(r'[@:]', result.netloc)
+            except Exception as ex:
+                # Any non-exit exceptions
+
+                raise ex
+
+            myJSON = XrayCoreConfiguration.build(
+                ProxyOutboundObjectSS(
+                    urllib.parse.unquote(method),
+                    urllib.parse.unquote(password),
+                    address,
+                    port,
+                )
+            )
+
+            QApplication.instance().MainWidget.importServer(
+                remark,
+                ujson.dumps(
+                    myJSON, indent=2, ensure_ascii=False, escape_forward_slashes=False
+                ),
+            )
+
+            logger.info(
+                f'import share link from clipboard success. '
+                f'Remark: {remark}. Protocol: {Protocol.Shadowsocks}'
+            )
+
+            return remark, True
+        except Exception as ex:
+            # Any non-exit exceptions
+
+            return '', False
+
+    def parseShareLinkSS(self, data):
+        try:
+            # ss://base64...
+            myData = Base64Encoder.decode(data[5:]).decode()
+            myJSON = XrayCoreConfiguration.build(
+                ProxyOutboundObjectSS(*re.split(r'[@:]', myData))
+            )
+
+            QApplication.instance().MainWidget.importServer(
+                'sslegacy',
+                ujson.dumps(
+                    myJSON, indent=2, ensure_ascii=False, escape_forward_slashes=False
+                ),
+            )
+
+            logger.info(
+                f'import share link from clipboard success. '
+                f'Remark: sslegacy. Protocol: {Protocol.Shadowsocks}'
+            )
+
+            return 'sslegacy', True
+        except Exception:
+            # Any non-exit exceptions
+
+            return self.parseShareLinkSIP002(data)
+
     def parseShareLink(self, shareLink):
         try:
             myHead, myBody = shareLink.split('://')
         except Exception:
             # Any non-exit exceptions
 
             return '', False
@@ -273,20 +352,23 @@
             if myHead.lower() == 'vmess':
                 try:
                     myData = Base64Encoder.decode(myBody).decode()
                     myJSON = Configuration.toJSON(myData)
                 except Exception:
                     # Any non-exit exceptions
 
-                    return self.parseShareLinkVMess(myBody, isV2rayN=False)
+                    return self.parseShareLinkVMess(shareLink, isV2rayN=False)
                 else:
                     return self.parseShareLinkVMess(myJSON, isV2rayN=True)
 
             if myHead.lower() == 'vless':
-                return self.parseShareLinkStandard('vless', myBody)
+                return self.parseShareLinkStandard('vless', shareLink)
+
+            if myHead.lower() == 'ss':
+                return self.parseShareLinkSS(shareLink)
 
             return '', False
 
     def triggeredCallback(self, checked):
         self.clipboard = QApplication.clipboard().text().strip()
 
         try:
```

### Comparing `Furious-GUI-0.1.7/Furious/Action/Language.py` & `Furious-GUI-0.1.8/Furious/Action/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Action/Routing.py` & `Furious-GUI-0.1.8/Furious/Action/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Action/Settings.py` & `Furious-GUI-0.1.8/Furious/Action/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Core/Configuration.py` & `Furious-GUI-0.1.8/Furious/Core/Configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from Furious.Core.Core import XrayCore
 from Furious.Core.Intellisense import Intellisense
 from Furious.Widget.Widget import MessageBox
 from Furious.Utility.Constants import APPLICATION_NAME
-from Furious.Utility.Utility import Base64Encoder, bootstrapIcon
+from Furious.Utility.Utility import Base64Encoder, Protocol, bootstrapIcon
 from Furious.Utility.Translator import gettext as _
 
 import copy
 import ujson
 import functools
 import urllib.parse
 
-quote = functools.partial(urllib.parse.quote)
+# '/' will be quoted for V2rayN compatibility.
+quote = functools.partial(urllib.parse.quote, safe='')
 unquote = functools.partial(urllib.parse.unquote)
 urlunparse = functools.partial(urllib.parse.urlunparse)
 
 
 class UnsupportedServerExport(Exception):
     pass
 
@@ -62,34 +63,34 @@
 
                 netobj = streamObject[
                     ProxyOutboundObject.getStreamNetworkSettingsName(netType)
                 ]
 
                 if netType == 'tcp':
                     try:
-                        if protocol.lower() == 'vmess':
+                        if protocol == Protocol.VMess:
                             kwargs['type'] = netobj['header']['type']
 
-                        if protocol.lower() == 'vless':
+                        if protocol == Protocol.VLESS:
                             kwargs['headerType'] = netobj['header']['type']
                     except Exception:
                         # Any non-exit exceptions
 
                         pass
 
                 elif netType == 'kcp':
                     try:
                         # Get order matters here
-                        if protocol.lower() == 'vmess':
+                        if protocol == Protocol.VMess:
                             if hasKey(netobj, 'seed'):
                                 kwargs['path'] = netobj['seed']
 
                             kwargs['type'] = netobj['header']['type']
 
-                        if protocol.lower() == 'vless':
+                        if protocol == Protocol.VLESS:
                             if hasKey(netobj, 'seed'):
                                 kwargs['seed'] = netobj['seed']
 
                             kwargs['headerType'] = netobj['header']['type']
                     except Exception:
                         # Any non-exit exceptions
 
@@ -119,42 +120,42 @@
                         # Any non-exit exceptions
 
                         pass
 
                 elif netType == 'quic':
                     try:
                         # Get order matters here
-                        if protocol.lower() == 'vmess':
+                        if protocol == Protocol.VMess:
                             if hasKey(netobj, 'security'):
                                 kwargs['host'] = netobj['security']
 
                             if hasKey(netobj, 'key'):
                                 kwargs['path'] = quote(netobj['key'])
 
                             kwargs['type'] = netobj['header']['type']
 
-                        if protocol.lower() == 'vless':
+                        if protocol == Protocol.VLESS:
                             if hasKey(netobj, 'security'):
                                 kwargs['quicSecurity'] = netobj['security']
 
                             if hasKey(netobj, 'key'):
                                 kwargs['path'] = quote(netobj['key'])
 
                             kwargs['headerType'] = netobj['header']['type']
                     except Exception:
                         # Any non-exit exceptions
 
                         pass
 
                 elif netType == 'grpc':
-                    if protocol.lower() == 'vmess':
+                    if protocol == Protocol.VMess:
                         if hasKey(netobj, 'serviceName'):
                             kwargs['path'] = netobj['serviceName']
 
-                    if protocol.lower() == 'vless':
+                    if protocol == Protocol.VLESS:
                         if hasKey(netobj, 'serviceName'):
                             kwargs['serviceName'] = netobj['serviceName']
 
                 return kwargs
 
             def getStreamTLSSettings(streamObject, tlsType):
                 if tlsType == 'none':
@@ -186,17 +187,17 @@
 
                     if tlsobj.get('spiderX'):
                         kwargs['spx'] = quote(tlsobj['spiderX'])
 
                 return kwargs
 
             # Begin export
-            coreProtocol = Intellisense.getCoreProtocol(ob).lower()
+            coreProtocol = Intellisense.getCoreProtocol(ob)
 
-            if coreProtocol == 'vmess' or coreProtocol == 'vless':
+            if coreProtocol == Protocol.VMess or coreProtocol == Protocol.VLESS:
                 proxyOutbound = None
 
                 for outbound in ob['outbounds']:
                     if outbound['tag'] == 'proxy':
                         proxyOutbound = outbound
 
                         break
@@ -207,15 +208,15 @@
                 proxyServer = proxyOutbound['settings']['vnext'][0]
                 proxyServerUser = proxyServer['users'][0]
 
                 proxyStream = proxyOutbound['streamSettings']
                 proxyStreamNet = proxyStream['network']
                 proxyStreamTLS = proxyStream['security']
 
-                if coreProtocol == 'vmess':
+                if coreProtocol == Protocol.VMess:
                     return (
                         'vmess://'
                         + Base64Encoder.encode(
                             ujson.dumps(
                                 {
                                     'v': '2',
                                     'ps': quote(remark),
@@ -234,15 +235,15 @@
                                 },
                                 ensure_ascii=False,
                                 escape_forward_slashes=False,
                             ).encode()
                         ).decode()
                     )
 
-                if coreProtocol == 'vless':
+                if coreProtocol == Protocol.VLESS:
                     flowArg = {}
 
                     if proxyServerUser.get('flow'):
                         flowArg['flow'] = proxyServerUser['flow']
 
                     netloc = f'{proxyServerUser["id"]}@{proxyServer["address"]}:{proxyServer["port"]}'
 
@@ -258,30 +259,63 @@
                                 coreProtocol, proxyStream, proxyStreamNet
                             ),
                             **getStreamTLSSettings(proxyStream, proxyStreamTLS),
                         }.items()
                     )
 
                     return urlunparse(['vless', netloc, '', '', query, quote(remark)])
+
+            if coreProtocol == Protocol.Shadowsocks:
+                proxyOutbound = None
+
+                for outbound in ob['outbounds']:
+                    if outbound['tag'] == 'proxy':
+                        proxyOutbound = outbound
+
+                        break
+
+                if proxyOutbound is None:
+                    raise Exception('No proxy outbound found')
+
+                proxyServer = proxyOutbound['settings']['servers'][0]
+
+                method = proxyServer['method']
+                password = proxyServer['password']
+                address = proxyServer['address']
+                port = proxyServer['port']
+
+                netloc = f'{quote(method)}:{quote(password)}@{address}:{port}'
+
+                return urlunparse(['ss', netloc, '', '', '', quote(remark)])
         else:
             raise UnsupportedServerExport('Unsupported core protocol export')
 
 
-class ProxyOutboundObject:
+class OutboundObject:
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def build(self):
+        raise NotImplementedError
+
+
+class ProxyOutboundObject(OutboundObject):
     def __init__(
         self,
         protocol,
         remote_host,
         remote_port,
         uuid_,
         encryption,
         type_,
         security,
         **kwargs,
     ):
+        super().__init__()
+
         self.protocol = protocol
         self.remote_host = remote_host
         self.remote_port = remote_port
         self.uuid_ = uuid_
         self.encryption = encryption
         self.type_ = type_
         self.security = security
@@ -492,14 +526,50 @@
         myJSON['streamSettings'][
             ProxyOutboundObject.getStreamNetworkSettingsName(self.type_)
         ] = self.getStreamNetworkSettings()
 
         return myJSON
 
 
+class ProxyOutboundObjectSS(OutboundObject):
+    def __init__(self, method, password, address, port, **kwargs):
+        super().__init__(**kwargs)
+
+        self.method = method
+        self.password = password
+        self.address = address
+        self.port = int(port)
+
+    def build(self):
+        myJSON = {
+            'tag': 'proxy',
+            'protocol': 'shadowsocks',
+            'settings': {
+                'servers': [
+                    {
+                        'address': self.address,
+                        'port': self.port,
+                        'method': self.method,
+                        'password': self.password,
+                        'ota': False,
+                    },
+                ]
+            },
+            'streamSettings': {
+                'network': 'tcp',
+            },
+            'mux': {
+                'enabled': False,
+                'concurrency': -1,
+            },
+        }
+
+        return myJSON
+
+
 class Outbounds:
     def __init__(self, proxyOutboundObject):
         self.proxyOutboundObject = proxyOutboundObject
 
     def build(self):
         return [
             # Proxy
```

### Comparing `Furious-GUI-0.1.7/Furious/Core/Core.py` & `Furious-GUI-0.1.8/Furious/Core/Core.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Core/Intellisense.py` & `Furious-GUI-0.1.8/Furious/Core/Intellisense.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from Furious.Core.Core import XrayCore, Hysteria
-from Furious.Utility.Utility import protocolRepr
+from Furious.Utility.Utility import Protocol, protocolRepr
 
 
 class Intellisense:
     @staticmethod
     def getCoreType(ob):
         if ob.get('inbounds') is not None or ob.get('outbounds') is not None:
             # Assuming is XrayCore
@@ -20,56 +20,78 @@
         try:
             if Intellisense.getCoreType(ob) == XrayCore.name():
                 for outbound in ob['outbounds']:
                     if outbound['tag'] == 'proxy':
                         return protocolRepr(outbound['protocol'])
 
             if Intellisense.getCoreType(ob) == Hysteria.name():
-                return 'hysteria'
+                return Protocol.Hysteria
 
             return ''
         except Exception:
             # Any non-exit exceptions
 
             return ''
 
     @staticmethod
     def getCoreAddr(ob):
         try:
             if Intellisense.getCoreType(ob) == XrayCore.name():
+                protocol = Intellisense.getCoreProtocol(ob)
+
                 for outbound in ob['outbounds']:
                     if outbound['tag'] == 'proxy':
-                        return ';'.join(
-                            list(
-                                f'{server["address"]}'
-                                for server in outbound['settings']['vnext']
+                        if protocol == Protocol.VMess or protocol == Protocol.VLESS:
+                            return ';'.join(
+                                list(
+                                    f'{server["address"]}'
+                                    for server in outbound['settings']['vnext']
+                                )
+                            )
+
+                        if protocol == Protocol.Shadowsocks:
+                            return ';'.join(
+                                list(
+                                    f'{server["address"]}'
+                                    for server in outbound['settings']['servers']
+                                )
                             )
-                        )
 
             if Intellisense.getCoreType(ob) == Hysteria.name():
                 return ob['server'].split(':')[0]
 
             return ''
         except Exception:
             # Any non-exit exceptions
 
             return ''
 
     @staticmethod
     def getCorePort(ob):
         try:
             if Intellisense.getCoreType(ob) == XrayCore.name():
+                protocol = Intellisense.getCoreProtocol(ob)
+
                 for outbound in ob['outbounds']:
                     if outbound['tag'] == 'proxy':
-                        return ';'.join(
-                            list(
-                                f'{server["port"]}'
-                                for server in outbound['settings']['vnext']
+                        if protocol == Protocol.VMess or protocol == Protocol.VLESS:
+                            return ';'.join(
+                                list(
+                                    f'{server["port"]}'
+                                    for server in outbound['settings']['vnext']
+                                )
+                            )
+
+                        if protocol == Protocol.Shadowsocks:
+                            return ';'.join(
+                                list(
+                                    f'{server["port"]}'
+                                    for server in outbound['settings']['servers']
+                                )
                             )
-                        )
 
             if Intellisense.getCoreType(ob) == Hysteria.name():
                 return ob['server'].split(':')[1]
 
             return ''
         except Exception:
             # Any non-exit exceptions
```

### Comparing `Furious-GUI-0.1.7/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.1.8/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.1.8/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.1.8/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.1.8/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.1.8/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Gui/Action.py` & `Furious-GUI-0.1.8/Furious/Gui/Action.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Constants.py` & `Furious-GUI-0.1.8/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Process.py` & `Furious-GUI-0.1.8/Furious/Utility/Process.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Proxy.py` & `Furious-GUI-0.1.8/Furious/Utility/Proxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Resources.py` & `Furious-GUI-0.1.8/Furious/Utility/Resources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Settings.py` & `Furious-GUI-0.1.8/Furious/Utility/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.1.8/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Theme.py` & `Furious-GUI-0.1.8/Furious/Utility/Theme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Translator.py` & `Furious-GUI-0.1.8/Furious/Utility/Translator.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Utility/Utility.py` & `Furious-GUI-0.1.8/Furious/Utility/Utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,22 @@
 class Base64Encoder:
     @staticmethod
     def encode(text):
         return pybase64.b64encode(text)
 
     @staticmethod
     def decode(text):
-        return pybase64.b64decode(text, validate=True)
+        return pybase64.b64decode(text, validate=False)
+
+
+class Protocol:
+    VMess = 'VMess'
+    VLESS = 'VLESS'
+    Shadowsocks = 'shadowsocks'
+    Hysteria = 'hysteria'
 
 
 class StateContext:
     def __init__(self, ob, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         assert hasattr(ob, 'setDisabled')
@@ -144,20 +151,23 @@
 
 bootstrapIcon = functools.partial(icon, 'bootstrap')
 bootstrapIconWhite = functools.partial(icon, 'bootstrap/white')
 
 
 def protocolRepr(protocol):
     if protocol.lower() == 'vmess':
-        return 'VMess'
+        return Protocol.VMess
 
     if protocol.lower() == 'vless':
-        return 'VLESS'
+        return Protocol.VLESS
+
+    if protocol.lower() == 'shadowsocks':
+        return Protocol.Shadowsocks
 
-    return ''
+    return protocol
 
 
 def getAbsolutePath(path):
     return path if os.path.isabs(path) else str(ROOT_DIR / path)
 
 
 def swapListItem(listOrTuple, index0, index1):
```

### Comparing `Furious-GUI-0.1.7/Furious/Widget/Application.py` & `Furious-GUI-0.1.8/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Widget/ConnectingProgressBar.py` & `Furious-GUI-0.1.8/Furious/Widget/ConnectingProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Widget/EditConfiguration.py` & `Furious-GUI-0.1.8/Furious/Widget/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Widget/ExportQRCode.py` & `Furious-GUI-0.1.8/Furious/Widget/ExportQRCode.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.1.8/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Widget/LogViewer.py` & `Furious-GUI-0.1.8/Furious/Widget/LogViewer.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.1.8/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/Widget/Widget.py` & `Furious-GUI-0.1.8/Furious/Widget/Widget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious/__main__.py` & `Furious-GUI-0.1.8/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.1.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,32 @@
-Metadata-Version: 2.1
-Name: Furious-GUI
-Version: 0.1.7
-Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
-Home-page: https://github.com/LorenEteval/Furious
-Author: Loren Eteval
-Author-email: loren.eteval@proton.me
-License: GPL v3.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: Proxy Servers
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Furious
 
 A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Support [Xray-core](https://github.com/XTLS/Xray-core)
 and [hysteria](https://github.com/apernet/hysteria).
 
 ![Furious](https://raw.githubusercontent.com/LorenEteval/Furious/main/Icons/png/rocket-takeoff-window-400x400.png)
 
 ## Features
 
-* Runs seamlessly on Windows, macOS and Linux.
+* Runs seamlessly on Windows, macOS and Linux(see the screenshot below).
 * Built-in support for [Xray-core](https://github.com/XTLS/Xray-core)
   and [hysteria](https://github.com/apernet/hysteria). Cores are actually Python bindings that shipped with the source
   code. See more information: [Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
   and [hysteria-python](https://github.com/LorenEteval/hysteria-python).
-* Support import from JSON or share link(`vmess://...` or `vless://...`, including the newest REALITY share standard).
+* Support import from JSON or share link(`vmess://...`, `vless://...` or `ss://`, including the
+  newest [REALITY](https://github.com/XTLS/REALITY) share standard).
 * Support export to JSON, share link or QRCode.
 * Two built-in routing mode support: Bypass Mainland China(with Ads filter) and Global. You can also choose to use your
   own routing rules.
 * Built-in editor support.
-* Ability to store and handle hundreds of servers, or even more.
 * VPN-client user experience.
 * Support system theme detection and switch to dark/light theme automatically.
 * Multiple language support: English, Spanish, Simplified Chinese and Traditional Chinese.
-* Built-in user-friendly feature.
+* Built-in user-friendly feature such as startup on boot.
 * ...
 
 ## Sreenshot
 
 ### Windows
 
 ![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-EN.png)
@@ -93,15 +70,15 @@
 
     * For Linux users: type `sudo apt update && sudo apt install g++` and that should work out fine.
     * For Windows users: install [MinGW-w64](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/)
       or [Cygwin](https://www.cygwin.com/) and make sure you have add them to PATH.
 
 ### Install Furious
 
-Furious requires Python 3.8 and above.
+Furious requires **Python 3.8 and above**.
 
 ```
 pip install Furious-GUI
 ```
 
 If the installation is successful, you will have a executable script(or `.exe` on Windows) in your PATH(if it's not in
 the PATH, you can always add the script location to the PATH later). That's Furious's application entry point.
@@ -114,24 +91,29 @@
 
 Furious will enable startup on boot by default if it's launched for the first time. Happy browsing!
 
 ## Run From Source
 
 Clone this repository and enter the project folder. Install requirements:
 
+> Note: To install requirements successfully you will also need
+> those [Core Building Tools](https://github.com/LorenEteval/Furious#core-building-tools) above.
+
 ```
 pip install -r requirements.txt
 ```
 
 Run:
 
 ```
 python -m Furious
 ```
 
+> Note: Furious will ignore current startup on boot request if it's lauched from source.
+
 ## Core Installation Script
 
 Below are some one-click/automatic installation script that's been tested to work in Furious.
 
 | Project Address                                                   |  Supported Core Installation  | Share Link Import Support? | JSON Import Support? |
 |-------------------------------------------------------------------|:-----------------------------:|:--------------------------:|:--------------------:|
 | [233boy/v2ray](https://github.com/233boy/v2ray)                   |          v2ray-core           |            Yes             |          /           |
@@ -139,7 +121,88 @@
 | [zxcvos/Xray-script](https://github.com/zxcvos/Xray-script)       |           Xray-core           |            Yes             |          /           |
 | [aleskxyz/reality-ezpz](https://github.com/aleskxyz/reality-ezpz) |           Xray-core           |            Yes             |          /           |
 | [emptysuns/Hi_Hysteria](https://github.com/emptysuns/Hi_Hysteria) |           hysteria            |             No             |         Yes          |
 
 ## License
 
 License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE).
+
+---
+
+## 功能
+
+* 可在Windows、macOS和Linux上运行（见上文运行截图）。
+* 内置对[Xray-core](https://github.com/XTLS/Xray-core)和[hysteria](https://github.com/apernet/hysteria)的支持。
+  Core实际是与源代码一起发行的Python绑定。更多信息: [Xray-core-python](https://github.com/LorenEteval/Xray-core-python), [hysteria-python](https://github.com/LorenEteval/hysteria-python)。
+* 支持从JSON或分享链接导入（`vmess://...`，`vless://...`或`ss://`，包括最新的[REALITY](https://github.com/XTLS/REALITY)
+  分享标准）。
+* 支持导出为JSON、分享链接或二维码。
+* 内置两种路由模式的支持：绕过中国大陆（带广告过滤）和全球。也可选择使用自己的路由规则。
+* 内置编辑器支持。
+* VPN客户端的使用体验。
+* 支持系统主题检测并自动切换深色/浅色主题。
+* 多语言支持：英语、西班牙语、简体中文和繁体中文。
+* 内置用户友好的功能，例如开机自启动等。
+* ...
+
+## 安装
+
+> 注意：由于Windows有更好的二进制文件兼容性，Windows用户可以跳过本节并在
+[release](https://github.com/LorenEteval/Furious/releases)页面中下载打包好的zip文件。否则安装过程需要按照以下步骤进行。
+
+### Core编译工具
+
+> 注意: 这些步骤与[Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
+> 和[hysteria-python](https://github.com/LorenEteval/hysteria-python)中*Core Building Tools*一节的步骤一样。
+
+根据上文所述，Core是对应的Python绑定以支持跨平台运行。所以要安装Furious你首先得准备好当前平台的Core编译工具。编译Core需要：
+
+* [go](https://go.dev/doc/install)在PATH中。建议使用go 1.20.0及以上版本。要检查go是否就绪，输入`go version`
+  。另外，如果你当前所在地区（例如中国大陆）屏蔽了google服务，还需要配置GOPROXY才能拉取go包。对于中国用户，请访问[goproxy.cn](https://goproxy.cn/)
+  了解更多信息。
+* [cmake](https://cmake.org/download/)在PATH中. 要检查cmake是否就绪，输入`cmake --version`。
+* GNU C++编译器（即GNU C++工具链）。要检查GNU C++编译器是否准备就绪，输入`g++ --version`
+  。默认情况下，这些工具应该已安装在Linux或macOS中。如果你仍然没有GNU C++工具链（特别是对于Windows用户）：
+
+    * 对于Linux用户：输入`sudo apt update && sudo apt install g++`。
+    * 对于Windows用户：安装[MinGW-w64](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/)
+      或[Cygwin](https://www.cygwin.com/)并确保已将它们添加至PATH。
+
+### 安装Furious
+
+运行Furious需要**Python 3.8及以上**版本。
+
+```
+pip install Furious-GUI
+```
+
+如果安装成功，PATH中将有一个可执行脚本（在Windows上是.exe）（如果它不在PATH中，可以稍后将脚本路径添加至PATH），这是Furious的应用程序入口点。
+
+要启动Furious，输入：
+
+```
+Furious
+```
+
+如果是首次运行，Furious将默认启用开机启动。Happy browsing!
+
+## 从源码运行
+
+克隆该仓库并进入项目文件夹。安装所需依赖包：
+
+> 注意：为了安装依赖包成功，你仍然需要准备好上文中的Core编译工具。
+
+```
+pip install -r requirements.txt
+```
+
+运行:
+
+```
+python -m Furious
+```
+
+> 注意：如果从源码运行，Furious将忽略当前的开机自启动请求。
+
+## License
+
+License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Furious-GUI-0.1.7/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.1.8/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/LICENSE` & `Furious-GUI-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.7/PKG-INFO` & `Furious-GUI-0.1.8/Furious_GUI.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.7
+Version: 0.1.8
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,29 +27,29 @@
 Support [Xray-core](https://github.com/XTLS/Xray-core)
 and [hysteria](https://github.com/apernet/hysteria).
 
 ![Furious](https://raw.githubusercontent.com/LorenEteval/Furious/main/Icons/png/rocket-takeoff-window-400x400.png)
 
 ## Features
 
-* Runs seamlessly on Windows, macOS and Linux.
+* Runs seamlessly on Windows, macOS and Linux(see the screenshot below).
 * Built-in support for [Xray-core](https://github.com/XTLS/Xray-core)
   and [hysteria](https://github.com/apernet/hysteria). Cores are actually Python bindings that shipped with the source
   code. See more information: [Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
   and [hysteria-python](https://github.com/LorenEteval/hysteria-python).
-* Support import from JSON or share link(`vmess://...` or `vless://...`, including the newest REALITY share standard).
+* Support import from JSON or share link(`vmess://...`, `vless://...` or `ss://`, including the
+  newest [REALITY](https://github.com/XTLS/REALITY) share standard).
 * Support export to JSON, share link or QRCode.
 * Two built-in routing mode support: Bypass Mainland China(with Ads filter) and Global. You can also choose to use your
   own routing rules.
 * Built-in editor support.
-* Ability to store and handle hundreds of servers, or even more.
 * VPN-client user experience.
 * Support system theme detection and switch to dark/light theme automatically.
 * Multiple language support: English, Spanish, Simplified Chinese and Traditional Chinese.
-* Built-in user-friendly feature.
+* Built-in user-friendly feature such as startup on boot.
 * ...
 
 ## Sreenshot
 
 ### Windows
 
 ![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-EN.png)
@@ -93,15 +93,15 @@
 
     * For Linux users: type `sudo apt update && sudo apt install g++` and that should work out fine.
     * For Windows users: install [MinGW-w64](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/)
       or [Cygwin](https://www.cygwin.com/) and make sure you have add them to PATH.
 
 ### Install Furious
 
-Furious requires Python 3.8 and above.
+Furious requires **Python 3.8 and above**.
 
 ```
 pip install Furious-GUI
 ```
 
 If the installation is successful, you will have a executable script(or `.exe` on Windows) in your PATH(if it's not in
 the PATH, you can always add the script location to the PATH later). That's Furious's application entry point.
@@ -114,24 +114,29 @@
 
 Furious will enable startup on boot by default if it's launched for the first time. Happy browsing!
 
 ## Run From Source
 
 Clone this repository and enter the project folder. Install requirements:
 
+> Note: To install requirements successfully you will also need
+> those [Core Building Tools](https://github.com/LorenEteval/Furious#core-building-tools) above.
+
 ```
 pip install -r requirements.txt
 ```
 
 Run:
 
 ```
 python -m Furious
 ```
 
+> Note: Furious will ignore current startup on boot request if it's lauched from source.
+
 ## Core Installation Script
 
 Below are some one-click/automatic installation script that's been tested to work in Furious.
 
 | Project Address                                                   |  Supported Core Installation  | Share Link Import Support? | JSON Import Support? |
 |-------------------------------------------------------------------|:-----------------------------:|:--------------------------:|:--------------------:|
 | [233boy/v2ray](https://github.com/233boy/v2ray)                   |          v2ray-core           |            Yes             |          /           |
@@ -139,7 +144,88 @@
 | [zxcvos/Xray-script](https://github.com/zxcvos/Xray-script)       |           Xray-core           |            Yes             |          /           |
 | [aleskxyz/reality-ezpz](https://github.com/aleskxyz/reality-ezpz) |           Xray-core           |            Yes             |          /           |
 | [emptysuns/Hi_Hysteria](https://github.com/emptysuns/Hi_Hysteria) |           hysteria            |             No             |         Yes          |
 
 ## License
 
 License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE).
+
+---
+
+## 功能
+
+* 可在Windows、macOS和Linux上运行（见上文运行截图）。
+* 内置对[Xray-core](https://github.com/XTLS/Xray-core)和[hysteria](https://github.com/apernet/hysteria)的支持。
+  Core实际是与源代码一起发行的Python绑定。更多信息: [Xray-core-python](https://github.com/LorenEteval/Xray-core-python), [hysteria-python](https://github.com/LorenEteval/hysteria-python)。
+* 支持从JSON或分享链接导入（`vmess://...`，`vless://...`或`ss://`，包括最新的[REALITY](https://github.com/XTLS/REALITY)
+  分享标准）。
+* 支持导出为JSON、分享链接或二维码。
+* 内置两种路由模式的支持：绕过中国大陆（带广告过滤）和全球。也可选择使用自己的路由规则。
+* 内置编辑器支持。
+* VPN客户端的使用体验。
+* 支持系统主题检测并自动切换深色/浅色主题。
+* 多语言支持：英语、西班牙语、简体中文和繁体中文。
+* 内置用户友好的功能，例如开机自启动等。
+* ...
+
+## 安装
+
+> 注意：由于Windows有更好的二进制文件兼容性，Windows用户可以跳过本节并在
+[release](https://github.com/LorenEteval/Furious/releases)页面中下载打包好的zip文件。否则安装过程需要按照以下步骤进行。
+
+### Core编译工具
+
+> 注意: 这些步骤与[Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
+> 和[hysteria-python](https://github.com/LorenEteval/hysteria-python)中*Core Building Tools*一节的步骤一样。
+
+根据上文所述，Core是对应的Python绑定以支持跨平台运行。所以要安装Furious你首先得准备好当前平台的Core编译工具。编译Core需要：
+
+* [go](https://go.dev/doc/install)在PATH中。建议使用go 1.20.0及以上版本。要检查go是否就绪，输入`go version`
+  。另外，如果你当前所在地区（例如中国大陆）屏蔽了google服务，还需要配置GOPROXY才能拉取go包。对于中国用户，请访问[goproxy.cn](https://goproxy.cn/)
+  了解更多信息。
+* [cmake](https://cmake.org/download/)在PATH中. 要检查cmake是否就绪，输入`cmake --version`。
+* GNU C++编译器（即GNU C++工具链）。要检查GNU C++编译器是否准备就绪，输入`g++ --version`
+  。默认情况下，这些工具应该已安装在Linux或macOS中。如果你仍然没有GNU C++工具链（特别是对于Windows用户）：
+
+    * 对于Linux用户：输入`sudo apt update && sudo apt install g++`。
+    * 对于Windows用户：安装[MinGW-w64](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/)
+      或[Cygwin](https://www.cygwin.com/)并确保已将它们添加至PATH。
+
+### 安装Furious
+
+运行Furious需要**Python 3.8及以上**版本。
+
+```
+pip install Furious-GUI
+```
+
+如果安装成功，PATH中将有一个可执行脚本（在Windows上是.exe）（如果它不在PATH中，可以稍后将脚本路径添加至PATH），这是Furious的应用程序入口点。
+
+要启动Furious，输入：
+
+```
+Furious
+```
+
+如果是首次运行，Furious将默认启用开机启动。Happy browsing!
+
+## 从源码运行
+
+克隆该仓库并进入项目文件夹。安装所需依赖包：
+
+> 注意：为了安装依赖包成功，你仍然需要准备好上文中的Core编译工具。
+
+```
+pip install -r requirements.txt
+```
+
+运行:
+
+```
+python -m Furious
+```
+
+> 注意：如果从源码运行，Furious将忽略当前的开机自启动请求。
+
+## License
+
+License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Furious-GUI-0.1.7/setup.py` & `Furious-GUI-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from Furious.Version import __version__
-from Furious.Utility.Constants import PLATFORM
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
@@ -16,15 +15,14 @@
     author='Loren Eteval',
     author_email='loren.eteval@proton.me',
     url='https://github.com/LorenEteval/Furious',
     packages=find_packages(),
     package_data={'Furious': ['Data/**']},
     include_package_data=True,
     install_requires=[
-        'wheel',
         'PySide6-Essentials',
         'Xray-core',
         'hysteria',
         'ujson',
         'pybase64',
         'pyqrcode',
         'sysproxy; sys_platform == "win32"',
```

