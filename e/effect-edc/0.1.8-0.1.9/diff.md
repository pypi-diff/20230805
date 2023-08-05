# Comparing `tmp/effect-edc-0.1.8.tar.gz` & `tmp/effect-edc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effect-edc-0.1.8.tar", last modified: Thu Jun  2 02:00:36 2022, max compression
+gzip compressed data, was "effect-edc-0.1.9.tar", last modified: Thu Jun  2 12:29:15 2022, max compression
```

## Comparing `effect-edc-0.1.8.tar` & `effect-edc-0.1.9.tar`

### file list

```diff
@@ -1,643 +1,643 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.679757 effect-edc-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       61 2022-01-19 01:36:21.000000 effect-edc-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)     4768 2022-01-19 01:36:21.000000 effect-edc-0.1.8/.env-tests
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.569040 effect-edc-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.578579 effect-edc-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2120 2022-05-05 04:24:48.000000 effect-edc-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1447 2022-05-05 04:24:48.000000 effect-edc-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-05 04:24:48.000000 effect-edc-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)     5730 2022-06-02 01:36:56.000000 effect-edc-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-16 11:21:34.000000 effect-edc-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-05-11 02:56:51.000000 effect-edc-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     3241 2022-06-02 02:00:36.679934 effect-edc-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2393 2022-01-19 01:36:21.000000 effect-edc-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5126 2022-05-11 02:56:51.000000 effect-edc-0.1.8/TODO.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-06-02 02:00:27.000000 effect-edc-0.1.8/VERSION
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.578764 effect-edc-0.1.8/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)   329717 2022-05-11 02:56:51.000000 effect-edc-0.1.8/docs/forms_reference.md
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.583260 effect-edc-0.1.8/effect_ae/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10962 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_ae/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.585510 effect-edc-0.1.8/effect_ae/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      460 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      412 2022-05-05 04:04:46.000000 effect-edc-0.1.8/effect_ae/admin/ae_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2500 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_ae/admin/ae_initial_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      406 2022-05-05 04:04:50.000000 effect-edc-0.1.8/effect_ae/admin/ae_local_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2022-05-05 04:04:52.000000 effect-edc-0.1.8/effect_ae/admin/ae_sponsor_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      391 2022-05-05 04:04:54.000000 effect-edc-0.1.8/effect_ae/admin/ae_susar_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:04:56.000000 effect-edc-0.1.8/effect_ae/admin/ae_tmg_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2300 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_ae/admin/death_report_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-05-05 04:05:02.000000 effect-edc-0.1.8/effect_ae/admin/death_report_tmg_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      470 2022-05-05 04:05:04.000000 effect-edc-0.1.8/effect_ae/admin/death_report_tmg_second_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3747 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_ae/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      289 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1288 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      931 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.585971 effect-edc-0.1.8/effect_ae/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4570 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_ae/form_validators/ae_initial.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.587913 effect-edc-0.1.8/effect_ae/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      438 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-05 04:05:15.000000 effect-edc-0.1.8/effect_ae/forms/ae_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      790 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/forms/ae_initial_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      255 2022-05-05 04:05:20.000000 effect-edc-0.1.8/effect_ae/forms/ae_local_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 04:05:22.000000 effect-edc-0.1.8/effect_ae/forms/ae_sponsor_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      241 2022-05-05 04:05:24.000000 effect-edc-0.1.8/effect_ae/forms/ae_susar_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-05-05 04:05:25.000000 effect-edc-0.1.8/effect_ae/forms/ae_tmg_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 04:05:27.000000 effect-edc-0.1.8/effect_ae/forms/death_report_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/forms/death_report_tmg_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-05-05 04:05:29.000000 effect-edc-0.1.8/effect_ae/forms/death_report_tmg_second_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      849 2022-05-05 21:05:13.000000 effect-edc-0.1.8/effect_ae/forms/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2285 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_ae/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.590206 effect-edc-0.1.8/effect_ae/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   157252 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_ae/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6316 2022-05-05 21:04:52.000000 effect-edc-0.1.8/effect_ae/migrations/0002_auto_20220309_1441.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1493 2022-05-05 21:04:54.000000 effect-edc-0.1.8/effect_ae/migrations/0003_auto_20220322_2029.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1141 2022-05-05 21:04:56.000000 effect-edc-0.1.8/effect_ae/migrations/0004_auto_20220419_2126.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9594 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_ae/migrations/0005_auto_20220504_0602.py
--rw-r--r--   0 erikvw     (501) staff       (20)      903 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_ae/migrations/0006_auto_20220516_1203.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4709 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_ae/migrations/0007_auto_20220516_1759.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.590610 effect-edc-0.1.8/effect_ae/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_ae/model_mixins/ae_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2734 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_ae/model_mixins/death_report_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.592386 effect-edc-0.1.8/effect_ae/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      357 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_ae/models/ae_followup.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.592874 effect-edc-0.1.8/effect_ae/models/ae_initial/
--rw-r--r--   0 erikvw     (501) staff       (20)       34 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/models/ae_initial/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1436 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_ae/models/ae_initial/ae_effect_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/models/ae_initial/ae_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/models/ae_local_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/models/ae_sponsor_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/models/ae_susar.py
--rw-r--r--   0 erikvw     (501) staff       (20)      226 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/models/ae_tmg.py
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/models/death_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/models/death_report_tmg.py
--rw-r--r--   0 erikvw     (501) staff       (20)      565 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/models/death_report_tmg_second.py
--rw-r--r--   0 erikvw     (501) staff       (20)      621 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/models/managers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.593361 effect-edc-0.1.8/effect_ae/pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/pdf_reports/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      171 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/pdf_reports/ae_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      183 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/pdf_reports/death_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      555 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_ae/pdf_reports/pdf_report_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.569684 effect-edc-0.1.8/effect_ae/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.569727 effect-edc-0.1.8/effect_ae/templates/effect_ae/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.593589 effect-edc-0.1.8/effect_ae/templates/effect_ae/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      877 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/templates/effect_ae/bootstrap3/ae_initial_description.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.593798 effect-edc-0.1.8/effect_ae/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1004 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_ae/templatetags/effect_ae_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.594206 effect-edc-0.1.8/effect_ae/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.594528 effect-edc-0.1.8/effect_ae/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4840 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_ae/tests/tests/test_actions.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13725 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_ae/tests/tests/test_ae_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      201 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_ae/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.595420 effect-edc-0.1.8/effect_auth/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_auth/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      229 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_auth/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2344 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_auth/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3053 2022-05-05 04:08:49.000000 effect-edc-0.1.8/effect_auth/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-05-05 04:08:52.000000 effect-edc-0.1.8/effect_auth/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.598544 effect-edc-0.1.8/effect_consent/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      760 2022-05-05 04:08:02.000000 effect-edc-0.1.8/effect_consent/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.599036 effect-edc-0.1.8/effect_consent/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3911 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_consent/admin/subject_consent_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2716 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_consent/admin/subject_reconsent_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_consent/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-05-05 04:08:08.000000 effect-edc-0.1.8/effect_consent/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1287 2022-05-05 04:08:11.000000 effect-edc-0.1.8/effect_consent/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      438 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)       31 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.599383 effect-edc-0.1.8/effect_consent/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)       53 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2358 2022-05-05 04:07:58.000000 effect-edc-0.1.8/effect_consent/forms/subject_consent_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.600420 effect-edc-0.1.8/effect_consent/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    66097 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_consent/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5339 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_consent/migrations/0002_auto_20220112_0015.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.601371 effect-edc-0.1.8/effect_consent/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/models/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3639 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_consent/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4098 2022-05-05 04:07:37.000000 effect-edc-0.1.8/effect_consent/models/subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3645 2022-05-05 04:07:39.000000 effect-edc-0.1.8/effect_consent/models/subject_reconsent.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.601744 effect-edc-0.1.8/effect_consent/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.601947 effect-edc-0.1.8/effect_consent/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_consent/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      384 2022-05-05 04:07:45.000000 effect-edc-0.1.8/effect_consent/tests/tests/test_subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)      920 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_consent/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-05-05 04:08:18.000000 effect-edc-0.1.8/effect_consent/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.602812 effect-edc-0.1.8/effect_dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      204 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.603052 effect-edc-0.1.8/effect_dashboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.603599 effect-edc-0.1.8/effect_dashboard/model_wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)      239 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/model_wrappers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/model_wrappers/ae_initial_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/model_wrappers/death_report_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2074 2022-05-05 04:06:52.000000 effect-edc-0.1.8/effect_dashboard/model_wrappers/subject_screening_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1177 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/patterns.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.570583 effect-edc-0.1.8/effect_dashboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.570620 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.570772 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.604468 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/
--rw-r--r--   0 erikvw     (501) staff       (20)      452 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/add_consent_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      324 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/dashboard_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/eligibility_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      424 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/refusal_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/screening_button.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.604632 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)     2183 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/screening/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.604986 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.605152 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)      230 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/dashboard/top_bar.html
--rw-r--r--   0 erikvw     (501) staff       (20)      275 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/dashboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1255 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.605406 effect-edc-0.1.8/effect_dashboard/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2877 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_dashboard/templatetags/effect_dashboard_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.605957 effect-edc-0.1.8/effect_dashboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      736 2022-05-05 04:07:09.000000 effect-edc-0.1.8/effect_dashboard/tests/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.606335 effect-edc-0.1.8/effect_dashboard/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2510 2022-05-05 04:07:04.000000 effect-edc-0.1.8/effect_dashboard/tests/tests/test_model_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2969 2022-05-05 04:07:13.000000 effect-edc-0.1.8/effect_dashboard/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1340 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.606534 effect-edc-0.1.8/effect_dashboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      239 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.607107 effect-edc-0.1.8/effect_dashboard/views/ae/
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      458 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/ae/ae_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      496 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/ae/death_report_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.607517 effect-edc-0.1.8/effect_dashboard/views/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      675 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/screening/filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2331 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/screening/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.607691 effect-edc-0.1.8/effect_dashboard/views/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/subject/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.608051 effect-edc-0.1.8/effect_dashboard/views/subject/dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/subject/dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/subject/dashboard/dashboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.608441 effect-edc-0.1.8/effect_dashboard/views/subject/listboard/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/subject/listboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1841 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_dashboard/views/subject/listboard/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.610041 effect-edc-0.1.8/effect_edc/
--rw-r--r--   0 erikvw     (501) staff       (20)      923 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      376 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/asgi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      789 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/celery.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.610840 effect-edc-0.1.8/effect_edc/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_edc/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.611127 effect-edc-0.1.8/effect_edc/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_edc/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1016 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_edc/management/commands/update_forms_reference.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1052 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/navbars.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.612657 effect-edc-0.1.8/effect_edc/settings/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/settings/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      666 2022-05-05 03:54:02.000000 effect-edc-0.1.8/effect_edc/settings/debug.py
--rw-r--r--   0 erikvw     (501) staff       (20)    19804 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_edc/settings/defaults.py
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-05-05 03:54:23.000000 effect-edc-0.1.8/effect_edc/settings/live.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1857 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_edc/settings/logging.py
--rw-r--r--   0 erikvw     (501) staff       (20)      579 2022-05-05 03:54:31.000000 effect-edc-0.1.8/effect_edc/settings/minimal.py
--rw-r--r--   0 erikvw     (501) staff       (20)      188 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_edc/settings/uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.571773 effect-edc-0.1.8/effect_edc/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.571811 effect-edc-0.1.8/effect_edc/templates/effect_edc/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.612997 effect-edc-0.1.8/effect_edc/templates/effect_edc/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/templates/effect_edc/bootstrap3/base.html
--rw-r--r--   0 erikvw     (501) staff       (20)     3720 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/templates/effect_edc/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.613313 effect-edc-0.1.8/effect_edc/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.614548 effect-edc-0.1.8/effect_edc/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      224 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/randomization_list.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.614669 effect-edc-0.1.8/effect_edc/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      752 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3283 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_edc/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.614877 effect-edc-0.1.8/effect_edc/views/
--rw-r--r--   0 erikvw     (501) staff       (20)       32 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      878 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/views/home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/wsgi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/wsgi_live.py
--rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_edc/wsgi_uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.610747 effect-edc-0.1.8/effect_edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     3241 2022-06-02 02:00:36.000000 effect-edc-0.1.8/effect_edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    22480 2022-06-02 02:00:36.000000 effect-edc-0.1.8/effect_edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-02 02:00:36.000000 effect-edc-0.1.8/effect_edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-09-28 18:19:31.000000 effect-edc-0.1.8/effect_edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       97 2022-06-02 02:00:36.000000 effect-edc-0.1.8/effect_edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      171 2022-06-02 02:00:36.000000 effect-edc-0.1.8/effect_edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.615316 effect-edc-0.1.8/effect_export/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_export/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      171 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_export/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_export/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      209 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_export/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.616583 effect-edc-0.1.8/effect_labs/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_labs/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       87 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_labs/aliquot_types.py
--rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_labs/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_labs/lab_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      128 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_labs/labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      477 2022-05-05 04:04:14.000000 effect-edc-0.1.8/effect_labs/list_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2352 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_labs/panels.py
--rw-r--r--   0 erikvw     (501) staff       (20)      630 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_labs/processing_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      404 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_labs/reportables.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.617162 effect-edc-0.1.8/effect_labs/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_labs/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      971 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_labs/tests/test_labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      522 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_labs/tests/test_reportables.py
--rw-r--r--   0 erikvw     (501) staff       (20)      116 2022-05-05 04:04:01.000000 effect-edc-0.1.8/effect_labs/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.618380 effect-edc-0.1.8/effect_lists/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      811 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13313 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_lists/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.619908 effect-edc-0.1.8/effect_lists/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    17765 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1482 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_lists/migrations/0002_bloodtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      563 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_lists/migrations/0003_auto_20220215_1625.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1690 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_lists/migrations/0004_auto_20220223_2142.py
--rw-r--r--   0 erikvw     (501) staff       (20)      306 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_lists/migrations/0005_delete_rankinscore.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1683 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_lists/migrations/0006_auto_20220322_2029.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_lists/migrations/0007_auto_20220330_1707.py
--rw-r--r--   0 erikvw     (501) staff       (20)      363 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_lists/migrations/0008_delete_medicinesday14.py
--rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_lists/migrations/0009_delete_bloodtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2031 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_lists/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.620067 effect-edc-0.1.8/effect_lists/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/tests/test_lists.py
--rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_lists/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.621191 effect-edc-0.1.8/effect_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3989 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_prn/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.622177 effect-edc-0.1.8/effect_prn/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      286 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_prn/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1993 2022-05-05 04:02:43.000000 effect-edc-0.1.8/effect_prn/admin/end_of_study_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2241 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_prn/admin/hospitalization_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1962 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/admin/loss_to_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      678 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/admin/onschedule_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3812 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/admin/protocol_deviation_violation_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      285 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1606 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_prn/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.622841 effect-edc-0.1.8/effect_prn/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1032 2022-05-05 04:03:04.000000 effect-edc-0.1.8/effect_prn/form_validators/death_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2135 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/form_validators/end_of_study.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1653 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/form_validators/protocol_deviation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2390 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_prn/form_validators/study_day_form_validator_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.623755 effect-edc-0.1.8/effect_prn/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      232 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_prn/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      863 2022-05-05 04:03:17.000000 effect-edc-0.1.8/effect_prn/forms/end_of_study_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_prn/forms/hospitalization_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1056 2022-05-05 04:03:19.000000 effect-edc-0.1.8/effect_prn/forms/loss_to_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 04:03:22.000000 effect-edc-0.1.8/effect_prn/forms/protocol_deviation_violation_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.625372 effect-edc-0.1.8/effect_prn/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    80461 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_prn/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      837 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/migrations/0002_auto_20220430_1945.py
--rw-r--r--   0 erikvw     (501) staff       (20)      769 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/migrations/0003_auto_20220505_0718.py
--rw-r--r--   0 erikvw     (501) staff       (20)    22376 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_prn/migrations/0004_historicalhospitalization_hospitalization.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2295 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_prn/migrations/0005_auto_20220516_1420.py
--rw-r--r--   0 erikvw     (501) staff       (20)      686 2022-06-02 02:00:27.000000 effect-edc-0.1.8/effect_prn/migrations/0006_alter_protocoldeviationviolation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.626403 effect-edc-0.1.8/effect_prn/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_prn/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1030 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_prn/models/base_study_termination.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2111 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_prn/models/end_of_study.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3165 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_prn/models/hospitalization.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2378 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/models/loss_to_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-05-05 04:01:21.000000 effect-edc-0.1.8/effect_prn/models/onschedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1585 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_prn/models/protocol_deviation_violation.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.626637 effect-edc-0.1.8/effect_prn/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.626806 effect-edc-0.1.8/effect_prn/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      280 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      204 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_prn/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.627866 effect-edc-0.1.8/effect_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.628253 effect-edc-0.1.8/effect_screening/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)       59 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7851 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/admin/subject_screening_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1387 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       28 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5394 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_screening/eligibility.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.628707 effect-edc-0.1.8/effect_screening/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)       57 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2294 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_screening/forms/subject_refusal_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1040 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_screening/forms/subject_screening_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.633998 effect-edc-0.1.8/effect_screening/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    53277 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2524 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0002_auto_20211118_2138.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1596 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0003_auto_20211118_2214.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4517 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/migrations/0004_auto_20211119_1937.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1782 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0005_auto_20211119_2024.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5566 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0006_auto_20211119_2106.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1774 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0007_auto_20211119_2118.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1796 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0008_auto_20211119_2125.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1129 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0009_auto_20220111_1649.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9030 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0010_auto_20220329_1743.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1809 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0011_auto_20220329_1745.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1607 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0012_auto_20220329_1758.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1367 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0013_auto_20220329_1818.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2605 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0014_auto_20220330_1707.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4471 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0015_auto_20220330_1816.py
--rw-r--r--   0 erikvw     (501) staff       (20)      789 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0016_auto_20220330_1828.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9569 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0017_auto_20220405_1936.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12545 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/migrations/0018_auto_20220411_1529.py
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0019_auto_20220411_1538.py
--rw-r--r--   0 erikvw     (501) staff       (20)      988 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_screening/migrations/0020_auto_20220419_2126.py
--rw-r--r--   0 erikvw     (501) staff       (20)      562 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_screening/migrations/0021_auto_20220516_1231.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3902 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/migrations/0022_auto_20220527_1351.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.634664 effect-edc-0.1.8/effect_screening/models/
--rw-r--r--   0 erikvw     (501) staff       (20)       48 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3275 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/models/daily_closing_log.py
--rw-r--r--   0 erikvw     (501) staff       (20)      984 2022-05-05 03:58:53.000000 effect-edc-0.1.8/effect_screening/models/daily_closing_log_revised.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8570 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/models/subject_screening.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.635154 effect-edc-0.1.8/effect_screening/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7099 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_screening/tests/effect_test_case_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_screening/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.635811 effect-edc-0.1.8/effect_screening/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17362 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/tests/tests/test_eligibility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2744 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_screening/tests/tests/test_screening.py
--rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-05-05 03:48:42.000000 effect-edc-0.1.8/effect_screening/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.636533 effect-edc-0.1.8/effect_sites/
--rw-r--r--   0 erikvw     (501) staff       (20)       35 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_sites/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      940 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_sites/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.636654 effect-edc-0.1.8/effect_sites/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_sites/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_sites/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2723 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_sites/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.638486 effect-edc-0.1.8/effect_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3273 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.642742 effect-edc-0.1.8/effect_subject/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     1488 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/admin/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.643624 effect-edc-0.1.8/effect_subject/admin/adherence/
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/adherence/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1255 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/adherence/adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      922 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_four_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      879 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_one_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1477 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_three_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      968 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_two_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2850 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/admin/arv_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/admin/arv_treatment_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/admin/autocomplete_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1036 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/blood_culture_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      913 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/chest_xray_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/admin/clinical_note_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1151 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/diagnoses_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1689 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/admin/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/health_economics_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/histopathology_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.644339 effect-edc-0.1.8/effect_subject/admin/lab_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/admin/lab_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      605 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/admin/lab_results/blood_results_chem_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      598 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/admin/lab_results/blood_results_fbc_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      549 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/admin/lab_results/urinalysis_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1854 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/lp_csf_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1258 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/admin/medical_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-05-05 04:00:27.000000 effect-edc-0.1.8/effect_subject/admin/medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1262 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/mental_status_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      375 2022-05-05 04:00:21.000000 effect-edc-0.1.8/effect_subject/admin/modeladmin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1600 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/admin/patient_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3500 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/patient_treatment_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      767 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/admin/radio_fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2319 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/admin/signs_and_symptoms_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1936 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/admin/study_medication_baseline_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/study_medication_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1929 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/subject_requisition_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2952 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/admin/subject_visit_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1395 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/subject_visit_missed_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1361 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin/tb_diagnostics_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1511 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/admin/vital_signs_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-05-05 04:01:47.000000 effect-edc-0.1.8/effect_subject/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      631 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8326 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      767 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.644574 effect-edc-0.1.8/effect_subject/fields/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/fields/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      962 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/fields/temperature.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.648666 effect-edc-0.1.8/effect_subject/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)     1404 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/forms/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.653931 effect-edc-0.1.8/effect_subject/forms/adherence/
--rw-r--r--   0 erikvw     (501) staff       (20)      288 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/adherence/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      407 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/adherence/adherence_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      452 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/adherence/adherence_stage_four_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/adherence/adherence_stage_one_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/adherence/adherence_stage_three_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/adherence/adherence_stage_two_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      367 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/arv_history_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/arv_treatment_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/blood_culture_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/chest_xray_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/clinical_note_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/diagnoses_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/health_economics_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/histopathology_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.654451 effect-edc-0.1.8/effect_subject/forms/lab_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      153 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/forms/lab_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      646 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/forms/lab_results/blood_results_chem_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      666 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/forms/lab_results/blood_results_fbc_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      655 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/forms/lab_results/urinalysis.py
--rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/lp_csf_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/medical_history_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      521 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/medication_adherence_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/mental_status_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      431 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/patient_history_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/patient_treatment_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      684 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/signs_and_symptoms_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      432 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/study_medication_baseline_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      625 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/study_medication_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      950 2022-05-05 03:51:56.000000 effect-edc-0.1.8/effect_subject/forms/subject_requisition_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1853 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/forms/subject_visit_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2173 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/subject_visit_missed_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2631 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/tb_diagnostics_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      442 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/forms/vital_signs_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      548 2022-05-05 04:02:00.000000 effect-edc-0.1.8/effect_subject/identifiers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.654802 effect-edc-0.1.8/effect_subject/metadata_rules/
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/metadata_rules/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/metadata_rules/metadata_rules.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.670006 effect-edc-0.1.8/effect_subject/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   442107 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    19279 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0002_auto_20211109_0418.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1397 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0003_auto_20220111_1649.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5950 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0004_auto_20220119_0438.py
--rw-r--r--   0 erikvw     (501) staff       (20)    32842 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0005_auto_20220215_1625.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1424 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0006_auto_20220215_1649.py
--rw-r--r--   0 erikvw     (501) staff       (20)   121710 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0007_auto_20220223_2142.py
--rw-r--r--   0 erikvw     (501) staff       (20)      945 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0008_auto_20220223_2236.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2505 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0009_auto_20220223_2256.py
--rw-r--r--   0 erikvw     (501) staff       (20)      591 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0010_auto_20220223_2258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2697 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0011_auto_20220224_1509.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4291 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0012_auto_20220224_1826.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1376 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0013_auto_20220224_1855.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2619 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0014_auto_20220224_1910.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6339 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0015_auto_20220224_1926.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2426 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0016_auto_20220225_0351.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3013 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0017_auto_20220225_0419.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1191 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0018_auto_20220225_0423.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7575 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0019_auto_20220225_0500.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2875 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0020_auto_20220225_2142.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6151 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0021_auto_20220228_2032.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13952 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0022_auto_20220228_2034.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17748 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0023_auto_20220228_2355.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7095 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0024_auto_20220303_2242.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3238 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0025_auto_20220304_1312.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4734 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0026_auto_20220309_1441.py
--rw-r--r--   0 erikvw     (501) staff       (20)   157714 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0027_auto_20220322_2029.py
--rw-r--r--   0 erikvw     (501) staff       (20)      959 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0028_auto_20220322_2146.py
--rw-r--r--   0 erikvw     (501) staff       (20)    19514 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0029_auto_20220324_1825.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4964 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0030_auto_20220324_1900.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3615 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0031_auto_20220329_1743.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1724 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0032_auto_20220331_1639.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0033_auto_20220405_1936.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10383 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0034_auto_20220414_1202.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2452 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0035_auto_20220414_1527.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1379 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0036_auto_20220419_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)    44258 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0037_auto_20220419_2126.py
--rw-r--r--   0 erikvw     (501) staff       (20)      462 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0038_auto_20220420_1158.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2520 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0039_auto_20220420_1619.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2288 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0040_auto_20220421_2009.py
--rw-r--r--   0 erikvw     (501) staff       (20)      500 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0041_auto_20220427_2246.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13589 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0042_auto_20220428_1146.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4502 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0043_auto_20220428_1228.py
--rw-r--r--   0 erikvw     (501) staff       (20)    80590 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0044_auto_20220430_1945.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2964 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0045_auto_20220501_1551.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1460 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0046_auto_20220501_1553.py
--rw-r--r--   0 erikvw     (501) staff       (20)    44820 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0047_auto_20220501_1554.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6211 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0048_auto_20220501_1555.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18593 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0049_auto_20220503_1933.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3632 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0050_auto_20220503_1935.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3503 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0051_auto_20220503_1936.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8157 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0052_auto_20220504_0602.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1983 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0053_auto_20220504_0720.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6165 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0054_auto_20220504_1918.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25469 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0055_auto_20220505_0623.py
--rw-r--r--   0 erikvw     (501) staff       (20)      545 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0056_auto_20220505_0630.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2393 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/migrations/0057_auto_20220505_0718.py
--rw-r--r--   0 erikvw     (501) staff       (20)    46241 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0058_auto_20220507_0553.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2077 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/migrations/0059_auto_20220510_1544.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4320 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/migrations/0060_auto_20220511_0236.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3993 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/migrations/0061_auto_20220511_0546.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11565 2022-05-11 11:52:20.000000 effect-edc-0.1.8/effect_subject/migrations/0062_auto_20220511_1439.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3167 2022-05-11 11:52:20.000000 effect-edc-0.1.8/effect_subject/migrations/0063_auto_20220511_1446.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2008 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/migrations/0064_auto_20220511_2105.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1264 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/migrations/0065_auto_20220512_0010.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8230 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/migrations/0066_auto_20220512_1728.py
--rw-r--r--   0 erikvw     (501) staff       (20)      858 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/migrations/0067_historicalsubjectvisit_document_status_comments_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1155 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/migrations/0068_remove_historicalfollowup_action_item_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1599 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/migrations/0069_auto_20220527_1351.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.670731 effect-edc-0.1.8/effect_subject/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      159 2022-03-30 10:32:49.000000 effect-edc-0.1.8/effect_subject/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2949 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/model_mixins/arv_history_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 03:50:29.000000 effect-edc-0.1.8/effect_subject/model_mixins/crf_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-05-05 03:50:31.000000 effect-edc-0.1.8/effect_subject/model_mixins/search_slug_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.674390 effect-edc-0.1.8/effect_subject/models/
--rw-r--r--   0 erikvw     (501) staff       (20)     1181 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4895 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/models/adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5640 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/models/arv_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2508 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/arv_treatment.py
--rw-r--r--   0 erikvw     (501) staff       (20)      904 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/blood_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/chest_xray.py
--rw-r--r--   0 erikvw     (501) staff       (20)      680 2022-05-05 03:43:40.000000 effect-edc-0.1.8/effect_subject/models/clinical_note.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2455 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/models/diagnoses.py
--rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/health_economics.py
--rw-r--r--   0 erikvw     (501) staff       (20)      912 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/histpathology.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.675074 effect-edc-0.1.8/effect_subject/models/lab_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      131 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/models/lab_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1459 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/models/lab_results/blood_results_chem.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1178 2022-05-11 11:52:20.000000 effect-edc-0.1.8/effect_subject/models/lab_results/blood_results_fbc.py
--rw-r--r--   0 erikvw     (501) staff       (20)      806 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/models/lab_results/urinalysis.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1357 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/lp_csf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2116 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/models/medical_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)      427 2022-05-05 03:43:21.000000 effect-edc-0.1.8/effect_subject/models/medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2181 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/models/mental_status.py
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/off_study_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2498 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/models/patient_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5572 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/models/patient_treatment.py
--rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/proxy_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4545 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/models/signs_and_symptoms.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.675578 effect-edc-0.1.8/effect_subject/models/study_medication/
--rw-r--r--   0 erikvw     (501) staff       (20)      172 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/study_medication/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2487 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/study_medication/study_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)      246 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/study_medication/study_medication_baseline.py
--rw-r--r--   0 erikvw     (501) staff       (20)      224 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/study_medication/study_medication_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      410 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/subject_requisition.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3613 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_subject/models/subject_visit.py
--rw-r--r--   0 erikvw     (501) staff       (20)      669 2022-05-05 03:42:19.000000 effect-edc-0.1.8/effect_subject/models/subject_visit_missed.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1111 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/models/tb_diagnostics.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2483 2022-06-02 01:36:56.000000 effect-edc-0.1.8/effect_subject/models/vital_signs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      349 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/reference_model_configs.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.676015 effect-edc-0.1.8/effect_subject/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.677944 effect-edc-0.1.8/effect_subject/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_subject/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3578 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      601 2022-05-05 03:39:55.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_baseline_actions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2031 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_clinical_note.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11505 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_diagnoses.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4813 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_mental_status.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7159 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_metadata_rules.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25948 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_patient_treatment.py
--rw-r--r--   0 erikvw     (501) staff       (20)    39786 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_signs_and_symptoms.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26738 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_subject_visit.py
--rw-r--r--   0 erikvw     (501) staff       (20)      558 2022-05-25 22:45:51.000000 effect-edc-0.1.8/effect_subject/tests/tests/test_vital_signs.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1180 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_subject/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      211 2022-05-05 04:02:05.000000 effect-edc-0.1.8/effect_subject/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.678361 effect-edc-0.1.8/effect_visit_schedule/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_visit_schedule/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_visit_schedule/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      124 2022-01-19 01:36:21.000000 effect-edc-0.1.8/effect_visit_schedule/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.678603 effect-edc-0.1.8/effect_visit_schedule/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_visit_schedule/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.678769 effect-edc-0.1.8/effect_visit_schedule/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_visit_schedule/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8860 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_visit_schedule/tests/tests/test_schedule.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 02:00:36.679570 effect-edc-0.1.8/effect_visit_schedule/visit_schedules/
--rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_visit_schedule/visit_schedules/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7549 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_visit_schedule/visit_schedules/crfs.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1360 2022-05-11 02:56:51.000000 effect-edc-0.1.8/effect_visit_schedule/visit_schedules/requisitions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4319 2022-05-05 04:24:48.000000 effect-edc-0.1.8/effect_visit_schedule/visit_schedules/schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      420 2022-05-05 03:48:05.000000 effect-edc-0.1.8/effect_visit_schedule/visit_schedules/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1425 2022-01-19 01:36:21.000000 effect-edc-0.1.8/holidays.csv
--rwxr-xr-x   0 erikvw     (501) staff       (20)      672 2022-01-19 01:36:21.000000 effect-edc-0.1.8/manage.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1996 2022-05-25 18:58:17.000000 effect-edc-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     7033 2022-05-25 22:45:51.000000 effect-edc-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1263 2022-06-02 02:00:36.680275 effect-edc-0.1.8/setup.cfg
--rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-01-19 01:36:21.000000 effect-edc-0.1.8/wsgi_live.py
--rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-01-19 01:36:21.000000 effect-edc-0.1.8/wsgi_uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.623108 effect-edc-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       61 2022-01-19 01:36:21.000000 effect-edc-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)     4768 2022-01-19 01:36:21.000000 effect-edc-0.1.9/.env-tests
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.516150 effect-edc-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.525571 effect-edc-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2120 2022-05-05 04:24:48.000000 effect-edc-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1447 2022-05-05 04:24:48.000000 effect-edc-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-05 04:24:48.000000 effect-edc-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)     5730 2022-06-02 01:36:56.000000 effect-edc-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-16 11:21:34.000000 effect-edc-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-05-11 02:56:51.000000 effect-edc-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     3241 2022-06-02 12:29:15.623273 effect-edc-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2393 2022-01-19 01:36:21.000000 effect-edc-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5126 2022-05-11 02:56:51.000000 effect-edc-0.1.9/TODO.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-06-02 12:29:06.000000 effect-edc-0.1.9/VERSION
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.525743 effect-edc-0.1.9/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)   329717 2022-05-11 02:56:51.000000 effect-edc-0.1.9/docs/forms_reference.md
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.528361 effect-edc-0.1.9/effect_ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10962 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_ae/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.530475 effect-edc-0.1.9/effect_ae/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      460 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      412 2022-05-05 04:04:46.000000 effect-edc-0.1.9/effect_ae/admin/ae_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2500 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_ae/admin/ae_initial_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      406 2022-05-05 04:04:50.000000 effect-edc-0.1.9/effect_ae/admin/ae_local_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2022-05-05 04:04:52.000000 effect-edc-0.1.9/effect_ae/admin/ae_sponsor_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      391 2022-05-05 04:04:54.000000 effect-edc-0.1.9/effect_ae/admin/ae_susar_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:04:56.000000 effect-edc-0.1.9/effect_ae/admin/ae_tmg_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2300 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_ae/admin/death_report_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-05-05 04:05:02.000000 effect-edc-0.1.9/effect_ae/admin/death_report_tmg_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      470 2022-05-05 04:05:04.000000 effect-edc-0.1.9/effect_ae/admin/death_report_tmg_second_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3747 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_ae/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      289 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1288 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      931 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.530889 effect-edc-0.1.9/effect_ae/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4570 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_ae/form_validators/ae_initial.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.532724 effect-edc-0.1.9/effect_ae/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      438 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-05 04:05:15.000000 effect-edc-0.1.9/effect_ae/forms/ae_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      790 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/forms/ae_initial_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      255 2022-05-05 04:05:20.000000 effect-edc-0.1.9/effect_ae/forms/ae_local_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 04:05:22.000000 effect-edc-0.1.9/effect_ae/forms/ae_sponsor_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      241 2022-05-05 04:05:24.000000 effect-edc-0.1.9/effect_ae/forms/ae_susar_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-05-05 04:05:25.000000 effect-edc-0.1.9/effect_ae/forms/ae_tmg_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 04:05:27.000000 effect-edc-0.1.9/effect_ae/forms/death_report_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/forms/death_report_tmg_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-05-05 04:05:29.000000 effect-edc-0.1.9/effect_ae/forms/death_report_tmg_second_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      849 2022-05-05 21:05:13.000000 effect-edc-0.1.9/effect_ae/forms/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2285 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_ae/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.535139 effect-edc-0.1.9/effect_ae/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   157252 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_ae/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6316 2022-05-05 21:04:52.000000 effect-edc-0.1.9/effect_ae/migrations/0002_auto_20220309_1441.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1493 2022-05-05 21:04:54.000000 effect-edc-0.1.9/effect_ae/migrations/0003_auto_20220322_2029.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1141 2022-05-05 21:04:56.000000 effect-edc-0.1.9/effect_ae/migrations/0004_auto_20220419_2126.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9594 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_ae/migrations/0005_auto_20220504_0602.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      903 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_ae/migrations/0006_auto_20220516_1203.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4709 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_ae/migrations/0007_auto_20220516_1759.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.535574 effect-edc-0.1.9/effect_ae/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_ae/model_mixins/ae_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2734 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_ae/model_mixins/death_report_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.537435 effect-edc-0.1.9/effect_ae/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      357 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_ae/models/ae_followup.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.537947 effect-edc-0.1.9/effect_ae/models/ae_initial/
+-rw-r--r--   0 erikvw     (501) staff       (20)       34 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/models/ae_initial/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1436 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_ae/models/ae_initial/ae_effect_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/models/ae_initial/ae_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/models/ae_local_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/models/ae_sponsor_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/models/ae_susar.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      226 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/models/ae_tmg.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/models/death_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/models/death_report_tmg.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      565 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/models/death_report_tmg_second.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      621 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/models/managers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.538454 effect-edc-0.1.9/effect_ae/pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/pdf_reports/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      171 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/pdf_reports/ae_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      183 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/pdf_reports/death_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      555 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_ae/pdf_reports/pdf_report_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.516797 effect-edc-0.1.9/effect_ae/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.516844 effect-edc-0.1.9/effect_ae/templates/effect_ae/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.538677 effect-edc-0.1.9/effect_ae/templates/effect_ae/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      877 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/templates/effect_ae/bootstrap3/ae_initial_description.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.538889 effect-edc-0.1.9/effect_ae/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1004 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_ae/templatetags/effect_ae_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.539339 effect-edc-0.1.9/effect_ae/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.539684 effect-edc-0.1.9/effect_ae/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4840 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_ae/tests/tests/test_actions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13725 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_ae/tests/tests/test_ae_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      201 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_ae/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.540594 effect-edc-0.1.9/effect_auth/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_auth/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      229 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_auth/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2344 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_auth/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3053 2022-05-05 04:08:49.000000 effect-edc-0.1.9/effect_auth/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-05-05 04:08:52.000000 effect-edc-0.1.9/effect_auth/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.542067 effect-edc-0.1.9/effect_consent/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      760 2022-05-05 04:08:02.000000 effect-edc-0.1.9/effect_consent/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.542565 effect-edc-0.1.9/effect_consent/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3911 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_consent/admin/subject_consent_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2716 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_consent/admin/subject_reconsent_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_consent/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-05-05 04:08:08.000000 effect-edc-0.1.9/effect_consent/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1287 2022-05-05 04:08:11.000000 effect-edc-0.1.9/effect_consent/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      438 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       31 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.542867 effect-edc-0.1.9/effect_consent/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)       53 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2358 2022-05-05 04:07:58.000000 effect-edc-0.1.9/effect_consent/forms/subject_consent_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.543594 effect-edc-0.1.9/effect_consent/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    66097 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_consent/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5339 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_consent/migrations/0002_auto_20220112_0015.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.544570 effect-edc-0.1.9/effect_consent/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/models/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3639 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_consent/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4098 2022-05-05 04:07:37.000000 effect-edc-0.1.9/effect_consent/models/subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3645 2022-05-05 04:07:39.000000 effect-edc-0.1.9/effect_consent/models/subject_reconsent.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.544941 effect-edc-0.1.9/effect_consent/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.545160 effect-edc-0.1.9/effect_consent/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_consent/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      384 2022-05-05 04:07:45.000000 effect-edc-0.1.9/effect_consent/tests/tests/test_subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      920 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_consent/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-05-05 04:08:18.000000 effect-edc-0.1.9/effect_consent/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.545974 effect-edc-0.1.9/effect_dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      204 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.546212 effect-edc-0.1.9/effect_dashboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.546767 effect-edc-0.1.9/effect_dashboard/model_wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)      239 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/model_wrappers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/model_wrappers/ae_initial_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/model_wrappers/death_report_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2074 2022-05-05 04:06:52.000000 effect-edc-0.1.9/effect_dashboard/model_wrappers/subject_screening_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1177 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/patterns.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.517694 effect-edc-0.1.9/effect_dashboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.517734 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.517902 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.547587 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/add_consent_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      324 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/dashboard_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/eligibility_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      424 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/refusal_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/buttons/screening_button.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.547751 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2183 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/screening/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.548052 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.548209 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)      230 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/dashboard/top_bar.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      275 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/dashboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1255 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.548466 effect-edc-0.1.9/effect_dashboard/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2877 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_dashboard/templatetags/effect_dashboard_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.549046 effect-edc-0.1.9/effect_dashboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      736 2022-05-05 04:07:09.000000 effect-edc-0.1.9/effect_dashboard/tests/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.549457 effect-edc-0.1.9/effect_dashboard/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2510 2022-05-05 04:07:04.000000 effect-edc-0.1.9/effect_dashboard/tests/tests/test_model_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2969 2022-05-05 04:07:13.000000 effect-edc-0.1.9/effect_dashboard/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1340 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.549640 effect-edc-0.1.9/effect_dashboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      239 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.550292 effect-edc-0.1.9/effect_dashboard/views/ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      458 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/ae/ae_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      496 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/ae/death_report_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.550748 effect-edc-0.1.9/effect_dashboard/views/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      675 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/screening/filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2331 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/screening/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.550901 effect-edc-0.1.9/effect_dashboard/views/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/subject/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.551246 effect-edc-0.1.9/effect_dashboard/views/subject/dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/subject/dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/subject/dashboard/dashboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.551666 effect-edc-0.1.9/effect_dashboard/views/subject/listboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/subject/listboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1841 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_dashboard/views/subject/listboard/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.553254 effect-edc-0.1.9/effect_edc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      923 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      376 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/asgi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      789 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/celery.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.554037 effect-edc-0.1.9/effect_edc/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_edc/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.554200 effect-edc-0.1.9/effect_edc/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_edc/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1016 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_edc/management/commands/update_forms_reference.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1052 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/navbars.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.555623 effect-edc-0.1.9/effect_edc/settings/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/settings/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      666 2022-05-05 03:54:02.000000 effect-edc-0.1.9/effect_edc/settings/debug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    19804 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_edc/settings/defaults.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-05-05 03:54:23.000000 effect-edc-0.1.9/effect_edc/settings/live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1857 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_edc/settings/logging.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      579 2022-05-05 03:54:31.000000 effect-edc-0.1.9/effect_edc/settings/minimal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-06-02 12:29:06.000000 effect-edc-0.1.9/effect_edc/settings/uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.518872 effect-edc-0.1.9/effect_edc/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.518913 effect-edc-0.1.9/effect_edc/templates/effect_edc/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.555913 effect-edc-0.1.9/effect_edc/templates/effect_edc/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/templates/effect_edc/bootstrap3/base.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     3720 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/templates/effect_edc/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.556218 effect-edc-0.1.9/effect_edc/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.557333 effect-edc-0.1.9/effect_edc/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      224 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/randomization_list.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.557453 effect-edc-0.1.9/effect_edc/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      752 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3283 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_edc/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.557663 effect-edc-0.1.9/effect_edc/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)       32 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      878 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/views/home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/wsgi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/wsgi_live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_edc/wsgi_uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.553937 effect-edc-0.1.9/effect_edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3241 2022-06-02 12:29:15.000000 effect-edc-0.1.9/effect_edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    22480 2022-06-02 12:29:15.000000 effect-edc-0.1.9/effect_edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-02 12:29:15.000000 effect-edc-0.1.9/effect_edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-09-28 18:19:31.000000 effect-edc-0.1.9/effect_edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       97 2022-06-02 12:29:15.000000 effect-edc-0.1.9/effect_edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      171 2022-06-02 12:29:15.000000 effect-edc-0.1.9/effect_edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.558167 effect-edc-0.1.9/effect_export/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_export/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      171 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_export/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_export/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      209 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_export/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.559714 effect-edc-0.1.9/effect_labs/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_labs/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       87 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_labs/aliquot_types.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_labs/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_labs/lab_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      128 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_labs/labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      477 2022-05-05 04:04:14.000000 effect-edc-0.1.9/effect_labs/list_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2352 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_labs/panels.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      630 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_labs/processing_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      404 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_labs/reportables.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.560372 effect-edc-0.1.9/effect_labs/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_labs/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      971 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_labs/tests/test_labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      522 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_labs/tests/test_reportables.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      116 2022-05-05 04:04:01.000000 effect-edc-0.1.9/effect_labs/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.561540 effect-edc-0.1.9/effect_lists/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      811 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13313 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_lists/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.563010 effect-edc-0.1.9/effect_lists/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    17765 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1482 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_lists/migrations/0002_bloodtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      563 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_lists/migrations/0003_auto_20220215_1625.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1690 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_lists/migrations/0004_auto_20220223_2142.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      306 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_lists/migrations/0005_delete_rankinscore.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1683 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_lists/migrations/0006_auto_20220322_2029.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_lists/migrations/0007_auto_20220330_1707.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      363 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_lists/migrations/0008_delete_medicinesday14.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_lists/migrations/0009_delete_bloodtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2031 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_lists/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.563167 effect-edc-0.1.9/effect_lists/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/tests/test_lists.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_lists/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.564278 effect-edc-0.1.9/effect_prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3989 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_prn/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.565306 effect-edc-0.1.9/effect_prn/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      286 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_prn/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1993 2022-05-05 04:02:43.000000 effect-edc-0.1.9/effect_prn/admin/end_of_study_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2241 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_prn/admin/hospitalization_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1962 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/admin/loss_to_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      678 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/admin/onschedule_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3812 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/admin/protocol_deviation_violation_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      285 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1606 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_prn/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.566066 effect-edc-0.1.9/effect_prn/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1032 2022-05-05 04:03:04.000000 effect-edc-0.1.9/effect_prn/form_validators/death_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2135 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/form_validators/end_of_study.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1653 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/form_validators/protocol_deviation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2390 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_prn/form_validators/study_day_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.567093 effect-edc-0.1.9/effect_prn/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      232 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_prn/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      863 2022-05-05 04:03:17.000000 effect-edc-0.1.9/effect_prn/forms/end_of_study_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_prn/forms/hospitalization_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1056 2022-05-05 04:03:19.000000 effect-edc-0.1.9/effect_prn/forms/loss_to_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 04:03:22.000000 effect-edc-0.1.9/effect_prn/forms/protocol_deviation_violation_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.568786 effect-edc-0.1.9/effect_prn/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    80461 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_prn/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      837 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/migrations/0002_auto_20220430_1945.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      769 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/migrations/0003_auto_20220505_0718.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    22376 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_prn/migrations/0004_historicalhospitalization_hospitalization.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2295 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_prn/migrations/0005_auto_20220516_1420.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      686 2022-06-02 02:00:27.000000 effect-edc-0.1.9/effect_prn/migrations/0006_alter_protocoldeviationviolation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.569793 effect-edc-0.1.9/effect_prn/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_prn/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1030 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_prn/models/base_study_termination.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2111 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_prn/models/end_of_study.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3165 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_prn/models/hospitalization.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2378 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/models/loss_to_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-05-05 04:01:21.000000 effect-edc-0.1.9/effect_prn/models/onschedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1585 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_prn/models/protocol_deviation_violation.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.570036 effect-edc-0.1.9/effect_prn/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.570199 effect-edc-0.1.9/effect_prn/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      280 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      204 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_prn/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.571332 effect-edc-0.1.9/effect_screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.571782 effect-edc-0.1.9/effect_screening/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)       59 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7851 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/admin/subject_screening_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1387 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       28 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5394 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_screening/eligibility.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.572413 effect-edc-0.1.9/effect_screening/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)       57 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2294 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_screening/forms/subject_refusal_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1040 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_screening/forms/subject_screening_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.576567 effect-edc-0.1.9/effect_screening/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    53277 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2524 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0002_auto_20211118_2138.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1596 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0003_auto_20211118_2214.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4517 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/migrations/0004_auto_20211119_1937.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1782 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0005_auto_20211119_2024.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5566 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0006_auto_20211119_2106.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1774 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0007_auto_20211119_2118.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1796 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0008_auto_20211119_2125.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1129 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0009_auto_20220111_1649.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9030 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0010_auto_20220329_1743.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1809 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0011_auto_20220329_1745.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1607 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0012_auto_20220329_1758.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1367 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0013_auto_20220329_1818.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2605 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0014_auto_20220330_1707.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4471 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0015_auto_20220330_1816.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      789 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0016_auto_20220330_1828.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9569 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0017_auto_20220405_1936.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12545 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/migrations/0018_auto_20220411_1529.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0019_auto_20220411_1538.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      988 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_screening/migrations/0020_auto_20220419_2126.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      562 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_screening/migrations/0021_auto_20220516_1231.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3902 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/migrations/0022_auto_20220527_1351.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.577226 effect-edc-0.1.9/effect_screening/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       48 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3275 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/models/daily_closing_log.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      984 2022-05-05 03:58:53.000000 effect-edc-0.1.9/effect_screening/models/daily_closing_log_revised.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8570 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/models/subject_screening.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.577739 effect-edc-0.1.9/effect_screening/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7099 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_screening/tests/effect_test_case_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_screening/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.578509 effect-edc-0.1.9/effect_screening/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17362 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/tests/tests/test_eligibility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2744 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_screening/tests/tests/test_screening.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-05-05 03:48:42.000000 effect-edc-0.1.9/effect_screening/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.579248 effect-edc-0.1.9/effect_sites/
+-rw-r--r--   0 erikvw     (501) staff       (20)       35 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_sites/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      940 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_sites/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.579406 effect-edc-0.1.9/effect_sites/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_sites/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_sites/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2723 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_sites/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.581457 effect-edc-0.1.9/effect_subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3273 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.586548 effect-edc-0.1.9/effect_subject/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1488 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/admin/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.587496 effect-edc-0.1.9/effect_subject/admin/adherence/
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/adherence/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1255 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/adherence/adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      922 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_four_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      879 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_one_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1477 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_three_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      968 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_two_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2850 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/admin/arv_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/admin/arv_treatment_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/admin/autocomplete_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1036 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/blood_culture_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      913 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/chest_xray_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/admin/clinical_note_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1151 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/diagnoses_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1689 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/admin/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/health_economics_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/histopathology_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.588312 effect-edc-0.1.9/effect_subject/admin/lab_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/admin/lab_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      605 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/admin/lab_results/blood_results_chem_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      598 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/admin/lab_results/blood_results_fbc_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      549 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/admin/lab_results/urinalysis_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1854 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/lp_csf_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1258 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/admin/medical_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-05-05 04:00:27.000000 effect-edc-0.1.9/effect_subject/admin/medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1262 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/mental_status_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      375 2022-05-05 04:00:21.000000 effect-edc-0.1.9/effect_subject/admin/modeladmin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1600 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/admin/patient_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3500 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/patient_treatment_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      767 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/admin/radio_fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2319 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/admin/signs_and_symptoms_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1936 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/admin/study_medication_baseline_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/study_medication_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1929 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/subject_requisition_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2952 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/admin/subject_visit_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1395 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/subject_visit_missed_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1361 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin/tb_diagnostics_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1511 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/admin/vital_signs_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-05-05 04:01:47.000000 effect-edc-0.1.9/effect_subject/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      631 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8326 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      767 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.588588 effect-edc-0.1.9/effect_subject/fields/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/fields/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      962 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/fields/temperature.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.592698 effect-edc-0.1.9/effect_subject/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1404 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/forms/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.594784 effect-edc-0.1.9/effect_subject/forms/adherence/
+-rw-r--r--   0 erikvw     (501) staff       (20)      288 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/adherence/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      407 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/adherence/adherence_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/adherence/adherence_stage_four_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/adherence/adherence_stage_one_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/adherence/adherence_stage_three_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/adherence/adherence_stage_two_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      367 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/arv_history_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/arv_treatment_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/blood_culture_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/chest_xray_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/clinical_note_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      362 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/diagnoses_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/health_economics_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/histopathology_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.595346 effect-edc-0.1.9/effect_subject/forms/lab_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      153 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/forms/lab_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      646 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/forms/lab_results/blood_results_chem_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      666 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/forms/lab_results/blood_results_fbc_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      655 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/forms/lab_results/urinalysis.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/lp_csf_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/medical_history_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      521 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/medication_adherence_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/mental_status_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      431 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/patient_history_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/patient_treatment_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      684 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/signs_and_symptoms_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      432 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/study_medication_baseline_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      625 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/study_medication_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      950 2022-05-05 03:51:56.000000 effect-edc-0.1.9/effect_subject/forms/subject_requisition_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1853 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/forms/subject_visit_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2173 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/subject_visit_missed_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2631 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/tb_diagnostics_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      442 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/forms/vital_signs_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      548 2022-05-05 04:02:00.000000 effect-edc-0.1.9/effect_subject/identifiers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.595733 effect-edc-0.1.9/effect_subject/metadata_rules/
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/metadata_rules/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/metadata_rules/metadata_rules.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.611240 effect-edc-0.1.9/effect_subject/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   442107 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    19279 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0002_auto_20211109_0418.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1397 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0003_auto_20220111_1649.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5950 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0004_auto_20220119_0438.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    32842 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0005_auto_20220215_1625.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1424 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0006_auto_20220215_1649.py
+-rw-r--r--   0 erikvw     (501) staff       (20)   121710 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0007_auto_20220223_2142.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      945 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0008_auto_20220223_2236.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2505 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0009_auto_20220223_2256.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      591 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0010_auto_20220223_2258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2697 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0011_auto_20220224_1509.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4291 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0012_auto_20220224_1826.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1376 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0013_auto_20220224_1855.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2619 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0014_auto_20220224_1910.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6339 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0015_auto_20220224_1926.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2426 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0016_auto_20220225_0351.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3013 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0017_auto_20220225_0419.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1191 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0018_auto_20220225_0423.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7575 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0019_auto_20220225_0500.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2875 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0020_auto_20220225_2142.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6151 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0021_auto_20220228_2032.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13952 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0022_auto_20220228_2034.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17748 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0023_auto_20220228_2355.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7095 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0024_auto_20220303_2242.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3238 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0025_auto_20220304_1312.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4734 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0026_auto_20220309_1441.py
+-rw-r--r--   0 erikvw     (501) staff       (20)   157714 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0027_auto_20220322_2029.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      959 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0028_auto_20220322_2146.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    19514 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0029_auto_20220324_1825.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4964 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0030_auto_20220324_1900.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3615 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0031_auto_20220329_1743.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1724 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0032_auto_20220331_1639.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0033_auto_20220405_1936.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10383 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0034_auto_20220414_1202.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2452 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0035_auto_20220414_1527.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1379 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0036_auto_20220419_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    44258 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0037_auto_20220419_2126.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      462 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0038_auto_20220420_1158.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2520 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0039_auto_20220420_1619.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2288 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0040_auto_20220421_2009.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      500 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0041_auto_20220427_2246.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13589 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0042_auto_20220428_1146.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4502 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0043_auto_20220428_1228.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    80590 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0044_auto_20220430_1945.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2964 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0045_auto_20220501_1551.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1460 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0046_auto_20220501_1553.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    44820 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0047_auto_20220501_1554.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6211 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0048_auto_20220501_1555.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18593 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0049_auto_20220503_1933.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3632 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0050_auto_20220503_1935.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3503 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0051_auto_20220503_1936.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8157 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0052_auto_20220504_0602.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1983 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0053_auto_20220504_0720.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6165 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0054_auto_20220504_1918.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25469 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0055_auto_20220505_0623.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      545 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0056_auto_20220505_0630.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2393 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/migrations/0057_auto_20220505_0718.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    46241 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0058_auto_20220507_0553.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2077 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/migrations/0059_auto_20220510_1544.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4320 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/migrations/0060_auto_20220511_0236.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3993 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/migrations/0061_auto_20220511_0546.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11565 2022-05-11 11:52:20.000000 effect-edc-0.1.9/effect_subject/migrations/0062_auto_20220511_1439.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3167 2022-05-11 11:52:20.000000 effect-edc-0.1.9/effect_subject/migrations/0063_auto_20220511_1446.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2008 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/migrations/0064_auto_20220511_2105.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1264 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/migrations/0065_auto_20220512_0010.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8230 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/migrations/0066_auto_20220512_1728.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      858 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/migrations/0067_historicalsubjectvisit_document_status_comments_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1155 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/migrations/0068_remove_historicalfollowup_action_item_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1599 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/migrations/0069_auto_20220527_1351.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.612042 effect-edc-0.1.9/effect_subject/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      159 2022-03-30 10:32:49.000000 effect-edc-0.1.9/effect_subject/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2949 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/model_mixins/arv_history_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-05 03:50:29.000000 effect-edc-0.1.9/effect_subject/model_mixins/crf_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-05-05 03:50:31.000000 effect-edc-0.1.9/effect_subject/model_mixins/search_slug_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.615678 effect-edc-0.1.9/effect_subject/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1181 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4895 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/models/adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5640 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/models/arv_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2508 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/arv_treatment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      904 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/blood_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/chest_xray.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      680 2022-05-05 03:43:40.000000 effect-edc-0.1.9/effect_subject/models/clinical_note.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2455 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/models/diagnoses.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/health_economics.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      912 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/histpathology.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.616398 effect-edc-0.1.9/effect_subject/models/lab_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      131 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/models/lab_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1459 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/models/lab_results/blood_results_chem.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1178 2022-05-11 11:52:20.000000 effect-edc-0.1.9/effect_subject/models/lab_results/blood_results_fbc.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      806 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/models/lab_results/urinalysis.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1357 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/lp_csf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2116 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/models/medical_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      427 2022-05-05 03:43:21.000000 effect-edc-0.1.9/effect_subject/models/medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2181 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/models/mental_status.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/off_study_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2498 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/models/patient_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5572 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/models/patient_treatment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/proxy_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4545 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/models/signs_and_symptoms.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.616939 effect-edc-0.1.9/effect_subject/models/study_medication/
+-rw-r--r--   0 erikvw     (501) staff       (20)      172 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/study_medication/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2487 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/study_medication/study_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      246 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/study_medication/study_medication_baseline.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      224 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/study_medication/study_medication_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      410 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/subject_requisition.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3613 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_subject/models/subject_visit.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      669 2022-05-05 03:42:19.000000 effect-edc-0.1.9/effect_subject/models/subject_visit_missed.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1111 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/models/tb_diagnostics.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2483 2022-06-02 01:36:56.000000 effect-edc-0.1.9/effect_subject/models/vital_signs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      349 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/reference_model_configs.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.617376 effect-edc-0.1.9/effect_subject/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.621237 effect-edc-0.1.9/effect_subject/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_subject/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3578 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      601 2022-05-05 03:39:55.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_baseline_actions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2031 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_clinical_note.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11505 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_diagnoses.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4813 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_mental_status.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7159 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_metadata_rules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25948 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_patient_treatment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    39786 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_signs_and_symptoms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26738 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_subject_visit.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      558 2022-05-25 22:45:51.000000 effect-edc-0.1.9/effect_subject/tests/tests/test_vital_signs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1180 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_subject/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      211 2022-05-05 04:02:05.000000 effect-edc-0.1.9/effect_subject/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.621699 effect-edc-0.1.9/effect_visit_schedule/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_visit_schedule/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_visit_schedule/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      124 2022-01-19 01:36:21.000000 effect-edc-0.1.9/effect_visit_schedule/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.621922 effect-edc-0.1.9/effect_visit_schedule/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_visit_schedule/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.622079 effect-edc-0.1.9/effect_visit_schedule/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_visit_schedule/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8860 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_visit_schedule/tests/tests/test_schedule.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-02 12:29:15.622865 effect-edc-0.1.9/effect_visit_schedule/visit_schedules/
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_visit_schedule/visit_schedules/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7549 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_visit_schedule/visit_schedules/crfs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1360 2022-05-11 02:56:51.000000 effect-edc-0.1.9/effect_visit_schedule/visit_schedules/requisitions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4319 2022-05-05 04:24:48.000000 effect-edc-0.1.9/effect_visit_schedule/visit_schedules/schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      420 2022-05-05 03:48:05.000000 effect-edc-0.1.9/effect_visit_schedule/visit_schedules/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1949 2022-06-02 12:29:06.000000 effect-edc-0.1.9/holidays.csv
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      672 2022-01-19 01:36:21.000000 effect-edc-0.1.9/manage.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1996 2022-05-25 18:58:17.000000 effect-edc-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     7033 2022-05-25 22:45:51.000000 effect-edc-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1263 2022-06-02 12:29:15.623649 effect-edc-0.1.9/setup.cfg
+-rw-r--r--   0 erikvw     (501) staff       (20)      176 2022-01-19 01:36:21.000000 effect-edc-0.1.9/wsgi_live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-01-19 01:36:21.000000 effect-edc-0.1.9/wsgi_uat.py
```

### Comparing `effect-edc-0.1.8/.env-tests` & `effect-edc-0.1.9/.env-tests`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/.github/workflows/build.yml` & `effect-edc-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/.gitignore` & `effect-edc-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/CHANGES` & `effect-edc-0.1.9/CHANGES`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/LICENSE` & `effect-edc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/PKG-INFO` & `effect-edc-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effect-edc
-Version: 0.1.8
+Version: 0.1.9
 Summary: EFFECT Trial EDC (http://www.isrctn.com/xxxxx)
 Home-page: https://github.com/clinicedc/effect-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc EFFECT EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `effect-edc-0.1.8/README.rst` & `effect-edc-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/TODO.txt` & `effect-edc-0.1.9/TODO.txt`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/docs/forms_reference.md` & `effect-edc-0.1.9/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/action_items.py` & `effect-edc-0.1.9/effect_ae/action_items.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/admin/ae_initial_admin.py` & `effect-edc-0.1.9/effect_ae/admin/ae_initial_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/admin/death_report_admin.py` & `effect-edc-0.1.9/effect_ae/admin/death_report_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/admin/modeladmin_mixins.py` & `effect-edc-0.1.9/effect_ae/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/baker_recipes.py` & `effect-edc-0.1.9/effect_ae/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/choices.py` & `effect-edc-0.1.9/effect_ae/choices.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/form_validators/ae_initial.py` & `effect-edc-0.1.9/effect_ae/form_validators/ae_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/forms/ae_initial_form.py` & `effect-edc-0.1.9/effect_ae/forms/ae_initial_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/forms/modelform_mixins.py` & `effect-edc-0.1.9/effect_ae/forms/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/list_data.py` & `effect-edc-0.1.9/effect_ae/list_data.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/migrations/0001_initial.py` & `effect-edc-0.1.9/effect_ae/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/migrations/0002_auto_20220309_1441.py` & `effect-edc-0.1.9/effect_ae/migrations/0002_auto_20220309_1441.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/migrations/0003_auto_20220322_2029.py` & `effect-edc-0.1.9/effect_ae/migrations/0003_auto_20220322_2029.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/migrations/0004_auto_20220419_2126.py` & `effect-edc-0.1.9/effect_ae/migrations/0004_auto_20220419_2126.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/migrations/0005_auto_20220504_0602.py` & `effect-edc-0.1.9/effect_ae/migrations/0005_auto_20220504_0602.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/migrations/0006_auto_20220516_1203.py` & `effect-edc-0.1.9/effect_ae/migrations/0006_auto_20220516_1203.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/migrations/0007_auto_20220516_1759.py` & `effect-edc-0.1.9/effect_ae/migrations/0007_auto_20220516_1759.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/model_mixins/ae_review_model_mixin.py` & `effect-edc-0.1.9/effect_ae/model_mixins/ae_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/model_mixins/death_report_model_mixin.py` & `effect-edc-0.1.9/effect_ae/model_mixins/death_report_model_mixin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/models/ae_initial/ae_effect_model_mixin.py` & `effect-edc-0.1.9/effect_ae/models/ae_initial/ae_effect_model_mixin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/models/death_report_tmg_second.py` & `effect-edc-0.1.9/effect_ae/models/death_report_tmg_second.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/models/managers.py` & `effect-edc-0.1.9/effect_ae/models/managers.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/pdf_reports/pdf_report_mixin.py` & `effect-edc-0.1.9/effect_ae/pdf_reports/pdf_report_mixin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/templates/effect_ae/bootstrap3/ae_initial_description.html` & `effect-edc-0.1.9/effect_ae/templates/effect_ae/bootstrap3/ae_initial_description.html`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/templatetags/effect_ae_extras.py` & `effect-edc-0.1.9/effect_ae/templatetags/effect_ae_extras.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/tests/holidays.csv` & `effect-edc-0.1.9/effect_ae/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/tests/tests/test_actions.py` & `effect-edc-0.1.9/effect_ae/tests/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_ae/tests/tests/test_ae_initial.py` & `effect-edc-0.1.9/effect_ae/tests/tests/test_ae_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_auth/auth_objects.py` & `effect-edc-0.1.9/effect_auth/auth_objects.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_auth/auths.py` & `effect-edc-0.1.9/effect_auth/auths.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/action_items.py` & `effect-edc-0.1.9/effect_consent/action_items.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/admin/subject_consent_admin.py` & `effect-edc-0.1.9/effect_consent/admin/subject_consent_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/admin/subject_reconsent_admin.py` & `effect-edc-0.1.9/effect_consent/admin/subject_reconsent_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/baker_recipes.py` & `effect-edc-0.1.9/effect_consent/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/forms/subject_consent_form.py` & `effect-edc-0.1.9/effect_consent/forms/subject_consent_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/migrations/0001_initial.py` & `effect-edc-0.1.9/effect_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/migrations/0002_auto_20220112_0015.py` & `effect-edc-0.1.9/effect_consent/migrations/0002_auto_20220112_0015.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/models/signals.py` & `effect-edc-0.1.9/effect_consent/models/signals.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/models/subject_consent.py` & `effect-edc-0.1.9/effect_consent/models/subject_consent.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/models/subject_reconsent.py` & `effect-edc-0.1.9/effect_consent/models/subject_reconsent.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/tests/holidays.csv` & `effect-edc-0.1.9/effect_consent/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_consent/tests/urls.py` & `effect-edc-0.1.9/effect_consent/tests/urls.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/model_wrappers/subject_screening_model_wrapper.py` & `effect-edc-0.1.9/effect_dashboard/model_wrappers/subject_screening_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/navbars.py` & `effect-edc-0.1.9/effect_dashboard/navbars.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/screening/listboard.html` & `effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/screening/listboard.html`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/listboard.html` & `effect-edc-0.1.9/effect_dashboard/templates/effect_dashboard/bootstrap3/subject/listboard.html`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/templatetags/effect_dashboard_extras.py` & `effect-edc-0.1.9/effect_dashboard/templatetags/effect_dashboard_extras.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/tests/admin.py` & `effect-edc-0.1.9/effect_dashboard/tests/admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/tests/holidays.csv` & `effect-edc-0.1.9/effect_dashboard/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/tests/tests/test_model_wrappers.py` & `effect-edc-0.1.9/effect_dashboard/tests/tests/test_model_wrappers.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/tests/urls.py` & `effect-edc-0.1.9/effect_dashboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/urls.py` & `effect-edc-0.1.9/effect_dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/views/screening/filters.py` & `effect-edc-0.1.9/effect_dashboard/views/screening/filters.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/views/screening/listboard_view.py` & `effect-edc-0.1.9/effect_dashboard/views/screening/listboard_view.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_dashboard/views/subject/listboard/listboard_view.py` & `effect-edc-0.1.9/effect_dashboard/views/subject/listboard/listboard_view.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/admin.py` & `effect-edc-0.1.9/effect_edc/admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/celery.py` & `effect-edc-0.1.9/effect_edc/celery.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/management/commands/update_forms_reference.py` & `effect-edc-0.1.9/effect_edc/management/commands/update_forms_reference.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/navbars.py` & `effect-edc-0.1.9/effect_edc/navbars.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/settings/debug.py` & `effect-edc-0.1.9/effect_edc/settings/debug.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/settings/defaults.py` & `effect-edc-0.1.9/effect_edc/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/settings/logging.py` & `effect-edc-0.1.9/effect_edc/settings/logging.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/settings/minimal.py` & `effect-edc-0.1.9/effect_edc/settings/minimal.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/templates/effect_edc/bootstrap3/home.html` & `effect-edc-0.1.9/effect_edc/templates/effect_edc/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/tests/etc/user-rsa-local-private.pem` & `effect-edc-0.1.9/effect_edc/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/tests/etc/user-rsa-restricted-private.pem` & `effect-edc-0.1.9/effect_edc/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/tests/urls.py` & `effect-edc-0.1.9/effect_edc/tests/urls.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/urls.py` & `effect-edc-0.1.9/effect_edc/urls.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc/views/home_view.py` & `effect-edc-0.1.9/effect_edc/views/home_view.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_edc.egg-info/PKG-INFO` & `effect-edc-0.1.9/effect_edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effect-edc
-Version: 0.1.8
+Version: 0.1.9
 Summary: EFFECT Trial EDC (http://www.isrctn.com/xxxxx)
 Home-page: https://github.com/clinicedc/effect-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc EFFECT EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `effect-edc-0.1.8/effect_edc.egg-info/SOURCES.txt` & `effect-edc-0.1.9/effect_edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_labs/lab_profiles.py` & `effect-edc-0.1.9/effect_labs/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_labs/panels.py` & `effect-edc-0.1.9/effect_labs/panels.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_labs/processing_profiles.py` & `effect-edc-0.1.9/effect_labs/processing_profiles.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_labs/tests/test_labs.py` & `effect-edc-0.1.9/effect_labs/tests/test_labs.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_labs/tests/test_reportables.py` & `effect-edc-0.1.9/effect_labs/tests/test_reportables.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/admin.py` & `effect-edc-0.1.9/effect_lists/admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/list_data.py` & `effect-edc-0.1.9/effect_lists/list_data.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/migrations/0001_initial.py` & `effect-edc-0.1.9/effect_lists/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/migrations/0002_bloodtests.py` & `effect-edc-0.1.9/effect_lists/migrations/0002_bloodtests.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/migrations/0003_auto_20220215_1625.py` & `effect-edc-0.1.9/effect_lists/migrations/0003_auto_20220215_1625.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/migrations/0004_auto_20220223_2142.py` & `effect-edc-0.1.9/effect_lists/migrations/0004_auto_20220223_2142.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/migrations/0006_auto_20220322_2029.py` & `effect-edc-0.1.9/effect_lists/migrations/0006_auto_20220322_2029.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/migrations/0007_auto_20220330_1707.py` & `effect-edc-0.1.9/effect_lists/migrations/0007_auto_20220330_1707.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_lists/models.py` & `effect-edc-0.1.9/effect_lists/models.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/action_items.py` & `effect-edc-0.1.9/effect_prn/action_items.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/admin/end_of_study_admin.py` & `effect-edc-0.1.9/effect_prn/admin/end_of_study_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/admin/hospitalization_admin.py` & `effect-edc-0.1.9/effect_prn/admin/hospitalization_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/admin/loss_to_followup_admin.py` & `effect-edc-0.1.9/effect_prn/admin/loss_to_followup_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/admin/onschedule_admin.py` & `effect-edc-0.1.9/effect_prn/admin/onschedule_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/admin/protocol_deviation_violation_admin.py` & `effect-edc-0.1.9/effect_prn/admin/protocol_deviation_violation_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/choices.py` & `effect-edc-0.1.9/effect_prn/choices.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/constants.py` & `effect-edc-0.1.9/effect_prn/constants.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/form_validators/death_report.py` & `effect-edc-0.1.9/effect_prn/form_validators/death_report.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/form_validators/end_of_study.py` & `effect-edc-0.1.9/effect_prn/form_validators/end_of_study.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/form_validators/protocol_deviation_violation.py` & `effect-edc-0.1.9/effect_prn/form_validators/protocol_deviation_violation.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/form_validators/study_day_form_validator_mixin.py` & `effect-edc-0.1.9/effect_prn/form_validators/study_day_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/forms/end_of_study_form.py` & `effect-edc-0.1.9/effect_prn/forms/end_of_study_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/forms/hospitalization_form.py` & `effect-edc-0.1.9/effect_prn/forms/hospitalization_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/forms/loss_to_followup_form.py` & `effect-edc-0.1.9/effect_prn/forms/loss_to_followup_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/migrations/0001_initial.py` & `effect-edc-0.1.9/effect_prn/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/migrations/0002_auto_20220430_1945.py` & `effect-edc-0.1.9/effect_prn/migrations/0002_auto_20220430_1945.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/migrations/0003_auto_20220505_0718.py` & `effect-edc-0.1.9/effect_prn/migrations/0003_auto_20220505_0718.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/migrations/0004_historicalhospitalization_hospitalization.py` & `effect-edc-0.1.9/effect_prn/migrations/0004_historicalhospitalization_hospitalization.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/migrations/0005_auto_20220516_1420.py` & `effect-edc-0.1.9/effect_prn/migrations/0005_auto_20220516_1420.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/migrations/0006_alter_protocoldeviationviolation_violation.py` & `effect-edc-0.1.9/effect_prn/migrations/0006_alter_protocoldeviationviolation_violation.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/models/base_study_termination.py` & `effect-edc-0.1.9/effect_prn/models/base_study_termination.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/models/end_of_study.py` & `effect-edc-0.1.9/effect_prn/models/end_of_study.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/models/hospitalization.py` & `effect-edc-0.1.9/effect_prn/models/hospitalization.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/models/loss_to_followup.py` & `effect-edc-0.1.9/effect_prn/models/loss_to_followup.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_prn/models/protocol_deviation_violation.py` & `effect-edc-0.1.9/effect_prn/models/protocol_deviation_violation.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/admin/subject_screening_admin.py` & `effect-edc-0.1.9/effect_screening/admin/subject_screening_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/choices.py` & `effect-edc-0.1.9/effect_screening/choices.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/eligibility.py` & `effect-edc-0.1.9/effect_screening/eligibility.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/forms/subject_refusal_form.py` & `effect-edc-0.1.9/effect_screening/forms/subject_refusal_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/forms/subject_screening_form.py` & `effect-edc-0.1.9/effect_screening/forms/subject_screening_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0001_initial.py` & `effect-edc-0.1.9/effect_screening/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0002_auto_20211118_2138.py` & `effect-edc-0.1.9/effect_screening/migrations/0002_auto_20211118_2138.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0003_auto_20211118_2214.py` & `effect-edc-0.1.9/effect_screening/migrations/0003_auto_20211118_2214.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0004_auto_20211119_1937.py` & `effect-edc-0.1.9/effect_screening/migrations/0004_auto_20211119_1937.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0005_auto_20211119_2024.py` & `effect-edc-0.1.9/effect_screening/migrations/0005_auto_20211119_2024.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0006_auto_20211119_2106.py` & `effect-edc-0.1.9/effect_screening/migrations/0006_auto_20211119_2106.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0007_auto_20211119_2118.py` & `effect-edc-0.1.9/effect_screening/migrations/0007_auto_20211119_2118.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0008_auto_20211119_2125.py` & `effect-edc-0.1.9/effect_screening/migrations/0008_auto_20211119_2125.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0009_auto_20220111_1649.py` & `effect-edc-0.1.9/effect_screening/migrations/0009_auto_20220111_1649.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0010_auto_20220329_1743.py` & `effect-edc-0.1.9/effect_screening/migrations/0010_auto_20220329_1743.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0011_auto_20220329_1745.py` & `effect-edc-0.1.9/effect_screening/migrations/0011_auto_20220329_1745.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0012_auto_20220329_1758.py` & `effect-edc-0.1.9/effect_screening/migrations/0012_auto_20220329_1758.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0013_auto_20220329_1818.py` & `effect-edc-0.1.9/effect_screening/migrations/0013_auto_20220329_1818.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0014_auto_20220330_1707.py` & `effect-edc-0.1.9/effect_screening/migrations/0014_auto_20220330_1707.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0015_auto_20220330_1816.py` & `effect-edc-0.1.9/effect_screening/migrations/0015_auto_20220330_1816.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0016_auto_20220330_1828.py` & `effect-edc-0.1.9/effect_screening/migrations/0016_auto_20220330_1828.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0017_auto_20220405_1936.py` & `effect-edc-0.1.9/effect_screening/migrations/0017_auto_20220405_1936.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0018_auto_20220411_1529.py` & `effect-edc-0.1.9/effect_screening/migrations/0018_auto_20220411_1529.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0019_auto_20220411_1538.py` & `effect-edc-0.1.9/effect_screening/migrations/0019_auto_20220411_1538.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0020_auto_20220419_2126.py` & `effect-edc-0.1.9/effect_screening/migrations/0020_auto_20220419_2126.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0021_auto_20220516_1231.py` & `effect-edc-0.1.9/effect_screening/migrations/0021_auto_20220516_1231.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/migrations/0022_auto_20220527_1351.py` & `effect-edc-0.1.9/effect_screening/migrations/0022_auto_20220527_1351.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/models/daily_closing_log.py` & `effect-edc-0.1.9/effect_screening/models/daily_closing_log.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/models/daily_closing_log_revised.py` & `effect-edc-0.1.9/effect_screening/models/daily_closing_log_revised.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/models/subject_screening.py` & `effect-edc-0.1.9/effect_screening/models/subject_screening.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/tests/effect_test_case_mixin.py` & `effect-edc-0.1.9/effect_screening/tests/effect_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/tests/holidays.csv` & `effect-edc-0.1.9/effect_screening/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/tests/tests/test_eligibility.py` & `effect-edc-0.1.9/effect_screening/tests/tests/test_eligibility.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_screening/tests/tests/test_screening.py` & `effect-edc-0.1.9/effect_screening/tests/tests/test_screening.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_sites/apps.py` & `effect-edc-0.1.9/effect_sites/apps.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_sites/sites.py` & `effect-edc-0.1.9/effect_sites/sites.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/action_items.py` & `effect-edc-0.1.9/effect_subject/action_items.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/__init__.py` & `effect-edc-0.1.9/effect_subject/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/adherence/adherence_admin.py` & `effect-edc-0.1.9/effect_subject/admin/adherence/adherence_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_four_admin.py` & `effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_four_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_one_admin.py` & `effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_one_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_three_admin.py` & `effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_three_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/adherence/adherence_stage_two_admin.py` & `effect-edc-0.1.9/effect_subject/admin/adherence/adherence_stage_two_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/arv_history_admin.py` & `effect-edc-0.1.9/effect_subject/admin/arv_history_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/arv_treatment_admin.py` & `effect-edc-0.1.9/effect_subject/admin/arv_treatment_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/blood_culture_admin.py` & `effect-edc-0.1.9/effect_subject/admin/blood_culture_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/chest_xray_admin.py` & `effect-edc-0.1.9/effect_subject/admin/chest_xray_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/clinical_note_admin.py` & `effect-edc-0.1.9/effect_subject/admin/clinical_note_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/diagnoses_admin.py` & `effect-edc-0.1.9/effect_subject/admin/diagnoses_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/fieldsets.py` & `effect-edc-0.1.9/effect_subject/admin/fieldsets.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/health_economics_admin.py` & `effect-edc-0.1.9/effect_subject/admin/health_economics_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/histopathology_admin.py` & `effect-edc-0.1.9/effect_subject/admin/histopathology_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/lab_results/blood_results_chem_admin.py` & `effect-edc-0.1.9/effect_subject/admin/lab_results/blood_results_chem_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/lab_results/blood_results_fbc_admin.py` & `effect-edc-0.1.9/effect_subject/admin/lab_results/blood_results_fbc_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/lab_results/urinalysis_admin.py` & `effect-edc-0.1.9/effect_subject/admin/lab_results/urinalysis_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/lp_csf_admin.py` & `effect-edc-0.1.9/effect_subject/admin/lp_csf_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/medical_history_admin.py` & `effect-edc-0.1.9/effect_subject/admin/medical_history_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/mental_status_admin.py` & `effect-edc-0.1.9/effect_subject/admin/mental_status_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/patient_history_admin.py` & `effect-edc-0.1.9/effect_subject/admin/patient_history_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/patient_treatment_admin.py` & `effect-edc-0.1.9/effect_subject/admin/patient_treatment_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/radio_fields.py` & `effect-edc-0.1.9/effect_subject/admin/radio_fields.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/signs_and_symptoms_admin.py` & `effect-edc-0.1.9/effect_subject/admin/signs_and_symptoms_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/study_medication_baseline_admin.py` & `effect-edc-0.1.9/effect_subject/admin/study_medication_baseline_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/study_medication_followup_admin.py` & `effect-edc-0.1.9/effect_subject/admin/study_medication_followup_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/subject_requisition_admin.py` & `effect-edc-0.1.9/effect_subject/admin/subject_requisition_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/subject_visit_admin.py` & `effect-edc-0.1.9/effect_subject/admin/subject_visit_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/subject_visit_missed_admin.py` & `effect-edc-0.1.9/effect_subject/admin/subject_visit_missed_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/tb_diagnostics_admin.py` & `effect-edc-0.1.9/effect_subject/admin/tb_diagnostics_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/admin/vital_signs_admin.py` & `effect-edc-0.1.9/effect_subject/admin/vital_signs_admin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/baker_recipes.py` & `effect-edc-0.1.9/effect_subject/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/choices.py` & `effect-edc-0.1.9/effect_subject/choices.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/constants.py` & `effect-edc-0.1.9/effect_subject/constants.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/fields/temperature.py` & `effect-edc-0.1.9/effect_subject/fields/temperature.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/__init__.py` & `effect-edc-0.1.9/effect_subject/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/lab_results/blood_results_chem_form.py` & `effect-edc-0.1.9/effect_subject/forms/lab_results/blood_results_chem_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/lab_results/blood_results_fbc_form.py` & `effect-edc-0.1.9/effect_subject/forms/lab_results/blood_results_fbc_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/lab_results/urinalysis.py` & `effect-edc-0.1.9/effect_subject/forms/lab_results/urinalysis.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/medication_adherence_form.py` & `effect-edc-0.1.9/effect_subject/forms/medication_adherence_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/signs_and_symptoms_form.py` & `effect-edc-0.1.9/effect_subject/forms/signs_and_symptoms_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/study_medication_followup_form.py` & `effect-edc-0.1.9/effect_subject/forms/study_medication_followup_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/subject_requisition_form.py` & `effect-edc-0.1.9/effect_subject/forms/subject_requisition_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/subject_visit_form.py` & `effect-edc-0.1.9/effect_subject/forms/subject_visit_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/subject_visit_missed_form.py` & `effect-edc-0.1.9/effect_subject/forms/subject_visit_missed_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/forms/tb_diagnostics_form.py` & `effect-edc-0.1.9/effect_subject/forms/tb_diagnostics_form.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/identifiers.py` & `effect-edc-0.1.9/effect_subject/identifiers.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/metadata_rules/metadata_rules.py` & `effect-edc-0.1.9/effect_subject/metadata_rules/metadata_rules.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0001_initial.py` & `effect-edc-0.1.9/effect_subject/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0002_auto_20211109_0418.py` & `effect-edc-0.1.9/effect_subject/migrations/0002_auto_20211109_0418.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0003_auto_20220111_1649.py` & `effect-edc-0.1.9/effect_subject/migrations/0003_auto_20220111_1649.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0004_auto_20220119_0438.py` & `effect-edc-0.1.9/effect_subject/migrations/0004_auto_20220119_0438.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0005_auto_20220215_1625.py` & `effect-edc-0.1.9/effect_subject/migrations/0005_auto_20220215_1625.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0006_auto_20220215_1649.py` & `effect-edc-0.1.9/effect_subject/migrations/0006_auto_20220215_1649.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0007_auto_20220223_2142.py` & `effect-edc-0.1.9/effect_subject/migrations/0007_auto_20220223_2142.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0008_auto_20220223_2236.py` & `effect-edc-0.1.9/effect_subject/migrations/0008_auto_20220223_2236.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0009_auto_20220223_2256.py` & `effect-edc-0.1.9/effect_subject/migrations/0009_auto_20220223_2256.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0010_auto_20220223_2258.py` & `effect-edc-0.1.9/effect_subject/migrations/0010_auto_20220223_2258.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0011_auto_20220224_1509.py` & `effect-edc-0.1.9/effect_subject/migrations/0011_auto_20220224_1509.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0012_auto_20220224_1826.py` & `effect-edc-0.1.9/effect_subject/migrations/0012_auto_20220224_1826.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0013_auto_20220224_1855.py` & `effect-edc-0.1.9/effect_subject/migrations/0013_auto_20220224_1855.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0014_auto_20220224_1910.py` & `effect-edc-0.1.9/effect_subject/migrations/0014_auto_20220224_1910.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0015_auto_20220224_1926.py` & `effect-edc-0.1.9/effect_subject/migrations/0015_auto_20220224_1926.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0016_auto_20220225_0351.py` & `effect-edc-0.1.9/effect_subject/migrations/0016_auto_20220225_0351.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0017_auto_20220225_0419.py` & `effect-edc-0.1.9/effect_subject/migrations/0017_auto_20220225_0419.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0018_auto_20220225_0423.py` & `effect-edc-0.1.9/effect_subject/migrations/0018_auto_20220225_0423.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0019_auto_20220225_0500.py` & `effect-edc-0.1.9/effect_subject/migrations/0019_auto_20220225_0500.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0020_auto_20220225_2142.py` & `effect-edc-0.1.9/effect_subject/migrations/0020_auto_20220225_2142.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0021_auto_20220228_2032.py` & `effect-edc-0.1.9/effect_subject/migrations/0021_auto_20220228_2032.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0022_auto_20220228_2034.py` & `effect-edc-0.1.9/effect_subject/migrations/0022_auto_20220228_2034.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0023_auto_20220228_2355.py` & `effect-edc-0.1.9/effect_subject/migrations/0023_auto_20220228_2355.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0024_auto_20220303_2242.py` & `effect-edc-0.1.9/effect_subject/migrations/0024_auto_20220303_2242.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0025_auto_20220304_1312.py` & `effect-edc-0.1.9/effect_subject/migrations/0025_auto_20220304_1312.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0026_auto_20220309_1441.py` & `effect-edc-0.1.9/effect_subject/migrations/0026_auto_20220309_1441.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0027_auto_20220322_2029.py` & `effect-edc-0.1.9/effect_subject/migrations/0027_auto_20220322_2029.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0028_auto_20220322_2146.py` & `effect-edc-0.1.9/effect_subject/migrations/0028_auto_20220322_2146.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0029_auto_20220324_1825.py` & `effect-edc-0.1.9/effect_subject/migrations/0029_auto_20220324_1825.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0030_auto_20220324_1900.py` & `effect-edc-0.1.9/effect_subject/migrations/0030_auto_20220324_1900.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0031_auto_20220329_1743.py` & `effect-edc-0.1.9/effect_subject/migrations/0031_auto_20220329_1743.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0032_auto_20220331_1639.py` & `effect-edc-0.1.9/effect_subject/migrations/0032_auto_20220331_1639.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0033_auto_20220405_1936.py` & `effect-edc-0.1.9/effect_subject/migrations/0033_auto_20220405_1936.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0034_auto_20220414_1202.py` & `effect-edc-0.1.9/effect_subject/migrations/0034_auto_20220414_1202.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0035_auto_20220414_1527.py` & `effect-edc-0.1.9/effect_subject/migrations/0035_auto_20220414_1527.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0036_auto_20220419_2036.py` & `effect-edc-0.1.9/effect_subject/migrations/0036_auto_20220419_2036.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0037_auto_20220419_2126.py` & `effect-edc-0.1.9/effect_subject/migrations/0037_auto_20220419_2126.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0039_auto_20220420_1619.py` & `effect-edc-0.1.9/effect_subject/migrations/0039_auto_20220420_1619.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0040_auto_20220421_2009.py` & `effect-edc-0.1.9/effect_subject/migrations/0040_auto_20220421_2009.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0042_auto_20220428_1146.py` & `effect-edc-0.1.9/effect_subject/migrations/0042_auto_20220428_1146.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0043_auto_20220428_1228.py` & `effect-edc-0.1.9/effect_subject/migrations/0043_auto_20220428_1228.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0044_auto_20220430_1945.py` & `effect-edc-0.1.9/effect_subject/migrations/0044_auto_20220430_1945.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0045_auto_20220501_1551.py` & `effect-edc-0.1.9/effect_subject/migrations/0045_auto_20220501_1551.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0046_auto_20220501_1553.py` & `effect-edc-0.1.9/effect_subject/migrations/0046_auto_20220501_1553.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0047_auto_20220501_1554.py` & `effect-edc-0.1.9/effect_subject/migrations/0047_auto_20220501_1554.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0048_auto_20220501_1555.py` & `effect-edc-0.1.9/effect_subject/migrations/0048_auto_20220501_1555.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0049_auto_20220503_1933.py` & `effect-edc-0.1.9/effect_subject/migrations/0049_auto_20220503_1933.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0050_auto_20220503_1935.py` & `effect-edc-0.1.9/effect_subject/migrations/0050_auto_20220503_1935.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0051_auto_20220503_1936.py` & `effect-edc-0.1.9/effect_subject/migrations/0051_auto_20220503_1936.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0052_auto_20220504_0602.py` & `effect-edc-0.1.9/effect_subject/migrations/0052_auto_20220504_0602.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0053_auto_20220504_0720.py` & `effect-edc-0.1.9/effect_subject/migrations/0053_auto_20220504_0720.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0054_auto_20220504_1918.py` & `effect-edc-0.1.9/effect_subject/migrations/0054_auto_20220504_1918.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0055_auto_20220505_0623.py` & `effect-edc-0.1.9/effect_subject/migrations/0055_auto_20220505_0623.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0056_auto_20220505_0630.py` & `effect-edc-0.1.9/effect_subject/migrations/0056_auto_20220505_0630.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0057_auto_20220505_0718.py` & `effect-edc-0.1.9/effect_subject/migrations/0057_auto_20220505_0718.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0058_auto_20220507_0553.py` & `effect-edc-0.1.9/effect_subject/migrations/0058_auto_20220507_0553.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0059_auto_20220510_1544.py` & `effect-edc-0.1.9/effect_subject/migrations/0059_auto_20220510_1544.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0060_auto_20220511_0236.py` & `effect-edc-0.1.9/effect_subject/migrations/0060_auto_20220511_0236.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0061_auto_20220511_0546.py` & `effect-edc-0.1.9/effect_subject/migrations/0061_auto_20220511_0546.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0062_auto_20220511_1439.py` & `effect-edc-0.1.9/effect_subject/migrations/0062_auto_20220511_1439.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0063_auto_20220511_1446.py` & `effect-edc-0.1.9/effect_subject/migrations/0063_auto_20220511_1446.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0064_auto_20220511_2105.py` & `effect-edc-0.1.9/effect_subject/migrations/0064_auto_20220511_2105.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0065_auto_20220512_0010.py` & `effect-edc-0.1.9/effect_subject/migrations/0065_auto_20220512_0010.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0066_auto_20220512_1728.py` & `effect-edc-0.1.9/effect_subject/migrations/0066_auto_20220512_1728.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0067_historicalsubjectvisit_document_status_comments_and_more.py` & `effect-edc-0.1.9/effect_subject/migrations/0067_historicalsubjectvisit_document_status_comments_and_more.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0068_remove_historicalfollowup_action_item_and_more.py` & `effect-edc-0.1.9/effect_subject/migrations/0068_remove_historicalfollowup_action_item_and_more.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/migrations/0069_auto_20220527_1351.py` & `effect-edc-0.1.9/effect_subject/migrations/0069_auto_20220527_1351.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/model_mixins/arv_history_model_mixin.py` & `effect-edc-0.1.9/effect_subject/model_mixins/arv_history_model_mixin.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/__init__.py` & `effect-edc-0.1.9/effect_subject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/adherence.py` & `effect-edc-0.1.9/effect_subject/models/adherence.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/arv_history.py` & `effect-edc-0.1.9/effect_subject/models/arv_history.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/arv_treatment.py` & `effect-edc-0.1.9/effect_subject/models/arv_treatment.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/blood_culture.py` & `effect-edc-0.1.9/effect_subject/models/blood_culture.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/chest_xray.py` & `effect-edc-0.1.9/effect_subject/models/chest_xray.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/clinical_note.py` & `effect-edc-0.1.9/effect_subject/models/clinical_note.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/diagnoses.py` & `effect-edc-0.1.9/effect_subject/models/diagnoses.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/histpathology.py` & `effect-edc-0.1.9/effect_subject/models/histpathology.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/lab_results/blood_results_chem.py` & `effect-edc-0.1.9/effect_subject/models/lab_results/blood_results_chem.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/lab_results/blood_results_fbc.py` & `effect-edc-0.1.9/effect_subject/models/lab_results/blood_results_fbc.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/lab_results/urinalysis.py` & `effect-edc-0.1.9/effect_subject/models/lab_results/urinalysis.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/lp_csf.py` & `effect-edc-0.1.9/effect_subject/models/lp_csf.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/medical_history.py` & `effect-edc-0.1.9/effect_subject/models/medical_history.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/mental_status.py` & `effect-edc-0.1.9/effect_subject/models/mental_status.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/patient_history.py` & `effect-edc-0.1.9/effect_subject/models/patient_history.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/patient_treatment.py` & `effect-edc-0.1.9/effect_subject/models/patient_treatment.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/proxy_models.py` & `effect-edc-0.1.9/effect_subject/models/proxy_models.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/signs_and_symptoms.py` & `effect-edc-0.1.9/effect_subject/models/signs_and_symptoms.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/study_medication/study_medication.py` & `effect-edc-0.1.9/effect_subject/models/study_medication/study_medication.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/subject_visit.py` & `effect-edc-0.1.9/effect_subject/models/subject_visit.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/subject_visit_missed.py` & `effect-edc-0.1.9/effect_subject/models/subject_visit_missed.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/tb_diagnostics.py` & `effect-edc-0.1.9/effect_subject/models/tb_diagnostics.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/models/vital_signs.py` & `effect-edc-0.1.9/effect_subject/models/vital_signs.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/holidays.csv` & `effect-edc-0.1.9/effect_subject/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/mixins.py` & `effect-edc-0.1.9/effect_subject/tests/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_baseline_actions.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_baseline_actions.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_clinical_note.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_clinical_note.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_diagnoses.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_diagnoses.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_mental_status.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_mental_status.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_metadata_rules.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_metadata_rules.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_patient_treatment.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_patient_treatment.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_signs_and_symptoms.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_signs_and_symptoms.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_subject_visit.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_subject_visit.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/tests/test_vital_signs.py` & `effect-edc-0.1.9/effect_subject/tests/tests/test_vital_signs.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_subject/tests/urls.py` & `effect-edc-0.1.9/effect_subject/tests/urls.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_visit_schedule/tests/tests/test_schedule.py` & `effect-edc-0.1.9/effect_visit_schedule/tests/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_visit_schedule/visit_schedules/crfs.py` & `effect-edc-0.1.9/effect_visit_schedule/visit_schedules/crfs.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_visit_schedule/visit_schedules/requisitions.py` & `effect-edc-0.1.9/effect_visit_schedule/visit_schedules/requisitions.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/effect_visit_schedule/visit_schedules/schedule.py` & `effect-edc-0.1.9/effect_visit_schedule/visit_schedules/schedule.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/holidays.csv` & `effect-edc-0.1.9/holidays.csv`

 * *Files 20% similar despite different names*

```diff
@@ -37,7 +37,22 @@
 2017-01-02,Public Holiday,zimbabwe
 2017-04-14,Good Friday,zimbabwe
 2017-04-17,Easter Monday,zimbabwe
 2017-05-25,Ascension Day,zimbabwe
 2017-12-25,Christmas Day,zimbabwe
 2017-12-26,Boxing Day,zimbabwe
 2017-01-01,New Year,zimbabwe
+2019-01-01,New Year's Day,tanzania
+2019-01-12,Zanzibar Revolution Day,tanzania
+2019-04-07,The Sheikh Abeid Amani Karume Day,tanzania
+2019-04-17,Easter Monday,tanzania
+2019-04-26,Union Day,tanzania
+2019-05-01,Labour Day,tanzania
+2019-06-26,Eid al-Fitr,tanzania
+2019-07-07,Saba Saba Day,tanzania
+2019-07-14,Good Friday,tanzania
+2019-08-08,Nane Nane Day,tanzania
+2019-10-14,Nyerere Day,tanzania
+2019-12-01,Mawlid Day,tanzania
+2019-12-09,Independence Day,tanzania
+2019-12-25,Christmas Day,tanzania
+2019-12-26,Boxing Day,tanzania
```

### Comparing `effect-edc-0.1.8/manage.py` & `effect-edc-0.1.9/manage.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/pyproject.toml` & `effect-edc-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/runtests.py` & `effect-edc-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `effect-edc-0.1.8/setup.cfg` & `effect-edc-0.1.9/setup.cfg`

 * *Files identical despite different names*

