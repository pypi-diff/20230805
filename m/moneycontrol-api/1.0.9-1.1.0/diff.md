# Comparing `tmp/moneycontrol_api-1.0.9.tar.gz` & `tmp/moneycontrol_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneycontrol_api-1.0.9.tar", last modified: Sat Jan 21 18:11:58 2023, max compression
+gzip compressed data, was "moneycontrol_api-1.1.0.tar", last modified: Sat Aug  5 14:22:26 2023, max compression
```

## Comparing `moneycontrol_api-1.0.9.tar` & `moneycontrol_api-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-21 18:11:58.071628 moneycontrol_api-1.0.9/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1686 2023-01-18 19:22:03.000000 moneycontrol_api-1.0.9/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1451 2023-01-21 18:11:58.071628 moneycontrol_api-1.0.9/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      884 2023-01-19 13:49:47.000000 moneycontrol_api-1.0.9/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-21 18:11:58.067628 moneycontrol_api-1.0.9/moneycontrol/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2587 2023-01-18 19:03:56.000000 moneycontrol_api-1.0.9/moneycontrol/moneycontrol_api.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-21 18:11:58.071628 moneycontrol_api-1.0.9/moneycontrol_api.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1451 2023-01-21 18:11:58.000000 moneycontrol_api-1.0.9/moneycontrol_api.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      234 2023-01-21 18:11:58.000000 moneycontrol_api-1.0.9/moneycontrol_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-21 18:11:58.000000 moneycontrol_api-1.0.9/moneycontrol_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-01-21 18:11:58.000000 moneycontrol_api-1.0.9/moneycontrol_api.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      650 2023-01-21 18:09:14.000000 moneycontrol_api-1.0.9/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-01-21 18:11:58.071628 moneycontrol_api-1.0.9/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      414 2023-01-21 18:11:44.000000 moneycontrol_api-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/src/moneycontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/src/moneycontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-08-05 14:22:15.000000 moneycontrol_api-1.1.0/src/moneycontrol/moneycontrol_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:22:26.933150 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 14:22:26.000000 moneycontrol_api-1.1.0/src/moneycontrol_api.egg-info/top_level.txt
```

### Comparing `moneycontrol_api-1.0.9/LICENSE` & `moneycontrol_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moneycontrol_api-1.0.9/moneycontrol/moneycontrol_api.py` & `moneycontrol_api-1.1.0/src/moneycontrol/moneycontrol_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,83 @@
+import json
+import requests
 from bs4 import BeautifulSoup
-import requests,json
 
 # Api for getting the latest news from moneycontrol.com
 
 # Constants
-title_text="Title:"
-link_text="Link:"
-date_text="Date:"
-html_parser="html.parser"
-news_type="News Type:"
-
+title_text = "Title:"
+link_text = "Link:"
+date_text = "Date:"
+html_parser = "html.parser"
+news_type = "News Type:"
 
 # Urls for getting the news
-url=["https://www.moneycontrol.com/news",
-"https://www.moneycontrol.com/news/business",
-"https://www.moneycontrol.com/news/latest-news/"]
+url = ["https://www.moneycontrol.com/news",
+       "https://www.moneycontrol.com/news/business",
+       "https://www.moneycontrol.com/news/latest-news/"]
+
 
 def get_news():
-    soup = BeautifulSoup(requests.get(url[0],timeout=60).text, html_parser)
-    # Get the title, link and date of the news
-    related_des_class = soup.find_all("h3", {"class": "related_des"})
-    related_date_class = soup.find_all("p", {"class": "related_date hide-mob"})
-    for h3_tag,p_tag in zip(related_des_class, related_date_class):
-        title = h3_tag.find("a").get("title")
-        link = h3_tag.find("a").get("href")
-        date = p_tag.text
-        json_data = {news_type:"News", title_text: title, link_text: link, date_text: date }
-        return json.dumps(json_data, indent=0)
+    """
+    Gets the news from the given URL and returns a JSON object containing the title, link,
+    and date of the news.
+
+    Parameters:
+    url (string): The URL from which to retrieve the news
+
+    Returns:
+    json_data (JSON object): A JSON object containing the title, link, and date of the news
+    """
+    url_data = requests.get(url[0], timeout=60)
+    soup = BeautifulSoup(url_data.text, "html.parser")
+    soup_process = soup.find_all("h3", {"class": "related_des"})
+    for i in soup_process:
+        title_info = i.find("a").get("title")
+        link_info = i.find("a").get("href")
+        json_data = {news_type: "News", title_text: title_info, link_text: link_info}
+        return json.dumps(json_data, indent=2)
+
 
 def get_business_news():
-    soup = BeautifulSoup(requests.get(url[1],timeout=60).text, html_parser)
+    """
+    Gets the news from the given URL and returns a JSON object containing the title, link,
+    and date of the news.
+
+    Parameters:
+    url (string): The URL from which to retrieve the news
+
+    Returns:
+    json_data (JSON object): A JSON object containing the title, link, and date of the news
+    """
+    soup = BeautifulSoup(requests.get(url[1], timeout=60).text, html_parser)
     # Get the title, link and date of the news
-    for i in range(1, 24):
-        new_list = "newslist-"+str(i)
-        news_list = soup.find("li", {"class": "clearfix", "id": new_list})
-        news_list_heading_2=soup.find("h1",{"class":"fleft"})
-        if news_list:
-            title_class = news_list.find("h2").find("a")
-            title = title_class.get("title")
-            link = title_class.get("href")
-            date_class = news_list.find("span")
-            date = date_class.text
-            print(news_type,news_list_heading_2.text)
-            json_data = {news_type:news_list_heading_2.text ,
-            title_text: title, link_text: link, date_text: date }
-            return json.dumps(json_data, indent=0)
-        else:
-            print(f"li element with class 'clearfix' and id '{id}' not found.")
-            return None
+    new_list = "newslist-0"
+    news_list = soup.find("li", {"class": "clearfix", "id": new_list})
+    title = news_list.find("h2").find("a").get("title")
+    link = news_list.find("h2").find("a").get("href")
+    date = news_list.find("span", {"class": "list_dt"})
+    json_data = {news_type: "Business News", title_text: title, link_text: link, date_text: date}
+    return json.dumps(json_data, indent=2)
+
 
 def get_latest_news():
-    soup = BeautifulSoup(requests.get(url[2],timeout=60).text, html_parser)
+    """
+    Gets the news from the given URL and returns a JSON object containing the title, link,
+    and date of the news.
+
+    Parameters:
+    url (string): The URL from which to retrieve the news
+
+    Returns:
+    json_data (JSON object): A JSON object containing the title, link, and date of the news
+    """
+    soup = BeautifulSoup(requests.get(url[2], timeout=60).text, html_parser)
     # Get the title, link and date of the news
     related_des_class = soup.find_all("h3", {"class": "related_des"})
     related_date_class = soup.find_all("p", {"class": "related_date hide-mob"})
-    for h3_tag,p_tag in zip(related_des_class, related_date_class):
+    for h3_tag, p_tag in zip(related_des_class, related_date_class):
         title = h3_tag.find("a").get("title")
         link = h3_tag.find("a").get("href")
         date = p_tag.text
-        json_data = {news_type:"Latest News", title_text: title, link_text: link, date_text: date}
-        return json.dumps(json_data, indent=0)
+        json_data = {news_type: "Latest News", title_text: title, link_text: link, date_text: date}
+        return json.dumps(json_data, indent=2)
```

### Comparing `moneycontrol_api-1.0.9/pyproject.toml` & `moneycontrol_api-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moneycontrol_api"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Arabian Coconut", email="x48cl9zm@duck.com" },
 ]
-description = "Moneycontrol API is a python library to get news data from moneycontrol.com"
+description = "Moneycontrol API is a python library to get news data from moneycontrol.com in JSON format."
 readme = "README.md"
-requires-python = ">=3.0"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 keywords = ["moneycontrol api","moneycontrol"]
 
 [project.urls]
 "Homepage" = "https://github.com/ArabianCoconut/Moneycontrol-api"
+"Live Demo" = "https://mc-api-j0rn.onrender.com"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["moneycontrol"]
+exclude = ["templates","app.py"]
```

