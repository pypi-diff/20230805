# Comparing `tmp/edc_visit_schedule-0.3.8-py3-none-any.whl.zip` & `tmp/edc_visit_schedule-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 72722 bytes, number of entries: 87
+Zip file size: 72724 bytes, number of entries: 87
 -rw-r--r--  2.0 unx      355 b- defN 21-Jun-29 19:44 edc_visit_schedule/__init__.py
 -rw-r--r--  2.0 unx      187 b- defN 21-May-14 21:54 edc_visit_schedule/admin_site.py
 -rw-r--r--  2.0 unx     1140 b- defN 20-Mar-05 16:53 edc_visit_schedule/apps.py
 -rw-r--r--  2.0 unx      304 b- defN 21-Feb-06 03:15 edc_visit_schedule/choices.py
 -rw-r--r--  2.0 unx      360 b- defN 20-Mar-04 23:38 edc_visit_schedule/constants.py
 -rw-r--r--  2.0 unx      408 b- defN 20-Mar-04 23:38 edc_visit_schedule/fieldsets.py
 -rw-r--r--  2.0 unx      423 b- defN 20-Mar-04 23:38 edc_visit_schedule/forms.py
@@ -77,13 +77,13 @@
 -rw-r--r--  2.0 unx     1421 b- defN 21-Mar-01 04:12 edc_visit_schedule/visit_schedule/schedules_collection.py
 -rw-r--r--  2.0 unx     4611 b- defN 21-Feb-06 03:15 edc_visit_schedule/visit_schedule/visit_schedule.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-04 23:38 visit_schedule_app/__init__.py
 -rw-r--r--  2.0 unx      310 b- defN 20-Jun-18 19:00 visit_schedule_app/apps.py
 -rw-r--r--  2.0 unx      363 b- defN 21-Feb-06 03:15 visit_schedule_app/consents.py
 -rw-r--r--  2.0 unx     4480 b- defN 21-Feb-06 03:15 visit_schedule_app/models.py
 -rw-r--r--  2.0 unx     3816 b- defN 21-Feb-06 03:15 visit_schedule_app/visit_schedule.py
--rw-r--r--  2.0 unx    18047 b- defN 21-Jul-01 15:39 edc_visit_schedule-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     6651 b- defN 21-Jul-01 15:39 edc_visit_schedule-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-01 15:39 edc_visit_schedule-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 21-Jul-01 15:39 edc_visit_schedule-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8747 b- defN 21-Jul-01 15:39 edc_visit_schedule-0.3.8.dist-info/RECORD
-87 files, 241849 bytes uncompressed, 58316 bytes compressed:  75.9%
+-rw-r--r--  2.0 unx    18047 b- defN 21-Jul-05 15:51 edc_visit_schedule-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6651 b- defN 21-Jul-05 15:51 edc_visit_schedule-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jul-05 15:51 edc_visit_schedule-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 21-Jul-05 15:51 edc_visit_schedule-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     8747 b- defN 21-Jul-05 15:51 edc_visit_schedule-0.3.9.dist-info/RECORD
+87 files, 241849 bytes uncompressed, 58318 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -240,23 +240,23 @@
 
 Filename: visit_schedule_app/models.py
 Comment: 
 
 Filename: visit_schedule_app/visit_schedule.py
 Comment: 
 
-Filename: edc_visit_schedule-0.3.8.dist-info/LICENSE
+Filename: edc_visit_schedule-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_visit_schedule-0.3.8.dist-info/METADATA
+Filename: edc_visit_schedule-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_visit_schedule-0.3.8.dist-info/WHEEL
+Filename: edc_visit_schedule-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_visit_schedule-0.3.8.dist-info/top_level.txt
+Filename: edc_visit_schedule-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_visit_schedule-0.3.8.dist-info/RECORD
+Filename: edc_visit_schedule-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `edc_visit_schedule-0.3.8.dist-info/LICENSE` & `edc_visit_schedule-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_visit_schedule-0.3.8.dist-info/METADATA` & `edc_visit_schedule-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-visit-schedule
-Version: 0.3.8
+Version: 0.3.9
 Summary: .
 Home-page: https://github.com/clinicedc/edc-visit-schedule
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django visit schedule clinical research
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 
 |pypi| |actions| |codecov| |downloads|
 
 edc-visit-schedule
 ------------------
 
 Add data collection schedules to your app.
```

## Comparing `edc_visit_schedule-0.3.8.dist-info/RECORD` & `edc_visit_schedule-0.3.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -76,12 +76,12 @@
 edc_visit_schedule/visit_schedule/schedules_collection.py,sha256=-rNrNPAYulCapmPgCy5Z_jcLGQcNaUJIcnuBo_8N3Qc,1421
 edc_visit_schedule/visit_schedule/visit_schedule.py,sha256=OMaAexJLg2900JxIAX8ZFqC-6vCONCm-4m-pIcAnpv4,4611
 visit_schedule_app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 visit_schedule_app/apps.py,sha256=8dpC_NRfMTIj9au_wjYxSJTs0fDUCX60yNZKJQL2_J4,310
 visit_schedule_app/consents.py,sha256=vdLcmvMFiW7VBzIjSU8D3tLSuYb5rTy79SCh4_Te5Wo,363
 visit_schedule_app/models.py,sha256=M-gyvcsd0hKJSSB5PazV3EEuPUZt11Ufs_G_yoobZwE,4480
 visit_schedule_app/visit_schedule.py,sha256=jBSvFjO_ct2KybVZ5cP4CdVOGj9IxSOL-EFlO65bQE4,3816
-edc_visit_schedule-0.3.8.dist-info/LICENSE,sha256=wDzqAntLQORAL6vQhVdzZyfsPVvFStZKtkct5DIZjK0,18047
-edc_visit_schedule-0.3.8.dist-info/METADATA,sha256=teJ58oCHZK7Ux9kysocrPuzOdB8kc-DAJvclJ6sR_DI,6651
-edc_visit_schedule-0.3.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-edc_visit_schedule-0.3.8.dist-info/top_level.txt,sha256=LLuPScAVKs_AuuHv2UOrhyMgtmYMhO65IC-Y6H_MBJY,38
-edc_visit_schedule-0.3.8.dist-info/RECORD,,
+edc_visit_schedule-0.3.9.dist-info/LICENSE,sha256=wDzqAntLQORAL6vQhVdzZyfsPVvFStZKtkct5DIZjK0,18047
+edc_visit_schedule-0.3.9.dist-info/METADATA,sha256=5cAgC3jcwDtqTAjMXAshWGf2vq9z4Ry8hcNbfot1l6c,6651
+edc_visit_schedule-0.3.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+edc_visit_schedule-0.3.9.dist-info/top_level.txt,sha256=LLuPScAVKs_AuuHv2UOrhyMgtmYMhO65IC-Y6H_MBJY,38
+edc_visit_schedule-0.3.9.dist-info/RECORD,,
```

