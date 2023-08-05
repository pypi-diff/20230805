# Comparing `tmp/moneycontrol_api-1.1.1.tar.gz` & `tmp/moneycontrol_api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneycontrol_api-1.1.1.tar", last modified: Sat Aug  5 14:39:21 2023, max compression
+gzip compressed data, was "moneycontrol_api-1.1.2.tar", last modified: Sat Aug  5 14:55:40 2023, max compression
```

## Comparing `moneycontrol_api-1.1.1.tar` & `moneycontrol_api-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.548103 moneycontrol_api-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/src/moneycontrol/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/src/moneycontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-08-05 14:39:05.000000 moneycontrol_api-1.1.1/src/moneycontrol/moneycontrol_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:39:21.552104 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 14:39:21.000000 moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:55:40.161209 moneycontrol_api-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-05 14:55:30.000000 moneycontrol_api-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:55:40.161209 moneycontrol_api-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-05 14:55:30.000000 moneycontrol_api-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-05 14:55:30.000000 moneycontrol_api-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:55:40.161209 moneycontrol_api-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:55:40.161209 moneycontrol_api-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:55:40.161209 moneycontrol_api-1.1.2/src/moneycontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 14:55:30.000000 moneycontrol_api-1.1.2/src/moneycontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-08-05 14:55:30.000000 moneycontrol_api-1.1.2/src/moneycontrol/moneycontrol_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:55:40.161209 moneycontrol_api-1.1.2/src/moneycontrol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 14:55:40.000000 moneycontrol_api-1.1.2/src/moneycontrol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-05 14:55:40.000000 moneycontrol_api-1.1.2/src/moneycontrol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:55:40.000000 moneycontrol_api-1.1.2/src/moneycontrol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 14:55:40.000000 moneycontrol_api-1.1.2/src/moneycontrol_api.egg-info/top_level.txt
```

### Comparing `moneycontrol_api-1.1.1/LICENSE` & `moneycontrol_api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moneycontrol_api-1.1.1/PKG-INFO` & `moneycontrol_api-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycontrol_api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Moneycontrol API is a python library to get news data from moneycontrol.com in JSON format.
 Author-email: Arabian Coconut <x48cl9zm@duck.com>
 Project-URL: Homepage, https://github.com/ArabianCoconut/Moneycontrol-api
 Project-URL: Live Demo, https://mc-api-j0rn.onrender.com
 Keywords: moneycontrol api,moneycontrol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `moneycontrol_api-1.1.1/README.md` & `moneycontrol_api-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `moneycontrol_api-1.1.1/pyproject.toml` & `moneycontrol_api-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moneycontrol_api"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Arabian Coconut", email="x48cl9zm@duck.com" },
 ]
 description = "Moneycontrol API is a python library to get news data from moneycontrol.com in JSON format."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `moneycontrol_api-1.1.1/src/moneycontrol/moneycontrol_api.py` & `moneycontrol_api-1.1.2/src/moneycontrol/moneycontrol_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     url_data = requests.get(url[0], timeout=60)
     soup = BeautifulSoup(url_data.text, "html.parser")
     soup_process = soup.find_all("h3", {"class": "related_des"})
     for i in soup_process:
         title_info = i.find("a").get("title")
         link_info = i.find("a").get("href")
         json_data = {news_type: "News", title_text: title_info, link_text: link_info}
-        return json.dumps(json_data, indent=2)
+        return json_data
 
 
 def get_business_news():
     """
     Gets the news from the given URL and returns a JSON object containing the title, link,
     and date of the news.
 
@@ -53,15 +53,15 @@
     # Get the title, link and date of the news
     new_list = "newslist-0"
     news_list = soup.find("li", {"class": "clearfix", "id": new_list})
     title = news_list.find("h2").find("a").get("title")
     link = news_list.find("h2").find("a").get("href")
     date = news_list.find("span", {"class": "list_dt"})
     json_data = {news_type: "Business News", title_text: title, link_text: link, date_text: date}
-    return json.dumps(json_data, indent=2)
+    return json_data
 
 
 def get_latest_news():
     """
     Gets the news from the given URL and returns a JSON object containing the title, link,
     and date of the news.
 
@@ -76,8 +76,8 @@
     related_des_class = soup.find_all("h3", {"class": "related_des"})
     related_date_class = soup.find_all("p", {"class": "related_date hide-mob"})
     for h3_tag, p_tag in zip(related_des_class, related_date_class):
         title = h3_tag.find("a").get("title")
         link = h3_tag.find("a").get("href")
         date = p_tag.text
         json_data = {news_type: "Latest News", title_text: title, link_text: link, date_text: date}
-        return json.dumps(json_data, indent=2)
+        return json_data
```

### Comparing `moneycontrol_api-1.1.1/src/moneycontrol_api.egg-info/PKG-INFO` & `moneycontrol_api-1.1.2/src/moneycontrol_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycontrol-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Moneycontrol API is a python library to get news data from moneycontrol.com in JSON format.
 Author-email: Arabian Coconut <x48cl9zm@duck.com>
 Project-URL: Homepage, https://github.com/ArabianCoconut/Moneycontrol-api
 Project-URL: Live Demo, https://mc-api-j0rn.onrender.com
 Keywords: moneycontrol api,moneycontrol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

