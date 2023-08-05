# Comparing `tmp/odoo_addons_oca_account_fiscal_rule-16.0.20230522.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_fiscal_rule-16.0.20230803.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1491 bytes, number of entries: 4
--rw-r--r--  2.0 unx      634 b- defN 23-May-23 02:39 odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 02:39 odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-23 02:39 odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      448 b- defN 23-May-23 02:39 odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/RECORD
-4 files, 1175 bytes uncompressed, 605 bytes compressed:  48.5%
+Zip file size: 1503 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      771 b- defN 23-Aug-04 02:43 odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 02:43 odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-04 02:43 odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      448 b- defN 23-Aug-04 02:43 odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/RECORD
+4 files, 1312 bytes uncompressed, 617 bytes compressed:  53.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_fiscal_rule-16.0.20230522.0.dist-info/METADATA` & `odoo_addons_oca_account_fiscal_rule-16.0.20230803.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-fiscal-rule
-Version: 16.0.20230522.0
+Version: 16.0.20230803.1
 Summary: Meta package for oca-account-fiscal-rule Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
+Requires-Dist: odoo-addon-account-avatax-oca (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-account-avatax-sale-oca (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-fiscal-position-partner-type (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-fiscal-position-type (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-product-fiscal-classification (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-l10n-eu-oss-oca (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

