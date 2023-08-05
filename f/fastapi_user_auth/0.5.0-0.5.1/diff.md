# Comparing `tmp/fastapi_user_auth-0.5.0.tar.gz` & `tmp/fastapi_user_auth-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_auth-0.5.0.tar", last modified: Sat Mar  4 15:50:02 2023, max compression
+gzip compressed data, was "fastapi_user_auth-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_user_auth-0.5.0.tar` & `fastapi_user_auth-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       98 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.flake8
--rw-r--r--   0        0        0     1662 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      977 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2070 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.gitignore
--rw-r--r--   0        0        0      326 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11157 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/README.md
--rw-r--r--   0        0        0    10288 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/README.zh.md
--rw-r--r--   0        0        0      345 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/__init__.py
--rw-r--r--   0        0        0    11465 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/admin.py
--rw-r--r--   0        0        0     3390 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/app.py
--rw-r--r--   0        0        0      119 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/__init__.py
--rw-r--r--   0        0        0    12985 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/auth.py
--rw-r--r--   0        0        0        0 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/__init__.py
--rw-r--r--   0        0        0      837 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/base.py
--rw-r--r--   0        0        0     1976 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/db.py
--rw-r--r--   0        0        0     1319 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/jwt.py
--rw-r--r--   0        0        0     1151 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/redis.py
--rw-r--r--   0        0        0     9027 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/models.py
--rw-r--r--   0        0        0      805 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/auth/schemas.py
--rw-r--r--   0        0        0     1902 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2949 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     2729 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/fastapi_user_auth/site.py
--rw-r--r--   0        0        0   177210 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/pdm.lock
--rw-r--r--   0        0        0     2380 2023-03-04 15:49:58.418149 fastapi_user_auth-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     1137 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/__init__.py
--rw-r--r--   0        0        0     4909 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/conftest.py
--rw-r--r--   0        0        0      812 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth.py
--rw-r--r--   0        0        0     1372 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_mount.py
--rw-r--r--   0        0        0     6711 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_requires.py
--rw-r--r--   0        0        0      945 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_router.py
--rw-r--r--   0        0        0     1241 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_auth_user_model.py
--rw-r--r--   0        0        0     1102 2023-03-04 15:49:58.422149 fastapi_user_auth-0.5.0/tests/test_auth/test_backend.py
--rw-r--r--   0        0        0    13416 1970-01-01 00:00:00.000000 fastapi_user_auth-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       98 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/.flake8
+-rw-r--r--   0        0        0     1662 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      977 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2083 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/.gitignore
+-rw-r--r--   0        0        0      326 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11156 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/README.md
+-rw-r--r--   0        0        0    10287 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/README.zh.md
+-rw-r--r--   0        0        0      345 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/fastapi_user_auth/__init__.py
+-rw-r--r--   0        0        0    11462 2023-08-05 14:32:15.892967 fastapi_user_auth-0.5.1/fastapi_user_auth/admin.py
+-rw-r--r--   0        0        0     3386 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/app.py
+-rw-r--r--   0        0        0      119 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/__init__.py
+-rw-r--r--   0        0        0    12985 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/auth.py
+-rw-r--r--   0        0        0        0 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/__init__.py
+-rw-r--r--   0        0        0      837 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/base.py
+-rw-r--r--   0        0        0     1976 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/db.py
+-rw-r--r--   0        0        0     1319 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/jwt.py
+-rw-r--r--   0        0        0     1151 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/redis.py
+-rw-r--r--   0        0        0     9027 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/models.py
+-rw-r--r--   0        0        0      805 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/auth/schemas.py
+-rw-r--r--   0        0        0     1902 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2949 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     2729 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/fastapi_user_auth/site.py
+-rw-r--r--   0        0        0   109557 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/pdm.lock
+-rw-r--r--   0        0        0     2414 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     1137 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/__init__.py
+-rw-r--r--   0        0        0     4909 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/conftest.py
+-rw-r--r--   0        0        0      812 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/test_auth.py
+-rw-r--r--   0        0        0     1372 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/test_auth_mount.py
+-rw-r--r--   0        0        0     6711 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/test_auth_requires.py
+-rw-r--r--   0        0        0      945 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/test_auth_router.py
+-rw-r--r--   0        0        0     1241 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/test_auth_user_model.py
+-rw-r--r--   0        0        0     1102 2023-08-05 14:32:15.896967 fastapi_user_auth-0.5.1/tests/test_auth/test_backend.py
+-rw-r--r--   0        0        0    13475 1970-01-01 00:00:00.000000 fastapi_user_auth-0.5.1/PKG-INFO
```

### Comparing `fastapi_user_auth-0.5.0/.github/workflows/pytest.yml` & `fastapi_user_auth-0.5.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/.github/workflows/python-publish.yml` & `fastapi_user_auth-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/.gitignore` & `fastapi_user_auth-0.5.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -135,7 +135,8 @@
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 *.db
 /.idea/
 /note/
+/.pdm-python
```

### Comparing `fastapi_user_auth-0.5.0/README.md` & `fastapi_user_auth-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 
 ```python
 # Customize the model management class, inherit and override the corresponding default management class
 class MyGroupAdmin(admin.ModelAdmin):
     page_schema = PageSchema(label='用户组管理', icon='fa fa-group')
     model = MyGroup
     link_model_fields = [Group.roles]
-    readonly_fields = ['key']
+    update_exclude = {"key"}
 
 # Customize the user authentication application, inherit and override the default user authentication application
 class MyUserAuthApp(UserAuthApp):
     GroupAdmin = MyGroupAdmin
 
 # Customize the user management site, inherit and override the default user management site
 class MyAuthAdminSite(AuthAdminSite):
```

### Comparing `fastapi_user_auth-0.5.0/README.zh.md` & `fastapi_user_auth-0.5.1/README.zh.md`

 * *Files 2% similar despite different names*

```diff
@@ -307,15 +307,15 @@
 
 ```python
 # 自定义模型管理类,继承重写对应的默认管理类
 class MyGroupAdmin(admin.ModelAdmin):
     page_schema = PageSchema(label='用户组管理', icon='fa fa-group')
     model = MyGroup
     link_model_fields = [Group.roles]
-    readonly_fields = ['key']
+    update_exclude = {"key"}
 
 # 自定义用户认证应用,继承重写默认的用户认证应用
 class MyUserAuthApp(UserAuthApp):
     GroupAdmin = MyGroupAdmin
 
 # 自定义用户管理站点,继承重写默认的用户管理站点
 class MyAuthAdminSite(AuthAdminSite):
```

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/admin.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,21 +259,21 @@
         return data
 
 
 class RoleAdmin(ModelAdmin):
     page_schema = PageSchema(label=_("Role"), icon="fa fa-group")
     model = Role
     link_model_fields = [Role.permissions]
-    readonly_fields = ["key"]
+    update_exclude = {"key"}
 
 
 class GroupAdmin(ModelAdmin):
     page_schema = PageSchema(label=_("Group"), icon="fa fa-group")
     model = Group
     link_model_fields = [Group.roles]
-    readonly_fields = ["key"]
+    update_exclude = {"key"}
 
 
 class PermissionAdmin(ModelAdmin):
     page_schema = PageSchema(label=_("Permission"), icon="fa fa-lock")
     model = Permission
-    readonly_fields = ["key"]
+    update_exclude = {"key"}
```

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/app.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Type
 
 from fastapi_amis_admin.admin import AdminApp, ModelAdmin, PageSchemaAdmin
 from fastapi_amis_admin.amis.components import PageSchema
-from fastapi_amis_admin.crud.utils import schema_create_by_schema
+from fastapi_amis_admin.utils.pydantic import create_model_by_model
 from fastapi_amis_admin.utils.translation import i18n as _
 from starlette.requests import Request
 
 from fastapi_user_auth.admin import GroupAdmin as DefaultGroupAdmin
 from fastapi_user_auth.admin import PermissionAdmin as DefaultPermissionAdmin
 from fastapi_user_auth.admin import RoleAdmin as DefaultRoleAdmin
 from fastapi_user_auth.admin import UserAdmin as DefaultUserAdmin
@@ -29,24 +29,24 @@
     PermissionAdmin: Type[ModelAdmin] = DefaultPermissionAdmin
 
     def __init__(self, app: "AdminApp"):
         AdminApp.__init__(self, app)
         self.auth = self.auth or self.site.auth
         AuthRouter.__init__(self)
         self.UserAdmin.model = self.UserAdmin.model or self.auth.user_model
-        self.UserLoginFormAdmin.schema = self.UserLoginFormAdmin.schema or schema_create_by_schema(
+        self.UserLoginFormAdmin.schema = self.UserLoginFormAdmin.schema or create_model_by_model(
             self.auth.user_model, "UserLoginIn", include={"username", "password"}
         )
         self.UserLoginFormAdmin.schema_submit_out = self.UserLoginFormAdmin.schema_submit_out or self.schema_user_login_out
-        self.UserRegFormAdmin.schema = self.UserRegFormAdmin.schema or schema_create_by_schema(
+        self.UserRegFormAdmin.schema = self.UserRegFormAdmin.schema or create_model_by_model(
             self.auth.user_model, "UserRegIn", include={"username", "password", "email"}
         )
         self.UserRegFormAdmin.schema_submit_out = self.UserRegFormAdmin.schema_submit_out or self.schema_user_login_out
         self.UserInfoFormAdmin.user_model = self.auth.user_model
-        self.UserInfoFormAdmin.schema = self.UserInfoFormAdmin.schema or schema_create_by_schema(
+        self.UserInfoFormAdmin.schema = self.UserInfoFormAdmin.schema or create_model_by_model(
             self.auth.user_model,
             "UserInfoForm",
             include={"nickname", "password", "avatar", "email"},
             set_none=True,
         )
         self.UserInfoFormAdmin.schema_submit_out = self.UserInfoFormAdmin.schema_submit_out or self.schema_user_info
         # register admin
```

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/auth.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/auth/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 )
 
 from fastapi import Depends, FastAPI, Form, HTTPException, params
 from fastapi.security import OAuth2PasswordBearer
 from fastapi.security.utils import get_authorization_scheme_param
 from fastapi_amis_admin.crud.base import RouterMixin
 from fastapi_amis_admin.crud.schema import BaseApiOut
-from fastapi_amis_admin.crud.utils import schema_create_by_schema
 from fastapi_amis_admin.utils.functools import cached_property
+from fastapi_amis_admin.utils.pydantic import create_model_by_model
 from fastapi_amis_admin.utils.translation import i18n as _
 from passlib.context import CryptContext
 from pydantic import BaseModel, SecretStr
 from sqlalchemy.orm import Session
 from sqlalchemy_database import AsyncDatabase, Database
 from sqlmodel import select
 from starlette.authentication import AuthenticationBackend
@@ -234,15 +234,15 @@
     schema_user_info: Type[BaseModel] = None
 
     def __init__(self, auth: Auth = None):
         self.auth = auth or self.auth
         assert self.auth, "auth is None"
         RouterMixin.__init__(self)
         self.router.dependencies.insert(0, Depends(self.auth.backend.authenticate))
-        self.schema_user_info = self.schema_user_info or schema_create_by_schema(
+        self.schema_user_info = self.schema_user_info or create_model_by_model(
             self.auth.user_model, "UserInfo", exclude={"password"}
         )
 
         self.router.add_api_route(
             "/userinfo",
             self.route_userinfo,
             methods=["GET"],
```

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/base.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/db.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/db.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/jwt.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/backends/redis.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/auth/backends/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/models.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/auth/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/auth/schemas.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_user_auth-0.5.1/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_user_auth-0.5.1/fastapi_user_auth/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/fastapi_user_auth/site.py` & `fastapi_user_auth-0.5.1/fastapi_user_auth/site.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/pyproject.toml` & `fastapi_user_auth-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "pydantic>=1.9",
-    "fastapi-amis-admin>=0.5.0,<0.6.0",
-    "email-validator",
+    "fastapi-amis-admin>=0.6.0,<0.7.0",
+    "email-validator>= 1.3.1",
     "passlib>=1.7.4",
     "bcrypt>=4.0.0",
-    "sqlmodelx>=0.0.2",
+    "sqlmodelx>=0.0.5",
 ]
 
 [project.urls]
 Documentation = "http://docs.amis.work/"
 Source = "https://github.com/amisadmin/fastapi_user_auth"
 FastAPI-Amis-Admin = "https://github.com/amisadmin/fastapi_amis_admin"
 
@@ -61,14 +61,15 @@
     "pytest >=6.2.4",
     "pytest-asyncio>=0.17",
     "aiosqlite>=0.15.0",
     "python-jose==3.3.0",
     "jinja2 >=2.11.2,<4.0.0",
     "ujson>=5.5.0",
     "requests>=2.28.1",
+    "httpx>=0.24.0,<1.0",
 ]
 dev = [
     "fastapi-user-auth[test]",
     "pre-commit>=2.20.0",
 ]
 all = [
     "fastapi-user-auth[dev]",
```

### Comparing `fastapi_user_auth-0.5.0/tests/conftest.py` & `fastapi_user_auth-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/tests/test_auth/conftest.py` & `fastapi_user_auth-0.5.1/tests/test_auth/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/tests/test_auth/test_auth.py` & `fastapi_user_auth-0.5.1/tests/test_auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/tests/test_auth/test_auth_mount.py` & `fastapi_user_auth-0.5.1/tests/test_auth/test_auth_mount.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/tests/test_auth/test_auth_requires.py` & `fastapi_user_auth-0.5.1/tests/test_auth/test_auth_requires.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/tests/test_auth/test_auth_router.py` & `fastapi_user_auth-0.5.1/tests/test_auth/test_auth_router.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/tests/test_auth/test_auth_user_model.py` & `fastapi_user_auth-0.5.1/tests/test_auth/test_auth_user_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/tests/test_auth/test_backend.py` & `fastapi_user_auth-0.5.1/tests/test_auth/test_backend.py`

 * *Files identical despite different names*

### Comparing `fastapi_user_auth-0.5.0/PKG-INFO` & `fastapi_user_auth-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_auth
-Version: 0.5.0
+Version: 0.5.1
 Summary: FastAPI-User-Auth is a simple and powerful FastAPI user RBAC authentication and authorization library. Based on FastAPI-Amis-Admin and provides a freely extensible visual management interface.
 Keywords: fastapi,fastapi-user-auth,fastapi-amis-admin,fastapi-auth,fastapi-users,fastapi-jwt-auth,sqlmodel
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
@@ -15,32 +15,33 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic>=1.9
-Requires-Dist: fastapi-amis-admin>=0.5.0,<0.6.0
-Requires-Dist: email-validator
+Requires-Dist: fastapi-amis-admin>=0.6.0,<0.7.0
+Requires-Dist: email-validator>= 1.3.1
 Requires-Dist: passlib>=1.7.4
 Requires-Dist: bcrypt>=4.0.0
-Requires-Dist: sqlmodelx>=0.0.2
+Requires-Dist: sqlmodelx>=0.0.5
 Requires-Dist: fastapi-user-auth[dev] ; extra == "all"
 Requires-Dist: fastapi-user-auth[test] ; extra == "dev"
 Requires-Dist: pre-commit>=2.20.0 ; extra == "dev"
 Requires-Dist: python-jose==3.3.0 ; extra == "jwt"
 Requires-Dist: aioredis ; extra == "redis"
 Requires-Dist: uvicorn[standard] >=0.19.0,<1.0 ; extra == "test"
 Requires-Dist: pytest >=6.2.4 ; extra == "test"
 Requires-Dist: pytest-asyncio>=0.17 ; extra == "test"
 Requires-Dist: aiosqlite>=0.15.0 ; extra == "test"
 Requires-Dist: python-jose==3.3.0 ; extra == "test"
 Requires-Dist: jinja2 >=2.11.2,<4.0.0 ; extra == "test"
 Requires-Dist: ujson>=5.5.0 ; extra == "test"
 Requires-Dist: requests>=2.28.1 ; extra == "test"
+Requires-Dist: httpx>=0.24.0,<1.0 ; extra == "test"
 Project-URL: Documentation, http://docs.amis.work/
 Project-URL: FastAPI-Amis-Admin, https://github.com/amisadmin/fastapi_amis_admin
 Project-URL: Source, https://github.com/amisadmin/fastapi_user_auth
 Provides-Extra: all
 Provides-Extra: db
 Provides-Extra: dev
 Provides-Extra: jwt
@@ -357,15 +358,15 @@
 
 ```python
 # Customize the model management class, inherit and override the corresponding default management class
 class MyGroupAdmin(admin.ModelAdmin):
     page_schema = PageSchema(label='用户组管理', icon='fa fa-group')
     model = MyGroup
     link_model_fields = [Group.roles]
-    readonly_fields = ['key']
+    update_exclude = {"key"}
 
 # Customize the user authentication application, inherit and override the default user authentication application
 class MyUserAuthApp(UserAuthApp):
     GroupAdmin = MyGroupAdmin
 
 # Customize the user management site, inherit and override the default user management site
 class MyAuthAdminSite(AuthAdminSite):
```

