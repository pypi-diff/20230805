# Comparing `tmp/edc_metadata-0.3.8-py3-none-any.whl.zip` & `tmp/edc_metadata-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 101986 bytes, number of entries: 123
+Zip file size: 101987 bytes, number of entries: 123
 -rw-r--r--  2.0 unx      577 b- defN 21-Mar-01 04:26 edc_metadata/__init__.py
 -rw-r--r--  2.0 unx      169 b- defN 21-May-14 21:39 edc_metadata/admin_site.py
 -rw-r--r--  2.0 unx      958 b- defN 21-Jul-25 23:52 edc_metadata/apps.py
 -rw-r--r--  2.0 unx      464 b- defN 21-Feb-04 19:47 edc_metadata/choices.py
 -rw-r--r--  2.0 unx      134 b- defN 20-Apr-05 14:05 edc_metadata/constants.py
 -rw-r--r--  2.0 unx      296 b- defN 20-May-13 01:40 edc_metadata/exim_resources.py
 -rw-r--r--  2.0 unx     1215 b- defN 20-Mar-04 23:32 edc_metadata/managers.py
@@ -113,13 +113,13 @@
 -rw-r--r--  2.0 unx    23155 b- defN 21-Apr-06 02:03 edc_metadata/tests/tests/test_requisition_rule_group.py
 -rw-r--r--  2.0 unx     3950 b- defN 21-Apr-06 02:03 edc_metadata/tests/tests/test_site_metadata_rules.py
 -rw-r--r--  2.0 unx     6841 b- defN 21-Jul-24 00:54 edc_metadata/tests/tests/test_view_mixin.py
 -rw-r--r--  2.0 unx       51 b- defN 20-Mar-04 23:32 edc_metadata/view_mixins/__init__.py
 -rw-r--r--  2.0 unx     4900 b- defN 21-Feb-04 19:47 edc_metadata/view_mixins/metadata_view_mixin.py
 -rw-r--r--  2.0 unx       32 b- defN 20-Mar-04 23:32 edc_metadata/views/__init__.py
 -rw-r--r--  2.0 unx      502 b- defN 21-Feb-04 19:47 edc_metadata/views/home_view.py
--rw-r--r--  2.0 unx    18047 b- defN 21-Jul-25 23:52 edc_metadata-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    18703 b- defN 21-Jul-25 23:52 edc_metadata-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-25 23:52 edc_metadata-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Jul-25 23:52 edc_metadata-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    12282 b- defN 21-Jul-25 23:52 edc_metadata-0.3.8.dist-info/RECORD
-123 files, 335391 bytes uncompressed, 81840 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx    18047 b- defN 21-Jul-28 02:14 edc_metadata-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18703 b- defN 21-Jul-28 02:14 edc_metadata-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jul-28 02:14 edc_metadata-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 21-Jul-28 02:14 edc_metadata-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    12282 b- defN 21-Jul-28 02:14 edc_metadata-0.3.9.dist-info/RECORD
+123 files, 335391 bytes uncompressed, 81841 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -348,23 +348,23 @@
 
 Filename: edc_metadata/views/__init__.py
 Comment: 
 
 Filename: edc_metadata/views/home_view.py
 Comment: 
 
-Filename: edc_metadata-0.3.8.dist-info/LICENSE
+Filename: edc_metadata-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_metadata-0.3.8.dist-info/METADATA
+Filename: edc_metadata-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_metadata-0.3.8.dist-info/WHEEL
+Filename: edc_metadata-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_metadata-0.3.8.dist-info/top_level.txt
+Filename: edc_metadata-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_metadata-0.3.8.dist-info/RECORD
+Filename: edc_metadata-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `edc_metadata-0.3.8.dist-info/LICENSE` & `edc_metadata-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_metadata-0.3.8.dist-info/METADATA` & `edc_metadata-0.3.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-metadata
-Version: 0.3.8
+Version: 0.3.9
 Summary: Add a metadata layer to data entry.
 Home-page: http://github/clinicedc/edc-metadata
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc data entry metadata
 Platform: UNKNOWN
```

## Comparing `edc_metadata-0.3.8.dist-info/RECORD` & `edc_metadata-0.3.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -112,12 +112,12 @@
 edc_metadata/tests/tests/test_requisition_rule_group.py,sha256=3Qyx72tlXInw46Zi2xuo6GBr-5SOQpm2ZKIyU6pXxl8,23155
 edc_metadata/tests/tests/test_site_metadata_rules.py,sha256=zy_Z-OhLZrl5NWQ5dzRM8z1CBI2-FNYX3c0ZLY6yOmU,3950
 edc_metadata/tests/tests/test_view_mixin.py,sha256=xb2ug2bc-EWnmv5KWwieXOYwiKIWpENBPiv6eSArCu0,6841
 edc_metadata/view_mixins/__init__.py,sha256=9T8WPkrX_NzR3sTZtqMVtjasI2NMBMUCHYZ4yQjKLtc,51
 edc_metadata/view_mixins/metadata_view_mixin.py,sha256=rpDutXuBZrEwZh8wQkFsUq0iSrqwfbvLGYn4sOL_Uc4,4900
 edc_metadata/views/__init__.py,sha256=TBXTih4Mpsg5Oh2jbyXqL9kH7bu3vWNRgVe93hvLCl8,32
 edc_metadata/views/home_view.py,sha256=j5P0kyWIU3NLJSaRffjw-ow3wA78TJqoc7IIkXCDFwk,502
-edc_metadata-0.3.8.dist-info/LICENSE,sha256=wDzqAntLQORAL6vQhVdzZyfsPVvFStZKtkct5DIZjK0,18047
-edc_metadata-0.3.8.dist-info/METADATA,sha256=6CD_NlXriocYrDM-gN0KqWl4wFF7DaqhYsVWHBTAxOs,18703
-edc_metadata-0.3.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-edc_metadata-0.3.8.dist-info/top_level.txt,sha256=K1AIVlo156Gk4JcEgygpOjPc0oe0aSA3KPlpVWtf8_E,13
-edc_metadata-0.3.8.dist-info/RECORD,,
+edc_metadata-0.3.9.dist-info/LICENSE,sha256=wDzqAntLQORAL6vQhVdzZyfsPVvFStZKtkct5DIZjK0,18047
+edc_metadata-0.3.9.dist-info/METADATA,sha256=Ft6y6ACrk1Q9iE7ziYeoMldWaIKnE-zARBG5aaGpb5s,18703
+edc_metadata-0.3.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+edc_metadata-0.3.9.dist-info/top_level.txt,sha256=K1AIVlo156Gk4JcEgygpOjPc0oe0aSA3KPlpVWtf8_E,13
+edc_metadata-0.3.9.dist-info/RECORD,,
```

