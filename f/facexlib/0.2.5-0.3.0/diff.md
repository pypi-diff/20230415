# Comparing `tmp/facexlib-0.2.5.tar.gz` & `tmp/facexlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facexlib-0.2.5.tar", last modified: Wed Aug 31 02:12:50 2022, max compression
+gzip compressed data, was "facexlib-0.3.0.tar", last modified: Sat Apr 15 06:51:52 2023, max compression
```

## Comparing `facexlib-0.2.5.tar` & `facexlib-0.3.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.537948 facexlib-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-08-31 02:11:59.000000 facexlib-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-31 02:11:59.000000 facexlib-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5169 2022-08-31 02:12:50.537948 facexlib-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4011 2022-08-31 02:11:59.000000 facexlib-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-31 02:11:59.000000 facexlib-0.2.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.529948 facexlib-0.2.5/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    16024 2022-08-31 02:11:59.000000 facexlib-0.2.5/assets/icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     9798 2022-08-31 02:11:59.000000 facexlib-0.2.5/assets/icon_small.png
--rw-r--r--   0 runner    (1001) docker     (121)   106650 2022-08-31 02:11:59.000000 facexlib-0.2.5/assets/landmarks_5.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   319183 2022-08-31 02:11:59.000000 facexlib-0.2.5/assets/landmarks_68.png
--rw-r--r--   0 runner    (1001) docker     (121)   492547 2022-08-31 02:11:59.000000 facexlib-0.2.5/assets/landmarks_98.png
--rw-r--r--   0 runner    (1001) docker     (121)    36969 2022-08-31 02:11:59.000000 facexlib-0.2.5/assets/test.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    55353 2022-08-31 02:11:59.000000 facexlib-0.2.5/assets/test2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.529948 facexlib-0.2.5/facexlib/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.529948 facexlib-0.2.5/facexlib/alignment/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/alignment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12351 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/alignment/awing_arch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/alignment/convert_98_to_68_landmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.529948 facexlib-0.2.5/facexlib/assessment/
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/assessment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11146 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/assessment/hyperiqa_net.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.529948 facexlib-0.2.5/facexlib/detection/
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7941 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (121)     8109 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/detection/matlab_cp2tform.py
--rw-r--r--   0 runner    (1001) docker     (121)    13240 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/detection/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/detection/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (121)    16452 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/detection/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.529948 facexlib-0.2.5/facexlib/headpose/
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/headpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/headpose/hopenet_arch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.533948 facexlib-0.2.5/facexlib/matting/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/matting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2570 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/matting/backbone.py
--rw-r--r--   0 runner    (1001) docker     (121)     6647 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/matting/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9798 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/matting/modnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.533948 facexlib-0.2.5/facexlib/parsing/
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (121)     6477 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.533948 facexlib-0.2.5/facexlib/recognition/
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/recognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8862 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/recognition/arcface_arch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.533948 facexlib-0.2.5/facexlib/tracking/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/tracking/data_association.py
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/tracking/kalman_tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/tracking/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.533948 facexlib-0.2.5/facexlib/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17282 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    10192 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-08-31 02:12:50.000000 facexlib-0.2.5/facexlib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.533948 facexlib-0.2.5/facexlib/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/visualization/vis_alignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/visualization/vis_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/visualization/vis_headpose.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.533948 facexlib-0.2.5/facexlib/weights/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-31 02:11:59.000000 facexlib-0.2.5/facexlib/weights/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.529948 facexlib-0.2.5/facexlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5169 2022-08-31 02:12:50.000000 facexlib-0.2.5/facexlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-08-31 02:12:50.000000 facexlib-0.2.5/facexlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 02:12:50.000000 facexlib-0.2.5/facexlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 02:12:49.000000 facexlib-0.2.5/facexlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-31 02:12:50.000000 facexlib-0.2.5/facexlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-31 02:12:50.000000 facexlib-0.2.5/facexlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.537948 facexlib-0.2.5/inference/
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_alignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_crop_standard_faces.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_headpose.py
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_hyperiqa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_matting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_parsing_parsenet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_recognition.py
--rw-r--r--   0 runner    (1001) docker     (121)     3657 2022-08-31 02:11:59.000000 facexlib-0.2.5/inference/inference_tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-31 02:11:59.000000 facexlib-0.2.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 02:12:50.537948 facexlib-0.2.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-08-31 02:11:59.000000 facexlib-0.2.5/scripts/crop_faces_5landmarks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-08-31 02:11:59.000000 facexlib-0.2.5/scripts/extract_detection_info_ffhq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-08-31 02:11:59.000000 facexlib-0.2.5/scripts/get_ffhq_template.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-08-31 02:12:50.537948 facexlib-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-08-31 02:11:59.000000 facexlib-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.807753 facexlib-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 06:51:04.000000 facexlib-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 06:51:04.000000 facexlib-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-15 06:51:52.807753 facexlib-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-15 06:51:04.000000 facexlib-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 06:51:04.000000 facexlib-0.3.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.799753 facexlib-0.3.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-04-15 06:51:04.000000 facexlib-0.3.0/assets/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-15 06:51:04.000000 facexlib-0.3.0/assets/icon_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106650 2023-04-15 06:51:04.000000 facexlib-0.3.0/assets/landmarks_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   319183 2023-04-15 06:51:04.000000 facexlib-0.3.0/assets/landmarks_68.png
+-rw-r--r--   0 runner    (1001) docker     (123)   492547 2023-04-15 06:51:04.000000 facexlib-0.3.0/assets/landmarks_98.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36969 2023-04-15 06:51:04.000000 facexlib-0.3.0/assets/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55353 2023-04-15 06:51:04.000000 facexlib-0.3.0/assets/test2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.799753 facexlib-0.3.0/facexlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/alignment/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/alignment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/alignment/awing_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/alignment/convert_98_to_68_landmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/assessment/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/assessment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/assessment/hyperiqa_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/detection/matlab_cp2tform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/detection/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/detection/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/detection/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/headpose/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/headpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/headpose/hopenet_arch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/matting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/matting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/matting/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/matting/mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/matting/modnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/recognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/recognition/arcface_arch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/tracking/data_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/tracking/kalman_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/tracking/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.807753 facexlib-0.3.0/facexlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 06:51:52.000000 facexlib-0.3.0/facexlib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.807753 facexlib-0.3.0/facexlib/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/visualization/vis_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/visualization/vis_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/visualization/vis_headpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.807753 facexlib-0.3.0/facexlib/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 06:51:04.000000 facexlib-0.3.0/facexlib/weights/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.803753 facexlib-0.3.0/facexlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-15 06:51:52.000000 facexlib-0.3.0/facexlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-15 06:51:52.000000 facexlib-0.3.0/facexlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 06:51:52.000000 facexlib-0.3.0/facexlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 06:51:51.000000 facexlib-0.3.0/facexlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-15 06:51:52.000000 facexlib-0.3.0/facexlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 06:51:52.000000 facexlib-0.3.0/facexlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.807753 facexlib-0.3.0/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_crop_standard_faces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_headpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_hyperiqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_matting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_parsing_parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-15 06:51:04.000000 facexlib-0.3.0/inference/inference_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-15 06:51:04.000000 facexlib-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 06:51:52.807753 facexlib-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-15 06:51:04.000000 facexlib-0.3.0/scripts/crop_faces_5landmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-15 06:51:04.000000 facexlib-0.3.0/scripts/extract_detection_info_ffhq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-15 06:51:04.000000 facexlib-0.3.0/scripts/get_ffhq_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-15 06:51:52.807753 facexlib-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-15 06:51:04.000000 facexlib-0.3.0/setup.py
```

### Comparing `facexlib-0.2.5/LICENSE` & `facexlib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/PKG-INFO` & `facexlib-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: facexlib
-Version: 0.2.5
+Version: 0.3.0
 Summary: Basic face library
 Home-page: https://github.com/xinntao/facexlib
 Author: Xintao Wang
 Author-email: xintao.wang@outlook.com
 License: Apache License 2.0
 Description: # ![icon](assets/icon_small.png) FaceXLib
         
         [![PyPI](https://img.shields.io/pypi/v/facexlib)](https://pypi.org/project/facexlib/)
         [![download](https://img.shields.io/github/downloads/xinntao/facexlib/total.svg)](https://github.com/xinntao/facexlib/releases)
         [![Open issue](https://img.shields.io/github/issues/xinntao/facexlib)](https://github.com/xinntao/facexlib/issues)
         [![Closed issue](https://img.shields.io/github/issues-closed/xinntao/facexlib)](https://github.com/xinntao/facexlib/issues)
         [![LICENSE](https://img.shields.io/github/license/xinntao/facexlib.svg)](https://github.com/xinntao/facexlib/blob/master/LICENSE)
         [![python lint](https://github.com/xinntao/facexlib/actions/workflows/pylint.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/pylint.yml)
         [![Publish-pip](https://github.com/xinntao/facexlib/actions/workflows/publish-pip.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/publish-pip.yml)
-        [![gitee mirror](https://github.com/xinntao/facexlib/actions/workflows/gitee-mirror.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/gitee-mirror.yml)
         
-        [English](README.md) **|** [简体中文](README_CN.md) &emsp; [GitHub](https://github.com/xinntao/facexlib) **|** [Gitee码云](https://gitee.com/xinntao/facexlib)
+        [English](README.md) **|** [简体中文](README_CN.md)
         
         ---
         
-        **facexlib** aims at providing ready-to-use **face-related** functions based on current STOA open-source methods. <br>
+        **facexlib** aims at providing ready-to-use **face-related** functions based on current SOTA open-source methods. <br>
         Only PyTorch reference codes are available. For training or fine-tuning, please refer to their original repositories listed below. <br>
         Note that we just provide a collection of these algorithms. You need to refer to their original LICENCEs for your intended use.
         
         If facexlib is helpful in your projects, please help to :star: this repo. Thanks:blush: <br>
         Other recommended projects: &emsp; :arrow_forward: [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) &emsp; :arrow_forward: [GFPGAN](https://github.com/TencentARC/GFPGAN) &emsp; :arrow_forward: [BasicSR](https://github.com/xinntao/BasicSR)
         
         ---
```

### Comparing `facexlib-0.2.5/README.md` & `facexlib-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 [![PyPI](https://img.shields.io/pypi/v/facexlib)](https://pypi.org/project/facexlib/)
 [![download](https://img.shields.io/github/downloads/xinntao/facexlib/total.svg)](https://github.com/xinntao/facexlib/releases)
 [![Open issue](https://img.shields.io/github/issues/xinntao/facexlib)](https://github.com/xinntao/facexlib/issues)
 [![Closed issue](https://img.shields.io/github/issues-closed/xinntao/facexlib)](https://github.com/xinntao/facexlib/issues)
 [![LICENSE](https://img.shields.io/github/license/xinntao/facexlib.svg)](https://github.com/xinntao/facexlib/blob/master/LICENSE)
 [![python lint](https://github.com/xinntao/facexlib/actions/workflows/pylint.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/pylint.yml)
 [![Publish-pip](https://github.com/xinntao/facexlib/actions/workflows/publish-pip.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/publish-pip.yml)
-[![gitee mirror](https://github.com/xinntao/facexlib/actions/workflows/gitee-mirror.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/gitee-mirror.yml)
 
-[English](README.md) **|** [简体中文](README_CN.md) &emsp; [GitHub](https://github.com/xinntao/facexlib) **|** [Gitee码云](https://gitee.com/xinntao/facexlib)
+[English](README.md) **|** [简体中文](README_CN.md)
 
 ---
 
-**facexlib** aims at providing ready-to-use **face-related** functions based on current STOA open-source methods. <br>
+**facexlib** aims at providing ready-to-use **face-related** functions based on current SOTA open-source methods. <br>
 Only PyTorch reference codes are available. For training or fine-tuning, please refer to their original repositories listed below. <br>
 Note that we just provide a collection of these algorithms. You need to refer to their original LICENCEs for your intended use.
 
 If facexlib is helpful in your projects, please help to :star: this repo. Thanks:blush: <br>
 Other recommended projects: &emsp; :arrow_forward: [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) &emsp; :arrow_forward: [GFPGAN](https://github.com/TencentARC/GFPGAN) &emsp; :arrow_forward: [BasicSR](https://github.com/xinntao/BasicSR)
 
 ---
```

### Comparing `facexlib-0.2.5/assets/icon.png` & `facexlib-0.3.0/assets/icon.png`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/assets/icon_small.png` & `facexlib-0.3.0/assets/icon_small.png`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/assets/landmarks_5.jpg` & `facexlib-0.3.0/assets/landmarks_5.jpg`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/assets/landmarks_68.png` & `facexlib-0.3.0/assets/landmarks_68.png`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/assets/landmarks_98.png` & `facexlib-0.3.0/assets/landmarks_98.png`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/assets/test.jpg` & `facexlib-0.3.0/assets/test.jpg`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/assets/test2.jpg` & `facexlib-0.3.0/assets/test2.jpg`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/alignment/__init__.py` & `facexlib-0.3.0/facexlib/alignment/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .convert_98_to_68_landmarks import landmark_98_to_68
 
 __all__ = ['FAN', 'landmark_98_to_68']
 
 
 def init_alignment_model(model_name, half=False, device='cuda', model_rootpath=None):
     if model_name == 'awing_fan':
-        model = FAN(num_modules=4, num_landmarks=98)
+        model = FAN(num_modules=4, num_landmarks=98, device=device)
         model_url = 'https://github.com/xinntao/facexlib/releases/download/v0.1.0/alignment_WFLW_4HG.pth'
     else:
         raise NotImplementedError(f'{model_name} is not implemented.')
 
     model_path = load_file_from_url(
         url=model_url, model_dir='facexlib/weights', progress=True, file_name=None, save_dir=model_rootpath)
     model.load_state_dict(torch.load(model_path)['state_dict'], strict=True)
```

### Comparing `facexlib-0.2.5/facexlib/alignment/awing_arch.py` & `facexlib-0.3.0/facexlib/alignment/awing_arch.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,27 +52,27 @@
 
     def forward(self, input_tensor, heatmap=None):
         """
         input_tensor: (batch, c, x_dim, y_dim)
         """
         batch_size_tensor = input_tensor.shape[0]
 
-        xx_ones = torch.ones([1, self.y_dim], dtype=torch.int32).cuda()
+        xx_ones = torch.ones([1, self.y_dim], dtype=torch.int32, device=input_tensor.device)
         xx_ones = xx_ones.unsqueeze(-1)
 
-        xx_range = torch.arange(self.x_dim, dtype=torch.int32).unsqueeze(0).cuda()
+        xx_range = torch.arange(self.x_dim, dtype=torch.int32, device=input_tensor.device).unsqueeze(0)
         xx_range = xx_range.unsqueeze(1)
 
         xx_channel = torch.matmul(xx_ones.float(), xx_range.float())
         xx_channel = xx_channel.unsqueeze(-1)
 
-        yy_ones = torch.ones([1, self.x_dim], dtype=torch.int32).cuda()
+        yy_ones = torch.ones([1, self.x_dim], dtype=torch.int32, device=input_tensor.device)
         yy_ones = yy_ones.unsqueeze(1)
 
-        yy_range = torch.arange(self.y_dim, dtype=torch.int32).unsqueeze(0).cuda()
+        yy_range = torch.arange(self.y_dim, dtype=torch.int32, device=input_tensor.device).unsqueeze(0)
         yy_range = yy_range.unsqueeze(-1)
 
         yy_channel = torch.matmul(yy_range.float(), yy_ones.float())
         yy_channel = yy_channel.unsqueeze(-1)
 
         xx_channel = xx_channel.permute(0, 3, 2, 1)
         yy_channel = yy_channel.permute(0, 3, 2, 1)
@@ -89,16 +89,16 @@
         if self.with_boundary and heatmap is not None:
             boundary_channel = torch.clamp(heatmap[:, -1:, :, :], 0.0, 1.0)
 
             zero_tensor = torch.zeros_like(xx_channel)
             xx_boundary_channel = torch.where(boundary_channel > 0.05, xx_channel, zero_tensor)
             yy_boundary_channel = torch.where(boundary_channel > 0.05, yy_channel, zero_tensor)
         if self.with_boundary and heatmap is not None:
-            xx_boundary_channel = xx_boundary_channel.cuda()
-            yy_boundary_channel = yy_boundary_channel.cuda()
+            xx_boundary_channel = xx_boundary_channel.to(input_tensor.device)
+            yy_boundary_channel = yy_boundary_channel.to(input_tensor.device)
         ret = torch.cat([input_tensor, xx_channel, yy_channel], dim=1)
 
         if self.with_r:
             rr = torch.sqrt(torch.pow(xx_channel, 2) + torch.pow(yy_channel, 2))
             rr = rr / torch.max(rr)
             ret = torch.cat([ret, rr], dim=1)
 
@@ -264,16 +264,17 @@
     def forward(self, x, heatmap):
         x, last_channel = self.coordconv(x, heatmap)
         return self._forward(self.depth, x), last_channel
 
 
 class FAN(nn.Module):
 
-    def __init__(self, num_modules=1, end_relu=False, gray_scale=False, num_landmarks=68):
+    def __init__(self, num_modules=1, end_relu=False, gray_scale=False, num_landmarks=68, device='cuda'):
         super(FAN, self).__init__()
+        self.device = device
         self.num_modules = num_modules
         self.gray_scale = gray_scale
         self.end_relu = end_relu
         self.num_landmarks = num_landmarks
 
         # Base part
         if self.gray_scale:
@@ -351,22 +352,22 @@
             if i < self.num_modules - 1:
                 ll = self._modules['bl' + str(i)](ll)
                 tmp_out_ = self._modules['al' + str(i)](tmp_out)
                 previous = previous + ll + tmp_out_
 
         return outputs, boundary_channels
 
-    def get_landmarks(self, img, device='cuda'):
+    def get_landmarks(self, img):
         H, W, _ = img.shape
         offset = W / 64, H / 64, 0, 0
 
         img = cv2.resize(img, (256, 256))
         inp = img[..., ::-1]
         inp = torch.from_numpy(np.ascontiguousarray(inp.transpose((2, 0, 1)))).float()
-        inp = inp.to(device)
+        inp = inp.to(self.device)
         inp.div_(255.0).unsqueeze_(0)
 
         outputs, _ = self.forward(inp)
         out = outputs[-1][:, :-1, :, :]
         heatmaps = out.detach().cpu().numpy()
 
         pred = calculate_points(heatmaps).reshape(-1, 2)
```

### Comparing `facexlib-0.2.5/facexlib/alignment/convert_98_to_68_landmarks.py` & `facexlib-0.3.0/facexlib/alignment/convert_98_to_68_landmarks.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/assessment/__init__.py` & `facexlib-0.3.0/facexlib/assessment/__init__.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/assessment/hyperiqa_net.py` & `facexlib-0.3.0/facexlib/assessment/hyperiqa_net.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/detection/__init__.py` & `facexlib-0.3.0/facexlib/detection/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 from facexlib.utils import load_file_from_url
 from .retinaface import RetinaFace
 
 
 def init_detection_model(model_name, half=False, device='cuda', model_rootpath=None):
     if model_name == 'retinaface_resnet50':
-        model = RetinaFace(network_name='resnet50', half=half)
+        model = RetinaFace(network_name='resnet50', half=half, device=device)
         model_url = 'https://github.com/xinntao/facexlib/releases/download/v0.1.0/detection_Resnet50_Final.pth'
     elif model_name == 'retinaface_mobile0.25':
-        model = RetinaFace(network_name='mobile0.25', half=half)
+        model = RetinaFace(network_name='mobile0.25', half=half, device=device)
         model_url = 'https://github.com/xinntao/facexlib/releases/download/v0.1.0/detection_mobilenet0.25_Final.pth'
     else:
         raise NotImplementedError(f'{model_name} is not implemented.')
 
     model_path = load_file_from_url(
         url=model_url, model_dir='facexlib/weights', progress=True, file_name=None, save_dir=model_rootpath)
```

### Comparing `facexlib-0.2.5/facexlib/detection/align_trans.py` & `facexlib-0.3.0/facexlib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/detection/matlab_cp2tform.py` & `facexlib-0.3.0/facexlib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/detection/retinaface.py` & `facexlib-0.3.0/facexlib/detection/retinaface.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from torchvision.models._utils import IntermediateLayerGetter as IntermediateLayerGetter
 
 from facexlib.detection.align_trans import get_reference_facial_points, warp_and_crop_face
 from facexlib.detection.retinaface_net import FPN, SSH, MobileNetV1, make_bbox_head, make_class_head, make_landmark_head
 from facexlib.detection.retinaface_utils import (PriorBox, batched_decode, batched_decode_landm, decode, decode_landm,
                                                  py_cpu_nms)
 
-device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-
 
 def generate_config(network_name):
 
     cfg_mnet = {
         'name': 'mobilenet0.25',
         'min_sizes': [[16, 32], [64, 128], [256, 512]],
         'steps': [8, 16, 32],
@@ -68,26 +66,28 @@
         return cfg_re50
     else:
         raise NotImplementedError(f'network_name={network_name}')
 
 
 class RetinaFace(nn.Module):
 
-    def __init__(self, network_name='resnet50', half=False, phase='test'):
+    def __init__(self, network_name='resnet50', half=False, phase='test', device=None):
+        self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu') if device is None else device
+
         super(RetinaFace, self).__init__()
         self.half_inference = half
         cfg = generate_config(network_name)
         self.backbone = cfg['name']
 
         self.model_name = f'retinaface_{network_name}'
         self.cfg = cfg
         self.phase = phase
         self.target_size, self.max_size = 1600, 2150
         self.resize, self.scale, self.scale1 = 1., None, None
-        self.mean_tensor = torch.tensor([[[[104.]], [[117.]], [[123.]]]]).to(device)
+        self.mean_tensor = torch.tensor([[[[104.]], [[117.]], [[123.]]]], device=self.device)
         self.reference = get_reference_facial_points(default_square=True)
         # Build network.
         backbone = None
         if cfg['name'] == 'mobilenet0.25':
             backbone = MobileNetV1()
             self.body = IntermediateLayerGetter(backbone, cfg['return_layers'])
         elif cfg['name'] == 'Resnet50':
@@ -108,15 +108,15 @@
         self.ssh2 = SSH(out_channels, out_channels)
         self.ssh3 = SSH(out_channels, out_channels)
 
         self.ClassHead = make_class_head(fpn_num=3, inchannels=cfg['out_channel'])
         self.BboxHead = make_bbox_head(fpn_num=3, inchannels=cfg['out_channel'])
         self.LandmarkHead = make_landmark_head(fpn_num=3, inchannels=cfg['out_channel'])
 
-        self.to(device)
+        self.to(self.device)
         self.eval()
         if self.half_inference:
             self.half()
 
     def forward(self, inputs):
         out = self.body(inputs)
 
@@ -141,27 +141,27 @@
         else:
             output = (bbox_regressions, F.softmax(classifications, dim=-1), ldm_regressions)
         return output
 
     def __detect_faces(self, inputs):
         # get scale
         height, width = inputs.shape[2:]
-        self.scale = torch.tensor([width, height, width, height], dtype=torch.float32).to(device)
+        self.scale = torch.tensor([width, height, width, height], dtype=torch.float32, device=self.device)
         tmp = [width, height, width, height, width, height, width, height, width, height]
-        self.scale1 = torch.tensor(tmp, dtype=torch.float32).to(device)
+        self.scale1 = torch.tensor(tmp, dtype=torch.float32, device=self.device)
 
         # forawrd
-        inputs = inputs.to(device)
+        inputs = inputs.to(self.device)
         if self.half_inference:
             inputs = inputs.half()
         loc, conf, landmarks = self(inputs)
 
         # get priorbox
         priorbox = PriorBox(self.cfg, image_size=inputs.shape[2:])
-        priors = priorbox.forward().to(device)
+        priors = priorbox.forward().to(self.device)
 
         return loc, conf, landmarks, priors
 
     # single image detection
     def transform(self, image, use_origin_size):
         # convert to opencv format
         if isinstance(image, Image.Image):
@@ -193,15 +193,15 @@
         self,
         image,
         conf_threshold=0.8,
         nms_threshold=0.4,
         use_origin_size=True,
     ):
         image, self.resize = self.transform(image, use_origin_size)
-        image = image.to(device)
+        image = image.to(self.device)
         if self.half_inference:
             image = image.half()
         image = image - self.mean_tensor
 
         loc, conf, landmarks, priors = self.__detect_faces(image)
 
         boxes = decode(loc.data.squeeze(0), priors.data, self.cfg['variance'])
@@ -312,15 +312,15 @@
         Returns:
             final_bounding_boxes: list of np.array ([n_boxes, 5],
                 type=np.float32).
             final_landmarks: list of np.array ([n_boxes, 10], type=np.float32).
         """
         # self.t['forward_pass'].tic()
         frames, self.resize = self.batched_transform(frames, use_origin_size)
-        frames = frames.to(device)
+        frames = frames.to(self.device)
         frames = frames - self.mean_tensor
 
         b_loc, b_conf, b_landmarks, priors = self.__detect_faces(frames)
 
         final_bounding_boxes, final_landmarks = [], []
 
         # decode
```

### Comparing `facexlib-0.2.5/facexlib/detection/retinaface_net.py` & `facexlib-0.3.0/facexlib/detection/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/detection/retinaface_utils.py` & `facexlib-0.3.0/facexlib/detection/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/headpose/__init__.py` & `facexlib-0.3.0/facexlib/headpose/__init__.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/headpose/hopenet_arch.py` & `facexlib-0.3.0/facexlib/headpose/hopenet_arch.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/matting/__init__.py` & `facexlib-0.3.0/facexlib/matting/__init__.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/matting/backbone.py` & `facexlib-0.3.0/facexlib/matting/backbone.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/matting/mobilenetv2.py` & `facexlib-0.3.0/facexlib/matting/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/matting/modnet.py` & `facexlib-0.3.0/facexlib/matting/modnet.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/parsing/__init__.py` & `facexlib-0.3.0/facexlib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/parsing/bisenet.py` & `facexlib-0.3.0/facexlib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/parsing/parsenet.py` & `facexlib-0.3.0/facexlib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/parsing/resnet.py` & `facexlib-0.3.0/facexlib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/recognition/__init__.py` & `facexlib-0.3.0/facexlib/recognition/__init__.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/recognition/arcface_arch.py` & `facexlib-0.3.0/facexlib/recognition/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/tracking/data_association.py` & `facexlib-0.3.0/facexlib/tracking/data_association.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/tracking/kalman_tracker.py` & `facexlib-0.3.0/facexlib/tracking/kalman_tracker.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/tracking/sort.py` & `facexlib-0.3.0/facexlib/tracking/sort.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/utils/face_restoration_helper.py` & `facexlib-0.3.0/facexlib/utils/face_restoration_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             h, w = int(h / scale), int(w / scale)
             input_img = cv2.resize(self.input_img, (w, h), interpolation=cv2.INTER_LANCZOS4)
 
         with torch.no_grad():
             bboxes = self.face_det.detect_faces(input_img, 0.97) * scale
         for bbox in bboxes:
             # remove faces with too small eye distance: side faces or too small faces
-            eye_dist = np.linalg.norm([bbox[6] - bbox[8], bbox[7] - bbox[9]])
+            eye_dist = np.linalg.norm([bbox[5] - bbox[7], bbox[6] - bbox[8]])
             if eye_dist_threshold is not None and (eye_dist < eye_dist_threshold):
                 continue
 
             if self.template_3points:
                 landmark = np.array([[bbox[i], bbox[i + 1]] for i in range(5, 11, 2)])
             else:
                 landmark = np.array([[bbox[i], bbox[i + 1]] for i in range(5, 15, 2)])
```

### Comparing `facexlib-0.2.5/facexlib/utils/face_utils.py` & `facexlib-0.3.0/facexlib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/utils/misc.py` & `facexlib-0.3.0/facexlib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/visualization/vis_detection.py` & `facexlib-0.3.0/facexlib/visualization/vis_detection.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/facexlib/visualization/vis_headpose.py` & `facexlib-0.3.0/facexlib/visualization/vis_headpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         height, width = img.shape[:2]
         tdx = width / 2
         tdy = height / 2
 
     # X axis pointing to right, drawn in red
     x1 = size * (cos(yaw) * cos(roll)) + tdx
     y1 = size * (cos(pitch) * sin(roll) + cos(roll) * sin(pitch) * sin(yaw)) + tdy
-    # Y axis poiting downside, drawn in green
+    # Y axis pointing downside, drawn in green
     x2 = size * (-cos(yaw) * sin(roll)) + tdx
     y2 = size * (cos(pitch) * cos(roll) - sin(pitch) * sin(yaw) * sin(roll)) + tdy
     # Z axis, out of the screen, drawn in blue
     x3 = size * (sin(yaw)) + tdx
     y3 = size * (-cos(yaw) * sin(pitch)) + tdy
 
     cv2.line(img, (int(tdx), int(tdy)), (int(x1), int(y1)), (0, 0, 255), 3)
```

### Comparing `facexlib-0.2.5/facexlib.egg-info/PKG-INFO` & `facexlib-0.3.0/facexlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: facexlib
-Version: 0.2.5
+Version: 0.3.0
 Summary: Basic face library
 Home-page: https://github.com/xinntao/facexlib
 Author: Xintao Wang
 Author-email: xintao.wang@outlook.com
 License: Apache License 2.0
 Description: # ![icon](assets/icon_small.png) FaceXLib
         
         [![PyPI](https://img.shields.io/pypi/v/facexlib)](https://pypi.org/project/facexlib/)
         [![download](https://img.shields.io/github/downloads/xinntao/facexlib/total.svg)](https://github.com/xinntao/facexlib/releases)
         [![Open issue](https://img.shields.io/github/issues/xinntao/facexlib)](https://github.com/xinntao/facexlib/issues)
         [![Closed issue](https://img.shields.io/github/issues-closed/xinntao/facexlib)](https://github.com/xinntao/facexlib/issues)
         [![LICENSE](https://img.shields.io/github/license/xinntao/facexlib.svg)](https://github.com/xinntao/facexlib/blob/master/LICENSE)
         [![python lint](https://github.com/xinntao/facexlib/actions/workflows/pylint.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/pylint.yml)
         [![Publish-pip](https://github.com/xinntao/facexlib/actions/workflows/publish-pip.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/publish-pip.yml)
-        [![gitee mirror](https://github.com/xinntao/facexlib/actions/workflows/gitee-mirror.yml/badge.svg)](https://github.com/xinntao/facexlib/blob/master/.github/workflows/gitee-mirror.yml)
         
-        [English](README.md) **|** [简体中文](README_CN.md) &emsp; [GitHub](https://github.com/xinntao/facexlib) **|** [Gitee码云](https://gitee.com/xinntao/facexlib)
+        [English](README.md) **|** [简体中文](README_CN.md)
         
         ---
         
-        **facexlib** aims at providing ready-to-use **face-related** functions based on current STOA open-source methods. <br>
+        **facexlib** aims at providing ready-to-use **face-related** functions based on current SOTA open-source methods. <br>
         Only PyTorch reference codes are available. For training or fine-tuning, please refer to their original repositories listed below. <br>
         Note that we just provide a collection of these algorithms. You need to refer to their original LICENCEs for your intended use.
         
         If facexlib is helpful in your projects, please help to :star: this repo. Thanks:blush: <br>
         Other recommended projects: &emsp; :arrow_forward: [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) &emsp; :arrow_forward: [GFPGAN](https://github.com/TencentARC/GFPGAN) &emsp; :arrow_forward: [BasicSR](https://github.com/xinntao/BasicSR)
         
         ---
```

### Comparing `facexlib-0.2.5/facexlib.egg-info/SOURCES.txt` & `facexlib-0.3.0/facexlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_alignment.py` & `facexlib-0.3.0/inference/inference_alignment.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from facexlib.alignment import init_alignment_model, landmark_98_to_68
 from facexlib.visualization import visualize_alignment
 
 
 def main(args):
     # initialize model
-    align_net = init_alignment_model(args.model_name)
+    align_net = init_alignment_model(args.model_name, device=args.device)
 
     img = cv2.imread(args.img_path)
     with torch.no_grad():
         landmarks = align_net.get_landmarks(img)
         if args.to68:
             landmarks = landmark_98_to_68(landmarks)
         visualize_alignment(img, [landmarks], args.save_path)
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('--img_path', type=str, default='assets/test2.jpg')
     parser.add_argument('--save_path', type=str, default='test_alignment.png')
     parser.add_argument('--model_name', type=str, default='awing_fan')
-    parser.add_argument('--half', action='store_true')
+    parser.add_argument('--device', type=str, default='cuda')
     parser.add_argument('--to68', action='store_true')
     args = parser.parse_args()
 
     main(args)
```

### Comparing `facexlib-0.2.5/inference/inference_crop_standard_faces.py` & `facexlib-0.3.0/inference/inference_crop_standard_faces.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_detection.py` & `facexlib-0.3.0/inference/inference_detection.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_headpose.py` & `facexlib-0.3.0/inference/inference_headpose.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_hyperiqa.py` & `facexlib-0.3.0/inference/inference_hyperiqa.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_matting.py` & `facexlib-0.3.0/inference/inference_matting.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_parsing.py` & `facexlib-0.3.0/inference/inference_parsing.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_parsing_parsenet.py` & `facexlib-0.3.0/inference/inference_parsing_parsenet.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_recognition.py` & `facexlib-0.3.0/inference/inference_recognition.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/inference/inference_tracking.py` & `facexlib-0.3.0/inference/inference_tracking.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/scripts/crop_faces_5landmarks.py` & `facexlib-0.3.0/scripts/crop_faces_5landmarks.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/scripts/extract_detection_info_ffhq.py` & `facexlib-0.3.0/scripts/extract_detection_info_ffhq.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/scripts/get_ffhq_template.py` & `facexlib-0.3.0/scripts/get_ffhq_template.py`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/setup.cfg` & `facexlib-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `facexlib-0.2.5/setup.py` & `facexlib-0.3.0/setup.py`

 * *Files identical despite different names*

