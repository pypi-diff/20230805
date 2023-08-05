# Comparing `tmp/Sidebar-nav-custom-icons-streamlit-0.0.2.tar.gz` & `tmp/Sidebar-nav-custom-icons-streamlit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sidebar-nav-custom-icons-streamlit-0.0.2.tar", last modified: Sat Aug  5 15:14:53 2023, max compression
+gzip compressed data, was "Sidebar-nav-custom-icons-streamlit-0.0.3.tar", last modified: Sat Aug  5 16:12:04 2023, max compression
```

## Comparing `Sidebar-nav-custom-icons-streamlit-0.0.2.tar` & `Sidebar-nav-custom-icons-streamlit-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 15:14:53.051495 Sidebar-nav-custom-icons-streamlit-0.0.2/
--rw-rw-rw-   0        0        0     1082 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       57 2023-08-05 14:33:15.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      617 2023-08-05 15:14:53.034227 Sidebar-nav-custom-icons-streamlit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 15:14:52.944150 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/
--rw-rw-rw-   0        0        0      617 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-08-05 15:14:52.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-08-05 15:14:51.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 15:14:53.025917 Sidebar-nav-custom-icons-streamlit-0.0.2/custom_sidebar_icons/
--rw-rw-rw-   0        0        0    14170 2023-08-05 15:13:20.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/custom_sidebar_icons/__init__.py
--rw-rw-rw-   0        0        0       42 2023-08-05 15:14:53.056040 Sidebar-nav-custom-icons-streamlit-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-08-05 15:13:29.000000 Sidebar-nav-custom-icons-streamlit-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:12:04.176021 Sidebar-nav-custom-icons-streamlit-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-08-05 14:33:15.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      617 2023-08-05 16:12:04.157870 Sidebar-nav-custom-icons-streamlit-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-04 14:44:24.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 16:12:04.098049 Sidebar-nav-custom-icons-streamlit-0.0.3/Sidebar_nav_custom_icons_streamlit.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-08-05 16:12:03.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-08-05 16:12:03.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/Sidebar_nav_custom_icons_streamlit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 16:12:03.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/Sidebar_nav_custom_icons_streamlit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-05 16:12:03.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/Sidebar_nav_custom_icons_streamlit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-05 16:12:03.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/Sidebar_nav_custom_icons_streamlit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 16:12:04.141432 Sidebar-nav-custom-icons-streamlit-0.0.3/custom_sidebar_icons/
+-rw-rw-rw-   0        0        0    14582 2023-08-05 16:10:04.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/custom_sidebar_icons/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 16:12:04.176021 Sidebar-nav-custom-icons-streamlit-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-08-05 16:10:47.000000 Sidebar-nav-custom-icons-streamlit-0.0.3/setup.py
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.2/LICENSE` & `Sidebar-nav-custom-icons-streamlit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.2/PKG-INFO` & `Sidebar-nav-custom-icons-streamlit-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sidebar-nav-custom-icons-streamlit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Streamlit component that allows you to set emojis from 5 prettier icon libraries
 Home-page: 
 Author: 
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.2/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO` & `Sidebar-nav-custom-icons-streamlit-0.0.3/Sidebar_nav_custom_icons_streamlit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sidebar-nav-custom-icons-streamlit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Streamlit component that allows you to set emojis from 5 prettier icon libraries
 Home-page: 
 Author: 
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.2/custom_sidebar_icons/__init__.py` & `Sidebar-nav-custom-icons-streamlit-0.0.3/custom_sidebar_icons/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,25 @@
 
                     page_links_title.forEach((el) => {{
                         el.classList.add('page-title-streamlit')
                     }})
                 </script>
             """
         st.components.v1.html(js)
+
+    def create_unique_class_for_streamlitTabs_(self):
+        """
+        Activate `create_unique_class_for_streamlitTabs()` method with placeholder so that it deletes the iframe on running. 
+        """
+        placeholder = st.empty()
+        with placeholder.container():
+            self.create_unique_class_for_streamlitTabs()
+            time.sleep(1)
+            placeholder.empty() 
+        
     
     def tabler_icons(self, data_object, index):
         """
         Function to render icons from tabler icons. For icons, view:https://tabler-icons.io/
         """
 
         js = f"""
```

### Comparing `Sidebar-nav-custom-icons-streamlit-0.0.2/setup.py` & `Sidebar-nav-custom-icons-streamlit-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="Sidebar-nav-custom-icons-streamlit",
-    version="0.0.2",
+    version="0.0.3",
     author="",
     author_email="",
     description="Streamlit component that allows you to set emojis from 5 prettier icon libraries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

