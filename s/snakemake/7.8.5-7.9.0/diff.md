# Comparing `tmp/snakemake-7.8.5.tar.gz` & `tmp/snakemake-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake-7.8.5.tar", last modified: Thu Jun 30 13:21:01 2022, max compression
+gzip compressed data, was "snakemake-7.9.0.tar", last modified: Tue Jul 19 13:05:30 2022, max compression
```

## Comparing `snakemake-7.8.5.tar` & `snakemake-7.9.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.196431 snakemake-7.8.5/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 13:20:44.000000 snakemake-7.8.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-06-30 13:20:44.000000 snakemake-7.8.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-30 13:20:44.000000 snakemake-7.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-06-30 13:21:01.196431 snakemake-7.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-06-30 13:20:44.000000 snakemake-7.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-30 13:20:44.000000 snakemake-7.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-06-30 13:21:01.196431 snakemake-7.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3122 2022-06-30 13:20:44.000000 snakemake-7.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.196431 snakemake-7.8.5/snakemake/
--rw-r--r--   0 runner    (1001) docker     (121)   126904 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-30 13:21:01.196431 snakemake-7.8.5/snakemake/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    10245 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.172431 snakemake-7.8.5/snakemake/caching/
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/caching/hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/caching/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/caching/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/checkpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.172431 snakemake-7.8.5/snakemake/common/
--rw-r--r--   0 runner    (1001) docker     (121)     6487 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/common/tbdstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     8609 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/cwl.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    91042 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/dag.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.176432 snakemake-7.8.5/snakemake/deployment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32033 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/deployment/conda.py
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/deployment/containerize.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/deployment/env_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     5521 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/deployment/singularity.py
--rw-r--r--   0 runner    (1001) docker     (121)    17702 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.176432 snakemake-7.8.5/snakemake/executors/
--rw-r--r--   0 runner    (1001) docker     (121)    92813 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/executors/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    11326 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/executors/ga4gh_tes.py
--rw-r--r--   0 runner    (1001) docker     (121)    40148 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/executors/google_lifesciences.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4045 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/executors/google_lifesciences_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/executors/jobscript.sh
--rw-r--r--   0 runner    (1001) docker     (121)    13781 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/gui.html
--rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    56366 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    53902 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.176432 snakemake-7.8.5/snakemake/linting/
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/linting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/linting/links.py
--rw-r--r--   0 runner    (1001) docker     (121)     6646 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/linting/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     4730 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/linting/snakefiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    24254 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     7833 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)    10277 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/output_index.py
--rw-r--r--   0 runner    (1001) docker     (121)    34554 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/path_modifier.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18319 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.184431 snakemake-7.8.5/snakemake/remote/
--rw-r--r--   0 runner    (1001) docker     (121)    13898 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/AzBlob.py
--rw-r--r--   0 runner    (1001) docker     (121)     7405 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/EGA.py
--rw-r--r--   0 runner    (1001) docker     (121)     7407 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/FTP.py
--rw-r--r--   0 runner    (1001) docker     (121)    12178 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/GS.py
--rw-r--r--   0 runner    (1001) docker     (121)     9803 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/HTTP.py
--rw-r--r--   0 runner    (1001) docker     (121)    28921 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/NCBI.py
--rw-r--r--   0 runner    (1001) docker     (121)    12747 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/S3.py
--rw-r--r--   0 runner    (1001) docker     (121)     4405 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/S3Mocked.py
--rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/SFTP.py
--rw-r--r--   0 runner    (1001) docker     (121)     9219 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/XRootD.py
--rw-r--r--   0 runner    (1001) docker     (121)    16009 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5789 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     4923 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/gfal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/gridftp.py
--rw-r--r--   0 runner    (1001) docker     (121)     9233 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/iRODS.py
--rw-r--r--   0 runner    (1001) docker     (121)     7448 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/webdav.py
--rw-r--r--   0 runner    (1001) docker     (121)     8544 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/remote/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.184431 snakemake-7.8.5/snakemake/report/
--rw-r--r--   0 runner    (1001) docker     (121)    29705 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.184431 snakemake-7.8.5/snakemake/report/data/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/categories.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/results.py
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/rulegraph.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/runtimes.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/data/timeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/rulegraph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.188432 snakemake-7.8.5/snakemake/report/template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.192432 snakemake-7.8.5/snakemake/report/template/components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/abstract_menu.js
--rw-r--r--   0 runner    (1001) docker     (121)     4256 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/abstract_results.js
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/app.js
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/breadcrumbs.js
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/button.js
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/category.js
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/common.js
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/content.js
--rw-r--r--   0 runner    (1001) docker     (121)     3925 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/icon.js
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/list_heading.js
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/list_item.js
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/menu.js
--rw-r--r--   0 runner    (1001) docker     (121)     9271 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/navbar.js
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/report_info.js
--rw-r--r--   0 runner    (1001) docker     (121)     6736 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/result_info.js
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/result_view_button.js
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/rule_graph.js
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/rule_info.js
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/search_results.js
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/stats.js
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/components/subcategory.js
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/index.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report/template/style.css
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/report.css
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/ruleinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)    47164 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)    33673 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)    43917 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/script.py
--rw-r--r--   0 runner    (1001) docker     (121)    11707 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)    12341 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/sourcecache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.192432 snakemake-7.8.5/snakemake/template_rendering/
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/template_rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/template_rendering/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/template_rendering/yte.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.192432 snakemake-7.8.5/snakemake/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4051 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.196431 snakemake-7.8.5/snakemake/unit_tests/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/unit_tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/unit_tests/templates/common.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/unit_tests/templates/ruletest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)    26562 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    71910 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-06-30 13:20:44.000000 snakemake-7.8.5/snakemake/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 13:21:01.172431 snakemake-7.8.5/snakemake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-06-30 13:21:00.000000 snakemake-7.8.5/snakemake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-06-30 13:21:01.000000 snakemake-7.8.5/snakemake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 13:21:00.000000 snakemake-7.8.5/snakemake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-06-30 13:21:00.000000 snakemake-7.8.5/snakemake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 13:20:58.000000 snakemake-7.8.5/snakemake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-06-30 13:21:00.000000 snakemake-7.8.5/snakemake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-30 13:21:01.000000 snakemake-7.8.5/snakemake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    68615 2022-06-30 13:20:44.000000 snakemake-7.8.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.536160 snakemake-7.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:08.000000 snakemake-7.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-07-19 13:05:08.000000 snakemake-7.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-19 13:05:08.000000 snakemake-7.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-07-19 13:05:30.536160 snakemake-7.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-07-19 13:05:08.000000 snakemake-7.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-19 13:05:08.000000 snakemake-7.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-07-19 13:05:30.536160 snakemake-7.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3122 2022-07-19 13:05:08.000000 snakemake-7.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.536160 snakemake-7.9.0/snakemake/
+-rw-r--r--   0 runner    (1001) docker     (121)   126904 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-19 13:05:30.536160 snakemake-7.9.0/snakemake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10245 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.512160 snakemake-7.9.0/snakemake/caching/
+-rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/caching/hash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/caching/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/caching/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/checkpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.512160 snakemake-7.9.0/snakemake/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     6487 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/common/tbdstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8609 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/cwl.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    91042 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/dag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.516160 snakemake-7.9.0/snakemake/deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32033 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/deployment/conda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/deployment/containerize.py
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/deployment/env_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5521 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/deployment/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17702 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.516160 snakemake-7.9.0/snakemake/executors/
+-rw-r--r--   0 runner    (1001) docker     (121)    92813 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/executors/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11326 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/executors/ga4gh_tes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40148 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/executors/google_lifesciences.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4045 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/executors/google_lifesciences_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/executors/jobscript.sh
+-rw-r--r--   0 runner    (1001) docker     (121)    13781 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/gui.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    56366 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53902 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.516160 snakemake-7.9.0/snakemake/linting/
+-rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/linting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/linting/links.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6646 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/linting/rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4730 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/linting/snakefiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24254 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8163 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10277 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/output_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35897 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4278 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/path_modifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    19113 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.524160 snakemake-7.9.0/snakemake/remote/
+-rw-r--r--   0 runner    (1001) docker     (121)    13898 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/AzBlob.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7405 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/EGA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7407 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/FTP.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12178 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/GS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9803 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/HTTP.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28921 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/NCBI.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12747 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/S3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4405 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/S3Mocked.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/SFTP.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9219 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/XRootD.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16009 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5789 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4923 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/gfal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/gridftp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9233 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/iRODS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7448 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8544 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/remote/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.524160 snakemake-7.9.0/snakemake/report/
+-rw-r--r--   0 runner    (1001) docker     (121)    29705 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.524160 snakemake-7.9.0/snakemake/report/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/packages.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/results.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/rulegraph.py
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/runtimes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/data/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/rulegraph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.528160 snakemake-7.9.0/snakemake/report/template/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.532160 snakemake-7.9.0/snakemake/report/template/components/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/abstract_menu.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4256 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/abstract_results.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/app.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/breadcrumbs.js
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/button.js
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/category.js
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/common.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/content.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3925 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/icon.js
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/list_heading.js
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/list_item.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/menu.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9271 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/navbar.js
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/report_info.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6736 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/result_info.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/result_view_button.js
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/rule_graph.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/rule_info.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/search_results.js
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/stats.js
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/components/subcategory.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/index.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report/template/style.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/report.css
+-rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/ruleinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47164 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33673 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44232 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/script.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11707 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/shell.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12341 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/sourcecache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.536160 snakemake-7.9.0/snakemake/template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/template_rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/template_rendering/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/template_rendering/yte.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.536160 snakemake-7.9.0/snakemake/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     4051 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.536160 snakemake-7.9.0/snakemake/unit_tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/unit_tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/unit_tests/templates/common.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/unit_tests/templates/ruletest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (121)    26562 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    72034 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-07-19 13:05:08.000000 snakemake-7.9.0/snakemake/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 13:05:30.512160 snakemake-7.9.0/snakemake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-07-19 13:05:30.000000 snakemake-7.9.0/snakemake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-07-19 13:05:30.000000 snakemake-7.9.0/snakemake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 13:05:30.000000 snakemake-7.9.0/snakemake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-07-19 13:05:30.000000 snakemake-7.9.0/snakemake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 13:05:30.000000 snakemake-7.9.0/snakemake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-19 13:05:30.000000 snakemake-7.9.0/snakemake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-07-19 13:05:30.000000 snakemake-7.9.0/snakemake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    68615 2022-07-19 13:05:08.000000 snakemake-7.9.0/versioneer.py
```

### Comparing `snakemake-7.8.5/LICENSE.md` & `snakemake-7.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/PKG-INFO` & `snakemake-7.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake
-Version: 7.8.5
+Version: 7.9.0
 Summary: Snakemake is a workflow management system that aims to reduce the complexity of creating workflows by providing a fast and comfortable execution environment, together with a clean and modern specification language in python style. Snakemake workflows are essentially Python scripts extended by declarative code to define rules. Rules describe how to create output files from input files.
 Home-page: https://snakemake.readthedocs.io
 Author: Johannes Köster
 Author-email: johannes.koester@tu-dortmund.de
 License: MIT
 Project-URL: Source, https://github.com/snakemake/snakemake
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `snakemake-7.8.5/README.md` & `snakemake-7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/setup.py` & `snakemake-7.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/__init__.py` & `snakemake-7.9.0/snakemake/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2440,18 +2440,14 @@
             file=sys.stderr,
         )
         exit(1)
 
     parser = get_argument_parser()
     args = parser.parse_args(argv)
 
-    if args.quiet is not None and len(args.quiet) == 0:
-        # default case, set quiet to progress and rule
-        args.quiet = ["progress", "rules"]
-
     if args.profile:
         # reparse args while inferring config file from profile
         parser = get_argument_parser(args.profile)
         args = parser.parse_args(argv)
 
         def adjust_path(f):
             if os.path.exists(f) or os.path.isabs(f):
@@ -2474,14 +2470,18 @@
             args.cluster_sync = adjust_path(args.cluster_sync)
         for key in "cluster_status", "cluster_cancel", "cluster_sidecar":
             if getattr(args, key):
                 setattr(args, key, adjust_path(getattr(args, key)))
         if args.report_stylesheet:
             args.report_stylesheet = adjust_path(args.report_stylesheet)
 
+    if args.quiet is not None and len(args.quiet) == 0:
+        # default case, set quiet to progress and rule
+        args.quiet = ["progress", "rules"]
+
     if args.bash_completion:
         cmd = b"complete -o bashdefault -C snakemake-bash-completion snakemake"
         sys.stdout.buffer.write(cmd)
         sys.exit(0)
 
     if args.batch is not None and args.forceall:
         print(
```

### Comparing `snakemake-7.8.5/snakemake/benchmark.py` & `snakemake-7.9.0/snakemake/benchmark.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/caching/__init__.py` & `snakemake-7.9.0/snakemake/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/caching/hash.py` & `snakemake-7.9.0/snakemake/caching/hash.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/caching/local.py` & `snakemake-7.9.0/snakemake/caching/local.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/caching/remote.py` & `snakemake-7.9.0/snakemake/caching/remote.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/checkpoints.py` & `snakemake-7.9.0/snakemake/checkpoints.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/common/__init__.py` & `snakemake-7.9.0/snakemake/common/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/common/tbdstring.py` & `snakemake-7.9.0/snakemake/common/tbdstring.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/cwl.py` & `snakemake-7.9.0/snakemake/cwl.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/dag.py` & `snakemake-7.9.0/snakemake/dag.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/deployment/conda.py` & `snakemake-7.9.0/snakemake/deployment/conda.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/deployment/containerize.py` & `snakemake-7.9.0/snakemake/deployment/containerize.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/deployment/env_modules.py` & `snakemake-7.9.0/snakemake/deployment/env_modules.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/deployment/singularity.py` & `snakemake-7.9.0/snakemake/deployment/singularity.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/exceptions.py` & `snakemake-7.9.0/snakemake/exceptions.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/executors/__init__.py` & `snakemake-7.9.0/snakemake/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/executors/common.py` & `snakemake-7.9.0/snakemake/executors/common.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/executors/ga4gh_tes.py` & `snakemake-7.9.0/snakemake/executors/ga4gh_tes.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/executors/google_lifesciences.py` & `snakemake-7.9.0/snakemake/executors/google_lifesciences.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/executors/google_lifesciences_helper.py` & `snakemake-7.9.0/snakemake/executors/google_lifesciences_helper.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/gui.html` & `snakemake-7.9.0/snakemake/gui.html`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/gui.py` & `snakemake-7.9.0/snakemake/gui.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/io.py` & `snakemake-7.9.0/snakemake/io.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/jobs.py` & `snakemake-7.9.0/snakemake/jobs.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/linting/__init__.py` & `snakemake-7.9.0/snakemake/linting/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/linting/links.py` & `snakemake-7.9.0/snakemake/linting/links.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/linting/rules.py` & `snakemake-7.9.0/snakemake/linting/rules.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/linting/snakefiles.py` & `snakemake-7.9.0/snakemake/linting/snakefiles.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/logging.py` & `snakemake-7.9.0/snakemake/logging.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/modules.py` & `snakemake-7.9.0/snakemake/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,25 +69,27 @@
         self.replace_prefix = replace_prefix
         self.prefix = prefix
 
     def use_rules(
         self,
         rules=None,
         name_modifier=None,
+        exclude_rules=None,
         ruleinfo=None,
         skip_global_report_caption=False,
     ):
         snakefile = self.get_snakefile()
         with WorkflowModifier(
             self.workflow,
             config=self.config,
             base_snakefile=snakefile,
             skip_configfile=self.config is not None,
             skip_validation=self.skip_validation,
             skip_global_report_caption=skip_global_report_caption,
+            rule_exclude_list=exclude_rules,
             rule_whitelist=self.get_rule_whitelist(rules),
             rulename_modifier=get_name_modifier_func(rules, name_modifier),
             ruleinfo_overwrite=ruleinfo,
             allow_rule_overwrite=True,
             namespace=self.name,
             replace_prefix=self.replace_prefix,
             prefix=self.prefix,
@@ -136,14 +138,15 @@
         config=None,
         base_snakefile=None,
         skip_configfile=False,
         skip_validation=False,
         skip_global_report_caption=False,
         rulename_modifier=None,
         rule_whitelist=None,
+        rule_exclude_list=None,
         ruleinfo_overwrite=None,
         allow_rule_overwrite=False,
         replace_prefix=None,
         prefix=None,
         replace_wrapper_tag=None,
         namespace=None,
     ):
@@ -152,14 +155,15 @@
             self.base_snakefile = parent_modifier.base_snakefile
             self.globals = parent_modifier.globals
             self.skip_configfile = parent_modifier.skip_configfile
             self.rulename_modifier = parent_modifier.rulename_modifier
             self.skip_validation = parent_modifier.skip_validation
             self.skip_global_report_caption = parent_modifier.skip_global_report_caption
             self.rule_whitelist = parent_modifier.rule_whitelist
+            self.rule_exclude_list = parent_modifier.rule_exclude_list
             self.ruleinfo_overwrite = parent_modifier.ruleinfo_overwrite
             self.allow_rule_overwrite = parent_modifier.allow_rule_overwrite
             self.path_modifier = parent_modifier.path_modifier
             self.replace_wrapper_tag = parent_modifier.replace_wrapper_tag
             self.namespace = parent_modifier.namespace
         else:
             # default settings for globals if not inheriting from parent
@@ -174,22 +178,25 @@
             self.globals["config"] = config
 
         self.skip_configfile = skip_configfile
         self.rulename_modifier = rulename_modifier
         self.skip_validation = skip_validation
         self.skip_global_report_caption = skip_global_report_caption
         self.rule_whitelist = rule_whitelist
+        self.rule_exclude_list = rule_exclude_list
         self.ruleinfo_overwrite = ruleinfo_overwrite
         self.allow_rule_overwrite = allow_rule_overwrite
         self.path_modifier = PathModifier(replace_prefix, prefix, workflow)
         self.replace_wrapper_tag = replace_wrapper_tag
         self.namespace = namespace
 
     def skip_rule(self, rulename):
-        return self.rule_whitelist is not None and rulename not in self.rule_whitelist
+        return (
+            self.rule_whitelist is not None and rulename not in self.rule_whitelist
+        ) or (self.rule_exclude_list is not None and rulename in self.rule_exclude_list)
 
     def modify_rulename(self, rulename):
         if self.rulename_modifier is not None:
             return self.rulename_modifier(rulename)
         return rulename
 
     def modify_path(self, path, property=None):
```

### Comparing `snakemake-7.8.5/snakemake/notebook.py` & `snakemake-7.9.0/snakemake/notebook.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/output_index.py` & `snakemake-7.9.0/snakemake/output_index.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/parser.py` & `snakemake-7.9.0/snakemake/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -943,24 +943,25 @@
 class UseRule(GlobalKeywordState):
     subautomata = rule_property_subautomata
 
     def __init__(self, snakefile, base_indent=0, dedent=0, root=True):
         super().__init__(snakefile, base_indent=base_indent, dedent=dedent, root=root)
         self.state = self.state_keyword_rule
         self.rules = []
+        self.exclude_rules = []
         self.has_with = False
         self.name_modifier = []
         self.from_module = None
         self._with_block = []
         self.lineno = self.snakefile.lines + 1
 
     def end(self):
         name_modifier = "".join(self.name_modifier) if self.name_modifier else None
-        yield "@workflow.userule(rules={!r}, from_module={!r}, name_modifier={!r}, lineno={})".format(
-            self.rules, self.from_module, name_modifier, self.lineno
+        yield "@workflow.userule(rules={!r}, from_module={!r}, exclude_rules={!r}, name_modifier={!r}, lineno={})".format(
+            self.rules, self.from_module, self.exclude_rules, name_modifier, self.lineno
         )
         yield "\n"
 
         if self._with_block:
             # yield with block
             yield from self._with_block
 
@@ -1056,14 +1057,17 @@
             )
 
     def state_modifier(self, token):
         if is_name(token):
             if token.string == "as" and not self.name_modifier:
                 self.state = self.state_as
                 yield from ()
+            elif token.string == "exclude":
+                self.state = self.state_exclude
+                yield from ()
             elif token.string == "with":
                 yield from self.handle_with(token)
             else:
                 self.error(
                     "Expecting at most one 'as' or 'with' statement, or the end of the line.",
                     token,
                 )
@@ -1107,17 +1111,51 @@
 
     def state_with(self, token):
         if is_colon(token):
             self.state = self.block
             yield from ()
         else:
             self.error(
-                "Expecting colon after 'with' keyword in 'use rule' statement.", token
+                "Expecting colon after 'with' keyword in 'use rule' statement.",
+                token,
             )
 
+    def state_exclude(self, token):
+        if is_name(token):
+            self.exclude_rules.append(token.string)
+            self.state = self.state_exclude_comma_or_end
+            yield from ()
+        else:
+            self.error(
+                "Expecting rule name(s) after 'exclude' keyword in 'use rule' statement.",
+                token,
+            )
+
+    def state_exclude_comma_or_end(self, token):
+        if is_name(token):
+            if token.string == "from" or token.string == "as":
+                if not self.exclude_rules:
+                    self.error(
+                        "Expecting rule names after 'exclude' statement.",
+                        token,
+                    )
+                if token.string == "from":
+                    self.state = self.state_from
+                else:
+                    self.state = self.state_as
+                yield from ()
+            else:
+                yield from ()
+        elif is_comma(token):
+            self.state = self.state_exclude
+            yield from ()
+        else:
+            self.state = self.state_modifier
+            yield from ()
+
     def block_content(self, token):
         if is_comment(token):
             yield "\n", token
             yield token.string, token
         elif is_name(token):
             try:
                 self._with_block.extend(self.subautomaton(token.string).consume())
```

### Comparing `snakemake-7.8.5/snakemake/path_modifier.py` & `snakemake-7.9.0/snakemake/path_modifier.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/persistence.py` & `snakemake-7.9.0/snakemake/persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import os
 import shutil
 import signal
 import marshal
 import pickle
 import json
+import tempfile
 import time
 from base64 import urlsafe_b64encode, b64encode
 from functools import lru_cache, partial
 from itertools import filterfalse, count
 from pathlib import Path
 
 import snakemake.exceptions
@@ -430,17 +431,28 @@
 
     @lru_cache()
     def _output(self, job):
         return sorted(job.output)
 
     def _record(self, subject, json_value, id):
         recpath = self._record_path(subject, id)
-        os.makedirs(os.path.dirname(recpath), exist_ok=True)
-        with open(recpath, "w") as f:
-            json.dump(json_value, f)
+        recdir = os.path.dirname(recpath)
+        os.makedirs(recdir, exist_ok=True)
+        # Write content to temporary file and rename it to the final file.
+        # This avoids race-conditions while writing (e.g. on NFS when the main job
+        # and the cluster node job propagate their content and the system has some
+        # latency including non-atomic propagation processes).
+        with tempfile.NamedTemporaryFile(
+            mode="w",
+            dir=recdir,
+            delete=False,
+            suffix=os.path.basename(recpath),
+        ) as tmpfile:
+            json.dump(json_value, tmpfile)
+        os.rename(tmpfile.name, recpath)
 
     def _delete_record(self, subject, id):
         try:
             recpath = self._record_path(subject, id)
             os.remove(recpath)
             recdirs = os.path.relpath(os.path.dirname(recpath), start=subject)
             if recdirs != ".":
@@ -458,15 +470,22 @@
     def _read_record_cached(self, subject, id):
         return self._read_record_uncached(subject, id)
 
     def _read_record_uncached(self, subject, id):
         if not self._exists_record(subject, id):
             return dict()
         with open(self._record_path(subject, id), "r") as f:
-            return json.load(f)
+            try:
+                return json.load(f)
+            except json.JSONDecodeError as e:
+                pass
+        # case: file is corrupted, delete it
+        logger.warning(f"Deleting corrupted metadata record.")
+        self._delete_record(subject, id)
+        return dict()
 
     def _exists_record(self, subject, id):
         return os.path.exists(self._record_path(subject, id))
 
     def _locks(self, type):
         return (
             f
```

### Comparing `snakemake-7.8.5/snakemake/remote/AzBlob.py` & `snakemake-7.9.0/snakemake/remote/AzBlob.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/EGA.py` & `snakemake-7.9.0/snakemake/remote/EGA.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/FTP.py` & `snakemake-7.9.0/snakemake/remote/FTP.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/GS.py` & `snakemake-7.9.0/snakemake/remote/GS.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/HTTP.py` & `snakemake-7.9.0/snakemake/remote/HTTP.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/NCBI.py` & `snakemake-7.9.0/snakemake/remote/NCBI.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/S3.py` & `snakemake-7.9.0/snakemake/remote/S3.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/S3Mocked.py` & `snakemake-7.9.0/snakemake/remote/S3Mocked.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/SFTP.py` & `snakemake-7.9.0/snakemake/remote/SFTP.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/XRootD.py` & `snakemake-7.9.0/snakemake/remote/XRootD.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/__init__.py` & `snakemake-7.9.0/snakemake/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/dropbox.py` & `snakemake-7.9.0/snakemake/remote/dropbox.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/gfal.py` & `snakemake-7.9.0/snakemake/remote/gfal.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/gridftp.py` & `snakemake-7.9.0/snakemake/remote/gridftp.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/iRODS.py` & `snakemake-7.9.0/snakemake/remote/iRODS.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/webdav.py` & `snakemake-7.9.0/snakemake/remote/webdav.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/remote/zenodo.py` & `snakemake-7.9.0/snakemake/remote/zenodo.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/__init__.py` & `snakemake-7.9.0/snakemake/report/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/data/common.py` & `snakemake-7.9.0/snakemake/report/data/common.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/data/packages.py` & `snakemake-7.9.0/snakemake/report/data/packages.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/data/results.py` & `snakemake-7.9.0/snakemake/report/data/results.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/data/rulegraph.py` & `snakemake-7.9.0/snakemake/report/data/rulegraph.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/data/runtimes.py` & `snakemake-7.9.0/snakemake/report/data/runtimes.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/data/timeline.py` & `snakemake-7.9.0/snakemake/report/data/timeline.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/rulegraph_spec.py` & `snakemake-7.9.0/snakemake/report/rulegraph_spec.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/abstract_menu.js` & `snakemake-7.9.0/snakemake/report/template/components/abstract_menu.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/abstract_results.js` & `snakemake-7.9.0/snakemake/report/template/components/abstract_results.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/app.js` & `snakemake-7.9.0/snakemake/report/template/components/app.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/breadcrumbs.js` & `snakemake-7.9.0/snakemake/report/template/components/breadcrumbs.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/category.js` & `snakemake-7.9.0/snakemake/report/template/components/category.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/content.js` & `snakemake-7.9.0/snakemake/report/template/components/content.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/icon.js` & `snakemake-7.9.0/snakemake/report/template/components/icon.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/menu.js` & `snakemake-7.9.0/snakemake/report/template/components/menu.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/navbar.js` & `snakemake-7.9.0/snakemake/report/template/components/navbar.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/report_info.js` & `snakemake-7.9.0/snakemake/report/template/components/report_info.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/result_info.js` & `snakemake-7.9.0/snakemake/report/template/components/result_info.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/result_view_button.js` & `snakemake-7.9.0/snakemake/report/template/components/result_view_button.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/rule_graph.js` & `snakemake-7.9.0/snakemake/report/template/components/rule_graph.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/rule_info.js` & `snakemake-7.9.0/snakemake/report/template/components/rule_info.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/search_results.js` & `snakemake-7.9.0/snakemake/report/template/components/search_results.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/components/stats.js` & `snakemake-7.9.0/snakemake/report/template/components/stats.js`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/index.html.jinja2` & `snakemake-7.9.0/snakemake/report/template/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/logo.svg` & `snakemake-7.9.0/snakemake/report/template/logo.svg`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report/template/style.css` & `snakemake-7.9.0/snakemake/report/template/style.css`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/report.css` & `snakemake-7.9.0/snakemake/report.css`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/resources.py` & `snakemake-7.9.0/snakemake/resources.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/ruleinfo.py` & `snakemake-7.9.0/snakemake/ruleinfo.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/rules.py` & `snakemake-7.9.0/snakemake/rules.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/scheduler.py` & `snakemake-7.9.0/snakemake/scheduler.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/script.py` & `snakemake-7.9.0/snakemake/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     def encode_numeric(cls, value):
         if value is None:
             return "as.numeric(NA)"
         return str(value)
 
     @classmethod
     def encode_value(cls, value):
+
         if value is None:
             return "NULL"
         elif isinstance(value, str):
             return repr(value)
         elif isinstance(value, Path):
             return repr(str(value))
         elif isinstance(value, dict):
@@ -198,14 +199,17 @@
         else:
             # Try to convert from numpy if numpy is present
             try:
                 import numpy as np
 
                 if isinstance(value, np.number):
                     return str(value)
+                elif isinstance(value, np.bool_):
+                    return "TRUE" if value else "FALSE"
+
             except ImportError:
                 pass
         raise ValueError("Unsupported value for conversion into R: {}".format(value))
 
     @classmethod
     def encode_list(cls, l):
         return "c({})".format(", ".join(map(cls.encode_value, l)))
@@ -528,21 +532,26 @@
         )
 
     def write_script(self, preamble, fd):
         fd.write(preamble.encode())
         fd.write(self.source.encode())
 
     def _is_python_env(self):
-        if self.conda_env is not None:
+        if self.conda_env is not None and ON_WINDOWS:
+            prefix = self.conda_env
+        elif self.conda_env is not None:
             prefix = os.path.join(self.conda_env, "bin")
         elif self.env_modules is not None:
             prefix = self._execute_cmd("echo $PATH", read=True).split(":")[0]
         else:
             raise NotImplementedError()
-        return os.path.exists(os.path.join(prefix, "python"))
+        if not ON_WINDOWS:
+            return os.path.exists(os.path.join(prefix, "python"))
+        else:
+            return os.path.exists(os.path.join(prefix, "python.exe"))
 
     def _get_python_version(self):
         out = self._execute_cmd(
             "python -c \"import sys; print('.'.join(map(str, sys.version_info[:2])))\"",
             read=True,
         )
         return tuple(map(int, out.strip().split(".")))
```

### Comparing `snakemake-7.8.5/snakemake/shell.py` & `snakemake-7.9.0/snakemake/shell.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/sourcecache.py` & `snakemake-7.9.0/snakemake/sourcecache.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/stats.py` & `snakemake-7.9.0/snakemake/stats.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/template_rendering/__init__.py` & `snakemake-7.9.0/snakemake/template_rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/template_rendering/jinja2.py` & `snakemake-7.9.0/snakemake/template_rendering/jinja2.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/unit_tests/__init__.py` & `snakemake-7.9.0/snakemake/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/unit_tests/templates/common.py.jinja2` & `snakemake-7.9.0/snakemake/unit_tests/templates/common.py.jinja2`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/unit_tests/templates/ruletest.py.jinja2` & `snakemake-7.9.0/snakemake/unit_tests/templates/ruletest.py.jinja2`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/utils.py` & `snakemake-7.9.0/snakemake/utils.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake/workflow.py` & `snakemake-7.9.0/snakemake/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1937,28 +1937,36 @@
             meta_wrapper=meta_wrapper,
             config=config,
             skip_validation=skip_validation,
             replace_prefix=replace_prefix,
             prefix=prefix,
         )
 
-    def userule(self, rules=None, from_module=None, name_modifier=None, lineno=None):
+    def userule(
+        self,
+        rules=None,
+        from_module=None,
+        exclude_rules=None,
+        name_modifier=None,
+        lineno=None,
+    ):
         def decorate(maybe_ruleinfo):
             if from_module is not None:
                 try:
                     module = self.modules[from_module]
                 except KeyError:
                     raise WorkflowError(
                         "Module {} has not been registered with 'module' statement before using it in 'use rule' statement.".format(
                             from_module
                         )
                     )
                 module.use_rules(
                     rules,
                     name_modifier,
+                    exclude_rules=exclude_rules,
                     ruleinfo=None if callable(maybe_ruleinfo) else maybe_ruleinfo,
                     skip_global_report_caption=self.report_text
                     is not None,  # do not overwrite existing report text via module
                 )
             else:
                 # local inheritance
                 if self.modifier.skip_rule(name_modifier):
```

### Comparing `snakemake-7.8.5/snakemake/wrapper.py` & `snakemake-7.9.0/snakemake/wrapper.py`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/snakemake.egg-info/PKG-INFO` & `snakemake-7.9.0/snakemake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake
-Version: 7.8.5
+Version: 7.9.0
 Summary: Snakemake is a workflow management system that aims to reduce the complexity of creating workflows by providing a fast and comfortable execution environment, together with a clean and modern specification language in python style. Snakemake workflows are essentially Python scripts extended by declarative code to define rules. Rules describe how to create output files from input files.
 Home-page: https://snakemake.readthedocs.io
 Author: Johannes Köster
 Author-email: johannes.koester@tu-dortmund.de
 License: MIT
 Project-URL: Source, https://github.com/snakemake/snakemake
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `snakemake-7.8.5/snakemake.egg-info/SOURCES.txt` & `snakemake-7.9.0/snakemake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snakemake-7.8.5/versioneer.py` & `snakemake-7.9.0/versioneer.py`

 * *Files identical despite different names*

