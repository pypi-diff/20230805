# Comparing `tmp/deployfish-mysql-1.2.8.tar.gz` & `tmp/deployfish-mysql-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deployfish-mysql-1.2.8.tar", last modified: Sat Sep  3 21:30:20 2022, max compression
+gzip compressed data, was "dist/deployfish-mysql-1.2.9.tar", last modified: Fri Sep 16 16:11:03 2022, max compression
```

## Comparing `deployfish-mysql-1.2.8.tar` & `deployfish-mysql-1.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.248080 deployfish-mysql-1.2.8/
--rw-rw-r--   0 cmalek     (501) admin       (80)       85 2022-08-31 21:07:24.000000 deployfish-mysql-1.2.8/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     4567 2022-09-03 21:30:20.248249 deployfish-mysql-1.2.8/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     3551 2022-08-30 22:42:50.000000 deployfish-mysql-1.2.8/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.243171 deployfish-mysql-1.2.8/deployfish_mysql/
--rw-r--r--   0 cmalek     (501) admin       (80)      406 2022-09-03 21:30:08.000000 deployfish-mysql-1.2.8/deployfish_mysql/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.245313 deployfish-mysql-1.2.8/deployfish_mysql/adapters/
--rw-rw-r--   0 cmalek     (501) admin       (80)       44 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.8/deployfish_mysql/adapters/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.245804 deployfish-mysql-1.2.8/deployfish_mysql/adapters/deployfish/
--rw-rw-r--   0 cmalek     (501) admin       (80)      261 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.8/deployfish_mysql/adapters/deployfish/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      227 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.8/deployfish_mysql/adapters/deployfish/mysql.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.246230 deployfish-mysql-1.2.8/deployfish_mysql/controllers/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-08-29 22:31:59.000000 deployfish-mysql-1.2.8/deployfish_mysql/controllers/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)    14443 2022-09-03 21:18:23.000000 deployfish-mysql-1.2.8/deployfish_mysql/controllers/mysql.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.246725 deployfish-mysql-1.2.8/deployfish_mysql/models/
--rw-rw-r--   0 cmalek     (501) admin       (80)       39 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.8/deployfish_mysql/models/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)    17747 2022-08-30 16:31:57.000000 deployfish-mysql-1.2.8/deployfish_mysql/models/mysql.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.247204 deployfish-mysql-1.2.8/deployfish_mysql/templates/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-08-29 21:35:59.000000 deployfish-mysql-1.2.8/deployfish_mysql/templates/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      423 2022-08-29 22:38:38.000000 deployfish-mysql-1.2.8/deployfish_mysql/templates/detail--mysqldatabase.jinja2
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-03 21:30:20.245054 deployfish-mysql-1.2.8/deployfish_mysql.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     4567 2022-09-03 21:30:20.000000 deployfish-mysql-1.2.8/deployfish_mysql.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      687 2022-09-03 21:30:20.000000 deployfish-mysql-1.2.8/deployfish_mysql.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2022-09-03 21:30:20.000000 deployfish-mysql-1.2.8/deployfish_mysql.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       47 2022-09-03 21:30:20.000000 deployfish-mysql-1.2.8/deployfish_mysql.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       40 2022-09-03 21:30:20.000000 deployfish-mysql-1.2.8/deployfish_mysql.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       17 2022-09-03 21:30:20.000000 deployfish-mysql-1.2.8/deployfish_mysql.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      595 2022-09-03 21:30:20.248956 deployfish-mysql-1.2.8/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)      912 2022-08-31 00:10:23.000000 deployfish-mysql-1.2.8/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.978741 deployfish-mysql-1.2.9/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       85 2022-08-31 21:07:24.000000 deployfish-mysql-1.2.9/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4567 2022-09-16 16:11:03.978922 deployfish-mysql-1.2.9/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3551 2022-08-30 22:42:50.000000 deployfish-mysql-1.2.9/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.973329 deployfish-mysql-1.2.9/deployfish_mysql/
+-rw-r--r--   0 cmalek     (501) admin       (80)      406 2022-09-16 16:11:01.000000 deployfish-mysql-1.2.9/deployfish_mysql/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.975786 deployfish-mysql-1.2.9/deployfish_mysql/adapters/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       44 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.9/deployfish_mysql/adapters/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.976346 deployfish-mysql-1.2.9/deployfish_mysql/adapters/deployfish/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      261 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.9/deployfish_mysql/adapters/deployfish/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      227 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.9/deployfish_mysql/adapters/deployfish/mysql.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.976829 deployfish-mysql-1.2.9/deployfish_mysql/controllers/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-08-29 22:31:59.000000 deployfish-mysql-1.2.9/deployfish_mysql/controllers/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    14822 2022-09-16 16:06:19.000000 deployfish-mysql-1.2.9/deployfish_mysql/controllers/mysql.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.977353 deployfish-mysql-1.2.9/deployfish_mysql/models/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       39 2021-05-17 17:45:07.000000 deployfish-mysql-1.2.9/deployfish_mysql/models/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    17747 2022-08-30 16:31:57.000000 deployfish-mysql-1.2.9/deployfish_mysql/models/mysql.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.977872 deployfish-mysql-1.2.9/deployfish_mysql/templates/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-08-29 21:35:59.000000 deployfish-mysql-1.2.9/deployfish_mysql/templates/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      423 2022-08-29 22:38:38.000000 deployfish-mysql-1.2.9/deployfish_mysql/templates/detail--mysqldatabase.jinja2
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2022-09-16 16:11:03.975426 deployfish-mysql-1.2.9/deployfish_mysql.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4567 2022-09-16 16:11:03.000000 deployfish-mysql-1.2.9/deployfish_mysql.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      687 2022-09-16 16:11:03.000000 deployfish-mysql-1.2.9/deployfish_mysql.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2022-09-16 16:11:03.000000 deployfish-mysql-1.2.9/deployfish_mysql.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       47 2022-09-16 16:11:03.000000 deployfish-mysql-1.2.9/deployfish_mysql.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       40 2022-09-16 16:11:03.000000 deployfish-mysql-1.2.9/deployfish_mysql.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       17 2022-09-16 16:11:03.000000 deployfish-mysql-1.2.9/deployfish_mysql.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      595 2022-09-16 16:11:03.979775 deployfish-mysql-1.2.9/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)      912 2022-08-31 00:10:23.000000 deployfish-mysql-1.2.9/setup.py
```

### Comparing `deployfish-mysql-1.2.8/PKG-INFO` & `deployfish-mysql-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deployfish-mysql
-Version: 1.2.8
+Version: 1.2.9
 Summary: Deployfish MySQL plugin
 Home-page: https://github.com/caltechads/deployfish-mysql
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 License: UNKNOWN
 Description: # deployfish-mysql
```

### Comparing `deployfish-mysql-1.2.8/README.md` & `deployfish-mysql-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `deployfish-mysql-1.2.8/deployfish_mysql/controllers/mysql.py` & `deployfish-mysql-1.2.9/deployfish_mysql/controllers/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,33 @@
         label = "mysql"
         description = 'Work with MySQL Databases'
         help = 'Work with MySQL Databases'
         stacked_type = 'nested'
 
     model: Type[Model] = MySQLDatabase
 
+    help_overrides: Dict[str, str] = {
+        'info': 'Show details about an MySQL database connection',
+        'exists': 'Show whether a MySQL database connection exists in deployfish.yml',
+        'list': 'List available MySQL database connections from deployfish.yml',
+    }
+
     info_template: str = 'detail--mysqldatabase.jinja2'
 
     list_ordering: str = 'Name'
     list_result_columns: Dict[str, Any] = {
         'Name': 'name',
         'Host': 'host',
         'DB': 'db',
         'User': 'user',
         'Password': 'password',
     }
 
     @ex(
-        help="Create a MySQL database and user for a Service.",
+        help="Create a MySQL database and user in the remote MySQL server.",
         arguments=[
             (['pk'], {'help': 'the name of the MySQL connection in deployfish.yml'}),
             (
                 ['--root-user'],
                 {
                     'help': 'the username of the root user for the MySQL server',
                     'default': None,
@@ -68,15 +74,15 @@
                     'default': False,
                     'dest': 'verbose',
                     'action': 'store_true'
                 }
             ),
         ],
         description="""
-Create a database and user in a remote MySQL server for a Service.
+Create a database and user in a remote MySQL server.
 """
     )
     @handle_model_exceptions
     def create(self):
         loader = self.loader(self)
         obj = loader.get_object_from_deployfish(self.app.pargs.pk)
         if not self.app.pargs.root_user:
@@ -105,15 +111,15 @@
         ]
         if output:
             lines.append(click.style('\nMySQL output:\n', fg='yellow'))
             lines.append(output)
         self.app.print('\n'.join(lines))
 
     @ex(
-        help="Update a MySQL database and user for a Service.",
+        help="Update a MySQL database and user for in the remote MySQL server.",
         arguments=[
             (['pk'], {'help': 'the name of the MySQL connection in deployfish.yml'}),
             (
                 ['--root-user'],
                 {
                     'help': 'the username of the root user for the MySQL server',
                     'default': None,
@@ -144,17 +150,17 @@
                     'default': False,
                     'dest': 'verbose',
                     'action': 'store_true'
                 }
             ),
         ],
         description="""
-Update an existing database and user in a remote MySQL server for a Service.  This allows you
-to change the database character set and collation, update the user's password and update the
-GRANTs for the user.
+Update an existing database and user in a remote MySQL server.  This allows you
+to change the database character set and collation, update the user's password
+and update the GRANTs for the user.
 """
     )
     @handle_model_exceptions
     def update(self):
         loader = self.loader(self)
         obj = loader.get_object_from_deployfish(self.app.pargs.pk)
         if not self.app.pargs.root_user:
@@ -183,15 +189,15 @@
         ]
         if output:
             lines.append(click.style('\nMySQL output:\n', fg='yellow'))
             lines.append(output)
         self.app.print('\n'.join(lines))
 
     @ex(
-        help="Validate that a MySQL user for a Service exists and has the password we expect.",
+        help="Validate that a MySQL database and user exists in the remote MySQL server and has the password we expect.",
         arguments=[
             (['pk'], {'help': 'the name of the MySQL connection in deployfish.yml'}),
             (
                 ['-c', '--choose'],
                 {
                     'help': 'Choose from all available ssh targets instead of choosing one automatically.',
                     'default': False,
@@ -206,15 +212,16 @@
                     'default': False,
                     'dest': 'verbose',
                     'action': 'store_true'
                 }
             ),
         ],
         description="""
-Validate that a user in a remote MySQL server exists and has the password we expect.
+Validate that a database and user in a remote MySQL server exists in the remote
+MySQL server and has the password we expect.
 """
     )
     @handle_model_exceptions
     def validate(self):
         loader = self.loader(self)
         obj = loader.get_object_from_deployfish(self.app.pargs.pk)
         target = get_ssh_target(self.app, obj.cluster, choose=self.app.pargs.choose)
@@ -286,15 +293,15 @@
         ]
         self.app.print('\n'.join(lines))
 
     @ex(
         help="Load the contents of a local SQL file into an existing MySQL database.",
         arguments=[
             (['pk'], {'help': 'the name of the MySQL connection in deployfish.yml'}),
-            (['filename'], {'help': 'the filename of the SQL file to load'}),
+            (['sqlfile'], {'help': 'the filename of the SQL file to load'}),
             (
                 ['-c', '--choose'],
                 {
                     'help': 'Choose from all available ssh targets instead of choosing one automatically.',
                     'default': False,
                     'dest': 'choose',
                     'action': 'store_true'
@@ -307,27 +314,27 @@
                     'default': False,
                     'dest': 'verbose',
                     'action': 'store_true'
                 }
             ),
         ],
         description="""
-Load the contents of a local SQL file into an existing MySQL database.
+Load the contents of a local SQL file into an existing MySQL database in the remote MySQL server.
 """
     )
     @handle_model_exceptions
     def load(self):
         loader = self.loader(self)
         obj = loader.get_object_from_deployfish(self.app.pargs.pk)
         target = get_ssh_target(self.app, obj.cluster, choose=self.app.pargs.choose)
-        output = obj.load(self.app.pargs.filename, ssh_target=target, verbose=self.app.pargs.verbose)
+        output = obj.load(self.app.pargs.sqlfile, ssh_target=target, verbose=self.app.pargs.verbose)
         lines = [
             click.style(
                 'Loaded file "{}" into database "{}" on mysql server {}:{}'.format(
-                    self.app.pargs.filename, obj.db, obj.host, obj.port
+                    self.app.pargs.sqlfile, obj.db, obj.host, obj.port
                 ),
                 fg='green'
             )
         ]
         if output.strip():
             # This is here just case `mysql` returns 0 but also prints something. Should probably never trigger.
             lines.append(click.style('Output from `mysql` command:\n{}'.format(output), fg='red'))
@@ -365,15 +372,15 @@
         loader = self.loader(self)
         obj = loader.get_object_from_deployfish(self.app.pargs.pk)
         target = get_ssh_target(self.app, obj.cluster, choose=self.app.pargs.choose)
         output = obj.show_grants(ssh_target=target, verbose=self.app.pargs.verbose)
         self.app.print(output)
 
     @ex(
-        help="Show the the MySQL Version for the remote MySQL server.",
+        help="Show the the MySQL version for the remote MySQL server.",
         arguments=[
             (['pk'], {'help': 'the name of the MySQL connection in deployfish.yml'}),
             (
                 ['-c', '--choose'],
                 {
                     'help': 'Choose from all available ssh targets instead of choosing one automatically.',
                     'default': False,
@@ -388,15 +395,15 @@
                     'default': False,
                     'dest': 'verbose',
                     'action': 'store_true'
                 }
             ),
         ],
         description="""
-Print the version of the remote MySQL server.
+Print the MySQL version of the remote MySQL server.
 """
     )
     @handle_model_exceptions
     def server_version(self):
         loader = self.loader(self)
         obj = loader.get_object_from_deployfish(self.app.pargs.pk)
         target = get_ssh_target(self.app, obj.cluster, choose=self.app.pargs.choose)
```

### Comparing `deployfish-mysql-1.2.8/deployfish_mysql/models/mysql.py` & `deployfish-mysql-1.2.9/deployfish_mysql/models/mysql.py`

 * *Files identical despite different names*

### Comparing `deployfish-mysql-1.2.8/deployfish_mysql.egg-info/PKG-INFO` & `deployfish-mysql-1.2.9/deployfish_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deployfish-mysql
-Version: 1.2.8
+Version: 1.2.9
 Summary: Deployfish MySQL plugin
 Home-page: https://github.com/caltechads/deployfish-mysql
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 License: UNKNOWN
 Description: # deployfish-mysql
```

### Comparing `deployfish-mysql-1.2.8/deployfish_mysql.egg-info/SOURCES.txt` & `deployfish-mysql-1.2.9/deployfish_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deployfish-mysql-1.2.8/setup.cfg` & `deployfish-mysql-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `deployfish-mysql-1.2.8/setup.py` & `deployfish-mysql-1.2.9/setup.py`

 * *Files identical despite different names*

