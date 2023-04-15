# Comparing `tmp/Simba-UW-tf-dev-1.56.2.tar.gz` & `tmp/Simba-UW-tf-dev-1.56.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.2.tar", last modified: Wed Apr 12 13:54:04 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.3.tar", last modified: Sat Apr 15 19:01:08 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.56.2.tar` & `Simba-UW-tf-dev-1.56.3.tar`

### file list

```diff
@@ -1,385 +1,389 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/
--rw-r--r--   0 simon      (501) staff       (20)    32475 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.2/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/misc.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/data_extractors.py
--rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/dbcv.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/umap_embedder.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualization_tools/
--rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualization_tools/vtk_embeddings.py
--rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/ui_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19383 2023-04-12 13:53:16.000000 Simba-UW-tf-dev-1.56.2/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-11 16:58:43.000000 Simba-UW-tf-dev-1.56.2/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42839 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21591 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21399 2023-04-11 16:58:31.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28019 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-11 20:41:01.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2317 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36798 2023-03-15 17:04:48.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46505 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24092 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16809 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.2/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.2/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.2/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41856 2023-04-05 17:24:50.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34563 2023-04-10 20:12:42.000000 Simba-UW-tf-dev-1.56.2/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12866 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.2/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.2/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.2/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.2/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     4142 2023-04-12 12:21:03.000000 Simba-UW-tf-dev-1.56.2/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14398 2023-04-10 19:08:11.000000 Simba-UW-tf-dev-1.56.2/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.2/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.2/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    46383 2023-04-10 20:10:32.000000 Simba-UW-tf-dev-1.56.2/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.2/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.2/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     3798 2023-04-12 13:45:31.000000 Simba-UW-tf-dev-1.56.2/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.2/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.2/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9548 2023-04-06 00:40:25.000000 Simba-UW-tf-dev-1.56.2/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.2/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.2/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.2/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14661 2023-04-10 20:11:46.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.2/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56847 2023-04-10 15:09:41.000000 Simba-UW-tf-dev-1.56.2/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16536 2023-03-20 13:30:18.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   232870 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.2/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.2/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64156 2023-04-12 13:52:14.000000 Simba-UW-tf-dev-1.56.2/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-11 20:46:03.000000 Simba-UW-tf-dev-1.56.2/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    21460 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.2/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8085 2023-04-12 13:31:27.000000 Simba-UW-tf-dev-1.56.2/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.2/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20742 2023-04-10 19:52:46.000000 Simba-UW-tf-dev-1.56.2/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.2/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13039 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      638 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.2/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.2/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.2/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1895 2023-04-12 13:53:57.000000 Simba-UW-tf-dev-1.56.2/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.3/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.3/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/misc.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/data_extractors.py
+-rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/dbcv.py
+-rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/umap_embedder.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualization_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualization_tools/vtk_embeddings.py
+-rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/ui_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19445 2023-04-14 17:48:54.000000 Simba-UW-tf-dev-1.56.3/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-13 14:09:44.000000 Simba-UW-tf-dev-1.56.3/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21399 2023-04-11 16:58:31.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-11 20:41:01.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36715 2023-04-14 16:41:10.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.3/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.3/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.3/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41904 2023-04-14 10:42:10.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34563 2023-04-10 20:12:42.000000 Simba-UW-tf-dev-1.56.3/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.3/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12866 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.3/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.3/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.3/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.3/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.3/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.3/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14398 2023-04-10 19:08:11.000000 Simba-UW-tf-dev-1.56.3/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.3/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.3/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    46716 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.3/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.3/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.3/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.3/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     3798 2023-04-12 13:45:31.000000 Simba-UW-tf-dev-1.56.3/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.3/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.3/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.3/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.3/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.3/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.3/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14661 2023-04-10 20:11:46.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.3/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56820 2023-04-15 18:59:15.000000 Simba-UW-tf-dev-1.56.3/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.3/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.3/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.3/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.3/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-13 18:18:32.000000 Simba-UW-tf-dev-1.56.3/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.3/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.3/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.3/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20742 2023-04-10 19:52:46.000000 Simba-UW-tf-dev-1.56.3/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.3/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13203 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      638 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.3/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.3/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.3/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1895 2023-04-15 19:00:54.000000 Simba-UW-tf-dev-1.56.3/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.56.2/PKG-INFO` & `Simba-UW-tf-dev-1.56.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.2
+Version: 1.56.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/video_processing.py` & `Simba-UW-tf-dev-1.56.3/simba/video_processing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 __author__ = "Simon Nilsson"
 
 import glob, os
 from simba.read_config_unit_tests import (check_file_exist_and_readable,
-                                          check_int)
-from simba.misc_tools import (get_fn_ext, get_video_meta_data)
+                                          check_int, check_if_filepath_list_is_empty)
+import threading
+from simba.misc_tools import (get_fn_ext,
+                              get_video_meta_data,
+                              find_all_videos_in_directory,
+                              find_core_cnt)
 from simba.utils.printing import stdout_success
 import cv2
 from pathlib import Path
-from PIL import Image
+import numpy as np
 from simba.extract_frames_fast import video_to_frames
 from simba.enums import Formats
 import re
 import subprocess
 import simba
+from simba.mixins.config_reader import ConfigReader
+from tkinter import *
+from datetime import datetime
+import time
+from PIL import Image, ImageTk
 from simba.utils.errors import (NotDirectoryError,
                                 NoFilesFoundError,
                                 FileExistError,
                                 CountError,
                                 InvalidInputError)
-from simba.utils.warnings import SameInputAndOutputWarning, FileExistWarning
+from simba.utils.warnings import (SameInputAndOutputWarning,
+                                  FileExistWarning)
+from concurrent.futures import ProcessPoolExecutor
+import multiprocessing
+import functools
 
+MAX_FRM_SIZE = 1080, 650
 
 def change_img_format(directory: str,
                       file_type_in: str,
                       file_type_out: str):
     """
     Helper to convert file type of all image files in a folder.
 
@@ -695,14 +709,147 @@
     if horizontal:
         command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale=-1:{}[v0];[v0][1:v]hstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['height'], save_path)
     else:
         command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale={}:-1[v0];[v0][1:v]vstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['width'], save_path)
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'Videos concatenated and saved at {save_path}')
 
+
+
+
+def _rotate_video(data: list,
+                  video_meta_info: dict,
+                  input_path: str,
+                  save_path: str,
+                  rotation_matrix: np.array):
+
+
+    cap = cv2.VideoCapture(input_path)
+
+    img_cnt = 0
+    while True:
+        ret, img = cap.read()
+        if not ret:
+            break
+        img = cv2.warpAffine(img, rotation_matrix, (video_meta_info['width'], video_meta_info['height']))
+        print(img)
+        writer.write(img)
+        img_cnt+=1
+        print(f'Rotating frame {img_cnt}/{video_meta_info["frame_count"]}')
+    cap.release()
+    writer.release()
+
+
+class VideoRotator(ConfigReader):
+    def __init__(self,
+                 input_path: str,
+                 output_dir: str):
+        _, self.cpu_cnt  = find_core_cnt()
+        self.save_dir = output_dir
+        self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
+        if os.path.isfile(input_path):
+            self.video_paths = [input_path]
+        else:
+            self.video_paths = find_all_videos_in_directory(directory=input_path, as_dict=True).values()
+            check_if_filepath_list_is_empty(filepaths=self.video_paths, error_msg=f'No videos found in {input_path} directory')
+
+    def __insert_img(self, img: np.array):
+        current_frm_pil = Image.fromarray(img)
+        current_frm_pil.thumbnail(MAX_FRM_SIZE, Image.ANTIALIAS)
+        current_frm_pil = ImageTk.PhotoImage(master=self.main_frm, image=current_frm_pil)
+        self.video_frame = Label(self.main_frm, image=current_frm_pil)
+        self.video_frame.image = current_frm_pil
+        self.video_frame.grid(row=0, column=0)
+
+    def __rotate(self, value: int, img: np.array):
+        self.dif_angle += value
+        rotation_matrix = cv2.getRotationMatrix2D((self.video_meta_data['width'] / 2, self.video_meta_data['height'] / 2), self.dif_angle, 1)
+        img = cv2.warpAffine(img, rotation_matrix, (self.video_meta_data['width'], self.video_meta_data['height']))
+        self.__insert_img(img=img)
+
+    def __run_rotation(self):
+        self.main_frm.destroy()
+        start = time.time()
+        for video_cnt, (video_path, rotation) in enumerate(self.results.items()):
+            cap = cv2.VideoCapture(video_path)
+            _, name, _ = get_fn_ext(filepath=video_path)
+            rotation_matrix = cv2.getRotationMatrix2D((self.video_meta_data['width'] / 2, self.video_meta_data['height'] / 2), rotation, 1)
+            save_path = os.path.join(self.save_dir, f'{name}_rotated_{self.datetime}.mp4')
+            video_meta = get_video_meta_data(video_path=video_path)
+            fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
+            writer = cv2.VideoWriter(save_path, fourcc, video_meta['fps'],(video_meta['width'], video_meta['height']))
+            img_cnt = 0
+            while True:
+                ret, img = cap.read()
+                if not ret:
+                    break
+                img = cv2.warpAffine(img, rotation_matrix,
+                                     (self.video_meta_data['width'], self.video_meta_data['height']))
+                writer.write(img)
+                img_cnt += 1
+                print(
+                    f'Rotating frame {img_cnt}/{video_meta["frame_count"]} (Video {video_cnt + 1}/{len(self.results.keys())}) ')
+            cap.release()
+            writer.release()
+        stdout_success(msg=f'All videos rotated and saved in {self.save_dir}', elapsed_time=str(round((time.time() - start), 2)))
+
+    def __save(self):
+        process = None
+        self.results[self.file_path] = self.dif_angle
+        if len(self.results.keys()) == len(self.video_paths):
+            process = multiprocessing.Process(target=self.__run_rotation())
+            process.start()
+        else:
+            self.__run_interface(file_path=self.video_paths[len(self.results.keys())-1])
+        if process is not None:
+            process.join()
+
+    def __bind_keys(self):
+        self.main_frm.bind('<Left>', lambda x: self.__rotate(value = 1, img=self._orig_img))
+        self.main_frm.bind('<Right>', lambda x: self.__rotate(value = -1, img=self._orig_img))
+        self.main_frm.bind('<Escape>', lambda x: self.__save())
+
+    def __run_interface(self, file_path: str):
+        self.dif_angle = 0
+        print(file_path)
+        self.video_meta_data = get_video_meta_data(video_path=file_path)
+        self.file_path = file_path
+        _, self.video_name, _ = get_fn_ext(filepath=file_path)
+        self.main_frm = Toplevel()
+        self.main_frm.title(f'ROTATE VIDEO {self.video_name}')
+        self.video_frm = Frame(self.main_frm)
+        self.video_frm.grid(row=0, column=0)
+        self.instruction_frm = Frame(self.main_frm, width=100, height=100)
+        self.instruction_frm.grid(row=0, column=2, sticky=NW)
+        self.key_lbls = Label(self.instruction_frm,
+                                    text='\n\n Navigation: '
+                                         '\n Left arrow = 1° left' 
+                                         '\n Right arrow = 1° right'
+                                         '\n Esc = Save')
+
+        self.key_lbls.grid(sticky=NW)
+        self.cap = cv2.VideoCapture(file_path)
+        _, self.img = self.cap.read()
+        self._orig_img = cv2.cvtColor(self.img, cv2.COLOR_RGB2BGR)
+        self.__insert_img(img=self._orig_img)
+        self.__bind_keys()
+
+    def run(self):
+        self.results = {}
+        for video_path in self.video_paths:
+            self.__run_interface(video_path)
+        self.main_frm.mainloop()
+
+
+
+# r = VideoRotator(input_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Testing/Together_1_downsampled.mp4',
+#              output_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Blah')
+# r.run()
+
+
 # video_concatenator(video_one_path='/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT_2.mp4',
 #                    video_two_path= '/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT.mp4',
 #                    resolution='Video 1',
 #                    horizontal=False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/misc.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/misc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/data_extractors.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/data_extractors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/dbcv.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/dbcv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualization_tools/vtk_embeddings.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualization_tools/vtk_embeddings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/enums.py` & `Simba-UW-tf-dev-1.56.3/simba/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     OUTLIER_CORRECTED = Path('csv/outlier_corrected_movement_location/')
     OUTLIER_CORRECTED_MOVEMENT = Path('csv/outlier_corrected_movement/')
     MACHINE_RESULTS_DIR = Path('csv/machine_results/')
     SKLEARN_RESULTS = Path('frames/output/sklearn_results/')
     CLUSTER_EXAMPLES = Path('frames/output/cluster_examples/')
     CLF_VALIDATION_DIR = Path('frames/output/classifier_validation/')
     CLF_DATA_VALIDATION_DIR = Path('csv/validation/')
+    TEST_PATH = '/Users/simon/Desktop/envs/simba_dev/simba/'
     SINGLE_CLF_VALIDATION = Path('frames/output/validation/')
     INPUT_FRAMES_DIR = Path('frames/input/')
     ICON_ASSETS = Path('assets/icons/')
     DATA_TABLE = Path('frames/output/live_data_table/')
     ROI_FEATURES = Path('frames/output/ROI_features/')
     ROI_ANALYSIS = Path('frames/output/ROI_analysis/')
     ANNOTATED_FRAMES_DIR = Path('frames/output/annotated_frames/')
@@ -115,14 +116,15 @@
     SPLASH_PATH_LINUX = Path('assets/img/splash.PNG')
     SPLASH_PATH_MOVIE = Path('assets/img/splash.mp4')
     BG_IMG_PATH = Path('assets/img/bg_2.png')
     LOGO_ICON_WINDOWS_PATH = Path('assets/icons/SimBA_logo.ico')
     LOGO_ICON_DARWIN_PATH = Path('assets/icons/SimBA_logo.png')
     UNSUPERVISED_MODEL_NAMES = Path('assets/lookups/model_names.parquet')
 
+
 class Formats(Enum):
     MP4_CODEC = 'mp4v'
     AVI_CODEC = 'XVID'
     LABELFRAME_HEADER_FORMAT = ('Helvetica', 12, 'bold')
     LABELFRAME_HEADER_CLICKABLE_FORMAT = ('Helvetica', 12, 'bold', 'underline')
     LABELFRAME_HEADER_CLICKABLE_COLOR = f'#{5:02x}{99:02x}{193:02x}'
     CSV = 'csv'
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
 00001650: 3230 7d2c 207b 3737 302c 2034 3336 7d7d  20}, {770, 436}}
 00001660: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
 00001670: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 00001680: 0000 0000 0000 0000 0000 0000 0000 009a  ................
 00001690: 0000 0005 0075 0074 0069 006c 0073 6473  .....u.t.i.l.sds
 000016a0: 636c 626f 6f6c 0000 0000 0500 7500 7400  clbool......u.t.
 000016b0: 6900 6c00 736c 6731 5363 6f6d 7000 0000  i.l.slg1Scomp...
-000016c0: 0000 0113 9500 0000 0500 7500 7400 6900  ..........u.t.i.
+000016c0: 0000 0113 9c00 0000 0500 7500 7400 6900  ..........u.t.i.
 000016d0: 6c00 736c 7376 4362 6c6f 6200 0002 9762  l.slsvCblob....b
 000016e0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
 000016f0: 090a 0b19 494a 0a4c 5f10 1276 6965 774f  ....IJ.L_..viewO
 00001700: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
 00001710: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00001720: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 00001730: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
@@ -442,15 +442,15 @@
 00001b90: 0147 0148 014a 014b 0154 0156 0157 0159  .G.H.J.K.T.V.W.Y
 00001ba0: 015a 0163 0165 0166 0168 0169 0172 0174  .Z.c.e.f.h.i.r.t
 00001bb0: 0175 0177 0178 0181 0183 0184 0187 0188  .u.w.x..........
 00001bc0: 0191 0192 0193 0194 019d 01a2 01a3 0000  ................
 00001bd0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00001be0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 00001bf0: 0005 0075 0074 0069 006c 0073 6d6f 4444  ...u.t.i.l.smoDD
-00001c00: 626c 6f62 0000 0008 fd0f 980d 4bf2 c441  blob........K..A
+00001c00: 626c 6f62 0000 0008 2102 3a7c 75f3 c441  blob....!.:|u..A
 00001c10: 0000 0005 0075 0074 0069 006c 0073 6d6f  .....u.t.i.l.smo
 00001c20: 6444 626c 6f62 0000 0008 b191 97e3 46f2  dDblob........F.
 00001c30: c441 0000 0005 0075 0074 0069 006c 0073  .A.....u.t.i.l.s
 00001c40: 7068 3153 636f 6d70 0000 0000 0001 6000  ph1Scomp......`.
 00001c50: 0000 0005 0075 0074 0069 006c 0073 7653  .....u.t.i.l.svS
 00001c60: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -509,260 +509,260 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0041 3e1a 0000 000b 005f 005f 0070  ...A>......_._.p
+00002030: 0000 0041 45b4 0000 000b 005f 005f 0070  ...AE......_._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 e5ad 83c6  moDDblob........
-00002060: d8f2 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 4f80 e6bf  moDDblob....O...
+00002060: 86f3 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 5667 2fa4 52f2  dDblob....Vg/.R.
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 004f 1000 0000 0006  comp.....O......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
-000020d0: 626c 6f62 0000 00c7 6270 6c69 7374 3030  blob....bplist00
+000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
 000020e0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 000020f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00002100: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
 00002110: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00002120: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00002130: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00002140: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002150: 7208 0809 0809 5f10 167b 7b30 2c20 3230  r....._..{{0, 20
-00002160: 307d 2c20 7b37 3730 2c20 3433 367d 7d09  0}, {770, 436}}.
-00002170: 0817 2531 3d49 606d 797a 7b7c 7d7e 9700  ..%1=I`myz{|}~..
-00002180: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00002190: 0000 0000 0000 0000 0000 0000 0000 9800  ................
-000021a0: 0000 0600 6100 7300 7300 6500 7400 736c  ....a.s.s.e.t.sl
-000021b0: 6731 5363 6f6d 7000 0000 0000 7dc8 d600  g1Scomp.....}...
-000021c0: 0000 0600 6100 7300 7300 6500 7400 736c  ....a.s.s.e.t.sl
-000021d0: 7376 4362 6c6f 6200 0002 b062 706c 6973  svCblob....bplis
-000021e0: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
-000021f0: 0d18 4849 484a 4b0c 5f10 1276 6965 774f  ..HIHJK._..viewO
-00002200: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
-00002210: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00002220: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00002230: 6174 6541 6c6c 5369 7a65 735f 100f 7363  ateAllSizes_..sc
-00002240: 726f 6c6c 506f 7369 7469 6f6e 5958 7465  rollPositionYXte
-00002250: 7874 5369 7a65 5f10 0f73 6372 6f6c 6c50  xtSize_..scrollP
-00002260: 6f73 6974 696f 6e58 5a73 6f72 7443 6f6c  ositionXZsortCol
-00002270: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
-00002280: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
-00002290: 0109 ab0e 171c 2125 2a2f 3439 3e43 d40f  ......!%*/49>C..
-000022a0: 1011 120c 140c 1657 7669 7369 626c 6555  .......WvisibleU
-000022b0: 7769 6474 6859 6173 6365 6e64 696e 675a  widthYascendingZ
-000022c0: 6964 656e 7469 6669 6572 0911 0127 0954  identifier...'.T
-000022d0: 6e61 6d65 d40f 1011 1218 1918 1b08 1023  name...........#
-000022e0: 0858 7562 6971 7569 7479 d40f 1011 120c  .Xubiquity......
-000022f0: 1e18 2009 10b5 085c 6461 7465 4d6f 6469  .. ....\dateModi
-00002300: 6669 6564 d40f 1011 1218 1e18 2408 085b  fied........$..[
-00002310: 6461 7465 4372 6561 7465 64d4 0f10 1112  dateCreated.....
-00002320: 0c27 1829 0910 6108 5473 697a 65d4 0f10  .'.)..a.Tsize...
-00002330: 1112 0c2c 0c2e 0910 7309 546b 696e 64d4  ...,....s.Tkind.
-00002340: 0f10 1112 1831 0c33 0810 6409 556c 6162  .....1.3..d.Ulab
-00002350: 656c d40f 1011 1218 360c 3808 104b 0957  el......6.8..K.W
-00002360: 7665 7273 696f 6ed4 0f10 1112 183b 0c3d  version......;.=
-00002370: 0811 012c 0958 636f 6d6d 656e 7473 d40f  ...,.Xcomments..
-00002380: 1011 1218 4018 4208 10c8 085e 6461 7465  ....@.B....^date
-00002390: 4c61 7374 4f70 656e 6564 d40f 1011 1218  LastOpened......
-000023a0: 1e18 4608 0859 6461 7465 4164 6465 6408  ..F..YdateAdded.
-000023b0: 2300 0000 0000 0000 0023 4028 0000 0000  #........#@(....
-000023c0: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
-000023d0: 0900 0800 1d00 3200 4400 4c00 6000 7200  ......2.D.L.`.r.
-000023e0: 7b00 8d00 9800 a100 b400 b600 b700 c300  {...............
-000023f0: cc00 d400 da00 e400 ef00 f000 f300 f400  ................
-00002400: f901 0201 0301 0501 0601 0f01 1801 1901  ................
-00002410: 1b01 1c01 2901 3201 3301 3401 4001 4901  ....).2.3.4.@.I.
-00002420: 4a01 4c01 4d01 5201 5b01 5c01 5e01 5f01  J.L.M.R.[.\.^._.
-00002430: 6401 6d01 6e01 7001 7101 7701 8001 8101  d.m.n.p.q.w.....
-00002440: 8301 8401 8c01 9501 9601 9901 9a01 a301  ................
-00002450: ac01 ad01 af01 b001 bf01 c801 c901 ca01  ................
-00002460: d401 d501 de01 e701 ec01 f500 0000 0000  ................
-00002470: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-00002480: 0000 0000 0000 0000 0001 f600 0000 0600  ................
-00002490: 6100 7300 7300 6500 7400 736c 7376 7062  a.s.s.e.t.slsvpb
-000024a0: 6c6f 6200 0002 9562 706c 6973 7430 30da  lob....bplist00.
-000024b0: 0102 0304 0506 0708 090a 0b0c 0d1f 4748  ..............GH
-000024c0: 4749 4a0c 5f10 1276 6965 774f 7074 696f  GIJ._..viewOptio
-000024d0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-000024e0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-000024f0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002500: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00002510: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-00002520: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-00002530: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e58  ionXZsortColumnX
-00002540: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-00002550: 6c61 7469 7665 4461 7465 7310 0109 d90e  lativeDates.....
-00002560: 0f10 1112 1314 1516 1720 2529 2d32 373c  ......... %)-27<
-00002570: 4158 636f 6d6d 656e 7473 5e64 6174 654c  AXcomments^dateL
-00002580: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-00002590: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-000025a0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-000025b0: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-000025c0: 1819 1a1b 1c1d 0c1f 5569 6e64 6578 5577  ........UindexUw
-000025d0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-000025e0: 6973 6962 6c65 1007 1101 2c09 08d4 1819  isible....,.....
-000025f0: 1a1b 2122 1f1f 1008 10c8 0808 d418 191a  ..!"............
-00002600: 1b0b 261f 0c10 b508 09d4 1819 1a1b 2a26  ..&...........*&
-00002610: 1f1f 1002 0808 d418 191a 1b2e 2f1f 0c10  ............/...
-00002620: 0310 6108 09d4 1819 1a1b 3334 0c1f 1005  ..a.......34....
-00002630: 1064 0908 d418 191a 1b38 390c 0c10 0410  .d.......89.....
-00002640: 7309 09d4 1819 1a1b 3d3e 0c1f 1006 104b  s.......=>.....K
-00002650: 0908 d418 191a 1b42 430c 0c10 0011 0127  .......BC......'
-00002660: 0909 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
-00002670: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
-00002680: 0000 0009 0008 001d 0032 0044 004c 0060  .........2.D.L.`
-00002690: 0072 007b 008d 0098 00a1 00b4 00b6 00b7  .r.{............
-000026a0: 00ca 00d3 00e2 00ef 00fb 0100 0106 010b  ................
-000026b0: 0113 0118 0121 0127 012d 0137 013f 0141  .....!.'.-.7.?.A
-000026c0: 0144 0145 0146 014f 0151 0153 0154 0155  .D.E.F.O.Q.S.T.U
-000026d0: 015e 0160 0161 0162 016b 016d 016e 016f  .^.`.a.b.k.m.n.o
-000026e0: 0178 017a 017c 017d 017e 0187 0189 018b  .x.z.|.}.~......
-000026f0: 018c 018d 0196 0198 019a 019b 019c 01a5  ................
-00002700: 01a7 01a9 01aa 01ab 01b4 01b6 01b9 01ba  ................
-00002710: 01bb 01bc 01c5 01ce 01d3 01dc 0000 0000  ................
-00002720: 0000 0201 0000 0000 0000 004c 0000 0000  ...........L....
-00002730: 0000 0000 0000 0000 0000 01dd 0000 0006  ................
-00002740: 0061 0073 0073 0065 0074 0073 6d6f 4444  .a.s.s.e.t.smoDD
-00002750: 626c 6f62 0000 0008 cf95 8ce8 d0e1 c441  blob...........A
-00002760: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-00002770: 6d6f 6444 626c 6f62 0000 0008 cf95 8ce8  modDblob........
-00002780: d0e1 c441 0000 0006 0061 0073 0073 0065  ...A.....a.s.s.e
-00002790: 0074 0073 7068 3153 636f 6d70 0000 0000  .t.sph1Scomp....
-000027a0: 0081 8000 0000 0006 0061 0073 0073 0065  .........a.s.s.e
-000027b0: 0074 0073 7653 726e 6c6f 6e67 0000 0001  .t.svSrnlong....
-000027c0: 0000 0014 0062 0061 0074 0063 0068 005f  .....b.a.t.c.h._
-000027d0: 0070 0072 006f 0063 0065 0073 0073 005f  .p.r.o.c.e.s.s._
-000027e0: 0076 0069 0064 0065 006f 0073 6277 7370  .v.i.d.e.o.sbwsp
-000027f0: 626c 6f62 0000 00ca 6270 6c69 7374 3030  blob....bplist00
-00002800: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00002810: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00002820: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00002830: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00002840: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00002850: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00002860: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002870: 7208 0809 0809 5f10 197b 7b31 3036 322c  r....._..{{1062,
-00002880: 2033 3733 7d2c 207b 3737 302c 2034 3336   373}, {770, 436
-00002890: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-000028a0: 7e9a 0000 0000 0000 0101 0000 0000 0000  ~...............
-000028b0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-000028c0: 009b 0000 0014 0062 0061 0074 0063 0068  .......b.a.t.c.h
-000028d0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-000028e0: 005f 0076 0069 0064 0065 006f 0073 6c67  ._.v.i.d.e.o.slg
-000028f0: 3153 636f 6d70 0000 0000 0001 7de7 0000  1Scomp......}...
-00002900: 0014 0062 0061 0074 0063 0068 005f 0070  ...b.a.t.c.h._.p
-00002910: 0072 006f 0063 0065 0073 0073 005f 0076  .r.o.c.e.s.s._.v
-00002920: 0069 0064 0065 006f 0073 6c73 7643 626c  .i.d.e.o.slsvCbl
-00002930: 6f62 0000 0307 6270 6c69 7374 3030 d801  ob....bplist00..
-00002940: 0203 0405 0607 0809 0a0b 1956 570a 5958  ...........VW.YX
-00002950: 6963 6f6e 5369 7a65 5f10 0f73 686f 7749  iconSize_..showI
-00002960: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00002970: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00002980: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00002990: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-000029a0: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
-000029b0: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-000029c0: 6f6e 2340 3000 0000 0000 0009 ae0c 151d  on#@0...........
-000029d0: 2226 2b30 353a 3f44 484d 51d4 0d0e 0f10  "&+05:?DHMQ.....
-000029e0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-000029f0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00002a00: 7669 7369 626c 6554 6e61 6d65 1103 2a09  visibleTname..*.
-00002a10: 09d4 1617 180d 191a 191c 5776 6973 6962  ..........Wvisib
-00002a20: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
-00002a30: 6e67 0810 2308 5875 6269 7175 6974 79d4  ng..#.Xubiquity.
-00002a40: 0d0e 0f10 1e1f 190a 5c64 6174 654d 6f64  ........\dateMod
-00002a50: 6966 6965 6410 b508 09d4 0d0e 0f10 231f  ified.........#.
-00002a60: 1919 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00002a70: d40d 0e0f 1027 2819 0a54 7369 7a65 1061  .....'(..Tsize.a
-00002a80: 0809 d40d 0e0f 102c 2d0a 0a54 6b69 6e64  .......,-..Tkind
-00002a90: 1073 0909 d40d 0e0f 1031 320a 1955 6c61  .s.......12..Ula
-00002aa0: 6265 6c10 6409 08d4 0d0e 0f10 3637 0a19  bel.d.......67..
-00002ab0: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
-00002ac0: 103b 3c0a 1958 636f 6d6d 656e 7473 1101  .;<..Xcomments..
-00002ad0: 2c09 08d4 0d0e 0f10 4041 1919 5e64 6174  ,.......@A..^dat
-00002ae0: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
-00002af0: 1617 180d 191f 1947 0808 5964 6174 6541  .......G..YdateA
-00002b00: 6464 6564 d40d 1718 1649 4a19 195a 7368  dded.....IJ..Zsh
-00002b10: 6172 654f 776e 6572 10d2 0808 d40d 1718  areOwner........
-00002b20: 164e 4a19 195f 100f 7368 6172 654c 6173  .NJ.._..shareLas
-00002b30: 7445 6469 746f 7208 08d4 0d17 1816 524a  tEditor.......RJ
-00002b40: 1919 5f10 1069 6e76 6974 6174 696f 6e53  .._..invitationS
-00002b50: 7461 7475 7308 0808 2340 2800 0000 0000  tatus...#@(.....
-00002b60: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
-00002b70: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
-00002b80: 9600 a500 ae00 b900 bf00 c900 d100 d600  ................
-00002b90: d900 da00 db00 e400 ec00 f200 fc00 fd00  ................
-00002ba0: ff01 0001 0901 1201 1f01 2101 2201 2301  ..........!.".#.
-00002bb0: 2c01 3801 3901 3a01 4301 4801 4a01 4b01  ,.8.9.:.C.H.J.K.
-00002bc0: 4c01 5501 5a01 5c01 5d01 5e01 6701 6d01  L.U.Z.\.].^.g.m.
-00002bd0: 6f01 7001 7101 7a01 8201 8401 8501 8601  o.p.q.z.........
-00002be0: 8f01 9801 9b01 9c01 9d01 a601 b501 b701  ................
-00002bf0: b801 b901 c201 c301 c401 ce01 d701 e201  ................
-00002c00: e401 e501 e601 ef02 0102 0202 0302 0c02  ................
-00002c10: 1f02 2002 2102 2202 2b02 3002 3100 0000  .. .!.".+.0.1...
-00002c20: 0000 0002 0100 0000 0000 0000 5a00 0000  ............Z...
-00002c30: 0000 0000 0000 0000 0000 0002 3300 0000  ............3...
-00002c40: 1400 6200 6100 7400 6300 6800 5f00 7000  ..b.a.t.c.h._.p.
-00002c50: 7200 6f00 6300 6500 7300 7300 5f00 7600  r.o.c.e.s.s._.v.
-00002c60: 6900 6400 6500 6f00 736c 7376 7062 6c6f  i.d.e.o.slsvpblo
-00002c70: 6200 0002 5e62 706c 6973 7430 30d8 0102  b...^bplist00...
-00002c80: 0304 0506 0708 090a 0b1a 4647 0a35 5869  ..........FG.5Xi
-00002c90: 636f 6e53 697a 655f 100f 7368 6f77 4963  conSize_..showIc
-00002ca0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00002cb0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00002cc0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00002cd0: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-00002ce0: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
-00002cf0: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00002d00: 6e23 4030 0000 0000 0000 09d9 0c0d 0e0f  n#@0............
-00002d10: 1011 1213 1415 1e23 282d 3236 3b40 5863  .......#(-26;@Xc
-00002d20: 6f6d 6d65 6e74 7355 6c61 6265 6c57 7665  ommentsUlabelWve
-00002d30: 7273 696f 6e5b 6461 7465 4372 6561 7465  rsion[dateCreate
-00002d40: 6454 7369 7a65 5c64 6174 654d 6f64 6966  dTsize\dateModif
-00002d50: 6965 6454 6b69 6e64 546e 616d 655e 6461  iedTkindTname^da
-00002d60: 7465 4c61 7374 4f70 656e 6564 d416 1718  teLastOpened....
-00002d70: 191a 1b0a 1d57 7669 7369 626c 6555 7769  .....WvisibleUwi
-00002d80: 6474 6859 6173 6365 6e64 696e 6755 696e  dthYascendingUin
-00002d90: 6465 7808 1101 2c09 1007 d416 1718 191a  dex...,.........
-00002da0: 200a 2208 1064 0910 05d4 1617 1819 1a25   ."..d.........%
-00002db0: 0a27 0810 4b09 1006 d416 1718 191a 2a1a  .'..K.........*.
-00002dc0: 2c08 10b5 0810 02d4 1617 1819 0a2f 1a31  ,............/.1
-00002dd0: 0910 6108 1003 d416 1718 190a 2a1a 3509  ..a.........*.5.
-00002de0: 0810 01d4 1617 1819 0a38 0a3a 0910 7309  .........8.:..s.
-00002df0: 1004 d416 1718 190a 3d0a 3f09 1103 2a09  ........=.?...*.
-00002e00: 1000 d416 1718 191a 421a 4408 10c8 0810  ........B.D.....
-00002e10: 0808 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
-00002e20: 0900 0800 1900 2200 3400 3c00 5000 5900  ......".4.<.P.Y.
-00002e30: 6400 7700 8c00 9500 9600 a900 b200 b800  d.w.............
-00002e40: c000 cc00 d100 de00 e300 e800 f701 0001  ................
-00002e50: 0801 0e01 1801 1e01 1f01 2201 2301 2501  ..........".#.%.
-00002e60: 2e01 2f01 3101 3201 3401 3d01 3e01 4001  ../.1.2.4.=.>.@.
-00002e70: 4101 4301 4c01 4d01 4f01 5001 5201 5b01  A.C.L.M.O.P.R.[.
-00002e80: 5c01 5e01 5f01 6101 6a01 6b01 6c01 6e01  \.^._.a.j.k.l.n.
-00002e90: 7701 7801 7a01 7b01 7d01 8601 8701 8a01  w.x.z.{.}.......
-00002ea0: 8b01 8d01 9601 9701 9901 9a01 9c01 9d01  ................
-00002eb0: a601 ab00 0000 0000 0002 0100 0000 0000  ................
-00002ec0: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
-00002ed0: 0001 ac00 0000 1400 6200 6100 7400 6300  ........b.a.t.c.
-00002ee0: 6800 5f00 7000 7200 6f00 6300 6500 7300  h._.p.r.o.c.e.s.
-00002ef0: 7300 5f00 7600 6900 6400 6500 6f00 736d  s._.v.i.d.e.o.sm
-00002f00: 6f44 4462 6c6f 6200 0000 084b 60d4 fa99  oDDblob....K`...
-00002f10: f1c4 4100 0000 1400 6200 6100 7400 6300  ..A.....b.a.t.c.
-00002f20: 6800 5f00 7000 7200 6f00 6300 6500 7300  h._.p.r.o.c.e.s.
-00002f30: 7300 5f00 7600 6900 6400 6500 6f00 736d  s._.v.i.d.e.o.sm
-00002f40: 6f64 4462 6c6f 6200 0000 084b 60d4 fa99  odDblob....K`...
-00002f50: f1c4 4100 0000 1400 6200 6100 7400 6300  ..A.....b.a.t.c.
-00002f60: 6800 5f00 7000 7200 6f00 6300 6500 7300  h._.p.r.o.c.e.s.
-00002f70: 7300 5f00 7600 6900 6400 6500 6f00 7370  s._.v.i.d.e.o.sp
-00002f80: 6831 5363 6f6d 7000 0000 0000 01f0 0000  h1Scomp.........
+00002150: 7208 0809 0809 5f10 177b 7b33 342c 2039  r....._..{{34, 9
+00002160: 307d 2c20 7b31 3031 352c 2037 3637 7d7d  0}, {1015, 767}}
+00002170: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e98  ...%1=I`myz{|}~.
+00002180: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+00002190: 0000 0000 0000 0000 0000 0000 0000 0099  ................
+000021a0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
+000021b0: 6c67 3153 636f 6d70 0000 0000 007d c8d6  lg1Scomp.....}..
+000021c0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
+000021d0: 6c73 7643 626c 6f62 0000 02b0 6270 6c69  lsvCblob....bpli
+000021e0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+000021f0: 0c0d 1848 4948 4a4b 0c5f 1012 7669 6577  ...HIHJK._..view
+00002200: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00002210: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00002220: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00002230: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00002240: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+00002250: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+00002260: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+00002270: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+00002280: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00002290: 1001 09ab 0e17 1c21 252a 2f34 393e 43d4  .......!%*/49>C.
+000022a0: 0f10 1112 0c14 0c16 5776 6973 6962 6c65  ........Wvisible
+000022b0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+000022c0: 5a69 6465 6e74 6966 6965 7209 1101 2709  Zidentifier...'.
+000022d0: 546e 616d 65d4 0f10 1112 1819 181b 0810  Tname...........
+000022e0: 2308 5875 6269 7175 6974 79d4 0f10 1112  #.Xubiquity.....
+000022f0: 0c1e 1820 0910 b508 5c64 6174 654d 6f64  ... ....\dateMod
+00002300: 6966 6965 64d4 0f10 1112 181e 1824 0808  ified........$..
+00002310: 5b64 6174 6543 7265 6174 6564 d40f 1011  [dateCreated....
+00002320: 120c 2718 2909 1061 0854 7369 7a65 d40f  ..'.)..a.Tsize..
+00002330: 1011 120c 2c0c 2e09 1073 0954 6b69 6e64  ....,....s.Tkind
+00002340: d40f 1011 1218 310c 3308 1064 0955 6c61  ......1.3..d.Ula
+00002350: 6265 6cd4 0f10 1112 1836 0c38 0810 4b09  bel......6.8..K.
+00002360: 5776 6572 7369 6f6e d40f 1011 1218 3b0c  Wversion......;.
+00002370: 3d08 1101 2c09 5863 6f6d 6d65 6e74 73d4  =...,.Xcomments.
+00002380: 0f10 1112 1840 1842 0810 c808 5e64 6174  .....@.B....^dat
+00002390: 654c 6173 744f 7065 6e65 64d4 0f10 1112  eLastOpened.....
+000023a0: 181e 1846 0808 5964 6174 6541 6464 6564  ...F..YdateAdded
+000023b0: 0823 0000 0000 0000 0000 2340 2800 0000  .#........#@(...
+000023c0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
+000023d0: 0009 0008 001d 0032 0044 004c 0060 0072  .......2.D.L.`.r
+000023e0: 007b 008d 0098 00a1 00b4 00b6 00b7 00c3  .{..............
+000023f0: 00cc 00d4 00da 00e4 00ef 00f0 00f3 00f4  ................
+00002400: 00f9 0102 0103 0105 0106 010f 0118 0119  ................
+00002410: 011b 011c 0129 0132 0133 0134 0140 0149  .....).2.3.4.@.I
+00002420: 014a 014c 014d 0152 015b 015c 015e 015f  .J.L.M.R.[.\.^._
+00002430: 0164 016d 016e 0170 0171 0177 0180 0181  .d.m.n.p.q.w....
+00002440: 0183 0184 018c 0195 0196 0199 019a 01a3  ................
+00002450: 01ac 01ad 01af 01b0 01bf 01c8 01c9 01ca  ................
+00002460: 01d4 01d5 01de 01e7 01ec 01f5 0000 0000  ................
+00002470: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
+00002480: 0000 0000 0000 0000 0000 01f6 0000 0006  ................
+00002490: 0061 0073 0073 0065 0074 0073 6c73 7670  .a.s.s.e.t.slsvp
+000024a0: 626c 6f62 0000 0295 6270 6c69 7374 3030  blob....bplist00
+000024b0: da01 0203 0405 0607 0809 0a0b 0c0d 1f47  ...............G
+000024c0: 4847 494a 0c5f 1012 7669 6577 4f70 7469  HGIJ._..viewOpti
+000024d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+000024e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+000024f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00002500: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+00002510: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+00002520: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+00002530: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+00002540: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
+00002550: 656c 6174 6976 6544 6174 6573 1001 09d9  elativeDates....
+00002560: 0e0f 1011 1213 1415 1617 2025 292d 3237  .......... %)-27
+00002570: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
+00002580: 4c61 7374 4f70 656e 6564 5c64 6174 654d  LastOpened\dateM
+00002590: 6f64 6966 6965 645b 6461 7465 4372 6561  odified[dateCrea
+000025a0: 7465 6454 7369 7a65 556c 6162 656c 546b  tedTsizeUlabelTk
+000025b0: 696e 6457 7665 7273 696f 6e54 6e61 6d65  indWversionTname
+000025c0: d418 191a 1b1c 1d0c 1f55 696e 6465 7855  .........UindexU
+000025d0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+000025e0: 7669 7369 626c 6510 0711 012c 0908 d418  visible....,....
+000025f0: 191a 1b21 221f 1f10 0810 c808 08d4 1819  ...!"...........
+00002600: 1a1b 0b26 1f0c 10b5 0809 d418 191a 1b2a  ...&...........*
+00002610: 261f 1f10 0208 08d4 1819 1a1b 2e2f 1f0c  &............/..
+00002620: 1003 1061 0809 d418 191a 1b33 340c 1f10  ...a.......34...
+00002630: 0510 6409 08d4 1819 1a1b 3839 0c0c 1004  ..d.......89....
+00002640: 1073 0909 d418 191a 1b3d 3e0c 1f10 0610  .s.......=>.....
+00002650: 4b09 08d4 1819 1a1b 4243 0c0c 1000 1101  K.......BC......
+00002660: 2709 0908 2300 0000 0000 0000 0023 4028  '...#........#@(
+00002670: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+00002680: 0000 0000 0900 0800 1d00 3200 4400 4c00  ..........2.D.L.
+00002690: 6000 7200 7b00 8d00 9800 a100 b400 b600  `.r.{...........
+000026a0: b700 ca00 d300 e200 ef00 fb01 0001 0601  ................
+000026b0: 0b01 1301 1801 2101 2701 2d01 3701 3f01  ......!.'.-.7.?.
+000026c0: 4101 4401 4501 4601 4f01 5101 5301 5401  A.D.E.F.O.Q.S.T.
+000026d0: 5501 5e01 6001 6101 6201 6b01 6d01 6e01  U.^.`.a.b.k.m.n.
+000026e0: 6f01 7801 7a01 7c01 7d01 7e01 8701 8901  o.x.z.|.}.~.....
+000026f0: 8b01 8c01 8d01 9601 9801 9a01 9b01 9c01  ................
+00002700: a501 a701 a901 aa01 ab01 b401 b601 b901  ................
+00002710: ba01 bb01 bc01 c501 ce01 d301 dc00 0000  ................
+00002720: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
+00002730: 0000 0000 0000 0000 0000 0001 dd00 0000  ................
+00002740: 0600 6100 7300 7300 6500 7400 736d 6f44  ..a.s.s.e.t.smoD
+00002750: 4462 6c6f 6200 0000 08cf 958c e8d0 e1c4  Dblob...........
+00002760: 4100 0000 0600 6100 7300 7300 6500 7400  A.....a.s.s.e.t.
+00002770: 736d 6f64 4462 6c6f 6200 0000 08cf 958c  smodDblob.......
+00002780: e8d0 e1c4 4100 0000 0600 6100 7300 7300  ....A.....a.s.s.
+00002790: 6500 7400 7370 6831 5363 6f6d 7000 0000  e.t.sph1Scomp...
+000027a0: 0000 8180 0000 0000 0600 6100 7300 7300  ..........a.s.s.
+000027b0: 6500 7400 7376 5372 6e6c 6f6e 6700 0000  e.t.svSrnlong...
+000027c0: 0100 0000 1400 6200 6100 7400 6300 6800  ......b.a.t.c.h.
+000027d0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+000027e0: 5f00 7600 6900 6400 6500 6f00 7362 7773  _.v.i.d.e.o.sbws
+000027f0: 7062 6c6f 6200 0000 ca62 706c 6973 7430  pblob....bplist0
+00002800: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
+00002810: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00002820: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
+00002830: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
+00002840: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
+00002850: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
+00002860: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
+00002870: 6172 0808 0908 095f 1019 7b7b 3130 3632  ar....._..{{1062
+00002880: 2c20 3337 337d 2c20 7b37 3730 2c20 3433  , 373}, {770, 43
+00002890: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
+000028a0: 7d7e 9a00 0000 0000 0001 0100 0000 0000  }~..............
+000028b0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+000028c0: 0000 9b00 0000 1400 6200 6100 7400 6300  ........b.a.t.c.
+000028d0: 6800 5f00 7000 7200 6f00 6300 6500 7300  h._.p.r.o.c.e.s.
+000028e0: 7300 5f00 7600 6900 6400 6500 6f00 736c  s._.v.i.d.e.o.sl
+000028f0: 6731 5363 6f6d 7000 0000 0000 017d e700  g1Scomp......}..
+00002900: 0000 1400 6200 6100 7400 6300 6800 5f00  ....b.a.t.c.h._.
+00002910: 7000 7200 6f00 6300 6500 7300 7300 5f00  p.r.o.c.e.s.s._.
+00002920: 7600 6900 6400 6500 6f00 736c 7376 4362  v.i.d.e.o.slsvCb
+00002930: 6c6f 6200 0003 0762 706c 6973 7430 30d8  lob....bplist00.
+00002940: 0102 0304 0506 0708 090a 0b19 5657 0a59  ............VW.Y
+00002950: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+00002960: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00002970: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00002980: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00002990: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+000029a0: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+000029b0: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+000029c0: 696f 6e23 4030 0000 0000 0000 09ae 0c15  ion#@0..........
+000029d0: 1d22 262b 3035 3a3f 4448 4d51 d40d 0e0f  ."&+05:?DHMQ....
+000029e0: 1011 120a 0a5a 6964 656e 7469 6669 6572  .....Zidentifier
+000029f0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00002a00: 5776 6973 6962 6c65 546e 616d 6511 032a  WvisibleTname..*
+00002a10: 0909 d416 1718 0d19 1a19 1c57 7669 7369  ...........Wvisi
+00002a20: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+00002a30: 696e 6708 1023 0858 7562 6971 7569 7479  ing..#.Xubiquity
+00002a40: d40d 0e0f 101e 1f19 0a5c 6461 7465 4d6f  .........\dateMo
+00002a50: 6469 6669 6564 10b5 0809 d40d 0e0f 1023  dified.........#
+00002a60: 1f19 195b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
+00002a70: 08d4 0d0e 0f10 2728 190a 5473 697a 6510  ......'(..Tsize.
+00002a80: 6108 09d4 0d0e 0f10 2c2d 0a0a 546b 696e  a.......,-..Tkin
+00002a90: 6410 7309 09d4 0d0e 0f10 3132 0a19 556c  d.s.......12..Ul
+00002aa0: 6162 656c 1064 0908 d40d 0e0f 1036 370a  abel.d.......67.
+00002ab0: 1957 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
+00002ac0: 0f10 3b3c 0a19 5863 6f6d 6d65 6e74 7311  ..;<..Xcomments.
+00002ad0: 012c 0908 d40d 0e0f 1040 4119 195e 6461  .,.......@A..^da
+00002ae0: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
+00002af0: d416 1718 0d19 1f19 4708 0859 6461 7465  ........G..Ydate
+00002b00: 4164 6465 64d4 0d17 1816 494a 1919 5a73  Added.....IJ..Zs
+00002b10: 6861 7265 4f77 6e65 7210 d208 08d4 0d17  hareOwner.......
+00002b20: 1816 4e4a 1919 5f10 0f73 6861 7265 4c61  ..NJ.._..shareLa
+00002b30: 7374 4564 6974 6f72 0808 d40d 1718 1652  stEditor.......R
+00002b40: 4a19 195f 1010 696e 7669 7461 7469 6f6e  J.._..invitation
+00002b50: 5374 6174 7573 0808 0823 4028 0000 0000  Status...#@(....
+00002b60: 0000 546e 616d 6509 1001 0008 0019 0022  ..Tname........"
+00002b70: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
+00002b80: 0096 00a5 00ae 00b9 00bf 00c9 00d1 00d6  ................
+00002b90: 00d9 00da 00db 00e4 00ec 00f2 00fc 00fd  ................
+00002ba0: 00ff 0100 0109 0112 011f 0121 0122 0123  ...........!.".#
+00002bb0: 012c 0138 0139 013a 0143 0148 014a 014b  .,.8.9.:.C.H.J.K
+00002bc0: 014c 0155 015a 015c 015d 015e 0167 016d  .L.U.Z.\.].^.g.m
+00002bd0: 016f 0170 0171 017a 0182 0184 0185 0186  .o.p.q.z........
+00002be0: 018f 0198 019b 019c 019d 01a6 01b5 01b7  ................
+00002bf0: 01b8 01b9 01c2 01c3 01c4 01ce 01d7 01e2  ................
+00002c00: 01e4 01e5 01e6 01ef 0201 0202 0203 020c  ................
+00002c10: 021f 0220 0221 0222 022b 0230 0231 0000  ... .!.".+.0.1..
+00002c20: 0000 0000 0201 0000 0000 0000 005a 0000  .............Z..
+00002c30: 0000 0000 0000 0000 0000 0000 0233 0000  .............3..
+00002c40: 0014 0062 0061 0074 0063 0068 005f 0070  ...b.a.t.c.h._.p
+00002c50: 0072 006f 0063 0065 0073 0073 005f 0076  .r.o.c.e.s.s._.v
+00002c60: 0069 0064 0065 006f 0073 6c73 7670 626c  .i.d.e.o.slsvpbl
+00002c70: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
+00002c80: 0203 0405 0607 0809 0a0b 1a46 470a 3558  ...........FG.5X
+00002c90: 6963 6f6e 5369 7a65 5f10 0f73 686f 7749  iconSize_..showI
+00002ca0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00002cb0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00002cc0: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+00002cd0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
+00002ce0: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
+00002cf0: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00002d00: 6f6e 2340 3000 0000 0000 0009 d90c 0d0e  on#@0...........
+00002d10: 0f10 1112 1314 151e 2328 2d32 363b 4058  ........#(-26;@X
+00002d20: 636f 6d6d 656e 7473 556c 6162 656c 5776  commentsUlabelWv
+00002d30: 6572 7369 6f6e 5b64 6174 6543 7265 6174  ersion[dateCreat
+00002d40: 6564 5473 697a 655c 6461 7465 4d6f 6469  edTsize\dateModi
+00002d50: 6669 6564 546b 696e 6454 6e61 6d65 5e64  fiedTkindTname^d
+00002d60: 6174 654c 6173 744f 7065 6e65 64d4 1617  ateLastOpened...
+00002d70: 1819 1a1b 0a1d 5776 6973 6962 6c65 5577  ......WvisibleUw
+00002d80: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
+00002d90: 6e64 6578 0811 012c 0910 07d4 1617 1819  ndex...,........
+00002da0: 1a20 0a22 0810 6409 1005 d416 1718 191a  . ."..d.........
+00002db0: 250a 2708 104b 0910 06d4 1617 1819 1a2a  %.'..K.........*
+00002dc0: 1a2c 0810 b508 1002 d416 1718 190a 2f1a  .,............/.
+00002dd0: 3109 1061 0810 03d4 1617 1819 0a2a 1a35  1..a.........*.5
+00002de0: 0908 1001 d416 1718 190a 380a 3a09 1073  ..........8.:..s
+00002df0: 0910 04d4 1617 1819 0a3d 0a3f 0911 032a  .........=.?...*
+00002e00: 0910 00d4 1617 1819 1a42 1a44 0810 c808  .........B.D....
+00002e10: 1008 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00002e20: 6509 0008 0019 0022 0034 003c 0050 0059  e......".4.<.P.Y
+00002e30: 0064 0077 008c 0095 0096 00a9 00b2 00b8  .d.w............
+00002e40: 00c0 00cc 00d1 00de 00e3 00e8 00f7 0100  ................
+00002e50: 0108 010e 0118 011e 011f 0122 0123 0125  ...........".#.%
+00002e60: 012e 012f 0131 0132 0134 013d 013e 0140  .../.1.2.4.=.>.@
+00002e70: 0141 0143 014c 014d 014f 0150 0152 015b  .A.C.L.M.O.P.R.[
+00002e80: 015c 015e 015f 0161 016a 016b 016c 016e  .\.^._.a.j.k.l.n
+00002e90: 0177 0178 017a 017b 017d 0186 0187 018a  .w.x.z.{.}......
+00002ea0: 018b 018d 0196 0197 0199 019a 019c 019d  ................
+00002eb0: 01a6 01ab 0000 0000 0000 0201 0000 0000  ................
+00002ec0: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
+00002ed0: 0000 01ac 0000 0014 0062 0061 0074 0063  .........b.a.t.c
+00002ee0: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
+00002ef0: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
+00002f00: 6d6f 4444 626c 6f62 0000 0008 4b60 d4fa  moDDblob....K`..
+00002f10: 99f1 c441 0000 0014 0062 0061 0074 0063  ...A.....b.a.t.c
+00002f20: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
+00002f30: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
+00002f40: 6d6f 6444 626c 6f62 0000 0008 4b60 d4fa  modDblob....K`..
+00002f50: 99f1 c441 0000 0014 0062 0061 0074 0063  ...A.....b.a.t.c
+00002f60: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
+00002f70: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
+00002f80: 7068 3153 636f 6d70 0000 0000 0001 f000  ph1Scomp........
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -965,15 +965,15 @@
 00003c40: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 00003c50: 9b00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00003c60: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00003c70: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00003c80: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00003c90: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00003ca0: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00003cb0: 6d70 0000 0000 0011 c675 0000 0012 0066  mp.......u.....f
+00003cb0: 6d70 0000 0000 0011 dfa2 0000 0012 0066  mp.............f
 00003cc0: 0065 0061 0074 0075 0072 0065 005f 0065  .e.a.t.u.r.e._.e
 00003cd0: 0078 0074 0072 0061 0063 0074 006f 0072  .x.t.r.a.c.t.o.r
 00003ce0: 0073 6c73 7643 626c 6f62 0000 02b8 6270  .slsvCblob....bp
 00003cf0: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
 00003d00: 0a0b 0c0d 1a48 4948 4a4b 0c5f 1012 7669  .....HIHJK._..vi
 00003d10: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
 00003d20: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
@@ -1029,15 +1029,15 @@
 00004040: ec48 4ecf 38f2 c441 0000 0012 0066 0065  .HN.8..A.....f.e
 00004050: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00004060: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
 00004070: 6d6f 6444 626c 6f62 0000 0008 ec48 4ecf  modDblob.....HN.
 00004080: 38f2 c441 0000 0012 0066 0065 0061 0074  8..A.....f.e.a.t
 00004090: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 000040a0: 0061 0063 0074 006f 0072 0073 7068 3153  .a.c.t.o.r.sph1S
-000040b0: 636f 6d70 0000 0000 0013 f000 0000 0012  comp............
+000040b0: 636f 6d70 0000 0000 0014 2000 0000 0012  comp...... .....
 000040c0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 000040d0: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 000040e0: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
 000040f0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00004100: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
 00004110: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
 00004120: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,15 +433,15 @@
 
             print('Calculating pose probability scores...')
             all_p_columns = self.mouse_2_p_headers + self.mouse_1_p_headers
             self.out_data['Sum_probabilities'] = self.out_data[all_p_columns].sum(axis=1)
             self.out_data['Sum_probabilities_deviation'] = (self.out_data['Sum_probabilities'].mean() - self.out_data['Sum_probabilities'])
             self.out_data['Sum_probabilities_deviation_percentile_rank'] = self.out_data['Sum_probabilities_deviation'].rank(pct=True)
             self.out_data['Sum_probabilities_percentile_rank'] = self.out_data['Sum_probabilities_deviation_percentile_rank'].rank(pct=True)
-            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(all_p_columns).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5', 'Low_prob_detections_0.75'])
+            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(all_p_columns).values, ranges=np.array([[0.0, 0.1], [0.0, 0.5], [0.0, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5', 'Low_prob_detections_0.75'])
             self.out_data = pd.concat([self.out_data, results], axis=1)
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time() - file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s)...'.format(self.video_name,
                                                                                              str(file_cnt + 1),
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 4% similar despite different names*

```diff
@@ -241,15 +241,15 @@
                 self.out_data[col_name] = tortuosities_results['Animal_1']
 
             print('Calculating pose probability scores...')
             self.out_data['Sum_probabilities'] = (self.out_data['Ear_left_p'] + self.out_data['Ear_right_p'] + self.out_data['Nose_p'] + self.out_data['Tail_base_p'])
             self.out_data['Sum_probabilities_deviation'] = (self.out_data['Sum_probabilities'].mean() - self.out_data['Sum_probabilities'])
             self.out_data['Sum_probabilities_deviation_percentile_rank'] = self.out_data['Sum_probabilities_deviation'].rank(pct=True)
             self.out_data['Sum_probabilities_percentile_rank'] = self.out_data['Sum_probabilities_deviation_percentile_rank'].rank(pct=True)
-            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(self.mouse_p_headers).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
+            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(self.mouse_p_headers).values, ranges=np.array([[0.0, 0.1], [0.0, 0.5], [0.0, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
             self.out_data = pd.concat([self.out_data, results], axis=1)
 
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
 
             print('Feature extraction complete for {} ({}/{})...'.format(self.video_name, str(file_cnt + 1),str(len(self.files_found))))
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
 
             print('Calculating pose probability scores...')
             all_p_columns = self.mouse_2_p_headers + self.mouse_1_p_headers
             self.out_data['Sum_probabilities'] = self.out_data[all_p_columns].sum(axis=1)
             self.out_data['Sum_probabilities_deviation'] = (self.out_data['Sum_probabilities'].mean() - self.out_data['Sum_probabilities'])
             self.out_data['Sum_probabilities_deviation_percentile_rank'] = self.out_data['Sum_probabilities_deviation'].rank(pct=True)
             self.out_data['Sum_probabilities_percentile_rank'] = self.out_data['Sum_probabilities_deviation_percentile_rank'].rank(pct=True)
-            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(all_p_columns).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5', 'Low_prob_detections_0.75'])
+            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(all_p_columns).values, ranges=np.array([[0.0, 0.1], [0.0, 0.5], [0.0, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5', 'Low_prob_detections_0.75'])
             self.out_data = pd.concat([self.out_data, results], axis=1)
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time()-file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s))...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found)), str(file_time)))
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/perimeter_jit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ### https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179
 
 import numpy as np
 from numba import njit, prange
 from numba.np.extensions import cross2d
-from numba import types
 
 @njit('(float64[:,:], int64[:], int64, int64)')
 def process(S, P, a, b):
     signed_dist = cross2d(S[P] - S[a], S[b] - S[a])
     K = np.array([i for s, i in zip(signed_dist, P) if s > 0 and i != a and i != b], dtype=np.int64)
     if len(K) == 0:
         return [a, b]
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/extract_features_9bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 import numpy as np
 from scipy.spatial import ConvexHull
 import scipy
 from simba.feature_extractors.unit_tests import check_minimum_roll_windows, read_video_info_csv, read_video_info
 from configparser import ConfigParser, NoOptionError, NoSectionError
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.drop_bp_cords import get_workflow_file_format
+
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 
 def extract_features_wotarget_9(inifile):
     config = ConfigParser()
     config.read(str(inifile))
     csv_dir = config.get('General settings', 'csv_path')
@@ -30,15 +30,15 @@
         ang = math.degrees(
             math.atan2(cy - by, cx - bx) - math.atan2(ay - by, ax - bx))
         return ang + 360 if ang < 0 else ang
 
     roll_windows_values = [2, 5, 6, 7.5, 15]
     roll_windows_values = check_minimum_roll_windows(roll_windows_values, vidinfDf['fps'].min())
 
-    wfileType = get_workflow_file_format(config)
+    wfileType = 'csv'
 
     filesFound = glob.glob(csv_dir_in + '/*.' + wfileType)
     print('Extracting features from ' + str(len(filesFound)) + ' file(s)...')
 
     ########### CREATE PD FOR RAW DATA AND PD FOR MOVEMENT BETWEEN FRAMES ###########
     for file_path in filesFound:
         M1_hull_large_euclidean_list = []
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             self.data_df['Mean_{}_{}'.format(i[1], i[0])] = self.data_df[i[1]].rolling(int(i[0]), min_periods=1).mean()
             self.data_df['Sum_{}_{}'.format(i[1], i[0])] = self.data_df[i[1]].rolling(int(i[0]), min_periods=1).sum()
 
     def __pose_probability_filters(self):
         p_df = self.data_df.filter(self.pcols, axis=1)
         self.data_df['Sum_probabilities'] = p_df.sum(axis=1)
         self.data_df['Mean_probabilities'] = p_df.mean(axis=1)
-        results = pd.DataFrame(self.count_values_in_range(data=self.data_df.filter(self.pcols).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
+        results = pd.DataFrame(self.count_values_in_range(data=self.data_df.filter(self.pcols).values, ranges=np.array([[0.0, 0.1], [0.0, 0.5], [0.0, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
         self.data_df = pd.concat([self.data_df, results], axis=1)
 
     def extract_features(self):
         """
         Method to compute and save features to disk. Results are saved in the `project_folder/csv/features_extracted`
         directory of the SimBA project.
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
 
             print('Calculating pose probability scores...')
             all_p_columns = self.mouse_2_p_headers + self.mouse_1_p_headers
             self.out_data['Sum_probabilities'] = self.out_data[all_p_columns].sum(axis=1)
             self.out_data['Sum_probabilities_deviation'] = (self.out_data['Sum_probabilities'].mean() - self.out_data['Sum_probabilities'])
             self.out_data['Sum_probabilities_deviation_percentile_rank'] = self.out_data['Sum_probabilities_deviation'].rank(pct=True)
             self.out_data['Sum_probabilities_percentile_rank'] = self.out_data['Sum_probabilities_deviation_percentile_rank'].rank(pct=True)
-            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(all_p_columns).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5', 'Low_prob_detections_0.75'])
+            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(all_p_columns).values, ranges=np.array([[0.0, 0.1], [0.0, 0.5], [0.0, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5', 'Low_prob_detections_0.75'])
             self.out_data = pd.concat([self.out_data, results], axis=1)
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time()-file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s)...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found)), str(file_time)))
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                 self.out_data[col_name] = tortuosities_results['Animal_1']
 
             print('Calculating pose probability scores...')
             self.out_data['Sum_probabilities'] = (self.out_data['Ear_left_p'] + self.out_data['Ear_right_p'] + self.out_data['Nose_p'] + self.out_data['Tail_base_p'])
             self.out_data['Sum_probabilities_deviation'] = (self.out_data['Sum_probabilities'].mean() - self.out_data['Sum_probabilities'])
             self.out_data['Sum_probabilities_deviation_percentile_rank'] = self.out_data['Sum_probabilities_deviation'].rank(pct=True)
             self.out_data['Sum_probabilities_percentile_rank'] = self.out_data['Sum_probabilities_deviation_percentile_rank'].rank(pct=True)
-            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(self.mouse_p_headers).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
+            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(self.mouse_p_headers).values, ranges=np.array([[0.0, 0.1], [0.0, 0.5], [0.0, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
             self.out_data = pd.concat([self.out_data, results], axis=1)
 
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time() - file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s)...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found)), str(file_time)))
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 self.out_data[col_name] = tortuosities_results['Animal_1']
 
             print('Calculating pose probability scores...')
             self.out_data['Sum_probabilities'] = (self.out_data['Ear_left_p'] + self.out_data['Ear_right_p'] + self.out_data['Nose_p'] + self.out_data['Tail_base_p'])
             self.out_data['Sum_probabilities_deviation'] = (self.out_data['Sum_probabilities'].mean() - self.out_data['Sum_probabilities'])
             self.out_data['Sum_probabilities_deviation_percentile_rank'] = self.out_data['Sum_probabilities_deviation'].rank(pct=True)
             self.out_data['Sum_probabilities_percentile_rank'] = self.out_data['Sum_probabilities_deviation_percentile_rank'].rank(pct=True)
-            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(self.mouse_p_headers).values, ranges=np.array([[0.0, 0.1], [0.000000000, 0.5], [0.000000000, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
+            results = pd.DataFrame(self.count_values_in_range(data=self.out_data.filter(self.mouse_p_headers).values, ranges=np.array([[0.0, 0.1], [0.0, 0.5], [0.0, 0.75]])), columns=['Low_prob_detections_0.1', 'Low_prob_detections_0.5','Low_prob_detections_0.75'])
             self.out_data = pd.concat([self.out_data, results], axis=1)
 
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
 
             print('Feature extraction complete for {} ({}/{})...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found))))
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.56.3/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/requirements.txt` & `Simba-UW-tf-dev-1.56.3/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/severity_processor.py` & `Simba-UW-tf-dev-1.56.3/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.56.3/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.56.3/simba/mixins/pop_up_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,19 @@
 import simba
 
 
 class PopUpMixin(object):
     def __init__(self,
                  title: str,
                  config_path: str or None=None,
+                 size: tuple=(400,400),
                  hyperlink: str or None=None):
 
         self.main_frm = Toplevel()
-        self.main_frm.minsize(400, 400)
+        self.main_frm.minsize(size[0], size[1])
         self.main_frm.wm_title(title)
 
         # self.menu_icons = get_icons_paths()
         # for k in self.menu_icons.keys():
         #     self.menu_icons[k]['img'] = ImageTk.PhotoImage(image=PIL.Image.open(os.path.join(os.path.dirname("__file__"), self.menu_icons[k]['icon_path'])))
         # self.main_frm.overrideredirect(True)
         # title_bar = Frame(self.main_frm, bg=Formats.HEADER_BG_CLR_FORMAT.value, relief='raised', bd=1)
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.56.3/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.56.3/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.56.3/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.56.3/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.56.3/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.56.3/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.56.3/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/video_info_table.py` & `Simba-UW-tf-dev-1.56.3/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.56.3/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.56.3/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/utils/errors.py` & `Simba-UW-tf-dev-1.56.3/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/utils/printing.py` & `Simba-UW-tf-dev-1.56.3/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.56.3/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.56.3/simba/train_model_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 from sklearn.metrics import precision_recall_curve
 from sklearn.ensemble import RandomForestClassifier
 from copy import deepcopy
 from sklearn.tree import export_graphviz
 from subprocess import call
 from yellowbrick.classifier import ClassificationReport
 import shap
-from simba.drop_bp_cords import GenerateMetaDataFileHeaders
 from tabulate import tabulate
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
 from simba.read_config_unit_tests import (check_int, check_str, check_if_dir_exists,
                                           check_float,
                                           read_config_entry)
 from concurrent.futures import ProcessPoolExecutor
+from concurrent.futures.process import BrokenProcessPool
 from itertools import repeat
 from simba.misc_tools import (create_single_color_lst,
                               SimbaTimer,
                               detect_bouts,
                               find_core_cnt)
 from simba.utils.errors import (ColumnNotFoundError,
                                 FaultyTrainingSetError,
@@ -38,14 +38,15 @@
                                 CorruptedFileError,
                                 FeatureNumberMismatchError,
                                 ClassifierInferenceError,
                                 CountError)
 from simba.utils.warnings import (NotEnoughDataWarning,
                                   NoModuleWarning,
                                   MissingUserInputWarning)
+from simba.utils.lookups import get_meta_data_file_headers
 import configparser
 import platform
 from sklearn.utils import parallel_backend
 import pickle
 from dtreeviz.trees import tree, dtreeviz
 import matplotlib.pyplot as plt
 from simba.enums import ReadConfig, Dtypes, MetaKeys
@@ -751,15 +752,15 @@
 
     Returns
     -------
     None
     """
     print('Saving model meta data file...')
     save_path = os.path.join(save_dir, clf_name + '_meta.csv')
-    out_df = pd.DataFrame(columns=GenerateMetaDataFileHeaders())
+    out_df = pd.DataFrame(columns=get_meta_data_file_headers())
     out_df.loc[len(out_df)] = meta_data_lst
     out_df.to_csv(save_path)
 
 
 def create_meta_data_csv_training_multiple_models(meta_data,
                                                   clf_name,
                                                   save_dir,
@@ -1069,20 +1070,23 @@
     pd.DataFrame
 
     """
     if platform.system() == "Darwin":
         multiprocessing.set_start_method('spawn', force=True)
     cpu_cnt, _ = find_core_cnt()
     df_lst = []
-    with ProcessPoolExecutor(int(np.ceil(cpu_cnt/2))) as pool:
-        for res in pool.map(_read_data_file_helper, file_paths, repeat(file_type), repeat(classifier_names)):
-            df_lst.append(res)
-    df_concat = pd.concat(df_lst, axis=0)
-    if 'scorer' in df_concat.columns:
-        df_concat = df_concat.set_index('scorer')
-    if len(df_concat) == 0:
-        raise ValueError('ANNOTATION ERROR: SimBA found 0 observations (frames) in the project_folder/csv/targets_inserted directory')
-    df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')]
-
-    return df_concat.reset_index(drop=True)
-
-
+    try:
+        with ProcessPoolExecutor(int(np.ceil(cpu_cnt/2))) as pool:
+            for res in pool.map(_read_data_file_helper, file_paths, repeat(file_type), repeat(classifier_names)):
+                df_lst.append(res)
+        df_concat = pd.concat(df_lst, axis=0)
+        if 'scorer' in df_concat.columns:
+            df_concat = df_concat.set_index('scorer')
+        if len(df_concat) == 0:
+            raise ValueError('ANNOTATION ERROR: SimBA found 0 observations (frames) in the project_folder/csv/targets_inserted directory')
+        df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')]
+        return df_concat.reset_index(drop=True)
+
+    except BrokenProcessPool:
+        return read_all_files_in_folder(file_paths=file_paths,
+                                        file_type=file_type,
+                                        classifier_names=classifier_names)
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.56.3/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.56.3/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/movement_processor.py` & `Simba-UW-tf-dev-1.56.3/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pybursts.py` & `Simba-UW-tf-dev-1.56.3/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.56.3/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.56.3/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.56.3/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.56.3/simba/tkinter_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,10 +257,23 @@
     label_image.grid(row=0, column=1)
     return LabelFrame(parent, labelwidget=frm)
 
 def callback(url):
     webbrowser.open_new(url)
 
 
+def create_scalebar(parent: Frame,
+                    name: str,
+                    min: int,
+                    max: int,
+                    cmd: object or None=None):
+
+    scale = Scale(parent, from_=min, to=max, orient=HORIZONTAL, length=200, label=name, command=cmd)
+    scale.set(0)
+    return scale
+
+
+
+
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/setting_menu.py` & `Simba-UW-tf-dev-1.56.3/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.56.3/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/run_inference.py` & `Simba-UW-tf-dev-1.56.3/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.56.3/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.56.3/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/dash_app.py` & `Simba-UW-tf-dev-1.56.3/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.56.3/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.56.3/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.56.3/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/misc_tools.py` & `Simba-UW-tf-dev-1.56.3/simba/misc_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 __author__ = "Simon Nilsson"
 
 import configparser
-from simba.drop_bp_cords import (get_fn_ext,
-                                 get_workflow_file_format)
+from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import (read_df,
                           save_df)
 import cv2
 from pylab import *
 import os, glob
 from copy import deepcopy
 import pandas as pd
@@ -21,15 +20,16 @@
 from numba import jit, prange
 from configparser import (ConfigParser,
                           MissingSectionHeaderError)
 import multiprocessing
 from simba.read_config_unit_tests import (check_file_exist_and_readable,
                                           read_config_entry,
                                           read_config_file,
-                                          check_if_filepath_list_is_empty)
+                                          check_if_filepath_list_is_empty,
+                                          read_project_path_and_file_type)
 from simba.enums import ReadConfig, Dtypes, Paths
 from simba.extract_frames_fast import video_to_frames
 from simba.utils.errors import (InvalidVideoFileError,
                                 NotDirectoryError,
                                 NoFilesFoundError,
                                 DirectoryExistError,
                                 InvalidFileTypeError,
@@ -64,34 +64,33 @@
     vdata: dict
         Python dictionary holding video meta data
 
     Notes
     ----------
 
     Examples
-    >>>  get_video_meta_data('tests/test_data/mouse_open_field/project_folder/videos/SI_DAY3_308_CD1_PRESENT.mp4')
-    {'video_name': 'SI_DAY3_308_CD1_PRESENT', 'fps': 15, 'width': 1500, 'height': 1350, 'frame_count': 900, 'resolution_str': '1500 x 1350'}
+    >>> get_video_meta_data('/Users/simon/Desktop/envs/simba_dev/tests/test_data/video_tests/Together_1.avi')
+    {'video_name': 'Together_1', 'fps': 30, 'width': 400, 'height': 600, 'frame_count': 300, 'resolution_str': '400 x 600', 'video_length_s': 10}
 
     """
 
     video_data = {}
     cap = cv2.VideoCapture(video_path)
     _, video_data['video_name'], _ = get_fn_ext(video_path)
     video_data['fps'] = int(cap.get(cv2.CAP_PROP_FPS))
     video_data['width'] = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
     video_data['height'] = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
     video_data['frame_count'] = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     for k, v in video_data.items():
         if v == 0:
-            raise InvalidVideoFileError(msg='SIMBA WARNING: Video {} has {} of {}.'.format(video_data['video_name'], k, str(v)))
-    video_data['resolution_str'] = str('{} x {}'.format(video_data['width'], video_data['height']))
+            raise InvalidVideoFileError(msg=f'SIMBA WARNING: Video {video_data["video_name"]} has {k} of {str(v)} (full error video path: {video_path}).')
+    video_data['resolution_str'] = str(f'{video_data["width"]} x {video_data["height"]}')
     video_data['video_length_s'] = int(video_data['frame_count'] / video_data['fps'])
     return video_data
 
-
 def check_directionality_viable(animal_bp_dict: dict):
     """
     Helper to check if it is possible to calculate ``directionality`` statistics (i.e., nose, and ear coordinates from
     pose estimation has to be present)
 
     Parameters
     ----------
@@ -366,16 +365,17 @@
 
     :return
     ----------
     list
 
     Examples
     ----------
-    >>> extract_frames_from_all_videos_in_directory(config_path='project_folder/project_config.ini', source='/MyVideoDirectory/')
+    >>> extract_frames_from_all_videos_in_directory(config_path='project_folder/project_config.ini', source='/tests/test_data/video_tests')
     """
+
     timer = SimbaTimer()
     timer.start_timer()
     video_paths, video_types = [], ['.avi', '.mp4']
     files_in_folder = glob.glob(directory + '/*')
     for file_path in files_in_folder:
         _, _, ext = get_fn_ext(filepath=file_path)
         if ext.lower() in video_types:
@@ -512,20 +512,20 @@
     """
 
     try:
         time_window_parameter = int(time_window_parameter)
     except:
         print('Savitzky-Golay smoothing failed for video {}. The specified time window parameter {} can not be interpreted as an integer.'.format(str(os.path.basename(file_path)), str(time_window_parameter)))
     _, filename, _ = get_fn_ext(file_path)
-    project_dir = config.get(ReadConfig.GENERAL_SETTINGS.value, ReadConfig.PROJECT_PATH.value)
+    project_dir, file_format = read_project_path_and_file_type(config=config)
+
     video_dir = os.path.join(project_dir, 'videos')
     video_file_path = find_video_of_file(video_dir, filename)
     if not video_file_path:
         raise NoFilesFoundError(msg=f'SIMBA ERROR: Import video for {filename} to perform Savitzky-Golay smoothing')
-    file_format = get_workflow_file_format(config)
     cap = cv2.VideoCapture(video_file_path)
     video_fps = int(cap.get(cv2.CAP_PROP_FPS))
     pose_df = read_df(file_path=file_path, file_type=file_format)
     header_cols = get_number_of_header_columns_in_df(df=pose_df)
     if header_cols == 2:
         idx_names = ['scorer', 'bodyparts', 'coords']
     else:
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_trk.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import scipy.io as sio
 from configparser import ConfigParser, MissingSectionHeaderError, NoSectionError, NoOptionError
 import h5py
 import cv2
 import pyarrow.parquet as pq
 import pyarrow as pa
 from simba.interpolate_pose import *
-from simba.drop_bp_cords import get_fn_ext, get_workflow_file_format
+from simba.drop_bp_cords import get_fn_ext
 from simba.misc_tools import check_multi_animal_status, smooth_data_gaussian
 
 
 def import_trk(inifile, dataFolder, idlist, interpolation_method, smooth_settings_dict):
     global currIDcounter
 
     def define_ID(event, x, y, flags, param):
@@ -36,15 +36,15 @@
 
     filesFound = glob.glob(dataFolder + '/*.trk')
     if len(filesFound) == 0: print('No TRK files found in ' + str(dataFolder))
 
     videoFolder = os.path.join(project_path, 'videos')
     outputDfFolder = os.path.join(project_path, 'csv', 'input_csv')
 
-    wfileType = get_workflow_file_format(config)
+    wfileType = 'csv'
 
     # ADD CORRECTION IF ONLY ONE ANIMAL
     if noAnimals < 2:
         idlist = ['Animal_1']
 
     multiAnimalStatus, multiAnimalIDList = check_multi_animal_status(config, noAnimals)
     Xcols, Ycols, Pcols = getBpNames(inifile)
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.3/simba/pop_up_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,16 @@
                                     extract_frame_range,
                                     extract_frames_single_video,
                                     batch_create_frames,
                                     change_single_video_fps,
                                     change_fps_of_multiple_videos,
                                     frames_to_movie,
                                     gif_creator,
-                                    video_concatenator)
+                                    video_concatenator,
+                                    VideoRotator)
 from simba.plotting.plot_clf_results import PlotSklearnResultsSingleCore
 from simba.plotting.plot_clf_results_mp import PlotSklearnResultsMultiProcess
 from simba.plotting.path_plotter import PathPlotterSingleCore
 from simba.plotting.path_plotter_mp import PathPlotterMulticore
 from simba.batch_process_videos.batch_process_menus import BatchProcessFrame
 from simba.plotting.Directing_animals_visualizer import DirectingOtherAnimalsVisualizer
 from simba.plotting.Directing_animals_visualizer_mp import DirectingOtherAnimalsVisualizerMultiprocess
@@ -3622,14 +3623,51 @@
                                                                          discrimination_threshold=float(self.discrimination_threshold),
                                                                          shortest_bout=int(self.shortest_bout),
                                                                          cores=int(self.multiprocess_dropdown.getChoices()),
                                                                          settings=settings,
                                                                          create_gantt=self.gantt_dropdown.getChoices())
         validation_video_creator.run()
 
+
+class VideoRotatorPopUp(PopUpMixin):
+    def __init__(self):
+        super().__init__(title='ROTATE VIDEOS')
+
+        self.save_dir_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SAVE LOCATION', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.save_dir = FolderSelect(self.save_dir_frm, 'Save directory:', lblwidth=20)
+
+        self.rotate_dir_frm = LabelFrame(self.main_frm, text='ROTATE VIDEOS IN DIRECTORY', font=Formats.LABELFRAME_HEADER_FORMAT.value)
+        self.input_dir = FolderSelect(self.rotate_dir_frm, 'Video directory:', lblwidth=20)
+        self.run_dir = Button(self.rotate_dir_frm, text='RUN', fg='blue', command=lambda: self.run(input_path=self.input_dir.folder_path,
+                                                                                                   output_path=self.save_dir.folder_path))
+
+        self.rotate_video_frm = LabelFrame(self.main_frm, text='ROTATE SINGLE VIDEO', font=Formats.LABELFRAME_HEADER_FORMAT.value)
+        self.input_file = FileSelect(self.rotate_video_frm, "Video path:", lblwidth=20)
+        self.run_file = Button(self.rotate_video_frm, text='RUN', fg='blue', command=lambda: self.run(input_path=self.input_file.file_path,
+                                                                                                   output_path=self.save_dir.folder_path))
+
+        self.save_dir_frm.grid(row=0, column=0, sticky=NW)
+        self.save_dir.grid(row=0, column=0, sticky=NW)
+
+        self.rotate_dir_frm.grid(row=1, column=0, sticky=NW)
+        self.input_dir.grid(row=0, column=0, sticky=NW)
+        self.run_dir.grid(row=1, column=0, sticky=NW)
+
+        self.rotate_video_frm.grid(row=2, column=0, sticky=NW)
+        self.input_file.grid(row=0, column=0, sticky=NW)
+        self.run_file.grid(row=1, column=0, sticky=NW)
+
+
+    def run(self, input_path: str, output_path: str):
+        check_if_dir_exists(in_dir=output_path)
+        rotator = VideoRotator(input_path=input_path, output_dir=output_path)
+        rotator.run()
+
+
+
 #_ = ValidationVideoPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 
 
 #_ = ThirdPartyAnnotatorAppenderPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.56.3/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.56.3/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.56.3/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/pose_reset.py` & `Simba-UW-tf-dev-1.56.3/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.56.3/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/SimBA.py` & `Simba-UW-tf-dev-1.56.3/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,16 @@
                                   InterpolatePopUp,
                                   SmoothingPopUp,
                                   BatchPreProcessPopUp,
                                   AppendROIFeaturesByBodyPartPopUp,
                                   ExtractAnnotationFramesPopUp,
                                   FeatureSubsetExtractorPopUp,
                                   ThirdPartyAnnotatorAppenderPopUp,
-                                  ValidationVideoPopUp)
+                                  ValidationVideoPopUp,
+                                  VideoRotatorPopUp)
 from simba.bounding_box_tools.boundary_menus import BoundaryMenus
 from simba.labelling_interface import select_labelling_video
 from simba.labelling_advanced_interface import select_labelling_video_advanced
 from simba.enums import (Formats,
                          OS,
                          Defaults,
                          TagNames)
@@ -358,15 +359,14 @@
 
         label_trainmachinemodel = CreateLabelFrameWithIcon(parent=tab8, header='TRAIN MACHINE MODELS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.TRAIN_ML_MODEL.value)
         #label_trainmachinemodel = LabelFrame(tab8,text='TRAIN MACHINE MODELS',font=Formats.LABELFRAME_HEADER_FORMAT.value,padx=5,pady=5,fg='black')
         button_trainmachinesettings = Button(label_trainmachinemodel,text='SETTINGS',command=self.trainmachinemodelsetting)
         button_trainmachinemodel = Button(label_trainmachinemodel,text='TRAIN SINGLE MODEL (GLOBAL ENVIRONMENT)',fg='blue',command = lambda: threading.Thread(target=self.train_single_model(config_path=self.config_path)).start())
         button_train_multimodel = Button(label_trainmachinemodel, text='TRAIN MULTIPLE MODELS (ONE FOR EACH SAVED SETTING)',fg='green',command = lambda: threading.Thread(target=self.train_multiple_models_from_meta(config_path=self.config_path)).start())
 
-
         label_model_validation = CreateLabelFrameWithIcon(parent=tab9, header='VALIDATE MODEL ON SINGLE VIDEO', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.OUT_OF_SAMPLE_VALIDATION.value)
         #label_model_validation = LabelFrame(tab9, text='VALIDATE MODEL ON SINGLE VIDEO', pady=5, padx=5, font=("Helvetica", 12, 'bold'), fg='blue')
         self.csvfile = FileSelect(label_model_validation, 'SELECT DATA FEATURE FILE', color='blue', lblwidth=30)
         self.modelfile = FileSelect(label_model_validation, 'SELECT MODEL FILE', color='blue', lblwidth=30)
         button_runvalidmodel = Button(label_model_validation, text='RUN MODEL', fg='blue', command=lambda: self.validate_model_first_step())
 
         button_generateplot = Button(label_model_validation, text="INTERACTIVE PROBABILITY PLOT", fg='blue', command= lambda: self.launch_interactive_plot())
@@ -790,14 +790,15 @@
         video_process_menu.add_cascade(label='Change formats...', compound='left', image=self.menu_icons['convert']['img'], menu=format_menu)
 
         video_process_menu.add_command(label='CLAHE enhance video', compound='left', image=self.menu_icons['clahe']['img'], command=CLAHEPopUp)
         video_process_menu.add_command(label='Superimpose frame numbers on video', compound='left', image=self.menu_icons['trash']['img'], command=lambda:superimpose_frame_count(file_path=askopenfilename()))
         video_process_menu.add_command(label='Convert to grayscale', compound='left', image=self.menu_icons['grey']['img'], command=lambda:video_to_greyscale(file_path=askopenfilename()))
         video_process_menu.add_command(label='Merge frames to video', compound='left', image=self.menu_icons['merge']['img'], command=MergeFrames2VideoPopUp)
         video_process_menu.add_command(label='Generate gifs', compound='left', image=self.menu_icons['gif']['img'], command=CreateGIFPopUP)
+        video_process_menu.add_command(label='Rotate videos', compound='left', image=self.menu_icons['rotate']['img'], command=VideoRotatorPopUp)
         video_process_menu.add_command(label='Print classifier info...', compound='left', image=self.menu_icons['print']['img'], command=PrintModelInfoPopUp)
 
         extract_frames_menu = Menu(video_process_menu)
         extract_frames_menu.add_command(label='Extract defined frames',command=ExtractSpecificFramesPopUp)
         extract_frames_menu.add_command(label='Extract frames',command=ExtractAllFramesPopUp)
         extract_frames_menu.add_command(label='Extract frames from seq files', command=ExtractSEQFramesPopUp)
         video_process_menu.add_cascade(label='Extract frames...', compound='left', image=self.menu_icons['frames']['img'], menu=extract_frames_menu)
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.56.3/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/assets/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -525,98 +525,98 @@
 000020c0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
 000020d0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
 000020f0: 0000 0500 6900 6300 6f00 6e00 736c 6731  ....i.c.o.n.slg1
 00002100: 5363 6f6d 7000 0000 0000 0590 7700 0000  Scomp.......w...
 00002110: 0500 6900 6300 6f00 6e00 736c 7376 4362  ..i.c.o.n.slsvCb
 00002120: 6c6f 6200 0002 af62 706c 6973 7430 30da  lob....bplist00.
-00002130: 0102 0304 0506 0708 090a 0b0c 0d18 4849  ..............HI
-00002140: 484a 0c4c 5869 636f 6e53 697a 655f 100f  HJ.LXiconSize_..
-00002150: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00002160: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00002170: 6174 6541 6c6c 5369 7a65 735f 100f 7363  ateAllSizes_..sc
-00002180: 726f 6c6c 506f 7369 7469 6f6e 5958 7465  rollPositionYXte
-00002190: 7874 5369 7a65 5f10 0f73 6372 6f6c 6c50  xtSize_..scrollP
-000021a0: 6f73 6974 696f 6e58 5a73 6f72 7443 6f6c  ositionXZsortCol
-000021b0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
-000021c0: 6544 6174 6573 5f10 1276 6965 774f 7074  eDates_..viewOpt
-000021d0: 696f 6e73 5665 7273 696f 6e23 4030 0000  ionsVersion#@0..
-000021e0: 0000 0000 09ab 0e17 1c21 252a 2f34 393e  .........!%*/49>
-000021f0: 43d4 0f10 1112 0c14 0c16 5776 6973 6962  C.........Wvisib
-00002200: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
-00002210: 6e67 5a69 6465 6e74 6966 6965 7209 10b3  ngZidentifier...
-00002220: 0954 6e61 6d65 d40f 1011 1218 1918 1b08  .Tname..........
-00002230: 1023 0858 7562 6971 7569 7479 d40f 1011  .#.Xubiquity....
-00002240: 120c 1e18 2009 10b5 085c 6461 7465 4d6f  .... ....\dateMo
-00002250: 6469 6669 6564 d40f 1011 1218 1e18 2408  dified........$.
-00002260: 085b 6461 7465 4372 6561 7465 64d4 0f10  .[dateCreated...
-00002270: 1112 0c27 1829 0910 6108 5473 697a 65d4  ...'.)..a.Tsize.
-00002280: 0f10 1112 0c2c 0c2e 0910 7309 546b 696e  .....,....s.Tkin
-00002290: 64d4 0f10 1112 1831 0c33 0810 6409 556c  d......1.3..d.Ul
-000022a0: 6162 656c d40f 1011 1218 360c 3808 104b  abel......6.8..K
-000022b0: 0957 7665 7273 696f 6ed4 0f10 1112 183b  .Wversion......;
-000022c0: 0c3d 0811 012c 0958 636f 6d6d 656e 7473  .=...,.Xcomments
-000022d0: d40f 1011 1218 4018 4208 10c8 085e 6461  ......@.B....^da
-000022e0: 7465 4c61 7374 4f70 656e 6564 d40f 1011  teLastOpened....
-000022f0: 1218 1e18 4608 0859 6461 7465 4164 6465  ....F..YdateAdde
-00002300: 6408 2300 0000 0000 0000 0023 4028 0000  d.#........#@(..
-00002310: 0000 0000 546e 616d 6509 1001 0008 001d  ....Tname.......
-00002320: 0026 0038 0040 0054 0066 006f 0081 008c  .&.8.@.T.f.o....
-00002330: 009f 00b4 00bd 00be 00ca 00d3 00db 00e1  ................
-00002340: 00eb 00f6 00f7 00f9 00fa 00ff 0108 0109  ................
-00002350: 010b 010c 0115 011e 011f 0121 0122 012f  ...........!."./
-00002360: 0138 0139 013a 0146 014f 0150 0152 0153  .8.9.:.F.O.P.R.S
-00002370: 0158 0161 0162 0164 0165 016a 0173 0174  .X.a.b.d.e.j.s.t
-00002380: 0176 0177 017d 0186 0187 0189 018a 0192  .v.w.}..........
-00002390: 019b 019c 019f 01a0 01a9 01b2 01b3 01b5  ................
-000023a0: 01b6 01c5 01ce 01cf 01d0 01da 01db 01e4  ................
-000023b0: 01ed 01f2 01f3 0000 0000 0000 0201 0000  ................
+00002130: 0102 0304 0506 0708 090a 0b0c 0d1a 4849  ..............HI
+00002140: 484a 0c4c 5f10 1276 6965 774f 7074 696f  HJ.L_..viewOptio
+00002150: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+00002160: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00002170: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00002180: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
+00002190: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
+000021a0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
+000021b0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
+000021c0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+000021d0: 6573 5869 636f 6e53 697a 6510 0109 ab0e  esXiconSize.....
+000021e0: 171c 2125 2a2f 3439 3e43 d40f 1011 1213  ..!%*/49>C......
+000021f0: 140c 0c5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
+00002200: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+00002210: 6973 6962 6c65 546e 616d 6510 ea09 09d4  isibleTname.....
+00002220: 0f10 1112 1819 1a1a 5875 6269 7175 6974  ........Xubiquit
+00002230: 7910 2308 08d4 0f10 1112 1d1e 1a0c 5c64  y.#...........\d
+00002240: 6174 654d 6f64 6966 6965 6410 b508 09d4  ateModified.....
+00002250: 0f10 1112 221e 1a1a 5b64 6174 6543 7265  ...."...[dateCre
+00002260: 6174 6564 0808 d40f 1011 1226 271a 0c54  ated.......&'..T
+00002270: 7369 7a65 1061 0809 d40f 1011 122b 2c0c  size.a.......+,.
+00002280: 0c54 6b69 6e64 1073 0909 d40f 1011 1230  .Tkind.s.......0
+00002290: 310c 1a55 6c61 6265 6c10 6409 08d4 0f10  1..Ulabel.d.....
+000022a0: 1112 3536 0c1a 5776 6572 7369 6f6e 104b  ..56..Wversion.K
+000022b0: 0908 d40f 1011 123a 3b0c 1a58 636f 6d6d  .......:;..Xcomm
+000022c0: 656e 7473 1101 2c09 08d4 0f10 1112 3f40  ents..,.......?@
+000022d0: 1a1a 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+000022e0: 6410 c808 08d4 0f10 1112 441e 1a1a 5964  d.........D...Yd
+000022f0: 6174 6541 6464 6564 0808 0823 0000 0000  ateAdded...#....
+00002300: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
+00002310: 6d65 0923 4030 0000 0000 0000 0008 001d  me.#@0..........
+00002320: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
+00002330: 00ab 00b4 00b6 00b7 00c3 00cc 00d7 00dd  ................
+00002340: 00e7 00ef 00f4 00f6 00f7 00f8 0101 010a  ................
+00002350: 010c 010d 010e 0117 0124 0126 0127 0128  .........$.&.'.(
+00002360: 0131 013d 013e 013f 0148 014d 014f 0150  .1.=.>.?.H.M.O.P
+00002370: 0151 015a 015f 0161 0162 0163 016c 0172  .Q.Z._.a.b.c.l.r
+00002380: 0174 0175 0176 017f 0187 0189 018a 018b  .t.u.v..........
+00002390: 0194 019d 01a0 01a1 01a2 01ab 01ba 01bc  ................
+000023a0: 01bd 01be 01c7 01d1 01d2 01d3 01d4 01dd  ................
+000023b0: 01e6 01eb 01ec 0000 0000 0000 0201 0000  ................
 000023c0: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
 000023d0: 0000 0000 01f5 0000 0005 0069 0063 006f  ...........i.c.o
 000023e0: 006e 0073 6c73 7670 626c 6f62 0000 0294  .n.slsvpblob....
 000023f0: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00002400: 0809 0a0b 0c0d 1f48 4948 4a0c 2658 6963  .......HIHJ.&Xic
-00002410: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
-00002420: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00002430: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00002440: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
-00002450: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
-00002460: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-00002470: 585a 736f 7274 436f 6c75 6d6e 5f10 1075  XZsortColumn_..u
-00002480: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
-00002490: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-000024a0: 7369 6f6e 2340 3000 0000 0000 0009 d90e  sion#@0.........
-000024b0: 0f10 1112 1314 1516 1720 252a 2e33 383d  ......... %*.38=
-000024c0: 4258 636f 6d6d 656e 7473 5e64 6174 654c  BXcomments^dateL
-000024d0: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-000024e0: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-000024f0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-00002500: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-00002510: 1819 1a1b 1c1d 0c1f 5569 6e64 6578 5577  ........UindexUw
-00002520: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-00002530: 6973 6962 6c65 1007 1101 2c09 08d4 1819  isible....,.....
-00002540: 1a1b 2122 1f1f 1008 10c8 0808 d418 191a  ..!"............
-00002550: 1b26 271f 0c10 0110 b508 09d4 1819 1a1b  .&'.............
-00002560: 2b27 1f1f 1002 0808 d418 191a 1b2f 301f  +'.........../0.
-00002570: 0c10 0310 6108 09d4 1819 1a1b 3435 0c1f  ....a.......45..
-00002580: 1005 1064 0908 d418 191a 1b39 3a0c 0c10  ...d.......9:...
-00002590: 0410 7309 09d4 1819 1a1b 3e3f 0c1f 1006  ..s.......>?....
-000025a0: 104b 0908 d418 191a 1b43 440c 0c10 0010  .K.......CD.....
-000025b0: b309 0908 2300 0000 0000 0000 0023 4028  ....#........#@(
-000025c0: 0000 0000 0000 546e 616d 6509 0008 001d  ......Tname.....
-000025d0: 0026 0038 0040 0054 0066 006f 0081 008c  .&.8.@.T.f.o....
-000025e0: 009f 00b4 00bd 00be 00d1 00da 00e9 00f6  ................
-000025f0: 0102 0107 010d 0112 011a 011f 0128 012e  .............(..
-00002600: 0134 013e 0146 0148 014b 014c 014d 0156  .4.>.F.H.K.L.M.V
-00002610: 0158 015a 015b 015c 0165 0167 0169 016a  .X.Z.[.\.e.g.i.j
-00002620: 016b 0174 0176 0177 0178 0181 0183 0185  .k.t.v.w.x......
-00002630: 0186 0187 0190 0192 0194 0195 0196 019f  ................
-00002640: 01a1 01a3 01a4 01a5 01ae 01b0 01b2 01b3  ................
-00002650: 01b4 01bd 01bf 01c1 01c2 01c3 01c4 01cd  ................
-00002660: 01d6 01db 0000 0000 0000 0201 0000 0000  ................
+00002400: 0809 0a0b 0c0d 1c47 4847 490c 4b5f 1012  .......GHGI.K_..
+00002410: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00002420: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00002430: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00002440: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00002450: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+00002460: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+00002470: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+00002480: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+00002490: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
+000024a0: 5369 7a65 1001 09d9 0e0f 1011 1213 1415  Size............
+000024b0: 1617 2025 292d 3237 3c41 5863 6f6d 6d65  .. %)-27<AXcomme
+000024c0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+000024d0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+000024e0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+000024f0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+00002500: 696f 6e54 6e61 6d65 d418 191a 1b1c 1d0c  ionTname........
+00002510: 1f57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+00002520: 6173 6365 6e64 696e 6755 696e 6465 7808  ascendingUindex.
+00002530: 1101 2c09 1007 d418 191a 1b1c 221c 2408  ..,.........".$.
+00002540: 10c8 0810 08d4 1819 1a1b 0c27 1c0b 0910  ...........'....
+00002550: b508 d418 191a 1b1c 271c 2c08 0810 02d4  ........'.,.....
+00002560: 1819 1a1b 0c2f 1c31 0910 6108 1003 d418  ...../.1..a.....
+00002570: 191a 1b1c 340c 3608 1064 0910 05d4 1819  ....4.6..d......
+00002580: 1a1b 0c39 0c3b 0910 7309 1004 d418 191a  ...9.;..s.......
+00002590: 1b1c 3e0c 4008 104b 0910 06d4 1819 1a1b  ..>.@..K........
+000025a0: 0c43 0c45 0910 ea09 1000 0823 0000 0000  .C.E.......#....
+000025b0: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
+000025c0: 6d65 0923 4030 0000 0000 0000 0008 001d  me.#@0..........
+000025d0: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
+000025e0: 00ab 00b4 00b6 00b7 00ca 00d3 00e2 00ef  ................
+000025f0: 00fb 0100 0106 010b 0113 0118 0121 0129  .............!.)
+00002600: 012f 0139 013f 0140 0143 0144 0146 014f  ./.9.?.@.C.D.F.O
+00002610: 0150 0152 0153 0155 015e 015f 0161 0162  .P.R.S.U.^._.a.b
+00002620: 016b 016c 016d 016f 0178 0179 017b 017c  .k.l.m.o.x.y.{.|
+00002630: 017e 0187 0188 018a 018b 018d 0196 0197  .~..............
+00002640: 0199 019a 019c 01a5 01a6 01a8 01a9 01ab  ................
+00002650: 01b4 01b5 01b7 01b8 01ba 01bb 01c4 01cd  ................
+00002660: 01d2 01d3 0000 0000 0000 0201 0000 0000  ................
 00002670: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
 00002680: 0000 01dc 0000 0005 0069 0063 006f 006e  .........i.c.o.n
 00002690: 0073 6d6f 4444 626c 6f62 0000 0008 da62  .smoDDblob.....b
 000026a0: afb9 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
 000026b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
 000026c0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
 000026d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.56.3/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.3/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.56.3/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.56.3/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.56.3/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.56.3/simba/drop_bp_cords.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 from simba.utils.warnings import BodypartColumnNotFoundWarning
-import configparser
 import pandas as pd
 import os
 from pathlib import Path
 from configparser import (ConfigParser,
                           NoOptionError)
 import glob
-import re
 from pylab import cm
 import shutil
 from datetime import datetime
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable)
-from simba.enums import ReadConfig, Paths
 from simba.utils.errors import InvalidFilepathError
-
+from simba.enums import Paths, ReadConfig, Dtypes
 
 
 def create_body_part_dictionary(multiAnimalStatus: bool,
                                 multiAnimalIDList: list,
                                 animalsNo: int,
                                 Xcols: list,
                                 Ycols: list,
@@ -150,66 +147,14 @@
     animal_bp_dict = create_body_part_dictionary(multi_animal_status, multi_animal_id_lst, no_animals, x_cols, y_cols, [], [])
     animal_bp_lists = []
     for animal_name, animal_data in animal_bp_dict.items():
         animal_bp_lists.append([x[0:-2] for x in animal_data['X_bps']])
     return animal_bp_lists
 
 
-
-# def define_bp_drop_down(configini):
-#     config = ConfigParser()
-#     configFile = str(configini)
-#     config.read(configFile)
-#     animalno = config.getint('General settings', 'animal_no')
-#     try:
-#         IDList = config.get('Multi animal IDs', 'id_list')
-#     except NoSectionError:
-#         IDList = []
-#
-#     # get list
-#     bpcsv = (os.path.join(os.path.dirname(configini), 'logs', 'measures', 'pose_configs', 'bp_names', 'project_bp_names.csv'))
-#     bplist = []
-#     with open(bpcsv) as f:
-#         for row in f:
-#             bplist.append(row)
-#     bplist = list(map(lambda x: x.replace('\n', ''), bplist))
-#
-#     if not IDList:
-#         if animalno != 1:
-#             animal1bp = [f for f in bplist if '_1' in f]
-#             animal2bp = [f for f in bplist if '_2' in f]
-#             return animal1bp,animal2bp
-#         else:
-#             animal1bp = bplist
-#             return animal1bp,['No body parts']
-#
-#     #multianimal
-#     if IDList:
-#         if animalno != 1:
-#             IDList = IDList.split(",")
-#             animalBpLists = []
-#             for animal in IDList:
-#                 animalBpLists.append([f for f in bplist if animal in f])
-#             if not animalBpLists[0]:
-#                 animalBpLists = []
-#                 for animal in range(animalno):
-#                     currStr = '_' + str(animal + 1)
-#                     currAnimalBp = [f for f in bplist if currStr in f]
-#                     animalBpLists.append(currAnimalBp)
-#             return animalBpLists
-#         else:
-#             animal1bp = bplist
-#             return animal1bp, ['No body parts']
-#
-#
-#
-#
-
-
-
 def drop_bp_cords(df: pd.DataFrame,
                   config_path: str):
 
     """
     Helper to remove pose-estimation data from dataframe.
 
     Parameters
@@ -241,119 +186,14 @@
         bp_headers.extend((colHead1, colHead2, colHead3))
     try:
         out_df = df.drop(bp_headers, axis=1)
         return out_df
     except KeyError as e:
         BodypartColumnNotFoundWarning(msg=f'SimBA could not drop body-part coordinates, some body-part names are missing in dataframe. SimBA expected the following body-parts, that could not be found inside the file: {e.args[0]}')
 
-def define_movement_cols(multi_animal_id_list: list):
-    """
-    Helper to create column names representing aggregate movement and velocity for each animal in the video.
-
-    Parameters
-    ----------
-    multi_animal_id_list: list
-        list of animal names
-
-    Examples
-    -----
-    >>> column_names = define_movement_cols(multi_animal_id_list=['Animal_1', 'Animal_2' 'Animal_3'])
-    """
-
-    columnNames = ['Video', 'Frames processed']
-    if len(multi_animal_id_list) == 1:
-        columnNames = ['Video', 'Frames processed', 'Total movement (cm)', 'Mean velocity (cm / s)', 'Median velocity (cm/s)']
-    if len(multi_animal_id_list) == 2:
-        movementCols, meanVelCols, MedianVelCols = [], [], []
-        for animal in multi_animal_id_list:
-            movementCols.append( 'Total movement (cm) ' + animal)
-            meanVelCols.append('Mean velocity (cm/s) ' + animal)
-            MedianVelCols.append('Median velocity (cm/s) ' + animal)
-        columnNames = columnNames + movementCols + meanVelCols + MedianVelCols
-        str4, str5 = 'Mean animal distance (cm)', 'Median animal distance (cm)'
-        columnNames.extend((str4, str5))
-    if len(multi_animal_id_list) > 2:
-        for animal in multi_animal_id_list:
-            str1, str2, str3, = 'Total movement (cm) ' + animal, 'Mean velocity (cm / s) ' + animal, 'Median velocity (cm / s) ' + animal
-            columnNames.extend((str1, str2, str3))
-
-    return columnNames
-
-def bodypartConfSchematic():
-    """Helper to return (i) named body-part schematics of all pose-estimation schemas in SimBA installation, and
-    (ii) the paths to the images representing those body-part schematics in SimBA installation
-    """
-
-    optionsBaseListImagesPath = os.path.join(os.path.dirname(__file__), Paths.SCHEMATICS.value)
-    optionsBaseListNamesPath = os.path.join(os.path.dirname(__file__), 'pose_configurations', 'configuration_names', 'pose_config_names.csv')
-    optionsBaseNameList = pd.read_csv(optionsBaseListNamesPath, header=None)
-    optionsBaseNameList = list(optionsBaseNameList[0])
-    optionsBaseNameList.append('Create pose config...')
-    optionsBasePhotosList = glob.glob(optionsBaseListImagesPath + '/*.png')
-    optionsBasePhotosList.sort(key=lambda var: [int(x) if x.isdigit() else x for x in re.findall(r'[^0-9]|[0-9]+', var)])
-    return optionsBaseNameList, optionsBasePhotosList
-
-
-def GenerateMetaDataFileHeaders():
-    """Helper to return the headings for the SimBA RF model config files."""
-
-
-    meta_data_headers = ["Classifier_name",
-                         "RF_criterion",
-                         "RF_max_features",
-                         "RF_min_sample_leaf",
-                         "RF_n_estimators",
-                         "compute_feature_permutation_importance",
-                         "generate_classification_report",
-                         "generate_example_decision_tree",
-                         "generate_features_importance_bar_graph",
-                         "generate_features_importance_log",
-                         "generate_precision_recall_curves",
-                         "generate_rf_model_meta_data_file",
-                         "generate_sklearn_learning_curves",
-                         "learning_curve_data_splits",
-                         "learning_curve_k_splits",
-                         "n_feature_importance_bars",
-                         "over_sample_ratio",
-                         "over_sample_setting",
-                         "train_test_size",
-                         "train_test_split_type",
-                         "under_sample_ratio",
-                         "under_sample_setting",
-                         "class_weights"]
-
-    return meta_data_headers
-
-
-def getBpHeaders(inifile: str):
-    """
-    Helper to create ordered list of all column header fields for SimBA project dataframes.
-
-    Parameters
-    ----------
-    inifile: str
-        Path to SimBA project_config.ini
-
-    Returns
-    -------
-    column_headers: list
-    """
-
-    column_headers = []
-    config = read_config_file(inifile)
-    project_path = config.get('General settings', 'project_path')
-    bodyparthListPath = os.path.join(project_path, 'logs', 'measures', 'pose_configs', 'bp_names','project_bp_names.csv')
-    poseConfigDf = pd.read_csv(bodyparthListPath, header=None)
-    poseConfigList = list(poseConfigDf[0])
-    for bodypart in poseConfigList:
-        colHead1, colHead2, colHead3 = (bodypart + '_x', bodypart + '_y', bodypart + '_p')
-        column_headers.extend((colHead1, colHead2, colHead3))
-    return column_headers
-
-
 def checkDirectionalityCords(animal_bp_dict: dict):
     """
     Helper to check if ear and nose body-parts are present within the pose-estimation data.
 
     Parameters
     ----------
     animal_bp_dict: dict
@@ -384,54 +224,14 @@
                     directionalityDict[animal]['Ear_left']['Y_bps'] = columnName
                 if ("Right".lower() in columnName.lower()) and ("X".lower() in columnName.lower()) and ("ear".lower() in columnName.lower()):
                     directionalityDict[animal]['Ear_right']['X_bps'] = columnName
                 if ("Right".lower() in columnName.lower()) and ("Y".lower() in columnName.lower()) and ("ear".lower() in columnName.lower()):
                     directionalityDict[animal]['Ear_right']['Y_bps'] = columnName
     return directionalityDict
 
-def createColorListofList(no_animals: int,
-                          map_size: int):
-    """
-    Helper to return a list of lists of bgr colors. Each list is pulled from a different palette
-    matplotlib color map.
-
-    Parameters
-    ----------
-    no_animals: int
-        Number of different palette lists
-    map_size: int
-        Number of colors in each created palette.
-
-    Returns
-     ----------
-     colorListofList: list
-        List of lists holding bgr colors
-
-    Notes
-    -----
-
-    Examples
-    -----
-    >>> colorListofList = createColorListofList(no_animals=2, map_size=8)
-    """
-
-    colorListofList = []
-    cmaps = ['spring', 'summer', 'autumn', 'cool', 'Wistia', 'Pastel1', 'Set1', 'winter', 'afmhot', 'gist_heat', 'copper']
-    for colormap in range(no_animals):
-        currColorMap = cm.get_cmap(cmaps[colormap], map_size)
-        currColorList = []
-        for i in range(currColorMap.N):
-            rgb = list((currColorMap(i)[:3]))
-            rgb = [i * 255 for i in rgb]
-            rgb.reverse()
-            currColorList.append(rgb)
-        colorListofList.append(currColorList)
-    return colorListofList
-
-
 def reverse_dlc_input_files(configini):
     dateTime = datetime.now().strftime('%Y%m%d%H%M%S')
     config = ConfigParser()
     config.read(configini)
     projectPath = config.get('General settings', 'project_path')
 
     input_folder_path = os.path.join(projectPath, 'csv', 'input_csv')
@@ -468,51 +268,109 @@
         for curr_df in reversed(df_list): reversed_df = pd.concat([reversed_df, curr_df], axis=1)
         reversed_df.columns = currentDf.columns
         reversed_df.iloc[0:1] = currentDf.iloc[0:1]
         shutil.move(file, os.path.join(store_original_files_folder, os.path.basename(file)))
         save_df(reversed_df, wfileType, file)
     print('All reversals complete.')
 
+
+def getBpHeaders(inifile: str):
+    """
+    Helper to create ordered list of all column header fields for SimBA project dataframes.
+
+    Parameters
+    ----------
+    inifile: str
+        Path to SimBA project_config.ini
+
+    Returns
+    -------
+    list
+    """
+
+    config = read_config_file(inifile)
+    project_path = read_config_entry(config=config, section=ReadConfig.GENERAL_SETTINGS.value, option=ReadConfig.PROJECT_PATH.value, data_type=Dtypes.STR.value)
+    bp_path = os.path.join(project_path, Paths.BP_NAMES.value)
+    check_file_exist_and_readable(file_path=bp_path)
+    bp_df = pd.read_csv(bp_path, header=None)
+    bp_lst = list(bp_df[0])
+    results = []
+    for bp in bp_lst:
+        c1, c2, c3 = (f'{bp}_x', f'{bp}_y', f'{bp}_p')
+        results.extend((c1, c2, c3))
+    return results
+
 def get_fn_ext(filepath: str):
     """
     Helper to split file path into three components: (i) directory, (ii) file name, and (iii) file extension.
-
     Parameters
     ----------
     filepath: str
         Path to file.
-
     Returns
     -------
     dir_name: str
     file_name: str
     file_extension: str
-
     """
     file_extension = Path(filepath).suffix
     try:
         file_name = os.path.basename(filepath.rsplit(file_extension, 1)[0])
     except ValueError:
         raise InvalidFilepathError(msg='{} is not a valid filepath'.format(filepath))
     dir_name = os.path.dirname(filepath)
     return dir_name, file_name, file_extension
 
 
-def get_workflow_file_format(config: configparser.ConfigParser):
+
+
+def createColorListofList(no_animals: int,
+                          map_size: int):
     """
-    Helper to read the workflow file format in SimBA project. If missing, then defaults to CSV.
+    Helper to return a list of lists of bgr colors. Each list is pulled from a different palette
+    matplotlib color map.
 
     Parameters
     ----------
-    config: configparser.ConfigParser
+    no_animals: int
+        Number of different palette lists
+    map_size: int
+        Number of colors in each created palette.
 
     Returns
-    -------
-    wfileType: str
+     ----------
+     colorListofList: list
+        List of lists holding bgr colors
+
+    Notes
+    -----
+
+    Examples
+    -----
+    >>> colorListofList = createColorListofList(no_animals=2, map_size=8)
     """
 
-    try:
-        wfileType = config.get('General settings', 'workflow_file_type')
-        return wfileType
-    except NoOptionError:
-        return 'csv'
+    colorListofList = []
+    cmaps = ['spring',
+            'summer',
+            'autumn',
+            'cool',
+            'Wistia',
+            'Pastel1',
+            'Set1',
+            'winter',
+            'afmhot',
+            'gist_heat',
+            'copper']
+    for colormap in range(no_animals):
+        currColorMap = cm.get_cmap(cmaps[colormap], map_size)
+        currColorList = []
+        for i in range(currColorMap.N):
+            rgb = list((currColorMap(i)[:3]))
+            rgb = [i * 255 for i in rgb]
+            rgb.reverse()
+            currColorList.append(rgb)
+        colorListofList.append(currColorList)
+    return colorListofList
+
+
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.56.3/simba/read_config_unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     try:
         if config.has_option(section, option):
             if data_type == 'float':
                 value = config.getfloat(section, option)
             elif data_type == 'int':
                 value = config.getint(section, option)
             elif data_type == 'str':
-                value = config.get(section, option)
+                value = config.get(section, option).strip()
             elif data_type == 'folder_path':
-                value = config.get(section, option)
+                value = config.get(section, option).strip()
                 if not os.path.isdir(value):
                     raise NotDirectoryError(msg=f'The SimBA config file includes paths to a folder ({value}) that does not exist.')
             if options != None:
                 if value not in options:
                     raise InvalidInputError(msg=f'{option} is set to {str(value)} in SimBA, but this is not among the valid options: ({options})')
                 else:
                     return value
```

### Comparing `Simba-UW-tf-dev-1.56.2/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.56.3/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.56.3/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/train_single_model.py` & `Simba-UW-tf-dev-1.56.3/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.56.3/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.56.3/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.56.3/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.56.3/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.2
+Version: 1.56.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 simba/assets/icons/outlier.png
 simba/assets/icons/path.png
 simba/assets/icons/pose.png
 simba/assets/icons/print.png
 simba/assets/icons/reorganize.png
 simba/assets/icons/restart.png
 simba/assets/icons/roi.png
+simba/assets/icons/rotate.png
 simba/assets/icons/sample.png
 simba/assets/icons/settings.png
 simba/assets/icons/superimpose.png
 simba/assets/icons/trash.png
 simba/assets/icons/video.png
 simba/assets/icons/visualize.png
 simba/assets/icons/concat_icons/horizontal.png
@@ -207,23 +208,26 @@
 simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
 simba/feature_extractors/misc/.DS_Store
 simba/feature_extractors/misc/add_probability_cnt_features.py
 simba/feature_extractors/misc/convex_hull_3_scratch_3.py
 simba/feature_extractors/misc/convex_hull_scratch_1.py
 simba/feature_extractors/misc/convex_hull_scratch_2.py
 simba/feature_extractors/misc/count_values_in_range.py
+simba/feature_extractors/misc/doctests.py
 simba/feature_extractors/misc/egocentrical_aligner.py
 simba/feature_extractors/misc/fish_feature_extractor_2022.py
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
+simba/feature_extractors/misc/video_color.py
+simba/feature_extractors/misc/video_rotator.py
 simba/mixins/.DS_Store
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/pop_up_mixin.py
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
 simba/outlier_tools/outlier_corrector_location.py
```

### Comparing `Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/LICENSE.md` & `Simba-UW-tf-dev-1.56.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/README.md` & `Simba-UW-tf-dev-1.56.3/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.2/setup.py` & `Simba-UW-tf-dev-1.56.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.56.2",
+    version="1.56.3",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

