# Comparing `tmp/edc-he-0.1.8.tar.gz` & `tmp/edc-he-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-he-0.1.8.tar", last modified: Wed Jul  5 00:30:52 2023, max compression
+gzip compressed data, was "edc-he-0.1.9.tar", last modified: Tue Jul 18 11:31:29 2023, max compression
```

## Comparing `edc-he-0.1.8.tar` & `edc-he-0.1.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.659640 edc-he-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2021-08-23 17:45:53.000000 edc-he-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-23 17:45:53.000000 edc-he-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.648266 edc-he-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.651939 edc-he-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:28.000000 edc-he-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-25 13:21:02.000000 edc-he-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:28.000000 edc-he-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:46:20.000000 edc-he-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-19 17:21:37.000000 edc-he-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 13:21:02.000000 edc-he-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-07-05 00:30:52.659716 edc-he-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-08-23 17:45:53.000000 edc-he-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:46:20.000000 edc-he-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.654203 edc-he-0.1.8/edc_he/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      691 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      109 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      452 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8724 2023-07-05 00:30:45.000000 edc-he-0.1.8/edc_he/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      287 2023-07-05 00:30:45.000000 edc-he-0.1.8/edc_he/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      725 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2272 2022-05-25 13:21:02.000000 edc-he-0.1.8/edc_he/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1474 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.655184 edc-he-0.1.8/edc_he/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    10762 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12993 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.656318 edc-he-0.1.8/edc_he/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      467 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5792 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/assets_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2176 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/education_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.656701 edc-he-0.1.8/edc_he/model_mixins/factory/
--rw-r--r--   0 erikvw     (501) staff       (20)      134 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/factory/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1387 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/factory/assets_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2624 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/factory/income_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3298 2023-05-24 22:27:22.000000 edc-he-0.1.8/edc_he/model_mixins/household_head_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      640 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/household_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2688 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/income_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2313 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/patient_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1812 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/property_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.657524 edc-he-0.1.8/edc_he/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      405 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4081 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/assets_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3562 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4418 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/income_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1621 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/patient_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1760 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/property_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1022 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.657989 edc-he-0.1.8/edc_he/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.659171 edc-he-0.1.8/edc_he/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      677 2022-10-05 19:09:01.000000 edc-he-0.1.8/edc_he/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      227 2022-09-25 18:36:50.000000 edc-he-0.1.8/edc_he/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.659427 edc-he-0.1.8/edc_he/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4059 2023-05-24 16:43:28.000000 edc-he-0.1.8/edc_he/tests/tests/test_he.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.654787 edc-he-0.1.8/edc_he.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2015 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-19 17:35:04.000000 edc-he-0.1.8/edc_he.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 16:43:28.000000 edc-he-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2329 2022-05-25 13:21:02.000000 edc-he-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1134 2023-07-05 00:30:52.660026 edc-he-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.271411 edc-he-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2021-08-23 17:45:53.000000 edc-he-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-23 17:45:53.000000 edc-he-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.256167 edc-he-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.260796 edc-he-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:28.000000 edc-he-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-25 13:21:02.000000 edc-he-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:28.000000 edc-he-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:46:20.000000 edc-he-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-19 17:21:37.000000 edc-he-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 13:21:02.000000 edc-he-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-07-18 11:31:29.271546 edc-he-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-08-23 17:45:53.000000 edc-he-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:46:20.000000 edc-he-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.263920 edc-he-0.1.9/edc_he/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      691 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      109 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8725 2023-07-18 11:31:21.000000 edc-he-0.1.9/edc_he/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2023-07-05 00:30:45.000000 edc-he-0.1.9/edc_he/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      725 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2272 2022-05-25 13:21:02.000000 edc-he-0.1.9/edc_he/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1474 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.265993 edc-he-0.1.9/edc_he/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    10762 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12993 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.267476 edc-he-0.1.9/edc_he/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      467 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5792 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/assets_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2176 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/education_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.268054 edc-he-0.1.9/edc_he/model_mixins/factory/
+-rw-r--r--   0 erikvw     (501) staff       (20)      134 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/factory/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1387 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/factory/assets_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2624 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/factory/income_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3477 2023-07-18 11:31:21.000000 edc-he-0.1.9/edc_he/model_mixins/household_head_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      698 2023-07-18 11:31:21.000000 edc-he-0.1.9/edc_he/model_mixins/household_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2678 2023-07-18 11:31:21.000000 edc-he-0.1.9/edc_he/model_mixins/income_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2313 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/patient_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1812 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/model_mixins/property_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.269037 edc-he-0.1.9/edc_he/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      405 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4081 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/modeladmin_mixins/assets_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3537 2023-07-18 11:31:21.000000 edc-he-0.1.9/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4373 2023-07-18 11:31:21.000000 edc-he-0.1.9/edc_he/modeladmin_mixins/income_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1621 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/modeladmin_mixins/patient_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1760 2023-05-24 17:41:22.000000 edc-he-0.1.9/edc_he/modeladmin_mixins/property_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1022 2023-07-18 11:31:01.000000 edc-he-0.1.9/edc_he/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.269535 edc-he-0.1.9/edc_he/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.270891 edc-he-0.1.9/edc_he/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      677 2022-10-05 19:09:01.000000 edc-he-0.1.9/edc_he/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      227 2022-09-25 18:36:50.000000 edc-he-0.1.9/edc_he/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.271159 edc-he-0.1.9/edc_he/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4059 2023-05-24 16:43:28.000000 edc-he-0.1.9/edc_he/tests/tests/test_he.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-08-23 17:45:53.000000 edc-he-0.1.9/edc_he/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 11:31:29.265218 edc-he-0.1.9/edc_he.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-07-18 11:31:29.000000 edc-he-0.1.9/edc_he.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2015 2023-07-18 11:31:29.000000 edc-he-0.1.9/edc_he.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-18 11:31:29.000000 edc-he-0.1.9/edc_he.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-19 17:35:04.000000 edc-he-0.1.9/edc_he.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-07-18 11:31:29.000000 edc-he-0.1.9/edc_he.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 16:43:28.000000 edc-he-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2329 2022-05-25 13:21:02.000000 edc-he-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1134 2023-07-18 11:31:29.271900 edc-he-0.1.9/setup.cfg
```

### Comparing `edc-he-0.1.8/.github/workflows/build.yml` & `edc-he-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/.gitignore` & `edc-he-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/.pre-commit-config.yaml` & `edc-he-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/LICENSE` & `edc-he-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/PKG-INFO` & `edc-he-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-he
-Version: 0.1.8
+Version: 0.1.9
 Summary: Base django classes for health economics
 Home-page: https://github.com/clinicedc/edc-he
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc health economics,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-he-0.1.8/README.rst` & `edc-he-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/admin.py` & `edc-he-0.1.9/edc_he/admin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/choices.py` & `edc-he-0.1.9/edc_he/choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     ("8", "Craft and related workers"),
     ("9", "Plant and machine operators and assemblers"),
     ("10", "Elementary occupations"),
     (DONT_KNOW, "Don’t know"),
     (NOT_APPLICABLE, "Not applicable"),
 )
 
+
 MARITAL_CHOICES = (
     ("1", "Never Married (but not co-habiting)"),
     ("2", "Co-habiting"),
     ("3", "Currently Married"),
     ("4", "Separated/Divorced"),
     ("5", "Widowed"),
     (OTHER, "Other, specify ..."),
```

### Comparing `edc-he-0.1.8/edc_he/fieldsets.py` & `edc-he-0.1.9/edc_he/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/form_validators.py` & `edc-he-0.1.9/edc_he/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/list_data.py` & `edc-he-0.1.9/edc_he/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/migrations/0001_initial.py` & `edc-he-0.1.9/edc_he/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py` & `edc-he-0.1.9/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/model_mixins/assets_model_mixin.py` & `edc-he-0.1.9/edc_he/model_mixins/assets_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/model_mixins/education_model_mixin.py` & `edc-he-0.1.9/edc_he/model_mixins/education_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/model_mixins/factory/assets_model_mixin_factory.py` & `edc-he-0.1.9/edc_he/model_mixins/factory/assets_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/model_mixins/factory/income_model_mixin_factory.py` & `edc-he-0.1.9/edc_he/model_mixins/factory/income_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/model_mixins/household_head_model_mixin.py` & `edc-he-0.1.9/edc_he/model_mixins/household_head_model_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from edc_constants.choices import GENDER, YES_NO
+from edc_constants.constants import NOT_APPLICABLE
 from edc_model_fields.fields import OtherCharField
 
 from ..choices import (
     EDUCATION_CHOICES,
     EMPLOYMENT_CHOICES,
     EMPLOYMENT_STATUS_CHOICES,
     ETHNICITY_CHOICES,
@@ -23,14 +24,16 @@
         choices=YES_NO,
     )
 
     relationship_to_hoh = models.CharField(
         verbose_name="What is your relationship to the household head?",
         max_length=25,
         choices=RELATIONSHIP_CHOICES,
+        default=NOT_APPLICABLE,
+        help_text="Not applicable if patient is head of household",
     )
 
     relationship_to_hoh_other = OtherCharField(
         verbose_name="If OTHER relationship, specify ...",
     )
 
     hoh_gender = models.CharField(
@@ -41,20 +44,14 @@
 
     hoh_age = models.IntegerField(
         verbose_name="How old is the household head?",
         validators=[MinValueValidator(18), MaxValueValidator(110)],
         help_text="In years",
     )
 
-    hoh_citizen = models.CharField(
-        verbose_name="Is the household head a citizen of this country?",
-        max_length=15,
-        choices=YES_NO,
-    )
-
     hoh_religion = models.CharField(
         verbose_name="How would you describe the household head’s religious orientation?",
         max_length=25,
         choices=RELIGION_CHOICES,
     )
 
     hoh_religion_other = OtherCharField(
@@ -89,14 +86,20 @@
 
     hoh_employment_type = models.CharField(
         verbose_name="Household head’s type of employment",
         max_length=25,
         choices=EMPLOYMENT_CHOICES,
     )
 
+    hoh_employment_type_other = OtherCharField(
+        verbose_name="Household head’s type of employment",
+        max_length=100,
+        help_text="... other type of employment",
+    )
+
     hoh_marital_status = models.CharField(
         verbose_name="Household head’s marital status",
         max_length=25,
         choices=MARITAL_CHOICES,
     )
 
     hoh_marital_status_other = OtherCharField(
```

### Comparing `edc-he-0.1.8/edc_he/model_mixins/household_model_mixin.py` & `edc-he-0.1.9/edc_he/model_mixins/household_model_mixin.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from django.db import models
 
 
 class HouseholdModelMixin(models.Model):
     hh_count = models.IntegerField(
         verbose_name="What is the total number of people who live in your household?",
         validators=[MinValueValidator(1), MaxValueValidator(25)],
+        help_text="Persons",
     )
 
     hh_minors_count = models.IntegerField(
         verbose_name=(
             "What is the total number of people 14 years or under "
             "who live in your household?"
         ),
         validators=[MinValueValidator(0), MaxValueValidator(25)],
+        help_text="Persons",
     )
 
     class Meta:
         abstract = True
```

### Comparing `edc-he-0.1.8/edc_he/model_mixins/income_model_mixin.py` & `edc-he-0.1.9/edc_he/model_mixins/income_model_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from edc_constants.choices import YES_NO_DONT_KNOW, YES_NO_DONT_KNOW_DWTA
 
 from ..choices import FINANCIAL_STATUS, REMITTANCE_CURRENCY_CHOICES, STATUS
 from .factory import income_model_mixin_factory
 
 
 class IncomeModelMixin(income_model_mixin_factory(), models.Model):
-    external_remittance_currency = models.CharField(
+    external_remit_currency = models.CharField(
         verbose_name="In what currency do you receive remittances?",
         max_length=50,
         choices=REMITTANCE_CURRENCY_CHOICES,
         null=True,
         blank=True,
     )
 
-    external_remittance_currency_other = models.CharField(
+    external_remit_currency_other = models.CharField(
         verbose_name="If OTHER currency, specify ...",
         max_length=50,
         null=True,
         blank=True,
     )
 
     more_sources_other = models.CharField(
```

### Comparing `edc-he-0.1.8/edc_he/model_mixins/patient_model_mixin.py` & `edc-he-0.1.9/edc_he/model_mixins/patient_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/model_mixins/property_model_mixin.py` & `edc-he-0.1.9/edc_he/model_mixins/property_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/modeladmin_mixins/assets_model_admin_mixin.py` & `edc-he-0.1.9/edc_he/modeladmin_mixins/assets_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py` & `edc-he-0.1.9/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,74 +12,73 @@
         "<p>We want to learn about the household and we use these questions "
         "to get an understanding of wealth and opportunities in the community.</p>"
     )
 
     fieldsets = (
         (None, {"fields": ("subject_visit", "report_datetime")}),
         (
+            "Household",
+            {
+                "description": format_html(
+                    "<H5><B><font color='orange'>Interviewer to read</font></B></H5>"
+                    "<p><B>HOUSEHOLD</B>: A person or persons (people/ members) who share "
+                    "the same kitchen (pot), live together, and run the household "
+                    "expenditure from the same income is known as a household.</P>"
+                    "<P><B>HOUSEHOLD MEMBER</B>: A household member should be identified on "
+                    "the basis that they shared a place of living together most of time for "
+                    "the past one year.</P><P><B>Note:</B> When it is difficult to demarcate "
+                    "'most of the time', living together for the past six months or more "
+                    "should be used to find out whether or not the person is a "
+                    "household member.</p>"
+                ),
+                "fields": (
+                    "hh_count",
+                    "hh_minors_count",
+                ),
+            },
+        ),
+        (
             "Household head",
             {
                 "description": format_html(
                     "<H5><B><font color='orange'>Interviewer to read</font></B></H5>"
                     "<p>By <B>HEAD OF THE HOUSEHOLD</B> we mean the main decision maker "
                     "in the HOUSEHOLD. The HEAD can be either male or female. If two "
                     "people are equal decision-makers, take the older person</p>"
                 ),
                 "fields": (
                     "hoh",
                     "relationship_to_hoh",
                     "relationship_to_hoh_other",
                     "hoh_gender",
                     "hoh_age",
-                    "hoh_citizen",
                     "hoh_religion",
                     "hoh_religion_other",
                     "hoh_ethnicity",
                     "hoh_ethnicity_other",
                     "hoh_education",
                     "hoh_education_other",
                     "hoh_employment",
                     "hoh_employment_type",
+                    "hoh_employment_type_other",
                     "hoh_marital_status",
                     "hoh_marital_status_other",
                     "hoh_insurance",
                     "hoh_insurance_other",
                 ),
             },
         ),
-        (
-            "Household",
-            {
-                "description": format_html(
-                    "<H5><B><font color='orange'>Interviewer to read</font></B></H5>"
-                    "<p><B>HOUSEHOLD</B>: A person or persons (people/ members) who share "
-                    "the same kitchen (pot), live together, and run the household "
-                    "expenditure from the same income is known as a household.</P>"
-                    "<P><B>HOUSEHOLD MEMBER</B>: A household member should be identified on "
-                    "the basis that they shared a place of living together most of time for "
-                    "the past one year.</P><P><B>Note:</B> When it is difficult to demarcate "
-                    "'most of the time', living together for the past six months or more "
-                    "should be used to find out whether or not the person is a "
-                    "household member.</p>"
-                ),
-                "fields": (
-                    "hh_count",
-                    "hh_minors_count",
-                ),
-            },
-        ),
         crf_status_fieldset_tuple,
         audit_fieldset_tuple,
     )
 
     radio_fields = {
         "hoh": admin.VERTICAL,
         "relationship_to_hoh": admin.VERTICAL,
         "hoh_gender": admin.VERTICAL,
-        "hoh_citizen": admin.VERTICAL,
         "hoh_religion": admin.VERTICAL,
         "hoh_ethnicity": admin.VERTICAL,
         "hoh_education": admin.VERTICAL,
         "hoh_employment": admin.VERTICAL,
         "hoh_employment_type": admin.VERTICAL,
         "hoh_marital_status": admin.VERTICAL,
         "crf_status": admin.VERTICAL,
```

### Comparing `edc-he-0.1.8/edc_he/modeladmin_mixins/income_model_admin_mixin.py` & `edc-he-0.1.9/edc_he/modeladmin_mixins/income_model_admin_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     for fld, label in sources:
         fields = [
             fld,
             f"{fld}_value_known",
             f"{fld}_value",
         ]
         if fld == "external_remittance":
-            fields.extend(
-                ["external_remittance_currency", "external_remittance_currency_other"]
-            )
+            fields.extend(["external_remit_currency", "external_remit_currency_other"])
         if fld == "more_sources":
             fields.insert(1, "more_sources_other")
 
         fieldsets.append(
             (
                 label,
                 {
@@ -96,15 +94,15 @@
         "ngo_assistance_value_known": admin.VERTICAL,
         "interest": admin.VERTICAL,
         "interest_value_known": admin.VERTICAL,
         "internal_remittance": admin.VERTICAL,
         "internal_remittance_value_known": admin.VERTICAL,
         "external_remittance": admin.VERTICAL,
         "external_remittance_value_known": admin.VERTICAL,
-        "external_remittance_currency": admin.VERTICAL,
+        "external_remit_currency": admin.VERTICAL,
         "more_sources": admin.VERTICAL,
         "more_sources_value_known": admin.VERTICAL,
         "income_enough": admin.VERTICAL,
         "financial_status": admin.VERTICAL,
         "financial_status_compare": admin.VERTICAL,
         "household_debt": admin.VERTICAL,
         "crf_status": admin.VERTICAL,
```

### Comparing `edc-he-0.1.8/edc_he/modeladmin_mixins/patient_model_admin_mixin.py` & `edc-he-0.1.9/edc_he/modeladmin_mixins/patient_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/modeladmin_mixins/property_model_admin_mixin.py` & `edc-he-0.1.9/edc_he/modeladmin_mixins/property_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/models.py` & `edc-he-0.1.9/edc_he/models.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/tests/etc/user-rsa-local-private.pem` & `edc-he-0.1.9/edc_he/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/tests/etc/user-rsa-restricted-private.pem` & `edc-he-0.1.9/edc_he/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/tests/forms.py` & `edc-he-0.1.9/edc_he/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he/tests/tests/test_he.py` & `edc-he-0.1.9/edc_he/tests/tests/test_he.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/edc_he.egg-info/PKG-INFO` & `edc-he-0.1.9/edc_he.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-he
-Version: 0.1.8
+Version: 0.1.9
 Summary: Base django classes for health economics
 Home-page: https://github.com/clinicedc/edc-he
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc health economics,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-he-0.1.8/edc_he.egg-info/SOURCES.txt` & `edc-he-0.1.9/edc_he.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/pyproject.toml` & `edc-he-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/runtests.py` & `edc-he-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.8/setup.cfg` & `edc-he-0.1.9/setup.cfg`

 * *Files identical despite different names*

