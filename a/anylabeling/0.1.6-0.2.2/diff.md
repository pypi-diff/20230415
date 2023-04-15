# Comparing `tmp/anylabeling-0.1.6.tar.gz` & `tmp/anylabeling-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.1.6.tar", last modified: Fri Apr 14 19:17:44 2023, max compression
+gzip compressed data, was "anylabeling-0.2.2.tar", last modified: Sat Apr 15 13:19:00 2023, max compression
```

## Comparing `anylabeling-0.1.6.tar` & `anylabeling-0.2.2.tar`

### file list

```diff
@@ -1,141 +1,145 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.003970 anylabeling-0.1.6/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.6/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      113 2023-04-12 17:03:45.000000 anylabeling-0.1.6/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2965 2023-04-14 19:17:44.003812 anylabeling-0.1.6/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2129 2023-04-14 18:24:46.000000 anylabeling-0.1.6/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.987513 anylabeling-0.1.6/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       67 2023-04-12 17:16:44.000000 anylabeling-0.1.6/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      927 2023-04-13 15:24:26.000000 anylabeling-0.1.6/anylabeling/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-14 19:12:33.000000 anylabeling-0.1.6/anylabeling/app_info.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.990586 anylabeling-0.1.6/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.990710 anylabeling-0.1.6/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.6/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      388 2023-04-14 18:53:48.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:53:56.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5l.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:53:58.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:01.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5n.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5s.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5x.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8l.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8n.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8s.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:17.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8x.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.990927 anylabeling-0.1.6/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   477720 2023-04-12 17:04:48.000000 anylabeling-0.1.6/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.991523 anylabeling-0.1.6/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.992329 anylabeling-0.1.6/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4337 2023-04-14 19:03:06.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6106 2023-04-14 19:00:06.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10178 2023-04-14 18:55:46.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1335 2023-04-12 17:29:20.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5329 2023-04-14 19:02:27.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5089 2023-04-14 19:02:27.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/yolov8.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.992536 anylabeling-0.1.6/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.992863 anylabeling-0.1.6/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9583 2023-04-12 17:30:44.000000 anylabeling-0.1.6/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.994006 anylabeling-0.1.6/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.6/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2771 2023-04-12 17:31:48.000000 anylabeling-0.1.6/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.000657 anylabeling-0.1.6/anylabeling/views/labeling/icons/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/.DS_Store
--rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    36597 2023-04-12 17:03:45.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5995 2023-04-12 17:33:36.000000 anylabeling-0.1.6/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    90545 2023-04-14 19:10:28.000000 anylabeling-0.1.6/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.6/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.6/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10441 2023-04-12 17:34:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.001429 anylabeling-0.1.6/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-12 17:21:05.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.003171 anylabeling-0.1.6/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.003603 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7373 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46999 2023-04-14 17:35:30.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8027 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5780 2023-04-12 17:34:51.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-14 02:24:11.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.988330 anylabeling-0.1.6/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2965 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5235 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      188 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      267 2023-04-14 19:13:58.000000 anylabeling-0.1.6/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-14 19:17:44.004015 anylabeling-0.1.6/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2333 2023-04-13 15:22:05.000000 anylabeling-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.673450 anylabeling-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 13:18:50.000000 anylabeling-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 13:18:50.000000 anylabeling-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-15 13:19:00.673450 anylabeling-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-15 13:18:50.000000 anylabeling-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.657449 anylabeling-0.2.2/anylabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.661450 anylabeling-0.2.2/anylabeling/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/anylabeling_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.661450 anylabeling-0.2.2/anylabeling/configs/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5x.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.661450 anylabeling-0.2.2/anylabeling/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.661450 anylabeling-0.2.2/anylabeling/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.665449 anylabeling-0.2.2/anylabeling/services/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/services/auto_labeling/yolov8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.665449 anylabeling-0.2.2/anylabeling/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.665449 anylabeling-0.2.2/anylabeling/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.665449 anylabeling-0.2.2/anylabeling/views/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.673450 anylabeling-0.2.2/anylabeling/views/labeling/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92281 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.673450 anylabeling-0.2.2/anylabeling/views/labeling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.673450 anylabeling-0.2.2/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.673450 anylabeling-0.2.2/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48593 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 13:18:50.000000 anylabeling-0.2.2/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:19:00.661450 anylabeling-0.2.2/anylabeling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-15 13:19:00.000000 anylabeling-0.2.2/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-15 13:19:00.000000 anylabeling-0.2.2/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:19:00.000000 anylabeling-0.2.2/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 13:19:00.000000 anylabeling-0.2.2/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 13:19:00.000000 anylabeling-0.2.2/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 13:19:00.000000 anylabeling-0.2.2/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-15 13:18:50.000000 anylabeling-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:19:00.673450 anylabeling-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-15 13:18:50.000000 anylabeling-0.2.2/setup.py
```

### Comparing `anylabeling-0.1.6/LICENSE` & `anylabeling-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/PKG-INFO` & `anylabeling-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.6
+Version: 0.2.2
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.6 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.2 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.1.6/README.md` & `anylabeling-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/app.py` & `anylabeling-0.2.2/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.2.2/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5l.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5n.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5x.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8l.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8m.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8n.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8s.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8x.yaml` & `anylabeling-0.2.2/anylabeling/configs/auto_labeling/yolov8x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/resources/resources.py` & `anylabeling-0.2.2/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.2.2/anylabeling/services/auto_labeling/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import logging
 import os
 import pathlib
 import urllib.request
 from abc import abstractmethod
 
 import yaml
+import onnx
+
+from PyQt5.QtCore import QFile
+from PyQt5.QtGui import QImage
 
 from .types import AutoLabelingResult
+from anylabeling.views.labeling.label_file import LabelFile, LabelFileError
 
 
 class Model:
     BASE_DOWNLOAD_URL = (
         "https://github.com/vietanhdev/anylabeling-assets/raw/main/"
     )
 
@@ -78,15 +83,25 @@
                 "anylabeling_data",
                 "models",
                 model_folder_name,
                 filename,
             )
         )
         if os.path.exists(model_abs_path):
-            return model_abs_path
+            if model_abs_path.lower().endswith(".onnx"):
+                try:
+                    onnx.checker.check_model(model_abs_path)
+                except onnx.checker.ValidationError as e:
+                    print("The model is invalid: %s" % e)
+                    print("Action: Delete and redownload...")
+                    os.remove(model_abs_path)
+                else:
+                    return model_abs_path
+            else:
+                return model_abs_path
         pathlib.Path(model_abs_path).parent.mkdir(parents=True, exist_ok=True)
 
         # Download model from url
         ellipsis_download_url = download_url
         if len(download_url) > 40:
             ellipsis_download_url = (
                 download_url[:20] + "..." + download_url[-20:]
@@ -118,19 +133,44 @@
         Check if config has all required config names
         """
         for name in config_names:
             if name not in config:
                 raise Exception(f"Missing config: {name}")
 
     @abstractmethod
-    def predict_shapes(self, image) -> AutoLabelingResult:
+    def predict_shapes(self, image, image_path=None) -> AutoLabelingResult:
         """
         Predict image and return AnyLabeling shapes
         """
         raise NotImplementedError
 
     @abstractmethod
     def unload(self):
         """
         Unload model from memory
         """
         raise NotImplementedError
+
+    @staticmethod
+    def load_image_from_filename(filename):
+        """Load image from labeling file and return image data and image path."""
+        label_file = os.path.splitext(filename)[0] + ".json"
+        if QFile.exists(label_file) and LabelFile.is_label_file(label_file):
+            try:
+                label_file = LabelFile(label_file)
+            except LabelFileError as e:
+                print("Error reading {}: {}".format(label_file, e))
+                return None, None
+            image_data = label_file.image_data
+        else:
+            image_data = LabelFile.load_image_file(filename)
+        image = QImage.fromData(image_data)
+        if image.isNull():
+            print("Error reading {}".format(filename))
+        return image
+
+    def on_next_files_changed(self, next_files):
+        """
+        Handle next files changed. This function can preload next files
+        and run inference to save time for user.
+        """
+        pass
```

### Comparing `anylabeling-0.1.6/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.2.2/anylabeling/services/auto_labeling/model_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 import copy
 import importlib.resources as pkg_resources
 from threading import Lock
 
 import yaml
 from PyQt5.QtCore import QObject, QThread, pyqtSignal, pyqtSlot
 
-from anylabeling import configs as anylabeling_configs
+from anylabeling.configs import auto_labeling as auto_labeling_configs
 from anylabeling.services.auto_labeling.types import AutoLabelingResult
 from anylabeling.utils import GenericWorker
 
 
 class ModelManager(QObject):
     """Model manager"""
 
     new_model_status = pyqtSignal(str)
     model_loaded = pyqtSignal(list)
     new_auto_labeling_result = pyqtSignal(AutoLabelingResult)
     auto_segmentation_model_selected = pyqtSignal()
     auto_segmentation_model_unselected = pyqtSignal()
-
-    model_configs = {
-        "segment_anything_vit_b-r20230415": "autolabel_segment_anything.yaml",
-        "yolov5n-r20230415": "autolabel_yolov5n.yaml",
-        "yolov5s-r20230415": "autolabel_yolov5s.yaml",
-        "yolov5m-r20230415": "autolabel_yolov5m.yaml",
-        "yolov5l-r20230415": "autolabel_yolov5l.yaml",
-        "yolov5x-r20230415": "autolabel_yolov5x.yaml",
-        "yolov8n-r20230415": "autolabel_yolov8n.yaml",
-        "yolov8s-r20230415": "autolabel_yolov8s.yaml",
-        "yolov8m-r20230415": "autolabel_yolov8m.yaml",
-        "yolov8l-r20230415": "autolabel_yolov8l.yaml",
-        "yolov8x-r20230415": "autolabel_yolov8x.yaml",
-    }
+    prediction_started = pyqtSignal()
+    prediction_finished = pyqtSignal()
+    request_next_files_requested = pyqtSignal()
+    model_configs = {}
 
     def __init__(self):
         super().__init__()
         self.model_infos = {}
+        self.model_list_config = {}
+
+        # Load list of models
+        with pkg_resources.open_text(
+            auto_labeling_configs, "models.yaml"
+        ) as f:
+            self.model_list_config = yaml.safe_load(f)
+        for model_config in self.model_list_config:
+            self.model_configs[model_config["model_name"]] = model_config[
+                "config_file"
+            ]
+
+        # Load model configs
         for model_name, config_name in ModelManager.model_configs.items():
             self.model_infos[model_name] = {}
             with pkg_resources.open_text(
-                anylabeling_configs, config_name
+                auto_labeling_configs, config_name
             ) as f:
                 config = yaml.safe_load(f)
             self.model_infos[model_name] = config
 
         self.loaded_model_info = None
         self.loaded_model_info_lock = Lock()
 
         self.model_download_thread = None
+        self.model_execution_thread = None
+        self.model_execution_thread_lock = Lock()
 
     def get_model_infos(self):
         """Return model infos"""
         return self.model_infos
 
     def get_model_names(self):
         """Return model names"""
@@ -129,14 +134,17 @@
         elif model_info["type"] == "segment_anything":
             from .segment_anything import SegmentAnything
 
             model_info["model"] = SegmentAnything(
                 model_info, on_message=self.new_model_status.emit
             )
             self.auto_segmentation_model_selected.emit()
+
+            # Request next files for prediction
+            self.request_next_files_requested.emit()
         else:
             raise Exception(f"Unknown model type: {model_info['type']}")
 
         self.loaded_model_info = model_info
         return self.loaded_model_info
 
     def set_auto_labeling_marks(self, marks):
@@ -152,16 +160,82 @@
 
     def unload_model(self):
         """Unload model"""
         if self.loaded_model_info is not None:
             self.loaded_model_info["model"].unload()
             self.loaded_model_info = None
 
-    @pyqtSlot()
-    def predict_shapes(self, image):
-        """Predict shapes"""
+    def predict_shapes(self, image, filename=None):
+        """Predict shapes.
+        NOTE: This function is blocking. The model can take a long time to
+        predict. So it is recommended to use predict_shapes_threading instead.
+        """
         if self.loaded_model_info is None:
-            raise Exception("Model is not loaded")
-        auto_labeling_result = self.loaded_model_info["model"].predict_shapes(
-            image
+            self.new_model_status.emit(
+                "Model is not loaded. Choose a mode to continue."
+            )
+            self.prediction_finished.emit()
+            return
+        try:
+            auto_labeling_result = self.loaded_model_info[
+                "model"
+            ].predict_shapes(image, filename)
+            self.new_auto_labeling_result.emit(auto_labeling_result)
+        except Exception as e:  # noqa
+            print(f"Error in predict_shapes: {e}")
+            self.new_model_status.emit(
+                "Error in model prediction. Please check the model."
+            )
+        self.new_model_status.emit(
+            "Finished inferencing AI model. Check the result."
         )
-        self.new_auto_labeling_result.emit(auto_labeling_result)
+        self.prediction_finished.emit()
+
+    @pyqtSlot()
+    def predict_shapes_threading(self, image, filename=None):
+        """Predict shapes.
+        This function starts a thread to run the prediction.
+        """
+        if self.loaded_model_info is None:
+            self.new_model_status.emit(
+                "Model is not loaded. Choose a mode to continue."
+            )
+            return
+        self.new_model_status.emit("Inferencing AI model. Please wait...")
+        self.prediction_started.emit()
+
+        with self.model_execution_thread_lock:
+            if (
+                self.model_execution_thread is not None
+                and self.model_execution_thread.isRunning()
+            ):
+                self.new_model_status.emit(
+                    "Another model is being executed. Please wait for it to finish."
+                )
+                self.prediction_finished.emit()
+                return
+
+            self.model_execution_thread = QThread()
+            self.model_execution_worker = GenericWorker(
+                self.predict_shapes, image, filename
+            )
+            self.model_execution_worker.finished.connect(
+                self.model_execution_thread.quit
+            )
+            self.model_execution_worker.moveToThread(
+                self.model_execution_thread
+            )
+            self.model_execution_thread.started.connect(
+                self.model_execution_worker.run
+            )
+            self.model_execution_thread.start()
+
+    def on_next_files_changed(self, next_files):
+        """Run prediction on next files in advance to save inference time later"""
+        if self.loaded_model_info is None:
+            return
+
+        # Currently only segment_anything model supports this feature
+        if self.loaded_model_info["type"] != "segment_anything":
+            return
+
+        self.loaded_model_info["model"].on_next_files_changed(next_files)
```

### Comparing `anylabeling-0.1.6/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.2.2/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.2.2/anylabeling/services/auto_labeling/yolov5.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 "score": score,
             }
 
             output_boxes.append(output_box)
 
         return output_boxes
 
-    def predict_shapes(self, image):
+    def predict_shapes(self, image, image_path=None):
         """
         Predict shapes from image
         """
 
         if image is None:
             return []
```

### Comparing `anylabeling-0.1.6/anylabeling/services/auto_labeling/yolov8.py` & `anylabeling-0.2.2/anylabeling/services/auto_labeling/yolov8.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                 "score": score,
             }
 
             output_boxes.append(output_box)
 
         return output_boxes
 
-    def predict_shapes(self, image):
+    def predict_shapes(self, image, image_path=None):
         """
         Predict shapes from image
         """
 
         if image is None:
             return []
```

### Comparing `anylabeling-0.1.6/anylabeling/views/common/toaster.py` & `anylabeling-0.2.2/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/__main__.py` & `anylabeling-0.2.2/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/config.py` & `anylabeling-0.2.2/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.2.2/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/label_file.py` & `anylabeling-0.2.2/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.2.2/anylabeling/views/labeling/label_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 LABEL_COLORMAP[1] = [0, 180, 33]
 
 
 class LabelmeWidget(LabelDialog):
     """Labelme widget"""
 
     FIT_WINDOW, FIT_WIDTH, MANUAL_ZOOM = 0, 1, 2
+    next_files_changed = QtCore.pyqtSignal(list)
 
     def __init__(
         self,
         parent=None,
         config=None,
         filename=None,
         output=None,
@@ -874,14 +875,26 @@
         )
         self.auto_labeling_widget.clear_auto_labeling_action_requested.connect(
             self.clear_auto_labeling_marks
         )
         self.auto_labeling_widget.finish_auto_labeling_object_action_requested.connect(
             self.finish_auto_labeling_object
         )
+        self.auto_labeling_widget.model_manager.prediction_started.connect(
+            lambda: self.canvas.set_loading(True, "Please wait...")
+        )
+        self.auto_labeling_widget.model_manager.prediction_finished.connect(
+            lambda: self.canvas.set_loading(False)
+        )
+        self.next_files_changed.connect(
+            self.auto_labeling_widget.model_manager.on_next_files_changed
+        )
+        self.auto_labeling_widget.model_manager.request_next_files_requested.connect(
+            lambda: self.inform_next_files(self.filename)
+        )
         self.auto_labeling_widget.hide()  # Hide by default
         central_layout.addWidget(self.label_instruction)
         central_layout.addWidget(self.auto_labeling_widget)
         central_layout.addWidget(scroll_area)
         layout.addItem(central_layout)
 
         # Save central area for resize
@@ -1758,18 +1771,47 @@
         contrast = dialog.slider_contrast.value()
         self.brightness_contrast_values[self.filename] = (brightness, contrast)
 
     def toggle_polygons(self, value):
         for item in self.label_list:
             item.setCheckState(Qt.Checked if value else Qt.Unchecked)
 
+    def get_next_files(self, filename, num_files):
+        """Get the next files in the list."""
+        if not self.image_list:
+            return []
+        filenames = []
+        current_index = 0
+        if filename is not None:
+            current_index = self.image_list.index(filename)
+        for _ in range(num_files):
+            if current_index + 1 < len(self.image_list):
+                filenames.append(self.image_list[current_index + 1])
+                current_index += 1
+            else:
+                filenames.append(self.image_list[-1])
+                break
+        return filenames
+
+    def inform_next_files(self, filename):
+        """Inform the next files to be annotated.
+        This list can be used by the user to preload the next files
+        or running a background process to process them
+        """
+        next_files = self.get_next_files(filename, 5)
+        if next_files:
+            self.next_files_changed.emit(next_files)
+
     def load_file(self, filename=None):  # noqa: C901
         """Load the specified file, or the last opened file if None."""
 
+        # For auto labeling, clear the previous marks
+        # and inform the next files to be annotated
         self.clear_auto_labeling_marks()
+        self.inform_next_files(filename)
 
         # Changing file_list_widget loads file
         if filename in self.image_list and (
             self.file_list_widget.currentRow()
             != self.image_list.index(filename)
         ):
             self.file_list_widget.setCurrentRow(
```

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.2.2/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/logger.py` & `anylabeling-0.2.2/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/shape.py` & `anylabeling-0.2.2/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/testing.py` & `anylabeling-0.2.2/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.2.2/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.2.2/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.2.2/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.2.2/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.2.2/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from anylabeling.services.auto_labeling.model_manager import ModelManager
 from anylabeling.services.auto_labeling.types import AutoLabelingMode
 
 
 class AutoLabelingWidget(QWidget):
     new_model_selected = pyqtSignal(str)
-    prediction_requested = pyqtSignal(QtGui.QImage)
     auto_segmentation_requested = pyqtSignal()
     auto_segmentation_disabled = pyqtSignal()
     auto_labeling_mode_changed = pyqtSignal(AutoLabelingMode)
     undo_auto_labeling_action_requested = pyqtSignal()
     clear_auto_labeling_action_requested = pyqtSignal()
     finish_auto_labeling_object_action_requested = pyqtSignal()
 
@@ -32,17 +31,14 @@
             self.enable_model_select_combobox
         )
         self.model_manager.new_auto_labeling_result.connect(
             lambda auto_labeling_result: self.parent.new_shapes_from_auto_labeling(
                 auto_labeling_result
             )
         )
-        self.prediction_requested.connect(
-            lambda image: self.model_manager.predict_shapes(image)
-        )
         self.model_manager.auto_segmentation_model_selected.connect(
             self.auto_segmentation_requested
         )
         self.model_manager.auto_segmentation_model_unselected.connect(
             self.auto_segmentation_disabled
         )
 
@@ -143,16 +139,18 @@
             self.auto_labeling_mode = AutoLabelingMode.NONE
         else:
             self.auto_labeling_mode = AutoLabelingMode(edit_mode, shape_type)
         self.auto_labeling_mode_changed.emit(self.auto_labeling_mode)
 
     def run_prediction(self):
         """Run prediction"""
-        if self.parent.image_path:
-            self.prediction_requested.emit(self.parent.image)
+        if self.parent.filename is not None:
+            self.model_manager.predict_shapes_threading(
+                self.parent.image, self.parent.filename
+            )
 
     def unload_and_hide(self):
         """Unload model and hide widget"""
         self.model_select_combobox.setCurrentIndex(0)
         self.hide()
 
     def on_new_model_status(self, status):
```

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,25 @@
         # Set widget options.
         self.setMouseTracking(True)
         self.setFocusPolicy(QtCore.Qt.WheelFocus)
         self.show_cross_line = True
         self.show_shape_groups = True
         self.show_texts = True
 
+        self.is_loading = False
+        self.loading_text = "Loading..."
+        self.loading_angle = 0
+
+    def set_loading(self, is_loading: bool, loading_text: str = None):
+        """Set loading state"""
+        self.is_loading = is_loading
+        if loading_text:
+            self.loading_text = loading_text
+        self.update()
+
     def set_auto_labeling_mode(self, mode: AutoLabelingMode):
         """Set auto labeling mode"""
         if mode == AutoLabelingMode.NONE:
             self.is_auto_labeling = False
             self.auto_labeling_mode = mode
         else:
             self.is_auto_labeling = True
@@ -242,14 +253,16 @@
     def selected_edge(self):
         """Check if selected an edge"""
         return self.h_edge is not None
 
     # QT Overload
     def mouseMoveEvent(self, ev):  # noqa: C901
         """Update line with last point and current coordinates"""
+        if self.is_loading:
+            return
         try:
             pos = self.transform_pos(ev.localPos())
         except AttributeError:
             return
 
         self.prev_move_point = pos
         self.repaint()
@@ -402,14 +415,16 @@
         self.h_hape = shape
         self.prev_h_vertex = None
         self.moving_shape = True  # Save changes
 
     # QT Overload
     def mousePressEvent(self, ev):
         """Mouse press event"""
+        if self.is_loading:
+            return
         pos = self.transform_pos(ev.localPos())
         if ev.button() == QtCore.Qt.LeftButton:
             if self.drawing():
                 if self.current:
                     # Add point to existing shape.
                     if self.create_mode == "polygon":
                         self.current.add_point(self.line[1])
@@ -465,14 +480,16 @@
                 )
                 self.repaint()
             self.prev_point = pos
 
     # QT Overload
     def mouseReleaseEvent(self, ev):
         """Mouse release event"""
+        if self.is_loading:
+            return
         if ev.button() == QtCore.Qt.RightButton:
             menu = self.menus[len(self.selected_shapes_copy) > 0]
             self.restore_cursor()
             if (
                 not menu.exec_(self.mapToGlobal(ev.pos()))
                 and self.selected_shapes_copy
             ):
@@ -534,14 +551,16 @@
     def can_close_shape(self):
         """Check if a shape can be closed (number of points > 2)"""
         return self.drawing() and self.current and len(self.current) > 2
 
     # QT Overload
     def mouseDoubleClickEvent(self, _):
         """Mouse double click event"""
+        if self.is_loading:
+            return
         # We need at least 4 points here, since the mousePress handler
         # adds an extra one before this handler is called.
         if (
             self.double_click == "close"
             and self.can_close_shape()
             and len(self.current) > 3
         ):
@@ -705,14 +724,46 @@
 
         p.scale(self.scale, self.scale)
         p.translate(self.offset_to_center())
 
         p.drawPixmap(0, 0, self.pixmap)
         Shape.scale = self.scale
 
+        # Draw loading/waiting screen
+        if self.is_loading:
+            # Draw a semi-transparent rectangle
+            p.setPen(Qt.NoPen)
+            p.setBrush(QtGui.QColor(0, 0, 0, 100))
+            p.drawRect(self.pixmap.rect())
+
+            # Draw a spinning wheel
+            p.setPen(QtGui.QColor(255, 255, 255))
+            p.setBrush(Qt.NoBrush)
+            p.save()
+            p.translate(self.pixmap.width() / 2, self.pixmap.height() / 2 - 50)
+            p.rotate(self.loading_angle)
+            p.drawEllipse(-20, -20, 40, 40)
+            p.drawLine(0, 0, 0, -20)
+            p.restore()
+            self.loading_angle += 30
+            if self.loading_angle >= 360:
+                self.loading_angle = 0
+
+            # Draw the loading text
+            p.setPen(QtGui.QColor(255, 255, 255))
+            p.setFont(QtGui.QFont("Arial", 20))
+            p.drawText(
+                self.pixmap.rect(),
+                Qt.AlignCenter,
+                self.loading_text,
+            )
+            p.end()
+            self.update()
+            return
+
         # Draw groups
         if self.show_shape_groups:
             pen = QtGui.QPen(QtGui.QColor("#AAAAAA"), 2, Qt.SolidLine)
             p.setPen(pen)
             grouped_shapes = {}
             for shape in self.shapes:
                 if shape.group_id is None:
```

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.2.2/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling/views/mainwindow.py` & `anylabeling-0.2.2/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.6/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.2.2/anylabeling.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.6
+Version: 0.2.2
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.6 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.2 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.1.6/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.2.2/anylabeling.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,51 +11,55 @@
 anylabeling.egg-info/SOURCES.txt
 anylabeling.egg-info/dependency_links.txt
 anylabeling.egg-info/entry_points.txt
 anylabeling.egg-info/requires.txt
 anylabeling.egg-info/top_level.txt
 anylabeling/configs/__init__.py
 anylabeling/configs/anylabeling_config.yaml
-anylabeling/configs/autolabel_segment_anything.yaml
-anylabeling/configs/autolabel_yolov5l.yaml
-anylabeling/configs/autolabel_yolov5m.yaml
-anylabeling/configs/autolabel_yolov5n.yaml
-anylabeling/configs/autolabel_yolov5s.yaml
-anylabeling/configs/autolabel_yolov5x.yaml
-anylabeling/configs/autolabel_yolov8l.yaml
-anylabeling/configs/autolabel_yolov8m.yaml
-anylabeling/configs/autolabel_yolov8n.yaml
-anylabeling/configs/autolabel_yolov8s.yaml
-anylabeling/configs/autolabel_yolov8x.yaml
-anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+anylabeling/configs/auto_labeling/__init__.py
+anylabeling/configs/auto_labeling/models.yaml
+anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
+anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
+anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
+anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
+anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
+anylabeling/configs/auto_labeling/yolov5l.yaml
+anylabeling/configs/auto_labeling/yolov5m.yaml
+anylabeling/configs/auto_labeling/yolov5n.yaml
+anylabeling/configs/auto_labeling/yolov5s.yaml
+anylabeling/configs/auto_labeling/yolov5x.yaml
+anylabeling/configs/auto_labeling/yolov8l.yaml
+anylabeling/configs/auto_labeling/yolov8m.yaml
+anylabeling/configs/auto_labeling/yolov8n.yaml
+anylabeling/configs/auto_labeling/yolov8s.yaml
+anylabeling/configs/auto_labeling/yolov8x.yaml
 anylabeling/resources/__init__.py
 anylabeling/resources/resources.py
 anylabeling/services/__init__.py
 anylabeling/services/auto_labeling/__init__.py
+anylabeling/services/auto_labeling/lru_cache.py
 anylabeling/services/auto_labeling/model.py
 anylabeling/services/auto_labeling/model_manager.py
 anylabeling/services/auto_labeling/segment_anything.py
 anylabeling/services/auto_labeling/types.py
 anylabeling/services/auto_labeling/yolov5.py
 anylabeling/services/auto_labeling/yolov8.py
 anylabeling/views/__init__.py
 anylabeling/views/mainwindow.py
 anylabeling/views/common/__init__.py
-anylabeling/views/common/tableview.py
 anylabeling/views/common/toaster.py
 anylabeling/views/labeling/__init__.py
 anylabeling/views/labeling/__main__.py
 anylabeling/views/labeling/config.py
 anylabeling/views/labeling/label_file.py
 anylabeling/views/labeling/label_widget.py
 anylabeling/views/labeling/label_wrapper.py
 anylabeling/views/labeling/logger.py
 anylabeling/views/labeling/shape.py
 anylabeling/views/labeling/testing.py
-anylabeling/views/labeling/icons/.DS_Store
 anylabeling/views/labeling/icons/brain.png
 anylabeling/views/labeling/icons/cancel.png
 anylabeling/views/labeling/icons/cartesian.png
 anylabeling/views/labeling/icons/circle.png
 anylabeling/views/labeling/icons/color-line.png
 anylabeling/views/labeling/icons/color.png
 anylabeling/views/labeling/icons/color_line.png
```

### Comparing `anylabeling-0.1.6/setup.py` & `anylabeling-0.2.2/setup.py`

 * *Files identical despite different names*

