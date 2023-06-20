# Comparing `tmp/Simba-UW-tf-dev-1.63.4.tar.gz` & `tmp/Simba-UW-tf-dev-1.63.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.4.tar", last modified: Sun Jun 18 20:27:59 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.5.tar", last modified: Tue Jun 20 19:00:50 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.63.4.tar` & `Simba-UW-tf-dev-1.63.5.tar`

### file list

```diff
@@ -1,559 +1,559 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.4/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.4/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.63.4/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.4/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.4/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.4/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20688 2023-06-11 20:18:17.000000 Simba-UW-tf-dev-1.63.4/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.4/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.63.4/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.4/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.4/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-17 19:01:05.000000 Simba-UW-tf-dev-1.63.4/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.4/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73254 2023-06-07 20:39:22.000000 Simba-UW-tf-dev-1.63.4/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.63.4/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21105 2023-06-17 18:47:23.000000 Simba-UW-tf-dev-1.63.4/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-17 19:01:05.000000 Simba-UW-tf-dev-1.63.4/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7601 2023-06-18 18:58:51.000000 Simba-UW-tf-dev-1.63.4/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.4/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.63.4/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9338 2023-06-17 18:35:53.000000 Simba-UW-tf-dev-1.63.4/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.4/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.63.4/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.4/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.4/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.63.4/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.63.4/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2105 2023-06-16 19:56:36.000000 Simba-UW-tf-dev-1.63.4/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2245 2023-06-17 15:40:08.000000 Simba-UW-tf-dev-1.63.4/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.63.4/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.63.4/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.4/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.4/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.4/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.4/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6774 2023-06-15 19:18:29.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7661 2023-06-15 20:00:19.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.63.4/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.4/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.4/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.4/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.4/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.4/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.4/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.4/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66084 2023-06-17 19:01:00.000000 Simba-UW-tf-dev-1.63.4/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-17 18:48:05.000000 Simba-UW-tf-dev-1.63.4/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.4/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.4/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.4/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.4/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.4/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.4/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.4/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    20500 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.4/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.4/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.4/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.4/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.4/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.4/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.4/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.4/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.4/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.4/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.4/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.4/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.4/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.4/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.4/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.4/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.4/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.4/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.4/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.4/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-18 20:27:57.000000 Simba-UW-tf-dev-1.63.4/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-18 20:27:59.000000 Simba-UW-tf-dev-1.63.4/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.5/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.5/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.63.5/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.5/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.5/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.5/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20696 2023-06-20 18:57:14.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.5/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.5/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-20 18:30:33.000000 Simba-UW-tf-dev-1.63.5/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.5/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 18:25:39.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.63.5/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.63.5/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.63.5/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-20 18:25:39.000000 Simba-UW-tf-dev-1.63.5/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7601 2023-06-18 18:58:51.000000 Simba-UW-tf-dev-1.63.5/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.5/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.63.5/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.63.5/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.5/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.63.5/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.5/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.5/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.63.5/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.63.5/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.5/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.5/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.63.5/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.63.5/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.5/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.5/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.5/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.5/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 18:25:39.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.63.5/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.5/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.5/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.5/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.5/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.5/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.5/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.5/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66068 2023-06-20 18:58:45.000000 Simba-UW-tf-dev-1.63.5/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-17 18:48:05.000000 Simba-UW-tf-dev-1.63.5/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.5/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.5/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.5/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.5/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.5/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.5/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.5/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    20508 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-20 19:00:49.000000 Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.5/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.5/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.5/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.5/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.5/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.5/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.5/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.5/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.5/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.5/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.5/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.5/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.5/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.5/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.5/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.5/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.5/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.5/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.5/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.5/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-20 18:57:14.000000 Simba-UW-tf-dev-1.63.5/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-20 19:00:50.000000 Simba-UW-tf-dev-1.63.5/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.63.4/PKG-INFO` & `Simba-UW-tf-dev-1.63.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.4
+Version: 1.63.5
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/ui/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -253,23 +253,23 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000c 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0001 c1a1 0000 000b 005f 005f 0070  ..........._._.p
+00001030: 0000 0002 a412 0000 000b 005f 005f 0070  ..........._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 bcee b1bf  moDDblob........
-00001060: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 2c2b 9e29  moDDblob....,+.)
+00001060: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 bcee b1bf 1b1f  dDblob..........
+00001080: 6444 626c 6f62 0000 0008 2c2b 9e29 7b20  dDblob....,+.){ 
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0002 2000 0000 0007  comp...... .....
+000010b0: 636f 6d70 0000 0000 0003 3000 0000 0007  comp......0.....
 000010c0: 0070 006f 0070 005f 0075 0070 0073 6277  .p.o.p._.u.p.sbw
 000010d0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
 000010e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000010f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001100: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 00001110: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001120: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
@@ -278,15 +278,15 @@
 00001150: 6261 7208 0809 0809 5f10 197b 7b33 3534  bar....._..{{354
 00001160: 2c20 3132 347d 2c20 7b31 3037 362c 2036  , 124}, {1076, 6
 00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
 00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
 000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-000011c0: 0000 000a 7f9b 0000 0007 0070 006f 0070  ...........p.o.p
+000011c0: 0000 000d a80a 0000 0007 0070 006f 0070  ...........p.o.p
 000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
 000011e0: 0000 02b8 6270 6c69 7374 3030 da01 0203  ....bplist00....
 000011f0: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
 00001200: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
 00001210: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00001220: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00001230: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -374,15 +374,15 @@
 00001750: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001760: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
 00001770: 6200 0000 08f5 31c6 66d3 1dc5 4100 0000  b.....1.f...A...
 00001780: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
 00001790: 6f64 4462 6c6f 6200 0000 08f5 31c6 66d3  odDblob.....1.f.
 000017a0: 1dc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
 000017b0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-000017c0: 0000 0e70 0000 0000 0700 7000 6f00 7000  ...p......p.o.p.
+000017c0: 0000 1300 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
 000017d0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 000017e0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
 00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -502,12 +502,12 @@
 00001f50: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001f60: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
 00001f70: 6200 0000 08f5 31c6 66d3 1dc5 4100 0000  b.....1.f...A...
 00001f80: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
 00001f90: 6f64 4462 6c6f 6200 0000 08f5 31c6 66d3  odDblob.....1.f.
 00001fa0: 1dc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
 00001fb0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-00001fc0: 0000 0e70 0000 0000 0700 7000 6f00 7000  ...p......p.o.p.
+00001fc0: 0000 1300 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
 00001fd0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 00001fe0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.63.5/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/labelling/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 000002b0: 0062 0065 006c 006c 0069 006e 0067 002f  .b.e.l.l.i.n.g./
 000002c0: 0000 000b 005f 005f 0069 006e 0069 0074  ....._._.i.n.i.t
 000002d0: 005f 005f 002e 0070 0079 7074 624e 7573  ._._...p.yptbNus
 000002e0: 7472 0000 000b 005f 005f 0069 006e 0069  tr....._._.i.n.i
 000002f0: 0074 005f 005f 002e 0070 0079 0000 000b  .t._._...p.y....
 00000300: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000310: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000320: 0000 0001 3c13 0000 000b 005f 005f 0070  ....<......_._.p
+00000320: 0000 0001 d1b3 0000 000b 005f 005f 0070  ..........._._.p
 00000330: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000340: 6d6f 4444 626c 6f62 0000 0008 8eb9 d848  moDDblob.......H
-00000350: af1d c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000340: 6d6f 4444 626c 6f62 0000 0008 d69d 9c29  moDDblob.......)
+00000350: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00000360: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000370: 6444 626c 6f62 0000 0008 8eb9 d848 af1d  dDblob.......H..
+00000370: 6444 626c 6f62 0000 0008 d69d 9c29 7b20  dDblob.......){ 
 00000380: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00000390: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000003a0: 636f 6d70 0000 0000 0001 7000 0000 0000  comp......p.....
+000003a0: 636f 6d70 0000 0000 0002 2000 0000 0000  comp...... .....
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.63.5/simba/labelling/labelling_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             check_file_exist_and_readable(file_path=self.targets_inserted_file_path)
             check_file_exist_and_readable(file_path=self.features_extracted_file_path)
             self.data_df = read_df(self.targets_inserted_file_path, self.file_type)
             self.data_df_features = read_df(self.features_extracted_file_path, self.file_type)
             missing_idx = self.data_df_features.index.difference(self.data_df.index)
             if len(missing_idx) > 0:
                 self.data_df_features = self.data_df_features.iloc[self.data_df_features.index.difference(self.data_df.index)]
-                self.data_df = pd.concat([self.data_df, self.data_df_features], axis=0).sort_index()
+                self.data_df = pd.concat([self.data_df.astype(int), self.data_df_features], axis=0).sort_index()
             self.main_window.title('SIMBA ANNOTATION INTERFACE (CONTINUING ANNOTATIONS) - {}'.format(self.video_name))
             self.frm_no = read_config_entry(self.config, 'Last saved frames', self.video_name, data_type='int', default_value=0)
 
         else:
             if setting == 'from_scratch':
                 check_file_exist_and_readable(file_path=self.features_extracted_file_path)
                 self.data_df = read_df(self.features_extracted_file_path, self.file_type)
@@ -120,29 +120,28 @@
         self.select_frm_btn.grid(row=2, column=1, sticky=N)
         self.jump_frame.grid(row=2, column=0)
         self.jump.grid(row=0, column=0, sticky=W)
         self.jump_size.grid(row=0, column=1, sticky=W)
         self.jump_back.grid(row=0, column=2, sticky=E)
         self.jump_forward.grid(row=0, column=3, sticky=W)
 
-        ## Behavior Checkbox
         self.check_frame = Frame(self.main_window, bd=2, width=300, height=500)
         self.check_frame.grid(row=0, column=1)
         self.check_behavior_lbl = Label(self.check_frame, text="Check Behavior:")
         self.check_behavior_lbl.config(font=("Calibri", 16))
         self.check_behavior_lbl.grid(sticky=N)
 
         self.checkboxes = {}
         for target_cnt, target in enumerate(self.target_lst):
             self.checkboxes[target] = {}
             self.checkboxes[target]['name'] = target
-            self.checkboxes[target]['var'] = IntVar()
+            self.checkboxes[target]['var'] = IntVar(value=self.data_df_targets[target].iloc[self.current_frm_n.get()])
             self.checkboxes[target]['cb'] = Checkbutton(self.check_frame, text=target, variable=self.checkboxes[target]['var'], command=lambda k=self.checkboxes[target]['name']: self.save_behavior_in_frm(frame_number=int(self.current_frm_n.get()), target=k))
             self.checkboxes[target]['cb'].grid(row=target_cnt + 1, sticky=W)
-            self.checkboxes[target]['var'].set(self.data_df_targets[target].iloc[self.current_frm_n.get()])
+
 
         self.range_on = IntVar(value=0)
         self.range_frames = Frame(self.main_window)
         self.range_frames.grid(row=1, column=1, sticky=S)
         self.select_range = Checkbutton(self.range_frames, text='Frame range', variable=self.range_on)
         self.select_range.grid(row=0, column=0, sticky=W)
         self.first_frame = Entry(self.range_frames, width=7)
@@ -177,15 +176,15 @@
                                  '\n Left Arrow = -1 frame'
                                  '\n Ctrl + s = Save annotations file'
                                  '\n Ctrl + a = +1 frame and keep choices'
                                  '\n Ctrl + p = Show annotation statistics'
                                  '\n Ctrl + l = Last frame'
                                  '\n Ctrl + o = First frame')
         self.key_presses_lbl.grid(sticky=S)
-        self.__read_frm(frm_number=0)
+        self.__advance_frame(new_frm_number=self.frm_no)
         self.main_window.mainloop()
 
     def __bind_shortcut_keys(self):
         self.main_window.bind('<Control-s>', lambda x: self.__save_results())
         self.main_window.bind('<Control-a>', lambda x: self.__advance_frame(new_frm_number=int(self.current_frm_n.get() + 1), save_and_keep_checks=True))
         self.main_window.bind('<Control-p>', lambda x: self.print_annotation_statistics())
         self.main_window.bind('<Right>', lambda x: self.__advance_frame(new_frm_number= int(self.current_frm_n.get() + 1)))
@@ -227,15 +226,15 @@
         self.current_frm_pil = Image.fromarray(self.current_frm_npy)
         self.current_frm_pil.thumbnail(self.max_frm_size, Image.ANTIALIAS)
         self.current_frm_pil = ImageTk.PhotoImage(master=self.main_window, image=self.current_frm_pil)
         self.video_frame = Label(self.main_window, image=self.current_frm_pil)
         self.video_frame.image = self.current_frm_pil
         self.video_frame.grid(row=0, column=0)
 
-    def __advance_frame(self, new_frm_number: int=None, save_and_keep_checks=False):
+    def __advance_frame(self, new_frm_number: int, save_and_keep_checks=False):
         if new_frm_number > self.max_frm_no:
             print("FRAME {} CANNOT BE SHOWN - YOU ARE VIEWING THE FINAL FRAME OF THE VIDEO (FRAME NUMBER {})".format(str(new_frm_number), str(self.max_frm_no)))
             self.current_frm_n = IntVar(value=self.max_frm_no)
             self.change_frm_box.delete(0, END)
             self.change_frm_box.insert(0, self.current_frm_n.get())
         elif new_frm_number < 0:
             print("FRAME {} CANNOT BE SHOWN - YOU ARE VIEWING THE FIRST FRAME OF THE VIDEO (FRAME NUMBER {})".format(str(new_frm_number), str(self.max_frm_no)))
@@ -245,15 +244,15 @@
         else:
             self.__create_print_statements()
             self.current_frm_n = IntVar(value=new_frm_number)
             self.change_frm_box.delete(0, END)
             self.change_frm_box.insert(0, self.current_frm_n.get())
             if not save_and_keep_checks:
                 for target in self.target_lst:
-                    self.checkboxes[target]['var'].set(self.data_df_targets[target].loc[int(self.current_frm_n.get())])
+                    self.checkboxes[target]['var'].set(bool(self.data_df_targets[target].loc[int(self.current_frm_n.get())]))
             else:
                 for target in self.target_lst:
                     self.checkboxes[target]['var'].set(self.data_df_targets[target].loc[int(self.current_frm_n.get() -1)])
                     self.save_behavior_in_frm(target=target)
             self.__read_frm(frm_number=int(self.current_frm_n.get()))
 
 
@@ -268,23 +267,23 @@
                     self.data_df_targets[target].loc[frm_no] = self.checkboxes[target]['var'].get()
             self.__read_frm(frm_number=int(end_frm))
             self.change_frm_box.delete(0, END)
             self.change_frm_box.insert(0, end_frm)
         self.__create_print_statements(frame_range=True, start_frame=start_frm, end_frame=end_frm)
 
     def save_behavior_in_frm(self, frame_number=None, target=None):
-        self.data_df_targets[target].loc[int(self.current_frm_n.get())] = self.checkboxes[target]['var'].get()
+        self.data_df_targets[target].loc[int(self.current_frm_n.get())] = int(self.checkboxes[target]['var'].get())
 
     def __save_results(self):
         self.save_df = read_df(self.features_extracted_file_path, self.file_type)
         self.save_df = pd.concat([self.save_df, self.data_df_targets], axis=1)
         try:
             write_df(self.save_df, self.file_type, self.targets_inserted_file_path)
         except Exception as e:
-            print(e, 'SIMBA ERROR: File for video {} could not be saved.')
+            print(e, f'SIMBA ERROR: File for video {get_fn_ext(self.features_extracted_file_path)[1]} could not be saved.')
             raise FileExistsError
         stdout_success(msg=f'SAVED: Annotation file for video {self.video_name} saved within the project_folder/csv/targets_inserted directory.')
         if not self.config.has_section('Last saved frames'):
             self.config.add_section('Last saved frames')
         self.config.set('Last saved frames', str(self.video_name), str(self.current_frm_n.get()))
         with open(self.config_path, 'w') as configfile:
             self.config.write(configfile)
@@ -320,23 +319,22 @@
              check_float(name=k, value=float(v.entry_get), min_value=0.0, max_value=1.0)
              threshold_dict_values[k] = float(v.entry_get)
         threshold_dict = threshold_dict_values
 
     check_file_exist_and_readable(video_file_path)
     video_meta = get_video_meta_data(video_file_path)
     _, video_name, _ = get_fn_ext(video_file_path)
-    print(threshold_dict)
 
 
     print('ANNOTATING VIDEO {}: '.format(video_name))
     print('VIDEO INFO')
     print(video_meta)
     _ = LabellingInterface(config_path=config_path,
                           file_path=video_file_path,
                           threshold_dict=threshold_dict,
                           setting=setting,
                           continuing=continuing)
 
-# test = select_labelling_video(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini',
-#                           threshold_dict={'Attack': 0.4},
-#                           setting='from_scratch',
-#                           continuing=False)
+# test = select_labelling_video(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                               threshold_dict={'Attack': 0.4},
+#                               setting='from_scratch',
+#                               continuing=True)
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.63.5/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.63.5/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.63.5/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.63.5/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0001 4e31 0000 000b 005f 005f 0070  ....N1....._._.p
+00000130: 0000 0005 1733 0000 000b 005f 005f 0070  .....3....._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 84f5 b3f1  moDDblob........
-00000160: cc0c c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 a32a e599  moDDblob.....*..
+00000160: 8d20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 84f5 b3f1 cc0c  dDblob..........
+00000180: 6444 626c 6f62 0000 0008 a32a e599 8d20  dDblob.....*... 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0001 a000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0006 a000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-00000000: 0000 0001 4275 6431 0000 2800 0000 0800  ....Bud1..(.....
-00000010: 0000 2800 0000 300c 0000 100c 0000 400c  ..(...0.......@.
+00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
+00000010: 0000 1800 0000 300c 0000 100b 0000 400c  ......0.......@.
 00000020: 0000 500c 0000 0000 0000 0000 0000 0800  ..P.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 000a 0000 0002 0000 00ba  ................
-00000050: 0000 000c 0000 1000 0078 0069 006e 0073  .........x.i.n.s
-00000060: 6c73 7670 0000 0000 0000 0000 0000 0000  lsvp............
+00000050: 0000 000c 0000 1000 006f 0074 0074 0069  .........o.t.t.i
+00000060: 006e 0067 0000 0000 0000 0000 0000 0000  .n.g............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -59,69 +59,69 @@
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0003 0000 0001 0000 000b  ................
-00000410: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00000420: 6c73 7670 626c 6f62 0000 0266 6270 6c69  lsvpblob...fbpli
-00000430: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00000440: 1a45 4647 0a5f 1012 7669 6577 4f70 7469  .EFG._..viewOpti
-00000450: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-00000460: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00000470: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00000480: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
-00000490: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
-000004a0: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
-000004b0: 6976 6544 6174 6573 1001 09d9 0c0d 0e0f  iveDates........
-000004c0: 1011 1213 1415 1e23 272b 3035 3a3f 5863  .......#'+05:?Xc
-000004d0: 6f6d 6d65 6e74 735e 6461 7465 4c61 7374  omments^dateLast
-000004e0: 4f70 656e 6564 5c64 6174 654d 6f64 6966  Opened\dateModif
-000004f0: 6965 645b 6461 7465 4372 6561 7465 6454  ied[dateCreatedT
-00000500: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
-00000510: 7665 7273 696f 6e54 6e61 6d65 d416 1718  versionTname....
-00000520: 191a 1b0a 1d57 7669 7369 626c 6555 7769  .....WvisibleUwi
-00000530: 6474 6859 6173 6365 6e64 696e 6755 696e  dthYascendingUin
-00000540: 6465 7808 1101 2c09 1007 d416 1718 191a  dex...,.........
-00000550: 201a 2208 10c8 0810 08d4 1617 1819 0a25   ."............%
-00000560: 1a09 0910 b508 d416 1718 191a 251a 2a08  ............%.*.
-00000570: 0810 02d4 1617 1819 0a2d 1a2f 0910 6108  .........-./..a.
-00000580: 1003 d416 1718 191a 320a 3408 1064 0910  ........2.4..d..
-00000590: 05d4 1617 1819 0a37 0a39 0910 7309 1004  .......7.9..s...
-000005a0: d416 1718 191a 3c0a 3e08 104b 0910 06d4  ......<.>..K....
-000005b0: 1617 1819 0a41 0a43 0911 01c7 0910 0008  .....A.C........
-000005c0: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
-000005d0: 6469 6669 6564 2340 3000 0000 0000 0009  dified#@0.......
-000005e0: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
-000005f0: 0079 008c 008e 008f 00a2 00ab 00ba 00c7  .y..............
-00000600: 00d3 00d8 00de 00e3 00eb 00f0 00f9 0101  ................
-00000610: 0107 0111 0117 0118 011b 011c 011e 0127  ...............'
-00000620: 0128 012a 012b 012d 0136 0137 0139 013a  .(.*.+.-.6.7.9.:
-00000630: 0143 0144 0145 0147 0150 0151 0153 0154  .C.D.E.G.P.Q.S.T
-00000640: 0156 015f 0160 0162 0163 0165 016e 016f  .V._.`.b.c.e.n.o
-00000650: 0171 0172 0174 017d 017e 0180 0181 0183  .q.r.t.}.~......
-00000660: 018c 018d 0190 0191 0193 0194 019d 01aa  ................
-00000670: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
-00000680: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00000690: 01b4 6564 0808 d40d 0e0f 1024 2518 0a54  ..ed.......$%..T
-000006a0: 7369 7a65 1061 0809 d40d 0e0f 1029 2a0a  size.a.......)*.
-000006b0: 0a54 6b69 6e64 1073 0909 d40d 0e0f 102e  .Tkind.s........
-000006c0: 2f0a 1855 6c61 6265 6c10 6409 08d4 0d0e  /..Ulabel.d.....
-000006d0: 0f10 3334 0a18 5776 6572 7369 6f6e 104b  ..34..Wversion.K
-000006e0: 0908 d40d 0e0f 1038 390a 1858 636f 6d6d  .......89..Xcomm
-000006f0: 656e 7473 1101 2c09 08d4 0d0e 0f10 3d3e  ents..,.......=>
-00000700: 1818 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-00000710: 6410 c808 08d4 0d0e 0f10 421c 1818 5964  d.........B...Yd
-00000720: 6174 6541 6464 6564 0808 0823 4028 0000  ateAdded...#@(..
-00000730: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00000740: 6409 1001 0008 0019 0022 0034 003c 0050  d........".4.<.P
-00000750: 0059 0064 0077 008c 0095 0096 00a2 00ab  .Y.d.w..........
-00000760: 00b6 00bc 00c6 00ce 00d3 00d6 00d7 00d8  ................
-00000770: 00e1 00ea 00ec 00ed 00ee 00f7 00f8 00fa  ................
+00000410: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
+00000420: 006e 0067 6c73 7643 626c 6f62 0000 0349  .n.glsvCblob...I
+00000430: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+00000440: 0809 0a0b 0c0d 1858 595a 5b0c 5d58 6963  .......XYZ[.]Xic
+00000450: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00000460: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00000470: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00000480: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
+00000490: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
+000004a0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+000004b0: 585a 736f 7274 436f 6c75 6d6e 5f10 1075  XZsortColumn_..u
+000004c0: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
+000004d0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+000004e0: 7369 6f6e 2340 3000 0000 0000 0009 ae0e  sion#@0.........
+000004f0: 171c 2125 2a2f 3439 3e43 474f 53d4 0f10  ..!%*/49>CGOS...
+00000500: 1112 0c14 0c16 5776 6973 6962 6c65 5577  ......WvisibleUw
+00000510: 6964 7468 5961 7363 656e 6469 6e67 5a69  idthYascendingZi
+00000520: 6465 6e74 6966 6965 7209 1101 c709 546e  dentifier.....Tn
+00000530: 616d 65d4 0f10 1112 1819 181b 0810 2308  ame...........#.
+00000540: 5875 6269 7175 6974 79d4 0f10 1112 0c1e  Xubiquity.......
+00000550: 1820 0910 b508 5c64 6174 654d 6f64 6966  . ....\dateModif
+00000560: 6965 64d4 0f10 1112 181e 1824 0808 5b64  ied........$..[d
+00000570: 6174 6543 7265 6174 6564 d40f 1011 120c  ateCreated......
+00000580: 2718 2909 1061 0854 7369 7a65 d40f 1011  '.)..a.Tsize....
+00000590: 120c 2c0c 2e09 1073 0954 6b69 6e64 d40f  ..,....s.Tkind..
+000005a0: 1011 1218 310c 3308 1064 0955 6c61 6265  ....1.3..d.Ulabe
+000005b0: 6cd4 0f10 1112 1836 0c38 0810 4b09 5776  l......6.8..K.Wv
+000005c0: 6572 7369 6f6e d40f 1011 1218 3b0c 3d08  ersion......;.=.
+000005d0: 1101 2c09 5863 6f6d 6d65 6e74 73d4 0f10  ..,.Xcomments...
+000005e0: 1112 1840 1842 0810 c808 5e64 6174 654c  ...@.B....^dateL
+000005f0: 6173 744f 7065 6e65 64d4 0f10 1112 181e  astOpened.......
+00000600: 1846 0808 5964 6174 6541 6464 6564 d448  .F..YdateAdded.H
+00000610: 494a 1218 4c18 4e57 7669 7369 626c 6555  IJ..L.NWvisibleU
+00000620: 7769 6474 6859 6173 6365 6e64 696e 6708  widthYascending.
+00000630: 10d2 085a 7368 6172 654f 776e 6572 d448  ...ZshareOwner.H
+00000640: 494a 1218 4c18 5208 085f 100f 7368 6172  IJ..L.R.._..shar
+00000650: 654c 6173 7445 6469 746f 72d4 4849 4a12  eLastEditor.HIJ.
+00000660: 184c 1856 0808 5f10 1069 6e76 6974 6174  .L.V.._..invitat
+00000670: 696f 6e53 7461 7475 7308 2340 5e40 0000  ionStatus.#@^@..
+00000680: 0000 0023 4028 0000 0000 0000 2340 0000  ...#@(......#@..
+00000690: 0000 0000 0054 6e61 6d65 0910 0100 0800  .....Tname......
+000006a0: 1d00 2600 3800 4000 5400 6600 6f00 8100  ..&.8.@.T.f.o...
+000006b0: 8c00 9f00 b400 bd00 be00 cd00 d600 de00  ................
+000006c0: e400 ee00 f900 fa00 fd00 fe01 0301 0c01  ................
+000006d0: 0d01 0f01 1001 1901 2201 2301 2501 2601  ........".#.%.&.
+000006e0: 3301 3c01 3d01 3e01 4a01 5301 5401 5601  3.<.=.>.J.S.T.V.
+000006f0: 5701 5c01 6501 6601 6801 6901 6e01 7701  W.\.e.f.h.i.n.w.
+00000700: 7801 7a01 7b01 8101 8a01 8b01 8d01 8e01  x.z.{...........
+00000710: 9601 9f01 a001 a301 a401 ad01 b601 b701  ................
+00000720: b901 ba01 c901 d201 d301 d401 de01 e701  ................
+00000730: ef01 f501 ff02 0002 0202 0302 0e02 1702  ................
+00000740: 1802 1902 2b02 3402 3502 3602 4902 4a02  ....+.4.5.6.I.J.
+00000750: 5302 5c02 6502 6a02 6b00 0000 0000 0002  S.\.e.j.k.......
+00000760: 0100 0000 0000 0000 5e00 0000 0000 0000  ........^.......
+00000770: 0000 0000 0000 0002 6dee 00f7 00f8 00fa  ........m.......
 00000780: 00fb 0108 0111 011d 011e 011f 0128 012d  .............(.-
 00000790: 012f 0130 0131 013a 013f 0141 0142 0143  ./.0.1.:.?.A.B.C
 000007a0: 014c 0152 0154 0155 0156 015f 0167 0169  .L.R.T.U.V._.g.i
 000007b0: 016a 016b 0174 017d 0180 0181 0182 018b  .j.k.t.}........
 000007c0: 019a 019c 019d 019e 01a7 01b1 01b2 01b3  ................
 000007d0: 01b4 01bd 01ca 01cb 0000 0000 0000 0201  ................
 000007e0: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
@@ -250,147 +250,147 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0002 0000 0005 0000 0007  ................
-00001010: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00001020: 006e 0067 6c73 7643 626c 6f62 0000 02b8  .n.glsvCblob....
-00001030: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00001040: 0809 0a0b 0c0d 1848 4948 4a4b 0c5f 1012  .......HIHJK._..
-00001050: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00001060: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00001070: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00001080: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00001090: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-000010a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-000010b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-000010c0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-000010d0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-000010e0: 6174 6573 1001 09ab 0e17 1c21 252a 2f34  ates.......!%*/4
-000010f0: 393e 43d4 0f10 1112 0c14 0c16 5776 6973  9>C.........Wvis
-00001100: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-00001110: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
-00001120: 1101 c709 546e 616d 65d4 0f10 1112 1819  ....Tname.......
-00001130: 181b 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
-00001140: 0f10 1112 0c1e 1820 0910 b508 5c64 6174  ....... ....\dat
-00001150: 654d 6f64 6966 6965 64d4 0f10 1112 181e  eModified.......
-00001160: 1824 0808 5b64 6174 6543 7265 6174 6564  .$..[dateCreated
-00001170: d40f 1011 120c 2718 2909 1061 0854 7369  ......'.)..a.Tsi
-00001180: 7a65 d40f 1011 120c 2c0c 2e09 1073 0954  ze......,....s.T
-00001190: 6b69 6e64 d40f 1011 1218 310c 3308 1064  kind......1.3..d
-000011a0: 0955 6c61 6265 6cd4 0f10 1112 1836 0c38  .Ulabel......6.8
-000011b0: 0810 4b09 5776 6572 7369 6f6e d40f 1011  ..K.Wversion....
-000011c0: 1218 3b0c 3d08 1101 2c09 5863 6f6d 6d65  ..;.=...,.Xcomme
-000011d0: 6e74 73d4 0f10 1112 1840 1842 0810 c808  nts......@.B....
-000011e0: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
-000011f0: 0f10 1112 181e 1846 0808 5964 6174 6541  .......F..YdateA
-00001200: 6464 6564 0823 0000 0000 0000 0000 2340  dded.#........#@
-00001210: 2800 0000 0000 005c 6461 7465 4d6f 6469  (......\dateModi
-00001220: 6669 6564 2340 3000 0000 0000 0009 0008  fied#@0.........
-00001230: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
-00001240: 0098 00a1 00b4 00b6 00b7 00c3 00cc 00d4  ................
-00001250: 00da 00e4 00ef 00f0 00f3 00f4 00f9 0102  ................
-00001260: 0103 0105 0106 010f 0118 0119 011b 011c  ................
-00001270: 0129 0132 0133 0134 0140 0149 014a 014c  .).2.3.4.@.I.J.L
-00001280: 014d 0152 015b 015c 015e 015f 0164 016d  .M.R.[.\.^._.d.m
-00001290: 016e 0170 0171 0177 0180 0181 0183 0184  .n.p.q.w........
-000012a0: 018c 0195 0196 0199 019a 01a3 01ac 01ad  ................
-000012b0: 01af 01b0 01bf 01c8 01c9 01ca 01d4 01d5  ................
-000012c0: 01de 01e7 01f4 01fd 0000 0000 0000 0201  ................
-000012d0: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
-000012e0: 0000 0000 0000 01fe 0000 0008 0000 000e  ................
-000012f0: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
-00001300: 006f 0072 0074 0065 0072 0073 6c73 7643  .o.r.t.e.r.slsvC
-00001310: 626c 6f62 0000 0281 6270 6c69 7374 3030  blob....bplist00
-00001320: d801 0203 0405 0607 0809 0a0b 1846 4748  .............FGH
-00001330: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
-00001340: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-00001350: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00001360: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00001370: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00001380: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-00001390: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-000013a0: 6174 6573 1001 09ab 0c15 1a1f 2328 2d32  ates........#(-2
-000013b0: 373c 41d4 0d0e 0f10 1112 0a0a 5a69 6465  7<A.........Zide
-000013c0: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
-000013d0: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
-000013e0: 6e61 6d65 1101 c709 09d4 0d0e 0f10 1617  name............
-000013f0: 1818 5875 6269 7175 6974 7910 2308 08d4  ..Xubiquity.#...
-00001400: 0d0e 0f10 1b1c 180a 5c64 6174 654d 6f64  ........\dateMod
-00001410: 6966 6965 6410 b508 09d4 0d0e 0f10 201c  ified......... .
-00001420: 1818 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00001430: d40d 0e0f 1024 2518 0a54 7369 7a65 1061  .....$%..Tsize.a
-00001440: 0809 d40d 0e0f 1029 2a0a 0a54 6b69 6e64  .......)*..Tkind
-00001450: 1073 0909 d40d 0e0f 102e 2f0a 1855 6c61  .s......../..Ula
-00001460: 6265 6c10 6409 08d4 0d0e 0f10 3334 0a18  bel.d.......34..
-00001470: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
-00001480: 1038 390a 1858 636f 6d6d 656e 7473 1101  .89..Xcomments..
-00001490: 2c09 08d4 0d0e 0f10 3d3e 1818 5e64 6174  ,.......=>..^dat
-000014a0: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
-000014b0: 0d0e 0f10 421c 1818 5964 6174 6541 6464  ....B...YdateAdd
-000014c0: 6564 0808 0823 4028 0000 0000 0000 5c64  ed...#@(......\d
-000014d0: 6174 654d 6f64 6966 6965 6423 4030 0000  ateModified#@0..
-000014e0: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
-000014f0: 5c00 6500 7000 7900 8c00 8e00 8f00 9b00  \.e.p.y.........
-00001500: a400 af00 b500 bf00 c700 cc00 cf00 d000  ................
-00001510: d100 da00 e300 e500 e600 e700 f000 fd00  ................
-00001520: ff01 0001 0101 0a01 1601 1701 1801 2101  ..............!.
-00001530: 2601 2801 2901 2a01 3301 3801 3a01 3b01  &.(.).*.3.8.:.;.
-00001540: 3c01 4501 4b01 4d01 4e01 4f01 5801 6001  <.E.K.M.N.O.X.`.
-00001550: 6201 6301 6401 6d01 7601 7901 7a01 7b01  b.c.d.m.v.y.z.{.
-00001560: 8401 9301 9501 9601 9701 a001 aa01 ab01  ................
-00001570: ac01 ad01 b601 c301 cc00 0000 0000 0002  ................
-00001580: 0100 0000 0000 0000 4a00 0000 0000 0000  ........J.......
-00001590: 0000 0000 0000 0001 cd00 0000 0900 0000  ................
-000015a0: 0900 7200 6f00 6900 5f00 7400 6f00 6f00  ..r.o.i._.t.o.o.
-000015b0: 6c00 736c 7376 7062 6c6f 6200 0002 5e62  l.slsvpblob...^b
-000015c0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
-000015d0: 090a 0b1d 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
-000015e0: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
-000015f0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00001600: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00001610: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-00001620: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
-00001630: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-00001640: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
-00001650: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
-00001660: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
-00001670: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-00001680: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-00001690: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-000016a0: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-000016b0: 1617 1819 1a1b 0a1d 5569 6e64 6578 5577  ........UindexUw
-000016c0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-000016d0: 6973 6962 6c65 1007 1101 2c09 08d4 1617  isible....,.....
-000016e0: 1819 1f20 1d1d 1008 10c8 0808 d416 1718  ... ............
-000016f0: 1909 241d 0a10 b508 09d4 1617 1819 2824  ..$...........($
-00001700: 1d1d 1002 0808 d416 1718 192c 2d1d 0a10  ...........,-...
-00001710: 0310 6108 09d4 1617 1819 3132 0a1d 1005  ..a.......12....
-00001720: 1064 0908 d416 1718 1936 370a 0a10 0410  .d.......67.....
-00001730: 7309 09d4 1617 1819 3b3c 0a1d 1006 104b  s.......;<.....K
-00001740: 0908 d416 1718 1940 410a 0a10 0011 01c7  .......@A.......
-00001750: 0909 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00001760: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
-00001770: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
-00001780: 8e00 8f00 a200 ab00 ba00 c700 d300 d800  ................
-00001790: de00 e300 eb00 f000 f900 ff01 0501 0f01  ................
-000017a0: 1701 1901 1c01 1d01 1e01 2701 2901 2b01  ..........'.).+.
-000017b0: 2c01 2d01 3601 3801 3901 3a01 4301 4501  ,.-.6.8.9.:.C.E.
-000017c0: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
-000017d0: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
-000017e0: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
-000017f0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
-00001800: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
-00001810: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
-00001820: 0c00 0000 0200 7500 6976 5372 6e6c 6f6e  ......u.ivSrnlon
-00001830: 6700 0000 0100 0000 0d00 0000 0500 7500  g.............u.
-00001840: 7400 6900 6c00 7364 7363 6c62 6f6f 6c00  t.i.l.sdsclbool.
+00001000: 0000 0000 0000 0002 0000 0004 0000 0008  ................
+00001010: 0000 000e 0070 006f 0073 0065 005f 0069  .....p.o.s.e._.i
+00001020: 006d 0070 006f 0072 0074 0065 0072 0073  .m.p.o.r.t.e.r.s
+00001030: 6c73 7643 626c 6f62 0000 0281 6270 6c69  lsvCblob....bpli
+00001040: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+00001050: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
+00001060: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+00001070: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00001080: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00001090: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
+000010a0: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
+000010b0: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
+000010c0: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
+000010d0: 2328 2d32 373c 41d4 0d0e 0f10 1112 0a0a  #(-27<A.........
+000010e0: 5a69 6465 6e74 6966 6965 7255 7769 6474  ZidentifierUwidt
+000010f0: 6859 6173 6365 6e64 696e 6757 7669 7369  hYascendingWvisi
+00001100: 626c 6554 6e61 6d65 1101 c709 09d4 0d0e  bleTname........
+00001110: 0f10 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
+00001120: 2308 08d4 0d0e 0f10 1b1c 180a 5c64 6174  #...........\dat
+00001130: 654d 6f64 6966 6965 6410 b508 09d4 0d0e  eModified.......
+00001140: 0f10 201c 1818 5b64 6174 6543 7265 6174  .. ...[dateCreat
+00001150: 6564 0808 d40d 0e0f 1024 2518 0a54 7369  ed.......$%..Tsi
+00001160: 7a65 1061 0809 d40d 0e0f 1029 2a0a 0a54  ze.a.......)*..T
+00001170: 6b69 6e64 1073 0909 d40d 0e0f 102e 2f0a  kind.s......../.
+00001180: 1855 6c61 6265 6c10 6409 08d4 0d0e 0f10  .Ulabel.d.......
+00001190: 3334 0a18 5776 6572 7369 6f6e 104b 0908  34..Wversion.K..
+000011a0: d40d 0e0f 1038 390a 1858 636f 6d6d 656e  .....89..Xcommen
+000011b0: 7473 1101 2c09 08d4 0d0e 0f10 3d3e 1818  ts..,.......=>..
+000011c0: 5e64 6174 654c 6173 744f 7065 6e65 6410  ^dateLastOpened.
+000011d0: c808 08d4 0d0e 0f10 421c 1818 5964 6174  ........B...Ydat
+000011e0: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
+000011f0: 0000 5c64 6174 654d 6f64 6966 6965 6423  ..\dateModified#
+00001200: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
+00001210: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
+00001220: 8f00 9b00 a400 af00 b500 bf00 c700 cc00  ................
+00001230: cf00 d000 d100 da00 e300 e500 e600 e700  ................
+00001240: f000 fd00 ff01 0001 0101 0a01 1601 1701  ................
+00001250: 1801 2101 2601 2801 2901 2a01 3301 3801  ..!.&.(.).*.3.8.
+00001260: 3a01 3b01 3c01 4501 4b01 4d01 4e01 4f01  :.;.<.E.K.M.N.O.
+00001270: 5801 6001 6201 6301 6401 6d01 7601 7901  X.`.b.c.d.m.v.y.
+00001280: 7a01 7b01 8401 9301 9501 9601 9701 a001  z.{.............
+00001290: aa01 ab01 ac01 ad01 b601 c301 cc00 0000  ................
+000012a0: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
+000012b0: 0000 0000 0000 0000 0000 0001 cd00 0000  ................
+000012c0: 0900 0000 0900 7200 6f00 6900 5f00 7400  ......r.o.i._.t.
+000012d0: 6f00 6f00 6c00 736c 7376 7062 6c6f 6200  o.o.l.slsvpblob.
+000012e0: 0002 5e62 706c 6973 7430 30d8 0102 0304  ..^bplist00.....
+000012f0: 0506 0708 090a 0b1d 4546 470a 5f10 1276  ........EFG._..v
+00001300: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00001310: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00001320: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00001330: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00001340: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00001350: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
+00001360: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
+00001370: 0109 d90c 0d0e 0f10 1112 1314 151e 2327  ..............#'
+00001380: 2b30 353a 3f58 636f 6d6d 656e 7473 5e64  +05:?Xcomments^d
+00001390: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+000013a0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+000013b0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+000013c0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+000013d0: 616d 65d4 1617 1819 1a1b 0a1d 5569 6e64  ame.........Uind
+000013e0: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
+000013f0: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
+00001400: 08d4 1617 1819 1f20 1d1d 1008 10c8 0808  ....... ........
+00001410: d416 1718 1909 241d 0a10 b508 09d4 1617  ......$.........
+00001420: 1819 2824 1d1d 1002 0808 d416 1718 192c  ..($...........,
+00001430: 2d1d 0a10 0310 6108 09d4 1617 1819 3132  -.....a.......12
+00001440: 0a1d 1005 1064 0908 d416 1718 1936 370a  .....d.......67.
+00001450: 0a10 0410 7309 09d4 1617 1819 3b3c 0a1d  ....s.......;<..
+00001460: 1006 104b 0908 d416 1718 1940 410a 0a10  ...K.......@A...
+00001470: 0011 01c7 0909 0823 4028 0000 0000 0000  .......#@(......
+00001480: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
+00001490: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
+000014a0: 7900 8c00 8e00 8f00 a200 ab00 ba00 c700  y...............
+000014b0: d300 d800 de00 e300 eb00 f000 f900 ff01  ................
+000014c0: 0501 0f01 1701 1901 1c01 1d01 1e01 2701  ..............'.
+000014d0: 2901 2b01 2c01 2d01 3601 3801 3901 3a01  ).+.,.-.6.8.9.:.
+000014e0: 4301 4501 4601 4701 5001 5201 5401 5501  C.E.F.G.P.R.T.U.
+000014f0: 5601 5f01 6101 6301 6401 6501 6e01 7001  V._.a.c.d.e.n.p.
+00001500: 7201 7301 7401 7d01 7f01 8101 8201 8301  r.s.t.}.........
+00001510: 8c01 8e01 9101 9201 9301 9401 9d01 a201  ................
+00001520: ab00 0000 0000 0002 0100 0000 0000 0000  ................
+00001530: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
+00001540: ac00 0000 0c00 0000 0200 7500 6976 5372  ..........u.ivSr
+00001550: 6e6c 6f6e 6700 0000 0100 0000 0d00 0000  nlong...........
+00001560: 0500 7500 7400 6900 6c00 7364 7363 6c62  ..u.t.i.l.sdsclb
+00001570: 6f6f 6c00 0000 0000 0000 0000 0000 0000  ool.............
+00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001800: 0000 0000 0000 000e 0000 0000 0000 180b  ................
+00001810: 0000 0045 0000 300c 0000 100b 0000 400c  ...E..0.......@.
+00001820: 0000 500c 0000 600c 0000 700c 0000 800c  ..P...`...p.....
+00001830: 0000 900c 0000 040a 0000 200c 0000 a00c  .......... .....
+00001840: 0000 b00c 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -442,79 +442,79 @@
 00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00001c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000 0000 0006 0000 0002 0000 0004  ................
+00001c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+00001c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001c50: 0100 0002 0000 0000 0000 0000 0100 0008  ................
+00001c60: 0000 0000 0000 0000 0000 0000 0100 00c0  ................
+00001c70: 0000 0000 0000 0000 0100 0100 0000 0000  ................
+00001c80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
+00001c90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
+00001ca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
+00001cb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
+00001cc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
+00001cd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
+00001ce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
+00001cf0: 0074 6543 7265 6174 6564 5473 697a 6555  .teCreatedTsizeU
+00001d00: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00001d10: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
+00001d20: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00001d30: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
+00001d40: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
+00001d50: c808 1008 d419 1718 1624 250a 0a10 0110  .........$%.....
+00001d60: b509 09d4 1617 1819 1a25 1a2b 0808 1002  .........%.+....
+00001d70: d416 1718 190a 2e1a 3009 1061 0810 03d4  ........0..a....
+00001d80: 1617 1819 1a33 0a35 0810 6409 1005 d416  .....3.5..d.....
+00001d90: 1718 190a 380a 3a09 1073 0910 04d4 1617  ....8.:..s......
+00001da0: 1819 1a3d 0a3f 0810 4b09 1006 d416 1718  ...=.?..K.......
+00001db0: 190a 420a 4409 1101 c709 1000 0823 4028  ..B.D........#@(
+00001dc0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
+00001dd0: 6965 6409 0008 0019 0022 0034 003c 0050  ied......".4.<.P
+00001de0: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
+00001df0: 00c1 00ce 00da 00df 00e5 00ea 00f2 00f7  ................
+00001e00: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
+00001e10: 0125 012e 012f 0131 0132 0134 013d 013f  .%.../.1.2.4.=.?
+00001e20: 0141 0142 0143 014c 014d 014e 0150 0159  .A.B.C.L.M.N.P.Y
+00001e30: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
+00001e40: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
+00001e50: 0189 018a 018c 0195 0196 0199 019a 019c  ................
+00001e60: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
+00001e70: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+00001e80: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
+00001e90: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00001ea0: 0064 6d6f 4444 626c 6f62 0000 0008 cbf3  .dmoDDblob......
+00001eb0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
+00001ec0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00001ed0: 0064 6d6f 6444 626c 6f62 0000 0008 cbf3  .dmodDblob......
+00001ee0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
+00001ef0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00001f00: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
+00001f10: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+00001f20: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
+00001f30: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
+00001f40: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
+00001f50: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00001f60: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+00001f70: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00001f80: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00001f90: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00001fa0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00001fb0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00001fc0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00001fd0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
+00001fe0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
+00001ff0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
+00002000: 0000 0001 0000 0007 0000 0003 0000 0004  ................
 00002010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
 00002020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
 00002030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
 00002040: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
 00002050: 0405 0607 0809 0a0b 1d45 4647 0a5f 1012  .........EFG._..
 00002060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00002070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
@@ -595,58 +595,58 @@
 00002520: 013b 0147 0150 0151 0153 0154 0159 0162  .;.G.P.Q.S.T.Y.b
 00002530: 0163 0165 0166 016b 0174 0175 0177 0178  .c.e.f.k.t.u.w.x
 00002540: 017e 0187 0188 018a 018b 0193 019c 019d  .~..............
 00002550: 01a0 01a1 01aa 01b3 01b4 01b6 01b7 01c6  ................
 00002560: 01cf 01d0 01d1 01db 01dc 01e5 01ee 01fb  ................
 00002570: 01fc 0000 0000 0000 0201 0000 0000 0000  ................
 00002580: 004d 0000 0000 0000 0000 0000 0000 0000  .M..............
-00002590: 01fe 0000 0000 0001 cd00 0000 0900 0000  ................
-000025a0: 0900 7200 6f00 6900 5f00 7400 6f00 6f00  ..r.o.i._.t.o.o.
-000025b0: 6c00 736c 7376 7062 6c6f 6200 0002 5e62  l.slsvpblob...^b
-000025c0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
-000025d0: 090a 0b1d 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
-000025e0: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
-000025f0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00002600: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00002610: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-00002620: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
-00002630: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-00002640: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
-00002650: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
-00002660: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
-00002670: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-00002680: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-00002690: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-000026a0: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-000026b0: 1617 1819 1a1b 0a1d 5569 6e64 6578 5577  ........UindexUw
-000026c0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-000026d0: 6973 6962 6c65 1007 1101 2c09 08d4 1617  isible....,.....
-000026e0: 1819 1f20 1d1d 1008 10c8 0808 d416 1718  ... ............
-000026f0: 1909 241d 0a10 b508 09d4 1617 1819 2824  ..$...........($
-00002700: 1d1d 1002 0808 d416 1718 192c 2d1d 0a10  ...........,-...
-00002710: 0310 6108 09d4 1617 1819 3132 0a1d 1005  ..a.......12....
-00002720: 1064 0908 d416 1718 1936 370a 0a10 0410  .d.......67.....
-00002730: 7309 09d4 1617 1819 3b3c 0a1d 1006 104b  s.......;<.....K
-00002740: 0908 d416 1718 1940 410a 0a10 0011 01c7  .......@A.......
-00002750: 0909 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00002760: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
-00002770: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
-00002780: 8e00 8f00 a200 ab00 ba00 c700 d300 d800  ................
-00002790: de00 e300 eb00 f000 f900 ff01 0501 0f01  ................
-000027a0: 1701 1901 1c01 1d01 1e01 2701 2901 2b01  ..........'.).+.
-000027b0: 2c01 2d01 3601 3801 3901 3a01 4301 4501  ,.-.6.8.9.:.C.E.
-000027c0: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
-000027d0: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
-000027e0: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
-000027f0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
-00002800: 0000 0002 0000 000e 0000 0000 0000 280b  ..............(.
-00002810: 0000 0045 0000 300c 0000 100c 0000 400c  ...E..0.......@.
-00002820: 0000 500c 0000 600c 0000 700c 0000 800c  ..P...`...p.....
-00002830: 0000 900c 0000 040a 0000 200b 0000 a00c  .......... .....
-00002840: 0000 b00c 0000 0000 0000 0000 0000 0000  ................
+00002590: 01fe 0000 0006 0000 0006 006d 0069 0078  ...........m.i.x
+000025a0: 0069 006e 0073 6c73 7670 626c 6f62 0000  .i.n.slsvpblob..
+000025b0: 0266 6270 6c69 7374 3030 d801 0203 0405  .fbplist00......
+000025c0: 0607 0809 0a0b 1a45 4647 0a5f 1012 7669  .......EFG._..vi
+000025d0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+000025e0: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+000025f0: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00002600: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00002610: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+00002620: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
+00002630: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
+00002640: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
+00002650: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
+00002660: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+00002670: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+00002680: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00002690: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+000026a0: 6d65 d416 1718 191a 1b0a 1d57 7669 7369  me.........Wvisi
+000026b0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+000026c0: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
+000026d0: d416 1718 191a 201a 2208 10c8 0810 08d4  ...... .".......
+000026e0: 1617 1819 0a25 1a09 0910 b508 d416 1718  .....%..........
+000026f0: 191a 251a 2a08 0810 02d4 1617 1819 0a2d  ..%.*..........-
+00002700: 1a2f 0910 6108 1003 d416 1718 191a 320a  ./..a.........2.
+00002710: 3408 1064 0910 05d4 1617 1819 0a37 0a39  4..d.........7.9
+00002720: 0910 7309 1004 d416 1718 191a 3c0a 3e08  ..s.........<.>.
+00002730: 104b 0910 06d4 1617 1819 0a41 0a43 0911  .K.........A.C..
+00002740: 01c7 0910 0008 2340 2800 0000 0000 005c  ......#@(......\
+00002750: 6461 7465 4d6f 6469 6669 6564 2340 3000  dateModified#@0.
+00002760: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+00002770: 005c 0065 0070 0079 008c 008e 008f 00a2  .\.e.p.y........
+00002780: 00ab 00ba 00c7 00d3 00d8 00de 00e3 00eb  ................
+00002790: 00f0 00f9 0101 0107 0111 0117 0118 011b  ................
+000027a0: 011c 011e 0127 0128 012a 012b 012d 0136  .....'.(.*.+.-.6
+000027b0: 0137 0139 013a 0143 0144 0145 0147 0150  .7.9.:.C.D.E.G.P
+000027c0: 0151 0153 0154 0156 015f 0160 0162 0163  .Q.S.T.V._.`.b.c
+000027d0: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
+000027e0: 0180 0181 0183 018c 018d 0190 0191 0193  ................
+000027f0: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
+00002800: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
+00002810: 0000 0000 0000 01b4 0000 0000 0000 0000  ................
+00002820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -698,81 +698,81 @@
 00002b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00002c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+00002c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00002c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00002c50: 0100 0002 0000 0000 0000 0000 0100 0008  ................
-00002c60: 0000 0000 0000 0000 0000 0000 0100 00c0  ................
-00002c70: 0000 0000 0000 0000 0100 0100 0000 0000  ................
-00002c80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
-00002c90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
-00002ca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
-00002cb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
-00002cc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
-00002cd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
-00002ce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002cf0: 0074 6543 7265 6174 6564 5473 697a 6555  .teCreatedTsizeU
-00002d00: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00002d10: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
-00002d20: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-00002d30: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
-00002d40: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
-00002d50: c808 1008 d419 1718 1624 250a 0a10 0110  .........$%.....
-00002d60: b509 09d4 1617 1819 1a25 1a2b 0808 1002  .........%.+....
-00002d70: d416 1718 190a 2e1a 3009 1061 0810 03d4  ........0..a....
-00002d80: 1617 1819 1a33 0a35 0810 6409 1005 d416  .....3.5..d.....
-00002d90: 1718 190a 380a 3a09 1073 0910 04d4 1617  ....8.:..s......
-00002da0: 1819 1a3d 0a3f 0810 4b09 1006 d416 1718  ...=.?..K.......
-00002db0: 190a 420a 4409 1101 c709 1000 0823 4028  ..B.D........#@(
-00002dc0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
-00002dd0: 6965 6409 0008 0019 0022 0034 003c 0050  ied......".4.<.P
-00002de0: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
-00002df0: 00c1 00ce 00da 00df 00e5 00ea 00f2 00f7  ................
-00002e00: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
-00002e10: 0125 012e 012f 0131 0132 0134 013d 013f  .%.../.1.2.4.=.?
-00002e20: 0141 0142 0143 014c 014d 014e 0150 0159  .A.B.C.L.M.N.P.Y
-00002e30: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
-00002e40: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
-00002e50: 0189 018a 018c 0195 0196 0199 019a 019c  ................
-00002e60: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
-00002e70: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
-00002e80: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
-00002e90: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00002ea0: 0064 6d6f 4444 626c 6f62 0000 0008 cbf3  .dmoDDblob......
-00002eb0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
-00002ec0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00002ed0: 0064 6d6f 6444 626c 6f62 0000 0008 cbf3  .dmodDblob......
-00002ee0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
-00002ef0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00002f00: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
-00002f10: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
-00002f20: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
-00002f30: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
-00002f40: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
-00002f50: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-00002f60: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-00002f70: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-00002f80: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-00002f90: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00002fa0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00002fb0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00002fc0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00002fd0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
-00002fe0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
-00002ff0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-00003000: 0000 0001 0000 0000 0000 0010 0000 0005  ................
+00002c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003000: 0000 0000 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0006 78bc 0000 0005 0075  mp......x......u
+00003020: 6d70 0000 0000 0008 6972 0000 0005 0075  mp......ir.....u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,20 +848,20 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 08c6 a590  smoDDblob.......
-00003570: 9d1b 1fc5 4100 0000 0500 7500 7400 6900  ....A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 08c6  l.smodDblob.....
-00003590: a590 9d1b 1fc5 4100 0000 0500 7500 7400  ......A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 0862 b162  smoDDblob....b.b
+00003570: fcec 20c5 4100 0000 0500 7500 7400 6900  .. .A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 0862  l.smodDblob....b
+00003590: b162 fcec 20c5 4100 0000 0500 7500 7400  .b.. .A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 07b0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
+000035b0: 0000 09f0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -876,15 +876,15 @@
 000036b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 000036c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
 000036d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
 000036e0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
 000036f0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
 00003700: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
 00003710: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
-00003720: 7000 0000 0000 0472 6400 0000 1000 7600  p......rd.....v.
+00003720: 7000 0000 0000 05a8 1400 0000 1000 7600  p.............v.
 00003730: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
 00003740: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
 00003750: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
 00003760: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
 00003770: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
 00003780: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00003790: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -971,16 +971,16 @@
 00003ca0: 0073 6d6f 4444 626c 6f62 0000 0008 c1a2  .smoDDblob......
 00003cb0: e9f8 b219 c541 0000 0010 0076 0069 0064  .....A.....v.i.d
 00003cc0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00003cd0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
 00003ce0: 6f62 0000 0008 c1a2 e9f8 b219 c541 0000  ob...........A..
 00003cf0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00003d00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003d10: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
-00003d20: 8000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
+00003d10: 0073 7068 3153 636f 6d70 0000 0000 0007  .sph1Scomp......
+00003d20: 0000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
 00003d30: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00003d40: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
 00003d50: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1034,24 +1034,24 @@
 00004090: 006d 0062 0061 005f 0064 0065 0076 002f  .m.b.a._.d.e.v./
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
-00004100: 005f 6c67 3153 636f 6d70 0000 0000 0001  ._lg1Scomp......
-00004110: 95ea 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
+00004100: 005f 6c67 3153 636f 6d70 0000 0000 0002  ._lg1Scomp......
+00004110: 5c61 0000 000b 005f 005f 0070 0079 0063  \a....._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 170e b937 1d1f c541  blob.......7...A
+00004130: 626c 6f62 0000 0008 cf1a a440 ee20 c541  blob.......@. .A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
-00004160: 6f62 0000 0008 13a7 42bc 1b1f c541 0000  ob......B....A..
+00004160: 6f62 0000 0008 cf1a a440 ee20 c541 0000  ob.......@. .A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
-00004190: 0000 0000 0001 c000 0000 0006 0061 0073  .............a.s
+00004190: 0000 0000 0002 a000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
 000041b0: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
 000041c0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 000041d0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 000041e0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 000041f0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00004200: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
@@ -1206,15 +1206,15 @@
 00004b50: 0000 0000 0000 0000 0000 009b 0000 0012  ................
 00004b60: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 00004b70: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 00004b80: 006c 0073 6473 636c 626f 6f6c 0000 0000  .l.sdsclbool....
 00004b90: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
 00004ba0: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
 00004bb0: 6f00 6c00 736c 6731 5363 6f6d 7000 0000  o.l.slg1Scomp...
-00004bc0: 0000 0244 4800 0000 1200 6200 6f00 7500  ...DH.....b.o.u.
+00004bc0: 0000 02e8 8d00 0000 1200 6200 6f00 7500  ..........b.o.u.
 00004bd0: 6e00 6400 6900 6e00 6700 5f00 6200 6f00  n.d.i.n.g._.b.o.
 00004be0: 7800 5f00 7400 6f00 6f00 6c00 736c 7376  x._.t.o.o.l.slsv
 00004bf0: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
 00004c00: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
 00004c10: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
 00004c20: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
 00004c30: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
@@ -1285,15 +1285,15 @@
 00005040: 1799 b1f1 cc0c c541 0000 0012 0062 006f  .......A.....b.o
 00005050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
 00005060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
 00005070: 6d6f 6444 626c 6f62 0000 0008 1799 b1f1  modDblob........
 00005080: cc0c c541 0000 0012 0062 006f 0075 006e  ...A.....b.o.u.n
 00005090: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
 000050a0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
-000050b0: 636f 6d70 0000 0000 0002 c000 0000 0012  comp............
+000050b0: 636f 6d70 0000 0000 0003 9000 0000 0012  comp............
 000050c0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 000050d0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 000050e0: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 000050f0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 00005100: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
 00005110: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
 00005120: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
@@ -1310,25 +1310,25 @@
 000051d0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 000051e0: 0000 0000 0000 9a00 0000 0f00 6300 7500  ............c.u.
 000051f0: 6500 5f00 6c00 6900 6700 6800 7400 5f00  e._.l.i.g.h.t._.
 00005200: 7400 6f00 6f00 6c00 7364 7363 6c62 6f6f  t.o.o.l.sdsclboo
 00005210: 6c00 0000 000f 0063 0075 0065 005f 006c  l......c.u.e._.l
 00005220: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005230: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
-00005240: 0002 98a5 0000 000f 0063 0075 0065 005f  .........c.u.e._
+00005240: 0003 5665 0000 000f 0063 0075 0065 005f  ..Ve.....c.u.e._
 00005250: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
 00005260: 006f 006c 0073 6d6f 4444 626c 6f62 0000  .o.l.smoDDblob..
 00005270: 0008 00ae d77f cc0c c541 0000 000f 0063  .........A.....c
 00005280: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
 00005290: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
 000052a0: 626c 6f62 0000 0008 00ae d77f cc0c c541  blob...........A
 000052b0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 000052c0: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
-000052d0: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
-000052e0: 7000 0000 000f 0063 0075 0065 005f 006c  p......c.u.e._.l
+000052d0: 0073 7068 3153 636f 6d70 0000 0000 0004  .sph1Scomp......
+000052e0: 8000 0000 000f 0063 0075 0065 005f 006c  .......c.u.e._.l
 000052f0: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005300: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00005310: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
 00005320: 0070 0070 6277 7370 626c 6f62 0000 00c9  .p.pbwspblob....
 00005330: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00005340: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00005350: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
@@ -1370,15 +1370,15 @@
 00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
 000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
 000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
 000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00005600: 0000 0005 24b1 0000 000f 0064 0061 0074  ....$......d.a.t
+00005600: 0000 0006 9ad9 0000 000f 0064 0061 0074  ...........d.a.t
 00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
 00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
 00005630: 0000 0281 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00005640: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
 00005650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00005660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00005670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
@@ -1457,22 +1457,22 @@
 00005b00: 6301 6501 6e01 6f01 7101 7201 7401 7d01  c.e.n.o.q.r.t.}.
 00005b10: 7e01 8001 8101 8301 8c01 8d01 9001 9101  ~...............
 00005b20: 9301 9401 9d01 aa01 b300 0000 0000 0002  ................
 00005b30: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
 00005b40: 0000 0000 0000 0001 b400 0000 0f00 6400  ..............d.
 00005b50: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 00005b60: 6500 7300 7300 6f00 7200 736d 6f44 4462  e.s.s.o.r.smoDDb
-00005b70: 6c6f 6200 0000 082d 2344 c1db 1dc5 4100  lob....-#D....A.
+00005b70: 6c6f 6200 0000 089a 4682 3d7b 20c5 4100  lob.....F.={ .A.
 00005b80: 0000 0f00 6400 6100 7400 6100 5f00 7000  ....d.a.t.a._.p.
 00005b90: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
-00005ba0: 736d 6f64 4462 6c6f 6200 0000 082d 2344  smodDblob....-#D
-00005bb0: c1db 1dc5 4100 0000 0f00 6400 6100 7400  ....A.....d.a.t.
+00005ba0: 736d 6f64 4462 6c6f 6200 0000 089a 4682  smodDblob.....F.
+00005bb0: 3d7b 20c5 4100 0000 0f00 6400 6100 7400  ={ .A.....d.a.t.
 00005bc0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005bd0: 7300 6f00 7200 7370 6831 5363 6f6d 7000  s.o.r.sph1Scomp.
-00005be0: 0000 0000 0690 0000 0000 0f00 6400 6100  ............d.a.
+00005be0: 0000 0000 0880 0000 0000 0f00 6400 6100  ............d.a.
 00005bf0: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
 00005c00: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
 00005c10: 6700 0000 0100 0000 1200 6600 6500 6100  g.........f.e.a.
 00005c20: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00005c30: 7200 6100 6300 7400 6f00 7200 7362 7773  r.a.c.t.o.r.sbws
 00005c40: 7062 6c6f 6200 0000 c962 706c 6973 7430  pblob....bplist0
 00005c50: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
@@ -1489,15 +1489,15 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 093f 8016 4008 10c8  omp......?..@...
+00005d70: 6f6d 7000 0000 0000 0b3d ba16 4008 10c8  omp......=..@...
 00005d80: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
 00005d90: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
 00005da0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
 00005db0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
 00005dc0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
 00005dd0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
 00005de0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
@@ -1586,185 +1586,185 @@
 00006310: 0869 3ef0 203f 0dc5 4100 0000 1200 6600  .i>. ?..A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
 00006340: 736d 6f64 4462 6c6f 6200 0000 0869 3ef0  smodDblob....i>.
 00006350: 203f 0dc5 4100 0000 1200 6600 6500 6100   ?..A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 0b60 0000 0000  Scomp......`....
+00006380: 5363 6f6d 7000 0000 0000 0db0 0000 0000  Scomp...........
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
-000063e0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-000063f0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-00006400: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-00006410: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-00006420: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00006430: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-00006440: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00006450: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00006460: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
-00006470: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
-00006480: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
-00006490: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-000064a0: 0000 0000 0000 0000 0000 009a 0000 0009  ................
-000064b0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
-000064c0: 0067 6c67 3153 636f 6d70 0000 0000 0002  .glg1Scomp......
-000064d0: 35ef 0000 0009 006c 0061 0062 0065 006c  5......l.a.b.e.l
-000064e0: 006c 0069 006e 0067 6c73 7643 626c 6f62  .l.i.n.glsvCblob
-000064f0: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
-00006500: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
-00006510: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00006520: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00006530: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00006540: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00006550: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-00006560: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-00006570: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00006580: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
-00006590: 0d0e 0f10 0a12 0a14 5776 6973 6962 6c65  ........Wvisible
-000065a0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-000065b0: 5a69 6465 6e74 6966 6965 7209 1101 c709  Zidentifier.....
-000065c0: 546e 616d 65d4 0d0e 0f10 1617 1619 0810  Tname...........
-000065d0: 2308 5875 6269 7175 6974 79d4 0d0e 0f10  #.Xubiquity.....
-000065e0: 0a1c 161e 0910 b508 5c64 6174 654d 6f64  ........\dateMod
-000065f0: 6966 6965 64d4 0d0e 0f10 161c 1622 0808  ified........"..
-00006600: 5b64 6174 6543 7265 6174 6564 d40d 0e0f  [dateCreated....
-00006610: 100a 2516 2709 1061 0854 7369 7a65 d40d  ..%.'..a.Tsize..
-00006620: 0e0f 100a 2a0a 2c09 1073 0954 6b69 6e64  ....*.,..s.Tkind
-00006630: d40d 0e0f 1016 2f0a 3108 1064 0955 6c61  ....../.1..d.Ula
-00006640: 6265 6cd4 0d0e 0f10 1634 0a36 0810 4b09  bel......4.6..K.
-00006650: 5776 6572 7369 6f6e d40d 0e0f 1016 390a  Wversion......9.
-00006660: 3b08 1101 2c09 5863 6f6d 6d65 6e74 73d4  ;...,.Xcomments.
-00006670: 0d0e 0f10 163e 1640 0810 c808 5e64 6174  .....>.@....^dat
-00006680: 654c 6173 744f 7065 6e65 64d4 0d0e 0f10  eLastOpened.....
-00006690: 161c 1644 0808 5964 6174 6541 6464 6564  ...D..YdateAdded
-000066a0: 0823 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
-000066b0: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
-000066c0: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
-000066d0: 8f00 9b00 a400 ac00 b200 bc00 c700 c800  ................
-000066e0: cb00 cc00 d100 da00 db00 dd00 de00 e700  ................
-000066f0: f000 f100 f300 f401 0101 0a01 0b01 0c01  ................
-00006700: 1801 2101 2201 2401 2501 2a01 3301 3401  ..!.".$.%.*.3.4.
-00006710: 3601 3701 3c01 4501 4601 4801 4901 4f01  6.7.<.E.F.H.I.O.
-00006720: 5801 5901 5b01 5c01 6401 6d01 6e01 7101  X.Y.[.\.d.m.n.q.
-00006730: 7201 7b01 8401 8501 8701 8801 9701 a001  r.{.............
-00006740: a101 a201 ac01 ad01 b601 bb01 c400 0000  ................
-00006750: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
-00006760: 0000 0000 0000 0000 0000 0001 c500 0000  ................
-00006770: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
-00006780: 6e00 676c 7376 7062 6c6f 6200 0002 5e62  n.glsvpblob...^b
-00006790: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
-000067a0: 090a 0b1d 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
-000067b0: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
-000067c0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-000067d0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-000067e0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-000067f0: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
-00006800: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-00006810: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
-00006820: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
-00006830: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
-00006840: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-00006850: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-00006860: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-00006870: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-00006880: 1617 1819 1a1b 0a1d 5569 6e64 6578 5577  ........UindexUw
-00006890: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-000068a0: 6973 6962 6c65 1007 1101 2c09 08d4 1617  isible....,.....
-000068b0: 1819 1f20 1d1d 1008 10c8 0808 d416 1718  ... ............
-000068c0: 1909 241d 0a10 b508 09d4 1617 1819 2824  ..$...........($
-000068d0: 1d1d 1002 0808 d416 1718 192c 2d1d 0a10  ...........,-...
-000068e0: 0310 6108 09d4 1617 1819 3132 0a1d 1005  ..a.......12....
-000068f0: 1064 0908 d416 1718 1936 370a 0a10 0410  .d.......67.....
-00006900: 7309 09d4 1617 1819 3b3c 0a1d 1006 104b  s.......;<.....K
-00006910: 0908 d416 1718 1940 410a 0a10 0011 01c7  .......@A.......
-00006920: 0909 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00006930: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
-00006940: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
-00006950: 8e00 8f00 a200 ab00 ba00 c700 d300 d800  ................
-00006960: de00 e300 eb00 f000 f900 ff01 0501 0f01  ................
-00006970: 1701 1901 1c01 1d01 1e01 2701 2901 2b01  ..........'.).+.
-00006980: 2c01 2d01 3601 3801 3901 3a01 4301 4501  ,.-.6.8.9.:.C.E.
-00006990: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
-000069a0: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
-000069b0: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
-000069c0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
-000069d0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
-000069e0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
-000069f0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
-00006a00: 6e00 676d 6f44 4462 6c6f 6200 0000 0834  n.gmoDDblob....4
-00006a10: 23b2 c431 1bc5 4100 0000 0900 6c00 6100  #..1..A.....l.a.
-00006a20: 6200 6500 6c00 6c00 6900 6e00 676d 6f64  b.e.l.l.i.n.gmod
-00006a30: 4462 6c6f 6200 0000 0834 23b2 c431 1bc5  Dblob....4#..1..
-00006a40: 4100 0000 0900 6c00 6100 6200 6500 6c00  A.....l.a.b.e.l.
-00006a50: 6c00 6900 6e00 6770 6831 5363 6f6d 7000  l.i.n.gph1Scomp.
-00006a60: 0000 0000 0290 0000 0000 0900 6c00 6100  ............l.a.
-00006a70: 6200 6500 6c00 6c00 6900 6e00 6776 5372  b.e.l.l.i.n.gvSr
-00006a80: 6e6c 6f6e 6700 0000 0100 0000 0600 6d00  nlong.........m.
-00006a90: 6900 7800 6900 6e00 7362 7773 7062 6c6f  i.x.i.n.sbwspblo
-00006aa0: 6200 0000 c862 706c 6973 7430 30d7 0102  b....bplist00...
-00006ab0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-00006ac0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-00006ad0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-00006ae0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-00006af0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-00006b00: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-00006b20: 0908 095f 1017 7b7b 302c 2031 3035 7d2c  ..._..{{0, 105},
-00006b30: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
-00006b40: 2531 3d49 606d 797a 7b7c 7d7e 9800 0000  %1=I`myz{|}~....
-00006b50: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00006b60: 0000 0000 0000 0000 0000 0000 9900 0000  ................
-00006b70: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
-00006b80: 5363 6f6d 7000 0000 0000 0d3e 5500 0000  Scomp......>U...
-00006b90: 0600 6d00 6900 7800 6900 6e00 736c 7376  ..m.i.x.i.n.slsv
-00006ba0: 4362 6c6f 6200 0002 8162 706c 6973 7430  Cblob....bplist0
-00006bb0: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
-00006bc0: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
-00006bd0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-00006be0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00006bf0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00006c00: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00006c10: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-00006c20: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-00006c30: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
-00006c40: 3237 3c41 d40d 0e0f 1011 120a 0a5a 6964  27<A.........Zid
-00006c50: 656e 7469 6669 6572 5577 6964 7468 5961  entifierUwidthYa
-00006c60: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
-00006c70: 546e 616d 6511 01c7 0909 d410 0e0f 0d16  Tname...........
-00006c80: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
-00006c90: d40d 0e0f 101b 1c16 0a5c 6461 7465 4d6f  .........\dateMo
-00006ca0: 6469 6669 6564 10b5 0809 d40d 0e0f 1020  dified......... 
-00006cb0: 1c16 165b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
-00006cc0: 08d4 0d0e 0f10 2425 160a 5473 697a 6510  ......$%..Tsize.
-00006cd0: 6108 09d4 0d0e 0f10 292a 0a0a 546b 696e  a.......)*..Tkin
-00006ce0: 6410 7309 09d4 0d0e 0f10 2e2f 0a16 556c  d.s......../..Ul
-00006cf0: 6162 656c 1064 0908 d40d 0e0f 1033 340a  abel.d.......34.
-00006d00: 1657 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
-00006d10: 0f10 3839 0a16 5863 6f6d 6d65 6e74 7311  ..89..Xcomments.
-00006d20: 012c 0908 d40d 0e0f 103d 3e16 165e 6461  .,.......=>..^da
-00006d30: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
-00006d40: d410 0e0f 0d16 1c16 4408 0859 6461 7465  ........D..Ydate
-00006d50: 4164 6465 6408 2340 2800 0000 0000 005c  Added.#@(......\
-00006d60: 6461 7465 4d6f 6469 6669 6564 2340 3000  dateModified#@0.
-00006d70: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
-00006d80: 005c 0065 0070 0079 008c 008e 008f 009b  .\.e.p.y........
-00006d90: 00a4 00af 00b5 00bf 00c7 00cc 00cf 00d0  ................
-00006da0: 00d1 00da 00db 00dd 00de 00e7 00f0 00fd  ................
-00006db0: 00ff 0100 0101 010a 0116 0117 0118 0121  ...............!
-00006dc0: 0126 0128 0129 012a 0133 0138 013a 013b  .&.(.).*.3.8.:.;
-00006dd0: 013c 0145 014b 014d 014e 014f 0158 0160  .<.E.K.M.N.O.X.`
-00006de0: 0162 0163 0164 016d 0176 0179 017a 017b  .b.c.d.m.v.y.z.{
-00006df0: 0184 0193 0195 0196 0197 01a0 01a1 01a2  ................
-00006e00: 01ac 01ad 01b6 01c3 01cc 0000 0000 0000  ................
-00006e10: 0201 0000 0000 0000 004a 0000 0000 0000  .........J......
-00006e20: 0000 0000 0000 0000 01cd 015c 0164 016d  ...........\.d.m
+000063e0: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
+000063f0: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
+00006400: 7475 7342 6172 5b53 686f 7754 6f6f 6c62  tusBar[ShowToolb
+00006410: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+00006420: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+00006430: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+00006440: 6473 5b53 686f 7753 6964 6562 6172 0809  ds[ShowSidebar..
+00006450: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
+00006460: 2c20 7b39 3237 2c20 3536 387d 7d09 0815  , {927, 568}}...
+00006470: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
+00006480: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
+00006490: 0000 0000 0000 0000 0000 8b00 0000 0900  ................
+000064a0: 6c00 6100 6200 6500 6c00 6c00 6900 6e00  l.a.b.e.l.l.i.n.
+000064b0: 676c 6731 5363 6f6d 7000 0000 0000 031c  glg1Scomp.......
+000064c0: bc00 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
+000064d0: 6c00 6900 6e00 676c 7376 4362 6c6f 6200  l.i.n.glsvCblob.
+000064e0: 0002 7962 706c 6973 7430 30d8 0102 0304  ..ybplist00.....
+000064f0: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
+00006500: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00006510: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00006520: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00006530: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00006540: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00006550: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
+00006560: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
+00006570: 0109 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
+00006580: 0e0f 100a 120a 1457 7669 7369 626c 6555  .......WvisibleU
+00006590: 7769 6474 6859 6173 6365 6e64 696e 675a  widthYascendingZ
+000065a0: 6964 656e 7469 6669 6572 0911 01c7 0954  identifier.....T
+000065b0: 6e61 6d65 d40d 0e0f 1016 1716 1908 1023  name...........#
+000065c0: 0858 7562 6971 7569 7479 d40d 0e0f 100a  .Xubiquity......
+000065d0: 1c16 1e09 10b5 085c 6461 7465 4d6f 6469  .......\dateModi
+000065e0: 6669 6564 d40d 0e0f 1016 1c16 2208 085b  fied........"..[
+000065f0: 6461 7465 4372 6561 7465 64d4 0d0e 0f10  dateCreated.....
+00006600: 0a25 1627 0910 6108 5473 697a 65d4 0d0e  .%.'..a.Tsize...
+00006610: 0f10 0a2a 0a2c 0910 7309 546b 696e 64d4  ...*.,..s.Tkind.
+00006620: 0d0e 0f10 162f 0a31 0810 6409 556c 6162  ...../.1..d.Ulab
+00006630: 656c d40d 0e0f 1016 340a 3608 104b 0957  el......4.6..K.W
+00006640: 7665 7273 696f 6ed4 0d0e 0f10 1639 0a3b  version......9.;
+00006650: 0811 012c 0958 636f 6d6d 656e 7473 d40d  ...,.Xcomments..
+00006660: 0e0f 1016 3e16 4008 10c8 085e 6461 7465  ....>.@....^date
+00006670: 4c61 7374 4f70 656e 6564 d40d 0e0f 1016  LastOpened......
+00006680: 1c16 4408 0859 6461 7465 4164 6465 6408  ..D..YdateAdded.
+00006690: 2340 2800 0000 0000 0054 6e61 6d65 2340  #@(......Tname#@
+000066a0: 3000 0000 0000 0009 0008 0019 002e 0040  0..............@
+000066b0: 0048 005c 0065 0070 0079 008c 008e 008f  .H.\.e.p.y......
+000066c0: 009b 00a4 00ac 00b2 00bc 00c7 00c8 00cb  ................
+000066d0: 00cc 00d1 00da 00db 00dd 00de 00e7 00f0  ................
+000066e0: 00f1 00f3 00f4 0101 010a 010b 010c 0118  ................
+000066f0: 0121 0122 0124 0125 012a 0133 0134 0136  .!.".$.%.*.3.4.6
+00006700: 0137 013c 0145 0146 0148 0149 014f 0158  .7.<.E.F.H.I.O.X
+00006710: 0159 015b 015c 0164 016d 016e 0171 0172  .Y.[.\.d.m.n.q.r
+00006720: 017b 0184 0185 0187 0188 0197 01a0 01a1  .{..............
+00006730: 01a2 01ac 01ad 01b6 01bb 01c4 0000 0000  ................
+00006740: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
+00006750: 0000 0000 0000 0000 0000 01c5 0000 0009  ................
+00006760: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
+00006770: 0067 6c73 7670 626c 6f62 0000 025e 6270  .glsvpblob...^bp
+00006780: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
+00006790: 0a0b 1d45 4647 0a5f 1012 7669 6577 4f70  ...EFG._..viewOp
+000067a0: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
+000067b0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+000067c0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+000067d0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
+000067e0: 697a 655a 736f 7274 436f 6c75 6d6e 5869  izeZsortColumnXi
+000067f0: 636f 6e53 697a 655f 1010 7573 6552 656c  conSize_..useRel
+00006800: 6174 6976 6544 6174 6573 1001 09d9 0c0d  ativeDates......
+00006810: 0e0f 1011 1213 1415 1e23 272b 3035 3a3f  .........#'+05:?
+00006820: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
+00006830: 7374 4f70 656e 6564 5c64 6174 654d 6f64  stOpened\dateMod
+00006840: 6966 6965 645b 6461 7465 4372 6561 7465  ified[dateCreate
+00006850: 6454 7369 7a65 556c 6162 656c 546b 696e  dTsizeUlabelTkin
+00006860: 6457 7665 7273 696f 6e54 6e61 6d65 d416  dWversionTname..
+00006870: 1718 191a 1b0a 1d55 696e 6465 7855 7769  .......UindexUwi
+00006880: 6474 6859 6173 6365 6e64 696e 6757 7669  dthYascendingWvi
+00006890: 7369 626c 6510 0711 012c 0908 d416 1718  sible....,......
+000068a0: 191f 201d 1d10 0810 c808 08d4 1617 1819  .. .............
+000068b0: 0924 1d0a 10b5 0809 d416 1718 1928 241d  .$...........($.
+000068c0: 1d10 0208 08d4 1617 1819 2c2d 1d0a 1003  ..........,-....
+000068d0: 1061 0809 d416 1718 1931 320a 1d10 0510  .a.......12.....
+000068e0: 6409 08d4 1617 1819 3637 0a0a 1004 1073  d.......67.....s
+000068f0: 0909 d416 1718 193b 3c0a 1d10 0610 4b09  .......;<.....K.
+00006900: 08d4 1617 1819 4041 0a0a 1000 1101 c709  ......@A........
+00006910: 0908 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+00006920: 2340 3000 0000 0000 0009 0008 0019 002e  #@0.............
+00006930: 0040 0048 005c 0065 0070 0079 008c 008e  .@.H.\.e.p.y....
+00006940: 008f 00a2 00ab 00ba 00c7 00d3 00d8 00de  ................
+00006950: 00e3 00eb 00f0 00f9 00ff 0105 010f 0117  ................
+00006960: 0119 011c 011d 011e 0127 0129 012b 012c  .........'.).+.,
+00006970: 012d 0136 0138 0139 013a 0143 0145 0146  .-.6.8.9.:.C.E.F
+00006980: 0147 0150 0152 0154 0155 0156 015f 0161  .G.P.R.T.U.V._.a
+00006990: 0163 0164 0165 016e 0170 0172 0173 0174  .c.d.e.n.p.r.s.t
+000069a0: 017d 017f 0181 0182 0183 018c 018e 0191  .}..............
+000069b0: 0192 0193 0194 019d 01a2 01ab 0000 0000  ................
+000069c0: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
+000069d0: 0000 0000 0000 0000 0000 01ac 0000 0009  ................
+000069e0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
+000069f0: 0067 6d6f 4444 626c 6f62 0000 0008 f5a6  .gmoDDblob......
+00006a00: 3155 1321 c541 0000 0009 006c 0061 0062  1U.!.A.....l.a.b
+00006a10: 0065 006c 006c 0069 006e 0067 6d6f 6444  .e.l.l.i.n.gmodD
+00006a20: 626c 6f62 0000 0008 f5a6 3155 1321 c541  blob......1U.!.A
+00006a30: 0000 0009 006c 0061 0062 0065 006c 006c  .....l.a.b.e.l.l
+00006a40: 0069 006e 0067 7068 3153 636f 6d70 0000  .i.n.gph1Scomp..
+00006a50: 0000 0003 a000 0000 0009 006c 0061 0062  ...........l.a.b
+00006a60: 0065 006c 006c 0069 006e 0067 7653 726e  .e.l.l.i.n.gvSrn
+00006a70: 6c6f 6e67 0000 0001 0000 0006 006d 0069  long.........m.i
+00006a80: 0078 0069 006e 0073 6277 7370 626c 6f62  .x.i.n.sbwspblob
+00006a90: 0000 00c8 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00006aa0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+00006ab0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00006ac0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00006ad0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00006ae0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00006af0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00006b00: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00006b10: 0809 5f10 177b 7b30 2c20 3130 357d 2c20  .._..{{0, 105}, 
+00006b20: 7b31 3139 392c 2037 3639 7d7d 0908 1725  {1199, 769}}...%
+00006b30: 313d 4960 6d79 7a7b 7c7d 7e98 0000 0000  1=I`myz{|}~.....
+00006b40: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+00006b50: 0000 0000 0000 0000 0000 0099 0000 0006  ................
+00006b60: 006d 0069 0078 0069 006e 0073 6c67 3153  .m.i.x.i.n.slg1S
+00006b70: 636f 6d70 0000 0000 0010 4db8 0000 0006  comp......M.....
+00006b80: 006d 0069 0078 0069 006e 0073 6c73 7643  .m.i.x.i.n.slsvC
+00006b90: 626c 6f62 0000 0281 6270 6c69 7374 3030  blob....bplist00
+00006ba0: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
+00006bb0: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
+00006bc0: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+00006bd0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00006be0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00006bf0: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+00006c00: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+00006c10: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+00006c20: 6174 6573 1001 09ab 0c15 1a1f 2328 2d32  ates........#(-2
+00006c30: 373c 41d4 0d0e 0f10 1112 0a0a 5a69 6465  7<A.........Zide
+00006c40: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
+00006c50: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
+00006c60: 6e61 6d65 1101 c709 09d4 100e 0f0d 1617  name............
+00006c70: 1619 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
+00006c80: 0d0e 0f10 1b1c 160a 5c64 6174 654d 6f64  ........\dateMod
+00006c90: 6966 6965 6410 b508 09d4 0d0e 0f10 201c  ified......... .
+00006ca0: 1616 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
+00006cb0: d40d 0e0f 1024 2516 0a54 7369 7a65 1061  .....$%..Tsize.a
+00006cc0: 0809 d40d 0e0f 1029 2a0a 0a54 6b69 6e64  .......)*..Tkind
+00006cd0: 1073 0909 d40d 0e0f 102e 2f0a 1655 6c61  .s......../..Ula
+00006ce0: 6265 6c10 6409 08d4 0d0e 0f10 3334 0a16  bel.d.......34..
+00006cf0: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
+00006d00: 1038 390a 1658 636f 6d6d 656e 7473 1101  .89..Xcomments..
+00006d10: 2c09 08d4 0d0e 0f10 3d3e 1616 5e64 6174  ,.......=>..^dat
+00006d20: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
+00006d30: 100e 0f0d 161c 1644 0808 5964 6174 6541  .......D..YdateA
+00006d40: 6464 6564 0823 4028 0000 0000 0000 5c64  dded.#@(......\d
+00006d50: 6174 654d 6f64 6966 6965 6423 4030 0000  ateModified#@0..
+00006d60: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
+00006d70: 5c00 6500 7000 7900 8c00 8e00 8f00 9b00  \.e.p.y.........
+00006d80: a400 af00 b500 bf00 c700 cc00 cf00 d000  ................
+00006d90: d100 da00 db00 dd00 de00 e700 f000 fd00  ................
+00006da0: ff01 0001 0101 0a01 1601 1701 1801 2101  ..............!.
+00006db0: 2601 2801 2901 2a01 3301 3801 3a01 3b01  &.(.).*.3.8.:.;.
+00006dc0: 3c01 4501 4b01 4d01 4e01 4f01 5801 6001  <.E.K.M.N.O.X.`.
+00006dd0: 6201 6301 6401 6d01 7601 7901 7a01 7b01  b.c.d.m.v.y.z.{.
+00006de0: 8401 9301 9501 9601 9701 a001 a101 a201  ................
+00006df0: ac01 ad01 b601 c301 cc00 0000 0000 0002  ................
+00006e00: 0100 0000 0000 0000 4a00 0000 0000 0000  ........J.......
+00006e10: 0000 0000 0000 0001 cd3c 0145 0146 0148  .........<.E.F.H
+00006e20: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
 00006e30: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
 00006e40: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
 00006e50: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
 00006e60: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
 00006e70: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
 00006e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 6a17 4f60 b41d c541  blob....j.O`...A
+00007020: 626c 6f62 0000 0008 1c97 c920 7b20 c541  blob....... { .A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 6a17 4f60  modDblob....j.O`
-00007050: b41d c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 1c97 c920  modDblob....... 
+00007050: 7b20 c541 0000 0006 006d 0069 0078 0069  { .A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 000e 6000 0000 0006 006d 0069 0078 0069  ..`......m.i.x.i
+00007070: 0011 a000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1810,16 +1810,16 @@
 00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00007120: 6261 7208 0809 0809 5f10 187b 7b33 3037  bar....._..{{307
 00007130: 2c20 3836 7d2c 207b 3130 3736 2c20 3632  , 86}, {1076, 62
 00007140: 317d 7d09 0817 2531 3d49 606d 797a 7b7c  1}}...%1=I`myz{|
 00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
-00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 01a4  llg1Scomp.......
-00007190: 7d00 0000 0500 6d00 6f00 6400 6500 6c6c  }.....m.o.d.e.ll
+00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 020d  llg1Scomp.......
+00007190: f700 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
 000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
 00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
@@ -1897,15 +1897,15 @@
 00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
 000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
 000076b0: 6f62 0000 0008 574d 2d38 4017 c541 0000  ob....WM-8@..A..
 000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
 000076d0: 626c 6f62 0000 0008 574d 2d38 4017 c541  blob....WM-8@..A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
-000076f0: 3153 636f 6d70 0000 0000 0001 f000 0000  1Scomp..........
+000076f0: 3153 636f 6d70 0000 0000 0002 7000 0000  1Scomp......p...
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00007730: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
 00007740: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 00007750: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 00007760: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
@@ -1917,15 +1917,15 @@
 000077c0: 5f10 197b 7b33 3534 2c20 3132 347d 2c20  _..{{354, 124}, 
 000077d0: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 000077e0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 000077f0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00007800: 0000 0000 0000 0000 0000 009b 0000 000d  ................
 00007810: 006f 0075 0074 006c 0069 0065 0072 005f  .o.u.t.l.i.e.r._
 00007820: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
-00007830: 6d70 0000 0000 0000 f7bc 0000 000d 006f  mp.............o
+00007830: 6d70 0000 0000 0001 31b8 0000 000d 006f  mp......1......o
 00007840: 0075 0074 006c 0069 0065 0072 005f 0074  .u.t.l.i.e.r._.t
 00007850: 006f 006f 006c 0073 6c73 7643 626c 6f62  .o.o.l.slsvCblob
 00007860: 0000 02b0 6270 6c69 7374 3030 da01 0203  ....bplist00....
 00007870: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
 00007880: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
 00007890: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 000078a0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
@@ -2016,290 +2016,290 @@
 00007df0: 736d 6f44 4462 6c6f 6200 0000 08aa 2e11  smoDDblob.......
 00007e00: 6564 14c5 4100 0000 0d00 6f00 7500 7400  ed..A.....o.u.t.
 00007e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00007e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08aa  l.smodDblob.....
 00007e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00007e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00007e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
-00007e60: 0000 01b0 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
+00007e60: 0000 0210 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00007e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00007e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00007e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-00007ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
-00007eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-00007ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00007ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00007ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00007ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00007f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00007f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00007f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00007f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
-00007f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
-00007f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-00007f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-00007f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
-00007f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00007f90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
+00007ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b862  n.gbwspblob....b
+00007eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
+00007ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00007ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
+00007ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
+00007ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
+00007f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
+00007f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
+00007f20: 187b 7b33 3335 2c20 3139 387d 2c20 7b39  .{{335, 198}, {9
+00007f30: 3237 2c20 3536 387d 7d09 0815 232f 3b52  27, 568}}...#/;R
+00007f40: 5f6b 6c6d 6e6f 8a00 0000 0000 0001 0100  _klmno..........
+00007f50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+00007f60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
+00007f70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+00007f80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+00007f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
 00008010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-00008020: 6c73 7670 626c 6f62 0000 029d 6270 6c69  lsvpblob....bpli
+00008020: 6c73 7670 626c 6f62 0000 02a0 6270 6c69  lsvpblob....bpli
 00008030: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00008040: 0c0d 1f47 4847 494a 0c5f 1012 7669 6577  ...GHGIJ._..view
-00008050: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00008060: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00008070: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00008080: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00008090: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-000080a0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-000080b0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-000080c0: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-000080d0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000080e0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-000080f0: 292d 3237 3c41 5863 6f6d 6d65 6e74 735e  )-27<AXcomments^
-00008100: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
-00008110: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
-00008120: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
-00008130: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
-00008140: 6e61 6d65 d418 191a 1b1c 1d0c 1f55 696e  name.........Uin
-00008150: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
-00008160: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
-00008170: 0908 d418 191a 1b21 221f 1f10 0810 c808  .......!".......
-00008180: 08d4 1819 1a1b 0b26 1f0c 10b5 0809 d418  .......&........
-00008190: 191a 1b2a 261f 1f10 0208 08d4 1819 1a1b  ...*&...........
-000081a0: 2e2f 1f0c 1003 1061 0809 d418 191a 1b33  ./.....a.......3
-000081b0: 340c 1f10 0510 6409 08d4 1819 1a1b 3839  4.....d.......89
-000081c0: 0c0c 1004 1073 0909 d418 191a 1b3d 3e0c  .....s.......=>.
-000081d0: 1f10 0610 4b09 08d4 1819 1a1b 4243 0c0c  ....K.......BC..
-000081e0: 1000 1101 c709 0908 2300 0000 0000 0000  ........#.......
-000081f0: 0023 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
-00008200: 6f64 6966 6965 6423 4030 0000 0000 0000  odified#@0......
-00008210: 0900 0800 1d00 3200 4400 4c00 6000 7200  ......2.D.L.`.r.
-00008220: 7b00 8d00 9800 a100 b400 b600 b700 ca00  {...............
-00008230: d300 e200 ef00 fb01 0001 0601 0b01 1301  ................
-00008240: 1801 2101 2701 2d01 3701 3f01 4101 4401  ..!.'.-.7.?.A.D.
-00008250: 4501 4601 4f01 5101 5301 5401 5501 5e01  E.F.O.Q.S.T.U.^.
-00008260: 6001 6101 6201 6b01 6d01 6e01 6f01 7801  `.a.b.k.m.n.o.x.
-00008270: 7a01 7c01 7d01 7e01 8701 8901 8b01 8c01  z.|.}.~.........
-00008280: 8d01 9601 9801 9a01 9b01 9c01 a501 a701  ................
-00008290: a901 aa01 ab01 b401 b601 b901 ba01 bb01  ................
-000082a0: bc01 c501 ce01 db01 e400 0000 0000 0002  ................
-000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
-000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
-000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 083d d3c5 a9d2 1dc5  Dblob....=......
-000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
-00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-00008310: 083d d3c5 a9d2 1dc5 4100 0000 0800 7000  .=......A.....p.
-00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
-00008330: 5363 6f6d 7000 0000 0000 0fb0 0000 0000  Scomp...........
-00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
-00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
-00008360: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
-00008370: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-00008380: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
-00008390: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-000083a0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-000083b0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-000083c0: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-000083d0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-000083e0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-000083f0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00008400: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00008410: 095f 1019 7b7b 3133 372c 2031 3433 7d2c  ._..{{137, 143},
-00008420: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
-00008430: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
-00008440: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00008450: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
-00008460: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
-00008470: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-00008480: 6900 6f00 6e00 7364 7363 6c62 6f6f 6c00  i.o.n.sdsclbool.
-00008490: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-000084a0: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-000084b0: 0074 0069 006f 006e 0073 6c67 3153 636f  .t.i.o.n.slg1Sco
-000084c0: 6d70 0000 0000 0006 ae56 0000 0013 0070  mp.......V.....p
-000084d0: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
-000084e0: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
-000084f0: 006e 0073 6c73 7643 626c 6f62 0000 02b0  .n.slsvCblob....
-00008500: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00008510: 0809 0a0b 0c0d 1848 4948 4a4b 0c5f 1012  .......HIHJK._..
-00008520: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00008530: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00008540: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00008550: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00008560: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-00008570: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-00008580: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-00008590: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-000085a0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-000085b0: 6174 6573 1001 09ab 0e17 1c21 252a 2f34  ates.......!%*/4
-000085c0: 393e 43d4 0f10 1112 0c14 0c16 5776 6973  9>C.........Wvis
-000085d0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-000085e0: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
-000085f0: 1101 c709 546e 616d 65d4 0f10 1112 1819  ....Tname.......
-00008600: 181b 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
-00008610: 0f10 1112 0c1e 1820 0910 b508 5c64 6174  ....... ....\dat
-00008620: 654d 6f64 6966 6965 64d4 0f10 1112 181e  eModified.......
-00008630: 1824 0808 5b64 6174 6543 7265 6174 6564  .$..[dateCreated
-00008640: d40f 1011 120c 2718 2909 1061 0854 7369  ......'.)..a.Tsi
-00008650: 7a65 d40f 1011 120c 2c0c 2e09 1073 0954  ze......,....s.T
-00008660: 6b69 6e64 d40f 1011 1218 310c 3308 1064  kind......1.3..d
-00008670: 0955 6c61 6265 6cd4 0f10 1112 1836 0c38  .Ulabel......6.8
-00008680: 0810 4b09 5776 6572 7369 6f6e d40f 1011  ..K.Wversion....
-00008690: 1218 3b0c 3d08 1101 2c09 5863 6f6d 6d65  ..;.=...,.Xcomme
-000086a0: 6e74 73d4 0f10 1112 1840 1842 0810 c808  nts......@.B....
-000086b0: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
-000086c0: 0f10 1112 181e 1846 0808 5964 6174 6541  .......F..YdateA
-000086d0: 6464 6564 0823 0000 0000 0000 0000 2340  dded.#........#@
-000086e0: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
-000086f0: 0000 0000 0009 0008 001d 0032 0044 004c  ...........2.D.L
-00008700: 0060 0072 007b 008d 0098 00a1 00b4 00b6  .`.r.{..........
-00008710: 00b7 00c3 00cc 00d4 00da 00e4 00ef 00f0  ................
-00008720: 00f3 00f4 00f9 0102 0103 0105 0106 010f  ................
-00008730: 0118 0119 011b 011c 0129 0132 0133 0134  .........).2.3.4
-00008740: 0140 0149 014a 014c 014d 0152 015b 015c  .@.I.J.L.M.R.[.\
-00008750: 015e 015f 0164 016d 016e 0170 0171 0177  .^._.d.m.n.p.q.w
-00008760: 0180 0181 0183 0184 018c 0195 0196 0199  ................
-00008770: 019a 01a3 01ac 01ad 01af 01b0 01bf 01c8  ................
-00008780: 01c9 01ca 01d4 01d5 01de 01e7 01ec 01f5  ................
-00008790: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
-000087a0: 0000 0000 0000 0000 0000 0000 0000 01f6  ................
-000087b0: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-000087c0: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-000087d0: 0074 0069 006f 006e 0073 6c73 7670 626c  .t.i.o.n.slsvpbl
-000087e0: 6f62 0000 0295 6270 6c69 7374 3030 da01  ob....bplist00..
-000087f0: 0203 0405 0607 0809 0a0b 0c0d 1f47 4847  .............GHG
-00008800: 494a 0c5f 1012 7669 6577 4f70 7469 6f6e  IJ._..viewOption
-00008810: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00008820: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00008830: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00008840: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
-00008850: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
-00008860: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
-00008870: 6f6e 585a 736f 7274 436f 6c75 6d6e 5869  onXZsortColumnXi
-00008880: 636f 6e53 697a 655f 1010 7573 6552 656c  conSize_..useRel
-00008890: 6174 6976 6544 6174 6573 1001 09d9 0e0f  ativeDates......
-000088a0: 1011 1213 1415 1617 2025 292d 3237 3c41  ........ %)-27<A
-000088b0: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
-000088c0: 7374 4f70 656e 6564 5c64 6174 654d 6f64  stOpened\dateMod
-000088d0: 6966 6965 645b 6461 7465 4372 6561 7465  ified[dateCreate
-000088e0: 6454 7369 7a65 556c 6162 656c 546b 696e  dTsizeUlabelTkin
-000088f0: 6457 7665 7273 696f 6e54 6e61 6d65 d418  dWversionTname..
-00008900: 191a 1b1c 1d0c 1f55 696e 6465 7855 7769  .......UindexUwi
-00008910: 6474 6859 6173 6365 6e64 696e 6757 7669  dthYascendingWvi
-00008920: 7369 626c 6510 0711 012c 0908 d418 191a  sible....,......
-00008930: 1b21 221f 1f10 0810 c808 08d4 1819 1a1b  .!".............
-00008940: 0b26 1f0c 10b5 0809 d418 191a 1b2a 261f  .&...........*&.
-00008950: 1f10 0208 08d4 1819 1a1b 2e2f 1f0c 1003  .........../....
-00008960: 1061 0809 d418 191a 1b33 340c 1f10 0510  .a.......34.....
-00008970: 6409 08d4 1819 1a1b 3839 0c0c 1004 1073  d.......89.....s
-00008980: 0909 d418 191a 1b3d 3e0c 1f10 0610 4b09  .......=>.....K.
-00008990: 08d4 1819 1a1b 4243 0c0c 1000 1101 c709  ......BC........
-000089a0: 0908 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
-000089b0: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
-000089c0: 0000 0900 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
-000089d0: 7200 7b00 8d00 9800 a100 b400 b600 b700  r.{.............
-000089e0: ca00 d300 e200 ef00 fb01 0001 0601 0b01  ................
-000089f0: 1301 1801 2101 2701 2d01 3701 3f01 4101  ....!.'.-.7.?.A.
-00008a00: 4401 4501 4601 4f01 5101 5301 5401 5501  D.E.F.O.Q.S.T.U.
-00008a10: 5e01 6001 6101 6201 6b01 6d01 6e01 6f01  ^.`.a.b.k.m.n.o.
-00008a20: 7801 7a01 7c01 7d01 7e01 8701 8901 8b01  x.z.|.}.~.......
-00008a30: 8c01 8d01 9601 9801 9a01 9b01 9c01 a501  ................
-00008a40: a701 a901 aa01 ab01 b401 b601 b901 ba01  ................
-00008a50: bb01 bc01 c501 ce01 d301 dc00 0000 0000  ................
-00008a60: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
-00008a70: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
-00008a80: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
-00008a90: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
-00008aa0: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
-00008ab0: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
-00008ac0: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
-00008ad0: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
-00008ae0: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
-00008af0: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
-00008b00: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
-00008b10: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00008b20: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
-00008b30: 0000 0000 1300 7000 6f00 7300 6500 5f00  ......p.o.s.e._.
-00008b40: 6300 6f00 6e00 6600 6900 6700 7500 7200  c.o.n.f.i.g.u.r.
-00008b50: 6100 7400 6900 6f00 6e00 7376 5372 6e6c  a.t.i.o.n.svSrnl
-00008b60: 6f6e 6700 0000 0100 0000 1b00 7000 6f00  ong.........p.o.
-00008b70: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
-00008b80: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00008b90: 7300 5f00 6100 7200 6300 6800 6900 7600  s._.a.r.c.h.i.v.
-00008ba0: 656c 6731 5363 6f6d 7000 0000 0000 06fa  elg1Scomp.......
-00008bb0: ed00 0000 1b00 7000 6f00 7300 6500 5f00  ......p.o.s.e._.
-00008bc0: 6300 6f00 6e00 6600 6900 6700 7500 7200  c.o.n.f.i.g.u.r.
-00008bd0: 6100 7400 6900 6f00 6e00 7300 5f00 6100  a.t.i.o.n.s._.a.
-00008be0: 7200 6300 6800 6900 7600 656d 6f44 4462  r.c.h.i.v.emoDDb
-00008bf0: 6c6f 6200 0000 0889 831e a9cb fec4 4100  lob...........A.
-00008c00: 0000 1b00 7000 6f00 7300 6500 5f00 6300  ....p.o.s.e._.c.
-00008c10: 6f00 6e00 6600 6900 6700 7500 7200 6100  o.n.f.i.g.u.r.a.
-00008c20: 7400 6900 6f00 6e00 7300 5f00 6100 7200  t.i.o.n.s._.a.r.
-00008c30: 6300 6800 6900 7600 656d 6f64 4462 6c6f  c.h.i.v.emodDblo
-00008c40: 6200 0000 0889 831e a9cb fec4 4100 0000  b...........A...
-00008c50: 1b00 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
-00008c60: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-00008c70: 6900 6f00 6e00 7300 5f00 6100 7200 6300  i.o.n.s._.a.r.c.
-00008c80: 6800 6900 7600 6570 6831 5363 6f6d 7000  h.i.v.eph1Scomp.
-00008c90: 0000 0000 0790 0000 0000 0e00 7000 6f00  ............p.o.
-00008ca0: 7300 6500 5f00 6900 6d00 7000 6f00 7200  s.e._.i.m.p.o.r.
-00008cb0: 7400 6500 7200 7362 7773 7062 6c6f 6200  t.e.r.sbwspblob.
-00008cc0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-00008cd0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-00008ce0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-00008cf0: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-00008d00: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00008d10: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-00008d20: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00008d30: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00008d40: 095f 1018 7b7b 3336 2c20 3133 317d 2c20  ._..{{36, 131}, 
-00008d50: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
-00008d60: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
-00008d70: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-00008d80: 0000 0000 0000 0000 0000 009a 0000 000e  ................
-00008d90: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
-00008da0: 006f 0072 0074 0065 0072 0073 6473 636c  .o.r.t.e.r.sdscl
-00008db0: 626f 6f6c 0000 0000 0e00 7000 6f00 7300  bool......p.o.s.
-00008dc0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
-00008dd0: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
-00008de0: 0000 02c9 b900 5f00 7400 6f00 6f00 6c00  ......_.t.o.o.l.
+00008040: 0c0d 1f48 494a 4b0c 3558 6963 6f6e 5369  ...HIJK.5XiconSi
+00008050: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00008060: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00008070: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00008080: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+00008090: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000080a0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000080b0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000080c0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+000080d0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+000080e0: 2340 3000 0000 0000 0009 d90e 0f10 1112  #@0.............
+000080f0: 1314 1516 1720 252a 2f34 383d 4258 636f  ..... %*/48=BXco
+00008100: 6d6d 656e 7473 556c 6162 656c 5776 6572  mmentsUlabelWver
+00008110: 7369 6f6e 5b64 6174 6543 7265 6174 6564  sion[dateCreated
+00008120: 5473 697a 655c 6461 7465 4d6f 6469 6669  Tsize\dateModifi
+00008130: 6564 546b 696e 6454 6e61 6d65 5e64 6174  edTkindTname^dat
+00008140: 654c 6173 744f 7065 6e65 64d4 1819 1a1b  eLastOpened.....
+00008150: 1c1d 0c1f 5569 6e64 6578 5577 6964 7468  ....UindexUwidth
+00008160: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00008170: 6c65 1007 1101 2c09 08d4 1819 1a1b 2122  le....,.......!"
+00008180: 0c1f 1005 1064 0908 d418 191a 1b26 270c  .....d.......&'.
+00008190: 1f10 0610 4b09 08d4 1819 1a1b 2b2c 1f1f  ....K.......+,..
+000081a0: 1002 10b5 0808 d418 191a 1b30 311f 0c10  ...........01...
+000081b0: 0310 6108 09d4 1819 1a1b 352c 1f0c 1001  ..a.......5,....
+000081c0: 0809 d418 191a 1b39 3a0c 0c10 0410 7309  .......9:.....s.
+000081d0: 09d4 1819 1a1b 3e3f 0c0c 1000 1101 c709  ......>?........
+000081e0: 09d4 1819 1a1b 4344 1f1f 1008 10c8 0808  ......CD........
+000081f0: 0823 405e 4000 0000 0000 2340 2800 0000  .#@^@.....#@(...
+00008200: 0000 0023 4000 0000 0000 0000 546e 616d  ...#@.......Tnam
+00008210: 6509 0008 001d 0026 0038 0040 0054 0066  e......&.8.@.T.f
+00008220: 006f 0081 008c 009f 00b4 00bd 00be 00d1  .o..............
+00008230: 00da 00e0 00e8 00f4 00f9 0106 010b 0110  ................
+00008240: 011f 0128 012e 0134 013e 0146 0148 014b  ...(...4.>.F.H.K
+00008250: 014c 014d 0156 0158 015a 015b 015c 0165  .L.M.V.X.Z.[.\.e
+00008260: 0167 0169 016a 016b 0174 0176 0178 0179  .g.i.j.k.t.v.x.y
+00008270: 017a 0183 0185 0187 0188 0189 0192 0194  .z..............
+00008280: 0195 0196 019f 01a1 01a3 01a4 01a5 01ae  ................
+00008290: 01b0 01b3 01b4 01b5 01be 01c0 01c2 01c3  ................
+000082a0: 01c4 01c5 01ce 01d7 01e0 01e5 0000 0000  ................
+000082b0: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
+000082c0: 0000 0000 0000 0000 0000 01e6 0000 0008  ................
+000082d0: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
+000082e0: 6d6f 4444 626c 6f62 0000 0008 b0f7 c86b  moDDblob.......k
+000082f0: eb20 c541 0000 0008 0070 006c 006f 0074  . .A.....p.l.o.t
+00008300: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
+00008310: 0000 0008 b0f7 c86b eb20 c541 0000 0008  .......k. .A....
+00008320: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
+00008330: 7068 3153 636f 6d70 0000 0000 0014 2000  ph1Scomp...... .
+00008340: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
+00008350: 006e 0067 7653 726e 6c6f 6e67 0000 0001  .n.gvSrnlong....
+00008360: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
+00008370: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
+00008380: 0074 0069 006f 006e 0073 6277 7370 626c  .t.i.o.n.sbwspbl
+00008390: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
+000083a0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+000083b0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+000083c0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+000083d0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+000083e0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+000083f0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00008400: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00008410: 0809 0809 5f10 197b 7b31 3337 2c20 3134  ...._..{{137, 14
+00008420: 337d 2c20 7b31 3330 322c 2037 3134 7d7d  3}, {1302, 714}}
+00008430: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+00008440: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+00008450: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+00008460: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
+00008470: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
+00008480: 0074 0069 006f 006e 0073 6473 636c 626f  .t.i.o.n.sdsclbo
+00008490: 6f6c 0000 0000 1300 7000 6f00 7300 6500  ol......p.o.s.e.
+000084a0: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
+000084b0: 7200 6100 7400 6900 6f00 6e00 736c 6731  r.a.t.i.o.n.slg1
+000084c0: 5363 6f6d 7000 0000 0000 06ae 5600 0000  Scomp.......V...
+000084d0: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
+000084e0: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
+000084f0: 6900 6f00 6e00 736c 7376 4362 6c6f 6200  i.o.n.slsvCblob.
+00008500: 0002 b062 706c 6973 7430 30da 0102 0304  ...bplist00.....
+00008510: 0506 0708 090a 0b0c 0d18 4849 484a 4b0c  ..........HIHJK.
+00008520: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00008530: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+00008540: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00008550: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00008560: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
+00008570: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
+00008580: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
+00008590: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+000085a0: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+000085b0: 7665 4461 7465 7310 0109 ab0e 171c 2125  veDates.......!%
+000085c0: 2a2f 3439 3e43 d40f 1011 120c 140c 1657  */49>C.........W
+000085d0: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+000085e0: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
+000085f0: 6572 0911 01c7 0954 6e61 6d65 d40f 1011  er.....Tname....
+00008600: 1218 1918 1b08 1023 0858 7562 6971 7569  .......#.Xubiqui
+00008610: 7479 d40f 1011 120c 1e18 2009 10b5 085c  ty........ ....\
+00008620: 6461 7465 4d6f 6469 6669 6564 d40f 1011  dateModified....
+00008630: 1218 1e18 2408 085b 6461 7465 4372 6561  ....$..[dateCrea
+00008640: 7465 64d4 0f10 1112 0c27 1829 0910 6108  ted......'.)..a.
+00008650: 5473 697a 65d4 0f10 1112 0c2c 0c2e 0910  Tsize......,....
+00008660: 7309 546b 696e 64d4 0f10 1112 1831 0c33  s.Tkind......1.3
+00008670: 0810 6409 556c 6162 656c d40f 1011 1218  ..d.Ulabel......
+00008680: 360c 3808 104b 0957 7665 7273 696f 6ed4  6.8..K.Wversion.
+00008690: 0f10 1112 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
+000086a0: 6d6d 656e 7473 d40f 1011 1218 4018 4208  mments......@.B.
+000086b0: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
+000086c0: 6564 d40f 1011 1218 1e18 4608 0859 6461  ed........F..Yda
+000086d0: 7465 4164 6465 6408 2300 0000 0000 0000  teAdded.#.......
+000086e0: 0023 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
+000086f0: 4030 0000 0000 0000 0900 0800 1d00 3200  @0............2.
+00008700: 4400 4c00 6000 7200 7b00 8d00 9800 a100  D.L.`.r.{.......
+00008710: b400 b600 b700 c300 cc00 d400 da00 e400  ................
+00008720: ef00 f000 f300 f400 f901 0201 0301 0501  ................
+00008730: 0601 0f01 1801 1901 1b01 1c01 2901 3201  ............).2.
+00008740: 3301 3401 4001 4901 4a01 4c01 4d01 5201  3.4.@.I.J.L.M.R.
+00008750: 5b01 5c01 5e01 5f01 6401 6d01 6e01 7001  [.\.^._.d.m.n.p.
+00008760: 7101 7701 8001 8101 8301 8401 8c01 9501  q.w.............
+00008770: 9601 9901 9a01 a301 ac01 ad01 af01 b001  ................
+00008780: bf01 c801 c901 ca01 d401 d501 de01 e701  ................
+00008790: ec01 f500 0000 0000 0002 0100 0000 0000  ................
+000087a0: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
+000087b0: 0001 f600 0000 1300 7000 6f00 7300 6500  ........p.o.s.e.
+000087c0: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
+000087d0: 7200 6100 7400 6900 6f00 6e00 736c 7376  r.a.t.i.o.n.slsv
+000087e0: 7062 6c6f 6200 0002 9562 706c 6973 7430  pblob....bplist0
+000087f0: 30da 0102 0304 0506 0708 090a 0b0c 0d1f  0...............
+00008800: 4748 4749 4a0c 5f10 1276 6965 774f 7074  GHGIJ._..viewOpt
+00008810: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
+00008820: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00008830: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00008840: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
+00008850: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
+00008860: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
+00008870: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+00008880: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
+00008890: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
+000088a0: d90e 0f10 1112 1314 1516 1720 2529 2d32  ........... %)-2
+000088b0: 373c 4158 636f 6d6d 656e 7473 5e64 6174  7<AXcomments^dat
+000088c0: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
+000088d0: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
+000088e0: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+000088f0: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+00008900: 65d4 1819 1a1b 1c1d 0c1f 5569 6e64 6578  e.........Uindex
+00008910: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00008920: 5776 6973 6962 6c65 1007 1101 2c09 08d4  Wvisible....,...
+00008930: 1819 1a1b 2122 1f1f 1008 10c8 0808 d418  ....!"..........
+00008940: 191a 1b0b 261f 0c10 b508 09d4 1819 1a1b  ....&...........
+00008950: 2a26 1f1f 1002 0808 d418 191a 1b2e 2f1f  *&............/.
+00008960: 0c10 0310 6108 09d4 1819 1a1b 3334 0c1f  ....a.......34..
+00008970: 1005 1064 0908 d418 191a 1b38 390c 0c10  ...d.......89...
+00008980: 0410 7309 09d4 1819 1a1b 3d3e 0c1f 1006  ..s.......=>....
+00008990: 104b 0908 d418 191a 1b42 430c 0c10 0011  .K.......BC.....
+000089a0: 01c7 0909 0823 0000 0000 0000 0000 2340  .....#........#@
+000089b0: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
+000089c0: 0000 0000 0009 0008 001d 0032 0044 004c  ...........2.D.L
+000089d0: 0060 0072 007b 008d 0098 00a1 00b4 00b6  .`.r.{..........
+000089e0: 00b7 00ca 00d3 00e2 00ef 00fb 0100 0106  ................
+000089f0: 010b 0113 0118 0121 0127 012d 0137 013f  .......!.'.-.7.?
+00008a00: 0141 0144 0145 0146 014f 0151 0153 0154  .A.D.E.F.O.Q.S.T
+00008a10: 0155 015e 0160 0161 0162 016b 016d 016e  .U.^.`.a.b.k.m.n
+00008a20: 016f 0178 017a 017c 017d 017e 0187 0189  .o.x.z.|.}.~....
+00008a30: 018b 018c 018d 0196 0198 019a 019b 019c  ................
+00008a40: 01a5 01a7 01a9 01aa 01ab 01b4 01b6 01b9  ................
+00008a50: 01ba 01bb 01bc 01c5 01ce 01d3 01dc 0000  ................
+00008a60: 0000 0000 0201 0000 0000 0000 004c 0000  .............L..
+00008a70: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
+00008a80: 0013 0070 006f 0073 0065 005f 0063 006f  ...p.o.s.e._.c.o
+00008a90: 006e 0066 0069 0067 0075 0072 0061 0074  .n.f.i.g.u.r.a.t
+00008aa0: 0069 006f 006e 0073 6d6f 4444 626c 6f62  .i.o.n.smoDDblob
+00008ab0: 0000 0008 d97e 4b74 e2dd c441 0000 0013  .....~Kt...A....
+00008ac0: 0070 006f 0073 0065 005f 0063 006f 006e  .p.o.s.e._.c.o.n
+00008ad0: 0066 0069 0067 0075 0072 0061 0074 0069  .f.i.g.u.r.a.t.i
+00008ae0: 006f 006e 0073 6d6f 6444 626c 6f62 0000  .o.n.smodDblob..
+00008af0: 0008 d97e 4b74 e2dd c441 0000 0013 0070  ...~Kt...A.....p
+00008b00: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
+00008b10: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
+00008b20: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
+00008b30: 0007 3000 0000 0013 0070 006f 0073 0065  ..0......p.o.s.e
+00008b40: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
+00008b50: 0072 0061 0074 0069 006f 006e 0073 7653  .r.a.t.i.o.n.svS
+00008b60: 726e 6c6f 6e67 0000 0001 0000 001b 0070  rnlong.........p
+00008b70: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
+00008b80: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
+00008b90: 006e 0073 005f 0061 0072 0063 0068 0069  .n.s._.a.r.c.h.i
+00008ba0: 0076 0065 6c67 3153 636f 6d70 0000 0000  .v.elg1Scomp....
+00008bb0: 0006 faed 0000 001b 0070 006f 0073 0065  .........p.o.s.e
+00008bc0: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
+00008bd0: 0072 0061 0074 0069 006f 006e 0073 005f  .r.a.t.i.o.n.s._
+00008be0: 0061 0072 0063 0068 0069 0076 0065 6d6f  .a.r.c.h.i.v.emo
+00008bf0: 4444 626c 6f62 0000 0008 8983 1ea9 cbfe  DDblob..........
+00008c00: c441 0000 001b 0070 006f 0073 0065 005f  .A.....p.o.s.e._
+00008c10: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
+00008c20: 0061 0074 0069 006f 006e 0073 005f 0061  .a.t.i.o.n.s._.a
+00008c30: 0072 0063 0068 0069 0076 0065 6d6f 6444  .r.c.h.i.v.emodD
+00008c40: 626c 6f62 0000 0008 8983 1ea9 cbfe c441  blob...........A
+00008c50: 0000 001b 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
+00008c60: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
+00008c70: 0074 0069 006f 006e 0073 005f 0061 0072  .t.i.o.n.s._.a.r
+00008c80: 0063 0068 0069 0076 0065 7068 3153 636f  .c.h.i.v.eph1Sco
+00008c90: 6d70 0000 0000 0007 9000 0000 000e 0070  mp.............p
+00008ca0: 006f 0073 0065 005f 0069 006d 0070 006f  .o.s.e._.i.m.p.o
+00008cb0: 0072 0074 0065 0072 0073 6277 7370 626c  .r.t.e.r.sbwspbl
+00008cc0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+00008cd0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00008ce0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00008cf0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00008d00: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00008d10: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00008d20: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00008d30: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00008d40: 0809 0809 5f10 187b 7b33 362c 2031 3331  ...._..{{36, 131
+00008d50: 7d2c 207b 3133 3032 2c20 3731 347d 7d09  }, {1302, 714}}.
+00008d60: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+00008d70: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00008d80: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+00008d90: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
+00008da0: 6d00 7000 6f00 7200 7400 6500 7200 7364  m.p.o.r.t.e.r.sd
+00008db0: 7363 6c62 6f6f 6c00 0000 000e 0070 006f  sclbool......p.o
+00008dc0: 0073 0065 005f 0069 006d 0070 006f 0072  .s.e._.i.m.p.o.r
+00008dd0: 0074 0065 0072 0073 6c67 3153 636f 6d70  .t.e.r.slg1Scomp
+00008de0: 0000 0000 0003 87aa 7400 6f00 6f00 6c00  ........t.o.o.l.
 00008df0: 736d 6f44 4462 6c6f 6200 0000 08aa 2e11  smoDDblob.......
 00008e00: 6564 14c5 4100 0000 0d00 6f00 7500 7400  ed..A.....o.u.t.
 00008e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00008e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08aa  l.smodDblob.....
 00008e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00008e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00008e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
-00008e60: 0000 01b0 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
+00008e60: 0000 0210 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00008e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00008e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00008e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-00008ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
-00008eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-00008ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00008ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00008ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00008ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00008f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00008f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00008f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00008f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
-00008f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
-00008f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-00008f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-00008f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
-00008f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00008f90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
+00008ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b862  n.gbwspblob....b
+00008eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
+00008ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00008ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
+00008ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
+00008ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
+00008f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
+00008f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
+00008f20: 187b 7b33 3335 2c20 3139 387d 2c20 7b39  .{{335, 198}, {9
+00008f30: 3237 2c20 3536 387d 7d09 0815 232f 3b52  27, 568}}...#/;R
+00008f40: 5f6b 6c6d 6e6f 8a00 0000 0000 0001 0100  _klmno..........
+00008f50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+00008f60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
+00008f70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+00008f80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+00008f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2349,15 +2349,15 @@
 000092c0: 4444 626c 6f62 0000 0008 23bd 51ed cc0c  DDblob....#.Q...
 000092d0: c541 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 000092e0: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
 000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 23bd  .smodDblob....#.
 00009300: 51ed cc0c c541 0000 000e 0070 006f 0073  Q....A.....p.o.s
 00009310: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009320: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
-00009330: 0000 0003 8000 0000 000e 0070 006f 0073  ...........p.o.s
+00009330: 0000 0004 8000 0000 000e 0070 006f 0073  ...........p.o.s
 00009340: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009350: 0065 0072 0073 7653 726e 6c6f 6e67 0000  .e.r.svSrnlong..
 00009360: 0001 0000 000f 0070 006f 0073 0065 005f  .......p.o.s.e._
 00009370: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
 00009380: 0072 0073 6277 7370 626c 6f62 0000 00ca  .r.sbwspblob....
 00009390: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 000093a0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
@@ -2370,15 +2370,15 @@
 00009410: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00009420: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00009430: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00009440: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00009450: 0000 0000 0000 0000 009b 0000 000f 0070  ...............p
 00009460: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
 00009470: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
-00009480: 636f 6d70 0000 0000 0000 def3 0000 000f  comp............
+00009480: 636f 6d70 0000 0000 0001 0ece 0000 000f  comp............
 00009490: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
 000094a0: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
 000094b0: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
 000094c0: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
 000094d0: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
 000094e0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
 000094f0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
@@ -2465,15 +2465,15 @@
 00009a00: 6f44 4462 6c6f 6200 0000 08e2 486d c51b  oDDblob.....Hm..
 00009a10: 1fc5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
 00009a20: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 00009a30: 6f00 7200 736d 6f64 4462 6c6f 6200 0000  o.r.smodDblob...
 00009a40: 08e2 486d c51b 1fc5 4100 0000 0f00 7000  ..Hm....A.....p.
 00009a50: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
 00009a60: 6500 7300 7300 6f00 7200 7370 6831 5363  e.s.s.o.r.sph1Sc
-00009a70: 6f6d 7000 0000 0000 0180 0000 0000 0f00  omp.............
+00009a70: 6f6d 7000 0000 0000 01e0 0000 0000 0f00  omp.............
 00009a80: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
 00009a90: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
 00009aa0: 6e6c 6f6e 6700 0000 0100 0000 0900 7200  nlong.........r.
 00009ab0: 6f00 6900 5f00 7400 6f00 6f00 6c00 7362  o.i._.t.o.o.l.sb
 00009ac0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
 00009ad0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
 00009ae0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
@@ -2485,15 +2485,15 @@
 00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
 00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
 00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
 00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 05ec 0b00 0000 0900  omp.............
+00009bb0: 6f6d 7000 0000 0000 079c 6d00 0000 0900  omp.......m.....
 00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
 00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
 00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
 00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
 00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -2528,56 +2528,56 @@
 00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
 00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
 00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
 00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
 00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
 00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
 00009e50: 0000 0000 01c5 6831 5363 6f6d 7000 0000  ......h1Scomp...
-00009e60: 0000 01b0 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
+00009e60: 0000 0210 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00009e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00009e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00009e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-00009ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
-00009eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-00009ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00009ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00009ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00009ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00009f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00009f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00009f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00009f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
-00009f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
-00009f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-00009f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-00009f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
-00009f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00009f90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
+00009ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b862  n.gbwspblob....b
+00009eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
+00009ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00009ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
+00009ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
+00009ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
+00009f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
+00009f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
+00009f20: 187b 7b33 3335 2c20 3139 387d 2c20 7b39  .{{335, 198}, {9
+00009f30: 3237 2c20 3536 387d 7d09 0815 232f 3b52  27, 568}}...#/;R
+00009f40: 5f6b 6c6d 6e6f 8a00 0000 0000 0001 0100  _klmno..........
+00009f50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+00009f60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
+00009f70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+00009f80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+00009f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0018 0000 0009  ................
 0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 5519  .smoDDblob....U.
 0000a030: 3cb9 d51b c541 0000 0009 0072 006f 0069  <....A.....r.o.i
 0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
 0000a050: 626c 6f62 0000 0008 5519 3cb9 d51b c541  blob....U.<....A
 0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
 0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-0000a080: 0000 0007 5000 0000 0009 0072 006f 0069  ....P......r.o.i
+0000a080: 0000 0009 8000 0000 0009 0072 006f 0069  ...........r.o.i
 0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
 0000a0a0: 6c6f 6e67 0000 0001 0000 0002 0073 0074  long.........s.t
-0000a0b0: 6c67 3153 636f 6d70 0000 0000 0000 30b5  lg1Scomp......0.
+0000a0b0: 6c67 3153 636f 6d70 0000 0000 0000 3102  lg1Scomp......1.
 0000a0c0: 0000 0002 0073 0074 6d6f 4444 626c 6f62  .....s.tmoDDblob
-0000a0d0: 0000 0008 16c0 6cac 051f c541 0000 0002  ......l....A....
+0000a0d0: 0000 0008 00a9 9ef5 7420 c541 0000 0002  ........t .A....
 0000a0e0: 0073 0074 6d6f 6444 626c 6f62 0000 0008  .s.tmodDblob....
-0000a0f0: 16c0 6cac 051f c541 0000 0002 0073 0074  ..l....A.....s.t
+0000a0f0: 00a9 9ef5 7420 c541 0000 0002 0073 0074  ....t .A.....s.t
 0000a100: 7068 3153 636f 6d70 0000 0000 0000 a000  ph1Scomp........
 0000a110: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
 0000a120: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
 0000a130: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
 0000a140: 006e 0064 0065 0072 0073 6277 7370 626c  .n.d.e.r.sbwspbl
 0000a150: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 0000a160: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
@@ -2592,15 +2592,15 @@
 0000a1f0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
 0000a200: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 0000a210: 0000 0000 0000 0000 0000 0000 0000 009b  ................
 0000a220: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
 0000a230: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
 0000a240: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
 0000a250: 006e 0064 0065 0072 0073 6c67 3153 636f  .n.d.e.r.slg1Sco
-0000a260: 6d70 0000 0000 0003 2437 0000 001b 0074  mp......$7.....t
+0000a260: 6d70 0000 0000 0004 0d76 0000 001b 0074  mp.......v.....t
 0000a270: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
 0000a280: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
 0000a290: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
 0000a2a0: 0072 0073 6c73 7643 626c 6f62 0000 0279  .r.slsvCblob...y
 0000a2b0: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
 0000a2c0: 0809 0a0b 1646 4748 0a5f 1012 7669 6577  .....FGH._..view
 0000a2d0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
@@ -2683,25 +2683,25 @@
 0000a7a0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
 0000a7b0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 0000a7c0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 0000a7d0: 1b00 7400 6800 6900 7200 6400 5f00 7000  ..t.h.i.r.d._.p.
 0000a7e0: 6100 7200 7400 7900 5f00 6c00 6100 6200  a.r.t.y._.l.a.b.
 0000a7f0: 6500 6c00 5f00 6100 7000 7000 6500 6e00  e.l._.a.p.p.e.n.
 0000a800: 6400 6500 7200 736d 6f44 4462 6c6f 6200  d.e.r.smoDDblob.
-0000a810: 0000 08ed 45eb 2346 19c5 4100 0000 1b00  ....E.#F..A.....
+0000a810: 0000 086b 121b 34c6 1fc5 4100 0000 1b00  ...k..4...A.....
 0000a820: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
 0000a830: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
 0000a840: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
 0000a850: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
-0000a860: 08ed 45eb 2346 19c5 4100 0000 1b00 7400  ..E.#F..A.....t.
+0000a860: 086b 121b 34c6 1fc5 4100 0000 1b00 7400  .k..4...A.....t.
 0000a870: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
 0000a880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
 0000a890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
 0000a8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-0000a8b0: 0400 0000 0000 1b00 7400 6800 6900 7200  ........t.h.i.r.
+0000a8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
 0000a8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000a8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000a8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
 0000a8f0: 6e6c 6f6e 6700 0000 0100 0000 0200 7500  nlong.........u.
 0000a900: 6962 7773 7062 6c6f 6200 0000 ca62 706c  ibwspblob....bpl
 0000a910: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
 0000a920: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
@@ -2713,15 +2713,15 @@
 0000a980: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
 0000a990: 3335 342c 2031 3234 7d2c 207b 3130 3736  354, 124}, {1076
 0000a9a0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
 0000a9b0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
 0000a9c0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 0000a9d0: 0000 0000 0000 9b00 0000 0200 7500 6964  ............u.id
 0000a9e0: 7363 6c62 6f6f 6c00 0000 0002 0075 0069  sclbool......u.i
-0000a9f0: 6c67 3153 636f 6d70 0000 0000 000d 9176  lg1Scomp.......v
+0000a9f0: 6c67 3153 636f 6d70 0000 0000 0011 9d6b  lg1Scomp.......k
 0000aa00: 0000 0002 0075 0069 6c73 7643 626c 6f62  .....u.ilsvCblob
 0000aa10: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
 0000aa20: 0405 0607 0809 0a0b 1846 4748 0a5f 1012  .........FGH._..
 0000aa30: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 0000aa40: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 0000aa50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 0000aa60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -2795,23 +2795,23 @@
 0000aea0: 4401 4501 4701 5001 5101 5201 5401 5601  D.E.G.P.Q.R.T.V.
 0000aeb0: 5f01 6001 6101 6301 6501 6e01 6f01 7001  _.`.a.c.e.n.o.p.
 0000aec0: 7201 7401 7d01 7e01 7f01 8101 8301 8c01  r.t.}.~.........
 0000aed0: 8e01 9101 9201 9301 9401 9d01 a201 ab00  ................
 0000aee0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
 0000aef0: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
 0000af00: 0000 0200 7500 696d 6f44 4462 6c6f 6200  ....u.imoDDblob.
-0000af10: 0000 0870 649a f46e 1cc5 4100 0000 0200  ...pd..n..A.....
-0000af20: 7500 696d 6f64 4462 6c6f 6200 0000 0870  u.imodDblob....p
-0000af30: 649a f46e 1cc5 4100 0000 0200 7500 6970  d..n..A.....u.ip
-0000af40: 6831 5363 6f6d 7000 0000 0000 1220 0049  h1Scomp...... .I
-0000af50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-0000af60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-0000af70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
-0000af80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000af90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
+0000af10: 0000 087e abce 1cd0 1fc5 4100 0000 0200  ...~......A.....
+0000af20: 7500 696d 6f64 4462 6c6f 6200 0000 087e  u.imodDblob....~
+0000af30: abce 1cd0 1fc5 4100 0000 0200 7500 6970  ......A.....u.ip
+0000af40: 6831 5363 6f6d 7000 0000 0000 17c0 0000  h1Scomp.........
+0000af50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+0000af60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
+0000af70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+0000af80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+0000af90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
@@ -2944,20 +2944,20 @@
 0000b7f0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 0000b800: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 0000b810: 0000 0000 0000 0000 0000 0000 9a00 1b00  ................
 0000b820: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
 0000b830: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
 0000b840: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
 0000b850: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
-0000b860: 08ed 45eb 2346 19c5 4100 0000 1b00 7400  ..E.#F..A.....t.
+0000b860: 086b 121b 34c6 1fc5 4100 0000 1b00 7400  .k..4...A.....t.
 0000b870: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
 0000b880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
 0000b890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
 0000b8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-0000b8b0: 0400 0000 0000 1b00 7400 6800 6900 7200  ........t.h.i.r.
+0000b8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
 0000b8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000b8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000b8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
 0000b8f0: 6e6c 6f6e 6700 0000 0100 0000 0200 7500  nlong.........u.
 0000b900: 6962 7773 7062 6c6f 6200 0000 ca62 706c  ibwspblob....bpl
 0000b910: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
 0000b920: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
@@ -2969,15 +2969,15 @@
 0000b980: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
 0000b990: 3335 342c 2031 3234 7d2c 207b 3130 3736  354, 124}, {1076
 0000b9a0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
 0000b9b0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
 0000b9c0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 0000b9d0: 0000 0000 0000 9b00 0000 0200 7500 6964  ............u.id
 0000b9e0: 7363 6c62 6f6f 6c00 0000 0002 0075 0069  sclbool......u.i
-0000b9f0: 6c67 3153 636f 6d70 0000 0000 000d 9176  lg1Scomp.......v
+0000b9f0: 6c67 3153 636f 6d70 0000 0000 0011 9d6b  lg1Scomp.......k
 0000ba00: 0000 0002 0075 0069 6c73 7643 626c 6f62  .....u.ilsvCblob
 0000ba10: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
 0000ba20: 0405 0607 0809 0a0b 1846 4748 0a5f 1012  .........FGH._..
 0000ba30: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 0000ba40: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 0000ba50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 0000ba60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -3051,23 +3051,23 @@
 0000bea0: 4401 4501 4701 5001 5101 5201 5401 5601  D.E.G.P.Q.R.T.V.
 0000beb0: 5f01 6001 6101 6301 6501 6e01 6f01 7001  _.`.a.c.e.n.o.p.
 0000bec0: 7201 7401 7d01 7e01 7f01 8101 8301 8c01  r.t.}.~.........
 0000bed0: 8e01 9101 9201 9301 9401 9d01 a201 ab00  ................
 0000bee0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
 0000bef0: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
 0000bf00: 0000 0200 7500 696d 6f44 4462 6c6f 6200  ....u.imoDDblob.
-0000bf10: 0000 0870 649a f46e 1cc5 4100 0000 0200  ...pd..n..A.....
-0000bf20: 7500 696d 6f64 4462 6c6f 6200 0000 0870  u.imodDblob....p
-0000bf30: 649a f46e 1cc5 4100 0000 0200 7500 6970  d..n..A.....u.ip
-0000bf40: 6831 5363 6f6d 7000 0000 0000 1220 0049  h1Scomp...... .I
-0000bf50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-0000bf60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-0000bf70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
-0000bf80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000bf90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
+0000bf10: 0000 087e abce 1cd0 1fc5 4100 0000 0200  ...~......A.....
+0000bf20: 7500 696d 6f64 4462 6c6f 6200 0000 087e  u.imodDblob....~
+0000bf30: abce 1cd0 1fc5 4100 0000 0200 7500 6970  ......A.....u.ip
+0000bf40: 6831 5363 6f6d 7000 0000 0000 17c0 0000  h1Scomp.........
+0000bf50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
+0000bf60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
+0000bf70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+0000bf80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+0000bf90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -276,23 +276,23 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 0002 404d 0000 000b 005f 005f 0070  ....@M....._._.p
+000011a0: 0000 0004 3e87 0000 000b 005f 005f 0070  ....>......_._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 d51e e6c2  moDDblob........
-000011d0: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 ea13 b999  moDDblob........
+000011d0: 8d20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-000011f0: 6444 626c 6f62 0000 0008 d51e e6c2 1b1f  dDblob..........
+000011f0: 6444 626c 6f62 0000 0008 ea13 b999 8d20  dDblob......... 
 00001200: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-00001220: 636f 6d70 0000 0000 0002 a000 0000 000b  comp............
+00001220: 636f 6d70 0000 0000 0004 f000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
 00001250: 0001 0000 0004 006d 0069 0073 0063 6277  .......m.i.s.cbw
 00001260: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 00001270: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00001280: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001290: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.5/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/requirements.txt` & `Simba-UW-tf-dev-1.63.5/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_processors/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0008 db95 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0000 a209 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 e768 c2c2  moDDblob.....h..
-00000160: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 beac 8729  moDDblob.......)
+00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 e768 c2c2 1b1f  dDblob.....h....
+00000180: 6444 626c 6f62 0000 0008 beac 8729 7b20  dDblob.......){ 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0009 b000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0001 4000 0000 0000  comp......@.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.63.5/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.63.5/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.63.5/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.5/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.63.5/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.63.5/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.63.5/simba/mixins/train_model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 from concurrent.futures.process import BrokenProcessPool
 from itertools import repeat
 import configparser
 import platform
 from sklearn.utils import parallel_backend
 import pickle
 import concurrent
-from dtreeviz.trees import tree, dtreeviz
+try:
+    from dtreeviz.trees import tree, dtreeviz
+except:
+    import dtreeviz
 import matplotlib.pyplot as plt
 import multiprocessing
 import functools
 from typing import List, Optional, Union, Dict, Any
 try:
     from typing import Literal
 except:
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0001 c8b0 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0002 aed8 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 67ae e6c2  moDDblob....g...
-00000160: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 69d4 8a29  moDDblob....i..)
+00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 67ae e6c2 1b1f  dDblob....g.....
+00000180: 6444 626c 6f62 0000 0008 69d4 8a29 7b20  dDblob....i..){ 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0002 6000 0000 0000  comp......`.....
+000001b0: 636f 6d70 0000 0000 0003 9000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 000002b0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
 000002c0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
 000002d0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
 000002e0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
 000002f0: 0000 0000 0000 0000 0000 9a00 0000 0b00  ................
 00000300: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 00000310: 6500 5f00 5f6c 6731 5363 6f6d 7000 0000  e._._lg1Scomp...
-00000320: 0000 017d af00 0000 0b00 5f00 5f00 7000  ...}......_._.p.
+00000320: 0000 023b 6f00 0000 0b00 5f00 5f00 7000  ...;o....._._.p.
 00000330: 7900 6300 6100 6300 6800 6500 5f00 5f6d  y.c.a.c.h.e._._m
-00000340: 6f44 4462 6c6f 6200 0000 08f7 cfab be1b  oDDblob.........
-00000350: 1fc5 4100 0000 0b00 5f00 5f00 7000 7900  ..A....._._.p.y.
+00000340: 6f44 4462 6c6f 6200 0000 088b 5608 147b  oDDblob.....V..{
+00000350: 20c5 4100 0000 0b00 5f00 5f00 7000 7900   .A....._._.p.y.
 00000360: 6300 6100 6300 6800 6500 5f00 5f6d 6f64  c.a.c.h.e._._mod
-00000370: 4462 6c6f 6200 0000 08f7 cfab be1b 1fc5  Dblob...........
+00000370: 4462 6c6f 6200 0000 088b 5608 147b 20c5  Dblob.....V..{ .
 00000380: 4100 0000 0b00 5f00 5f00 7000 7900 6300  A....._._.p.y.c.
 00000390: 6100 6300 6800 6500 5f00 5f70 6831 5363  a.c.h.e._._ph1Sc
-000003a0: 6f6d 7000 0000 0000 0220 0000 0000 0b00  omp...... ......
+000003a0: 6f6d 7000 0000 0000 0330 0000 0000 0b00  omp......0......
 000003b0: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 000003c0: 6500 5f00 5f76 5372 6e6c 6f6e 6700 0000  e._._vSrnlong...
 000003d0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.63.5/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/enums.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
     PARTIAL_DEPENDENCY = 'partial_dependency'
     TRAIN_TEST_SPLIT_TYPE = 'train_test_split_type'
 
 class OS(Enum):
     WINDOWS = 'Windows'
     LINUX = 'Linux'
     MAC = 'Darwin'
-    PYTHON_VER = float(f'{sys.version_info.major}.{sys.version_info.minor}')
+    PYTHON_VER = str(f'{sys.version_info.major}.{sys.version_info.minor}')
 
 class Links(Enum):
     FEATURE_SUBSETS = 'https://github.com/sgoldenlab/simba/blob/master/docs/feature_subsets.md'
     HEATMAP_LOCATION = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#heatmaps'
     HEATMAP_CLF = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-classification-heatmaps'
     DATA_TABLES = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-data-tables'
     CONCAT_VIDEOS = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#merging-concatenating-videos'
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/utils/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -253,23 +253,23 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0004 15bd 0000 000b 005f 005f 0070  ..........._._.p
+00001030: 0000 0006 042d 0000 000b 005f 005f 0070  .....-....._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 0480 4f38  moDDblob......O8
-00001060: 1d1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 693d 1a27  moDDblob....i=.'
+00001060: ee20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 0480 4f38 1d1f  dDblob......O8..
+00001080: 6444 626c 6f62 0000 0008 693d 1a27 ee20  dDblob....i=.'. 
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0004 e000 0000 0003  comp............
+000010b0: 636f 6d70 0000 0000 0007 2000 0000 0003  comp...... .....
 000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
 000010d0: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 000010e0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 000010f0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
 00001100: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
 00001110: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00001120: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/checks.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/lookups.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,30 +127,40 @@
             'BENTO': 'annot'}
 
 
 def get_emojis() -> dict:
     """
     Helper to get dictionary of emojis with names as keys and emojis as values.
     """
-    python_version = float(f'{sys.version_info.major}.{sys.version_info.minor}')
-    if python_version <= 3.6:
+    python_version = str(f'{sys.version_info.major}.{sys.version_info.minor}')
+    if python_version == '3.6':
         return {'thank_you': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001f64f'.encode('utf-16be'))),
                 'relaxed': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F600'.encode('utf-16be'))),
                 'error': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F6A8'.encode('utf-16be'))),
                 'complete': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F680'.encode('utf-16be'))),
                 'warning': ''.join(chr(x) for x in struct.unpack('>2H', '\u2757\uFE0F'.encode('utf-16be'))),
                 'trash': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F5D1'.encode('utf-16be')))}
 
-    if python_version > 3.6:
+    if python_version == '3.10':
+        return {'thank_you': '\U0001f64f'.encode('utf-8', 'replace').decode(),
+                'relaxed': '\U0001F600'.encode('utf-8', 'replace').decode(),
+                'warning': '\u2757\uFE0F'.encode('utf-8', 'replace').decode(),
+                'error': '\U0001F6A8'.encode('utf-8', 'replace').decode(),
+                'complete': '\U0001F680'.encode('utf-8', 'replace').decode(),
+                'trash': '\U0001F5D1'.encode('utf-8', 'replace').decode()}
+
+    if python_version == '3.7':
         return {'thank_you': '\U0001f64f'.encode('utf16', errors='surrogatepass').decode('utf16'),
                 'relaxed': '\U0001F600'.encode('utf16', errors='surrogatepass').decode('utf16'),
                 'error': '\U0001F6A8'.encode('utf16', errors='surrogatepass').decode('utf16'),
                 'complete': '\U0001F680'.encode('utf16', errors='surrogatepass').decode('utf16'),
                 'warning': '\u2757\uFE0F'.encode('utf16', errors='surrogatepass').decode('utf16'),
-                'trash': 'U0001F5D1F'.encode('utf16', errors='surrogatepass').decode('utf16')}
+                'trash': '\U0001F5D1F'.encode('utf16', errors='surrogatepass').decode('utf16')}
+
+
 
 
 def get_meta_data_file_headers() -> List[str]:
     """
     Get List of headers for SimBA classifier metadata output.
 
     :return List[str]:
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/errors.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/data.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/utils/printing.py` & `Simba-UW-tf-dev-1.63.5/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.63.5/simba/st/select_groups_pg.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,8 +45,8 @@
         grid_options = gb.build()
         self.data_df = AgGrid(self.data_df, gridOptions=grid_options, allallow_unsafe_jscode=True)
         st.write("---")
 
         file_path = st.file_uploader("Import file")
         if file_path is not None:
             self.data_df = pd.read_csv(file_path)
-            st.info('Data has been loaded.')
+            st.info('Group data loaded.')
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.63.5/simba/st/aggregate_statistics.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,26 +20,30 @@
     def read_data(_config: ConfigReader) -> pd.DataFrame:
         return TrainModelMixin().read_all_files_in_folder_mp(file_paths=_config.machine_results_paths,
                                                              file_type=_config.file_type,
                                                              classifier_names=_config.clf_names)
 
     @staticmethod
     @st.experimental_memo
-    def aggregator(df: pd.DataFrame, video_info: pd.DataFrame, agg_type: str, clf: str) -> pd.DataFrame:
-        if agg_type == 'VIDEO':
-            df = df.groupby('VIDEO')[clf].agg(['sum', 'count']).rename(columns={'sum': 'clf_frame_count', 'count': 'video_frame_count'})
-            df['fps'] = df.index
-            df['fps'] = df['fps'].map(video_info[['Video', 'fps']].set_index('Video').squeeze().to_dict())
-            df[f'{clf} (seconds)'] = round(df['clf_frame_count'] / df['fps'], 3)
-            df[f'{clf} (% session)'] = round(df['clf_frame_count'] / df['video_frame_count'], 3)
-        else:
-            pass
+    def video_aggregator(df: pd.DataFrame, video_info: pd.DataFrame, clf: str) -> pd.DataFrame:
+        df = df.groupby('VIDEO')[clf].agg(['sum', 'count']).rename(columns={'sum': 'clf_frame_count', 'count': 'video_frame_count'})
+        df['fps'] = df.index
+        df['fps'] = df['fps'].map(video_info[['Video', 'fps']].set_index('Video').squeeze().to_dict())
+        df[f'{clf} (seconds)'] = round(df['clf_frame_count'] / df['fps'], 3)
+        df[f'{clf} (% session)'] = round(df['clf_frame_count'] / df['video_frame_count'], 3)
 
         return df.reset_index()
 
+    def group_aggregator(df: pd.DataFrame, video_info: pd.DataFrame, clf: str, group_df: pd.DataFrame) -> pd.DataFrame:
+        pass
+
     def run(self):
         data = self.read_data(_config=self.config).reset_index().rename(columns={'index': 'VIDEO'})
-        df = self.aggregator(df=data, video_info=self.config.video_info_df, agg_type=self.select_agg, clf=self.select_clf)
         if self.select_agg == 'VIDEO':
+            df = self.video_aggregator(df=data, video_info=self.config.video_info_df, clf=self.select_clf)
             chart = (alt.Chart(df).mark_bar().encode(alt.X("VIDEO"), alt.Y(f"{self.select_clf} (seconds)"), alt.Color("VIDEO"), alt.Tooltip("VIDEO")).interactive())
-            st.altair_chart(chart, use_container_width=True)
+        if self.select_agg == 'VIDEO':
+            pass
+
+
+        st.altair_chart(chart, use_container_width=True)
         st.write("---")
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/st/app.py` & `Simba-UW-tf-dev-1.63.5/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/mixins/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0000 722e 0000 000b 005f 005f 0070  ....r......_._.p
+00000130: 0000 000b ead3 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 3d3b e5c2  moDDblob....=;..
-00000160: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 26a2 1753  moDDblob....&..S
+00000160: ee20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 3d3b e5c2 1b1f  dDblob....=;....
+00000180: 6444 626c 6f62 0000 0008 26a2 1753 ee20  dDblob....&..S. 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0000 e000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 000c f000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/.DS_Store`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,35 +26,35 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
+00000200: 0000 0000 0000 0000 0000 0009 0000 000b  ................
 00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000230: 0000 0006 ec07 0000 000b 005f 005f 0070  ..........._._.p
+00000230: 0000 0002 3883 0000 000b 005f 005f 0070  ....8......_._.p
 00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 d3cb d3c2  moDDblob........
-00000260: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000250: 6d6f 4444 626c 6f62 0000 0008 fb7c 3914  moDDblob.....|9.
+00000260: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000280: 6444 626c 6f62 0000 0008 d3cb d3c2 1b1f  dDblob..........
+00000280: 6444 626c 6f62 0000 0008 fb7c 3914 7b20  dDblob.....|9.{ 
 00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000002b0: 636f 6d70 0000 0000 0009 0000 0000 0005  comp............
-000002c0: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
-000002d0: 6d70 0000 0000 0000 3d66 0000 0005 0074  mp......=f.....t
-000002e0: 006f 006f 006c 0073 6d6f 4444 626c 6f62  .o.o.l.smoDDblob
-000002f0: 0000 0008 1e86 d77f cc0c c541 0000 0005  ...........A....
-00000300: 0074 006f 006f 006c 0073 6d6f 6444 626c  .t.o.o.l.smodDbl
-00000310: 6f62 0000 0008 1e86 d77f cc0c c541 0000  ob...........A..
-00000320: 0005 0074 006f 006f 006c 0073 7068 3153  ...t.o.o.l.sph1S
-00000330: 636f 6d70 0000 0000 0000 6000 0000 0000  comp......`.....
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 636f 6d70 0000 0000 0003 0000 0000 0004  comp............
+000002c0: 006d 0069 0073 0063 6473 636c 626f 6f6c  .m.i.s.cdsclbool
+000002d0: 0000 0000 0400 6d00 6900 7300 636c 6731  ......m.i.s.clg1
+000002e0: 5363 6f6d 7000 0000 0000 0037 0b00 0000  Scomp......7....
+000002f0: 0400 6d00 6900 7300 636d 6f44 4462 6c6f  ..m.i.s.cmoDDblo
+00000300: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
+00000310: 0400 6d00 6900 7300 636d 6f64 4462 6c6f  ..m.i.s.cmodDblo
+00000320: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
+00000330: 0400 6d00 6900 7300 6370 6831 5363 6f6d  ..m.i.s.cph1Scom
+00000340: 7000 0000 0000 0040 0000 0000 0000 0000  p......@........
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/pose_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
                 pool.terminate()
                 pool.join()
 
             print(f'Joining {video_name} multi-processed video...')
             concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=save_video_path, remove_splits=True)
             video_timer.stop_timer()
             stdout_success(msg=f'Pose video {video_name} complete', elapsed_time=video_timer.elapsed_time_str)
-
         self.config.timer.stop_timer()
         stdout_success(f'Pose visualizations for {len(list(self.data.keys()))} video(s) created in {self.out_dir} directory', elapsed_time=self.config.timer.elapsed_time_str)
 
 # test = PosePlotter(in_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/outlier_corrected_movement_location',
 #                    out_dir='/Users/simon/Desktop/video_tests_',
 #                    sample_time=5,
 #                    circle_size=10,
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.63.5/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.63.5/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.63.5/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.63.5/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/bounding_box_tools/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0002 fed9 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0001 f276 0000 000b 005f 005f 0070  .....v....._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 20e0 e7c2  moDDblob.... ...
-00000160: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 190a 9a29  moDDblob.......)
+00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 20e0 e7c2 1b1f  dDblob.... .....
+00000180: 6444 626c 6f62 0000 0008 190a 9a29 7b20  dDblob.......){ 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0004 0000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0002 7000 0000 0000  comp......p.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/fsttc_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         """
 
         self.find_sequences()
         self.results_dict = {}
         for video_name, video_data in self.video_sequence_dict.items():
             self.results_dict[video_name] = {}
             fps, session_frames = video_data['fps'], video_data['session_length_frames']
+            #print(video_data['session_length_frames'])
             for first_clf, second_clf in self.clf_permutations:
                 if first_clf not in self.results_dict[video_name].keys():
                     self.results_dict[video_name][first_clf] = {}
                 self.results_dict[video_name][first_clf][second_clf] = {}
                 sequence_data = video_data[f'FSTTC {first_clf} {second_clf}']
                 if sequence_data is None:
                     self.results_dict[video_name][first_clf][second_clf] = 'No events'
@@ -164,14 +165,15 @@
                         self.results_dict[video_name][first_clf][second_clf] = 0.0
                     else:
                         clf_1_2_df = sequence_data[(sequence_data['First behaviour'] == first_clf) & (sequence_data['Second behaviour'] == second_clf)]
                         P = len_clf_1_2 / len_clf_1
                         Ta = sum(clf_1_2_df['Total_window_frames']) / session_frames
                         Tb = sum(clf_1_2_df['Time 2nd behaviour start to time window end']) / session_frames
                         self.results_dict[video_name][first_clf][second_clf] = 0.5 * ((P - Tb) / (1 - (P * Tb)) + ((P - Ta) / (1 - (P * Ta))))
+                        #print(self.results_dict[video_name][first_clf][second_clf])
         self.save()
         if self.graph_status:
             self.plot_FSTTC()
 
     def plot_FSTTC(self):
         """
         Method to visualize forward spike-time tiling coefficients (FSTTC) as png violin plots. Results are stored on
@@ -208,19 +210,28 @@
                     self.out_df.loc[len(self.out_df)] = [video_name, first_behavior, second_behavior, fsttc]
         self.file_save_path = os.path.join(self.logs_path, 'FSTTC_{}.csv'.format(str(self.datetime)))
         self.out_df.to_csv(self.file_save_path)
         self.timer.stop_timer()
         stdout_success(msg=f'FSTTC data saved at {self.file_save_path}', elapsed_time=self.timer.elapsed_time_str)
 
 # test = FSTTCCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                      time_window=2000,
+#                      time_window=10000,
 #                      behavior_lst=['Attack', 'Sniffing'],
 #                     create_graphs=False)
 # test.run()
 
+
+# test = FSTTCCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                       time_window=600000,
+#                       behavior_lst=['licking_grooming', 'active_nursing'], #'passive_nursing', 'nest_attendance'
+#                       create_graphs=False)
+# test.run()
+
+
+
 #
 # test = FSTTCCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini',
 #                      time_window=2000,
 #                      behavior_lst=['Erratic Turning', 'Bottom', 'Normal Swimming', 'Freezing', 'Wall Bumping'],
 #                     create_graphs=True)
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.63.5/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/model/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 000002b0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
 000002c0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
 000002d0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
 000002e0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
 000002f0: 0000 0000 0000 0000 0000 9a00 0000 0b00  ................
 00000300: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 00000310: 6500 5f00 5f6c 6731 5363 6f6d 7000 0000  e._._lg1Scomp...
-00000320: 0000 00d2 7c00 0000 0b00 5f00 5f00 7000  ....|....._._.p.
+00000320: 0000 013b f600 0000 0b00 5f00 5f00 7000  ...;......_._.p.
 00000330: 7900 6300 6100 6300 6800 6500 5f00 5f6d  y.c.a.c.h.e._._m
-00000340: 6f44 4462 6c6f 6200 0000 0897 88b1 bf1b  oDDblob.........
-00000350: 1fc5 4100 0000 0b00 5f00 5f00 7000 7900  ..A....._._.p.y.
+00000340: 6f44 4462 6c6f 6200 0000 0878 db7a 237b  oDDblob....x.z#{
+00000350: 20c5 4100 0000 0b00 5f00 5f00 7000 7900   .A....._._.p.y.
 00000360: 6300 6100 6300 6800 6500 5f00 5f6d 6f64  c.a.c.h.e._._mod
-00000370: 4462 6c6f 6200 0000 0897 88b1 bf1b 1fc5  Dblob...........
+00000370: 4462 6c6f 6200 0000 0878 db7a 237b 20c5  Dblob....x.z#{ .
 00000380: 4100 0000 0b00 5f00 5f00 7000 7900 6300  A....._._.p.y.c.
 00000390: 6100 6300 6800 6500 5f00 5f70 6831 5363  a.c.h.e._._ph1Sc
-000003a0: 6f6d 7000 0000 0000 0100 0000 0000 0b00  omp.............
+000003a0: 6f6d 7000 0000 0000 0180 0000 0000 0b00  omp.............
 000003b0: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 000003c0: 6500 5f00 5f76 5372 6e6c 6f6e 6700 0000  e._._vSrnlong...
 000003d0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.63.5/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.63.5/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.63.5/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/data_processors/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0003 66d1 0000 000b 005f 005f 0070  ....f......_._.p
+00000130: 0000 0004 7300 0000 000b 005f 005f 0070  ....s......_._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 e267 c4c2  moDDblob.....g..
-00000160: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 1f94 bb4d  moDDblob.......M
+00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 e267 c4c2 1b1f  dDblob.....g....
+00000180: 6444 626c 6f62 0000 0008 1f94 bb4d 7b20  dDblob.......M{ 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0004 7000 0000 0000  comp......p.....
+000001b0: 636f 6d70 0000 0000 0005 f000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.63.5/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/plotting/.DS_Store`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,35 +26,35 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0009 0000 000b  ................
+00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
 00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000230: 0000 0001 7a92 0000 000b 005f 005f 0070  ....z......_._.p
+00000230: 0000 000a 5a7d 0000 000b 005f 005f 0070  ....Z}....._._.p
 00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 9123 7abf  moDDblob.....#z.
-00000260: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000250: 6d6f 4444 626c 6f62 0000 0008 a566 122d  moDDblob.....f.-
+00000260: ee20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
 00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000280: 6444 626c 6f62 0000 0008 9123 7abf 1b1f  dDblob.....#z...
+00000280: 6444 626c 6f62 0000 0008 a566 122d ee20  dDblob.....f.-. 
 00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000002b0: 636f 6d70 0000 0000 0002 0000 0000 0004  comp............
-000002c0: 006d 0069 0073 0063 6473 636c 626f 6f6c  .m.i.s.cdsclbool
-000002d0: 0000 0000 0400 6d00 6900 7300 636c 6731  ......m.i.s.clg1
-000002e0: 5363 6f6d 7000 0000 0000 0037 0b00 0000  Scomp......7....
-000002f0: 0400 6d00 6900 7300 636d 6f44 4462 6c6f  ..m.i.s.cmoDDblo
-00000300: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
-00000310: 0400 6d00 6900 7300 636d 6f64 4462 6c6f  ..m.i.s.cmodDblo
-00000320: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
-00000330: 0400 6d00 6900 7300 6370 6831 5363 6f6d  ..m.i.s.cph1Scom
-00000340: 7000 0000 0000 0040 0000 0000 0000 0000  p......@........
+000002b0: 636f 6d70 0000 0000 000d 7000 0000 0005  comp......p.....
+000002c0: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
+000002d0: 6d70 0000 0000 0000 50f8 0000 0005 0074  mp......P......t
+000002e0: 006f 006f 006c 0073 6d6f 4444 626c 6f62  .o.o.l.smoDDblob
+000002f0: 0000 0008 1e86 d77f cc0c c541 0000 0005  ...........A....
+00000300: 0074 006f 006f 006c 0073 6d6f 6444 626c  .t.o.o.l.smodDbl
+00000310: 6f62 0000 0008 1e86 d77f cc0c c541 0000  ob...........A..
+00000320: 0005 0074 006f 006f 006c 0073 7068 3153  ...t.o.o.l.sph1S
+00000330: 636f 6d70 0000 0000 0000 8000 0000 0000  comp............
+00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.63.5/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.63.5/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.63.5/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.63.5/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.63.5/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.63.5/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.5/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/SimBA.py` & `Simba-UW-tf-dev-1.63.5/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,23 +833,22 @@
         y_sb.config(command=self.txt.yview)
         self.txt.config(state=DISABLED, font=Formats.TKINTER_FONT.value)
 
         clear_txt_btn = Button(self.frame, text=' CLEAR', compound=LEFT, image=self.menu_icons['clean']['img'], font=Formats.LABELFRAME_HEADER_FORMAT.value, command=lambda: self.clean_txt())
         clear_txt_btn.pack(side=BOTTOM, fill=X)
         sys.stdout = StdRedirector(self.txt)
 
-        if OS.PYTHON_VER.value != 3.6:
-            PythonVersionWarning(msg=f'SimBA is not extensively tested beyond python3.6. You are using python{OS.PYTHON_VER.value}. If you encounter errors, in python>={OS.PYTHON_VER.value}, please report them on GitHub or Gitter and w (links in the help toolbar)')
+        if OS.PYTHON_VER.value != '3.6':
+            PythonVersionWarning(msg=f'SimBA is not extensively tested beyond python 3.6. You are using python {OS.PYTHON_VER.value}. If you encounter errors in python>3.6, please report them on GitHub or Gitter and we will fix! (links in the help toolbar)')
 
     def restart(self):
         confirm_restart = askyesno(title='RESTART', message='Are you sure that you want restart SimBA?')
         if confirm_restart:
             self.root.destroy()
-            python = sys.executable
-            os.execl(python, python, *sys.argv)
+            os.execl(sys.executable, sys.executable, *sys.argv)
 
     def clean_txt(self):
         self.txt.config(state=NORMAL)
         self.txt.delete('1.0', END)
 
     def show_right_click_pop_up(self, event):
         try:
@@ -943,15 +942,15 @@
             ret, frame = self.cap.read()
             if not ret: break
             frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGBA)
             frame = ImageTk.PhotoImage(image=PIL.Image.fromarray(frame))
             self.img_lbl.configure(image=frame)
             self.img_lbl.imgtk = frame
             self.parent.update()
-            cv2.waitKey(int(self.meta_['fps'] / 1000))
+            cv2.waitKey(max(33, int(self.meta_['fps'] / 1000)))
         self.parent.destroy()
 
 def terminate_children(children):
     for process in children:
         process.terminate()
 
 def main():
```

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.63.5/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.63.5/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.5/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.63.5/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.63.5/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.63.5/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.63.5/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.63.5/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.63.5/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.63.5/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.63.5/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.63.5/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.63.5/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.5/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.63.5/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.63.5/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.63.5/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.4
+Version: 1.63.5
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,15 @@
 simba/feature_extractors/misc/video_rotator.py
 simba/feature_extractors/misc/video_rotator_mp.py
 simba/labelling/.DS_Store
 simba/labelling/__init__.py
 simba/labelling/extract_labelled_frames.py
 simba/labelling/labelling_advanced_interface.py
 simba/labelling/labelling_interface.py
+simba/labelling/labelling_interface_old.py
 simba/labelling/play_annotation_video.py
 simba/mixins/.DS_Store
 simba/mixins/__init__.py
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/plotting_mixin.py
 simba/mixins/pop_up_mixin.py
@@ -255,15 +256,14 @@
 simba/plotting/heat_mapper_location.py
 simba/plotting/heat_mapper_location_mp.py
 simba/plotting/interactive_probability_grapher.py
 simba/plotting/path_plotter.py
 simba/plotting/path_plotter_mp.py
 simba/plotting/plot_clf_results.py
 simba/plotting/plot_clf_results_mp.py
-simba/plotting/plot_pose_in_dir.py
 simba/plotting/pose_plotter_mp.py
 simba/plotting/probability_plot_creator.py
 simba/plotting/probability_plot_creator_mp.py
 simba/plotting/shap_agg_stats_visualizer.py
 simba/plotting/single_run_model_validation_video.py
 simba/plotting/single_run_model_validation_video_mp.py
 simba/plotting/tools/tkinter_tools.py
```

### Comparing `Simba-UW-tf-dev-1.63.4/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.63.5/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/LICENSE.md` & `Simba-UW-tf-dev-1.63.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.63.5/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.63.5/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.63.5/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.63.5/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.5/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.63.5/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.63.5/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.63.5/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.63.5/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.63.5/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.63.5/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.63.5/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.63.5/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.63.5/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.63.5/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/README.md` & `Simba-UW-tf-dev-1.63.5/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.4/setup.py` & `Simba-UW-tf-dev-1.63.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.63.4",
+    version="1.63.5",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

