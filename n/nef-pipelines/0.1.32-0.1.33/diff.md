# Comparing `tmp/nef_pipelines-0.1.32.tar.gz` & `tmp/nef_pipelines-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.32.tar", last modified: Thu Mar 23 08:33:29 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.33.tar", last modified: Sat Apr 15 16:26:08 2023, max compression
```

## Comparing `nef_pipelines-0.1.32.tar` & `nef_pipelines-0.1.33.tar`

### file list

```diff
@@ -1,330 +1,334 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.960477 nef_pipelines-0.1.32/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.813155 nef_pipelines-0.1.32/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.876309 nef_pipelines-0.1.32/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.32/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.893015 nef_pipelines-0.1.32/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.32/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.32/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.32/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.897036 nef_pipelines-0.1.32/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.32/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.32/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.32/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      404 2023-01-30 22:58:25.000000 nef_pipelines-0.1.32/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.32/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.32/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.32/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     2595 2023-03-19 15:56:44.000000 nef_pipelines-0.1.32/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.32/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.32/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-03-23 08:33:29.960808 nef_pipelines-0.1.32/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.32/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.32/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.32/pyproject.toml
--rw-r--r--   0 garythompson   (501) staff       (20)      967 2023-03-23 08:28:05.000000 nef_pipelines-0.1.32/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      318 2023-03-19 15:38:54.000000 nef_pipelines-0.1.32/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1575 2023-03-23 08:33:29.968400 nef_pipelines-0.1.32/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.32/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.814246 nef_pipelines-0.1.32/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.905728 nef_pipelines-0.1.32/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.32/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.939417 nef_pipelines-0.1.32/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-01-31 10:45:30.000000 nef_pipelines-0.1.32/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.991614 nef_pipelines-0.1.32/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2636 2023-03-20 08:57:38.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16036 2023-03-22 17:47:26.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    13851 2023-03-20 21:01:51.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    19514 2023-03-18 23:11:49.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3828 2023-03-19 15:41:24.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8776 2023-02-05 14:12:26.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.997225 nef_pipelines-0.1.32/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20435 2023-03-19 00:08:54.000000 nef_pipelines-0.1.32/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3749 2023-03-22 22:37:49.000000 nef_pipelines-0.1.32/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.997885 nef_pipelines-0.1.32/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.025696 nef_pipelines-0.1.32/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.040809 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.053635 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.054914 nef_pipelines-0.1.32/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.058958 nef_pipelines-0.1.32/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.060112 nef_pipelines-0.1.32/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.064118 nef_pipelines-0.1.32/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.074530 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.094375 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_delete.py
--rwxr--r--   0 garythompson   (501) staff       (20)     1123 2022-12-16 21:06:48.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_tabulate.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.101353 nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.104443 nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.131926 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.180101 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14354 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.218611 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.277501 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.280616 nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.288566 nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.325320 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.335569 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.338041 nef_pipelines-0.1.32/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.377828 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.408979 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    11454 2023-03-19 00:04:43.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.436233 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/test_agv.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7643 2023-03-18 23:11:48.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/test_test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.447845 nef_pipelines-0.1.32/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.468318 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.536357 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.550845 nef_pipelines-0.1.32/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     1479 2023-02-07 13:11:18.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.576686 nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2592 2022-12-13 19:17:42.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.581282 nef_pipelines-0.1.32/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.592436 nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-03-19 00:07:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7769 2023-03-21 21:57:01.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.595840 nef_pipelines-0.1.32/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.602236 nef_pipelines-0.1.32/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10429 2023-03-20 09:03:07.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-03-11 19:52:51.000000 nef_pipelines-0.1.32/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.613191 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.613995 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.620767 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.623679 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.626151 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.628790 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-01-16 22:41:06.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.632192 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.671373 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.674286 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11481 2023-03-19 00:07:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.680460 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.726496 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3373 2023-02-07 21:14:19.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3019 2023-02-07 21:08:19.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20232 2022-11-27 19:45:21.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.737619 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.752554 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.795130 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2196 2022-11-27 19:45:21.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5647 2023-02-07 23:05:11.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.797518 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.802574 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10789 2023-01-30 23:23:18.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.805229 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.807018 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.809351 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.811482 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.839478 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.842812 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6315 2023-02-08 23:35:44.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.845203 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      727 2023-03-20 21:00:52.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.847615 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16042 2023-03-19 15:44:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.857472 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14367 2023-03-21 20:30:29.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.895166 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.897929 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.909119 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.913590 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:29.958004 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-01-11 22:40:51.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-03-23 08:33:28.919110 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-03-23 08:33:28.000000 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    12274 2023-03-23 08:33:28.000000 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-03-23 08:33:28.000000 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-03-23 08:33:28.000000 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-03-23 08:33:28.000000 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-03-23 08:33:28.000000 nef_pipelines-0.1.32/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.32/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.697196 nef_pipelines-0.1.33/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.587116 nef_pipelines-0.1.33/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.651299 nef_pipelines-0.1.33/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.33/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.669834 nef_pipelines-0.1.33/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.33/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.33/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.674463 nef_pipelines-0.1.33/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      404 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.33/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.33/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.33/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     2595 2023-03-19 15:56:44.000000 nef_pipelines-0.1.33/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.33/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.33/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-15 16:26:08.697457 nef_pipelines-0.1.33/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.33/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.33/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.33/pyproject.toml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1002 2023-04-15 16:20:01.000000 nef_pipelines-0.1.33/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      352 2023-04-15 16:14:41.000000 nef_pipelines-0.1.33/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1575 2023-04-15 16:26:08.699523 nef_pipelines-0.1.33/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.33/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.588472 nef_pipelines-0.1.33/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.684162 nef_pipelines-0.1.33/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.33/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.720287 nef_pipelines-0.1.33/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-01-31 10:45:30.000000 nef_pipelines-0.1.33/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.766706 nef_pipelines-0.1.33/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2636 2023-03-20 08:57:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16036 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    13851 2023-03-20 21:01:51.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    19514 2023-03-18 23:11:49.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3828 2023-03-19 15:41:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8776 2023-02-05 14:12:26.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.769913 nef_pipelines-0.1.33/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20435 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5239 2023-03-24 21:55:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.773118 nef_pipelines-0.1.33/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.795419 nef_pipelines-0.1.33/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.807378 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.811151 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.821369 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.824399 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.825363 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.834704 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.844240 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.848060 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64962 2023-04-15 12:23:49.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/ubiquitin_short.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     1123 2022-12-16 21:06:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_tabulate.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.857626 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.880762 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.909017 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.959303 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14354 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.005104 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.072936 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.110021 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.113827 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.115316 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.135901 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.142044 nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.147039 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.174141 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.181592 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/test_agv.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7643 2023-03-18 23:11:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.215656 nef_pipelines-0.1.33/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.239313 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.303883 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.337562 nef_pipelines-0.1.33/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.362146 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2592 2022-12-13 19:17:42.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.368950 nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.387406 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7769 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6717 2023-04-15 16:16:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.394934 nef_pipelines-0.1.33/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.399812 nef_pipelines-0.1.33/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10429 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-03-11 19:52:51.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.403390 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.405781 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.409635 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.414249 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.418012 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.441394 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-01-16 22:41:06.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.446899 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.463966 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.468506 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11481 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.494129 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.504422 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3373 2023-02-07 21:14:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3019 2023-02-07 21:08:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20232 2022-11-27 19:45:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.508925 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.544689 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.556385 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2196 2022-11-27 19:45:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5647 2023-02-07 23:05:11.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.559407 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.566616 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10789 2023-01-30 23:23:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.590782 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.594354 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.600157 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.604192 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.607510 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.611914 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6315 2023-02-08 23:35:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.615278 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      727 2023-03-20 21:00:52.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.646853 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17136 2023-03-24 20:03:59.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.654545 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14367 2023-03-21 20:30:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.657627 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.660883 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.682099 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.687390 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.696048 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.696172 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    12466 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.33/tox.ini
```

### Comparing `nef_pipelines-0.1.32/.github/workflows/ci.yml` & `nef_pipelines-0.1.33/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.33/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/.pre-commit-config.yaml` & `nef_pipelines-0.1.33/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/CHANGELOG.md` & `nef_pipelines-0.1.33/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/CONTRIBUTING.md` & `nef_pipelines-0.1.33/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/LICENSE.txt` & `nef_pipelines-0.1.33/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/PKG-INFO` & `nef_pipelines-0.1.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.32
+Version: 0.1.33
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.32/README.md` & `nef_pipelines-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/TODO.md` & `nef_pipelines-0.1.33/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/release_to_pypi.sh` & `nef_pipelines-0.1.33/release_to_pypi.sh`

 * *Files 16% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 # define where the version file is found
 VERSION_FILE=src/nef_pipelines/VERSION
 
 # cheange to the correct working directory
 cd /Users/garythompson/Dropbox/nef_pipelines/nef_pipelines
 
 #clear dists but don't complain if its empty
+setopt localoptions rmstarsilent
 rm -rf  dist/* || true
 
 # increase version and tag it
 ver  --file $VERSION_FILE  up --patch
-ver  --file $VERSION_FILE tag
+
 
 # grab the version
 VERSION=`ver --file $VERSION_FILE |  awk '{print $3}'`
 
 # update the version  in the repo
 git add src/nef_pipelines/VERSION
 git commit -m "updated version to $VERSION" --no-verify
 
+ver  --file $VERSION_FILE tag
+
 # stash any uncommited changes to avoid version+1 errors
 git stash
 
 #build and publish
 tox -e build  # to build your package distribution
 tox -e publish -- --repository pypi
```

### Comparing `nef_pipelines-0.1.32/setup.cfg` & `nef_pipelines-0.1.33/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/setup.py` & `nef_pipelines-0.1.33/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.33/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/peak_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.33/src/nef_pipelines/lib/util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,41 @@
     STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
 
     result = run_and_report(app, ["--file-name-template", "-"], input=STREAM)
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
+EXPECTED_SUPPRESS_ASSIGNMENT = """\
+****************************** nef_nmr_spectrum_peaks ******************************
+
+       w1       w2      Height  Volume
+
+  120.519  6.169        9       1
+  104.406  6.180       10       2
+  104.408  6.517       11       3
+  103.504  7.048       12       4
+************************************************************************************
+
+"""
+
+
+def test_ppm_out_short_suppress_assigment():
+
+    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
+
+    result = run_and_report(
+        app,
+        ["--file-name-template", "-", "--suppress-column", "assignment"],
+        input=STREAM,
+    )
+
+    assert_lines_match(EXPECTED_SUPPRESS_ASSIGNMENT, result.stdout)
+
+
 EXPECTED_NO_HEIGHT = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
 
 Assignment       w1       w2        Volume
 
   PR_36N-H       120.519  6.169          1
   PR_66N-H       104.406  6.180          2
@@ -52,15 +79,15 @@
 
 
 def test_ppm_out_short_no_height():
 
     STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
 
     result = run_and_report(
-        app, ["--file-name-template", "-", "--no-height"], input=STREAM
+        app, ["--file-name-template", "-", "--suppress-column", "height"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_NO_HEIGHT, result.stdout)
 
 
 EXPECTED_NO_VOLUME = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
@@ -78,15 +105,15 @@
 
 
 def test_ppm_out_short_no_volume():
 
     STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
 
     result = run_and_report(
-        app, ["--file-name-template", "-", "--no-volume"], input=STREAM
+        app, ["--file-name-template", "-", "--suppress-column", "volume"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_NO_VOLUME, result.stdout)
 
 
 EXPECTED_NO_HEIGHT_OR_VOLUME = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
@@ -104,27 +131,42 @@
 
 
 def test_ppm_out_short_no_height_or_volume():
 
     STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
 
     result = run_and_report(
-        app, ["--file-name-template", "-", "--no-volume", "--no-height"], input=STREAM
+        app,
+        [
+            "--file-name-template",
+            "-",
+            "--suppress-column",
+            "volume",
+            "--suppress-column",
+            "height",
+        ],
+        input=STREAM,
     )
 
     assert_lines_match(EXPECTED_NO_HEIGHT_OR_VOLUME, result.stdout)
 
 
 def test_ppm_out_short_no_height_or_volume_with_data():
 
     STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
 
     result = run_and_report(
         app,
-        ["--file-name-template", "-", "--no-volume", "--no-height", "--add-data"],
+        [
+            "--file-name-template",
+            "-",
+            "--suppress-column",
+            "volume,height",
+            "--add-data",
+        ],
         input=STREAM,
     )
 
     assert_lines_match(EXPECTED_NO_HEIGHT_OR_VOLUME, result.stdout)
 
 
 EXPECTED_DIFFERENT_RESIDUES = """\
```

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/about.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,58 @@
+import platform
 import sys
 from datetime import date
 from textwrap import dedent, indent
 
 import typer
 
 from nef_pipelines import nef_app
 from nef_pipelines.lib.util import get_version
 
+VERBOSE_HELP = """\
+    display more verbose information about NEF-Pipelines and its environment,
+    [ignored with the --version option]"
+"""
+
 if nef_app:
     # noinspection PyUnusedLocal
     @nef_app.app.command()
     def about(
         version: bool = typer.Option(
             False, "--version", help="only display the current version"
-        )
+        ),
+        verbose: bool = typer.Option(False, "-v", "--verbose", help=VERBOSE_HELP),
     ):
         "- info about NEF-Pipelines"
 
-        print(cmd(version), file=sys.stderr)
+        print(cmd(version, verbose), file=sys.stderr)
 
-    def cmd(version):
+    def cmd(version, verbose=False):
         version_data = get_version()
 
         if version:
             result = str(version_data)
         else:
             NEF_PIPLINES_URL = "https://github.com/varioustoxins/NEF-Pipelines"
+
+            if verbose:
+                # TODO add the modules in requirements.txt and their versions
+                extra_msg = f"""\
+
+                    Environment
+                    -----------
+
+                    Python version:   {platform.python_version()}
+                    Operating system: {platform.platform(aliased=True, terse=True)}
+
+                """
+            else:
+                extra_msg = ""
+            extra_msg = dedent(extra_msg)
+
             msg = f"""\
 
                 This is NEF-Pipelines version {version_data}
 
                 For information about this program and the code please see: {NEF_PIPLINES_URL}
                 For bug reporting please goto: {NEF_PIPLINES_URL}/issues
 
@@ -43,10 +66,12 @@
 
             msg = dedent(msg)
 
             max_width = max([len(line) for line in msg.split("\n")])
 
             header = "=" * (max_width + 4)
 
-            result = "\n".join([header, indent(msg, "  "), header])
+            result = "\n".join(
+                [header, indent(msg, "  "), indent(extra_msg, "  "), header]
+            )
 
         return result
```

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,9 @@
         help="-  carry out operations on frames in nef frames",
     )
 
     # import of specific importers must be after app creation to avoid circular imports
     import nef_pipelines.tools.frames.delete  # noqa: F401
     import nef_pipelines.tools.frames.insert  # noqa: F401
     import nef_pipelines.tools.frames.list  # noqa: F401
+    import nef_pipelines.tools.frames.rename  # noqa: F401
     import nef_pipelines.tools.frames.tabulate  # noqa: F401
```

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.33/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/pdbx/importers/sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # TODO move some of this to a spark lib
 import re
 import sys
+from enum import auto
 from os.path import commonprefix
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 import typer
 from pynmrstar import Entry, Loop
+from strenum import LowercaseStrEnum
 from tabulate import tabulate
 
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     read_entry_from_file_or_stdin_or_exit_error,
     select_frames_by_name,
 )
@@ -93,14 +95,26 @@
     "[default: @-.@65-1..CA -> PR_65p1CA with this option @-.@65-1..CA -> ?CA]"
 )
 
 DISCARD_ASSIGNMENTS_HELP = (
     "discard the peak assignments. note: peaks unassign provides more options"
 )
 
+
+class SUPRESSABLE_COLUMNS(LowercaseStrEnum):
+    ASSIGNMENT = auto()
+    HEIGHT = auto()
+    VOLUME = auto()
+
+
+COLUMNS_TO_SUPPRESS_HELP = f"""
+    name columns to suppress in the output [{', '.join(SUPRESSABLE_COLUMNS)}], can be called multiple times or with a
+    comma sepatated list [no spaces!]
+"""
+
 DEFAULT_CHAIN_SEPARATOR = "."
 
 
 # noinspection PyUnusedLocal
 @export_app.command()
 def peaks(
     file_name_template: str = typer.Option(
@@ -122,23 +136,29 @@
     full_assignments: bool = typer.Option(False, help=FULL_ASSIGNMENTS_HELP),
     add_data: bool = typer.Option(False, help=ADD_DATA_HELP),
     no_chains: bool = typer.Option(False, help=NO_CHAINS_HELP),
     chain_separator: str = typer.Option(
         DEFAULT_CHAIN_SEPARATOR, help="characters used to separate chains from residues"
     ),
     no_negative_residues: bool = typer.Option(False, help=NO_NEGATIVES_HELP),
-    no_volume: bool = typer.Option(
-        False, help="don't include a volume column in the output"
-    ),
-    no_height: bool = typer.Option(
-        False, help="don't include a height column in the output"
+    columns_to_suppress: List[str] = typer.Option(
+        [], "--suppress-column", help=COLUMNS_TO_SUPPRESS_HELP
     ),
+    # no_volume: bool = typer.Option(
+    #     False, help="don't include a volume column in the output"
+    # ),
+    # no_height: bool = typer.Option(
+    #     False, help="don't include a height column in the output"
+    # ),
+    # no_assignment: bool = Typer
 ):
     """-  write sparky peaks"""
 
+    columns_to_suppress = parse_comma_separated_options(columns_to_suppress)
+
     output_to_files = file_name_template != STDOUT_STR
 
     frame_selectors = parse_comma_separated_options(frame_selectors)
 
     if len(frame_selectors) == 0:
         frame_selectors = [
             "*",
@@ -166,16 +186,15 @@
             selected_frame_names,
             include_assignments=not discard_assignments,
             include_full_assignments=full_assignments,
             show_data_tag_in_header=add_data,
             chain_separator=chain_separator,
             no_negative_pseudo_residues=no_negative_residues,
             no_chains=no_chains,
-            no_height=no_height,
-            no_volume=no_volume,
+            columns_to_suppress=columns_to_suppress,
         )
     except SparkyPeaksExportException as e:
         exit_error(str(e))
 
     sparky_tables = _map_frame_names_to_paths_if_required(
         sparky_tables, frame_name_to_file_name, output_to_files
     )
@@ -298,16 +317,15 @@
     selected_frame_names: List[str],
     include_assignments=True,
     include_full_assignments: bool = False,
     show_data_tag_in_header=False,
     chain_separator=":",
     no_negative_pseudo_residues=False,
     no_chains=False,
-    no_volume=False,
-    no_height=False,
+    columns_to_suppress: List[SUPRESSABLE_COLUMNS] = (),
 ) -> Tuple[Entry, Dict[str, List[str]]]:
 
     selected_frame_names = set(selected_frame_names)
 
     spectrum_frames = entry.get_saveframes_by_category(SPECTRUM_CATEGORY)
 
     names_and_frames = {
@@ -328,16 +346,15 @@
             peaks,
             include_assignments=include_assignments,
             abbreviate_assignments=not include_full_assignments,
             show_data_tag_in_header=show_data_tag_in_header,
             chain_sequence_separator=chain_separator,
             no_negative_pseudo_residues=no_negative_pseudo_residues,
             no_chains=no_chains,
-            no_heights=no_height,
-            no_volumes=no_volume,
+            columns_to_suppress=columns_to_suppress,
         )
 
     return entry, sparky_lines
 
 
 def _check_column_has_floats(peak_list: List[NewPeak], column_name: str):
     result = False
@@ -363,33 +380,40 @@
     peaks_list: List[NewPeak],
     include_assignments=False,
     abbreviate_assignments=False,
     show_data_tag_in_header=False,
     chain_sequence_separator=".",
     no_negative_pseudo_residues=False,
     no_chains=False,
-    no_volumes=False,
-    no_heights=False,
+    columns_to_suppress=(),
 ):
 
     lines = []
 
-    header = ["Assignment"]
+    header = []
+    if SUPRESSABLE_COLUMNS.ASSIGNMENT not in columns_to_suppress:
+        header.append("Assignment")
 
     if len(peaks_list) > 0:
         num_dimensions = len(peaks_list[0].shifts)
 
         position_headers = [
             f"w{dimension}" for dimension in range(1, num_dimensions + 1)
         ]
 
         header.extend(position_headers)
 
-        has_volumes = _peak_loop_has_volumes(peaks_list) and not no_volumes
-        has_heights = _peak_loop_has_heights(peaks_list) and not no_heights
+        has_volumes = (
+            _peak_loop_has_volumes(peaks_list)
+            and SUPRESSABLE_COLUMNS.VOLUME not in columns_to_suppress
+        )
+        has_heights = (
+            _peak_loop_has_heights(peaks_list)
+            and SUPRESSABLE_COLUMNS.HEIGHT not in columns_to_suppress
+        )
 
         if (has_heights or has_volumes) and show_data_tag_in_header:
             header.append("Data")
 
         if has_heights:
             header.append("Height")
 
@@ -412,80 +436,81 @@
             )
             number_chains = len(
                 set([shift.atom.residue.chain_code for shift in peak.shifts])
             )
 
             can_abbreviate = number_residues == 1 and number_chains == 1
 
-            if include_assignments:
-                for atom in [shift.atom for shift in peak.shifts]:
-
-                    chain_code = atom.residue.chain_code
-                    sequence_code = str(atom.residue.sequence_code)
-                    residue_name = atom.residue.residue_name
-                    atom_name = atom.atom_name
-                    current_chain_sequence_separator = chain_sequence_separator
-
-                    if chain_code == "@-":
-                        chain_code = ""
-                    elif chain_code.startswith("#"):
-                        chain_code = f"PC_{chain_code}"
-                    elif chain_code == UNUSED or no_chains:
-                        chain_code = ""
-                        current_chain_sequence_separator = ""
-
-                    if not chain_code or len(chain_code) == 0:
-                        current_chain_sequence_separator = ""
-
-                    if sequence_code.endswith("-1"):
-                        if no_negative_pseudo_residues:
-                            sequence_code = "?"
-                        else:
-                            sequence_code = f"{sequence_code[:-2]}"
-                            atom_name = f"{atom_name}m1"
-                        can_abbreviate = False
-
-                    if sequence_code.startswith("@"):
-                        sequence_code = f"PR_{sequence_code[1:]}"
-                    # if chain_code.startswith('PC_'):
-                    #     sequence_code = f'{chain_code}:{sequence_code}'
-                    #     chain_sequence_separator = ''
-
-                    if residue_name in TRANSLATIONS_3_1:
-                        residue_name = TRANSLATIONS_3_1[residue_name]
-
-                    if not residue_name:
-                        residue_name = ""
-
-                    group = f"{chain_code}{current_chain_sequence_separator}{residue_name}{sequence_code}"
-
-                    assignment = f"{group}{atom_name}"
-                    assignments.append(assignment)
-
-            else:
-                assignments.extend(["?"] * num_dimensions)
-
-            common_prefix = commonprefix(assignments)
-            need_to_join = True
-            if common_prefix != "?" and abbreviate_assignments and can_abbreviate:
-
-                split_common_prefix = re.split(r"(\d+)", common_prefix)
-                common_prefix = f"{split_common_prefix[0]}{split_common_prefix[1]}"
-
-                if len(common_prefix) > 0 and common_prefix != "?":
-                    for i, assignment in enumerate(assignments):
-                        assignments[i] = assignment[len(common_prefix) :]
+            if SUPRESSABLE_COLUMNS.ASSIGNMENT not in columns_to_suppress:
+                if include_assignments:
+                    for atom in [shift.atom for shift in peak.shifts]:
+
+                        chain_code = atom.residue.chain_code
+                        sequence_code = str(atom.residue.sequence_code)
+                        residue_name = atom.residue.residue_name
+                        atom_name = atom.atom_name
+                        current_chain_sequence_separator = chain_sequence_separator
+
+                        if chain_code == "@-":
+                            chain_code = ""
+                        elif chain_code.startswith("#"):
+                            chain_code = f"PC_{chain_code}"
+                        elif chain_code == UNUSED or no_chains:
+                            chain_code = ""
+                            current_chain_sequence_separator = ""
+
+                        if not chain_code or len(chain_code) == 0:
+                            current_chain_sequence_separator = ""
+
+                        if sequence_code.endswith("-1"):
+                            if no_negative_pseudo_residues:
+                                sequence_code = "?"
+                            else:
+                                sequence_code = f"{sequence_code[:-2]}"
+                                atom_name = f"{atom_name}m1"
+                            can_abbreviate = False
+
+                        if sequence_code.startswith("@"):
+                            sequence_code = f"PR_{sequence_code[1:]}"
+                        # if chain_code.startswith('PC_'):
+                        #     sequence_code = f'{chain_code}:{sequence_code}'
+                        #     chain_sequence_separator = ''
+
+                        if residue_name in TRANSLATIONS_3_1:
+                            residue_name = TRANSLATIONS_3_1[residue_name]
+
+                        if not residue_name:
+                            residue_name = ""
+
+                        group = f"{chain_code}{current_chain_sequence_separator}{residue_name}{sequence_code}"
+
+                        assignment = f"{group}{atom_name}"
+                        assignments.append(assignment)
+
+                else:
+                    assignments.extend(["?"] * num_dimensions)
+
+                common_prefix = commonprefix(assignments)
+                need_to_join = True
+                if common_prefix != "?" and abbreviate_assignments and can_abbreviate:
+
+                    split_common_prefix = re.split(r"(\d+)", common_prefix)
+                    common_prefix = f"{split_common_prefix[0]}{split_common_prefix[1]}"
+
+                    if len(common_prefix) > 0 and common_prefix != "?":
+                        for i, assignment in enumerate(assignments):
+                            assignments[i] = assignment[len(common_prefix) :]
 
-                    assignments = f"{common_prefix}{'-'.join(assignments)}"
-                    need_to_join = False
+                        assignments = f"{common_prefix}{'-'.join(assignments)}"
+                        need_to_join = False
 
-            if need_to_join:
-                assignments = "-".join(assignments)
+                if need_to_join:
+                    assignments = "-".join(assignments)
 
-            out_row.append(assignments)
+                out_row.append(assignments)
 
             out_row.extend([f"{shift.value:7.3f}" for shift in peak.shifts])
 
             if (has_heights or has_volumes) and show_data_tag_in_header:
                 out_row.append("")
             if has_heights:
                 height = peak.height if peak.height != UNUSED else 0.000
```

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.33/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef-pipelines
-Version: 0.1.32
+Version: 0.1.33
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.32/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.33/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,19 @@
 src/nef_pipelines/tests/csv/test_data/short_complete.csv
 src/nef_pipelines/tests/fasta/test_sequence.py
 src/nef_pipelines/tests/fasta/test_data/3aa.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
 src/nef_pipelines/tests/frames/__init__.py
 src/nef_pipelines/tests/frames/test_delete.py
 src/nef_pipelines/tests/frames/test_list.py
+src/nef_pipelines/tests/frames/test_rename.py
 src/nef_pipelines/tests/frames/test_tabulate.py
 src/nef_pipelines/tests/frames/test_data/frames.nef
 src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+src/nef_pipelines/tests/frames/test_data/ubiquitin_short.nef
 src/nef_pipelines/tests/mars/__init__.py
 src/nef_pipelines/tests/mars/test_export_shifts.py
 src/nef_pipelines/tests/mars/test_import_shifts.py
 src/nef_pipelines/tests/mars/test_data/sec5_short.neff
 src/nef_pipelines/tests/mars/test_data/sec5_short.txt
 src/nef_pipelines/tests/nmrpipe/__init__.py
 src/nef_pipelines/tests/nmrpipe/test_gdb.py
@@ -139,14 +141,15 @@
 src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
 src/nef_pipelines/tests/test_data/3a_ab.neff
+src/nef_pipelines/tests/test_data/empty.nef
 src/nef_pipelines/tests/test_data/header.nef
 src/nef_pipelines/tests/test_data/multi_chain.nef
 src/nef_pipelines/tests/test_data/nef_3_peaks.nef
 src/nef_pipelines/tests/test_data/tailin_seq_short.nef
 src/nef_pipelines/tests/test_data/test_agv.neff
 src/nef_pipelines/tests/xcamshift/test_export_shifts.py
 src/nef_pipelines/tests/xplor/test_dihedrals.py
@@ -184,14 +187,15 @@
 src/nef_pipelines/tools/chains/renumber.py
 src/nef_pipelines/tools/entry/__init__.py
 src/nef_pipelines/tools/entry/rename.py
 src/nef_pipelines/tools/frames/__init__.py
 src/nef_pipelines/tools/frames/delete.py
 src/nef_pipelines/tools/frames/insert.py
 src/nef_pipelines/tools/frames/list.py
+src/nef_pipelines/tools/frames/rename.py
 src/nef_pipelines/tools/frames/tabulate.py
 src/nef_pipelines/tools/peaks/match.py
 src/nef_pipelines/tools/shifts/__init__.py
 src/nef_pipelines/tools/shifts/make_peaks.py
 src/nef_pipelines/transcoders/__init__.py
 src/nef_pipelines/transcoders/csv/__init__.py
 src/nef_pipelines/transcoders/csv/importers/__init__.py
```

### Comparing `nef_pipelines-0.1.32/tox.ini` & `nef_pipelines-0.1.33/tox.ini`

 * *Files identical despite different names*

