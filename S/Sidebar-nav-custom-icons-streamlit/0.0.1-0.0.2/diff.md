# Comparing `tmp/Sidebar-nav-custom-icons-streamlit-0.0.1.tar.gz` & `tmp/Sidebar-nav-custom-icons-streamlit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sidebar-nav-custom-icons-streamlit-0.0.1.tar", last modified: Sat Aug  5 14:32:17 2023, max compression
+gzip compressed data, was "Sidebar-nav-custom-icons-streamlit-0.0.2.tar", last modified: Sat Aug  5 15:14:53 2023, max compression
```

## Comparing `Sidebar-nav-custom-icons-streamlit-0.0.1.tar` & `Sidebar-nav-custom-icons-streamlit-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 14:32:17.534300 Sidebar-nav-custom-icons-streamlit-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       49 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      617 2023-08-05 14:32:17.531299 Sidebar-nav-custom-icons-streamlit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 14:32:17.513295 Sidebar-nav-custom-icons-streamlit-0.0.1/Sidebar_nav_custom_icons_streamlit.egg-info/
--rw-rw-rw-   0        0        0      617 2023-08-05 14:32:16.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-08-05 14:32:17.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/Sidebar_nav_custom_icons_streamlit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 14:32:17.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/Sidebar_nav_custom_icons_streamlit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-05 14:32:17.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/Sidebar_nav_custom_icons_streamlit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-08-05 14:32:17.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/Sidebar_nav_custom_icons_streamlit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 14:32:17.519298 Sidebar-nav-custom-icons-streamlit-0.0.1/custom_sidebar_icons/
--rw-rw-rw-   0        0        0    14262 2023-08-05 14:14:41.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/custom_sidebar_icons/__init__.py
--rw-rw-rw-   0        0        0       42 2023-08-05 14:32:17.535306 Sidebar-nav-custom-icons-streamlit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-08-05 14:27:25.000000 Sidebar-nav-custom-icons-streamlit-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:14:53.051495 Sidebar-nav-custom-icons-streamlit-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-08-05 14:33:15.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      617 2023-08-05 15:14:53.034227 Sidebar-nav-custom-icons-streamlit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 15:14:52.944150 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-08-05 15:14:52.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 15:14:53.025917 Sidebar-nav-custom-icons-streamlit-0.0.2/custom_sidebar_icons/
+-rw-rw-rw-   0        0        0    14170 2023-08-05 15:13:20.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/custom_sidebar_icons/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 15:14:53.056040 Sidebar-nav-custom-icons-streamlit-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-08-05 15:13:29.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/setup.py
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.1/LICENSE` & `Sidebar-nav-custom-icons-streamlit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.1/PKG-INFO` & `Sidebar-nav-custom-icons-streamlit-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sidebar-nav-custom-icons-streamlit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to set emojis from 5 prettier icon libraries
 Home-page: 
 Author: 
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.1/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO` & `Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sidebar-nav-custom-icons-streamlit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to set emojis from 5 prettier icon libraries
 Home-page: 
 Author: 
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.1/custom_sidebar_icons/__init__.py` & `Sidebar-nav-custom-icons-streamlit-0.0.2/custom_sidebar_icons/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
 import streamlit as st
 import time
-st.markdown('<style>' + open('./style.css').read() + '</style>', unsafe_allow_html=True)
-
   
 class Set_Nav_Emojis:
 
     def __init__(self, emojisToRender, uniform_icon_ID="page-title-icon"):
         """
         Load in the emojis to show - list of dictionaries. Also the uniform id for all icon ids
         """
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.1/setup.py` & `Sidebar-nav-custom-icons-streamlit-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="Sidebar-nav-custom-icons-streamlit",
-    version="0.0.1",
+    version="0.0.2",
     author="",
     author_email="",
     description="Streamlit component that allows you to set emojis from 5 prettier icon libraries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

