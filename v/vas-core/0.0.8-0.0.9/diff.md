# Comparing `tmp/vas_core-0.0.8.tar.gz` & `tmp/vas_core-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vas_core-0.0.8.tar", last modified: Thu Mar 30 21:30:20 2023, max compression
+gzip compressed data, was "vas_core-0.0.9.tar", last modified: Sat Aug  5 10:14:42 2023, max compression
```

## Comparing `vas_core-0.0.8.tar` & `vas_core-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-30 21:30:20.900920 vas_core-0.0.8/
--rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 vas_core-0.0.8/LICENSE
--rw-r--r--   0 macbookpro   (501) staff       (20)      416 2023-03-30 21:30:20.900697 vas_core-0.0.8/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 vas_core-0.0.8/pyproject.toml
--rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-03-30 21:30:20.900982 vas_core-0.0.8/setup.cfg
--rw-r--r--   0 macbookpro   (501) staff       (20)     1103 2023-03-30 21:30:03.000000 vas_core-0.0.8/setup.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-30 21:30:20.891598 vas_core-0.0.8/vas_core/
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2022-06-12 16:59:19.000000 vas_core-0.0.8/vas_core/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      799 2022-06-14 10:21:06.000000 vas_core-0.0.8/vas_core/api_response.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-30 21:30:20.894187 vas_core-0.0.8/vas_core/app/
--rw-r--r--   0 macbookpro   (501) staff       (20)      374 2023-03-13 12:45:19.000000 vas_core-0.0.8/vas_core/app/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1794 2022-10-03 07:58:29.000000 vas_core-0.0.8/vas_core/app/admin.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      502 2022-09-17 00:59:28.000000 vas_core-0.0.8/vas_core/app/apps.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-30 21:30:20.894847 vas_core-0.0.8/vas_core/app/managers/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2022-06-13 10:16:14.000000 vas_core-0.0.8/vas_core/app/managers/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      510 2022-06-24 19:33:41.000000 vas_core-0.0.8/vas_core/app/managers/base_redis_manager.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1211 2022-09-10 21:26:34.000000 vas_core-0.0.8/vas_core/app/managers/config_manager.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-30 21:30:20.896524 vas_core-0.0.8/vas_core/app/migrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)    20064 2022-10-03 08:16:24.000000 vas_core-0.0.8/vas_core/app/migrations/0001_initial.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     5460 2023-03-11 11:00:38.000000 vas_core-0.0.8/vas_core/app/migrations/0002_rename_deletedviacascade_accountconfig_deleted_via_cascade_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      608 2023-03-28 18:45:41.000000 vas_core-0.0.8/vas_core/app/migrations/0003_biller_requires_consent_category_requires_consent.py
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2022-06-12 15:54:24.000000 vas_core-0.0.8/vas_core/app/migrations/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-30 21:30:20.900413 vas_core-0.0.8/vas_core/app/models/
--rw-r--r--   0 macbookpro   (501) staff       (20)      219 2022-10-03 07:58:29.000000 vas_core-0.0.8/vas_core/app/models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1808 2023-03-28 18:21:21.000000 vas_core-0.0.8/vas_core/app/models/accounting_entry.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1693 2022-10-10 01:54:57.000000 vas_core-0.0.8/vas_core/app/models/base.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2321 2023-03-30 21:30:03.000000 vas_core-0.0.8/vas_core/app/models/biller.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      822 2023-03-28 18:21:21.000000 vas_core-0.0.8/vas_core/app/models/biller_field.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1045 2023-03-28 18:21:21.000000 vas_core-0.0.8/vas_core/app/models/category.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      839 2023-03-28 18:21:21.000000 vas_core-0.0.8/vas_core/app/models/channel.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      914 2023-03-28 18:21:21.000000 vas_core-0.0.8/vas_core/app/models/country.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      309 2022-09-09 22:07:42.000000 vas_core-0.0.8/vas_core/app/models/localization.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1796 2023-03-13 12:45:19.000000 vas_core-0.0.8/vas_core/app/models/provider.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      762 2023-03-28 18:21:21.000000 vas_core-0.0.8/vas_core/app/models/request.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      748 2022-10-03 08:05:31.000000 vas_core-0.0.8/vas_core/app/models/user.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2935 2023-03-13 16:30:29.000000 vas_core-0.0.8/vas_core/app/signals.py
--rw-r--r--   0 macbookpro   (501) staff       (20)       60 2022-06-12 15:54:24.000000 vas_core-0.0.8/vas_core/app/tests.py
--rw-r--r--   0 macbookpro   (501) staff       (20)       63 2022-06-23 03:08:01.000000 vas_core-0.0.8/vas_core/app/views.py
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2022-06-12 17:02:00.000000 vas_core-0.0.8/vas_core/middlewares.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1734 2022-06-13 08:10:42.000000 vas_core-0.0.8/vas_core/settings.example.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4516 2022-10-10 01:54:57.000000 vas_core-0.0.8/vas_core/settings.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2671 2023-03-14 22:35:19.000000 vas_core-0.0.8/vas_core/utils.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-30 21:30:20.892478 vas_core-0.0.8/vas_core.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)      416 2023-03-30 21:30:20.000000 vas_core-0.0.8/vas_core.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     1227 2023-03-30 21:30:20.000000 vas_core-0.0.8/vas_core.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-03-30 21:30:20.000000 vas_core-0.0.8/vas_core.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      124 2023-03-30 21:30:20.000000 vas_core-0.0.8/vas_core.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        9 2023-03-30 21:30:20.000000 vas_core-0.0.8/vas_core.egg-info/top_level.txt
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-08-05 10:14:42.310647 vas_core-0.0.9/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 vas_core-0.0.9/LICENSE
+-rw-r--r--   0 macbookpro   (501) staff       (20)      416 2023-08-05 10:14:42.310412 vas_core-0.0.9/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 vas_core-0.0.9/pyproject.toml
+-rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-08-05 10:14:42.310711 vas_core-0.0.9/setup.cfg
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1103 2023-08-05 10:13:21.000000 vas_core-0.0.9/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-08-05 10:14:42.285338 vas_core-0.0.9/vas_core/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2022-06-12 16:59:19.000000 vas_core-0.0.9/vas_core/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      799 2022-06-14 10:21:06.000000 vas_core-0.0.9/vas_core/api_response.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-08-05 10:14:42.287660 vas_core-0.0.9/vas_core/app/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      374 2023-03-13 12:45:19.000000 vas_core-0.0.9/vas_core/app/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1946 2023-05-18 12:54:12.000000 vas_core-0.0.9/vas_core/app/admin.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      653 2023-05-03 07:29:46.000000 vas_core-0.0.9/vas_core/app/apps.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-08-05 10:14:42.303980 vas_core-0.0.9/vas_core/app/managers/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2022-06-13 10:16:14.000000 vas_core-0.0.9/vas_core/app/managers/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      510 2022-06-24 19:33:41.000000 vas_core-0.0.9/vas_core/app/managers/base_redis_manager.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1211 2022-09-10 21:26:34.000000 vas_core-0.0.9/vas_core/app/managers/config_manager.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-08-05 10:14:42.306505 vas_core-0.0.9/vas_core/app/migrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)    20064 2022-10-03 08:16:24.000000 vas_core-0.0.9/vas_core/app/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     5460 2023-03-11 11:00:38.000000 vas_core-0.0.9/vas_core/app/migrations/0002_rename_deletedviacascade_accountconfig_deleted_via_cascade_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      608 2023-03-28 18:45:41.000000 vas_core-0.0.9/vas_core/app/migrations/0003_biller_requires_consent_category_requires_consent.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3925 2023-05-03 08:21:33.000000 vas_core-0.0.9/vas_core/app/migrations/0004_billerform_billerformfield_billerformproduct_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2949 2023-05-14 13:26:04.000000 vas_core-0.0.9/vas_core/app/migrations/0005_transaction.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4457 2023-05-18 13:14:34.000000 vas_core-0.0.9/vas_core/app/migrations/0006_remove_accountingentry_fees_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      671 2023-05-18 16:40:39.000000 vas_core-0.0.9/vas_core/app/migrations/0007_remove_accountingentry_settlement_account_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2022-06-12 15:54:24.000000 vas_core-0.0.9/vas_core/app/migrations/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-08-05 10:14:42.310088 vas_core-0.0.9/vas_core/app/models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      273 2023-05-14 10:42:22.000000 vas_core-0.0.9/vas_core/app/models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2473 2023-05-18 14:34:33.000000 vas_core-0.0.9/vas_core/app/models/accounting_entry.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1693 2022-10-10 01:54:57.000000 vas_core-0.0.9/vas_core/app/models/base.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2028 2023-05-18 15:01:36.000000 vas_core-0.0.9/vas_core/app/models/biller.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1361 2023-05-03 06:06:27.000000 vas_core-0.0.9/vas_core/app/models/biller_field.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1714 2023-05-18 14:34:33.000000 vas_core-0.0.9/vas_core/app/models/biller_form.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1053 2023-04-04 14:28:00.000000 vas_core-0.0.9/vas_core/app/models/category.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      866 2023-08-05 07:02:00.000000 vas_core-0.0.9/vas_core/app/models/channel.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      914 2023-03-28 18:21:21.000000 vas_core-0.0.9/vas_core/app/models/country.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      309 2022-09-09 22:07:42.000000 vas_core-0.0.9/vas_core/app/models/localization.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1730 2023-05-18 12:14:09.000000 vas_core-0.0.9/vas_core/app/models/provider.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      762 2023-03-28 18:21:21.000000 vas_core-0.0.9/vas_core/app/models/request.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1758 2023-08-05 07:02:00.000000 vas_core-0.0.9/vas_core/app/models/transaction.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      748 2022-10-03 08:05:31.000000 vas_core-0.0.9/vas_core/app/models/user.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4217 2023-05-03 07:29:46.000000 vas_core-0.0.9/vas_core/app/signals.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)       60 2022-06-12 15:54:24.000000 vas_core-0.0.9/vas_core/app/tests.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)       63 2022-06-23 03:08:01.000000 vas_core-0.0.9/vas_core/app/views.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      531 2023-08-05 07:02:00.000000 vas_core-0.0.9/vas_core/constants.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2022-06-12 17:02:00.000000 vas_core-0.0.9/vas_core/middlewares.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1734 2022-06-13 08:10:42.000000 vas_core-0.0.9/vas_core/settings.example.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4516 2022-10-10 01:54:57.000000 vas_core-0.0.9/vas_core/settings.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2669 2023-04-04 13:38:25.000000 vas_core-0.0.9/vas_core/utils.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-08-05 10:14:42.286109 vas_core-0.0.9/vas_core.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      416 2023-08-05 10:14:42.000000 vas_core-0.0.9/vas_core.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1601 2023-08-05 10:14:42.000000 vas_core-0.0.9/vas_core.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-08-05 10:14:42.000000 vas_core-0.0.9/vas_core.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      124 2023-08-05 10:14:42.000000 vas_core-0.0.9/vas_core.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        9 2023-08-05 10:14:42.000000 vas_core-0.0.9/vas_core.egg-info/top_level.txt
```

### Comparing `vas_core-0.0.8/LICENSE` & `vas_core-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/setup.py` & `vas_core-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'VAS Orchestra core package'
 LONG_DESCRIPTION = 'Package that holds all models and common ' \
                    'functions/classes of VAS Orchestra project'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
```

### Comparing `vas_core-0.0.8/vas_core/api_response.py` & `vas_core-0.0.9/vas_core/api_response.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/admin.py` & `vas_core-0.0.9/vas_core/app/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -49,11 +49,15 @@
 admin.site.register(User_, UserAdmin)
 admin.site.register(Category)
 admin.site.register(Country)
 admin.site.register(AccountConfig)
 admin.site.register(FeeAccountConfig)
 admin.site.register(AccountingEntry)
 admin.site.register(Biller)
-admin.site.register(BillerField)
+admin.site.register(BillerForm)
+admin.site.register(BillerFormField)
+admin.site.register(BillerFormProduct)
 admin.site.register(Provider)
 admin.site.register(Channel)
 admin.site.register(Request)
+admin.site.register(Transaction)
+admin.site.register(ChannelAccountingEntry)
```

### Comparing `vas_core-0.0.8/vas_core/app/managers/config_manager.py` & `vas_core-0.0.9/vas_core/app/managers/config_manager.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/migrations/0001_initial.py` & `vas_core-0.0.9/vas_core/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/migrations/0002_rename_deletedviacascade_accountconfig_deleted_via_cascade_and_more.py` & `vas_core-0.0.9/vas_core/app/migrations/0002_rename_deletedviacascade_accountconfig_deleted_via_cascade_and_more.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/migrations/0003_biller_requires_consent_category_requires_consent.py` & `vas_core-0.0.9/vas_core/app/migrations/0003_biller_requires_consent_category_requires_consent.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/models/accounting_entry.py` & `vas_core-0.0.9/vas_core/app/models/accounting_entry.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,39 +19,50 @@
             "account": self.account,
             "desc": self.description,
             "is_dynamic": self.is_dynamic,
         }
 
 
 class FeeAccountConfig(BaseModelAbstract, models.Model):
+    accounting_entry = models.ForeignKey('AccountingEntry', on_delete=models.CASCADE, related_name='fees')
+    description = models.CharField(max_length=100)
     account = models.ForeignKey("AccountConfig", on_delete=models.CASCADE)
     amount = models.DecimalField(decimal_places=5, max_digits=50, null=False,
                                  blank=False)
+    max_amount = models.DecimalField(decimal_places=5, max_digits=50, default=0)
     is_percentage = models.BooleanField(default=False)
+    deduct_from_amount = models.BooleanField(default=False)
 
     def __str__(self):
-        return f"{self.account} - {self.amount}{ self.is_percentage if '%' else ''}"
+        return f"{self.account} - {self.amount}{ '%' if self.is_percentage else ''}"
 
     def __unicode__(self):
         return self.__str__()
 
     def to_dict(self) -> dict:
         return {
             "account_config": self.account.to_dict(),
             "amount": self.amount,
             "is_percentage": self.is_percentage,
         }
 
 
 class AccountingEntry(BaseModelAbstract, models.Model):
-    settlement_account = models.ForeignKey("AccountConfig",
-                                           on_delete=models.CASCADE)
-    fees = models.ManyToManyField("FeeAccountConfig", null=True, blank=True)
+    country = models.ForeignKey('Country', on_delete=models.CASCADE)
+    description = models.CharField(max_length=100)
+    currency = models.CharField(max_length=5)
+    transit_account = models.CharField(max_length=30, null=True, blank=True)
 
     def to_dict(self) -> dict:
         _fees = []
         for fee in self.fees.all():
             _fees.append(fee.to_dict())
         return {
-            "settlement_account": "",
+            # "settlement_account": self.settlement_account.to_dict(),
             "fees": _fees
         }
+
+
+class ChannelAccountingEntry(BaseModelAbstract, models.Model):
+    biller_form = models.ForeignKey('BillerForm', on_delete=models.CASCADE)
+    channel = models.ForeignKey('Channel', on_delete=models.CASCADE)
+    accounting_entry = models.ForeignKey('AccountingEntry', on_delete=models.CASCADE)
```

### Comparing `vas_core-0.0.8/vas_core/app/models/base.py` & `vas_core-0.0.9/vas_core/app/models/base.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/models/biller.py` & `vas_core-0.0.9/vas_core/app/models/biller.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,24 +14,21 @@
                                  on_delete=models.SET_NULL)
     provider = models.ForeignKey("Provider", null=True, blank=True,
                                  on_delete=models.SET_NULL)
     country = models.ForeignKey("Country", null=True, blank=True,
                                 on_delete=models.SET_NULL)
     display_sequence = models.IntegerField(default=1)
     channels = models.ManyToManyField("Channel")
-    accounting_entry = models.OneToOneField("AccountingEntry",
-                                            null=True, blank=True,
-                                            on_delete=models.SET_NULL)
     narration_format = models.TextField(null=True, blank=True)
     requires_consent = models.BooleanField(default=False)
     is_active = models.BooleanField(default=True)
 
     def __str__(self):
         x = []
-        for k, v in self.name:
+        for k, v in self.name.items():
             x.append(f"{k}: {v}")
         out = ',\n'.join(x)
         return f"{out}\n{self.biller_id}"
 
     def __unicode__(self):
         return self.__str__()
 
@@ -47,10 +44,9 @@
             "category_id": self.category.id if self.category else None,
             "provider_id": self.provider.id if self.provider else None,
             "country_code": self.country.code,
             "narration": self.narration_format,
             "display_sequence": self.display_sequence,
             "requires_consent": self.requires_consent,
             "channels": ",".join([c.code for c in channels]),
-            "accounting_entry": self.accounting_entry.to_dict() if self.accounting_entry else None,
         }
         return json.dumps(data)
```

### Comparing `vas_core-0.0.8/vas_core/app/models/category.py` & `vas_core-0.0.9/vas_core/app/models/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     country = models.ForeignKey("Country", on_delete=models.DO_NOTHING,
                                 null=True, blank=True)
     is_active = models.BooleanField(default=True)
     requires_consent = models.BooleanField(default=False)
 
     def __str__(self):
         x = []
-        for k, v in self.description:
+        for k, v in self.description.items():
             x.append(f"{k}: {v}")
         return ',\n'.join(x)
 
     def __unicode__(self):
         return self.__str__()
 
     class Meta:
```

### Comparing `vas_core-0.0.8/vas_core/app/models/channel.py` & `vas_core-0.0.9/vas_core/app/models/channel.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,11 +20,12 @@
     def save(self, keep_deleted=False, **kwargs):
         self.code = self.code.upper()
         self.shortcode = self.shortcode.upper()
         super(BaseModelAbstract, self).save(keep_deleted, **kwargs)
 
     def to_redis(self) -> str:
         data = {
+            "id": self.id,
             "code": self.code,
             "desc": self.description
         }
         return json.dumps(data)
```

### Comparing `vas_core-0.0.8/vas_core/app/models/country.py` & `vas_core-0.0.9/vas_core/app/models/country.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/models/provider.py` & `vas_core-0.0.9/vas_core/app/models/provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,17 +18,24 @@
     api_url = models.URLField(null=True, blank=True)
     api_type = models.CharField(max_length=10, choices=API_TYPES, null=False,
                                 blank=False)
     auth_username = models.CharField(null=True, blank=True, max_length=255)
     auth_password = models.CharField(null=True, blank=True, max_length=255)
     auth_token = models.CharField(null=True, blank=True, max_length=255)
     notify = models.BooleanField(default=True)
-    accounting_entry = models.OneToOneField("AccountingEntry",
-                                            null=True, blank=True,
-                                            on_delete=models.SET_NULL)
+
+    def __str__(self):
+        x = []
+        for k, v in self.name.items():
+            x.append(f"{k}: {v}")
+        out = ',\n'.join(x)
+        return f"{out}\n{self.code}"
+
+    def __unicode__(self):
+        return self.__str__()
 
     @property
     def has_url(self) -> bool:
         return self.api_url not in (None, '')
 
     @property
     def is_json(self) -> bool:
@@ -44,10 +51,9 @@
             "code": self.code,
             "api_url": self.api_url,
             "api_type": self.api_type,
             "auth_username": self.auth_username,
             "auth_password": self.auth_password,
             "auth_token": self.auth_token,
             "notify": self.notify,
-            "accounting_entry": self.accounting_entry if self.accounting_entry.to_dict() else None,
         }
         return json.dumps(data)
```

### Comparing `vas_core-0.0.8/vas_core/app/models/request.py` & `vas_core-0.0.9/vas_core/app/models/request.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/app/models/user.py` & `vas_core-0.0.9/vas_core/app/models/user.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/settings.example.py` & `vas_core-0.0.9/vas_core/settings.example.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/settings.py` & `vas_core-0.0.9/vas_core/settings.py`

 * *Files identical despite different names*

### Comparing `vas_core-0.0.8/vas_core/utils.py` & `vas_core-0.0.9/vas_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def log_debug(source: str, data: Any):
     logger = logging.getLogger(source)
     logger.debug(msg=data)
 
 
 def log_error(source: str, data: Any):
     logger = logging.getLogger(source)
-    logger.warning(msg=data)
+    logger.error(msg=data)
 
 
 def log_warning(source: str, data: Any):
     logger = logging.getLogger(source)
     logger.warning(msg=data)
```

### Comparing `vas_core-0.0.8/vas_core.egg-info/SOURCES.txt` & `vas_core-0.0.9/vas_core.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 pyproject.toml
 setup.py
 vas_core/__init__.py
 vas_core/api_response.py
+vas_core/constants.py
 vas_core/middlewares.py
 vas_core/settings.example.py
 vas_core/settings.py
 vas_core/utils.py
 vas_core.egg-info/PKG-INFO
 vas_core.egg-info/SOURCES.txt
 vas_core.egg-info/dependency_links.txt
@@ -20,20 +21,26 @@
 vas_core/app/views.py
 vas_core/app/managers/__init__.py
 vas_core/app/managers/base_redis_manager.py
 vas_core/app/managers/config_manager.py
 vas_core/app/migrations/0001_initial.py
 vas_core/app/migrations/0002_rename_deletedviacascade_accountconfig_deleted_via_cascade_and_more.py
 vas_core/app/migrations/0003_biller_requires_consent_category_requires_consent.py
+vas_core/app/migrations/0004_billerform_billerformfield_billerformproduct_and_more.py
+vas_core/app/migrations/0005_transaction.py
+vas_core/app/migrations/0006_remove_accountingentry_fees_and_more.py
+vas_core/app/migrations/0007_remove_accountingentry_settlement_account_and_more.py
 vas_core/app/migrations/__init__.py
 vas_core/app/models/__init__.py
 vas_core/app/models/accounting_entry.py
 vas_core/app/models/base.py
 vas_core/app/models/biller.py
 vas_core/app/models/biller_field.py
+vas_core/app/models/biller_form.py
 vas_core/app/models/category.py
 vas_core/app/models/channel.py
 vas_core/app/models/country.py
 vas_core/app/models/localization.py
 vas_core/app/models/provider.py
 vas_core/app/models/request.py
+vas_core/app/models/transaction.py
 vas_core/app/models/user.py
```

