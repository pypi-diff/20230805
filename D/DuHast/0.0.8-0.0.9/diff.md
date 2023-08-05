# Comparing `tmp/DuHast-0.0.8.tar.gz` & `tmp/DuHast-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DuHast-0.0.8.tar", last modified: Mon Jul 24 10:42:36 2023, max compression
+gzip compressed data, was "DuHast-0.0.9.tar", last modified: Sat Aug  5 10:26:20 2023, max compression
```

## Comparing `DuHast-0.0.8.tar` & `DuHast-0.0.9.tar`

### file list

```diff
@@ -1,493 +1,509 @@
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.434000 DuHast-0.0.8/
--rw-r--r--   0 janchristel   (501) staff       (20)       66 2023-07-23 12:58:56.000000 DuHast-0.0.8/MANIFEST.in
--rw-r--r--   0 janchristel   (501) staff       (20)      780 2023-07-24 10:42:36.434285 DuHast-0.0.8/PKG-INFO
--rw-r--r--   0 janchristel   (501) staff       (20)      407 2023-07-12 08:39:01.000000 DuHast-0.0.8/README.md
--rw-r--r--   0 janchristel   (501) staff       (20)      643 2023-07-24 10:21:13.000000 DuHast-0.0.8/pyproject.toml
--rw-r--r--   0 janchristel   (501) staff       (20)      394 2023-07-24 10:42:36.435286 DuHast-0.0.8/setup.cfg
--rw-r--r--   0 janchristel   (501) staff       (20)      474 2023-07-12 08:39:01.000000 DuHast-0.0.8/setup.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.170902 DuHast-0.0.8/src/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.194741 DuHast-0.0.8/src/DuHast.egg-info/
--rw-r--r--   0 janchristel   (501) staff       (20)      780 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/PKG-INFO
--rw-r--r--   0 janchristel   (501) staff       (20)    19041 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/SOURCES.txt
--rw-r--r--   0 janchristel   (501) staff       (20)        1 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/dependency_links.txt
--rw-r--r--   0 janchristel   (501) staff       (20)        7 2023-07-24 10:42:36.000000 DuHast-0.0.8/src/DuHast.egg-info/top_level.txt
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.195283 DuHast-0.0.8/src/duHast/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.196517 DuHast-0.0.8/src/duHast/Data/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.198106 DuHast-0.0.8/src/duHast/Data/Objects/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.202705 DuHast-0.0.8/src/duHast/Data/Objects/Properties/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.205420 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7146 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2144 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3720 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3133 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2820 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3336 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_design_set_option.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4202 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_element_geometry.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3089 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_instance_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3215 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_level.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3072 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_phasing.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2894 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_revit_model.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3215 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_type_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Objects/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5997 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/data_ceiling.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5419 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Objects/data_room.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.207578 DuHast-0.0.8/src/duHast/Data/Utils/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/Utils/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2452 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2868 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_export.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6201 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_import.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2732 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/Utils/data_to_file.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10863 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/data_to_shapely.py
--rw-r--r--   0 janchristel   (501) staff       (20)    22884 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Data/process_ceilings_to_rooms.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.208870 DuHast-0.0.8/src/duHast/Revit/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.214277 DuHast-0.0.8/src/duHast/Revit/Annotation/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.217563 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1296 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2609 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1278 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7001 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.218670 DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3693 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3078 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/annotation.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5149 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/arrow_heads.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4369 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/dimensions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3684 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/generic_annotation.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3078 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6455 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7452 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_modify_properties.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6135 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3979 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/multi_ref_annotation.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12895 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/purge_unused_annotation_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4334 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/spot_dimensions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2879 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/stair_path.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3660 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Annotation/text.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.220493 DuHast-0.0.8/src/duHast/Revit/BIM360/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BIM360/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5104 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BIM360/bim_360.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4372 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BIM360/util_bim_360.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.222185 DuHast-0.0.8/src/duHast/Revit/BuildingPads/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.223357 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2044 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.225274 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     3950 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2324 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:56.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5676 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/building_pads.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4787 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.227538 DuHast-0.0.8/src/duHast/Revit/Categories/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.230039 DuHast-0.0.8/src/duHast/Revit/Categories/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12624 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10648 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4708 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_purge_unused.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.232110 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3052 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6769 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_utils.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.235307 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7330 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12561 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2766 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_property_names.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12740 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10421 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/categories.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3675 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Categories/change_family_category.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13460 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Categories/family_sub_categories.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.237104 DuHast-0.0.8/src/duHast/Revit/Ceilings/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.238221 DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6363 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.239337 DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3239 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/geometry.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.241657 DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1221 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.243544 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2330 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3013 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6718 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/ceilings.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6184 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.254776 DuHast-0.0.8/src/duHast/Revit/Common/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.256463 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    24242 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/geometry.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2318 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Geometry/solids.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.259231 DuHast-0.0.8/src/duHast/Revit/Common/Objects/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3085 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/colour_base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2270 2023-07-24 10:28:32.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_cut.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3379 2023-07-24 10:32:37.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_graphic_base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2298 2023-07-24 10:32:43.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_projection.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2322 2023-07-24 10:33:04.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_background.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2322 2023-07-24 10:33:10.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_foreground.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3425 2023-07-24 10:33:17.000000 DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_graphic_base.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.260539 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2030 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/groups_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2019 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2737 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15678 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/common.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4951 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4273 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_actions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4548 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_tests.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5119 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/delete.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5636 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/design_set_options.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7988 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/element_filtering.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11442 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/file_io.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8015 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/groups.py
--rw-r--r--   0 janchristel   (501) staff       (20)    19924 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/parameter_get_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4357 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/parameter_grouping.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9995 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/parameter_set_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2274 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/phases.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8916 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/purge_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)      289 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/revit_version.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3519 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Common/transaction.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15172 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Common/worksets.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.261502 DuHast-0.0.8/src/duHast/Revit/DetailItems/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.262321 DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1207 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.262966 DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2673 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6435 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/detail_items.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8656 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.265019 DuHast-0.0.8/src/duHast/Revit/Exports/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.270825 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7953 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8068 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8105 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13561 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13564 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2305 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14053 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_settings.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2105 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Exports/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2831 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/export.py
--rw-r--r--   0 janchristel   (501) staff       (20)    17682 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/export_ifc.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10789 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Exports/export_navis.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.277020 DuHast-0.0.8/src/duHast/Revit/Family/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.290265 DuHast-0.0.8/src/duHast/Revit/Family/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7889 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15521 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11953 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_missing_families.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4383 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12682 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py
--rw-r--r--   0 janchristel   (501) staff       (20)    16815 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    23829 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_category_data_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10972 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_data_collector.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6755 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7792 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_files.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8666 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_find_host_families.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8083 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_loaded_families.py
--rw-r--r--   0 janchristel   (501) staff       (20)    19921 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/family_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2346 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_action.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4278 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9216 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_processor.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.291359 DuHast-0.0.8/src/duHast/Revit/Family/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10439 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/Utility/loadable_family_categories.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3782 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_element_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1734 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_load_option.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5737 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_parameter_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7608 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_reference_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9406 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_reload.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5993 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_rename_files_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)    16256 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/family_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7401 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Family/purge_unused_family_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.292872 DuHast-0.0.8/src/duHast/Revit/Floors/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.293520 DuHast-0.0.8/src/duHast/Revit/Floors/Export/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Export/__init__.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.294548 DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1213 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/floors_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.296369 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2376 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2993 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6963 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Floors/floors.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5625 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Floors/purge_unused_floor_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.299346 DuHast-0.0.8/src/duHast/Revit/Grids/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.301052 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2849 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grid_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2059 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grids_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Grids/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8256 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/grids.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14876 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/grids_appearance.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6624 2023-07-24 10:32:46.000000 DuHast-0.0.8/src/duHast/Revit/Grids/grids_worksets.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3456 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Grids/purge_unused_grid_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7652 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/LICENSE
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.303732 DuHast-0.0.8/src/duHast/Revit/Levels/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.305407 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2021 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2914 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Levels/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4732 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Levels/levels.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14798 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/levels_appearance.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4496 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Levels/purge_unused_level_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.309670 DuHast-0.0.8/src/duHast/Revit/LinePattern/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2221 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/fill_patterns.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12827 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7537 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4312 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10621 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_patterns.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3360 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/LinePattern/line_styles.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.313221 DuHast-0.0.8/src/duHast/Revit/Links/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.316383 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2062 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5068 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2121 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5072 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_utils.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.317616 DuHast-0.0.8/src/duHast/Revit/Links/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1562 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/Utility/link_path.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Links/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9372 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/cad_links.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3455 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/cad_links_geometry.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5379 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/image_links.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11463 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/links.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3412 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Links/purge_unused_image_link_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.322653 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.323739 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1976 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.327184 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     2487 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3485 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3814 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3763 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6507 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6366 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/cable_trays.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6278 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/conduits.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6366 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/ducts.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6480 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/flex_ducts.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6149 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/pipes.py
--rw-r--r--   0 janchristel   (501) staff       (20)    11392 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py
--rw-r--r--   0 janchristel   (501) staff       (20)    14331 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.328059 DuHast-0.0.8/src/duHast/Revit/Materials/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.332934 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2064 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3471 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Materials/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3554 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Materials/materials.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.333974 DuHast-0.0.8/src/duHast/Revit/ModelHealth/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.335107 DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5675 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    27455 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/ModelHealth/model_health.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.337739 DuHast-0.0.8/src/duHast/Revit/Purge/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Purge/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3735 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Purge/purge_action.py
--rw-r--r--   0 janchristel   (501) staff       (20)    25813 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7869 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused_e_transmit.py
--rw-r--r--   0 janchristel   (501) staff       (20)      402 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/README.md
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.339855 DuHast-0.0.8/src/duHast/Revit/Railings/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.340849 DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2024 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/railings_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.344234 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2487 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/merge_lists.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2431 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_categories.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2230 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_family_names.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4327 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3773 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7015 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/balusters.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7825 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8385 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Railings/railings.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.345843 DuHast-0.0.8/src/duHast/Revit/Ramps/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.346872 DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2013 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.349417 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     1993 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2356 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3589 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4005 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/purge_unused_ramp_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3588 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Ramps/ramps.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.351814 DuHast-0.0.8/src/duHast/Revit/Revisions/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6698 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/new_revision.py
--rw-r--r--   0 janchristel   (501) staff       (20)    18321 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/revisions.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4524 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Revisions/sequence.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.352842 DuHast-0.0.8/src/duHast/Revit/Roofs/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.353461 DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2013 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.354838 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)     2121 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3035 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3716 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5651 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/purge_unused_roof_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6312 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Roofs/roofs.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.355717 DuHast-0.0.8/src/duHast/Revit/Rooms/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.356321 DuHast-0.0.8/src/duHast/Revit/Rooms/Export/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Export/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6045 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Export/to_data_room.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.356935 DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5565 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/geometry.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.357559 DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1194 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3698 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/room_tags.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4473 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Rooms/rooms.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.360234 DuHast-0.0.8/src/duHast/Revit/SharedParameters/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.361247 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)     5295 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7833 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5764 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.362206 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4832 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2074 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13905 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_add.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5295 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8096 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_swap.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8193 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py
--rw-r--r--   0 janchristel   (501) staff       (20)    10845 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6667 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_delete.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1215 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.365415 DuHast-0.0.8/src/duHast/Revit/Stairs/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.366302 DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2019 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.367774 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2448 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3604 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2210 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/cut_marks.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2223 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/landings.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2574 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/path.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15680 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/purge_unused_stair_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2170 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/runs.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5819 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/stairs.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2539 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Stairs/stringers_carriages.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.373472 DuHast-0.0.8/src/duHast/Revit/Views/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.377072 DuHast-0.0.8/src/duHast/Revit/Views/Objects/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3700 2023-07-24 10:35:01.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/category_base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2596 2023-07-24 10:34:10.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_by_category.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2299 2023-07-24 10:34:15.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_by_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3822 2023-07-24 10:34:40.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_cut.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3996 2023-07-24 10:34:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_projection.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3983 2023-07-24 10:34:50.000000 DuHast-0.0.8/src/duHast/Revit/Views/Objects/view_graphics_settings.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.380661 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7426 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/schedules_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6825 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/sheets_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3141 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2541 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7502 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4724 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.382220 DuHast-0.0.8/src/duHast/Revit/Views/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2795 2023-07-24 10:40:32.000000 DuHast-0.0.8/src/duHast/Revit/Views/Utility/data_view.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1527 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/Utility/view_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9094 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/delete.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5923 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/filters.py
--rw-r--r--   0 janchristel   (501) staff       (20)    15057 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Views/referencing.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3619 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/schedules.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5901 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/sheets.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7016 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/templates.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6545 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/views.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8145 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/views_purge_unused.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4849 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Views/visibility_graphics_utils.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.386049 DuHast-0.0.8/src/duHast/Revit/Walls/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.387640 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3909 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report.py
--rw-r--r--   0 janchristel   (501) staff       (20)     1299 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report_header.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.389226 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2052 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_filter.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2967 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_type_sorting.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9609 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/curtain_wall_elements.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3207 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/curtain_walls.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5681 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7760 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_wall_types.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2912 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/stacked_walls.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6331 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Walls/walls.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.412592 DuHast-0.0.8/src/duHast/Revit/Warnings/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.413629 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4861 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3725 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data_processor.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5498 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/solver.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5490 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/solver_duplicate_mark.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3641 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/solver_room_tag_to_room.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2413 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/Warnings/warnings.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Revit/__init__.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.419415 DuHast-0.0.8/src/duHast/UI/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:01.000000 DuHast-0.0.8/src/duHast/UI/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3001 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/file_item.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9641 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/UI/file_list.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3240 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/file_select_settings.py
--rw-r--r--   0 janchristel   (501) staff       (20)    13347 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/script.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7559 2023-07-12 08:39:01.000000 DuHast-0.0.8/src/duHast/UI/ui.xaml
--rw-r--r--   0 janchristel   (501) staff       (20)     4907 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/ui_file_select.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3282 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/workload_bucket.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4349 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/UI/workloader.py
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.431136 DuHast-0.0.8/src/duHast/Utilities/
-drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-07-24 10:42:36.433444 DuHast-0.0.8/src/duHast/Utilities/Objects/
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2872 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/base.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4896 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/result.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3669 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/Objects/timer.py
--rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-07-12 08:39:01.000000 DuHast-0.0.8/src/duHast/Utilities/__init__.py
--rw-r--r--   0 janchristel   (501) staff       (20)    29998 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/batch_processor_log_utils.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3500 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/compare.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4916 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/console_out.py
--rw-r--r--   0 janchristel   (501) staff       (20)     4818 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/date_stamps.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5343 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/directory_io.py
--rw-r--r--   0 janchristel   (501) staff       (20)    12861 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_combine.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5425 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_csv.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8431 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_get.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8550 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_io.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3813 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_json.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5061 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/files_tab.py
--rw-r--r--   0 janchristel   (501) staff       (20)     5053 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/padding.py
--rw-r--r--   0 janchristel   (501) staff       (20)     8755 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/solibri_ifc_optimizer.py
--rw-r--r--   0 janchristel   (501) staff       (20)     7525 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/system_process.py
--rw-r--r--   0 janchristel   (501) staff       (20)     2665 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/unit_conversion.py
--rw-r--r--   0 janchristel   (501) staff       (20)     3773 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/util_batch_p.py
--rw-r--r--   0 janchristel   (501) staff       (20)     6651 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/utility.py
--rw-r--r--   0 janchristel   (501) staff       (20)     9172 2023-07-24 10:19:35.000000 DuHast-0.0.8/src/duHast/Utilities/worksharing_monitor_process.py
--rw-r--r--   0 janchristel   (501) staff       (20)      246 2023-07-23 12:58:57.000000 DuHast-0.0.8/src/duHast/__init__.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.958409 DuHast-0.0.9/
+-rw-r--r--   0 janchristel   (501) staff       (20)       24 2023-08-04 10:27:33.000000 DuHast-0.0.9/MANIFEST.in
+-rw-r--r--   0 janchristel   (501) staff       (20)     1070 2023-08-05 10:26:20.958590 DuHast-0.0.9/PKG-INFO
+-rw-r--r--   0 janchristel   (501) staff       (20)      633 2023-07-12 08:39:01.000000 DuHast-0.0.9/README.md
+-rw-r--r--   0 janchristel   (501) staff       (20)      608 2023-08-05 10:15:57.000000 DuHast-0.0.9/pyproject.toml
+-rw-r--r--   0 janchristel   (501) staff       (20)      388 2023-08-05 10:26:20.959192 DuHast-0.0.9/setup.cfg
+-rw-r--r--   0 janchristel   (501) staff       (20)      439 2023-08-04 10:27:33.000000 DuHast-0.0.9/setup.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.741300 DuHast-0.0.9/src/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.762652 DuHast-0.0.9/src/DuHast.egg-info/
+-rw-r--r--   0 janchristel   (501) staff       (20)     1070 2023-08-05 10:26:20.000000 DuHast-0.0.9/src/DuHast.egg-info/PKG-INFO
+-rw-r--r--   0 janchristel   (501) staff       (20)    20526 2023-08-05 10:26:20.000000 DuHast-0.0.9/src/DuHast.egg-info/SOURCES.txt
+-rw-r--r--   0 janchristel   (501) staff       (20)        1 2023-08-05 10:26:20.000000 DuHast-0.0.9/src/DuHast.egg-info/dependency_links.txt
+-rw-r--r--   0 janchristel   (501) staff       (20)        7 2023-08-05 10:26:20.000000 DuHast-0.0.9/src/DuHast.egg-info/top_level.txt
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.763007 DuHast-0.0.9/src/duHast/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.764175 DuHast-0.0.9/src/duHast/Data/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.765450 DuHast-0.0.9/src/duHast/Data/Objects/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.768766 DuHast-0.0.9/src/duHast/Data/Objects/Properties/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.771602 DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7146 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2144 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3720 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3133 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2820 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3336 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_design_set_option.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4202 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_element_geometry.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3089 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_instance_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3215 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_level.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3072 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_phasing.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2894 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_revit_model.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3215 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_type_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5997 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/data_ceiling.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5419 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Objects/data_room.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.773947 DuHast-0.0.9/src/duHast/Data/Utils/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Utils/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2452 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Utils/data_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2868 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Utils/data_export.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6201 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Utils/data_import.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2732 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/Utils/data_to_file.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10863 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/data_to_shapely.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    22884 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Data/process_ceilings_to_rooms.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.774645 DuHast-0.0.9/src/duHast/Revit/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.782029 DuHast-0.0.9/src/duHast/Revit/Annotation/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.784744 DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1296 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2609 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1278 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7001 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.785830 DuHast-0.0.9/src/duHast/Revit/Annotation/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3693 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3078 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/annotation.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5149 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/arrow_heads.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4369 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/dimensions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3684 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/generic_annotation.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3078 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6455 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7452 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags_modify_properties.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6135 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3979 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/multi_ref_annotation.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12895 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/purge_unused_annotation_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4334 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/spot_dimensions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2879 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/stair_path.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3660 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Annotation/text.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.787479 DuHast-0.0.9/src/duHast/Revit/BIM360/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BIM360/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5104 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BIM360/bim_360.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4372 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BIM360/util_bim_360.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.789092 DuHast-0.0.9/src/duHast/Revit/BuildingPads/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.790102 DuHast-0.0.9/src/duHast/Revit/BuildingPads/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2044 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.791754 DuHast-0.0.9/src/duHast/Revit/BuildingPads/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     3950 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2324 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5676 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/building_pads.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4787 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.794326 DuHast-0.0.9/src/duHast/Revit/Categories/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.796650 DuHast-0.0.9/src/duHast/Revit/Categories/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12624 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Data/category_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10648 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Data/category_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4708 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Data/category_data_purge_unused.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.798258 DuHast-0.0.9/src/duHast/Revit/Categories/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3052 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Reporting/categories_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6769 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Reporting/categories_report_utils.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.800460 DuHast-0.0.9/src/duHast/Revit/Categories/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7330 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12561 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2766 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Utility/category_property_names.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12740 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11225 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/categories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2684 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/categories_model.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5491 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/change_family_category.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13460 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Categories/family_sub_categories.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.802052 DuHast-0.0.9/src/duHast/Revit/Ceilings/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.803059 DuHast-0.0.9/src/duHast/Revit/Ceilings/Export/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Export/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6363 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.804174 DuHast-0.0.9/src/duHast/Revit/Ceilings/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3239 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Geometry/geometry.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.805261 DuHast-0.0.9/src/duHast/Revit/Ceilings/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1221 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.806800 DuHast-0.0.9/src/duHast/Revit/Ceilings/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2330 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3013 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6718 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/ceilings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6184 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.814622 DuHast-0.0.9/src/duHast/Revit/Common/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.816125 DuHast-0.0.9/src/duHast/Revit/Common/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    25657 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Geometry/geometry.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2318 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Geometry/solids.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.816496 DuHast-0.0.9/src/duHast/Revit/Common/Objects/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.820219 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3473 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/colour_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2300 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/line_cut.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4207 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/line_graphic_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2328 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/line_projection.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2353 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/pattern_background.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2353 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/pattern_foreground.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4308 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/pattern_graphic_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3407 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/pattern_settings_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Objects/__init__.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.822237 DuHast-0.0.9/src/duHast/Revit/Common/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2030 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Reporting/groups_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2019 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Reporting/worksets_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2737 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Reporting/worksets_report_utils.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.823468 DuHast-0.0.9/src/duHast/Revit/Common/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2448 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/Utility/revit_to_data_conversion.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15678 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/common.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4951 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/custom_element_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4273 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/custom_element_filter_actions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4548 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/custom_element_filter_tests.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5132 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/delete.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5636 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/design_set_options.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7988 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/element_filtering.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2464 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/element_functions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11442 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/file_io.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8015 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/groups.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    20358 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/parameter_get_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4357 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/parameter_grouping.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9995 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/parameter_set_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2818 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/phases.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8916 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/purge_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)      289 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/revit_version.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3519 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/transaction.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15172 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Common/worksets.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.825185 DuHast-0.0.9/src/duHast/Revit/DetailItems/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.826295 DuHast-0.0.9/src/duHast/Revit/DetailItems/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/DetailItems/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1207 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.827454 DuHast-0.0.9/src/duHast/Revit/DetailItems/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/DetailItems/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2673 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/DetailItems/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6435 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/DetailItems/detail_items.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8656 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.829904 DuHast-0.0.9/src/duHast/Revit/Exports/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.834275 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7953 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8068 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8105 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13561 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13564 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2305 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14053 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/ifc_export_settings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2105 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2831 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/export.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    17682 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/export_ifc.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10789 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Exports/export_navis.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.839040 DuHast-0.0.9/src/duHast/Revit/Family/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.848399 DuHast-0.0.9/src/duHast/Revit/Family/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7889 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15521 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11953 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_missing_families.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4383 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12682 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    16815 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    23829 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_category_data_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10972 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_data_collector.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6755 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7792 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_rename_files.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8666 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_rename_find_host_families.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8083 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_rename_loaded_families.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    19921 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/family_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2346 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/ifamily_action.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4278 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/ifamily_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9216 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Data/ifamily_processor.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.849416 DuHast-0.0.9/src/duHast/Revit/Family/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10439 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/Utility/loadable_family_categories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3782 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_element_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1639 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_functions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1734 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_load_option.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5737 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_parameter_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7608 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_reference_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9406 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_reload.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5993 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_rename_files_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    16256 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/family_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7401 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Family/purge_unused_family_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.851083 DuHast-0.0.9/src/duHast/Revit/Floors/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.851676 DuHast-0.0.9/src/duHast/Revit/Floors/Export/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/Export/__init__.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.852652 DuHast-0.0.9/src/duHast/Revit/Floors/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1213 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/Reporting/floors_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.854420 DuHast-0.0.9/src/duHast/Revit/Floors/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2376 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/Utility/floors_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2993 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/Utility/floors_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6963 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/floors.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5625 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Floors/purge_unused_floor_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.857260 DuHast-0.0.9/src/duHast/Revit/Grids/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.858421 DuHast-0.0.9/src/duHast/Revit/Grids/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2849 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/Reporting/grid_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2059 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/Reporting/grids_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8256 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/grids.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14876 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/grids_appearance.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6624 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/grids_worksets.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3456 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Grids/purge_unused_grid_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.860426 DuHast-0.0.9/src/duHast/Revit/Levels/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.861709 DuHast-0.0.9/src/duHast/Revit/Levels/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Levels/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2021 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Levels/Reporting/levels_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2914 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Levels/Reporting/levels_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Levels/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4732 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Levels/levels.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14798 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Levels/levels_appearance.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4496 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Levels/purge_unused_level_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.864731 DuHast-0.0.9/src/duHast/Revit/LinePattern/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.865119 DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.866126 DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2341 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/Data/fill_pattern_settings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2342 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/Data/line_pattern_settings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2267 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/fill_patterns.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    12827 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/line_pattern_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7537 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/line_pattern_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4312 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10673 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/line_patterns.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3360 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/LinePattern/line_styles.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.869974 DuHast-0.0.9/src/duHast/Revit/Links/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.872933 DuHast-0.0.9/src/duHast/Revit/Links/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2062 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/Reporting/cad_links_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5068 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2121 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/Reporting/links_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5072 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/Reporting/links_report_utils.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.874053 DuHast-0.0.9/src/duHast/Revit/Links/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1562 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/Utility/link_path.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9372 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/cad_links.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3455 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/cad_links_geometry.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5379 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/image_links.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3278 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/link_functions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11463 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/links.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3412 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Links/purge_unused_image_link_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.879543 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.880635 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1976 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.884579 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     2487 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3485 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3814 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3763 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6507 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6366 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/cable_trays.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6278 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/conduits.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6366 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/ducts.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6480 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/flex_ducts.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6149 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/pipes.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11392 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14331 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.885488 DuHast-0.0.9/src/duHast/Revit/Materials/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.887039 DuHast-0.0.9/src/duHast/Revit/Materials/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Materials/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2064 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Materials/Reporting/materials_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3471 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Materials/Reporting/materials_report_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Materials/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3554 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Materials/materials.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.888006 DuHast-0.0.9/src/duHast/Revit/ModelHealth/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.889063 DuHast-0.0.9/src/duHast/Revit/ModelHealth/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/ModelHealth/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5675 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/ModelHealth/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    27455 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/ModelHealth/model_health.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.891206 DuHast-0.0.9/src/duHast/Revit/Purge/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Purge/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3735 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Purge/purge_action.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    25813 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Purge/purge_unused.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7869 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Purge/purge_unused_e_transmit.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.893682 DuHast-0.0.9/src/duHast/Revit/Railings/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.894801 DuHast-0.0.9/src/duHast/Revit/Railings/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2024 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Reporting/railings_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.898241 DuHast-0.0.9/src/duHast/Revit/Railings/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2487 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Utility/merge_lists.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2431 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railing_categories.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2230 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railing_family_names.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4327 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railings_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3773 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railings_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7015 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/balusters.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7825 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8385 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Railings/railings.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.899227 DuHast-0.0.9/src/duHast/Revit/Ramps/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.899805 DuHast-0.0.9/src/duHast/Revit/Ramps/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2013 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.901320 DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     1993 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2356 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3589 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4005 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/purge_unused_ramp_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3588 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Ramps/ramps.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.903083 DuHast-0.0.9/src/duHast/Revit/Revisions/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Revisions/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6698 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Revisions/new_revision.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    18321 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Revisions/revisions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4524 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Revisions/sequence.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.904392 DuHast-0.0.9/src/duHast/Revit/Roofs/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.905254 DuHast-0.0.9/src/duHast/Revit/Roofs/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2013 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.907461 DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)     2121 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3035 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3716 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5651 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/purge_unused_roof_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6312 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Roofs/roofs.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.909270 DuHast-0.0.9/src/duHast/Revit/Rooms/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.910082 DuHast-0.0.9/src/duHast/Revit/Rooms/Export/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/Export/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6045 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/Export/to_data_room.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.910815 DuHast-0.0.9/src/duHast/Revit/Rooms/Geometry/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/Geometry/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5692 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/Geometry/geometry.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.911489 DuHast-0.0.9/src/duHast/Revit/Rooms/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1194 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    11479 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/room_functions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3698 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/room_tags.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4951 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Rooms/rooms.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.914597 DuHast-0.0.9/src/duHast/Revit/SharedParameters/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.915609 DuHast-0.0.9/src/duHast/Revit/SharedParameters/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4832 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2074 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13905 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_add.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5295 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8096 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_swap.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8193 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    10845 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameters.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6667 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameters_delete.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1215 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.918434 DuHast-0.0.9/src/duHast/Revit/Stairs/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.919050 DuHast-0.0.9/src/duHast/Revit/Stairs/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2019 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.919956 DuHast-0.0.9/src/duHast/Revit/Stairs/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2448 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/Utility/stairs_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3604 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2210 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/cut_marks.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2223 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/landings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2574 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/path.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15680 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/purge_unused_stair_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2170 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/runs.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5819 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/stairs.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2539 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Stairs/stringers_carriages.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.925322 DuHast-0.0.9/src/duHast/Revit/Views/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.926291 DuHast-0.0.9/src/duHast/Revit/Views/Objects/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.929148 DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4630 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_by_base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2431 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_by_category.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2979 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_by_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4345 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_cut.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4546 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_projection.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3516 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Objects/view_graphics_settings.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.932917 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7426 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/schedules_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6825 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/sheets_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3141 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/view_property_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2541 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/view_property_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4673 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/views_data_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7502 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/views_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4724 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Reporting/views_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.934396 DuHast-0.0.9/src/duHast/Revit/Views/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15556 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Utility/data_view.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1527 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/Utility/view_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9094 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/delete.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5923 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/filters.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    15057 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/referencing.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3619 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/schedules.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2728 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/sheet_functions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5901 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/sheets.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7016 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/templates.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6545 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/views.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8145 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/views_purge_unused.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4849 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Views/visibility_graphics_utils.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.938283 DuHast-0.0.9/src/duHast/Revit/Walls/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.939900 DuHast-0.0.9/src/duHast/Revit/Walls/Reporting/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/Reporting/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3909 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/Reporting/walls_report.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1299 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/Reporting/walls_report_header.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.941465 DuHast-0.0.9/src/duHast/Revit/Walls/Utility/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/Utility/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2052 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/Utility/walls_filter.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2967 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/Utility/walls_type_sorting.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9609 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/curtain_wall_elements.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3207 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/curtain_walls.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5681 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7760 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/purge_unused_wall_types.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2912 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/stacked_walls.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     1804 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/wall_functions.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6331 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Walls/walls.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.943819 DuHast-0.0.9/src/duHast/Revit/Warnings/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.945171 DuHast-0.0.9/src/duHast/Revit/Warnings/Data/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/Data/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4861 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/Data/warnings_data.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3725 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/Data/warnings_data_processor.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5498 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/solver.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5490 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/solver_duplicate_mark.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3641 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/solver_room_tag_to_room.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2413 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/Warnings/warnings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Revit/__init__.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.948313 DuHast-0.0.9/src/duHast/UI/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3001 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/file_item.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9641 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/file_list.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3240 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/file_select_settings.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    13347 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/script.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4907 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/ui_file_select.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3282 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/workload_bucket.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4349 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/UI/workloader.py
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.955962 DuHast-0.0.9/src/duHast/Utilities/
+drwxr-xr-x   0 janchristel   (501) staff       (20)        0 2023-08-05 10:26:20.957952 DuHast-0.0.9/src/duHast/Utilities/Objects/
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/Objects/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3796 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/Objects/base.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4896 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/Objects/result.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3669 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/Objects/timer.py
+-rw-r--r--   0 janchristel   (501) staff       (20)        0 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/__init__.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    29998 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/batch_processor_log_utils.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2628 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/benchmarking.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3500 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/compare.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4916 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/console_out.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     4818 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/date_stamps.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5343 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/directory_io.py
+-rw-r--r--   0 janchristel   (501) staff       (20)    14414 2023-08-05 01:57:26.000000 DuHast-0.0.9/src/duHast/Utilities/files_combine.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5425 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/files_csv.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8431 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/files_get.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8550 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/files_io.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3813 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/files_json.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5061 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/files_tab.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     5053 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/padding.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     8755 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/solibri_ifc_optimizer.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     7525 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/system_process.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     2665 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/unit_conversion.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     3773 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/util_batch_p.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     6651 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/utility.py
+-rw-r--r--   0 janchristel   (501) staff       (20)     9172 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/Utilities/worksharing_monitor_process.py
+-rw-r--r--   0 janchristel   (501) staff       (20)      246 2023-08-04 10:28:29.000000 DuHast-0.0.9/src/duHast/__init__.py
```

### Comparing `DuHast-0.0.8/pyproject.toml` & `DuHast-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 requires = ["setuptools==43.0.0", "wheel==0.33.6"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
 Homepage = "https://github.com/jchristel/SampleCodeRevitBatchProcessor"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"../docsource/source/conf.py" = ['release = "{version}"']
+"pyproject.toml" = ['current_version = "{version}"']
+"docsource/conf.py" = ['release = "{version}"']
 "setup.cfg" = ['version = {version}']
```

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_design_set_option.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_design_set_option.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_element_geometry.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_element_geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_instance_properties.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_instance_properties.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_level.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_level.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_phasing.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_phasing.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_revit_model.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_revit_model.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/Properties/data_type_properties.py` & `DuHast-0.0.9/src/duHast/Data/Objects/Properties/data_type_properties.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/data_ceiling.py` & `DuHast-0.0.9/src/duHast/Data/Objects/data_ceiling.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Objects/data_room.py` & `DuHast-0.0.9/src/duHast/Data/Objects/data_room.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Utils/data_base.py` & `DuHast-0.0.9/src/duHast/Data/Utils/data_base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Utils/data_export.py` & `DuHast-0.0.9/src/duHast/Data/Utils/data_export.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Utils/data_import.py` & `DuHast-0.0.9/src/duHast/Data/Utils/data_import.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/Utils/data_to_file.py` & `DuHast-0.0.9/src/duHast/Data/Utils/data_to_file.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/data_to_shapely.py` & `DuHast-0.0.9/src/duHast/Data/data_to_shapely.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Data/process_ceilings_to_rooms.py` & `DuHast-0.0.9/src/duHast/Data/process_ceilings_to_rooms.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     :rtype: list of list of str
     """
 
     data = []
     revit_version = get_revit_version_number(doc)
     tag_instances = get_all_independent_tags(doc)
     for tag_instance in tag_instances:
-        row = []
+        row = {}
         try:
             if custom_element_filter != None:
                 if custom_element_filter.check_element(doc, tag_instance.Id):
                     # this can throw an exception...wrap in try catch
                     tag_text = "<empty>"
                     try:
                         tag_text = tag_instance.TagText
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/annotation.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/arrow_heads.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/arrow_heads.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/dimensions.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/dimensions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/generic_annotation.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/generic_annotation.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_modify_properties.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags_modify_properties.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/multi_ref_annotation.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/multi_ref_annotation.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/purge_unused_annotation_types.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/purge_unused_annotation_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/spot_dimensions.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/spot_dimensions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/stair_path.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/stair_path.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Annotation/text.py` & `DuHast-0.0.9/src/duHast/Revit/Annotation/text.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/BIM360/bim_360.py` & `DuHast-0.0.9/src/duHast/Revit/BIM360/bim_360.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/BIM360/util_bim_360.py` & `DuHast-0.0.9/src/duHast/Revit/BIM360/util_bim_360.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py` & `DuHast-0.0.9/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py` & `DuHast-0.0.9/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/BuildingPads/building_pads.py` & `DuHast-0.0.9/src/duHast/Revit/BuildingPads/building_pads.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py` & `DuHast-0.0.9/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Data/category_data.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_processor.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Data/category_data_processor.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Data/category_data_purge_unused.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Data/category_data_purge_unused.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Reporting/categories_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Reporting/categories_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Reporting/categories_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/category_property_names.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Utility/category_property_names.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/categories.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/categories.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 
 
 import clr
 import System
 from System.Collections.Generic import List
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Categories/family_sub_categories.py` & `DuHast-0.0.9/src/duHast/Revit/Categories/family_sub_categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py` & `DuHast-0.0.9/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ceilings/Geometry/geometry.py` & `DuHast-0.0.9/src/duHast/Revit/Ceilings/Geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py` & `DuHast-0.0.9/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py` & `DuHast-0.0.9/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ceilings/ceilings.py` & `DuHast-0.0.9/src/duHast/Revit/Ceilings/ceilings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py` & `DuHast-0.0.9/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Geometry/geometry.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Geometry/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,57 @@
     """
 
     returnValue = ""
     for p in edge.Tessellate():
         returnValue = returnValue + "\n" + get_point_as_string(p)
     return returnValue
 
+def UV_pt_list_from_crv_list(curve_list):
+    """ 
+    Returns a list of UV points from a list of curves
+    :param curve_list: A list of curves
+    :param type: list
+    :return: A list of UV points
+    :rtype: list
+    """
+    pt_list = []
+
+    for crv in curve_list:
+        st_pt = crv.GetEndPoint(0)
+        pt_list.append((st_pt.X, st_pt.Y))
+
+    return pt_list
+
+def point_in_polygon(point, polygon):
+    """
+    Returns True if a point is inside a polygon, and False if it is not
+    :param point: The point to check
+    :type point: list, tuple, or set
+    :param polygon: The polygon to check
+    :type polygon: list, tuple, or set
+    :return: True if the point is inside the polygon, False if it is not
+    :rtype: bool
+    """
+
+    num_of_polygon_sides = len(polygon)
+    is_inside = False
+
+    pt_1_x, pt_1_y = polygon[0]
+    for i in range(num_of_polygon_sides+1):
+        pt_2_x, pt_2_y = polygon[i % num_of_polygon_sides]
+        if point[1] > min(pt_1_y, pt_2_y):
+            if point[1] <= max(pt_1_y, pt_2_y):
+                if point[0] <= max(pt_1_x, pt_2_x):
+                    if pt_1_y != pt_2_y:
+                        x_intersection = (point[1] - pt_1_y) * (pt_2_x - pt_1_x) / (pt_2_y - pt_1_y) + pt_1_x
+                    if pt_1_x == pt_2_x or point[0] <= x_intersection:
+                        is_inside = not is_inside
+        pt_1_x, pt_1_y = pt_2_x, pt_2_y
+
+    return is_inside
 
 # ---------------------------- math utility ----------------------------
 
 
 def is_close(a, b, rel_tol=1e-09, abs_tol=0.0):
     """
     Compares two floats with a tolerance. Returns True if they are close enough, otherwise False
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Geometry/solids.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Geometry/solids.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Objects/colour_base.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/ifamily_action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-A base class used to store colour values.
+Interface for family data storage / processing class.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-
-Stores colour values as rgb.
-
 """
 
-
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -28,55 +23,29 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-import json
-
 from duHast.Utilities.Objects import base
 
-class ColourBase(base.Base):
-    data_type = "colour"
-    
-    def __init__(self,j={},**kwargs):
-        """
-        Class constructor.
-
-        """
-
-        super(ColourBase, self).__init__(**kwargs)
-
-        # check if any data was past in with constructor!
-        if j != None and len(j) > 0:
-            # check type of data that came in:
-            if type(j) == str:
-                # a string
-                j = json.loads(j)
-            elif type(j) == dict:
-                # no action required
-                pass
-            else:
-                raise ValueError(
-                    "Argument supplied must be of type string or type dictionary"
-                )
-            
-            # load overrides
-            if "red" in j:
-                self.red = j["red"]
-            else:
-                self.red = 0
-            
-            if "green" in j:
-                self.green = j["green"]
-            else:
-                self.green = 0
-            
-            if "blue" in j:
-                self.blue = j["blue"]
-            else:
-                self.blue = 0
+
+class IFamilyAction(base.Base):
+    def __init__(self, action_type, **kwargs):
+
+        # forwards all unused arguments
+        # ini super class to allow multi inheritance in children!
+        super(IFamilyAction, self).__init__(**kwargs)
+
+        self.data = []
+
+        if action_type != None:
+            self.data_type = action_type
         else:
-            self.red = 0
-            self.green = 0 
-            self.blue = 0
+            self.data_type = "not declared"
+
+    def process(self, doc):
+        pass
+
+    def get_data(self):
+        pass
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_cut.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/line_cut.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,31 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
-from duHast.Revit.Common.Objects.line_graphic_base import LineGraphicBase
+from duHast.Revit.Common.Objects.Data.line_graphic_base import LineGraphicBase
+
 
 class LineCut(LineGraphicBase):
     data_type = "line_cut"
 
     def __init__(self, j={}):
         """
         Class constructor.
 
         :param j: A json formatted dictionary of this class, defaults to {}
         :type j: dict, optional
         """
 
         # store data type  in base class
-        super(LineCut, self).__init__(j=j)
+        super(LineCut, self).__init__(data_type=self.data_type, j=j)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Objects/line_projection.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/line_projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,30 +21,31 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
-from duHast.Revit.Common.Objects.line_graphic_base import LineGraphicBase
+from duHast.Revit.Common.Objects.Data.line_graphic_base import LineGraphicBase
+
 
 class LineProjection(LineGraphicBase):
     data_type = "line_projection"
 
     def __init__(self, j={}):
         """
         Class constructor.
 
         :param j: A json formatted dictionary of this class, defaults to {}
         :type j: dict, optional
         """
 
         # store data type  in base class
-        super(LineProjection, self).__init__(j=j)
+        super(LineProjection, self).__init__(data_type=self.data_type, j=j)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_background.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/pattern_foreground.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 A base class used to store pattern category overrides.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
-Stores overrides of background patterns.
+Stores overrides of foreground patterns.
 
 """
 
 
 #
 # License:
 #
@@ -29,22 +29,22 @@
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
-from duHast.Revit.Common.Objects.pattern_graphic_base import PatternGraphicBase
+from duHast.Revit.Common.Objects.Data.pattern_graphic_base import PatternGraphicBase
 
-class PatternBackground(PatternGraphicBase):
-    data_type = "pattern_background"
+class PatternForeground(PatternGraphicBase):
+    data_type = "pattern_foreground"
 
     def __init__(self, j={}):
         """
         Class constructor.
 
         :param j: A json formatted dictionary of this class, defaults to {}
         :type j: dict, optional
         """
 
         # store data type  in base class
-        super(PatternBackground, self).__init__(j=j)
+        super(PatternForeground, self).__init__(data_type=self.data_type, j=j)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_foreground.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/Data/fill_pattern_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 A base class used to store pattern category overrides.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
-Stores overrides of foreground patterns.
+Stores line patterns.
 
 """
 
 
 #
 # License:
 #
@@ -29,22 +29,22 @@
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
-from duHast.Revit.Common.Objects.pattern_graphic_base import PatternGraphicBase
+from duHast.Revit.Common.Objects.Data.pattern_settings_base import PatternSettingBase
 
-class PatternForeground(PatternGraphicBase):
-    data_type = "pattern_foreground"
+class FillPatternSettings(PatternSettingBase):
+    data_type = "fill_pattern_setting"
 
     def __init__(self, j={}):
         """
         Class constructor.
 
         :param j: A json formatted dictionary of this class, defaults to {}
         :type j: dict, optional
         """
 
         # store data type  in base class
-        super(PatternForeground, self).__init__(j=j)
+        super(FillPatternSettings, self).__init__(data_type=self.data_type, j=j)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Objects/pattern_graphic_base.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_by_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-A base class used to store pattern graphic settings.
+A base class used to store category overrides.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
-Stores pattern graphic settings:
-
-- colour
-- pattern_id
-- is_visible
+Stores common overrides between categories and filters
 
 """
 
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -24,67 +21,52 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
-
 import json
 
-from duHast.Utilities.Objects import base
-from duHast.Revit.Common.Objects.colour_base import ColourBase
+from duHast.Revit.Views.Objects.Data.override_by_base import OverrideByBase
+
+
+class OverrideByFilter(OverrideByBase):
+    data_type = "override_by_filter"
 
-class PatternGraphicBase(base.Base):
-    def __init__(self,j={},**kwargs):
+    def __init__(self, filter_name="", filter_id=-1, j={}):
         """
         Class constructor.
 
         """
 
-        super(PatternGraphicBase, self).__init__(**kwargs)
+        super(OverrideByFilter, self).__init__(data_type=self.data_type, j=j)
+
+        self.filter_name = filter_name
+        self.filter_id = filter_id
 
         # check if any data was past in with constructor!
         if j != None and len(j) > 0:
             # check type of data that came in:
             if type(j) == str:
                 # a string
                 j = json.loads(j)
             elif type(j) == dict:
                 # no action required
                 pass
             else:
                 raise ValueError(
                     "Argument supplied must be of type string or type dictionary"
                 )
-            
-            # load overrides
-            
-            if ColourBase.data_type in j:
-                self.colour = ColourBase(
-                        j[ColourBase.data_type]
-                    )
-            else:
-                self.colour = ColourBase()
-                
-            if "is_visible" in j:
-                self.is_visible = j["is_visible"]
-            else:
-                self.is_visible = True
-            
-            if "pattern_id" in j:
-                self.pattern_id = j["pattern_id"]
+
+            if "is_enabled" in j:
+                self.is_enabled = j["is_enabled"]
             else:
-                self.pattern_id = -1
+                self.is_enabled = True
         else:
-            # set default values
-            self.colour = ColourBase()
-            self.pattern_id = -1
-            self.is_visible = True
-
-        
+            self.is_enabled = True
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Reporting/groups_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Reporting/groups_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Reporting/worksets_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/Reporting/worksets_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Reporting/worksets_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/common.py` & `DuHast-0.0.9/src/duHast/Revit/Common/common.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter.py` & `DuHast-0.0.9/src/duHast/Revit/Common/custom_element_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_actions.py` & `DuHast-0.0.9/src/duHast/Revit/Common/custom_element_filter_actions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/custom_element_filter_tests.py` & `DuHast-0.0.9/src/duHast/Revit/Common/custom_element_filter_tests.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/delete.py` & `DuHast-0.0.9/src/duHast/Revit/Common/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-import Autodesk.Revit.DB as rdb
+
+from Autodesk.Revit.DB import Element, ElementId, Transaction
 
 from duHast.Revit.Common import transaction as rTran
 from duHast.Utilities.Objects import result as res
 
 # required for .ToList()
 import clr
 
@@ -64,23 +65,23 @@
     """
 
     return_value = res.Result()
 
     def action():
         action_return_value = res.Result()
         try:
-            doc.Delete(ids.ToList[rdb.ElementId]())
+            doc.Delete(ids.ToList[ElementId]())
             action_return_value.message = "Deleted {} {}".format(len(ids), element_name)
         except Exception as e:
             action_return_value.update_sep(
                 False, "Failed to delete {} with exception: {}".format(element_name, e)
             )
         return action_return_value
 
-    transaction = rdb.Transaction(doc, transaction_name)
+    transaction = Transaction(doc, transaction_name)
     return_value = rTran.in_transaction(transaction, action)
     return return_value
 
 
 def delete_by_element_ids_one_by_one(
     doc,
     ids,
@@ -107,21 +108,21 @@
 
     return_value = res.Result()
     for id in ids:
 
         def action():
             action_return_value = res.Result()
             element = doc.GetElement(id)
-            n = rdb.Element.Name.GetValue(element)
+            n = Element.Name.GetValue(element)
             try:
                 doc.Delete(id)
                 action_return_value.message = "Deleted [{}] {}".format(id, n)
             except Exception as e:
                 action_return_value.update_sep(
                     False,
                     "Failed to delete {} [{}] with exception: {}".format(n, id, e),
                 )
             return action_return_value
 
-        transaction = rdb.Transaction(doc, transaction_name)
+        transaction = Transaction(doc, transaction_name)
         return_value.update(rTran.in_transaction(transaction, action))
     return return_value
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/design_set_options.py` & `DuHast-0.0.9/src/duHast/Revit/Common/design_set_options.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/element_filtering.py` & `DuHast-0.0.9/src/duHast/Revit/Common/element_filtering.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/file_io.py` & `DuHast-0.0.9/src/duHast/Revit/Common/file_io.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/groups.py` & `DuHast-0.0.9/src/duHast/Revit/Common/groups.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/parameter_get_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Common/parameter_get_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 clr.AddReference("System.Core")
 from System import Linq
 
 clr.ImportExtensions(Linq)
 
 # import everything from Autodesk Revit DataBase namespace (Revit API)
+from Autodesk.Revit.DB import ElementId #, ParameterType, StorageType
 import Autodesk.Revit.DB as rdb
 
 # utilities
 from duHast.Utilities import utility as util
 from duHast.Utilities import unit_conversion as unitConversion
 
 # type checker
@@ -456,15 +457,15 @@
     :return:
         Default value is -1 if parameter value is empty or storage type is not integer.
         Otherwise the actual parameter value.
     :rtype: int
     """
 
     # set return value default
-    parameter_value = rdb.ElementId.InvalidElementId
+    parameter_value = ElementId.InvalidElementId
 
     value_getter = {rdb.StorageType.ElementId: getter_element_id_as_element_id}
 
     # check if element id...otherwise return the default value
     if para.StorageType == rdb.StorageType.ElementId:
         parameter_value = get_parameter_value_with_over_load(para, value_getter)
     return parameter_value
@@ -552,7 +553,24 @@
     parameter_value = None
     paras = element.GetOrderedParameters()
     for para in paras:
         if para.Definition.Name == parameter_name:
             parameter_value = parameter_value_getter(para)
             break
     return parameter_value
+
+def param_is_empty_or_null(param):
+	""" 
+	Checks if a parameter is empty or null
+	:param param: The parameter to check
+	:type param: Parameter
+	:return: True if the parameter is empty or null, False if it is not
+	:rtype: bool
+	"""
+
+	if param == None:
+		return True
+	else:
+		if param.AsString() == '' or param.AsString() == None:
+			return True
+		else:
+			return False
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/parameter_grouping.py` & `DuHast-0.0.9/src/duHast/Revit/Common/parameter_grouping.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/parameter_set_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Common/parameter_set_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/phases.py` & `DuHast-0.0.9/src/duHast/Revit/Common/phases.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,7 +64,25 @@
     phases = get_all_phases(doc)
     if len(phases) > 0:
         if phase_id in phases:
             return_value = phases[phase_id]
         else:
             return_value = "Invalid phase id."
     return return_value
+
+def get_name_to_phase_dict(rvt_doc):
+    '''
+    Returns a dictionary where key is the name and value is the phase.
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    
+    :return: A dictionary where key is the name and value is the phase. Dictionary will be empty if no phases exist (family doc?)
+    :rtype: dic{key str: value Autodesk.Revit.DB.Phase}
+    '''
+    phases = rvt_doc.Phases
+    phase_dict = {}
+
+    for phase in phases:
+        phase_dict[phase.Name] = phase
+    
+    return phase_dict
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/purge_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Common/purge_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/transaction.py` & `DuHast-0.0.9/src/duHast/Revit/Common/transaction.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Common/worksets.py` & `DuHast-0.0.9/src/duHast/Revit/Common/worksets.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py` & `DuHast-0.0.9/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/DetailItems/detail_items.py` & `DuHast-0.0.9/src/duHast/Revit/DetailItems/detail_items.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py` & `DuHast-0.0.9/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_settings.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/ifc_export_settings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/export.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/export.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/export_ifc.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/export_ifc.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Exports/export_navis.py` & `DuHast-0.0.9/src/duHast/Revit/Exports/export_navis.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_missing_families.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_missing_families.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_processor.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_processor.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_base_data_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_base_data_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_category_data_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_category_data_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_data_collector.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_data_collector.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_files.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_rename_files.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_find_host_families.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_rename_find_host_families.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_rename_loaded_families.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_rename_loaded_families.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/family_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/family_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_action.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railing_categories.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Interface for family data storage / processing class.
+Revit railings built-in categories. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-"""
 
+- useful for filtering out families which can be used in MEP system types
+
+"""
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -23,29 +25,23 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Utilities.Objects import base
-
-
-class IFamilyAction(base.Base):
-    def __init__(self, action_type, **kwargs):
-
-        # forwards all unused arguments
-        # ini super class to allow multi inheritance in children!
-        super(IFamilyAction, self).__init__(**kwargs)
-
-        self.data = []
-
-        if action_type != None:
-            self.data_type = action_type
-        else:
-            self.data_type = "not declared"
-
-    def process(self, doc):
-        pass
-
-    def get_data(self):
-        pass
+#: category filter for all railing element filters by category
+import Autodesk.Revit.DB as rdb
+from System.Collections.Generic import List
+
+
+RAILING_CATEGORY_FILTER = List[rdb.BuiltInCategory](
+    [
+        rdb.BuiltInCategory.OST_Railings,
+        rdb.BuiltInCategory.OST_RailingBalusterRail,
+        rdb.BuiltInCategory.OST_RailingHandRail,
+        rdb.BuiltInCategory.OST_RailingSupport,
+        rdb.BuiltInCategory.OST_RailingSystem,
+        rdb.BuiltInCategory.OST_RailingTermination,
+        rdb.BuiltInCategory.OST_RailingTopRail,
+    ]
+)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_data.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/ifamily_data.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Data/ifamily_processor.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Data/ifamily_processor.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/Utility/loadable_family_categories.py` & `DuHast-0.0.9/src/duHast/Revit/Family/Utility/loadable_family_categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/family_element_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/family_element_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/family_load_option.py` & `DuHast-0.0.9/src/duHast/Revit/Family/family_load_option.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/family_parameter_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/family_parameter_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/family_reference_elements.py` & `DuHast-0.0.9/src/duHast/Revit/Family/family_reference_elements.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/family_reload.py` & `DuHast-0.0.9/src/duHast/Revit/Family/family_reload.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/family_rename_files_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/family_rename_files_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/family_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Family/family_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Family/purge_unused_family_types.py` & `DuHast-0.0.9/src/duHast/Revit/Family/purge_unused_family_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Floors/Reporting/floors_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Floors/Reporting/floors_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_filter.py` & `DuHast-0.0.9/src/duHast/Revit/Floors/Utility/floors_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Floors/Utility/floors_type_sorting.py` & `DuHast-0.0.9/src/duHast/Revit/Floors/Utility/floors_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Floors/floors.py` & `DuHast-0.0.9/src/duHast/Revit/Floors/floors.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Floors/purge_unused_floor_types.py` & `DuHast-0.0.9/src/duHast/Revit/Floors/purge_unused_floor_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grid_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Grids/Reporting/grid_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Grids/Reporting/grids_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Grids/Reporting/grids_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Grids/grids.py` & `DuHast-0.0.9/src/duHast/Revit/Grids/grids.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Grids/grids_appearance.py` & `DuHast-0.0.9/src/duHast/Revit/Grids/grids_appearance.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Grids/grids_worksets.py` & `DuHast-0.0.9/src/duHast/Revit/Grids/grids_worksets.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Grids/purge_unused_grid_types.py` & `DuHast-0.0.9/src/duHast/Revit/Grids/purge_unused_grid_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Levels/Reporting/levels_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Levels/Reporting/levels_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Levels/Reporting/levels_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Levels/levels.py` & `DuHast-0.0.9/src/duHast/Revit/Levels/levels.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Levels/levels_appearance.py` & `DuHast-0.0.9/src/duHast/Revit/Levels/levels_appearance.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Levels/purge_unused_level_types.py` & `DuHast-0.0.9/src/duHast/Revit/Levels/purge_unused_level_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/LinePattern/fill_patterns.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/fill_patterns.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 #
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
-import Autodesk.Revit.DB as rdb
 
+from Autodesk.Revit.DB import FilteredElementCollector, FillPatternElement
 
 def get_all_fill_pattern(doc):
     """
     Gets all fill pattern elements in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of all fill pattern elements.
-    :rtype: list of Autodesk.Revit.DB.FillPatternElement
+    :return: A filtered element collector of all fill pattern elements.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return rdb.FilteredElementCollector(doc).OfClass(rdb.FillPatternElement).ToList()
+    return FilteredElementCollector(doc).OfClass(FillPatternElement)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/line_pattern_data.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_processor.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/line_pattern_data_processor.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_patterns.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/line_patterns.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import clr
 
@@ -36,15 +36,22 @@
 
 # import common library modules
 from duHast.Revit.Common import delete as rDel, parameter_get_utils as rParaGet
 from duHast.Utilities.Objects import result as res
 
 
 # import Autodesk
-import Autodesk.Revit.DB as rdb
+from Autodesk.Revit.DB import (
+    BuiltInParameter,
+    Element,
+    ElementId,
+    GraphicsStyleType,
+    LinePatternElement,
+    FilteredElementCollector,
+)
 
 # -------------------------------------------------PATTERN PROPERTIES ------------
 
 #: pattern name
 PROPERTY_PATTERN_NAME = "PatternName"
 #: pattern name default value, hard coded solid line pattern name
 PROPERTY_PATTERN_NAME_VALUE_DEFAULT = "Solid"
@@ -65,28 +72,28 @@
     :return: A dictionary.
     :rtype: dictionary {str: str, str: Autodesk.Revit.DB.ElementId}
     """
 
     dic_pattern = {}
     dic_pattern[PROPERTY_PATTERN_NAME] = PROPERTY_PATTERN_NAME_VALUE_DEFAULT
     dic_pattern[PROPERTY_PATTERN_ID] = pattern_id = cat.GetLinePatternId(
-        rdb.GraphicsStyleType.Projection
+        GraphicsStyleType.Projection
     )
     """check for 'solid' pattern which apparently is not a pattern at all
     *The RevitAPI.chm documents says: Note that Solid is special. It isn't a line pattern at all -- 
     * it is a special code that tells drawing and export code to use solid lines rather than patterned lines. 
     * Solid is visible to the user when selecting line patterns. 
     """
-    if pattern_id != rdb.LinePatternElement.GetSolidPatternId():
+    if pattern_id != LinePatternElement.GetSolidPatternId():
         # not a solid line pattern
-        collector = rdb.FilteredElementCollector(doc).OfClass(rdb.LinePatternElement)
+        collector = FilteredElementCollector(doc).OfClass(LinePatternElement)
         line_pattern_element = None
         for c in collector:
             if pattern_id == c.Id:
-                dic_pattern[PROPERTY_PATTERN_NAME] = rdb.Element.Name.GetValue(c)
+                dic_pattern[PROPERTY_PATTERN_NAME] = Element.Name.GetValue(c)
     return dic_pattern
 
 
 def get_line_pattern_from_level_element(doc, level):
     """
     Returns the line pattern properties as a dictionary\
          where keys are pattern name and pattern id.
@@ -98,23 +105,23 @@
 
     :return: A dictionary.
     :rtype: dictionary {str: str, str: Autodesk.Revit.DB.ElementId}
     """
 
     dic_pattern = {}
     dic_pattern[PROPERTY_PATTERN_NAME] = PROPERTY_PATTERN_NAME_VALUE_DEFAULT
-    dic_pattern[PROPERTY_PATTERN_ID] = rdb.ElementId.InvalidElementId
+    dic_pattern[PROPERTY_PATTERN_ID] = ElementId.InvalidElementId
     try:
         l_type_id = level.GetTypeId()
         level_type = doc.GetElement(l_type_id)
         line_pattern_id_string = rParaGet.get_built_in_parameter_value(
-            level_type, rdb.BuiltInParameter.LINE_PATTERN
+            level_type, BuiltInParameter.LINE_PATTERN
         )
-        dic_pattern[PROPERTY_PATTERN_ID] = rdb.ElementId(int(line_pattern_id_string))
-        dic_pattern[PROPERTY_PATTERN_NAME] = rdb.Element.Name.GetValue(level_type)
+        dic_pattern[PROPERTY_PATTERN_ID] = ElementId(int(line_pattern_id_string))
+        dic_pattern[PROPERTY_PATTERN_NAME] = Element.Name.GetValue(level_type)
     except Exception as ex:
         dic_pattern[PROPERTY_PATTERN_NAME] = str(ex)
     return dic_pattern
 
 
 # ------------------------------------------------ DELETE LINE PATTERNS ----------------------------------------------
 
@@ -133,23 +140,23 @@
 
         - .result = True if line pattern where deleted successfully. Otherwise False.
         - .message will contain delete status per pattern.
 
     :rtype: :class:`.Result`
     """
 
-    lps = rdb.FilteredElementCollector(doc).OfClass(rdb.LinePatternElement).ToList()
+    lps = FilteredElementCollector(doc).OfClass(LinePatternElement).ToList()
     ids = list(
         lp.Id for lp in lps if lp.GetLinePattern().Name.Contains(contains)
-    ).ToList[rdb.ElementId]()
+    ).ToList[ElementId]()
     result = rDel.delete_by_element_ids(
         doc,
         ids,
-        "Deleting line patterns where name contains: " + str(contains),
-        "line patterns containing: " + str(contains),
+        "Deleting line patterns where name contains: {}".format(contains),
+        "line patterns containing: {}".format(contains),
     )
     return result
 
 
 def delete_line_pattern_starts_with(doc, starts_with):
     """
     Deletes all line patterns where the name starts with provided string.
@@ -164,18 +171,18 @@
 
         - .result = True if line pattern where deleted successfully. Otherwise False.
         - .message will contain delete status per pattern.
 
     :rtype: :class:`.Result`
     """
 
-    lps = rdb.FilteredElementCollector(doc).OfClass(rdb.LinePatternElement).ToList()
+    lps = FilteredElementCollector(doc).OfClass(LinePatternElement).ToList()
     ids = list(
         lp.Id for lp in lps if lp.GetLinePattern().Name.StartsWith(starts_with)
-    ).ToList[rdb.ElementId]()
+    ).ToList[ElementId]()
     result = rDel.delete_by_element_ids(
         doc,
         ids,
         "Delete line patterns where name starts with: " + str(starts_with),
         "line patterns starting with: " + str(starts_with),
     )
     return result
@@ -195,19 +202,19 @@
 
         - .result = True if line pattern where deleted successfully. Otherwise False.
         - .message will contain delete status per pattern.
 
     :rtype: :class:`.Result`
     """
 
-    lps = rdb.FilteredElementCollector(doc).OfClass(rdb.LinePatternElement).ToList()
-    ids = list(lp.Id for lp in lps).ToList[rdb.ElementId]()
+    lps = FilteredElementCollector(doc).OfClass(LinePatternElement).ToList()
+    ids = list(lp.Id for lp in lps).ToList[ElementId]()
     ids_contain = list(
         lp.Id for lp in lps if lp.GetLinePattern().Name.Contains(contains)
-    ).ToList[rdb.ElementId]()
+    ).ToList[ElementId]()
     delete_ids = list(set(ids) - set(ids_contain))
     result = rDel.delete_by_element_ids(
         doc,
         delete_ids,
         "Delete line patterns where name does not contain: " + str(contains),
         "line patterns without: " + str(contains),
     )
@@ -217,33 +224,33 @@
 def get_all_line_patterns(doc):
     """
     Gets all line patterns in the model.
 
     :param doc: _description_
     :type doc: _type_
 
-    :return: List of all line pattern elements in model.
-    :rtype: list of Autodesk.Revit.DB.LinePatternElement
+    :return: filtered element collector of all line pattern elements in model.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
-    return rdb.FilteredElementCollector(doc).OfClass(rdb.LinePatternElement).ToList()
+    return FilteredElementCollector(doc).OfClass(LinePatternElement)
 
 
 def build_patterns_dictionary_by_name(doc):
     """
     Returns a dictionary where line pattern name is key, values are all ids of line patterns with the exact same name.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
     :return: A dictionary where line pattern name is key, values are all ids of line patterns with the exact same name
     :rtype: dictionary(key str, value list of Autodesk.Revit.DB.ElementId)
     """
 
     lp_dic = {}
-    lps = rdb.FilteredElementCollector(doc).OfClass(rdb.LinePatternElement)
+    lps = FilteredElementCollector(doc).OfClass(LinePatternElement)
     for lp in lps:
         if lp_dic.has_key(lp.GetLinePattern().Name):
             lp_dic[lp.GetLinePattern().Name].append(lp.Id)
         else:
             lp_dic[lp.GetLinePattern().Name] = [lp.Id]
     return lp_dic
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/LinePattern/line_styles.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/line_styles.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Links/Reporting/cad_links_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Links/Reporting/links_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/Reporting/links_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Links/Reporting/links_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/Utility/link_path.py` & `DuHast-0.0.9/src/duHast/Revit/Links/Utility/link_path.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/cad_links.py` & `DuHast-0.0.9/src/duHast/Revit/Links/cad_links.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/cad_links_geometry.py` & `DuHast-0.0.9/src/duHast/Revit/Links/cad_links_geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/image_links.py` & `DuHast-0.0.9/src/duHast/Revit/Links/image_links.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/links.py` & `DuHast-0.0.9/src/duHast/Revit/Links/links.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Links/purge_unused_image_link_types.py` & `DuHast-0.0.9/src/duHast/Revit/Links/purge_unused_image_link_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/cable_trays.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/cable_trays.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/conduits.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/conduits.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/ducts.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/ducts.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/flex_ducts.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/flex_ducts.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/pipes.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/pipes.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py` & `DuHast-0.0.9/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Materials/Reporting/materials_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Materials/Reporting/materials_report_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Materials/Reporting/materials_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Materials/materials.py` & `DuHast-0.0.9/src/duHast/Revit/Materials/materials.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py` & `DuHast-0.0.9/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/ModelHealth/model_health.py` & `DuHast-0.0.9/src/duHast/Revit/ModelHealth/model_health.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Purge/purge_action.py` & `DuHast-0.0.9/src/duHast/Revit/Purge/purge_action.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused.py` & `DuHast-0.0.9/src/duHast/Revit/Purge/purge_unused.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Purge/purge_unused_e_transmit.py` & `DuHast-0.0.9/src/duHast/Revit/Purge/purge_unused_e_transmit.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/Reporting/railings_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/Reporting/railings_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/merge_lists.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/Utility/merge_lists.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_categories.py` & `DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Revit railings built-in categories. 
+This module contains a Revit roofs utility functions. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-- useful for filtering out families which can be used in MEP system types
-
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
@@ -25,23 +22,52 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-#: category filter for all railing element filters by category
+# import Autodesk
 import Autodesk.Revit.DB as rdb
-from System.Collections.Generic import List
 
 
-RAILING_CATEGORY_FILTER = List[rdb.BuiltInCategory](
-    [
-        rdb.BuiltInCategory.OST_Railings,
-        rdb.BuiltInCategory.OST_RailingBalusterRail,
-        rdb.BuiltInCategory.OST_RailingHandRail,
-        rdb.BuiltInCategory.OST_RailingSupport,
-        rdb.BuiltInCategory.OST_RailingSystem,
-        rdb.BuiltInCategory.OST_RailingTermination,
-        rdb.BuiltInCategory.OST_RailingTopRail,
-    ]
-)
+def _get_all_roof_types_by_category(doc):
+    """
+    Gets a filtered element collector of all roof types in the model.
+
+    - Basic Roof
+    - In place families or loaded families
+    - sloped glazing
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+
+    :return: A filtered element collector containing roof types.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    """
+
+    collector = (
+        rdb.FilteredElementCollector(doc)
+        .OfCategory(rdb.BuiltInCategory.OST_Roofs)
+        .WhereElementIsElementType()
+    )
+    return collector
+
+
+def _get_roof_types_by_class(doc):
+    """
+    Gets a filtered element collector of all Roof types in the model:
+
+    - Basic Roof
+    - sloped glazing
+
+    Since this is based of class roof it will therefore not return any in place family types!
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+
+    :return: A filtered element collector containing roof types.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    """
+
+    collector = rdb.FilteredElementCollector(doc).OfClass(rdb.RoofType)
+    return collector
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railing_family_names.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railing_family_names.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_filter.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railings_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/Utility/railings_type_sorting.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/Utility/railings_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/balusters.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/balusters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Railings/railings.py` & `DuHast-0.0.9/src/duHast/Revit/Railings/railings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py` & `DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py` & `DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py` & `DuHast-0.0.9/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ramps/purge_unused_ramp_types.py` & `DuHast-0.0.9/src/duHast/Revit/Ramps/purge_unused_ramp_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Ramps/ramps.py` & `DuHast-0.0.9/src/duHast/Revit/Ramps/ramps.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Revisions/new_revision.py` & `DuHast-0.0.9/src/duHast/Revit/Revisions/new_revision.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Revisions/revisions.py` & `DuHast-0.0.9/src/duHast/Revit/Revisions/revisions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Revisions/sequence.py` & `DuHast-0.0.9/src/duHast/Revit/Revisions/sequence.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py` & `DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py` & `DuHast-0.0.9/src/duHast/Revit/Common/element_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a Revit roofs utility functions. 
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+This module contains a number of lists containing loadable family categories. 
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
@@ -22,52 +22,31 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-# import Autodesk
-import Autodesk.Revit.DB as rdb
+from Autodesk.Revit.DB import BuiltInParameter
 
-
-def _get_all_roof_types_by_category(doc):
-    """
-    Gets a filtered element collector of all roof types in the model.
-
-    - Basic Roof
-    - In place families or loaded families
-    - sloped glazing
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector containing roof types.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
-    """
-
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Roofs)
-        .WhereElementIsElementType()
-    )
-    return collector
-
-
-def _get_roof_types_by_class(doc):
-    """
-    Gets a filtered element collector of all Roof types in the model:
-
-    - Basic Roof
-    - sloped glazing
-
-    Since this is based of class roof it will therefore not return any in place family types!
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector containing roof types.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
-    """
-
-    collector = rdb.FilteredElementCollector(doc).OfClass(rdb.RoofType)
-    return collector
+def get_room_element_is_in(element, phase_dict):
+	'''
+	Get the room an element is in
+	:param element: The element to check
+	:type element: FamilyInstance
+	:param phase_dict: The dictionary of phase name to phase element
+	:type phase_dict: dict
+	:return: The room the element is in
+	:rtype: Room
+	'''
+	el_phase = element.get_Parameter(BuiltInParameter.PHASE_CREATED)
+	if el_phase != None:
+		el_phase_name = el_phase.AsValueString()
+		try:
+			el_phase_elem = phase_dict[el_phase_name]
+		except:
+			return None
+		el_room = element.get_Room(el_phase_elem)
+		
+		return el_room
+	else:
+		return None
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py` & `DuHast-0.0.9/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Roofs/purge_unused_roof_types.py` & `DuHast-0.0.9/src/duHast/Revit/Roofs/purge_unused_roof_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Roofs/roofs.py` & `DuHast-0.0.9/src/duHast/Revit/Roofs/roofs.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Rooms/Export/to_data_room.py` & `DuHast-0.0.9/src/duHast/Revit/Rooms/Export/to_data_room.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Rooms/Geometry/geometry.py` & `DuHast-0.0.9/src/duHast/Revit/Rooms/Geometry/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,30 @@
 
 import Autodesk.Revit.DB as rdb
 
 from duHast.Revit.Rooms.rooms import get_all_rooms
 from duHast.Data.Objects.Properties.Geometry import geometry_polygon as dGeometryPoly
 
 
-def get_room_boundary_loops(revit_room):
+def get_room_boundary_loops(revit_room,
+                            spatial_boundary_option=rdb.SpatialElementBoundaryOptions(),
+                            boundary_location=rdb.SpatialElementBoundaryLocation.Center):
     """
-    Returns all boundary loops for a rooms.
+    Returns all boundary loops for a rooms. Default value set to the center
+    boundary location.
     :param revit_room: The room.
     :type revit_room: Autodesk.Revit.DB.Architecture.Room
     :return: List of boundary loops defining the room.
     :rtype: List of lists of Autodesk.Revit.DB.BoundarySegment
     """
 
     all_boundary_loops = []
     # set up spatial boundary option
-    spatial_boundary_option = rdb.SpatialElementBoundaryOptions()
     spatial_boundary_option.StoreFreeBoundaryFaces = True
-    spatial_boundary_option.SpatialElementBoundaryLocation = (
-        rdb.SpatialElementBoundaryLocation.Center
-    )
+    spatial_boundary_option.SpatialElementBoundaryLocation = boundary_location
     # get loops
     loops = revit_room.GetBoundarySegments(spatial_boundary_option)
     all_boundary_loops.append(loops)
     return all_boundary_loops
 
 
 def get_points_from_room_boundaries(boundary_loops):
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Rooms/room_tags.py` & `DuHast-0.0.9/src/duHast/Revit/Rooms/room_tags.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Rooms/rooms.py` & `DuHast-0.0.9/src/duHast/Revit/Rooms/rooms.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,7 +117,23 @@
     unplaced = []
     boundary_option = rdb.SpatialElementBoundaryOptions()
     for r in coll:
         boundary_segments = r.GetBoundarySegments(boundary_option)
         if r.Area == 0.0 and (boundary_segments != None and len(boundary_segments) > 0):
             unplaced.append(r)
     return unplaced
+
+def get_all_placed_rooms(doc):
+    """
+    Gets a list of all placed rooms from the model.
+
+    Placed criteria is Location is not null and Area > 0.0m2
+
+    :param doc: Revit model document to search.
+    :type doc: Autodesk.Revit.DB.Document
+
+    :return: All the placed rooms in the model as a list.
+    :rtype: List Autodesk.Revit.DB.Architecture.Room
+    """
+
+    all_rooms = get_all_rooms(doc)
+    return [rm for rm in all_rooms if rm.Location != None and rm.Area > 0.0]
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_data.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_processor.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_swap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,171 +1,200 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Family shared parameter data processor class.
+This module contains a function to swap out one shard parameter for another.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The swap is done by:
+- changing current shared parameter to a family parameter (dummy)
+- deleting the old shared parameter definition
+- swapping the family parameter (dummy) to the new shared parameter.
+
+Note: storage types of old and new shared parameter need to be identical.
+
+Parameter change directives are read from a .csv file:
+
+- header row: yes
+- column 1: current shared parameter name
+- column 2: new shared parameter name
+- column 3: fully qualified file path of shared parameter file
+- column 4: Is parameter instance (True / False)
+- column 5: parameter grouping name ( refer to module: RevitParameterGrouping)
+
 """
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# BSD License
-# Copyright 2023, Jan Christel
-# All rights reserved.
-
-# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+# Copyright (c) 2021  Jan Christel
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
-# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
+#
+
+import clr
+import System
 
-from duHast.Revit.Family.Data.ifamily_processor import IFamilyProcessor
-from duHast.Revit.SharedParameters import shared_parameter_data as rSharedData
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+# import common library modules
+# from duHast.APISamples.Common import RevitCommonAPI as com
 from duHast.Utilities.Objects import result as res
+from duHast.Utilities import files_csv as fileCSV
+from duHast.Revit.SharedParameters import shared_parameter_add as rSharedPAdd
+from duHast.Revit.SharedParameters import shared_parameters_tuple as rSharedT
+from duHast.Revit.Common import parameter_grouping as rPG
+from duHast.Revit.SharedParameters import shared_parameters as rSharedPara
+from duHast.Revit.SharedParameters import shared_parameters_delete as rSharedParaDelete
+from duHast.Revit.SharedParameters import (
+    shared_parameter_type_change as rSharedTypeChange,
+)
 
+from collections import namedtuple
 
-class SharedParameterProcessor(IFamilyProcessor):
-    def __init__(self, pre_actions=None, post_actions=None):
-        """
-        Class constructor.
-        """
-
-        # setup report header
-        string_report_headers = [
-            IFamData.ROOT,
-            IFamData.ROOT_CATEGORY,
-            IFamData.FAMILY_NAME,
-            IFamData.FAMILY_FILE_PATH,
-            rSharedData.PARAMETER_NAME,
-            rSharedData.PARAMETER_GUID,
-            rSharedData.PARAMETER_ID,
-            IFamData.USAGE_COUNTER,
-            IFamData.USED_BY,
-        ]
-
-        # store data type  in base class
-        super(SharedParameterProcessor, self).__init__(
-            pre_actions=pre_actions,
-            post_actions=[self._post_action_update_used_shared_parameters],
-            data_type="SharedParameter",
-            string_report_headers=string_report_headers,
-        )
-
-        # self.data = []
-        # self.dataType = 'SharedParameter'
-        # self.preActions = preActions
-        # set default post action to updated shared parameters used in root processor with any shared parameters found in nested
-        # families
-        # self.postActions = [self._postActionUpdateUsedSharedParameters]
-        # add any other post actions
-        if post_actions != None:
-            for post_action in post_actions:
-                self.post_actions.append(post_action)
-
-    def process(self, doc, root_path, root_category_path):
-        """
-        Calls processor instance with the document and root path provided and adds processor instance to class property .data
-
-        :param doc: Current family document.
-        :type doc: Autodesk.Revit.DB.Document
-        :param rootPath: The path of the nested family in a tree: rootFamilyName::nestedFamilyNameOne::nestedFamilyTwo\
-            This includes the actual family name as the last node.
-        :type rootPath: str
-        :param rootCategoryPath: The categroy path of the nested family in a tree: rootFamilyCategory::nestedFamilyOneCategory::nestedFamilyTwoCategory\
-            This includes the actual family category as the last node.
-        :type rootCategoryPath: str
-        """
-
-        dummy = rSharedData.SharedParameterData(
-            root_path, root_category_path, self.data_type
-        )
-        dummy.process(doc)
-        self.data.append(dummy)
-
-    def _is_shared_parameter_present(
-        self, root_family_data, nested_family_line_pattern
-    ):
-        match = None
-        for root_fam in root_family_data:
-            if (
-                root_fam[rSharedData.PARAMETER_GUID]
-                == nested_family_line_pattern[rSharedData.PARAMETER_GUID]
-            ):
-                match = root_fam
-                break
-        return match
-
-    def _update_root_family_data(self, root_family_data, nested_families_data):
-        # loop over nested family data
-        for nested_item in nested_families_data:
-            # check if item is already in root family
-            matching_root_fam_pattern = self._is_shared_parameter_present(
-                root_family_data, nested_item
-            )
-            if matching_root_fam_pattern != None:
-                # update used by list
-                # TODO: this check looks odd!! ( guid vs a dictionary?)
-                if (
-                    nested_item[rSharedData.PARAMETER_GUID]
-                    not in matching_root_fam_pattern[IFamData.USED_BY]
-                ):
-                    # add the root path to the used by list for ease of identification of the origin of this shared parameter
-                    matching_root_fam_pattern[IFamData.USED_BY].append(
-                        {
-                            rSharedData.PARAMETER_GUID: nested_item[
-                                rSharedData.PARAMETER_GUID
-                            ],
-                            rSharedData.PARAMETER_NAME: nested_item[
-                                rSharedData.PARAMETER_NAME
-                            ],
-                            IFamData.ROOT: nested_item[IFamData.ROOT],
-                        }
-                    )
-                    # update used by counter
-                    matching_root_fam_pattern[IFamData.USAGE_COUNTER] = (
-                        matching_root_fam_pattern[IFamData.USAGE_COUNTER] + 1
-                    )
-            else:
-                pass
-                # nothing to do if that shared parameter has not been reported to start off with
 
-    def _get_used_shared_parameters(self, data):
-        used_shared_paras = []
-        for d in data:
-            if d[IFamData.USAGE_COUNTER] > 0:
-                used_shared_paras.append(d)
-        return used_shared_paras
-
-    def _post_action_update_used_shared_parameters(self, doc):
-        return_value = res.Result()
-        try:
-            # find all shared parameters of nested families
-            nested_family_data = self._find_nested_families_data()
-            # get used shared parameters from nested data
-            nested_family_shared_parameters = self._get_used_shared_parameters(
-                nested_family_data
-            )
-            # update root family data only
-            rootFamilyData = self._find_root_family_data()
-            # update root processor data as required
-            self._update_root_family_data(
-                rootFamilyData, nested_family_shared_parameters
+"""
+Tuple containing settings data on how to swap a shared parameter retrieved from a file.
+"""
+
+PARAMETER_SETTINGS_DATA = namedtuple(
+    "parameterSettingsData", "oldParameterName newParameterData sharedParameterPath"
+)
+
+
+def _load_shared_parameter_data_from_file(file_path):
+    """
+    _summary_
+
+    :param file_path: Fully qualified file path to shared parameter change directive file.
+    :type file_path: str
+
+    :return: A dictionary in format; key: current parameter name, value: named tuple of type parameterSettingsData
+    :rtype: {str:named tuple}
+    """
+
+    parameter_mapper = {}
+    file_data = fileCSV.read_csv_file(file_path)
+    for i in range(1, len(file_data)):
+        row = file_data[i]
+        if len(row) == 5:
+            flag = False
+            if row[3].upper() == "TRUE":
+                flag = True
+            t = rSharedT.PARAMETER_DATA(
+                row[1], flag, rPG.PRAMETER_GROPUING_TO_BUILD_IN_PARAMETER_GROUPS[row[4]]
             )
-            return_value.update_sep(
-                True, "Post Action Update shared parameters data successful completed."
+            parameter_mapper[row[0]] = PARAMETER_SETTINGS_DATA(row[0], t, row[2])
+    return parameter_mapper
+
+
+def swap_shared_parameters(doc, change_directive_file_path):
+    """
+    Swaps out a shared parameter for another. (refer to module header for details)
+
+    :param doc: Current Revit family document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param change_directive_file_path: Fully qualified file path to shared parameter change directive.
+    :type change_directive_file_path: str
+
+    :return:
+        Result class instance.
+
+        - False if an exception occurred, otherwise True.
+        - result.message will contain the names of the changed shared parameter(s).
+        - result status will contain lists of new shared parameters
+
+        On exception (handled by optimizer itself!):
+
+        - result.status (bool) will be False.
+        - result.message will contain exception message.
+
+    :rtype: :class:`.Result`
+    """
+
+    return_value = res.Result()
+    _parameter_prefix_ = "_dummy_"
+    # load change directive
+    parameter_directives = _load_shared_parameter_data_from_file(
+        change_directive_file_path
+    )
+    if len(parameter_directives) > 0:
+        # loop over directive and
+        for p_directive in parameter_directives:
+            # load shared para file
+            shared_para_def_file = rSharedPAdd.load_shared_parameter_file(
+                doc, parameter_directives[p_directive].sharedParameterPath
             )
-        except Exception as e:
-            return_value.update_sep(
-                False,
-                "Post Action Update shared parameters data failed with exception: "
-                + str(e),
+            return_value.append_message(
+                "Read shared parameter file: {}".format(
+                    parameter_directives[p_directive].sharedParameterPath
+                )
             )
-        return return_value
+            if shared_para_def_file != None:
+                #   - swap shared parameter to family parameter
+                status_change_to_fam_para = (
+                    rSharedTypeChange.change_shared_parameter_to_family_parameter(
+                        doc, p_directive, _parameter_prefix_
+                    )
+                )
+                return_value.update(status_change_to_fam_para)
+                if status_change_to_fam_para.status:
+                    #   - delete all shared parameter definition
+                    status_delete_old_shared_para_def = (
+                        rSharedParaDelete.delete_shared_parameter_by_name(
+                            doc, p_directive
+                        )
+                    )
+                    return_value.update(status_delete_old_shared_para_def)
+                    if status_delete_old_shared_para_def.status:
+                        # get shared parameter definition
+                        s_para_def = rSharedPara.get_shared_parameter_definition(
+                            parameter_directives[p_directive].newParameterData.name,
+                            shared_para_def_file,
+                        )
+                        #   - add new shared parameter
+                        if s_para_def != None:
+                            return_value.append_message(
+                                "Retrieved shared parameter definition for: {}".format(
+                                    parameter_directives[
+                                        p_directive
+                                    ].newParameterData.name
+                                )
+                            )
+                            #   - swap family parameter to shared parameter
+                            status_swap_fam_to_shared_p = rSharedTypeChange.change_family_parameter_to_shared_parameter(
+                                doc,
+                                _parameter_prefix_ + p_directive,  # add prefix
+                                parameter_directives[p_directive].newParameterData,
+                                s_para_def,
+                            )
+                            return_value.update(status_swap_fam_to_shared_p)
+                        else:
+                            return_value.update_sep(
+                                False,
+                                "Failed to get shared parameter definition from file.",
+                            )
+                    else:
+                        return_value.update(status_delete_old_shared_para_def)
+                else:
+                    return_value.update(status_change_to_fam_para)
+            else:
+                return_value.update_sep(
+                    False,
+                    "Failed to load shared parameter def file from: "
+                    + parameter_directives[p_directive].sharedParameterPath,
+                )
+    else:
+        return_value.status = False
+        return_value.message = "No change directives in file."
+    return return_value
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py` & `DuHast-0.0.9/src/duHast/Revit/Warnings/solver_duplicate_mark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Family shared parameters purge unused utilities.
+Duplicate mark warnings solver class.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-This will delete all shared parameter definitions which are not used by any family parameter.
-
-- requires a revit shared parameter processor object
-
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
@@ -27,95 +23,96 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-# class used for stats reporting
+from duHast.Revit.Common import parameter_get_utils as rParaGet
+from duHast.Revit.Common import parameter_set_utils as rParaSet
 from duHast.Utilities.Objects import result as res
-from duHast.Revit.Family.Data import ifamily_data as IFamData
-from duHast.Revit.SharedParameters import shared_parameter_data as rSharedParaData
-from duHast.Revit.Categories import categories as rCat
-from duHast.Revit.Common import delete as rDel
 
+
+# import Autodesk
 import Autodesk.Revit.DB as rdb
+from duHast.Utilities.Objects import base
 
 
-def purge_unused(doc, processor):
-    """
-    This will delete all shared parameter definitions which are not used by any family parameter in the family or nested families.
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :param processor: An RevitSharedParameterDataProcessor object containing all shared parameter information of the family document and any nested families.
-    :type processor: :class:`.SharedParameterProcessor`
-
-    :return:
-        Result class instance.
-
-        - True if all unused shared parameters where deleted successfully or none needed to be deleted. Otherwise False.
-        - Result.message property updated in format: Found unused shared parameter: shared parameter Name [GUID]
-
-        On exception:
-
-        - status (bool) will be False.
-        - message will contain the exception message.
-
-    :rtype: :class:`.Result`
-    """
-
-    # from processor instance get all root line pattern entries where usage counter == 0.
-    # delete those line patterns by id
-
-    return_value = res.Result()
-
-    # check the category of the family first:
-    # Tags and generic annotations (may) contain labels which in turn use shared parameters to drive them
-    # there is currently no way in the api (Revit 2022) to find out what parameter is driving the label...
-
-    # get the family category name:
-    fam_cat_name = list(rCat.get_family_category(doc))[0]
-    if fam_cat_name != "Generic Annotations" and fam_cat_name.endswith("Tags") == False:
-        ids_to_delete = []
-        # get categories found in root processor data only
-        root_fam_data = processor._findRootFamilyData()
-        # get all root line pattern entries where usage counter == 0.
-        for root_fam in root_fam_data:
-            if root_fam[IFamData.USAGE_COUNTER] == 0:
-                return_value.append_message(
-                    "Found unused shared parameter: {} [{}]".format(
-                        root_fam[rSharedParaData.PARAMETER_NAME],
-                        root_fam[rSharedParaData.PARAMETER_GUID],
-                    )
-                )
-                ids_to_delete.append(
-                    rdb.ElementId(root_fam[rSharedParaData.PARAMETER_ID])
-                )
-        # delete any subcategories found
-        if len(ids_to_delete) > 0:
-            result_delete = rDel.delete_by_element_ids(
-                doc,
-                ids_to_delete,
-                "Deleting unused shared parameters.",
-                "Shared Parameters",
-            )
-            return_value.update(result_delete)
-            # may need to delete shared parameters one by one if one or more cant be deleted
-            if result_delete.status == False:
-                result_delete_one_by_one = rDel.delete_by_element_ids_one_by_one(
-                    doc,
-                    ids_to_delete,
-                    "Deleting unused shared parameters: one by one.",
-                    "Shared Parameters",
-                )
-                return_value.update(result_delete_one_by_one)
+class RevitWarningsSolverDuplicateMark(base.Base):
+    def __init__(self, filter_func, filter_values=[]):
+        """
+        Constructor: this solver takes two arguments: a filter function and a list of values to filter by
+
+        :param filter_func: A function to filter elements in warnings by
+        :type filter_func: func(document, elementId, list of filter values)
+        :param filter_values: A list of filter values, defaults to []
+        :type filter_values: list, optional
+        """
+
+        # ini super class to allow multi inheritance in children!
+        super(RevitWarningsSolverDuplicateMark, self).__init__()
+
+        self.filter = filter_func
+        self.filter_values = filter_values
+        self.filter_name = "Duplicate mark value."
+
+    # --------------------------- duplicate mark guid ---------------------------
+    #: guid identifying this specific warning
+    GUID = "6e1efefe-c8e0-483d-8482-150b9f1da21a"
+
+    def solve_warnings(self, doc, warnings):
+        """
+        Solver setting element mark to nothing, provided it passes the filter.
+
+        :param doc: Current Revit model document.
+        :type doc: Autodesk.Revit.DB.Document
+        :param warnings: List of warnings to be solved.
+        :type warnings: Autodesk.Revit.DB.FailureMessage
+
+        :return:
+            Result class instance.
+
+            - .result = True if all duplicate mark warnings could be solved. Otherwise False.
+            - .message will contain stats in format parameter value set to ''
+
+        :rtype: :class:`.Result`
+        """
+
+        return_value = res.Result()
+        if len(warnings) > 0:
+            for warning in warnings:
+                element_ids = warning.GetFailingElements()
+                for el_id in element_ids:
+                    element = doc.GetElement(el_id)
+                    # check whether element passes filter
+                    if self.filter(doc, el_id, self.filter_values):
+                        try:
+                            p_value = rParaGet.get_built_in_parameter_value(
+                                element, rdb.BuiltInParameter.ALL_MODEL_MARK
+                            )
+                            if p_value != None:
+                                result = rParaSet.set_built_in_parameter_value(
+                                    doc,
+                                    element,
+                                    rdb.BuiltInParameter.ALL_MODEL_MARK,
+                                    "",
+                                )
+                                return_value.update(result)
+                        except Exception as e:
+                            return_value.update_sep(
+                                False,
+                                "Failed to solve warning duplicate mark with exception: {}".format(
+                                    e
+                                ),
+                            )
+                    else:
+                        return_value.update_sep(
+                            True,
+                            "Element removed by filter: {} : {}".format(
+                                self.filter_name, rdb.Element.Name.GetValue(element)
+                            ),
+                        )
         else:
             return_value.update_sep(
-                True, "No unused shared parameters found. Nothing was deleted."
+                True, "No warnings of type: duplicate mark in model."
             )
-    else:
-        return_value.update_sep(
-            True,
-            "This is an annotation family (tag or generic annotation). Due to limitations in the Revit API no shared parameter was purged.",
-        )
-    return return_value
+        return return_value
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_add.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_add.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_delete.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameters_delete.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py` & `DuHast-0.0.9/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_filter.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/Utility/stairs_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/cut_marks.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/cut_marks.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/landings.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/landings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/path.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/path.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/purge_unused_stair_types.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/purge_unused_stair_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/runs.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/runs.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/stairs.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/stairs.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Stairs/stringers_carriages.py` & `DuHast-0.0.9/src/duHast/Revit/Stairs/stringers_carriages.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Objects/category_base.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/colour_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-A base class used to store category overrides.
+A base class used to store colour values.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
-Stores common overrides between categories and filters
+Stores colour values as rgb.
 
 """
 
 
 #
 # License:
 #
@@ -31,26 +31,26 @@
 #
 #
 #
 
 import json
 
 from duHast.Utilities.Objects import base
-from duHast.Revit.Views.Objects.override_projection import OverrideProjection
-from duHast.Revit.Views.Objects.override_cut import OverrideCut
 
 
-class OverrideModelCategory(base.Base):
+class ColourBase(base.Base):
+    data_type = "colour"
+
     def __init__(self, j={}, **kwargs):
         """
         Class constructor.
 
         """
 
-        super(OverrideModelCategory, self).__init__(**kwargs)
+        super(ColourBase, self).__init__(**kwargs)
 
         # check if any data was past in with constructor!
         if j != None and len(j) > 0:
             # check type of data that came in:
             if type(j) == str:
                 # a string
                 j = json.loads(j)
@@ -59,33 +59,37 @@
                 pass
             else:
                 raise ValueError(
                     "Argument supplied must be of type string or type dictionary"
                 )
 
             # load overrides
-            if "halftone" in j:
-                self.halftone = j["halftone"]
+            if "red" in j:
+                self.red = j["red"]
             else:
-                self.halftone = False
+                self.red = 0
 
-            if "transparency" in j:
-                self.transparency = j["transparency"]
+            if "green" in j:
+                self.green = j["green"]
             else:
-                self.transparency = 0
+                self.green = 0
 
-            if OverrideProjection.data_type in j:
-                self.override_projection = OverrideProjection(
-                    j[OverrideProjection.data_type]
-                )
+            if "blue" in j:
+                self.blue = j["blue"]
             else:
-                self.override_projection = OverrideProjection()
-
-            if OverrideCut.data_type in j:
-                self.override_cut = OverrideCut(j[OverrideCut.data_type])
-            else:
-                self.override_cut = OverrideCut()
+                self.blue = 0
         else:
-            self.halftone = False
-            self.transparency = 0
-            self.override_projection = OverrideProjection()
-            self.override_cut = OverrideCut()
+            self.red = 0
+            self.green = 0
+            self.blue = 0
+
+    def __eq__(self, other):
+        """
+        Custom compare is equal override
+
+        :param other: Another instance of colour class
+        :type other: :class:`.ColourBase`
+        :return: True if RGB values of other colour class instance equal the RGB values of this instance, otherwise False.
+        :rtype: Bool
+        """
+
+        return (self.red, self.green, self.blue) == (other.red, other.green, other.blue)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_by_category.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_by_category.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,37 +21,35 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Views.Objects.category_base import OverrideModelCategory
+import json
 
+from duHast.Revit.Views.Objects.Data.override_by_base import OverrideByBase
 
-class OverrideByCategory(OverrideModelCategory):
-
+class OverrideByCategory(OverrideByBase):
     data_type = "override_by_category"
-    
-    def __init__(self,main_category_name = "" , sub_category_name = "" , category_id = -1, j={}):
+
+    def __init__(
+        self, main_category_name="", sub_category_name="", category_id=-1, j={}
+    ):
         """
         Class constructor.
 
         """
 
-        super(OverrideByCategory, self).__init__(j=j)
+        super(OverrideByCategory, self).__init__(data_type=self.data_type, j=j)
 
-        self.main_category_name=main_category_name
+        self.main_category_name = main_category_name
         self.sub_category_name = sub_category_name
         self.category_id = category_id
 
-    def update(self,override):
-        self.main_category_name = override.main_category_name
-        self.sub_category_name = override.sub_category_name
-        self.category_id= override.category_id
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_by_filter.py` & `DuHast-0.0.9/src/duHast/Revit/LinePattern/Objects/Data/line_pattern_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-A base class used to store category overrides.
+A base class used to store pattern category overrides.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
-Stores common overrides between categories and filters
+Stores line patterns.
 
 """
 
 
 #
 # License:
 #
@@ -28,27 +28,23 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Views.Objects.category_base import OverrideModelCategory
 
+from duHast.Revit.Common.Objects.Data.pattern_settings_base import PatternSettingBase
 
-class OverrideByFilter(OverrideModelCategory):
+class LinePatternSettings(PatternSettingBase):
+    data_type = "line_pattern_settings"
 
-    data_type = "override_by_filter"
-    
-    def __init__(self,filter_name = "" , filter_id = -1, j={}):
+    def __init__(self, j={}):
         """
         Class constructor.
 
+        :param j: A json formatted dictionary of this class, defaults to {}
+        :type j: dict, optional
         """
 
-        super(OverrideByFilter, self).__init__(j=j)
-
-        self.filter_name = filter_name
-        self.filter_id = filter_id
-
-
-        
+        # store data type  in base class
+        super(LinePatternSettings, self).__init__(data_type=self.data_type, j=j)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_cut.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_cut.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 #
 #
 #
 
 import json
 
 from duHast.Utilities.Objects import base
-from duHast.Revit.Common.Objects import pattern_foreground, pattern_background, line_cut
+from duHast.Revit.Common.Objects.Data import pattern_foreground, pattern_background, line_cut
 
 
 class OverrideCut(base.Base):
     data_type = "override_cut"
 
     def __init__(self, j={}, **kwargs):
         """
@@ -82,7 +82,23 @@
                 self.line_cut = line_cut.LineCut(j[line_cut.LineCut.data_type])
             else:
                 self.line_cut = line_cut.LineCut()
         else:
             self.pattern_background = pattern_background.PatternBackground()
             self.pattern_foreground = pattern_foreground.PatternForeground()
             self.line_cut = line_cut.LineCut()
+
+    def __eq__(self, other):
+        """
+        Custom compare is equal override.
+
+        :param other: Another instance of OverrideCut class
+        :type other: :class:`.OverrideCut`
+        :return: True if all properties of compared class instances are equal, otherwise False.
+        :rtype: Bool
+        """
+
+        return (self.pattern_background, self.pattern_foreground, self.line_cut) == (
+            other.pattern_background,
+            other.pattern_foreground,
+            other.line_cut,
+        )
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Objects/override_projection.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Objects/Data/override_projection.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 #
 #
 #
 
 import json
 
 from duHast.Utilities.Objects import base
-from duHast.Revit.Common.Objects import (
+from duHast.Revit.Common.Objects.Data import (
     pattern_foreground,
     pattern_background,
     line_projection,
 )
 
 
 class OverrideProjection(base.Base):
@@ -88,7 +88,23 @@
                 )
             else:
                 self.line_projection = line_projection.LineProjection()
         else:
             self.pattern_background = pattern_background.PatternBackground()
             self.pattern_foreground = pattern_foreground.PatternForeground()
             self.line_projection = line_projection.LineProjection()
+
+    def __eq__(self, other):
+        """
+        Custom compare is equal override.
+
+        :param other: Another instance of OverrideProjection class
+        :type other: :class:`.OverrideProjection`
+        :return: True if all properties of compared class instances are equal, otherwise False.
+        :rtype: Bool
+        """
+
+        return (self.pattern_background, self.pattern_foreground, self.line_projection) == (
+            other.pattern_background,
+            other.pattern_foreground,
+            other.line_projection,
+        )
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Objects/view_graphics_settings.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Objects/view_graphics_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 #
 #
 
 import json
 
 from duHast.Utilities.Objects import base
 
-from duHast.Revit.Views.Objects.override_by_category import OverrideByCategory
-from duHast.Revit.Views.Objects.override_by_filter import OverrideByFilter
+from duHast.Revit.Views.Objects.Data.override_by_category import OverrideByCategory
+from duHast.Revit.Views.Objects.Data.override_by_filter import OverrideByFilter
 
 
 class ViewGraphicsSettings(base.Base):
     def __init__(self, view_name="", view_id=-1, j={}, **kwargs):
         """
         Class constructor.
 
@@ -83,26 +83,7 @@
             else:
                 self.override_by_filter = []
 
         else:
             self.override_by_category = []
             self.override_by_filter = []
 
-    def add_overrides_by_category(self, override):
-        """
-        Add overrides by category settings
-
-        :param override: _description_
-        :type override: _type_
-        """
-
-        self.override_by_category.append(override)
-
-    def add_overrides_by_filter(self, override):
-        """
-        Add overrides by filter settings
-
-        :param override: _description_
-        :type override: _type_
-        """
-
-        self.override_by_filter.append(override)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/schedules_report.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Reporting/schedules_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/sheets_report.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Reporting/sheets_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_filter.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Reporting/view_property_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/view_property_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Reporting/view_property_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Reporting/views_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Reporting/views_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Reporting/views_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Utility/data_view.py` & `DuHast-0.0.9/src/duHast/Revit/Common/Objects/Data/pattern_settings_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Category override data storage class.
+A base class used to store pattern data.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+
+Stores pattern base data for line and fill pattern.
+
 """
+
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -23,43 +29,62 @@
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import json
-from duHast.Revit.Views.Objects.override_by_category import OverrideByCategory
-from duHast.Revit.Views.Objects.override_by_filter import OverrideByFilter
-from duHast.Revit.Views.Objects.view_graphics_settings import ViewGraphicsSettings
-
-
-def _get_model_overrides(view):
-    pass
-
-
-def _get_filter_overrides(view):
-    pass
-
-
-def convert_revit_view_to_data(doc, view):
-    """
-    Convertes a Revit view element into an instance of class ViewGraphicsSettings
-
-    :param view: A Revit view instance.
-    :type view: Autodesk.Revit.DB.View
-    :return: A storage class which contains graphics settings
-    :rtype: :class:`.ViewGraphicsSettings`
-    """
 
-    data_dic = {}
+from duHast.Utilities.Objects import base
 
-    data_dic[OverrideByCategory.data_type] = _get_model_overrides(view)
-    data_dic[OverrideByFilter.data_type] = _get_filter_overrides(view)
 
-    return_value = ViewGraphicsSettings(
-        view_name=view.Name,
-        view_id=view.Id.IntegerValue,
-        j=data_dic,
-    )
+class PatternSettingBase(base.Base):
+    def __init__(self, data_type="unknown", j={}, **kwargs):
+        """
+        Class constructor.
+
+        """
+
+        super(PatternSettingBase, self).__init__(**kwargs)
+
+        self.data_type = data_type
+
+        # check if any data was past in with constructor!
+        if j != None and len(j) > 0:
+            # check type of data that came in:
+            if type(j) == str:
+                # a string
+                j = json.loads(j)
+            elif type(j) == dict:
+                # no action required
+                pass
+            else:
+                raise ValueError(
+                    "Argument supplied must be of type string or type dictionary"
+                )
+
+            # load overrides
+            if "id" in j:
+                self.id = j["id"]
+            else:
+                self.id = -1
+
+            if "name" in j:
+                self.name = j["name"]
+            else:
+                self.name = "unknown pattern"
+
+        else:
+            self.id = -1
+            self.name = "unknown pattern"
+
+    def __eq__(self, other):
+        """
+        Custom compare is equal override (name comparison only!)
+
+        :param other: Another instance of pattern class
+        :type other: :class:`.PatternBase`
+        :return: True if name value of other colour class instance equal the name values of this instance, otherwise False.
+        :rtype: Bool
+        """
 
-    return return_value
- 
+        return (self.name) == (other.name)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/Utility/view_types.py` & `DuHast-0.0.9/src/duHast/Revit/Views/Utility/view_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/delete.py` & `DuHast-0.0.9/src/duHast/Revit/Views/delete.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/filters.py` & `DuHast-0.0.9/src/duHast/Revit/Views/filters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/referencing.py` & `DuHast-0.0.9/src/duHast/Revit/Views/referencing.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/schedules.py` & `DuHast-0.0.9/src/duHast/Revit/Views/schedules.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/sheets.py` & `DuHast-0.0.9/src/duHast/Revit/Views/sheets.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/templates.py` & `DuHast-0.0.9/src/duHast/Revit/Views/templates.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/views.py` & `DuHast-0.0.9/src/duHast/Revit/Views/views.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/views_purge_unused.py` & `DuHast-0.0.9/src/duHast/Revit/Views/views_purge_unused.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Views/visibility_graphics_utils.py` & `DuHast-0.0.9/src/duHast/Revit/Views/visibility_graphics_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/Reporting/walls_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/Reporting/walls_report_header.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/Reporting/walls_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_filter.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/Utility/walls_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/Utility/walls_type_sorting.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/Utility/walls_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/curtain_wall_elements.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/curtain_wall_elements.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/curtain_walls.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/curtain_walls.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/purge_unused_wall_types.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/purge_unused_wall_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/stacked_walls.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/stacked_walls.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Walls/walls.py` & `DuHast-0.0.9/src/duHast/Revit/Walls/walls.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data.py` & `DuHast-0.0.9/src/duHast/Revit/Warnings/Data/warnings_data.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Warnings/Data/warnings_data_processor.py` & `DuHast-0.0.9/src/duHast/Revit/Warnings/Data/warnings_data_processor.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Warnings/solver.py` & `DuHast-0.0.9/src/duHast/Revit/Warnings/solver.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Warnings/solver_duplicate_mark.py` & `DuHast-0.0.9/src/duHast/Utilities/utility.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Duplicate mark warnings solver class.
+This module contains a number of helper functions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 """
 #
 # License:
 #
 #
@@ -23,96 +23,196 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Common import parameter_get_utils as rParaGet
-from duHast.Revit.Common import parameter_set_utils as rParaSet
-from duHast.Utilities.Objects import result as res
-
-
-# import Autodesk
-import Autodesk.Revit.DB as rdb
-from duHast.Utilities.Objects import base
-
-
-class RevitWarningsSolverDuplicateMark(base.Base):
-    def __init__(self, filter_func, filter_values=[]):
-        """
-        Constructor: this solver takes two arguments: a filter function and a list of values to filter by
-
-        :param filter_func: A function to filter elements in warnings by
-        :type filter_func: func(document, elementId, list of filter values)
-        :param filter_values: A list of filter values, defaults to []
-        :type filter_values: list, optional
-        """
-
-        # ini super class to allow multi inheritance in children!
-        super(RevitWarningsSolverDuplicateMark, self).__init__()
-
-        self.filter = filter_func
-        self.filter_values = filter_values
-        self.filter_name = "Duplicate mark value."
-
-    # --------------------------- duplicate mark guid ---------------------------
-    #: guid identifying this specific warning
-    GUID = "6e1efefe-c8e0-483d-8482-150b9f1da21a"
-
-    def solve_warnings(self, doc, warnings):
-        """
-        Solver setting element mark to nothing, provided it passes the filter.
-
-        :param doc: Current Revit model document.
-        :type doc: Autodesk.Revit.DB.Document
-        :param warnings: List of warnings to be solved.
-        :type warnings: Autodesk.Revit.DB.FailureMessage
-
-        :return:
-            Result class instance.
-
-            - .result = True if all duplicate mark warnings could be solved. Otherwise False.
-            - .message will contain stats in format parameter value set to ''
-
-        :rtype: :class:`.Result`
-        """
-
-        return_value = res.Result()
-        if len(warnings) > 0:
-            for warning in warnings:
-                element_ids = warning.GetFailingElements()
-                for el_id in element_ids:
-                    element = doc.GetElement(el_id)
-                    # check whether element passes filter
-                    if self.filter(doc, el_id, self.filter_values):
-                        try:
-                            p_value = rParaGet.get_built_in_parameter_value(
-                                element, rdb.BuiltInParameter.ALL_MODEL_MARK
-                            )
-                            if p_value != None:
-                                result = rParaSet.set_built_in_parameter_value(
-                                    doc,
-                                    element,
-                                    rdb.BuiltInParameter.ALL_MODEL_MARK,
-                                    "",
-                                )
-                                return_value.update(result)
-                        except Exception as e:
-                            return_value.update_sep(
-                                False,
-                                "Failed to solve warning duplicate mark with exception: {}".format(
-                                    e
-                                ),
-                            )
-                    else:
-                        return_value.update_sep(
-                            True,
-                            "Element removed by filter: {} : {}".format(
-                                self.filter_name, rdb.Element.Name.GetValue(element)
-                            ),
-                        )
+# import clr
+# import System
+# from numpy import empty
+import os
+import os.path
+import collections
+
+# import clr
+# clr.AddReference("System.Core")
+# from System import Linq
+# clr.ImportExtensions(Linq)
+
+
+def get_local_app_data_path():
+    """
+    return directory path to local app data folder
+
+    :return: Path to local app data
+    :rtype: str
+    """
+
+    return os.environ["LOCALAPPDATA"]
+
+
+def get_current_user_name():
+    """
+    Returns the current user name
+
+    :return: the user name
+    :rtype: str
+    """
+
+    return os.environ["USERNAME"]
+
+
+# ---------------------------------------------------------------------------------------------------------------------------------
+
+
+def parse_string_to_bool(text):
+    """
+    Converts a string to lower case and then to bool. Will throw an exception if it fails to do so.
+
+    ( 'true' = True, 'false' = False)
+
+    :param text: The string representing a bool.
+    :type text: str
+    :raises Exception: If string to bool conversion fails the 'String cant be converted to bool' exception will be raised.
+
+    :return: True or False
+    :rtype: bool
+    """
+
+    if text.lower() == "true":
+        return True
+    elif text.lower() == "false":
+        return False
+    else:
+        raise Exception("String cant be converted to bool")
+
+
+# ---------------------------------------------------------------------------------------------------------------------------------
+
+#: two digit padding
+PAD_SINGLE_DIGIT_TO_TWO = "%02d"
+#: three digit padding
+PAD_SINGLE_DIGIT_TO_THREE = "%03d"
+
+
+def pad_single_digit_numeric_string(numericString, format=PAD_SINGLE_DIGIT_TO_TWO):
+    """
+    Pads a single digit integer (past in as a string) with a leading zero (default)
+
+    :param numericString: Integer as string.
+    :type numericString: str
+    :param format: The integer padding format, defaults to PAD_SINGLE_DIGIT_TO_TWO
+    :type format: str, optional
+
+    :return: The padded integer as string.
+    :rtype: str
+    """
+
+    # attempt to convert string to int first
+    try:
+        value = int(numericString)
+        return str(format % value)
+    except Exception:
+        # string was not an integer...
+        return numericString
+
+
+def encode_ascii(string):
+    """
+    Encode a string as ascii and replaces all non ascii characters
+
+    If a non string is past in the value will be returned unchanged.
+
+    :param string: The string to be ascii encoded.
+    :type string: str
+
+    :return: ascii encoded string
+    :rtype: str
+    """
+    if type(string) == str:
+        return string.encode("ascii", "replace")
+    else:
+        return string
+
+
+def get_first(iterable, default, condition=lambda x: True):
+    """
+    Returns the first value in a list matching condition. If no value found returns the specified default value.
+
+    :param iterable: the list to be searched.
+    :type iterable: iterable
+    :param default: The default value
+    :type default: var
+    :param condition: The condition to be checked, defaults to lambda x:True
+    :type condition: _type_, optional
+
+    :return: First value matching condition, otherwise default value
+    :rtype: var
+    """
+
+    return next((x for x in iterable if condition(x)), default)
+
+
+def index_of(list, item):
+    """
+    Gets the index of item in list
+
+    :param list: The list
+    :type list: list
+    :param item: The item of which to return the index.
+    :type item: var
+
+    :return: The index of the item in the list, if no match -1 will be returned
+    :rtype: int
+    """
+    try:
+        return list.index(item)
+    except:
+        return -1
+
+
+def remove_items_from_list(sourceList, removeIdsList):
+    """
+    helper removes items from a source list
+
+    :param sourceList: The list containing items
+    :type sourceList: list var
+    :param removeIdsList: the list containing items to be removed
+    :type removeIdsList: list var
+
+    :return: The filtered source list.
+    :rtype: list var
+    """
+
+    try:
+        for item in removeIdsList:
+            sourceList.remove(item)
+    except:
+        pass
+    return sourceList
+
+
+def flatten(d, parent_key="", sep="_"):
+    """
+    Flattens a dictionary as per stack overflow
+
+    https://stackoverflow.com/questions/6027558/flatten-nested-dictionaries-compressing-keys/6027615#6027615
+
+    :param d: _description_
+    :type d: _type_
+    :param parent_key: _description_, defaults to ''
+    :type parent_key: str, optional
+    :param sep: _description_, defaults to '_'
+    :type sep: str, optional
+    :return: _description_
+    :rtype: _type_
+    """
+
+    items = []
+    for k, v in d.items():
+        new_key = parent_key + sep + k if parent_key else k
+        if isinstance(v, collections.MutableMapping):
+            items.extend(flatten(v, new_key, sep=sep).items())
         else:
-            return_value.update_sep(
-                True, "No warnings of type: duplicate mark in model."
-            )
-        return return_value
+            items.append((new_key, v))
+    return dict(items)
```

### Comparing `DuHast-0.0.8/src/duHast/Revit/Warnings/solver_room_tag_to_room.py` & `DuHast-0.0.9/src/duHast/Revit/Warnings/solver_room_tag_to_room.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Revit/Warnings/warnings.py` & `DuHast-0.0.9/src/duHast/Revit/Warnings/warnings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/UI/file_item.py` & `DuHast-0.0.9/src/duHast/UI/file_item.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/UI/file_list.py` & `DuHast-0.0.9/src/duHast/UI/file_list.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/UI/file_select_settings.py` & `DuHast-0.0.9/src/duHast/UI/file_select_settings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/UI/script.py` & `DuHast-0.0.9/src/duHast/UI/script.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/UI/ui_file_select.py` & `DuHast-0.0.9/src/duHast/UI/ui_file_select.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/UI/workload_bucket.py` & `DuHast-0.0.9/src/duHast/UI/workload_bucket.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/UI/workloader.py` & `DuHast-0.0.9/src/duHast/UI/workloader.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/Objects/base.py` & `DuHast-0.0.9/src/duHast/Utilities/Objects/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import json
 
@@ -65,7 +65,38 @@
         Convert the instance of this class to json.
 
         :return: A Json object.
         :rtype: json
         """
 
         return json.dumps(self, indent=None, default=lambda o: o.__dict__)
+
+    def _is_primitive(self, obj):
+        """
+        Checks whether object past in is a python primitive
+
+        :param obj: The object to be tested.
+        :type obj: obj
+        :return: True if object is a python primitive, Otherwise False.
+        :rtype: Bool
+        """
+
+        return isinstance(obj, (int, float, str, bool))
+
+    def class_to_dict(self):
+        """
+        Returns all class properties and their values as a dictionary
+
+        :return: A dictionary of all class properties names and their values
+        :rtype: {str:var,}
+        """
+
+        if isinstance(self, object):
+            class_dict = {}
+            for key, value in self.__dict__.items():
+                if self._is_primitive(value):
+                    class_dict[key] = value
+                else:
+                    class_dict[key] = value.class_to_dict()
+            return class_dict
+        else:
+            return self
```

### Comparing `DuHast-0.0.8/src/duHast/Utilities/Objects/result.py` & `DuHast-0.0.9/src/duHast/Utilities/Objects/result.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/Objects/timer.py` & `DuHast-0.0.9/src/duHast/Utilities/Objects/timer.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/batch_processor_log_utils.py` & `DuHast-0.0.9/src/duHast/Utilities/batch_processor_log_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/compare.py` & `DuHast-0.0.9/src/duHast/Utilities/compare.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/console_out.py` & `DuHast-0.0.9/src/duHast/Utilities/console_out.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/date_stamps.py` & `DuHast-0.0.9/src/duHast/Utilities/date_stamps.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/directory_io.py` & `DuHast-0.0.9/src/duHast/Utilities/directory_io.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/files_combine.py` & `DuHast-0.0.9/src/duHast/Utilities/files_combine.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,29 +67,71 @@
     :param out_put_file_name: The file name of the combined file, defaults to 'result.txt'
     :type out_put_file_name: str, optional
     :param file_getter: Function returning list of files to be combined, defaults to GetFilesSingleFolder
     :type file_getter: func(folder_path, file_prefix, file_suffix, file_extension), optional
     """
 
     file_list = file_getter(folder_path, file_prefix, file_suffix, file_extension)
-    with open(folder_path + "\\" + out_put_file_name, "w") as result:
+    with open(os.path.join(folder_path , out_put_file_name), "w") as result:
         file_counter = 0
         for file_ in file_list:
             line_counter = 0
             fp = open(file_, "r")
             lines = fp.readlines()
             fp.close()
             for line in lines:
                 # ensure header from first file is copied over
                 if file_counter == 0 and line_counter == 0 or line_counter != 0:
                     result.write(line)
                 line_counter += 1
 
             file_counter += 1
 
+def combine_files_basic(
+    folder_path,
+    file_prefix="",
+    file_suffix="",
+    file_extension=".txt",
+    out_put_file_name="result.txt",
+    file_getter=get_files_single_directory,
+):
+    """
+    Combines multiple text files into a single new file.
+    Assumes:
+
+    - files are text files
+
+    The new file will be saved into the same folder as the original files.
+
+    :param folder_path: Folder path from which to get files to be combined and to which the combined file will be saved.
+    :type folder_path: str
+    :param file_prefix: Filter: File name starts with this value
+    :type file_prefix: str
+    :param file_suffix: Filter: File name ends with this value.
+    :type file_suffix: str
+    :param file_extension: Filter: File needs to have this file extension
+    :type file_extension: str, format '.extension'
+    :param out_put_file_name: The file name of the combined file, defaults to 'result.txt'
+    :type out_put_file_name: str, optional
+    :param file_getter: Function returning list of files to be combined, defaults to GetFilesSingleFolder
+    :type file_getter: func(folder_path, file_prefix, file_suffix, file_extension), optional
+    """
+
+    file_list = file_getter(folder_path, file_prefix, file_suffix, file_extension)
+    with open(os.path.join(folder_path , out_put_file_name), "w") as f:
+        for file_ in file_list:
+            fp = open(file_, "r")
+            lines = fp.readlines()
+            fp.close()
+            for line in lines:
+                f.write(line)
+        f.close()
+
+
+            
 
 def append_to_file(source_file, append_file, ignore_first_row=False):
     """
     Appends one text file to another. Assumes same number of headers (columns) in both files.
 
     :param source_file: The fully qualified file path of the file to which the other file will be appended.
     :type source_file: str
```

### Comparing `DuHast-0.0.8/src/duHast/Utilities/files_csv.py` & `DuHast-0.0.9/src/duHast/Utilities/files_csv.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/files_get.py` & `DuHast-0.0.9/src/duHast/Utilities/files_get.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/files_io.py` & `DuHast-0.0.9/src/duHast/Utilities/files_io.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/files_json.py` & `DuHast-0.0.9/src/duHast/Utilities/files_json.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/files_tab.py` & `DuHast-0.0.9/src/duHast/Utilities/files_tab.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/padding.py` & `DuHast-0.0.9/src/duHast/Utilities/padding.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/solibri_ifc_optimizer.py` & `DuHast-0.0.9/src/duHast/Utilities/solibri_ifc_optimizer.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/system_process.py` & `DuHast-0.0.9/src/duHast/Utilities/system_process.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/unit_conversion.py` & `DuHast-0.0.9/src/duHast/Utilities/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/util_batch_p.py` & `DuHast-0.0.9/src/duHast/Utilities/util_batch_p.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.0.8/src/duHast/Utilities/worksharing_monitor_process.py` & `DuHast-0.0.9/src/duHast/Utilities/worksharing_monitor_process.py`

 * *Files identical despite different names*

