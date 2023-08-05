# Comparing `tmp/spec2nii-0.6.9.tar.gz` & `tmp/spec2nii-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec2nii-0.6.9.tar", last modified: Fri Jul  7 14:10:42 2023, max compression
+gzip compressed data, was "spec2nii-0.7.0.tar", last modified: Sat Aug  5 19:01:46 2023, max compression
```

## Comparing `spec2nii-0.6.9.tar` & `spec2nii-0.7.0.tar`

### file list

```diff
@@ -1,83 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.384826 spec2nii-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-07 14:10:30.000000 spec2nii-0.6.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-07 14:10:30.000000 spec2nii-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-07 14:10:30.000000 spec2nii-0.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-07 14:10:42.384826 spec2nii-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-07-07 14:10:30.000000 spec2nii-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 14:10:30.000000 spec2nii-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 14:10:30.000000 spec2nii-0.6.9/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 14:10:42.384826 spec2nii-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-07 14:10:30.000000 spec2nii-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.384826 spec2nii-0.6.9/spec2nii/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/GE/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/VESPA_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161091 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/ge_hdr_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/ge_pfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    47855 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/ge_read_pfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/GSL/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GSL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GSL/gslfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/Philips/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/philips.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/philips_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    23678 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/philips_dcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/Siemens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/dicomfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/rda.py
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/twix_special_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    46734 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/twixfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 14:10:42.384826 spec2nii-0.6.9/spec2nii/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/anonymise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/bruker_fid_override.json
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/bruker_properties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.380826 spec2nii-0.6.9/spec2nii/dcm2niiOrientation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/dcm2niiOrientation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/dcm2niiOrientation/orientationFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/fileiobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/jmrui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/nifti_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/other_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)    31584 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/spec2nii.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/uih.py
--rw-r--r--   0 runner    (1001) docker     (123)    64350 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/varian.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/varian_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.384826 spec2nii-0.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/io_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_anon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_ge_pfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_ge_pfile_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_jmrui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_nifti_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_other_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_dicom_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_sdat_spar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_sdat_spar_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_mrsi_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_rda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_special_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_svs_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_twix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_uih.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_uih_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_varian.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-07 14:10:30.000000 spec2nii-0.6.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.067433 spec2nii-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-05 19:01:38.000000 spec2nii-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-08-05 19:01:38.000000 spec2nii-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-05 19:01:38.000000 spec2nii-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-08-05 19:01:46.067433 spec2nii-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-08-05 19:01:38.000000 spec2nii-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-05 19:01:38.000000 spec2nii-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-05 19:01:38.000000 spec2nii-0.7.0/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-05 19:01:46.067433 spec2nii-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-05 19:01:38.000000 spec2nii-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.063433 spec2nii-0.7.0/spec2nii/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.063433 spec2nii-0.7.0/spec2nii/GE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/GE/VESPA_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/GE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161091 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/GE/ge_hdr_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/GE/ge_pfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47976 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/GE/ge_read_pfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.063433 spec2nii-0.7.0/spec2nii/GSL/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/GSL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/GSL/gslfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.063433 spec2nii-0.7.0/spec2nii/Philips/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Philips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Philips/philips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Philips/philips_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Philips/philips_dcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.067433 spec2nii-0.7.0/spec2nii/Siemens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Siemens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Siemens/dicomfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Siemens/rda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Siemens/twix_special_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45997 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/Siemens/twixfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-05 19:01:46.067433 spec2nii-0.7.0/spec2nii/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/anonymise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/bruker_fid_override.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/bruker_properties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.067433 spec2nii-0.7.0/spec2nii/dcm2niiOrientation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/dcm2niiOrientation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/dcm2niiOrientation/orientationFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/fileiobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/jmrui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/nifti_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/other_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31584 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/spec2nii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/uih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64350 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/varian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-08-05 19:01:38.000000 spec2nii-0.7.0/spec2nii/varian_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.063433 spec2nii-0.7.0/spec2nii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-08-05 19:01:46.000000 spec2nii-0.7.0/spec2nii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-05 19:01:46.000000 spec2nii-0.7.0/spec2nii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:01:46.000000 spec2nii-0.7.0/spec2nii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-05 19:01:46.000000 spec2nii-0.7.0/spec2nii.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-05 19:01:46.000000 spec2nii-0.7.0/spec2nii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 19:01:46.000000 spec2nii-0.7.0/spec2nii.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:01:46.067433 spec2nii-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_anon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_ge_pfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_ge_pfile_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_jmrui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_nifti_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_other_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_philips_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_philips_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_philips_dicom_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_philips_orientation_dcm_spar_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_philips_sdat_spar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_philips_sdat_spar_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_siemens_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_siemens_mrsi_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_siemens_rda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_siemens_special_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_siemens_svs_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_twix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_uih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_uih_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-05 19:01:38.000000 spec2nii-0.7.0/tests/test_varian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-08-05 19:01:38.000000 spec2nii-0.7.0/versioneer.py
```

### Comparing `spec2nii-0.6.9/CHANGELOG.md` & `spec2nii-0.7.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 This document contains the Spec2nii release history in reverse chronological order.
 
+0.7.0 (Saturday 5th August 2023)
+--------------------------------
+- Fixed a bug in Philips Classic DICOM orientations (supplementing the fixes to Enhanced DICOM in `0.6.11`)
+- Updated Hyper sequence special case for Siemens twix and GE.
+
+0.6.11 (Friday 28th July 2023)
+------------------------------
+- Fixed a bug in Philips spar/sdat orientations - this will affect voxels with rotations in more than one axes.
+- Fixed a bug in Philips DICOM orientations - this will affect voxels with rotations in more than one axes.
+- Python 3.7 now in [end of life](https://devguide.python.org/versions/) status and is no longer supported.
+- `spec2nii dump/extract/insert` can now be used to inspect and fix non-compliant NIfTI-MRS files.
+
+0.6.10 (Monday 10th July 2023)
+------------------------------
+- Stop tests being vendored as a top-level package. Bug introduced in `0.6.9`.
+
 0.6.9 (Friday 7th July 2023)
 ----------------------------
 - Add handling for the `fidall` sequence in GE.
 - Add handling for the `slaser` sequence in GE.
 - Update to nifti-mrs-tools 1.0.0 API.
 - Minor code fixes contributed by the community.
```

### Comparing `spec2nii-0.6.9/LICENSE` & `spec2nii-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/PKG-INFO` & `spec2nii-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: spec2nii
-Version: 0.6.9
+Version: 0.7.0
 Summary: Multi-format in vivo MR spectroscopy conversion to NIFTI
 Home-page: https://github.com/wtclarke/spec2nii
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spec2nii
 ![PyPI](https://img.shields.io/pypi/v/spec2nii)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spec2nii)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5907960.svg)](https://doi.org/10.5281/zenodo.5907960)
@@ -61,16 +60,16 @@
 | Format        | File extension | SVS | MRSI| Automatic orientation |
 |---------------|----------------|-----|-----|-----------------------|
 | Siemens Twix  | .dat           | Yes | †   | Yes                   |
 | Siemens DICOM | .ima / .dcm    | Yes | Yes | Yes                   |
 | Siemens RDA   | .rda           | Yes | No  | Yes (WIP)             |
 | Philips       | .SPAR/.SDAT    | Yes | No  | Yes                   |
 | Philips       | .data/.list    | Yes | No  | Yes                   |
-| Philips DICOM | .dcm           | Yes | No  | Yes (WIP)             |
-| GE            | .7 (pfile)     | Yes | Yes | Yes                   |
+| Philips DICOM | .dcm           | Yes | No  | Yes                   |
+| GE            | .7 (pfile)     | Yes | Yes | Yes  (WIP)            |
 | UIH DICOM     | .dcm           | Yes | Yes | Yes                   |
 | Bruker        | 2dseq          | Yes | Yes | Yes                   |
 | Bruker        | fid            | Yes | Yes | Yes (WIP)             |
 | Varian        | fid            | Yes | No  | No (WIP)              |
 | LCModel       | .RAW           | Yes | No  | No                    |
 | jMRUI         | .txt           | Yes | No  | No                    |
 | jMRUI         | .mrui          | Yes | No  | No                    |
@@ -122,28 +121,28 @@
 `spec2nii ge FILE`
 
 ### Philips (SPAR/SDAT)
 `spec2nii philips SDAT_FILE SPAR_FILE`
 
 Two optional arguments are available for the SPAR/SDAT pathway:
 - `-t/--tags` allows the user to specify the dimension tags for each of the higher dimensions (up to three).
-- `-s/--shape` allows the user to perform numpy style reshaping of multiple transients. By default (without specifying a shape) all transients will be listed in a single 5th dimension.
+- `-s/--shape` allows the user to perform Numpy style reshaping of multiple transients. By default (without specifying a shape) all transients will be listed in a single 5th dimension.
 
 ### Philips (data/list)
 Must be provided along side a matching SPAR file.
 `spec2nii philips_dl DATA_FILE LIST_FILE SPAR_FILE`
 
 ### Philips DICOM
 `spec2nii philips_dcm DCM_FILE_or_DIR`
 
 NIfTI MRS dimension tags (e.g. `DIM_COIL`) can be specified using the `-t` command line argument.
 
 Generates separate reference file if present.
 
-**NOTE** Only enhanced DICOM is currently handled. Older 'classic' DICOM may work but is likely to need more testing with appropriate example data first.
+Both classic and enhanced DICOM is handled.
 
 ### Bruker (2dseq/fid)
 `spec2nii bruker -m 2DSEQ 2DSEQ_FILE_or_DIR`
 `spec2nii bruker -m FID FID_FILE_or_DIR`
 
 Use the `-d` option to dump the header files (method and acqp for fid, visu_pars for 2dseq) into the header extension.
```

### Comparing `spec2nii-0.6.9/README.md` & `spec2nii-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 | Format        | File extension | SVS | MRSI| Automatic orientation |
 |---------------|----------------|-----|-----|-----------------------|
 | Siemens Twix  | .dat           | Yes | †   | Yes                   |
 | Siemens DICOM | .ima / .dcm    | Yes | Yes | Yes                   |
 | Siemens RDA   | .rda           | Yes | No  | Yes (WIP)             |
 | Philips       | .SPAR/.SDAT    | Yes | No  | Yes                   |
 | Philips       | .data/.list    | Yes | No  | Yes                   |
-| Philips DICOM | .dcm           | Yes | No  | Yes (WIP)             |
-| GE            | .7 (pfile)     | Yes | Yes | Yes                   |
+| Philips DICOM | .dcm           | Yes | No  | Yes                   |
+| GE            | .7 (pfile)     | Yes | Yes | Yes  (WIP)            |
 | UIH DICOM     | .dcm           | Yes | Yes | Yes                   |
 | Bruker        | 2dseq          | Yes | Yes | Yes                   |
 | Bruker        | fid            | Yes | Yes | Yes (WIP)             |
 | Varian        | fid            | Yes | No  | No (WIP)              |
 | LCModel       | .RAW           | Yes | No  | No                    |
 | jMRUI         | .txt           | Yes | No  | No                    |
 | jMRUI         | .mrui          | Yes | No  | No                    |
@@ -103,28 +103,28 @@
 `spec2nii ge FILE`
 
 ### Philips (SPAR/SDAT)
 `spec2nii philips SDAT_FILE SPAR_FILE`
 
 Two optional arguments are available for the SPAR/SDAT pathway:
 - `-t/--tags` allows the user to specify the dimension tags for each of the higher dimensions (up to three).
-- `-s/--shape` allows the user to perform numpy style reshaping of multiple transients. By default (without specifying a shape) all transients will be listed in a single 5th dimension.
+- `-s/--shape` allows the user to perform Numpy style reshaping of multiple transients. By default (without specifying a shape) all transients will be listed in a single 5th dimension.
 
 ### Philips (data/list)
 Must be provided along side a matching SPAR file.
 `spec2nii philips_dl DATA_FILE LIST_FILE SPAR_FILE`
 
 ### Philips DICOM
 `spec2nii philips_dcm DCM_FILE_or_DIR`
 
 NIfTI MRS dimension tags (e.g. `DIM_COIL`) can be specified using the `-t` command line argument.
 
 Generates separate reference file if present.
 
-**NOTE** Only enhanced DICOM is currently handled. Older 'classic' DICOM may work but is likely to need more testing with appropriate example data first.
+Both classic and enhanced DICOM is handled.
 
 ### Bruker (2dseq/fid)
 `spec2nii bruker -m 2DSEQ 2DSEQ_FILE_or_DIR`
 `spec2nii bruker -m FID FID_FILE_or_DIR`
 
 Use the `-d` option to dump the header files (method and acqp for fid, visu_pars for 2dseq) into the header extension.
```

### Comparing `spec2nii-0.6.9/setup.cfg` & `spec2nii-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/setup.py` & `spec2nii-0.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,25 +19,24 @@
       cmdclass=versioneer.get_cmdclass(),
       description='Multi-format in vivo MR spectroscopy conversion to NIFTI',
       author='Will Clarke',
       author_email='william.clarke@ndcn.ox.ac.uk',
       url='https://github.com/wtclarke/spec2nii',
       long_description=long_description,
       long_description_content_type="text/markdown",
-      packages=find_packages(),
+      packages=find_packages(exclude=["tests*"]),
       install_requires=install_requires,
       classifiers=[
           "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
           "License :: OSI Approved :: BSD License",
           "Operating System :: OS Independent"],
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       entry_points={"console_scripts": [
           "spec2nii = spec2nii.spec2nii:main"]},
       package_data={'spec2nii': ['bruker_properties.json',
                                  'bruker_fid_override.json'],
                     'spec2nii.GE': ['VESPA_LICENSE']}
       )
```

### Comparing `spec2nii-0.6.9/spec2nii/GE/VESPA_LICENSE` & `spec2nii-0.7.0/spec2nii/GE/VESPA_LICENSE`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/GE/ge_hdr_fields.py` & `spec2nii-0.7.0/spec2nii/GE/ge_hdr_fields.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/GE/ge_pfile.py` & `spec2nii-0.7.0/spec2nii/GE/ge_pfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     if psd in ('probe-p', 'probe-s'):
         data, meta, dwelltime, fname_suffix = _process_probe_p(pfile)
     elif psd in ('oslaser', 'slaser_cni'):
         data, meta, dwelltime, fname_suffix = _process_oslaser(pfile)
     elif psd in ('slaser'):
         data, meta, dwelltime, fname_suffix = _process_slaser(pfile)
-    elif psd == 'gaba':
+    elif psd in ['gaba', 'hbcd']:
         data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     elif 'jpress_ac' in psd:  # Bergen patch
         data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     elif psd == 'jpress':
         data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     else:
         raise UnsupportedPulseSequenceError(f'Unrecognised sequence {psd}.')
```

### Comparing `spec2nii-0.6.9/spec2nii/GE/ge_read_pfile.py` & `spec2nii-0.7.0/spec2nii/GE/ge_read_pfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,17 @@
             mapper = PfileMapper
         elif psd == 'epsi_3d_24':
             # bjs - added for soher check of MIDAS Browndyke data
             mapper = PfileMapper
         elif psd == 'gaba':
             # wtc - added for Nottingham MEGA-PRESS sequence.
             mapper = PfileMapperGaba
+        elif psd == 'hbcd':
+            # ATG - added HBCD - reuse GABA mapper
+            mapper = PfileMapperGaba
         elif psd == 'probe-sl':
             # wtc - added for CSI sequence from Manchester.
             mapper = PfileMapperProbeSL
         elif 'jpress_ac' in psd:
             # ARC : Added for Bergen jpress patch
             mapper = PfileMapperGaba
         elif psd == 'jpress':
@@ -1243,15 +1246,15 @@
         if nechoes == 1:
             tempData = tempData.reshape((1, 1, 1, nreceivers, totalframes, npoints))
             self.raw_data = np.swapaxes(tempData, -1, -3)
 
             if (dataframes + refframes) != nframes:
                 mult = 1
                 dataframes *= nex
-                refframes = nframes - dataframes
+                refframes = int(nframes - dataframes)
             else:
                 mult = 1.0 / nex
 
             self.raw_unsuppressed = self.raw_data[:, :, :, :, 1:(refframes + 1), :]
             self.raw_suppressed   = self.raw_data[:, :, :, :, (refframes + 1):, :]
 
         else:
```

### Comparing `spec2nii-0.6.9/spec2nii/GSL/gslfunctions.py` & `spec2nii-0.7.0/spec2nii/GSL/gslfunctions.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/Philips/philips.py` & `spec2nii-0.7.0/spec2nii/Philips/philips.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return _special_case_hyper_ref(data, dwelltime, meta, orientation.Q44, mainStr)
     elif spar_params['scan_id'].lower() == 'hyper'\
             or (special is not None and
                 special.lower() == 'hyper'):
         return _special_case_hyper(data, dwelltime, meta, orientation.Q44, mainStr)
     else:
         # Normal case
-        return [gen_nifti_mrs_hdr_ext(data, dwelltime, meta, orientation.Q44, no_conj=True), ],\
+        return [gen_nifti_mrs_hdr_ext(data, dwelltime, meta, orientation.Q44, no_conj=True), ], \
                [mainStr, ]
 
 
 def read_spar(filename):
     '''Read the .spar file.
     :param filename: file path
 
@@ -354,23 +354,23 @@
 
     meta_edited.set_dim_info(1, 'DIM_DYN')
     meta_edited.set_standard_def("EditPulse", edit_pulse_val)
     meta_edited.set_standard_def("WaterSuppressed", True)
     meta_edited.set_standard_def("EchoTime", 0.08)
 
     return [gen_nifti_mrs_hdr_ext(data_short_te, dwelltime, meta_short_te, orientation, no_conj=True),
-            gen_nifti_mrs_hdr_ext(data_edited, dwelltime, meta_edited, orientation, no_conj=True)],\
+            gen_nifti_mrs_hdr_ext(data_edited, dwelltime, meta_edited, orientation, no_conj=True)], \
            [fout_str + '_hyper_short_te', fout_str + '_hyper_edited']
 
 
 def _special_case_hyper_ref(data, dwelltime, meta, orientation, fout_str):
     """Special case handling for the HYPER sequence (water reference component).
 
     Contains 8 references (every 32 scans from index 0). Starts with TE = 80 and alternates to TE = 35.
-    Output two ntime x 4 (DIM_DYN) shape files to match main acqusition
+    Output two ntime x 4 (DIM_DYN) shape files to match main acquisition
 
     :param data: Combined short TE and editing-TE data
     :type data: numpy.ndarray
     :param dwelltime: Spectral dwelltime
     :type dwelltime: float
     :param meta: raw meta object extracted from data
     :type meta: nifti_mrs.hdr_ext.Hdr_Ext
@@ -395,9 +395,9 @@
 
     meta_edited = meta.copy()
     meta_edited.set_dim_info(0, 'DIM_DYN')
     meta_edited.set_standard_def("WaterSuppressed", False)
     meta_short_te.set_standard_def("EchoTime", 0.08)
 
     return [gen_nifti_mrs_hdr_ext(data_short_te, dwelltime, meta_short_te, orientation, no_conj=True),
-            gen_nifti_mrs_hdr_ext(data_edited, dwelltime, meta_edited, orientation, no_conj=True)],\
+            gen_nifti_mrs_hdr_ext(data_edited, dwelltime, meta_edited, orientation, no_conj=True)], \
            [fout_str + '_hyper_ref_short_te', fout_str + '_hyper_ref_edited']
```

### Comparing `spec2nii-0.6.9/spec2nii/Philips/philips_data_list.py` & `spec2nii-0.7.0/spec2nii/Philips/philips_data_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from nibabel.nicom.dicomwrappers import wrapper_from_file
 from pydicom.errors import InvalidDicomError
 
 from nifti_mrs.create_nmrs import gen_nifti_mrs_hdr_ext
 
 from spec2nii.Philips.philips import read_spar, spar_to_nmrs_hdrext, _philips_orientation
 from spec2nii.Philips.philips_dcm import \
-    _enhanced_dcm_svs_to_orientation,\
-    _is_new_format,\
-    _extractDicomMetadata_new,\
+    _enhanced_dcm_svs_to_orientation, \
+    _is_new_format, \
+    _extractDicomMetadata_new, \
     _extractDicomMetadata_old
 from spec2nii.nifti_orientation import NIFTIOrient
 
 
 index_options = ['STD', 'REJ', 'PHC', 'FRC', 'NOI', 'NAV']
 index_headers = ['typ', 'mix', 'dyn', 'card', 'echo', 'loca',
                  'chan', 'extr1', 'extr2', 'kx', 'ky', 'kz',
@@ -316,9 +316,9 @@
         'DIM_EDIT',
         dim_info,
         dim_header)
 
     meta_edited.set_dim_info(2, 'DIM_DYN')
     meta_edited.set_standard_def("EditPulse", edit_pulse_val)
 
-    return [data_short_te, data_edited],\
+    return [data_short_te, data_edited], \
            [meta_short_te, meta_edited]
```

### Comparing `spec2nii-0.6.9/spec2nii/Philips/philips_dcm.py` & `spec2nii-0.7.0/spec2nii/Philips/philips_dcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,48 +271,51 @@
 
 def _enhanced_dcm_svs_to_orientation(img, verbose=False):
     '''Convert the Volume Localization Sequence (0018,9126) enhanced DICOM tag
     to a 4x4 affine format.
 
     Assumes the center of all slabs are aligned currently.'''
 
-    # affine3 = []
-    # voxsize = []
-    # for vl in img.dcm_data.VolumeLocalizationSequence:
-    #     affine3.append(vl.SlabOrientation)
-    #     voxsize.append(vl.SlabThickness)
-    # affine3 = np.asarray(affine3)
-    # voxsize = np.diag(np.asarray(voxsize))
-
-    # locSeq = img.dcm_data.VolumeLocalizationSequence
-    # if not np.allclose(locSeq[0].MidSlabPosition, locSeq[1].MidSlabPosition) \
-    #         or not np.allclose(locSeq[0].MidSlabPosition, locSeq[2].MidSlabPosition):
-    #     raise ValueError('Mid Slab Position must be the same for all three entries')
-
-    # pos3 = np.asarray(img.dcm_data.VolumeLocalizationSequence[0].MidSlabPosition)
-
-    # affine4 = np.eye(4)
-    # affine4[:3, :3] = affine3 @ voxsize
-    # affine4[:3, 3] = pos3
-
-    # Above didn't work. Drop back to original method.
-
     # Extract dicom parameters
     if _is_new_format(img):
+        # Enhanced DICOM
+
+        '''
+        # Code before July 2023 when testing using JH data revealed problems.
         imageOrientationPatient = img.dcm_data.PerFrameFunctionalGroupsSequence[0]\
             .PlaneOrientationSequence[0].ImageOrientationPatient
         imageOrientationPatient = np.asarray(imageOrientationPatient).reshape(2, 3)
         imagePositionPatient = img.dcm_data.PerFrameFunctionalGroupsSequence[0]\
             .PlanePositionSequence[0].ImagePositionPatient
         imagePositionPatient = np.asarray(imagePositionPatient)
         xyzMM = [float(img.dcm_data.PerFrameFunctionalGroupsSequence[0].PixelMeasuresSequence[0].PixelSpacing[0]),
                  float(img.dcm_data.PerFrameFunctionalGroupsSequence[0].PixelMeasuresSequence[0].PixelSpacing[1]),
                  float(img.dcm_data.PerFrameFunctionalGroupsSequence[0].PixelMeasuresSequence[0].SliceThickness)]
         xyzMM = np.asarray(xyzMM)
+        '''
+
+        locSeq = img.dcm_data.VolumeLocalizationSequence
+        imageOrientationPatient = np.concatenate((locSeq[0].SlabOrientation, locSeq[1].SlabOrientation))
+        imageOrientationPatient = np.asarray(imageOrientationPatient).reshape(2, 3)
+        imageOrientationPatient *= -1
+        imagePositionPatient = np.asarray(locSeq[0].MidSlabPosition)
+        xyzMM = np.asarray(
+            [locSeq[1].SlabThickness,
+             locSeq[0].SlabThickness,
+             locSeq[2].SlabThickness])
+
+        return dcm_to_nifti_orientation(
+            imageOrientationPatient,
+            imagePositionPatient,
+            xyzMM,
+            (1, 1, 1),
+            half_shift=False,
+            verbose=verbose)
     else:
+        # Classic DICOM
         import warnings
         warnings.warn('The orientation and position code for old format Philips DICOM is untested.\
                        Please provide example data to improve the handling of this format.')
         # As implemented in vespa (vespa/analysis/fileio/dicom_philips.py#L181)
         try:
             section  = img.dcm_data[0x2005, 0x1085][0]
             angle_lr = float(section[0x02005, 0x1056].value)
@@ -321,39 +324,39 @@
             dim_lr   = float(section[0x02005, 0x1059].value)
             dim_ap   = float(section[0x02005, 0x1057].value)
             dim_hf   = float(section[0x02005, 0x1058].value)
             shift_lr = float(section[0x02005, 0x105c].value)
             shift_ap = float(section[0x02005, 0x105a].value)
             shift_hf = float(section[0x02005, 0x105b].value)
 
-            xyzMM = np.array([dim_lr, dim_ap, dim_hf])
+            # This matches the spar/sdat pathway in spec2nii.Philips.philips._philips_orientation
+            from spec2nii.nifti_orientation import NIFTIOrient, calc_affine
+            angles = [-angle_lr, -angle_ap, angle_hf]
+            dimensions = [dim_lr, dim_ap, dim_hf]
+            shift = [-shift_lr, -shift_ap, shift_hf]
 
-            from scipy.spatial.transform import Rotation
-            rot = Rotation.from_euler('xyz', [-angle_lr, -angle_ap, angle_hf], degrees=True)
-            # THIS NEEDS TESTING!!! CODE WILL PASS BUT I DON"T TRUST IT AT ALL.
-            imageOrientationPatient = rot.as_matrix()[:, :2].T
-            imagePositionPatient = [-shift_lr, -shift_ap, shift_hf]
+            return NIFTIOrient(calc_affine(angles, dimensions, shift))
 
         except KeyError:
             # Default orientation
-            print('No orientation infroamtion found in header. Tag (2005, 1085) missing. '
-                  'Default orientation will be used.')
+            print(
+                'No orientation information found in header. Tag (2005, 1085) missing. '
+                'Default orientation will be used.')
             imageOrientationPatient = [[1, 0, 0], [0, 1, 0]]
             imagePositionPatient = [0, 0, 0]
             xyzMM = [float(x) for x in img.dcm_data[0x0028, 0x0030].value] \
                 + [float(img.dcm_data[0x0018, 0x0050].value), ]
 
-    currNiftiOrientation = dcm_to_nifti_orientation(imageOrientationPatient,
-                                                    imagePositionPatient,
-                                                    xyzMM,
-                                                    (1, 1, 1),
-                                                    half_shift=False,
-                                                    verbose=verbose)
-
-    return currNiftiOrientation
+            return dcm_to_nifti_orientation(
+                imageOrientationPatient,
+                imagePositionPatient,
+                xyzMM,
+                (1, 1, 1),
+                half_shift=False,
+                verbose=verbose)
 
 
 def _extractDicomMetadata_old(dcmdata, water_suppressed=True):
     """ Extract information from the nibabel DICOM object to insert into the json header ext.
 
     Args:
         dcmdata: nibabel.nicom image object
```

### Comparing `spec2nii-0.6.9/spec2nii/Siemens/dicomfunctions.py` & `spec2nii-0.7.0/spec2nii/Siemens/dicomfunctions.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/Siemens/rda.py` & `spec2nii-0.7.0/spec2nii/Siemens/rda.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/Siemens/twix_special_case.py` & `spec2nii-0.7.0/spec2nii/Siemens/twix_special_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Functions to hangle sequences/situations that are special-cased
+"""Functions to handle sequences/situations that are special-cased
 converted from twix/.dat data.
 
 Will Clarke, University of Oxford, 2022
 """
 import numpy as np
 
 
@@ -29,15 +29,15 @@
         twixObj['hdr']['Phoenix'][('sWipMemBlock', 'alFree', '12')] = Pulse Duration
 
         twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree',  '8')] = 4.58 ppm
         twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree',  '9')] = 1.90 ppm
         twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '10')] = 3.67 ppm (unused here)
         twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '11')] = 4.18 ppm
 
-    Sequence Mode Referred to Above is Carried Over from mgs_svs sequenes:
+    Sequence Mode Referred to Above is Carried Over from mgs_svs sequences:
         0 = MEGA PRESS
         1 = HERMES GABA GSH
         2 = HERMES GABA GSH EtOH
         3 = HERCULES  (This is what should get chosen for HBCD)
         4 = HERMES GABA LAC
 
     Author : Aaron Gudmundson, Johns Hopkins University, 2023
@@ -56,26 +56,32 @@
 
     dim_info        = f'Hyper - {subseq_name}'                                                  # Subscan Name
 
     if subseq == 0:                                                                             # Short TE Water Ref
         reord_data = reord_data[:, :, 33::66]                                                   # Short TE Water Refs
         meta_obj.set_standard_def('EchoTime', short_TE)                                         # Echo Time
         meta_obj.set_standard_def('WaterSuppressed', False)                                     # Water Suppression
+        meta_obj.set_standard_def('TxOffset', 0.0)                                              # Transmitter Frequency
 
     elif subseq == 1:                                                                           # Long  TE Water Ref
         reord_data  = reord_data[:, :, 0::66]                                                   # Long  TE Water Refs
+        meta_obj.set_standard_def('EchoTime', 0.080)                                            # Echo Time
         meta_obj.set_standard_def('WaterSuppressed', False)                                     # Water Suppression
+        meta_obj.set_standard_def('TxOffset', 0.0)                                              # Transmitter Frequency
 
     elif subseq == 2:                                                                           # Short TE PRESS
         meta_obj.set_standard_def('EchoTime', short_TE)                                         # Echo Time
         meta_obj.set_standard_def('WaterSuppressed', True)                                      # Water Suppression
+        meta_obj.set_standard_def('TxOffset', -1.7)                                             # Transmitter Frequency
         reord_data  = reord_data[:, :, 1:33]                                                    # Isolated PRESS
 
     elif subseq == 3:                                                                           # Long  TE HERCULES
+        meta_obj.set_standard_def('EchoTime', 0.080)                                            # Echo Time
         meta_obj.set_standard_def('WaterSuppressed', True)                                      # Water Suppression
+        meta_obj.set_standard_def('TxOffset', -1.7)                                             # Transmitter Frequency
 
         reord_mask       = np.ones(reord_data.shape[-1], dtype=bool)                            # Create a Mask
         reord_mask[::33] = False                                                                # Remove Water Refs
         reord_mask[: 33] = False                                                                # Remove PRESS
         reord_data       = reord_data[..., reord_mask]                                          # Isolated HERCULES
 
         # Handle Incomplete
@@ -99,29 +105,29 @@
 
         orig_shape  = reord_data.shape[:-1]                                                     # Remove Averages Dim
         orig_shape += (edit_cases, -1)                                                          # Include Subscans
         reord_data  = reord_data.T.reshape(orig_shape[::-1]).T                                  # With Subscan Dim
 
         dim_tags.insert(len(orig_shape) - 3, 'DIM_EDIT')                                        # Update Dimensions
 
-        for idx, dt in enumerate(dim_tags):                                                     # Iterate Dimensions
-            if dt == 'DIM_EDIT':
-                meta_obj.set_dim_info(idx, dt, dim_info, dim_header)                            # Set Dimension
-            else:
-                meta_obj.set_dim_info(idx, dt)                                                  # Set Dimension
+    for idx, dt in enumerate(dim_tags):                                                         # Iterate Dimensions
+        if dt == 'DIM_EDIT':
+            meta_obj.set_dim_info(idx, dt, dim_info, dim_header)                                # Set Dimension
+        else:
+            meta_obj.set_dim_info(idx, dt)                                                      # Set Dimension
 
     print(f'{subseq:3d} {subseq_name:<20} - Completed  - Final Array Size: ', reord_data.shape)
 
     return reord_data, meta_obj, dim_tags
 
 
 def mgs_svs_ed_twix(twixObj, reord_data, meta_obj, dim_tags):
     """Special case handling for the mgs_svs_ed (VX) and smm_svs_herc (XA) sequence
 
-    MEGA/HURCULES sequence (2/4 editing case)
+    MEGA/HERCULES sequence (2/4 editing case)
     """
     seq_mode = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'alFree', '7')]
     pulse_length = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'alFree', '12')] / 1E6
     edit_pulse_1 = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '8')]
     edit_pulse_2 = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '9')]
     edit_pulse_3 = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '10')]
     edit_pulse_off = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '11')]
```

### Comparing `spec2nii-0.6.9/spec2nii/Siemens/twixfunctions.py` & `spec2nii-0.7.0/spec2nii/Siemens/twixfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,39 +379,30 @@
 
         hyp_names  = ['35ms Water Reference',
                       '80ms Water Reference',
                       '35ms PRESS',
                       '80ms HERCULES']                                                      # Hyper Subscan Names
         hyp_suffix = ['ref_short_te', 'ref_edited', 'short_te', 'edited']                   # Hyper Suffixes
 
-        reord_list = []                                                                     # List of Reord Data
-        meta_list  = []                                                                     # List of Meta Objects
-        dim_list   = []                                                                     # List of Dimensions
-
         # Reording the Data & Adjusting the Header Appropriately
         for ii in range(len(hyp_names)):                                                    # Iterate over Subscans
             print(f'{ii:3d} {hyp_names[ii]:<20}', end='\r')
             reord_data_, meta_obj_, dim_tags_ = smm_svs_herc_hyper(twixObj,
                                                                    reord_data,
                                                                    meta_obj,
                                                                    dim_tags,
                                                                    subseq=ii,
                                                                    subseq_name=hyp_names[ii])
 
-            reord_list.append(reord_data_)                                                  # Current Scan Data
-            meta_list.append(meta_obj_)                                                     # Current Scan Metadata
-            dim_list.append(dim_tags_)                                                      # Current Scan Dimensions
-
-        for ii in range(len(hyp_names)):
-            if reord_list[ii].ndim <= 4:                                                    # 4 or less Dims
-                newshape  = (1, 1, 1) + reord_list[ii].shape                                # Pad 3 singleton dims
-                nifit_mrs_out.append(assemble_nifti_mrs(reord_list[ii].reshape(newshape),
+            if reord_data_.ndim <= 4:                                                       # 4 or less Dims
+                newshape  = (1, 1, 1) + reord_data_.shape                                   # Pad 3 singleton dims
+                nifit_mrs_out.append(assemble_nifti_mrs(reord_data_.reshape(newshape),
                                                         dwellTime,
                                                         orientation,
-                                                        meta_list[ii]))
+                                                        meta_obj_))
                 filename_out.append(f'{mainStr}_{hyp_suffix[ii]}')
 
         return nifit_mrs_out, filename_out
 
     # HERCULES Data
     elif (xa_or_vx(twixObj['hdr']) == 'xa' and 'smm_svs_herc' in twixObj['hdr']['Meas'][('tSequenceFileName')]):
         from spec2nii.Siemens.twix_special_case import mgs_svs_ed_twix
```

### Comparing `spec2nii-0.6.9/spec2nii/anonymise.py` & `spec2nii-0.7.0/spec2nii/anonymise.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/bruker.py` & `spec2nii-0.7.0/spec2nii/bruker.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/bruker_fid_override.json` & `spec2nii-0.7.0/spec2nii/bruker_fid_override.json`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/bruker_properties.json` & `spec2nii-0.7.0/spec2nii/bruker_properties.json`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/dcm2niiOrientation/orientationFuncs.py` & `spec2nii-0.7.0/spec2nii/dcm2niiOrientation/orientationFuncs.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/fileiobase.py` & `spec2nii-0.7.0/spec2nii/fileiobase.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/jmrui.py` & `spec2nii-0.7.0/spec2nii/jmrui.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/nifti_orientation.py` & `spec2nii-0.7.0/spec2nii/nifti_orientation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         self.dz = dz
         self.qfac = qfac
 
 
 def calc_affine(angles, dimensions, shift):
 
     scalingMat = np.diag(dimensions)
-    rot = Rotation.from_euler('xyz', angles, degrees=True)
+    # Rotations appear to be intrinsic
+    rot = Rotation.from_euler('XYZ', angles, degrees=True)
     m33 = rot.as_matrix() @ scalingMat
     m44 = np.zeros((4, 4))
     m44[0:3, 0:3] = m33
     m44[3, 3] = 1.0
     m44[0:3, 3] = shift
 
     return m44
```

### Comparing `spec2nii-0.6.9/spec2nii/other.py` & `spec2nii-0.7.0/spec2nii/other.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def dump_headers(args):
     """Print the nifti headers and header extensions
 
     :param args: Command line arguments
     """
     # Load file
-    nifti_mrs_img = NIFTI_MRS(args.file)
+    nifti_mrs_img = NIFTI_MRS(args.file, validate_on_creation=False)
 
     # Print NIfTI header
     print('NIfTI header: ')
     print(nifti_mrs_img.header)
 
     print('\nNIfTI-MRS header extension: ')
     pp = pprint.PrettyPrinter()
@@ -27,15 +27,15 @@
 
 
 def extract_hdr_ext(args):
     """Generate a json sidecar file for input file
 
     :param args: Command line arguments
     """
-    nifti_mrs_img = NIFTI_MRS(args.file)
+    nifti_mrs_img = NIFTI_MRS(args.file, validate_on_creation=False)
 
     if args.outdir:
         args.outdir.mkdir(exist_ok=True, parents=True)
         out_json = args.outdir / (args.file.with_suffix('').with_suffix('').name + '.json')
     else:
         out_json = args.file.parent / (args.file.with_suffix('').with_suffix('').name + '.json')
 
@@ -54,15 +54,15 @@
     """
 
     with open(args.json_file) as jf:
         new_hdr = json.load(jf)
 
     # Load data
     try:
-        nifti_mrs_img = NIFTI_MRS(args.file)
+        nifti_mrs_img = NIFTI_MRS(args.file, validate_on_creation=False)
         nifti_mrs_img.hdr_ext = new_hdr
 
     except NotNIFTI_MRS:
         print(f'{args.file} is not compliant with the NIfTI-MRS standard, attempting to convert')
         from fsl.data.image import Image
         from nifti_mrs.create_nmrs import gen_nifti_mrs_hdr_ext
         from nifti_mrs.hdr_ext import Hdr_Ext
```

### Comparing `spec2nii-0.6.9/spec2nii/other_formats.py` & `spec2nii-0.7.0/spec2nii/other_formats.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/spec2nii.py` & `spec2nii-0.7.0/spec2nii/spec2nii.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/uih.py` & `spec2nii-0.7.0/spec2nii/uih.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/varian.py` & `spec2nii-0.7.0/spec2nii/varian.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii/varian_importer.py` & `spec2nii-0.7.0/spec2nii/varian_importer.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/spec2nii.egg-info/PKG-INFO` & `spec2nii-0.7.0/spec2nii.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: spec2nii
-Version: 0.6.9
+Version: 0.7.0
 Summary: Multi-format in vivo MR spectroscopy conversion to NIFTI
 Home-page: https://github.com/wtclarke/spec2nii
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spec2nii
 ![PyPI](https://img.shields.io/pypi/v/spec2nii)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spec2nii)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5907960.svg)](https://doi.org/10.5281/zenodo.5907960)
@@ -61,16 +60,16 @@
 | Format        | File extension | SVS | MRSI| Automatic orientation |
 |---------------|----------------|-----|-----|-----------------------|
 | Siemens Twix  | .dat           | Yes | †   | Yes                   |
 | Siemens DICOM | .ima / .dcm    | Yes | Yes | Yes                   |
 | Siemens RDA   | .rda           | Yes | No  | Yes (WIP)             |
 | Philips       | .SPAR/.SDAT    | Yes | No  | Yes                   |
 | Philips       | .data/.list    | Yes | No  | Yes                   |
-| Philips DICOM | .dcm           | Yes | No  | Yes (WIP)             |
-| GE            | .7 (pfile)     | Yes | Yes | Yes                   |
+| Philips DICOM | .dcm           | Yes | No  | Yes                   |
+| GE            | .7 (pfile)     | Yes | Yes | Yes  (WIP)            |
 | UIH DICOM     | .dcm           | Yes | Yes | Yes                   |
 | Bruker        | 2dseq          | Yes | Yes | Yes                   |
 | Bruker        | fid            | Yes | Yes | Yes (WIP)             |
 | Varian        | fid            | Yes | No  | No (WIP)              |
 | LCModel       | .RAW           | Yes | No  | No                    |
 | jMRUI         | .txt           | Yes | No  | No                    |
 | jMRUI         | .mrui          | Yes | No  | No                    |
@@ -122,28 +121,28 @@
 `spec2nii ge FILE`
 
 ### Philips (SPAR/SDAT)
 `spec2nii philips SDAT_FILE SPAR_FILE`
 
 Two optional arguments are available for the SPAR/SDAT pathway:
 - `-t/--tags` allows the user to specify the dimension tags for each of the higher dimensions (up to three).
-- `-s/--shape` allows the user to perform numpy style reshaping of multiple transients. By default (without specifying a shape) all transients will be listed in a single 5th dimension.
+- `-s/--shape` allows the user to perform Numpy style reshaping of multiple transients. By default (without specifying a shape) all transients will be listed in a single 5th dimension.
 
 ### Philips (data/list)
 Must be provided along side a matching SPAR file.
 `spec2nii philips_dl DATA_FILE LIST_FILE SPAR_FILE`
 
 ### Philips DICOM
 `spec2nii philips_dcm DCM_FILE_or_DIR`
 
 NIfTI MRS dimension tags (e.g. `DIM_COIL`) can be specified using the `-t` command line argument.
 
 Generates separate reference file if present.
 
-**NOTE** Only enhanced DICOM is currently handled. Older 'classic' DICOM may work but is likely to need more testing with appropriate example data first.
+Both classic and enhanced DICOM is handled.
 
 ### Bruker (2dseq/fid)
 `spec2nii bruker -m 2DSEQ 2DSEQ_FILE_or_DIR`
 `spec2nii bruker -m FID FID_FILE_or_DIR`
 
 Use the `-d` option to dump the header files (method and acqp for fid, visu_pars for 2dseq) into the header extension.
```

### Comparing `spec2nii-0.6.9/spec2nii.egg-info/SOURCES.txt` & `spec2nii-0.7.0/spec2nii.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,27 @@
 spec2nii/Siemens/__init__.py
 spec2nii/Siemens/dicomfunctions.py
 spec2nii/Siemens/rda.py
 spec2nii/Siemens/twix_special_case.py
 spec2nii/Siemens/twixfunctions.py
 spec2nii/dcm2niiOrientation/__init__.py
 spec2nii/dcm2niiOrientation/orientationFuncs.py
-tests/__init__.py
-tests/io_for_tests.py
 tests/test_anon.py
 tests/test_auto.py
 tests/test_bruker.py
 tests/test_ge_pfile.py
 tests/test_ge_pfile_orientation.py
 tests/test_jmrui.py
 tests/test_nifti_options.py
 tests/test_other.py
 tests/test_other_func.py
 tests/test_philips_data_list.py
 tests/test_philips_dicom.py
 tests/test_philips_dicom_orientation.py
+tests/test_philips_orientation_dcm_spar_new.py
 tests/test_philips_sdat_spar.py
 tests/test_philips_sdat_spar_orientation.py
 tests/test_siemens_dicom.py
 tests/test_siemens_mrsi_orientation.py
 tests/test_siemens_rda.py
 tests/test_siemens_special_data.py
 tests/test_siemens_svs_orientation.py
```

### Comparing `spec2nii-0.6.9/tests/test_anon.py` & `spec2nii-0.7.0/tests/test_anon.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_auto.py` & `spec2nii-0.7.0/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_bruker.py` & `spec2nii-0.7.0/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_ge_pfile.py` & `spec2nii-0.7.0/tests/test_ge_pfile.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_ge_pfile_orientation.py` & `spec2nii-0.7.0/tests/test_ge_pfile_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_jmrui.py` & `spec2nii-0.7.0/tests/test_jmrui.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_nifti_options.py` & `spec2nii-0.7.0/tests/test_nifti_options.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_other.py` & `spec2nii-0.7.0/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_other_func.py` & `spec2nii-0.7.0/tests/test_other_func.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_philips_data_list.py` & `spec2nii-0.7.0/tests/test_philips_data_list.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_philips_dicom.py` & `spec2nii-0.7.0/tests/test_philips_dicom.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_philips_dicom_orientation.py` & `spec2nii-0.7.0/tests/test_philips_dicom_orientation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-'''Orientation tests for Philips DICOM format conversion.
+'''OLD Orientation tests for Philips DICOM format conversion.
+This test has been superseded by the new test test_philips_orientation_dcm_spar_new.py
 
 Copyright William Clarke, University of Oxford 2021
 Subject to the BSD 3-Clause License.
 '''
 
 import subprocess
 from pathlib import Path
@@ -64,30 +65,29 @@
         out.paste(cropped_0, (int(width / 3), 0))
         out.paste(cropped_1, (2 * int(width / 3) + 17, 0))
     return out
 
 
 @pytest.mark.orientation
 def test_svs_orientation(tmp_path):
-
     sub_images = []
     for idx, (d_path, p_path, pos) in enumerate(zip(data_path, screenshot_path, t1_pos)):
         subprocess.check_call(['spec2nii', 'philips_dcm',
-                               '-f', 'svs',
+                               '-f', f'svs_{idx}',
                                '-o', tmp_path,
                                '-j',
                                str(d_path)])
 
         # Make fsleyes rendering
         subprocess.check_call(['fsleyes', 'render',
                                '-of', tmp_path / f'svs_{idx}.png',
                                '-vl', str(pos[0]), str(pos[1]), str(pos[2]),
                                '-xc', '0', '0', '-yc', '0', '0', '-zc', '0', '0',
                                '-hc', structural_data,
-                               tmp_path / 'svs.nii.gz', '-ot', 'complex',
+                               tmp_path / f'svs_{idx}.nii.gz', '-ot', 'complex',
                                '-a', '50', '-cm', 'blue'])
 
         fsl_ss = Image.open(tmp_path / f'svs_{idx}.png')
         width, height = fsl_ss.size
         if idx == 2:
             swap = '123'
         else:
@@ -102,13 +102,13 @@
         fsl_ss_cropped = fsl_ss_cropped.resize(ss_cropped.size)
         sub_images.append(get_concat_v(fsl_ss_cropped, ss_cropped))
 
     final_img = Image.new('RGB', (sub_images[0].width * 2, sub_images[0].height * 3))
     draw = ImageDraw.Draw(final_img)
     for idx, si in enumerate(sub_images):
         c = idx % 2
-        r = int(idx / 3)
-        final_img.paste(si, (si.width * r, si.height * c))
-        draw.text((10 + si.width * r, 10 + si.height * c), f'P{idx + 1}', (255, 0, 0))
+        r = int(idx / 2)
+        final_img.paste(si, (si.width * c, si.height * r))
+        draw.text((10 + si.width * c, 10 + si.height * r), f'P{idx + 1}', (255, 0, 0))
 
     final_img.save(output_path / 'philips_dicom_svs.png')
     print(tmp_path)
```

### Comparing `spec2nii-0.6.9/tests/test_philips_sdat_spar.py` & `spec2nii-0.7.0/tests/test_philips_sdat_spar.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_philips_sdat_spar_orientation.py` & `spec2nii-0.7.0/tests/test_philips_sdat_spar_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_siemens_dicom.py` & `spec2nii-0.7.0/tests/test_siemens_dicom.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_siemens_mrsi_orientation.py` & `spec2nii-0.7.0/tests/test_siemens_mrsi_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_siemens_rda.py` & `spec2nii-0.7.0/tests/test_siemens_rda.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_siemens_special_data.py` & `spec2nii-0.7.0/tests/test_siemens_special_data.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_siemens_svs_orientation.py` & `spec2nii-0.7.0/tests/test_siemens_svs_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_twix.py` & `spec2nii-0.7.0/tests/test_twix.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_uih.py` & `spec2nii-0.7.0/tests/test_uih.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_uih_orientation.py` & `spec2nii-0.7.0/tests/test_uih_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/tests/test_varian.py` & `spec2nii-0.7.0/tests/test_varian.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.9/versioneer.py` & `spec2nii-0.7.0/versioneer.py`

 * *Files identical despite different names*

