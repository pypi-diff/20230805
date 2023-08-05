# Comparing `tmp/OctoBot-Tentacles-Manager-2.9.2.tar.gz` & `tmp/OctoBot-Tentacles-Manager-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Tentacles-Manager-2.9.2.tar", last modified: Sun Jul 23 13:50:55 2023, max compression
+gzip compressed data, was "OctoBot-Tentacles-Manager-2.9.3.tar", last modified: Sat Aug  5 14:33:38 2023, max compression
```

## Comparing `OctoBot-Tentacles-Manager-2.9.2.tar` & `OctoBot-Tentacles-Manager-2.9.3.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.244009 OctoBot-Tentacles-Manager-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.228009 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-23 13:50:55.000000 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-23 13:50:55.000000 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 13:50:55.000000 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-23 13:50:55.000000 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 13:50:55.000000 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-23 13:50:55.000000 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-23 13:50:55.000000 OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-23 13:50:55.244009 OctoBot-Tentacles-Manager-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.228009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.228009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.228009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/util/tentacles_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.228009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.228009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/compiled_package_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.232009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Mode_config.template
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Social_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Strategies_config.template
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/TA_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Util_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/description_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.232009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/artifact_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/tentacle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.232009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/loaders/tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.232009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/profiles_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/tentacle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.236009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.236009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/artifact_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/metadata_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/profile_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_requirements_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.236009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/s3_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.236009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.236009 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/repair_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/single_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/tentacles_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/update_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-23 13:50:55.244009 OctoBot-Tentacles-Manager-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.224009 OctoBot-Tentacles-Manager-2.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/api/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/api/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/api/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/api/test_tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/api/test_uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/api/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/configuration/test_tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/configuration/test_tentacles_setup_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/tests/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/exporters/test_tentacle_bundle_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/loaders/test_tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/managers/test_tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/util/test_tentacle_fetching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/tests/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/workers/test_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/workers/test_uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/tests/workers/test_update_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:50:55.240009 OctoBot-Tentacles-Manager-2.9.2/upload_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/upload_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/upload_tests/_test_nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-23 13:50:00.000000 OctoBot-Tentacles-Manager-2.9.2/upload_tests/test_s3_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.810821 OctoBot-Tentacles-Manager-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.782821 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-05 14:33:38.000000 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-05 14:33:38.000000 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:33:38.000000 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-05 14:33:38.000000 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:33:38.000000 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-05 14:33:38.000000 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-05 14:33:38.000000 OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-05 14:33:38.810821 OctoBot-Tentacles-Manager-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.782821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.786821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.786821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/util/tentacles_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.786821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.790821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/compiled_package_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.790821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Mode_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Social_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Strategies_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/TA_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Util_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/description_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.790821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/artifact_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/tentacle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.794821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/loaders/tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.794821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/profiles_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/tentacle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.794821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.798821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/artifact_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/metadata_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/profile_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_requirements_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.798821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/s3_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.802821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.802821 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/repair_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/single_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/tentacles_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/update_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-05 14:33:38.810821 OctoBot-Tentacles-Manager-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.778820 OctoBot-Tentacles-Manager-2.9.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.802821 OctoBot-Tentacles-Manager-2.9.3/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/api/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/api/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/api/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/api/test_tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/api/test_uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/api/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.806821 OctoBot-Tentacles-Manager-2.9.3/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/configuration/test_tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/configuration/test_tentacles_setup_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.806821 OctoBot-Tentacles-Manager-2.9.3/tests/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/exporters/test_tentacle_bundle_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.806821 OctoBot-Tentacles-Manager-2.9.3/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/loaders/test_tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.806821 OctoBot-Tentacles-Manager-2.9.3/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/managers/test_tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.806821 OctoBot-Tentacles-Manager-2.9.3/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/util/test_tentacle_fetching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.806821 OctoBot-Tentacles-Manager-2.9.3/tests/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/workers/test_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/workers/test_uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/tests/workers/test_update_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:33:38.810821 OctoBot-Tentacles-Manager-2.9.3/upload_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/upload_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/upload_tests/_test_nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-05 14:32:57.000000 OctoBot-Tentacles-Manager-2.9.3/upload_tests/test_s3_uploader.py
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/CHANGELOG.md` & `OctoBot-Tentacles-Manager-2.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.9.3] - 2023-08-05
+### Added
+- API: set_tentacle_config_proxy context manager
+
 ## [2.9.2] - 2023-07-23
 ### Added
 - API: set_tentacle_config_proxy
 ### Updated
 - TentaclesSetupConfiguration#from_activated_tentacles_classes: accept tentacles classes as str
 
 ## [2.9.1] - 2023-05-05
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/LICENSE` & `OctoBot-Tentacles-Manager-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.9.2
+Version: 2.9.3
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Tentacles-Manager [2.9.2](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.3](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt` & `OctoBot-Tentacles-Manager-2.9.3/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.9.2
+Version: 2.9.3
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Tentacles-Manager [2.9.2](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.3](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/README.md` & `OctoBot-Tentacles-Manager-2.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Tentacles-Manager [2.9.2](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.3](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-VERSION = "2.9.2"
+VERSION = "2.9.3"
 PROJECT_NAME = "OctoBot-Tentacles-Manager"
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     save_tentacles_setup_configuration,
     has_profile_local_configuration,
     get_activated_tentacles,
     update_tentacle_config,
     import_user_tentacles_config_folder,
     get_tentacle_config,
     set_tentacle_config_proxy,
+    local_tentacle_config_proxy,
     factory_tentacle_reset_config,
     get_tentacle_config_schema_path,
     get_compiled_tentacles_url,
     set_tentacles_setup_configuration_path,
     ensure_setup_configuration,
     refresh_profile_tentacles_setup_config,
     get_code_hash,
@@ -117,14 +118,15 @@
     "deactivate_all_tentacles",
     "save_tentacles_setup_configuration",
     "has_profile_local_configuration",
     "get_activated_tentacles",
     "update_tentacle_config",
     "get_tentacle_config",
     "set_tentacle_config_proxy",
+    "local_tentacle_config_proxy",
     "import_user_tentacles_config_folder",
     "factory_tentacle_reset_config",
     "get_tentacle_config_schema_path",
     "get_compiled_tentacles_url",
     "set_tentacles_setup_configuration_path",
     "get_code_hash",
     "get_config_hash",
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/configurator.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,18 @@
     return configuration.get_config(tentacles_setup_config, klass)
 
 
 def set_tentacle_config_proxy(new_proxy) -> dict:
     return configuration.set_get_config_proxy(new_proxy)
 
 
+def local_tentacle_config_proxy(new_proxy):
+    return configuration.local_get_config_proxy(new_proxy)
+
+
 def factory_tentacle_reset_config(tentacles_setup_config: configuration.TentaclesSetupConfiguration, klass) -> None:
     return configuration.factory_reset_config(tentacles_setup_config, klass)
 
 
 def get_tentacle_config_schema_path(klass) -> str:
     return configuration.get_config_schema_path(klass)
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/creator.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/inspector.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/installer.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/loader.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/loader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/updater.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/uploader.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/api/util/tentacles_management.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/api/util/tentacles_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/cli.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,28 +20,30 @@
 
 from octobot_tentacles_manager.configuration.tentacles_setup_configuration import (
     TentaclesSetupConfiguration,
 )
 from octobot_tentacles_manager.configuration.tentacle_configuration import (
     get_config,
     set_get_config_proxy,
+    local_get_config_proxy,
     update_config,
     factory_reset_config,
     get_config_schema_path,
     get_user_tentacles_config_folder,
     get_profile_config_specific_file_path,
 )
 from octobot_tentacles_manager.configuration.config_file import (
     read_config,
     write_config,
 )
 
 __all__ = [
     "TentaclesSetupConfiguration",
     "set_get_config_proxy",
+    "local_get_config_proxy",
     "get_config",
     "update_config",
     "factory_reset_config",
     "get_config_schema_path",
     "get_user_tentacles_config_folder",
     "get_profile_config_specific_file_path",
     "read_config",
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/config_file.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/config_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/tentacle_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import contextlib
 import os
 import os.path as path
 import shutil
 
 import octobot_tentacles_manager.configuration as configuration
 import octobot_tentacles_manager.constants as constants
 import octobot_tentacles_manager.loaders as loaders
@@ -30,19 +31,29 @@
     return configuration.read_config(config_path)
 
 
 _GET_CONFIG_PROXY = _get_config_from_file_system
 
 
 def set_get_config_proxy(new_proxy):
-    # todo concurrency
+    # todo handle concurrency
     global _GET_CONFIG_PROXY
     _GET_CONFIG_PROXY = new_proxy
 
 
+@contextlib.contextmanager
+def local_get_config_proxy(new_proxy):
+    previous_proxy = _GET_CONFIG_PROXY
+    try:
+        set_get_config_proxy(new_proxy)
+        yield
+    finally:
+        set_get_config_proxy(previous_proxy)
+
+
 def get_config(tentacles_setup_config, klass) -> dict:
     return _GET_CONFIG_PROXY(tentacles_setup_config, klass)
 
 
 def update_config(tentacles_setup_config, klass, config_update, keep_existing=True) -> None:
     config_file = _get_config_file_path(tentacles_setup_config, klass)
     current_config = configuration.read_config(config_file)
```

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/constants.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/compiled_package_manager.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/compiled_package_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Mode_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Mode_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/templates/Social_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/templates/Social_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/creators/tentacle_creator.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/creators/tentacle_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/enums.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/artifact_exporter.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/artifact_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/tentacle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/tentacle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/exporters/tentacle_package_exporter.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/exporters/tentacle_package_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/loaders/tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/loaders/tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/profiles_manager.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/profiles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/python_modules_requirements_manager.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/python_modules_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/tentacle_manager.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/tentacle_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/tentacles_init_files_manager.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/tentacles_init_files_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/managers/tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/managers/tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/artifact.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/artifact.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/artifact_metadata.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/artifact_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/metadata_factory.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/metadata_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/profile_metadata.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/profile_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/tentacle_metadata.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/tentacle_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/profile.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/profile.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_factory.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_package.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_package.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_requirements_tree.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_requirements_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/models/tentacle_type.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/models/tentacle_type.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/uploaders/uploader.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/uploaders/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/file_util.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/file_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/hashing.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/hashing.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/os_util.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/os_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_cleaner.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_cleaner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_explorer.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_explorer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/util/tentacle_filter.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/util/tentacle_filter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/install_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/repair_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/repair_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/single_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/single_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/tentacles_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/tentacles_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/octobot_tentacles_manager/workers/update_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/octobot_tentacles_manager/workers/update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/setup.py` & `OctoBot-Tentacles-Manager-2.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/api/test_configurator.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/api/test_configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/api/test_creator.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/api/test_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/api/test_installer.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/api/test_installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/api/test_uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/api/test_uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/api/test_updater.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/api/test_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/configuration/test_tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/configuration/test_tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/configuration/test_tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/configuration/test_tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/exporters/test_tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/exporters/test_tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/loaders/test_tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/loaders/test_tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/managers/test_tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/managers/test_tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/util/test_tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/util/test_tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/workers/test_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/workers/test_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/workers/test_uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/workers/test_uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/tests/workers/test_update_worker.py` & `OctoBot-Tentacles-Manager-2.9.3/tests/workers/test_update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/upload_tests/__init__.py` & `OctoBot-Tentacles-Manager-2.9.3/upload_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/upload_tests/_test_nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.3/upload_tests/_test_nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.2/upload_tests/test_s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.3/upload_tests/test_s3_uploader.py`

 * *Files identical despite different names*

