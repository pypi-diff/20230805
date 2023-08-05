# Comparing `tmp/django_eveuniverse-1.3.0.tar.gz` & `tmp/django_eveuniverse-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_eveuniverse-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_eveuniverse-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_eveuniverse-1.3.0.tar` & `django_eveuniverse-1.3.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1070 2023-07-02 13:03:38.571581 django_eveuniverse-1.3.0/LICENSE
--rw-r--r--   0        0        0     3082 2023-07-02 13:03:38.571581 django_eveuniverse-1.3.0/README.rst
--rw-r--r--   0        0        0      184 2023-07-11 20:13:24.749730 django_eveuniverse-1.3.0/eveuniverse/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/admin.py
--rw-r--r--   0        0        0     2857 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/app_settings.py
--rw-r--r--   0        0        0      254 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/apps.py
--rw-r--r--   0        0        0      873 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/backends.py
--rw-r--r--   0        0        0      423 2023-07-11 20:13:24.749730 django_eveuniverse-1.3.0/eveuniverse/constants.py
--rw-r--r--   0        0        0        0 2023-07-11 20:24:19.171556 django_eveuniverse-1.3.0/eveuniverse/core/__init__.py
--rw-r--r--   0        0        0     1781 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/dotlan.py
--rw-r--r--   0        0        0      423 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/esitools.py
--rw-r--r--   0        0        0     5127 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/eveimageserver.py
--rw-r--r--   0        0        0      358 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/eveitems.py
--rw-r--r--   0        0        0     2598 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/evemicros.py
--rw-r--r--   0        0        0     2431 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/evesdeapi.py
--rw-r--r--   0        0        0      457 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/eveskinserver.py
--rw-r--r--   0        0        0     1145 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/evewho.py
--rw-r--r--   0        0        0     2864 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/core/evexml.py
--rw-r--r--   0        0        0     1713 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/core/zkillboard.py
--rw-r--r--   0        0        0     1745 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/helpers.py
--rw-r--r--   0        0        0      365 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/__init__.py
--rw-r--r--   0        0        0     4574 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_data.py
--rw-r--r--   0        0        0     5348 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_types.py
--rw-r--r--   0        0        0     1644 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_purge_data.py
--rw-r--r--   0        0        0    47900 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/managers.py
--rw-r--r--   0        0        0    51659 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0001_initial.py
--rw-r--r--   0        0        0      968 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0002_load_eveunit.py
--rw-r--r--   0        0        0     1009 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0003_evemarketprice.py
--rw-r--r--   0        0        0      478 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0004_effect_longer_name.py
--rw-r--r--   0        0        0     2702 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0005_type_materials_and_sections.py
--rw-r--r--   0        0        0      429 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
--rw-r--r--   0        0        0      409 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0007_evetype_description.py
--rw-r--r--   0        0        0     7547 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py
--rw-r--r--   0        0        0      989 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0009_load_industry_activities.py
--rw-r--r--   0        0        0     1768 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py
--rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/migrations/__init__.py
--rw-r--r--   0        0        0     5336 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/eve_unit.json
--rw-r--r--   0        0        0      934 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/industry_activities.json
--rw-r--r--   0        0        0    65441 2023-07-11 20:13:24.749730 django_eveuniverse-1.3.0/eveuniverse/models.py
--rw-r--r--   0        0        0      250 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/providers.py
--rw-r--r--   0        0        0    14542 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_128.png
--rw-r--r--   0        0        0     2142 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_32.png
--rw-r--r--   0        0        0     4141 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_64.png
--rw-r--r--   0        0        0   887006 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/swagger.json
--rw-r--r--   0        0        0    10805 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/tasks.py
--rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tests/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/pilot.py
--rw-r--r--   0        0        0     1046 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_backends.py
--rw-r--r--   0        0        0    10307 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_commands.py
--rw-r--r--   0        0        0    22736 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_core.py
--rw-r--r--   0        0        0     2136 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_helpers.py
--rw-r--r--   0        0        0    52520 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_1.py
--rw-r--r--   0        0        0    28662 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_2.py
--rw-r--r--   0        0        0    56264 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_3.py
--rw-r--r--   0        0        0    30870 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_4.py
--rw-r--r--   0        0        0     6759 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_tasks.py
--rw-r--r--   0        0        0     3009 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_tools_testdata.py
--rw-r--r--   0        0        0     4006 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_utils.py
--rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/__init__.py
--rw-r--r--   0        0        0     7725 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi.py
--rw-r--r--   0        0        0    83831 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi_data.json
--rw-r--r--   0        0        0     4500 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/factories.py
--rw-r--r--   0        0        0     1659 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py
--rw-r--r--   0        0        0     1183 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/generate_sde.py
--rw-r--r--   0        0        0      610 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde.py
--rw-r--r--   0        0        0     5187 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde_data.json
--rw-r--r--   0        0        0     4636 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata_example.json
--rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tests/tools/__init__.py
--rw-r--r--   0        0        0      760 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tools/__init__.py
--rw-r--r--   0        0        0     1373 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tools/drop_tables.sql
--rw-r--r--   0        0        0     5235 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tools/testdata.py
--rw-r--r--   0        0        0     2821 2023-07-08 11:35:53.902984 django_eveuniverse-1.3.0/eveuniverse/utils.py
--rw-r--r--   0        0        0     1733 2023-07-02 13:03:38.599582 django_eveuniverse-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4432 1970-01-01 00:00:00.000000 django_eveuniverse-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-26 11:55:54.137706 django_eveuniverse-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3082 2023-07-26 11:55:54.141705 django_eveuniverse-1.3.1/README.rst
+-rw-r--r--   0        0        0      217 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/admin.py
+-rw-r--r--   0        0        0     2857 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/app_settings.py
+-rw-r--r--   0        0        0      254 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/apps.py
+-rw-r--r--   0        0        0      873 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/backends.py
+-rw-r--r--   0        0        0      423 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/constants.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:47:58.287651 django_eveuniverse-1.3.1/eveuniverse/core/__init__.py
+-rw-r--r--   0        0        0     1781 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/core/dotlan.py
+-rw-r--r--   0        0        0      433 2023-08-05 14:26:23.931796 django_eveuniverse-1.3.1/eveuniverse/core/esitools.py
+-rw-r--r--   0        0        0     5015 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/core/eveimageserver.py
+-rw-r--r--   0        0        0      358 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/core/eveitems.py
+-rw-r--r--   0        0        0     2619 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/core/evemicros.py
+-rw-r--r--   0        0        0     2452 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/core/evesdeapi.py
+-rw-r--r--   0        0        0      457 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/core/eveskinserver.py
+-rw-r--r--   0        0        0     1145 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/core/evewho.py
+-rw-r--r--   0        0        0     2885 2023-08-05 14:26:23.931796 django_eveuniverse-1.3.1/eveuniverse/core/evexml.py
+-rw-r--r--   0        0        0     1713 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/core/zkillboard.py
+-rw-r--r--   0        0        0     1745 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/helpers.py
+-rw-r--r--   0        0        0      365 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/management/commands/__init__.py
+-rw-r--r--   0        0        0     4574 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/management/commands/eveuniverse_load_data.py
+-rw-r--r--   0        0        0     5348 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/management/commands/eveuniverse_load_types.py
+-rw-r--r--   0        0        0     1671 2023-08-05 14:26:23.931796 django_eveuniverse-1.3.1/eveuniverse/management/commands/eveuniverse_purge_data.py
+-rw-r--r--   0        0        0    48278 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/managers.py
+-rw-r--r--   0        0        0    51659 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0002_load_eveunit.py
+-rw-r--r--   0        0        0     1009 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0003_evemarketprice.py
+-rw-r--r--   0        0        0      478 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0004_effect_longer_name.py
+-rw-r--r--   0        0        0     2702 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0005_type_materials_and_sections.py
+-rw-r--r--   0        0        0      429 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
+-rw-r--r--   0        0        0      409 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0007_evetype_description.py
+-rw-r--r--   0        0        0     7547 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py
+-rw-r--r--   0        0        0      989 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0009_load_industry_activities.py
+-rw-r--r--   0        0        0     1768 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:47:58.287651 django_eveuniverse-1.3.1/eveuniverse/migrations/__init__.py
+-rw-r--r--   0        0        0     5336 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/eve_unit.json
+-rw-r--r--   0        0        0      934 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/migrations/industry_activities.json
+-rw-r--r--   0        0        0    65414 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/models.py
+-rw-r--r--   0        0        0      250 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/providers.py
+-rw-r--r--   0        0        0    14542 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/static/eveuniverse/skin_generic_128.png
+-rw-r--r--   0        0        0     2142 2023-07-26 11:55:54.149705 django_eveuniverse-1.3.1/eveuniverse/static/eveuniverse/skin_generic_32.png
+-rw-r--r--   0        0        0     4141 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/static/eveuniverse/skin_generic_64.png
+-rw-r--r--   0        0        0   887006 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/swagger.json
+-rw-r--r--   0        0        0    10835 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/tasks.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:47:58.287651 django_eveuniverse-1.3.1/eveuniverse/tests/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/pilot.py
+-rw-r--r--   0        0        0     1046 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_backends.py
+-rw-r--r--   0        0        0    10307 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_commands.py
+-rw-r--r--   0        0        0    22736 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_core.py
+-rw-r--r--   0        0        0     2136 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_helpers.py
+-rw-r--r--   0        0        0    52520 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_models_1.py
+-rw-r--r--   0        0        0    28662 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_models_2.py
+-rw-r--r--   0        0        0    56264 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_models_3.py
+-rw-r--r--   0        0        0    33770 2023-08-05 15:36:37.034141 django_eveuniverse-1.3.1/eveuniverse/tests/test_models_4.py
+-rw-r--r--   0        0        0     6759 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_tasks.py
+-rw-r--r--   0        0        0     3009 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_tools_testdata.py
+-rw-r--r--   0        0        0     4006 2023-07-26 11:55:54.153705 django_eveuniverse-1.3.1/eveuniverse/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:47:58.287651 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     7683 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/esi.py
+-rw-r--r--   0        0        0    83831 2023-07-26 11:55:54.157704 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0     4509 2023-08-05 14:26:23.931796 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/factories.py
+-rw-r--r--   0        0        0     1647 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/fetch_esi_raw_data.py
+-rw-r--r--   0        0        0     1183 2023-07-26 11:55:54.157704 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/generate_sde.py
+-rw-r--r--   0        0        0      602 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/sde.py
+-rw-r--r--   0        0        0     5187 2023-07-26 11:55:54.157704 django_eveuniverse-1.3.1/eveuniverse/tests/testdata/sde_data.json
+-rw-r--r--   0        0        0     4636 2023-07-26 11:55:54.157704 django_eveuniverse-1.3.1/eveuniverse/tests/testdata_example.json
+-rw-r--r--   0        0        0        0 2023-08-05 15:47:58.287651 django_eveuniverse-1.3.1/eveuniverse/tests/tools/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-26 11:55:54.157704 django_eveuniverse-1.3.1/eveuniverse/tests/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:47:58.287651 django_eveuniverse-1.3.1/eveuniverse/tools/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-26 11:55:54.157704 django_eveuniverse-1.3.1/eveuniverse/tools/drop_tables.sql
+-rw-r--r--   0        0        0     5308 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/tools/testdata.py
+-rw-r--r--   0        0        0     2823 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/eveuniverse/utils.py
+-rw-r--r--   0        0        0     1988 2023-08-05 15:19:18.890804 django_eveuniverse-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 django_eveuniverse-1.3.1/PKG-INFO
```

### Comparing `django_eveuniverse-1.3.0/LICENSE` & `django_eveuniverse-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/README.rst` & `django_eveuniverse-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/admin.py` & `django_eveuniverse-1.3.1/eveuniverse/admin.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/app_settings.py` & `django_eveuniverse-1.3.1/eveuniverse/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/backends.py` & `django_eveuniverse-1.3.1/eveuniverse/backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/core/dotlan.py` & `django_eveuniverse-1.3.1/eveuniverse/core/dotlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,16 @@
         _Category.SOLARSYSTEM: "system",
         _Category.STATION: "station",
     }
     try:
         partial = partials[category]
     except KeyError:
         raise ValueError(f"Invalid category: {category}") from None
-    return urljoin(
-        _BASE_URL, "{}/{}".format(partial, quote(str(name).replace(" ", "_")))
-    )
+    url_part = quote(str(name).replace(" ", "_"))
+    return urljoin(_BASE_URL, f"{partial}/{url_part}")
 
 
 def alliance_url(name: str) -> str:
     """URL for page about given alliance on dotlan."""
     return _build_url(_Category.ALLIANCE, name)
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/core/eveimageserver.py` & `django_eveuniverse-1.3.1/eveuniverse/core/eveimageserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,44 +83,42 @@
                 ImageVariant.RENDER,
                 ImageVariant.BPO,
                 ImageVariant.BPC,
             ],
         },
     }
     if not entity_id:
-        raise ValueError("Invalid entity_id: {}".format(entity_id))
-    else:
-        entity_id = int(entity_id)
+        raise ValueError(f"Invalid entity_id: {entity_id}")
+
+    entity_id = int(entity_id)
 
     if not size or size < 32 or size > 1024 or (size & (size - 1) != 0):
-        raise ValueError("Invalid size: {}".format(size))
+        raise ValueError(f"Invalid size: {size}")
 
-    if type(category) is not EsiCategory:
-        raise ValueError("Invalid category {}".format(category))
-    else:
-        endpoint = categories[category]["endpoint"]
+    if not isinstance(category, EsiCategory):
+        raise ValueError(f"Invalid category {category}")
+
+    endpoint = categories[category]["endpoint"]
 
     if variant:
         if variant not in categories[category]["variants"]:
-            raise ValueError(
-                "Invalid variant {} for category {}".format(variant, category)
-            )
+            raise ValueError(f"Invalid variant {variant} for category {category}")
         my_variant = variant
     else:
         my_variant = categories[category]["variants"][0]
 
-    if tenant and type(tenant) is not EsiTenant:
-        raise ValueError("Invalid tenant {}".format(tenant))
+    if tenant and not isinstance(tenant, EsiTenant):
+        raise ValueError(f"Invalid tenant {tenant}")
 
     # compose result URL
-    result = "{}/{}/{}/{}?size={}".format(
-        _EVE_IMAGE_SERVER_URL, endpoint, entity_id, my_variant.value, size
+    result = (
+        f"{_EVE_IMAGE_SERVER_URL}/{endpoint}/{entity_id}/{my_variant.value}?size={size}"
     )
     if tenant:
-        result += "&tenant={}".format(tenant.value)
+        result += f"&tenant={tenant.value}"
 
     return result
 
 
 def alliance_logo_url(alliance_id: int, size: int = _DEFAULT_IMAGE_SIZE) -> str:
     """image URL for the given alliance ID"""
     return _eve_entity_image_url(EsiCategory.ALLIANCE, alliance_id, size)
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/core/evemicros.py` & `django_eveuniverse-1.3.1/eveuniverse/core/evemicros.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
     Returns None if data from API does not have expected structure.
     """
     params = map(str, map(int, [solar_system_id, x, y, z]))
     query = urlencode({"nearestCelestials": ",".join(params)})
     cache_key = f"EVEUNIVERSE_NEAREST_CELESTIAL_{query}"
     result = cache.get(key=cache_key)
     if not result:
-        r = requests.get(
+        response = requests.get(
             f"{_BASE_URL}?{query}", timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT
         )
-        r.raise_for_status()
-        data = r.json()
+        response.raise_for_status()
+        data = response.json()
         if "ok" not in data or not data["ok"] or "result" not in data:
             return None
         result = data["result"]
         cache.set(key=cache_key, value=result, timeout=_CACHE_TIMEOUT)
     return result
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/core/evesdeapi.py` & `django_eveuniverse-1.3.1/eveuniverse/core/evesdeapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,14 @@
     if group_id is not None:
         params["group_id"] = int(group_id)
     cache_key = f"eveuniverse_nearest_celestial_{dict_hash(params)}"
     result = cache.get(key=cache_key)
     if not result:
         url = f"{_BASE_URL}/universe/systems/{solar_system_id}/nearest_celestials"
         logger.info("Sending request: %s", url)
-        r = requests.get(
+        response = requests.get(
             url, params=params, timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT
         )
-        r.raise_for_status()
-        result = r.json()
+        response.raise_for_status()
+        result = response.json()
         cache.set(key=cache_key, value=result, timeout=_CACHE_TIMEOUT)
     return result
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/core/evewho.py` & `django_eveuniverse-1.3.1/eveuniverse/core/evewho.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/core/evexml.py` & `django_eveuniverse-1.3.1/eveuniverse/core/evexml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Tools for dealing with eve data in XML."""
 import re
 import unicodedata
 
 from django.core.exceptions import ValidationError
 from django.core.validators import URLValidator
 
-from ..constants import EveCategoryId, EveGroupId
-from ..models import EveEntity, EveType
+from eveuniverse.constants import EveCategoryId, EveGroupId
+from eveuniverse.models import EveEntity, EveType
+
 from . import zkillboard
 
 
 def eve_link_to_url(link: str) -> str:
     """Convert an eve style link into a normal URL.
 
     Example: ``showinfo:5//30004984`` => ``"https://evemaps.dotlan.net/system/Abune"``
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/core/zkillboard.py` & `django_eveuniverse-1.3.1/eveuniverse/core/zkillboard.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/helpers.py` & `django_eveuniverse-1.3.1/eveuniverse/helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_data.py` & `django_eveuniverse-1.3.1/eveuniverse/management/commands/eveuniverse_load_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_types.py` & `django_eveuniverse-1.3.1/eveuniverse/management/commands/eveuniverse_load_types.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_purge_data.py` & `django_eveuniverse-1.3.1/eveuniverse/management/commands/eveuniverse_purge_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 
 from django.core.management.base import BaseCommand
 from django.db import transaction
 
-from ... import __title__
-from ...models import EveUniverseBaseModel
-from ...utils import LoggerAddTag
+from eveuniverse import __title__
+from eveuniverse.models import EveUniverseBaseModel
+from eveuniverse.utils import LoggerAddTag
+
 from . import get_input
 
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
 
 
 class Command(BaseCommand):
     help = (
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/managers.py` & `django_eveuniverse-1.3.1/eveuniverse/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Managers and Querysets for Eve universe models."""
 
+# pylint: disable = import-outside-toplevel, missing-class-docstring
+
 import datetime as dt
 import logging
 from abc import ABC, abstractmethod
 from collections import defaultdict, namedtuple
-from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, TypeVar
+from typing import Any, Dict, Iterable, Optional, Set, Tuple
 from urllib.parse import urljoin
 
 import requests
 from bravado.exception import HTTPNotFound
 from django.core.cache import cache
 from django.db import models, transaction
 from django.db.utils import IntegrityError
@@ -34,15 +36,15 @@
     :meta private:
     """
 
     def _defaults_from_esi_obj(
         self, eve_data_obj: dict, enabled_sections: Optional[Set[str]] = None
     ) -> dict:
         """compiles defaults from an esi data object for update/creating the model"""
-        defaults = dict()
+        defaults = {}
         for field_name, mapping in self.model._esi_mapping(enabled_sections).items():
             if not mapping.is_pk:
                 if not isinstance(mapping.esi_name, tuple):
                     if mapping.esi_name in eve_data_obj:
                         esi_value = eve_data_obj[mapping.esi_name]
                     else:
                         esi_value = None
@@ -55,22 +57,25 @@
                             mapping.esi_name[1]
                         ]
                     else:
                         esi_value = None
 
                 if esi_value is not None:
                     if mapping.is_fk:
-                        ParentClass = mapping.related_model
+                        parent_class = mapping.related_model
                         try:
-                            value = ParentClass.objects.get(id=esi_value)
-                        except ParentClass.DoesNotExist:
+                            value = parent_class.objects.get(id=esi_value)
+                        except parent_class.DoesNotExist:
                             value = None
                             if mapping.create_related:
                                 try:
-                                    value, _ = ParentClass.objects.update_or_create_esi(
+                                    (
+                                        value,
+                                        _,
+                                    ) = parent_class.objects.update_or_create_esi(
                                         id=esi_value,
                                         include_children=False,
                                         wait_for_children=True,
                                     )
                                 except AttributeError:
                                     pass
 
@@ -81,39 +86,39 @@
                             value = esi_value
 
                     defaults[field_name] = value
 
         return defaults
 
 
-ModelType = TypeVar("ModelType", bound=models.Model)
-
-
 class EveUniverseEntityModelManager(EveUniverseBaseModelManager):
     """Manager for most Eve models."""
 
     def get_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Optional[Iterable[str]] = None,
         task_priority: Optional[int] = None,
-    ) -> Tuple[ModelType, bool]:
+    ) -> Tuple[Any, bool]:
         """gets or creates an eve universe object.
 
         The object is automatically fetched from ESI if it does not exist (blocking).
         Will always get/create parent objects.
 
         Args:
             id: Eve Online ID of object
-            include_children: if child objects should be updated/created as well (only when a new object is created)
-            wait_for_children: when true child objects will be updated/created blocking (if any), else async (only when a new object is created)
-            enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
+            include_children: if child objects should be updated/created as well
+            (only when a new object is created)
+            wait_for_children: when true child objects will be updated/created blocking
+            (if any), else async (only when a new object is created)
+            enabled_sections: Sections to load regardless of current settings,
+            e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
             task_priority: priority of started tasks
 
         Returns:
             A tuple consisting of the requested object and a created flag
         """
         id = int(id)
         effective_sections = self.model.determine_effective_sections(enabled_sections)
@@ -141,23 +146,25 @@
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Optional[Iterable[str]] = None,
         task_priority: Optional[int] = None,
-    ) -> Tuple[ModelType, bool]:
+    ) -> Tuple[Any, bool]:
         """updates or creates an Eve universe object by fetching it from ESI (blocking).
         Will always get/create parent objects
 
         Args:
             id: Eve Online ID of object
             include_children: if child objects should be updated/created as well (if any)
-            wait_for_children: when true child objects will be updated/created blocking (if any), else async
-            enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
+            wait_for_children: when true child objects will be updated/created blocking
+            (if any), else async
+            enabled_sections: Sections to load regardless of current settings,
+            e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
             task_priority: priority of started tasks
 
         Returns:
             A tuple consisting of the requested object and a created flag
         """
         id = int(id)
         effective_sections = self.model.determine_effective_sections(enabled_sections)
@@ -205,15 +212,15 @@
     ) -> dict:
         """make request to ESI and return response data.
         Can handle raw ESI response from both list and normal endpoints.
         """
         if id is not None and not self.model._is_list_only_endpoint():
             args = {self.model._esi_pk(): id}
         else:
-            args = dict()
+            args = {}
         category, method = self.model._esi_path_object()
         esi_data = getattr(
             getattr(esi.client, category),
             method,
         )(**args).results()
         return esi_data
 
@@ -249,47 +256,43 @@
         """
         from .tasks import (
             update_or_create_inline_object as task_update_or_create_inline_object,
         )
 
         if not parent_eve_data_obj or not parent_obj:
             raise ValueError(
-                "%s: Tried to create inline object from empty parent object"
-                % self.model.__name__,
+                f"{self.model.__name__}: Tried to create inline object "
+                "from empty parent object"
             )
 
         for inline_field, model_name in inline_objects.items():
             if (
                 inline_field in parent_eve_data_obj
                 and parent_eve_data_obj[inline_field]
             ):
-                InlineModel = self.model.get_model_class(model_name)
-                esi_mapping = InlineModel._esi_mapping()
+                inline_model_class = self.model.get_model_class(model_name)
+                esi_mapping = inline_model_class._esi_mapping()
                 parent_fk = None
                 other_pk = None
-                ParentClass2 = None
+                parent_class_2 = None
                 for field_name, mapping in esi_mapping.items():
                     if mapping.is_pk:
                         if mapping.is_parent_fk:
                             parent_fk = field_name
                         else:
                             other_pk = (field_name, mapping)
-                            ParentClass2 = mapping.related_model
+                            parent_class_2 = mapping.related_model
 
                 if not parent_fk or not other_pk:
                     raise ValueError(
-                        "ESI Mapping for %s not valid: %s, %s"
-                        % (
-                            model_name,
-                            parent_fk,
-                            other_pk,
-                        )
+                        f"ESI Mapping for {model_name} not valid: "
+                        f"{parent_fk}, {other_pk}"
                     )
 
-                parent2_model_name = ParentClass2.__name__ if ParentClass2 else None
+                parent2_model_name = parent_class_2.__name__ if parent_class_2 else None
                 other_pk_info = {
                     "name": other_pk[0],
                     "esi_name": other_pk[1].esi_name,
                     "is_fk": other_pk[1].is_fk,
                 }
                 for eve_data_obj in parent_eve_data_obj[inline_field]:
                     if wait_for_children:
@@ -328,36 +331,36 @@
         parent2_model_name: Optional[str],
         inline_model_name: str,
         enabled_sections: Iterable[str],
     ):
         """Updates or creates a single inline object.
         Will automatically create additional parent objects as needed
         """
-        InlineModel = self.model.get_model_class(inline_model_name)
+        inline_model_class = self.model.get_model_class(inline_model_name)
 
         args = {f"{parent_fk}_id": parent_obj_id}
         esi_value = eve_data_obj.get(other_pk_info["esi_name"])
         if other_pk_info["is_fk"]:
-            ParentClass2 = self.model.get_model_class(parent2_model_name)
+            parent_class_2 = self.model.get_model_class(parent2_model_name)
             try:
-                value = ParentClass2.objects.get(id=esi_value)
-            except ParentClass2.DoesNotExist:
+                value = parent_class_2.objects.get(id=esi_value)
+            except parent_class_2.DoesNotExist:
                 try:
-                    value, _ = ParentClass2.objects.update_or_create_esi(id=esi_value)
+                    value, _ = parent_class_2.objects.update_or_create_esi(id=esi_value)
                 except AttributeError:
                     value = None
         else:
             value = esi_value
 
         key = other_pk_info["name"]
         args[key] = value  # type: ignore
-        args["defaults"] = InlineModel.objects._defaults_from_esi_obj(
+        args["defaults"] = inline_model_class.objects._defaults_from_esi_obj(
             eve_data_obj,
         )
-        InlineModel.objects.update_or_create(**args)
+        inline_model_class.objects.update_or_create(**args)
 
     def _update_or_create_children(
         self,
         *,
         parent_eve_data_obj: dict,
         include_children: bool,
         wait_for_children: bool,
@@ -367,26 +370,26 @@
         """updates or creates child objects as defined for this parent model (if any)"""
         from .tasks import (
             update_or_create_eve_object as task_update_or_create_eve_object,
         )
 
         if not parent_eve_data_obj:
             raise ValueError(
-                "%s: Tried to create children from empty parent object"
-                % self.model.__name__,
+                f"{self.model.__name__}: Tried to create children "
+                "from empty parent object"
             )
 
         for key, child_class in self.model._children(enabled_sections).items():
             if key in parent_eve_data_obj and parent_eve_data_obj[key]:
                 for obj in parent_eve_data_obj[key]:
                     # TODO: Refactor this hack
                     id = obj["planet_id"] if key == "planets" else obj
                     if wait_for_children:
-                        ChildClass = self.model.get_model_class(child_class)
-                        ChildClass.objects.update_or_create_esi(
+                        child_model_class = self.model.get_model_class(child_class)
+                        child_model_class.objects.update_or_create_esi(
                             id=id,
                             include_children=include_children,
                             wait_for_children=wait_for_children,
                             enabled_sections=enabled_sections,
                             task_priority=task_priority,
                         )
 
@@ -625,15 +628,15 @@
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Optional[Iterable[str]] = None,
         task_priority: Optional[int] = None,
-    ) -> Tuple[ModelType, bool]:
+    ) -> Tuple[Any, bool]:
         """updates or creates an EveStargate object by fetching it from ESI (blocking).
         Will always get/create parent objects
 
         Args:
             id: Eve Online ID of object
             include_children: (no effect)
             wait_for_children: (no effect)
@@ -676,15 +679,15 @@
         enabled_sections: Iterable[str],
         task_priority: Optional[int] = None,
     ) -> None:
         """updates_or_creates station service objects for EveStations"""
         from .models import EveStationService
 
         if "services" in parent_eve_data_obj:
-            services = list()
+            services = []
             for service_name in parent_eve_data_obj["services"]:
                 service, _ = EveStationService.objects.get_or_create(name=service_name)
                 services.append(service)
 
             if services:
                 parent_obj.services.add(*services)
 
@@ -698,15 +701,15 @@
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Optional[Iterable[str]] = None,
         task_priority: Optional[int] = None,
-    ) -> Tuple[ModelType, bool]:
+    ) -> Tuple[Any, bool]:
         obj, created = super().update_or_create_esi(
             id=id,
             include_children=include_children,
             wait_for_children=wait_for_children,
             enabled_sections=enabled_sections,
             task_priority=task_priority,
         )
@@ -759,15 +762,15 @@
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Optional[Iterable[str]] = None,
         task_priority: Optional[int] = None,
-    ) -> Tuple[ModelType, bool]:
+    ) -> Tuple[Any, bool]:
         """gets or creates an EvEntity object.
 
         The object is automatically fetched from ESI if it does not exist (blocking)
         or if it has not yet been resolved.
 
         Args:
             id: Eve Online ID of object
@@ -793,15 +796,15 @@
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Optional[Iterable[str]] = None,
         task_priority: Optional[int] = None,
-    ) -> Tuple[ModelType, bool]:
+    ) -> Tuple[Any, bool]:
         """Update or create an EveEntity object by fetching it from ESI (blocking).
 
         Args:
             id: Eve Online ID of object
             include_children: (no effect)
             wait_for_children: (no effect)
 
@@ -895,59 +898,69 @@
 
     def fetch_by_names_esi(
         self, names: Iterable[str], update: bool = False
     ) -> models.QuerySet:
         """Fetch entities matching given names.
         Will fetch missing entities from ESI if needed or requested.
 
+        Note that names that are not found by ESI are ignored.
+
         Args:
             names: Names of entities to fetch
             update: When True will always update from ESI
 
         Returns:
             query with matching entities.
         """
-        names = list(set(names))
-        query = self.filter(name__in=names)
-        if update or not query.exists():
-            result = self._fetch_names_from_esi(names)
-            if result:
-                result_compressed = {
-                    category: entities
-                    for category, entities in result.items()
-                    if entities
-                }
-                for category_key, entities in result_compressed.items():
-                    try:
-                        category = self._map_category_key_to_category(category_key)
-                    except ValueError:
-                        logger.warning(
-                            "Ignoring entities with unknown category %s: %s",
-                            category_key,
-                            entities,
-                        )
-                    else:
-                        for entity in entities:
-                            self.update_or_create(
-                                id=entity["id"],
-                                defaults={"name": entity["name"], "category": category},
-                            )
-        return query
+        names = set(names)
+        if update:
+            names_to_fetch = names
+        else:
+            existing_names = set(
+                self.filter(name__in=names).values_list("name", flat=True)
+            )
+            names_to_fetch = names - existing_names
+        if names_to_fetch:
+            esi_result = self._fetch_names_from_esi(names_to_fetch)
+            if esi_result:
+                self._update_or_create_entities(esi_result)
+        return self.filter(name__in=names)
+
+    def _update_or_create_entities(self, esi_result):
+        for category_key, entities in esi_result.items():
+            try:
+                category = self._map_category_key_to_category(category_key)
+            except ValueError:
+                logger.warning(
+                    "Ignoring entities with unknown category %s: %s",
+                    category_key,
+                    entities,
+                )
+                continue
+
+            for entity in entities:
+                self.update_or_create(
+                    id=entity["id"],
+                    defaults={"name": entity["name"], "category": category},
+                )
 
-    def _fetch_names_from_esi(self, names: List[str]) -> dict:
+    def _fetch_names_from_esi(self, names: Iterable[str]) -> dict:
         logger.info("Trying to fetch EveEntities from ESI by name")
         result = defaultdict(list)
-        for chunk_names in chunks(names, 500):
+        for chunk_names in chunks(list(names), 500):
             result_chunk = esi.client.Universe.post_universe_ids(
                 names=chunk_names
             ).results()
             for category, entities in result_chunk.items():
                 if entities:
                     result[category] += entities
-        return result
+        result_compressed = {
+            category: entities for category, entities in result.items() if entities
+        }
+        return result_compressed
 
     def _map_category_key_to_category(self, category_key: str) -> str:
         """Map category keys from ESI result to categories."""
         my_map = {
             "alliances": self.model.CATEGORY_ALLIANCE,
             "characters": self.model.CATEGORY_CHARACTER,
             "constellations": self.model.CATEGORY_CONSTELLATION,
@@ -982,15 +995,15 @@
             }
         )
 
     def update_from_esi_by_id(self, ids: Iterable[int]) -> int:
         """Updates all Eve entity objects by id from ESI."""
         if not ids:
             return 0
-        ids = list(set([int(id) for id in ids if id not in self.model.ESI_INVALID_IDS]))
+        ids = list(set((int(id) for id in ids if id not in self.model.ESI_INVALID_IDS)))
         logger.info("Updating %d entities from ESI", len(ids))
         resolved_counter = 0
         for chunk_ids in chunks(ids, POST_UNIVERSE_NAMES_MAX_ITEMS):
             logger.debug("Trying to resolve the following IDs from ESI:\n%s", chunk_ids)
             resolved_counter = self._resolve_entities_from_esi(chunk_ids)
         return resolved_counter
 
@@ -1022,18 +1035,20 @@
 
 
 EveEntityManager = EveEntityManagerBase.from_queryset(EveEntityQuerySet)
 
 
 class EveMarketPriceManager(models.Manager):
     def update_from_esi(self, minutes_until_stale: Optional[int] = None) -> int:
-        """Updates market prices from ESI. Will only create new price objects for EveTypes that already exist in the database.
+        """Updates market prices from ESI. Will only create new price objects
+        for EveTypes that already exist in the database.
 
         Args:
-            minutes_until_stale: only prices older then given minutes are regarding as stale and will be updated. Will use default (60) if not specified.
+            minutes_until_stale: only prices older then given minutes are regarding
+            as stale and will be updated. Will use default (60) if not specified.
 
         Returns:
             Count of updated types
         """
         from .models import EveType
 
         minutes_until_stale = (
@@ -1096,37 +1111,38 @@
         pass
 
     @property
     def sde_cache_timeout(self):
         return 3600 * 24
 
     @classmethod
-    def _response_to_cache(cls, r: requests.Response) -> dict:
-        data_all = dict()
-        for row in r.json():
+    def _response_to_cache(cls, response: requests.Response) -> dict:
+        data_all = {}
+        for row in response.json():
             type_id = row["typeID"]
             if type_id not in data_all:
-                data_all[type_id] = list()
+                data_all[type_id] = []
             data_all[type_id].append(row)
         cache.set(
             key=cls.sde_cache_key,
             value=data_all,
             timeout=cls.sde_cache_timeout,
         )
         return data_all
 
     @classmethod
     def _fetch_sde_data_cached(cls) -> dict:
         data = cache.get(cls.sde_cache_key)
         if not data:
-            r = requests.get(
-                urljoin(EVEUNIVERSE_API_SDE_URL, "latest/" + cls.sde_api_route)
+            response = requests.get(
+                urljoin(EVEUNIVERSE_API_SDE_URL, "latest/" + cls.sde_api_route),
+                timeout=10,
             )
-            r.raise_for_status()
-            data = cls._response_to_cache(r)
+            response.raise_for_status()
+            data = cls._response_to_cache(response)
             cache.set(
                 key=cls.sde_cache_key,
                 value=data,
                 timeout=cls.sde_cache_timeout,
             )
         return data
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/0001_initial.py` & `django_eveuniverse-1.3.1/eveuniverse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/0002_load_eveunit.py` & `django_eveuniverse-1.3.1/eveuniverse/migrations/0002_load_eveunit.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/0003_evemarketprice.py` & `django_eveuniverse-1.3.1/eveuniverse/migrations/0003_evemarketprice.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/0005_type_materials_and_sections.py` & `django_eveuniverse-1.3.1/eveuniverse/migrations/0005_type_materials_and_sections.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py` & `django_eveuniverse-1.3.1/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/0009_load_industry_activities.py` & `django_eveuniverse-1.3.1/eveuniverse/migrations/0009_load_industry_activities.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py` & `django_eveuniverse-1.3.1/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/eve_unit.json` & `django_eveuniverse-1.3.1/eveuniverse/migrations/eve_unit.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/migrations/industry_activities.json` & `django_eveuniverse-1.3.1/eveuniverse/migrations/industry_activities.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/models.py` & `django_eveuniverse-1.3.1/eveuniverse/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Eve universe models."""
 
+# pylint: disable = too-few-public-methods
+
 import enum
 import inspect
 import math
 import re
 import sys
 from collections import namedtuple
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
@@ -97,53 +99,57 @@
             [
                 f
                 for f in self._meta.get_fields()
                 if isinstance(f, models.Field) and f.name != "last_updated"
             ],
             key=lambda x: x.name,
         )
-        fields_2 = list()
-        for f in fields:
-            if f.many_to_one or f.one_to_one:
-                name = f"{f.name}_id"
+        fields_2 = []
+        for field in fields:
+            if field.many_to_one or field.one_to_one:
+                name = f"{field.name}_id"
                 value = getattr(self, name)
-            elif f.many_to_many:
-                name = f.name
-                value = ", ".join(sorted([str(x) for x in getattr(self, f.name).all()]))
+            elif field.many_to_many:
+                name = field.name
+                value = ", ".join(
+                    sorted([str(x) for x in getattr(self, field.name).all()])
+                )
             else:
-                name = f.name
-                value = getattr(self, f.name)
+                name = field.name
+                value = getattr(self, field.name)
 
             if isinstance(value, str):
-                if isinstance(f, models.TextField) and len(value) > 32:
+                if isinstance(field, models.TextField) and len(value) > 32:
                     value = f"{value[:32]}..."
                 text = f"{name}='{value}'"
             else:
                 text = f"{name}={value}"
 
             fields_2.append(text)
 
         return f"{self.__class__.__name__}({', '.join(fields_2)})"
 
     @classmethod
     def all_models(cls) -> List[Dict[models.Model, int]]:
-        """returns a list of all Eve Universe model classes sorted by load order"""
-        mappings = list()
-        for _, ModelClass in inspect.getmembers(sys.modules[__name__], inspect.isclass):
+        """Return a list of all Eve Universe model classes sorted by load order."""
+        mappings = []
+        for _, model_class in inspect.getmembers(
+            sys.modules[__name__], inspect.isclass
+        ):
             if issubclass(
-                ModelClass, (EveUniverseEntityModel, EveUniverseInlineModel)
-            ) and ModelClass not in (
+                model_class, (EveUniverseEntityModel, EveUniverseInlineModel)
+            ) and model_class not in (
                 cls,
                 EveUniverseEntityModel,
                 EveUniverseInlineModel,
             ):
                 mappings.append(
                     {
-                        "model": ModelClass,
-                        "load_order": ModelClass._eve_universe_meta_attr_strict(
+                        "model": model_class,
+                        "load_order": model_class._eve_universe_meta_attr_strict(
                             "load_order"
                         ),
                     }
                 )
 
         return [y["model"] for y in sorted(mappings, key=lambda x: x["load_order"])]
 
@@ -154,24 +160,24 @@
             x[0]: x[1]
             for x in inspect.getmembers(sys.modules[__name__], inspect.isclass)
             if issubclass(x[1], (EveUniverseBaseModel, EveUniverseInlineModel))
         }
         try:
             return classes[model_name]
         except KeyError:
-            raise ValueError("Unknown model_name: %s" % model_name) from None
+            raise ValueError(f"Unknown model_name: {model_name}") from None
 
     @classmethod
     def _esi_mapping(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
         field_mappings = cls._eve_universe_meta_attr("field_mappings")
         functional_pk = cls._eve_universe_meta_attr("functional_pk")
         parent_fk = cls._eve_universe_meta_attr("parent_fk")
         dont_create_related = cls._eve_universe_meta_attr("dont_create_related")
         disabled_fields = cls._disabled_fields(enabled_sections)
-        mapping = dict()
+        mapping = {}
         for field in [
             field
             for field in cls._meta.get_fields()
             if not field.auto_created
             and field.name not in {"last_updated", "enabled_sections"}
             and field.name not in disabled_fields
             and not field.many_to_many
@@ -185,18 +191,15 @@
                 is_pk = True
                 esi_name = cls._esi_pk()  # FIXME: This might fail
             elif functional_pk and field.name in functional_pk:
                 is_pk = True
             else:
                 is_pk = False
 
-            if parent_fk and is_pk and field.name in parent_fk:
-                is_parent_fk = True
-            else:
-                is_parent_fk = False
+            is_parent_fk = bool(parent_fk and is_pk and field.name in parent_fk)
 
             if isinstance(field, models.ForeignKey):
                 is_fk = True
                 related_model = field.related_model
             else:
                 is_fk = False
                 related_model = None
@@ -240,16 +243,16 @@
     ) -> Optional[Any]:
         try:
             value = getattr(cls.EveUniverseMeta, attr_name)  # type: ignore
         except AttributeError:
             value = None
             if is_mandatory:
                 raise ValueError(
-                    "Mandatory attribute EveUniverseMeta.%s not defined "
-                    "for class %s" % (attr_name, cls.__name__)
+                    f"Mandatory attribute EveUniverseMeta.{attr_name} not defined "
+                    f"for class {cls.__name__}"
                 ) from None
 
         return value
 
 
 class EveUniverseEntityModel(EveUniverseBaseModel):
     """Base class for Eve Universe Entity models.
@@ -352,21 +355,21 @@
             raise ValueError(f"{attr_name} not valid")
         return path.split(".")
 
     @classmethod
     def _children(cls, enabled_sections: Optional[Iterable[str]] = None) -> dict:
         """returns the mapping of children for this class"""
         mappings = cls._eve_universe_meta_attr("children")
-        return mappings if mappings else dict()
+        return mappings if mappings else {}
 
     @classmethod
     def _inline_objects(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
         """returns a dict of inline objects if any"""
         inline_objects = cls._eve_universe_meta_attr("inline_objects")
-        return inline_objects if inline_objects else dict()
+        return inline_objects if inline_objects else {}
 
     @classmethod
     def _is_list_only_endpoint(cls) -> bool:
         esi_path_list = cls._eve_universe_meta_attr("esi_path_list")
         esi_path_object = cls._eve_universe_meta_attr("esi_path_object")
         return (
             bool(esi_path_list)
@@ -393,15 +396,16 @@
 class EveEntity(EveUniverseEntityModel):
     """An Eve object from one of the categories supported by ESI's
     `/universe/names/` endpoint:
 
     alliance, character, constellation, faction, type, region, solar system, station
 
 
-    This is a special model model dedicated to quick resolution of Eve IDs to names and their categories, e.g. for characters. See also manager methods.
+    This is a special model model dedicated to quick resolution of Eve IDs to names
+    and their categories, e.g. for characters. See also manager methods.
     """
 
     # NPC IDs
     NPC_CORPORATION_ID_BEGIN = 1_000_000
     NPC_CORPORATION_ID_END = 2_000_000
     NPC_CHARACTER_ID_BEGIN = 3_000_000
     NPC_CHARACTER_ID_END = 4_000_000
@@ -440,15 +444,15 @@
     class EveUniverseMeta:
         esi_pk = "ids"
         esi_path_object = "Universe.post_universe_names"
         load_order = 110
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self._CATEGORIES = self.categories()
+        self._categories = self.categories()
 
     def __str__(self) -> str:
         if self.name:
             return self.name
         return f"ID:{self.id}"
 
     @property
@@ -535,33 +539,41 @@
         """URL to default third party website with profile info about this entity.
 
         Supported for:
         alliance, character, corporation, faction, region, solar system, station, type
         """
         if self.is_alliance:
             return dotlan.alliance_url(self.name)
-        elif self.is_character:
+
+        if self.is_character:
             return evewho.character_url(self.id)
-        elif self.is_corporation:
+
+        if self.is_corporation:
             return dotlan.corporation_url(self.name)
-        elif self.is_faction:
+
+        if self.is_faction:
             return dotlan.faction_url(self.name)
-        elif self.is_region:
+
+        if self.is_region:
             return dotlan.region_url(self.name)
-        elif self.is_solar_system:
+
+        if self.is_solar_system:
             return dotlan.solar_system_url(self.name)
-        elif self.is_station:
+
+        if self.is_station:
             return dotlan.station_url(self.name)
-        elif self.is_type:
+
+        if self.is_type:
             return eveitems.type_url(self.id)
+
         return ""
 
     def is_category(self, category: str) -> bool:
         """returns True if this entity has the given category, else False"""
-        return category in self._CATEGORIES and self.category == category
+        return category in self._categories and self.category == category
 
     def update_from_esi(self) -> "EveEntity":
         """Update the current object from ESI
 
         Returns:
             itself after update
         """
@@ -582,17 +594,17 @@
             self.CATEGORY_CHARACTER: "character_portrait_url",
             self.CATEGORY_CORPORATION: "corporation_logo_url",
             self.CATEGORY_FACTION: "faction_logo_url",
             self.CATEGORY_INVENTORY_TYPE: "type_icon_url",
         }
         if self.category not in map_category_2_other:
             return ""
-        else:
-            func = map_category_2_other[self.category]
-            return getattr(eveimageserver, func)(self.id, size=size)
+
+        func = map_category_2_other[self.category]
+        return getattr(eveimageserver, func)(self.id, size=size)
 
     @classmethod
     def categories(cls) -> Set[str]:
         """Set of valid categories."""
         return {x[0] for x in cls.CATEGORY_CHOICES}
 
     @classmethod
@@ -1002,20 +1014,18 @@
 
     objects = EveMarketPriceManager()
 
     def __str__(self) -> str:
         return f"{self.eve_type}: {self.average_price}"
 
     def __repr__(self) -> str:
-        return "{}(eve_type='{}', adjusted_price={}, average_price={}, updated_at={})".format(
-            type(self).__name__,
-            self.eve_type,
-            self.adjusted_price,
-            self.average_price,
-            self.updated_at.isoformat(),
+        return (
+            f"{type(self).__name__}(eve_type='{self.eve_type}', "
+            f"adjusted_price={self.adjusted_price}, average_price={self.average_price}, "
+            f"updated_at={self.updated_at})"
         )
 
 
 class EveMoon(EveUniverseEntityModel):
     """A moon in Eve Online"""
 
     eve_planet = models.ForeignKey(
@@ -1098,15 +1108,15 @@
         """
         matches = re.findall(r"Planet \((\S*)\)", self.eve_type.name)
         return matches[0] if matches else ""
 
     @classmethod
     def _children(cls, enabled_sections: Optional[Iterable[str]] = None) -> dict:
         enabled_sections = cls.determine_effective_sections(enabled_sections)
-        children = dict()
+        children = {}
         if cls.Section.ASTEROID_BELTS in enabled_sections:
             children["asteroid_belts"] = "EveAsteroidBelt"
         if cls.Section.MOONS in enabled_sections:
             children["moons"] = "EveMoon"
         return children
 
 
@@ -1330,15 +1340,16 @@
 
         Route is calculated by ESI
 
         Args:
             destination_id: ID of the other solar system to use in calculation
 
         Returns:
-            List of solar system IDs incl. origin and destination or None if no route can be found (e.g. if one system is in WH space)
+            List of solar system IDs incl. origin and destination
+            or None if no route can be found (e.g. if one system is in WH space)
         """
 
         try:
             return esi.client.Routes.get_route_origin_destination(
                 origin=origin_id, destination=destination_id
             ).results()
         except OSError:  # FIXME: ESI is supposed to return 404,
@@ -1371,26 +1382,26 @@
             EveGroupId.MOON: EveMoon,
             EveGroupId.PLANET: EvePlanet,
             EveGroupId.STAR: EveStar,
             EveGroupId.STARGATE: EveStargate,
             EveGroupId.STATION: EveStation,
         }
         try:
-            MyClass = class_mapping[eve_type.eve_group_id]
+            my_class = class_mapping[eve_type.eve_group_id]
         except KeyError:
             return None
-        obj, _ = MyClass.objects.get_or_create_esi(id=item.id)
+        obj, _ = my_class.objects.get_or_create_esi(id=item.id)
         return self.NearestCelestial(
             eve_type=eve_type, eve_object=obj, distance=item.distance
         )
 
     @classmethod
     def _children(cls, enabled_sections: Optional[Iterable[str]] = None) -> dict:
         enabled_sections = cls.determine_effective_sections(enabled_sections)
-        children = dict()
+        children = {}
         if cls.Section.PLANETS in enabled_sections:
             children["planets"] = "EvePlanet"
         if cls.Section.STARGATES in enabled_sections:
             children["stargates"] = "EveStargate"
         if cls.Section.STATIONS in enabled_sections:
             children["stations"] = "EveStation"
         return children
@@ -1401,15 +1412,15 @@
         if cls.Section.STARS not in enabled_sections:
             return {"eve_star"}
         return set()
 
     @classmethod
     def _inline_objects(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
         if not enabled_sections or cls.Section.PLANETS not in enabled_sections:
-            return dict()
+            return {}
         return super()._inline_objects()
 
 
 class EveStar(EveUniverseEntityModel):
     """A star in Eve Online"""
 
     age = models.BigIntegerField()
@@ -1671,15 +1682,16 @@
 
         if variant is self.IconVariant.SKIN:
             size = EveUniverseEntityModel.DEFAULT_ICON_SIZE if not size else size
             if EVEUNIVERSE_USE_EVESKINSERVER:
                 return eveskinserver.type_icon_url(self.id, size=size)
 
             if size < 32 or size > 128 or (size & (size - 1) != 0):
-                raise ValueError("Invalid size: {}".format(size))
+                raise ValueError(f"Invalid size: {size}")
+
             filename = f"eveuniverse/skin_generic_{size}.png"
             return staticfiles_storage.url(filename)
 
         return eveimageserver.type_icon_url(self.id, size=size)
 
     def render_url(self, size=EveUniverseEntityModel.DEFAULT_ICON_SIZE) -> str:
         """return an image URL to this type as render"""
@@ -1694,15 +1706,15 @@
         if cls.Section.MARKET_GROUPS not in enabled_sections:
             disabled_fields.add("eve_market_group")
         return disabled_fields
 
     @classmethod
     def _inline_objects(cls, enabled_sections: Optional[Set[str]] = None) -> dict:
         if not enabled_sections or cls.Section.DOGMAS not in enabled_sections:
-            return dict()
+            return {}
         return super()._inline_objects()
 
     @classmethod
     def eve_entity_category(cls) -> str:
         return EveEntity.CATEGORY_INVENTORY_TYPE
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_128.png` & `django_eveuniverse-1.3.1/eveuniverse/static/eveuniverse/skin_generic_128.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_32.png` & `django_eveuniverse-1.3.1/eveuniverse/static/eveuniverse/skin_generic_32.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_64.png` & `django_eveuniverse-1.3.1/eveuniverse/static/eveuniverse/skin_generic_64.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/swagger.json` & `django_eveuniverse-1.3.1/eveuniverse/swagger.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tasks.py` & `django_eveuniverse-1.3.1/eveuniverse/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 def load_eve_object(
     model_name: str, id: int, include_children=False, wait_for_children=True
 ) -> None:
     """Task for loading an eve object.
     Will only be created from ESI if it does not exist
     """
     logger.info("Loading %s with ID %s", model_name, id)
-    ModelClass = EveUniverseEntityModel.get_model_class(model_name)
-    ModelClass.objects.get_or_create_esi(  # type: ignore
+    model_class = EveUniverseEntityModel.get_model_class(model_name)
+    model_class.objects.get_or_create_esi(  # type: ignore
         id=id, include_children=include_children, wait_for_children=wait_for_children
     )
 
 
 @shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def update_or_create_eve_object(
     model_name: str,
@@ -67,22 +67,25 @@
     task_priority: Optional[int] = None,
 ) -> None:
     """Update or create an eve object from ESI.
 
     Args:
         model_name: Name of the respective Django model, e.g. ``"EveType"``
         id: Eve Online ID of object
-        include_children: if child objects should be updated/created as well (only when a new object is created)
-        wait_for_children: when true child objects will be updated/created blocking (if any), else async (only when a new object is created)
-        enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
+        include_children: if child objects should be updated/created as well
+        (only when a new object is created)
+        wait_for_children: when true child objects will be updated/created blocking (if any),
+        else async (only when a new object is created)
+        enabled_sections: Sections to load regardless of current settings,
+        e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
         task_priority: priority of started tasks
     """
     logger.info("Updating/Creating %s with ID %s", model_name, id)
-    ModelClass = EveUniverseEntityModel.get_model_class(model_name)
-    ModelClass.objects.update_or_create_esi(  # type: ignore
+    model_class = EveUniverseEntityModel.get_model_class(model_name)
+    model_class.objects.update_or_create_esi(  # type: ignore
         id=id,
         include_children=include_children,
         wait_for_children=wait_for_children,
         enabled_sections=enabled_sections,
         task_priority=task_priority,
     )
 
@@ -101,16 +104,16 @@
     """Task for updating or creating a single inline object from ESI"""
     logger.info(
         "Updating/Creating inline object %s for %s wit ID %s",
         inline_model_name,
         parent_model_name,
         parent_obj_id,
     )
-    ModelClass = EveUniverseEntityModel.get_model_class(parent_model_name)
-    ModelClass.objects._update_or_create_inline_object(  # type: ignore
+    model_class = EveUniverseEntityModel.get_model_class(parent_model_name)
+    model_class.objects._update_or_create_inline_object(  # type: ignore
         parent_obj_id=parent_obj_id,
         parent_fk=parent_fk,
         eve_data_obj=eve_data_obj,
         other_pk_info=other_pk_info,
         parent2_model_name=parent2_model_name,
         inline_model_name=inline_model_name,
         enabled_sections=enabled_sections,
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/pilot.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/pilot.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_backends.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_commands.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_core.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_helpers.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_1.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_models_1.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_2.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_models_2.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_3.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_models_3.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_4.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_models_4.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Eve Entity tests."""
 
+from typing import Dict
 from unittest.mock import patch
 
 from eveuniverse.models import EveEntity
 from eveuniverse.utils import NoSocketsTestCase
 
 from .testdata.esi import BravadoOperationStub, EsiClientStub
 from .testdata.factories import create_eve_entity
@@ -272,49 +273,14 @@
         # when
         self.assertEqual(EveEntity.objects.resolve_name(1001), "Bruce Wayne")
         self.assertEqual(EveEntity.objects.resolve_name(2001), "Wayne Technologies")
         self.assertEqual(EveEntity.objects.resolve_name(3001), "Wayne Enterprises")
         self.assertEqual(EveEntity.objects.resolve_name(999), "")
         self.assertEqual(EveEntity.objects.resolve_name(None), "")
 
-    def test_can_fetch_entity_by_name_from_esi(self, mock_esi):
-        # given
-        mock_esi.client = EsiClientStub()
-        # when
-        result = EveEntity.objects.fetch_by_names_esi(["Bruce Wayne"])
-        # then
-        self.assertListEqual(list(result), list(EveEntity.objects.filter(id=1001)))
-
-    def test_can_fetch_entities_by_name_from_esi(self, mock_esi):
-        # given
-        mock_esi.client = EsiClientStub()
-        # when
-        result = EveEntity.objects.fetch_by_names_esi(["Bruce Wayne", "Caldari State"])
-        # then
-        self.assertListEqual(
-            list(result), list(EveEntity.objects.filter(id__in=[500001, 1001]))
-        )
-
-    def test_can_fetch_entities_by_name_from_esi_huge(self, mock_esi):
-        # given
-        def my_endpoint(names):
-            characters = [
-                {"id": int(name.split("_")[1]), "name": name} for name in names
-            ]
-            data = {"characters": characters}
-            return BravadoOperationStub(data)
-
-        mock_esi.client.Universe.post_universe_ids.side_effect = my_endpoint
-        names = [f"dummy_{num + 1001}" for num in range(600)]
-        # when
-        result = EveEntity.objects.fetch_by_names_esi(names)
-        # then
-        self.assertEqual(mock_esi.client.Universe.post_universe_ids.call_count, 2)
-        self.assertEqual(len(result), 600)
-
     def test_can_bulk_resolve_name(self, mock_esi):
         # given
         mock_esi.client = EsiClientStub()
         resolver = EveEntity.objects.bulk_resolve_names([1001, 2001, 3001])
         # when
         self.assertEqual(resolver.to_name(1001), "Bruce Wayne")
         self.assertEqual(resolver.to_name(2001), "Wayne Technologies")
@@ -542,14 +508,117 @@
         self.assertFalse(obj.is_station)
         obj, _ = EveEntity.objects.update_or_create_esi(id=60015068)  # station
         self.assertTrue(obj.is_station)
         obj = EveEntity(id=666)
         self.assertFalse(obj.is_station)
 
 
+@patch(MANAGERS_PATH + ".esi")
+class TestEveEntityManagerFetchEntitiesByName(NoSocketsTestCase):
+    def test_can_fetch_entity_by_name_from_esi(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        # when
+        result = EveEntity.objects.fetch_by_names_esi(["Bruce Wayne"])
+        # then
+        self.assertListEqual(list(result), list(EveEntity.objects.filter(id=1001)))
+
+    def test_can_fetch_multiple_entities_by_name_from_esi(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        # when
+        result = EveEntity.objects.fetch_by_names_esi(["Bruce Wayne", "Caldari State"])
+        # then
+        self.assertListEqual(
+            list(result), list(EveEntity.objects.filter(id__in=[500001, 1001]))
+        )
+
+    def test_should_make_multiple_esi_request_when_fetching_large_number_of_entities(
+        self, mock_esi
+    ):
+        # given
+        def my_endpoint(names):
+            characters = [
+                {"id": int(name.split("_")[1]), "name": name} for name in names
+            ]
+            data = {"characters": characters}
+            return BravadoOperationStub(data)
+
+        mock_esi.client.Universe.post_universe_ids.side_effect = my_endpoint
+        names = [f"dummy_{num + 1001}" for num in range(600)]
+        # when
+        result = EveEntity.objects.fetch_by_names_esi(names)
+        # then
+        self.assertEqual(mock_esi.client.Universe.post_universe_ids.call_count, 2)
+        self.assertEqual(len(result), 600)
+
+    def test_should_fetch_unknown_entities_from_esi_only(self, mock_esi):
+        # given
+        mock_esi.client.Universe.post_universe_ids.return_value = BravadoOperationStub(
+            {
+                "characters": [
+                    {"id": 9991, "name": "alpha"},
+                    {"id": 9992, "name": "bravo"},
+                ],
+                "corporations": [
+                    {"id": 9993, "name": "charlie"},
+                ],
+            }
+        )
+        create_eve_entity(
+            id=1001, name="Bruce Wayne", category=EveEntity.CATEGORY_CHARACTER
+        )
+        # when
+        result_qs = EveEntity.objects.fetch_by_names_esi(
+            ["Bruce Wayne", "alpha", "bravo", "charlie"]
+        )
+        # then
+        self.assertTrue(mock_esi.client.Universe.post_universe_ids.called)
+        _, kwargs = mock_esi.client.Universe.post_universe_ids.call_args
+        self.assertSetEqual(set(kwargs["names"]), {"alpha", "bravo", "charlie"})
+        objs: Dict[int, EveEntity] = {obj.id: obj for obj in result_qs}
+        self.assertSetEqual(set(objs.keys()), {1001, 9991, 9992, 9993})
+        self.assertEqual(objs[1001].name, "Bruce Wayne")
+        self.assertTrue(objs[1001].is_character)
+        self.assertEqual(objs[9991].name, "alpha")
+        self.assertTrue(objs[9991].is_character)
+        self.assertEqual(objs[9992].name, "bravo")
+        self.assertTrue(objs[9992].is_character)
+        self.assertEqual(objs[9993].name, "charlie")
+        self.assertTrue(objs[9993].is_corporation)
+
+    def test_should_fetch_all_names_when_requested(self, mock_esi):
+        # given
+        mock_esi.client.Universe.post_universe_ids.return_value = BravadoOperationStub(
+            {
+                "characters": [
+                    {"id": 9991, "name": "alpha"},
+                    {"id": 1001, "name": "Bruce Wayne"},
+                ],
+            }
+        )
+        create_eve_entity(
+            id=1001, name="Bruce Wayne", category=EveEntity.CATEGORY_FACTION
+        )
+        # when
+        result_qs = EveEntity.objects.fetch_by_names_esi(
+            ["Bruce Wayne", "alpha"], update=True
+        )
+        # then
+        self.assertTrue(mock_esi.client.Universe.post_universe_ids.called)
+        _, kwargs = mock_esi.client.Universe.post_universe_ids.call_args
+        self.assertSetEqual(set(kwargs["names"]), {"Bruce Wayne", "alpha"})
+        objs: Dict[int, EveEntity] = {obj.id: obj for obj in result_qs}
+        self.assertSetEqual(set(objs.keys()), {1001, 9991})
+        self.assertEqual(objs[1001].name, "Bruce Wayne")
+        self.assertTrue(objs[1001].is_character)
+        self.assertEqual(objs[9991].name, "alpha")
+        self.assertTrue(objs[9991].is_character)
+
+
 class TestEveEntityProfileUrl(NoSocketsTestCase):
     def test_should_handle_alliance(self):
         # given
         obj = create_eve_entity(
             id=3001, name="Wayne Enterprises", category=EveEntity.CATEGORY_ALLIANCE
         )
         # when/then
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_tasks.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_tools_testdata.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_tools_testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/test_utils.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata/esi.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,17 +150,15 @@
             EsiEndpoint("Universe", "get_universe_types_type_id", "type_id"),
             EsiEndpoint("Universe", "get_universe_types", None),
             EsiEndpoint("Universe", "post_universe_names", None),
             EsiEndpoint("Universe", "post_universe_ids", None),
         ]
         for endpoint in esi_endpoints:
             if not hasattr(cls, endpoint.category):
-                setattr(
-                    cls, endpoint.category, type(endpoint.category, (object,), dict())
-                )
+                setattr(cls, endpoint.category, type(endpoint.category, (object,), {}))
             my_category = getattr(cls, endpoint.category)
             if not hasattr(my_category, endpoint.method):
                 setattr(
                     my_category,
                     endpoint.method,
                     EsiRoute(endpoint.category, endpoint.method, endpoint.key).call,
                 )
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi_data.json` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/factories.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...models import EveEntity
+from eveuniverse.models import EveEntity
 
 _items = {
     40170698: {
         "itemID": 40170698,
         "itemName": "Colelie VI - Asteroid Belt 1",
         "typeID": 15,
         "typeName": "Asteroid Belt",
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata/fetch_esi_raw_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     21961,
     21967,
 ]
 
 print("Fetching ESI raw data...")
 
 # fetching types from ESI
-esi_data = {"categories": dict(), "groups": dict(), "types": dict()}
+esi_data = {"categories": {}, "groups": {}, "types": {}}
 category_ids = set()
 group_ids = set()
 print("Fetching types...")
 for type_id in TYPE_IDS:
     r = requests.get(
         f"https://esi.evetech.net/latest/universe/types/{type_id}/",
         timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT,
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/generate_sde.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata/generate_sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata/sde.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def type_materials_cache_content():
     return cache_content(table="type_materials")
 
 
 def cache_content(table):
-    data_all = dict()
+    data_all = {}
     cached_data = sde_data[table]
     for row in cached_data:
         type_id = row["typeID"]
         if type_id not in data_all:
-            data_all[type_id] = list()
+            data_all[type_id] = []
         data_all[type_id].append(row)
     return data_all
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde_data.json` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata/sde_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/testdata_example.json` & `django_eveuniverse-1.3.1/eveuniverse/tests/testdata_example.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tests/tools/clear_celery_once_locks.py` & `django_eveuniverse-1.3.1/eveuniverse/tests/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tools/drop_tables.sql` & `django_eveuniverse-1.3.1/eveuniverse/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.3.0/eveuniverse/tools/testdata.py` & `django_eveuniverse-1.3.1/eveuniverse/tools/testdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 import logging
 from collections import OrderedDict, namedtuple
 from copy import deepcopy
 from typing import Iterable, List
 
 from django.core.serializers.json import DjangoJSONEncoder
 
+from eveuniverse import __title__
+from eveuniverse.core.esitools import is_esi_online
 from eveuniverse.models import EveSolarSystem, EveStargate, EveUniverseBaseModel
-
-from .. import __title__
-from ..core.esitools import is_esi_online
-from ..utils import LoggerAddTag
+from eveuniverse.utils import LoggerAddTag
 
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
 
 
 _ModelSpec = namedtuple(
     "ModelSpec", ["model_name", "ids", "include_children", "enabled_sections"]
 )
 
 
+# pylint: disable = invalid-name
 def ModelSpec(
     model_name: str,
     ids: List[int],
     include_children: bool = False,
     enabled_sections: Iterable[str] = None,
 ) -> _ModelSpec:
     """Wrapper for creating ModelSpec objects.
 
-    A Modelspec class defines what objects are to be loaded as test data
+    A ModelSpec class defines what objects are to be loaded as test data
 
     Args:
         model_name: Name of Eve Universe model
         ids: List of Eve IDs to be loaded
         include_children: Whether to also load children of those objects
     """
     return _ModelSpec(
@@ -96,16 +96,16 @@
                     del row["last_updated"]
                 except KeyError:
                     pass
 
             data[MyModel.__name__] = my_data
 
     print(f"Writing testdata to: {filepath}")
-    with open(filepath, "w", encoding="utf-8") as f:
-        json.dump(data, f, cls=DjangoJSONEncoder, indent=4, sort_keys=True)
+    with open(filepath, "w", encoding="utf-8") as file:
+        json.dump(data, file, cls=DjangoJSONEncoder, indent=4, sort_keys=True)
 
 
 def load_testdata_from_dict(testdata: dict) -> None:
     """creates eve objects in the database from testdata dump given as dict
 
     Args:
         testdata: The dict containing the testdata as created by `create_testdata()`
@@ -142,11 +142,11 @@
 
 def load_testdata_from_file(filepath: str) -> None:
     """creates eve objects in the database from testdata dump given as JSON file
 
     Args:
         filepath: Absolute path to the JSON file containing the testdata created by `create_testdata()`
     """
-    with open(filepath, "r", encoding="utf-8") as f:
-        testdata = json.load(f)
+    with open(filepath, "r", encoding="utf-8") as file:
+        testdata = json.load(file)
 
     load_testdata_from_dict(testdata)
```

### Comparing `django_eveuniverse-1.3.0/eveuniverse/utils.py` & `django_eveuniverse-1.3.1/eveuniverse/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 DATETIME_FORMAT = "%Y-%m-%d %H:%M"
 
 
 class LoggerAddTag(logging.LoggerAdapter):
     """add custom tag to a logger"""
 
     def __init__(self, my_logger, prefix):
-        super(LoggerAddTag, self).__init__(my_logger, {})
+        super().__init__(my_logger, {})
         self.prefix = prefix
 
     def process(self, msg, kwargs):
-        return "[%s] %s" % (self.prefix, msg), kwargs
+        return f"[{self.prefix}] {msg}", kwargs
 
 
 logger = LoggerAddTag(logging.getLogger(__name__), __package__)
 
 
 def chunks(lst, size):
     """Yield successive sized chunks from lst."""
@@ -66,16 +66,18 @@
             and (min_value is None or dirty_value >= min_value)
             and (max_value is None or dirty_value <= max_value)
             and (choices is None or dirty_value in choices)
         ):
             cleaned_value = dirty_value
         else:
             logger.warning(
-                "Your setting for {} it not valid. Please correct it. "
-                "Using default for now: {}".format(name, default_value)
+                "Your setting for %s it not valid. Please correct it. "
+                "Using default for now: %s",
+                name,
+                default_value,
             )
             cleaned_value = default_value
     return cleaned_value
 
 
 class SocketAccessError(Exception):
     pass
```

### Comparing `django_eveuniverse-1.3.0/pyproject.toml` & `django_eveuniverse-1.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-eveuniverse"
 dynamic = ["description", "version"]
 readme = "README.rst"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 requires-python = ">=3.8"
-authors = [
-    { name = "Erik Kalkoken", email = "kalkoken87@gmail.com" },
-]
+authors = [{ name = "Erik Kalkoken", email = "kalkoken87@gmail.com" }]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
@@ -44,20 +43,31 @@
 
 [tool.flit.module]
 name = "eveuniverse"
 
 [tool.isort]
 profile = "black"
 
+
 [tool.pylint.'MASTER']
-ignore-patterns="test_.*.py,__init__.py,generate_.*.py"
+ignore-patterns = ["__init__.py", "apps.py", "admin.py"]
+ignore-paths = ["^.*/tests/.*$", "^.*/migrations/.*$"]
 
 [tool.pylint.'BASIC']
-# Good variable names which should always be accepted, separated by a comma
-good-names="i,j,k,x,f,ex"
+good-names = ["i", "j", "k", "x", "y", "z", "ex", "id"]
 
 [tool.pylint.'FORMAT']
-# Maximum number of characters on a single line.
-max-line-length=100
+max-line-length = 120
 
 [tool.pylint.'MESSAGES CONTROL']
-disable="R,C"
+disable = [
+    "cyclic-import",
+    "fixme",
+    "too-many-arguments",
+    "redefined-builtin",
+    # "import-outside-toplevel",
+    # "too-many-instance-attributes",
+    # "too-few-public-methods",
+    # "imported-auth-user",
+    # "redefined-builtin",
+    # "no-member",
+]
```

### Comparing `django_eveuniverse-1.3.0/PKG-INFO` & `django_eveuniverse-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: django-eveuniverse
-Version: 1.3.0
+Version: 1.3.1
 Summary: Complete set of Eve Universe models with on-demand loading from ESI.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

