# Comparing `tmp/cuppa-0.9.98.tar.gz` & `tmp/cuppa-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuppa-0.9.98.tar", last modified: Fri Feb 24 14:04:45 2023, max compression
+gzip compressed data, was "cuppa-0.9.99.tar", last modified: Fri Feb 24 15:38:34 2023, max compression
```

## Comparing `cuppa-0.9.98.tar` & `cuppa-0.9.99.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.396688 cuppa-0.9.98/
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1339 2016-11-09 10:52:08.000000 cuppa-0.9.98/LICENSE_1_0.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)       57 2016-11-09 10:52:08.000000 cuppa-0.9.98/MANIFEST.in
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6964 2023-02-24 14:04:45.396688 cuppa-0.9.98/PKG-INFO
--rw-r--r--   0 jamie     (1000) jamie     (1000)    56472 2022-08-12 00:31:17.000000 cuppa-0.9.98/README.md
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6333 2016-11-09 10:52:08.000000 cuppa-0.9.98/README.rst
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.384688 cuppa-0.9.98/cuppa/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        7 2023-02-24 14:01:28.000000 cuppa-0.9.98/cuppa/VERSION
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2392 2020-07-21 16:22:11.000000 cuppa-0.9.98/cuppa/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3661 2021-03-31 22:12:28.000000 cuppa-0.9.98/cuppa/__main__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1920 2017-07-30 14:59:31.000000 cuppa-0.9.98/cuppa/build_platform.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    14421 2020-06-05 13:06:00.000000 cuppa-0.9.98/cuppa/build_with_location.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      870 2017-07-05 10:18:14.000000 cuppa-0.9.98/cuppa/build_with_profile.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     8272 2022-11-13 21:57:41.000000 cuppa-0.9.98/cuppa/colourise.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    11299 2020-02-20 15:19:36.000000 cuppa-0.9.98/cuppa/configure.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    42008 2023-02-24 14:01:28.000000 cuppa-0.9.98/cuppa/construct.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.388688 cuppa-0.9.98/cuppa/core/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/core/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6089 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/core/base_options.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7853 2022-11-12 23:50:47.000000 cuppa-0.9.98/cuppa/core/environment.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3635 2021-03-31 17:37:43.000000 cuppa-0.9.98/cuppa/core/location_options.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      722 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/core/options.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2542 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/core/storage_options.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.388688 cuppa-0.9.98/cuppa/cpp/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      212 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/cpp/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    17748 2021-03-31 17:37:43.000000 cuppa-0.9.98/cuppa/cpp/create_version_file_cpp.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    28035 2020-06-05 13:06:00.000000 cuppa-0.9.98/cuppa/cpp/run_boost_test.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    37530 2022-10-04 19:31:10.000000 cuppa-0.9.98/cuppa/cpp/run_gcov_coverage.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    31245 2020-03-09 16:37:08.000000 cuppa-0.9.98/cuppa/cpp/run_patched_boost_test.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    14815 2020-03-09 16:37:08.000000 cuppa-0.9.98/cuppa/cpp/run_process_test.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.388688 cuppa-0.9.98/cuppa/cpp/templates/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/cpp/templates/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7081 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/cpp/templates/coverage_index.html
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.388688 cuppa-0.9.98/cuppa/dependencies/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/dependencies/__init__.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.392688 cuppa-0.9.98/cuppa/dependencies/boost/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/dependencies/boost/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     8036 2022-08-12 00:31:17.000000 cuppa-0.9.98/cuppa/dependencies/boost/b2.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    69512 2020-07-21 16:22:11.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_bug_fix_1.73.0.diff
--rw-r--r--   0 jamie     (1000) jamie     (1000)    19862 2022-08-12 00:31:17.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_builder.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      597 2020-02-17 21:46:30.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_exception.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3636 2017-07-30 15:00:34.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_library_methods.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    36915 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.58.0.diff
--rw-r--r--   0 jamie     (1000) jamie     (1000)    12061 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.67.0.diff
--rw-r--r--   0 jamie     (1000) jamie     (1000)    12778 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.68.0.diff
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7737 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.71.0.diff
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7724 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.72.0.diff
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2714 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/configjam.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3334 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/library_dependencies.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4027 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/dependencies/boost/library_naming.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3216 2022-06-26 15:37:22.000000 cuppa-0.9.98/cuppa/dependencies/boost/patch_boost.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     8210 2022-12-15 18:28:05.000000 cuppa-0.9.98/cuppa/dependencies/boost/version_and_location.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7783 2020-09-10 23:44:40.000000 cuppa-0.9.98/cuppa/dependencies/build_with_boost.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4486 2020-02-20 15:19:36.000000 cuppa-0.9.98/cuppa/dependencies/build_with_qt4.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4405 2020-02-20 15:19:36.000000 cuppa-0.9.98/cuppa/dependencies/build_with_qt5.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7218 2022-09-15 09:07:07.000000 cuppa-0.9.98/cuppa/dependencies/build_with_quince.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    36175 2021-03-31 22:12:28.000000 cuppa-0.9.98/cuppa/location.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4392 2020-02-18 10:16:18.000000 cuppa-0.9.98/cuppa/log.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.392688 cuppa-0.9.98/cuppa/method_helpers/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/method_helpers/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    11642 2021-03-31 22:12:28.000000 cuppa-0.9.98/cuppa/method_helpers/run_process.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.392688 cuppa-0.9.98/cuppa/methods/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/methods/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4443 2022-12-11 18:16:57.000000 cuppa-0.9.98/cuppa/methods/asciidoc_to_html.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1856 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/methods/build.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1254 2017-07-30 14:59:31.000000 cuppa-0.9.98/cuppa/methods/build_library.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2272 2017-07-30 14:59:31.000000 cuppa-0.9.98/cuppa/methods/build_profile.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2462 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/methods/build_test.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2491 2022-11-12 23:50:47.000000 cuppa-0.9.98/cuppa/methods/build_with.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2998 2020-02-18 10:16:18.000000 cuppa-0.9.98/cuppa/methods/compile.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2329 2022-12-11 18:14:31.000000 cuppa-0.9.98/cuppa/methods/compile_scss.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1335 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/methods/copyfiles.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1236 2017-01-06 14:33:42.000000 cuppa-0.9.98/cuppa/methods/copyfilesas.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3882 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/methods/coverage.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1250 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/methods/create_version.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1846 2020-02-18 10:16:18.000000 cuppa-0.9.98/cuppa/methods/expand_template_file.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      825 2017-01-06 14:33:42.000000 cuppa-0.9.98/cuppa/methods/filter.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1936 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/methods/markdown_to_html.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3479 2021-03-31 22:12:28.000000 cuppa-0.9.98/cuppa/methods/relative_recursive_glob.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1124 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/methods/remove_flags.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     5603 2023-02-24 14:01:28.000000 cuppa-0.9.98/cuppa/methods/render_jinja_template.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      700 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/methods/replace_flags.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2188 2020-03-09 16:37:08.000000 cuppa-0.9.98/cuppa/methods/run.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2571 2022-12-11 18:16:57.000000 cuppa-0.9.98/cuppa/methods/run_and_redirect_to_file.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1659 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/methods/stdcpp.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      699 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/methods/target_from.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2276 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/methods/test.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      777 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/methods/toolchain.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      782 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/methods/using.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.392688 cuppa-0.9.98/cuppa/modules/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      212 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/modules/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4126 2021-03-31 22:12:28.000000 cuppa-0.9.98/cuppa/modules/registration.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      882 2020-07-21 16:22:11.000000 cuppa-0.9.98/cuppa/output.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    13448 2021-03-31 22:12:28.000000 cuppa-0.9.98/cuppa/output_processor.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1917 2020-03-09 16:37:08.000000 cuppa-0.9.98/cuppa/path.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.392688 cuppa-0.9.98/cuppa/platforms/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/platforms/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2983 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/platforms/darwin.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3931 2020-03-09 16:37:08.000000 cuppa-0.9.98/cuppa/platforms/linux.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2122 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/platforms/windows.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.392688 cuppa-0.9.98/cuppa/profiles/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/profiles/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4589 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/progress.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.392688 cuppa-0.9.98/cuppa/project_generators/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/project_generators/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    20332 2020-07-21 16:35:48.000000 cuppa-0.9.98/cuppa/project_generators/codeblocks.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2402 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/recursive_glob.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.396688 cuppa-0.9.98/cuppa/scms/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      211 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/scms/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2711 2020-06-05 13:06:00.000000 cuppa-0.9.98/cuppa/scms/bazaar.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    10934 2022-10-03 21:18:54.000000 cuppa-0.9.98/cuppa/scms/git.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2682 2020-06-05 13:06:00.000000 cuppa-0.9.98/cuppa/scms/mercurial.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1896 2021-03-31 17:37:43.000000 cuppa-0.9.98/cuppa/scms/scms.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2675 2020-06-05 13:06:00.000000 cuppa-0.9.98/cuppa/scms/subversion.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.396688 cuppa-0.9.98/cuppa/test_report/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/test_report/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1409 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/test_report/cuppa_json.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3257 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/test_report/generate_bitten_report.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    28672 2022-10-03 21:20:17.000000 cuppa-0.9.98/cuppa/test_report/html_report.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.396688 cuppa-0.9.98/cuppa/test_report/templates/
--rw-r--r--   0 jamie     (1000) jamie     (1000)    20406 2022-10-03 21:18:54.000000 cuppa-0.9.98/cuppa/test_report/templates/test_report_index.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)    23545 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/test_report/templates/test_suite_index.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4493 2020-02-18 10:16:18.000000 cuppa-0.9.98/cuppa/timer.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.396688 cuppa-0.9.98/cuppa/toolchains/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/toolchains/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    11751 2022-01-10 11:38:28.000000 cuppa-0.9.98/cuppa/toolchains/cl.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    25355 2020-09-10 23:44:40.000000 cuppa-0.9.98/cuppa/toolchains/clang.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    29045 2023-02-24 14:01:28.000000 cuppa-0.9.98/cuppa/toolchains/gcc.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1936 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/tree.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.396688 cuppa-0.9.98/cuppa/utility/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2017-01-06 14:33:42.000000 cuppa-0.9.98/cuppa/utility/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      636 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/utility/attr_tools.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      663 2021-03-31 22:12:28.000000 cuppa-0.9.98/cuppa/utility/dict_tools.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1992 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/utility/filter.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     5255 2022-04-08 12:08:01.000000 cuppa-0.9.98/cuppa/utility/pip_imports.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      582 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/utility/preprocess.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1898 2022-01-10 11:38:28.000000 cuppa-0.9.98/cuppa/utility/python2to3.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      582 2017-01-06 14:33:42.000000 cuppa-0.9.98/cuppa/utility/types.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      726 2017-01-06 14:33:42.000000 cuppa-0.9.98/cuppa/utility/version.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.396688 cuppa-0.9.98/cuppa/variants/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/variants/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      822 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/variants/cov.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      774 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/variants/dbg.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      788 2016-11-09 10:52:08.000000 cuppa-0.9.98/cuppa/variants/rel.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1262 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/variants/run.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1321 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/variants/test.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1331 2020-02-17 17:01:23.000000 cuppa-0.9.98/cuppa/version.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 14:04:45.384688 cuppa-0.9.98/cuppa.egg-info/
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6964 2023-02-24 14:04:44.000000 cuppa-0.9.98/cuppa.egg-info/PKG-INFO
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3927 2023-02-24 14:04:45.000000 cuppa-0.9.98/cuppa.egg-info/SOURCES.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)        1 2023-02-24 14:04:44.000000 cuppa-0.9.98/cuppa.egg-info/dependency_links.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)      400 2023-02-24 14:04:45.000000 cuppa-0.9.98/cuppa.egg-info/entry_points.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)       57 2023-02-24 14:04:45.000000 cuppa-0.9.98/cuppa.egg-info/requires.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)        6 2023-02-24 14:04:45.000000 cuppa-0.9.98/cuppa.egg-info/top_level.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)       38 2023-02-24 14:04:45.396688 cuppa-0.9.98/setup.cfg
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3362 2023-02-24 14:01:28.000000 cuppa-0.9.98/setup.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.961190 cuppa-0.9.99/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1339 2016-11-09 10:52:08.000000 cuppa-0.9.99/LICENSE_1_0.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       57 2016-11-09 10:52:08.000000 cuppa-0.9.99/MANIFEST.in
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6964 2023-02-24 15:38:34.961190 cuppa-0.9.99/PKG-INFO
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    56472 2022-08-12 00:31:17.000000 cuppa-0.9.99/README.md
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6333 2016-11-09 10:52:08.000000 cuppa-0.9.99/README.rst
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.945190 cuppa-0.9.99/cuppa/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        7 2023-02-24 15:38:28.000000 cuppa-0.9.99/cuppa/VERSION
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2392 2020-07-21 16:22:11.000000 cuppa-0.9.99/cuppa/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3661 2021-03-31 22:12:28.000000 cuppa-0.9.99/cuppa/__main__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1920 2017-07-30 14:59:31.000000 cuppa-0.9.99/cuppa/build_platform.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    14421 2020-06-05 13:06:00.000000 cuppa-0.9.99/cuppa/build_with_location.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      870 2017-07-05 10:18:14.000000 cuppa-0.9.99/cuppa/build_with_profile.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     8272 2022-11-13 21:57:41.000000 cuppa-0.9.99/cuppa/colourise.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    11299 2020-02-20 15:19:36.000000 cuppa-0.9.99/cuppa/configure.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    42008 2023-02-24 14:01:28.000000 cuppa-0.9.99/cuppa/construct.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.945190 cuppa-0.9.99/cuppa/core/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/core/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6089 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/core/base_options.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7853 2022-11-12 23:50:47.000000 cuppa-0.9.99/cuppa/core/environment.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3635 2021-03-31 17:37:43.000000 cuppa-0.9.99/cuppa/core/location_options.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      722 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/core/options.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2542 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/core/storage_options.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.949190 cuppa-0.9.99/cuppa/cpp/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      212 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/cpp/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    17748 2021-03-31 17:37:43.000000 cuppa-0.9.99/cuppa/cpp/create_version_file_cpp.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    28035 2020-06-05 13:06:00.000000 cuppa-0.9.99/cuppa/cpp/run_boost_test.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    37530 2022-10-04 19:31:10.000000 cuppa-0.9.99/cuppa/cpp/run_gcov_coverage.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    31245 2020-03-09 16:37:08.000000 cuppa-0.9.99/cuppa/cpp/run_patched_boost_test.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    14815 2020-03-09 16:37:08.000000 cuppa-0.9.99/cuppa/cpp/run_process_test.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.949190 cuppa-0.9.99/cuppa/cpp/templates/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/cpp/templates/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7081 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/cpp/templates/coverage_index.html
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.949190 cuppa-0.9.99/cuppa/dependencies/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/dependencies/__init__.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.949190 cuppa-0.9.99/cuppa/dependencies/boost/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/dependencies/boost/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     8036 2022-08-12 00:31:17.000000 cuppa-0.9.99/cuppa/dependencies/boost/b2.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    69512 2020-07-21 16:22:11.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_bug_fix_1.73.0.diff
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    19862 2022-08-12 00:31:17.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_builder.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      597 2020-02-17 21:46:30.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_exception.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3636 2017-07-30 15:00:34.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_library_methods.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    36915 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.58.0.diff
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    12061 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.67.0.diff
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    12778 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.68.0.diff
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7737 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.71.0.diff
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7724 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.72.0.diff
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2714 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/configjam.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3334 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/library_dependencies.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4027 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/dependencies/boost/library_naming.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3216 2022-06-26 15:37:22.000000 cuppa-0.9.99/cuppa/dependencies/boost/patch_boost.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     8210 2022-12-15 18:28:05.000000 cuppa-0.9.99/cuppa/dependencies/boost/version_and_location.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7783 2020-09-10 23:44:40.000000 cuppa-0.9.99/cuppa/dependencies/build_with_boost.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4486 2020-02-20 15:19:36.000000 cuppa-0.9.99/cuppa/dependencies/build_with_qt4.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4405 2020-02-20 15:19:36.000000 cuppa-0.9.99/cuppa/dependencies/build_with_qt5.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7218 2022-09-15 09:07:07.000000 cuppa-0.9.99/cuppa/dependencies/build_with_quince.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    36175 2021-03-31 22:12:28.000000 cuppa-0.9.99/cuppa/location.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4392 2020-02-18 10:16:18.000000 cuppa-0.9.99/cuppa/log.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.949190 cuppa-0.9.99/cuppa/method_helpers/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/method_helpers/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    11642 2021-03-31 22:12:28.000000 cuppa-0.9.99/cuppa/method_helpers/run_process.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.953189 cuppa-0.9.99/cuppa/methods/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/methods/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4443 2022-12-11 18:16:57.000000 cuppa-0.9.99/cuppa/methods/asciidoc_to_html.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1856 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/methods/build.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1254 2017-07-30 14:59:31.000000 cuppa-0.9.99/cuppa/methods/build_library.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2272 2017-07-30 14:59:31.000000 cuppa-0.9.99/cuppa/methods/build_profile.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2462 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/methods/build_test.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2491 2022-11-12 23:50:47.000000 cuppa-0.9.99/cuppa/methods/build_with.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2998 2020-02-18 10:16:18.000000 cuppa-0.9.99/cuppa/methods/compile.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2329 2022-12-11 18:14:31.000000 cuppa-0.9.99/cuppa/methods/compile_scss.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1335 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/methods/copyfiles.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1236 2017-01-06 14:33:42.000000 cuppa-0.9.99/cuppa/methods/copyfilesas.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3882 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/methods/coverage.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1250 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/methods/create_version.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1846 2020-02-18 10:16:18.000000 cuppa-0.9.99/cuppa/methods/expand_template_file.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      825 2017-01-06 14:33:42.000000 cuppa-0.9.99/cuppa/methods/filter.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1936 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/methods/markdown_to_html.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3479 2021-03-31 22:12:28.000000 cuppa-0.9.99/cuppa/methods/relative_recursive_glob.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1124 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/methods/remove_flags.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     5603 2023-02-24 14:01:28.000000 cuppa-0.9.99/cuppa/methods/render_jinja_template.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      700 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/methods/replace_flags.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2188 2020-03-09 16:37:08.000000 cuppa-0.9.99/cuppa/methods/run.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2571 2022-12-11 18:16:57.000000 cuppa-0.9.99/cuppa/methods/run_and_redirect_to_file.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1659 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/methods/stdcpp.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      699 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/methods/target_from.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2276 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/methods/test.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      777 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/methods/toolchain.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      782 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/methods/using.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.953189 cuppa-0.9.99/cuppa/modules/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      212 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/modules/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4126 2021-03-31 22:12:28.000000 cuppa-0.9.99/cuppa/modules/registration.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      882 2020-07-21 16:22:11.000000 cuppa-0.9.99/cuppa/output.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    13448 2021-03-31 22:12:28.000000 cuppa-0.9.99/cuppa/output_processor.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1917 2020-03-09 16:37:08.000000 cuppa-0.9.99/cuppa/path.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.953189 cuppa-0.9.99/cuppa/platforms/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/platforms/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2983 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/platforms/darwin.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3931 2020-03-09 16:37:08.000000 cuppa-0.9.99/cuppa/platforms/linux.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2122 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/platforms/windows.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.953189 cuppa-0.9.99/cuppa/profiles/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/profiles/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4589 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/progress.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.953189 cuppa-0.9.99/cuppa/project_generators/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/project_generators/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    20332 2020-07-21 16:35:48.000000 cuppa-0.9.99/cuppa/project_generators/codeblocks.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2402 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/recursive_glob.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.957190 cuppa-0.9.99/cuppa/scms/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      211 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/scms/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2711 2020-06-05 13:06:00.000000 cuppa-0.9.99/cuppa/scms/bazaar.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    10934 2022-10-03 21:18:54.000000 cuppa-0.9.99/cuppa/scms/git.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2682 2020-06-05 13:06:00.000000 cuppa-0.9.99/cuppa/scms/mercurial.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1896 2021-03-31 17:37:43.000000 cuppa-0.9.99/cuppa/scms/scms.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2675 2020-06-05 13:06:00.000000 cuppa-0.9.99/cuppa/scms/subversion.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.957190 cuppa-0.9.99/cuppa/test_report/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/test_report/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1409 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/test_report/cuppa_json.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3257 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/test_report/generate_bitten_report.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    28672 2022-10-03 21:20:17.000000 cuppa-0.9.99/cuppa/test_report/html_report.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.957190 cuppa-0.9.99/cuppa/test_report/templates/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    20406 2022-10-03 21:18:54.000000 cuppa-0.9.99/cuppa/test_report/templates/test_report_index.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    23545 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/test_report/templates/test_suite_index.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4493 2020-02-18 10:16:18.000000 cuppa-0.9.99/cuppa/timer.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.957190 cuppa-0.9.99/cuppa/toolchains/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/toolchains/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    11751 2022-01-10 11:38:28.000000 cuppa-0.9.99/cuppa/toolchains/cl.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    25355 2020-09-10 23:44:40.000000 cuppa-0.9.99/cuppa/toolchains/clang.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    29045 2023-02-24 14:01:28.000000 cuppa-0.9.99/cuppa/toolchains/gcc.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1936 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/tree.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.957190 cuppa-0.9.99/cuppa/utility/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        2 2017-01-06 14:33:42.000000 cuppa-0.9.99/cuppa/utility/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      636 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/utility/attr_tools.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      663 2021-03-31 22:12:28.000000 cuppa-0.9.99/cuppa/utility/dict_tools.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      784 2023-02-24 15:38:28.000000 cuppa-0.9.99/cuppa/utility/file_types.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1992 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/utility/filter.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     5255 2022-04-08 12:08:01.000000 cuppa-0.9.99/cuppa/utility/pip_imports.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      582 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/utility/preprocess.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1898 2022-01-10 11:38:28.000000 cuppa-0.9.99/cuppa/utility/python2to3.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      582 2017-01-06 14:33:42.000000 cuppa-0.9.99/cuppa/utility/types.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      726 2017-01-06 14:33:42.000000 cuppa-0.9.99/cuppa/utility/version.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.957190 cuppa-0.9.99/cuppa/variants/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      298 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/variants/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      822 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/variants/cov.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      774 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/variants/dbg.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      788 2016-11-09 10:52:08.000000 cuppa-0.9.99/cuppa/variants/rel.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1262 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/variants/run.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1321 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/variants/test.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1331 2020-02-17 17:01:23.000000 cuppa-0.9.99/cuppa/version.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-02-24 15:38:34.945190 cuppa-0.9.99/cuppa.egg-info/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6964 2023-02-24 15:38:34.000000 cuppa-0.9.99/cuppa.egg-info/PKG-INFO
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3955 2023-02-24 15:38:34.000000 cuppa-0.9.99/cuppa.egg-info/SOURCES.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        1 2023-02-24 15:38:34.000000 cuppa-0.9.99/cuppa.egg-info/dependency_links.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      400 2023-02-24 15:38:34.000000 cuppa-0.9.99/cuppa.egg-info/entry_points.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       57 2023-02-24 15:38:34.000000 cuppa-0.9.99/cuppa.egg-info/requires.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        6 2023-02-24 15:38:34.000000 cuppa-0.9.99/cuppa.egg-info/top_level.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       38 2023-02-24 15:38:34.961190 cuppa-0.9.99/setup.cfg
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3362 2023-02-24 14:01:28.000000 cuppa-0.9.99/setup.py
```

### Comparing `cuppa-0.9.98/LICENSE_1_0.txt` & `cuppa-0.9.99/LICENSE_1_0.txt`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/PKG-INFO` & `cuppa-0.9.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuppa
-Version: 0.9.98
+Version: 0.9.99
 Summary: Cuppa, an extension package to simplify and extend Scons
 Home-page: https://github.com/ja11sop/cuppa
 Author: ja11sop
 License: Boost Software License 1.0 - http://www.boost.org/LICENSE_1_0.txt
 Keywords: scons,build,c++
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Intended Audience :: Developers
```

### Comparing `cuppa-0.9.98/README.md` & `cuppa-0.9.99/README.md`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/README.rst` & `cuppa-0.9.99/README.rst`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/__init__.py` & `cuppa-0.9.99/cuppa/__init__.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/__main__.py` & `cuppa-0.9.99/cuppa/__main__.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/build_platform.py` & `cuppa-0.9.99/cuppa/build_platform.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/build_with_location.py` & `cuppa-0.9.99/cuppa/build_with_location.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/build_with_profile.py` & `cuppa-0.9.99/cuppa/build_with_profile.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/colourise.py` & `cuppa-0.9.99/cuppa/colourise.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/configure.py` & `cuppa-0.9.99/cuppa/configure.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/construct.py` & `cuppa-0.9.99/cuppa/construct.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/core/base_options.py` & `cuppa-0.9.99/cuppa/core/base_options.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/core/environment.py` & `cuppa-0.9.99/cuppa/core/environment.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/core/location_options.py` & `cuppa-0.9.99/cuppa/core/location_options.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/core/options.py` & `cuppa-0.9.99/cuppa/core/options.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/core/storage_options.py` & `cuppa-0.9.99/cuppa/core/storage_options.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/cpp/create_version_file_cpp.py` & `cuppa-0.9.99/cuppa/cpp/create_version_file_cpp.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/cpp/run_boost_test.py` & `cuppa-0.9.99/cuppa/cpp/run_boost_test.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/cpp/run_gcov_coverage.py` & `cuppa-0.9.99/cuppa/cpp/run_gcov_coverage.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/cpp/run_patched_boost_test.py` & `cuppa-0.9.99/cuppa/cpp/run_patched_boost_test.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/cpp/run_process_test.py` & `cuppa-0.9.99/cuppa/cpp/run_process_test.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/cpp/templates/coverage_index.html` & `cuppa-0.9.99/cuppa/cpp/templates/coverage_index.html`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/b2.py` & `cuppa-0.9.99/cuppa/dependencies/boost/b2.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_bug_fix_1.73.0.diff` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_bug_fix_1.73.0.diff`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_builder.py` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_builder.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_exception.py` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_exception.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_library_methods.py` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_library_methods.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.58.0.diff` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.58.0.diff`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.67.0.diff` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.67.0.diff`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.68.0.diff` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.68.0.diff`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.71.0.diff` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.71.0.diff`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/boost_test_patch_1.72.0.diff` & `cuppa-0.9.99/cuppa/dependencies/boost/boost_test_patch_1.72.0.diff`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/configjam.py` & `cuppa-0.9.99/cuppa/dependencies/boost/configjam.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/library_dependencies.py` & `cuppa-0.9.99/cuppa/dependencies/boost/library_dependencies.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/library_naming.py` & `cuppa-0.9.99/cuppa/dependencies/boost/library_naming.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/patch_boost.py` & `cuppa-0.9.99/cuppa/dependencies/boost/patch_boost.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/boost/version_and_location.py` & `cuppa-0.9.99/cuppa/dependencies/boost/version_and_location.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/build_with_boost.py` & `cuppa-0.9.99/cuppa/dependencies/build_with_boost.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/build_with_qt4.py` & `cuppa-0.9.99/cuppa/dependencies/build_with_qt4.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/build_with_qt5.py` & `cuppa-0.9.99/cuppa/dependencies/build_with_qt5.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/dependencies/build_with_quince.py` & `cuppa-0.9.99/cuppa/dependencies/build_with_quince.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/location.py` & `cuppa-0.9.99/cuppa/location.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/log.py` & `cuppa-0.9.99/cuppa/log.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/method_helpers/run_process.py` & `cuppa-0.9.99/cuppa/method_helpers/run_process.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/asciidoc_to_html.py` & `cuppa-0.9.99/cuppa/methods/asciidoc_to_html.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/build.py` & `cuppa-0.9.99/cuppa/methods/build.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/build_library.py` & `cuppa-0.9.99/cuppa/methods/build_library.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/build_profile.py` & `cuppa-0.9.99/cuppa/methods/build_profile.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/build_test.py` & `cuppa-0.9.99/cuppa/methods/build_test.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/build_with.py` & `cuppa-0.9.99/cuppa/methods/build_with.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/compile.py` & `cuppa-0.9.99/cuppa/methods/compile.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/compile_scss.py` & `cuppa-0.9.99/cuppa/methods/compile_scss.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/copyfiles.py` & `cuppa-0.9.99/cuppa/methods/copyfiles.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/copyfilesas.py` & `cuppa-0.9.99/cuppa/methods/copyfilesas.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/coverage.py` & `cuppa-0.9.99/cuppa/methods/coverage.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/create_version.py` & `cuppa-0.9.99/cuppa/methods/create_version.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/expand_template_file.py` & `cuppa-0.9.99/cuppa/methods/expand_template_file.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/filter.py` & `cuppa-0.9.99/cuppa/methods/filter.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/markdown_to_html.py` & `cuppa-0.9.99/cuppa/methods/markdown_to_html.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/relative_recursive_glob.py` & `cuppa-0.9.99/cuppa/methods/relative_recursive_glob.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/remove_flags.py` & `cuppa-0.9.99/cuppa/methods/remove_flags.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/render_jinja_template.py` & `cuppa-0.9.99/cuppa/methods/render_jinja_template.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/replace_flags.py` & `cuppa-0.9.99/cuppa/methods/replace_flags.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/run.py` & `cuppa-0.9.99/cuppa/methods/run.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/run_and_redirect_to_file.py` & `cuppa-0.9.99/cuppa/methods/run_and_redirect_to_file.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/stdcpp.py` & `cuppa-0.9.99/cuppa/methods/stdcpp.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/target_from.py` & `cuppa-0.9.99/cuppa/methods/target_from.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/test.py` & `cuppa-0.9.99/cuppa/methods/test.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/toolchain.py` & `cuppa-0.9.99/cuppa/methods/toolchain.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/methods/using.py` & `cuppa-0.9.99/cuppa/methods/using.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/modules/registration.py` & `cuppa-0.9.99/cuppa/modules/registration.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/output.py` & `cuppa-0.9.99/cuppa/output.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/output_processor.py` & `cuppa-0.9.99/cuppa/output_processor.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/path.py` & `cuppa-0.9.99/cuppa/path.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/platforms/darwin.py` & `cuppa-0.9.99/cuppa/platforms/darwin.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/platforms/linux.py` & `cuppa-0.9.99/cuppa/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/platforms/windows.py` & `cuppa-0.9.99/cuppa/platforms/windows.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/progress.py` & `cuppa-0.9.99/cuppa/progress.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/project_generators/codeblocks.py` & `cuppa-0.9.99/cuppa/project_generators/codeblocks.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/recursive_glob.py` & `cuppa-0.9.99/cuppa/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/scms/bazaar.py` & `cuppa-0.9.99/cuppa/scms/bazaar.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/scms/git.py` & `cuppa-0.9.99/cuppa/scms/git.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/scms/mercurial.py` & `cuppa-0.9.99/cuppa/scms/mercurial.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/scms/scms.py` & `cuppa-0.9.99/cuppa/scms/scms.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/scms/subversion.py` & `cuppa-0.9.99/cuppa/scms/subversion.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/test_report/cuppa_json.py` & `cuppa-0.9.99/cuppa/test_report/cuppa_json.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/test_report/generate_bitten_report.py` & `cuppa-0.9.99/cuppa/test_report/generate_bitten_report.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/test_report/html_report.py` & `cuppa-0.9.99/cuppa/test_report/html_report.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/test_report/templates/test_report_index.html` & `cuppa-0.9.99/cuppa/test_report/templates/test_report_index.html`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/test_report/templates/test_suite_index.html` & `cuppa-0.9.99/cuppa/test_report/templates/test_suite_index.html`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/timer.py` & `cuppa-0.9.99/cuppa/timer.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/toolchains/cl.py` & `cuppa-0.9.99/cuppa/toolchains/cl.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/toolchains/clang.py` & `cuppa-0.9.99/cuppa/toolchains/clang.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/toolchains/gcc.py` & `cuppa-0.9.99/cuppa/toolchains/gcc.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/tree.py` & `cuppa-0.9.99/cuppa/tree.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/attr_tools.py` & `cuppa-0.9.99/cuppa/utility/attr_tools.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/dict_tools.py` & `cuppa-0.9.99/cuppa/utility/dict_tools.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/filter.py` & `cuppa-0.9.99/cuppa/utility/filter.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/pip_imports.py` & `cuppa-0.9.99/cuppa/utility/pip_imports.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/preprocess.py` & `cuppa-0.9.99/cuppa/utility/preprocess.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/python2to3.py` & `cuppa-0.9.99/cuppa/utility/python2to3.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/types.py` & `cuppa-0.9.99/cuppa/utility/types.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/utility/version.py` & `cuppa-0.9.99/cuppa/utility/version.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/variants/cov.py` & `cuppa-0.9.99/cuppa/variants/cov.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/variants/dbg.py` & `cuppa-0.9.99/cuppa/variants/dbg.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/variants/rel.py` & `cuppa-0.9.99/cuppa/variants/rel.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/variants/run.py` & `cuppa-0.9.99/cuppa/variants/run.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/variants/test.py` & `cuppa-0.9.99/cuppa/variants/test.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa/version.py` & `cuppa-0.9.99/cuppa/version.py`

 * *Files identical despite different names*

### Comparing `cuppa-0.9.98/cuppa.egg-info/PKG-INFO` & `cuppa-0.9.99/cuppa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuppa
-Version: 0.9.98
+Version: 0.9.99
 Summary: Cuppa, an extension package to simplify and extend Scons
 Home-page: https://github.com/ja11sop/cuppa
 Author: ja11sop
 License: Boost Software License 1.0 - http://www.boost.org/LICENSE_1_0.txt
 Keywords: scons,build,c++
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Intended Audience :: Developers
```

### Comparing `cuppa-0.9.98/cuppa.egg-info/SOURCES.txt` & `cuppa-0.9.99/cuppa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 cuppa/toolchains/__init__.py
 cuppa/toolchains/cl.py
 cuppa/toolchains/clang.py
 cuppa/toolchains/gcc.py
 cuppa/utility/__init__.py
 cuppa/utility/attr_tools.py
 cuppa/utility/dict_tools.py
+cuppa/utility/file_types.py
 cuppa/utility/filter.py
 cuppa/utility/pip_imports.py
 cuppa/utility/preprocess.py
 cuppa/utility/python2to3.py
 cuppa/utility/types.py
 cuppa/utility/version.py
 cuppa/variants/__init__.py
```

### Comparing `cuppa-0.9.98/setup.py` & `cuppa-0.9.99/setup.py`

 * *Files identical despite different names*

