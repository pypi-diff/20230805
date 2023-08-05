# Comparing `tmp/castep_outputs-0.1.1.tar.gz` & `tmp/castep_outputs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castep_outputs-0.1.1.tar", last modified: Fri Aug  4 22:13:43 2023, max compression
+gzip compressed data, was "castep_outputs-0.1.2.tar", last modified: Fri Aug  4 22:48:12 2023, max compression
```

## Comparing `castep_outputs-0.1.1.tar` & `castep_outputs-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-04 22:13:43.879648 castep_outputs-0.1.1/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1500 2023-07-14 07:56:48.000000 castep_outputs-0.1.1/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6549 2023-08-04 22:13:43.879648 castep_outputs-0.1.1/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5814 2023-08-04 22:05:09.000000 castep_outputs-0.1.1/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6171 2023-08-04 22:10:38.000000 castep_outputs-0.1.1/README.rst
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-04 22:13:43.879648 castep_outputs-0.1.1/castep_outputs/
--rw-r--r--   0 jacob     (1000) jacob     (1000)      103 2023-07-23 09:09:17.000000 castep_outputs-0.1.1/castep_outputs/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      129 2023-07-14 07:58:04.000000 castep_outputs-0.1.1/castep_outputs/__main__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5440 2023-08-04 21:55:28.000000 castep_outputs-0.1.1/castep_outputs/args.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3321 2023-08-04 20:37:03.000000 castep_outputs-0.1.1/castep_outputs/castep_outputs_main.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10049 2023-08-04 20:37:03.000000 castep_outputs-0.1.1/castep_outputs/castep_res.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1016 2023-08-04 20:37:03.000000 castep_outputs-0.1.1/castep_outputs/constants.py
--rwxr-xr-x   0 jacob     (1000) jacob     (1000)    54164 2023-08-04 20:01:12.000000 castep_outputs-0.1.1/castep_outputs/parse_castep_file.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2238 2023-08-04 17:59:44.000000 castep_outputs-0.1.1/castep_outputs/parse_cell_param_file.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11854 2023-08-04 20:37:03.000000 castep_outputs-0.1.1/castep_outputs/parse_extra_files.py
--rwxr-xr-x   0 jacob     (1000) jacob     (1000)     1436 2023-08-04 20:37:03.000000 castep_outputs-0.1.1/castep_outputs/parse_md_geom_file.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6168 2023-08-04 17:59:44.000000 castep_outputs-0.1.1/castep_outputs/utility.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-04 22:13:43.879648 castep_outputs-0.1.1/castep_outputs.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6549 2023-08-04 22:13:43.000000 castep_outputs-0.1.1/castep_outputs.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      629 2023-08-04 22:13:43.000000 castep_outputs-0.1.1/castep_outputs.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-08-04 22:13:43.000000 castep_outputs-0.1.1/castep_outputs.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       75 2023-08-04 22:13:43.000000 castep_outputs-0.1.1/castep_outputs.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       52 2023-08-04 22:13:43.000000 castep_outputs-0.1.1/castep_outputs.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       15 2023-08-04 22:13:43.000000 castep_outputs-0.1.1/castep_outputs.egg-info/top_level.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       80 2023-08-04 21:31:38.000000 castep_outputs-0.1.1/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-08-04 22:13:43.879648 castep_outputs-0.1.1/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1162 2023-08-04 22:12:58.000000 castep_outputs-0.1.1/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-04 22:48:12.396314 castep_outputs-0.1.2/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1500 2023-07-14 07:56:48.000000 castep_outputs-0.1.2/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7384 2023-08-04 22:48:12.396314 castep_outputs-0.1.2/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6569 2023-08-04 22:28:48.000000 castep_outputs-0.1.2/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7006 2023-08-04 22:32:51.000000 castep_outputs-0.1.2/README.rst
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-04 22:48:12.396314 castep_outputs-0.1.2/castep_outputs/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      709 2023-08-04 22:47:08.000000 castep_outputs-0.1.2/castep_outputs/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      129 2023-07-14 07:58:04.000000 castep_outputs-0.1.2/castep_outputs/__main__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5440 2023-08-04 22:18:43.000000 castep_outputs-0.1.2/castep_outputs/args.py
+-rwxr-xr-x   0 jacob     (1000) jacob     (1000)    54174 2023-08-04 22:39:09.000000 castep_outputs-0.1.2/castep_outputs/castep_file_parser.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3328 2023-08-04 22:37:44.000000 castep_outputs-0.1.2/castep_outputs/castep_outputs_main.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10049 2023-08-04 20:37:03.000000 castep_outputs-0.1.2/castep_outputs/castep_res.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2321 2023-08-04 22:27:25.000000 castep_outputs-0.1.2/castep_outputs/cell_param_file_parser.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1016 2023-08-04 20:37:03.000000 castep_outputs-0.1.2/castep_outputs/constants.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11854 2023-08-04 20:37:03.000000 castep_outputs-0.1.2/castep_outputs/extra_files_parser.py
+-rwxr-xr-x   0 jacob     (1000) jacob     (1000)     1436 2023-08-04 20:37:03.000000 castep_outputs-0.1.2/castep_outputs/md_geom_file_parser.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6168 2023-08-04 17:59:44.000000 castep_outputs-0.1.2/castep_outputs/utility.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-04 22:48:12.396314 castep_outputs-0.1.2/castep_outputs.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     7384 2023-08-04 22:48:12.000000 castep_outputs-0.1.2/castep_outputs.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      633 2023-08-04 22:48:12.000000 castep_outputs-0.1.2/castep_outputs.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-08-04 22:48:12.000000 castep_outputs-0.1.2/castep_outputs.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       75 2023-08-04 22:48:12.000000 castep_outputs-0.1.2/castep_outputs.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       52 2023-08-04 22:48:12.000000 castep_outputs-0.1.2/castep_outputs.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       15 2023-08-04 22:48:12.000000 castep_outputs-0.1.2/castep_outputs.egg-info/top_level.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       80 2023-08-04 22:18:43.000000 castep_outputs-0.1.2/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-08-04 22:48:12.396314 castep_outputs-0.1.2/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1161 2023-08-04 22:47:49.000000 castep_outputs-0.1.2/setup.py
```

### Comparing `castep_outputs-0.1.1/LICENSE` & `castep_outputs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `castep_outputs-0.1.1/PKG-INFO` & `castep_outputs-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,188 +1,191 @@
-Metadata-Version: 2.1
-Name: castep_outputs
-Version: 0.1.1
-Summary: A package for extracting information from castep outputs
-Home-page: https://github.com/oerc0122/castep_outputs
-Download-URL: https://github.com/oerc0122/castep_outputs
-Author: Jacob Wilkins
-Author-email: jacob.wilkins@stfc.ac.uk
-License: BSD3
-Requires-Python: >=3.8
-Provides-Extra: ruamel
-Provides-Extra: yaml
-
-castep_outputs
-==============
-
+# castep_outputs
 Parser for CASTEP output files
 
-``castep_outputs`` parses the output files of
-`castep <https://www.castep.org/>`__ into a standard form and is able to
+`castep_outputs` parses the output files of [castep](https://www.castep.org/) into a standard form and is able to
 subsequently dump the processed data into a standard format.
 
-Install
--------
-
-To install ``castep_outputs`` simply run:
+## Install
 
-::
+To install `castep_outputs` simply run:
 
-   pip install castep_outputs
+```
+pip install castep_outputs
+```
 
 To check it is installed run:
 
-::
-
-   python -m castep_outputs -h
-
-Dependencies
-------------
-
-``castep_outputs`` is designed to have no external dependencies beyond
-the standard library, however, it is possible to use either
-`PyYAML <https://pypi.org/project/PyYAML/>`__ or
-`ruamel.yaml <https://pypi.org/project/ruamel.yaml/>`__ to dump in the
-YAML format.
-
-Command-line
-------------
-
-When run as a commandline tool, it attempts to find all files for the
-given seedname, filtered by ``inc`` args (default: all). Explicit files
-can be passed using longname arguments. castep_outputs can parse most
-human-readable castep outputs including: ``.castep``, ``.param``,
-``.cell``, ``.geom``, ``.md``, ``.bands``, ``.hug``, ``.phonon_dos``,
-``.efield``, ``.xrd_sf``, ``.elf_fmt``, ``.chdiff_fmt``,
-``.pot_fmt, .den_fmt``, ``.elastic``, ``.ts``.
+```
+python -m castep_outputs -h
+```
+
+## Dependencies
+
+`castep_outputs` is designed to have no external dependencies beyond the standard library, however, it is possible to
+use either [PyYAML](https://pypi.org/project/PyYAML/) or [ruamel.yaml](https://pypi.org/project/ruamel.yaml/) to dump in
+the YAML format.
+
+## Command-line
+
+When run as a commandline tool, it attempts to find all files for the given seedname, filtered by `inc` args (default:
+all). Explicit files can be passed using longname arguments. castep_outputs can parse most human-readable castep outputs
+including: `.castep`, `.param`, `.cell`, `.geom`, `.md`, `.bands`, `.hug`, `.phonon_dos`, `.efield`, `.xrd_sf`,
+`.elf_fmt`, `.chdiff_fmt`, `.pot_fmt, .den_fmt`, `.elastic`, `.ts`.
 
 to run in basic mode:
 
-::
-
-   python -m castep_outputs seedname
-
-Which will attempt to detect all found files and dump a ``.json`` to
-stdout, ready for piping.
-
-::
-
-   python -m castep_outputs --inc-castep --inc-param seedname
-
-Will parse only the ``seedname.castep`` and ``seedname.param`` files if
-found.
-
-::
-
-   python -m castep_outputs seedname.castep
-
-Will parse the single named file and again dump a ``.json`` to stdout.
-
-::
-
-   python -m castep_outputs --castep seedname.param
-
-Will attempt to parse the file ``seedname.param`` as though it were a
-``.castep`` file. While not ordinarily useful it can help with manually
-renamed files.
-
-Full usage
-----------
-
-::
-
-   usage: castep_outputs [-h] [-V] [-L {DEBUG,INFO,WARNING,ERROR,CRITICAL}] [-o OUTPUT]
-                         [-f {json,ruamel,yaml,pprint,print}] [-t] [-A] [-c] [-g] [-m] [-b] [-p] [-e] [-x] [-H] [-E]
-                         [-C] [-P] [-D] [-X] [-T] [--inc-param] [--inc-cell] [--castep [CASTEP ...]]
-                         [--geom [GEOM ...]] [--cell [CELL ...]] [--param [PARAM ...]] [--md [MD ...]]
-                         [--bands [BANDS ...]] [--hug [HUG ...]] [--phonon_dos [PHONON_DOS ...]]
-                         [--efield [EFIELD ...]] [--xrd_sf [XRD_SF ...]] [--elf_fmt [ELF_FMT ...]]
-                         [--chdiff_fmt [CHDIFF_FMT ...]] [--pot_fmt [POT_FMT ...]] [--den_fmt [DEN_FMT ...]]
-                         [--elastic [ELASTIC ...]] [--ts [TS ...]]
-                         ...
-
-   Attempts to find all files for seedname, filtered by `inc` args (default: all). Explicit files can be passed
-   using longname arguments. Parse most human-readable castep outputs including: .castep, .param, .cell, .geom, .md,
-   .bands, .hug, .phonon_dos, .efield, .xrd_sf, .elf_fmt, .chdiff_fmt, .pot_fmt, .den_fmt, .elastic, .ts
-
-   positional arguments:
-     seedname              Seed name for data
-
-   options:
-     -h, --help            show this help message and exit
-     -V, --version         show program's version number and exit
-     -L {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --log {DEBUG,INFO,WARNING,ERROR,CRITICAL}
-                           Verbose output
-     -o OUTPUT, --output OUTPUT
-                           File to write output, default: screen
-     -f {json,ruamel,yaml,pprint,print}, --out-format {json,ruamel,yaml,pprint,print}
-                           Output format
-     -t, --testing         Set testing mode to produce flat outputs
-     -A, --inc-all         Extract all available information
-     -c, --inc-castep      Extract .castep information
-     -g, --inc-geom        Extract .geom information
-     -m, --inc-md          Extract .md information
-     -b, --inc-bands       Extract .bands information
-     -p, --inc-phonon_dos  Extract .phonon_dos information
-     -e, --inc-efield      Extract .efield information
-     -x, --inc-xrd_sf      Extract .xrd_sf information
-     -H, --inc-hug         Extract .hug information
-     -E, --inc-elf_fmt     Extract .elf_fmt information
-     -C, --inc-chdiff_fmt  Extract .chdiff_fmt information
-     -P, --inc-pot_fmt     Extract .pot_fmt information
-     -D, --inc-den_fmt     Extract .den_fmt information
-     -X, --inc-elastic     Extract .elastic information
-     -T, --inc-ts          Extract .ts information
-     --inc-param           Extract .param information
-     --inc-cell            Extract .cell information
-     --castep [CASTEP ...]
-                           Extract from CASTEP as .castep type
-     --geom [GEOM ...]     Extract from GEOM as .geom type
-     --cell [CELL ...]     Extract from CELL as .cell type
-     --param [PARAM ...]   Extract from PARAM as .param type
-     --md [MD ...]         Extract from MD as .md type
-     --bands [BANDS ...]   Extract from BANDS as .bands type
-     --hug [HUG ...]       Extract from HUG as .hug type
-     --phonon_dos [PHONON_DOS ...]
-                           Extract from PHONON_DOS as .phonon_dos type
-     --efield [EFIELD ...]
-                           Extract from EFIELD as .efield type
-     --xrd_sf [XRD_SF ...]
-                           Extract from XRD_SF as .xrd_sf type
-     --elf_fmt [ELF_FMT ...]
-                           Extract from ELF_FMT as .elf_fmt type
-     --chdiff_fmt [CHDIFF_FMT ...]
-                           Extract from CHDIFF_FMT as .chdiff_fmt type
-     --pot_fmt [POT_FMT ...]
-                           Extract from POT_FMT as .pot_fmt type
-     --den_fmt [DEN_FMT ...]
-                           Extract from DEN_FMT as .den_fmt type
-     --elastic [ELASTIC ...]
-                           Extract from ELASTIC as .elastic type
-     --ts [TS ...]         Extract from TS as .ts type
+```
+python -m castep_outputs seedname
+```
+
+Which will attempt to detect all found files and dump a `.json` to stdout, ready for piping.
+
+```
+python -m castep_outputs --inc-castep --inc-param seedname
+```
+
+Will parse only the `seedname.castep` and `seedname.param` files if found.
+
+```
+python -m castep_outputs seedname.castep
+```
+
+Will parse the single named file and again dump a `.json` to stdout.
+
+```
+python -m castep_outputs --castep seedname.param
+```
+
+Will attempt to parse the file `seedname.param` as though it were a `.castep` file. While not ordinarily useful it can
+help with manually renamed files.
+
+```
+python -m castep_outputs -o my_file.yaml -f yaml seedname.castep
+```
+Will parse `seedname.castep`, dump it to `my_file.yaml` in `yaml` format using the `PyYAML` engine.
+
+## As a module
+
+Importing `castep_outputs` gives you access to all of the parsers. These are:
+
+- `parse_castep_file`
+- `parse_cell_param_file`
+- `parse_param_file`
+- `parse_cell_file`
+- `parse_md_geom_file`
+- `parse_md_file`
+- `parse_geom_file`
+- `parse_bands_file`
+- `parse_hug_file`
+- `parse_phonon_dos_file`
+- `parse_efield_file`
+- `parse_xrd_sf_file`
+- `parse_elf_fmt_file`
+- `parse_chdiff_fmt_file`
+- `parse_pot_fmt_file`
+- `parse_den_fmt_file`
+- `parse_elastic_file`
+- `parse_ts_file`
+
+Which return processed `list`s of `dict`s of data ready for use in other applications.
+
+
+## Full usage
+
+```
+usage: castep_outputs [-h] [-V] [-L {DEBUG,INFO,WARNING,ERROR,CRITICAL}] [-o OUTPUT]
+                      [-f {json,ruamel,yaml,pprint,print}] [-t] [-A] [-c] [-g] [-m] [-b] [-p] [-e] [-x] [-H] [-E]
+                      [-C] [-P] [-D] [-X] [-T] [--inc-param] [--inc-cell] [--castep [CASTEP ...]]
+                      [--geom [GEOM ...]] [--cell [CELL ...]] [--param [PARAM ...]] [--md [MD ...]]
+                      [--bands [BANDS ...]] [--hug [HUG ...]] [--phonon_dos [PHONON_DOS ...]]
+                      [--efield [EFIELD ...]] [--xrd_sf [XRD_SF ...]] [--elf_fmt [ELF_FMT ...]]
+                      [--chdiff_fmt [CHDIFF_FMT ...]] [--pot_fmt [POT_FMT ...]] [--den_fmt [DEN_FMT ...]]
+                      [--elastic [ELASTIC ...]] [--ts [TS ...]]
+                      ...
+
+Attempts to find all files for seedname, filtered by `inc` args (default: all). Explicit files can be passed
+using longname arguments. Parse most human-readable castep outputs including: .castep, .param, .cell, .geom, .md,
+.bands, .hug, .phonon_dos, .efield, .xrd_sf, .elf_fmt, .chdiff_fmt, .pot_fmt, .den_fmt, .elastic, .ts
+
+positional arguments:
+  seedname              Seed name for data
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         show program's version number and exit
+  -L {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --log {DEBUG,INFO,WARNING,ERROR,CRITICAL}
+                        Verbose output
+  -o OUTPUT, --output OUTPUT
+                        File to write output, default: screen
+  -f {json,ruamel,yaml,pprint,print}, --out-format {json,ruamel,yaml,pprint,print}
+                        Output format
+  -t, --testing         Set testing mode to produce flat outputs
+  -A, --inc-all         Extract all available information
+  -c, --inc-castep      Extract .castep information
+  -g, --inc-geom        Extract .geom information
+  -m, --inc-md          Extract .md information
+  -b, --inc-bands       Extract .bands information
+  -p, --inc-phonon_dos  Extract .phonon_dos information
+  -e, --inc-efield      Extract .efield information
+  -x, --inc-xrd_sf      Extract .xrd_sf information
+  -H, --inc-hug         Extract .hug information
+  -E, --inc-elf_fmt     Extract .elf_fmt information
+  -C, --inc-chdiff_fmt  Extract .chdiff_fmt information
+  -P, --inc-pot_fmt     Extract .pot_fmt information
+  -D, --inc-den_fmt     Extract .den_fmt information
+  -X, --inc-elastic     Extract .elastic information
+  -T, --inc-ts          Extract .ts information
+  --inc-param           Extract .param information
+  --inc-cell            Extract .cell information
+  --castep [CASTEP ...]
+                        Extract from CASTEP as .castep type
+  --geom [GEOM ...]     Extract from GEOM as .geom type
+  --cell [CELL ...]     Extract from CELL as .cell type
+  --param [PARAM ...]   Extract from PARAM as .param type
+  --md [MD ...]         Extract from MD as .md type
+  --bands [BANDS ...]   Extract from BANDS as .bands type
+  --hug [HUG ...]       Extract from HUG as .hug type
+  --phonon_dos [PHONON_DOS ...]
+                        Extract from PHONON_DOS as .phonon_dos type
+  --efield [EFIELD ...]
+                        Extract from EFIELD as .efield type
+  --xrd_sf [XRD_SF ...]
+                        Extract from XRD_SF as .xrd_sf type
+  --elf_fmt [ELF_FMT ...]
+                        Extract from ELF_FMT as .elf_fmt type
+  --chdiff_fmt [CHDIFF_FMT ...]
+                        Extract from CHDIFF_FMT as .chdiff_fmt type
+  --pot_fmt [POT_FMT ...]
+                        Extract from POT_FMT as .pot_fmt type
+  --den_fmt [DEN_FMT ...]
+                        Extract from DEN_FMT as .den_fmt type
+  --elastic [ELASTIC ...]
+                        Extract from ELASTIC as .elastic type
+  --ts [TS ...]         Extract from TS as .ts type
+```
 
 Current Parsers:
 
--  ``.castep``
--  ``.param``
--  ``.cell``
--  ``.geom``
--  ``.md``
--  ``.bands``
--  ``.hug``
--  ``.phonon_dos``
--  ``.efield``
--  ``.xrd_sf``
--  ``.elf_fmt``
--  ``.chdiff_fmt``
--  ``.pot_fmt``
--  ``.den_fmt``
--  ``.elastic``
--  ``.ts``
+- `.castep`
+- `.param`
+- `.cell`
+- `.geom`
+- `.md`
+- `.bands`
+- `.hug`
+- `.phonon_dos`
+- `.efield`
+- `.xrd_sf`
+- `.elf_fmt`
+- `.chdiff_fmt`
+- `.pot_fmt`
+- `.den_fmt`
+- `.elastic`
+- `.ts`
 
 Current dumpers:
 
--  ``json``
--  ``ruamel.yaml``
--  ``pyyaml``
--  ``print``
--  ``pprint``
+- `json`
+- `ruamel.yaml`
+- `pyyaml`
+- `print`
+- `pprint`
```

### Comparing `castep_outputs-0.1.1/README.rst` & `castep_outputs-0.1.2/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -68,14 +68,49 @@
 
    python -m castep_outputs --castep seedname.param
 
 Will attempt to parse the file ``seedname.param`` as though it were a
 ``.castep`` file. While not ordinarily useful it can help with manually
 renamed files.
 
+::
+
+   python -m castep_outputs -o my_file.yaml -f yaml seedname.castep
+
+Will parse ``seedname.castep``, dump it to ``my_file.yaml`` in ``yaml``
+format using the ``PyYAML`` engine.
+
+As a module
+-----------
+
+Importing ``castep_outputs`` gives you access to all of the parsers.
+These are:
+
+-  ``parse_castep_file``
+-  ``parse_cell_param_file``
+-  ``parse_param_file``
+-  ``parse_cell_file``
+-  ``parse_md_geom_file``
+-  ``parse_md_file``
+-  ``parse_geom_file``
+-  ``parse_bands_file``
+-  ``parse_hug_file``
+-  ``parse_phonon_dos_file``
+-  ``parse_efield_file``
+-  ``parse_xrd_sf_file``
+-  ``parse_elf_fmt_file``
+-  ``parse_chdiff_fmt_file``
+-  ``parse_pot_fmt_file``
+-  ``parse_den_fmt_file``
+-  ``parse_elastic_file``
+-  ``parse_ts_file``
+
+Which return processed ``list``\ s of ``dict``\ s of data ready for use
+in other applications.
+
 Full usage
 ----------
 
 ::
 
    usage: castep_outputs [-h] [-V] [-L {DEBUG,INFO,WARNING,ERROR,CRITICAL}] [-o OUTPUT]
                          [-f {json,ruamel,yaml,pprint,print}] [-t] [-A] [-c] [-g] [-m] [-b] [-p] [-e] [-x] [-H] [-E]
```

### Comparing `castep_outputs-0.1.1/castep_outputs/args.py` & `castep_outputs-0.1.2/castep_outputs/args.py`

 * *Files identical despite different names*

### Comparing `castep_outputs-0.1.1/castep_outputs/castep_outputs_main.py` & `castep_outputs-0.1.2/castep_outputs/castep_outputs_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import fileinput
 import io
 import sys
 import os.path
 
 from .args import (parse_args, args_to_dict)
 from .utility import (json_safe, flatten_dict, get_dumpers)
-from .parse_castep_file import parse_castep_file
-from .parse_cell_param_file import parse_cell_param_file
-from .parse_md_geom_file import parse_md_geom_file
-from .parse_extra_files import (parse_bands_file, parse_hug_file, parse_phonon_dos_file,
-                                parse_efield_file, parse_xrd_sf_file, parse_elf_fmt_file,
-                                parse_chdiff_fmt_file, parse_pot_fmt_file, parse_den_fmt_file,
-                                parse_elastic_file, parse_ts_file)
+from .castep_file_parser import parse_castep_file
+from .cell_param_file_parser import parse_cell_param_file
+from .md_geom_file_parser import parse_md_geom_file
+from .extra_files_parser import (parse_bands_file, parse_hug_file, parse_phonon_dos_file,
+                                 parse_efield_file, parse_xrd_sf_file, parse_elf_fmt_file,
+                                 parse_chdiff_fmt_file, parse_pot_fmt_file, parse_den_fmt_file,
+                                 parse_elastic_file, parse_ts_file)
 
 
 PARSERS = {
     ".castep": parse_castep_file,
     ".cell": parse_cell_param_file,
     ".param": parse_cell_param_file,
     ".geom": parse_md_geom_file,
```

### Comparing `castep_outputs-0.1.1/castep_outputs/castep_res.py` & `castep_outputs-0.1.2/castep_outputs/castep_res.py`

 * *Files identical despite different names*

### Comparing `castep_outputs-0.1.1/castep_outputs/constants.py` & `castep_outputs-0.1.2/castep_outputs/constants.py`

 * *Files identical despite different names*

### Comparing `castep_outputs-0.1.1/castep_outputs/parse_castep_file.py` & `castep_outputs-0.1.2/castep_outputs/castep_file_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from .castep_res import labelled_floats, get_numbers, get_block
 
 from .constants import SHELLS
 
 from .utility import (fix_data_types, add_aliases, to_type,
                       stack_dict, normalise_string,
                       atreg_to_index, log_factory)
-from .parse_extra_files import (parse_bands_file,
-                                parse_hug_file,
-                                parse_phonon_dos_file,
-                                parse_efield_file,
-                                parse_xrd_sf_file,
-                                parse_elf_fmt_file,
-                                parse_chdiff_fmt_file,
-                                parse_pot_fmt_file,
-                                parse_den_fmt_file,
-                                parse_elastic_file)
+from .extra_files_parser import (parse_bands_file,
+                                 parse_hug_file,
+                                 parse_phonon_dos_file,
+                                 parse_efield_file,
+                                 parse_xrd_sf_file,
+                                 parse_elf_fmt_file,
+                                 parse_chdiff_fmt_file,
+                                 parse_pot_fmt_file,
+                                 parse_den_fmt_file,
+                                 parse_elastic_file)
 
 AtomIndex = Tuple[str, float]
 ThreeVector = Tuple[float, float, float]
 ThreeByThreeMatrix = Tuple[ThreeVector, ThreeVector, ThreeVector]
 
 
 def parse_castep_file(castep_file: TextIO) -> List[Dict[str, Any]]:
```

### Comparing `castep_outputs-0.1.1/castep_outputs/parse_cell_param_file.py` & `castep_outputs-0.1.2/castep_outputs/cell_param_file_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,7 +66,11 @@
             key, val = re.split(r'\s*[ :=]+\s*', line, maxsplit=1)
 
             key = key.lower()
             logger("Found param %s", key)
 
             curr[key] = val
     return [curr]
+
+
+parse_cell_file = parse_cell_param_file
+parse_param_file = parse_cell_param_file
```

### Comparing `castep_outputs-0.1.1/castep_outputs/parse_extra_files.py` & `castep_outputs-0.1.2/castep_outputs/extra_files_parser.py`

 * *Files identical despite different names*

### Comparing `castep_outputs-0.1.1/castep_outputs/parse_md_geom_file.py` & `castep_outputs-0.1.2/castep_outputs/md_geom_file_parser.py`

 * *Files identical despite different names*

### Comparing `castep_outputs-0.1.1/castep_outputs/utility.py` & `castep_outputs-0.1.2/castep_outputs/utility.py`

 * *Files identical despite different names*

### Comparing `castep_outputs-0.1.1/castep_outputs.egg-info/PKG-INFO` & `castep_outputs-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: castep-outputs
-Version: 0.1.1
+Name: castep_outputs
+Version: 0.1.2
 Summary: A package for extracting information from castep outputs
 Home-page: https://github.com/oerc0122/castep_outputs
 Download-URL: https://github.com/oerc0122/castep_outputs
 Author: Jacob Wilkins
 Author-email: jacob.wilkins@stfc.ac.uk
 License: BSD3
 Requires-Python: >=3.8
@@ -81,14 +81,49 @@
 
    python -m castep_outputs --castep seedname.param
 
 Will attempt to parse the file ``seedname.param`` as though it were a
 ``.castep`` file. While not ordinarily useful it can help with manually
 renamed files.
 
+::
+
+   python -m castep_outputs -o my_file.yaml -f yaml seedname.castep
+
+Will parse ``seedname.castep``, dump it to ``my_file.yaml`` in ``yaml``
+format using the ``PyYAML`` engine.
+
+As a module
+-----------
+
+Importing ``castep_outputs`` gives you access to all of the parsers.
+These are:
+
+-  ``parse_castep_file``
+-  ``parse_cell_param_file``
+-  ``parse_param_file``
+-  ``parse_cell_file``
+-  ``parse_md_geom_file``
+-  ``parse_md_file``
+-  ``parse_geom_file``
+-  ``parse_bands_file``
+-  ``parse_hug_file``
+-  ``parse_phonon_dos_file``
+-  ``parse_efield_file``
+-  ``parse_xrd_sf_file``
+-  ``parse_elf_fmt_file``
+-  ``parse_chdiff_fmt_file``
+-  ``parse_pot_fmt_file``
+-  ``parse_den_fmt_file``
+-  ``parse_elastic_file``
+-  ``parse_ts_file``
+
+Which return processed ``list``\ s of ``dict``\ s of data ready for use
+in other applications.
+
 Full usage
 ----------
 
 ::
 
    usage: castep_outputs [-h] [-V] [-L {DEBUG,INFO,WARNING,ERROR,CRITICAL}] [-o OUTPUT]
                          [-f {json,ruamel,yaml,pprint,print}] [-t] [-A] [-c] [-g] [-m] [-b] [-p] [-e] [-x] [-H] [-E]
```

### Comparing `castep_outputs-0.1.1/castep_outputs.egg-info/SOURCES.txt` & `castep_outputs-0.1.2/castep_outputs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 README.md
 README.rst
 pyproject.toml
 setup.py
 castep_outputs/__init__.py
 castep_outputs/__main__.py
 castep_outputs/args.py
+castep_outputs/castep_file_parser.py
 castep_outputs/castep_outputs_main.py
 castep_outputs/castep_res.py
+castep_outputs/cell_param_file_parser.py
 castep_outputs/constants.py
-castep_outputs/parse_castep_file.py
-castep_outputs/parse_cell_param_file.py
-castep_outputs/parse_extra_files.py
-castep_outputs/parse_md_geom_file.py
+castep_outputs/extra_files_parser.py
+castep_outputs/md_geom_file_parser.py
 castep_outputs/utility.py
 castep_outputs.egg-info/PKG-INFO
 castep_outputs.egg-info/SOURCES.txt
 castep_outputs.egg-info/dependency_links.txt
 castep_outputs.egg-info/entry_points.txt
 castep_outputs.egg-info/requires.txt
 castep_outputs.egg-info/top_level.txt
```

### Comparing `castep_outputs-0.1.1/setup.py` & `castep_outputs-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 To install locally:
 
     python setup.py install
 
 """
 
 import sys
-
 from setuptools import setup, find_packages
 
 # Check for valid Python version
 if sys.version_info[:2] < (3, 8):
     print(f"castep_outputs requires Python 3.8. Python {'.'.join(sys.version_info[:2])} detected")
 
 packages_test = find_packages()
 
 with open("README.rst", "r", encoding="utf-8") as readme:
     README = readme.read()
 
 setup(
     name="castep_outputs",
-    version="0.1.1",
+    version="0.1.2",
     license='BSD3',
     license_files=('LICENSE'),
     description='A package for extracting information from castep outputs',
     long_description=README,
     packages=find_packages(),
     author="Jacob Wilkins",
     author_email="jacob.wilkins@stfc.ac.uk",
```

