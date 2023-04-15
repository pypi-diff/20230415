# Comparing `tmp/peegy-1.3.4.tar.gz` & `tmp/peegy-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peegy-1.3.4.tar", last modified: Sun Mar  5 16:11:22 2023, max compression
+gzip compressed data, was "peegy-1.3.6.tar", last modified: Sat Apr 15 08:16:52 2023, max compression
```

## Comparing `peegy-1.3.4.tar` & `peegy-1.3.6.tar`

### file list

```diff
@@ -1,209 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.610292 peegy-1.3.4/
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-03-05 15:53:57.000000 peegy-1.3.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1150 2023-03-05 16:11:22.610292 peegy-1.3.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.397276 peegy-1.3.4/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10796 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_abr_peak_detection.py
--rw-rw-rw-   0 root         (0) root         (0)    17277 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_acc_eog_removal_template_.py
--rw-rw-rw-   0 root         (0) root         (0)    10930 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_acc_peak_detection.py
--rw-rw-rw-   0 root         (0) root         (0)    10923 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_acc_peak_detection_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    12109 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_acc_video.py
--rw-rw-rw-   0 root         (0) root         (0)    12378 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_acc_weighted_average.py
--rw-rw-rw-   0 root         (0) root         (0)    10304 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_acc_weighted_vs_standard_average.py
--rw-rw-rw-   0 root         (0) root         (0)    12620 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_dss_frequency_domain_bias_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12503 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_dss_time_domain_bias_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_f_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11144 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_ht2_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11861 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_ht2_test_weighted_average.py
--rw-rw-rw-   0 root         (0) root         (0)     8671 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
--rw-rw-rw-   0 root         (0) root         (0)     6918 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_no_layout.py
--rw-rw-rw-   0 root         (0) root         (0)     6851 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_assr_phase_locking_value_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12611 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_ffr_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     7895 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_using_own_data_trials.py
--rw-rw-rw-   0 root         (0) root         (0)     7952 2023-03-05 15:53:57.000000 peegy-1.3.4/examples/example_using_own_raw_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.398276 peegy-1.3.4/peegy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.443279 peegy-1.3.4/peegy/definitions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/definitions/channel_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    31413 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/definitions/edf_bdf_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    57262 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/definitions/eegReaderAbstractClasses.py
--rw-rw-rw-   0 root         (0) root         (0)     9074 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/definitions/eeg_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     7273 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/definitions/events.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/definitions/tables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.444280 peegy-1.3.4/peegy/directories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/directories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/directories/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.448280 peegy-1.3.4/peegy/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20916 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/edf_bdf_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.449280 peegy-1.3.4/peegy/io/eeg/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/eeg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/eeg/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.451280 peegy-1.3.4/peegy/io/external_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/external_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.457280 peegy-1.3.4/peegy/io/external_tools/aep_gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/external_tools/aep_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    11573 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/external_tools/aep_gui/dataReadingTools.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/external_tools/aep_gui/extsys_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    20273 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/external_tools/file_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4695 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/generic_csv_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.460281 peegy-1.3.4/peegy/io/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10450 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/storage/data_storage_reading_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    16923 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/storage/data_storage_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    23563 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/storage/plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/synergy_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/io/xml_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.474282 peegy-1.3.4/peegy/layouts/
--rw-rw-rw-   0 root         (0) root         (0)    10895 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/KIT-160.lay
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5612 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi128.lay
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi16.lay
--rw-rw-rw-   0 root         (0) root         (0)     7045 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi160.lay
--rw-rw-rw-   0 root         (0) root         (0)    11339 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi256.lay
--rw-rw-rw-   0 root         (0) root         (0)     1379 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi32.lay
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi32_2_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi32_fnirs_MP.lay
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi32_fnirs_jaime.lay
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi64.lay
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi64_2_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)     2903 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/biosemi64_3_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)      597 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/emotive14.lay
--rw-rw-rw-   0 root         (0) root         (0)     5246 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/layouts.py
--rw-rw-rw-   0 root         (0) root         (0)     3821 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/layouts/neuroscan64.lay
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.477282 peegy-1.3.4/peegy/plot/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50150 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/plot/eeg_ave_epochs_plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/plot/eeg_plot_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.478282 peegy-1.3.4/peegy/processing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.479282 peegy-1.3.4/peegy/processing/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3067 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/events/event_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.516285 peegy-1.3.4/peegy/processing/pipe/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/attach.py
--rw-rw-rw-   0 root         (0) root         (0)    23278 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/detection.py
--rw-rw-rw-   0 root         (0) root         (0)    30039 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/epochs.py
--rw-rw-rw-   0 root         (0) root         (0)    27509 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/general.py
--rw-rw-rw-   0 root         (0) root         (0)     9032 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    13088 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/io.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)    15881 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     6983 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/regression.py
--rw-rw-rw-   0 root         (0) root         (0)    22084 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/simulate.py
--rw-rw-rw-   0 root         (0) root         (0)    37719 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/spatial_filtering.py
--rw-rw-rw-   0 root         (0) root         (0)    27211 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10453 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/pipe/time_frequency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.518285 peegy-1.3.4/peegy/processing/statistics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/statistics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5518 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/statistics/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    14330 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/statistics/eeg_statistic_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.520285 peegy-1.3.4/peegy/processing/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/system/memory.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/system/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.522285 peegy-1.3.4/peegy/processing/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.524285 peegy-1.3.4/peegy/processing/tools/detection/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/detection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8780 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/detection/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     9602 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/detection/time_domain_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    20594 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/eeg_epoch_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    69125 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/epochs_processing_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.525286 peegy-1.3.4/peegy/processing/tools/filters/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15600 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/eegFiltering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.526286 peegy-1.3.4/peegy/processing/tools/filters/eog_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/eog_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19683 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/eog_tools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/resampling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.527286 peegy-1.3.4/peegy/processing/tools/filters/spatial_filtering/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/spatial_filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/spatial_filtering/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     4255 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.528286 peegy-1.3.4/peegy/processing/tools/fitting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/fitting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/fitting/fitting_functions.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/math_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.529286 peegy-1.3.4/peegy/processing/tools/multiprocessing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/multiprocessing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.530286 peegy-1.3.4/peegy/processing/tools/template_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/template_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13598 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/template_generator/auditory_waveforms.py
--rw-rw-rw-   0 root         (0) root         (0)    37074 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/template_generator/h0.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.531286 peegy-1.3.4/peegy/processing/tools/video/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/video/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/video/recording.py
--rw-rw-rw-   0 root         (0) root         (0)    48703 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/processing/tools/weightedAverage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.605291 peegy-1.3.4/peegy/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.606291 peegy-1.3.4/peegy/test/artifact_removal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/artifact_removal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3258 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/artifact_removal/ir_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4867 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/artifact_removal/regression_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     4857 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/artifact_removal/xcorr_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/dss_unit_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/eeg_test_resampling.py
--rw-rw-rw-   0 root         (0) root         (0)     3638 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/javerager_test.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/read_data_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3406 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_assr_moving_average.py
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_average_spectrogram_power.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_biosemi_class.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_biosemi_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_bootstraping.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_edf_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_eeg_notch_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_eog_removal_correlation.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_eog_template_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_eog_template_valderrama_20118.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_et_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2582 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_fir_filter_mt.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_fir_filter_ols.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_fiter_mt.py
--rw-rw-rw-   0 root         (0) root         (0)     5716 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_freq_noise_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_frequency_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_generic_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     2032 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_hotelling_t2.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_ica_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_noise_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_norm_corr.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_parse_processing_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_peakdetection.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_phase_locking_value.py
--rw-rw-rw-   0 root         (0) root         (0)     6025 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_pooled_freq_noise_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_scrolling.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_spatial_filtering_example1.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_spatial_filtering_example6.py
--rw-rw-rw-   0 root         (0) root         (0)     6015 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_spatial_filtering_freq_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     7035 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_spatial_filtering_freq_domain_2.py
--rw-rw-rw-   0 root         (0) root         (0)     8319 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_w_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/test/test_xml_to_dict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.607292 peegy-1.3.4/peegy/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.607292 peegy-1.3.4/peegy/tools/aep_gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/tools/aep_gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.608292 peegy-1.3.4/peegy/tools/signal_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/tools/signal_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4417 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/tools/signal_generator/noise_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.609292 peegy-1.3.4/peegy/tools/units/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/tools/units/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-03-05 15:53:57.000000 peegy-1.3.4/peegy/tools/units/unit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.399276 peegy-1.3.4/peegy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-03-05 16:11:21.000000 peegy-1.3.4/peegy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6499 2023-03-05 16:11:22.000000 peegy-1.3.4/peegy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-05 16:11:21.000000 peegy-1.3.4/peegy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-05 16:11:21.000000 peegy-1.3.4/peegy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-05 16:11:21.000000 peegy-1.3.4/peegy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-05 16:11:22.610292 peegy-1.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-03-05 15:53:57.000000 peegy-1.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-05 16:11:22.609292 peegy-1.3.4/test_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-05 15:53:57.000000 peegy-1.3.4/test_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.154836 peegy-1.3.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-04-15 07:57:16.000000 peegy-1.3.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-15 08:16:52.153836 peegy-1.3.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.975818 peegy-1.3.6/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10796 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_abr_peak_detection.py
+-rw-rw-rw-   0 root         (0) root         (0)    17277 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_eog_removal_template_.py
+-rw-rw-rw-   0 root         (0) root         (0)    10930 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_peak_detection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8276 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_peak_detection_bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    10923 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_peak_detection_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    12109 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_video.py
+-rw-rw-rw-   0 root         (0) root         (0)    12378 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_weighted_average.py
+-rw-rw-rw-   0 root         (0) root         (0)    10304 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_weighted_vs_standard_average.py
+-rw-rw-rw-   0 root         (0) root         (0)    15470 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_dss_frequency_domain_bias_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12503 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_dss_time_domain_bias_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9505 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_f_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    11144 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_ht2_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    11861 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_ht2_test_weighted_average.py
+-rw-rw-rw-   0 root         (0) root         (0)     8671 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6918 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_no_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)     6851 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_phase_locking_value_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12611 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_ffr_artifact_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     7895 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_using_own_data_trials.py
+-rw-rw-rw-   0 root         (0) root         (0)     7952 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_using_own_raw_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.977818 peegy-1.3.6/peegy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.986819 peegy-1.3.6/peegy/definitions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/channel_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31413 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/edf_bdf_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    57262 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/eegReaderAbstractClasses.py
+-rw-rw-rw-   0 root         (0) root         (0)     9074 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/eeg_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7273 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/tables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.987819 peegy-1.3.6/peegy/directories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/directories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/directories/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.991820 peegy-1.3.6/peegy/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20916 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/edf_bdf_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.992820 peegy-1.3.6/peegy/io/eeg/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/eeg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7491 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/eeg/reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.994820 peegy-1.3.6/peegy/io/external_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.998820 peegy-1.3.6/peegy/io/external_tools/aep_gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    11573 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/dataReadingTools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/extsys_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    20273 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/file_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4695 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/generic_csv_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.004821 peegy-1.3.6/peegy/io/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10450 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/data_storage_reading_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    16923 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/data_storage_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    29181 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/synergy_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/xml_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.018822 peegy-1.3.6/peegy/layouts/
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/KIT-160.lay
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi128.lay
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi16.lay
+-rw-rw-rw-   0 root         (0) root         (0)     7045 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi160.lay
+-rw-rw-rw-   0 root         (0) root         (0)    11339 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi256.lay
+-rw-rw-rw-   0 root         (0) root         (0)     1379 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32.lay
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32_2_EXT.lay
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32_fnirs_MP.lay
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32_fnirs_jaime.lay
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi64.lay
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi64_2_EXT.lay
+-rw-rw-rw-   0 root         (0) root         (0)     2903 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi64_3_EXT.lay
+-rw-rw-rw-   0 root         (0) root         (0)      597 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/emotive14.lay
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/layouts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3821 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/neuroscan64.lay
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.022823 peegy-1.3.6/peegy/plot/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50150 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/plot/eeg_ave_epochs_plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3001 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/plot/eeg_plot_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.023823 peegy-1.3.6/peegy/processing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.023823 peegy-1.3.6/peegy/processing/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3067 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/events/event_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.081829 peegy-1.3.6/peegy/processing/pipe/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/attach.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.082829 peegy-1.3.6/peegy/processing/pipe/bootstrap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/bootstrap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12387 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/bootstrap/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    25813 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/detection.py
+-rw-rw-rw-   0 root         (0) root         (0)    30969 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)    33757 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     9032 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13088 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     4961 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)    15881 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6983 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)    22084 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/simulate.py
+-rw-rw-rw-   0 root         (0) root         (0)    38597 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/spatial_filtering.py
+-rw-rw-rw-   0 root         (0) root         (0)    27211 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6463 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10453 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/time_frequency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.084829 peegy-1.3.6/peegy/processing/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/statistics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/statistics/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14461 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/statistics/eeg_statistic_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.085829 peegy-1.3.6/peegy/processing/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/system/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/system/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.088829 peegy-1.3.6/peegy/processing/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.090829 peegy-1.3.6/peegy/processing/tools/detection/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/detection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8780 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/detection/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9602 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/detection/time_domain_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    20468 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/eeg_epoch_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    69736 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/epochs_processing_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.091830 peegy-1.3.6/peegy/processing/tools/filters/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15600 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/eegFiltering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.092830 peegy-1.3.6/peegy/processing/tools/filters/eog_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/eog_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19679 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/eog_tools/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/resampling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.094830 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6169 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.095830 peegy-1.3.6/peegy/processing/tools/fitting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/fitting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/fitting/fitting_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/math_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.095830 peegy-1.3.6/peegy/processing/tools/multiprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/multiprocessing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.097830 peegy-1.3.6/peegy/processing/tools/template_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/template_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13598 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/template_generator/auditory_waveforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    37074 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/template_generator/h0.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.098830 peegy-1.3.6/peegy/processing/tools/video/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/video/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/video/recording.py
+-rw-rw-rw-   0 root         (0) root         (0)    48703 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/weightedAverage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.148835 peegy-1.3.6/peegy/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.150836 peegy-1.3.6/peegy/test/artifact_removal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3258 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/ir_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/regression_artifact_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4857 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/xcorr_artifact_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/dss_unit_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/eeg_test_resampling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3638 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/javerager_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/read_data_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3406 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_assr_moving_average.py
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_average_spectrogram_power.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_biosemi_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_biosemi_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_bootstraping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_edf_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eeg_notch_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eog_removal_correlation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eog_template_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eog_template_valderrama_20118.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_et_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2582 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_fir_filter_mt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_fir_filter_ols.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_fiter_mt.py
+-rw-rw-rw-   0 root         (0) root         (0)     5716 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_freq_noise_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3476 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_freq_noise_estimation_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_frequency_average_epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_generic_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_hotelling_t2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_ica_average_epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_noise_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_norm_corr.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_parse_processing_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_peakdetection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_phase_locking_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     6025 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_pooled_freq_noise_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_scrolling.py
+-rw-rw-rw-   0 root         (0) root         (0)     5499 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_example1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_example6.py
+-rw-rw-rw-   0 root         (0) root         (0)     6047 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     7065 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     8319 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_w_average_epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_xml_to_dict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.150836 peegy-1.3.6/peegy/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.151836 peegy-1.3.6/peegy/tools/aep_gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/aep_gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.152836 peegy-1.3.6/peegy/tools/signal_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/signal_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/signal_generator/noise_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.153836 peegy-1.3.6/peegy/tools/units/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/units/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/units/unit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.979818 peegy-1.3.6/peegy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6684 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 08:16:52.154836 peegy-1.3.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-15 07:57:16.000000 peegy-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.153836 peegy-1.3.6/test_data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/test_data/__init__.py
```

### Comparing `peegy-1.3.4/LICENSE.txt` & `peegy-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/PKG-INFO` & `peegy-1.3.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peegy
-Version: 1.3.4
+Version: 1.3.6
 Summary: Tools to pipeline bulk analyses of EEG and other modalities.
 Home-page: https://jundurraga.gitlab.io/peegy/
 Author: Jaime A. Undurraga
 Author-email: jaime.undurraga@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `peegy-1.3.4/examples/example_abr_peak_detection.py` & `peegy-1.3.6/examples/example_abr_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_acc_eog_removal_template_.py` & `peegy-1.3.6/examples/example_acc_eog_removal_template_.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_acc_peak_detection.py` & `peegy-1.3.6/examples/example_acc_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_acc_peak_detection_filters.py` & `peegy-1.3.6/examples/example_acc_peak_detection_filters.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_acc_video.py` & `peegy-1.3.6/examples/example_acc_video.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_acc_weighted_average.py` & `peegy-1.3.6/examples/example_acc_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_acc_weighted_vs_standard_average.py` & `peegy-1.3.6/examples/example_acc_weighted_vs_standard_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_assr_dss_frequency_domain_bias_test.py` & `peegy-1.3.6/examples/example_assr_dss_time_domain_bias_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
-.. _tut-assr-ht2-test-frequency-bias-sim:
+.. _tut-assr-ht2-test-dss-time-bias-sim:
 
-##################################################
-ASSR using DSS in the frequency-domain (Simulated)
-##################################################
+##############################################
+ASSR using DSS in the time-domain (Simulated)
+##############################################
 
 In this example we simulate a low-frequency ASSR, and we assess its significance using the Hotelling's T2 test and
 F-test.
 The background-noise is pink (controlled by noise attenuation = 3) and the presence of the signal is controlled by
 return_noise_only=False (if True, only the noise is returned).
 The signal is equal in all channels so that the detection rate obtained by keeping components can be assessed.
-The spatial filter is biased using the covariance obtained in the frequency-domain.
-This example shows that biasing in the frequency-domain requires > 16 components (about half channels) to keep the
-false detection rate under 5%
+The spatial filter is biased using the covariance obtained in the time-domain.
+This example shows that biasing in the frequency-domain requires only 1 component to keep the
+false detection rate at zero and true detection rate at 100%.
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
@@ -60,21 +60,21 @@
 
 template_waveform, _ = aep(fs=fs)
 n_channels = 32
 event_times = np.arange(0, 360.0, 1 / assr_frequency.to(u.Hz).value)
 reader = GenerateInputData(template_waveform=template_waveform,
                            fs=fs,
                            n_channels=n_channels,
+                           mixing_matrix=np.diag(np.ones(n_channels))/n_channels,
                            snr=0.001,
                            layout_file_name='biosemi32.lay',
                            event_times=event_times,
                            event_code=1.0,
-                           figures_subset_folder='assr_dss_frequency_domain_test',
+                           figures_subset_folder='assr_dss_time_domain_test',
                            return_noise_only=True,
-                           mixing_matrix=np.diag(np.ones(n_channels))/n_channels,
                            noise_attenuation=3,
                            noise_seed=0)
 reader.run()
 
 # %%
 # Resize events
 # ===================
@@ -105,17 +105,16 @@
 
 # %%
 # Plot components in the frequency-domain
 # ---------------------------------------
 # Spatial filter is a applied in the frequency-domain
 
 pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
-                                                          sf_join_frequencies=join_frequencies,
                                                           test_frequencies=test_frequencies,
-                                                          sf_components=np.arange(17),
+                                                          sf_components=np.arange(1),
                                                           projection_domain=Domain.frequency,
                                                           block_size=10,
                                                           return_figures=True,
                                                           delta_frequency=2 * u.Hz,
                                                           plot_y_lim=[0, 5])
 pipeline.run()
 
@@ -157,29 +156,29 @@
 
 pipeline['std_fft_ave_gfp_ftest'] = FTest(
     pipeline['std_fft_ave_gfp'],
     test_frequencies=test_frequencies,
     delta_frequency=5 * u.Hz)
 pipeline.run()
 
-pipeline['fft_ave'].output_node.statistical_tests['hotelling_t2_freq'][[
-    "test_name", "df_1", "df_2", "f", "f_critic", "p_value"]].head()
+pipeline['fft_ave'].output_node.statistical_tests['hotelling_t2_freq'][
+    ["test_name", "df_1", "df_2", "f", "f_critic", "p_value"]].head()
 
 
 ht2 = pipeline['fft_ave'].output_node.statistical_tests['hotelling_t2_freq']
-print('\n HT2-Test \n'
+print('\nHT2-Test \n'
       'n = {:} \n'
       'detections = {:} \n'
       'Detection rate {:} %'.format(ht2.shape[0],
                                     np.sum(ht2["p_value"] < 0.05),
                                     np.round(100 * np.sum(ht2["p_value"] < 0.05) / ht2.shape[0],
                                              decimals=2)))
 
 f_test = pipeline['fft_ave_gfp_ftest'].output_node.statistical_tests['f_test_freq']
-print('\n F-Test \n'
+print('\nF-Test \n'
       'n = {:} \n'
       'detections = {:} \n'
       'Detection rate {:} %'.format(f_test.shape[0],
                                     np.sum(f_test["p_value"] < 0.05),
                                     np.round(100 * np.sum(f_test["p_value"] < 0.05) / f_test.shape[0],
                                              decimals=2)))
 # %%
@@ -211,15 +210,15 @@
 
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
     date='Today',
     experiment='sim')
 
 _parameters = {'Type': 'ASSR'}
-database_path = reader.input_node.paths.file_directory + os.sep + 'assr_dss_frequency_domain_test.sqlite'
+database_path = reader.input_node.paths.file_directory + os.sep + 'assr_dss_time_domain_test.sqlite'
 pipeline['database'] = SaveToDatabase(database_path=database_path,
                                       measurement_information=measurement_info,
                                       subject_information=subject_info,
                                       recording_information={'recording_device': 'dummy_device'},
                                       stimuli_information=_parameters,
                                       processes_list=[pipeline['fft_ave_gfp'],
                                                       pipeline['std_fft_ave_gfp'],
```

### Comparing `peegy-1.3.4/examples/example_assr_dss_time_domain_bias_test.py` & `peegy-1.3.6/examples/example_assr_ht2_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 """
-.. _tut-assr-ht2-test-dss-time-bias-sim:
+.. _tut-assr-ht2-test-sim:
 
 ##############################################
-ASSR using DSS in the time-domain (Simulated)
+ASSR Hotelling-T2 test (Simulated)
 ##############################################
 
-In this example we simulate a low-frequency ASSR, and we assess its significance using the Hotelling's T2 test and
-F-test.
-The background-noise is pink (controlled by noise attenuation = 3) and the presence of the signal is controlled by
-return_noise_only=False (if True, only the noise is returned).
-The signal is equal in all channels so that the detection rate obtained by keeping components can be assessed.
-The spatial filter is biased using the covariance obtained in the time-domain.
-This example shows that biasing in the frequency-domain requires only 1 component to keep the
-false detection rate at zero and true detection rate at 100%.
+In this example we simulate an ASSR, and we assess its significance using the Hotelling's T2 test.
+This method uses the real and imaginary part of the frequency bin of interest to assess whether the points from
+each epoch are significantly different from zero (the center of the polar complex-plane)
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
@@ -45,37 +40,37 @@
 # ===================
 # We generate some auditory steady-state response (ASSR)
 
 
 fs = 256.0 * u.Hz
 epoch_length = 4.0 * u.s
 epoch_length = np.ceil(epoch_length * fs) / fs  # fit to fs rate
-assr_frequency = np.array([6.75]) * u.Hz
+assr_frequency = np.array([41.0]) * u.Hz
 assr_frequency = np.ceil(epoch_length * assr_frequency) / epoch_length  # fit to epoch length
 
-join_frequencies = np.arange(1, 4) * assr_frequency
 # here we pick some random frequencies to test statistical detection
 random_frequencies = np.unique(np.random.rand(2)*5) * u.Hz
 
-test_frequencies = assr_frequency
+test_frequencies = np.concatenate((
+    assr_frequency,
+    2 * assr_frequency,
+    random_frequencies))
 
 template_waveform, _ = aep(fs=fs)
 n_channels = 32
 event_times = np.arange(0, 360.0, 1 / assr_frequency.to(u.Hz).value)
 reader = GenerateInputData(template_waveform=template_waveform,
                            fs=fs,
                            n_channels=n_channels,
-                           mixing_matrix=np.diag(np.ones(n_channels))/n_channels,
-                           snr=0.001,
+                           mixing_matrix=np.diag(np.arange(n_channels)) / n_channels,
+                           snr=0.05,
                            layout_file_name='biosemi32.lay',
                            event_times=event_times,
                            event_code=1.0,
-                           figures_subset_folder='assr_dss_time_domain_test',
-                           return_noise_only=True,
-                           noise_attenuation=3,
+                           figures_subset_folder='assr_ht2_test',
                            noise_seed=0)
 reader.run()
 
 # %%
 # Resize events
 # ===================
 # Now we keep events at intervals that correspond to our desired epoch length
@@ -88,16 +83,18 @@
 
 # %%
 # Start the pipeline
 # ===================
 # Some processing to obtain clean epochs
 
 pipeline = PipePool()
-
-pipeline['channel_cleaned'] = AutoRemoveBadChannels(reader)
+pipeline['referenced'] = ReferenceData(reader,
+                                       reference_channels=['Cz'],
+                                       invert_polarity=True)
+pipeline['channel_cleaned'] = AutoRemoveBadChannels(pipeline['referenced'])
 
 pipeline['time_filtered_data'] = FilterData(pipeline['channel_cleaned'],
                                             high_pass=2.0 * u.Hz,
                                             low_pass=100.0 * u.Hz)
 pipeline['time_epochs'] = EpochData(pipeline['time_filtered_data'],
                                     event_code=1.0,
                                     base_line_correction=False)
@@ -105,21 +102,18 @@
 
 # %%
 # Plot components in the frequency-domain
 # ---------------------------------------
 # Spatial filter is a applied in the frequency-domain
 
 pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
-                                                          test_frequencies=test_frequencies,
-                                                          sf_components=np.arange(1),
-                                                          projection_domain=Domain.frequency,
                                                           block_size=10,
                                                           return_figures=True,
-                                                          delta_frequency=2 * u.Hz,
-                                                          plot_y_lim=[0, 5])
+                                                          projection_domain=Domain.frequency,
+                                                          plot_y_lim=[0, 0.2])
 pipeline.run()
 
 # %%
 # Average epochs
 # ---------------------------------------
 # We compute the average and simultaneously get statistical tests on the test_frequencies
 
@@ -149,57 +143,40 @@
 pipeline['std_fft_ave_gfp'] = AppendGFPChannel(pipeline['std_fft_ave'])
 pipeline.run()
 
 pipeline['fft_ave_gfp_ftest'] = FTest(
     pipeline['fft_ave_gfp'],
     test_frequencies=test_frequencies,
     delta_frequency=5 * u.Hz)
-
+pipeline.run()
 pipeline['std_fft_ave_gfp_ftest'] = FTest(
     pipeline['std_fft_ave_gfp'],
     test_frequencies=test_frequencies,
     delta_frequency=5 * u.Hz)
 pipeline.run()
 
 pipeline['fft_ave'].output_node.statistical_tests['hotelling_t2_freq'][
     ["test_name", "df_1", "df_2", "f", "f_critic", "p_value"]].head()
+pipeline.run()
 
-
-ht2 = pipeline['fft_ave'].output_node.statistical_tests['hotelling_t2_freq']
-print('\nHT2-Test \n'
-      'n = {:} \n'
-      'detections = {:} \n'
-      'Detection rate {:} %'.format(ht2.shape[0],
-                                    np.sum(ht2["p_value"] < 0.05),
-                                    np.round(100 * np.sum(ht2["p_value"] < 0.05) / ht2.shape[0],
-                                             decimals=2)))
-
-f_test = pipeline['fft_ave_gfp_ftest'].output_node.statistical_tests['f_test_freq']
-print('\nF-Test \n'
-      'n = {:} \n'
-      'detections = {:} \n'
-      'Detection rate {:} %'.format(f_test.shape[0],
-                                    np.sum(f_test["p_value"] < 0.05),
-                                    np.round(100 * np.sum(f_test["p_value"] < 0.05) / f_test.shape[0],
-                                             decimals=2)))
 # %%
 # Generate figures
 # ---------------------------------------
 # Now we run plot the average waveforms and show the stats
 
 
 pipeline['waveform_plotter'] = PlotWaveforms(pipeline['fft_ave_gfp_ftest'],
                                              overlay=[pipeline['std_fft_ave_gfp_ftest']],
                                              plot_x_lim=[0, 90],
                                              ch_to_plot=np.array(['O2', 'T8', 'T7', 'GFP']),
                                              statistical_test='f_test_freq',
                                              show_following_stats=['f'],
                                              return_figures=True,
                                              user_naming_rule='standard_and_dss')
-
+pipeline.run()
 pipeline['topographic_map'] = PlotTopographicMap(pipeline['fft_ave'],
                                                  topographic_channels=np.array(['O2', 'T8', 'T7', 'GFP']),
                                                  plot_x_lim=[0, 90],
                                                  plot_y_lim=[0, 6],
                                                  return_figures=True)
 pipeline.run()
 
@@ -210,15 +187,15 @@
 
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
     date='Today',
     experiment='sim')
 
 _parameters = {'Type': 'ASSR'}
-database_path = reader.input_node.paths.file_directory + os.sep + 'assr_dss_time_domain_test.sqlite'
+database_path = reader.input_node.paths.file_directory + os.sep + 'assr_ht2_test.sqlite'
 pipeline['database'] = SaveToDatabase(database_path=database_path,
                                       measurement_information=measurement_info,
                                       subject_information=subject_info,
                                       recording_information={'recording_device': 'dummy_device'},
                                       stimuli_information=_parameters,
                                       processes_list=[pipeline['fft_ave_gfp'],
                                                       pipeline['std_fft_ave_gfp'],
```

### Comparing `peegy-1.3.4/examples/example_assr_f_test.py` & `peegy-1.3.6/examples/example_assr_f_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_assr_ht2_test.py` & `peegy-1.3.6/examples/example_assr_ht2_test_weighted_average.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """
-.. _tut-assr-ht2-test-sim:
+.. _tut-assr-ht2-test-weighted-average-sim:
 
-##############################################
-ASSR Hotelling-T2 test (Simulated)
-##############################################
+##################################################################
+ASSR Hotelling-T2 test using different average types (Simulated)
+##################################################################
 
 In this example we simulate an ASSR, and we assess its significance using the Hotelling's T2 test.
-This method uses the real and imaginary part of the frequency bin of interest to assess whether the points from
-each epoch are significantly different from zero (the center of the polar complex-plane)
+Several types of average are used to illustrate how EOG artefacts impact the different weighting methods.
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
 # if 'Qt5Agg' in matplotlib.rcsetup.all_backends:
 #     matplotlib.use('Qt5Agg')
 from peegy.processing.pipe.pipeline import PipePool
-from peegy.processing.pipe.definitions import Events, Domain
+from peegy.processing.pipe.definitions import Events
 from peegy.processing.pipe.general import ReferenceData, FilterData, AutoRemoveBadChannels
-from peegy.processing.pipe.epochs import AverageEpochsFrequencyDomain, AverageEpochs, EpochData
+from peegy.processing.pipe.epochs import AverageEpochsFrequencyDomain, EpochData
 from peegy.processing.pipe.attach import AppendGFPChannel
 from peegy.processing.pipe.statistics import FTest
-from peegy.processing.pipe.plot import PlotWaveforms, PlotTopographicMap
-from peegy.processing.pipe.spatial_filtering import CreateAndApplySpatialFilter
+from peegy.processing.pipe.plot import PlotWaveforms
 from peegy.processing.pipe.simulate import GenerateInputData
 from peegy.processing.tools.template_generator.auditory_waveforms import aep
 from peegy.processing.pipe.storage import MeasurementInformation, SubjectInformation, SaveToDatabase
 from peegy.io.storage.data_storage_reading_tools import sqlite_tables_to_pandas, sqlite_waveforms_to_pandas
 from peegy.io.storage.plot_tools import plot_time_frequency_responses, plot_topographic_maps
 import os
 import astropy.units as u
@@ -38,39 +36,34 @@
 # %%
 # Generate some data
 # ===================
 # We generate some auditory steady-state response (ASSR)
 
 
 fs = 256.0 * u.Hz
-epoch_length = 4.0 * u.s
+epoch_length = 1.0 * u.s
 epoch_length = np.ceil(epoch_length * fs) / fs  # fit to fs rate
-assr_frequency = np.array([41.0]) * u.Hz
+assr_frequency = np.array([6.0]) * u.Hz
 assr_frequency = np.ceil(epoch_length * assr_frequency) / epoch_length  # fit to epoch length
 
-# here we pick some random frequencies to test statistical detection
-random_frequencies = np.unique(np.random.rand(2)*5) * u.Hz
-
-test_frequencies = np.concatenate((
-    assr_frequency,
-    2 * assr_frequency,
-    random_frequencies))
+test_frequencies = assr_frequency
 
 template_waveform, _ = aep(fs=fs)
 n_channels = 32
 event_times = np.arange(0, 360.0, 1 / assr_frequency.to(u.Hz).value)
 reader = GenerateInputData(template_waveform=template_waveform,
                            fs=fs,
                            n_channels=n_channels,
                            mixing_matrix=np.diag(np.arange(n_channels)) / n_channels,
                            snr=0.05,
                            layout_file_name='biosemi32.lay',
                            event_times=event_times,
                            event_code=1.0,
-                           figures_subset_folder='assr_ht2_test',
+                           include_eog_events=True,
+                           figures_subset_folder='assr_ht2_test_weighted_average',
                            noise_seed=0)
 reader.run()
 
 # %%
 # Resize events
 # ===================
 # Now we keep events at intervals that correspond to our desired epoch length
@@ -89,121 +82,133 @@
 pipeline = PipePool()
 pipeline['referenced'] = ReferenceData(reader,
                                        reference_channels=['Cz'],
                                        invert_polarity=True)
 pipeline['channel_cleaned'] = AutoRemoveBadChannels(pipeline['referenced'])
 
 pipeline['time_filtered_data'] = FilterData(pipeline['channel_cleaned'],
-                                            high_pass=2.0 * u.Hz,
+                                            high_pass=0.5 * u.Hz,
                                             low_pass=100.0 * u.Hz)
 pipeline['time_epochs'] = EpochData(pipeline['time_filtered_data'],
                                     event_code=1.0,
                                     base_line_correction=False)
 pipeline.run()
 
 # %%
-# Plot components in the frequency-domain
+# Average epochs
 # ---------------------------------------
-# Spatial filter is a applied in the frequency-domain
+# We compute the average and simultaneously get statistical tests on the test_frequencies
 
-pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
-                                                          block_size=10,
-                                                          return_figures=True,
-                                                          projection_domain=Domain.frequency,
-                                                          plot_y_lim=[0, 0.2])
+pipeline['fft_ave_standard'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
+                                                            n_fft=int(epoch_length*fs),
+                                                            test_frequencies=test_frequencies,
+                                                            weighted_average=False,
+                                                            weighted_frequency_domain=False)
 pipeline.run()
 
-# %%
-# Average epochs
-# ---------------------------------------
-# We compute the average and simultaneously get statistical tests on the test_frequencies
+pipeline['fft_ave_frequency_weights_target_frequency'] = AverageEpochsFrequencyDomain(
+    pipeline['time_epochs'],
+    weighted_average=True,
+    weighted_frequency_domain=True,
+    n_fft=int(epoch_length*fs),
+    weight_frequencies=assr_frequency,
+    test_frequencies=test_frequencies,
+    delta_frequency=2 * u.Hz)
+pipeline.run()
 
+pipeline['fft_ave_time_weights_across'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
+                                                                       n_fft=int(epoch_length*fs),
+                                                                       weighted_average=True,
+                                                                       weighted_frequency_domain=False,
+                                                                       weight_across_epochs=True,
+                                                                       test_frequencies=test_frequencies)
+pipeline.run()
+
+pipeline['fft_ave_time_weights_within'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
+                                                                       n_fft=int(epoch_length*fs),
+                                                                       weighted_average=True,
+                                                                       weight_across_epochs=False,
+                                                                       weighted_frequency_domain=False,
+                                                                       test_frequencies=test_frequencies)
 
-pipeline['fft_ave'] = AverageEpochsFrequencyDomain(pipeline['dss_time_epochs'],
-                                                   n_fft=int(epoch_length*fs),
-                                                   weight_frequencies=assr_frequency,
-                                                   test_frequencies=test_frequencies,
-                                                   delta_frequency=2 * u.Hz)
-pipeline['time_ave'] = AverageEpochs(pipeline['dss_time_epochs'])
-
-pipeline['std_fft_ave'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
-                                                       n_fft=int(epoch_length * fs),
-                                                       weight_frequencies=assr_frequency,
-                                                       test_frequencies=test_frequencies,
-                                                       delta_frequency=2 * u.Hz)
 pipeline.run()
 
 # %%
 # Compute global field power (GFP)
 # ---------------------------------------
 # We compute the GFP across channels and epochs. A new channel with the GFP is appended to the data
 
-pipeline['fft_ave_gfp'] = AppendGFPChannel(pipeline['fft_ave'])
-pipeline.run()
+pipeline['fft_ave_frequency_weights_target_frequency_gfp'] = AppendGFPChannel(
+    pipeline['fft_ave_frequency_weights_target_frequency'])
+pipeline['fft_ave_standard_gfp'] = AppendGFPChannel(pipeline['fft_ave_standard'])
+pipeline['fft_ave_time_weights_across_gfp'] = AppendGFPChannel(pipeline['fft_ave_time_weights_across'])
+pipeline['fft_ave_time_weights_within_gfp'] = AppendGFPChannel(pipeline['fft_ave_time_weights_within'])
 
-pipeline['std_fft_ave_gfp'] = AppendGFPChannel(pipeline['std_fft_ave'])
 pipeline.run()
 
-pipeline['fft_ave_gfp_ftest'] = FTest(
-    pipeline['fft_ave_gfp'],
+pipeline['ftest_ave_freq_freq'] = FTest(
+    pipeline['fft_ave_frequency_weights_target_frequency_gfp'],
+    test_frequencies=test_frequencies,
+    delta_frequency=2 * u.Hz)
+pipeline.run()
+pipeline['ftest_ave_standard'] = FTest(
+    pipeline['fft_ave_standard_gfp'],
     test_frequencies=test_frequencies,
-    delta_frequency=5 * u.Hz)
+    delta_frequency=2 * u.Hz)
 pipeline.run()
-pipeline['std_fft_ave_gfp_ftest'] = FTest(
-    pipeline['std_fft_ave_gfp'],
+pipeline['ftest_ave_time_across'] = FTest(
+    pipeline['fft_ave_time_weights_across_gfp'],
     test_frequencies=test_frequencies,
-    delta_frequency=5 * u.Hz)
+    delta_frequency=2 * u.Hz)
 pipeline.run()
 
-pipeline['fft_ave'].output_node.statistical_tests['hotelling_t2_freq'][
-    ["test_name", "df_1", "df_2", "f", "f_critic", "p_value"]].head()
+pipeline['ftest_ave_time_within'] = FTest(
+    pipeline['fft_ave_time_weights_within_gfp'],
+    test_frequencies=test_frequencies,
+    delta_frequency=2 * u.Hz)
 pipeline.run()
 
+
 # %%
 # Generate figures
 # ---------------------------------------
 # Now we run plot the average waveforms and show the stats
 
 
-pipeline['waveform_plotter'] = PlotWaveforms(pipeline['fft_ave_gfp_ftest'],
-                                             overlay=[pipeline['std_fft_ave_gfp_ftest']],
-                                             plot_x_lim=[0, 90],
+pipeline['waveform_plotter'] = PlotWaveforms(pipeline['fft_ave_standard_gfp'],
+                                             overlay=[pipeline['fft_ave_frequency_weights_target_frequency_gfp'],
+                                                      pipeline['fft_ave_time_weights_across_gfp'],
+                                                      pipeline['fft_ave_time_weights_within_gfp']],
+                                             plot_x_lim=[0, 12],
                                              ch_to_plot=np.array(['O2', 'T8', 'T7', 'GFP']),
-                                             statistical_test='f_test_freq',
+                                             statistical_test='hotelling_t2_freq',
                                              show_following_stats=['f'],
-                                             return_figures=True,
-                                             user_naming_rule='standard_and_dss')
+                                             return_figures=True)
 pipeline.run()
-pipeline['topographic_map'] = PlotTopographicMap(pipeline['fft_ave'],
-                                                 topographic_channels=np.array(['O2', 'T8', 'T7', 'GFP']),
-                                                 plot_x_lim=[0, 90],
-                                                 plot_y_lim=[0, 6],
-                                                 return_figures=True)
-pipeline.run()
-
 # %%
 # Save results to a database
 # ---------------------------------------
 # We get the measurements we are interested in and save them into a database
 
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
     date='Today',
     experiment='sim')
 
 _parameters = {'Type': 'ASSR'}
-database_path = reader.input_node.paths.file_directory + os.sep + 'assr_ht2_test.sqlite'
+database_path = reader.input_node.paths.file_directory + os.sep + 'assr_ht2_test_weighted_average.sqlite'
 pipeline['database'] = SaveToDatabase(database_path=database_path,
                                       measurement_information=measurement_info,
                                       subject_information=subject_info,
                                       recording_information={'recording_device': 'dummy_device'},
                                       stimuli_information=_parameters,
-                                      processes_list=[pipeline['fft_ave_gfp'],
-                                                      pipeline['std_fft_ave_gfp'],
-                                                      pipeline['time_ave']],
+                                      processes_list=[pipeline['fft_ave_standard_gfp'],
+                                                      pipeline['fft_ave_frequency_weights_target_frequency_gfp'],
+                                                      pipeline['fft_ave_time_weights_across_gfp'],
+                                                      pipeline['fft_ave_time_weights_within_gfp']],
                                       include_waveforms=True
                                       )
 pipeline.run()
 
 # %%
 # Generate pipeline diagram
 # ------------------------------------
```

### Comparing `peegy-1.3.4/examples/example_assr_ht2_test_weighted_average.py` & `peegy-1.3.6/examples/example_assr_ht2_test_wrong_bias_frequnecy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,257 +1,195 @@
 """
-.. _tut-assr-ht2-test-weighted-average-sim:
+.. _tut-assr-ht2-test-sim-wrong-bias:
 
-##################################################################
-ASSR Hotelling-T2 test using different average types (Simulated)
-##################################################################
-
-In this example we simulate an ASSR, and we assess its significance using the Hotelling's T2 test.
-Several types of average are used to illustrate how EOG artefacts impact the different weighting methods.
+############################################################################################
+ASSR Hotelling-T2 test with spatial filtering biased with wrong frequencies(Simulated)
+############################################################################################
+
+In this example we simulate an ASSR and we assess its significance using the Hotelling's T2 test.
+However, we used DSS with a bias frequency which does not correspond to the ASSR frequency. This is a wrong bias and
+the example illustrates how this may significantly reduce the amplitude of the ASSR.
+This method uses the real and imaginary part of the frequency bin of interest to assess whether the points from
+each epoch are significantly different from zero (the center of the polar complex-plane).
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
 # if 'Qt5Agg' in matplotlib.rcsetup.all_backends:
-#     matplotlib.use('Qt5Agg')
+#    matplotlib.use('Qt5Agg')
 from peegy.processing.pipe.pipeline import PipePool
-from peegy.processing.pipe.definitions import Events
+from peegy.processing.pipe.definitions import Events, Domain
 from peegy.processing.pipe.general import ReferenceData, FilterData, AutoRemoveBadChannels
 from peegy.processing.pipe.epochs import AverageEpochsFrequencyDomain, EpochData
 from peegy.processing.pipe.attach import AppendGFPChannel
 from peegy.processing.pipe.statistics import FTest
-from peegy.processing.pipe.plot import PlotWaveforms
+from peegy.processing.pipe.plot import PlotWaveforms, PlotTopographicMap
+from peegy.processing.pipe.spatial_filtering import CreateAndApplySpatialFilter
 from peegy.processing.pipe.simulate import GenerateInputData
 from peegy.processing.tools.template_generator.auditory_waveforms import aep
 from peegy.processing.pipe.storage import MeasurementInformation, SubjectInformation, SaveToDatabase
-from peegy.io.storage.data_storage_reading_tools import sqlite_tables_to_pandas, sqlite_waveforms_to_pandas
-from peegy.io.storage.plot_tools import plot_time_frequency_responses, plot_topographic_maps
 import os
 import astropy.units as u
 import numpy as np
 
 
 # %%
 # Generate some data
 # ===================
 # We generate some auditory steady-state response (ASSR)
 
-
 fs = 256.0 * u.Hz
-epoch_length = 1.0 * u.s
+epoch_length = 4.0 * u.s
 epoch_length = np.ceil(epoch_length * fs) / fs  # fit to fs rate
-assr_frequency = np.array([6.0]) * u.Hz
+assr_frequency = np.array([41.0]) * u.Hz
 assr_frequency = np.ceil(epoch_length * assr_frequency) / epoch_length  # fit to epoch length
-
-test_frequencies = assr_frequency
-
+# we select several unrelated frequencies to the ASSR to bias the filter
+wrong_bias = np.array([13, 26, 39]) * u.Hz
+test_frequencies = np.concatenate((
+    assr_frequency,
+    2 * assr_frequency,
+    wrong_bias
+))
 template_waveform, _ = aep(fs=fs)
 n_channels = 32
-event_times = np.arange(0, 360.0, 1 / assr_frequency.to(u.Hz).value)
+event_times = np.arange(0, 360.0, 1 / assr_frequency.to(u.Hz).value) * u.s
 reader = GenerateInputData(template_waveform=template_waveform,
                            fs=fs,
                            n_channels=n_channels,
-                           mixing_matrix=np.diag(np.arange(n_channels)) / n_channels,
+                           mixing_matrix=np.diag(np.arange(n_channels))/n_channels,
                            snr=0.05,
                            layout_file_name='biosemi32.lay',
                            event_times=event_times,
                            event_code=1.0,
-                           include_eog_events=True,
-                           figures_subset_folder='assr_ht2_test_weighted_average',
-                           noise_seed=0)
+                           noise_attenuation=0,
+                           return_noise_only=False,
+                           figures_subset_folder='assr_ht2_test_wrong_bias')
 reader.run()
-
 # %%
 # Resize events
-# ===================
+# =======================
 # Now we keep events at intervals that correspond to our desired epoch length
 
 
 events = reader.output_node.events.get_events(code=1)
 # skip events to preserve only those at each epoch point
 _new_events = Events(events=events[0:-1:int(epoch_length * assr_frequency)])
 reader.output_node.events = _new_events
 
+
 # %%
 # Start the pipeline
-# ===================
+# ============================
 # Some processing to obtain clean epochs
 
+
 pipeline = PipePool()
 pipeline['referenced'] = ReferenceData(reader,
                                        reference_channels=['Cz'],
                                        invert_polarity=True)
 pipeline['channel_cleaned'] = AutoRemoveBadChannels(pipeline['referenced'])
-
 pipeline['time_filtered_data'] = FilterData(pipeline['channel_cleaned'],
-                                            high_pass=0.5 * u.Hz,
-                                            low_pass=100.0 * u.Hz)
+                                            high_pass=0.05 * u.Hz,
+                                            low_pass=None)
 pipeline['time_epochs'] = EpochData(pipeline['time_filtered_data'],
                                     event_code=1.0,
                                     base_line_correction=False)
 pipeline.run()
 
 # %%
-# Average epochs
-# ---------------------------------------
-# We compute the average and simultaneously get statistical tests on the test_frequencies
-
-pipeline['fft_ave_standard'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
-                                                            n_fft=int(epoch_length*fs),
-                                                            test_frequencies=test_frequencies,
-                                                            weighted_average=False,
-                                                            weighted_frequency_domain=False)
-pipeline.run()
-
-pipeline['fft_ave_frequency_weights_target_frequency'] = AverageEpochsFrequencyDomain(
-    pipeline['time_epochs'],
-    weighted_average=True,
-    weighted_frequency_domain=True,
-    n_fft=int(epoch_length*fs),
-    weight_frequencies=assr_frequency,
-    test_frequencies=test_frequencies,
-    delta_frequency=2 * u.Hz)
+# Compute and plot components in the frequency-domain
+# ----------------------------------------------------
+# Spatial filter is a applied in the frequency-domain
+
+pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
+                                                          sf_join_frequencies=wrong_bias,
+                                                          test_frequencies=test_frequencies,
+                                                          projection_domain=Domain.frequency,
+                                                          plot_y_lim=[0, 1],
+                                                          return_figures=True
+                                                          )
 pipeline.run()
 
-pipeline['fft_ave_time_weights_across'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
-                                                                       n_fft=int(epoch_length*fs),
-                                                                       weighted_average=True,
-                                                                       weighted_frequency_domain=False,
-                                                                       weight_across_epochs=True,
-                                                                       test_frequencies=test_frequencies)
-pipeline.run()
+# %%
+# Compute global field power (GFP)
+# ----------------------------------
+# We compute the GFP across channels and epochs. A new channel with the GFP is appended to the data
 
-pipeline['fft_ave_time_weights_within'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
-                                                                       n_fft=int(epoch_length*fs),
-                                                                       weighted_average=True,
-                                                                       weight_across_epochs=False,
-                                                                       weighted_frequency_domain=False,
-                                                                       test_frequencies=test_frequencies)
 
+pipeline['dss_time_epochs_with_gfp'] = AppendGFPChannel(pipeline['dss_time_epochs'])
 pipeline.run()
 
 # %%
-# Compute global field power (GFP)
-# ---------------------------------------
-# We compute the GFP across channels and epochs. A new channel with the GFP is appended to the data
+# Average epochs
+# ----------------------------------
+# We compute the average and simultaneously get statistical tests on the test_frequencies
 
-pipeline['fft_ave_frequency_weights_target_frequency_gfp'] = AppendGFPChannel(
-    pipeline['fft_ave_frequency_weights_target_frequency'])
-pipeline['fft_ave_standard_gfp'] = AppendGFPChannel(pipeline['fft_ave_standard'])
-pipeline['fft_ave_time_weights_across_gfp'] = AppendGFPChannel(pipeline['fft_ave_time_weights_across'])
-pipeline['fft_ave_time_weights_within_gfp'] = AppendGFPChannel(pipeline['fft_ave_time_weights_within'])
 
-pipeline.run()
+pipeline['fft_ave'] = AverageEpochsFrequencyDomain(pipeline['dss_time_epochs_with_gfp'],
+                                                   n_fft=int(epoch_length*fs),
+                                                   test_frequencies=test_frequencies)
 
-pipeline['ftest_ave_freq_freq'] = FTest(
-    pipeline['fft_ave_frequency_weights_target_frequency_gfp'],
-    test_frequencies=test_frequencies,
-    delta_frequency=2 * u.Hz)
-pipeline.run()
-pipeline['ftest_ave_standard'] = FTest(
-    pipeline['fft_ave_standard_gfp'],
-    test_frequencies=test_frequencies,
-    delta_frequency=2 * u.Hz)
-pipeline.run()
-pipeline['ftest_ave_time_across'] = FTest(
-    pipeline['fft_ave_time_weights_across_gfp'],
-    test_frequencies=test_frequencies,
-    delta_frequency=2 * u.Hz)
-pipeline.run()
+pipeline['fft_ave_f_test'] = FTest(pipeline['fft_ave'],
+                                   test_frequencies=test_frequencies,
+                                   delta_frequency=15 * u.Hz)
+
+pipeline['std_fft_ave'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
+                                                       n_fft=int(epoch_length * fs),
+                                                       test_frequencies=test_frequencies)
 
-pipeline['ftest_ave_time_within'] = FTest(
-    pipeline['fft_ave_time_weights_within_gfp'],
-    test_frequencies=test_frequencies,
-    delta_frequency=2 * u.Hz)
 pipeline.run()
 
+pipeline['fft_ave_f_test'].output_node.statistical_tests['f_test_freq'][
+    ["test_name", "df_1", "df_2", "f", "f_critic", "p_value"]].head()
 
 # %%
 # Generate figures
-# ---------------------------------------
+# ----------------------------------
 # Now we run plot the average waveforms and show the stats
 
 
-pipeline['waveform_plotter'] = PlotWaveforms(pipeline['fft_ave_standard_gfp'],
-                                             overlay=[pipeline['fft_ave_frequency_weights_target_frequency_gfp'],
-                                                      pipeline['fft_ave_time_weights_across_gfp'],
-                                                      pipeline['fft_ave_time_weights_within_gfp']],
-                                             plot_x_lim=[0, 12],
-                                             ch_to_plot=np.array(['O2', 'T8', 'T7', 'GFP']),
-                                             statistical_test='hotelling_t2_freq',
-                                             show_following_stats=['f'],
-                                             return_figures=True)
+pipeline['waveforms'] = PlotWaveforms(pipeline['std_fft_ave'],
+                                      overlay=[pipeline['fft_ave']],
+                                      plot_x_lim=[0, 90],
+                                      ch_to_plot=np.array(['O2', 'T8', 'T7']),
+                                      user_naming_rule='standard_and_dss',
+                                      statistical_test='hotelling_t2_freq',
+                                      show_following_stats=['test_name', 'f', 'frequency_tested'],
+                                      return_figures=True)
+
+pipeline['topographic_map'] = PlotTopographicMap(pipeline['fft_ave'],
+                                                 topographic_channels=np.array(['O2', 'T8', 'T7', 'GFP']),
+                                                 plot_x_lim=[0, 90],
+                                                 plot_y_lim=[0, 6],
+                                                 return_figures=True)
 pipeline.run()
 # %%
 # Save results to a database
-# ---------------------------------------
+# ----------------------------------
 # We get the measurements we are interested in and save them into a database
 
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
     date='Today',
     experiment='sim')
 
 _parameters = {'Type': 'ASSR'}
-database_path = reader.input_node.paths.file_directory + os.sep + 'assr_ht2_test_weighted_average.sqlite'
+database_path = reader.input_node.paths.file_directory + os.sep + 'assr_ht2_test_wrong_bias.sqlite'
 pipeline['database'] = SaveToDatabase(database_path=database_path,
                                       measurement_information=measurement_info,
                                       subject_information=subject_info,
                                       recording_information={'recording_device': 'dummy_device'},
                                       stimuli_information=_parameters,
-                                      processes_list=[pipeline['fft_ave_standard_gfp'],
-                                                      pipeline['fft_ave_frequency_weights_target_frequency_gfp'],
-                                                      pipeline['fft_ave_time_weights_across_gfp'],
-                                                      pipeline['fft_ave_time_weights_within_gfp']],
+                                      processes_list=[pipeline['fft_ave']],
                                       include_waveforms=True
                                       )
 pipeline.run()
 
 # %%
 # Generate pipeline diagram
 # ------------------------------------
 pipeline.diagram(file_name=reader.output_node.paths.figures_current_dir + 'pipeline.png',
                  return_figure=True,
                  dpi=600)
-
-
-# Read waveforms from generated database and plot them
-# ------------------------------------
-df_waves = sqlite_waveforms_to_pandas(database_path=database_path,
-                                      group_factors=['data_source', 'channel'],
-                                      channels=['T8', 'T7'])
-
-fig_out_1 = plot_time_frequency_responses(dataframe=df_waves,
-                                          rows_by='channel',
-                                          cols_by='data_source',
-                                          title_by='col',
-                                          blend_subcategories=True,
-                                          show_legend=True)
-
-fig_out_2 = plot_time_frequency_responses(dataframe=df_waves,
-                                          rows_by='channel',
-                                          cols_by='domain',
-                                          title_by='both',
-                                          blend_subcategories=False,
-                                          show_legend=True)
-
-fig_out_3 = plot_time_frequency_responses(dataframe=df_waves,
-                                          rows_by='channel',
-                                          cols_by='domain',
-                                          title_by='both',
-                                          blend_subcategories=True,
-                                          show_legend=True)
-
-df_ht2 = sqlite_tables_to_pandas(database_path=database_path,
-                                 tables=['hotelling_t2_freq'])['hotelling_t2_freq']
-
-# We show the topographic maps for the two Hotelling T2 (standard processing and denoise using dss)
-
-fig_out_4 = plot_topographic_maps(dataframe=df_ht2,
-                                  channels_column='channel',
-                                  rows_by='data_source',
-                                  layout='biosemi32.lay',
-                                  color_map_label='Amplitude [uV]',
-                                  topographic_value='mean_amplitude')
```

### Comparing `peegy-1.3.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py` & `peegy-1.3.6/examples/example_assr_no_layout.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,186 +1,149 @@
 """
-.. _tut-assr-ht2-test-sim-wrong-bias:
+.. _tut-assr-no-layout-test-sim:
 
-############################################################################################
-ASSR Hotelling-T2 test with spatial filtering biased with wrong frequencies(Simulated)
-############################################################################################
-
-In this example we simulate an ASSR and we assess its significance using the Hotelling's T2 test.
-However, we used DSS with a bias frequency which does not correspond to the ASSR frequency. This is a wrong bias and
-the example illustrates how this may significantly reduce the amplitude of the ASSR.
-This method uses the real and imaginary part of the frequency bin of interest to assess whether the points from
-each epoch are significantly different from zero (the center of the polar complex-plane).
+########################################################
+ASSR Without using a topographic layout (Simulated)
+########################################################
+
+In this example we simulate an ASSR recorded without any specific layout.
+The significance of the response is assessed using the Hotelling's T2 test.
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
 # if 'Qt5Agg' in matplotlib.rcsetup.all_backends:
 #    matplotlib.use('Qt5Agg')
 from peegy.processing.pipe.pipeline import PipePool
 from peegy.processing.pipe.definitions import Events, Domain
-from peegy.processing.pipe.general import ReferenceData, FilterData, AutoRemoveBadChannels
-from peegy.processing.pipe.epochs import AverageEpochsFrequencyDomain, EpochData
-from peegy.processing.pipe.attach import AppendGFPChannel
-from peegy.processing.pipe.statistics import FTest
-from peegy.processing.pipe.plot import PlotWaveforms, PlotTopographicMap
+from peegy.processing.pipe.general import ReferenceData, FilterData, AutoRemoveBadChannels, RegressOutEOG, ReSampling
+from peegy.processing.pipe.epochs import AverageEpochsFrequencyDomain, EpochData, AverageEpochs
+from peegy.processing.pipe.plot import PlotTopographicMap
 from peegy.processing.pipe.spatial_filtering import CreateAndApplySpatialFilter
 from peegy.processing.pipe.simulate import GenerateInputData
 from peegy.processing.tools.template_generator.auditory_waveforms import aep
 from peegy.processing.pipe.storage import MeasurementInformation, SubjectInformation, SaveToDatabase
 import os
 import astropy.units as u
 import numpy as np
 
-
 # %%
 # Generate some data
-# ===================
+# ==================================
 # We generate some auditory steady-state response (ASSR)
 
-fs = 256.0 * u.Hz
+
+fs = 512.0 * u.Hz
 epoch_length = 4.0 * u.s
 epoch_length = np.ceil(epoch_length * fs) / fs  # fit to fs rate
 assr_frequency = np.array([41.0]) * u.Hz
 assr_frequency = np.ceil(epoch_length * assr_frequency) / epoch_length  # fit to epoch length
-# we select several unrelated frequencies to the ASSR to bias the filter
-wrong_bias = np.array([13, 26, 39]) * u.Hz
-test_frequencies = np.concatenate((
-    assr_frequency,
-    2 * assr_frequency,
-    wrong_bias
-))
+# here we pick some random frequencies to test statistical detection
+random_frequencies = np.unique(np.random.rand(10)*30) * u.Hz
 template_waveform, _ = aep(fs=fs)
-n_channels = 32
-event_times = np.arange(0, 360.0, 1 / assr_frequency.to(u.Hz).value) * u.s
+n_channels = 8
+event_times = np.arange(0, 360.0, 1/assr_frequency.to(u.Hz).value) * u.s
 reader = GenerateInputData(template_waveform=template_waveform,
                            fs=fs,
                            n_channels=n_channels,
                            mixing_matrix=np.diag(np.arange(n_channels))/n_channels,
                            snr=0.05,
-                           layout_file_name='biosemi32.lay',
+                           include_eog_events=True,
                            event_times=event_times,
                            event_code=1.0,
-                           noise_attenuation=0,
-                           return_noise_only=False,
-                           figures_subset_folder='assr_ht2_test_wrong_bias')
+                           figures_subset_folder='assr_no_layout_test')
 reader.run()
 # %%
 # Resize events
-# =======================
+# ============================
 # Now we keep events at intervals that correspond to our desired epoch length
 
 
 events = reader.output_node.events.get_events(code=1)
 # skip events to preserve only those at each epoch point
 _new_events = Events(events=events[0:-1:int(epoch_length * assr_frequency)])
 reader.output_node.events = _new_events
 
-
 # %%
 # Start the pipeline
 # ============================
 # Some processing to obtain clean epochs
 
 
 pipeline = PipePool()
 pipeline['referenced'] = ReferenceData(reader,
-                                       reference_channels=['Cz'],
-                                       invert_polarity=True)
+                                       reference_channels=['CH_0'],
+                                       invert_polarity=False)
 pipeline['channel_cleaned'] = AutoRemoveBadChannels(pipeline['referenced'])
-pipeline['time_filtered_data'] = FilterData(pipeline['channel_cleaned'],
-                                            high_pass=0.05 * u.Hz,
-                                            low_pass=None)
+pipeline['eog_removed'] = RegressOutEOG(pipeline['channel_cleaned'],
+                                        ref_channel_labels=['EOG1'])
+pipeline['down_sampled'] = ReSampling(pipeline['eog_removed'],
+                                      new_sampling_rate=256. * u.Hz)
+pipeline['time_filtered_data'] = FilterData(pipeline['down_sampled'],
+                                            high_pass=2.0 * u.Hz,
+                                            low_pass=60.0 * u.Hz)
 pipeline['time_epochs'] = EpochData(pipeline['time_filtered_data'],
                                     event_code=1.0,
-                                    base_line_correction=False)
+                                    base_line_correction=False,
+                                    post_stimulus_interval=epoch_length)
 pipeline.run()
 
 # %%
 # Compute and plot components in the frequency-domain
-# ----------------------------------------------------
-# Spatial filter is a applied in the frequency-domain
+# ---------------------------------------------------
+# Spatial filter is applied in the frequency-domain
 
 pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
-                                                          sf_join_frequencies=wrong_bias,
-                                                          test_frequencies=test_frequencies,
                                                           projection_domain=Domain.frequency,
-                                                          plot_y_lim=[0, 1],
-                                                          return_figures=True
-                                                          )
-pipeline.run()
-
-# %%
-# Compute global field power (GFP)
-# ----------------------------------
-# We compute the GFP across channels and epochs. A new channel with the GFP is appended to the data
-
-
-pipeline['dss_time_epochs_with_gfp'] = AppendGFPChannel(pipeline['dss_time_epochs'])
+                                                          return_figures=True)
 pipeline.run()
 
 # %%
-# Average epochs
-# ----------------------------------
+# Average epochs in time- and frequency-domain
+# ----------------------------------------------
 # We compute the average and simultaneously get statistical tests on the test_frequencies
 
-
-pipeline['fft_ave'] = AverageEpochsFrequencyDomain(pipeline['dss_time_epochs_with_gfp'],
-                                                   n_fft=int(epoch_length*fs),
-                                                   test_frequencies=test_frequencies)
-
-pipeline['fft_ave_f_test'] = FTest(pipeline['fft_ave'],
-                                   test_frequencies=test_frequencies,
-                                   delta_frequency=15 * u.Hz)
-
-pipeline['std_fft_ave'] = AverageEpochsFrequencyDomain(pipeline['time_epochs'],
-                                                       n_fft=int(epoch_length * fs),
-                                                       test_frequencies=test_frequencies)
-
+pipeline['fft_ave'] = AverageEpochsFrequencyDomain(pipeline['dss_time_epochs'],
+                                                   test_frequencies=np.concatenate((
+                                                       assr_frequency, random_frequencies)))
+pipeline['time_ave'] = AverageEpochs(pipeline['dss_time_epochs'])
 pipeline.run()
 
-pipeline['fft_ave_f_test'].output_node.statistical_tests['f_test_freq'][
-    ["test_name", "df_1", "df_2", "f", "f_critic", "p_value"]].head()
-
 # %%
 # Generate figures
-# ----------------------------------
-# Now we run plot the average waveforms and show the stats
+# ------------------
+# Now we run plot the average waveforms
 
 
-pipeline['waveforms'] = PlotWaveforms(pipeline['std_fft_ave'],
-                                      overlay=[pipeline['fft_ave']],
-                                      plot_x_lim=[0, 90],
-                                      ch_to_plot=np.array(['O2', 'T8', 'T7']),
-                                      user_naming_rule='standard_and_dss',
-                                      statistical_test='hotelling_t2_freq',
-                                      show_following_stats=['test_name', 'f', 'frequency_tested'],
-                                      return_figures=True)
-
-pipeline['topographic_map'] = PlotTopographicMap(pipeline['fft_ave'],
-                                                 topographic_channels=np.array(['O2', 'T8', 'T7', 'GFP']),
-                                                 plot_x_lim=[0, 90],
-                                                 plot_y_lim=[0, 6],
-                                                 return_figures=True)
+pipeline['topographic_map_1'] = PlotTopographicMap(pipeline['fft_ave'],
+                                                   plot_x_lim=[0, 60],
+                                                   plot_y_lim=[0, 6],
+                                                   return_figures=True)
+pipeline['topographic_map_2'] = PlotTopographicMap(pipeline['time_ave'],
+                                                   times=np.concatenate(([0], 1 / assr_frequency.to(u.Hz).value)),
+                                                   plot_x_lim=[0, epoch_length.to(u.s).value],
+                                                   plot_y_lim=[-6, 6],
+                                                   return_figures=True)
 pipeline.run()
+
 # %%
 # Save results to a database
-# ----------------------------------
+# ---------------------------
 # We get the measurements we are interested in and save them into a database
 
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
     date='Today',
     experiment='sim')
 
 _parameters = {'Type': 'ASSR'}
-database_path = reader.input_node.paths.file_directory + os.sep + 'assr_ht2_test_wrong_bias.sqlite'
+database_path = reader.input_node.paths.file_directory + os.sep + 'assr_no_layout_test_data.sqlite'
 pipeline['database'] = SaveToDatabase(database_path=database_path,
                                       measurement_information=measurement_info,
                                       subject_information=subject_info,
                                       recording_information={'recording_device': 'dummy_device'},
                                       stimuli_information=_parameters,
                                       processes_list=[pipeline['fft_ave']],
                                       include_waveforms=True
```

### Comparing `peegy-1.3.4/examples/example_assr_no_layout.py` & `peegy-1.3.6/examples/example_using_own_raw_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,158 +1,176 @@
 """
-.. _tut-assr-no-layout-test-sim:
+.. _tut-assr-using-own-raw-data-sim:
 
-########################################################
-ASSR Without using a topographic layout (Simulated)
-########################################################
-
-In this example we simulate an ASSR recorded without any specific layout.
-The significance of the response is assessed using the Hotelling's T2 test.
+#######################################################################
+ASSR F-Test Example using 'external' data (time x channels) (Simulated)
+#######################################################################
+
+This example shows how you can pass any data to the pipeline (e.g. matlab data, or text file data) in the shape of time
+x channels alongside with event times used to epoch the data.
+In this example we simulate an ASSR (as it was read from an external file), and we investigate the significance of
+the response by means of an F-test that compares the variance of the frequency of interest with the variance of
+neighbouring frequency bins.
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
 # if 'Qt5Agg' in matplotlib.rcsetup.all_backends:
 #    matplotlib.use('Qt5Agg')
 from peegy.processing.pipe.pipeline import PipePool
-from peegy.processing.pipe.definitions import Events, Domain
-from peegy.processing.pipe.general import ReferenceData, FilterData, AutoRemoveBadChannels, RegressOutEOG, ReSampling
-from peegy.processing.pipe.epochs import AverageEpochsFrequencyDomain, EpochData, AverageEpochs
-from peegy.processing.pipe.plot import PlotTopographicMap
+from peegy.processing.pipe.definitions import Domain
+from peegy.processing.pipe.io import GenericInputData
+from peegy.processing.pipe.statistics import FTest
+from peegy.processing.pipe.general import FilterData
+from peegy.processing.pipe.epochs import AverageEpochs, EpochData
+from peegy.processing.pipe.plot import PlotWaveforms, PlotTopographicMap
 from peegy.processing.pipe.spatial_filtering import CreateAndApplySpatialFilter
-from peegy.processing.pipe.simulate import GenerateInputData
-from peegy.processing.tools.template_generator.auditory_waveforms import aep
 from peegy.processing.pipe.storage import MeasurementInformation, SubjectInformation, SaveToDatabase
 import os
 import astropy.units as u
 import numpy as np
 
 # %%
-# Generate some data
-# ==================================
-# We generate some auditory steady-state response (ASSR)
+# Generate some data (time x channels) and add event times
+# ==========================================================
+# We generate some data in this example, for the sake of exemplify it. The data is put into GenericInputData class and
+# then used in a standard pipeline
 
 
-fs = 512.0 * u.Hz
+fs = 256.0 * u.Hz
 epoch_length = 4.0 * u.s
 epoch_length = np.ceil(epoch_length * fs) / fs  # fit to fs rate
 assr_frequency = np.array([41.0]) * u.Hz
 assr_frequency = np.ceil(epoch_length * assr_frequency) / epoch_length  # fit to epoch length
-# here we pick some random frequencies to test statistical detection
-random_frequencies = np.unique(np.random.rand(10)*30) * u.Hz
-template_waveform, _ = aep(fs=fs)
-n_channels = 8
-event_times = np.arange(0, 360.0, 1/assr_frequency.to(u.Hz).value) * u.s
-reader = GenerateInputData(template_waveform=template_waveform,
-                           fs=fs,
-                           n_channels=n_channels,
-                           mixing_matrix=np.diag(np.arange(n_channels))/n_channels,
-                           snr=0.05,
-                           include_eog_events=True,
-                           event_times=event_times,
-                           event_code=1.0,
-                           figures_subset_folder='assr_no_layout_test')
+# here we generate and pass our own data
+n_epochs = 20
+time = np.arange(0, epoch_length.to(u.s).value * n_epochs, 1 / fs.to(u.Hz).value) * u.s
+my_sin = np.sin(2 * np.pi * u.rad * assr_frequency * time)
+template_waveform = np.array([my_sin, 0.5 * my_sin, 0.25 * my_sin]).T
+# add some noise
+np.random.seed(1)
+template_waveform = template_waveform + np.random.randn(*template_waveform.shape)
+event_times = np.arange(0, n_epochs) * epoch_length
+reader = GenericInputData(data=template_waveform,
+                          fs=fs,
+                          event_times=event_times,
+                          event_code=1.0,
+                          figures_subset_folder='my_own_raw_assr_f_test')
 reader.run()
 # %%
-# Resize events
-# ============================
-# Now we keep events at intervals that correspond to our desired epoch length
+# Start the pipeline
+# ==========================================================
 
 
-events = reader.output_node.events.get_events(code=1)
-# skip events to preserve only those at each epoch point
-_new_events = Events(events=events[0:-1:int(epoch_length * assr_frequency)])
-reader.output_node.events = _new_events
+pipeline = PipePool()
+pipeline['time_filtered_data'] = FilterData(reader,
+                                            high_pass=2.0 * u.Hz,
+                                            low_pass=100.0 * u.Hz)
+pipeline.run()
 
 # %%
-# Start the pipeline
-# ============================
-# Some processing to obtain clean epochs
+# Get Epochs
+# -----------------------------------------
+# We partition the data into epochs or trials based on the event code used.
 
 
-pipeline = PipePool()
-pipeline['referenced'] = ReferenceData(reader,
-                                       reference_channels=['CH_0'],
-                                       invert_polarity=False)
-pipeline['channel_cleaned'] = AutoRemoveBadChannels(pipeline['referenced'])
-pipeline['eog_removed'] = RegressOutEOG(pipeline['channel_cleaned'],
-                                        ref_channel_labels=['EOG1'])
-pipeline['down_sampled'] = ReSampling(pipeline['eog_removed'],
-                                      new_sampling_rate=256. * u.Hz)
-pipeline['time_filtered_data'] = FilterData(pipeline['down_sampled'],
-                                            high_pass=2.0 * u.Hz,
-                                            low_pass=60.0 * u.Hz)
 pipeline['time_epochs'] = EpochData(pipeline['time_filtered_data'],
                                     event_code=1.0,
-                                    base_line_correction=False,
-                                    post_stimulus_interval=epoch_length)
+                                    base_line_correction=False)
 pipeline.run()
 
 # %%
-# Compute and plot components in the frequency-domain
-# ---------------------------------------------------
-# Spatial filter is applied in the frequency-domain
+# Get DSS components and clean data
+# -----------------------------------------
+# Compute spatial filter of time epochs
+
 
 pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
-                                                          projection_domain=Domain.frequency,
-                                                          return_figures=True)
+                                                          test_frequencies=np.array([assr_frequency,
+                                                                                     2 * assr_frequency]),
+                                                          components_to_plot=np.arange(0, 5),
+                                                          projection_domain=Domain.frequency)
 pipeline.run()
 
 # %%
-# Average epochs in time- and frequency-domain
-# ----------------------------------------------
-# We compute the average and simultaneously get statistical tests on the test_frequencies
+# Compute average responses
+# -----------------------------------------
+# We compute weighted average on epochs with and without spatial filtering (DSS)
 
-pipeline['fft_ave'] = AverageEpochsFrequencyDomain(pipeline['dss_time_epochs'],
-                                                   test_frequencies=np.concatenate((
-                                                       assr_frequency, random_frequencies)))
-pipeline['time_ave'] = AverageEpochs(pipeline['dss_time_epochs'])
+pipeline['time_ave_dss'] = AverageEpochs(pipeline['dss_time_epochs'])
+pipeline['time_ave'] = AverageEpochs(pipeline['time_epochs'])
 pipeline.run()
 
 # %%
-# Generate figures
-# ------------------
-# Now we run plot the average waveforms
-
-
-pipeline['topographic_map_1'] = PlotTopographicMap(pipeline['fft_ave'],
-                                                   plot_x_lim=[0, 60],
-                                                   plot_y_lim=[0, 6],
-                                                   return_figures=True)
-pipeline['topographic_map_2'] = PlotTopographicMap(pipeline['time_ave'],
-                                                   times=np.concatenate(([0], 1 / assr_frequency.to(u.Hz).value)),
-                                                   plot_x_lim=[0, epoch_length.to(u.s).value],
-                                                   plot_y_lim=[-6, 6],
-                                                   return_figures=True)
+# Run F-Test
+# -----------------------------------------
+# Now we run an F-test to determine if frequency component is significant
+
+
+pipeline['fft_ave_f_tests_dss'] = FTest(pipeline['time_ave_dss'],
+                                        n_fft=int(epoch_length*fs*1),
+                                        test_frequencies=assr_frequency,
+                                        delta_frequency=9.0 * u.Hz)
+pipeline['fft_ave_f_tests'] = FTest(pipeline['time_ave'],
+                                    n_fft=int(epoch_length * fs * 1),
+                                    test_frequencies=assr_frequency,
+                                    delta_frequency=9. * u.Hz)
+
+# %%
+# Show some waveforms
+# -----------------------------------------
+
+pipeline['topographic_map_1'] = PlotTopographicMap(pipeline['fft_ave_f_tests_dss'],
+                                                   plot_x_lim=[0, 90],
+                                                   plot_y_lim=[0, 4],
+                                                   topographic_channels=np.array(['CH_0', 'CH_1', 'CH_2']),
+                                                   return_figures=True,
+                                                   user_naming_rule='dss')
+
+pipeline['topographic_map_2'] = PlotTopographicMap(pipeline['fft_ave_f_tests'],
+                                                   plot_x_lim=[0, 90],
+                                                   plot_y_lim=[0, 4],
+                                                   topographic_channels=np.array(['CH_0', 'CH_1', 'CH_2']),
+                                                   return_figures=True,
+                                                   user_naming_rule='standard')
+
+pipeline['plotter'] = PlotWaveforms(pipeline['fft_ave_f_tests'],
+                                    ch_to_plot=np.array(['CH_0']),
+                                    overlay=[pipeline['fft_ave_f_tests_dss']],
+                                    plot_x_lim=[0, 90],
+                                    show_following_stats=['frequency_tested', 'f'],
+                                    return_figures=True,
+                                    user_naming_rule='waveforms',
+                                    fig_format='.png')
 pipeline.run()
 
 # %%
-# Save results to a database
-# ---------------------------
+# Get generated data and save to database
+# -----------------------------------------
 # We get the measurements we are interested in and save them into a database
 
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
     date='Today',
     experiment='sim')
-
 _parameters = {'Type': 'ASSR'}
-database_path = reader.input_node.paths.file_directory + os.sep + 'assr_no_layout_test_data.sqlite'
+database_path = reader.input_node.paths.file_directory + os.sep + 'assr_own_raw_data_f_test_data.sqlite'
 pipeline['database'] = SaveToDatabase(database_path=database_path,
                                       measurement_information=measurement_info,
                                       subject_information=subject_info,
                                       recording_information={'recording_device': 'dummy_device'},
                                       stimuli_information=_parameters,
-                                      processes_list=[pipeline['fft_ave']],
+                                      processes_list=[pipeline['fft_ave_f_tests'],
+                                                      pipeline['fft_ave_f_tests_dss']],
                                       include_waveforms=True
                                       )
 pipeline.run()
 
 # %%
 # Generate pipeline diagram
-# ------------------------------------
+# -----------------------------------------
 pipeline.diagram(file_name=reader.output_node.paths.figures_current_dir + 'pipeline.png',
                  return_figure=True,
                  dpi=600)
```

### Comparing `peegy-1.3.4/examples/example_assr_phase_locking_value_test.py` & `peegy-1.3.6/examples/example_assr_phase_locking_value_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_ffr_artifact_removal.py` & `peegy-1.3.6/examples/example_ffr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_using_own_data_trials.py` & `peegy-1.3.6/examples/example_using_own_data_trials.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/examples/example_using_own_raw_data.py` & `peegy-1.3.6/examples/example_acc_peak_detection_bootstrap.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,176 +1,189 @@
 """
-.. _tut-assr-using-own-raw-data-sim:
+.. _tut-acc-standard-pipeline-sim:
 
-#######################################################################
-ASSR F-Test Example using 'external' data (time x channels) (Simulated)
-#######################################################################
-
-This example shows how you can pass any data to the pipeline (e.g. matlab data, or text file data) in the shape of time
-x channels alongside with event times used to epoch the data.
-In this example we simulate an ASSR (as it was read from an external file), and we investigate the significance of
-the response by means of an F-test that compares the variance of the frequency of interest with the variance of
-neighbouring frequency bins.
+##################################
+ACC Standard analysis (Simulated)
+##################################
+
+In this example we simulate an ACC response and detect the peaks using n standard pipeline.
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
 # if 'Qt5Agg' in matplotlib.rcsetup.all_backends:
 #    matplotlib.use('Qt5Agg')
 from peegy.processing.pipe.pipeline import PipePool
-from peegy.processing.pipe.definitions import Domain
-from peegy.processing.pipe.io import GenericInputData
-from peegy.processing.pipe.statistics import FTest
-from peegy.processing.pipe.general import FilterData
-from peegy.processing.pipe.epochs import AverageEpochs, EpochData
-from peegy.processing.pipe.plot import PlotWaveforms, PlotTopographicMap
+from peegy.processing.pipe.simulate import GenerateInputData
+from peegy.processing.tools.detection.definitions import TimePeakWindow, PeakToPeakMeasure, TimeROI
+from peegy.processing.tools.template_generator.auditory_waveforms import aep
+from peegy.processing.pipe.bootstrap.bootstrap import Bootstrap, BootstrapTarget
+from peegy.processing.pipe.general import FilterData, ReSampling, AutoRemoveBadChannels, ReferenceData, RegressOutEOG, \
+    BaselineCorrection
+from peegy.processing.pipe.epochs import EpochData, AverageEpochs
 from peegy.processing.pipe.spatial_filtering import CreateAndApplySpatialFilter
+from peegy.processing.pipe.statistics import HotellingT2Test
+from peegy.processing.pipe.detection import PeakDetectionTimeDomain
+from peegy.processing.pipe.plot import PlotWaveforms, PlotTopographicMap
+from peegy.processing.pipe.attach import AppendGFPChannel
 from peegy.processing.pipe.storage import MeasurementInformation, SubjectInformation, SaveToDatabase
 import os
-import astropy.units as u
 import numpy as np
+import astropy.units as u
 
 # %%
-# Generate some data (time x channels) and add event times
-# ==========================================================
-# We generate some data in this example, for the sake of exemplify it. The data is put into GenericInputData class and
-# then used in a standard pipeline
-
-
-fs = 256.0 * u.Hz
-epoch_length = 4.0 * u.s
-epoch_length = np.ceil(epoch_length * fs) / fs  # fit to fs rate
-assr_frequency = np.array([41.0]) * u.Hz
-assr_frequency = np.ceil(epoch_length * assr_frequency) / epoch_length  # fit to epoch length
-# here we generate and pass our own data
-n_epochs = 20
-time = np.arange(0, epoch_length.to(u.s).value * n_epochs, 1 / fs.to(u.Hz).value) * u.s
-my_sin = np.sin(2 * np.pi * u.rad * assr_frequency * time)
-template_waveform = np.array([my_sin, 0.5 * my_sin, 0.25 * my_sin]).T
-# add some noise
-np.random.seed(1)
-template_waveform = template_waveform + np.random.randn(*template_waveform.shape)
-event_times = np.arange(0, n_epochs) * epoch_length
-reader = GenericInputData(data=template_waveform,
-                          fs=fs,
-                          event_times=event_times,
-                          event_code=1.0,
-                          figures_subset_folder='my_own_raw_assr_f_test')
+# Time windows
+# ============================
+# Time windows are used to define where to look for different peaks
+
+
+tw = np.array([TimePeakWindow(ini_time=50 * u.ms, end_ref='N1', label='P1', positive_peak=True,
+                              exclude_channels=['GFP']),
+               TimePeakWindow(ini_time=80 * u.ms, end_time=200 * u.ms, label='N1', positive_peak=False,
+                              exclude_channels=['GFP']),
+               TimePeakWindow(ini_ref='N1', end_time=300 * u.ms, label='P2', positive_peak=True,
+                              exclude_channels=['GFP']),
+               TimePeakWindow(ini_time=50 * u.ms, end_time=150 * u.ms, label='gfp1', positive_peak=True,
+                              target_channels=['GFP']),
+               TimePeakWindow(ini_time=150 * u.ms, end_time=500 * u.ms, label='gfp2', positive_peak=True,
+                              target_channels=['GFP'])])
+
+# %%
+# Peak-to-peak Measures
+# ============================
+# Peak-to-peak measures are defined based on the labels of the TimePeaks defined above.
+
+
+pm = np.array([PeakToPeakMeasure(ini_peak='N1', end_peak='P2')])
+
+# %%
+# Time regions of interest
+# ============================
+# TimeROI are defined as time regions where different measures will be performed, e.g. SNR measure or statistical
+# measures
+
+
+roi_windows = np.array(
+    [TimeROI(ini_time=100.0 * u.ms, end_time=300.0 * u.ms, measure="snr", label="acc_snr"),
+     TimeROI(ini_time=500.0 * u.ms, end_time=700.0 * u.ms, measure="snr", label="control")])
+
+# %%
+# Generate some data
+# ===================
+# First we generate some ACC data
+
+n_channels=32
+fs = 512.0 * u.Hz
+template_waveform, _ = aep(fs=fs)
+event_times = np.arange(0, 100.0, 1.0) * u.s
+reader = GenerateInputData(template_waveform=template_waveform,
+                           fs=fs,
+                           n_channels=n_channels,
+                           mixing_matrix=np.diag(np.arange(n_channels))/n_channels,
+                           layout_file_name='biosemi32.lay',
+                           snr=0.1,
+                           event_times=event_times,
+                           event_code=1.0,
+                           figures_subset_folder='acc_test',
+                           include_eog_events=True,
+                           )
 reader.run()
+
 # %%
 # Start the pipeline
-# ==========================================================
+# ============================
+# Now we proceed with our basic processing pipeline
 
 
 pipeline = PipePool()
-pipeline['time_filtered_data'] = FilterData(reader,
-                                            high_pass=2.0 * u.Hz,
-                                            low_pass=100.0 * u.Hz)
+pipeline['referenced'] = ReferenceData(reader,
+                                       reference_channels=['Cz'],
+                                       invert_polarity=True)
+pipeline['channel_cleaned'] = AutoRemoveBadChannels(pipeline.referenced)
+pipeline['down_sampled'] = ReSampling(pipeline.channel_cleaned,
+                                      new_sampling_rate=256. * u.Hz)
+pipeline['eog_removed'] = RegressOutEOG(pipeline.down_sampled,
+                                        ref_channel_labels=['EOG1'])
 pipeline.run()
-
 # %%
-# Get Epochs
-# -----------------------------------------
-# We partition the data into epochs or trials based on the event code used.
-
+# Show EOG removal Output
+# ------------------------------------
 
-pipeline['time_epochs'] = EpochData(pipeline['time_filtered_data'],
-                                    event_code=1.0,
-                                    base_line_correction=False)
-pipeline.run()
+pipeline.eog_removed.plot(plot_input=True,
+                          plot_output=True,
+                          ch_to_plot=['CP1', 'CP5', 'P7'],
+                          interactive=False)
 
 # %%
-# Get DSS components and clean data
-# -----------------------------------------
-# Compute spatial filter of time epochs
-
+# Continue with the pipeline
+# ------------------------------------
 
-pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
-                                                          test_frequencies=np.array([assr_frequency,
-                                                                                     2 * assr_frequency]),
-                                                          components_to_plot=np.arange(0, 5),
-                                                          projection_domain=Domain.frequency)
-pipeline.run()
-
-# %%
-# Compute average responses
-# -----------------------------------------
-# We compute weighted average on epochs with and without spatial filtering (DSS)
+pipeline['time_filtered_data'] = FilterData(pipeline.eog_removed,
+                                            high_pass=2.0 * u.Hz,
+                                            low_pass=30.0 * u.Hz)
 
-pipeline['time_ave_dss'] = AverageEpochs(pipeline['dss_time_epochs'])
-pipeline['time_ave'] = AverageEpochs(pipeline['time_epochs'])
 pipeline.run()
 
 # %%
-# Run F-Test
-# -----------------------------------------
-# Now we run an F-test to determine if frequency component is significant
-
-
-pipeline['fft_ave_f_tests_dss'] = FTest(pipeline['time_ave_dss'],
-                                        n_fft=int(epoch_length*fs*1),
-                                        test_frequencies=assr_frequency,
-                                        delta_frequency=9.0 * u.Hz)
-pipeline['fft_ave_f_tests'] = FTest(pipeline['time_ave'],
-                                    n_fft=int(epoch_length * fs * 1),
-                                    test_frequencies=assr_frequency,
-                                    delta_frequency=9. * u.Hz)
-
-# %%
-# Show some waveforms
-# -----------------------------------------
-
-pipeline['topographic_map_1'] = PlotTopographicMap(pipeline['fft_ave_f_tests_dss'],
-                                                   plot_x_lim=[0, 90],
-                                                   plot_y_lim=[0, 4],
-                                                   topographic_channels=np.array(['CH_0', 'CH_1', 'CH_2']),
-                                                   return_figures=True,
-                                                   user_naming_rule='dss')
-
-pipeline['topographic_map_2'] = PlotTopographicMap(pipeline['fft_ave_f_tests'],
-                                                   plot_x_lim=[0, 90],
-                                                   plot_y_lim=[0, 4],
-                                                   topographic_channels=np.array(['CH_0', 'CH_1', 'CH_2']),
-                                                   return_figures=True,
-                                                   user_naming_rule='standard')
-
-pipeline['plotter'] = PlotWaveforms(pipeline['fft_ave_f_tests'],
-                                    ch_to_plot=np.array(['CH_0']),
-                                    overlay=[pipeline['fft_ave_f_tests_dss']],
-                                    plot_x_lim=[0, 90],
-                                    show_following_stats=['frequency_tested', 'f'],
-                                    return_figures=True,
-                                    user_naming_rule='waveforms',
-                                    fig_format='.png')
+# Bootstrapping
+# ------------------------------------
+# We generate a new pipeline indicating what would be bootstrapped
+pipeline_bootstrap = PipePool()
+
+pipeline_bootstrap['time_epochs'] = EpochData(pipeline['time_filtered_data'],
+                                              event_code=1.0,
+                                              post_stimulus_interval=1 * u.s)
+pipeline_bootstrap['time_epochs_dss'] = CreateAndApplySpatialFilter(input_process=pipeline_bootstrap['time_epochs'],
+                                                                    plot_projections=False,
+                                                                    components_to_plot=None,
+                                                                    plot_power=False)
+pipeline_bootstrap['time_epochs_with_baseline_corrected'] = BaselineCorrection(
+    pipeline_bootstrap['time_epochs_dss'],
+    ini_time=0 * u.ms,
+    end_time=20 * u.ms)
+pipeline_bootstrap['ht2'] = HotellingT2Test(pipeline_bootstrap['time_epochs_with_baseline_corrected'],
+                                            roi_windows=roi_windows)
+pipeline_bootstrap['ftest'] = AverageEpochs(pipeline_bootstrap['time_epochs_with_baseline_corrected'],
+                                            roi_windows=roi_windows,
+                                            weighted_average=False)
+
+# bootstrap the pipe
+pipeline['bootstrap'] = Bootstrap(at_each_bootstrap_do=pipeline_bootstrap,
+                                  n_bootstraps=100,
+                                  event_code=1.0,
+                                  bootstrap_targets=[
+                                      BootstrapTarget(
+                                          table_name='hotelling_t2_time',
+                                          group_by=['channel', 'label', 'ini_time', 'end_time'],
+                                          target_values=['f']),
+                                      BootstrapTarget(
+                                          table_name='f_test_time',
+                                          group_by=['channel', 'label', 'ini_time', 'end_time'],
+                                          target_values=['f'])])
 pipeline.run()
 
-# %%
-# Get generated data and save to database
-# -----------------------------------------
-# We get the measurements we are interested in and save them into a database
-
+# now we save our data to a database
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
     date='Today',
     experiment='sim')
-_parameters = {'Type': 'ASSR'}
-database_path = reader.input_node.paths.file_directory + os.sep + 'assr_own_raw_data_f_test_data.sqlite'
+
+_parameters = {'Type': 'ACC'}
+database_path = reader.input_node.paths.file_directory + os.sep + 'acc_test_bootstrap_data.sqlite'
 pipeline['database'] = SaveToDatabase(database_path=database_path,
                                       measurement_information=measurement_info,
                                       subject_information=subject_info,
                                       recording_information={'recording_device': 'dummy_device'},
                                       stimuli_information=_parameters,
-                                      processes_list=[pipeline['fft_ave_f_tests'],
-                                                      pipeline['fft_ave_f_tests_dss']],
-                                      include_waveforms=True
+                                      processes_list=[pipeline['bootstrap']]
                                       )
 pipeline.run()
 
 # %%
 # Generate pipeline diagram
-# -----------------------------------------
+# ------------------------------------
 pipeline.diagram(file_name=reader.output_node.paths.figures_current_dir + 'pipeline.png',
                  return_figure=True,
                  dpi=600)
```

### Comparing `peegy-1.3.4/peegy/definitions/channel_definitions.py` & `peegy-1.3.6/peegy/definitions/channel_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/definitions/edf_bdf_reader.py` & `peegy-1.3.6/peegy/definitions/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/definitions/eegReaderAbstractClasses.py` & `peegy-1.3.6/peegy/definitions/eegReaderAbstractClasses.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/definitions/eeg_definitions.py` & `peegy-1.3.6/peegy/definitions/eeg_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/definitions/events.py` & `peegy-1.3.6/peegy/definitions/events.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/definitions/tables.py` & `peegy-1.3.6/peegy/definitions/tables.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/directories/tools.py` & `peegy-1.3.6/peegy/directories/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/edf_bdf_reader.py` & `peegy-1.3.6/peegy/io/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/eeg/reader.py` & `peegy-1.3.6/peegy/io/eeg/reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py` & `peegy-1.3.6/peegy/io/external_tools/aep_gui/aep_matlab_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/external_tools/aep_gui/dataReadingTools.py` & `peegy-1.3.6/peegy/io/external_tools/aep_gui/dataReadingTools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/external_tools/aep_gui/extsys_tools.py` & `peegy-1.3.6/peegy/io/external_tools/aep_gui/extsys_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py` & `peegy-1.3.6/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/external_tools/file_tools.py` & `peegy-1.3.6/peegy/io/external_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/generic_csv_reader.py` & `peegy-1.3.6/peegy/io/generic_csv_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/storage/data_storage_reading_tools.py` & `peegy-1.3.6/peegy/io/storage/data_storage_reading_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/storage/data_storage_tools.py` & `peegy-1.3.6/peegy/io/storage/data_storage_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/storage/plot_tools.py` & `peegy-1.3.6/peegy/io/storage/plot_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,16 @@
                                   time_vmarkers: np.array = None,
                                   freq_vmarkers: np.array = None,
                                   freq_vmarkers_style: str = None,
                                   show_individual_waveforms: bool = True,
                                   individual_waveforms_alpha: float = 0.1,
                                   show_sem: bool = True,
                                   sem_alpha: float = 0.2,
+                                  show_sd: bool = True,
+                                  sd_alpha: float = 0.2,
                                   show_legend: bool = True,
                                   title_by: str = 'row',
                                   title_v_offset: float = 0.0,
                                   ylabel: str = None,
                                   y_unit_to: u.Unit = None,
                                   x_unit_to: u.Unit = None,
                                   fontsize: float = 6,
@@ -55,14 +57,16 @@
     :param freq_ylim: y axis limis for the frequency-domain panels
     :param time_vmarkers: array with x values to add a vertical marker in the time-domain panels
     :param freq_vmarkers: array with x values to add a vertical marker in the frequency-domain panels
     :param show_individual_waveforms: if true, individual waveforms will be shown.
     :param individual_waveforms_alpha: value between 0 and 1 indicating the alpha level of individual waveforms
     :param show_sem: if true, the standard error of the mean will be shown
     :param sem_alpha: value between 0 and 1 indicating the alpha level of the sem
+    :param show_sd: if true, the standard deviation of the mean will be shown
+    :param sd_alpha: value between 0 and 1 indicating the alpha level of the standard deviation
     :param show_legend: if True, the legend for any other category present in the dataframe will be shown
     :param title_by: string specifying from which factor you want to show the titles in each panel. This can be: "row",
     "col", or "both"
     :param title_v_offset: float specifying the vertical offset of the title
     :param freq_vmarkers_style: style of the marker in the frequency-domain. If not passed, vertical lines are used.
     :param ylabel: Label to put in the vertical axis. If empty, the Amplitude and unit of it are used.
     :param y_unit_to: Specify the units in which the vertical axis will be displayed
@@ -104,15 +108,16 @@
     groups = df.groupby(_rows_and_cols)
     fig_out, ax = plt.subplots(n_rows, n_cols)
     gs = gridspec.GridSpec(n_rows, n_cols)
     for _id, ((_current_row_group, _current_col_group), _group) in enumerate(groups):
         _current_group = _group
         if blend_subcategories:
             _current_group = _group.iloc[[0]].copy().reset_index()
-            _current_group['y'] = _current_group['y'].apply(lambda x: np.vstack(_group.y).T)
+            if _current_group['y'].shape[0] > 1:
+                _current_group['y'] = _current_group['y'].apply(lambda x: np.vstack(_group.y).T)
         _idx_row = idx_rows[_current_row_group == row_conditions].squeeze()
         _idx_col = idx_cols[_current_col_group == col_conditions].squeeze()
         _columns_legends = []
         _colors = plt.cm.get_cmap('viridis', _current_group.shape[0])
         _y_unit_to = y_unit_to
         _x_unit_to = x_unit_to
         for _col in _current_group:
@@ -143,17 +148,18 @@
 
             if _domain == 'time' and sub_average_time_buffer_size is not None:
                 fs = 1 / np.mean(np.diff(x))
                 used_samples = int(np.floor(y.shape[0] // sub_average_time_buffer_size) * sub_average_time_buffer_size)
                 y_f = y[0: used_samples, :]
                 y_f = np.transpose(np.reshape(y_f, (sub_average_time_buffer_size, -1, y_f.shape[1]), order='F'),
                                    [0, 2, 1])
+                # demean
                 y_f = np.mean(y_f, axis=2)
                 x = np.arange(0, sub_average_time_buffer_size) / fs
-                y_single_responses = y_f
+                y_single_responses = y_f - np.mean(y_f, axis=0)
 
             ax = plt.subplot(gs[_idx_row, _idx_col])
             title = ''
             if title_by == 'row':
                 title = '{:}'.format(_current_row_group)
 
             if title_by == 'col':
@@ -166,43 +172,52 @@
                 if _idx_row == 0:
                     ax.set_title(title, y=1 + title_v_offset, size=fontsize)
             else:
                 ax.set_title(title, y=1 + title_v_offset, size=fontsize)
 
             if _domain == 'time':
                 y_mean = np.mean(y_single_responses, axis=1)
-                y_sem = np.std(y_single_responses, axis=1) / np.sqrt(y_single_responses.shape[1])
+                y_sd = np.std(y_single_responses, axis=1)
+                y_sem = y_sd / np.sqrt(y_single_responses.shape[1])
                 if show_individual_waveforms:
                     ax.plot(x, y_single_responses,
-                            linewidth=1.0,
+                            linewidth=0.5,
                             alpha=individual_waveforms_alpha,
                             color=_colors(_i)
                             )
             if _domain == 'frequency':
                 y_mean = np.mean(np.abs(y_single_responses), axis=1)
-                y_sem = np.std(np.abs(y_single_responses), axis=1) / np.sqrt(y_single_responses.shape[1])
+                y_sd = np.std(np.abs(y_single_responses), axis=1)
+                y_sem = y_sd / np.sqrt(y_single_responses.shape[1])
                 if show_individual_waveforms:
                     ax.plot(x, np.abs(y_single_responses),
-                            linewidth=1.0,
+                            linewidth=0.5,
                             alpha=individual_waveforms_alpha,
                             color=_colors(_i))
 
             ax.plot(x, y_mean,
                     color=_colors(_i),
-                    linewidth=1.5,
+                    linewidth=0.8,
                     label=_group_label)
             if ylabel is None:
                 ax.set_ylabel('Amplitude [{:}]'.format(y_mean.unit), size=fontsize)
             if show_sem:
                 ax.fill_between(x.value,
                                 (y_mean - y_sem).value,
                                 (y_mean + y_sem).value,
                                 alpha=sem_alpha,
                                 edgecolor="none",
                                 facecolor=_colors(_i))
+            if show_sd:
+                ax.fill_between(x.value,
+                                (y_mean - y_sd).value,
+                                (y_mean + y_sd).value,
+                                alpha=sd_alpha,
+                                edgecolor="none",
+                                facecolor=_colors(_i))
             if _idx_col == n_cols - 1:
                 ax_row_label = ax.twinx()
                 ax_row_label.set_ylabel(_current_row_group, size=fontsize)
                 ax_row_label.set_yticklabels([])
                 ax_row_label.tick_params(
                     axis='y',  # changes apply to the x-axis
                     which='both',  # both major and minor ticks are affected
@@ -266,46 +281,66 @@
     return fig_out
 
 
 def plot_topographic_maps(dataframe: pd.DataFrame = None,
                           rows_by: str = None,
                           cols_by: str = None,
                           subject_id_column: str = 'subject_id',
+                          normalize_by: str = 'subject_id',
                           channels_column: str = 'channel',
                           title: str = '',
-                          topographic_value: float = None,
+                          topographic_value: str = None,
                           layout: str = None,
                           title_by: str = 'row',
                           title_v_offset: float = 0.0,
+                          fontsize: float = 6,
                           grid_size: np.complex = 600j,
                           color_map_label: str = None,
                           normalize: bool = False,
-                          show_sensors: bool = True
+                          show_sensors: bool = True,
+                          show_sensor_label: bool = False,
+                          n_contour_levels: int = 35,
+                          max_topographic_value: float = None,
+                          min_topographic_value: float = None,
+                          contour_line_width: float = 0.1,
+                          apply_function: object = lambda x: np.mean(x, axis=2),
+                          fun_args: dict = {}
                           ) -> plt.figure:
     """
     This function will plot the waveforms contained in a pandas dataframe read using the sqlite_waveforms_to_pandas
     function of pEEGy.
     The rows and columns of the output plot are specified by the factors of the dataframe.
-    The output will show the data for each of those factors (both individual and average data).
-    :param dataframe: a pandas dataframe returned by sqlite_waveforms_to_pandas function of pEEGy.
-    :param rows_by: name of the factor in the dataframe for which the rows in the plot will be split.
-    :param cols_by: name of the factor in the dataframe for which the columns in the plot will be split.
+    The output will show the data for each of those factors (both individual and average data)
+    :param dataframe: a pandas dataframe returned by sqlite_waveforms_to_pandas function of pEEGy
+    :param rows_by: name of the factor in the dataframe for which the rows in the plot will be split
+    :param cols_by: name of the factor in the dataframe for which the columns in the plot will be split
     :param subject_id_column: string indicating the column name with subject ids
+    :param normalize_by: string indicating the column that will be used to normalized the data
     :param channels_column: name of column containing channel labels
     :param title: title of the figure
     :param topographic_value: name of column containing the value to be shown by the topographic map
     :param layout: path or name of the layout to be used
     :param title_by: string specifying from which factor you want to show the titles in each panel. This can be: "row",
     "col", or "both"
     :param title_v_offset: float specifying the vertical offset of the title
+    :param fontsize: the fontsize
     :param grid_size: complex number indicating the size of the grid,
     :param color_map_label: string with the label that would be use of the colourmap. If empty, the default value will
     be the topographic_value
-    :param normalize: if True, topographic maps will be normalized within subject
-    :param show_sensors: if True, the positin of the sensors will be shown
+    :param normalize: if True, topographic maps will be normalized within normalize_by
+    :param show_sensors: if True, the position of the sensors will be shown
+    :param show_sensor_label: if True, the label of the sensor will be shown
+    :param n_contour_levels: number of contour lines to plot
+    :param min_topographic_value: if given, the colour scale will be restricted to have this value as maximum, otherwise
+    it will be determined from the data.
+    :param max_topographic_value: if given, the colour scale will be restricted to have this value as minimum, otherwise
+    it will be determined from the data.
+    :param contour_line_width: float indicating the with (in points) of the contour lines
+    :param apply_function: function to be applied to each subgroup
+    :param fun_args: extra arguments to be used by apply_function. This is a dictionary with the desired parameters
     :return:
     """
     df = copy.copy(dataframe)
     _rows_and_cols = []
     row_conditions = np.array([1])
     col_conditions = np.array([1])
     if rows_by is not None:
@@ -324,54 +359,68 @@
         n_cols = col_conditions.size
     else:
         df.loc[:, 'dummy_col'] = 1
         _rows_and_cols.append('dummy_col')
         n_cols = 1
     idx_cols = np.arange(col_conditions.size)
 
-    df['topo_value'] = df[topographic_value]
-    if normalize:
-        df = df.assign(
-            topo_value=df.groupby(
-                [subject_id_column])[topographic_value].transform(lambda x: x / np.max(x)))
-    if len(_rows_and_cols):
-        sub_groups = df.groupby(_rows_and_cols).apply(
-            lambda x: get_topographic_maps(x,
-                                           subject_id_column=subject_id_column,
-                                           layout=layout,
-                                           channels_column=channels_column,
-                                           topographic_value='topo_value',
-                                           grid_size=grid_size))
-    else:
-        _potentials = get_topographic_maps(df,
-                                           subject_id_column=subject_id_column,
-                                           layout=layout,
-                                           channels_column=channels_column,
-                                           topographic_value='topo_value',
-                                           grid_size=grid_size)
-        df['potentials'] = _potentials
+    if not len(_rows_and_cols):
         df['dummy_row'] = 1
         df['dummy_col'] = 1
         _rows_and_cols = ['dummy_row', 'dummy_col']
+    # check if input dataframe already contains the potentials. If not, then we extract them
+    if 'potentials' in df.keys():
+        if normalize:
+            if normalize_by is not None:
+                df = df.assign(
+                    potentials=df.groupby(
+                        normalize_by)['potentials'].transform(
+                        lambda x: x / np.ma.max(np.abs(np.ma.dstack([_val for _val in x])))))
+            else:
+                df = df.assign(
+                    potentials=df.groupby(
+                        [True] * len(df))['potentials'].transform(
+                        lambda x: x / np.ma.max(np.abs(np.ma.dstack([_val for _val in x])))))
         sub_groups = df
+    else:
+        df['topo_value'] = df[topographic_value]
+        if normalize:
+            df = df.assign(
+                topo_value=df.groupby(
+                    [normalize_by])[topographic_value].transform(lambda x: x / np.max(np.abs(x))))
+        sub_groups = get_topographic_maps_as_df(dataframe=df,
+                                                subject_id_column=subject_id_column,
+                                                group_by=_rows_and_cols,
+                                                channels_column='channel',
+                                                topographic_value='topo_value',
+                                                layout=layout,
+                                                apply_function=apply_function,
+                                                fun_args=fun_args
+                                                )
+
     if color_map_label is None:
         color_map_label = topographic_value
 
     groups = sub_groups.groupby(_rows_and_cols)
     fig_out = plt.figure(constrained_layout=True)
     widths = [1.0] * n_cols
     heights = [1.0] * n_rows
     heights.append(0.1)
     gs = fig_out.add_gridspec(ncols=n_cols, nrows=n_rows + 1,
                               width_ratios=widths,
                               height_ratios=heights)
-    max_sub = sub_groups.potentials.apply(
-        lambda x: np.ma.mean(x, axis=2) if isinstance(x, np.ndarray) else np.nan).apply(np.max).max()
-    min_sub = sub_groups.potentials.apply(
-        lambda x: np.ma.mean(x, axis=2) if isinstance(x, np.ndarray) else np.nan).apply(np.min).min()
+    if max_topographic_value is None:
+        max_sub = sub_groups.potentials.apply(lambda x: np.ma.dstack([_val for _val in x]).max()).max()
+    else:
+        max_sub = max_topographic_value
+
+    if min_topographic_value is None:
+        min_sub = sub_groups.potentials.apply(lambda x: np.ma.dstack([_val for _val in x]).min()).min()
+    else:
+        min_sub = min_topographic_value
     max_distance = sub_groups.max_distance.max()
 
     for _id, ((_current_row_group, _current_col_group), _group) in enumerate(groups):
         if _group.shape[0] == 0 or np.all(np.isnan(_group.potentials.values[0])):
             continue
         _idx_row = idx_rows[_current_row_group == row_conditions].squeeze()
         _idx_col = idx_cols[_current_col_group == col_conditions].squeeze()
@@ -381,53 +430,61 @@
             panel_title = '{:}'.format(_current_row_group)
         if title_by == 'col':
             panel_title = '{:}'.format(_current_col_group)
 
         if title_by == 'both':
             panel_title = '{:} / {:}'.format(_current_row_group, _current_col_group)
 
-        ax.set_title(panel_title, y=1 + title_v_offset, size=8)
-        std_average = np.ma.mean(_group.potentials.values[0], axis=2)
+        ax.set_title(panel_title, y=1 + title_v_offset, size=fontsize)
+        # std_average = np.ma.mean(_group.potentials.values[0], axis=2)
+        if _group.potentials.values.size > 1:
+            std_average = _group.potentials.apply(
+                lambda x: apply_function(np.ma.dstack([_val for _val in x]), *fun_args)).values[0]
+        else:
+            std_average = _group.potentials.values[0]
         ax_im = ax.imshow(std_average.T, origin='lower',
                           extent=(-max_distance, max_distance, -max_distance, max_distance),
                           vmin=min_sub,
                           vmax=max_sub,
                           aspect=1.0)
         ax_im.set_cmap('nipy_spectral')
 
-        levels = np.arange(0, max_sub, max_sub / 5.0)
+        levels = np.linspace(min_sub, max_sub, n_contour_levels)
         ax.contour(std_average.T,
                    levels,
                    origin='lower',
                    extent=(-max_distance, max_distance, -max_distance, max_distance),
-                   linewidths=1.0,
-                   colors='k')
+                   linewidths=contour_line_width,
+                   colors='k',
+                   linestyles='solid')
         ax.autoscale(enable=False)
         # plot color bar
 
         if _id == 0:
             c_bar_ax = plt.subplot(gs[-1, :])
             c_bar = fig_out.colorbar(ax_im, cax=c_bar_ax, orientation='horizontal', format='%.1f')
-            c_bar.set_label(color_map_label, fontsize=8)
+            c_bar.set_label(color_map_label, fontsize=fontsize)
             tick_locator = ticker.MaxNLocator(nbins=3)
             c_bar.locator = tick_locator
             c_bar.update_ticks()
-            c_bar.ax.tick_params(labelsize=8)
+            c_bar.ax.tick_params(labelsize=fontsize)
         channels = _group.channels.values[0]
         channel_labels = [ch['label'] for ch in channels]
         ax.plot(0, max_distance * 1.0, '|', markersize=8, color='k')
         if show_sensors:
             _lay = Layout()
             _layout = _lay.get_layout(file_name=layout)
             _layout = np.array([_l for _l in _layout if _l.label not in ['COMNT', 'SCALE']])
             for i, lay in enumerate(_layout):
                 if lay.label in channel_labels:
                     ax.plot(lay.x, lay.y, 'o', color='b', markersize=0.2)
                 else:
-                    ax.plot(lay.x, lay.y, 'o', color='b', markersize=0.2)
+                    ax.plot(lay.x, lay.y, 'o', color='grey', markersize=0.2)
+                if show_sensor_label:
+                    ax.text(lay.x, lay.y, s=lay.label, fontsize=6)
         ax.set_xticks([])
         ax.set_yticks([])
         ax.axis('off')
 
     all_axes = fig_out.get_axes()
     for ax in all_axes:
         if ax == c_bar.ax:
@@ -444,15 +501,17 @@
 
 
 def get_topographic_maps(df,
                          subject_id_column: str = 'subject_id',
                          channels_column: str = 'channel',
                          topographic_value: str = None,
                          layout: str = None,
-                         grid_size: np.complex = 600j):
+                         grid_size: np.complex = 600j,
+                         apply_function: object = None,
+                         fun_args: dict = {}):
     _lay = Layout()
     _layout = _lay.get_layout(file_name=layout)
     _layout = np.array([_l for _l in _layout if _l.label not in ['COMNT', 'SCALE']])
     _single_responses = np.array([])
 
     _subject_groups = df.groupby(subject_id_column)
     for _, (_id_sub, _sub_group) in enumerate(_subject_groups):
@@ -476,11 +535,52 @@
                                                                        z=np.array(z).reshape(-1, 1),
                                                                        grid=grid_size)
         max_potential
         if not _single_responses.size:
             _single_responses = _potentials[:, :, None]
         else:
             _single_responses = np.ma.dstack((_single_responses, _potentials))
+    if apply_function is not None:
+        _single_responses = apply_function(_single_responses, **fun_args)
     out = pd.Series(data={'potentials': _single_responses,
                           'max_distance': max_distance,
                           'channels': channels})
     return out
+
+
+def get_topographic_maps_as_df(dataframe: pd.DataFrame = None,
+                               group_by: [str] = None,
+                               subject_id_column: str = 'subject_id',
+                               channels_column: str = 'channel',
+                               topographic_value: str = None,
+                               layout: str = None,
+                               grid_size: np.complex = 600j,
+                               apply_function: object = np.mean,
+                               fun_args: dict = {}
+                               ) -> pd.DataFrame:
+    """
+    This function will plot the waveforms contained in a pandas dataframe read using the sqlite_waveforms_to_pandas
+    function of pEEGy.
+    The rows and columns of the output plot are specified by the factors of the dataframe.
+    The output will show the data for each of those factors (both individual and average data).
+    :param dataframe: a pandas dataframe returned by sqlite_waveforms_to_pandas function of pEEGy.
+    :param group_by: name of factors to group and obtain potentials.
+    :param subject_id_column: string indicating the column name with subject ids
+    :param channels_column: name of column containing channel labels
+    :param topographic_value: name of column containing the value to be shown by the topographic map
+    :param layout: path or name of the layout to be used
+    :param grid_size: complex number indicating the size of the grid,
+    :return:
+    """
+    df = copy.copy(dataframe)
+    df['topo_value'] = df[topographic_value]
+    group_by = [True] * len(df) if group_by is None else group_by
+    sub_groups = df.groupby(group_by, group_keys=False).apply(
+        lambda x: get_topographic_maps(x,
+                                       subject_id_column=subject_id_column,
+                                       layout=layout,
+                                       channels_column=channels_column,
+                                       topographic_value='topo_value',
+                                       grid_size=grid_size,
+                                       apply_function=apply_function,
+                                       fun_args=fun_args)).reset_index()
+    return sub_groups
```

### Comparing `peegy-1.3.4/peegy/io/synergy_reader.py` & `peegy-1.3.6/peegy/io/synergy_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/io/xml_tools.py` & `peegy-1.3.6/peegy/io/xml_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/KIT-160.lay` & `peegy-1.3.6/peegy/layouts/KIT-160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi128.lay` & `peegy-1.3.6/peegy/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi16.lay` & `peegy-1.3.6/peegy/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi160.lay` & `peegy-1.3.6/peegy/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi256.lay` & `peegy-1.3.6/peegy/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi32.lay` & `peegy-1.3.6/peegy/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi32_2_EXT.lay` & `peegy-1.3.6/peegy/layouts/biosemi32_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi32_fnirs_MP.lay` & `peegy-1.3.6/peegy/layouts/biosemi32_fnirs_MP.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi32_fnirs_jaime.lay` & `peegy-1.3.6/peegy/layouts/biosemi32_fnirs_jaime.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi64.lay` & `peegy-1.3.6/peegy/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi64_2_EXT.lay` & `peegy-1.3.6/peegy/layouts/biosemi64_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/biosemi64_3_EXT.lay` & `peegy-1.3.6/peegy/layouts/biosemi64_3_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/emotive14.lay` & `peegy-1.3.6/peegy/layouts/emotive14.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/layouts/layouts.py` & `peegy-1.3.6/peegy/layouts/layouts.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,14 @@
     def plot_layout(self):
         fig_out = plt.figure(constrained_layout=True)
         widths = [1.0]
         heights = [1.0]
         gs = fig_out.add_gridspec(ncols=1, nrows=1, width_ratios=widths,
                                   height_ratios=heights)
         inch = 2.54
-        fig_out.subplots_adjust(wspace=0.0, hspace=0.0)
+        # fig_out.subplots_adjust(wspace=0.0, hspace=0.0)
         fig_out.set_size_inches(20.0 / inch, 20.0 / inch)
         ax = plt.subplot(gs[0, 0])
         for i, lay in enumerate(self.layout):
             ax.plot(lay.x, lay.y, 'o', color='b', markersize=1)
             ax.text(lay.x, lay.y, lay.label)
         return fig_out
```

### Comparing `peegy-1.3.4/peegy/layouts/neuroscan64.lay` & `peegy-1.3.6/peegy/layouts/neuroscan64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/plot/eeg_ave_epochs_plot_tools.py` & `peegy-1.3.6/peegy/plot/eeg_ave_epochs_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/plot/eeg_plot_tools.py` & `peegy-1.3.6/peegy/plot/eeg_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/events/event_tools.py` & `peegy-1.3.6/peegy/processing/events/event_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/attach.py` & `peegy-1.3.6/peegy/processing/pipe/attach.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/definitions.py` & `peegy-1.3.6/peegy/processing/pipe/definitions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 
 from peegy.definitions.channel_definitions import Domain, ChannelItem, ChannelType
 from peegy.definitions import tables
 from peegy.directories.tools import DirectoryPaths
-from peegy.definitions.events import Events
+from peegy.definitions.events import Events, SingleEvent
 from peegy.tools.units.unit_tools import set_default_unit
 import inspect
 import pandas as pd
 import io
 import gc
 import astropy.units as u
 import itertools
@@ -57,16 +57,16 @@
                  ):
         # n * m * t data array
         # if data represent time or frequency
         # time offset from origin
         # layout
         # list used to store processing history that resulted in the current data
 
+        self._data = set_default_unit(data, u.dimensionless_unscaled)
         self.fs = fs
-        self._data = data
         self.domain = domain
         self.x_offset = x_offset
         self.layout = layout
         self.events = events
         self.events_annotations = events_annotations
         self.process_history = process_history
         self.paths = paths
@@ -76,22 +76,21 @@
         self.snr = snr
         self.cum_snr = cum_snr
         self.s_var = s_var
         self.n = n
         self.rn_df = rn_df
         self.w = w
         self.alpha = alpha
+        # statistical data
         self._statistical_tests = tables.Tables()
         # other processing tables
         self._processing_tables_global = processing_tables_global
         self._processing_tables_local = tables.Tables()
         # peak measures
         self.peaks = peaks
-        # self.peak_frequency = peak_frequency
-        # self.peak_to_peak_amplitudes = peak_to_peak_amplitudes
         self.peak_time_windows = peak_time_windows
         self.roi_windows = roi_windows
         self.markers = markers
         self.n_fft = n_fft
         if self.layout is None and data.size:
             self.layout = np.array([ChannelItem() for _ in range(self.data.shape[1])])  # default channel information
         self._x = None
@@ -258,14 +257,65 @@
                                               end_time.to(u.s).value]) * u.s)
         _extact_time_offset = self.x[samples[0]]
         self._data = self._data[samples[0]: samples[-1], ::]
         self.events.clip(ini_time=ini_time, end_time=end_time)
         # apply offset
         self.events.set_offset(time_offset=_extact_time_offset)
 
+    def randomize_events(self, epoch_length: u.Quantity = None,
+                         n_events: int = None,
+                         event_code: float = 1,
+                         dur: u.Quantity = 100 * u.us,
+                         min_time: u.Quantity = None,
+                         max_time: u.Quantity = None):
+        """
+        Generate random time events.
+        :param epoch_length: Time of epoch length. This value will only affect the maximum timing of the random events
+        so that when the data is epoched with the desired epoch length the last event position will not be beyond the
+        total timing of the data minus the epoch length. In this way ensuring that all random event will be used when
+        epoching the data.
+        :param n_events: Number of random events to be generated. If empty the original event number is used
+        :param event_code: float with the event code that will be used to generate/assign new random events
+        :param dur: time duration that will be assigned to the new random events
+        :param min_time: minimum time of new events
+        :param max_time: maximum time of new events
+        :return: None
+        """
+        # generate random events based on original number of events or given number of events
+        _n_events = None
+        _min_time, _max_time = None, None
+        if self.events.get_events_code(code=event_code).size:
+            _n_events = self.events.get_events_code(code=event_code).size
+            _min_time = self.events.get_events_time(code=event_code).min()
+            _max_time = self.events.get_events_time(code=event_code).max()
+        if n_events is None:
+            n_events = _n_events
+        if min_time:
+            _min_time = min_time
+
+        if max_time is not None:
+            _max_time = max_time
+
+        if not _min_time:
+            _min_time = 0 * u.s
+        if not _max_time:
+            _max_time = self._data.shape[0] / self.fs
+
+        if n_events:
+            if epoch_length is None:
+                epoch_length = ((_max_time - _min_time) / n_events)
+            new_event_times = np.sort(
+                _min_time + np.random.rand(n_events) * (_max_time - _min_time - epoch_length))
+            events = np.array([])
+            for _s, in zip(new_event_times):
+                events = np.append(events, SingleEvent(code=event_code,
+                                                       time_pos=_s,
+                                                       dur=dur))
+            self.events = Events(events=np.array(events))
+
 
 class InputOutputQtFigure(object):
     """
     This class is a wrapper to allow sphinx showing qt figures
     """
     def __init__(self, figure: pg.GraphicsView = None):
         self.figure = figure
```

### Comparing `peegy-1.3.4/peegy/processing/pipe/detection.py` & `peegy-1.3.6/peegy/processing/pipe/detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,7 +28,8 @@
         self.output_node.peaks = _data_pd
         self.output_node.processing_tables_local = Tables(table_name='peaks_time',
                                                           data=_data_pd,
                                                           data_source=self.name)
         self.output_node.processing_tables_local.append(Tables(table_name='amplitudes',
                                                                data=_amps_pd,
                                                                data_source=self.name))
+        self.output_node.statistical_tests = self.input_process.output_node.statistical_tests
```

### Comparing `peegy-1.3.4/peegy/processing/pipe/epochs.py` & `peegy-1.3.6/peegy/processing/pipe/epochs.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         # ensure sufficient data for baseline-correction
         if baseline_correction_ini_time < 0:
             pre_stimulus_interval = np.maximum(pre_stimulus_interval, np.abs(baseline_correction_ini_time))
         if baseline_correction_end_time > 0:
             post_stimulus_interval = np.maximum(post_stimulus_interval, baseline_correction_end_time)
 
         buffer_size = np.int((post_stimulus_interval + pre_stimulus_interval) * self.input_node.fs)
-        events_index = events_index - int((pre_stimulus_interval + self.input_node.x_offset) * self.input_node.fs)
+        events_index = events_index - int((pre_stimulus_interval - self.input_node.x_offset) * self.input_node.fs)
         events_index = events_index[events_index >= 0]
         epochs = np.zeros((buffer_size, self.input_node.data.shape[1], events_index.size), dtype=np.float32)
         print('There are {:} events with code {:}'.format(events_index.shape[0], self.event_code))
         for i, _event in enumerate(tqdm(events_index, desc='Epoching data')):
             # ensure that blocks match buffer size
             if _event + buffer_size > self.input_node.data.shape[0]:
                 epochs = epochs[:, :, list(range(i))]
@@ -274,24 +274,24 @@
 
 
 class AverageEpochs(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  weighted_average: bool = True,
                  weight_across_epochs: bool = True,
                  n_tracked_points: int = None,
-                 block_size: int = 5,
+                 block_size: int = 10,
                  roi_windows: np.array([TimeROI]) = None,
                  **kwargs):
         """
         This InputOutputProcess average epochs
         :param input_process: InputOutputProcess Class
         :param weighted_average: if True, weighted average will be used
         :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights
         are computed within epoch (1 / variance across time)
-        :param n_tracked_points: number of equally spaced points over time used to estimate residual noise
+        :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
         :param block_size: number of trials that will be stacked together to estimate the residual noise
         :param roi_windows: time windows used to perform some measures (snr, rms)
         :param kwargs: extra parameters to be passed to the superclass
         """
         super(AverageEpochs, self).__init__(input_process=input_process, **kwargs)
         self.weighted_average = weighted_average
         self.n_tracked_points = n_tracked_points
@@ -352,16 +352,16 @@
                     FmpTest(df_1=df_num[_idx_ch],
                             df_2=df_den[_idx_ch],
                             f=f_value[_idx_ch],
                             f_critic=f_critic[_idx_ch],
                             p_value=p_value[_idx_ch],
                             rn=self.output_node.rn[_idx_ch],
                             snr=final_snr[_idx_ch, _iw],
-                            time_ini=_ini / self.output_node.fs,
-                            time_end=_end / self.output_node.fs,
+                            ini_time=_ini / self.output_node.fs,
+                            end_time=_end / self.output_node.fs,
                             n_epochs=self.output_node.n,
                             channel=_ch.label,
                             label=_label).__dict__
                 )
         out = pd.DataFrame(tests)
         return out
 
@@ -374,29 +374,29 @@
 
         return roi_samples
 
 
 class AverageEpochsFrequencyDomain(InputOutputProcess):
     def __init__(self,
                  input_process=InputOutputProcess,
-                 n_tracked_points: int = 256,
-                 block_size: int = 5,
+                 n_tracked_points: int = None,
+                 block_size: int = 10,
                  test_frequencies: np.array = None,
                  n_fft: int = None,
                  weighted_average: bool = True,
-                 weighted_frequency_domain: bool = True,
+                 weighted_frequency_domain: bool = False,
                  weight_across_epochs: bool = True,
                  weight_frequencies: np.array = None,
                  delta_frequency: u.Quantity = 5. * u.Hz,
                  power_line_frequency: u.Quantity = 50 * u.Hz,
                  **kwargs):
         """
         This InputOutputProcess average epochs in the frequency domain
         :param input_process: InputOutputProcess Class
-        :param n_tracked_points: number of equally spaced points over time used to estimate residual noise
+        :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
         :param block_size: number of trials that will be stack together to estimate the residual noise
         :param test_frequencies: numpy array with frequencies that will be used to compute statistics (Hotelling test)
         :param weighted_average: bool indicating if weighted average is to be used, otherwise standard average is used
         :param weighted_frequency_domain: boll indicating if the weghts are compute in the time or frequency domain
         :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights
         are computed within epoch (1 / variance across time)
         :param weight_frequencies: numpy array with frequencies that will be used to estimate weights when
@@ -415,38 +415,43 @@
         self.weighted_frequency_domain = weighted_frequency_domain
         self.weight_across_epochs = weight_across_epochs
         self.delta_frequency = set_default_unit(delta_frequency, u.Hz)
         self.power_line_frequency = set_default_unit(power_line_frequency, u.Hz)
 
     def transform_data(self):
         # average processed data across epochs including frequency average
-        if self.weight_frequencies is None and self.test_frequencies is not None:
-            print('No specific frequency provided to estimate weights in the frequency-domain. Pooling across '
-                  'test frequencies {:}. Results may be inaccurate if test frequencies contain no '
-                  'relevant signal'.format(self.test_frequencies.to_string()))
-            self.weight_frequencies = self.test_frequencies
+        if self.weighted_frequency_domain:
+            if self.weight_frequencies is None and self.test_frequencies is not None:
+                print('No specific frequency provided to estimate weights in the frequency-domain. Pooling across '
+                      'test frequencies {:}. Results may be inaccurate if test frequencies contain no '
+                      'relevant signal'.format(self.test_frequencies.to_string()))
+                self.weight_frequencies = self.test_frequencies
 
         exact_frequencies = np.array([]) * u.dimensionless_unscaled
         freq_samples = np.array([]) * u.dimensionless_unscaled
         if self.weighted_frequency_domain and self.weighted_frequency_domain and self.weight_frequencies is not None:
             w_ave, snr, rn, by_freq_rn, by_freq_snr, w_fft, w, freq_samples, exact_frequencies = et_frequency_mean2(
                 epochs=self.input_node.data,
                 fs=self.input_node.fs,
                 weighted_average=self.weighted_average,
                 test_frequencies=self.test_frequencies,
                 delta_frequency=self.delta_frequency,
                 block_size=self.block_size,
                 power_line_frequency=self.power_line_frequency
             )
         else:
+            if self.n_tracked_points is None:
+                self.n_tracked_points = self.input_node.data.shape[0]
+            samples_distance = int(max(self.input_node.data.shape[0] // self.n_tracked_points, 1))
             w_ave, w, rn, cum_rn, w_fft, n, wb, nb, snr = \
                 et_mean(epochs=self.input_node.data,
                         block_size=self.block_size,
                         weighted=self.weighted_average,
-                        weight_across_epochs=self.weight_across_epochs
+                        weight_across_epochs=self.weight_across_epochs,
+                        samples_distance=samples_distance
                         )
             if self.test_frequencies is not None:
                 n = w_ave.shape[0]
                 freqs = np.arange(0, n) * self.input_node.fs / n
                 k = np.array([np.argmin(np.abs(freqs - _f)) for _f in self.test_frequencies])
                 exact_frequencies = freqs[k]
 
@@ -507,32 +512,44 @@
                 spectral_phase=_s_ht.mean_phase)
             f_peaks.append(_f_peak.__dict__)
         _data_pd = pd.DataFrame(f_peaks)
         return _data_pd
 
 
 class DeEpoch(InputOutputProcess):
-    def __init__(self, input_process=InputOutputProcess, de_mean=True, **kwargs):
+    def __init__(self, input_process=InputOutputProcess,
+                 demean_edges=True,
+                 edge_duration: u.Quantity = None,
+                 event_code: int = 1,
+                 **kwargs):
         """
         This function will convert a n*m*p matrix into an (n*p) * m matrix
         :param input_process: InputOutputProcess Class
-        :param de_mean: whether data should be demeaned before converting
+        :param demean_edges: whether data should be demeaned at the edgesbefore converting
         :param kwargs: extra parameters to be passed to the superclass
         """
         super(DeEpoch, self).__init__(input_process=input_process, **kwargs)
-        self.de_mean = de_mean
+        self.demean_edges = demean_edges
+        self.edge_duration = edge_duration
+        self.event_code = event_code
 
     def transform_data(self):
-        _data = np.array(self.input_node.data.data)
-        # if self.de_mean:
-        #     _data -= np.mean(_data, axis=0)
-        for _i in range(1, _data.shape[2]):
-            _data[:, :, _i] = _data[:, :, _i] - (_data[0, :, _i] - _data[-1, :, _i - 1])
+        _data = self.input_node.data.copy()
+        if self.demean_edges:
+            if self.edge_duration is None:
+                _edge_samples = 1
+            else:
+                _edge_samples = int(self.edge_duration * self.input_node.fs)
+
+            for _i in range(1, _data.shape[2]):
+                _previous_edge = np.mean(_data[-_edge_samples::, :, _i - 1], axis=0, keepdims=True)
+                _current_edge = np.mean(_data[0:_edge_samples, :, _i], axis=0, keepdims=True)
+                _data[:, :, _i] = _data[:, :, _i] - (_current_edge - _previous_edge)
 
         self.output_node.data = np.reshape(np.transpose(_data, [0, 2, 1]), [-1, _data.shape[1]], order='F')
         events = []
         for _i in range(_data.shape[2]):
-            events.append(SingleEvent(code=1,
+            events.append(SingleEvent(code=self.event_code,
                                       time_pos=_i * _data.shape[0] / self.input_node.fs,
                                       dur=0))
         events = Events(events=np.array(events))
         self.output_node.events = events
```

### Comparing `peegy-1.3.4/peegy/processing/pipe/general.py` & `peegy-1.3.6/peegy/processing/pipe/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from peegy.processing.pipe.definitions import InputOutputProcess
 from peegy.processing.tools.epochs_processing_tools import et_subtract_oeg_template, et_subtract_correlated_ref
+from peegy.processing.tools.template_generator.auditory_waveforms import fade_in_out_window
 from peegy.processing.tools.multiprocessing.multiprocessesing_filter import filt_data
+from peegy.processing.pipe.epochs import EpochData, AverageEpochs
 import matplotlib.pyplot as plt
 import peegy.processing.tools.filters.eegFiltering as eegf
 from peegy.processing.tools.filters.resampling import eeg_resampling
 from peegy.processing.tools.eeg_epoch_operators import et_unfold
 import numpy as np
 from sklearn.decomposition import FastICA
 from sklearn.cross_decomposition import CCA
@@ -508,7 +510,104 @@
                 self.rejection_threshold
             ))
             print('Setting {:} out of {:} events as bad (based on threshold and DC)'.format(
                 _idx_bad_events.size,
                 events_index.size
             ))
             print(self.output_node.events.summary())
+
+
+class RemoveEvokedResponse(InputOutputProcess):
+    def __init__(self, input_process=InputOutputProcess,
+                 pre_stimulus_interval: u.quantity.Quantity = None,
+                 post_stimulus_interval: u.quantity.Quantity = None,
+                 baseline_correction_ini_time: u.quantity.Quantity = None,
+                 baseline_correction_end_time: u.quantity.Quantity = None,
+                 event_code: float = None,
+                 base_line_correction: bool = False,
+                 demean: bool = True,
+                 events_mask: int = None,
+                 weighted_average: bool = True,
+                 weight_across_epochs: bool = True,
+                 n_tracked_points: int = None,
+                 block_size: int = 10,
+                 fade_in_out: bool = True,
+                 **kwargs):
+        """
+        This class will remove the evoked response from the continuous data and return the continuous data.
+        :param input_process: InputOutputProcess Class
+        :param pre_stimulus_interval: the length (in sec) of the data to be read before the trigger
+        :param post_stimulus_interval: the length (in sec) of the data to be read after the trigger
+        :param event_code: integer indicating the event code to be used to epoch the data
+        :param base_line_correction: whether to perform baseline correction or not. The initial and final time points
+        used to compute the baseline correction are given by baseline_correction_ini_time and
+        baseline_correction_end_time
+        :param baseline_correction_ini_time: initial time (relative to trigger) to compute the mean for baseline
+        correction. For example, if trigger is at zero, and you want to compute the baseline correction from -200 ms you
+        can set baseline_correction_ini_time = -200 * u.ms
+        :param baseline_correction_end_time: end time (relative to trigger) to compute the mean for baseline
+        correction. For example, if trigger is at zero, and you want to compute the baseline correction
+        between -200 * ms and -50 ms, you can set baseline_correction_ini_time = -200 * u.ms and
+        baseline_correction_end_time = -50 * u.ms
+        :param demean: whether to remove the mean from each epoch
+        :param events_mask: integer value used to masker triggers codes. This is useful to ignore triggers inputs above
+        a particular value. For example, if only the first 8 trigger inputs were used (max decimal value is 255), in a
+        system with 16 trigger inputs, then the masker could be set to 255 to ignore any trigger from trigger inputs 9
+        to 16
+        :param weighted_average: if True, weighted average will be used
+        :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights
+        are computed within epoch (1 / variance across time)
+        :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
+        :param block_size: number of trials that will be stacked together to estimate the residual noise
+        :param fade_in_out: It True, a faded in and out window will be applied to evoked response to prevent edge
+        artefacts
+        :param kwargs: extra parameters to be passed to the superclass
+        """
+        super(RemoveEvokedResponse, self).__init__(input_process=input_process, **kwargs)
+        self.pre_stimulus_interval = set_default_unit(pre_stimulus_interval, u.s)
+        self.post_stimulus_interval = set_default_unit(post_stimulus_interval, u.s)
+        self.event_code = event_code
+        self.base_line_correction = base_line_correction
+        self.demean = demean
+        self.events_mask = events_mask
+        self.baseline_correction_ini_time = baseline_correction_ini_time
+        self.baseline_correction_end_time = baseline_correction_end_time
+        self.weighted_average = weighted_average
+        self.n_tracked_points = n_tracked_points
+        self.block_size = block_size
+        self.weight_across_epochs = weight_across_epochs
+        self.fade_in_out = fade_in_out
+
+    def transform_data(self):
+        data = self.input_node.data.copy()
+        epochs = EpochData(input_process=self.input_process,
+                           pre_stimulus_interval=self.pre_stimulus_interval,
+                           post_stimulus_interval=self.post_stimulus_interval,
+                           event_code=self.event_code,
+                           events_mask=self.events_mask,
+                           base_line_correction=self.base_line_correction,
+                           baseline_correction_ini_time=self.baseline_correction_ini_time,
+                           baseline_correction_end_time=self.baseline_correction_end_time,
+                           keep_input_node=True
+                           )
+        epochs.run()
+        evoked_response = AverageEpochs(input_process=epochs,
+                                        keep_input_node=False,
+                                        weighted_average=self.weighted_average,
+                                        weight_across_epochs=self.weight_across_epochs,
+                                        block_size=self.block_size,
+                                        roi_windows=None,
+                                        n_tracked_points=self.n_tracked_points)
+        evoked_response.run()
+        _epoch_samples = evoked_response.output_node.data.shape[0]
+        evoked_data = evoked_response.output_node.data
+        if self.fade_in_out:
+            fade_window = fade_in_out_window(n_samples=_epoch_samples,
+                                             fraction=0.05)
+            evoked_data = evoked_data * fade_window
+
+        for _events in self.input_node.events.get_events_index(self.event_code, fs=self.input_node.fs):
+            _ini = _events
+            _end = np.minimum(_events + _epoch_samples, data.shape[0])
+            _er = evoked_data[0: _end - _ini, :]
+            data[_ini: _end, :] = data[_ini: _end, :] - _er
+        self.output_node.data = data
```

### Comparing `peegy-1.3.4/peegy/processing/pipe/interpolation.py` & `peegy-1.3.6/peegy/processing/pipe/interpolation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/io.py` & `peegy-1.3.6/peegy/processing/pipe/io.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/pipeline.py` & `peegy-1.3.6/peegy/processing/pipe/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 
     def __getitem__(self, key):
         out = None
         if key in self.keys():
             out = super(PipePool, self).__getitem__(key)
         return out
 
-    def run(self):
+    def run(self, force: bool = False):
         for _item, _value in self.items():
-            if _value.ready:
+            if _value.ready and not force:
                 continue
             _value.run()
             _value.ready = True
 
     def diagram(self,
                 file_name: str = '',
                 return_figure=False,
```

### Comparing `peegy-1.3.4/peegy/processing/pipe/plot.py` & `peegy-1.3.6/peegy/processing/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/regression.py` & `peegy-1.3.6/peegy/processing/pipe/regression.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/simulate.py` & `peegy-1.3.6/peegy/processing/pipe/simulate.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/spatial_filtering.py` & `peegy-1.3.6/peegy/processing/pipe/spatial_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,83 +21,94 @@
 
 
 class SpatialFilter(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  sf_join_frequencies: np.array = None,
                  demean_data: bool = True,
                  weight_data: bool = True,
+                 weighted_frequency_domain: bool = False,
                  weight_across_epochs: bool = True,
                  keep0: int = None,
                  keep1: float = 1e-9,
                  perc0: float = .99,
                  perc1: float = None,
                  block_size: int = 10,
+                 n_tracked_points: int = None,
                  delta_frequency: u.Quantity = 5 * u.Hz,
                  **kwargs):
         """
         This class will create a spatial filter based on the data. If sf_join_frequencies are passed, the spatial
         filter will use a biased function based on the covariance of those frequencies only.
         :param input_process:  InputOutputProcess Class
         :param sf_join_frequencies: numpy array indicating the biased frequencies (useful for steady-state responses)
         :param demean_data: if true, data will be demeaned prior filter estimation
         :param weight_data: if true, dss filter will be estimated using weights
+        :param weighted_frequency_domain: boll indicating if the weghts are compute in the time or frequency domain
         :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights
         are computed within epoch (1 / variance across time)
         :param keep0: integer controlling  whitening of unbiased components in DSS. This integer value represent the
         number of components to keep.
         :param keep1: float controlling  whitening of unbiased components in DSS. This value will remove components
         below keep1 which is relative to the maximum eigen value.
         :param perc0: float (between 0 and 1) controlling whitening of unbiased components in DSS.
         This value will preserve components that explain the percentage of variance.
         :param perc1: float (between 0 and 1) controlling the number of biased components kept in DSS.
         This value will preserve the components of the biased PCA analysis that explain the percentage of variance.
-        :param block_size: integer indicating the number of trials that would be use to estimate the weights
+        :param block_size: integer indicating the number of trials that would be used to estimate the weights
+        :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
         :param delta_frequency: frequency size around each sf_join_frequency to estimate noise
         :param kwargs: extra parameters to be passed to the superclass
         """
         super(SpatialFilter, self).__init__(input_process=input_process, **kwargs)
         self.sf_join_frequencies = set_default_unit(sf_join_frequencies, u.Hz)
         self.demean_data = demean_data
         self.weight_data = weight_data
+        self.weighted_frequency_domain = weighted_frequency_domain
         self.weight_across_epochs = weight_across_epochs
         self.pwr0 = None
         self.pwr1 = None
         self.n_components_rotation_1 = None
         self.n_components_rotation_2 = None
         self.n_possible_components = None
         self.cov = None
         self.keep0 = keep0
         self.keep1 = keep1
         self.perc0 = perc0
         self.perc1 = perc1
         self.block_size = block_size
+        self.n_tracked_points = n_tracked_points
         self.delta_frequency = delta_frequency
+        self.weights = None
 
     def transform_data(self):
         # compute spatial filter
-        z, pwr0, pwr1, cov, n_0, n_1, _ = et_get_spatial_filtering(epochs=self.input_node.data,
-                                                                   fs=self.input_node.fs,
-                                                                   sf_join_frequencies=self.sf_join_frequencies,
-                                                                   demean_data=self.demean_data,
-                                                                   weight_data=self.weight_data,
-                                                                   weight_across_epochs=self.weight_across_epochs,
-                                                                   weights=self.input_node.w,
-                                                                   keep0=self.keep0,
-                                                                   keep1=self.keep1,
-                                                                   perc0=self.perc0,
-                                                                   perc1=self.perc1,
-                                                                   block_size=self.block_size,
-                                                                   delta_frequency=self.delta_frequency)
+        z, pwr0, pwr1, cov, n_0, n_1, weights = et_get_spatial_filtering(
+            epochs=self.input_node.data,
+            fs=self.input_node.fs,
+            sf_join_frequencies=self.sf_join_frequencies,
+            demean_data=self.demean_data,
+            weight_data=self.weight_data,
+            weighted_frequency_domain=self.weighted_frequency_domain,
+            weight_across_epochs=self.weight_across_epochs,
+            weights=self.input_node.w,
+            keep0=self.keep0,
+            keep1=self.keep1,
+            perc0=self.perc0,
+            perc1=self.perc1,
+            block_size=self.block_size,
+            n_tracked_points=self.n_tracked_points,
+            delta_frequency=self.delta_frequency)
         self.output_node.data = z * u.dimensionless_unscaled
         self.pwr0 = pwr0
         self.pwr1 = pwr1
         self.cov = cov
         self.n_components_rotation_1 = n_0
         self.n_components_rotation_2 = n_1
         self.n_possible_components = self.input_node.data.shape[1]
+        self.weights = weights
 
 
 class ApplySpatialFilter(InputOutputProcess):
     def __init__(self,
                  input_process: SpatialFilter = None,
                  sf_components: np.array = np.array([]),
                  sf_thr: float = 0.8,
@@ -130,21 +141,23 @@
 class CreateAndApplySpatialFilter(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  sf_join_frequencies: np.array = None,
                  sf_components=np.array([]),
                  sf_thr: float = 0.8,
                  keep0: int = None,
                  keep1: float = 1e-9,
-                 perc0: float = .99,
+                 perc0: float = 0.99,
                  perc1: float = None,
                  test_frequencies: u.Quantity = None,
                  delta_frequency: u.Quantity = 5 * u.Hz,
                  block_size: int = 10,
+                 n_tracked_points: int = None,
                  demean_data: bool = True,
                  weight_data: bool = True,
+                 weighted_frequency_domain: bool = False,
                  weight_across_epochs: bool = True,
                  projection_domain: Domain = Domain.time,
                  components_to_plot: np.array = np.arange(0, 10),
                  plot_projections: bool = True,
                  plot_power: bool = True,
                  plot_x_lim: [float, float] = None,
                  plot_y_lim: [float, float] = None,
@@ -166,27 +179,30 @@
         This value will preserve components that explain the percentage of variance.
         :param perc1: float (between 0 and 1) controlling the number of biased components kept in DSS.
         This value will preserve the components of the biased PCA analysis that explain the percentage of variance.
         :param test_frequencies: frequency array to compute statistics in the frequency-domain in the component space.
         :param delta_frequency: frequency size around each sf_join_frequency to estimate noise
         :param demean_data: If true, filter will be created with demeaned data
         :param weight_data: if true, weighted average will be use to create the filter
+        :param weighted_frequency_domain: boll indicating if the weghts are compute in the time or frequency domain
         :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights
         are computed within epoch (1 / variance across time)
         :param projection_domain: indicate the domain in which component will be projected in plots
         :param components_to_plot: numpy array indicating which components will be plotted.
         :param plot_projections: if true, components will be projected to the original space and plots will be generated
         :param plot_power: if true both bias and unbiased component's power as well as their rations will be plotted
         :param plot_x_lim: list with minimum and maximum horizontal range of x axis
         :param plot_y_lim: list with minimum and maximum vertical range of y axis
         :param user_naming_rule: string indicating a user naming to be included in the figure file name
         :param fig_format: string indicating the format of the output figure (e.g. '.png' or '.pdf')
         :param return_figures: bool indicating if figure handle should be returned in self.figures
         :param save_to_file: bool indicating whether figure should be saved to file
-        :param block_size: number of trials that will be stack together to estimate the residual noise
+        :param block_size: number of trials that will be stacked together to estimate the residual noise
+        :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
+        n_tracked_points
         :param kwargs: extra parameters to be passed to the superclass
         """
         super(CreateAndApplySpatialFilter, self).__init__(input_process=input_process, **kwargs)
         self.sf_join_frequencies = set_default_unit(sf_join_frequencies, u.Hz)
         self.sf_components = sf_components
         self.sf_thr = sf_thr
         self.keep0 = keep0
@@ -196,20 +212,23 @@
         self.p_ratio = None
         self.pwr0 = None
         self.pwr1 = None
         self.kept_components = None
         self.test_frequencies = test_frequencies
         self.delta_frequency = delta_frequency
         self.block_size = block_size
+        self.n_tracked_points = n_tracked_points
+        self.weights = None
         self.components_to_plot = components_to_plot
         self.plot_projections = plot_projections
         self.plot_power = plot_power
         self.projection_domain = projection_domain
         self.demean_data = demean_data
         self.weight_data = weight_data
+        self.weighted_frequency_domain = weighted_frequency_domain
         self.weight_across_epochs = weight_across_epochs
         self.plot_x_lim = plot_x_lim
         self.plot_y_lim = plot_y_lim
         self.user_naming_rule = user_naming_rule
         self.fig_format = fig_format
         self.return_figures = return_figures
         self.save_to_file = save_to_file
@@ -221,34 +240,37 @@
             self.test_frequencies = self.sf_join_frequencies
         if self.return_figures:
             figures = []
         spatial_filter = SpatialFilter(input_process=self.input_process,
                                        sf_join_frequencies=self.sf_join_frequencies,
                                        demean_data=self.demean_data,
                                        weight_data=self.weight_data,
+                                       weighted_frequency_domain=self.weighted_frequency_domain,
                                        weight_across_epochs=self.weight_across_epochs,
                                        keep0=self.keep0,
                                        keep1=self.keep1,
                                        perc0=self.perc0,
                                        perc1=self.perc1,
                                        block_size=self.block_size,
+                                       n_tracked_points=self.n_tracked_points,
                                        delta_frequency=self.delta_frequency
                                        )
         spatial_filter.run()
         filtered_data = ApplySpatialFilter(input_process=spatial_filter,
                                            sf_components=self.sf_components,
                                            sf_thr=self.sf_thr,
                                            **self.__kwargs)
         filtered_data.run()
 
         self.output_node = filtered_data.output_node
         self.p_ratio = spatial_filter.pwr1 / spatial_filter.pwr0
         self.pwr0 = spatial_filter.pwr0
         self.pwr1 = spatial_filter.pwr1
         self.kept_components = filtered_data.kept_components
+        self.weights = spatial_filter.weights
 
         if self.components_to_plot is not None:
             plotter_1 = PlotSpatialFilterComponents(spatial_filter,
                                                     plot_x_lim=self.plot_x_lim,
                                                     plot_y_lim=self.plot_y_lim,
                                                     user_naming_rule=self.user_naming_rule,
                                                     fig_format=self.fig_format,
@@ -313,27 +335,31 @@
         gs = gridspec.GridSpec(3, 1)
         ax = plt.subplot(gs[0, 0])
         _normalized_raw_power = self.pwr0 / np.sum(self.pwr0)
         _normalized_evoked_power = self.pwr1 / np.sum(self.pwr1)
 
         ax.plot(_normalized_raw_power, marker='o', label='Raw')
         ax.plot(_normalized_evoked_power, marker='o', label='Evoked')
-        ax.plot(_normalized_evoked_power[self.kept_components], marker='*', label='Kept', linestyle='None')
+        ax.plot(self.kept_components,
+                _normalized_evoked_power[self.kept_components],
+                marker='*', label='Kept', linestyle='None')
         ax.axvline(self.kept_components.max(), color='black', label=None)
         ax.set_xlabel('Component rank')
         ax.legend(loc="upper right")
         ax.set_title('Normalized Power')
 
         ax = plt.subplot(gs[1, 0])
 
         _accumulated_raw_power = np.cumsum(self.pwr0 / np.sum(self.pwr0))
         _accumulated_evoked_power = np.cumsum(self.pwr1) / np.sum(self.pwr1)
         ax.plot(_accumulated_raw_power, marker='o', label='Raw')
         ax.plot(_accumulated_evoked_power, marker='o', label='Evoked')
-        ax.plot(_accumulated_evoked_power[self.kept_components], marker='*', label='Kept', linestyle='None')
+        ax.plot(self.kept_components,
+                _accumulated_evoked_power[self.kept_components],
+                marker='*', label='Kept', linestyle='None')
         ax.axvline(self.kept_components.max(), color='black', label=None)
         ax.set_ylim([0, 1])
         ax.set_xlabel('Component rank')
         ax.set_title('Accumulated power')
         ax.legend(loc="upper right")
 
         ax = plt.subplot(gs[2, 0])
@@ -342,15 +368,16 @@
             self.pwr1 / self.pwr0)
         ax.plot(_per_component_explained_power,
                 marker='o',
                 label='Per component')
         ax.plot(_accumulated_component_explained_power,
                 marker='o',
                 label='Accumulated')
-        ax.plot(_per_component_explained_power[self.kept_components],
+        ax.plot(self.kept_components,
+                _per_component_explained_power[self.kept_components],
                 marker='*', label='Kept', linestyle='None')
         ax.axvline(self.kept_components.max(), color='black', label=None)
         # ax.set_ylim([0, 1])
         ax.set_xlabel('Component rank')
         ax.set_title('Evoked power per component / Total power')
         ax.legend(loc="upper right")
 
@@ -534,15 +561,15 @@
 class CreateAndApplyICAFilter(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  sf_components=np.array([]),
                  sf_thr=0.8,
                  components_to_plot: np.array = np.arange(0, 10),
                  plot_x_lim: [float, float] = None,
                  plot_y_lim: [float, float] = None,
-                 n_tracked_points=256,
+                 n_tracked_points=None,
                  block_size=5,
                  weight_data=True,
                  user_naming_rule: str = '',
                  fig_format: str = '.png',
                  return_figures: bool = False,
                  **kwargs):
         """
```

### Comparing `peegy-1.3.4/peegy/processing/pipe/statistics.py` & `peegy-1.3.6/peegy/processing/pipe/statistics.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/storage.py` & `peegy-1.3.6/peegy/processing/pipe/storage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/pipe/time_frequency.py` & `peegy-1.3.6/peegy/processing/pipe/time_frequency.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/statistics/definitions.py` & `peegy-1.3.6/peegy/processing/statistics/definitions.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 class TestType(object):
     hotelling_t2_time = 'hotelling_t2_time'  # hotelling-t2 test in the time-domain
     hotelling_t2_freq = 'hotelling_t2_freq'  # hotelling-t2 test in the frequency-domain
     f_test_freq = 'f_test_freq'  # f-ratio in frequency domain
     f_test_time = 'f_test_time'  # f-ratio using multiple points in the time-domain
     rayleigh_test = 'rayleigh_test'  # phase-locking value
     covariance = 'covariance'  # covariance
+    bootstrap = 'bootstrap'
 
     def get_available_methods(self):
         members = [attr for attr in dir(self) if not callable(getattr(self, attr)) and not attr.startswith("__")]
         return members
 
 
 class HotellingTSquareFrequencyTest(object):
@@ -26,15 +27,18 @@
                  n_epochs=None,
                  spectral_magnitude=None,
                  spectral_phase=None,
                  rn=None,
                  snr=None,
                  snr_db=None,
                  f_critic=None,
-                 channel=None):
+                 channel=None,
+                 ini_time: float = None,
+                 end_time: float = None
+                 ):
         self.data_source = data_source
         self.test_name = test_name
         self.frequency_tested = frequency_tested
         self.df_1 = df_1
         self.df_2 = df_2
         self.t_square = t_square
         self.f = f
@@ -43,14 +47,16 @@
         self.spectral_phase = spectral_phase
         self.rn = rn
         self.n_epochs = n_epochs
         self.snr = snr
         self.snr_db = snr_db
         self.f_critic = f_critic
         self.channel = channel
+        self.ini_time = ini_time
+        self.end_time = end_time
 
 
 class HotellingTSquareTest(object):
     def __init__(self,
                  test_name='HT2',
                  df_1=None,
                  df_2=None,
@@ -64,14 +70,16 @@
                  n_epochs=None,
                  snr=None,
                  snr_db=None,
                  snr_critic_db=None,
                  snr_critic=None,
                  channel=None,
                  frequency_tested=None,
+                 ini_time: float = None,
+                 end_time: float = None,
                  **kwargs
                  ):
         self.test_name = test_name
         self.df_1 = df_1
         self.df_2 = df_2
         self.t_square = t_square
         self.f = f
@@ -83,14 +91,16 @@
         self.n_epochs = n_epochs
         self.snr = snr
         self.snr_db = snr_db
         self.snr_critic_db = snr_critic_db
         self.snr_critic = snr_critic
         self.channel = channel
         self.frequency_tested = frequency_tested
+        self.ini_time = ini_time
+        self.end_time = end_time
         for _item, _value in kwargs.items():
             setattr(self, _item, _value)
 
 
 class FrequencyFTest(object):
     def __init__(self,
                  test_name='F-test',
@@ -101,75 +111,84 @@
                  p_value=None,
                  spectral_magnitude=None,
                  spectral_phase=None,
                  rn=None,
                  snr=None,
                  snr_db=None,
                  f_critic=None,
-                 channel=None):
+                 channel=None,
+                 ini_time: float = None,
+                 end_time: float = None,
+                 ):
         self.test_name = test_name
         self.frequency_tested = frequency_tested
         self.df_1 = df_1
         self.df_2 = df_2
         self.f = f
         self.p_value = p_value
         self.spectral_magnitude = spectral_magnitude
         self.spectral_phase = spectral_phase
         self.rn = rn
         self.snr = snr
         self.snr_db = snr_db
         self.f_critic = f_critic
         self.channel = channel
+        self.ini_time = ini_time
+        self.end_time = end_time
 
 
 class PhaseLockingValueTest(object):
     def __init__(self,
                  test_name='rayleigh_test',
                  plv=None,
                  df_1=None,
                  z_value=None,
                  z_critic=None,
                  p_value=None,
                  mean_phase=None,
                  channel=None,
                  frequency_tested=None,
+                 ini_time: float = None,
+                 end_time: float = None,
                  rn=None):
         self.test_name = test_name
         self.plv = plv
         self.df_1 = df_1
         self.z_value = z_value
         self.z_critic = z_critic
         self.p_value = p_value
         self.mean_phase = mean_phase
         self.channel = channel
         self.frequency_tested = frequency_tested
         self.rn = rn
+        self.ini_time = ini_time
+        self.end_time = end_time
 
 
 class FmpTest(object):
     def __init__(self,
                  test_name='Fmp',
                  label: str = None,
                  df_1: float = None,
                  df_2: float = None,
                  f: float = None,
                  f_critic: float = None,
                  p_value: float = None,
                  rn: float = None,
                  snr: float = None,
-                 time_ini: float = None,
-                 time_end: float = None,
+                 ini_time: float = None,
+                 end_time: float = None,
                  n_epochs: int = None,
                  channel: str = None):
         self.test_name = test_name
         self.label = label
         self.df_1 = df_1
         self.df_2 = df_2
         self.f = f
         self.f_critic = f_critic
         self.p_value = p_value
         self.rn = rn
         self.snr = snr
-        self.time_ini = time_ini
-        self.time_end = time_end
+        self.ini_time = ini_time
+        self.end_time = end_time
         self.n_epochs = n_epochs
         self.channel = channel
```

### Comparing `peegy-1.3.4/peegy/processing/statistics/eeg_statistic_tools.py` & `peegy-1.3.6/peegy/processing/statistics/eeg_statistic_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,19 @@
     data_demeaned = samples - mean_data[..., None]
     with np.errstate(divide='ignore', invalid='ignore'):
         for _ch in tqdm(range(samples.shape[1]), desc="Hotelling-T2"):
             # _cov_mat = np.cov(data_ch.value.squeeze(), aweights=_weights.value.squeeze()) * data_ch.unit ** 2.0
             data_ch = data_demeaned[:, _ch, :]
             mean_ch = mean_data[:, _ch]
             _cov_mat = np.cov(data_ch.value, aweights=weights[_ch, :].value) * data_ch.unit ** 2.0
-            _t_square = dof[_ch] * mean_ch.dot(np.linalg.pinv(_cov_mat)).dot(mean_ch.T)
+            if _cov_mat.ndim == 0:
+                _t_square = dof[_ch] * mean_ch.dot(1 / _cov_mat).dot(mean_ch.T)
+            else:
+                _t_square = dof[_ch] * mean_ch.dot(np.linalg.pinv(_cov_mat)).dot(mean_ch.T)
+            _t_square = _t_square.value
             n_p = data_ch.shape[0]
             n_n = dof[_ch]
             _f = (n_n - n_p) / (n_p * (n_n - 1.0)) * _t_square
             _d1 = n_p
             _d2 = np.maximum(n_n - n_p, 0)
             _f_95 = st.f.ppf(0.95, _d1, _d2)
             if _d2 > 0:
@@ -146,17 +150,17 @@
     z = dof * plv ** 2
 
     # D.Wilkie. Rayleigh Test for Randomness of Circular Data".Applied Statistics.1983.
     tmp = np.ones(z.shape)
     _idx_tmp = (dof < 50).squeeze()
 
     if np.any(_idx_tmp):
-        _tmp_coorection = 1.0 + (2.0 * z - z * z) / (4.0 * dof) - (
+        _tmp_correction = 1.0 + (2.0 * z - z * z) / (4.0 * dof) - (
                 24.0 * z - 132.0 * z ** 2.0 + 76.0 * z ** 3.0 - 9.0 * z ** 4.0) / (288.0 * dof * dof)
-        tmp[:, _idx_tmp] = _tmp_coorection
+        tmp[:, _idx_tmp] = _tmp_correction
     z_crit = -np.log(alpha) - (2 * np.log(alpha) + np.log(alpha) ** 2.0) / (4 * dof)
     p_values = np.exp(-z) * tmp
 
     return spectral_amp, plv, z, z_crit, p_values, angles, dof, residual_noise
 
 
 def discrete_phase_locking_value(
@@ -194,18 +198,18 @@
     plv = np.abs(np.sum(yfft * weights, axis=2) / np.sum(weights, axis=2))
     z = dof * plv ** 2
     # D.Wilkie. Rayleigh Test for Randomness of Circular Data".Applied Statistics.1983.
     tmp = np.ones(z.shape)
     _idx_tmp = (dof < 50).squeeze()
 
     if np.any(_idx_tmp):
-        _tmp_coorection = 1.0 + (2.0 * z - z * z) / (4.0 * dof) - (24.0 * z - 132.0 * z ** 2.0 +
+        _tmp_correction = 1.0 + (2.0 * z - z * z) / (4.0 * dof) - (24.0 * z - 132.0 * z ** 2.0 +
                                                                    76.0 * z ** 3.0 - 9.0 * z ** 4.0) / (
                                       288.0 * dof * dof)
-        tmp[:, _idx_tmp] = _tmp_coorection
+        tmp[:, _idx_tmp] = _tmp_correction
     z_crit = -np.log(alpha) - (2 * np.log(alpha) + np.log(alpha) ** 2.0) / (4 * dof)
     p_values = np.exp(-z) * tmp
 
     return spectral_amp, plv, z, z_crit, p_values, angles, dof, residual_noise
 
 
 def get_discrete_frequency_value(
@@ -240,16 +244,15 @@
     yfft = 2 * yfft / data.shape[0]
     return yfft, spectral_amp, residual_noise
 
 
 def freq_bin_phase_locking_value(
         yfft: np.array = None,
         alpha: float = 0.05,
-        weights: np.array = None,
-        regularization_factor: float = 0.005) -> np.array:
+        weights: np.array = None) -> np.array:
     """
     Compute phase, and  phase-locking value (PLV) using Rayleigh test for an array of trials from a single frequency
     component.
     :param yfft: fft_bin (complex) x channels x trials numpy array in the time domain
     :param alpha: float indicating the alpha value for significance
     :param frequency: float indicating the frequency of interest
     :param weights: trial by trial weights
@@ -293,14 +296,14 @@
     z = dof * plv ** 2
 
     # D.Wilkie. Rayleigh Test for Randomness of Circular Data".Applied Statistics.1983.
     tmp = np.ones(z.shape)
     _idx_tmp = (dof < 50).squeeze()
 
     if np.any(_idx_tmp):
-        _tmp_coorection = 1.0 + (2.0 * z - z * z) / (4.0 * dof) - (
+        _tmp_correction = 1.0 + (2.0 * z - z * z) / (4.0 * dof) - (
                 24.0 * z - 132.0 * z ** 2.0 + 76.0 * z ** 3.0 - 9.0 * z ** 4.0) / (288.0 * dof * dof)
-        tmp[:, _idx_tmp] = _tmp_coorection
+        tmp[:, _idx_tmp] = _tmp_correction
     z_crit = -np.log(alpha) - (2 * np.log(alpha) + np.log(alpha) ** 2.0) / (4 * dof)
     p_values = np.exp(-z) * tmp
 
     return spectral_amp, plv, z, z_crit, p_values, angles, dof, residual_noise
```

### Comparing `peegy-1.3.4/peegy/processing/system/progress.py` & `peegy-1.3.6/peegy/processing/system/progress.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/detection/definitions.py` & `peegy-1.3.6/peegy/processing/tools/detection/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/detection/time_domain_tools.py` & `peegy-1.3.6/peegy/processing/tools/detection/time_domain_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/eeg_epoch_operators.py` & `peegy-1.3.6/peegy/processing/tools/eeg_epoch_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,16 +495,15 @@
 #     #  idx allows x to be aligned with z
 #     offset = np.maximum(0, -mn)
 #     idx=np.arange(offset, offset + z.shape[0])
 #
 #
 #
 def et_demean(x: np.array = np.array([]),
-              w: np.array = np.array([]),
-              eps: float = np.finfo(float).eps):
+              w: np.array = np.array([])):
 
     if w.size and w.size < x.shape[0]:
         w = w[:]
         # interpret w as array of indices to set to 1
         assert ~(np.min(w) < 0 or np.max(w) > x.shape[0]), 'w interpreted as indices but values are out of range'
         ww = np.zeros((x.shape[0], 1, 1))
         ww[w] = 1
@@ -527,17 +526,17 @@
         mn = np.mean(x, axis=0)
         x = x - mn
     else:
         # w = et_unfold(w)
         if w.shape[0] != x.shape[0]:
             raise Exception('X and W should have same number of rows')
         if w.shape[1] == 1:
-            mn = np.sum(x * w, axis=0) / (np.sum(w, axis=0) + eps)
+            mn = np.sum(x * w, axis=0) / (np.sum(w, axis=0))
         elif w.shape[1] == n:
-            mn = np.sum(x * w, axis=0) / (np.sum(w, axis=0) + eps)
+            mn = np.sum(x * w, axis=0) / (np.sum(w, axis=0))
         else:
             raise Exception('W should have same number of columns as X, or else 1')
         x = x - mn
     return x
 
 
 def w_mean(epochs: np.array = np.array([]),
@@ -576,10 +575,9 @@
     https://docs.displayr.com/wiki/Design_Effects_and_Effective_Sample_Size
 
     :param weights: array of weights
     :param axis: direction indicating how weights are summed
     :return:
     """
     weights = set_default_unit(weights, u.dimensionless_unscaled)
-    epsilon = np.finfo(float).eps * weights.unit ** 2.0
-    ess = np.sum(weights, axis=axis) ** 2.0 / (np.sum(weights ** 2.0, axis=axis) + epsilon)
+    ess = np.sum(weights, axis=axis) ** 2.0 / (np.sum(weights ** 2.0, axis=axis))
     return ess
```

### Comparing `peegy-1.3.4/peegy/processing/tools/epochs_processing_tools.py` & `peegy-1.3.6/peegy/processing/tools/epochs_processing_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
             cumulative_rn = np.vstack((cumulative_rn, np.sqrt(1.0 / np.sum(w[:, 0:_i + 1], axis=1))))
 
     n_epochs = np.sum(nk)
     return w, rn, cumulative_rn, n_epochs, wb, nk
 
 
 def et_mean(epochs: np.array = np.array([]),
-            block_size: int = 5,
-            samples_distance: int = 10,
+            block_size: int = 10,
+            samples_distance: int = 1,
             weighted: bool = True,
             normalize_weights: bool = False,
             demean_epochs: bool = True,
             weight_across_epochs: bool = True):
     """
     Compute the mean of the input epochs
     :param epochs: samples x channels x trials numpy array
@@ -157,15 +157,15 @@
     :param normalize_weights: if true weights will be normalized so that their sum across x is equal to 1
     :param demean_epochs: if True, individual epochs will be demeaned
     :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights are
     computed within epoch (1 / variance across time)
     :return: average data (standard or weighted), weights, residual noise, cumulative residual noise over trials,
     spectrum of final average scaled to time domain amplitudes, array with number of sources per noise source
     """
-
+    epochs = set_default_unit(epochs, u.dimensionless_unscaled)
     if weighted:
         if weight_across_epochs:
             w, final_rn, cumulative_rn, n, wb, nb = et_get_epoch_weights_and_rn_weighted_average(
                 epochs=epochs,
                 block_size=block_size,
                 samples_distance=samples_distance,
                 demean_epochs=demean_epochs
@@ -472,15 +472,15 @@
                              crest_factor_threshold=10,
                              plot_results=False,
                              figure_path: str = '',
                              figure_basename: str = '',
                              minimum_interval_width: u.Quantity = 0.075 * u.s,
                              eog_peak_width: u.Quantity = 0.02 * u.s,
                              n_iterations: int = 10,
-                             kernel_bandwidth: float = 4 * 0.15,
+                             kernel_bandwidth: float = 0.15,
                              use_initial_template: bool = True):
     """
     This function removes EOG artefacts via a variation of the template subtraction method described in Valderrama
     et al., 2018.The algorithm performs several steps:
     1 - Blinks are detected in the EOG channel using a peak detection and generating a starting template.
     2 - The template is iteratively adjusted using  a math-filter.
     The location of the events is recomputed using the match filter and a new template is estimated over each iteration.
@@ -533,15 +533,19 @@
                                                         n_iterations=n_iterations,
                                                         kernel_bandwidth=kernel_bandwidth,
                                                         use_initial_template=use_initial_template)
         reconstructed = reconstruct_eog(data=data,
                                         template=template,
                                         blink_positions=eog_events)
 
+        # remove from original data (untouched)
         output_data = output_data - reconstructed * data.unit
+        # also remove from filtered data used to reconstruct, otherwise the reconstructed data will have EOG components
+        # what were previousely removed.
+        data = data - reconstructed * data.unit
         figures = []
         if plot_results:
             time = np.arange(0, output_data.shape[0]) / fs
             time_template = (np.arange(0, template.shape[0]) - template.shape[0] / 2) / fs
             fig = plt.figure()
             ax = fig.add_subplot(311)
             ax.plot(time_template, template, label='fitted template')
@@ -566,71 +570,79 @@
     return output_data, figures, template, z, eog_events
 
 
 def et_get_spatial_filtering(epochs: np.array = np.array([]),
                              fs: u.Quantity = None,
                              sf_join_frequencies: np.array = None,
                              weight_data: bool = True,
+                             weighted_frequency_domain: bool = False,
                              weight_across_epochs: bool = True,
                              weights: np.array = None,
                              demean_data: bool = True,
                              keep0: int = None,
                              keep1: float = 1e-9,
-                             perc0: float = .99,
+                             perc0: float = 1,
                              perc1: float = None,
                              block_size: int = 10,
+                             n_tracked_points: int = None,
                              delta_frequency: u.Quantity = 5 * u.Hz
                              ):
     """
 
     :param epochs: m x n x l (samples, channels, epochs)
     :param fs: sampling rate
     :param sf_join_frequencies: numpy array with frequencies to bias the filter
     :param weight_data: if True, covariance and mean will be estimated using weights
+    :param weighted_frequency_domain: boll indicating if the weghts are compute in the time or frequency domain
     :param weight_across_epochs: if True, weights are computed across epochs (as in Elbeling 1984) otherwise weights
     are computed within epoch (1 / variance across time)
     :param weights: array of weights to use when weighted_average is true. If none and weighted_average is true,
     these will be estimated.
     :param demean_data: if True, data will be demeaned prior weights estimation.
     :param keep0: integer controlling  whitening of unbiased components in DSS. This integer value represent the number
     of components to keep.
     :param keep1: float controlling  whitening of unbiased components in DSS. This value will remove components below
     keep1 which is relative to the maximum eigen value.
     :param perc0: float (between 0 and 1) controlling whitening of unbiased components in DSS.
     This value will preserve components that explain the percentage of variance.
     :param perc1: float (between 0 and 1) controlling the number of biased components kept in DSS.
     This value will preserve the components of the biased PCA analysis that explain the percentage of variance.
     :param block_size: integer indicating the number of trials that would be use to estimate the weights
+    :param n_tracked_points: number of equally spaced points over time used to estimate residual noise and weights
     :param delta_frequency: frequency size around each sf_join_frequency to estimate noise
     :return: z, pwr0, pwr1, cov_1, weights: components, unbiased power, biased power, covariance rotation,
     estimated weights
     """
     print('computing spatial filter')
 
     # bias function uses weighted mean or standard mean
     if weight_data and weights is None:
-        if sf_join_frequencies is None:
-            _, weights, *_ = et_mean(epochs,
-                                     weighted=weight_data,
-                                     weight_across_epochs=weight_across_epochs,
-                                     block_size=block_size)
-        else:
+        if weighted_frequency_domain:
             weights, *_ = get_pooled_frequency_weights(
                 epochs=epochs,
                 fs=fs,
                 frequencies=sf_join_frequencies,
                 weighted_average=weight_data,
                 block_size=block_size,
                 delta_frequency=delta_frequency,
             )
+        else:
+            if n_tracked_points is None:
+                n_tracked_points = epochs.shape[0]
+            samples_distance = int(max(epochs.shape[0] // n_tracked_points, 1))
+            _, weights, *_ = et_mean(epochs,
+                                     weighted=weight_data,
+                                     weight_across_epochs=weight_across_epochs,
+                                     block_size=block_size,
+                                     samples_distance=samples_distance)
 
     if weights is None:
         weights = np.ones(epochs.shape) * u.dimensionless_unscaled
     if demean_data:
-        epochs = eo.et_demean(epochs, w=weights, eps=np.finfo(float).eps * weights.unit)
+        epochs = eo.et_demean(epochs, w=weights)
 
     average = eo.w_mean(epochs, weights=weights)
 
     if sf_join_frequencies is not None:
         n_frequencies = sf_join_frequencies / fs
         c0, t0 = eo.et_freq_weighted_cov(epochs, normalized_frequencies=n_frequencies, w=weights.value)
         c1, t1 = eo.et_freq_weighted_cov(average, normalized_frequencies=n_frequencies)
@@ -1283,26 +1295,23 @@
 
 
 def get_discrete_frequencies_weights(
         epochs: np.array = None,
         fs: float = None,
         frequencies: float = None,
         block_size: int = 5,
-        weighted_average=True,
-        regularization_factor: float = 0.005,) -> np.array:
+        weighted_average=True) -> np.array:
     """
     Compute spectral amplitude for a given frequencies
     component.
     :param epochs: time x channels x trials numpy array in the time domain
     :param fs: float indicating the sampling rate in Hz
     :param frequencies: array with the frequencies of interest
     :param block_size: integer indicating the number of trials that would be use to estimate the weights
     :param weighted_average: if false, frequency bins will not be weighted to compute mean and std
-    :param regularization_factor: This value is used to regularize the variance if too small (based on Tikhonov
-     regularization)
     """
     epochs = set_default_unit(epochs, u.uV)
     fs = set_default_unit(fs, u.Hz)
     frequencies = set_default_unit(frequencies, u.Hz)
 
     y_fft, exact_frequencies = discrete_dft(epochs, fs, frequencies)
 
@@ -1315,28 +1324,28 @@
     total_var = np.zeros((y_fft.shape[0], epochs.shape[1], n_blocks)) * epochs.unit ** 2.0
     wb = np.ones(total_var.shape) * total_var.unit
     ini_block, end_block = blocks[:-1], np.cumsum(np.diff(blocks))[::1]
     for i, (_ini_trial, _end_trial) in enumerate(zip(ini_block, end_block)):
         mag = np.abs(y_fft[:, :, _ini_trial: _end_trial])
         ang = np.angle(y_fft[:, :, _ini_trial: _end_trial]).value
         if weighted_average:
-            angular_weights = (mag + regularization_factor * mag.unit) ** 2.0
+            angular_weights = mag ** 2.0
             angular_weights = angular_weights / np.sum(angular_weights, axis=2, keepdims=True)
         else:
             angular_weights = 1.0
 
         norm_r[:, :, i] = np.abs(np.sum((angular_weights * np.exp(1j * ang)), axis=2))
         mean_x = np.sum((mag * angular_weights * np.cos(ang)), axis=2, keepdims=True)
         mean_y = np.sum((mag * angular_weights * np.sin(ang)), axis=2, keepdims=True)
         r[:, :, i] = np.sqrt(mean_x ** 2.0 + mean_y ** 2)[:, :, 0]
         var_x = np.sum(angular_weights * (mag * np.cos(ang) - mean_x) ** 2.0, axis=2)
         var_y = np.sum(angular_weights * (mag * np.sin(ang) - mean_y) ** 2.0, axis=2)
         # we assumed that variance on x and y axis are independent from each other
         # this encapsulates the variance: sigma_r^2 <= variance <= sigma_r^2 + 4 * sum(w_angular*r_i*mean(r_i))
-        total_var[:, :, i] = var_x + var_y + (regularization_factor * mag.unit) ** 2.0
+        total_var[:, :, i] = var_x + var_y
         # purely radial
         # mean_r = np.sum(mag * angular_weights, axis=2, keepdims=True)
         # total_var[:, :, i] = np.sum(angular_weights * (mag - mean_r) ** 2.0, axis=2)
 
         # fig, ax = plt.subplots(subplot_kw={'projection': 'polar'})
         # ax.plot(ang.T.squeeze(), mag.T.squeeze(), 'o')
         # ax.plot(np.angle(mean_x + 1j*mean_y).squeeze(), r[:, :, i].squeeze(), 'o', markersize=8, color='k')
```

### Comparing `peegy-1.3.4/peegy/processing/tools/filters/eegFiltering.py` & `peegy-1.3.6/peegy/processing/tools/filters/eegFiltering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/filters/eog_tools/tools.py` & `peegy-1.3.6/peegy/processing/tools/filters/eog_tools/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
                                        prominence=threshold,
                                        width=1)
     return dirac_peaks
 
 
 def detect_blinks(eog_data: np.array = None,
                   template: np.array = None,
-                  kernel_bandwidth: float = 4 * 0.15
+                  kernel_bandwidth: float = 0.15
                   ):
     """
     This function will use a match filter based on normalized cross correlation to detect the position at which the
     input template matches best.
     :param eog_data: numpy array with eog data
     :param template: template generated from the eog data (see generate_eog_template)
     :param kernel_bandwidth: factor use to control the with of the Gaussian kernel in threshold detection
```

### Comparing `peegy-1.3.4/peegy/processing/tools/filters/resampling.py` & `peegy-1.3.6/peegy/processing/tools/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/filters/spatial_filtering/definitions.py` & `peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py` & `peegy-1.3.6/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/template_generator/auditory_waveforms.py` & `peegy-1.3.6/peegy/processing/tools/template_generator/auditory_waveforms.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/template_generator/h0.json` & `peegy-1.3.6/peegy/processing/tools/template_generator/h0.json`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/video/recording.py` & `peegy-1.3.6/peegy/processing/tools/video/recording.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/processing/tools/weightedAverage.py` & `peegy-1.3.6/peegy/processing/tools/weightedAverage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/artifact_removal/ir_test.py` & `peegy-1.3.6/peegy/test/artifact_removal/ir_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/artifact_removal/regression_artifact_removal.py` & `peegy-1.3.6/peegy/test/artifact_removal/regression_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/artifact_removal/xcorr_artifact_removal.py` & `peegy-1.3.6/peegy/test/artifact_removal/xcorr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/dss_unit_tests.py` & `peegy-1.3.6/peegy/test/dss_unit_tests.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/eeg_test_resampling.py` & `peegy-1.3.6/peegy/test/eeg_test_resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/javerager_test.py` & `peegy-1.3.6/peegy/test/javerager_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/read_data_test.py` & `peegy-1.3.6/peegy/test/read_data_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_assr_moving_average.py` & `peegy-1.3.6/peegy/test/test_assr_moving_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_average_spectrogram_power.py` & `peegy-1.3.6/peegy/test/test_average_spectrogram_power.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_biosemi_class.py` & `peegy-1.3.6/peegy/test/test_biosemi_class.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_biosemi_reader.py` & `peegy-1.3.6/peegy/test/test_biosemi_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_bootstraping.py` & `peegy-1.3.6/peegy/test/test_bootstraping.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_edf_reader.py` & `peegy-1.3.6/peegy/test/test_edf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_eeg_notch_filter.py` & `peegy-1.3.6/peegy/test/test_eeg_notch_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_eog_removal_correlation.py` & `peegy-1.3.6/peegy/test/test_eog_removal_correlation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_eog_template_removal.py` & `peegy-1.3.6/peegy/test/test_eog_template_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_eog_template_valderrama_20118.py` & `peegy-1.3.6/peegy/test/test_eog_template_valderrama_20118.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_et_tools.py` & `peegy-1.3.6/peegy/test/test_et_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_filter.py` & `peegy-1.3.6/peegy/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_fir_filter_mt.py` & `peegy-1.3.6/peegy/test/test_fir_filter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_fir_filter_ols.py` & `peegy-1.3.6/peegy/test/test_fir_filter_ols.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_fiter_mt.py` & `peegy-1.3.6/peegy/test/test_fiter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_freq_noise_estimation.py` & `peegy-1.3.6/peegy/test/test_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_frequency_average_epochs.py` & `peegy-1.3.6/peegy/test/test_frequency_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_hotelling_t2.py` & `peegy-1.3.6/peegy/test/test_hotelling_t2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_ica_average_epochs.py` & `peegy-1.3.6/peegy/test/test_ica_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_multiprocessing.py` & `peegy-1.3.6/peegy/test/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_noise_generator.py` & `peegy-1.3.6/peegy/test/test_noise_generator.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_norm_corr.py` & `peegy-1.3.6/peegy/test/test_norm_corr.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_peakdetection.py` & `peegy-1.3.6/peegy/test/test_peakdetection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_phase_locking_value.py` & `peegy-1.3.6/peegy/test/test_phase_locking_value.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_pooled_freq_noise_estimation.py` & `peegy-1.3.6/peegy/test/test_pooled_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_scrolling.py` & `peegy-1.3.6/peegy/test/test_scrolling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/test/test_spatial_filtering_example1.py` & `peegy-1.3.6/peegy/test/test_spatial_filtering_example1.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,37 +90,37 @@
 
 # clean data using dss with weighted average as bias. Data covariance weighted with same weights
 cref, tw_ref = et_weighted_covariance(data, w=w_w)
 c1, tw1 = et_weighted_covariance(w_ave)
 cref = cref / tw_ref
 c1 = c1 / tw1
 # plot_covariances(covariances=[cref, c1, cref, c1])
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1, keep1=1e-4)
+todss, pwr0, pwr1, n0, n1 = sf.nt_dss0(cref, c1, keep1=1e-4)
 z0 = et_mmat(data, todss)
 cov_1, tw_cov = et_time_shifted_xcovariance(z0, data, wy=w_w)
 cov_1 = cov_1 / tw_cov
 data_clean0 = et_mmat(z0[:, n_components, :], cov_1[n_components, :])
 
 # clean data using dss with standard average as bias and standard average weights for the covariance.
 cref, tw_ref = et_weighted_covariance(data, w=s_w)
 c1, tw1 = et_weighted_covariance(s_ave)
 cref = cref / tw_ref
 c1 = c1 / tw1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1)
+todss, pwr0, pwr1, n0, n1 = sf.nt_dss0(cref, c1)
 z1 = et_mmat(data, todss)
 cov_1, tw_cov = et_time_shifted_xcovariance(z1, data, wy=s_w)
 cov_1 = cov_1 / tw_cov
 data_clean1 = et_mmat(z1[:, n_components, :], cov_1[n_components, :])
 
 # clean data using dss with weighted average as bias. Covariance weighted with standard average weights
 cref, tw_ref = et_weighted_covariance(data, w=s_w)
 c1, tw1 = et_weighted_covariance(w_ave)
 cref = cref / tw_ref
 c1 = c1 / tw1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1, keep1=1e-4)
+todss, pwr0, pwr1, n0, n1 = sf.nt_dss0(cref, c1, keep1=1e-4)
 z2 = et_mmat(data, todss)
 cov_1, tw_cov = et_time_shifted_xcovariance(z2, data, wy=s_w)
 cov_1 = cov_1 / tw_cov
 data_clean2 = et_mmat(z2[:, n_components, :], cov_1[n_components, :])
 
 w_ave_0, *_ = et_mean(data_clean0, block_size=5, weighted=True)
 w_ave_1, *_ = et_mean(data_clean1, block_size=5, weighted=True)
```

### Comparing `peegy-1.3.4/peegy/test/test_spatial_filtering_example6.py` & `peegy-1.3.6/peegy/test/test_spatial_filtering_example6.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 SNR = 10
 noise = np.random.normal(0, 0.1, size=(nsamples, nchans, ntrials))
 n_source = SNR * s / np.std(s)
 data = noise / np.std(noise) + n_source
 
 c0, c1 = sf.nt_bias_fft(data, np.array([f1]) / fs)
 
-todss, pwr0, pwr1 = sf.nt_dss0(c0, c1)
+todss, pwr0, pwr1, n0, n1 = sf.nt_dss0(c0, c1)
 z = eo.et_mmat(data, todss)
 n_components = np.arange(1)
 cov_1 = eo.et_x_covariance(z, data)
 data_clean = eo.et_mmat(z[:, n_components, :], cov_1[n_components, :])
 
 ax = plt.subplot(131)
 ax.plot(np.mean(n_source, axis=2))
```

### Comparing `peegy-1.3.4/peegy/test/test_spatial_filtering_freq_domain.py` & `peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,52 +81,52 @@
 # generate non-stationary noise
 for i in np.arange(1, 4):
     _ini = i*20
     _end = _ini + 10
     scaled_noise[:, :, _ini: _end] += 1e4 * i * scaled_noise[:, :, _ini: _end]
 
 # mix data
-data = scaled_noise + scaled_source
+data = (scaled_noise + scaled_source)
 
 # standard averaging of the data
 s_ave, s_w, s_rn, *_ = et_mean(data, block_size=20, weighted=False)
 # weighted averaging of the data
 w_ave, w_w, w_rn, *_ = et_mean(data, block_size=20, weighted=True)
 n_components = np.arange(1)
 
 # clean data using weighted dss
 n_freq = freq * np.arange(4) / fs
 cref, tref = et_freq_weighted_cov(data, normalized_frequencies=n_freq, w=w_w)
 c1, t1 = et_freq_weighted_cov(w_ave, normalized_frequencies=n_freq)
 cref = cref / tref
 c1 = c1 / t1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1, keep1=1e-5)
+todss, pwr0, pwr1, n_0, n_1 = sf.nt_dss0(cref, c1, keep1=1e-5)
 z0 = et_mmat(data, todss)
 cov_1, tw_cov = et_freq_shifted_xcovariance(z0, data, wy=w_w, normalized_frequencies=n_freq)
 cov_1 = cov_1 / tw_cov
 data_clean0 = et_mmat(z0[:, n_components, :], cov_1[n_components, :])
 
 # clean data using dss with standard average
 cref, tref = et_freq_weighted_cov(data, normalized_frequencies=n_freq, w=s_w)
 c1, t1 = et_freq_weighted_cov(s_ave, normalized_frequencies=n_freq)
 cref = cref / tref
 c1 = c1 / t1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1)
+todss, pwr0, pwr1, n_0, n_1 = sf.nt_dss0(cref, c1)
 z1 = et_mmat(data, todss)
 cov_1, tw_cov = et_freq_shifted_xcovariance(z1, data, wy=s_w, normalized_frequencies=n_freq)
 cov_1 = cov_1 / tw_cov
 data_clean1 = et_mmat(z1[:, n_components, :], cov_1[n_components, :])
 
 
 # clean data using dss only on weighted average
 cref, tref = et_freq_weighted_cov(data, normalized_frequencies=n_freq, w=s_w)
 c1, t1 = et_freq_weighted_cov(w_ave, normalized_frequencies=n_freq)
 cref = cref / tref
 c1 = c1 / t1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1, keep1=1e-5)
+todss, pwr0, pwr1, n_0, n_1 = sf.nt_dss0(cref, c1, keep1=1e-5)
 z2 = et_mmat(data, todss)
 cov_1, tw_cov = et_freq_shifted_xcovariance(z2, data, normalized_frequencies=n_freq, wy=s_w)
 cov_1 = cov_1 / tw_cov
 data_clean2 = et_mmat(z2[:, n_components, :], cov_1[n_components, :])
 
 # plot the results
```

### Comparing `peegy-1.3.4/peegy/test/test_spatial_filtering_freq_domain_2.py` & `peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,38 +104,38 @@
 
 # clean data using weighted dss
 n_freq = frequencies / fs
 cref, tref = et_freq_weighted_cov(data, normalized_frequencies=n_freq, w=w_w)
 c1, t1 = et_freq_weighted_cov(w_ave, normalized_frequencies=n_freq)
 cref = cref / tref
 c1 = c1 / t1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1, keep1=1e-5)
+todss, pwr0, pwr1, n_0, n_1 = sf.nt_dss0(cref, c1, keep1=1e-5)
 z0 = et_mmat(data, todss)
 cov_1, tw_cov = et_freq_shifted_xcovariance(z0, data, wy=w_w, normalized_frequencies=n_freq)
 cov_1 = cov_1 / tw_cov
 data_clean0 = et_mmat(z0[:, n_components, :], cov_1[n_components, :])
 
 # clean data using dss with standard average
 cref, tref = et_freq_weighted_cov(data, normalized_frequencies=n_freq, w=s_w)
 c1, t1 = et_freq_weighted_cov(s_ave, normalized_frequencies=n_freq)
 cref = cref / tref
 c1 = c1 / t1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1)
+todss, pwr0, pwr1, n_0, n_1 = sf.nt_dss0(cref, c1)
 z1 = et_mmat(data, todss)
 cov_1, tw_cov = et_freq_shifted_xcovariance(z1, data, wy=s_w, normalized_frequencies=n_freq)
 cov_1 = cov_1 / tw_cov
 data_clean1 = et_mmat(z1[:, n_components, :], cov_1[n_components, :])
 
 
 # clean data using dss only on weighted average
 cref, tref = et_freq_weighted_cov(data, normalized_frequencies=n_freq, w=s_w)
 c1, t1 = et_freq_weighted_cov(w_ave, normalized_frequencies=n_freq)
 cref = cref / tref
 c1 = c1 / t1
-todss, pwr0, pwr1 = sf.nt_dss0(cref, c1, keep1=1e-5)
+todss, pwr0, pwr1, n_0, n_1 = sf.nt_dss0(cref, c1, keep1=1e-5)
 z2 = et_mmat(data, todss)
 cov_1, tw_cov = et_freq_shifted_xcovariance(z2, data, normalized_frequencies=n_freq, wy=s_w)
 cov_1 = cov_1 / tw_cov
 data_clean2 = et_mmat(z2[:, n_components, :], cov_1[n_components, :])
 
 # plot the results
```

### Comparing `peegy-1.3.4/peegy/test/test_w_average_epochs.py` & `peegy-1.3.6/peegy/test/test_w_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/tools/signal_generator/noise_functions.py` & `peegy-1.3.6/peegy/tools/signal_generator/noise_functions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy/tools/units/unit_tools.py` & `peegy-1.3.6/peegy/tools/units/unit_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/peegy.egg-info/PKG-INFO` & `peegy-1.3.6/peegy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peegy
-Version: 1.3.4
+Version: 1.3.6
 Summary: Tools to pipeline bulk analyses of EEG and other modalities.
 Home-page: https://jundurraga.gitlab.io/peegy/
 Author: Jaime A. Undurraga
 Author-email: jaime.undurraga@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `peegy-1.3.4/peegy.egg-info/SOURCES.txt` & `peegy-1.3.6/peegy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 setup.py
 examples/__init__.py
 examples/example_abr_peak_detection.py
 examples/example_acc_eog_removal_template_.py
 examples/example_acc_peak_detection.py
+examples/example_acc_peak_detection_bootstrap.py
 examples/example_acc_peak_detection_filters.py
 examples/example_acc_video.py
 examples/example_acc_weighted_average.py
 examples/example_acc_weighted_vs_standard_average.py
 examples/example_assr_dss_frequency_domain_bias_test.py
 examples/example_assr_dss_time_domain_bias_test.py
 examples/example_assr_f_test.py
@@ -86,14 +87,16 @@
 peegy/processing/pipe/plot.py
 peegy/processing/pipe/regression.py
 peegy/processing/pipe/simulate.py
 peegy/processing/pipe/spatial_filtering.py
 peegy/processing/pipe/statistics.py
 peegy/processing/pipe/storage.py
 peegy/processing/pipe/time_frequency.py
+peegy/processing/pipe/bootstrap/__init__.py
+peegy/processing/pipe/bootstrap/bootstrap.py
 peegy/processing/statistics/__init__.py
 peegy/processing/statistics/definitions.py
 peegy/processing/statistics/eeg_statistic_tools.py
 peegy/processing/system/__init__.py
 peegy/processing/system/memory.py
 peegy/processing/system/progress.py
 peegy/processing/tools/__init__.py
@@ -138,14 +141,15 @@
 peegy/test/test_eog_template_valderrama_20118.py
 peegy/test/test_et_tools.py
 peegy/test/test_filter.py
 peegy/test/test_fir_filter_mt.py
 peegy/test/test_fir_filter_ols.py
 peegy/test/test_fiter_mt.py
 peegy/test/test_freq_noise_estimation.py
+peegy/test/test_freq_noise_estimation_plots.py
 peegy/test/test_frequency_average_epochs.py
 peegy/test/test_generic_reader.py
 peegy/test/test_hotelling_t2.py
 peegy/test/test_ica_average_epochs.py
 peegy/test/test_multiprocessing.py
 peegy/test/test_noise_generator.py
 peegy/test/test_norm_corr.py
```

### Comparing `peegy-1.3.4/peegy.egg-info/requires.txt` & `peegy-1.3.6/peegy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.3.4/setup.py` & `peegy-1.3.6/setup.py`

 * *Files identical despite different names*

