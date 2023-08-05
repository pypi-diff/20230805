# Comparing `tmp/CairoSVG-2.7.0.tar.gz` & `tmp/CairoSVG-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CairoSVG-2.7.0.tar", last modified: Mon Mar 20 14:32:52 2023, max compression
+gzip compressed data, was "CairoSVG-2.7.1.tar", last modified: Sat Aug  5 09:02:26 2023, max compression
```

## Comparing `CairoSVG-2.7.0.tar` & `CairoSVG-2.7.1.tar`

### file list

```diff
@@ -1,1300 +1,1300 @@
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.550481 CairoSVG-2.7.0/
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.314477 CairoSVG-2.7.0/.github/
--rw-r--r--   0 lize      (1000) lize      (1000)       78 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/.github/FUNDING.yml
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.314477 CairoSVG-2.7.0/.github/workflows/
--rw-r--r--   0 lize      (1000) lize      (1000)     1075 2023-03-20 14:31:13.000000 CairoSVG-2.7.0/.github/workflows/tests.yml
--rw-r--r--   0 lize      (1000) lize      (1000)      107 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/.gitignore
--rw-r--r--   0 lize      (1000) lize      (1000)       95 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/.gitmodules
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.315477 CairoSVG-2.7.0/CairoSVG.egg-info/
--rw-r--r--   0 lize      (1000) lize      (1000)     2393 2023-03-20 14:32:52.000000 CairoSVG-2.7.0/CairoSVG.egg-info/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)    64093 2023-03-20 14:32:52.000000 CairoSVG-2.7.0/CairoSVG.egg-info/SOURCES.txt
--rw-r--r--   0 lize      (1000) lize      (1000)        1 2023-03-20 14:32:52.000000 CairoSVG-2.7.0/CairoSVG.egg-info/dependency_links.txt
--rw-r--r--   0 lize      (1000) lize      (1000)       52 2023-03-20 14:32:52.000000 CairoSVG-2.7.0/CairoSVG.egg-info/entry_points.txt
--rw-r--r--   0 lize      (1000) lize      (1000)      107 2023-03-20 14:32:52.000000 CairoSVG-2.7.0/CairoSVG.egg-info/requires.txt
--rw-r--r--   0 lize      (1000) lize      (1000)        9 2023-03-20 14:32:52.000000 CairoSVG-2.7.0/CairoSVG.egg-info/top_level.txt
--rw-r--r--   0 lize      (1000) lize      (1000)     7650 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/LICENSE
--rw-r--r--   0 lize      (1000) lize      (1000)    11328 2023-03-20 14:31:13.000000 CairoSVG-2.7.0/NEWS.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     2393 2023-03-20 14:32:52.550481 CairoSVG-2.7.0/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)     1056 2023-01-12 16:45:06.000000 CairoSVG-2.7.0/README.rst
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.318477 CairoSVG-2.7.0/cairosvg/
--rw-r--r--   0 lize      (1000) lize      (1000)        5 2023-03-20 14:31:13.000000 CairoSVG-2.7.0/cairosvg/VERSION
--rw-r--r--   0 lize      (1000) lize      (1000)     4799 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/__init__.py
--rw-r--r--   0 lize      (1000) lize      (1000)     3045 2023-03-20 14:31:13.000000 CairoSVG-2.7.0/cairosvg/__main__.py
--rw-r--r--   0 lize      (1000) lize      (1000)    13988 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/bounding_box.py
--rw-r--r--   0 lize      (1000) lize      (1000)    10672 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/colors.py
--rw-r--r--   0 lize      (1000) lize      (1000)     4029 2023-03-20 14:29:52.000000 CairoSVG-2.7.0/cairosvg/css.py
--rw-r--r--   0 lize      (1000) lize      (1000)    13674 2022-12-27 11:44:40.000000 CairoSVG-2.7.0/cairosvg/defs.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1572 2023-01-12 16:37:55.000000 CairoSVG-2.7.0/cairosvg/features.py
--rw-r--r--   0 lize      (1000) lize      (1000)    12715 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/helpers.py
--rw-r--r--   0 lize      (1000) lize      (1000)     4051 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/image.py
--rw-r--r--   0 lize      (1000) lize      (1000)    16202 2023-03-20 14:31:13.000000 CairoSVG-2.7.0/cairosvg/parser.py
--rw-r--r--   0 lize      (1000) lize      (1000)    17067 2023-03-05 08:28:56.000000 CairoSVG-2.7.0/cairosvg/path.py
--rw-r--r--   0 lize      (1000) lize      (1000)     3432 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/shapes.py
--rw-r--r--   0 lize      (1000) lize      (1000)    20834 2023-03-20 14:31:13.000000 CairoSVG-2.7.0/cairosvg/surface.py
--rw-r--r--   0 lize      (1000) lize      (1000)      272 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/svg.py
--rw-r--r--   0 lize      (1000) lize      (1000)     6938 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/test_api.py
--rw-r--r--   0 lize      (1000) lize      (1000)     9769 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/text.py
--rw-r--r--   0 lize      (1000) lize      (1000)     4743 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/cairosvg/url.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1843 2023-03-20 14:32:52.550481 CairoSVG-2.7.0/setup.cfg
--rwxr-xr-x   0 lize      (1000) lize      (1000)      574 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/setup.py
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.318477 CairoSVG-2.7.0/test_non_regression/
--rw-r--r--   0 lize      (1000) lize      (1000)     1592 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/LICENSE
--rw-r--r--   0 lize      (1000) lize      (1000)     1323 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/test_non_regression/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)      934 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/test_non_regression/__init__.py
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.318477 CairoSVG-2.7.0/test_non_regression/fail/
--rw-r--r--   0 lize      (1000) lize      (1000)      508 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/README.rst
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.319477 CairoSVG-2.7.0/test_non_regression/fail/cap/
--rw-r--r--   0 lize      (1000) lize      (1000)      346 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/cap/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     5998 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/cap/painting-control-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2938 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/cap/painting-control-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11044 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/cap/painting-stroke-10-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3559 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/cap/painting-stroke-10-t.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.321477 CairoSVG-2.7.0/test_non_regression/fail/color/
--rw-r--r--   0 lize      (1000) lize      (1000)      148 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/color/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     6677 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/color/color-prof-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3965 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/color/color-prof-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14587 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8956 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9867 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4742 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-02-b.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.321477 CairoSVG-2.7.0/test_non_regression/fail/css/
--rw-r--r--   0 lize      (1000) lize      (1000)       82 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/css/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     3406 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/css/struct-use-04-b.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.322477 CairoSVG-2.7.0/test_non_regression/fail/draft/
--rw-r--r--   0 lize      (1000) lize      (1000)      816 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/draft/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     6039 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/draft/painting-marker-properties-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4618 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/draft/painting-marker-properties-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6858 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/draft/paths-data-20-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4243 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/draft/paths-data-20-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23588 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/draft/types-basic-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4413 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/draft/types-basic-02-f.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.345477 CairoSVG-2.7.0/test_non_regression/fail/filter/
--rw-r--r--   0 lize      (1000) lize      (1000)     1717 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     9655 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/enable-background-01.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3701 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/enable-background-01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7578 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feColorMatrix.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2585 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feColorMatrix.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6366 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feComponentTransfer.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2875 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feComponentTransfer.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14985 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feComposite.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9265 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feComposite.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5449 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feMorphology.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1525 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feMorphology.svg
--rw-r--r--   0 lize      (1000) lize      (1000)   139525 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feTurbulence.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3221 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/feTurbulence.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18824 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-background-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8520 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-background-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16420 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-blend-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6769 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-blend-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24542 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6533 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7439 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5593 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16884 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9284 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6192 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4521 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)   127777 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4314 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    35393 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-05-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3530 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16794 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-comptran-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6826 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-comptran-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    53536 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6835 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    38250 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4243 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    34066 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5246 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    87653 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8527 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13705 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-05-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4305 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21863 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-diffuse-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8988 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-diffuse-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    45323 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7173 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8965 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5267 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    22359 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-example-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5037 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-example-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12696 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4743 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16264 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6255 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19453 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4927 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8057 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4010 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6482 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3036 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    97345 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3094 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    27365 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3817 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12119 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8286 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12942 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6359 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19087 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-05-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10170 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    33436 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    11316 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    15541 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5061 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17717 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6747 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13372 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8278 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    32032 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-05-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    14645 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    35887 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-morph-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6101 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-morph-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10643 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-offset-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5516 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-offset-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    34417 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8871 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    37965 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9644 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    37965 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8962 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    29857 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-specular-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    12017 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-specular-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10145 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-tile-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4736 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-tile-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)   145859 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5779 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    39568 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7575 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7470 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters00.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2149 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters00.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20546 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters01.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1942 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/filter/filters01.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.353478 CairoSVG-2.7.0/test_non_regression/fail/font/
--rw-r--r--   0 lize      (1000) lize      (1000)      223 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     6480 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5673 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6635 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7873 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5695 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6131 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6090 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7704 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7969 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-05-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7907 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21468 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    11668 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24186 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13993 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21350 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8683 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21554 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-04-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8628 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-04-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19758 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-05-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6873 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18088 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-06-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5987 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21567 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-07-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    12099 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-07-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8872 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7433 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6444 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4332 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4959 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3808 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19451 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-kern-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    14696 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-kern-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    15190 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-overview-201-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7031 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/font/fonts-overview-201-t.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.354478 CairoSVG-2.7.0/test_non_regression/fail/image/
--rw-r--r--   0 lize      (1000) lize      (1000)      625 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/image/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     8956 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3538 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5910 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-12-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3837 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-12-b.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.356478 CairoSVG-2.7.0/test_non_regression/fail/linking/
--rw-r--r--   0 lize      (1000) lize      (1000)      141 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    10632 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4209 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9175 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4316 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10053 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-09-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3418 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-09-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13107 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-10-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4392 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-10-f.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.356478 CairoSVG-2.7.0/test_non_regression/fail/marker/
--rw-r--r--   0 lize      (1000) lize      (1000)      435 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/marker/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    33258 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4984 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6790 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-07-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3322 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-07-f.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.359478 CairoSVG-2.7.0/test_non_regression/fail/mask/
--rw-r--r--   0 lize      (1000) lize      (1000)      703 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    16512 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-intro-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4354 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-intro-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12281 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-05-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4088 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13226 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-07-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6905 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-07-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5544 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-10-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10900 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-11-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3116 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-11-b.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.359478 CairoSVG-2.7.0/test_non_regression/fail/na/
--rw-r--r--   0 lize      (1000) lize      (1000)      156 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/README.rst
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.398478 CairoSVG-2.7.0/test_non_regression/fail/na/animation/
--rw-r--r--   0 lize      (1000) lize      (1000)      116 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    25548 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7691 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7806 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3797 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8577 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8059 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21535 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8614 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24499 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3892 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    22806 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-05-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4341 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24082 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-06-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3813 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23933 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-07-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3856 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18593 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-08-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5024 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-08-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12462 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-09-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5401 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-09-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13129 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-10-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5045 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-10-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13097 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-11-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4945 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-11-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13129 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-12-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5217 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-12-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21499 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-13-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5549 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-13-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    25216 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-14-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4414 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-14-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    25244 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-15-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4442 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-15-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24592 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-17-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4673 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-17-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24160 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-19-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4397 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-19-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11242 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-20-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4547 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-20-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20639 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-21-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6929 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-21-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10117 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-22-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4961 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-22-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10826 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-23-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4650 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-23-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18552 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-24-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7843 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-24-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9446 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-25-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4772 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-25-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    30940 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-26-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4707 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-26-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9432 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-27-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5122 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-27-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18159 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-28-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3434 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-28-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17135 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-29-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5556 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-29-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19446 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-30-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    23625 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-30-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    25641 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-31-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7866 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-31-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7342 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-32-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8953 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-32-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    31180 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-33-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8702 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-33-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    28498 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-34-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    11620 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-34-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    33113 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-35-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    12497 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-35-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    29058 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-36-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    23340 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-36-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23814 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-37-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6147 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-37-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    30316 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-38-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8576 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-38-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    33860 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-39-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    58809 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-39-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    32710 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-40-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    27138 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-40-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17437 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-41-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    23364 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-41-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-42-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-43-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    31958 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-44-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9176 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-44-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-45-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    17446 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-46-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    15603 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-46-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-47-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-48-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-49-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-50-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-51-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    24229 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-52-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6444 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-52-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    22293 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-53-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7983 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-53-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12902 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-60-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13574 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-60-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13181 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-61-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10412 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-61-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12622 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-62-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13951 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-62-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12947 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-63-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10385 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-63-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9787 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-64-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6083 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-64-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14497 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-65-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10887 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-65-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14700 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-66-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9991 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-66-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13466 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-67-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8529 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-67-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14799 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-68-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6473 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-68-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    15396 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-69-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7227 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-69-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11774 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-70-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7390 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-70-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    25262 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-77-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    16962 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-77-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17992 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-78-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    29790 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-78-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    36424 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-80-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    16515 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-80-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    15234 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-81-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10658 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-81-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26693 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-82-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    16381 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-82-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    30301 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-83-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13076 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-83-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6684 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-84-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4176 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-84-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8949 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-85-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5604 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-85-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9696 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-86-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4312 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-86-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19173 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-87-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4431 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-87-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6832 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-88-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3106 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-88-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8809 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-89-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6147 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-89-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10267 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-90-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5427 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-90-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18212 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-91-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9883 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-91-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12824 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-92-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5084 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-92-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23518 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-events-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6348 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-events-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13322 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    14328 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    27854 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7708 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    32196 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    15898 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    28162 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    15504 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5497 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5851 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13547 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-script-elem-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4213 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-script-elem-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10620 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-struct-dom-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4183 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-struct-dom-01-b.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.411478 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/
--rw-r--r--   0 lize      (1000) lize      (1000)      124 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    18644 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-cursor-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8733 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-cursor-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14244 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-dom-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5967 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-dom-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    15501 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6264 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9858 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3816 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6479 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-202-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4040 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-202-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    37532 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-203-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6589 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-203-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23273 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4974 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23225 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4738 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    28455 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4562 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18753 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    12139 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17662 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    27871 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    12235 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18878 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    12430 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19059 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-05-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9199 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    27854 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-07-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7310 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    42079 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-08-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    14175 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-08-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    36298 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-09-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13782 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-09-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8584 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-10-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3891 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-10-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    32461 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-201-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    28405 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-202-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    11533 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3991 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11409 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3957 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7971 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3868 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6068 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4104 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9702 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3656 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10340 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3660 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16212 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3719 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    25280 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/styling-css-06-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    29103 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/styling-css-06-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    47910 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4184 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17418 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6480 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16487 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6866 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-03-f.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.437479 CairoSVG-2.7.0/test_non_regression/fail/na/script/
--rw-r--r--   0 lize      (1000) lize      (1000)      104 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    16479 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/conform-viewers-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5496 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/conform-viewers-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5961 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4300 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6683 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3595 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13845 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4904 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26786 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6387 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23309 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/extend-namespace-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8597 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/extend-namespace-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6804 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-09-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3211 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-09-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6255 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-12-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3855 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-12-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20157 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6828 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14035 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9645 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13547 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-elem-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    11528 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4514 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20894 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5731 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21007 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5504 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21948 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-04-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5585 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-04-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7586 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3589 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17730 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3626 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11914 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8647 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13586 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5409 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17061 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5426 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23161 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-04-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6246 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-04-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    25222 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-05-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6229 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6362 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-06-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5048 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-06-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4927 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-07-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4499 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-07-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7916 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-08-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3546 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-08-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10620 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-09-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    11003 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-11-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5653 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-11-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13374 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-12-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4324 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-12-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8464 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-13-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5400 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-13-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5814 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-14-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5211 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-14-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5605 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-15-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6660 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-15-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7018 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-16-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5992 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-16-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9094 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-17-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4712 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-17-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8317 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-18-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6931 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-18-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10833 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-19-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4342 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-19-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6621 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-20-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7282 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-20-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5891 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-image-11-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3607 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-image-11-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18997 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4862 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7763 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6768 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4632 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-13-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3834 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-13-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6070 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-14-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3551 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-14-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6056 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-15-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4024 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-15-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24861 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/styling-pres-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9352 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/styling-pres-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    40319 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/svgdom-over-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8040 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/svgdom-over-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8542 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13929 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20452 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5572 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24608 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5410 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7013 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6746 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18793 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-05-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7071 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    41270 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6560 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20310 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6180 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13096 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3502 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26379 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-04-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9585 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-04-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    24883 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-05-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5146 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9597 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-06-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5190 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-06-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13434 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-07-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6288 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-07-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    27349 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-08-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8417 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-08-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7350 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4126 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7397 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4788 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7506 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4799 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7397 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4628 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7316 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3830 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.437479 CairoSVG-2.7.0/test_non_regression/fail/path/
--rw-r--r--   0 lize      (1000) lize      (1000)      363 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/path/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     5156 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/path/paths-data-18-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4726 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/path/paths-data-18-f.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.454479 CairoSVG-2.7.0/test_non_regression/fail/text/
--rw-r--r--   0 lize      (1000) lize      (1000)      460 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    10718 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/styling-css-05-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3815 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/styling-css-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    22700 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3974 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20507 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-05-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3981 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    14330 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-06-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4743 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-06-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11059 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-07-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4714 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9132 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-08-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4826 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-align-08-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    19582 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6770 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    15957 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    17278 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    18828 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    18401 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10028 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-bidi-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3190 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-bidi-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    36556 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-deco-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4100 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-deco-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26203 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5278 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    22378 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-02-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4914 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17952 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-03-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7279 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17952 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4212 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7046 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-05-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2980 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    30341 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-202-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5153 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-202-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    23273 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-203-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6498 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-203-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    25143 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-204-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6129 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-204-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26424 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5301 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17870 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-02-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4692 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16629 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4859 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    27205 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4455 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16824 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-05-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4205 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13298 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-06-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4786 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    20255 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-07-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3237 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    17910 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-09-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4764 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-09-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    16847 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-10-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4315 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-10-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    15955 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-11-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4758 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-11-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12313 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-12-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4480 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-12-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    31007 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-spacing-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3784 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-spacing-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    73363 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-01-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10257 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26482 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-03-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5248 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12954 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)    11509 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12351 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-05-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8364 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7969 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-06-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7434 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13842 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-12-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8863 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/text-text-12-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10455 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/textdecoration01.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1076 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/text/textdecoration01.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.456479 CairoSVG-2.7.0/test_non_regression/fail/use/
--rw-r--r--   0 lize      (1000) lize      (1000)      828 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)    29471 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-05-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4910 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6764 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-06-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3514 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-06-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11701 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-08-b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3876 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-08-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6415 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-12-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5877 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-12-f.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.456479 CairoSVG-2.7.0/test_non_regression/fail/viewbox/
--rw-r--r--   0 lize      (1000) lize      (1000)      550 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/viewbox/README.rst
--rw-r--r--   0 lize      (1000) lize      (1000)      862 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-01-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2438 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6330 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-04-t.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3590 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-04-t.svg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.483480 CairoSVG-2.7.0/test_non_regression/images/
--rw-r--r--   0 lize      (1000) lize      (1000)     1038 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/20x20.png
--rw-r--r--   0 lize      (1000) lize      (1000)      238 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/50x50-viewbox-greencircle.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/50x50greencircle.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2470 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/DisplaceChecker.png
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.499480 CairoSVG-2.7.0/test_non_regression/images/PngSuite/
--rw-r--r--   0 lize      (1000) lize      (1000)      217 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi0g01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      154 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi0g02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      247 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      254 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      299 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      315 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      595 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      132 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      193 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      327 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1527 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi4a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2855 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi4a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      361 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi6a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     4180 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi6a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      164 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn0g01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      104 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn0g02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      145 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      138 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      167 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      145 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      302 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      112 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      146 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1286 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      126 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn4a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2206 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn4a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      184 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn6a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3435 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn6a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgai4a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2855 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgai4a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      184 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgan6a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3435 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgan6a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      140 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgbn4a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2220 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bggn4a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      202 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgwn6a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3453 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgyn6a16.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1514 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ccwn2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1554 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ccwn3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      404 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cdfn2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      344 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cdhn2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      232 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cdsn2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      724 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cdun2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      258 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ch1n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1810 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ch2n3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      292 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cm0n0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      292 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cm7n0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      292 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cm9n0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cs3n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      259 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cs3n3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      186 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cs5n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      271 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cs5n3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      149 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cs8n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      256 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/cs8n3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      273 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ct0n0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      792 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ct1n0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      753 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ctzn0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      319 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f00n0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2475 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f00n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      321 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f01n0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1180 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f01n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      355 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f02n0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1729 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f02n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      389 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f03n0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1291 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f03n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      269 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f04n0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      985 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/f04n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      345 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g03n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      370 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g03n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g03n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      363 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g04n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      377 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g04n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      219 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g04n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      339 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g05n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      350 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g05n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      206 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g05n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      321 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g07n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      340 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g07n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      207 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g07n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      262 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g10n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      285 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g10n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g10n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      383 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g25n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      405 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g25n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      215 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/g25n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      167 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi1n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      302 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi1n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      179 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi2n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      314 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi2n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      203 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi4n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      338 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi4n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1283 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi9n0g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3038 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi9n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)    20519 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/pngsuite.doc
--rw-r--r--   0 lize      (1000) lize      (1000)     2262 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/pngsuite_logo.png
--rw-r--r--   0 lize      (1000) lize      (1000)      962 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/pp0n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      818 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/pp0n6a08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1477 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps1n0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1641 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps1n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2341 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps2n0g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2505 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps2n2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)      113 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s01i3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      113 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s01n3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      114 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s02i3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      115 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s02n3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      118 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s03i3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      120 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s03n3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      126 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s04i3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      121 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s04n3p01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      134 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s05i3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      129 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s05n3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      143 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s06i3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      131 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s06n3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      149 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s07i3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      138 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s07n3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      149 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s08i3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      139 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s08n3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      147 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s09i3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      143 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s09n3p02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      355 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s32i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      263 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s32n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      385 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s33i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      329 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s33n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      349 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s34i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      248 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s34n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      399 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s35i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      338 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s35n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      356 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s36i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      258 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s36n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      393 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s37i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      336 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s37n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      357 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s38i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      245 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s38n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      420 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s39i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      352 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s39n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      357 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s40i3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      256 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/s40n3p04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      419 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbbn1g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1994 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbbn2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1128 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbbn3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1994 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbgn2c16.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1128 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbgn3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1347 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbrn2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1146 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbwn1g16.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1131 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbwn3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1131 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbyn3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      689 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp0n1g08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1311 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp0n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1120 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp0n3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1115 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp1n3p08.png
--rw-r--r--   0 lize      (1000) lize      (1000)       49 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/x00n0g01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      261 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/xcrn0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)      240 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/xlfn0g04.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3172 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/z00n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      232 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/z03n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      224 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/z06n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)      224 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/PngSuite/z09n2c08.png
--rw-r--r--   0 lize      (1000) lize      (1000)    57657 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/SVG-1.1-monolithic-fixed.dtd
--rw-r--r--   0 lize      (1000) lize      (1000)     1722 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/SVGImageTest.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13238 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/animation-add-BE-09.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      951 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/animation-extRef-image1.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      844 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/animation-extRef-image2.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      725 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/animation-extRef-image3.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/black10x10.png
--rw-r--r--   0 lize      (1000) lize      (1000)      159 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/blue1x1.png
--rw-r--r--   0 lize      (1000) lize      (1000)       83 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/blue_10x10.png
--rw-r--r--   0 lize      (1000) lize      (1000)      833 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/blue_10x10.ppm
--rw-r--r--   0 lize      (1000) lize      (1000)    37497 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/bluesquidj.png
--rw-r--r--   0 lize      (1000) lize      (1000)      973 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/bullet-small.png
--rw-r--r--   0 lize      (1000) lize      (1000)      971 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/bullet-white.png
--rw-r--r--   0 lize      (1000) lize      (1000)      972 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/bullet.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1998 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/bumpMap.png
--rw-r--r--   0 lize      (1000) lize      (1000)      657 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/bumpMap2.png
--rw-r--r--   0 lize      (1000) lize      (1000)      433 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/bumpMap3.png
--rw-r--r--   0 lize      (1000) lize      (1000)       35 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/case-insensitivity.css
--rw-r--r--   0 lize      (1000) lize      (1000)      740 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/changeColor.ICM
--rw-r--r--   0 lize      (1000) lize      (1000)      705 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/colorprof.png
--rw-r--r--   0 lize      (1000) lize      (1000)     9281 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/convolveImage.png
--rw-r--r--   0 lize      (1000) lize      (1000)    29842 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/coords-units-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13340 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/coords-units-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4750 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/copyright-documents-19990405.html
--rw-r--r--   0 lize      (1000) lize      (1000)      997 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/diagarrow.png
--rw-r--r--   0 lize      (1000) lize      (1000)        0 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/empty.js
--rw-r--r--   0 lize      (1000) lize      (1000)     3697 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/ext-TestComic.svg
--rw-r--r--   0 lize      (1000) lize      (1000)        4 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/f.js
--rw-r--r--   0 lize      (1000) lize      (1000)      740 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/fillChangeColor.ICM
--rw-r--r--   0 lize      (1000) lize      (1000)     7343 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-blend-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7818 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-color-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9754 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-composite-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7805 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-comptran-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9281 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-conv-01-f.includeimage.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7987 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-conv-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10092 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-diffuse-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7577 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/filters-example-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    48928 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/footprints.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)   313676 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/footprints2.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)    12435 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/galpha.png
--rw-r--r--   0 lize      (1000) lize      (1000)      213 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam030.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1029 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam030b.png
--rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam045.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1059 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam045b.png
--rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam056.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1059 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam056b.png
--rw-r--r--   0 lize      (1000) lize      (1000)      205 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam100.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1044 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam100b.png
--rw-r--r--   0 lize      (1000) lize      (1000)      187 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam200.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1019 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/gam200b.png
--rw-r--r--   0 lize      (1000) lize      (1000)      159 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/green1x1.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1111 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/greentopbutton.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)      612 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/happysmiley.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1884 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/image.png
--rw-r--r--   0 lize      (1000) lize      (1000)    34183 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/image1.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)   394416 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/image1.png
--rw-r--r--   0 lize      (1000) lize      (1000)    12586 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/image1_b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     6643 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/image2_b.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)     7412 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/image2_b.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1541 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/inline2.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7566 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/interact-dom-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2921 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/interact-order-02-b-targ.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2936 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/interact-order-03-b-targ.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      124 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/leftarrow.png
--rw-r--r--   0 lize      (1000) lize      (1000)      153 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/level1.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      140 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/level2.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8845 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8183 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-1st.png
--rw-r--r--   0 lize      (1000) lize      (1000)    34164 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-2nd.png
--rw-r--r--   0 lize      (1000) lize      (1000)    34164 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-3rd.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13626 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-4th.png
--rw-r--r--   0 lize      (1000) lize      (1000)    34164 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-start.png
--rw-r--r--   0 lize      (1000) lize      (1000)    28465 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-03-f-1st.png
--rw-r--r--   0 lize      (1000) lize      (1000)    26549 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linking-uri-03-f-start.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1919 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linkingCircle-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2649 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/linkingToc-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      268 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/magnify.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1985 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/makealpha.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4402 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/myimage.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)      264 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_bullet.png
--rw-r--r--   0 lize      (1000) lize      (1000)      252 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_down.png
--rw-r--r--   0 lize      (1000) lize      (1000)      170 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_downleft.png
--rw-r--r--   0 lize      (1000) lize      (1000)      169 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_downright.png
--rw-r--r--   0 lize      (1000) lize      (1000)      155 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_frame.png
--rw-r--r--   0 lize      (1000) lize      (1000)      166 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_left.png
--rw-r--r--   0 lize      (1000) lize      (1000)      270 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_noframe.png
--rw-r--r--   0 lize      (1000) lize      (1000)      168 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_right.png
--rw-r--r--   0 lize      (1000) lize      (1000)      155 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_svg.png
--rw-r--r--   0 lize      (1000) lize      (1000)      173 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_up.png
--rw-r--r--   0 lize      (1000) lize      (1000)      172 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_upleft.png
--rw-r--r--   0 lize      (1000) lize      (1000)      173 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/nav_upright.png
--rw-r--r--   0 lize      (1000) lize      (1000)    36641 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/old-name-2-new-name1.html
--rw-r--r--   0 lize      (1000) lize      (1000)    36446 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13254 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    42041 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-02-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10827 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    38026 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-03-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    10687 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    30546 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-04-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)    14511 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/paths-data-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    31090 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/pinksquidj.png
--rw-r--r--   0 lize      (1000) lize      (1000)   145806 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/plant.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)    48672 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/purplesquidj.png
--rw-r--r--   0 lize      (1000) lize      (1000)      500 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/rects.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      419 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/rects_b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      159 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/red1x1.png
--rw-r--r--   0 lize      (1000) lize      (1000)    13717 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/rgbalpha.png
--rw-r--r--   0 lize      (1000) lize      (1000)      963 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/rightarrow.png
--rw-r--r--   0 lize      (1000) lize      (1000)     1434 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/rotate20.png
--rw-r--r--   0 lize      (1000) lize      (1000)      274 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/selector-types-fill-green.css
--rw-r--r--   0 lize      (1000) lize      (1000)      374 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/selector-types-visibility-hidden.css
--rw-r--r--   0 lize      (1000) lize      (1000)     3247 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/shapes-ellipse-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    31126 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/shapes-ellipse-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     7752 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/shapes-ellipse-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3445 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/shapes-rect-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26453 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/shapes-rect-01-f.png
--rw-r--r--   0 lize      (1000) lize      (1000)     8003 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/shapes-rect-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10647 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/sign.png
--rw-r--r--   0 lize      (1000) lize      (1000)     2856 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/smiley.png
--rw-r--r--   0 lize      (1000) lize      (1000)     5923 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/sphere.png
--rwxr-xr-x   0 lize      (1000) lize      (1000)     1499 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/star.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12777 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/stefan_252_tRNS_opti.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3141 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-frag-01-B.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4751 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-01.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)    63238 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-01.png
--rw-r--r--   0 lize      (1000) lize      (1000)     3779 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-02.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)    35887 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-02.png
--rw-r--r--   0 lize      (1000) lize      (1000)      320 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-11-b-1.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      333 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-11-b-2.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      448 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-12-b-cycle.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      455 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-12-b-nocycle.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      287 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-image-17-b-1.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    71497 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-symbol-01.png
--rw-r--r--   0 lize      (1000) lize      (1000)      521 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-use-06-b-1.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      529 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/struct-use-08-b-cycles.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2376 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/svgRef1.svg
--rw-r--r--   0 lize      (1000) lize      (1000)       92 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/svgRef4.css
--rw-r--r--   0 lize      (1000) lize      (1000)     1632 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/svgRef4.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5992 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-align-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8674 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-align-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6069 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-align-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11291 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-altglyph-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2352 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-extTref-BE-18-targ.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8077 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-intro-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9985 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-tref-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9374 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/text-ws-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3191 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/toc-sv.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3251 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/toc-svcmp.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    52480 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/townsville.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)    66460 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/tree.jpg
--rw-r--r--   0 lize      (1000) lize      (1000)     1232 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/images/uparrow.png
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.501480 CairoSVG-2.7.0/test_non_regression/resources/
--rw-r--r--   0 lize      (1000) lize      (1000)    22708 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/Anglepoise.otf
--rw-r--r--   0 lize      (1000) lize      (1000)     1860 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/Blocky.otf
--rw-r--r--   0 lize      (1000) lize      (1000)   166392 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/CalaLig.otf
--rw-r--r--   0 lize      (1000) lize      (1000)    15656 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/FreeSerif.otf
--rw-r--r--   0 lize      (1000) lize      (1000)    15360 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/FreeSerifBold.otf
--rw-r--r--   0 lize      (1000) lize      (1000)    17636 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/FreeSerifBoldItalic.otf
--rw-r--r--   0 lize      (1000) lize      (1000)    20924 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/FreeSerifItalic.otf
--rw-r--r--   0 lize      (1000) lize      (1000)    26220 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/resources/SVGFreeSans.otf
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-03-20 14:32:52.550481 CairoSVG-2.7.0/test_non_regression/svg/
--rw-r--r--   0 lize      (1000) lize      (1000)      816 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/svg/InitialCoords.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1538 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/svg/Nested.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1233 2022-12-27 11:37:30.000000 CairoSVG-2.7.0/test_non_regression/svg/NewCoordSys.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      655 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/OrigCoordSys.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4086 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/PreserveAspectRatio.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1508 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/RotateScale.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1516 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/Skew.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1837 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/Units.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1090 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/ViewBox.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      999 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/arcs01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2387 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/arcs02.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      583 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/circle01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4128 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/color-prop-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6324 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/color-prop-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5422 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/color-prop-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5806 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/color-prop-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3175 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/color-prop-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2188 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/conform-viewers-01-t.svgz
--rw-r--r--   0 lize      (1000) lize      (1000)     4070 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/conform-viewers-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3619 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-coord-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3628 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-coord-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12864 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9961 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5473 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4908 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4953 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4192 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3913 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4128 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-08-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4892 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-09-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4346 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-10-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4354 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-11-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4405 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-12-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4286 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-13-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4458 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-trans-14-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5001 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4527 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3794 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3551 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4382 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11342 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-units-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8314 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-units-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9072 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-units-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8509 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    53178 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6064 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7005 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1857 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/cubic01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5443 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/cubic02.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      709 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/ellipse01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1948 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/feBlend.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2995 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/fillrule-evenodd.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2994 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/fillrule-nonzero.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4141 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/filters-offset-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2870 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/imp-path-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      784 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/inheritance.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      911 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/line01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1789 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linecap.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1684 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linejoin.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      879 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/lingrad01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6414 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-a-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5740 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-a-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5860 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-a-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3214 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-a-08-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3761 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-frag-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8847 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-uri-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9537 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-uri-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5464 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/linking-uri-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      805 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/marker.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1383 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/mask01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4003 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-filter-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7239 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-mask-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2805 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-mask-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5995 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-opacity-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5047 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4541 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6772 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4003 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-04-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3862 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-06-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5760 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-08-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2801 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-13-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4238 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/masking-path-14-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    21666 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/metadata-example-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1952 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/opacity01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5238 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-control-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3497 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-control-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3400 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-control-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5839 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-control-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3408 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-control-06-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3551 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-fill-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3711 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-fill-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3488 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-fill-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4352 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-fill-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4502 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-fill-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    10160 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-marker-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    13254 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-marker-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5040 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-marker-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12550 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-marker-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9894 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-marker-06-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3899 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3727 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3758 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3827 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5369 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4032 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3855 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4737 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-08-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3245 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-09-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    11078 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8577 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     8433 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5482 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5328 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5520 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5448 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5355 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-08-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5268 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-09-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5896 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-10-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3945 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-12-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3149 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-13-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3628 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-14-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3555 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-15-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3273 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-16-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3309 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-17-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5939 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/paths-data-19-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      859 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pattern01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      821 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/polygon01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      852 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/polyline01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3902 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4696 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4428 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5034 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-04-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5501 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6668 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-06-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5130 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-07-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5472 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-08-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6779 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-09-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5644 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-10-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7514 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-11-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6758 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-12-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     9242 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-13-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6443 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-14-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3773 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-15-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4408 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-16-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5433 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-17-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5634 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-18-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4961 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-20-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6614 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-21-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4269 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-22-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3835 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-23-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3598 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-24-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3846 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-stops-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6524 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2939 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4585 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3652 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3492 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3273 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-06-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3419 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-07-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3413 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-08-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3683 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-09-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1135 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/quad01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1026 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/radgrad01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      581 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/rect01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      714 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/rect02.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3337 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-elems-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3403 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-elems-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3513 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-elems-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3658 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-elems-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3619 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-elems-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3684 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-elems-08-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6712 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-groups-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6004 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/render-groups-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3192 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-circle-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3235 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-circle-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4439 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-ellipse-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3197 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-ellipse-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3815 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-ellipse-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3330 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-grammar-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6517 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-intro-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4847 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-intro-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4390 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-line-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2758 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-line-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4842 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-polygon-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4184 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-polygon-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3159 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-polygon-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5435 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-polyline-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4328 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-polyline-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4641 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3380 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6546 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3396 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4015 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3562 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-06-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2921 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-07-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3230 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-cond-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    26599 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-cond-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4189 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-cond-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4062 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-02-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3347 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3443 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3821 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3513 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-defs-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3554 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-frag-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3611 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-frag-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4942 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-frag-05-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4767 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-frag-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4231 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-group-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4436 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-group-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    12165 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-group-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3289 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5000 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)    32937 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-04-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3096 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-05-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5562 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-06-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3932 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3159 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-08-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3161 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-09-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3157 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-10-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5522 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-13-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5517 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-14-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6635 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-15-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2706 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-16-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3156 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-17-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3152 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-18-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3368 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-image-19-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3111 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-svg-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5049 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-symbol-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5603 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-use-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3756 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-use-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4399 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-use-07-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3852 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-use-09-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5176 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-use-10-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5940 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/struct-use-11-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3363 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-class-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4160 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4137 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5246 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     7242 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2899 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-07-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4884 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-08-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4404 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-09-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3559 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-css-10-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3519 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-elem-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4258 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-inherit-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3395 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-pres-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     2773 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-pres-03-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4049 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-pres-04-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3615 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/styling-pres-05-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4138 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-align-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3996 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-align-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4939 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-align-04-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4931 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-path-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4941 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-path-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4255 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-text-07-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3766 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-text-08-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4579 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-text-09-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4553 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-text-10-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4903 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-text-11-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3737 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-tref-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3698 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-tref-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3749 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-tref-03-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6449 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-tspan-01-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     6546 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-tspan-02-b.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5664 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-ws-01-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     5769 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-ws-02-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     4026 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text-ws-03-t.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      595 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/text01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      929 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/toap01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1040 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/toap02.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      973 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/toap03.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      979 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/toap04.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      865 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/tref01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      542 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/triangle01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1139 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/test_non_regression/svg/tspan-dx-dy.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      685 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/tspan01.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      813 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/tspan02.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      808 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/tspan03.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      677 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/tspan04.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     1100 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/tspan05.svg
--rw-r--r--   0 lize      (1000) lize      (1000)     3521 2022-12-27 11:37:31.000000 CairoSVG-2.7.0/test_non_regression/svg/types-basic-01-f.svg
--rw-r--r--   0 lize      (1000) lize      (1000)      914 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/test_non_regression/test_helpers.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1288 2022-12-27 11:39:42.000000 CairoSVG-2.7.0/test_non_regression/test_non_regression.py
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.339043 CairoSVG-2.7.1/
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.219040 CairoSVG-2.7.1/.github/
+-rw-r--r--   0 lize      (1000) lize      (1000)       78 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/.github/FUNDING.yml
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.219040 CairoSVG-2.7.1/.github/workflows/
+-rw-r--r--   0 lize      (1000) lize      (1000)      976 2023-08-05 08:44:33.000000 CairoSVG-2.7.1/.github/workflows/tests.yml
+-rw-r--r--   0 lize      (1000) lize      (1000)      107 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/.gitignore
+-rw-r--r--   0 lize      (1000) lize      (1000)       95 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/.gitmodules
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.220040 CairoSVG-2.7.1/CairoSVG.egg-info/
+-rw-r--r--   0 lize      (1000) lize      (1000)     2393 2023-08-05 09:02:26.000000 CairoSVG-2.7.1/CairoSVG.egg-info/PKG-INFO
+-rw-r--r--   0 lize      (1000) lize      (1000)    64093 2023-08-05 09:02:26.000000 CairoSVG-2.7.1/CairoSVG.egg-info/SOURCES.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)        1 2023-08-05 09:02:26.000000 CairoSVG-2.7.1/CairoSVG.egg-info/dependency_links.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)       52 2023-08-05 09:02:26.000000 CairoSVG-2.7.1/CairoSVG.egg-info/entry_points.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)      107 2023-08-05 09:02:26.000000 CairoSVG-2.7.1/CairoSVG.egg-info/requires.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)        9 2023-08-05 09:02:26.000000 CairoSVG-2.7.1/CairoSVG.egg-info/top_level.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)     7650 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/LICENSE
+-rw-r--r--   0 lize      (1000) lize      (1000)    11612 2023-08-05 09:01:34.000000 CairoSVG-2.7.1/NEWS.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     2393 2023-08-05 09:02:26.339043 CairoSVG-2.7.1/PKG-INFO
+-rw-r--r--   0 lize      (1000) lize      (1000)     1056 2023-01-12 16:45:06.000000 CairoSVG-2.7.1/README.rst
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.221040 CairoSVG-2.7.1/cairosvg/
+-rw-r--r--   0 lize      (1000) lize      (1000)        5 2023-08-05 08:56:28.000000 CairoSVG-2.7.1/cairosvg/VERSION
+-rw-r--r--   0 lize      (1000) lize      (1000)     4799 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/cairosvg/__init__.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     3045 2023-03-20 14:31:13.000000 CairoSVG-2.7.1/cairosvg/__main__.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    13980 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/bounding_box.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    10672 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/cairosvg/colors.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     4029 2023-03-20 14:29:52.000000 CairoSVG-2.7.1/cairosvg/css.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    13555 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/defs.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     1572 2023-01-12 16:37:55.000000 CairoSVG-2.7.1/cairosvg/features.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    12713 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/helpers.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     4145 2023-04-29 11:54:46.000000 CairoSVG-2.7.1/cairosvg/image.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    16134 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/parser.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    17029 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/path.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     3432 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/cairosvg/shapes.py
+-rw-r--r--   0 lize      (1000) lize      (1000)    20864 2023-08-04 22:29:03.000000 CairoSVG-2.7.1/cairosvg/surface.py
+-rw-r--r--   0 lize      (1000) lize      (1000)      272 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/cairosvg/svg.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     6930 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/test_api.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     9751 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/text.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     4992 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/cairosvg/url.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     1843 2023-08-05 09:02:26.339043 CairoSVG-2.7.1/setup.cfg
+-rwxr-xr-x   0 lize      (1000) lize      (1000)      574 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/setup.py
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.222040 CairoSVG-2.7.1/test_non_regression/
+-rw-r--r--   0 lize      (1000) lize      (1000)     1592 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/LICENSE
+-rw-r--r--   0 lize      (1000) lize      (1000)     1323 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/test_non_regression/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)      934 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/test_non_regression/__init__.py
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.222040 CairoSVG-2.7.1/test_non_regression/fail/
+-rw-r--r--   0 lize      (1000) lize      (1000)      508 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/README.rst
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.222040 CairoSVG-2.7.1/test_non_regression/fail/cap/
+-rw-r--r--   0 lize      (1000) lize      (1000)      346 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/cap/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     5998 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/cap/painting-control-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2938 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/cap/painting-control-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11044 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/cap/painting-stroke-10-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3559 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/cap/painting-stroke-10-t.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.223040 CairoSVG-2.7.1/test_non_regression/fail/color/
+-rw-r--r--   0 lize      (1000) lize      (1000)      148 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/color/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     6677 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/color/color-prof-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3965 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/color/color-prof-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14587 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8956 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9867 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4742 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-02-b.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.223040 CairoSVG-2.7.1/test_non_regression/fail/css/
+-rw-r--r--   0 lize      (1000) lize      (1000)       82 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/css/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     3406 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/css/struct-use-04-b.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.224040 CairoSVG-2.7.1/test_non_regression/fail/draft/
+-rw-r--r--   0 lize      (1000) lize      (1000)      816 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/draft/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     6039 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/draft/painting-marker-properties-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4618 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/draft/painting-marker-properties-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6858 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/draft/paths-data-20-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4243 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/draft/paths-data-20-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23588 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/draft/types-basic-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4413 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/draft/types-basic-02-f.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.235041 CairoSVG-2.7.1/test_non_regression/fail/filter/
+-rw-r--r--   0 lize      (1000) lize      (1000)     1717 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     9655 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/enable-background-01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3701 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/enable-background-01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7578 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feColorMatrix.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2585 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feColorMatrix.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6366 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feComponentTransfer.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2875 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feComponentTransfer.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14985 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feComposite.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9265 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feComposite.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5449 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feMorphology.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1525 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feMorphology.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)   139525 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feTurbulence.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3221 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/feTurbulence.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18824 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-background-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8520 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-background-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16420 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-blend-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6769 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-blend-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24542 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6533 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7439 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5593 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16884 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9284 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6192 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4521 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)   127777 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4314 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    35393 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-05-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3530 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16794 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-comptran-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6826 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-comptran-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    53536 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6835 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    38250 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4243 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    34066 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5246 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    87653 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8527 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13705 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-05-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4305 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21863 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-diffuse-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8988 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-diffuse-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    45323 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7173 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8965 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5267 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    22359 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-example-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5037 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-example-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12696 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4743 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16264 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6255 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19453 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4927 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8057 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4010 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6482 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3036 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    97345 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3094 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    27365 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3817 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12119 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8286 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12942 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6359 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19087 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-05-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10170 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    33436 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    11316 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    15541 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5061 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17717 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6747 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13372 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8278 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    32032 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-05-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    14645 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    35887 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-morph-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6101 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-morph-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10643 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-offset-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5516 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-offset-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    34417 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8871 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    37965 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9644 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    37965 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8962 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    29857 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-specular-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    12017 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-specular-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10145 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-tile-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4736 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-tile-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)   145859 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5779 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    39568 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7575 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7470 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters00.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2149 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters00.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20546 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1942 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/filter/filters01.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.239041 CairoSVG-2.7.1/test_non_regression/fail/font/
+-rw-r--r--   0 lize      (1000) lize      (1000)      223 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     6480 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5673 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6635 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7873 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5695 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6131 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6090 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7704 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7969 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-05-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7907 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21468 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    11668 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24186 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13993 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21350 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8683 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21554 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-04-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8628 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-04-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19758 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-05-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6873 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18088 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-06-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5987 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21567 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-07-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    12099 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-07-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8872 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7433 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6444 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4332 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4959 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3808 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19451 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-kern-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    14696 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-kern-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    15190 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-overview-201-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7031 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/font/fonts-overview-201-t.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.239041 CairoSVG-2.7.1/test_non_regression/fail/image/
+-rw-r--r--   0 lize      (1000) lize      (1000)      625 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/image/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     8956 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3538 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5910 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-12-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3837 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-12-b.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.240041 CairoSVG-2.7.1/test_non_regression/fail/linking/
+-rw-r--r--   0 lize      (1000) lize      (1000)      141 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    10632 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4209 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9175 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4316 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10053 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-09-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3418 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-09-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13107 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-10-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4392 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-10-f.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.240041 CairoSVG-2.7.1/test_non_regression/fail/marker/
+-rw-r--r--   0 lize      (1000) lize      (1000)      435 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/marker/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    33258 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4984 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6790 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-07-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3322 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-07-f.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.241041 CairoSVG-2.7.1/test_non_regression/fail/mask/
+-rw-r--r--   0 lize      (1000) lize      (1000)      703 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    16512 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-intro-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4354 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-intro-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12281 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-05-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4088 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13226 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-07-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6905 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-07-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5544 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-10-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10900 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-11-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3116 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-11-b.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.241041 CairoSVG-2.7.1/test_non_regression/fail/na/
+-rw-r--r--   0 lize      (1000) lize      (1000)      156 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/README.rst
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.258041 CairoSVG-2.7.1/test_non_regression/fail/na/animation/
+-rw-r--r--   0 lize      (1000) lize      (1000)      116 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    25548 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7691 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7806 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3797 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8577 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8059 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21535 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8614 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24499 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3892 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    22806 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-05-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4341 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24082 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-06-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3813 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23933 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-07-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3856 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18593 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-08-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5024 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-08-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12462 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-09-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5401 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-09-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13129 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-10-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5045 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-10-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13097 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-11-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4945 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-11-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13129 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-12-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5217 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-12-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21499 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-13-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5549 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-13-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    25216 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-14-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4414 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-14-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    25244 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-15-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4442 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-15-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24592 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-17-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4673 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-17-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24160 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-19-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4397 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-19-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11242 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-20-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4547 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-20-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20639 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-21-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6929 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-21-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10117 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-22-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4961 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-22-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10826 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-23-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4650 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-23-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18552 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-24-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7843 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-24-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9446 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-25-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4772 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-25-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    30940 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-26-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4707 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-26-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9432 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-27-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5122 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-27-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18159 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-28-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3434 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-28-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17135 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-29-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5556 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-29-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19446 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-30-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    23625 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-30-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    25641 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-31-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7866 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-31-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7342 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-32-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8953 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-32-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    31180 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-33-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8702 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-33-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    28498 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-34-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    11620 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-34-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    33113 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-35-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    12497 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-35-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    29058 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-36-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    23340 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-36-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23814 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-37-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6147 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-37-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    30316 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-38-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8576 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-38-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    33860 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-39-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    58809 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-39-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    32710 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-40-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    27138 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-40-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17437 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-41-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    23364 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-41-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-42-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-43-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    31958 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-44-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9176 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-44-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-45-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    17446 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-46-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    15603 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-46-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-47-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-48-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-49-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-50-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-51-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    24229 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-52-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6444 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-52-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    22293 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-53-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7983 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-53-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12902 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-60-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13574 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-60-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13181 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-61-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10412 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-61-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12622 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-62-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13951 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-62-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12947 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-63-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10385 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-63-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9787 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-64-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6083 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-64-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14497 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-65-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10887 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-65-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14700 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-66-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9991 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-66-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13466 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-67-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8529 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-67-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14799 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-68-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6473 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-68-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    15396 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-69-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7227 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-69-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11774 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-70-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7390 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-70-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    25262 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-77-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    16962 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-77-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17992 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-78-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    29790 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-78-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    36424 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-80-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    16515 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-80-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    15234 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-81-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10658 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-81-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26693 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-82-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    16381 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-82-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    30301 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-83-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13076 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-83-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6684 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-84-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4176 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-84-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8949 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-85-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5604 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-85-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9696 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-86-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4312 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-86-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19173 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-87-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4431 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-87-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6832 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-88-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3106 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-88-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8809 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-89-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6147 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-89-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10267 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-90-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5427 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-90-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18212 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-91-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9883 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-91-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12824 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-92-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5084 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-92-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23518 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-events-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6348 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-events-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13322 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    14328 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    27854 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7708 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    32196 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    15898 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    28162 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    15504 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5497 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5851 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13547 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-script-elem-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4213 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-script-elem-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10620 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-struct-dom-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4183 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-struct-dom-01-b.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.264041 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/
+-rw-r--r--   0 lize      (1000) lize      (1000)      124 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    18644 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-cursor-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8733 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-cursor-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14244 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-dom-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5967 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-dom-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    15501 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6264 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9858 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3816 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6479 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-202-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4040 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-202-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    37532 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-203-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6589 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-203-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23273 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4974 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23225 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4738 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    28455 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4562 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18753 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    12139 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17662 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    27871 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    12235 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18878 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    12430 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19059 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-05-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9199 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    27854 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-07-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7310 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    42079 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-08-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    14175 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-08-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    36298 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-09-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13782 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-09-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8584 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-10-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3891 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-10-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    32461 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-201-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    28405 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-202-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    11533 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3991 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11409 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3957 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7971 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3868 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6068 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4104 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9702 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3656 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10340 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3660 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16212 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3719 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    25280 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/styling-css-06-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    29103 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/styling-css-06-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    47910 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4184 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17418 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6480 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16487 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6866 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-03-f.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.275041 CairoSVG-2.7.1/test_non_regression/fail/na/script/
+-rw-r--r--   0 lize      (1000) lize      (1000)      104 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    16479 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/conform-viewers-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5496 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/conform-viewers-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5961 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4300 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6683 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3595 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13845 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4904 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26786 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6387 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23309 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/extend-namespace-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8597 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/extend-namespace-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6804 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-09-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3211 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-09-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6255 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-12-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3855 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-12-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20157 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6828 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14035 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9645 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13547 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-elem-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    11528 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4514 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20894 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5731 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21007 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5504 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21948 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-04-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5585 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-04-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7586 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3589 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17730 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3626 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11914 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8647 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13586 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5409 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17061 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5426 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23161 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-04-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6246 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-04-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    25222 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-05-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6229 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6362 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-06-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5048 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-06-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4927 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-07-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4499 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-07-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7916 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-08-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3546 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-08-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10620 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-09-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    11003 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-11-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5653 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-11-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13374 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-12-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4324 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-12-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8464 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-13-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5400 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-13-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5814 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-14-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5211 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-14-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5605 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-15-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6660 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-15-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7018 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-16-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5992 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-16-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9094 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-17-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4712 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-17-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8317 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-18-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6931 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-18-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10833 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-19-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4342 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-19-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6621 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-20-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7282 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-20-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5891 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-image-11-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3607 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-image-11-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18997 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4862 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7763 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6768 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4632 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-13-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3834 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-13-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6070 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-14-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3551 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-14-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6056 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-15-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4024 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-15-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24861 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/styling-pres-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9352 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/styling-pres-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    40319 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/svgdom-over-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8040 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/svgdom-over-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8542 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13929 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20452 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5572 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24608 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5410 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7013 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6746 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18793 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-05-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7071 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    41270 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6560 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20310 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6180 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13096 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3502 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26379 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-04-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9585 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-04-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    24883 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-05-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5146 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9597 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-06-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5190 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-06-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13434 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-07-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6288 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-07-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    27349 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-08-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8417 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-08-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7350 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4126 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7397 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4788 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7506 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4799 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7397 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4628 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7316 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3830 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.276041 CairoSVG-2.7.1/test_non_regression/fail/path/
+-rw-r--r--   0 lize      (1000) lize      (1000)      363 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/path/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)     5156 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/path/paths-data-18-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4726 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/path/paths-data-18-f.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.283041 CairoSVG-2.7.1/test_non_regression/fail/text/
+-rw-r--r--   0 lize      (1000) lize      (1000)      460 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    10718 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/styling-css-05-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3815 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/styling-css-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    22700 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3974 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20507 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-05-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3981 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    14330 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-06-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4743 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-06-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11059 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-07-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4714 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9132 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-08-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4826 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-align-08-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    19582 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6770 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    15957 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    17278 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    18828 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    18401 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10028 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-bidi-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3190 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-bidi-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    36556 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-deco-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4100 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-deco-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26203 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5278 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    22378 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-02-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4914 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17952 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-03-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7279 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17952 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4212 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7046 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-05-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2980 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    30341 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-202-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5153 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-202-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    23273 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-203-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6498 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-203-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    25143 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-204-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6129 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-204-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26424 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5301 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17870 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-02-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4692 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16629 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4859 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    27205 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4455 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16824 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-05-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4205 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13298 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-06-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4786 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    20255 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-07-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3237 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    17910 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-09-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4764 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-09-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    16847 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-10-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4315 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-10-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    15955 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-11-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4758 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-11-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12313 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-12-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4480 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-12-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    31007 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-spacing-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3784 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-spacing-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    73363 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-01-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10257 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26482 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-03-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5248 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12954 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    11509 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12351 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-05-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8364 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7969 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-06-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7434 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13842 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-12-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8863 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/text-text-12-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10455 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/textdecoration01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1076 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/text/textdecoration01.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.284042 CairoSVG-2.7.1/test_non_regression/fail/use/
+-rw-r--r--   0 lize      (1000) lize      (1000)      828 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)    29471 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-05-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4910 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6764 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-06-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3514 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-06-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11701 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-08-b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3876 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-08-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6415 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-12-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5877 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-12-f.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.284042 CairoSVG-2.7.1/test_non_regression/fail/viewbox/
+-rw-r--r--   0 lize      (1000) lize      (1000)      550 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/viewbox/README.rst
+-rw-r--r--   0 lize      (1000) lize      (1000)      862 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-01-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2438 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6330 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-04-t.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3590 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-04-t.svg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.300042 CairoSVG-2.7.1/test_non_regression/images/
+-rw-r--r--   0 lize      (1000) lize      (1000)     1038 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/20x20.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      238 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/50x50-viewbox-greencircle.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/50x50greencircle.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2470 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/DisplaceChecker.png
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.313042 CairoSVG-2.7.1/test_non_regression/images/PngSuite/
+-rw-r--r--   0 lize      (1000) lize      (1000)      217 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi0g01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      154 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi0g02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      247 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      254 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      299 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      315 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      595 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      132 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      193 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      327 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1527 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi4a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2855 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi4a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      361 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi6a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     4180 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi6a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      164 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn0g01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      104 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn0g02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      145 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      138 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      167 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      145 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      302 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      112 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      146 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1286 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      126 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn4a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2206 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn4a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      184 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn6a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3435 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn6a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgai4a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2855 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgai4a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      184 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgan6a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3435 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgan6a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      140 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgbn4a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2220 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bggn4a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      202 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgwn6a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3453 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgyn6a16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1514 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ccwn2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1554 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ccwn3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      404 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cdfn2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      344 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cdhn2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      232 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cdsn2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      724 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cdun2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      258 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ch1n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1810 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ch2n3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      292 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cm0n0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      292 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cm7n0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      292 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cm9n0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cs3n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      259 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cs3n3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      186 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cs5n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      271 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cs5n3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      149 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cs8n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      256 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/cs8n3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      273 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ct0n0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      792 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ct1n0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      753 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ctzn0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      319 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f00n0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2475 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f00n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      321 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f01n0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1180 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f01n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      355 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f02n0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1729 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f02n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      389 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f03n0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1291 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f03n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      269 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f04n0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      985 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/f04n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      345 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g03n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      370 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g03n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g03n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      363 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g04n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      377 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g04n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      219 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g04n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      339 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g05n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      350 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g05n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      206 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g05n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      321 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g07n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      340 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g07n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      207 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g07n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      262 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g10n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      285 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g10n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      214 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g10n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      383 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g25n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      405 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g25n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      215 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/g25n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      167 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi1n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      302 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi1n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      179 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi2n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      314 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi2n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      203 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi4n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      338 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi4n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1283 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi9n0g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3038 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi9n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    20519 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/pngsuite.doc
+-rw-r--r--   0 lize      (1000) lize      (1000)     2262 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/pngsuite_logo.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      962 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/pp0n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      818 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/pp0n6a08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1477 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps1n0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1641 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps1n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2341 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps2n0g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2505 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps2n2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      113 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s01i3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      113 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s01n3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      114 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s02i3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      115 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s02n3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      118 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s03i3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      120 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s03n3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      126 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s04i3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      121 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s04n3p01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      134 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s05i3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      129 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s05n3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      143 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s06i3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      131 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s06n3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      149 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s07i3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      138 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s07n3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      149 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s08i3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      139 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s08n3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      147 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s09i3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      143 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s09n3p02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      355 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s32i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      263 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s32n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      385 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s33i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      329 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s33n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      349 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s34i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      248 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s34n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      399 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s35i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      338 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s35n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      356 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s36i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      258 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s36n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      393 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s37i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      336 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s37n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      357 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s38i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      245 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s38n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      420 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s39i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      352 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s39n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      357 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s40i3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      256 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/s40n3p04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      419 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbbn1g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1994 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbbn2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1128 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbbn3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1994 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbgn2c16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1128 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbgn3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1347 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbrn2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1146 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbwn1g16.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1131 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbwn3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1131 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbyn3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      689 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp0n1g08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1311 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp0n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1120 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp0n3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1115 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp1n3p08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)       49 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/x00n0g01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      261 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/xcrn0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      240 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/xlfn0g04.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3172 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/z00n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      232 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/z03n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      224 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/z06n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      224 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/PngSuite/z09n2c08.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    57657 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/SVG-1.1-monolithic-fixed.dtd
+-rw-r--r--   0 lize      (1000) lize      (1000)     1722 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/SVGImageTest.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13238 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/animation-add-BE-09.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      951 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/animation-extRef-image1.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      844 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/animation-extRef-image2.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      725 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/animation-extRef-image3.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/black10x10.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      159 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/blue1x1.png
+-rw-r--r--   0 lize      (1000) lize      (1000)       83 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/blue_10x10.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      833 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/blue_10x10.ppm
+-rw-r--r--   0 lize      (1000) lize      (1000)    37497 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/bluesquidj.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      973 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/bullet-small.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      971 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/bullet-white.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      972 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/bullet.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1998 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/bumpMap.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      657 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/bumpMap2.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      433 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/bumpMap3.png
+-rw-r--r--   0 lize      (1000) lize      (1000)       35 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/case-insensitivity.css
+-rw-r--r--   0 lize      (1000) lize      (1000)      740 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/changeColor.ICM
+-rw-r--r--   0 lize      (1000) lize      (1000)      705 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/colorprof.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     9281 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/convolveImage.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    29842 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/coords-units-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13340 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/coords-units-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4750 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/copyright-documents-19990405.html
+-rw-r--r--   0 lize      (1000) lize      (1000)      997 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/diagarrow.png
+-rw-r--r--   0 lize      (1000) lize      (1000)        0 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/empty.js
+-rw-r--r--   0 lize      (1000) lize      (1000)     3697 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/ext-TestComic.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)        4 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/f.js
+-rw-r--r--   0 lize      (1000) lize      (1000)      740 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/fillChangeColor.ICM
+-rw-r--r--   0 lize      (1000) lize      (1000)     7343 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-blend-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7818 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-color-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9754 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-composite-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7805 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-comptran-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9281 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-conv-01-f.includeimage.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7987 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-conv-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10092 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-diffuse-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7577 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/filters-example-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    48928 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/footprints.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)   313676 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/footprints2.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12435 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/galpha.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      213 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam030.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1029 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam030b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam045.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1059 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam045b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      216 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam056.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1059 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam056b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      205 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam100.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1044 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam100b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      187 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam200.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1019 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/gam200b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      159 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/green1x1.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1111 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/greentopbutton.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)      612 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/happysmiley.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1884 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/image.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    34183 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/image1.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)   394416 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/image1.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    12586 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/image1_b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     6643 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/image2_b.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7412 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/image2_b.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1541 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/inline2.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7566 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/interact-dom-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2921 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/interact-order-02-b-targ.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2936 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/interact-order-03-b-targ.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      124 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/leftarrow.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      153 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/level1.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      140 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/level2.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8845 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8183 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-1st.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    34164 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-2nd.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    34164 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-3rd.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13626 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-4th.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    34164 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-start.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    28465 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-03-f-1st.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    26549 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linking-uri-03-f-start.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1919 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linkingCircle-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2649 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/linkingToc-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      268 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/magnify.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1985 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/makealpha.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4402 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/myimage.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)      264 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_bullet.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      252 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_down.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      170 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_downleft.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      169 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_downright.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      155 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_frame.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      166 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_left.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      270 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_noframe.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      168 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_right.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      155 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_svg.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      173 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_up.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      172 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_upleft.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      173 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/nav_upright.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    36641 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/old-name-2-new-name1.html
+-rw-r--r--   0 lize      (1000) lize      (1000)    36446 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13254 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    42041 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-02-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10827 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    38026 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-03-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    10687 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    30546 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-04-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    14511 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/paths-data-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    31090 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/pinksquidj.png
+-rw-r--r--   0 lize      (1000) lize      (1000)   145806 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/plant.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)    48672 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/purplesquidj.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      500 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/rects.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      419 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/rects_b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      159 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/red1x1.png
+-rw-r--r--   0 lize      (1000) lize      (1000)    13717 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/rgbalpha.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      963 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/rightarrow.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     1434 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/rotate20.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      274 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/selector-types-fill-green.css
+-rw-r--r--   0 lize      (1000) lize      (1000)      374 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/selector-types-visibility-hidden.css
+-rw-r--r--   0 lize      (1000) lize      (1000)     3247 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/shapes-ellipse-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    31126 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/shapes-ellipse-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     7752 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/shapes-ellipse-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3445 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/shapes-rect-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26453 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/shapes-rect-01-f.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     8003 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/shapes-rect-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10647 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/sign.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     2856 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/smiley.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     5923 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/sphere.png
+-rwxr-xr-x   0 lize      (1000) lize      (1000)     1499 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/star.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12777 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/stefan_252_tRNS_opti.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3141 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-frag-01-B.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4751 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-01.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)    63238 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)     3779 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-02.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)    35887 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-02.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      320 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-11-b-1.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      333 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-11-b-2.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      448 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-12-b-cycle.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      455 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-12-b-nocycle.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      287 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-image-17-b-1.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    71497 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-symbol-01.png
+-rw-r--r--   0 lize      (1000) lize      (1000)      521 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-use-06-b-1.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      529 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/struct-use-08-b-cycles.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2376 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/svgRef1.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)       92 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/svgRef4.css
+-rw-r--r--   0 lize      (1000) lize      (1000)     1632 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/svgRef4.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5992 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-align-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8674 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-align-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6069 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-align-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11291 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-altglyph-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2352 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-extTref-BE-18-targ.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8077 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-intro-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9985 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-tref-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9374 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/text-ws-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3191 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/toc-sv.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3251 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/toc-svcmp.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    52480 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/townsville.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)    66460 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/tree.jpg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1232 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/images/uparrow.png
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.314042 CairoSVG-2.7.1/test_non_regression/resources/
+-rw-r--r--   0 lize      (1000) lize      (1000)    22708 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/Anglepoise.otf
+-rw-r--r--   0 lize      (1000) lize      (1000)     1860 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/Blocky.otf
+-rw-r--r--   0 lize      (1000) lize      (1000)   166392 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/CalaLig.otf
+-rw-r--r--   0 lize      (1000) lize      (1000)    15656 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/FreeSerif.otf
+-rw-r--r--   0 lize      (1000) lize      (1000)    15360 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/FreeSerifBold.otf
+-rw-r--r--   0 lize      (1000) lize      (1000)    17636 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/FreeSerifBoldItalic.otf
+-rw-r--r--   0 lize      (1000) lize      (1000)    20924 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/FreeSerifItalic.otf
+-rw-r--r--   0 lize      (1000) lize      (1000)    26220 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/resources/SVGFreeSans.otf
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-08-05 09:02:26.339043 CairoSVG-2.7.1/test_non_regression/svg/
+-rw-r--r--   0 lize      (1000) lize      (1000)      816 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/svg/InitialCoords.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1538 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/svg/Nested.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1233 2022-12-27 11:37:30.000000 CairoSVG-2.7.1/test_non_regression/svg/NewCoordSys.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      655 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/OrigCoordSys.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4086 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/PreserveAspectRatio.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1508 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/RotateScale.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1516 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/Skew.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1837 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/Units.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1090 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/ViewBox.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      999 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/arcs01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2387 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/arcs02.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      583 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/circle01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4128 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/color-prop-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6324 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/color-prop-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5422 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/color-prop-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5806 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/color-prop-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3175 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/color-prop-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2188 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/conform-viewers-01-t.svgz
+-rw-r--r--   0 lize      (1000) lize      (1000)     4070 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/conform-viewers-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3619 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-coord-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3628 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-coord-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12864 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9961 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5473 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4908 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4953 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4192 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3913 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4128 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-08-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4892 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-09-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4346 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-10-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4354 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-11-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4405 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-12-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4286 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-13-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4458 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-trans-14-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5001 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4527 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3794 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3551 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4382 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11342 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-units-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8314 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-units-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9072 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-units-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8509 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    53178 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6064 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7005 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1857 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/cubic01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5443 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/cubic02.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      709 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/ellipse01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1948 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/feBlend.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2995 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/fillrule-evenodd.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2994 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/fillrule-nonzero.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4141 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/filters-offset-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2870 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/imp-path-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      784 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/inheritance.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      911 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/line01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1789 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linecap.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1684 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linejoin.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      879 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/lingrad01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6414 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-a-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5740 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-a-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5860 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-a-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3214 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-a-08-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3761 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-frag-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8847 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-uri-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9537 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-uri-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5464 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/linking-uri-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      805 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/marker.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1383 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/mask01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4003 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-filter-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7239 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-mask-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2805 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-mask-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5995 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-opacity-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5047 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4541 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6772 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4003 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-04-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3862 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-06-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5760 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-08-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2801 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-13-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4238 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/masking-path-14-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    21666 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/metadata-example-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1952 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/opacity01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5238 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-control-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3497 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-control-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3400 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-control-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5839 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-control-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3408 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-control-06-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3551 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-fill-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3711 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-fill-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3488 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-fill-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4352 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-fill-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4502 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-fill-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    10160 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-marker-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    13254 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-marker-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5040 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-marker-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12550 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-marker-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9894 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-marker-06-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3899 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3727 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3758 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3827 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5369 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4032 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3855 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4737 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-08-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3245 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-09-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    11078 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8577 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     8433 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5482 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5328 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5520 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5448 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5355 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-08-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5268 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-09-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5896 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-10-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3945 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-12-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3149 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-13-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3628 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-14-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3555 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-15-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3273 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-16-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3309 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-17-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5939 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/paths-data-19-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      859 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pattern01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      821 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/polygon01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      852 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/polyline01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3902 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4696 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4428 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5034 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-04-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5501 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6668 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-06-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5130 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-07-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5472 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-08-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6779 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-09-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5644 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-10-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7514 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-11-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6758 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-12-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     9242 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-13-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6443 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-14-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3773 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-15-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4408 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-16-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5433 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-17-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5634 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-18-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4961 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-20-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6614 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-21-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4269 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-22-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3835 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-23-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3598 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-24-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3846 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-stops-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6524 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2939 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4585 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3652 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3492 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3273 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-06-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3419 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-07-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3413 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-08-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3683 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-09-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1135 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/quad01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1026 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/radgrad01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      581 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/rect01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      714 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/rect02.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3337 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-elems-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3403 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-elems-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3513 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-elems-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3658 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-elems-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3619 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-elems-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3684 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-elems-08-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6712 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-groups-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6004 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/render-groups-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3192 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-circle-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3235 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-circle-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4439 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-ellipse-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3197 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-ellipse-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3815 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-ellipse-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3330 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-grammar-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6517 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-intro-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4847 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-intro-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4390 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-line-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2758 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-line-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4842 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-polygon-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4184 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-polygon-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3159 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-polygon-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5435 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-polyline-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4328 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-polyline-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4641 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3380 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6546 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3396 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4015 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3562 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-06-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2921 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-07-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3230 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-cond-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    26599 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-cond-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4189 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-cond-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4062 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-02-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3347 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3443 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3821 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3513 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-defs-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3554 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-frag-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3611 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-frag-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4942 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-frag-05-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4767 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-frag-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4231 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-group-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4436 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-group-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    12165 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-group-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3289 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5000 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)    32937 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-04-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3096 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-05-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5562 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-06-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3932 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3159 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-08-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3161 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-09-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3157 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-10-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5522 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-13-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5517 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-14-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6635 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-15-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2706 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-16-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3156 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-17-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3152 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-18-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3368 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-image-19-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3111 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-svg-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5049 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-symbol-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5603 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-use-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3756 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-use-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4399 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-use-07-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3852 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-use-09-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5176 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-use-10-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5940 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/struct-use-11-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3363 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-class-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4160 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4137 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5246 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     7242 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2899 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-07-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4884 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-08-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4404 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-09-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3559 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-css-10-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3519 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-elem-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4258 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-inherit-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3395 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-pres-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     2773 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-pres-03-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4049 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-pres-04-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3615 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/styling-pres-05-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4138 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-align-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3996 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-align-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4939 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-align-04-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4931 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-path-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4941 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-path-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4255 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-text-07-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3766 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-text-08-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4579 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-text-09-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4553 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-text-10-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4903 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-text-11-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3737 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-tref-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3698 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-tref-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3749 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-tref-03-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6449 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-tspan-01-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     6546 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-tspan-02-b.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5664 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-ws-01-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     5769 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-ws-02-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     4026 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text-ws-03-t.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      595 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/text01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      929 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/toap01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1040 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/toap02.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      973 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/toap03.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      979 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/toap04.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      865 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/tref01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      542 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/triangle01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1139 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/test_non_regression/svg/tspan-dx-dy.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      685 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/tspan01.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      813 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/tspan02.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      808 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/tspan03.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      677 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/tspan04.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     1100 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/tspan05.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)     3521 2022-12-27 11:37:31.000000 CairoSVG-2.7.1/test_non_regression/svg/types-basic-01-f.svg
+-rw-r--r--   0 lize      (1000) lize      (1000)      914 2022-12-27 11:39:42.000000 CairoSVG-2.7.1/test_non_regression/test_helpers.py
+-rw-r--r--   0 lize      (1000) lize      (1000)     1270 2023-08-05 08:56:20.000000 CairoSVG-2.7.1/test_non_regression/test_non_regression.py
```

### Comparing `CairoSVG-2.7.0/.github/workflows/tests.yml` & `CairoSVG-2.7.1/.github/workflows/tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 on: [push, pull_request]
 
 jobs:
   tests:
     name: ${{ matrix.os }} - ${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
     strategy:
-      fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version:
-          - "3.7"
-          - "3.8"
-          - "3.9"
-          - "3.10"
-          - "3.11"
+        python-version: ['3.7', '3.11']
     steps:
       - uses: actions/checkout@v3
         with:
           submodules: true
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `CairoSVG-2.7.0/CairoSVG.egg-info/PKG-INFO` & `CairoSVG-2.7.1/CairoSVG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CairoSVG
-Version: 2.7.0
+Version: 2.7.1
 Summary: A Simple SVG Converter based on Cairo
 Home-page: https://courtbouillon.org/cairosvg
 Author: Guillaume Ayoub
 Author-email: contact@courtbouillon.org
 License: LGPLv3+
 Project-URL: Documentation, https://cairosvg.org/documentation/
 Project-URL: Code, https://github.com/Kozea/CairoSVG/
```

### Comparing `CairoSVG-2.7.0/CairoSVG.egg-info/SOURCES.txt` & `CairoSVG-2.7.1/CairoSVG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/LICENSE` & `CairoSVG-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/NEWS.rst` & `CairoSVG-2.7.1/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 ======
  News
 ======
 
 
+Version 2.7.1 released on 2023-08-05
+====================================
+
+- Don’t draw clipPath when defined after reference
+- Handle evenodd fill rule with gradients and patterns
+- Fix ratio and clip for "image" tags with no size
+- Handle data-URLs in safe mode
+- Use f-strings
+
+
 Version 2.7.0 released on 2023-03-20
 ====================================
 
 **WARNING:** this is a security update.
 
 When processing SVG files, CairoSVG could access other files online, possibly
 leading to very long renderings or other security problems.
```

### Comparing `CairoSVG-2.7.0/PKG-INFO` & `CairoSVG-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CairoSVG
-Version: 2.7.0
+Version: 2.7.1
 Summary: A Simple SVG Converter based on Cairo
 Home-page: https://courtbouillon.org/cairosvg
 Author: Guillaume Ayoub
 Author-email: contact@courtbouillon.org
 License: LGPLv3+
 Project-URL: Documentation, https://cairosvg.org/documentation/
 Project-URL: Code, https://github.com/Kozea/CairoSVG/
```

### Comparing `CairoSVG-2.7.0/README.rst` & `CairoSVG-2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/cairosvg/__init__.py` & `CairoSVG-2.7.1/cairosvg/__init__.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/cairosvg/__main__.py` & `CairoSVG-2.7.1/cairosvg/__main__.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/cairosvg/bounding_box.py` & `CairoSVG-2.7.1/cairosvg/bounding_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 def bounding_box_path(surface, node):
     """Get the bounding box of a ``path`` node."""
     path_data = node.get('d', '')
 
     # Normalize path data for correct parsing
     for letter in PATH_LETTERS:
-        path_data = path_data.replace(letter, ' {} '.format(letter))
+        path_data = path_data.replace(letter, f' {letter} ')
     path_data = normalize(path_data)
 
     bounding_box = EMPTY_BOUNDING_BOX
     previous_x = 0
     previous_y = 0
     letter = 'M'    # Move as default
     while path_data:
```

### Comparing `CairoSVG-2.7.0/cairosvg/colors.py` & `CairoSVG-2.7.1/cairosvg/colors.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/cairosvg/css.py` & `CairoSVG-2.7.1/cairosvg/css.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/cairosvg/defs.py` & `CairoSVG-2.7.1/cairosvg/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """Update the attributes of the def according to its href attribute."""
     def_node = def_dict[def_name]
     href = parse_url(def_node.get_href()).fragment
     if href in def_dict:
         update_def_href(surface, href, def_dict)
         href_node = def_dict[href]
         def_dict[def_name] = Tree(
-            url='#{}'.format(def_name), url_fetcher=def_node.url_fetcher,
+            url=f'#{def_name}', url_fetcher=def_node.url_fetcher,
             parent=href_node, parent_children=(not def_node.children),
             tree_cache=surface.tree_cache, unsafe=def_node.unsafe)
         # Inherit attributes generally not inherited
         for key, value in href_node.items():
             if key not in def_dict[def_name]:
                 def_dict[def_name][key] = value
 
@@ -60,15 +60,15 @@
 
 def parse_def(surface, node):
     """Parse the SVG definitions."""
     for def_type in (
             'marker', 'gradient', 'pattern', 'path', 'mask', 'filter',
             'image'):
         if def_type in node.tag.lower() and 'id' in node:
-            getattr(surface, '{}s'.format(def_type))[node['id']] = node
+            getattr(surface, f'{def_type}s')[node['id']] = node
 
 
 def gradient_or_pattern(surface, node, name, opacity):
     """Gradient or pattern color."""
     if name in surface.gradients:
         update_def_href(surface, name, surface.gradients)
         return draw_gradient(surface, node, name, opacity)
@@ -135,17 +135,15 @@
         surface, mask_node.get('height', '120%'), height_ref)
     mask_node['width'] = size(
         surface, mask_node.get('width', '120%'), width_ref)
 
     if mask_node.get('maskUnits') == 'userSpaceOnUse':
         x = mask_node['x']
         y = mask_node['y']
-        mask_node['viewBox'] = '{} {} {} {}'.format(
-            mask_node['x'], mask_node['y'],
-            mask_node['width'], mask_node['height'])
+        mask_node['viewBox'] = '{x} {y} {width} {height}'.format(**mask_node)
 
     from .surface import SVGSurface  # circular import
     mask_surface = SVGSurface(mask_node, None, surface.dpi, surface)
     surface.context.save()
     surface.context.translate(x, y)
     surface.context.scale(
         mask_node['width'] / mask_surface.width,
@@ -244,16 +242,15 @@
             size(surface, pattern_node.pop('width', '1'), 1) * width)
         pattern_height = (
             size(surface, pattern_node.pop('height', '1'), 1) * height)
         if 'viewBox' not in pattern_node:
             pattern_node['width'] = pattern_width
             pattern_node['height'] = pattern_height
             if pattern_node.get('patternContentUnits') == 'objectBoundingBox':
-                pattern_node['transform'] = 'scale({}, {})'.format(
-                    width, height)
+                pattern_node['transform'] = f'scale({width}, {height})'
 
     # Fail if pattern has an invalid size
     if pattern_width == 0.0 or pattern_height == 0.0:
         return False
 
     from .surface import SVGSurface  # circular import
     pattern_surface = SVGSurface(pattern_node, None, surface.dpi, surface)
```

### Comparing `CairoSVG-2.7.0/cairosvg/features.py` & `CairoSVG-2.7.1/cairosvg/features.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/cairosvg/helpers.py` & `CairoSVG-2.7.1/cairosvg/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,17 @@
     elif node.tag in ('svg', 'image', 'g'):
         node_width, node_height, _ = node_format(surface, node)
         width = width or node_width
         height = height or node_height
         viewbox_width, viewbox_height = node.image_width, node.image_height
     else:
         raise TypeError(
-            ('Root node is {}. Should be one of '
-             'marker, svg, image, or g.').format(node.tag))
+            f'Root node is {node.tag}. Should be one of '
+            'marker, svg, image, or g.'
+        )
 
     translate_x = 0
     translate_y = 0
     scale_x = width / viewbox_width if viewbox_width > 0 else 1
     scale_y = height / viewbox_height if viewbox_height > 0 else 1
 
     aspect_ratio = node.get('preserveAspectRatio', 'xMidYMid').split()
```

### Comparing `CairoSVG-2.7.0/cairosvg/image.py` & `CairoSVG-2.7.1/cairosvg/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,18 @@
     image_surface = cairo.ImageSurface.create_from_png(png_file)
     image_surface.pattern = cairo.SurfacePattern(image_surface)
     image_surface.pattern.set_filter(IMAGE_RENDERING.get(
         node.get('image-rendering'), cairo.FILTER_GOOD))
 
     node.image_width = image_surface.get_width()
     node.image_height = image_surface.get_height()
+    width = width or node.image_width
+    height = height or node.image_height
     scale_x, scale_y, translate_x, translate_y = preserve_ratio(
-        surface, node)
+        surface, node, width, height)
 
     # Clip image region (if necessary)
     if not (translate_x == 0 and
             translate_y == 0 and
             width == scale_x * node.image_width and
             height == scale_y * node.image_height):
         surface.context.rectangle(x, y, width, height)
```

### Comparing `CairoSVG-2.7.0/cairosvg/parser.py` & `CairoSVG-2.7.1/cairosvg/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import cssselect2
 from defusedxml import ElementTree
 
 from . import css
 from .features import match_features
 from .helpers import flatten, pop_rotation, rotations
-from .url import fetch, parse_url, read_url
+from .url import fetch, parse_url, read_url, safe_fetch
 
 # 'display' is actually inherited but handled differently because some markers
 # are part of a none-displaying group (see test painting-marker-07-f.svg)
 NOT_INHERITED_ATTRIBUTES = frozenset((
     'clip',
     'clip-path',
     'display',
@@ -164,15 +164,15 @@
 
         node = element.etree_element
         self.element = element
         self.style = style
         self.tag = (
             element.local_name
             if element.namespace_url in ('', 'http://www.w3.org/2000/svg') else
-            '{%s}%s' % (element.namespace_url, element.local_name))
+            f'{{{element.namespace_url}}}{element.local_name}')
         self.text = node.text
         self.url_fetcher = url_fetcher
         self.unsafe = unsafe
 
         # Only set xml_tree if it's not been set before (ie. if node is a tree)
         self.xml_tree = getattr(self, 'xml_tree', node)
 
@@ -389,29 +389,28 @@
                 bytestring = gzip.decompress(bytestring)
             tree = ElementTree.fromstring(
                 bytestring, forbid_entities=not unsafe,
                 forbid_external=not unsafe)
 
         # Don’t allow fetching external files unless explicitly asked for
         if 'url_fetcher' not in kwargs and not unsafe:
-            self.url_fetcher = (
-                lambda *args, **kwargs: b'<svg width="1" height="1"></svg>')
+            self.url_fetcher = safe_fetch
 
         self.xml_tree = tree
         root = cssselect2.ElementWrapper.from_xml_root(tree)
         style = parent.style if parent else css.parse_stylesheets(self, url)
         if element_id:
             for element in root.iter_subtree():
                 if element.id == element_id:
                     root = element
                     self.xml_tree = element.etree_element
                     break
             else:
                 raise TypeError(
-                    'No tag with id="{}" found.'.format(element_id))
+                    f'No tag with id="{element_id}" found.')
         super().__init__(
             root, style, self.url_fetcher, parent, parent_children, self.url,
             unsafe)
         self.root = True
         if tree_cache is not None and self.url:
             tree_cache[(self.url, self.get('id'))] = self
```

### Comparing `CairoSVG-2.7.0/cairosvg/path.py` & `CairoSVG-2.7.1/cairosvg/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """Draw the markers attached to a path ``node``."""
     if not getattr(node, 'vertices', None):
         return
 
     markers = {}
     common_marker = parse_url(node.get('marker', '')).fragment
     for position in ('start', 'mid', 'end'):
-        attribute = 'marker-{}'.format(position)
+        attribute = f'marker-{position}'
         if attribute in node:
             markers[position] = parse_url(node[attribute]).fragment
         else:
             markers[position] = common_marker
 
     angle1, angle2 = None, None
     position = 'start'
@@ -121,15 +121,15 @@
 def path(surface, node):
     """Draw a path ``node``."""
     string = node.get('d', '')
 
     node.vertices = []
 
     for letter in PATH_LETTERS:
-        string = string.replace(letter, ' {} '.format(letter))
+        string = string.replace(letter, f' {letter} ')
 
     last_letter = None
     string = normalize(string)
 
     # Keep the current point because Cairo's get_current_point is not accurate
     # enough. See https://github.com/Kozea/CairoSVG/issues/111.
     if surface.context.has_current_point():
@@ -186,18 +186,18 @@
 
             # rx=0 or ry=0 means straight line
             if not rx or not ry:
                 if string and string[0] not in PATH_LETTERS:
                     # As we replace the current operation by l, we must be sure
                     # that the next letter is set to the real current letter (a
                     # or A) in case it’s omitted
-                    next_letter = '{} '.format(letter)
+                    next_letter = f'{letter} '
                 else:
                     next_letter = ''
-                string = 'l {} {} {}{}'.format(x3, y3, next_letter, string)
+                string = f'l {x3} {y3} {next_letter}{string}'
                 continue
 
             radii_ratio = ry / rx
 
             # Cancel the rotation of the second point
             xe, ye = rotate(x3, y3, -rotation)
             ye /= radii_ratio
```

### Comparing `CairoSVG-2.7.0/cairosvg/shapes.py` & `CairoSVG-2.7.1/cairosvg/shapes.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/cairosvg/surface.py` & `CairoSVG-2.7.1/cairosvg/surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,14 +382,15 @@
                     height = size(self, node.get('height'), 'y')
                     self.context.translate(x, y)
                     self.context.scale(width, height)
                 path.tag = 'g'
                 self.stroke_and_fill = False
                 self.draw(path)
                 self.stroke_and_fill = True
+                path.tag = 'clipPath'
                 self.context.restore()
                 # TODO: fill rules are not handled by cairo for clips
                 # if node.get('clip-rule') == 'evenodd':
                 #     self.context.set_fill_rule(cairo.FILL_RULE_EVEN_ODD)
                 self.context.clip()
                 self.context.set_fill_rule(cairo.FILL_RULE_WINDING)
 
@@ -430,17 +431,17 @@
         self.context.set_font_options(font_options)
 
         # Fill and stroke
         if self.stroke_and_fill and visible and node.tag in TAGS:
             # Fill
             self.context.save()
             paint_source, paint_color = paint(node.get('fill', 'black'))
+            if node.get('fill-rule') == 'evenodd':
+                self.context.set_fill_rule(cairo.FILL_RULE_EVEN_ODD)
             if not gradient_or_pattern(self, node, paint_source, fill_opacity):
-                if node.get('fill-rule') == 'evenodd':
-                    self.context.set_fill_rule(cairo.FILL_RULE_EVEN_ODD)
                 self.context.set_source_rgba(
                     *self.map_color(paint_color, fill_opacity))
             if TAGS[node.tag] == text:
                 self.cursor_position = save_cursor[0]
                 self.cursor_d_position = save_cursor[1]
                 self.text_path_width = save_cursor[2]
                 text(self, node, draw_as_text=True)
```

### Comparing `CairoSVG-2.7.0/cairosvg/test_api.py` & `CairoSVG-2.7.1/cairosvg/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         temp_0 = os.path.join(temp, 'sample_0.svg')
         with open(temp_0, 'wb') as file_object:
             file_object.write(SVG_SAMPLE)
 
         # Read from a filename
         assert svg2png(url=temp_0) == expected_content
         assert svg2png(
-            url='file://{}'.format(temp_0)) == expected_content
+            url=f'file://{temp_0}') == expected_content
 
         with open(temp_0, 'rb') as file_object:
             # Read from a real file object
             assert svg2png(file_obj=file_object) == expected_content
 
         temp_1 = os.path.join(temp, 'result_1.png')
         with open(temp_1, 'wb') as file_object:
```

### Comparing `CairoSVG-2.7.0/cairosvg/text.py` & `CairoSVG-2.7.1/cairosvg/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
 
 def text(surface, node, draw_as_text=False):
     """Draw a text ``node``."""
     font_family = (
         (node.get('font-family') or 'sans-serif').split(',')[0].strip('"\' '))
     font_style = getattr(
-        cairo, ('font_slant_{}'.format(node.get('font-style')).upper()),
+        cairo, f'font_slant_{node.get("font-style")}'.upper(),
         cairo.FONT_SLANT_NORMAL)
     node_font_weight = node.get('font-weight')
     if (node_font_weight and node_font_weight.isdigit()
             and int(node_font_weight) >= 550):
         node_font_weight = 'bold'
     font_weight = getattr(
-        cairo, ('font_weight_{}'.format(node_font_weight).upper()),
+        cairo, (f'font_weight_{node_font_weight}'.upper()),
         cairo.FONT_WEIGHT_NORMAL)
     surface.context.select_font_face(font_family, font_style, font_weight)
     surface.context.set_font_size(surface.font_size)
     ascent, descent, _, max_x_advance, max_y_advance = (
         surface.context.font_extents())
 
     text_path_href = parse_url(node.get_href() or node.parent.get_href() or '')
```

### Comparing `CairoSVG-2.7.0/cairosvg/url.py` & `CairoSVG-2.7.1/cairosvg/url.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 from pathlib import Path
 from urllib.parse import urljoin, urlparse
 from urllib.request import Request, urlopen
 
 from . import VERSION
 
-HTTP_HEADERS = {'User-Agent': 'CairoSVG {}'.format(VERSION)}
+HTTP_HEADERS = {'User-Agent': f'CairoSVG {VERSION}'}
 
 URL = re.compile(r'url\((.+)\)')
 
 
 def normalize_url(url):
     """Normalize ``url`` for underlying NT/Unix operating systems.
 
@@ -80,14 +80,25 @@
     ``resource_type`` is the mimetype of the resource (currently one of
     image/*, image/svg+xml, text/css).
 
     """
     return urlopen(Request(url, headers=HTTP_HEADERS)).read()
 
 
+def safe_fetch(url, resource_type):
+    """Fetch the content of ``url`` only if it’s a data-URL.
+
+    Otherwise, return an empty SVG.
+
+    """
+    if url and url.startswith('data:'):
+        return fetch(url, resource_type)
+    return b'<svg width="1" height="1"></svg>'
+
+
 def parse_url(url, base=None):
     """Parse an URL.
 
     The URL can be surrounded by a ``url()`` string. If ``base`` is not `None`,
     the "folder" part of it is prepended to the URL.
 
     """
@@ -117,15 +128,15 @@
                             url = os.path.join(
                                 parsed_base_path, parsed_url_path)
                         else:
                             url = ''
                     else:
                         url = ''
                     if parsed_url.fragment:
-                        url = '{}#{}'.format(url, parsed_url.fragment)
+                        url = f'{url}#{parsed_url.fragment}'
             elif parsed_url.scheme in ('', parsed_base.scheme):
                 # `urljoin` automatically uses the "folder" part of `base`
                 url = urljoin(base, url)
         url = normalize_url(url.strip('\'"'))
     return urlparse(url or '')
 
 
@@ -133,11 +144,11 @@
     """Get bytes in a parsed ``url`` using ``url_fetcher``.
 
     If ``url_fetcher`` is None a default (no limitations) URLFetcher is used.
     """
     if url.scheme:
         url = url.geturl()
     else:
-        url = 'file://{}'.format(os.path.abspath(url.geturl()))
+        url = f'file://{os.path.abspath(url.geturl())}'
         url = normalize_url(url)
 
     return url_fetcher(url, resource_type)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CairoSVG-2.7.0/setup.cfg` & `CairoSVG-2.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/setup.py` & `CairoSVG-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/LICENSE` & `CairoSVG-2.7.1/test_non_regression/LICENSE`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/README.rst` & `CairoSVG-2.7.1/test_non_regression/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/__init__.py` & `CairoSVG-2.7.1/test_non_regression/__init__.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/cap/painting-control-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/cap/painting-control-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/cap/painting-control-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/cap/painting-control-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/cap/painting-stroke-10-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/cap/painting-stroke-10-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/cap/painting-stroke-10-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/cap/painting-stroke-10-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/color/color-prof-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/color/color-prof-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/color/color-prof-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/color/color-prof-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/color/painting-render-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/color/painting-render-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/css/struct-use-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/css/struct-use-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/draft/README.rst` & `CairoSVG-2.7.1/test_non_regression/fail/draft/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/draft/painting-marker-properties-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/draft/painting-marker-properties-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/draft/painting-marker-properties-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/draft/painting-marker-properties-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/draft/paths-data-20-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/draft/paths-data-20-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/draft/paths-data-20-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/draft/paths-data-20-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/draft/types-basic-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/draft/types-basic-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/draft/types-basic-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/draft/types-basic-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/README.rst` & `CairoSVG-2.7.1/test_non_regression/fail/filter/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/enable-background-01.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/enable-background-01.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/enable-background-01.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/enable-background-01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feColorMatrix.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feColorMatrix.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feColorMatrix.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feColorMatrix.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feComponentTransfer.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feComponentTransfer.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feComponentTransfer.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feComponentTransfer.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feComposite.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feComposite.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feComposite.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feComposite.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feMorphology.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feMorphology.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feMorphology.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feMorphology.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feTurbulence.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feTurbulence.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/feTurbulence.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/feTurbulence.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-background-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-background-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-background-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-background-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-blend-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-blend-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-blend-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-blend-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-color-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-color-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-05-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-05-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-composite-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-composite-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-comptran-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-comptran-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-comptran-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-comptran-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-05-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-05-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-conv-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-conv-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-diffuse-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-diffuse-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-diffuse-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-diffuse-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-displace-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-displace-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-example-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-example-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-example-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-example-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-felem-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-felem-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-gauss-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-gauss-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-05-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-05-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-image-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-image-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-05-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-05-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-light-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-light-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-morph-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-morph-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-morph-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-morph-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-offset-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-offset-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-offset-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-offset-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-overview-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-overview-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-specular-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-specular-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-specular-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-specular-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-tile-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-tile-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-tile-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-tile-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters-turb-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters-turb-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters00.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters00.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters00.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters00.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters01.png` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters01.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/filter/filters01.svg` & `CairoSVG-2.7.1/test_non_regression/fail/filter/filters01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-05-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-05-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-desc-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-desc-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-04-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-04-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-05-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-05-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-06-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-06-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-07-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-07-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-elem-07-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-elem-07-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-glyph-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-glyph-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-kern-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-kern-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-kern-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-kern-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-overview-201-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-overview-201-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/font/fonts-overview-201-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/font/fonts-overview-201-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/image/README.rst` & `CairoSVG-2.7.1/test_non_regression/fail/image/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-12-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-12-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/image/struct-image-12-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/image/struct-image-12-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-09-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-09-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-09-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-09-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-10-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-10-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/linking/linking-a-10-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/linking/linking-a-10-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-07-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-07-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/marker/painting-marker-07-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/marker/painting-marker-07-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/README.rst` & `CairoSVG-2.7.1/test_non_regression/fail/mask/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-intro-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-intro-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-intro-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-intro-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-05-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-05-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-07-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-07-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-07-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-07-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-10-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-10-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-11-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-11-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/mask/masking-path-11-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/mask/masking-path-11-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-dom-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-dom-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-05-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-05-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-06-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-06-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-07-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-07-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-08-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-08-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-08-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-08-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-09-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-09-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-09-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-09-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-10-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-10-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-10-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-10-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-11-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-11-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-11-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-11-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-12-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-12-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-12-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-12-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-13-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-13-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-13-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-13-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-14-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-14-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-14-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-14-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-15-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-15-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-15-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-15-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-17-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-17-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-17-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-17-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-19-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-19-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-19-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-19-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-20-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-20-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-20-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-20-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-21-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-21-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-21-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-21-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-22-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-22-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-22-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-22-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-23-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-23-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-23-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-23-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-24-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-24-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-24-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-24-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-25-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-25-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-25-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-25-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-26-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-26-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-26-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-26-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-27-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-27-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-27-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-27-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-28-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-28-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-28-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-28-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-29-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-29-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-29-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-29-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-30-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-30-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-30-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-30-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-31-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-31-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-31-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-31-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-32-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-32-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-32-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-32-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-33-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-33-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-33-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-33-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-34-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-34-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-34-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-34-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-35-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-35-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-35-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-35-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-36-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-36-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-36-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-36-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-37-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-37-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-37-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-37-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-38-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-38-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-38-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-38-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-39-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-39-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-39-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-39-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-40-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-40-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-40-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-40-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-41-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-41-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-41-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-41-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-42-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-42-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-43-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-43-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-44-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-44-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-44-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-44-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-45-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-45-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-46-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-46-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-46-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-46-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-47-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-47-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-48-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-48-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-49-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-49-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-50-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-50-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-51-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-51-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-52-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-52-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-52-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-52-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-53-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-53-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-53-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-53-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-60-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-60-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-60-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-60-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-61-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-61-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-61-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-61-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-62-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-62-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-62-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-62-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-63-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-63-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-63-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-63-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-64-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-64-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-64-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-64-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-65-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-65-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-65-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-65-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-66-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-66-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-66-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-66-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-67-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-67-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-67-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-67-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-68-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-68-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-68-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-68-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-69-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-69-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-69-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-69-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-70-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-70-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-70-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-70-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-77-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-77-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-77-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-77-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-78-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-78-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-78-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-78-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-80-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-80-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-80-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-80-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-81-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-81-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-81-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-81-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-82-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-82-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-82-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-82-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-83-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-83-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-83-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-83-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-84-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-84-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-84-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-84-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-85-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-85-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-85-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-85-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-86-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-86-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-86-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-86-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-87-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-87-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-87-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-87-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-88-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-88-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-88-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-88-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-89-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-89-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-89-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-89-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-90-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-90-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-90-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-90-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-91-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-91-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-91-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-91-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-92-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-92-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-elem-92-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-elem-92-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-events-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-events-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-events-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-events-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-interact-pevents-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-pservers-grad-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-script-elem-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-script-elem-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-script-elem-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-script-elem-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-struct-dom-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-struct-dom-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/animation/animate-struct-dom-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/animation/animate-struct-dom-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-cursor-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-cursor-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-cursor-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-cursor-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-dom-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-dom-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-dom-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-dom-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-202-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-202-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-202-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-202-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-203-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-203-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-events-203-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-events-203-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-order-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-order-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-05-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-05-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-07-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-07-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-08-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-08-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-08-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-08-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-09-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-09-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-09-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-09-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-10-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-10-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-10-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-10-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-201-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-201-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pevents-202-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pevents-202-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-pointer-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-pointer-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/interact-zoom-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/interact-zoom-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/styling-css-06-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/styling-css-06-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/styling-css-06-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/styling-css-06-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/interaction/text-tselect-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/interaction/text-tselect-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/conform-viewers-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/conform-viewers-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/conform-viewers-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/conform-viewers-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/coords-dom-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/coords-dom-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/extend-namespace-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/extend-namespace-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/extend-namespace-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/extend-namespace-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-09-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-09-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-09-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-09-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-12-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-12-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/masking-path-12-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/masking-path-12-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/paths-dom-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/paths-dom-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-elem-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-elem-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-04-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-04-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-handle-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-handle-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/script-specify-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/script-specify-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-04-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-04-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-05-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-05-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-06-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-06-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-06-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-06-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-07-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-07-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-07-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-07-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-08-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-08-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-08-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-08-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-09-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-09-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-11-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-11-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-11-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-11-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-12-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-12-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-12-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-12-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-13-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-13-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-13-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-13-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-14-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-14-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-14-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-14-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-15-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-15-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-15-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-15-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-16-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-16-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-16-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-16-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-17-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-17-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-17-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-17-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-18-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-18-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-18-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-18-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-19-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-19-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-19-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-19-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-20-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-20-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-dom-20-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-dom-20-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-image-11-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-image-11-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-image-11-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-image-11-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-svg-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-svg-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-13-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-13-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-13-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-13-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-14-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-14-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-14-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-14-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-15-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-15-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/struct-use-15-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/struct-use-15-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/styling-pres-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/styling-pres-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/styling-pres-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/styling-pres-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/svgdom-over-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/svgdom-over-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/svgdom-over-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/svgdom-over-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-03-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-04-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-05-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-05-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/text-dom-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/text-dom-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-02-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-04-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-04-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-05-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-05-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-06-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-06-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-06-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-06-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-07-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-07-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-07-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-07-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-08-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-08-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-08-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-08-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgfittoviewbox-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svglengthlist-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgnumberlist-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgstringlist-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/na/script/types-dom-svgtransformable-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/path/paths-data-18-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/path/paths-data-18-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/path/paths-data-18-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/path/paths-data-18-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/styling-css-05-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/styling-css-05-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/styling-css-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/styling-css-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-05-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-05-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-06-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-06-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-06-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-06-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-07-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-07-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-08-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-08-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-align-08-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-align-08-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-altglyph-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-altglyph-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-bidi-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-bidi-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-bidi-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-bidi-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-deco-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-deco-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-deco-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-deco-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-02-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-02-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-03-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-03-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-05-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-05-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-202-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-202-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-202-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-202-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-203-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-203-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-203-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-203-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-204-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-204-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-fonts-204-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-fonts-204-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-02-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-02-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-05-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-05-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-06-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-06-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-07-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-07-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-09-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-09-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-09-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-09-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-10-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-10-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-10-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-10-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-11-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-11-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-11-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-11-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-12-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-12-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-intro-12-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-intro-12-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-spacing-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-spacing-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-spacing-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-spacing-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-01-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-01-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-03-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-03-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-05-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-05-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-06-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-06-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-12-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-12-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/text-text-12-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/text-text-12-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/textdecoration01.png` & `CairoSVG-2.7.1/test_non_regression/fail/text/textdecoration01.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/text/textdecoration01.svg` & `CairoSVG-2.7.1/test_non_regression/fail/text/textdecoration01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/README.rst` & `CairoSVG-2.7.1/test_non_regression/fail/use/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-05-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-05-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-06-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-06-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-06-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-06-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-08-b.png` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-08-b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-08-b.svg` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-08-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-12-f.png` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-12-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/use/struct-use-12-f.svg` & `CairoSVG-2.7.1/test_non_regression/fail/use/struct-use-12-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/viewbox/README.rst` & `CairoSVG-2.7.1/test_non_regression/fail/viewbox/README.rst`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-01-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-01-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-04-t.png` & `CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-04-t.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/fail/viewbox/struct-frag-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/fail/viewbox/struct-frag-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/20x20.png` & `CairoSVG-2.7.1/test_non_regression/images/20x20.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/DisplaceChecker.png` & `CairoSVG-2.7.1/test_non_regression/images/DisplaceChecker.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi2c16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi2c16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi4a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi4a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/basi6a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/basi6a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn4a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn4a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/basn6a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/basn6a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgai4a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgai4a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgan6a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgan6a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/bggn4a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/bggn4a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/bgyn6a16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/bgyn6a16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ccwn2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ccwn2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ccwn3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ccwn3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/cdun2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/cdun2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ch2n3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ch2n3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ct1n0g04.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ct1n0g04.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ctzn0g04.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ctzn0g04.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/f00n2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/f00n2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/f01n2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/f01n2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/f02n2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/f02n2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/f03n2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/f03n2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/f04n2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/f04n2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi9n0g16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi9n0g16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/oi9n2c16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/oi9n2c16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/pngsuite.doc` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/pngsuite.doc`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/pngsuite_logo.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/pngsuite_logo.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/pp0n2c16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/pp0n2c16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/pp0n6a08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/pp0n6a08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps1n0g08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps1n0g08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps1n2c16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps1n2c16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps2n0g08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps2n0g08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/ps2n2c16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/ps2n2c16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbbn2c16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbbn2c16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbbn3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbbn3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbgn2c16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbgn2c16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbgn3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbgn3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbrn2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbrn2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbwn1g16.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbwn1g16.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbwn3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbwn3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tbyn3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tbyn3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp0n1g08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp0n1g08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp0n2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp0n2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp0n3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp0n3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/tp1n3p08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/tp1n3p08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/PngSuite/z00n2c08.png` & `CairoSVG-2.7.1/test_non_regression/images/PngSuite/z00n2c08.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/SVG-1.1-monolithic-fixed.dtd` & `CairoSVG-2.7.1/test_non_regression/images/SVG-1.1-monolithic-fixed.dtd`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/SVGImageTest.svg` & `CairoSVG-2.7.1/test_non_regression/images/SVGImageTest.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/animation-add-BE-09.svg` & `CairoSVG-2.7.1/test_non_regression/images/animation-add-BE-09.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/animation-extRef-image1.svg` & `CairoSVG-2.7.1/test_non_regression/images/animation-extRef-image1.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/animation-extRef-image2.svg` & `CairoSVG-2.7.1/test_non_regression/images/animation-extRef-image2.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/animation-extRef-image3.svg` & `CairoSVG-2.7.1/test_non_regression/images/animation-extRef-image3.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/bluesquidj.png` & `CairoSVG-2.7.1/test_non_regression/images/bluesquidj.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/bullet-small.png` & `CairoSVG-2.7.1/test_non_regression/images/bullet-small.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/bullet-white.png` & `CairoSVG-2.7.1/test_non_regression/images/bullet-white.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/bullet.png` & `CairoSVG-2.7.1/test_non_regression/images/bullet.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/bumpMap.png` & `CairoSVG-2.7.1/test_non_regression/images/bumpMap.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/bumpMap2.png` & `CairoSVG-2.7.1/test_non_regression/images/bumpMap2.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/changeColor.ICM` & `CairoSVG-2.7.1/test_non_regression/images/changeColor.ICM`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/colorprof.png` & `CairoSVG-2.7.1/test_non_regression/images/colorprof.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/convolveImage.png` & `CairoSVG-2.7.1/test_non_regression/images/convolveImage.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/coords-units-01-f.png` & `CairoSVG-2.7.1/test_non_regression/images/coords-units-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/coords-units-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/coords-units-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/copyright-documents-19990405.html` & `CairoSVG-2.7.1/test_non_regression/images/copyright-documents-19990405.html`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/diagarrow.png` & `CairoSVG-2.7.1/test_non_regression/images/diagarrow.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/ext-TestComic.svg` & `CairoSVG-2.7.1/test_non_regression/images/ext-TestComic.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/fillChangeColor.ICM` & `CairoSVG-2.7.1/test_non_regression/images/fillChangeColor.ICM`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-blend-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/filters-blend-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-color-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/filters-color-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-composite-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/filters-composite-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-comptran-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/filters-comptran-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-conv-01-f.includeimage.png` & `CairoSVG-2.7.1/test_non_regression/images/filters-conv-01-f.includeimage.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-conv-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/filters-conv-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-diffuse-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/filters-diffuse-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/filters-example-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/filters-example-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/footprints.jpg` & `CairoSVG-2.7.1/test_non_regression/images/footprints.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/footprints2.jpg` & `CairoSVG-2.7.1/test_non_regression/images/footprints2.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/galpha.png` & `CairoSVG-2.7.1/test_non_regression/images/galpha.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/gam030b.png` & `CairoSVG-2.7.1/test_non_regression/images/gam030b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/gam045b.png` & `CairoSVG-2.7.1/test_non_regression/images/gam045b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/gam056b.png` & `CairoSVG-2.7.1/test_non_regression/images/gam056b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/gam100b.png` & `CairoSVG-2.7.1/test_non_regression/images/gam100b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/gam200b.png` & `CairoSVG-2.7.1/test_non_regression/images/gam200b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/greentopbutton.jpg` & `CairoSVG-2.7.1/test_non_regression/images/greentopbutton.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/happysmiley.svg` & `CairoSVG-2.7.1/test_non_regression/images/happysmiley.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/image.png` & `CairoSVG-2.7.1/test_non_regression/images/image.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/image1.jpg` & `CairoSVG-2.7.1/test_non_regression/images/image1.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/image1.png` & `CairoSVG-2.7.1/test_non_regression/images/image1.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/image1_b.png` & `CairoSVG-2.7.1/test_non_regression/images/image1_b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/image2_b.jpg` & `CairoSVG-2.7.1/test_non_regression/images/image2_b.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/image2_b.png` & `CairoSVG-2.7.1/test_non_regression/images/image2_b.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/inline2.png` & `CairoSVG-2.7.1/test_non_regression/images/inline2.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/interact-dom-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/interact-dom-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/interact-order-02-b-targ.svg` & `CairoSVG-2.7.1/test_non_regression/images/interact-order-02-b-targ.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/interact-order-03-b-targ.svg` & `CairoSVG-2.7.1/test_non_regression/images/interact-order-03-b-targ.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-1st.png` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-1st.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-2nd.png` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-2nd.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-3rd.png` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-3rd.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-4th.png` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-4th.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-01-f-start.png` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-01-f-start.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-03-f-1st.png` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-03-f-1st.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linking-uri-03-f-start.png` & `CairoSVG-2.7.1/test_non_regression/images/linking-uri-03-f-start.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linkingCircle-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/linkingCircle-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/linkingToc-t.svg` & `CairoSVG-2.7.1/test_non_regression/images/linkingToc-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/makealpha.svg` & `CairoSVG-2.7.1/test_non_regression/images/makealpha.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/myimage.jpg` & `CairoSVG-2.7.1/test_non_regression/images/myimage.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/old-name-2-new-name1.html` & `CairoSVG-2.7.1/test_non_regression/images/old-name-2-new-name1.html`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-01-f.png` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-02-f.png` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-02-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-03-f.png` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-03-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-04-f.png` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-04-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/paths-data-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/paths-data-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/pinksquidj.png` & `CairoSVG-2.7.1/test_non_regression/images/pinksquidj.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/plant.jpg` & `CairoSVG-2.7.1/test_non_regression/images/plant.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/purplesquidj.png` & `CairoSVG-2.7.1/test_non_regression/images/purplesquidj.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/rgbalpha.png` & `CairoSVG-2.7.1/test_non_regression/images/rgbalpha.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/rightarrow.png` & `CairoSVG-2.7.1/test_non_regression/images/rightarrow.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/rotate20.png` & `CairoSVG-2.7.1/test_non_regression/images/rotate20.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/shapes-ellipse-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/images/shapes-ellipse-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/shapes-ellipse-01-f.png` & `CairoSVG-2.7.1/test_non_regression/images/shapes-ellipse-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/shapes-ellipse-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/shapes-ellipse-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/shapes-rect-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/images/shapes-rect-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/shapes-rect-01-f.png` & `CairoSVG-2.7.1/test_non_regression/images/shapes-rect-01-f.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/shapes-rect-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/shapes-rect-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/sign.png` & `CairoSVG-2.7.1/test_non_regression/images/sign.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/smiley.png` & `CairoSVG-2.7.1/test_non_regression/images/smiley.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/sphere.png` & `CairoSVG-2.7.1/test_non_regression/images/sphere.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/star.svg` & `CairoSVG-2.7.1/test_non_regression/images/star.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/stefan_252_tRNS_opti.png` & `CairoSVG-2.7.1/test_non_regression/images/stefan_252_tRNS_opti.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-frag-01-B.svg` & `CairoSVG-2.7.1/test_non_regression/images/struct-frag-01-B.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-image-01.jpg` & `CairoSVG-2.7.1/test_non_regression/images/struct-image-01.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-image-01.png` & `CairoSVG-2.7.1/test_non_regression/images/struct-image-01.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-image-02.jpg` & `CairoSVG-2.7.1/test_non_regression/images/struct-image-02.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-image-02.png` & `CairoSVG-2.7.1/test_non_regression/images/struct-image-02.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-symbol-01.png` & `CairoSVG-2.7.1/test_non_regression/images/struct-symbol-01.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-use-06-b-1.svg` & `CairoSVG-2.7.1/test_non_regression/images/struct-use-06-b-1.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/struct-use-08-b-cycles.svg` & `CairoSVG-2.7.1/test_non_regression/images/struct-use-08-b-cycles.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/svgRef1.svg` & `CairoSVG-2.7.1/test_non_regression/images/svgRef1.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/svgRef4.svg` & `CairoSVG-2.7.1/test_non_regression/images/svgRef4.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-align-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-align-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-align-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-align-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-align-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-align-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-altglyph-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-altglyph-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-extTref-BE-18-targ.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-extTref-BE-18-targ.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-intro-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-intro-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-tref-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-tref-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/text-ws-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/images/text-ws-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/toc-sv.svg` & `CairoSVG-2.7.1/test_non_regression/images/toc-sv.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/toc-svcmp.svg` & `CairoSVG-2.7.1/test_non_regression/images/toc-svcmp.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/townsville.jpg` & `CairoSVG-2.7.1/test_non_regression/images/townsville.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/tree.jpg` & `CairoSVG-2.7.1/test_non_regression/images/tree.jpg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/images/uparrow.png` & `CairoSVG-2.7.1/test_non_regression/images/uparrow.png`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/Anglepoise.otf` & `CairoSVG-2.7.1/test_non_regression/resources/Anglepoise.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/Blocky.otf` & `CairoSVG-2.7.1/test_non_regression/resources/Blocky.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/CalaLig.otf` & `CairoSVG-2.7.1/test_non_regression/resources/CalaLig.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/FreeSerif.otf` & `CairoSVG-2.7.1/test_non_regression/resources/FreeSerif.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/FreeSerifBold.otf` & `CairoSVG-2.7.1/test_non_regression/resources/FreeSerifBold.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/FreeSerifBoldItalic.otf` & `CairoSVG-2.7.1/test_non_regression/resources/FreeSerifBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/FreeSerifItalic.otf` & `CairoSVG-2.7.1/test_non_regression/resources/FreeSerifItalic.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/resources/SVGFreeSans.otf` & `CairoSVG-2.7.1/test_non_regression/resources/SVGFreeSans.otf`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/InitialCoords.svg` & `CairoSVG-2.7.1/test_non_regression/svg/InitialCoords.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/Nested.svg` & `CairoSVG-2.7.1/test_non_regression/svg/Nested.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/NewCoordSys.svg` & `CairoSVG-2.7.1/test_non_regression/svg/NewCoordSys.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/OrigCoordSys.svg` & `CairoSVG-2.7.1/test_non_regression/svg/OrigCoordSys.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/PreserveAspectRatio.svg` & `CairoSVG-2.7.1/test_non_regression/svg/PreserveAspectRatio.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/RotateScale.svg` & `CairoSVG-2.7.1/test_non_regression/svg/RotateScale.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/Skew.svg` & `CairoSVG-2.7.1/test_non_regression/svg/Skew.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/Units.svg` & `CairoSVG-2.7.1/test_non_regression/svg/Units.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/ViewBox.svg` & `CairoSVG-2.7.1/test_non_regression/svg/ViewBox.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/arcs01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/arcs01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/arcs02.svg` & `CairoSVG-2.7.1/test_non_regression/svg/arcs02.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/circle01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/circle01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/color-prop-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/color-prop-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/color-prop-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/color-prop-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/color-prop-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/color-prop-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/color-prop-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/color-prop-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/color-prop-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/color-prop-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/conform-viewers-01-t.svgz` & `CairoSVG-2.7.1/test_non_regression/svg/conform-viewers-01-t.svgz`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/conform-viewers-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/conform-viewers-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-coord-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-coord-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-coord-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-coord-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-08-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-08-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-09-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-09-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-10-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-10-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-11-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-11-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-12-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-12-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-13-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-13-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-trans-14-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-trans-14-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-transformattr-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-transformattr-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-units-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-units-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-units-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-units-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-units-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-units-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/coords-viewattr-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/coords-viewattr-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/cubic01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/cubic01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/cubic02.svg` & `CairoSVG-2.7.1/test_non_regression/svg/cubic02.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/ellipse01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/ellipse01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/feBlend.svg` & `CairoSVG-2.7.1/test_non_regression/svg/feBlend.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/fillrule-evenodd.svg` & `CairoSVG-2.7.1/test_non_regression/svg/fillrule-evenodd.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/fillrule-nonzero.svg` & `CairoSVG-2.7.1/test_non_regression/svg/fillrule-nonzero.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/filters-offset-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/filters-offset-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/imp-path-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/imp-path-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/inheritance.svg` & `CairoSVG-2.7.1/test_non_regression/svg/inheritance.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/line01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/line01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linecap.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linecap.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linejoin.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linejoin.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/lingrad01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/lingrad01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-a-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-a-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-a-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-a-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-a-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-a-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-a-08-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-a-08-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-frag-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-frag-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-uri-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-uri-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-uri-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-uri-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/linking-uri-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/linking-uri-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/marker.svg` & `CairoSVG-2.7.1/test_non_regression/svg/marker.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/mask01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/mask01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-filter-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-filter-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-mask-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-mask-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-mask-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-mask-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-opacity-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-opacity-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-06-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-06-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-08-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-08-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-13-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-13-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/masking-path-14-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/masking-path-14-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/metadata-example-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/metadata-example-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/opacity01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/opacity01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-control-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-control-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-control-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-control-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-control-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-control-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-control-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-control-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-control-06-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-control-06-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-fill-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-fill-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-fill-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-fill-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-fill-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-fill-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-fill-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-fill-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-fill-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-fill-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-marker-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-marker-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-marker-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-marker-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-marker-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-marker-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-marker-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-marker-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-marker-06-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-marker-06-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-08-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-08-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/painting-stroke-09-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/painting-stroke-09-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-08-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-08-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-09-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-09-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-10-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-10-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-12-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-12-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-13-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-13-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-14-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-14-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-15-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-15-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-16-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-16-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-17-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-17-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/paths-data-19-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/paths-data-19-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pattern01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pattern01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/polygon01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/polygon01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/polyline01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/polyline01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-06-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-06-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-07-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-07-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-08-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-08-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-09-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-09-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-10-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-10-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-11-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-11-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-12-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-12-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-13-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-13-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-14-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-14-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-15-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-15-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-16-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-16-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-17-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-17-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-18-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-18-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-20-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-20-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-21-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-21-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-22-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-22-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-23-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-23-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-24-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-24-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-grad-stops-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-grad-stops-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-06-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-06-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-07-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-07-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-08-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-08-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/pservers-pattern-09-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/pservers-pattern-09-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/quad01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/quad01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/radgrad01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/radgrad01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/rect01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/rect01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/rect02.svg` & `CairoSVG-2.7.1/test_non_regression/svg/rect02.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-elems-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-elems-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-elems-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-elems-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-elems-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-elems-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-elems-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-elems-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-elems-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-elems-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-elems-08-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-elems-08-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-groups-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-groups-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/render-groups-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/render-groups-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-circle-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-circle-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-circle-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-circle-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-ellipse-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-ellipse-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-ellipse-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-ellipse-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-ellipse-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-ellipse-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-grammar-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-grammar-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-intro-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-intro-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-intro-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-intro-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-line-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-line-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-line-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-line-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-polygon-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-polygon-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-polygon-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-polygon-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-polygon-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-polygon-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-polyline-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-polyline-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-polyline-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-polyline-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-06-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-06-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/shapes-rect-07-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/shapes-rect-07-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-cond-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-cond-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-cond-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-cond-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-cond-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-cond-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-02-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-02-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-cond-overview-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-cond-overview-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-defs-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-defs-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-frag-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-frag-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-frag-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-frag-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-frag-05-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-frag-05-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-frag-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-frag-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-group-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-group-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-group-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-group-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-group-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-group-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-04-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-04-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-05-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-05-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-06-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-06-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-08-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-08-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-09-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-09-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-10-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-10-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-13-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-13-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-14-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-14-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-15-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-15-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-16-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-16-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-17-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-17-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-18-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-18-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-image-19-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-image-19-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-svg-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-svg-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-symbol-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-symbol-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-use-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-use-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-use-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-use-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-use-07-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-use-07-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-use-09-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-use-09-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-use-10-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-use-10-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/struct-use-11-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/struct-use-11-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-class-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-class-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-07-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-07-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-08-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-08-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-09-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-09-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-css-10-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-css-10-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-elem-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-elem-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-inherit-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-inherit-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-pres-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-pres-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-pres-03-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-pres-03-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-pres-04-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-pres-04-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/styling-pres-05-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/styling-pres-05-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-align-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-align-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-align-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-align-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-align-04-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-align-04-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-path-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-path-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-path-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-path-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-text-07-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-text-07-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-text-08-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-text-08-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-text-09-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-text-09-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-text-10-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-text-10-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-text-11-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-text-11-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-tref-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-tref-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-tref-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-tref-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-tref-03-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-tref-03-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-tspan-01-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-tspan-01-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-tspan-02-b.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-tspan-02-b.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-ws-01-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-ws-01-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-ws-02-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-ws-02-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text-ws-03-t.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text-ws-03-t.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/text01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/text01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/toap01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/toap01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/toap02.svg` & `CairoSVG-2.7.1/test_non_regression/svg/toap02.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/toap03.svg` & `CairoSVG-2.7.1/test_non_regression/svg/toap03.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/toap04.svg` & `CairoSVG-2.7.1/test_non_regression/svg/toap04.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/tref01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/tref01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/triangle01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/triangle01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/tspan-dx-dy.svg` & `CairoSVG-2.7.1/test_non_regression/svg/tspan-dx-dy.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/tspan01.svg` & `CairoSVG-2.7.1/test_non_regression/svg/tspan01.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/tspan02.svg` & `CairoSVG-2.7.1/test_non_regression/svg/tspan02.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/tspan03.svg` & `CairoSVG-2.7.1/test_non_regression/svg/tspan03.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/tspan04.svg` & `CairoSVG-2.7.1/test_non_regression/svg/tspan04.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/tspan05.svg` & `CairoSVG-2.7.1/test_non_regression/svg/tspan05.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/svg/types-basic-01-f.svg` & `CairoSVG-2.7.1/test_non_regression/svg/types-basic-01-f.svg`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/test_helpers.py` & `CairoSVG-2.7.1/test_non_regression/test_helpers.py`

 * *Files identical despite different names*

### Comparing `CairoSVG-2.7.0/test_non_regression/test_non_regression.py` & `CairoSVG-2.7.1/test_non_regression/test_non_regression.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,9 +36,9 @@
         os.remove(ref_png.name)
         os.remove(test_png.name)
     else:  # pragma: no cover
         ref_surface.finish()
         test_surface.finish()
 
         raise AssertionError(
-            'Images are different: {} {}'.format(
-                ref_png.name, test_png.name))
+            f'Images are different: {ref_png.name} {test_png.name}'
+        )
```

