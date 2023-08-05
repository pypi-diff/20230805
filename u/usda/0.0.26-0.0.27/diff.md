# Comparing `tmp/usda-0.0.26.tar.gz` & `tmp/usda-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usda-0.0.26.tar", last modified: Sat Jul 22 05:16:06 2023, max compression
+gzip compressed data, was "usda-0.0.27.tar", last modified: Sat Aug  5 13:38:44 2023, max compression
```

## Comparing `usda-0.0.26.tar` & `usda-0.0.27.tar`

### file list

```diff
@@ -1,326 +1,332 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.084477 usda-0.0.26/
--rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:46.000000 usda-0.0.26/LICENSE
--rw-rw-rw-   0        0        0     1563 2023-07-22 05:16:06.083480 usda-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0       63 2022-10-24 05:51:50.000000 usda-0.0.26/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-22 05:16:06.084477 usda-0.0.26/setup.cfg
--rw-rw-rw-   0        0        0     4305 2023-05-21 04:03:08.000000 usda-0.0.26/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.794235 usda-0.0.26/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.816013 usda-0.0.26/src/usda/
--rw-rw-rw-   0        0        0      636 2023-07-22 05:16:01.000000 usda-0.0.26/src/usda/__init__.py
--rw-rw-rw-   0        0        0      731 2022-10-16 01:25:30.000000 usda-0.0.26/src/usda/_min_dependencies.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.830947 usda-0.0.26/src/usda/data_process/
--rw-rw-rw-   0        0        0     1147 2023-03-26 03:42:06.000000 usda-0.0.26/src/usda/data_process/__init__.py
--rw-rw-rw-   0        0        0     2125 2022-10-22 01:49:00.000000 usda-0.0.26/src/usda/data_process/_geoinfodata_conversion.py
--rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:52.000000 usda-0.0.26/src/usda/data_process/_image_pixel_sampling_zoom.py
--rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:58.000000 usda-0.0.26/src/usda/data_process/_kitti_dataprocess.py
--rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:20.000000 usda-0.0.26/src/usda/data_process/_landsat_dataprocess.py
--rw-rw-rw-   0        0        0     1854 2023-03-26 07:52:40.000000 usda-0.0.26/src/usda/data_process/_naip_dataprocess.py
--rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:40.000000 usda-0.0.26/src/usda/data_process/_osm_dataprocess.py
--rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:32.000000 usda-0.0.26/src/usda/data_process/_raster_dataprocess.py
--rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:56.000000 usda-0.0.26/src/usda/data_process/_tiler_calculation.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.833657 usda-0.0.26/src/usda/data_visual/
--rw-rw-rw-   0        0        0      304 2023-07-09 12:19:48.000000 usda-0.0.26/src/usda/data_visual/__init__.py
--rw-rw-rw-   0        0        0      499 2023-05-14 10:52:14.000000 usda-0.0.26/src/usda/data_visual/_plot_style.py
--rw-rw-rw-   0        0        0     1362 2023-07-09 12:16:32.000000 usda-0.0.26/src/usda/data_visual/_worldcover_plot_style.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.855765 usda-0.0.26/src/usda/data_visualization/
--rw-rw-rw-   0        0        0     3205 2023-05-30 14:40:54.000000 usda-0.0.26/src/usda/data_visualization/__init__.py
--rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:26.000000 usda-0.0.26/src/usda/data_visualization/_chart_custom.py
--rw-rw-rw-   0        0        0     3729 2023-05-30 14:40:36.000000 usda-0.0.26/src/usda/data_visualization/_colors.py
--rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:08.000000 usda-0.0.26/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
--rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:52.000000 usda-0.0.26/src/usda/data_visualization/_gdf_plot.py
--rw-rw-rw-   0        0        0      952 2022-10-28 11:19:34.000000 usda-0.0.26/src/usda/data_visualization/_gif_show.py
--rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:46.000000 usda-0.0.26/src/usda/data_visualization/_graphic_drawing.py
--rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:52.000000 usda-0.0.26/src/usda/data_visualization/_image_process.py
--rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:40.000000 usda-0.0.26/src/usda/data_visualization/_img_feature_extraction.py
--rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:08.000000 usda-0.0.26/src/usda/data_visualization/_img_theme_color.py
--rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:26.000000 usda-0.0.26/src/usda/data_visualization/_imgs_layout_show.py
--rw-rw-rw-   0        0        0     4174 2023-03-15 02:00:20.000000 usda-0.0.26/src/usda/data_visualization/_imgs_show.py
--rw-rw-rw-   0        0        0      822 2022-11-02 06:07:16.000000 usda-0.0.26/src/usda/data_visualization/_knee_line_graph.py
--rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:54.000000 usda-0.0.26/src/usda/data_visualization/_moving_average_inflection.py
--rw-rw-rw-   0        0        0     3176 2023-02-24 07:31:40.000000 usda-0.0.26/src/usda/data_visualization/_panorama_show.py
--rw-rw-rw-   0        0        0     8051 2023-03-19 04:08:54.000000 usda-0.0.26/src/usda/data_visualization/_plot_single_function.py
--rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:42.000000 usda-0.0.26/src/usda/data_visualization/_raster_percentile_slider.py
--rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:14.000000 usda-0.0.26/src/usda/data_visualization/_raster_show.py
--rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:08.000000 usda-0.0.26/src/usda/data_visualization/_stats_charts.py
--rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:16.000000 usda-0.0.26/src/usda/data_visualization/_superpixel_segmentation_show.py
--rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:40.000000 usda-0.0.26/src/usda/data_visualization/_table_show.py
--rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:24.000000 usda-0.0.26/src/usda/data_visualization/_tile_show.py
--rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.26/src/usda/data_visualization/data_generator.py
--rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.26/src/usda/data_visualization/knee_locator.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.861749 usda-0.0.26/src/usda/database/
--rw-rw-rw-   0        0        0      839 2023-03-21 05:11:08.000000 usda-0.0.26/src/usda/database/__init__.py
--rw-rw-rw-   0        0        0      693 2022-10-30 12:15:42.000000 usda-0.0.26/src/usda/database/_data_file_rw.py
--rw-rw-rw-   0        0        0     4636 2023-03-21 05:10:02.000000 usda-0.0.26/src/usda/database/_data_format_conversion.py
--rw-rw-rw-   0        0        0     5605 2023-03-21 05:08:28.000000 usda-0.0.26/src/usda/database/_database.py
--rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:56.000000 usda-0.0.26/src/usda/database/_read_matlab_fig.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.871330 usda-0.0.26/src/usda/datasets/
--rw-rw-rw-   0        0        0     2575 2023-07-16 13:40:52.000000 usda-0.0.26/src/usda/datasets/__init__.py
--rw-rw-rw-   0        0        0    17136 2023-03-13 12:40:58.000000 usda-0.0.26/src/usda/datasets/_artificial_data.py
--rw-rw-rw-   0        0        0    19730 2023-03-14 01:14:46.000000 usda-0.0.26/src/usda/datasets/_base.py
--rw-rw-rw-   0        0        0     5186 2023-07-12 12:41:27.000000 usda-0.0.26/src/usda/datasets/_coordinate_transformation.py
--rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:20.000000 usda-0.0.26/src/usda/datasets/_dataset_info.py
--rw-rw-rw-   0        0        0     5119 2023-07-09 08:43:56.000000 usda-0.0.26/src/usda/datasets/_files_downloading.py
--rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:34.000000 usda-0.0.26/src/usda/datasets/_img_info.py
--rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:30.000000 usda-0.0.26/src/usda/datasets/_kml_info.py
--rw-rw-rw-   0        0        0     9014 2023-07-16 13:40:13.000000 usda-0.0.26/src/usda/datasets/_panorama_baidu_download.py
--rw-rw-rw-   0        0        0     8376 2023-07-14 01:16:17.000000 usda-0.0.26/src/usda/datasets/_poi_crawler.py
--rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:04.000000 usda-0.0.26/src/usda/datasets/_rs_image.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.880566 usda-0.0.26/src/usda/datasets/data/
--rw-rw-rw-   0        0        0      125 2022-08-21 07:11:22.000000 usda-0.0.26/src/usda/datasets/data/__init__.py
--rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:28.000000 usda-0.0.26/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0      950 2023-02-23 02:44:30.000000 usda-0.0.26/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
--rw-rw-rw-   0        0        0     8356 2023-03-13 12:16:38.000000 usda-0.0.26/src/usda/datasets/data/jisperveld_data.pickle
--rw-rw-rw-   0        0        0     1486 2023-02-27 14:21:30.000000 usda-0.0.26/src/usda/datasets/data/microclimate_in_office_rooms.pickle
--rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:56.000000 usda-0.0.26/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:58.000000 usda-0.0.26/src/usda/datasets/data/sales_data_cartoon_database.pickle
--rw-rw-rw-   0        0        0     1352 2023-02-24 07:53:40.000000 usda-0.0.26/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
--rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:20.000000 usda-0.0.26/src/usda/datasets/data/test_score_cartoon_statistic.pickle
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.881568 usda-0.0.26/src/usda/demo/
--rw-rw-rw-   0        0        0      247 2023-07-20 12:56:10.000000 usda-0.0.26/src/usda/demo/__init__.py
--rw-rw-rw-   0        0        0     1840 2023-07-20 12:55:58.000000 usda-0.0.26/src/usda/demo/_demo_isotonic_regression.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.892538 usda-0.0.26/src/usda/geodata_process/
--rw-rw-rw-   0        0        0     2010 2023-07-12 00:21:48.000000 usda-0.0.26/src/usda/geodata_process/__init__.py
--rw-rw-rw-   0        0        0     2906 2023-07-10 11:42:16.000000 usda-0.0.26/src/usda/geodata_process/_build_clipped_raster_dataset.py
--rw-rw-rw-   0        0        0     1197 2023-07-10 09:55:04.000000 usda-0.0.26/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py
--rw-rw-rw-   0        0        0     1872 2023-07-15 09:08:58.000000 usda-0.0.26/src/usda/geodata_process/_data_format_conversion.py
--rw-rw-rw-   0        0        0     6447 2023-07-10 00:45:08.000000 usda-0.0.26/src/usda/geodata_process/_quadrat.py
--rw-rw-rw-   0        0        0     6535 2023-03-22 16:40:24.000000 usda-0.0.26/src/usda/geodata_process/_raster_dataprocess.py
--rw-rw-rw-   0        0        0     6633 2023-03-22 14:50:34.000000 usda-0.0.26/src/usda/geodata_process/_raster_stats.py
--rw-rw-rw-   0        0        0     6661 2023-03-21 13:12:00.000000 usda-0.0.26/src/usda/geodata_process/_rasterize.py
--rw-rw-rw-   0        0        0     3093 2023-07-22 05:13:34.000000 usda-0.0.26/src/usda/geodata_process/_rio_tiler.py
--rw-rw-rw-   0        0        0     4952 2023-06-02 02:08:48.000000 usda-0.0.26/src/usda/geodata_process/_sample_pts.py
--rw-rw-rw-   0        0        0     1040 2023-04-17 23:16:56.000000 usda-0.0.26/src/usda/geodata_process/_shp_dataprocess.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.894565 usda-0.0.26/src/usda/imgs_process/
--rw-rw-rw-   0        0        0      457 2023-06-08 12:42:38.000000 usda-0.0.26/src/usda/imgs_process/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-06-08 12:45:28.000000 usda-0.0.26/src/usda/imgs_process/_imgs_process_basic.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.896528 usda-0.0.26/src/usda/indices/
--rw-rw-rw-   0        0        0      189 2022-10-26 06:14:58.000000 usda-0.0.26/src/usda/indices/__init__.py
--rw-rw-rw-   0        0        0      574 2022-10-26 06:15:30.000000 usda-0.0.26/src/usda/indices/_rs_indices.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.897525 usda-0.0.26/src/usda/manifold/
--rw-rw-rw-   0        0        0      349 2023-07-18 09:55:09.000000 usda-0.0.26/src/usda/manifold/__init__.py
--rw-rw-rw-   0        0        0     4131 2023-07-19 02:10:50.000000 usda-0.0.26/src/usda/manifold/_manifold_learning_illustration.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.901515 usda-0.0.26/src/usda/maths/
--rw-rw-rw-   0        0        0      645 2023-04-11 23:36:36.000000 usda-0.0.26/src/usda/maths/__init__.py
--rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:04.000000 usda-0.0.26/src/usda/maths/_algebra.py
--rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:20.000000 usda-0.0.26/src/usda/maths/_geometric_calculation.py
--rw-rw-rw-   0        0        0     8051 2023-04-11 23:36:08.000000 usda-0.0.26/src/usda/maths/_plot_single_function.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.914514 usda-0.0.26/src/usda/meta_heuristics/
--rw-rw-rw-   0        0        0      843 2023-03-19 01:33:30.000000 usda-0.0.26/src/usda/meta_heuristics/__init__.py
--rw-rw-rw-   0        0        0     5889 2023-03-18 13:00:34.000000 usda-0.0.26/src/usda/meta_heuristics/_cuckoo_s.py
--rw-rw-rw-   0        0        0     4919 2023-03-19 01:22:54.000000 usda-0.0.26/src/usda/meta_heuristics/_firefly_a.py
--rw-rw-rw-   0        0        0    11373 2023-03-10 03:50:44.000000 usda-0.0.26/src/usda/meta_heuristics/_ga.py
--rw-rw-rw-   0        0        0    13840 2023-03-15 22:13:02.000000 usda-0.0.26/src/usda/meta_heuristics/_ga_2d.py
--rw-rw-rw-   0        0        0    14213 2023-03-16 01:38:06.000000 usda-0.0.26/src/usda/meta_heuristics/_ga_2d_fixed_map.py
--rw-rw-rw-   0        0        0    15440 2023-03-15 14:33:58.000000 usda-0.0.26/src/usda/meta_heuristics/_ga_2d_testing_1.py
--rw-rw-rw-   0        0        0    25287 2023-03-17 02:56:08.000000 usda-0.0.26/src/usda/meta_heuristics/_ga_2d_testing_2.py
--rw-rw-rw-   0        0        0     4177 2023-03-10 02:05:30.000000 usda-0.0.26/src/usda/meta_heuristics/_ga_SegaranT.py
--rw-rw-rw-   0        0        0     7982 2023-03-01 00:42:28.000000 usda-0.0.26/src/usda/meta_heuristics/_gwo.py
--rw-rw-rw-   0        0        0     5251 2023-03-17 04:06:14.000000 usda-0.0.26/src/usda/meta_heuristics/_pso.py
--rw-rw-rw-   0        0        0     7564 2023-03-18 04:30:42.000000 usda-0.0.26/src/usda/meta_heuristics/_pso_2d.py
--rw-rw-rw-   0        0        0     8467 2023-03-18 05:15:56.000000 usda-0.0.26/src/usda/meta_heuristics/_pso_2d_testing.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.915511 usda-0.0.26/src/usda/migrated_project/
--rw-rw-rw-   0        0        0      216 2023-07-13 07:05:32.000000 usda-0.0.26/src/usda/migrated_project/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.915511 usda-0.0.26/src/usda/migrated_project/invest/
--rw-rw-rw-   0        0        0      711 2023-06-11 01:34:28.000000 usda-0.0.26/src/usda/migrated_project/invest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.924519 usda-0.0.26/src/usda/migrated_project/invest/configs/
--rw-rw-rw-   0        0        0     1150 2023-06-09 12:59:24.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-05-21 14:16:58.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/_carbon_configs.py
--rw-rw-rw-   0        0        0     5303 2023-05-22 07:01:14.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py
--rw-rw-rw-   0        0        0     2352 2023-05-22 09:31:34.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py
--rw-rw-rw-   0        0        0     3674 2023-05-22 08:55:40.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py
--rw-rw-rw-   0        0        0      490 2023-05-21 18:26:42.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/_habitat_quality_configs.py
--rw-rw-rw-   0        0        0      117 2023-06-09 13:00:22.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/_urban_cooling_configs.py
--rw-rw-rw-   0        0        0     2095 2023-04-29 10:05:58.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv
--rw-rw-rw-   0        0        0     1684 2023-05-16 20:54:58.000000 usda-0.0.26/src/usda/migrated_project/invest/configs/unit_definitions.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.933840 usda-0.0.26/src/usda/migrated_project/invest/esv/
--rw-rw-rw-   0        0        0      700 2023-06-09 23:15:34.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/__init__.py
--rw-rw-rw-   0        0        0    23442 2023-05-31 01:40:44.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_carbon.py
--rw-rw-rw-   0        0        0    66377 2023-05-22 12:57:04.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_crop_pollination.py
--rw-rw-rw-   0        0        0    37499 2023-05-22 10:16:22.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_crop_production_percentile.py
--rw-rw-rw-   0        0        0    43341 2023-05-22 13:20:46.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_crop_production_regression.py
--rw-rw-rw-   0        0        0    41477 2023-05-22 12:35:32.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_habitat_quality.py
--rw-rw-rw-   0        0        0      610 2023-05-21 04:07:42.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_unit_registry.py
--rw-rw-rw-   0        0        0    56182 2023-06-10 02:41:06.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_urban_cooling_model.py
--rw-rw-rw-   0        0        0    44236 2023-05-21 14:00:32.000000 usda-0.0.26/src/usda/migrated_project/invest/esv/_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.938851 usda-0.0.26/src/usda/migrated_project/pass_panoseg/
--rw-rw-rw-   0        0        0      201 2023-07-13 09:09:37.000000 usda-0.0.26/src/usda/migrated_project/pass_panoseg/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-07-13 08:45:47.000000 usda-0.0.26/src/usda/migrated_project/pass_panoseg/_dataset.py
--rw-rw-rw-   0        0        0     5566 2023-07-13 07:08:21.000000 usda-0.0.26/src/usda/migrated_project/pass_panoseg/_erfnet_pspnet.py
--rw-rw-rw-   0        0        0     3370 2023-07-14 05:43:09.000000 usda-0.0.26/src/usda/migrated_project/pass_panoseg/_semantic_seg.py
--rw-rw-rw-   0        0        0     2896 2020-01-18 16:35:00.000000 usda-0.0.26/src/usda/migrated_project/pass_panoseg/_transform.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.943842 usda-0.0.26/src/usda/migrated_project/pix2pix/
--rw-rw-rw-   0        0        0     1969 2023-04-20 08:47:18.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/A2B.py
--rw-rw-rw-   0        0        0      217 2023-04-21 13:54:28.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.951439 usda-0.0.26/src/usda/migrated_project/pix2pix/data/
--rw-rw-rw-   0        0        0     4100 2023-04-20 05:37:12.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-17 06:17:14.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py
--rw-rw-rw-   0        0        0     6235 2023-04-17 05:52:32.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/_base_dataset.py
--rw-rw-rw-   0        0        0     2897 2023-04-17 06:22:00.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py
--rw-rw-rw-   0        0        0     1885 2023-03-14 20:28:50.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/_image_folder.py
--rw-rw-rw-   0        0        0     1658 2023-04-17 06:20:00.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/_single_dataset.py
--rw-rw-rw-   0        0        0     3589 2023-04-17 03:48:22.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/_template_dataset.py
--rw-rw-rw-   0        0        0     3526 2023-04-17 05:45:04.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.952426 usda-0.0.26/src/usda/migrated_project/pix2pix/datasets/
--rw-rw-rw-   0        0        0      198 2023-04-17 01:54:38.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.954423 usda-0.0.26/src/usda/migrated_project/pix2pix/imgs/
--rw-rw-rw-   0        0        0      127 2023-04-21 13:57:20.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/imgs/__init__.py
--rw-rw-rw-   0        0        0    14064 2023-04-21 14:08:06.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/imgs/example.jpg
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.960373 usda-0.0.26/src/usda/migrated_project/pix2pix/models/
--rw-rw-rw-   0        0        0     3349 2023-04-20 02:44:46.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/models/__init__.py
--rw-rw-rw-   0        0        0    10810 2023-04-17 07:20:12.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/models/_base_model.py
--rw-rw-rw-   0        0        0    29098 2023-04-17 07:31:08.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/models/_networks.py
--rw-rw-rw-   0        0        0     7024 2023-04-17 07:21:12.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py
--rw-rw-rw-   0        0        0     3392 2023-04-17 12:08:32.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/models/_test_model.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.964363 usda-0.0.26/src/usda/migrated_project/pix2pix/options/
--rw-rw-rw-   0        0        0      425 2023-04-17 11:42:48.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/options/__init__.py
--rw-rw-rw-   0        0        0     3447 2023-04-17 08:10:08.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/options/_base_options.py
--rw-rw-rw-   0        0        0     1045 2023-04-17 12:42:34.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/options/_test_options.py
--rw-rw-rw-   0        0        0     2533 2023-04-17 11:39:46.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/options/_train_options.py
--rw-rw-rw-   0        0        0     8846 2023-04-22 00:58:20.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/sketch_A2B.py
--rw-rw-rw-   0        0        0     6019 2023-04-17 13:04:36.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/test.py
--rw-rw-rw-   0        0        0     6788 2023-04-18 09:54:16.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/train.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.970347 usda-0.0.26/src/usda/migrated_project/pix2pix/util/
--rw-rw-rw-   0        0        0      270 2023-04-17 11:51:20.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/util/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-03-14 20:28:50.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/util/_get_data.py
--rw-rw-rw-   0        0        0     3223 2023-03-14 20:28:50.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/util/_html.py
--rw-rw-rw-   0        0        0     2226 2023-03-14 20:28:50.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/util/_image_pool.py
--rw-rw-rw-   0        0        0     3175 2023-03-14 20:28:50.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/util/_util.py
--rw-rw-rw-   0        0        0    12408 2023-04-17 09:41:46.000000 usda-0.0.26/src/usda/migrated_project/pix2pix/util/_visualizer.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.978356 usda-0.0.26/src/usda/migrated_project/stylegan/
--rw-rw-rw-   0        0        0      898 2023-04-17 10:27:42.000000 usda-0.0.26/src/usda/migrated_project/stylegan/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-04-16 06:09:10.000000 usda-0.0.26/src/usda/migrated_project/stylegan/_config.py
--rw-rw-rw-   0        0        0     4425 2023-04-11 12:13:44.000000 usda-0.0.26/src/usda/migrated_project/stylegan/_convert.py
--rw-rw-rw-   0        0        0     3527 2023-04-11 12:16:26.000000 usda-0.0.26/src/usda/migrated_project/stylegan/_generate_grid.py
--rw-rw-rw-   0        0        0     5616 2023-04-16 11:14:58.000000 usda-0.0.26/src/usda/migrated_project/stylegan/_generate_mixing_figure.py
--rw-rw-rw-   0        0        0     4595 2023-04-16 07:34:50.000000 usda-0.0.26/src/usda/migrated_project/stylegan/_generate_samples.py
--rw-rw-rw-   0        0        0     3430 2023-04-16 08:58:06.000000 usda-0.0.26/src/usda/migrated_project/stylegan/_generate_truncation_figure.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.982313 usda-0.0.26/src/usda/migrated_project/stylegan/data/
--rw-rw-rw-   0        0        0      558 2023-04-11 11:18:12.000000 usda-0.0.26/src/usda/migrated_project/stylegan/data/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-04-11 10:36:08.000000 usda-0.0.26/src/usda/migrated_project/stylegan/data/_datasets.py
--rw-rw-rw-   0        0        0     1457 2023-04-11 10:36:56.000000 usda-0.0.26/src/usda/migrated_project/stylegan/data/_make_dataset.py
--rw-rw-rw-   0        0        0     1014 2023-04-11 10:37:16.000000 usda-0.0.26/src/usda/migrated_project/stylegan/data/_transforms.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.984340 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/
--rw-rw-rw-   0        0        0      799 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.987300 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/submission/
--rw-rw-rw-   0        0        0      392 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/submission/__init__.py
--rw-rw-rw-   0        0        0     4337 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py
--rw-rw-rw-   0        0        0    11131 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.992288 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/
--rw-rw-rw-   0        0        0      524 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py
--rw-rw-rw-   0        0        0     7537 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py
--rw-rw-rw-   0        0        0    30121 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py
--rw-rw-rw-   0        0        0    10027 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py
--rw-rw-rw-   0        0        0     9306 2023-04-11 12:36:20.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py
--rw-rw-rw-   0        0        0    13756 2021-12-18 03:07:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/util.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.994314 usda-0.0.26/src/usda/migrated_project/stylegan/extracted_funcs/
--rw-rw-rw-   0        0        0      186 2023-04-12 06:22:04.000000 usda-0.0.26/src/usda/migrated_project/stylegan/extracted_funcs/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-04-12 06:27:24.000000 usda-0.0.26/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.000266 usda-0.0.26/src/usda/migrated_project/stylegan/models/
--rw-rw-rw-   0        0        0     6331 2023-04-11 11:53:58.000000 usda-0.0.26/src/usda/migrated_project/stylegan/models/_Blocks.py
--rw-rw-rw-   0        0        0    11748 2023-04-11 11:32:54.000000 usda-0.0.26/src/usda/migrated_project/stylegan/models/_CustomLayers.py
--rw-rw-rw-   0        0        0    38792 2023-04-11 11:52:56.000000 usda-0.0.26/src/usda/migrated_project/stylegan/models/_GAN.py
--rw-rw-rw-   0        0        0     8277 2023-04-11 11:27:24.000000 usda-0.0.26/src/usda/migrated_project/stylegan/models/_Losses.py
--rw-rw-rw-   0        0        0     1771 2023-04-11 11:56:28.000000 usda-0.0.26/src/usda/migrated_project/stylegan/models/__init__.py
--rw-rw-rw-   0        0        0     1388 2023-04-11 11:40:44.000000 usda-0.0.26/src/usda/migrated_project/stylegan/models/_update_average.py
--rw-rw-rw-   0        0        0     6150 2023-04-17 03:27:44.000000 usda-0.0.26/src/usda/migrated_project/stylegan/train.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.002261 usda-0.0.26/src/usda/migrated_project/stylegan/utils/
--rw-rw-rw-   0        0        0      247 2023-04-11 07:34:42.000000 usda-0.0.26/src/usda/migrated_project/stylegan/utils/__init__.py
--rw-rw-rw-   0        0        0     2159 2023-04-11 09:44:26.000000 usda-0.0.26/src/usda/migrated_project/stylegan/utils/_copy.py
--rw-rw-rw-   0        0        0      685 2023-04-11 10:33:58.000000 usda-0.0.26/src/usda/migrated_project/stylegan/utils/_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.009168 usda-0.0.26/src/usda/models/
--rw-rw-rw-   0        0        0     5522 2023-07-16 09:52:51.000000 usda-0.0.26/src/usda/models/__init__.py
--rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:20.000000 usda-0.0.26/src/usda/models/_bow_feature_builder.py
--rw-rw-rw-   0        0        0     1014 2023-03-24 02:28:50.000000 usda-0.0.26/src/usda/models/_clustering.py
--rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:32.000000 usda-0.0.26/src/usda/models/_computational_performance.py
--rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:10.000000 usda-0.0.26/src/usda/models/_curve_segmentation.py
--rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:06.000000 usda-0.0.26/src/usda/models/_decision_tree.py
--rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:42.000000 usda-0.0.26/src/usda/models/_dim1_convolution.py
--rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:50.000000 usda-0.0.26/src/usda/models/_entropy.py
--rw-rw-rw-   0        0        0     1458 2023-03-24 10:49:06.000000 usda-0.0.26/src/usda/models/_global_local_autocorrelation.py
--rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:06.000000 usda-0.0.26/src/usda/models/_image_tag_extractor.py
--rw-rw-rw-   0        0        0     2087 2023-06-21 23:53:50.000000 usda-0.0.26/src/usda/models/_label_encoder.py
--rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:58.000000 usda-0.0.26/src/usda/models/_neighbors.py
--rw-rw-rw-   0        0        0     9967 2023-06-30 10:21:04.000000 usda-0.0.26/src/usda/models/_nlp_tools.py
--rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:26.000000 usda-0.0.26/src/usda/models/_random_forest_classifier.py
--rw-rw-rw-   0        0        0    13684 2023-07-16 09:52:28.000000 usda-0.0.26/src/usda/models/_rnn_lstm.py
--rw-rw-rw-   0        0        0    16007 2023-06-30 12:22:04.000000 usda-0.0.26/src/usda/models/_seq2seq.py
--rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:46.000000 usda-0.0.26/src/usda/models/_sir_model.py
--rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:06.000000 usda-0.0.26/src/usda/models/_superpixel_segmentation.py
--rw-rw-rw-   0        0        0     9756 2023-07-01 03:01:18.000000 usda-0.0.26/src/usda/models/_transformer.py
--rw-rw-rw-   0        0        0     8564 2023-07-11 03:52:38.000000 usda-0.0.26/src/usda/models/_vit.py
--rw-rw-rw-   0        0        0     9313 2023-06-27 08:00:24.000000 usda-0.0.26/src/usda/models/_word2vec_sgns.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.025010 usda-0.0.26/src/usda/net/
--rw-rw-rw-   0        0        0      120 2023-04-05 02:07:50.000000 usda-0.0.26/src/usda/net/_.py
--rw-rw-rw-   0        0        0      856 2023-04-05 02:18:10.000000 usda-0.0.26/src/usda/net/__init__.py
--rw-rw-rw-   0        0        0    28490 2023-04-05 02:16:40.000000 usda-0.0.26/src/usda/net/_networks_pix2pix.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.028511 usda-0.0.26/src/usda/network/
--rw-rw-rw-   0        0        0      404 2023-04-01 07:37:22.000000 usda-0.0.26/src/usda/network/__init__.py
--rw-rw-rw-   0        0        0     4050 2023-03-10 11:37:14.000000 usda-0.0.26/src/usda/network/_g_drawing.py
--rw-rw-rw-   0        0        0     2896 2023-04-01 07:46:52.000000 usda-0.0.26/src/usda/network/_pt_pattern.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.043476 usda-0.0.26/src/usda/pano_projection_transformation/
--rw-rw-rw-   0        0        0    10333 2023-07-15 05:00:44.000000 usda-0.0.26/src/usda/pano_projection_transformation/_Key_point_size_metrics.py
--rw-rw-rw-   0        0        0    12906 2023-07-15 10:24:02.000000 usda-0.0.26/src/usda/pano_projection_transformation/_POI_street_feature.py
--rw-rw-rw-   0        0        0     2641 2023-07-15 09:26:19.000000 usda-0.0.26/src/usda/pano_projection_transformation/__init__.py
--rw-rw-rw-   0        0        0     4689 2023-07-15 01:49:23.000000 usda-0.0.26/src/usda/pano_projection_transformation/_color_metrics.py
--rw-rw-rw-   0        0        0     8920 2023-07-15 01:22:29.000000 usda-0.0.26/src/usda/pano_projection_transformation/_color_metrics_pool.py
--rw-rw-rw-   0        0        0     1461 2023-07-14 07:12:51.000000 usda-0.0.26/src/usda/pano_projection_transformation/_equi2cube.py
--rw-rw-rw-   0        0        0    12692 2023-07-14 07:28:14.000000 usda-0.0.26/src/usda/pano_projection_transformation/_equi2cube_pool.py
--rw-rw-rw-   0        0        0     1253 2023-07-14 10:05:43.000000 usda-0.0.26/src/usda/pano_projection_transformation/_equi2polar.py
--rw-rw-rw-   0        0        0     6805 2023-07-14 10:12:49.000000 usda-0.0.26/src/usda/pano_projection_transformation/_equi2polar_pool.py
--rw-rw-rw-   0        0        0    19002 2023-07-15 05:27:17.000000 usda-0.0.26/src/usda/pano_projection_transformation/_imgs_arranging.py
--rw-rw-rw-   0        0        0    26655 2023-07-15 08:41:15.000000 usda-0.0.26/src/usda/pano_projection_transformation/_metric_clustering.py
--rw-rw-rw-   0        0        0     2335 2023-07-15 06:43:18.000000 usda-0.0.26/src/usda/pano_projection_transformation/_metrics_clustering_pool.py
--rw-rw-rw-   0        0        0     5662 2023-07-15 01:05:08.000000 usda-0.0.26/src/usda/pano_projection_transformation/_skyline_shape_metrics.py
--rw-rw-rw-   0        0        0     3541 2023-07-14 11:58:36.000000 usda-0.0.26/src/usda/pano_projection_transformation/_spherical_panorama.py
--rw-rw-rw-   0        0        0     6815 2023-07-14 13:09:54.000000 usda-0.0.26/src/usda/pano_projection_transformation/_visual_field_proportion_metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.050457 usda-0.0.26/src/usda/pattern_signature/
--rw-rw-rw-   0        0        0     1340 2023-03-24 06:18:08.000000 usda-0.0.26/src/usda/pattern_signature/__init__.py
--rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:52.000000 usda-0.0.26/src/usda/pattern_signature/_distance_metric.py
--rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:18.000000 usda-0.0.26/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
--rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:30.000000 usda-0.0.26/src/usda/pattern_signature/_img_region_growing.py
--rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:58.000000 usda-0.0.26/src/usda/pattern_signature/_pattern_module.py
--rw-rw-rw-   0        0        0     7729 2023-03-24 07:51:32.000000 usda-0.0.26/src/usda/pattern_signature/_signature.py
--rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:50.000000 usda-0.0.26/src/usda/pattern_signature/_signature2distance_integration.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.059431 usda-0.0.26/src/usda/pgm/
--rw-rw-rw-   0        0        0     3024 2023-06-08 14:28:50.000000 usda-0.0.26/src/usda/pgm/_MRF.py
--rw-rw-rw-   0        0        0     6429 2023-06-12 05:30:16.000000 usda-0.0.26/src/usda/pgm/_MRF_urban_cooling.py
--rw-rw-rw-   0        0        0     1374 2023-06-10 12:20:50.000000 usda-0.0.26/src/usda/pgm/__init__.py
--rw-rw-rw-   0        0        0     4688 2023-06-09 02:45:58.000000 usda-0.0.26/src/usda/pgm/_image_segmentation_using_mrf.py
--rw-rw-rw-   0        0        0     3817 2023-06-02 07:46:24.000000 usda-0.0.26/src/usda/pgm/_pgm_calculating.py
--rw-rw-rw-   0        0        0      372 2023-05-11 01:14:46.000000 usda-0.0.26/src/usda/pgm/_pgm_conversion.py
--rw-rw-rw-   0        0        0     4763 2023-06-08 02:43:38.000000 usda-0.0.26/src/usda/pgm/_pgm_draw.py
--rw-rw-rw-   0        0        0     1292 2023-05-15 12:25:46.000000 usda-0.0.26/src/usda/pgm/_probability_theory.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.064452 usda-0.0.26/src/usda/stats/
--rw-rw-rw-   0        0        0     1045 2023-05-02 13:19:48.000000 usda-0.0.26/src/usda/stats/__init__.py
--rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:20.000000 usda-0.0.26/src/usda/stats/_descriptive_stats.py
--rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:58.000000 usda-0.0.26/src/usda/stats/_kde.py
--rw-rw-rw-   0        0        0      778 2022-10-20 03:57:20.000000 usda-0.0.26/src/usda/stats/_outlier.py
--rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:30.000000 usda-0.0.26/src/usda/stats/_regression.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.065448 usda-0.0.26/src/usda/tools/
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.070434 usda-0.0.26/src/usda/tools/DL_layers_visualizer/
--rw-rw-rw-   0        0        0     4066 2023-03-29 04:55:12.000000 usda-0.0.26/src/usda/tools/DL_layers_visualizer/0_72.jpg
--rw-rw-rw-   0        0        0    13876 2023-03-29 04:55:12.000000 usda-0.0.26/src/usda/tools/DL_layers_visualizer/0_8.jpg
--rw-rw-rw-   0        0        0     3757 2023-03-29 04:55:14.000000 usda-0.0.26/src/usda/tools/DL_layers_visualizer/0_9.jpg
--rw-rw-rw-   0        0        0     1064 2023-04-08 15:24:38.000000 usda-0.0.26/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
--rw-rw-rw-   0        0        0      199 2023-04-09 05:39:16.000000 usda-0.0.26/src/usda/tools/DL_layers_visualizer/__init__.py
--rw-rw-rw-   0        0        0      232 2023-04-09 05:40:00.000000 usda-0.0.26/src/usda/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.079491 usda-0.0.26/src/usda/utils/
--rw-rw-rw-   0        0        0     1396 2023-07-16 08:13:41.000000 usda-0.0.26/src/usda/utils/__init__.py
--rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:34.000000 usda-0.0.26/src/usda/utils/_bunch.py
--rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:28.000000 usda-0.0.26/src/usda/utils/_coordinate_transformation.py
--rw-rw-rw-   0        0        0     3970 2023-02-23 09:40:48.000000 usda-0.0.26/src/usda/utils/_df_process.py
--rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:18.000000 usda-0.0.26/src/usda/utils/_displayable_path.py
--rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:32.000000 usda-0.0.26/src/usda/utils/_file_structure.py
--rw-rw-rw-   0        0        0     5812 2023-07-16 11:18:22.000000 usda-0.0.26/src/usda/utils/_gadgets.py
--rw-rw-rw-   0        0        0      606 2022-10-22 00:35:58.000000 usda-0.0.26/src/usda/utils/_operating_time.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:06.082490 usda-0.0.26/src/usda/weight/
--rw-rw-rw-   0        0        0     1014 2023-03-03 07:14:30.000000 usda-0.0.26/src/usda/weight/__init__.py
--rw-rw-rw-   0        0        0    38486 2023-03-03 07:13:36.000000 usda-0.0.26/src/usda/weight/_decision_rule.py
--rw-rw-rw-   0        0        0     2745 2023-02-23 12:30:36.000000 usda-0.0.26/src/usda/weight/_entropy_weight.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:16:05.821988 usda-0.0.26/src/usda.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-07-22 05:16:05.000000 usda-0.0.26/src/usda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12628 2023-07-22 05:16:05.000000 usda-0.0.26/src/usda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 05:16:05.000000 usda-0.0.26/src/usda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-16 07:33:52.000000 usda-0.0.26/src/usda.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-07-22 05:16:05.000000 usda-0.0.26/src/usda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-22 05:16:05.000000 usda-0.0.26/src/usda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.817611 usda-0.0.27/
+-rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:46.000000 usda-0.0.27/LICENSE
+-rw-rw-rw-   0        0        0     1563 2023-08-05 13:38:44.816614 usda-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2022-10-24 05:51:50.000000 usda-0.0.27/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-05 13:38:44.817611 usda-0.0.27/setup.cfg
+-rw-rw-rw-   0        0        0     4305 2023-05-21 04:03:08.000000 usda-0.0.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:43.990823 usda-0.0.27/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.015576 usda-0.0.27/src/usda/
+-rw-rw-rw-   0        0        0      636 2023-08-05 13:38:16.000000 usda-0.0.27/src/usda/__init__.py
+-rw-rw-rw-   0        0        0      731 2022-10-16 01:25:30.000000 usda-0.0.27/src/usda/_min_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.045520 usda-0.0.27/src/usda/data_process/
+-rw-rw-rw-   0        0        0     1147 2023-03-26 03:42:06.000000 usda-0.0.27/src/usda/data_process/__init__.py
+-rw-rw-rw-   0        0        0     2125 2022-10-22 01:49:00.000000 usda-0.0.27/src/usda/data_process/_geoinfodata_conversion.py
+-rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:52.000000 usda-0.0.27/src/usda/data_process/_image_pixel_sampling_zoom.py
+-rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:58.000000 usda-0.0.27/src/usda/data_process/_kitti_dataprocess.py
+-rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:20.000000 usda-0.0.27/src/usda/data_process/_landsat_dataprocess.py
+-rw-rw-rw-   0        0        0     1854 2023-03-26 07:52:40.000000 usda-0.0.27/src/usda/data_process/_naip_dataprocess.py
+-rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:40.000000 usda-0.0.27/src/usda/data_process/_osm_dataprocess.py
+-rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:32.000000 usda-0.0.27/src/usda/data_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:56.000000 usda-0.0.27/src/usda/data_process/_tiler_calculation.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.056555 usda-0.0.27/src/usda/data_visual/
+-rw-rw-rw-   0        0        0      434 2023-07-25 10:22:38.000000 usda-0.0.27/src/usda/data_visual/__init__.py
+-rw-rw-rw-   0        0        0     3737 2023-07-25 10:36:16.000000 usda-0.0.27/src/usda/data_visual/_colors.py
+-rw-rw-rw-   0        0        0      771 2023-07-24 10:24:40.000000 usda-0.0.27/src/usda/data_visual/_plot_style.py
+-rw-rw-rw-   0        0        0     1362 2023-07-09 12:16:32.000000 usda-0.0.27/src/usda/data_visual/_worldcover_plot_style.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.123962 usda-0.0.27/src/usda/data_visualization/
+-rw-rw-rw-   0        0        0     3205 2023-05-30 14:40:54.000000 usda-0.0.27/src/usda/data_visualization/__init__.py
+-rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:26.000000 usda-0.0.27/src/usda/data_visualization/_chart_custom.py
+-rw-rw-rw-   0        0        0     3729 2023-05-30 14:40:36.000000 usda-0.0.27/src/usda/data_visualization/_colors.py
+-rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:08.000000 usda-0.0.27/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
+-rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:52.000000 usda-0.0.27/src/usda/data_visualization/_gdf_plot.py
+-rw-rw-rw-   0        0        0      952 2022-10-28 11:19:34.000000 usda-0.0.27/src/usda/data_visualization/_gif_show.py
+-rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:46.000000 usda-0.0.27/src/usda/data_visualization/_graphic_drawing.py
+-rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:52.000000 usda-0.0.27/src/usda/data_visualization/_image_process.py
+-rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:40.000000 usda-0.0.27/src/usda/data_visualization/_img_feature_extraction.py
+-rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:08.000000 usda-0.0.27/src/usda/data_visualization/_img_theme_color.py
+-rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:26.000000 usda-0.0.27/src/usda/data_visualization/_imgs_layout_show.py
+-rw-rw-rw-   0        0        0     4174 2023-03-15 02:00:20.000000 usda-0.0.27/src/usda/data_visualization/_imgs_show.py
+-rw-rw-rw-   0        0        0      822 2022-11-02 06:07:16.000000 usda-0.0.27/src/usda/data_visualization/_knee_line_graph.py
+-rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:54.000000 usda-0.0.27/src/usda/data_visualization/_moving_average_inflection.py
+-rw-rw-rw-   0        0        0     3176 2023-02-24 07:31:40.000000 usda-0.0.27/src/usda/data_visualization/_panorama_show.py
+-rw-rw-rw-   0        0        0     8051 2023-03-19 04:08:54.000000 usda-0.0.27/src/usda/data_visualization/_plot_single_function.py
+-rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:42.000000 usda-0.0.27/src/usda/data_visualization/_raster_percentile_slider.py
+-rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:14.000000 usda-0.0.27/src/usda/data_visualization/_raster_show.py
+-rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:08.000000 usda-0.0.27/src/usda/data_visualization/_stats_charts.py
+-rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:16.000000 usda-0.0.27/src/usda/data_visualization/_superpixel_segmentation_show.py
+-rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:40.000000 usda-0.0.27/src/usda/data_visualization/_table_show.py
+-rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:24.000000 usda-0.0.27/src/usda/data_visualization/_tile_show.py
+-rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.27/src/usda/data_visualization/data_generator.py
+-rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.27/src/usda/data_visualization/knee_locator.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.137564 usda-0.0.27/src/usda/database/
+-rw-rw-rw-   0        0        0      839 2023-03-21 05:11:08.000000 usda-0.0.27/src/usda/database/__init__.py
+-rw-rw-rw-   0        0        0      693 2022-10-30 12:15:42.000000 usda-0.0.27/src/usda/database/_data_file_rw.py
+-rw-rw-rw-   0        0        0     4636 2023-03-21 05:10:02.000000 usda-0.0.27/src/usda/database/_data_format_conversion.py
+-rw-rw-rw-   0        0        0     5605 2023-03-21 05:08:28.000000 usda-0.0.27/src/usda/database/_database.py
+-rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:56.000000 usda-0.0.27/src/usda/database/_read_matlab_fig.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.169786 usda-0.0.27/src/usda/datasets/
+-rw-rw-rw-   0        0        0     2575 2023-07-16 13:40:52.000000 usda-0.0.27/src/usda/datasets/__init__.py
+-rw-rw-rw-   0        0        0    17136 2023-03-13 12:40:58.000000 usda-0.0.27/src/usda/datasets/_artificial_data.py
+-rw-rw-rw-   0        0        0    19730 2023-03-14 01:14:46.000000 usda-0.0.27/src/usda/datasets/_base.py
+-rw-rw-rw-   0        0        0     5186 2023-07-12 12:41:27.000000 usda-0.0.27/src/usda/datasets/_coordinate_transformation.py
+-rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:20.000000 usda-0.0.27/src/usda/datasets/_dataset_info.py
+-rw-rw-rw-   0        0        0     5119 2023-07-09 08:43:56.000000 usda-0.0.27/src/usda/datasets/_files_downloading.py
+-rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:34.000000 usda-0.0.27/src/usda/datasets/_img_info.py
+-rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:30.000000 usda-0.0.27/src/usda/datasets/_kml_info.py
+-rw-rw-rw-   0        0        0     9014 2023-07-16 13:40:13.000000 usda-0.0.27/src/usda/datasets/_panorama_baidu_download.py
+-rw-rw-rw-   0        0        0     8376 2023-07-14 01:16:17.000000 usda-0.0.27/src/usda/datasets/_poi_crawler.py
+-rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:04.000000 usda-0.0.27/src/usda/datasets/_rs_image.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.193357 usda-0.0.27/src/usda/datasets/data/
+-rw-rw-rw-   0        0        0      125 2022-08-21 07:11:22.000000 usda-0.0.27/src/usda/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:28.000000 usda-0.0.27/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0      950 2023-02-23 02:44:30.000000 usda-0.0.27/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
+-rw-rw-rw-   0        0        0     8356 2023-03-13 12:16:38.000000 usda-0.0.27/src/usda/datasets/data/jisperveld_data.pickle
+-rw-rw-rw-   0        0        0     1486 2023-02-27 14:21:30.000000 usda-0.0.27/src/usda/datasets/data/microclimate_in_office_rooms.pickle
+-rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:56.000000 usda-0.0.27/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:58.000000 usda-0.0.27/src/usda/datasets/data/sales_data_cartoon_database.pickle
+-rw-rw-rw-   0        0        0     1352 2023-02-24 07:53:40.000000 usda-0.0.27/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
+-rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:20.000000 usda-0.0.27/src/usda/datasets/data/test_score_cartoon_statistic.pickle
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.197199 usda-0.0.27/src/usda/demo/
+-rw-rw-rw-   0        0        0      631 2023-07-26 09:05:12.000000 usda-0.0.27/src/usda/demo/__init__.py
+-rw-rw-rw-   0        0        0    16814 2023-07-26 09:14:15.000000 usda-0.0.27/src/usda/demo/_demo_misc.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.224185 usda-0.0.27/src/usda/geodata_process/
+-rw-rw-rw-   0        0        0     2306 2023-08-02 02:04:25.000000 usda-0.0.27/src/usda/geodata_process/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-07-10 11:42:16.000000 usda-0.0.27/src/usda/geodata_process/_build_clipped_raster_dataset.py
+-rw-rw-rw-   0        0        0     1197 2023-07-10 09:55:04.000000 usda-0.0.27/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py
+-rw-rw-rw-   0        0        0     1872 2023-07-15 09:08:58.000000 usda-0.0.27/src/usda/geodata_process/_data_format_conversion.py
+-rw-rw-rw-   0        0        0     3148 2023-08-02 02:13:21.000000 usda-0.0.27/src/usda/geodata_process/_overlapping_polygons.py
+-rw-rw-rw-   0        0        0     6447 2023-07-10 00:45:08.000000 usda-0.0.27/src/usda/geodata_process/_quadrat.py
+-rw-rw-rw-   0        0        0     6535 2023-03-22 16:40:24.000000 usda-0.0.27/src/usda/geodata_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     6633 2023-03-22 14:50:34.000000 usda-0.0.27/src/usda/geodata_process/_raster_stats.py
+-rw-rw-rw-   0        0        0     6661 2023-03-21 13:12:00.000000 usda-0.0.27/src/usda/geodata_process/_rasterize.py
+-rw-rw-rw-   0        0        0     3095 2023-08-01 13:31:20.000000 usda-0.0.27/src/usda/geodata_process/_rio_tiler.py
+-rw-rw-rw-   0        0        0     4952 2023-06-02 02:08:48.000000 usda-0.0.27/src/usda/geodata_process/_sample_pts.py
+-rw-rw-rw-   0        0        0     1040 2023-04-17 23:16:56.000000 usda-0.0.27/src/usda/geodata_process/_shp_dataprocess.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.228539 usda-0.0.27/src/usda/imgs_process/
+-rw-rw-rw-   0        0        0      457 2023-06-08 12:42:38.000000 usda-0.0.27/src/usda/imgs_process/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-06-08 12:45:28.000000 usda-0.0.27/src/usda/imgs_process/_imgs_process_basic.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.233528 usda-0.0.27/src/usda/indices/
+-rw-rw-rw-   0        0        0      189 2022-10-26 06:14:58.000000 usda-0.0.27/src/usda/indices/__init__.py
+-rw-rw-rw-   0        0        0      574 2022-10-26 06:15:30.000000 usda-0.0.27/src/usda/indices/_rs_indices.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.246658 usda-0.0.27/src/usda/manifold/
+-rw-rw-rw-   0        0        0      689 2023-07-28 05:21:21.000000 usda-0.0.27/src/usda/manifold/__init__.py
+-rw-rw-rw-   0        0        0     3226 2023-07-27 08:50:38.000000 usda-0.0.27/src/usda/manifold/_correlations_embedding.py
+-rw-rw-rw-   0        0        0     4131 2023-07-19 02:10:50.000000 usda-0.0.27/src/usda/manifold/_manifold_learning_illustration.py
+-rw-rw-rw-   0        0        0     1919 2023-07-24 07:30:58.000000 usda-0.0.27/src/usda/manifold/_rbf_kernel_pca.py
+-rw-rw-rw-   0        0        0     6599 2023-07-28 06:13:42.000000 usda-0.0.27/src/usda/manifold/_tsne.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.261585 usda-0.0.27/src/usda/maths/
+-rw-rw-rw-   0        0        0      645 2023-04-11 23:36:36.000000 usda-0.0.27/src/usda/maths/__init__.py
+-rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:04.000000 usda-0.0.27/src/usda/maths/_algebra.py
+-rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:20.000000 usda-0.0.27/src/usda/maths/_geometric_calculation.py
+-rw-rw-rw-   0        0        0     8051 2023-04-11 23:36:08.000000 usda-0.0.27/src/usda/maths/_plot_single_function.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.310956 usda-0.0.27/src/usda/meta_heuristics/
+-rw-rw-rw-   0        0        0      843 2023-03-19 01:33:30.000000 usda-0.0.27/src/usda/meta_heuristics/__init__.py
+-rw-rw-rw-   0        0        0     5889 2023-03-18 13:00:34.000000 usda-0.0.27/src/usda/meta_heuristics/_cuckoo_s.py
+-rw-rw-rw-   0        0        0     4919 2023-03-19 01:22:54.000000 usda-0.0.27/src/usda/meta_heuristics/_firefly_a.py
+-rw-rw-rw-   0        0        0    11373 2023-03-10 03:50:44.000000 usda-0.0.27/src/usda/meta_heuristics/_ga.py
+-rw-rw-rw-   0        0        0    13840 2023-03-15 22:13:02.000000 usda-0.0.27/src/usda/meta_heuristics/_ga_2d.py
+-rw-rw-rw-   0        0        0    14213 2023-03-16 01:38:06.000000 usda-0.0.27/src/usda/meta_heuristics/_ga_2d_fixed_map.py
+-rw-rw-rw-   0        0        0    15440 2023-03-15 14:33:58.000000 usda-0.0.27/src/usda/meta_heuristics/_ga_2d_testing_1.py
+-rw-rw-rw-   0        0        0    25287 2023-03-17 02:56:08.000000 usda-0.0.27/src/usda/meta_heuristics/_ga_2d_testing_2.py
+-rw-rw-rw-   0        0        0     4177 2023-03-10 02:05:30.000000 usda-0.0.27/src/usda/meta_heuristics/_ga_SegaranT.py
+-rw-rw-rw-   0        0        0     7982 2023-03-01 00:42:28.000000 usda-0.0.27/src/usda/meta_heuristics/_gwo.py
+-rw-rw-rw-   0        0        0     5251 2023-03-17 04:06:14.000000 usda-0.0.27/src/usda/meta_heuristics/_pso.py
+-rw-rw-rw-   0        0        0     7564 2023-03-18 04:30:42.000000 usda-0.0.27/src/usda/meta_heuristics/_pso_2d.py
+-rw-rw-rw-   0        0        0     8467 2023-03-18 05:15:56.000000 usda-0.0.27/src/usda/meta_heuristics/_pso_2d_testing.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.313951 usda-0.0.27/src/usda/migrated_project/
+-rw-rw-rw-   0        0        0      216 2023-07-13 07:05:32.000000 usda-0.0.27/src/usda/migrated_project/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.315946 usda-0.0.27/src/usda/migrated_project/invest/
+-rw-rw-rw-   0        0        0      711 2023-06-11 01:34:28.000000 usda-0.0.27/src/usda/migrated_project/invest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.341171 usda-0.0.27/src/usda/migrated_project/invest/configs/
+-rw-rw-rw-   0        0        0     1150 2023-06-09 12:59:24.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-05-21 14:16:58.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/_carbon_configs.py
+-rw-rw-rw-   0        0        0     5303 2023-05-22 07:01:14.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py
+-rw-rw-rw-   0        0        0     2352 2023-05-22 09:31:34.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py
+-rw-rw-rw-   0        0        0     3674 2023-05-22 08:55:40.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py
+-rw-rw-rw-   0        0        0      490 2023-05-21 18:26:42.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/_habitat_quality_configs.py
+-rw-rw-rw-   0        0        0      117 2023-06-09 13:00:22.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/_urban_cooling_configs.py
+-rw-rw-rw-   0        0        0     2095 2023-04-29 10:05:58.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv
+-rw-rw-rw-   0        0        0     1684 2023-05-16 20:54:58.000000 usda-0.0.27/src/usda/migrated_project/invest/configs/unit_definitions.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.369470 usda-0.0.27/src/usda/migrated_project/invest/esv/
+-rw-rw-rw-   0        0        0      700 2023-06-09 23:15:34.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/__init__.py
+-rw-rw-rw-   0        0        0    23442 2023-05-31 01:40:44.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_carbon.py
+-rw-rw-rw-   0        0        0    66377 2023-05-22 12:57:04.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_crop_pollination.py
+-rw-rw-rw-   0        0        0    37499 2023-05-22 10:16:22.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_crop_production_percentile.py
+-rw-rw-rw-   0        0        0    43341 2023-05-22 13:20:46.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_crop_production_regression.py
+-rw-rw-rw-   0        0        0    41477 2023-05-22 12:35:32.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_habitat_quality.py
+-rw-rw-rw-   0        0        0      610 2023-05-21 04:07:42.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_unit_registry.py
+-rw-rw-rw-   0        0        0    56182 2023-06-10 02:41:06.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_urban_cooling_model.py
+-rw-rw-rw-   0        0        0    44236 2023-05-21 14:00:32.000000 usda-0.0.27/src/usda/migrated_project/invest/esv/_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.383497 usda-0.0.27/src/usda/migrated_project/pass_panoseg/
+-rw-rw-rw-   0        0        0      201 2023-07-13 09:09:37.000000 usda-0.0.27/src/usda/migrated_project/pass_panoseg/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-07-13 08:45:47.000000 usda-0.0.27/src/usda/migrated_project/pass_panoseg/_dataset.py
+-rw-rw-rw-   0        0        0     5566 2023-07-13 07:08:21.000000 usda-0.0.27/src/usda/migrated_project/pass_panoseg/_erfnet_pspnet.py
+-rw-rw-rw-   0        0        0     3370 2023-07-14 05:43:09.000000 usda-0.0.27/src/usda/migrated_project/pass_panoseg/_semantic_seg.py
+-rw-rw-rw-   0        0        0     2896 2020-01-18 16:35:00.000000 usda-0.0.27/src/usda/migrated_project/pass_panoseg/_transform.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.396591 usda-0.0.27/src/usda/migrated_project/pix2pix/
+-rw-rw-rw-   0        0        0     1969 2023-04-20 08:47:18.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/A2B.py
+-rw-rw-rw-   0        0        0      217 2023-04-21 13:54:28.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.418880 usda-0.0.27/src/usda/migrated_project/pix2pix/data/
+-rw-rw-rw-   0        0        0     4100 2023-04-20 05:37:12.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-17 06:17:14.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py
+-rw-rw-rw-   0        0        0     6235 2023-04-17 05:52:32.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/_base_dataset.py
+-rw-rw-rw-   0        0        0     2897 2023-04-17 06:22:00.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py
+-rw-rw-rw-   0        0        0     1885 2023-03-14 20:28:50.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/_image_folder.py
+-rw-rw-rw-   0        0        0     1658 2023-04-17 06:20:00.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/_single_dataset.py
+-rw-rw-rw-   0        0        0     3589 2023-04-17 03:48:22.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/_template_dataset.py
+-rw-rw-rw-   0        0        0     3526 2023-04-17 05:45:04.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.421268 usda-0.0.27/src/usda/migrated_project/pix2pix/datasets/
+-rw-rw-rw-   0        0        0      198 2023-04-17 01:54:38.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.427814 usda-0.0.27/src/usda/migrated_project/pix2pix/imgs/
+-rw-rw-rw-   0        0        0      127 2023-04-21 13:57:20.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/imgs/__init__.py
+-rw-rw-rw-   0        0        0    14064 2023-04-21 14:08:06.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/imgs/example.jpg
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.442393 usda-0.0.27/src/usda/migrated_project/pix2pix/models/
+-rw-rw-rw-   0        0        0     3349 2023-04-20 02:44:46.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/models/__init__.py
+-rw-rw-rw-   0        0        0    10810 2023-04-17 07:20:12.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/models/_base_model.py
+-rw-rw-rw-   0        0        0    29098 2023-04-17 07:31:08.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/models/_networks.py
+-rw-rw-rw-   0        0        0     7024 2023-04-17 07:21:12.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py
+-rw-rw-rw-   0        0        0     3392 2023-04-17 12:08:32.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/models/_test_model.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.452996 usda-0.0.27/src/usda/migrated_project/pix2pix/options/
+-rw-rw-rw-   0        0        0      425 2023-04-17 11:42:48.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/options/__init__.py
+-rw-rw-rw-   0        0        0     3447 2023-04-17 08:10:08.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/options/_base_options.py
+-rw-rw-rw-   0        0        0     1045 2023-04-17 12:42:34.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/options/_test_options.py
+-rw-rw-rw-   0        0        0     2533 2023-04-17 11:39:46.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/options/_train_options.py
+-rw-rw-rw-   0        0        0     8846 2023-04-22 00:58:20.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/sketch_A2B.py
+-rw-rw-rw-   0        0        0     6019 2023-04-17 13:04:36.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/test.py
+-rw-rw-rw-   0        0        0     6788 2023-04-18 09:54:16.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/train.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.472533 usda-0.0.27/src/usda/migrated_project/pix2pix/util/
+-rw-rw-rw-   0        0        0      270 2023-04-17 11:51:20.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/util/__init__.py
+-rw-rw-rw-   0        0        0     3639 2023-03-14 20:28:50.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/util/_get_data.py
+-rw-rw-rw-   0        0        0     3223 2023-03-14 20:28:50.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/util/_html.py
+-rw-rw-rw-   0        0        0     2226 2023-03-14 20:28:50.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/util/_image_pool.py
+-rw-rw-rw-   0        0        0     3175 2023-03-14 20:28:50.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/util/_util.py
+-rw-rw-rw-   0        0        0    12408 2023-04-17 09:41:46.000000 usda-0.0.27/src/usda/migrated_project/pix2pix/util/_visualizer.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.495009 usda-0.0.27/src/usda/migrated_project/stylegan/
+-rw-rw-rw-   0        0        0      898 2023-04-17 10:27:42.000000 usda-0.0.27/src/usda/migrated_project/stylegan/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-04-16 06:09:10.000000 usda-0.0.27/src/usda/migrated_project/stylegan/_config.py
+-rw-rw-rw-   0        0        0     4425 2023-04-11 12:13:44.000000 usda-0.0.27/src/usda/migrated_project/stylegan/_convert.py
+-rw-rw-rw-   0        0        0     3527 2023-04-11 12:16:26.000000 usda-0.0.27/src/usda/migrated_project/stylegan/_generate_grid.py
+-rw-rw-rw-   0        0        0     5616 2023-04-16 11:14:58.000000 usda-0.0.27/src/usda/migrated_project/stylegan/_generate_mixing_figure.py
+-rw-rw-rw-   0        0        0     4595 2023-04-16 07:34:50.000000 usda-0.0.27/src/usda/migrated_project/stylegan/_generate_samples.py
+-rw-rw-rw-   0        0        0     3430 2023-04-16 08:58:06.000000 usda-0.0.27/src/usda/migrated_project/stylegan/_generate_truncation_figure.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.507156 usda-0.0.27/src/usda/migrated_project/stylegan/data/
+-rw-rw-rw-   0        0        0      558 2023-04-11 11:18:12.000000 usda-0.0.27/src/usda/migrated_project/stylegan/data/__init__.py
+-rw-rw-rw-   0        0        0     4744 2023-04-11 10:36:08.000000 usda-0.0.27/src/usda/migrated_project/stylegan/data/_datasets.py
+-rw-rw-rw-   0        0        0     1457 2023-04-11 10:36:56.000000 usda-0.0.27/src/usda/migrated_project/stylegan/data/_make_dataset.py
+-rw-rw-rw-   0        0        0     1014 2023-04-11 10:37:16.000000 usda-0.0.27/src/usda/migrated_project/stylegan/data/_transforms.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.511638 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/
+-rw-rw-rw-   0        0        0      799 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.519617 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/submission/
+-rw-rw-rw-   0        0        0      392 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/submission/__init__.py
+-rw-rw-rw-   0        0        0     4337 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py
+-rw-rw-rw-   0        0        0    11131 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.534200 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/
+-rw-rw-rw-   0        0        0      524 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py
+-rw-rw-rw-   0        0        0     7537 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py
+-rw-rw-rw-   0        0        0    30121 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py
+-rw-rw-rw-   0        0        0    10027 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py
+-rw-rw-rw-   0        0        0     9306 2023-04-11 12:36:20.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py
+-rw-rw-rw-   0        0        0    13756 2021-12-18 03:07:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/util.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.540629 usda-0.0.27/src/usda/migrated_project/stylegan/extracted_funcs/
+-rw-rw-rw-   0        0        0      186 2023-04-12 06:22:04.000000 usda-0.0.27/src/usda/migrated_project/stylegan/extracted_funcs/__init__.py
+-rw-rw-rw-   0        0        0     1354 2023-04-12 06:27:24.000000 usda-0.0.27/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.559616 usda-0.0.27/src/usda/migrated_project/stylegan/models/
+-rw-rw-rw-   0        0        0     6331 2023-04-11 11:53:58.000000 usda-0.0.27/src/usda/migrated_project/stylegan/models/_Blocks.py
+-rw-rw-rw-   0        0        0    11748 2023-04-11 11:32:54.000000 usda-0.0.27/src/usda/migrated_project/stylegan/models/_CustomLayers.py
+-rw-rw-rw-   0        0        0    38792 2023-04-11 11:52:56.000000 usda-0.0.27/src/usda/migrated_project/stylegan/models/_GAN.py
+-rw-rw-rw-   0        0        0     8277 2023-04-11 11:27:24.000000 usda-0.0.27/src/usda/migrated_project/stylegan/models/_Losses.py
+-rw-rw-rw-   0        0        0     1771 2023-04-11 11:56:28.000000 usda-0.0.27/src/usda/migrated_project/stylegan/models/__init__.py
+-rw-rw-rw-   0        0        0     1388 2023-04-11 11:40:44.000000 usda-0.0.27/src/usda/migrated_project/stylegan/models/_update_average.py
+-rw-rw-rw-   0        0        0     6150 2023-04-17 03:27:44.000000 usda-0.0.27/src/usda/migrated_project/stylegan/train.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.568734 usda-0.0.27/src/usda/migrated_project/stylegan/utils/
+-rw-rw-rw-   0        0        0      247 2023-04-11 07:34:42.000000 usda-0.0.27/src/usda/migrated_project/stylegan/utils/__init__.py
+-rw-rw-rw-   0        0        0     2159 2023-04-11 09:44:26.000000 usda-0.0.27/src/usda/migrated_project/stylegan/utils/_copy.py
+-rw-rw-rw-   0        0        0      685 2023-04-11 10:33:58.000000 usda-0.0.27/src/usda/migrated_project/stylegan/utils/_logger.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.628165 usda-0.0.27/src/usda/models/
+-rw-rw-rw-   0        0        0     5660 2023-07-25 11:51:23.000000 usda-0.0.27/src/usda/models/__init__.py
+-rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:20.000000 usda-0.0.27/src/usda/models/_bow_feature_builder.py
+-rw-rw-rw-   0        0        0     1014 2023-03-24 02:28:50.000000 usda-0.0.27/src/usda/models/_clustering.py
+-rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:32.000000 usda-0.0.27/src/usda/models/_computational_performance.py
+-rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:10.000000 usda-0.0.27/src/usda/models/_curve_segmentation.py
+-rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:06.000000 usda-0.0.27/src/usda/models/_decision_tree.py
+-rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:42.000000 usda-0.0.27/src/usda/models/_dim1_convolution.py
+-rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:50.000000 usda-0.0.27/src/usda/models/_entropy.py
+-rw-rw-rw-   0        0        0     1458 2023-03-24 10:49:06.000000 usda-0.0.27/src/usda/models/_global_local_autocorrelation.py
+-rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:06.000000 usda-0.0.27/src/usda/models/_image_tag_extractor.py
+-rw-rw-rw-   0        0        0     2087 2023-06-21 23:53:50.000000 usda-0.0.27/src/usda/models/_label_encoder.py
+-rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:58.000000 usda-0.0.27/src/usda/models/_neighbors.py
+-rw-rw-rw-   0        0        0     9967 2023-06-30 10:21:04.000000 usda-0.0.27/src/usda/models/_nlp_tools.py
+-rw-rw-rw-   0        0        0     3945 2023-07-25 11:52:51.000000 usda-0.0.27/src/usda/models/_plot_components.py
+-rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:26.000000 usda-0.0.27/src/usda/models/_random_forest_classifier.py
+-rw-rw-rw-   0        0        0    13684 2023-07-16 09:52:28.000000 usda-0.0.27/src/usda/models/_rnn_lstm.py
+-rw-rw-rw-   0        0        0    16007 2023-06-30 12:22:04.000000 usda-0.0.27/src/usda/models/_seq2seq.py
+-rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:46.000000 usda-0.0.27/src/usda/models/_sir_model.py
+-rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:06.000000 usda-0.0.27/src/usda/models/_superpixel_segmentation.py
+-rw-rw-rw-   0        0        0     9756 2023-07-01 03:01:18.000000 usda-0.0.27/src/usda/models/_transformer.py
+-rw-rw-rw-   0        0        0     8564 2023-07-11 03:52:38.000000 usda-0.0.27/src/usda/models/_vit.py
+-rw-rw-rw-   0        0        0     9313 2023-06-27 08:00:24.000000 usda-0.0.27/src/usda/models/_word2vec_sgns.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.635753 usda-0.0.27/src/usda/net/
+-rw-rw-rw-   0        0        0      120 2023-04-05 02:07:50.000000 usda-0.0.27/src/usda/net/_.py
+-rw-rw-rw-   0        0        0      856 2023-04-05 02:18:10.000000 usda-0.0.27/src/usda/net/__init__.py
+-rw-rw-rw-   0        0        0    28490 2023-04-05 02:16:40.000000 usda-0.0.27/src/usda/net/_networks_pix2pix.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.644422 usda-0.0.27/src/usda/network/
+-rw-rw-rw-   0        0        0      404 2023-04-01 07:37:22.000000 usda-0.0.27/src/usda/network/__init__.py
+-rw-rw-rw-   0        0        0     4050 2023-03-10 11:37:14.000000 usda-0.0.27/src/usda/network/_g_drawing.py
+-rw-rw-rw-   0        0        0     2896 2023-04-01 07:46:52.000000 usda-0.0.27/src/usda/network/_pt_pattern.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.694827 usda-0.0.27/src/usda/pano_projection_transformation/
+-rw-rw-rw-   0        0        0    10333 2023-07-15 05:00:44.000000 usda-0.0.27/src/usda/pano_projection_transformation/_Key_point_size_metrics.py
+-rw-rw-rw-   0        0        0    12906 2023-07-15 10:24:02.000000 usda-0.0.27/src/usda/pano_projection_transformation/_POI_street_feature.py
+-rw-rw-rw-   0        0        0     2641 2023-07-15 09:26:19.000000 usda-0.0.27/src/usda/pano_projection_transformation/__init__.py
+-rw-rw-rw-   0        0        0     4689 2023-07-15 01:49:23.000000 usda-0.0.27/src/usda/pano_projection_transformation/_color_metrics.py
+-rw-rw-rw-   0        0        0     8920 2023-07-15 01:22:29.000000 usda-0.0.27/src/usda/pano_projection_transformation/_color_metrics_pool.py
+-rw-rw-rw-   0        0        0     1461 2023-07-14 07:12:51.000000 usda-0.0.27/src/usda/pano_projection_transformation/_equi2cube.py
+-rw-rw-rw-   0        0        0    12692 2023-07-14 07:28:14.000000 usda-0.0.27/src/usda/pano_projection_transformation/_equi2cube_pool.py
+-rw-rw-rw-   0        0        0     1253 2023-07-14 10:05:43.000000 usda-0.0.27/src/usda/pano_projection_transformation/_equi2polar.py
+-rw-rw-rw-   0        0        0     6805 2023-07-14 10:12:49.000000 usda-0.0.27/src/usda/pano_projection_transformation/_equi2polar_pool.py
+-rw-rw-rw-   0        0        0    19002 2023-07-15 05:27:17.000000 usda-0.0.27/src/usda/pano_projection_transformation/_imgs_arranging.py
+-rw-rw-rw-   0        0        0    26655 2023-07-15 08:41:15.000000 usda-0.0.27/src/usda/pano_projection_transformation/_metric_clustering.py
+-rw-rw-rw-   0        0        0     2335 2023-07-15 06:43:18.000000 usda-0.0.27/src/usda/pano_projection_transformation/_metrics_clustering_pool.py
+-rw-rw-rw-   0        0        0     5662 2023-07-15 01:05:08.000000 usda-0.0.27/src/usda/pano_projection_transformation/_skyline_shape_metrics.py
+-rw-rw-rw-   0        0        0     3541 2023-07-14 11:58:36.000000 usda-0.0.27/src/usda/pano_projection_transformation/_spherical_panorama.py
+-rw-rw-rw-   0        0        0     6815 2023-07-14 13:09:54.000000 usda-0.0.27/src/usda/pano_projection_transformation/_visual_field_proportion_metrics.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.716769 usda-0.0.27/src/usda/pattern_signature/
+-rw-rw-rw-   0        0        0     1340 2023-03-24 06:18:08.000000 usda-0.0.27/src/usda/pattern_signature/__init__.py
+-rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:52.000000 usda-0.0.27/src/usda/pattern_signature/_distance_metric.py
+-rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:18.000000 usda-0.0.27/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
+-rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:30.000000 usda-0.0.27/src/usda/pattern_signature/_img_region_growing.py
+-rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:58.000000 usda-0.0.27/src/usda/pattern_signature/_pattern_module.py
+-rw-rw-rw-   0        0        0     7729 2023-03-24 07:51:32.000000 usda-0.0.27/src/usda/pattern_signature/_signature.py
+-rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:50.000000 usda-0.0.27/src/usda/pattern_signature/_signature2distance_integration.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.742405 usda-0.0.27/src/usda/pgm/
+-rw-rw-rw-   0        0        0     3024 2023-06-08 14:28:50.000000 usda-0.0.27/src/usda/pgm/_MRF.py
+-rw-rw-rw-   0        0        0     6429 2023-06-12 05:30:16.000000 usda-0.0.27/src/usda/pgm/_MRF_urban_cooling.py
+-rw-rw-rw-   0        0        0     1374 2023-06-10 12:20:50.000000 usda-0.0.27/src/usda/pgm/__init__.py
+-rw-rw-rw-   0        0        0     4688 2023-06-09 02:45:58.000000 usda-0.0.27/src/usda/pgm/_image_segmentation_using_mrf.py
+-rw-rw-rw-   0        0        0     3817 2023-06-02 07:46:24.000000 usda-0.0.27/src/usda/pgm/_pgm_calculating.py
+-rw-rw-rw-   0        0        0      372 2023-05-11 01:14:46.000000 usda-0.0.27/src/usda/pgm/_pgm_conversion.py
+-rw-rw-rw-   0        0        0     4763 2023-06-08 02:43:38.000000 usda-0.0.27/src/usda/pgm/_pgm_draw.py
+-rw-rw-rw-   0        0        0     1292 2023-05-15 12:25:46.000000 usda-0.0.27/src/usda/pgm/_probability_theory.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.759371 usda-0.0.27/src/usda/stats/
+-rw-rw-rw-   0        0        0     1045 2023-05-02 13:19:48.000000 usda-0.0.27/src/usda/stats/__init__.py
+-rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:20.000000 usda-0.0.27/src/usda/stats/_descriptive_stats.py
+-rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:58.000000 usda-0.0.27/src/usda/stats/_kde.py
+-rw-rw-rw-   0        0        0      778 2022-10-20 03:57:20.000000 usda-0.0.27/src/usda/stats/_outlier.py
+-rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:30.000000 usda-0.0.27/src/usda/stats/_regression.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.761527 usda-0.0.27/src/usda/tools/
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.780340 usda-0.0.27/src/usda/tools/DL_layers_visualizer/
+-rw-rw-rw-   0        0        0     4066 2023-03-29 04:55:12.000000 usda-0.0.27/src/usda/tools/DL_layers_visualizer/0_72.jpg
+-rw-rw-rw-   0        0        0    13876 2023-03-29 04:55:12.000000 usda-0.0.27/src/usda/tools/DL_layers_visualizer/0_8.jpg
+-rw-rw-rw-   0        0        0     3757 2023-03-29 04:55:14.000000 usda-0.0.27/src/usda/tools/DL_layers_visualizer/0_9.jpg
+-rw-rw-rw-   0        0        0     1064 2023-04-08 15:24:38.000000 usda-0.0.27/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
+-rw-rw-rw-   0        0        0      199 2023-04-09 05:39:16.000000 usda-0.0.27/src/usda/tools/DL_layers_visualizer/__init__.py
+-rw-rw-rw-   0        0        0      232 2023-04-09 05:40:00.000000 usda-0.0.27/src/usda/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.803373 usda-0.0.27/src/usda/utils/
+-rw-rw-rw-   0        0        0     1396 2023-07-16 08:13:41.000000 usda-0.0.27/src/usda/utils/__init__.py
+-rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:34.000000 usda-0.0.27/src/usda/utils/_bunch.py
+-rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:28.000000 usda-0.0.27/src/usda/utils/_coordinate_transformation.py
+-rw-rw-rw-   0        0        0     3970 2023-02-23 09:40:48.000000 usda-0.0.27/src/usda/utils/_df_process.py
+-rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:18.000000 usda-0.0.27/src/usda/utils/_displayable_path.py
+-rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:32.000000 usda-0.0.27/src/usda/utils/_file_structure.py
+-rw-rw-rw-   0        0        0     5812 2023-07-16 11:18:22.000000 usda-0.0.27/src/usda/utils/_gadgets.py
+-rw-rw-rw-   0        0        0      606 2022-10-22 00:35:58.000000 usda-0.0.27/src/usda/utils/_operating_time.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.815616 usda-0.0.27/src/usda/weight/
+-rw-rw-rw-   0        0        0     1014 2023-03-03 07:14:30.000000 usda-0.0.27/src/usda/weight/__init__.py
+-rw-rw-rw-   0        0        0    38486 2023-03-03 07:13:36.000000 usda-0.0.27/src/usda/weight/_decision_rule.py
+-rw-rw-rw-   0        0        0     2745 2023-02-23 12:30:36.000000 usda-0.0.27/src/usda/weight/_entropy_weight.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:38:44.021592 usda-0.0.27/src/usda.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-08-05 13:38:43.000000 usda-0.0.27/src/usda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12840 2023-08-05 13:38:43.000000 usda-0.0.27/src/usda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 13:38:43.000000 usda-0.0.27/src/usda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-16 07:33:52.000000 usda-0.0.27/src/usda.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-08-05 13:38:43.000000 usda-0.0.27/src/usda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-05 13:38:43.000000 usda-0.0.27/src/usda.egg-info/top_level.txt
```

### Comparing `usda-0.0.26/LICENSE` & `usda-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/PKG-INFO` & `usda-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.26
+Version: 0.0.27
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.26/setup.py` & `usda-0.0.27/setup.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/__init__.py` & `usda-0.0.27/src/usda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Created on Sun Aug 21 15:11:00 2022
 
 @author: Richie Bao-caDesign设计(cadesign.cn)
 
 python setup.py sdist
 twine upload dist/usda-0.0.22.tar.gz
 """
-__version__ = "0.0.26"
+__version__ = "0.0.27"
 
 __all__ = [
     "data_process"
     "datasets",
     "database",
     "utils",
     "data_visualization",
```

### Comparing `usda-0.0.26/src/usda/_min_dependencies.py` & `usda-0.0.27/src/usda/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/__init__.py` & `usda-0.0.27/src/usda/data_process/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_geoinfodata_conversion.py` & `usda-0.0.27/src/usda/data_process/_geoinfodata_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_image_pixel_sampling_zoom.py` & `usda-0.0.27/src/usda/data_process/_image_pixel_sampling_zoom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_kitti_dataprocess.py` & `usda-0.0.27/src/usda/data_process/_kitti_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_landsat_dataprocess.py` & `usda-0.0.27/src/usda/data_process/_landsat_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_naip_dataprocess.py` & `usda-0.0.27/src/usda/data_process/_naip_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_osm_dataprocess.py` & `usda-0.0.27/src/usda/data_process/_osm_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_raster_dataprocess.py` & `usda-0.0.27/src/usda/data_process/_raster_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_process/_tiler_calculation.py` & `usda-0.0.27/src/usda/data_process/_tiler_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visual/_worldcover_plot_style.py` & `usda-0.0.27/src/usda/data_visual/_worldcover_plot_style.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/__init__.py` & `usda-0.0.27/src/usda/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_chart_custom.py` & `usda-0.0.27/src/usda/data_visualization/_chart_custom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_colors.py` & `usda-0.0.27/src/usda/data_visualization/_colors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_dynamic_streetView_visual_perception.py` & `usda-0.0.27/src/usda/data_visualization/_dynamic_streetView_visual_perception.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_gdf_plot.py` & `usda-0.0.27/src/usda/data_visualization/_gdf_plot.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_gif_show.py` & `usda-0.0.27/src/usda/data_visualization/_gif_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_graphic_drawing.py` & `usda-0.0.27/src/usda/data_visualization/_graphic_drawing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_image_process.py` & `usda-0.0.27/src/usda/data_visualization/_image_process.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_img_feature_extraction.py` & `usda-0.0.27/src/usda/data_visualization/_img_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_img_theme_color.py` & `usda-0.0.27/src/usda/data_visualization/_img_theme_color.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_imgs_layout_show.py` & `usda-0.0.27/src/usda/data_visualization/_imgs_layout_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_imgs_show.py` & `usda-0.0.27/src/usda/data_visualization/_imgs_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_knee_line_graph.py` & `usda-0.0.27/src/usda/data_visualization/_knee_line_graph.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_moving_average_inflection.py` & `usda-0.0.27/src/usda/data_visualization/_moving_average_inflection.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_panorama_show.py` & `usda-0.0.27/src/usda/data_visualization/_panorama_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_plot_single_function.py` & `usda-0.0.27/src/usda/data_visualization/_plot_single_function.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_raster_percentile_slider.py` & `usda-0.0.27/src/usda/data_visualization/_raster_percentile_slider.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_raster_show.py` & `usda-0.0.27/src/usda/data_visualization/_raster_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_stats_charts.py` & `usda-0.0.27/src/usda/data_visualization/_stats_charts.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_superpixel_segmentation_show.py` & `usda-0.0.27/src/usda/data_visualization/_superpixel_segmentation_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_table_show.py` & `usda-0.0.27/src/usda/data_visualization/_table_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/_tile_show.py` & `usda-0.0.27/src/usda/data_visualization/_tile_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/data_generator.py` & `usda-0.0.27/src/usda/data_visualization/data_generator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/data_visualization/knee_locator.py` & `usda-0.0.27/src/usda/data_visualization/knee_locator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/database/__init__.py` & `usda-0.0.27/src/usda/database/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/database/_data_file_rw.py` & `usda-0.0.27/src/usda/database/_data_file_rw.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/database/_data_format_conversion.py` & `usda-0.0.27/src/usda/database/_data_format_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/database/_database.py` & `usda-0.0.27/src/usda/database/_database.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/database/_read_matlab_fig.py` & `usda-0.0.27/src/usda/database/_read_matlab_fig.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/__init__.py` & `usda-0.0.27/src/usda/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_artificial_data.py` & `usda-0.0.27/src/usda/datasets/_artificial_data.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_base.py` & `usda-0.0.27/src/usda/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_coordinate_transformation.py` & `usda-0.0.27/src/usda/datasets/_coordinate_transformation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_dataset_info.py` & `usda-0.0.27/src/usda/datasets/_dataset_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_files_downloading.py` & `usda-0.0.27/src/usda/datasets/_files_downloading.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_img_info.py` & `usda-0.0.27/src/usda/datasets/_img_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_kml_info.py` & `usda-0.0.27/src/usda/datasets/_kml_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_panorama_baidu_download.py` & `usda-0.0.27/src/usda/datasets/_panorama_baidu_download.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_poi_crawler.py` & `usda-0.0.27/src/usda/datasets/_poi_crawler.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/_rs_image.py` & `usda-0.0.27/src/usda/datasets/_rs_image.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle` & `usda-0.0.27/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/evaluation_criteria_raw_values.pickle` & `usda-0.0.27/src/usda/datasets/data/evaluation_criteria_raw_values.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/jisperveld_data.pickle` & `usda-0.0.27/src/usda/datasets/data/jisperveld_data.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/microclimate_in_office_rooms.pickle` & `usda-0.0.27/src/usda/datasets/data/microclimate_in_office_rooms.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle` & `usda-0.0.27/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/sales_data_cartoon_database.pickle` & `usda-0.0.27/src/usda/datasets/data/sales_data_cartoon_database.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle` & `usda-0.0.27/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/datasets/data/test_score_cartoon_statistic.pickle` & `usda-0.0.27/src/usda/datasets/data/test_score_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/__init__.py` & `usda-0.0.27/src/usda/geodata_process/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 
 from ._shp_dataprocess import shp2gdf
 from ._build_clipped_raster_dataset import xy_size_elevation
 from ._build_clipped_raster_dataset import build_clipped_raster_dataset
 
 from ._data_format_conversion import kml2gdf_folder
 
+from ._overlapping_polygons import IoU_2Polygons
+from ._overlapping_polygons import drop_overlapping_polygons
+from ._overlapping_polygons import planetary_computer_items_filter4download
+
 __all__ = [
     "pt_coordi_transform",
     "pt_on_quadrat",
     "rio_read_subset",
     "rec_quadrats_gdf",
     "raster2polygon",
     "raster_reprojection",
@@ -57,9 +61,12 @@
     "extract_raster_vals_at_pts",
     "extract_raster_vals_at_pts_batch",
     "rasters_minimum_bound",
     "rastercells2shp",
     "xy_size_elevation",
     "build_clipped_raster_dataset",
     "kml2gdf_folder",
+    "drop_overlapping_polygons",
+    "IoU_2Polygons",
+    "planetary_computer_items_filter4download",
     ]
```

### Comparing `usda-0.0.26/src/usda/geodata_process/_build_clipped_raster_dataset.py` & `usda-0.0.27/src/usda/geodata_process/_build_clipped_raster_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py` & `usda-0.0.27/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_data_format_conversion.py` & `usda-0.0.27/src/usda/geodata_process/_data_format_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_quadrat.py` & `usda-0.0.27/src/usda/geodata_process/_quadrat.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_raster_dataprocess.py` & `usda-0.0.27/src/usda/geodata_process/_raster_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_raster_stats.py` & `usda-0.0.27/src/usda/geodata_process/_raster_stats.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_rasterize.py` & `usda-0.0.27/src/usda/geodata_process/_rasterize.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_rio_tiler.py` & `usda-0.0.27/src/usda/geodata_process/_rio_tiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Mar 21 17:30:43 2023
 
 @author: richie bao
 """
 import math  
-from rio_tiler.io import COGReader # proj problem
+# from rio_tiler.io import COGReader # proj problem
 import numpy as np
 import matplotlib.pyplot as plt
 
 def deg2num(lat_deg, lon_deg, zoom):
     '''
     code migration
     function - 将经纬度坐标转换为指定zoom level缩放级别下，金子塔中瓦片的坐标。
```

### Comparing `usda-0.0.26/src/usda/geodata_process/_sample_pts.py` & `usda-0.0.27/src/usda/geodata_process/_sample_pts.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/geodata_process/_shp_dataprocess.py` & `usda-0.0.27/src/usda/geodata_process/_shp_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/imgs_process/_imgs_process_basic.py` & `usda-0.0.27/src/usda/imgs_process/_imgs_process_basic.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/indices/_rs_indices.py` & `usda-0.0.27/src/usda/indices/_rs_indices.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/manifold/_manifold_learning_illustration.py` & `usda-0.0.27/src/usda/manifold/_manifold_learning_illustration.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/maths/__init__.py` & `usda-0.0.27/src/usda/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/maths/_algebra.py` & `usda-0.0.27/src/usda/maths/_algebra.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/maths/_geometric_calculation.py` & `usda-0.0.27/src/usda/maths/_geometric_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/maths/_plot_single_function.py` & `usda-0.0.27/src/usda/maths/_plot_single_function.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/__init__.py` & `usda-0.0.27/src/usda/meta_heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_cuckoo_s.py` & `usda-0.0.27/src/usda/meta_heuristics/_cuckoo_s.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_firefly_a.py` & `usda-0.0.27/src/usda/meta_heuristics/_firefly_a.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_ga.py` & `usda-0.0.27/src/usda/meta_heuristics/_ga.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_ga_2d.py` & `usda-0.0.27/src/usda/meta_heuristics/_ga_2d.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_ga_2d_fixed_map.py` & `usda-0.0.27/src/usda/meta_heuristics/_ga_2d_fixed_map.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_ga_2d_testing_1.py` & `usda-0.0.27/src/usda/meta_heuristics/_ga_2d_testing_1.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_ga_2d_testing_2.py` & `usda-0.0.27/src/usda/meta_heuristics/_ga_2d_testing_2.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_ga_SegaranT.py` & `usda-0.0.27/src/usda/meta_heuristics/_ga_SegaranT.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_gwo.py` & `usda-0.0.27/src/usda/meta_heuristics/_gwo.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_pso.py` & `usda-0.0.27/src/usda/meta_heuristics/_pso.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_pso_2d.py` & `usda-0.0.27/src/usda/meta_heuristics/_pso_2d.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/meta_heuristics/_pso_2d_testing.py` & `usda-0.0.27/src/usda/meta_heuristics/_pso_2d_testing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/__init__.py` & `usda-0.0.27/src/usda/migrated_project/invest/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/configs/__init__.py` & `usda-0.0.27/src/usda/migrated_project/invest/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/configs/_carbon_configs.py` & `usda-0.0.27/src/usda/migrated_project/invest/configs/_carbon_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py` & `usda-0.0.27/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py` & `usda-0.0.27/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py` & `usda-0.0.27/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv` & `usda-0.0.27/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/configs/unit_definitions.txt` & `usda-0.0.27/src/usda/migrated_project/invest/configs/unit_definitions.txt`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/__init__.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_carbon.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_carbon.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_crop_pollination.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_crop_pollination.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_crop_production_percentile.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_crop_production_percentile.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_crop_production_regression.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_crop_production_regression.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_habitat_quality.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_habitat_quality.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_unit_registry.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_unit_registry.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_urban_cooling_model.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_urban_cooling_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/invest/esv/_utils.py` & `usda-0.0.27/src/usda/migrated_project/invest/esv/_utils.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pass_panoseg/_dataset.py` & `usda-0.0.27/src/usda/migrated_project/pass_panoseg/_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pass_panoseg/_erfnet_pspnet.py` & `usda-0.0.27/src/usda/migrated_project/pass_panoseg/_erfnet_pspnet.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pass_panoseg/_semantic_seg.py` & `usda-0.0.27/src/usda/migrated_project/pass_panoseg/_semantic_seg.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pass_panoseg/_transform.py` & `usda-0.0.27/src/usda/migrated_project/pass_panoseg/_transform.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/A2B.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/A2B.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/__init__.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/_base_dataset.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/_base_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/_image_folder.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/_image_folder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/_single_dataset.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/_single_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/_template_dataset.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/_template_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/imgs/example.jpg` & `usda-0.0.27/src/usda/migrated_project/pix2pix/imgs/example.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/models/__init__.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/models/_base_model.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/models/_base_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/models/_networks.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/models/_networks.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/models/_test_model.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/models/_test_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/options/_base_options.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/options/_base_options.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/options/_test_options.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/options/_test_options.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/options/_train_options.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/options/_train_options.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/sketch_A2B.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/sketch_A2B.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/test.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/test.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/train.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/train.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/util/_get_data.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/util/_get_data.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/util/_html.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/util/_html.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/util/_image_pool.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/util/_image_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/util/_util.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/util/_util.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/pix2pix/util/_visualizer.py` & `usda-0.0.27/src/usda/migrated_project/pix2pix/util/_visualizer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/__init__.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/_config.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/_config.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/_convert.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/_convert.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/_generate_grid.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/_generate_grid.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/_generate_mixing_figure.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/_generate_mixing_figure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/_generate_samples.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/_generate_samples.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/_generate_truncation_figure.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/_generate_truncation_figure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/data/__init__.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/data/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/data/_datasets.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/data/_datasets.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/data/_make_dataset.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/data/_make_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/data/_transforms.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/data/_transforms.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/__init__.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/dnnlib/util.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/dnnlib/util.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/models/_Blocks.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/models/_Blocks.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/models/_CustomLayers.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/models/_CustomLayers.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/models/_GAN.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/models/_GAN.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/models/_Losses.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/models/_Losses.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/models/__init__.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/models/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/models/_update_average.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/models/_update_average.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/train.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/train.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/utils/_copy.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/utils/_copy.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/migrated_project/stylegan/utils/_logger.py` & `usda-0.0.27/src/usda/migrated_project/stylegan/utils/_logger.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/__init__.py` & `usda-0.0.27/src/usda/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 
 from ._vit import img_to_patch
 from ._vit import AttentionBlock
 from ._vit import VisionTransformer
 from ._vit import ViT
 from ._vit import train_model4ViT
 
+from ._plot_components import plot_components
+from ._plot_components import resize_array
+
 __all__=[
     "k_neighbors_entire",
     "PolynomialFeatures_regularization",
     "dim1_convolution_SubplotAnimation",
     "G_T_type_1",
     "F_T_type_1",
     "G_T_type_2",
@@ -153,11 +156,13 @@
     "train_model4ViT",
     "Simple_LSTM",
     "spatial_metrics_train",
     "train_test_rmse_plot",
     "timeseries_pred_plot",
     "timeseries_pred_generation",
     "timeseries_pred_generation_plot",
+    "plot_components",
+    "resize_array",
     ]
```

### Comparing `usda-0.0.26/src/usda/models/_bow_feature_builder.py` & `usda-0.0.27/src/usda/models/_bow_feature_builder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_clustering.py` & `usda-0.0.27/src/usda/models/_clustering.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_computational_performance.py` & `usda-0.0.27/src/usda/models/_computational_performance.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_curve_segmentation.py` & `usda-0.0.27/src/usda/models/_curve_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_decision_tree.py` & `usda-0.0.27/src/usda/models/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_dim1_convolution.py` & `usda-0.0.27/src/usda/models/_dim1_convolution.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_entropy.py` & `usda-0.0.27/src/usda/models/_entropy.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_global_local_autocorrelation.py` & `usda-0.0.27/src/usda/models/_global_local_autocorrelation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_image_tag_extractor.py` & `usda-0.0.27/src/usda/models/_image_tag_extractor.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_label_encoder.py` & `usda-0.0.27/src/usda/models/_label_encoder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_neighbors.py` & `usda-0.0.27/src/usda/models/_neighbors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_nlp_tools.py` & `usda-0.0.27/src/usda/models/_nlp_tools.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_random_forest_classifier.py` & `usda-0.0.27/src/usda/models/_random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_rnn_lstm.py` & `usda-0.0.27/src/usda/models/_rnn_lstm.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_seq2seq.py` & `usda-0.0.27/src/usda/models/_seq2seq.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_sir_model.py` & `usda-0.0.27/src/usda/models/_sir_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_superpixel_segmentation.py` & `usda-0.0.27/src/usda/models/_superpixel_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_transformer.py` & `usda-0.0.27/src/usda/models/_transformer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_vit.py` & `usda-0.0.27/src/usda/models/_vit.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/models/_word2vec_sgns.py` & `usda-0.0.27/src/usda/models/_word2vec_sgns.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/net/__init__.py` & `usda-0.0.27/src/usda/net/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/net/_networks_pix2pix.py` & `usda-0.0.27/src/usda/net/_networks_pix2pix.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/network/_g_drawing.py` & `usda-0.0.27/src/usda/network/_g_drawing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/network/_pt_pattern.py` & `usda-0.0.27/src/usda/network/_pt_pattern.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_Key_point_size_metrics.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_Key_point_size_metrics.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_POI_street_feature.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_POI_street_feature.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/__init__.py` & `usda-0.0.27/src/usda/pano_projection_transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_color_metrics.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_color_metrics.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_color_metrics_pool.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_color_metrics_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_equi2cube.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_equi2cube.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_equi2cube_pool.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_equi2cube_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_equi2polar.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_equi2polar.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_equi2polar_pool.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_equi2polar_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_imgs_arranging.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_imgs_arranging.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_metric_clustering.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_metric_clustering.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_metrics_clustering_pool.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_metrics_clustering_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_skyline_shape_metrics.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_skyline_shape_metrics.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_spherical_panorama.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_spherical_panorama.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pano_projection_transformation/_visual_field_proportion_metrics.py` & `usda-0.0.27/src/usda/pano_projection_transformation/_visual_field_proportion_metrics.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pattern_signature/__init__.py` & `usda-0.0.27/src/usda/pattern_signature/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pattern_signature/_distance_metric.py` & `usda-0.0.27/src/usda/pattern_signature/_distance_metric.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pattern_signature/_grid_neighbors_xy_finder.py` & `usda-0.0.27/src/usda/pattern_signature/_grid_neighbors_xy_finder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pattern_signature/_img_region_growing.py` & `usda-0.0.27/src/usda/pattern_signature/_img_region_growing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pattern_signature/_pattern_module.py` & `usda-0.0.27/src/usda/pattern_signature/_pattern_module.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pattern_signature/_signature.py` & `usda-0.0.27/src/usda/pattern_signature/_signature.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pattern_signature/_signature2distance_integration.py` & `usda-0.0.27/src/usda/pattern_signature/_signature2distance_integration.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pgm/_MRF.py` & `usda-0.0.27/src/usda/pgm/_MRF.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pgm/_MRF_urban_cooling.py` & `usda-0.0.27/src/usda/pgm/_MRF_urban_cooling.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pgm/__init__.py` & `usda-0.0.27/src/usda/pgm/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pgm/_image_segmentation_using_mrf.py` & `usda-0.0.27/src/usda/pgm/_image_segmentation_using_mrf.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pgm/_pgm_calculating.py` & `usda-0.0.27/src/usda/pgm/_pgm_calculating.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pgm/_pgm_draw.py` & `usda-0.0.27/src/usda/pgm/_pgm_draw.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/pgm/_probability_theory.py` & `usda-0.0.27/src/usda/pgm/_probability_theory.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/stats/__init__.py` & `usda-0.0.27/src/usda/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/stats/_descriptive_stats.py` & `usda-0.0.27/src/usda/stats/_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/stats/_kde.py` & `usda-0.0.27/src/usda/stats/_kde.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/stats/_outlier.py` & `usda-0.0.27/src/usda/stats/_outlier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/stats/_regression.py` & `usda-0.0.27/src/usda/stats/_regression.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/tools/DL_layers_visualizer/0_72.jpg` & `usda-0.0.27/src/usda/tools/DL_layers_visualizer/0_72.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/tools/DL_layers_visualizer/0_8.jpg` & `usda-0.0.27/src/usda/tools/DL_layers_visualizer/0_8.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/tools/DL_layers_visualizer/0_9.jpg` & `usda-0.0.27/src/usda/tools/DL_layers_visualizer/0_9.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py` & `usda-0.0.27/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/__init__.py` & `usda-0.0.27/src/usda/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/_bunch.py` & `usda-0.0.27/src/usda/utils/_bunch.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/_coordinate_transformation.py` & `usda-0.0.27/src/usda/utils/_coordinate_transformation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/_df_process.py` & `usda-0.0.27/src/usda/utils/_df_process.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/_displayable_path.py` & `usda-0.0.27/src/usda/utils/_displayable_path.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/_file_structure.py` & `usda-0.0.27/src/usda/utils/_file_structure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/_gadgets.py` & `usda-0.0.27/src/usda/utils/_gadgets.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/utils/_operating_time.py` & `usda-0.0.27/src/usda/utils/_operating_time.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/weight/__init__.py` & `usda-0.0.27/src/usda/weight/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/weight/_decision_rule.py` & `usda-0.0.27/src/usda/weight/_decision_rule.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda/weight/_entropy_weight.py` & `usda-0.0.27/src/usda/weight/_entropy_weight.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.26/src/usda.egg-info/PKG-INFO` & `usda-0.0.27/src/usda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.26
+Version: 0.0.27
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.26/src/usda.egg-info/SOURCES.txt` & `usda-0.0.27/src/usda.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/usda/data_process/_kitti_dataprocess.py
 src/usda/data_process/_landsat_dataprocess.py
 src/usda/data_process/_naip_dataprocess.py
 src/usda/data_process/_osm_dataprocess.py
 src/usda/data_process/_raster_dataprocess.py
 src/usda/data_process/_tiler_calculation.py
 src/usda/data_visual/__init__.py
+src/usda/data_visual/_colors.py
 src/usda/data_visual/_plot_style.py
 src/usda/data_visual/_worldcover_plot_style.py
 src/usda/data_visualization/__init__.py
 src/usda/data_visualization/_chart_custom.py
 src/usda/data_visualization/_colors.py
 src/usda/data_visualization/_dynamic_streetView_visual_perception.py
 src/usda/data_visualization/_gdf_plot.py
@@ -67,32 +68,36 @@
 src/usda/datasets/data/jisperveld_data.pickle
 src/usda/datasets/data/microclimate_in_office_rooms.pickle
 src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
 src/usda/datasets/data/sales_data_cartoon_database.pickle
 src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
 src/usda/datasets/data/test_score_cartoon_statistic.pickle
 src/usda/demo/__init__.py
-src/usda/demo/_demo_isotonic_regression.py
+src/usda/demo/_demo_misc.py
 src/usda/geodata_process/__init__.py
 src/usda/geodata_process/_build_clipped_raster_dataset.py
 src/usda/geodata_process/_build_clipped_raster_dataset_pool.py
 src/usda/geodata_process/_data_format_conversion.py
+src/usda/geodata_process/_overlapping_polygons.py
 src/usda/geodata_process/_quadrat.py
 src/usda/geodata_process/_raster_dataprocess.py
 src/usda/geodata_process/_raster_stats.py
 src/usda/geodata_process/_rasterize.py
 src/usda/geodata_process/_rio_tiler.py
 src/usda/geodata_process/_sample_pts.py
 src/usda/geodata_process/_shp_dataprocess.py
 src/usda/imgs_process/__init__.py
 src/usda/imgs_process/_imgs_process_basic.py
 src/usda/indices/__init__.py
 src/usda/indices/_rs_indices.py
 src/usda/manifold/__init__.py
+src/usda/manifold/_correlations_embedding.py
 src/usda/manifold/_manifold_learning_illustration.py
+src/usda/manifold/_rbf_kernel_pca.py
+src/usda/manifold/_tsne.py
 src/usda/maths/__init__.py
 src/usda/maths/_algebra.py
 src/usda/maths/_geometric_calculation.py
 src/usda/maths/_plot_single_function.py
 src/usda/meta_heuristics/__init__.py
 src/usda/meta_heuristics/_cuckoo_s.py
 src/usda/meta_heuristics/_firefly_a.py
@@ -204,14 +209,15 @@
 src/usda/models/_dim1_convolution.py
 src/usda/models/_entropy.py
 src/usda/models/_global_local_autocorrelation.py
 src/usda/models/_image_tag_extractor.py
 src/usda/models/_label_encoder.py
 src/usda/models/_neighbors.py
 src/usda/models/_nlp_tools.py
+src/usda/models/_plot_components.py
 src/usda/models/_random_forest_classifier.py
 src/usda/models/_rnn_lstm.py
 src/usda/models/_seq2seq.py
 src/usda/models/_sir_model.py
 src/usda/models/_superpixel_segmentation.py
 src/usda/models/_transformer.py
 src/usda/models/_vit.py
```

