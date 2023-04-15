# Comparing `tmp/anylabeling-0.2.3.tar.gz` & `tmp/anylabeling-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.2.3.tar", last modified: Sat Apr 15 17:54:31 2023, max compression
+gzip compressed data, was "anylabeling-0.2.4.tar", last modified: Sat Apr 15 19:45:11 2023, max compression
```

## Comparing `anylabeling-0.2.3.tar` & `anylabeling-0.2.4.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.908132 anylabeling-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 17:54:18.000000 anylabeling-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 17:54:18.000000 anylabeling-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-15 17:54:31.908132 anylabeling-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-15 17:54:18.000000 anylabeling-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.852132 anylabeling-0.2.3/anylabeling/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.852132 anylabeling-0.2.3/anylabeling/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/anylabeling_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.860132 anylabeling-0.2.3/anylabeling/configs/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5x.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.864132 anylabeling-0.2.3/anylabeling/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.864132 anylabeling-0.2.3/anylabeling/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.868132 anylabeling-0.2.3/anylabeling/services/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/services/auto_labeling/yolov8.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.868132 anylabeling-0.2.3/anylabeling/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.868132 anylabeling-0.2.3/anylabeling/views/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.872132 anylabeling-0.2.3/anylabeling/views/labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.900132 anylabeling-0.2.3/anylabeling/views/labeling/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    92452 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.900132 anylabeling-0.2.3/anylabeling/views/labeling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.908132 anylabeling-0.2.3/anylabeling/views/labeling/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.908132 anylabeling-0.2.3/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48593 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 17:54:18.000000 anylabeling-0.2.3/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:54:31.852132 anylabeling-0.2.3/anylabeling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-15 17:54:31.000000 anylabeling-0.2.3/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-15 17:54:31.000000 anylabeling-0.2.3/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:54:31.000000 anylabeling-0.2.3/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 17:54:31.000000 anylabeling-0.2.3/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 17:54:31.000000 anylabeling-0.2.3/anylabeling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 17:54:31.000000 anylabeling-0.2.3/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-15 17:54:18.000000 anylabeling-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 17:54:31.908132 anylabeling-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-15 17:54:18.000000 anylabeling-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.464981 anylabeling-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 19:45:02.000000 anylabeling-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 19:45:02.000000 anylabeling-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-15 19:45:11.464981 anylabeling-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-15 19:45:02.000000 anylabeling-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/anylabeling_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/configs/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5x.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/services/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/views/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.460981 anylabeling-0.2.4/anylabeling/views/labeling/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92452 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.460981 anylabeling-0.2.4/anylabeling/views/labeling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.464981 anylabeling-0.2.4/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.464981 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48612 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-15 19:45:02.000000 anylabeling-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:45:11.464981 anylabeling-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-15 19:45:02.000000 anylabeling-0.2.4/setup.py
```

### Comparing `anylabeling-0.2.3/LICENSE` & `anylabeling-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/PKG-INFO` & `anylabeling-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.3
+Version: 0.2.4
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img style="width: 150px; max-width: 100%; height: auto; border-radius: 20px; overflow: hidden;" src="https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-4cbc-9132-c81cbc201265.png"/>
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.3 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.4 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
-Only Description-Content-Type: text/markdown License-File: LICENSE
+Language :: Python :: 3 :: Only Description-Content-Type: text/markdown
+License-File: LICENSE
  [https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-
                           4cbc-9132-c81cbc201265.png]
                       ****** ð AnyLabeling ð ******
    Effortless data labeling with AI support from YOLO and Segment Anything!
         AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
```

### Comparing `anylabeling-0.2.3/README.md` & `anylabeling-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/app.py` & `anylabeling-0.2.4/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.2.4/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/models.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/models.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5l.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5m.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5n.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5s.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov5x.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8l.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8m.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8n.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8s.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/configs/auto_labeling/yolov8x.yaml` & `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/resources/resources.py` & `anylabeling-0.2.4/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/services/auto_labeling/lru_cache.py` & `anylabeling-0.2.4/anylabeling/services/auto_labeling/lru_cache.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.2.4/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.2.4/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.2.4/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.2.4/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/services/auto_labeling/yolov8.py` & `anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov8.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/common/toaster.py` & `anylabeling-0.2.4/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/__main__.py` & `anylabeling-0.2.4/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/config.py` & `anylabeling-0.2.4/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/label_file.py` & `anylabeling-0.2.4/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.2.4/anylabeling/views/labeling/label_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.2.4/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/logger.py` & `anylabeling-0.2.4/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/shape.py` & `anylabeling-0.2.4/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/testing.py` & `anylabeling-0.2.4/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.2.4/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.2.4/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.2.4/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.2.4/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.2.4/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         #   - create_mode == 'polygon': edge from last point to current
         #   - create_mode == 'rectangle': diagonal line of the rectangle
         #   - create_mode == 'line': the line
         #   - create_mode == 'point': the point
         self.line = Shape()
         self.prev_point = QtCore.QPoint()
         self.prev_move_point = QtCore.QPoint()
-        self.offsets = QtCore.QPoint(), QtCore.QPoint()
+        self.offsets = QtCore.QPointF(), QtCore.QPointF()
         self.scale = 1.0
         self.pixmap = QtGui.QPixmap()
         self.visible = {}
         self._hide_backround = False
         self.hide_backround = False
         self.h_hape = None
         self.prev_h_shape = None
@@ -613,15 +613,15 @@
             if rect.bottom() > bottom:
                 bottom = rect.bottom()
 
         x1 = left - point.x()
         y1 = top - point.y()
         x2 = right - point.x()
         y2 = bottom - point.y()
-        self.offsets = QtCore.QPoint(x1, y1), QtCore.QPoint(x2, y2)
+        self.offsets = QtCore.QPointF(x1, y1), QtCore.QPointF(x2, y2)
 
     def bounded_move_vertex(self, pos):
         """Move a vertex. Adjust position to be bounded by pixmap border"""
         index, shape = self.h_vertex, self.h_hape
         point = shape[index]
         if self.out_off_pixmap(pos):
             pos = self.intersection_point(point, pos)
@@ -696,16 +696,16 @@
         """
         Shift shapes by an offset. Adjust positions to be bounded
         by pixmap borders
         """
         # Try to move in one direction, and if it fails in another.
         # Give up if both fail.
         point = shapes[0][0]
-        offset = QtCore.QPoint(2.0, 2.0)
-        self.offsets = QtCore.QPoint(), QtCore.QPoint()
+        offset = QtCore.QPointF(2.0, 2.0)
+        self.offsets = QtCore.QPointF(), QtCore.QPointF()
         self.prev_point = point
         if not self.bounded_move_shapes(shapes, point - offset):
             self.bounded_move_shapes(shapes, point + offset)
 
     # QT Overload
     def paintEvent(self, event):  # noqa: C901
         """Paint event for canvas"""
@@ -880,39 +880,39 @@
                 QtGui.QColor("#00FF00"),
                 max(1, int(round(2.0 / Shape.scale))),
                 Qt.DashLine,
             )
             p.setPen(pen)
             p.setOpacity(0.5)
             p.drawLine(
-                QtCore.QPoint(self.prev_move_point.x(), 0),
-                QtCore.QPoint(self.prev_move_point.x(), self.pixmap.height()),
+                QtCore.QPointF(self.prev_move_point.x(), 0),
+                QtCore.QPointF(self.prev_move_point.x(), self.pixmap.height()),
             )
             p.drawLine(
-                QtCore.QPoint(0, self.prev_move_point.y()),
-                QtCore.QPoint(self.pixmap.width(), self.prev_move_point.y()),
+                QtCore.QPointF(0, self.prev_move_point.y()),
+                QtCore.QPointF(self.pixmap.width(), self.prev_move_point.y()),
             )
 
         p.end()
 
     def transform_pos(self, point):
         """Convert from widget-logical coordinates to painter-logical ones."""
         return point / self.scale - self.offset_to_center()
 
     def offset_to_center(self):
         """Calculate offset to the center"""
         if self.pixmap is None:
-            return QtCore.QPoint()
+            return QtCore.QPointF()
         s = self.scale
         area = super().size()
         w, h = self.pixmap.width() * s, self.pixmap.height() * s
         area_width, area_height = area.width(), area.height()
         x = (area_width - w) / (2 * s) if area_width > w else 0
         y = (area_height - h) / (2 * s) if area_height > h else 0
-        return QtCore.QPoint(x, y)
+        return QtCore.QPointF(x, y)
 
     def out_off_pixmap(self, p):
         """Check if a position is out of pixmap"""
         if self.pixmap is None:
             return True
         w, h = self.pixmap.width(), self.pixmap.height()
         return not (0 <= p.x() <= w - 1 and 0 <= p.y() <= h - 1)
@@ -1060,16 +1060,16 @@
                 #   nua == nub == 0: Coincident
                 #   otherwise: Parallel
                 continue
             ua, ub = nua / denom, nub / denom
             if 0 <= ua <= 1 and 0 <= ub <= 1:
                 x = x1 + ua * (x2 - x1)
                 y = y1 + ua * (y2 - y1)
-                m = QtCore.QPoint((x3 + x4) / 2, (y3 + y4) / 2)
-                d = utils.distance(m - QtCore.QPoint(x2, y2))
+                m = QtCore.QPointF((x3 + x4) / 2, (y3 + y4) / 2)
+                d = utils.distance(m - QtCore.QPointF(x2, y2))
                 yield d, i, (x, y)
 
     # These two, along with a call to adjustSize are required for the
     # scroll area.
     # QT Overload
     def sizeHint(self):
         """Get size hint"""
@@ -1118,21 +1118,21 @@
                 self.update()
             elif key == QtCore.Qt.Key_Return and self.can_close_shape():
                 self.finalise()
             elif modifiers == QtCore.Qt.AltModifier:
                 self.snapping = False
         elif self.editing():
             if key == QtCore.Qt.Key_Up:
-                self.move_by_keyboard(QtCore.QPoint(0.0, -MOVE_SPEED))
+                self.move_by_keyboard(QtCore.QPointF(0.0, -MOVE_SPEED))
             elif key == QtCore.Qt.Key_Down:
-                self.move_by_keyboard(QtCore.QPoint(0.0, MOVE_SPEED))
+                self.move_by_keyboard(QtCore.QPointF(0.0, MOVE_SPEED))
             elif key == QtCore.Qt.Key_Left:
-                self.move_by_keyboard(QtCore.QPoint(-MOVE_SPEED, 0.0))
+                self.move_by_keyboard(QtCore.QPointF(-MOVE_SPEED, 0.0))
             elif key == QtCore.Qt.Key_Right:
-                self.move_by_keyboard(QtCore.QPoint(MOVE_SPEED, 0.0))
+                self.move_by_keyboard(QtCore.QPointF(MOVE_SPEED, 0.0))
 
     # QT Overload
     def keyReleaseEvent(self, ev):
         """Key release event"""
         modifiers = ev.modifiers()
         if self.drawing():
             if int(modifiers) == 0:
```

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
         painter.restore()
 
     # QT Overload
     def sizeHint(self, _, _2):
         margin_constant = 4
         return QtCore.QSize(
-            self.doc.idealWidth(),
-            self.doc.size().height() - margin_constant,
+            int(self.doc.idealWidth()),
+            int(self.doc.size().height() - margin_constant),
         )
 
 
 class LabelListWidgetItem(QtGui.QStandardItem):
     def __init__(self, text=None, shape=None):
         super(LabelListWidgetItem, self).__init__()
         self.setText(text or "")
```

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.2.4/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling/views/mainwindow.py` & `anylabeling-0.2.4/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.2.4/anylabeling.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.3
+Version: 0.2.4
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img style="width: 150px; max-width: 100%; height: auto; border-radius: 20px; overflow: hidden;" src="https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-4cbc-9132-c81cbc201265.png"/>
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.3 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.4 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
-Only Description-Content-Type: text/markdown License-File: LICENSE
+Language :: Python :: 3 :: Only Description-Content-Type: text/markdown
+License-File: LICENSE
  [https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-
                           4cbc-9132-c81cbc201265.png]
                       ****** ð AnyLabeling ð ******
    Effortless data labeling with AI support from YOLO and Segment Anything!
         AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
```

### Comparing `anylabeling-0.2.3/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.2.4/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.3/setup.py` & `anylabeling-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "anylabeling=anylabeling.app:main",
         ],
```

