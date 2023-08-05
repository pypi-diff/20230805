# Comparing `tmp/ss3a-0.0.2.tar.gz` & `tmp/ss3a-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ss3a-0.0.2.tar", last modified: Sat Aug  5 17:20:10 2023, max compression
+gzip compressed data, was "ss3a-0.0.3.tar", last modified: Sat Aug  5 17:27:00 2023, max compression
```

## Comparing `ss3a-0.0.2.tar` & `ss3a-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ken        (501) staff       (20)        0 2023-08-05 17:20:10.569251 ss3a-0.0.2/
--rw-r--r--   0 ken        (501) staff       (20)     1094 2023-08-05 07:34:10.000000 ss3a-0.0.2/LICENSE
--rw-r--r--   0 ken        (501) staff       (20)      563 2023-08-05 17:20:10.569125 ss3a-0.0.2/PKG-INFO
--rw-r--r--   0 ken        (501) staff       (20)        4 2023-08-05 07:41:17.000000 ss3a-0.0.2/README.md
-drwxr-xr-x   0 ken        (501) staff       (20)        0 2023-08-05 17:20:10.568131 ss3a-0.0.2/model/
--rw-r--r--   0 ken        (501) staff       (20)     1660 2023-08-05 17:17:09.000000 ss3a-0.0.2/model/__init__.py
--rw-r--r--   0 ken        (501) staff       (20)      421 2023-08-05 11:43:02.000000 ss3a-0.0.2/model/model_utilty.py
--rw-r--r--   0 ken        (501) staff       (20)     1839 2023-08-05 17:17:15.000000 ss3a-0.0.2/model/ss3a_models.py
--rw-r--r--   0 ken        (501) staff       (20)       38 2023-08-05 17:20:10.569292 ss3a-0.0.2/setup.cfg
--rw-r--r--   0 ken        (501) staff       (20)     1365 2023-08-05 17:17:46.000000 ss3a-0.0.2/setup.py
-drwxr-xr-x   0 ken        (501) staff       (20)        0 2023-08-05 17:20:10.568961 ss3a-0.0.2/ss3a.egg-info/
--rw-r--r--   0 ken        (501) staff       (20)      563 2023-08-05 17:20:10.000000 ss3a-0.0.2/ss3a.egg-info/PKG-INFO
--rw-r--r--   0 ken        (501) staff       (20)      226 2023-08-05 17:20:10.000000 ss3a-0.0.2/ss3a.egg-info/SOURCES.txt
--rw-r--r--   0 ken        (501) staff       (20)        1 2023-08-05 17:20:10.000000 ss3a-0.0.2/ss3a.egg-info/dependency_links.txt
--rw-r--r--   0 ken        (501) staff       (20)       38 2023-08-05 17:20:10.000000 ss3a-0.0.2/ss3a.egg-info/requires.txt
--rw-r--r--   0 ken        (501) staff       (20)        6 2023-08-05 17:20:10.000000 ss3a-0.0.2/ss3a.egg-info/top_level.txt
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2023-08-05 17:27:00.823046 ss3a-0.0.3/
+-rw-r--r--   0 ken        (501) staff       (20)     1094 2023-08-05 07:34:10.000000 ss3a-0.0.3/LICENSE
+-rw-r--r--   0 ken        (501) staff       (20)      563 2023-08-05 17:27:00.822892 ss3a-0.0.3/PKG-INFO
+-rw-r--r--   0 ken        (501) staff       (20)        4 2023-08-05 07:41:17.000000 ss3a-0.0.3/README.md
+-rw-r--r--   0 ken        (501) staff       (20)       38 2023-08-05 17:27:00.823105 ss3a-0.0.3/setup.cfg
+-rw-r--r--   0 ken        (501) staff       (20)     1365 2023-08-05 17:26:01.000000 ss3a-0.0.3/setup.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2023-08-05 17:27:00.822229 ss3a-0.0.3/ss3a.egg-info/
+-rw-r--r--   0 ken        (501) staff       (20)      563 2023-08-05 17:27:00.000000 ss3a-0.0.3/ss3a.egg-info/PKG-INFO
+-rw-r--r--   0 ken        (501) staff       (20)      236 2023-08-05 17:27:00.000000 ss3a-0.0.3/ss3a.egg-info/SOURCES.txt
+-rw-r--r--   0 ken        (501) staff       (20)        1 2023-08-05 17:27:00.000000 ss3a-0.0.3/ss3a.egg-info/dependency_links.txt
+-rw-r--r--   0 ken        (501) staff       (20)       38 2023-08-05 17:27:00.000000 ss3a-0.0.3/ss3a.egg-info/requires.txt
+-rw-r--r--   0 ken        (501) staff       (20)       11 2023-08-05 17:27:00.000000 ss3a-0.0.3/ss3a.egg-info/top_level.txt
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2023-08-05 17:27:00.822697 ss3a-0.0.3/ss3a_model/
+-rw-r--r--   0 ken        (501) staff       (20)     1665 2023-08-05 17:25:37.000000 ss3a-0.0.3/ss3a_model/__init__.py
+-rw-r--r--   0 ken        (501) staff       (20)      421 2023-08-05 11:43:02.000000 ss3a-0.0.3/ss3a_model/model_utilty.py
+-rw-r--r--   0 ken        (501) staff       (20)     1844 2023-08-05 17:25:37.000000 ss3a-0.0.3/ss3a_model/models.py
```

### Comparing `ss3a-0.0.2/LICENSE` & `ss3a-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ss3a-0.0.2/PKG-INFO` & `ss3a-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ss3a
-Version: 0.0.2
+Version: 0.0.3
 Summary: SYLKSOFT常用工具
 Home-page: https://www.sylksoft.com
 Download-URL: https://pypi.org/project/ss3a/
 Author: Ken Chen
 Author-email: ken@sylksoft.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ss3a-0.0.2/model/__init__.py` & `ss3a-0.0.3/ss3a_model/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Author: ken
 Date: 2023/7/18
 """
 
 from sqlalchemy import Connection, event, text
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Mapper
-from model import model_utilty
+from ss3a_model import model_utilty
 
 
 Base = declarative_base()
 
 
 class GenericEntity(Base):
     __abstract__ = True
```

### Comparing `ss3a-0.0.2/model/ss3a_models.py` & `ss3a-0.0.3/ss3a_model/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sqlalchemy import Column, String, Boolean, DateTime
 
-from model import Base
+from ss3a_model import Base
 
 
 class Ss3aMember(Base):
     __tablename__ = 'ss3a_member'
     id_ = Column('member_id', String(50), primary_key=True)
     password = Column('member_password', String(100))
     mobile = Column('mobile', String(10))
```

### Comparing `ss3a-0.0.2/setup.py` & `ss3a-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 PACKAGE_NAME = "ss3a"
 AUTHOR = "Ken Chen"
 AUTHOR_EMAIL = "ken@sylksoft.com"
 URL = "https://www.sylksoft.com"
 DOWNLOAD_URL = "https://pypi.org/project/ss3a/"
 
 LICENSE = "MIT"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "SYLKSOFT常用工具"
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
```

### Comparing `ss3a-0.0.2/ss3a.egg-info/PKG-INFO` & `ss3a-0.0.3/ss3a.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ss3a
-Version: 0.0.2
+Version: 0.0.3
 Summary: SYLKSOFT常用工具
 Home-page: https://www.sylksoft.com
 Download-URL: https://pypi.org/project/ss3a/
 Author: Ken Chen
 Author-email: ken@sylksoft.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
```

