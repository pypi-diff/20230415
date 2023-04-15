# Comparing `tmp/microt_preprocessing-0.1.8.tar.gz` & `tmp/microt_preprocessing-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microt_preprocessing-0.1.8.tar", last modified: Tue May 31 12:29:03 2022, max compression
+gzip compressed data, was "microt_preprocessing-0.1.9.tar", last modified: Thu Jun  2 22:58:17 2022, max compression
```

## Comparing `microt_preprocessing-0.1.8.tar` & `microt_preprocessing-0.1.9.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.799190 microt_preprocessing-0.1.8/
--rw-rw-rw-   0        0        0     1108 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     9257 2022-05-31 12:29:03.799190 microt_preprocessing-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8544 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.713190 microt_preprocessing-0.1.8/microt_preprocessing.egg-info/
--rw-rw-rw-   0        0        0     9257 2022-05-31 12:29:03.000000 microt_preprocessing-0.1.8/microt_preprocessing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8636 2022-05-31 12:29:03.000000 microt_preprocessing-0.1.8/microt_preprocessing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-31 12:29:03.000000 microt_preprocessing-0.1.8/microt_preprocessing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-05-31 12:29:03.000000 microt_preprocessing-0.1.8/microt_preprocessing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      782 2022-05-31 12:29:03.802190 microt_preprocessing-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1075 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.716190 microt_preprocessing-0.1.8/time_study_preprocessing_main/
--rw-rw-rw-   0        0        0      171 2022-04-21 03:06:46.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/__init__.py
--rw-rw-rw-   0        0        0       21 2022-05-31 12:26:27.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/_version.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.717189 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/
--rw-rw-rw-   0        0        0       63 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.717189 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.719190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/GPS/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/GPS/__init__.py
--rw-rw-rw-   0        0        0     4813 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/GPS/main.py
--rw-rw-rw-   0        0        0     1046 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/GPS/parse.py
--rw-rw-rw-   0        0        0        0 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.721190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/__init__.py
--rw-rw-rw-   0        0        0     4142 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/main.py
--rw-rw-rw-   0        0        0     1044 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.723190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/__init__.py
--rw-rw-rw-   0        0        0     4154 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/main.py
--rw-rw-rw-   0        0        0     2027 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.727188 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/__init__.py
--rw-rw-rw-   0        0        0     4135 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/main.py
--rw-rw-rw-   0        0        0     1595 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.729190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/__init__.py
--rw-rw-rw-   0        0        0     4136 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/main.py
--rw-rw-rw-   0        0        0     1075 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.731191 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/battery/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/battery/__init__.py
--rw-rw-rw-   0        0        0     4129 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/battery/main.py
--rw-rw-rw-   0        0        0     1493 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/battery/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.734190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/__init__.py
--rw-rw-rw-   0        0        0     5681 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/main.py
--rw-rw-rw-   0        0        0     1913 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.736190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/__init__.py
--rw-rw-rw-   0        0        0     5676 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/main.py
--rw-rw-rw-   0        0        0     4343 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.738190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/__init__.py
--rw-rw-rw-   0        0        0     2218 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/main.py
--rw-rw-rw-   0        0        0        0 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.740190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/__init__.py
--rw-rw-rw-   0        0        0     4316 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/main.py
--rw-rw-rw-   0        0        0     1135 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.743193 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/__init__.py
--rw-rw-rw-   0        0        0     5180 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/main.py
--rw-rw-rw-   0        0        0     1860 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.746190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/__init__.py
--rw-rw-rw-   0        0        0     4139 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/main.py
--rw-rw-rw-   0        0        0     1082 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.748192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/__init__.py
--rw-rw-rw-   0        0        0     3127 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/main.py
--rw-rw-rw-   0        0        0     1046 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.750192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/__init__.py
--rw-rw-rw-   0        0        0     4173 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/main.py
--rw-rw-rw-   0        0        0     1564 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.752192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/__init__.py
--rw-rw-rw-   0        0        0     4140 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/main.py
--rw-rw-rw-   0        0        0     4223 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.754192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/__init__.py
--rw-rw-rw-   0        0        0     3793 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/main.py
--rw-rw-rw-   0        0        0     3265 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.758191 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/__init__.py
--rw-rw-rw-   0        0        0     4102 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/main.py
--rw-rw-rw-   0        0        0     1090 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.760192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/__init__.py
--rw-rw-rw-   0        0        0     4094 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/main.py
--rw-rw-rw-   0        0        0     1351 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.762192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/step_count/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/step_count/__init__.py
--rw-rw-rw-   0        0        0     4135 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/step_count/main.py
--rw-rw-rw-   0        0        0     1088 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/step_count/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.764192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/__init__.py
--rw-rw-rw-   0        0        0     4146 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/main.py
--rw-rw-rw-   0        0        0     1956 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.773193 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/
--rw-rw-rw-   0        0        0      247 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/__init__.py
--rw-rw-rw-   0        0        0     2140 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/convert_timestamp.py
--rw-rw-rw-   0        0        0      350 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/fix_nulls.py
--rw-rw-rw-   0        0        0      930 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/get_time_zone.py
--rw-rw-rw-   0        0        0     2239 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/output_summary_report.py
--rw-rw-rw-   0        0        0     4732 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/parse_cml_argv.py
--rw-rw-rw-   0        0        0     1150 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/parse_information.py
--rw-rw-rw-   0        0        0     1724 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/parse_participants.py
--rw-rw-rw-   0        0        0     3191 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/validate_dates.py
--rw-rw-rw-   0        0        0     1478 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/validate_hours.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.774192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/
--rw-rw-rw-   0        0        0       87 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.781190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/
--rw-rw-rw-   0        0        0     1689 2022-05-30 19:17:28.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_hour.py
--rw-rw-rw-   0        0        0     5500 2022-05-31 12:16:51.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_minute.py
--rw-rw-rw-   0        0        0     1714 2022-05-30 14:00:18.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_hour.py
--rw-rw-rw-   0        0        0     3615 2022-05-30 14:00:18.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_minute.py
--rw-rw-rw-   0        0        0      255 2022-05-30 17:36:51.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/__init__.py
--rw-rw-rw-   0        0        0     1468 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/bafToCSV.py
--rw-rw-rw-   0        0        0     3357 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/baf_to_dataframe.py
--rw-rw-rw-   0        0        0     2780 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/csvToMIMS.py
--rw-rw-rw-   0        0        0     1925 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/dataframe_to_MIMS.py
--rw-rw-rw-   0        0        0    14182 2022-05-31 12:25:49.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/main.py
--rw-rw-rw-   0        0        0      963 2022-05-30 14:52:23.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.784192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/
--rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/__init__.py
--rw-rw-rw-   0        0        0     4250 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/main.py
--rw-rw-rw-   0        0        0     1241 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.788191 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/
--rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/__init__.py
--rw-rw-rw-   0        0        0     3764 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/main.py
--rw-rw-rw-   0        0        0     1329 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.790189 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/power_status/
--rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/power_status/__init__.py
--rw-rw-rw-   0        0        0     3797 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/power_status/main.py
--rw-rw-rw-   0        0        0     1887 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/power_status/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.792192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/
--rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/__init__.py
--rw-rw-rw-   0        0        0     3752 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/main.py
--rw-rw-rw-   0        0        0     2428 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.794192 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/
--rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/__init__.py
--rw-rw-rw-   0        0        0     4019 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/main.py
--rw-rw-rw-   0        0        0     1337 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.796190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/
--rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/__init__.py
--rw-rw-rw-   0        0        0     3578 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/main.py
--rw-rw-rw-   0        0        0     1199 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/parse.py
-drwxrwxrwx   0        0        0        0 2022-05-31 12:29:03.798190 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/
--rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/__init__.py
--rw-rw-rw-   0        0        0     3771 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/main.py
--rw-rw-rw-   0        0        0     1618 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/parse.py
--rw-rw-rw-   0        0        0     5987 2022-04-21 03:08:00.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocessing_all_ema.py
--rw-rw-rw-   0        0        0     4353 2022-04-21 03:08:00.000000 microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocessing_all_uema.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.636202 microt_preprocessing-0.1.9/
+-rw-rw-rw-   0        0        0     1108 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     9257 2022-06-02 22:58:17.637202 microt_preprocessing-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8544 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.275878 microt_preprocessing-0.1.9/microt_preprocessing.egg-info/
+-rw-rw-rw-   0        0        0     9257 2022-06-02 22:58:16.000000 microt_preprocessing-0.1.9/microt_preprocessing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8636 2022-06-02 22:58:17.000000 microt_preprocessing-0.1.9/microt_preprocessing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-02 22:58:16.000000 microt_preprocessing-0.1.9/microt_preprocessing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2022-06-02 22:58:17.000000 microt_preprocessing-0.1.9/microt_preprocessing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      782 2022-06-02 22:58:17.640203 microt_preprocessing-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.313793 microt_preprocessing-0.1.9/time_study_preprocessing_main/
+-rw-rw-rw-   0        0        0      171 2022-04-21 03:06:46.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/__init__.py
+-rw-rw-rw-   0        0        0       21 2022-06-02 22:56:54.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/_version.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.320089 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/
+-rw-rw-rw-   0        0        0       63 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.320089 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.332088 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/GPS/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/GPS/__init__.py
+-rw-rw-rw-   0        0        0     4813 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/GPS/main.py
+-rw-rw-rw-   0        0        0     1046 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/GPS/parse.py
+-rw-rw-rw-   0        0        0        0 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.340088 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/__init__.py
+-rw-rw-rw-   0        0        0     4142 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/main.py
+-rw-rw-rw-   0        0        0     1044 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.349087 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/__init__.py
+-rw-rw-rw-   0        0        0     4154 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/main.py
+-rw-rw-rw-   0        0        0     2027 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.359450 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/__init__.py
+-rw-rw-rw-   0        0        0     4135 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/main.py
+-rw-rw-rw-   0        0        0     1595 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.368450 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/__init__.py
+-rw-rw-rw-   0        0        0     4136 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/main.py
+-rw-rw-rw-   0        0        0     1075 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.377452 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/battery/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/battery/__init__.py
+-rw-rw-rw-   0        0        0     4129 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/battery/main.py
+-rw-rw-rw-   0        0        0     1493 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/battery/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.386451 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/__init__.py
+-rw-rw-rw-   0        0        0     5681 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/main.py
+-rw-rw-rw-   0        0        0     1913 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.395452 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/__init__.py
+-rw-rw-rw-   0        0        0     5676 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/main.py
+-rw-rw-rw-   0        0        0     4343 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.401452 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/__init__.py
+-rw-rw-rw-   0        0        0     2218 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/main.py
+-rw-rw-rw-   0        0        0        0 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.409452 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/__init__.py
+-rw-rw-rw-   0        0        0     4316 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/main.py
+-rw-rw-rw-   0        0        0     1135 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.418450 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/__init__.py
+-rw-rw-rw-   0        0        0     5180 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/main.py
+-rw-rw-rw-   0        0        0     1860 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.427451 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/__init__.py
+-rw-rw-rw-   0        0        0     4139 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/main.py
+-rw-rw-rw-   0        0        0     1082 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.433474 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/__init__.py
+-rw-rw-rw-   0        0        0     3127 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/main.py
+-rw-rw-rw-   0        0        0     1046 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.442118 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/__init__.py
+-rw-rw-rw-   0        0        0     4173 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/main.py
+-rw-rw-rw-   0        0        0     1564 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.452118 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/__init__.py
+-rw-rw-rw-   0        0        0     4140 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/main.py
+-rw-rw-rw-   0        0        0     4223 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.462055 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/__init__.py
+-rw-rw-rw-   0        0        0     3793 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/main.py
+-rw-rw-rw-   0        0        0     3265 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.470451 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/__init__.py
+-rw-rw-rw-   0        0        0     4102 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/main.py
+-rw-rw-rw-   0        0        0     1090 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.479451 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/__init__.py
+-rw-rw-rw-   0        0        0     4094 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/main.py
+-rw-rw-rw-   0        0        0     1351 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.488453 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/step_count/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/step_count/__init__.py
+-rw-rw-rw-   0        0        0     4135 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/step_count/main.py
+-rw-rw-rw-   0        0        0     1088 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/step_count/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.496934 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/__init__.py
+-rw-rw-rw-   0        0        0     4146 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/main.py
+-rw-rw-rw-   0        0        0     1956 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.532745 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/
+-rw-rw-rw-   0        0        0      247 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/__init__.py
+-rw-rw-rw-   0        0        0     2140 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/convert_timestamp.py
+-rw-rw-rw-   0        0        0      350 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/fix_nulls.py
+-rw-rw-rw-   0        0        0      930 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/get_time_zone.py
+-rw-rw-rw-   0        0        0     2239 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/output_summary_report.py
+-rw-rw-rw-   0        0        0     4732 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/parse_cml_argv.py
+-rw-rw-rw-   0        0        0     1150 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/parse_information.py
+-rw-rw-rw-   0        0        0     1724 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/parse_participants.py
+-rw-rw-rw-   0        0        0     3191 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/validate_dates.py
+-rw-rw-rw-   0        0        0     1478 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/validate_hours.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.535746 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/
+-rw-rw-rw-   0        0        0       87 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.571502 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/
+-rw-rw-rw-   0        0        0     1689 2022-05-30 19:17:28.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_hour.py
+-rw-rw-rw-   0        0        0     5515 2022-06-02 22:56:54.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_minute.py
+-rw-rw-rw-   0        0        0     1714 2022-05-30 14:00:18.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_hour.py
+-rw-rw-rw-   0        0        0     3615 2022-05-30 14:00:18.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_minute.py
+-rw-rw-rw-   0        0        0      255 2022-05-30 17:36:51.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/__init__.py
+-rw-rw-rw-   0        0        0     1468 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/bafToCSV.py
+-rw-rw-rw-   0        0        0     3357 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/baf_to_dataframe.py
+-rw-rw-rw-   0        0        0     2780 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/csvToMIMS.py
+-rw-rw-rw-   0        0        0     1925 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/dataframe_to_MIMS.py
+-rw-rw-rw-   0        0        0    14225 2022-06-02 22:55:30.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/main.py
+-rw-rw-rw-   0        0        0      963 2022-05-30 14:52:23.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.581502 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/
+-rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/__init__.py
+-rw-rw-rw-   0        0        0     4250 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/main.py
+-rw-rw-rw-   0        0        0     1241 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.590502 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/
+-rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/__init__.py
+-rw-rw-rw-   0        0        0     3764 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/main.py
+-rw-rw-rw-   0        0        0     1329 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.598503 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/power_status/
+-rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/power_status/__init__.py
+-rw-rw-rw-   0        0        0     3797 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/power_status/main.py
+-rw-rw-rw-   0        0        0     1887 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/power_status/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.608503 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/
+-rw-rw-rw-   0        0        0       39 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/__init__.py
+-rw-rw-rw-   0        0        0     3752 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/main.py
+-rw-rw-rw-   0        0        0     2428 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.618202 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/
+-rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/__init__.py
+-rw-rw-rw-   0        0        0     4019 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/main.py
+-rw-rw-rw-   0        0        0     1337 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.626202 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/
+-rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/__init__.py
+-rw-rw-rw-   0        0        0     3578 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/main.py
+-rw-rw-rw-   0        0        0     1199 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/parse.py
+drwxrwxrwx   0        0        0        0 2022-06-02 22:58:17.635202 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/
+-rw-rw-rw-   0        0        0       41 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/__init__.py
+-rw-rw-rw-   0        0        0     3771 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/main.py
+-rw-rw-rw-   0        0        0     1618 2022-03-21 15:20:43.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/parse.py
+-rw-rw-rw-   0        0        0     5987 2022-04-21 03:08:00.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocessing_all_ema.py
+-rw-rw-rw-   0        0        0     4353 2022-04-21 03:08:00.000000 microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocessing_all_uema.py
```

### Comparing `microt_preprocessing-0.1.8/LICENSE.txt` & `microt_preprocessing-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/PKG-INFO` & `microt_preprocessing-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microt_preprocessing
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package that transforms raw sensor data collected from Time study app into intermediate CSV file for analysis of various purposes
 Home-page: https://bitbucket.org/mhealthresearchgroup/microt_preprocessing/src/master/
 Author: Jixin Li, Aditya Ponnada
 Author-email: li.jix@northeastern.edu
 Project-URL: Bug Tracker, https://bitbucket.org/mhealthresearchgroup/microt_preprocessing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `microt_preprocessing-0.1.8/README.md` & `microt_preprocessing-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/microt_preprocessing.egg-info/PKG-INFO` & `microt_preprocessing-0.1.9/microt_preprocessing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microt-preprocessing
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package that transforms raw sensor data collected from Time study app into intermediate CSV file for analysis of various purposes
 Home-page: https://bitbucket.org/mhealthresearchgroup/microt_preprocessing/src/master/
 Author: Jixin Li, Aditya Ponnada
 Author-email: li.jix@northeastern.edu
 Project-URL: Bug Tracker, https://bitbucket.org/mhealthresearchgroup/microt_preprocessing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `microt_preprocessing-0.1.8/microt_preprocessing.egg-info/SOURCES.txt` & `microt_preprocessing-0.1.9/microt_preprocessing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/setup.cfg` & `microt_preprocessing-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6963 726f 745f 7072 6570 726f   = microt_prepro
 00000020: 6365 7373 696e 670d 0a76 6572 7369 6f6e  cessing..version
-00000030: 203d 2030 2e31 2e38 0d0a 6175 7468 6f72   = 0.1.8..author
+00000030: 203d 2030 2e31 2e39 0d0a 6175 7468 6f72   = 0.1.9..author
 00000040: 203d 204a 6978 696e 204c 692c 2041 6469   = Jixin Li, Adi
 00000050: 7479 6120 506f 6e6e 6164 610d 0a61 7574  tya Ponnada..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6c69 2e6a  hor_email = li.j
 00000070: 6978 406e 6f72 7468 6561 7374 6572 6e2e  ix@northeastern.
 00000080: 6564 750d 0a64 6573 6372 6970 7469 6f6e  edu..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6861   = A package tha
 000000a0: 7420 7472 616e 7366 6f72 6d73 2072 6177  t transforms raw
```

### Comparing `microt_preprocessing-0.1.8/setup.py` & `microt_preprocessing-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/GPS/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/GPS/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/GPS/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/GPS/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ambient_press_sensor/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_usage/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/app_use_duration/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/apps_installed/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/battery/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/battery/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/battery/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/battery/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/burst_status/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_notes/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/daily_report/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/detected_activity/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/dnd_status/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/light_sensor/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/location_cluster_json/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/notif_logs/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/phone_broadcasts/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/prompt_response/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/proximity_sensor/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/ringer_mode/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/step_count/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/step_count/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/step_count/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/step_count/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/phone/wifi_state/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/convert_timestamp.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/convert_timestamp.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/get_time_zone.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/get_time_zone.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/output_summary_report.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/output_summary_report.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/parse_cml_argv.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/parse_cml_argv.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/parse_information.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/parse_information.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/parse_participants.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/parse_participants.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/validate_dates.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/validate_dates.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/utils/validate_hours.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/utils/validate_hours.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_hour.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_hour.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_minute.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/AUC_minute.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,17 @@
     datetime_list = convert_timestamp_int_list_to_readable_time(df_auc_day[2], list(tz_set_clean)[0])
     # print(datetime_list)
     for ts in datetime_list:
         time_str_components = ts.split(" ")[1].split(":")
         if len(ts.split(" ")) == 3:
             try:
                 hour_list.append(int(time_str_components[0]))
-            except ValueError:
-                print(hour_list)
-                raise ValueError
+            except ValueError as ee:
+                print("valueError===="+hour_list)
+                raise ee
             minute_list.append(int(time_str_components[1]))
         else:
             hour_list.append(NAN)
             minute_list.append(NAN)
 
     df_auc_day.loc[:, "Hour"] = hour_list
     df_auc_day.loc[:, "Minute"] = minute_list
```

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_hour.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_hour.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_minute.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/MIMS_minute.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/bafToCSV.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/bafToCSV.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/baf_to_dataframe.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/baf_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/csvToMIMS.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/csvToMIMS.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/dataframe_to_MIMS.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/dataframe_to_MIMS.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,17 +237,17 @@
                     # time_zone = get_time_zone(hour_folder_path)
                     # step 2.1: read target hourly file
                     target_file_matched = list(glob(path.join(hour_folder_path, "Watch-AccelSampling*")))
                     # binary_df = None
                     if len(target_file_matched) > 0:
                         target_file_path = target_file_matched[0]
                         try:
-                            df_hour_auc = pd.read_csv(target_file_path, header=None, on_bad_lines='skip')
+                            df_hour_auc = pd.read_csv(target_file_path, header=None, error_bad_lines=False, warn_bad_lines=True)
                         except (pd.errors.ParserError, pd.errors.EmptyDataError) as ee:
-                            print(target_file_path)
+                            print("EmptyDataError---"+target_file_path)
                             raise ee
                         df_participant_auc = pd.concat([df_participant_auc, df_hour_auc])
 
                 df_participant_auc.reset_index(inplace=True, drop=True)
                 df_auc_minute = get_auc_matrix_minute(df_participant_auc)
                 if df_auc_minute is not None:
                     df_auc_minute.to_csv(day_file_name_auc_minute, index=False)
```

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/accelerometer/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/battery_level/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/dnd_status/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/power_status/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/power_status/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/power_status/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/power_status/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/prompt_response/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/sampling_rate/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/uema_undo_counts/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/main.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/main.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/parse.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocess_scripts/watch/watch_accel_sampling/parse.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocessing_all_ema.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocessing_all_ema.py`

 * *Files identical despite different names*

### Comparing `microt_preprocessing-0.1.8/time_study_preprocessing_main/preprocessing_all_uema.py` & `microt_preprocessing-0.1.9/time_study_preprocessing_main/preprocessing_all_uema.py`

 * *Files identical despite different names*

