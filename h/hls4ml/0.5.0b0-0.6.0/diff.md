# Comparing `tmp/hls4ml-0.5.0b0.tar.gz` & `tmp/hls4ml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hls4ml-0.5.0b0.tar", last modified: Mon Jan 18 16:20:11 2021, max compression
+gzip compressed data, was "hls4ml-0.6.0.tar", last modified: Fri Nov 12 12:26:47 2021, max compression
```

## Comparing `hls4ml-0.5.0b0.tar` & `hls4ml-0.6.0.tar`

### file list

```diff
@@ -1,219 +1,265 @@
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    11357 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/LICENSE
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      122 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/MANIFEST.in
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3355 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/PKG-INFO
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2098 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/README.md
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      799 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/build_prj.tcl
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2689 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/myproject.cpp
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1150 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/myproject.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2173 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/parameters.h
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/weights/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      148 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/weights/b1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      179 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/weights/b2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      668 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/weights/w1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1257 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/weights/w2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)       72 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/myproject.tcl
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2177 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv-1layer/myproject_test.cpp
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      799 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/build_prj.tcl
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2869 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/myproject.cpp
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1213 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/myproject.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2953 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/parameters.h
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/weights/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      155 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/weights/b1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      292 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/weights/b2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      418 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/weights/w1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    21834 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/weights/w2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)       72 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/myproject.tcl
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     5176 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/conv2d-1layer/myproject_test.cpp
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/demo-conversion/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      232 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/demo-conversion/README.md
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      284 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/demo-conversion/keras-config.yml
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      798 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/build_prj.tcl
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2175 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/myproject.cpp
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1142 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/myproject.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1991 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/parameters.h
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      632 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/b1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      111 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/b2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     5393 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/w1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      641 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/w2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)       72 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/myproject.tcl
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1368 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/higgs-1layer/myproject_test.cpp
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/sublayer/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      550 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/build_prj.tcl
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3621 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/myproject.cpp
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1218 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/myproject.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3994 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/parameters.h
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1460 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      804 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      460 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b2_0.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      474 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b2_1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      804 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b3.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      230 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b4.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    12253 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    17994 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w2.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     9318 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w2_0.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     8811 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w2_1.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     8872 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w3.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2146 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w4.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1380 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/example-prjs/sublayer/myproject_test.cpp
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      146 2021-01-18 15:33:00.000000 hls4ml-0.5.0b0/hls4ml/__init__.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/converters/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3424 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/__init__.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)        0 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3073 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/convolution.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     4626 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/core.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2175 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/graph.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1337 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/merge.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3833 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/pooling.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3570 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/qkeras.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     4660 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/qkeras_layers.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1642 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/reshape.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3353 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras/reshaping.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    13272 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/keras_to_hls.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    17893 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/onnx_to_hls.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3483 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/pytorch_to_hls.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    14936 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/converters/tf_to_hls.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/model/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      227 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    80334 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/hls_layers.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    22979 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/hls_model.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2063 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1219 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/optimizer.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)        0 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1341 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/bn_fuse.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     8992 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/bn_quant.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2957 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/clone.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3565 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/conv_same_pad.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      707 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/fuse_biasadd.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      510 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/nop.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2137 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/pointwise.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     9479 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/qkeras.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1823 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/repack_stream.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    20358 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/model/profiling.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/report/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      159 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/report/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     6811 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/report/vivado_report.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/templates/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      220 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1075 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/templates.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    10180 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_common.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     6473 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_decl.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    12185 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    85182 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed_base.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    27302 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed_ref.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     6985 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed_special.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    10012 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    71735 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int_base.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    55218 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int_ref.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     6301 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int_special.h
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/etc/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)   261465 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/etc/ap_private.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     7480 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/hls_stream.h
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/utils/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2227 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/utils/x_hls_utils.h
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)      529 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/build_lib.sh
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3730 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/build_prj.tcl
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/firmware/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      220 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/firmware/defines.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1338 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/firmware/myproject.cpp
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1056 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/firmware/myproject.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      271 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/firmware/parameters.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1651 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/myproject_bridge.cpp
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3209 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/myproject_test.cpp
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)       89 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/README.md
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    29354 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_activation.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    23865 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_activation_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1254 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_array.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     5560 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     4571 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2781 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_common.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2403 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     5004 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_latency.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     8427 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_resource.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2228 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3352 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    14998 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_latency.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    10626 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_resource.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2839 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3681 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1444 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3690 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_compressed.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     5287 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_latency.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    10540 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_resource.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2275 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    32133 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_garnet.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    12754 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_helpers.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1246 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_image.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1192 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_image_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    11508 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_merge.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     5501 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_merge_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2713 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_mult.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     4192 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_padding.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1769 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_padding_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     9386 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_pooling.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    14115 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_pooling_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3879 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv1d_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     4627 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv2d_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     6323 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2718 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_stream.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      704 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_types.h
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      139 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado/vivado_synth.tcl
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    32389 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/templates/vivado_template.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/utils/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      217 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/utils/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     9479 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/utils/config.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     5446 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/utils/example_models.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     8789 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/utils/plot.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml/writer/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      204 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/writer/__init__.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)    29832 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/writer/vivado_writer.py
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      371 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/hls4ml/writer/writers.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/hls4ml.egg-info/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     3355 2021-01-18 16:20:10.000000 hls4ml-0.5.0b0/hls4ml.egg-info/PKG-INFO
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     7362 2021-01-18 16:20:10.000000 hls4ml-0.5.0b0/hls4ml.egg-info/SOURCES.txt
--rw-rw-r--   0 sioni     (1000) sioni     (1000)        1 2021-01-18 16:20:10.000000 hls4ml-0.5.0b0/hls4ml.egg-info/dependency_links.txt
--rw-rw-r--   0 sioni     (1000) sioni     (1000)       73 2021-01-18 16:20:10.000000 hls4ml-0.5.0b0/hls4ml.egg-info/requires.txt
--rw-rw-r--   0 sioni     (1000) sioni     (1000)        7 2021-01-18 16:20:10.000000 hls4ml-0.5.0b0/hls4ml.egg-info/top_level.txt
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/scripts/
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     8515 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/scripts/hls4ml
--rw-rw-r--   0 sioni     (1000) sioni     (1000)       79 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/setup.cfg
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1850 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/setup.py
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/test/
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     3301 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/build-prj.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     1040 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/cleanup.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     2955 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/compare-reports.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     2374 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/convert-keras-models.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     2173 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/convert-onnx-models.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     2180 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/convert-pytorch-models.sh
-drwxrwxr-x   0 sioni     (1000) sioni     (1000)        0 2021-01-18 16:20:11.000000 hls4ml-0.5.0b0/test/docker/
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2668 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/docker/Dockerfile
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     2962 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/docker/README.md
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1647 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/docker/install_config-2017.2.txt
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1743 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/docker/install_config.txt
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     1519 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/gather-reports.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)      804 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/hls4ml-keras-test.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     1146 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/hls4ml-onnx-test.sh
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     1170 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/hls4ml-pytorch-test.sh
--rw-rw-r--   0 sioni     (1000) sioni     (1000)     1466 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/keras-models.txt
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     3341 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/keras-to-hls.sh
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      792 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/onnx-models.txt
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     2379 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/onnx-to-hls.sh
--rw-rw-r--   0 sioni     (1000) sioni     (1000)      616 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/pytorch-models.txt
--rwxrwxr-x   0 sioni     (1000) sioni     (1000)     2381 2021-01-18 14:37:28.000000 hls4ml-0.5.0b0/test/pytorch-to-hls.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.390328 hls4ml-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-12 12:26:42.000000 hls4ml-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-11-12 12:26:42.000000 hls4ml-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3002 2021-11-12 12:26:47.390328 hls4ml-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2021-11-12 12:26:42.000000 hls4ml-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.346327 hls4ml-0.6.0/example-prjs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.350327 hls4ml-0.6.0/example-prjs/conv-1layer/
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/build_prj.tcl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/myproject.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/myproject.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2173 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/parameters.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/weights/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/weights/b1.h
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/weights/b2.h
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/weights/w1.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/firmware/weights/w2.h
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/myproject.tcl
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv-1layer/myproject_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/conv2d-1layer/
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/build_prj.tcl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/
+-rw-r--r--   0 runner    (1001) docker     (121)     2869 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/myproject.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/myproject.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2953 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/parameters.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/weights/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/weights/b1.h
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/weights/b2.h
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/weights/w1.h
+-rw-r--r--   0 runner    (1001) docker     (121)    21834 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/weights/w2.h
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/myproject.tcl
+-rw-r--r--   0 runner    (1001) docker     (121)     5176 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/conv2d-1layer/myproject_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/demo-conversion/
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/demo-conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/demo-conversion/keras-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/higgs-1layer/
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/build_prj.tcl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.354328 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/myproject.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/myproject.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/parameters.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.358327 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/b1.h
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/b2.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5393 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/w1.h
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/w2.h
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/myproject.tcl
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/higgs-1layer/myproject_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.358327 hls4ml-0.6.0/example-prjs/sublayer/
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/build_prj.tcl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.358327 hls4ml-0.6.0/example-prjs/sublayer/firmware/
+-rw-r--r--   0 runner    (1001) docker     (121)     3621 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/myproject.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/myproject.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3994 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/parameters.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.358327 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b1.h
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b2.h
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b2_0.h
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b2_1.h
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b3.h
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b4.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12253 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w1.h
+-rw-r--r--   0 runner    (1001) docker     (121)    17994 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w2.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9318 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w2_0.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8811 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w2_1.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8872 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w3.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2146 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w4.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1380 2021-11-12 12:26:42.000000 hls4ml-0.6.0/example-prjs/sublayer/myproject_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.358327 hls4ml-0.6.0/hls4ml/
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.362328 hls4ml-0.6.0/hls4ml/converters/
+-rw-r--r--   0 runner    (1001) docker     (121)    14532 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.362328 hls4ml-0.6.0/hls4ml/converters/keras/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2981 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/merge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3755 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/qkeras.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5199 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/qkeras_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2556 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras/reshaping.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13305 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/keras_to_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.362328 hls4ml-0.6.0/hls4ml/converters/onnx/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3520 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/onnx/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3868 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/onnx/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/onnx/merge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4564 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/onnx/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/onnx/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11228 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/onnx_to_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.362328 hls4ml-0.6.0/hls4ml/converters/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/pytorch/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2409 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/pytorch/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/pytorch/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6659 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/pytorch_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14936 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/tf_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2945 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/converters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.366328 hls4ml-0.6.0/hls4ml/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86993 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/hls_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30134 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/hls_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.366328 hls4ml-0.6.0/hls4ml/model/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (121)     2723 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.366328 hls4ml-0.6.0/hls4ml/model/optimizer/passes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/bn_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8721 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/bn_quant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3035 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/clone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3632 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/conv_same_pad.py
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/fuse_biasadd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/multi_dense.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/nop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2519 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/pointwise.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11376 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/qkeras.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5557 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/repack_stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/optimizer/passes/transpose_opt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24654 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/model/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.366328 hls4ml-0.6.0/hls4ml/report/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6797 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/report/vivado_report.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.370328 hls4ml-0.6.0/hls4ml/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/supported_boards.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.370328 hls4ml-0.6.0/hls4ml/templates/vivado/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.374328 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/
+-rw-r--r--   0 runner    (1001) docker     (121)    10180 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6473 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_decl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12185 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed.h
+-rw-r--r--   0 runner    (1001) docker     (121)    85182 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed_base.h
+-rw-r--r--   0 runner    (1001) docker     (121)    27302 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed_ref.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6985 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed_special.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10012 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int.h
+-rw-r--r--   0 runner    (1001) docker     (121)    71735 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int_base.h
+-rw-r--r--   0 runner    (1001) docker     (121)    55218 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int_ref.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6301 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int_special.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4894 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_shift_reg.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.374328 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/etc/
+-rw-r--r--   0 runner    (1001) docker     (121)   261465 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/etc/ap_private.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7480 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/hls_stream.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.374328 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/utils/x_hls_utils.h
+-rwxr-xr-x   0 runner    (1001) docker     (121)      529 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/build_lib.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     3730 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/build_prj.tcl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.374328 hls4ml-0.6.0/hls4ml/templates/vivado/firmware/
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/firmware/defines.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/firmware/myproject.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1055 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/firmware/myproject.h
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/firmware/parameters.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/myproject_bridge.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3252 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/myproject_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    29708 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_activation.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23337 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_activation_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_array.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5586 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4639 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2409 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8073 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_latency.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8253 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_resource.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3557 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3364 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19428 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_latency.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10328 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_resource.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4788 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13944 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3690 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_compressed.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5377 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_latency.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10540 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_resource.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2275 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    32133 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_garnet.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13118 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_image.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_image_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11530 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_merge.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9459 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_merge_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3450 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_mult.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4192 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_padding.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_padding_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11812 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_pooling.h
+-rw-r--r--   0 runner    (1001) docker     (121)    23183 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_pooling_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4897 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv1d_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6243 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv2d_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10909 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3580 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_types.h
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado/vivado_synth.tcl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/build_lib.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/myproject_axi.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/myproject_axi.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.350327 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/pynq-z2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/pynq-z2/python_drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/pynq-z2/python_drivers/axi_stream_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/pynq-z2/tcl_scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/pynq-z2/tcl_scripts/axi_lite_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (121)     3454 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/pynq-z2/tcl_scripts/axi_stream_design.tcl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.350327 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/zcu102/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/zcu102/python_drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/zcu102/python_drivers/axi_stream_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/zcu102/tcl_scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     3898 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator/zcu102/tcl_scripts/axi_stream_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (121)     6364 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3334 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_accelerator_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35803 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/templates/vivado_template.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14380 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5485 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/utils/example_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8789 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/utils/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.382328 hls4ml-0.6.0/hls4ml/writer/
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20850 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/writer/vivado_accelerator_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32743 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/writer/vivado_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2021-11-12 12:26:42.000000 hls4ml-0.6.0/hls4ml/writer/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.358327 hls4ml-0.6.0/hls4ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3002 2021-11-12 12:26:47.000000 hls4ml-0.6.0/hls4ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8901 2021-11-12 12:26:47.000000 hls4ml-0.6.0/hls4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-12 12:26:47.000000 hls4ml-0.6.0/hls4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-11-12 12:26:47.000000 hls4ml-0.6.0/hls4ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-11-12 12:26:47.000000 hls4ml-0.6.0/hls4ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-12 12:26:47.000000 hls4ml-0.6.0/hls4ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.386328 hls4ml-0.6.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8480 2021-11-12 12:26:42.000000 hls4ml-0.6.0/scripts/hls4ml
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-11-12 12:26:47.390328 hls4ml-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-11-12 12:26:42.000000 hls4ml-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.386328 hls4ml-0.6.0/test/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3301 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/build-prj.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1040 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/cleanup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2955 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/compare-reports.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2600 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/convert-keras-models.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2173 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/convert-onnx-models.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2180 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/convert-pytorch-models.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.390328 hls4ml-0.6.0/test/docker/
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     2962 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/docker/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/docker/install_config-2017.2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/docker/install_config.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1519 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/gather-reports.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      804 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/hls4ml-keras-test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1146 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/hls4ml-onnx-test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1170 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/hls4ml-pytorch-test.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/keras-models.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3747 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/keras-to-hls.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/onnx-models.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2379 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/onnx-to-hls.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 12:26:47.390328 hls4ml-0.6.0/test/pytest/
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/ci-template.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/generate_ci_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3051 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/test_cnn_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2728 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/test_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/test_globalpooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6947 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19189 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/test_keras_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10463 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/test_qkeras.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2810 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytest/test_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytorch-models.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2381 2021-11-12 12:26:42.000000 hls4ml-0.6.0/test/pytorch-to-hls.sh
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hls4ml-0.5.0b0/LICENSE` & `hls4ml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/PKG-INFO` & `hls4ml-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 Metadata-Version: 2.1
 Name: hls4ml
-Version: 0.5.0b0
+Version: 0.6.0
 Summary: Machine learning in FPGAs using HLS
 Home-page: https://github.com/hls-fpga-machine-learning/hls4ml
 Author: HLS4ML Team
 Author-email: hls4ml.help@gmail.com
 License: Apache 2.0
-Description: <p float="left">
-           <img src="https://fastmachinelearning.github.io/hls4ml/img/logo.jpg" alt="hls4ml" width="400"/>
-        </p>
-        
-        [![DOI](https://zenodo.org/badge/108329371.svg)](https://zenodo.org/badge/latestdoi/108329371)
-        [![PyPI version](https://badge.fury.io/py/hls4ml.svg)](https://badge.fury.io/py/hls4ml)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/hls4ml.svg)](https://pypi.org/project/hls4ml/)
-        
-        A package for machine learning inference in FPGAs. We create firmware implementations of machine learning algorithms using high level synthesis language (HLS). We translate traditional open-source machine learning package models into HLS that can be configured for your use-case!
-        
-        **Contact:** hls4ml.help@gmail.com
-        
-        # Documentation & Tutorial
-        
-        For more information visit the webpage: [https://fastmachinelearning.org/hls4ml/](https://fastmachinelearning.org/hls4ml/)
-        
-        Detailed tutorials on how to use `hls4ml`'s various functionalities can be found [here](https://github.com/hls-fpga-machine-learning/hls4ml-tutorial).
-        
-        # Installation
-        ```
-        pip install hls4ml
-        ```
-        
-        To install the extra dependencies for profiling: 
-        
-        ```
-        pip install hls4ml[profiling]
-        ```
-        
-        # Getting Started
-        ### Creating an HLS project
-        ```Python
-        import hls4ml
-        
-        #Fetch a keras model from our example repository
-        #This will download our example model to your working directory and return an example configuration file
-        config = hls4ml.utils.fetch_example_model('KERAS_3layer.json')
-        
-        print(config) #You can print the configuration to see some default parameters
-        
-        #Convert it to a hls project
-        hls_model = hls4ml.converters.keras_to_hls(config)
-        
-        # Print full list of example models if you want to explore more
-        hls4ml.utils.fetch_example_list()
-        ```
-        
-        ### Building a project with Xilinx Vitis (after downloading and installing from [here](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vitis.html))
-        
-        ```Python
-        #Use Vivado HLS to synthesize the model
-        #This might take several minutes
-        hls_model.build()
-        
-        #Print out the report if you want
-        hls4ml.report.read_vivado_report('my-hls-test')
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: profiling
+License-File: LICENSE
+
+<p float="left">
+   <img src="https://fastmachinelearning.github.io/hls4ml/img/logo.jpg" alt="hls4ml" width="400"/>
+</p>
+
+[![DOI](https://zenodo.org/badge/108329371.svg)](https://zenodo.org/badge/latestdoi/108329371)
+[![PyPI version](https://badge.fury.io/py/hls4ml.svg)](https://badge.fury.io/py/hls4ml)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/hls4ml.svg)](https://pypi.org/project/hls4ml/)
+
+A package for machine learning inference in FPGAs. We create firmware implementations of machine learning algorithms using high level synthesis language (HLS). We translate traditional open-source machine learning package models into HLS that can be configured for your use-case!
+
+**Contact:** hls4ml.help@gmail.com
+
+# Documentation & Tutorial
+
+For more information visit the webpage: [https://fastmachinelearning.org/hls4ml/](https://fastmachinelearning.org/hls4ml/)
+
+Detailed tutorials on how to use `hls4ml`'s various functionalities can be found [here](https://github.com/hls-fpga-machine-learning/hls4ml-tutorial).
+
+# Installation
+```
+pip install hls4ml
+```
+
+To install the extra dependencies for profiling: 
+
+```
+pip install hls4ml[profiling]
+```
+
+# Getting Started
+### Creating an HLS project
+```Python
+import hls4ml
+
+#Fetch a keras model from our example repository
+#This will download our example model to your working directory and return an example configuration file
+config = hls4ml.utils.fetch_example_model('KERAS_3layer.json')
+
+print(config) #You can print the configuration to see some default parameters
+
+#Convert it to a hls project
+hls_model = hls4ml.converters.keras_to_hls(config)
+
+# Print full list of example models if you want to explore more
+hls4ml.utils.fetch_example_list()
+```
+
+### Building a project with Xilinx Vivado HLS (after downloading and installing from [here](https://www.xilinx.com/products/design-tools/vivado/integration/esl-design.html))
+Note: Vitis HLS is not yet supported. Vivado HLS versions between 2018.2 and 2020.1 are recommended.
+
+```Python
+#Use Vivado HLS to synthesize the model
+#This might take several minutes
+hls_model.build()
+
+#Print out the report if you want
+hls4ml.report.read_vivado_report('my-hls-test')
+```
+
+
```

### Comparing `hls4ml-0.5.0b0/README.md` & `hls4ml-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 #Convert it to a hls project
 hls_model = hls4ml.converters.keras_to_hls(config)
 
 # Print full list of example models if you want to explore more
 hls4ml.utils.fetch_example_list()
 ```
 
-### Building a project with Xilinx Vitis (after downloading and installing from [here](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vitis.html))
+### Building a project with Xilinx Vivado HLS (after downloading and installing from [here](https://www.xilinx.com/products/design-tools/vivado/integration/esl-design.html))
+Note: Vitis HLS is not yet supported. Vivado HLS versions between 2018.2 and 2020.1 are recommended.
 
 ```Python
 #Use Vivado HLS to synthesize the model
 #This might take several minutes
 hls_model.build()
 
 #Print out the report if you want
```

### Comparing `hls4ml-0.5.0b0/example-prjs/conv-1layer/build_prj.tcl` & `hls4ml-0.6.0/example-prjs/conv-1layer/build_prj.tcl`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/myproject.cpp` & `hls4ml-0.6.0/example-prjs/conv-1layer/firmware/myproject.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/myproject.h` & `hls4ml-0.6.0/example-prjs/conv-1layer/firmware/myproject.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/parameters.h` & `hls4ml-0.6.0/example-prjs/conv-1layer/firmware/parameters.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/weights/w1.h` & `hls4ml-0.6.0/example-prjs/conv-1layer/firmware/weights/w1.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv-1layer/firmware/weights/w2.h` & `hls4ml-0.6.0/example-prjs/conv-1layer/firmware/weights/w2.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv-1layer/myproject_test.cpp` & `hls4ml-0.6.0/example-prjs/conv-1layer/myproject_test.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv2d-1layer/build_prj.tcl` & `hls4ml-0.6.0/example-prjs/conv2d-1layer/build_prj.tcl`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/myproject.cpp` & `hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/myproject.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/myproject.h` & `hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/myproject.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/parameters.h` & `hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/parameters.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv2d-1layer/firmware/weights/w2.h` & `hls4ml-0.6.0/example-prjs/conv2d-1layer/firmware/weights/w2.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/conv2d-1layer/myproject_test.cpp` & `hls4ml-0.6.0/example-prjs/conv2d-1layer/myproject_test.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/build_prj.tcl` & `hls4ml-0.6.0/example-prjs/higgs-1layer/build_prj.tcl`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/myproject.cpp` & `hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/myproject.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/myproject.h` & `hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/myproject.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/parameters.h` & `hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/parameters.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/b1.h` & `hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/b1.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/w1.h` & `hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/w1.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/firmware/weights/w2.h` & `hls4ml-0.6.0/example-prjs/higgs-1layer/firmware/weights/w2.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/higgs-1layer/myproject_test.cpp` & `hls4ml-0.6.0/example-prjs/higgs-1layer/myproject_test.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/build_prj.tcl` & `hls4ml-0.6.0/example-prjs/sublayer/build_prj.tcl`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/myproject.cpp` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/myproject.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/myproject.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/myproject.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/parameters.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/parameters.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b1.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b1.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b2.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b2.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/b3.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/b3.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w1.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w1.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w2.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w2.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w2_0.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w2_0.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w2_1.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w2_1.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w3.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w3.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/firmware/weights/w4.h` & `hls4ml-0.6.0/example-prjs/sublayer/firmware/weights/w4.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/example-prjs/sublayer/myproject_test.cpp` & `hls4ml-0.6.0/example-prjs/sublayer/myproject_test.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/convolution.py` & `hls4ml-0.6.0/hls4ml/converters/keras/convolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import math
 from hls4ml.converters.keras_to_hls import parse_default_keras_layer
 from hls4ml.converters.keras_to_hls import keras_handler
-from hls4ml.converters.keras_to_hls import parse_data_format
-from hls4ml.converters.keras_to_hls import compute_padding_1d
-from hls4ml.converters.keras_to_hls import compute_padding_2d
-
+from hls4ml.converters.utils import parse_data_format, compute_padding_1d, compute_padding_2d
 
 @keras_handler('Conv1D', 'SeparableConv1D')
 def parse_conv1d_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert('Conv1D' in keras_layer['class_name'])
 
     layer = parse_default_keras_layer(keras_layer, input_names)
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/core.py` & `hls4ml-0.6.0/hls4ml/converters/keras/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,48 +66,49 @@
         layer['bias_quantizer'] = BinaryQuantizer(bits=2)
     elif 'Ternary' in layer['class_name']:
         layer['weight_quantizer'] = TernaryQuantizer()
         layer['bias_quantizer'] = TernaryQuantizer()
     else:
         layer['weight_quantizer'] = None
         layer['bias_quantizer'] = None
-    output_shape = [input_shapes[0][0], layer['n_out']]
+    output_shape = input_shapes[0][:]
+    output_shape[-1] = layer['n_out']
 
     return layer, output_shape
 
 
 activation_layers = ['Activation', 'LeakyReLU', 'ThresholdedReLU', 'ELU', 'PReLU', 'Softmax', 'ReLU']
 @keras_handler(*activation_layers)
 def parse_activation_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert(keras_layer['class_name'] in activation_layers)
 
     layer = parse_default_keras_layer(keras_layer, input_names)
 
     if layer['class_name'] != 'Activation':
         layer['activation'] = layer['class_name']
     if layer['class_name'] == 'LeakyReLU':
-        layer['activ_param'] = keras_layer["config"].get('alpha', 0.3)
+        layer['activ_param'] = keras_layer['config'].get('alpha', 0.3)
     elif layer['class_name'] == 'ThresholdedReLU':
-        layer['activ_param'] = keras_layer["config"].get('theta', 1.)
+        layer['activ_param'] = keras_layer['config'].get('theta', 1.)
     elif layer['class_name'] == 'ELU':
-        layer['activ_param'] = keras_layer["config"].get('alpha', 1.)
+        layer['activ_param'] = keras_layer['config'].get('alpha', 1.)
     elif layer['class_name'] == 'ReLU':
         layer['class_name'] = 'Activation'
 
     if layer['class_name'] == 'Activation' and layer['activation'] == 'softmax':
         layer['class_name'] = 'Softmax'
-    if layer['class_name'] == 'ReLU':
-        layer['class_name'] = 'Activation'
+    if layer['class_name'] == 'Softmax':
+        layer['axis'] = keras_layer['config'].get('axis', -1)
     
     return layer, [shape for shape in input_shapes[0]]
 
 
 @keras_handler('BatchNormalization')
 def parse_batchnorm_layer(keras_layer, input_names, input_shapes, data_reader, config):
-    assert('BatchNormalization' in keras_layer['class_name'])
+    assert('BatchNormalization' in keras_layer['class_name'] or 'QConv2DBatchnorm' in keras_layer['class_name'])
 
     layer = parse_default_keras_layer(keras_layer, input_names)
 
     in_size = 1
     for dim in input_shapes[0][1:]:
         in_size *= dim
     layer['n_in'] = in_size
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/graph.py` & `hls4ml-0.6.0/hls4ml/converters/keras/graph.py`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/merge.py` & `hls4ml-0.6.0/hls4ml/converters/keras/merge.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 def parse_merge_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert(keras_layer['class_name'] in merge_layers)
 
     layer = parse_default_keras_layer(keras_layer, input_names)
 
     layer['op'] = layer['class_name'].lower()
 
+    output_shape = input_shapes[0][:]
     if layer['class_name'] == 'Concatenate':
         rank = len(input_shapes[0][1:])
         if rank > 3:
             raise Exception('ERROR: Concatenation of tensors with rank > 3 is not yet supported.')
         layer['op'] = layer['class_name'].lower() + '{}d'.format(rank)
         layer['axis'] = keras_layer['config']['axis']
-        #TODO handle output shape
+        output_shape[layer['axis']] += input_shapes[1][layer['axis']]
     elif layer['class_name'] == 'Dot':
         rank = len(input_shapes[0][1:])
         if rank > 1:
             raise Exception('ERROR: Dot of tensors with rank > 1 is not yet supported.')
         layer['op'] = layer['class_name'].lower() + '{}d'.format(rank) 
     else:
         layer['class_name'] = 'Merge'
     if len(layer['inputs']) > 2:
         raise Exception('ERROR: Merging more than two tensors is not yet supported.')
 
-    return layer, input_shapes[0]
+    return layer, output_shape
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/pooling.py` & `hls4ml-0.6.0/hls4ml/converters/keras/pooling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import math
 from hls4ml.converters.keras_to_hls import parse_default_keras_layer
 from hls4ml.converters.keras_to_hls import keras_handler
-from hls4ml.converters.keras_to_hls import parse_data_format
-from hls4ml.converters.keras_to_hls import compute_padding_1d
-from hls4ml.converters.keras_to_hls import compute_padding_2d
-
+from hls4ml.converters.utils import parse_data_format, compute_padding_1d, compute_padding_2d
 
 pooling_layers = ['MaxPooling1D', 'MaxPooling2D', 'AveragePooling1D', 'AveragePooling2D']
 @keras_handler(*pooling_layers)
 def parse_pooling_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert('Pooling' in keras_layer['class_name'])
 
     layer = parse_default_keras_layer(keras_layer, input_names)
@@ -71,16 +68,16 @@
         if layer['data_format'] == 'channels_last':
             output_shape=[input_shapes[0][0], layer['out_height'], layer['out_width'], layer['n_filt']]
         elif layer['data_format'] == 'channels_first':
             output_shape=[input_shapes[0][0], layer['n_filt'], layer['out_height'], layer['out_width']]
     
     return layer, output_shape
 
-pooling_layers = ['GlobalMaxPooling1D', 'GlobalMaxPooling2D', 'GlobalAveragePooling1D', 'GlobalAveragePooling2D']
-@keras_handler(*pooling_layers)
+global_pooling_layers = ['GlobalMaxPooling1D', 'GlobalMaxPooling2D', 'GlobalAveragePooling1D', 'GlobalAveragePooling2D']
+@keras_handler(*global_pooling_layers)
 def parse_global_pooling_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert('Pooling' in keras_layer['class_name'])
 
     layer = parse_default_keras_layer(keras_layer, input_names)
 
     if int(layer['class_name'][-2]) == 1:
         (
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/qkeras.py` & `hls4ml-0.6.0/hls4ml/converters/keras/qkeras.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         return ExponentPrecisionType(width=width, signed=True)
     if width == integer:
         if width == 1:
             return XnorPrecisionType()
         else:
             return IntegerPrecisionType(width=width, signed=True)
     else:
-        return FixedPrecisionType(width=width+1, integer=integer+1, signed=True)
+        return FixedPrecisionType(width=width, integer=integer+1, signed=True)
 
 def get_quantizer_from_config(keras_layer, quantizer_var):
     quantizer_config = keras_layer['config']['{}_quantizer'.format(quantizer_var)]
     if keras_layer['class_name'] == 'QBatchNormalization':
         return QKerasQuantizer(quantizer_config)
     elif 'binary' in quantizer_config['class_name']:
         return QKerasBinaryQuantizer(quantizer_config, xnor=(quantizer_var == 'kernel'))
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/qkeras_layers.py` & `hls4ml-0.6.0/hls4ml/converters/keras/qkeras_layers.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     return layer, output_shape
 
 
 @keras_handler('QConv1D', 'QConv2D')
 def parse_qconv_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert('QConv' in keras_layer['class_name'])
     
-    if int(keras_layer['class_name'][-2]) == 1:
+    if '1D' in keras_layer['class_name']:
         layer, output_shape = parse_conv1d_layer(keras_layer, input_names, input_shapes, data_reader, config)
-    elif int(keras_layer['class_name'][-2]) == 2:
+    elif '2D' in keras_layer['class_name']:
         layer, output_shape = parse_conv2d_layer(keras_layer, input_names, input_shapes, data_reader, config)
 
     layer['weight_quantizer'] = get_quantizer_from_config(keras_layer, 'kernel')
     if keras_layer['config']['bias_quantizer'] is not None:
         layer['bias_quantizer'] = get_quantizer_from_config(keras_layer, 'bias')
     else:
         layer['bias_quantizer'] = None
@@ -47,46 +47,47 @@
 def parse_qactivation_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert(keras_layer['class_name'] == 'QActivation')
     supported_activations = ['quantized_relu', 'quantized_tanh', 'binary_tanh', 'ternary_tanh', 'quantized_bits', 'binary', 'ternary']
     
     layer = parse_default_keras_layer(keras_layer, input_names)
 
     activation_config = keras_layer['config']['activation']
-    if isinstance(activation_config, str):
-        quantizer_obj = get_quantizer(activation_config)
-
-    if isinstance(activation_config, str):
-        quantizer_obj = get_quantizer(activation_config)
-        activation_config = {}
-        # some activations are classes 
-        if hasattr(quantizer_obj, 'get_config'):
-            print("Name: " + quantizer_obj.__class__.__name__)
-            activation_config['class_name'] = quantizer_obj.__class__.__name__
-            if activation_config['class_name'] == 'ternary' or activation_config['class_name'] == 'binary':
-                activation_config['class_name'] += '_tanh'
-            activation_config['config'] = quantizer_obj.get_config()
-        # some activation quantizers are just functions with no config
+    quantizer_obj = get_quantizer(activation_config)
+    activation_config = {}
+    # some activations are classes 
+    if hasattr(quantizer_obj, 'get_config'):
+        activation_config['class_name'] = quantizer_obj.__class__.__name__
+        if activation_config['class_name'] == 'ternary' or activation_config['class_name'] == 'binary':
+            activation_config['class_name'] += '_tanh'
+        activation_config['config'] = quantizer_obj.get_config()
+    # some activation quantizers are just functions with no config
+    else:
+        activation_config['config'] = {}
+        if 'binary' in quantizer_obj.__name__:
+            activation_config['class_name'] = 'binary_tanh'
+            activation_config['config']['bits'] = 1
+            activation_config['config']['integer'] = 1
+        elif 'ternary' in quantizer_obj.__name__:
+            activation_config['class_name'] = 'ternary_tanh'
+            activation_config['config']['bits'] = 2
+            activation_config['config']['integer'] = 2
         else:
-            activation_config['config'] = {}
-            if 'binary' in quantizer_obj.__name__:
-                activation_config['class_name'] = 'binary_tanh'
-                activation_config['config']['bits'] = 1
-                activation_config['config']['integer'] = 1
-            elif 'ternary' in quantizer_obj.__name__:
-                activation_config['class_name'] = 'ternary_tanh'
-                activation_config['config']['bits'] = 2
-                activation_config['config']['integer'] = 2
-            else:
-                activation_config['class_name'] = 'unknown'
+            activation_config['class_name'] = 'unknown'
     
     if activation_config['class_name'] not in supported_activations:
         raise Exception('Unsupported QKeras activation: {}'.format(activation_config['class_name']))
 
 
-    layer['class_name'] = 'Activation'
+    if activation_config['class_name'] == 'ternary_tanh':
+        layer['class_name'] = 'TernaryTanh'
+        layer['threshold'] = activation_config.get('config', {}).get('threshold', 0.33)
+        if layer['threshold'] is None:
+            layer['threshold'] = 0.33 # the default ternary tanh threshold for QKeras
+    else:
+        layer['class_name'] = 'Activation'
     if activation_config['class_name'] == 'quantized_bits':
         activation_config['class_name'] = 'linear'
     layer['activation'] = activation_config['class_name'].replace('quantized_', '')
     return layer, [shape for shape in input_shapes[0]]
 
 @keras_handler('QBatchNormalization')
 def parse_qbatchnorm_layer(keras_layer, input_names, input_shapes, data_reader, config):
@@ -96,7 +97,16 @@
     layer['mean_quantizer'] = get_quantizer_from_config(keras_layer, 'mean')
     layer['variance_quantizer'] = get_quantizer_from_config(keras_layer, 'variance')
     layer['beta_quantizer'] = get_quantizer_from_config(keras_layer, 'beta')
     layer['gamma_quantizer'] = get_quantizer_from_config(keras_layer, 'gamma')
 
     return layer, output_shape
 
+
+@keras_handler('QConv2DBatchnorm')
+def parse_qconv2dbatchnorm_layer(keras_layer, input_names, input_shapes, data_reader, config):
+    intermediate_shape = list()
+    conv_layer, shape_qconv = parse_qconv_layer(keras_layer, input_names, input_shapes, data_reader, config)
+    intermediate_shape.append(shape_qconv)
+    temp_shape = intermediate_shape
+    batch_layer, out_shape = parse_batchnorm_layer(keras_layer, input_names, temp_shape, data_reader, config)
+    return {**conv_layer, **batch_layer}, out_shape
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/reshape.py` & `hls4ml-0.6.0/hls4ml/converters/keras/reshape.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 import numpy as np
 
 from hls4ml.converters.keras_to_hls import parse_default_keras_layer
 from hls4ml.converters.keras_to_hls import keras_handler
-from hls4ml.converters.keras_to_hls import parse_data_format
+from hls4ml.converters.utils import parse_data_format
+
+@keras_handler('Flatten')
+def parse_flatten_layer(keras_layer, input_names, input_shapes, data_reader, config):
+    assert(keras_layer["class_name"] == 'Flatten')
+
+    layer = parse_default_keras_layer(keras_layer, input_names)
+    
+    layer['class_name'] = 'Reshape'
+    layer['target_shape'] = [input_shapes[0][0], np.prod(input_shapes[0][1:])]
+    output_shape = layer['target_shape']
+    
+    return layer, output_shape
 
 @keras_handler('Reshape')
 def parse_reshape_layer(keras_layer, input_names, input_shapes, data_reader, config):
     assert(keras_layer["class_name"] == 'Reshape')
 
     layer = parse_default_keras_layer(keras_layer, input_names)
     
@@ -37,8 +49,22 @@
     layer['out_width'] = layer['in_width'] * layer['width_factor']
     
     if layer['data_format'] == 'channels_first':
         output_shape = [input_shapes[0][0], layer['n_chan'], layer['out_height'], layer['out_width']]
     else:
         output_shape = [input_shapes[0][0], layer['out_height'], layer['out_width'], layer['n_chan']]
 
-    return layer, output_shape
+    return layer, output_shape
+
+@keras_handler('Permute')
+def parse_permute_layer(keras_layer, input_names, input_shapes, data_reader, config):
+    assert(keras_layer['class_name'] == 'Permute')
+
+    layer = parse_default_keras_layer(keras_layer, input_names)
+
+    layer['class_name'] = 'Transpose'
+    dims = keras_layer['config']['dims']
+    layer['perm'] = [dim - 1 for dim in keras_layer['config']['dims']]
+    
+    output_shape = [input_shapes[0][0]] + [input_shapes[0][s] for s in dims]
+
+    return layer, output_shape
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras/reshaping.py` & `hls4ml-0.6.0/hls4ml/converters/keras/reshaping.py`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/keras_to_hls.py` & `hls4ml-0.6.0/hls4ml/converters/keras_to_hls.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,17 +120,16 @@
         layer['epsilon'] = keras_layer['config']['epsilon']
     if 'use_bias' in keras_layer['config']:
         layer['use_bias'] = keras_layer['config']['use_bias']
 
     return layer
 
 def parse_data_format(input_shape, data_format='channels_last'):
-    if input_shape[0] is None:
-        # Ignore batch size
-        input_shape = input_shape[1:]
+    # Ignore batch size
+    input_shape = input_shape[1:]
     
     if data_format.lower() == 'channels_last':
         if len(input_shape) == 2: # 1D, (n_in, n_filt)
             return (input_shape[0], input_shape[1])
         elif len(input_shape) == 3: # 2D, (in_height, in_width, n_filt)
             return (input_shape[0], input_shape[1], input_shape[2])
         
@@ -198,16 +197,20 @@
     ######################
 
     #This is a list of dictionaries to hold all the layer info we need to generate HLS
     layer_list = []
 
     if 'KerasModel' in config:
         # Model instance passed in config from API
-        model_arch = json.loads(config['KerasModel'].to_json())
-        reader = KerasModelReader(config['KerasModel'])
+        keras_model = config['KerasModel']
+        if isinstance(keras_model, str):
+            from tensorflow.keras.models import load_model
+            keras_model = load_model(keras_model)
+        model_arch = json.loads(keras_model.to_json())
+        reader = KerasModelReader(keras_model)
     elif 'KerasJson' in config:
         # Extract model architecture from json
         with open(config['KerasJson']) as json_file:
             model_arch = json.load(json_file)
         reader = KerasFileReader(config)
     elif 'KerasH5' in config:
         # Model arch and weights are in H5 file (from model.save() function)
@@ -221,15 +224,15 @@
         reader = KerasFileReader(config)
     else:
         raise ValueError('No model found in config file.')
 
     #print(model_arch)
 
     #Define layers to skip for conversion to HLS
-    skip_layers = ['Dropout', 'Flatten']
+    skip_layers = ['Dropout']
     #All supported layers
     supported_layers = get_supported_keras_layers() + skip_layers
 
     #Map inputs of skipped and split (activation) layers
     inputs_map = {}
 
     #Loop through layers
@@ -266,63 +269,61 @@
     output_shapes = {}
     output_shape = None
 
     print('Topology:')
     for keras_layer in layer_config:
         if 'batch_input_shape' in keras_layer['config']:
             if 'inbound_nodes' in keras_layer and len(keras_layer['inbound_nodes']) > 0:
-                input_shapes = [output_shapes[inbound_node[0][0]] for inbound_node in keras_layer['inbound_nodes']]
+                input_shapes = [output_shapes[inbound_node[0]] for inbound_node in keras_layer['inbound_nodes'][0]]
             else:
                 input_shapes = [keras_layer['config']['batch_input_shape']]
         else:
             if 'inbound_nodes' in keras_layer:
-                input_shapes = [output_shapes[inbound_node[0][0]] for inbound_node in keras_layer['inbound_nodes']]
+                input_shapes = [output_shapes[inbound_node[0]] for inbound_node in keras_layer['inbound_nodes'][0]]
             else:
                 # Sequential model, so output_shape from the previous layer is still valid 
                 input_shapes = [output_shape]
 
         keras_class = keras_layer['class_name']
 
         if keras_class in skip_layers:
             if 'inbound_nodes' in keras_layer:
                 name = keras_layer['config']['name']
                 #Currently supported skipped layers have only one input
                 parent_input = keras_layer['inbound_nodes'][0][0][0]
                 #Skipped layers can follow each other (e.g., Dropout -> Flatten)
                 inputs_map[name] = inputs_map.get(parent_input, parent_input)
 
-            if keras_class == 'Flatten':
-                output_shapes[keras_layer['config']['name']] = [input_shapes[0][0], np.prod(input_shapes[0][1:])]
-            else:
-                output_shapes[keras_layer['config']['name']] = input_shapes[0]
+            output_shapes[keras_layer['config']['name']] = input_shapes[0]
 
             continue
 
         if keras_class in supported_layers:
             layer_counter = layer_counter + 1
 
         #Extract inbound nodes
         if 'inbound_nodes' in keras_layer and len(keras_layer['inbound_nodes']) > 0:
             input_names = [ inputs_map.get(inp[0], inp[0]) for inp in keras_layer['inbound_nodes'][0] ]
         else:
             input_names = None
 
         layer, output_shape = layer_handlers[keras_class](keras_layer, input_names, input_shapes, reader, config)
 
-        print('Layer name: {}, layer type: {}, current shape: {}'.format(layer['name'], layer['class_name'], input_shapes))
+        print('Layer name: {}, layer type: {}, input shapes: {}, output shape: {}'.format(layer['name'], layer['class_name'], input_shapes, output_shape))
         layer_list.append( layer )
-        if 'activation' in layer and layer['class_name'] not in ['Activation', 'LeakyReLU', 'ThresholdedReLU', 'ELU', 'PReLU', 'Softmax']:# + qkeras_layers:
+        if 'activation' in layer and layer['class_name'] not in ['Activation', 'LeakyReLU', 'ThresholdedReLU', 'ELU', 'PReLU', 'Softmax', 'TernaryTanh']:# + qkeras_layers:
             act_layer = {}
             act_layer['name'] = layer['name'] + '_' + layer['activation']
             act_layer['activation'] = layer['activation']
             if 'activ_param' in layer:
                 act_layer['activ_param'] = layer['activ_param']
                 act_layer['class_name'] = layer['activation']
             elif layer['activation'] == 'softmax':
                 act_layer['class_name'] = 'Softmax'
+                act_layer['axis'] = -1
             else:
                 act_layer['class_name'] = 'Activation'
             inputs_map[layer['name']] = act_layer['name']
             if output_layers is not None and layer['name'] in output_layers:
                 output_layers = [act_layer['name'] if name == layer['name'] else name for name in output_layers]
             layer_list.append(act_layer)
```

### Comparing `hls4ml-0.5.0b0/hls4ml/converters/tf_to_hls.py` & `hls4ml-0.6.0/hls4ml/converters/tf_to_hls.py`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/model/hls_layers.py` & `hls4ml-0.6.0/hls4ml/model/hls_layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -360,14 +360,15 @@
         self.weights = OrderedDict()
         self.variables = OrderedDict()
         self.precision = OrderedDict()
         accum_t = HLSType(*reversed(self.model.config.get_precision(self, 'accum')))
         self.precision[accum_t.name] = accum_t
         self.set_attr('accum_t', accum_t.precision)
         self.reuse_factor = self.model.config.get_reuse_factor(self)
+        self.target_cycles = self.model.config.get_target_cycles(self)
 
         layer_config = self.model.config.get_layer_config(self)
         for config_key, config_value in layer_config.items():
             if config_key in self.attributes:
                 print('WARNING: Config parameter "{}" overwrites an existing attribute in layer "{}" ({})'.format(config_key, self.name, self.__class__.__name__))
             self.attributes[config_key] = config_value
 
@@ -380,15 +381,19 @@
         self.attributes[key] = value
 
     def get_attr(self, key, default=None):
         return self.attributes.get(key, default)
 
     def get_input_node(self, input_name=None):
         if input_name is not None:
-            return self.model.graph.get(input_name)
+            nodes = [node for node in self.model.graph.values() if input_name in node.outputs]
+            if len(nodes) == 0:
+                return None
+            else:
+                return nodes[0]
         else:
             return self.model.graph.get(self.inputs[0])
 
     def get_input_variable(self, input_name=None):
         if input_name is not None:
             return self.model.get_layer_output_variable(input_name)
         else:
@@ -500,14 +505,20 @@
         else:
             var = WeightVariable(var_name, type_name=type_name, precision=precision, quantizer=quantizer, data=data, index=self.index)
 
         var.data_unquantized = data_unquantized
         self.weights[name] = var
         self.precision[var.type.name] = var.type
 
+        # Register weights as BRAM if exceeds threshold
+        bramport_size = self.model.config.get_bram_size(self)
+        if(np.prod(data.shape) > bramport_size):
+            var_out = var_name.replace("{index}",str(self.index))
+            self.model.register_bram_variable(var_out,var)
+
     def _default_function_params(self):
         params = {}
         params['config'] = 'config{}'.format(self.index)
         params['input_t'] = self.get_input_variable().type.name
         params['output_t'] = self.get_output_variable().type.name
         params['input'] = self.get_input_variable().name
         params['output'] = self.get_output_variable().name
@@ -586,34 +597,39 @@
         return None
 
     def config_cpp(self):
         return None
 
 class Dense(Layer):
     def initialize(self):
-        shape = [self.attributes['n_out']]
-        dims = ['N_LAYER_{}'.format(self.index)]
+        shape = self.get_input_variable().shape[:]
+        shape[-1] = self.attributes['n_out']
+        if len(shape) > 1:
+            dims = ['N_LAYER_{}_{}'.format(i, self.index) for i in range(1, len(shape) + 1)]
+        else:
+            dims = ['N_LAYER_{}'.format(self.index)]
         compression = self.model.config.get_compression(self)
         if self.model.config.is_resource_strategy(self):
-            if self.model.config.backend.name == 'Vivado':
+            if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
+                self.model.config.backend.set_target_reuse_factor(self)
                 self.model.config.backend.set_closest_reuse_factor(self)
             if compression:
                 self.set_attr('strategy', 'compressed')
             else:
                 self.set_attr('strategy', 'resource')
         else:
             self.set_attr('strategy', 'latency')
         self.add_output_variable(shape, dims)
         self.add_weights(quantizer=self.get_attr('weight_quantizer'), compression=compression)
         index_t = IntegerPrecisionType(width=1, signed=False)
         if self.model.config.is_resource_strategy(self):
             if self.model.config.get_compression(self):
                 index_t = self.get_weights('weight').type.index_precision
             else:
-                if self.model.config.backend.name == 'Vivado':
+                if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
                     self.weights['weight'].data = np.transpose(self.weights['weight'].data)
                     
         self.set_attr('index_t', index_t)
         self.add_bias(quantizer=self.get_attr('bias_quantizer'))
 
     def function_cpp(self):
         params = self._default_function_params()
@@ -641,21 +657,26 @@
         else:
             shape = [self.attributes['n_filt'], self.attributes['out_width']]
             dims = ['N_FILT_{}'.format(self.index), 'N_OUTPUTS_{}'.format(self.index)]
 
         self.add_output_variable(shape, dims)
         self.add_weights(quantizer = self.get_attr('weight_quantizer'))
         self.add_bias(quantizer = self.get_attr('bias_quantizer'))
+        if len(self.weights['weight'].data.shape) == 2: # This can happen if we assign weights of Dense layer to 1x1 Conv2D
+            self.weights['weight'].data = np.expand_dims(self.weights['weight'].data, axis=0)
+
         if self.model.config.is_resource_strategy(self):
             self.set_attr('strategy', 'resource')
-            if self.model.config.backend.name == 'Vivado':
+            if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
+                self.model.config.backend.set_target_reuse_factor(self)
                 self.model.config.backend.set_closest_reuse_factor(self)
-                self.weights['weight'].data = np.transpose(self.weights['weight'].data, axes=[2, 1, 0]) #(W,C,F) => (F,C,W)
+                self.weights['weight'].data = np.transpose(self.weights['weight'].data, axes=[2, 0, 1]) #(W,C,F) => (F,W,C)
         else:
             self.set_attr('strategy', 'latency')
+        self.set_attr('implementation', self.model.config.get_conv_implementation(self).lower())
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
         params['w'] = self.get_weights('weight').name
         params['b'] = self.get_weights('bias').name
 
@@ -717,20 +738,22 @@
         
         zero_bias_data = np.zeros((self.attributes['n_chan'],))
         self.add_weights_variable(name='zero_bias', var_name='z{index}', data=zero_bias_data)
 
         self.add_bias(quantizer=self.get_attr('bias_quantizer'))
         if self.model.config.is_resource_strategy(self):
             self.set_attr('strategy', 'resource')
-            if self.model.config.backend.name == 'Vivado':
+            if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
                 self.model.config.backend.set_closest_reuse_factor(self)
-                self.weights['depthwise'].data = np.transpose(self.weights['depthwise'].data, axes=[2, 1, 0]) #(W,C,F) => (F,C,W)
-                self.weights['pointwise'].data = np.transpose(self.weights['pointwise'].data, axes=[2, 1, 0]) #(W,C,F) => (F,C,W)
+                self.weights['depthwise'].data = np.transpose(self.weights['depthwise'].data, axes=[2, 0, 1]) #(W,C,F) => (F,W,C)
+                self.weights['pointwise'].data = np.transpose(self.weights['pointwise'].data, axes=[2, 0, 1]) #(W,C,F) => (F,W,C)
         else:
             self.set_attr('strategy', 'latency')
+        self.set_attr('implementation', self.model.config.get_conv_implementation(self).lower())
+        
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
         params['d'] = self.get_weights('depthwise').name
         params['p'] = self.get_weights('pointwise').name
         params['b'] = self.get_weights('bias').name
@@ -830,19 +853,25 @@
             dims = ['OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index), 'N_FILT_{}'.format(self.index)]
         else:
             shape = [self.attributes['n_filt'], self.attributes['out_height'], self.attributes['out_width']]
             dims = ['N_FILT_{}'.format(self.index), 'OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index)]
         self.add_output_variable(shape, dims)
         self.add_weights(quantizer=self.get_attr('weight_quantizer'))
         self.add_bias(quantizer=self.get_attr('bias_quantizer'))
+        if len(self.weights['weight'].data.shape) == 2: # This can happen if we assign weights of Dense layer to 1x1 Conv2D
+            self.weights['weight'].data = np.expand_dims(self.weights['weight'].data, axis=(0,1))
+
+        self.set_attr('implementation', self.model.config.get_conv_implementation(self).lower())
+
         if self.model.config.is_resource_strategy(self):
             self.set_attr('strategy', 'resource')
-            if self.model.config.backend.name == 'Vivado':
+            if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
+                self.model.config.backend.set_target_reuse_factor(self)
                 self.model.config.backend.set_closest_reuse_factor(self)
-                self.weights['weight'].data = np.transpose(self.weights['weight'].data, axes=[3, 2, 0, 1]) #(H,W,C,F) => (F,C,H,W)
+                self.weights['weight'].data = np.transpose(self.weights['weight'].data, axes=[3, 0, 1, 2]) #(H,W,C,F) => (F,H,W,C)
         else:
             self.set_attr('strategy', 'latency')
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
         params['w'] = self.get_weights('weight').name
@@ -892,14 +921,66 @@
         mult_params['n_in'] = self.get_attr('n_chan') * self.get_attr('filt_height') * self.get_attr('filt_width')
         mult_params['n_out'] = self.get_attr('n_filt')
         mult_params['product_type'] = self.model.config.backend.product_type(self.get_input_variable().type.precision, self.get_weights('weight').type.precision)
         mult_config = self._config_template[1].format(**mult_params)
 
         return mult_config + '\n' + conv_config
 
+
+class Conv2DBatchnorm(Conv2D):
+    def _get_folded_weights(self):
+        """
+        Function to get the batchnorm folded weights.
+        This function converts the weights by folding batchnorm parameters into
+        the weight of QConv2D. The high-level equation:
+        W_fold = gamma * W / sqrt(variance + epsilon)
+        bias_fold = gamma * (bias - moving_mean) / sqrt(variance + epsilon) + beta
+        """
+        kernel = self.model.get_weights_data(self.name, 'kernel')
+        bias = self.model.get_weights_data(self.name, 'bias')
+        if bias is None:
+            bias = 0
+
+        # get batchnorm weights and moving stats
+        gamma = self.model.get_weights_data(self.name, 'gamma')
+        beta = self.model.get_weights_data(self.name, 'beta')
+        moving_mean = self.model.get_weights_data(self.name, 'moving_mean')
+        moving_variance = self.model.get_weights_data(self.name, 'moving_variance')
+        # get the inversion factor so that we replace division by multiplication
+        inv = np.reciprocal(np.sqrt(moving_variance + self.get_attr('epsilon')))
+        if gamma is not None:
+            inv *= gamma
+
+        # wrap conv kernel and bias with bn parameters
+        folded_kernel = inv * kernel
+        folded_bias = inv * (bias - moving_mean) + beta
+
+        return [folded_kernel, folded_bias]
+
+    def initialize(self):
+        super(Conv2DBatchnorm, self).initialize()
+        folded_weights, folded_bias = self._get_folded_weights()
+        if self.model.config.is_resource_strategy(self) and self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
+            self.weights['weight'].data_unquantized = np.transpose(folded_weights, axes=[3, 0, 1, 2])
+            self.weights['weight'].data = self.get_attr('weight_quantizer')(self.weights['weight'].data_unquantized)
+
+        else:
+            self.weights['weight'].data_unquantized = folded_weights
+            self.weights['weight'].data = self.get_attr('weight_quantizer')(folded_weights)
+        self.weights['bias'].data_unquantized = folded_bias
+        bias_q = self.get_attr('bias_quantizer')
+        if bias_q is not None:
+            self.weights['bias'].data = bias_q(folded_bias)
+
+    def function_cpp(self):
+        return super(Conv2DBatchnorm, self).function_cpp()
+
+    def config_cpp(self):
+        return super(Conv2DBatchnorm, self).config_cpp()
+
 class SeparableConv2D(Layer):
     def initialize(self):
         if self.get_attr('data_format') == 'channels_last':
             shape = [self.attributes['out_height'], self.attributes['out_width'], self.attributes['n_filt']]
             dims = ['OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index), 'N_FILT_{}'.format(self.index)]
         else:
             shape = [self.attributes['n_filt'], self.attributes['out_height'], self.attributes['out_width']]
@@ -914,20 +995,22 @@
         
         zero_bias_data = np.zeros((self.attributes['n_chan'],))
         self.add_weights_variable(name='zero_bias', var_name='z{index}', data=zero_bias_data)
 
         self.add_bias(quantizer=self.get_attr('bias_quantizer'))
         if self.model.config.is_resource_strategy(self):
             self.set_attr('strategy', 'resource')
-            if self.model.config.backend.name == 'Vivado':
+            if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
                 self.model.config.backend.set_closest_reuse_factor(self)
-                self.weights['depthwise'].data = np.transpose(self.weights['depthwise'].data, axes=[3, 2, 0, 1]) #(H,W,C,F) => (F,C,H,W)
-                self.weights['pointwise'].data = np.transpose(self.weights['pointwise'].data, axes=[3, 2, 0, 1]) #(H,W,C,F) => (F,C,H,W)
+                self.weights['depthwise'].data = np.transpose(self.weights['depthwise'].data, axes=[3, 0, 1, 2]) #(H,W,C,F) => (F,H,W,C)
+                self.weights['pointwise'].data = np.transpose(self.weights['pointwise'].data, axes=[3, 0, 1, 2]) #(H,W,C,F) => (F,H,W,C)
         else:
             self.set_attr('strategy', 'latency')
+        
+        self.set_attr('implementation', self.model.config.get_conv_implementation(self).lower())
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
         params['d'] = self.get_weights('depthwise').name
         params['p'] = self.get_weights('pointwise').name
         params['b'] = self.get_weights('bias').name
@@ -1045,30 +1128,33 @@
 
         depthwise_data = self.model.get_weights_data(self.name, 'depthwise_kernel')
         self.add_weights_variable(name='weight', var_name='w{index}', data=depthwise_data, quantizer=self.get_attr('depthwise_quantizer'))
 
         self.add_bias(quantizer=self.get_attr('bias_quantizer'))
         if self.model.config.is_resource_strategy(self):
             self.set_attr('strategy', 'resource')
-            if self.model.config.backend.name == 'Vivado':
+            if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
                 self.model.config.backend.set_closest_reuse_factor(self)
-                self.weights['weight'].data = np.transpose(self.weights['weight'].data, axes=[3, 2, 0, 1]) #(H,W,C,F) => (F,C,H,W)
+                self.weights['weight'].data = np.transpose(self.weights['weight'].data, axes=[3, 0, 1, 2]) #(H,W,C,F) => (F,H,W,C)
         else:
             self.set_attr('strategy', 'latency')
+        
+        self.set_attr('implementation', self.model.config.get_conv_implementation(self).lower())
 
 class Pooling1D(Layer):
     def initialize(self):
         if self.get_attr('data_format') == 'channels_last':
             shape = [self.attributes['n_out'], self.attributes['n_filt']]
             dims = ['N_OUTPUTS_{}'.format(self.index), 'N_FILT_{}'.format(self.index)]
         else:
             shape = [self.attributes['n_filt'], self.attributes['n_out']]
             dims = ['N_FILT_{}'.format(self.index), 'N_OUTPUTS_{}'.format(self.index)]
         self.add_output_variable(shape, dims)
         self.set_attr('pool_op', self.get_attr('class_name').split('Pooling')[0])
+        self.set_attr('implementation', self.model.config.get_conv_implementation(self).lower())
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
 
         return [self._function_template.format(**params)]
 
@@ -1076,29 +1162,30 @@
         params = self._default_config_params()
         if self.get_attr('data_format') == 'channels_last':
             params['n_in'] = self.get_input_variable().dim_names[0]
             params['n_out'] = self.get_output_variable().dim_names[0]
             params['n_filt'] = self.get_output_variable().dim_names[1]
         else:
             params['n_in'] = self.get_input_variable().dim_names[1]
-            params['n_out'] = self.get_input_variable().dim_names[1]
+            params['n_out'] = self.get_output_variable().dim_names[1]
             params['n_filt'] = self.get_output_variable().dim_names[0]
 
         return self._config_template.format(**params)
 
 class Pooling2D(Layer):
     def initialize(self):
         if self.get_attr('data_format') == 'channels_last':
             shape = [self.attributes['out_height'], self.attributes['out_width'], self.attributes['n_filt']]
             dims = ['OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index), 'N_FILT_{}'.format(self.index)]
         else:
             shape = [self.attributes['n_filt'], self.attributes['out_height'], self.attributes['out_width']]
             dims = ['N_FILT_{}'.format(self.index), 'OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index)]
         self.add_output_variable(shape, dims)
         self.set_attr('pool_op', self.get_attr('class_name').split('Pooling')[0])
+        self.set_attr('implementation', self.model.config.get_conv_implementation(self).lower())
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
 
         return [self._function_template.format(**params)]
 
@@ -1117,27 +1204,32 @@
             params['out_height'] = self.get_output_variable().dim_names[1]
             params['out_width'] = self.get_output_variable().dim_names[2]
 
         return self._config_template.format(**params)
 
 class GlobalPooling1D(Layer):
     def initialize(self):
-        shape = [self.attributes['n_out'], self.attributes['n_filt']]
-        dims = ['N_OUTPUTS_{}'.format(self.index), 'N_FILT_{}'.format(self.index)]
+        shape = [self.attributes['n_filt']]
+        dims = ['N_FILT_{}'.format(self.index)]
         self.add_output_variable(shape, dims)
         self.set_attr('pool_op', self.get_attr('class_name').split('Pooling')[0].replace('Global', ''))
 
     def function_cpp(self):
         params = self._default_function_params()
-
+        params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
         return [self._function_template.format(**params)]
 
     def config_cpp(self):
         params = self._default_config_params()
-        params['n_in'] = self.get_input_variable().size_cpp()
+        if self.get_attr('data_format') == 'channels_last':
+            params['n_in'] = self.get_input_variable().dim_names[0]
+            params['n_filt'] = self.get_input_variable().dim_names[1]
+        else:
+            params['n_in'] = self.get_input_variable().dim_names[1]
+            params['n_filt'] = self.get_input_variable().dim_names[0]
 
         return self._config_template.format(**params)
 
 class GlobalPooling2D(Layer):
     def initialize(self):
         shape = [self.attributes['n_filt']]
         dims = ['N_FILT_{}'.format(self.index)]
@@ -1158,21 +1250,22 @@
             params['in_height'] = self.get_input_variable().dim_names[1]
             params['in_width'] = self.get_input_variable().dim_names[2]
 
         return self._config_template.format(**params)
 
 class ZeroPadding1D(Layer):
     def initialize(self):
+        inp = self.get_input_variable()
         if self.get_attr('data_format') == 'channels_last':
             shape = [self.attributes['out_width'], self.attributes['n_chan']]
             dims = ['OUT_WIDTH_{}'.format(self.index), 'N_CHAN_{}'.format(self.index)]
         else:
             shape = [self.attributes['n_chan'], self.attributes['out_width']]
             dims = ['N_CHAN_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index)]
-        self.add_output_variable(shape, dims)
+        self.add_output_variable(shape, dims, precision=inp.type.precision)
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
         return [self._function_template.format(**params)]
 
     def config_cpp(self):
@@ -1186,21 +1279,22 @@
             params['in_width'] = self.get_input_variable().dim_names[1]
             params['out_width'] = self.get_output_variable().dim_names[1]
 
         return self._config_template.format(**params)
 
 class ZeroPadding2D(Layer):
     def initialize(self):
+        inp = self.get_input_variable()
         if self.get_attr('data_format') == 'channels_last':
             shape = [self.attributes['out_height'], self.attributes['out_width'], self.attributes['n_chan']]
             dims = ['OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index), 'N_CHAN_{}'.format(self.index)]
         else:
             shape = [self.attributes['n_chan'], self.attributes['out_height'], self.attributes['out_width']]
             dims = ['N_CHAN_{}'.format(self.index), 'OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index)]
-        self.add_output_variable(shape, dims)
+        self.add_output_variable(shape, dims, precision=inp.type.precision)
 
     def function_cpp(self):
         params = self._default_function_params()
         params['data_format'] = 'cf' if self.get_attr('data_format') == 'channels_first' else 'cl'
         return [self._function_template.format(**params)]
 
     def config_cpp(self):
@@ -1222,15 +1316,15 @@
 
 class Activation(Layer):
     def initialize(self):
         inp = self.get_input_variable()
         shape = inp.shape
         dims = inp.dim_names
         self.add_output_variable(shape, dims)
-        if self.model.config.backend.name == 'Vivado':
+        if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
             if 'table_t' not in self.attributes:
                 self.set_attr('table_t', FixedPrecisionType(width=18, integer=8))
             if 'table_size' not in self.attributes:
                 self.set_attr('table_size', 1024)
 
     def function_cpp(self):
         params = self._default_function_params()
@@ -1276,24 +1370,31 @@
         params['config'] = '{}_config{}'.format(self.get_attr('activation'), self.index)
 
         return [self._function_template.format(**params)]
 
 class Softmax(Activation):
     def initialize(self):
         super(Softmax, self).initialize()
-        if self.model.config.backend.name == 'Vivado':
+        if self.model.config.backend.name in ['Vivado', 'VivadoAccelerator']:
             if 'exp_table_t' not in self.attributes:
                 self.set_attr('exp_table_t', self.get_attr('table_t'))
             if 'inv_table_t' not in self.attributes:
                 self.set_attr('inv_table_t', self.get_attr('table_t'))
             if self.model.config.is_resource_strategy(self):
                 # 'resource' strategy = 'latency' for Softmax
                 self.set_attr('implementation', 'latency')
             else:
                 self.set_attr('implementation', self.model.config.get_strategy(self).lower())
+            
+            if self.model.config.get_config_value('IOType') == 'io_parallel':
+                assert len(self.get_input_variable().shape) == 1, 'Softmax with io_parallel strategy cannot be used on multidimensional tensors.'
+
+class TernaryTanh(Activation):
+    def initialize(self):
+        super(TernaryTanh, self).initialize()
 
 class BatchNormalization(Layer):
     def initialize(self):
         inp = self.get_input_variable()
         shape = inp.shape
         dims = inp.dim_names
         self.add_output_variable(shape, dims)
@@ -1324,17 +1425,20 @@
         return self._config_template.format(**params)
 
 class Merge(Layer):
     def initialize(self):
         assert(len(self.inputs) == 2)
         inp1 = self.get_input_variable(self.inputs[0])
         inp2 = self.get_input_variable(self.inputs[1])
-        shape = inp1.shape
-        assert(inp1.shape == inp2.shape)
-        dims = inp1.dim_names
+        if np.prod(inp2.shape) > np.prod(inp1.shape):
+            shape = inp2.shape
+            dims = inp2.dim_names
+        else:
+            shape = inp1.shape
+            dims = inp1.dim_names
         self.add_output_variable(shape, dims)
 
     def function_cpp(self):
         params = {}
         params['merge'] = self.get_attr('op').lower()
         params['config'] = 'config{}'.format(self.index)
         params['input1_t'] = self.get_input_variable(self.inputs[0]).type.name
@@ -1344,15 +1448,20 @@
         params['input2'] = self.get_input_variable(self.inputs[1]).name
         params['output'] = self.get_output_variable().name
 
         return [self._function_template.format(**params)]
 
     def config_cpp(self):
         params = self._default_config_params()
-        params['n_elem'] = self.get_input_variable(self.inputs[0]).size_cpp()
+        inp1 = self.get_input_variable(self.inputs[0])
+        inp2 = self.get_input_variable(self.inputs[1])
+        if np.prod(inp2.shape) > np.prod(inp1.shape):
+            params['n_elem'] = inp2.size_cpp()
+        else:
+            params['n_elem'] = inp1.size_cpp()
 
         return self._config_template.format(**params)
 
 class Dot(Merge):
     def initialize(self):
         assert(len(self.inputs) == 2)
         inp1 = self.get_input_variable(self.inputs[0])
@@ -1360,25 +1469,29 @@
         assert(inp1.shape == inp2.shape)
         if len(inp1.shape) > 1:
             raise Exception('ERROR: Dot of tensors with rank > 1 is not yet supported.')
 
         self.add_output_variable(shape=[1], dim_names=['OUT_DOT_{}'.format(self.index)])
 
     def config_cpp(self):
+        inp1 = self.get_input_variable(self.inputs[0])
+        inp2 = self.get_input_variable(self.inputs[1])
         params = self._default_config_params()
         params['n_out'] = 1
-        params['n_in'] = self.get_input_variable(self.inputs[0]).shape[0]
+        params['n_in'] = inp1.shape[0]
+        params['product_type'] = self.model.config.backend.product_type(inp1.type.precision, inp2.type.precision)
         return self._config_template.format(**params)
 
 class Concatenate(Merge):
     def initialize(self):
         assert(len(self.inputs) == 2)
         inp1 = self.get_input_variable(self.inputs[0])
         inp2 = self.get_input_variable(self.inputs[1])
         axis = self.attributes['axis']
+        if axis > 0: axis -= 1
         shape = inp1.shape[:]
         shape[axis] += inp2.shape[axis]
         rank = len(shape)
         if rank > 1:
             dims = ['OUT_CONCAT_{}_{}'.format(i, self.index) for i in range(rank)]
         else:
             dims = ['OUT_CONCAT_{}'.format(self.index)]
@@ -1409,17 +1522,18 @@
         raise Exception('Layer {} should not be exported to HLS'.format(self.__class__.__name__))
 
     def config_cpp(self):
         raise Exception('Layer {} should not be exported to HLS'.format(self.__class__.__name__))
 
 class Resize(Layer):
     def initialize(self):
+        inp = self.get_input_variable()
         shape = [self.get_attr('out_height'), self.get_attr('out_width'), self.get_attr('n_chan')]
         dims = ['OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index), 'N_CHAN_{}'.format(self.index)]
-        self.add_output_variable(shape, dims)
+        self.add_output_variable(shape, dims, precision=inp.type.precision)
 
     def function_cpp(self):
         params = self._default_function_params()
         params['algorithm'] = self.get_attr('algorithm')
 
         return [self._function_template.format(**params)]
 
@@ -1429,29 +1543,42 @@
         return self._config_template.format(**params)
 
 class Transpose(Layer):
     def initialize(self):
         inp = self.get_input_variable(self.inputs[0])
         perm = self.get_attr('perm')
         self.set_attr('dim', '{}d'.format(len(inp.shape)))
-        if len(perm) == 4 and perm[0] == 0:
-            perm = [i - 1 for i in perm[1:]]
-        shape = [inp.shape[i] for i in perm]
+
+        if len(perm) > 3:
+            raise Exception('ERROR: Transpose of tensors with rank > 3 is not yet supported.')
+        
+        #ONNX double transpose specific, sometimes ONNX injects
+        #useless double transpose layers when converting 
+        #from other frameworks
+        if len(perm) == 1:
+            shape = inp.shape #dummy shape
+            dims = ['DUMMY'] #dummy dims
+            self.set_attr('perm', [0])
+        else:
+            shape = [inp.shape[i] for i in perm]
+
         self.set_attr('perm_str', ','.join([str(i) for i in perm]))
+        
         if len(shape) == 2:
+            self.set_attr('perm_str', ','.join(['0'] + [str(i+1) for i in perm]))
             dims = ['OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index)]
             self.set_attr('depth', 1)
-            self.set_attr('height', shape[0])
-            self.set_attr('width', shape[1])
-        else:
+            self.set_attr('height', inp.shape[0])
+            self.set_attr('width', inp.shape[1])
+        elif len(shape) > 2:
             dims = ['OUT_DEPTH_{}'.format(self.index), 'OUT_HEIGHT_{}'.format(self.index), 'OUT_WIDTH_{}'.format(self.index)]
-            self.set_attr('depth', shape[0])
-            self.set_attr('height', shape[1])
-            self.set_attr('width', shape[2])
-        self.add_output_variable(shape, dims)
+            self.set_attr('depth', inp.shape[0])
+            self.set_attr('height', inp.shape[1])
+            self.set_attr('width', inp.shape[2])
+        self.add_output_variable(shape, dims, precision=inp.type.precision)
 
     def function_cpp(self):
         params = self._default_function_params()
         params['dim'] = self.get_attr('dim')
 
         return [self._function_template.format(**params)]
 
@@ -1728,24 +1855,26 @@
     'Activation'             : Activation,
     'QActivation'            : Activation,
     'LeakyReLU'              : ParametrizedActivation,
     'ThresholdedReLU'        : ParametrizedActivation,
     'ELU'                    : ParametrizedActivation,
     'PReLU'                  : PReLU,
     'Softmax'                : Softmax,
+    'TernaryTanh'            : TernaryTanh,
     'Reshape'                : Reshape,
     'Dense'                  : Dense,
     'BinaryDense'            : Dense,
     'TernaryDense'           : Dense,
     'QDense'                 : Dense,
     'Conv1D'                 : Conv1D,
     'QConv1D'                : Conv1D,
     'Conv2D'                 : Conv2D,
     'BinaryConv2D'           : Conv2D,
     'QConv2D'                : Conv2D,
+    'QConv2DBatchnorm'       : Conv2DBatchnorm,
     'SeparableConv1D'        : SeparableConv1D,
     'SeparableConv2D'        : SeparableConv2D,
     'DepthwiseConv2D'        : DepthwiseConv2D,
     'BatchNormalization'     : BatchNormalization,
     'QBatchNormalization'    : BatchNormalization,
     'MaxPooling1D'           : Pooling1D,
     'AveragePooling1D'       : Pooling1D,
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/hls_model.py` & `hls4ml-0.6.0/hls4ml/model/hls_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,30 +14,37 @@
 from hls4ml.writer import get_writer
 from hls4ml.model.optimizer import optimize_model, get_available_passes
 from hls4ml.report.vivado_report import parse_vivado_report
 
 class HLSConfig(object):
     def __init__(self, config):
         self.config = config
-
         self.backend = get_backend(self.config.get('Backend', 'Vivado'))
         self.writer = get_writer(self.config.get('Backend', 'Vivado'))
 
         self.model_precision = {}
         self.layer_type_precision = {}
         self.layer_name_precision = {}
 
         self.model_rf = None
         self.layer_type_rf = {}
         self.layer_name_rf = {}
 
+        self.model_targ_cycles = None
+        self.layer_type_targ_cycles = {}
+        self.layer_name_targ_cycles = {}
+
         self.model_strategy = 'Latency'
         self.layer_type_strategy = {}
         self.layer_name_strategy = {}
 
+        self.model_conv_implementation = 'LineBuffer'
+        self.layer_type_conv_implementation = {}
+        self.layer_name_conv_implementation = {}
+
         self.model_compression = False
         self.layer_type_compression = {}
         self.layer_name_compression = {}
 
         self.trace_output = self.get_config_value('TraceOutput', False)
 
         self._parse_hls_config()
@@ -107,34 +114,56 @@
         if precision is None:
             raise Exception('No precision for {}->{} found and no default specified.'.format(layer.name, var))
 
         precision = self.backend.convert_precision_string(precision)
 
         return (precision, type_name)
 
+    def get_bram_size(self, layer):
+        bf = self.model_bf
+        return bf
+
     def get_reuse_factor(self, layer):
         rf = self.layer_name_rf.get(layer.name.lower())
         if rf is None:
             rf = self.layer_type_rf.get(layer.__class__.__name__.lower())
         if rf is None:
             rf = self.model_rf
 
         if rf is None:
             raise Exception('No reuse factor for {} found and no default specified.'.format(layer.name))
 
         return rf
 
+    def get_target_cycles(self, layer):
+        targ_cycles = self.layer_name_targ_cycles.get(layer.name.lower())
+        if targ_cycles is None:
+            targ_cycles = self.layer_name_targ_cycles.get(layer.__class__.__name__.lower())
+        if targ_cycles is None:
+            targ_cycles = self.model_targ_cycles
+ 
+        return targ_cycles
+
     def get_strategy(self, layer):
         strategy = self.layer_name_strategy.get(layer.name.lower())
         if strategy is None:
             strategy = self.layer_type_strategy.get(layer.__class__.__name__.lower())
         if strategy is None:
             strategy = self.model_strategy
 
         return strategy
+    
+    def get_conv_implementation(self, layer):
+        conv_implementation = self.layer_name_conv_implementation.get(layer.name.lower())
+        if conv_implementation is None:
+            conv_implementation = self.layer_type_conv_implementation.get(layer.__class__.__name__.lower())
+        if conv_implementation is None:
+            conv_implementation = self.model_conv_implementation
+
+        return conv_implementation
 
     def is_resource_strategy(self, layer):
         return self.get_strategy(layer).lower() == 'resource'
 
     def get_compression(self, layer):
         compression = self.layer_name_compression.get(layer.name.lower())
         if compression is None:
@@ -166,15 +195,18 @@
             if precision_cfg is not None:
                 if isinstance(precision_cfg, dict):
                     for var, precision in precision_cfg.items():
                         self.model_precision[var] = precision
                 else:
                     self.model_precision['default'] = precision_cfg # Default precision for everything
 
+            self.model_bf = model_cfg.get('BramFactor', np.inf) # Weight threshold to be external BRAM
             self.model_rf = model_cfg.get('ReuseFactor')
+            self.model_targ_cycles = model_cfg.get('TargetCycles')
+            self.model_conv_implementation = model_cfg.get('ConvImplementation', 'LineBuffer')
             self.model_strategy = model_cfg.get('Strategy', 'Latency')
             self.model_compression = bool(model_cfg.get('Compression', 0))
 
         layer_type_cfg = hls_config.get('LayerType')
         if layer_type_cfg is not None:
             for layer_type, layer_cfg in layer_type_cfg.items():
                 precision_cfg = layer_cfg.get('Precision')
@@ -183,19 +215,27 @@
                         self.layer_type_precision[layer_type.lower() + '_' + var] = precision
                 else:
                     self.layer_type_precision[layer_type.lower() + '_default'] = precision_cfg
 
                 rf = layer_cfg.get('ReuseFactor')
                 if rf is not None:
                     self.layer_type_rf[layer_type.lower()] = rf
+                
+                targ_cycles = layer_cfg.get('TargetCycles')
+                if targ_cycles is not None:
+                    self.layer_type_targ_cycles[layer_type.lower()] = targ_cycles
 
                 strategy = layer_cfg.get('Strategy')
                 if strategy is not None:
                     self.layer_type_strategy[layer_type.lower()] = strategy
 
+                conv_implementation = layer_cfg.get('ConvImplementation')
+                if conv_implementation is not None:
+                    self.layer_type_conv_implementation[layer_type.lower()] = conv_implementation
+
                 compression = layer_cfg.get('Compression')
                 if compression is not None:
                     self.layer_type_compression[layer_type.lower()] = bool(compression)
 
         layer_name_cfg = hls_config.get('LayerName')
         if layer_name_cfg is not None:
             for layer_name, layer_cfg in layer_name_cfg.items():
@@ -206,18 +246,26 @@
                 else:
                     self.layer_name_precision[layer_name.lower() + '_default'] = precision_cfg
 
                 rf = layer_cfg.get('ReuseFactor')
                 if rf is not None:
                     self.layer_name_rf[layer_name.lower()] = rf
 
+                targ_cycles = layer_cfg.get('TargetCycles')
+                if targ_cycles is not None:
+                    self.layer_name_targ_cycles[layer_name.lower()] = targ_cycles
+
                 strategy = layer_cfg.get('Strategy')
                 if strategy is not None:
                     self.layer_name_strategy[layer_name.lower()] = strategy
 
+                conv_implementation = layer_cfg.get('ConvImplementation')
+                if conv_implementation is not None:
+                    self.layer_name_conv_implementation[layer_name.lower()] = conv_implementation
+
                 compression = layer_cfg.get('Compression')
                 if compression is not None:
                     self.layer_name_compression[layer_name.lower()] = bool(compression)
 
     def _validate_hls_config(self):
         use_resource = False
         if self.model_strategy.lower() == 'latency' and self.model_compression:
@@ -256,96 +304,180 @@
         self.inputs = inputs if inputs is not None else [layer_list[0]['name']]
         self.outputs = outputs if outputs is not None else [layer_list[-1]['name']]
 
         self.index = 0
         self.graph = OrderedDict()
         self.output_vars = {}
 
+        # External BRAM 
+        self.bram_vars = {}
+
         self._top_function_lib = None
 
         self._make_graph(layer_list)
 
         self._optimize_model(self.config.optimizers)
 
     def _make_graph(self, layer_list):
         for layer in layer_list:
             kind = layer['class_name']
             name = layer['name']
             inputs = layer.get('inputs', [])
             outputs = layer.get('outputs', [])
-            if len(inputs) == 0:
+            if kind in ['InputLayer', 'Input']:
+                inputs = ['input']
+            elif len(inputs) == 0:
                 inputs = [next(reversed(self.graph), 'input')]
             if len(outputs) == 0:
                 outputs = [name]
 
             self.graph[name] = self.make_node(kind, name, layer, inputs, outputs)
 
     def _optimize_model(self, optimizers):
         optimize_model(self, optimizers)
 
     def make_node(self, kind, name, attributes, inputs, outputs=None):
+        """ Make a new node not connected to the model graph.
+
+        The 'kind' should be a valid layer registered with `register_layer`. If no outputs
+        are specified, a default output named the same as the node will be created. The 
+        returned node should be added to the graph with `insert_node` or `replace_node`
+        functions.
+
+        Args:
+            kind (str): Type of node to add
+            name (str): Name of the node
+            attributes (dict): Initial set of attributes required to construct the node (Layer)
+            inputs (list): List of inputs to the layer
+            outputs (list, optional): The optional list of named outputs of the node
+
+        Raises:
+            Exception: If an attempt to insert a node with multiple inputs is made or if
+                `before` does not specify a correct node in sequence.
+
+        Returns:
+            Layer: The node created.
+        """
+
+        if kind not in layer_map:
+            raise Exception('Layer {} not found in registry.'.format(kind))
+
         node = layer_map[kind](self, name, attributes, inputs, outputs)
         for o in node.outputs:
             out_var = node.get_output_variable(output_name=o)
             if o in self.outputs:
                 out_var.type.name = 'result_t'
             self.output_vars[o] = out_var
-
         return node
 
-    def insert_node(self, node):
+    def insert_node(self, node, before=None):
+        """ Insert a new node into the model graph.
+
+        The node to be inserted should be created with `make_node()` function. The optional 
+        parameter `before` can be used to specify the node that follows in case of ambiguities.
+
+        Args:
+            node (Layer): Node to insert
+            before (Layer, optional): The next node in sequence before which a
+                new node should be inserted. 
+        Raises:
+            Exception: If an attempt to insert a node with multiple inputs is made or if
+                `before` does not specify a correct node in sequence.
+
+        """
         if len(node.inputs) > 1:
             raise Exception('Cannot insert a node with more than one input (for now).')
 
-        prev_node = self.graph.get(node.inputs[0])
-        next_node = next((x for x in self.graph.values() if x.inputs[0] == prev_node.outputs[0]), None)
+        prev_node = node.get_input_node(node.inputs[0])
+        next_nodes = [x for x in self.graph.values() if x.inputs[0] in prev_node.outputs]
+        if before is None:
+            next_node = next((x for x in self.graph.values() if x.inputs[0] in prev_node.outputs), None)
+        else:
+            if before not in next_nodes:
+                raise Exception('Cannot insert a node {} before {} (candidates: {}).'.format(node.name, before.name, ','.join([n.name for n in next_nodes])))
+            next_node = before
+
         if next_node is not None:
             next_node.inputs[0] = node.outputs[0]
 
         new_graph = OrderedDict()
         for k, v in self.graph.items():
             new_graph[k] = v
             if k == prev_node.name:
                 new_graph[node.name] = node
 
         self.graph = new_graph
+        self._update_model_outputs()
 
     def remove_node(self, node, rewire=True):
+        """ Remove a node from a graph.
+
+        By default, this function can connect the outputs of previous node to the input of next one.
+        Note that when removing a leaf node `rewire` should be set to `False`.
+
+        Args:
+            node (Layer): The node to remove
+            rewire (bool, optional): If `True`, connects the outputs of the previous node
+                to the inputs of the next node
+
+        Raises:
+            Exception: If an attempt is made to rewire a leaf node or a node with multiple
+                inputs/outpus.
+
+        """
         if rewire:
             if len(node.inputs) > 1 or len(node.outputs) > 1:
                 raise Exception('Cannot rewire a node with multiple inputs/outputs')
             prev_node = self.graph.get(node.inputs[0])
             next_node = next((x for x in self.graph.values() if node.outputs[0] in x.inputs), None)
             if prev_node is not None:
                 if next_node is not None:
                     for i,_ in enumerate(next_node.inputs):
                         if node.outputs[0] == next_node.inputs[i]:
                             next_node.inputs[i] = prev_node.outputs[0]
                             break
                 else:
-                    if node.outputs[0] in self.outputs:
-                        self.outputs = [prev_node.outputs[0] if x == node.outputs[0] else x for x in self.outputs]
-                    else:
+                    if not node.outputs[0] in self.outputs:
                         raise Exception('Cannot rewire a node without child')
             else:
                 raise Exception('Cannot rewire a node without a parent')
-
+        
         del self.output_vars[node.outputs[0]]
         del self.graph[node.name]
+        self._update_model_outputs()
 
     def replace_node(self, old_node, new_node):
+        """ Replace an existing node in the graph with a new one.
+
+        Args:
+            old_node (Layer): The node to replace
+            new_node (Layer): The new node
+
+        """
         prev_node = self.graph.get(old_node.inputs[0])
         next_node = next((x for x in self.graph.values() if x.inputs[0] == old_node.outputs[0]), None)
         if next_node is not None:
             next_node.inputs[0] = new_node.outputs[0]
         if prev_node is not None:
             if new_node.inputs is None or len(new_node.inputs) == 0: # Check if already rewired
                 new_node.inputs = [prev_node.outputs[0]]
 
         self.graph = OrderedDict((new_node.name, new_node) if k == old_node.name else (k, v) for k, v in self.graph.items())
+        self._update_model_outputs()
+
+    def _update_model_outputs(self):
+        ''' Update the model outputs
+
+        All node outputs and inputs are found. The model outputs are set to all node outputs
+        that are not also node inputs.
+        '''
+        node_outputs = np.array([out for node in self.graph.values() for out in node.outputs])
+        node_inputs = np.array([inp for node in self.graph.values() for inp in node.inputs])
+        model_outputs = node_outputs[np.isin(node_outputs, node_inputs, invert=True)]
+        self.outputs = model_outputs.tolist()
 
     def get_weights_data(self, layer_name, var_name):
         return self.reader.get_weights_data(layer_name, var_name)
 
     def next_layer(self):
         self.index += 1
         return self.index
@@ -355,27 +487,33 @@
 
     def get_input_variables(self):
         variables = []
         for inp in self.inputs:
             variables.append(self.graph[inp].get_output_variable())
         return variables
 
+    def register_bram_variable(self, out_name, variable):
+        self.bram_vars[out_name] = variable
+
+    def get_bram_variables(self):
+        return self.bram_vars.values()
+
     def register_output_variable(self, out_name, variable):
         if out_name in self.outputs:
             variable.type.name = 'result_t'
         self.output_vars[out_name] = variable
 
     def get_output_variables(self):
         variables = []
         for out in self.outputs:
             variables.append(self.output_vars[out])
         return variables
 
     def get_layer_output_variable(self, output_name):
-        return self.output_vars[output_name]
+        return self.output_vars.get(output_name, None)
 
     def write(self):
         def make_stamp():
             from string import hexdigits
             from random import choice
             length = 8
             return ''.join(choice(hexdigits) for m in range(length))
@@ -408,63 +546,88 @@
             self._top_function_lib = ctypes.cdll.LoadLibrary(lib_name)
         finally:
             os.chdir(curr_dir)
 
     def _get_top_function(self, x):
         if self._top_function_lib is None:
             raise Exception('Model not compiled')
-        if len(self.get_input_variables()) > 1 or len(self.get_input_variables()) > 1:
-            raise Exception('Calling "predict" on models with multiple inputs or outputs is not supported (yet)')
-
-        if not isinstance(x, np.ndarray):
-            raise Exception('Expected numpy.ndarray, but got {}'.format(type(x)))
-        if not x.flags['C_CONTIGUOUS']:
-            raise Exception('Array must be c_contiguous, try using numpy.ascontiguousarray(x)')
+        if len(self.get_input_variables()) == 1:
+            xlist = [x]
+        else: 
+            xlist = x
+        
+        for xi in xlist:
+            if not isinstance(xi, np.ndarray):
+                raise Exception('Expected numpy.ndarray, but got {}'.format(type(x)))
+            if not xi.flags['C_CONTIGUOUS']:
+                raise Exception('Array must be c_contiguous, try using numpy.ascontiguousarray(x)')
 
-        if x.dtype in [np.single, np.float32]:
+        x0 = xlist[0]
+        if x0.dtype in [np.single, np.float32]:
             top_function = getattr(self._top_function_lib, self.config.get_project_name() + '_float')
             ctype = ctypes.c_float
-        elif x.dtype in [np.double, np.float64, np.float_]:
+        elif x0.dtype in [np.double, np.float64, np.float_]:
             top_function = getattr(self._top_function_lib, self.config.get_project_name() + '_double')
             ctype = ctypes.c_double
         else:
-            raise Exception('Invalid type ({}) of numpy array. Supported types are: single, float32, double, float64, float_.'.format(x.dtype))
+            raise Exception('Invalid type ({}) of numpy array. Supported types are: single, float32, double, float64, float_.'.format(x0.dtype))
+
 
         top_function.restype = None
-        top_function.argtypes = [npc.ndpointer(ctype, flags="C_CONTIGUOUS"), npc.ndpointer(ctype, flags="C_CONTIGUOUS"),
-            ctypes.POINTER(ctypes.c_ushort), ctypes.POINTER(ctypes.c_ushort)]
+        top_function.argtypes = [npc.ndpointer(ctype, flags="C_CONTIGUOUS") for i in range(len(xlist)+1)]
+        top_function.argtypes += [ctypes.POINTER(ctypes.c_ushort) for i in range(len(xlist)+1)]
 
         return top_function, ctype
 
     def _compute_n_samples(self, x):
-        expected_size = self.get_input_variables()[0].size()
-        x_size = np.prod(x.shape)
-        n_samples, rem = divmod(x_size, expected_size)
-        if rem != 0:
-            raise Exception('Input size mismatch, got {}, expected {}'.format(x_size.shape, self.get_input_variables()[0].shape))
+        if len(self.get_input_variables()) == 1:
+            xlist = [x]
+        else:
+            xlist = x
+        n_samples = []
+        for i, xi in enumerate(xlist):
+            expected_size = self.get_input_variables()[i].size()
+            x_size = np.prod(xi.shape)
+            n_sample, rem = divmod(x_size, expected_size)
+            if rem != 0:
+                raise Exception('Input size mismatch, got {}, expected {}'.format(x_size.shape, self.get_input_variables()[i].shape))
+            n_samples.append(n_sample)
+
+        if not all([n_samples[i] == n_samples[i+1] for i in range(len(xlist)-1)]):
+            raise Exception('Input size mismatch, not all inputs match')
 
-        return n_samples
+        return n_sample
 
     def predict(self, x):
         top_function, ctype = self._get_top_function(x)
         n_samples = self._compute_n_samples(x)
+        n_inputs = len(self.get_input_variables())
 
         curr_dir = os.getcwd()
         os.chdir(self.config.get_output_dir() + '/firmware')
 
         output = []
-        if n_samples == 1:
+        if n_samples == 1 and n_inputs == 1:
             x = [x]
 
         try:
             for i in range(n_samples):
                 predictions = np.zeros(self.get_output_variables()[0].size(), dtype=ctype)
-                top_function(x[i], predictions, ctypes.byref(ctypes.c_ushort()), ctypes.byref(ctypes.c_ushort()))
+                if n_inputs == 1:
+                    top_function(x[i], predictions, ctypes.byref(ctypes.c_ushort()), ctypes.byref(ctypes.c_ushort()))
+                else:
+                    inp = [xj[i] for xj in x]
+                    argtuple = inp
+                    argtuple += [predictions]
+                    argtuple += [ctypes.byref(ctypes.c_ushort()) for k in range(len(inp)+1)]
+                    argtuple = tuple(argtuple)
+                    top_function(*argtuple)
                 output.append(predictions)
 
+
             #Convert to numpy array
             output = np.asarray(output)
         finally:
             os.chdir(curr_dir)
 
         if n_samples == 1:
             return output[0]
@@ -474,14 +637,15 @@
     def trace(self, x):
         print('Recompiling {} with tracing'.format(self.config.get_project_name()))
         self.config.trace_output = True
         self.compile()
 
         top_function, ctype = self._get_top_function(x)
         n_samples = self._compute_n_samples(x)
+        n_inputs = len(self.get_input_variables())
 
         class TraceData(ctypes.Structure):
             _fields_ = [('name', ctypes.c_char_p),
                         ('data', ctypes.c_void_p)]
 
         trace_output = {}
         layer_sizes = {}
@@ -505,23 +669,31 @@
         free_func.argtypes = None
         free_func.restype = None
 
         curr_dir = os.getcwd()
         os.chdir(self.config.get_output_dir() + '/firmware')
 
         output = []
-        if n_samples == 1:
+        if n_samples == 1 and n_inputs == 1:
             x = [x]
 
         try:
             alloc_func(ctypes.sizeof(ctype))
 
             for i in range(n_samples):
                 predictions = np.zeros(self.get_output_variables()[0].size(), dtype=ctype)
-                top_function(x[i], predictions, ctypes.byref(ctypes.c_ushort()), ctypes.byref(ctypes.c_ushort()))
+                if n_inputs == 1:
+                    top_function(x[i], predictions, ctypes.byref(ctypes.c_ushort()), ctypes.byref(ctypes.c_ushort()))
+                else:
+                    inp = [xj[i] for xj in x]
+                    argtuple = inp
+                    argtuple += [predictions]
+                    argtuple += [ctypes.byref(ctypes.c_ushort()) for k in range(len(inp)+1)]
+                    argtuple = tuple(argtuple)
+                    top_function(*argtuple)
                 output.append(predictions)
                 collect_func(trace_data)
                 for trace in trace_data:
                     layer_name = str(trace.name, 'utf-8')
                     layer_data = ctypes.cast(trace.data, ctypes.POINTER(ctype))
                     np_array = np.ctypeslib.as_array(layer_data, shape=layer_sizes[layer_name])
                     trace_output[layer_name].append(np.copy(np_array))
@@ -540,15 +712,15 @@
             return output[0], trace_output
         else:
             return output, trace_output
 
     def build(self, reset=False, csim=True, synth=True, cosim=False, validation=False, export=False, vsynth=False):
         if 'linux' in sys.platform:
             backend = self.config.get_config_value('Backend', 'Vivado')
-            if backend == 'Vivado':
+            if backend in ['Vivado', 'VivadoAccelerator']:
                 found = os.system('command -v vivado_hls > /dev/null')
                 if found != 0:
                     raise Exception('Vivado HLS installation not found. Make sure "vivado_hls" is on PATH.')
 
             elif backend == 'Intel':
                 raise NotImplementedError
             elif backend == 'Mentor':
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/__init__.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 from __future__ import absolute_import
 
 from hls4ml.model.optimizer.optimizer import OptimizerPass, register_pass, get_optimizer, optimize_model, get_available_passes
 
 
 from hls4ml.model.optimizer.passes.nop import EliminateLinearActivation
-from hls4ml.model.optimizer.passes.bn_quant import MergeBatchNormAndQuantizedTanh, QuantizeDenseOutput
+from hls4ml.model.optimizer.passes.bn_quant import MergeBatchNormAndQuantizedTanh
+from hls4ml.model.optimizer.passes.bn_quant import QuantizeDenseOutput
 from hls4ml.model.optimizer.passes.bn_fuse import FuseBatchNormalization
 from hls4ml.model.optimizer.passes.fuse_biasadd import FuseBiasAdd
 from hls4ml.model.optimizer.passes.conv_same_pad import InsertZeroPaddingBeforeConv1D
 from hls4ml.model.optimizer.passes.conv_same_pad import InsertZeroPaddingBeforeConv2D
 from hls4ml.model.optimizer.passes.pointwise import OptimizePointwiseConv
 from hls4ml.model.optimizer.passes.clone import CloneOutput
-from hls4ml.model.optimizer.passes.repack_stream import ReshapeStream
+from hls4ml.model.optimizer.passes.repack_stream import ReshapeStream, BroadcastStream, RemoveFinalReshape
+from hls4ml.model.optimizer.passes.transpose_opt import RemoveUselessTranspose
+from hls4ml.model.optimizer.passes.multi_dense import ReplaceMultidimensionalDenseWithConv
 
 try:
     from hls4ml.model.optimizer.passes.qkeras import OutputRoundingSaturationMode
     from hls4ml.model.optimizer.passes.qkeras import QKerasFactorizeAlpha
     from hls4ml.model.optimizer.passes.qkeras import FuseConsecutiveBatchNormalization
+    from hls4ml.model.optimizer.passes.qkeras import ExtractTernaryThreshold
     __qkeras_optimizers__ = True
 except ImportError:
     __qkeras_optimizers__ = False
 
+if __qkeras_optimizers__:
+    register_pass('output_rounding_saturation_mode', OutputRoundingSaturationMode)
+    register_pass('qkeras_factorize_alpha', QKerasFactorizeAlpha)
+    register_pass('extract_ternary_threshold', ExtractTernaryThreshold)
+    register_pass('fuse_consecutive_batch_normalization', FuseConsecutiveBatchNormalization) 
+
 register_pass('eliminate_linear_activation', EliminateLinearActivation)
 register_pass('merge_batch_norm_quantized_tanh', MergeBatchNormAndQuantizedTanh)
 register_pass('quantize_dense_output', QuantizeDenseOutput)
 register_pass('fuse_batch_norm', FuseBatchNormalization)
 register_pass('fuse_biasadd', FuseBiasAdd)
 register_pass('conv1d_same_pad', InsertZeroPaddingBeforeConv1D)
 register_pass('conv2d_same_pad', InsertZeroPaddingBeforeConv2D)
 register_pass('optimize_pointwise_conv', OptimizePointwiseConv)
 register_pass('clone_output', CloneOutput)
+register_pass('remove_final_reshape', RemoveFinalReshape)
 register_pass('reshape_stream', ReshapeStream)
-
-if __qkeras_optimizers__:
-    register_pass('output_rounding_saturation_mode', OutputRoundingSaturationMode)
-    register_pass('qkeras_factorize_alpha', QKerasFactorizeAlpha)
-    register_pass('fuse_consecutive_batch_normalization', FuseConsecutiveBatchNormalization) 
+register_pass('remove_useless_transpose', RemoveUselessTranspose)
+register_pass('replace_multidense_conv', ReplaceMultidimensionalDenseWithConv)
+register_pass('broadcast_stream', BroadcastStream)
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/optimizer.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/bn_fuse.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/passes/bn_fuse.py`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/bn_quant.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/passes/bn_quant.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,43 +12,20 @@
         sign of the input flips after the quantized (binary or ternary) Tanh activation.
     '''
 
     def initialize(self):
         inp = self.get_input_variable()
         shape = inp.shape
         dims = inp.dim_names
-        precision = self.model.config.backend.convert_precision_string(inp.type.precision)
-        W, I, F = precision.width, precision.integer, precision.fractional
-        original_name = self.attributes.get('original_name')
-        variance = self.model.get_weights_data(original_name, 'moving_variance')
-        mean = self.model.get_weights_data(original_name, 'moving_mean')
-        gamma = self.model.get_weights_data(original_name, 'gamma')
-        beta = self.model.get_weights_data(original_name, 'beta')
-        mean_quantizer = self.get_attr('mean_quantizer')
-        variance_quantizer = self.get_attr('variance_quantizer')
-        gamma_quantizer = self.get_attr('gamma_quantizer')
-        beta_quantizer = self.get_attr('beta_quantizer')
-        mean = mean_quantizer(mean) if mean_quantizer is not None else mean
-        variance = variance_quantizer(variance) if variance_quantizer is not None else variance
-        gamma = gamma_quantizer(gamma) if gamma_quantizer is not None else gamma
-        beta = beta_quantizer(beta) if beta_quantizer is not None else beta
-        epsilon = self.attributes.get('epsilon')
-        threshold = mean - beta * np.sqrt(variance + epsilon) / gamma
         if self.get_attr('quantize') == 2:
             self.add_output_variable(shape, dims, precision=XnorPrecisionType())
-            threshold = np.floor(threshold * 2**F) / 2**F
-            self.add_weights_variable(name='threshold', var_name='t{index}', data=threshold, type_name='threshold{index}_t', precision=inp.type.precision)
         elif self.get_attr('quantize') == 3:
             self.add_output_variable(shape, dims, precision=IntegerPrecisionType(width=2))
-            threshold_hi = 0.5/(gamma/np.sqrt(variance + epsilon)) + threshold
-            threshold_lo = -0.5/(gamma/np.sqrt(variance + epsilon)) + threshold
-            threshold_hi = np.floor(threshold_hi * 2**F) / 2**F
-            threshold_lo = np.floor(threshold_lo * 2**F) / 2**F
-            self.add_weights_variable(name='threshold_hi', var_name='th{index}', data=threshold_hi, type_name='threshold_hi_{index}_t', precision=inp.type.precision)
-            self.add_weights_variable(name='threshold_lo', var_name='tl{index}', data=threshold_lo, type_name='threshold_lo_{index}_t', precision=inp.type.precision)
+        else:
+            raise Exception('Unsupported quantize attribute for BatchNormalizationQuantizedTanh: {}'.format(self.get_attr('quantize')))
 
     def function_cpp(self):
         params = self._default_function_params()
         if self.get_attr('quantize') == 2:
             params['quantize'] = 'binary'
             params['threshold'] = self.get_weights('threshold').name
         elif self.get_attr('quantize') == 3:
@@ -59,71 +36,93 @@
 
     def config_cpp(self):
         params = self._default_config_params()
         params['n_in'] = self.get_input_variable().size_cpp()
 
         return self._config_template.format(**params)
 
+    def set_thresholds(self, scale, bias, ternary_threshold=0.5):
+        inp = self.get_input_variable()
+        shape = inp.shape
+        dims = inp.dim_names
+        precision = self.model.config.backend.convert_precision_string(inp.type.precision)
+        W, I, F = precision.width, precision.integer, precision.fractional
+        threshold = - bias / scale
+        if self.get_attr('quantize') == 2:
+            self.add_output_variable(shape, dims, precision=XnorPrecisionType())
+            threshold = np.floor(threshold * 2**F) / 2**F
+            self.add_weights_variable(name='threshold', var_name='t{index}', data=threshold, type_name='threshold{index}_t', precision=inp.type.precision)
+        elif self.get_attr('quantize') == 3:
+            self.add_output_variable(shape, dims, precision=IntegerPrecisionType(width=2))
+            threshold_hi = ternary_threshold / scale + threshold
+            threshold_lo = -ternary_threshold / scale + threshold
+            threshold_hi = np.floor(threshold_hi * 2**F) / 2**F
+            threshold_lo = np.floor(threshold_lo * 2**F) / 2**F
+            self.add_weights_variable(name='threshold_hi', var_name='th{index}', data=threshold_hi, type_name='threshold_hi_{index}_t', precision=inp.type.precision)
+            self.add_weights_variable(name='threshold_lo', var_name='tl{index}', data=threshold_lo, type_name='threshold_lo_{index}_t', precision=inp.type.precision)
+
 batchnorm_quantized_tanh_config_template = """struct config{index} : nnet::batchnorm_quantized_tanh_config {{
     static const unsigned n_in = {n_in};
     static const unsigned n_filt = {n_filt};
     static const unsigned io_type = nnet::{iotype};
     static const unsigned reuse_factor = {reuse};
 }};\n"""
 
 batchnorm_quantized_tanh_function_template = 'nnet::normalize_{quantize}_tanh<{input_t}, {config}>({input}, {output}, {threshold});'
 
 # Register the layer types to the layer map
 register_layer('BatchNormalizationQuantizedTanh', BatchNormalizationQuantizedTanh)
 
+from hls4ml.templates.vivado_template import batchnorm_include_list
+
 # Register the templates for config and function
-templates.get_backend('Vivado').register_templates('BatchNormalizationQuantizedTanh', batchnorm_quantized_tanh_function_template, batchnorm_quantized_tanh_config_template)
+for backend in ['Vivado', 'VivadoAccelerator']:
+    templates.get_backend(backend).register_templates('BatchNormalizationQuantizedTanh', batchnorm_quantized_tanh_function_template, batchnorm_quantized_tanh_config_template, batchnorm_include_list)
 
 class MergeBatchNormAndQuantizedTanh(OptimizerPass):
     def match(self, node):
         is_match = (node.__class__.__name__ == 'Activation'
-            and node.get_attr('activation') in ['binary_tanh', 'ternary_tanh']
-            and isinstance(node.get_input_node(), BatchNormalization))
+            and node.get_attr('activation') in ['binary', 'binary_tanh', 'ternary', 'ternary_tanh']
+            or node.__class__.__name__ == 'TernaryTanh')
+        is_match = is_match and isinstance(node.get_input_node(), BatchNormalization)
         return is_match
 
     def transform(self, model, node):
         bn_layer = node.get_input_node()
-        # Remove the Activation layer
-        model.remove_node(node, rewire=True)
         # Make a new layer with the new attributes
         quantize = 0
-        if node.get_attr('activation') == 'binary_tanh':
+        if 'binary' in node.get_attr('activation'):
             quantize = 2
-        if node.get_attr('activation') == 'ternary_tanh':
+        if 'ternary' in node.get_attr('activation'):
             quantize = 3
         attrs = {
             'name' : bn_layer.get_attr('name'),
             'original_name' : bn_layer.get_attr('name'),
             'class_name' : 'BatchNormalizationQuantizedTanh',
             'n_in' : bn_layer.get_attr('n_in'),
             'n_out' : bn_layer.get_attr('n_in'),
             'n_filt' : bn_layer.get_attr('n_filt'),
-            'epsilon' : bn_layer.get_attr('epsilon'),
             'quantize' : quantize,
-            'beta_quantizer' : bn_layer.get_attr('beta_quantizer'),
-            'gamma_quantizer' : bn_layer.get_attr('gamma_quantizer'),
-            'mean_quantizer' : bn_layer.get_attr('mean_quantizer'),
-            'variance_quantizer' : bn_layer.get_attr('variance_quantizer'),
             'Trace' : bn_layer.get_attr('Trace')
         }
         bnbt_layer = model.make_node('BatchNormalizationQuantizedTanh', 'bnbt_' + bn_layer.name, attrs, bn_layer.inputs)
-        # Replace the old BatchNormalization layer with this one
-        model.replace_node(bn_layer, bnbt_layer)
+        bnbt_layer.set_thresholds(bn_layer.get_weights('scale').data, bn_layer.get_weights('bias').data, node.get_attr('threshold',0.5))
+        # Remove the BatchNormalization layer
+        model.remove_node(bn_layer, rewire=True)
+        # Replace the old Activation layer with this one
+        model.replace_node(node, bnbt_layer)
 
         return True
 
 class QuantizeDenseOutput(OptimizerPass):
     def match(self, node):
-        is_match = (node.__class__.__name__ == 'Dense' and node.get_attr('weight_quantizer') is not None
-            and node.get_input_node().__class__.__name__ == 'BatchNormalizationQuantizedTanh')
+        is_match = node.__class__.__name__ == 'Dense'
+        is_match = is_match and node.get_input_node().__class__.__name__ == 'BatchNormalizationQuantizedTanh'
+        quantizer = node.get_attr('weight_quantizer')
+        is_match = is_match and (quantizer.__class__.__name__ == 'BinaryQuantizer' or quantizer.__class__.__name__ == 'TernaryQuantizer')
         return is_match
 
     def transform(self, model, node):
         # Compute the required precision and update the variables
         # Number of bits for output is log2 of number of input nodes
         # Since this is the number of uint<1>'s which are summed
         nbits = int(np.ceil(np.log2(node.attributes['n_in'])) + 2)
@@ -170,7 +169,8 @@
                     var_names.append('threshold_lo')
                 for var_name in var_names:
                     threshold_var = out_node.weights[var_name]
                     threshold_var.update_precision(out_type)
                     threshold_var.data = np.floor(threshold_var.data)
 
         return False
+
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/clone.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/passes/clone.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,28 +26,29 @@
 clone_function_template = 'nnet::clone_stream<{input_t}, {output_t}, {size}>({input}, {output1}, {output2});'
 clone_include_list = ['nnet_utils/nnet_stream.h']
 
 # Register the layer types to the layer map
 register_layer('Clone', Clone)
 
 # Register the templates for config and function
-templates.get_backend('Vivado').register_templates('Clone', clone_function_template, None, clone_include_list)
+for backend in ['Vivado', 'VivadoAccelerator']:
+    templates.get_backend(backend).register_templates('Clone', clone_function_template, None, clone_include_list)
 
 
 class CloneOutput(OptimizerPass):
     ''' Clones streams that are used multiple times '''
     def match(self, node):
         # We may have already inserted the Clone layer
         if node.__class__.__name__ == 'Clone':
             return False
 
         return True
 
     def transform(self, model, node):
-        if model.config.backend.name != 'Vivado' or \
+        if model.config.backend.name not in ['Vivado', 'VivadoAccelerator'] or \
             model.config.get_config_value('IOType') != 'io_stream':
             return False
 
         output_map = {}
         for output in node.outputs:
             output_map[output] = []
             for layer in model.get_layers():
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/conv_same_pad.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/passes/conv_same_pad.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     def match(self, node):
         is_match = 'Conv1D' in node.__class__.__name__ and \
             node.get_attr('padding') == 'same' and \
             node.get_attr('filt_width') != 1
         return is_match
 
     def transform(self, model, node):
-        if model.config.backend.name != 'Vivado' or \
+        if model.config.backend.name not in ['Vivado', 'VivadoAccelerator'] or \
             model.config.get_config_value('IOType') != 'io_stream':
             return False
         
         # Get the padding parameters from Conv1D layer
         pad_left = node.get_attr('pad_left')
         pad_right = node.get_attr('pad_right')
 
@@ -44,15 +44,15 @@
     def match(self, node):
         is_match = 'Conv2D' in node.__class__.__name__ and \
             node.get_attr('padding') == 'same' and \
             node.get_attr('filt_height') != 1 and node.get_attr('filt_width') != 1
         return is_match
 
     def transform(self, model, node):
-        if model.config.backend.name != 'Vivado' or \
+        if model.config.backend.name not in ['Vivado', 'VivadoAccelerator'] or \
             model.config.get_config_value('IOType') != 'io_stream':
             return False
         
         # Get the padding parameters from Conv2D layer
         pad_top = node.get_attr('pad_top')
         pad_bottom = node.get_attr('pad_bottom')
         pad_left = node.get_attr('pad_left')
@@ -82,10 +82,10 @@
         node.set_attr('pad_right', 0)
         node.set_attr('in_height', out_height)
         node.set_attr('in_width', out_width)
 
         # Insert new ZeroPadding2D node above Conv2D
         padding_layer = model.make_node('ZeroPadding2D', 'zp2d_' + node.name, attrs, node.inputs.copy())
         padding_layer.get_output_variable().type.precision = node.get_input_variable().type.precision
-        model.insert_node(padding_layer)
+        model.insert_node(padding_layer, before=node)
 
         return True
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/pointwise.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/passes/pointwise.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,33 +24,37 @@
 sepconv2d_include_list = ['nnet_utils/nnet_conv2d.h', 'nnet_utils/nnet_sepconv2d_stream.h']
 
 # Register the layer types to the layer map
 register_layer('PointwiseConv1D', PointwiseConv1D)
 register_layer('PointwiseConv2D', PointwiseConv2D)
 
 # Register the templates for config and function
-templates.get_backend('Vivado').register_templates(
-    'PointwiseConv1D',
-    pointwise_conv1d_function_template,
-    templates.get_backend('Vivado').get_config_template('Conv1D'),
-    sepconv1d_include_list
-)
+for backend in ['Vivado', 'VivadoAccelerator']:
+    templates.get_backend(backend).register_templates(
+        'PointwiseConv1D',
+        pointwise_conv1d_function_template,
+        templates.get_backend(backend).get_config_template('Conv1D'),
+        sepconv1d_include_list
+    )
 
-templates.get_backend('Vivado').register_templates(
-    'PointwiseConv2D',
-    pointwise_conv2d_function_template,
-    templates.get_backend('Vivado').get_config_template('Conv2D'),
-    sepconv2d_include_list
-)
+    templates.get_backend(backend).register_templates(
+        'PointwiseConv2D',
+        pointwise_conv2d_function_template,
+        templates.get_backend(backend).get_config_template('Conv2D'),
+        sepconv2d_include_list
+    )
 
 class OptimizePointwiseConv(OptimizerPass):
     def match(self, node):
         return node.__class__.__name__ in ['Conv1D', 'Conv2D'] and \
             node.get_attr('filt_height', 1) == 1 and \
             node.get_attr('filt_width') == 1
 
     def transform(self, model, node):
         dim = node.__class__.__name__[-2:] # '1D' or '2D'
         pw_node = model.make_node('PointwiseConv' + dim, node.name, node.attributes.copy(), node.inputs.copy())
+        if len(node.weights['weight'].data.shape) == 2: # This can happen if we assign weights of Dense layer to 1x1 Conv2D
+            pw_node.weights['weight'].data = np.expand_dims(node.weights['weight'].data, axis=(0,1))
+        pw_node.weights['bias'].data = node.weights['bias'].data
         model.replace_node(node, pw_node)
         
         return True
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/optimizer/passes/qkeras.py` & `hls4ml-0.6.0/hls4ml/model/optimizer/passes/qkeras.py`

 * *Files 14% similar despite different names*

```diff
@@ -92,24 +92,25 @@
 
     def add_bias(self, bias, quantizer=None):
         self.add_weights_variable(name='bias', var_name='b{index}', data=bias, quantizer=quantizer)
 
 # register the layer and its templates
 register_layer('ApplyAlpha', ApplyAlpha)
 # TODO ideally: for backend in backends
-temps = templates.get_backend('Vivado')
-temps.register_templates('ApplyAlpha', temps.get_function_template('BatchNormalization'), temps.get_config_template('BatchNormalization'), temps.get_include_list('BatchNormalization'))
+for backend in ['Vivado', 'VivadoAccelerator']:
+    temps = templates.get_backend(backend)
+    temps.register_templates('ApplyAlpha', temps.get_function_template('BatchNormalization'), temps.get_config_template('BatchNormalization'), temps.get_include_list('BatchNormalization'))
 
 class QKerasFactorizeAlpha(OptimizerPass):
     '''OptimizerPass for extracting alpha "scale" from QKeras quantized layer.
        The weights of the Q{Dense, Conv} layer are scaled to the common data type,
        and an 'ApplyAlpha' layer is inserted to reapply the scale.
     '''
     def match(self, node):
-        q_layer = node.__class__.__name__ in ["Dense", "Conv1D", "Conv2D"]
+        q_layer = node.__class__.__name__ in ["Dense", "Conv1D", "Conv2D", "Conv2DBatchnorm"]
         has_w_quant = node.get_attr('weight_quantizer') is not None 
         has_b_quant = node.get_attr('bias_quantizer') is not None
         has_w_alpha, has_b_alpha = False, False
         if has_w_quant:
             if hasattr(node.get_attr('weight_quantizer'), 'alpha'):
                 w_alpha = node.get_attr('weight_quantizer').alpha
                 has_w_alpha = w_alpha != 1 and w_alpha is not None
@@ -127,15 +128,15 @@
     def transform(self, model, node):
         # The quantizer has to be applied to set the scale attribute
         # This must be applied to the _unquantized_ weights to obtain the correct scale
         quantizer = node.weights['weight'].quantizer.quantizer_fn # get QKeras quantizer
         weights = node.weights['weight'].data_unquantized # get weights
         qweights = quantizer(tf.convert_to_tensor(weights))
         if isinstance(quantizer.scale, (int, float)):
-            scale = np.ones(shape=node.get_output_variable().shape) * quantizer.scale
+            scale = np.ones(shape=node.get_output_variable().shape[-1]) * quantizer.scale
         else:
             scale = quantizer.scale.numpy()
         unscale = 1. / scale
 
         new_weights = unscale * qweights # use the quantized weights for safety
 
 
@@ -143,15 +144,20 @@
         alpha = qcfg['alpha']
         # Set the alpha to 1 to avoid hitting this pass again
         qcfg['alpha'] = 1
         node.weights['weight'].quantizer.quantizer_fn = quantizer.from_config(qcfg)
 
         # update the weights also applying the hls4ml quantizer
         # this is only needed for the binary layers which encode -1 as 0
-        node.weights['weight'].data = node.weights['weight'].quantizer(new_weights.numpy())
+        quantized_new_weights = node.weights['weight'].quantizer(new_weights.numpy())
+        if node.model.config.is_resource_strategy(node):
+            ndim = len(weights.shape) - 1
+            perm = [ndim] + [i for i in range(ndim)]
+            quantized_new_weights = np.transpose(quantized_new_weights, axes=perm)
+        node.weights['weight'].data = quantized_new_weights
 
         # Move the biases from the Dense layer to the ApplyAlpha layer
         bias = node.weights['bias'].data
         bias_quantizer = None
         if hasattr(node.weights['bias'], 'quantizer'):
             bias_quantizer = node.weights['bias'].quantizer
         node.weights['bias'].data = np.zeros(bias.shape)
@@ -213,7 +219,44 @@
         b2 = s1 * b0 + b1
 
         bn0.weights['scale'].data = s2
         bn0.weights['bias'].data = b2
 
         model.remove_node(node, rewire=True)
         return True
+
+class ExtractTernaryThreshold(OptimizerPass):
+    ''' The input value (threshold) at which the output of a a ternary activation
+    changes is configurable. This pass extracts that threshold point, inserting
+    a BatchNormalization layer to execute the scaling. That BatchNormalization
+    layer is then expected to be fused into a BatchNormalizationQuantizedTanh
+    layer configured with the correct threshold.
+    '''
+
+    def match(self, node):
+        return node.__class__.__name__ == 'TernaryTanh' and node.get_attr('threshold', None) != 0.5
+
+    def transform(self, model, node):
+        shape = node.get_input_variable().shape
+        scale = np.full(shape, 0.5 / node.get_attr('threshold', 0.5))
+        bias = np.zeros_like(scale)
+        node.set_attr('threshold', 0.5)
+
+        attrs = {
+            'name' : node.get_attr('name') + '_scale',
+            'class_name' : 'Alpha',
+            'inputs' : node.get_input_node().outputs,
+            'outputs' : node.inputs,
+            'n_filt' : node.get_attr('n_filt', -1),
+            'reuse_factor' : node.get_attr('reuse_factor'),
+            # These should just be placeholders
+            'bias_t' : IntegerPrecisionType(1),
+            'scale_t' : FixedPrecisionType(16,6),
+            'Trace' : node.get_attr('Trace', False)
+        }
+
+        layer = model.make_node('ApplyAlpha', node.name + '_scale', attrs, node.inputs.copy())
+        layer.add_weights(scale)
+        layer.add_bias(bias)
+        model.insert_node(layer, before=node)
+        return True
+
```

### Comparing `hls4ml-0.5.0b0/hls4ml/model/profiling.py` & `hls4ml-0.6.0/hls4ml/model/profiling.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import importlib
 from hls4ml.model.hls_model import HLSModel
 from hls4ml.model.hls_layers import IntegerPrecisionType, FixedPrecisionType
-import qkeras
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas
 import seaborn as sb
+import uuid
+import os
+import shutil
+import json
+from collections import defaultdict
 
 from hls4ml.model.hls_model import HLSModel
 
 try:
     from tensorflow import keras
     import qkeras
     __tf_profiling_enabled__ = True
@@ -19,14 +22,34 @@
 try:
     import torch
     __torch_profiling_enabled__ = True
 except ImportError:
     __torch_profiling_enabled__ = False
 
 
+def get_unoptimized_hlsmodel(model):
+    from hls4ml.converters import convert_from_config
+
+    new_config = model.config.config.copy()
+    new_config['HLSConfig'] = json.loads(json.dumps(new_config['HLSConfig']))
+
+    new_output_dir = uuid.uuid4().hex
+
+    while os.path.exists(new_output_dir):
+        new_output_dir = uuid.uuid4().hex
+
+    if 'SkipOptimizers' in new_config['HLSConfig']:
+        del new_config['HLSConfig']['SkipOptimizers']
+
+    new_config['HLSConfig']['Optimizers'] = []
+    new_config['OutputDir'] = new_output_dir
+
+    return convert_from_config(new_config), new_output_dir
+
+
 def array_to_summary(x, fmt='boxplot'):
     if fmt == 'boxplot':
         y = {'med' : np.median(x),
              'q1' : np.percentile(x, 25),
              'q3' : np.percentile(x, 75),
              'whislo' : min(x),
              'whishi' : max(x)
@@ -132,102 +155,160 @@
             col = colors[np.argwhere(layers == row['layer'])[0][0]]
             plt.plot((row['low'], row['low']), ylim, '--', color=col)
             plt.plot((row['high'], row['high']), ylim, '--', color=col)
 
 types_plots = {'boxplot' : types_boxplot,
                'histogram' : types_histogram}
 
-def ap_fixed_WIF(dtype):
+def ap_fixed_WIFS(dtype):
     from hls4ml.templates.vivado_template import VivadoBackend
     dtype = VivadoBackend.convert_precision_string(None, dtype) 
-    W, I, F = dtype.width, dtype.integer, dtype.fractional
-    return W, I, F
+    W, I, F, S = dtype.width, dtype.integer, dtype.fractional, dtype.signed
+    return W, I, F, S
 
 def types_hlsmodel(model):
+    suffix = ['w', 'b']
     data = {'layer' : [], 'low' : [], 'high' : []}
     # Plot the default precision
     default_precision = model.config.model_precision['default']
-    # assumes ap_fixed
-    W, I, F = ap_fixed_WIF(default_precision)
+    W, I, F, S = ap_fixed_WIFS(default_precision)
     data['layer'].append('model')
     data['low'].append(-F)
-    data['high'].append(I-1)
+    data['high'].append(I-1 if S else I)
 
     for layer in model.get_layers():
         for iw, weight in enumerate(layer.get_weights()):
-            wname = '{}/{}'.format(layer.name, iw)
+            wname = '{}/{}'.format(layer.name, suffix[iw])
             T = weight.type
             if T.name != 'model':
-                W, I, F = ap_fixed_WIF(T.precision)
+                W, I, F, S = ap_fixed_WIFS(T.precision)
                 data['layer'].append(wname)
                 data['low'].append(-F)
-                data['high'].append(I-1)
+                data['high'].append(I-1 if S else I)
     data = pandas.DataFrame(data)
     return data
 
 def activation_types_hlsmodel(model):
     data = {'layer' : [], 'low' : [], 'high' : []}
     # Get the default precision
     default_precision = model.config.model_precision['default']
-    W, I, F = ap_fixed_WIF(default_precision)
+    W, I, F, S = ap_fixed_WIFS(default_precision)
     data['layer'].append('model')
     data['low'].append(-F)
-    data['high'].append(I-1)
+    data['high'].append(I-1 if S else I)
     for layer in model.get_layers():
         T = layer.get_output_variable().type.precision
-        W, I, F = ap_fixed_WIF(T)
+        W, I, F, S = ap_fixed_WIFS(T)
         data['layer'].append(layer.name)
         data['low'].append(-F)
-        data['high'].append(I-1)
+        data['high'].append(I-1 if S else I)
     data = pandas.DataFrame(data)
     return data
 
 def weights_hlsmodel(model, fmt='longform', plot='boxplot'):
     suffix = ['w', 'b']
     if fmt == 'longform':
         data = {'x' : [], 'layer' : [], 'weight' : []}
     elif fmt == 'summary':
         data = []
+
     for layer in model.get_layers():
         name = layer.name
         for iw, weight in enumerate(layer.get_weights()):
             l = '{}/{}'.format(name, suffix[iw])
             w = weight.data.flatten()
             w = abs(w[w != 0])
             n = len(w)
             if n == 0:
+                print(f'Weights for {name} are only zeros, ignoring.')
                 break
             if fmt == 'longform':
                 data['x'].extend(w.tolist())
                 data['layer'].extend([name for i in range(len(w))])
                 data['weight'].extend([l for i in range(len(w))])
             elif fmt == 'summary':
                 data.append(array_to_summary(w, fmt=plot))
                 data[-1]['layer'] = name
                 data[-1]['weight'] = l
 
     if fmt == 'longform':
         data = pandas.DataFrame(data)
     return data
 
+
+def _keras_batchnorm(layer):
+    weights = layer.get_weights()
+    epsilon = layer.epsilon
+
+    gamma = weights[0]
+    beta = weights[1]
+    mean = weights[2]
+    var = weights[3]
+
+    scale = gamma / np.sqrt(var + epsilon)
+    bias = beta - gamma * mean / np.sqrt(var + epsilon)
+
+    return [scale, bias], ['s', 'b']
+
+
+def _keras_layer(layer):
+    return layer.get_weights(), ['w', 'b']
+
+
+keras_process_layer_map = defaultdict(lambda: _keras_layer,
+                                      {
+                                          'BatchNormalization': _keras_batchnorm,
+                                          'QBatchNormalization': _keras_batchnorm
+                                      })
+
+
+def activations_hlsmodel(model, X, fmt='summary', plot='boxplot'):
+    if fmt == 'longform':
+        raise NotImplemented
+    elif fmt == 'summary':
+        data = []
+
+    _, trace = model.trace(np.ascontiguousarray(X))
+
+    if len(trace) == 0:
+        raise RuntimeError("HLSModel must have tracing on for at least 1 layer (this can be set in its config)")
+
+    for layer in trace.keys():
+        print("   {}".format(layer))
+
+        if fmt == 'summary':
+            y = trace[layer].flatten()
+            y = abs(y[y != 0])
+
+            if len(y) == 0:
+                print(f'Activations for {layer} are only zeros, ignoring.')
+                continue
+
+            data.append(array_to_summary(y, fmt=plot))
+            data[-1]['weight'] = layer
+
+    return data
+
+
 def weights_keras(model, fmt='longform', plot='boxplot'):
-    suffix = ['w', 'b']
     if fmt == 'longform':
         data = {'x' : [], 'layer' : [], 'weight' : []}
     elif fmt == 'summary':
         data = []
     for layer in model.layers:
         name = layer.name
-        weights = layer.get_weights()
+        weights, suffix = keras_process_layer_map[type(layer).__name__](layer)
+
         for i, w in enumerate(weights):
             l = '{}/{}'.format(name, suffix[i])
             w = w.flatten()
             w = abs(w[w != 0])
             n = len(w)
             if n == 0:
+                print(f'Weights for {name} are only zeros, ignoring.')
                 break
             if fmt == 'longform':
                 data['x'].extend(w.tolist())
                 data['layer'].extend([name for j in range(n)])
                 data['weight'].extend([l for j in range(n)])
             elif fmt == 'summary':
                 data.append(array_to_summary(w, fmt=plot))
@@ -245,22 +326,22 @@
         # seaborn boxplot
         data = {'x' : [], 'weight' : []}
     elif fmt == 'summary':
         # return summary statistics for matplotlib.axes.Axes.bxp
         # or histogram bin edges and heights
         data = []
 
-    partial_model = keras.models.Sequential()
     for layer in model.layers:
         print("   {}".format(layer.name))
-        partial_model.add(layer)
-        partial_model.compile(optimizer='adam', loss='mse')
         if not isinstance(layer, keras.layers.InputLayer):
-            y = partial_model.predict(X).flatten()
+            y = _get_output(layer, X, model.input).flatten()
             y = abs(y[y != 0])
+            if len(y) == 0:
+                print(f'Activations for {layer.name} are only zeros, ignoring.')
+                continue
             if fmt == 'longform':
                 data['x'].extend(y.tolist())
                 data['weight'].extend([layer.name for i in range(len(y))])
             elif fmt == 'summary':
                 data.append(array_to_summary(y, fmt=plot))
                 data[-1]['weight'] = layer.name
 
@@ -282,14 +363,15 @@
             for i, w in enumerate(weights):
                 l = '{}/{}'.format(name, suffix[i])
                 w = weights[i].detach().numpy()
                 w = w.flatten()
                 w = abs(w[w != 0])
                 n = len(w)
                 if n == 0:
+                    print(f'Weights for {name} are only zeros, ignoring.')
                     break
                 if fmt == 'longform':
                     data['x'].extend(w.tolist())
                     data['layer'].extend([name for _ in range(n)])
                     data['weight'].extend([l for _ in range(n)])
                 elif fmt == 'summary':
                     data.append(array_to_summary(w, fmt=plot))
@@ -313,14 +395,17 @@
     for layer in model.children():
         lname = layer.__class__.__name__
         layers.append(layer)
         pm = partial_model(*layers)
         print("   {}".format(lname))
         y = pm(X).flatten().detach().numpy()
         y = abs(y[y != 0])
+        if len(y) == 0:
+            print(f'Activations for {lname} are only zeros, ignoring.')
+            continue
         if fmt == 'longform':
             data['x'].extend(y.tolist())
             data['weight'].extend([lname for _ in range(len(y))])
         elif fmt == 'summary':
             data.append(array_to_summary(y, fmt=plot))
             data[-1]['weight'] = lname
 
@@ -337,135 +422,180 @@
     ----------
     model : keras or pytorch model
         The model to profile
     hls_model : HLSModel
         The HLSModel to profile
     X : array-like, optional
         Test data on which to evaluate the model to profile activations
-        Must be formatted suitably for the model.predict(X) method
+        Must be formatted suitably for the ``model.predict(X)`` method
     plot : str, optional
         The type of plot to produce.
         Options are: 'boxplot' (default), 'violinplot', 'histogram',
         'FacetGrid'
 
     Returns
     -------
     tuple
-        The pair of produced figures. First weights and biases,
-        then activations
+        The quadruple of produced figures. First weights and biases
+        for the pre- and post-optimization models respectively,
+        then activations for the pre- and post-optimization models
+        respectively. (Optimizations are applied to an HLSModel by hls4ml,
+        a post-optimization HLSModel is a final model)
     """
-    wp, ap = None, None
+    wp, wph, ap, aph = None, None, None, None
+
+    hls_model_present = hls_model is not None and isinstance(hls_model, HLSModel)
+    model_present = model is not None
 
-    print("Profiling weights")
+    if hls_model_present:
+        before = " (before optimization)"
+        after = " (final / after optimization)"
+        hls_model_unoptimized, tmp_output_dir = get_unoptimized_hlsmodel(hls_model)
+    else:
+        before = ""
+        after = ""
+        hls_model_unoptimized, tmp_output_dir = None, None
+
+    print("Profiling weights" + before)
     data = None
-    if hls_model is not None and isinstance(hls_model, HLSModel):
-        data = weights_hlsmodel(hls_model, fmt='summary', plot=plot)
-    elif model is not None:
+
+    if hls_model_present:
+        data = weights_hlsmodel(hls_model_unoptimized, fmt='summary', plot=plot)
+    elif model_present:
         if __tf_profiling_enabled__ and isinstance(model, keras.Model):
             data = weights_keras(model, fmt='summary', plot=plot)
         elif __torch_profiling_enabled__ and \
                 isinstance(model, torch.nn.Sequential):
             data = weights_torch(model, fmt='summary', plot=plot)
+
     if data is None:
         print("Only keras, PyTorch (Sequential) and HLSModel models " +
               "can currently be profiled")
-        return wp, ap
+
+        if hls_model_present and os.path.exists(tmp_output_dir):
+            shutil.rmtree(tmp_output_dir)
+
+        return wp, wph, ap, aph
 
     wp = plots[plot](data, fmt='summary')  # weight plot
-    if isinstance(hls_model, HLSModel) and plot in types_plots:
-        t_data = types_hlsmodel(hls_model)
+
+    if hls_model_present and plot in types_plots:
+        t_data = types_hlsmodel(hls_model_unoptimized)
         types_plots[plot](t_data, fmt='summary')
 
-    plt.title("Distribution of (non-zero) weights")
+    plt.title("Distribution of (non-zero) weights" + before)
     plt.tight_layout()
 
-    print("Profiling activations")
-    data = None
+    if hls_model_present:
+        print("Profiling weights" + after)
+
+        data = weights_hlsmodel(hls_model, fmt='summary', plot=plot)
+        wph = plots[plot](data, fmt='summary')  # weight plot
+
+        if plot in types_plots:
+            t_data = types_hlsmodel(hls_model)
+            types_plots[plot](t_data, fmt='summary')
+
+        plt.title("Distribution of (non-zero) weights" + after)
+        plt.tight_layout()
+
     if X is not None:
+        print("Profiling activations" + before)
+        data = None
         if __tf_profiling_enabled__ and isinstance(model, keras.Model):
             data = activations_keras(model, X, fmt='summary', plot=plot)
         elif __torch_profiling_enabled__ and \
                 isinstance(model, torch.nn.Sequential):
             data = activations_torch(model, X, fmt='summary', plot=plot)
-    if data is not None:
-        ap = plots[plot](data, fmt='summary')  # activation plot
-        plt.title("Distribution of (non-zero) activations")
-        plt.tight_layout()
 
-    if X is not None and isinstance(hls_model, HLSModel):
-        t_data = activation_types_hlsmodel(hls_model)
-        types_plots[plot](t_data, fmt='summary')
+        if data is not None:
+            ap = plots[plot](data, fmt='summary')  # activation plot
+            if hls_model_present and plot in types_plots:
+                t_data = activation_types_hlsmodel(hls_model_unoptimized)
+                types_plots[plot](t_data, fmt='summary')
+            plt.title("Distribution of (non-zero) activations" + before)
+            plt.tight_layout()
+
+        if hls_model_present:
+            print("Profiling activations" + after)
+            data = activations_hlsmodel(hls_model, X, fmt='summary', plot=plot)
+            aph = plots[plot](data, fmt='summary')
+
+            t_data = activation_types_hlsmodel(hls_model)
+            types_plots[plot](t_data, fmt='summary')
+
+            plt.title("Distribution of (non-zero) activations (final / after optimization)")
+            plt.tight_layout()
+
+    if hls_model_present and os.path.exists(tmp_output_dir):
+        shutil.rmtree(tmp_output_dir)
 
-    return wp, ap
+    return wp, wph, ap, aph
 
 
 ########COMPARE OUTPUT IMPLEMENTATION########
 def _is_ignored_layer(layer):
     """Some layers need to be ingored during inference"""
     if isinstance(layer, (keras.layers.InputLayer,
                         keras.layers.Dropout)):
         return True
     return False
 
-def _get_output(ymodel, layer, X):
-    
-    #If there is no layer in the model just take that layer's output
-    if len(ymodel.keys()) == 0:
-        y = layer(X)
-    else:
-        #If there are already layers then calculate next output based on last layer's output
-        y = layer(ymodel[list(ymodel.keys())[-1]])
+def _get_output(layer, X, model_input):
+    """Get output of partial model"""
+    partial_model = keras.models.Model(inputs=model_input,
+                                       outputs=layer.output)
+    y = partial_model.predict(X)
     return y
 
 def get_ymodel_keras(keras_model, X):
     """
     Calculate each layer's ouput and put them into a dictionary
-    Params:
-    ------
-    keras_model: a keras model
+
+    Parameters
+    ----------
+    keras_model :
+        a keras model
     X : array-like
-        Test data on which to evaluate the model to profile activations
-        Must be formatted suitably for the model.predict(X) method
-    Return:
-    ------
+        Test data on which to evaluate the model to profile activations.
+        Must be formatted suitably for the ``model.predict(X)`` method.
+
+    Returns
+    -------
+    dictionary
         A dictionary in the form {"layer_name": ouput array of layer}
     """
     
-    partial_model = keras.models.Sequential()
     ymodel = {}
     
     for layer in keras_model.layers:
         print("Processing {} in Keras model...".format(layer.name))
         if not _is_ignored_layer(layer):
             #If the layer has activation integrated then separate them
             #Note that if the layer is a standalone activation layer then skip this
             if hasattr(layer, 'activation') and not (isinstance(layer,keras.layers.Activation) or isinstance(layer, qkeras.qlayers.QActivation)):
                 if layer.activation:
                     
                     if layer.activation.__class__.__name__ == "linear":
-                        ymodel[layer.name] = _get_output(ymodel, layer, X)
+                        ymodel[layer.name] = _get_output(layer, X, keras_model.input)
                     
                     else:
                         temp_activation = layer.activation
                         layer.activation = None
                         #Get output for layer without activation
-                        ymodel[layer.name] = _get_output(ymodel, layer, X)
+                        ymodel[layer.name] = _get_output(layer, X, keras_model.input)
 
-                        #Get ouput for activation
-                        ymodel[layer.name + "_{}".format(temp_activation.__class__.__name__)] =  _get_output(ymodel, temp_activation, X)
-
-                        #Add the activation back
+                        #Add the activation back 
                         layer.activation = temp_activation
+                        #Get ouput for activation
+                        ymodel[layer.name + "_{}".format(temp_activation.__class__.__name__)] =  _get_output(layer, X, keras_model.input)
                 else:
-                    ymodel[layer.name] = _get_output(ymodel, layer, X)
+                    ymodel[layer.name] = _get_output(layer, X, keras_model.input)
             else:    
-                ymodel[layer.name] = _get_output(ymodel, layer, X)
-        
-        #Add the layer for later processing
-        partial_model.add(layer)
+                ymodel[layer.name] = _get_output(layer, X, keras_model.input)
     print("Done taking outputs for Keras model.")
     return ymodel
 
 def _norm_diff(ymodel, ysim):
     """Calculate the square root of the sum of the squares of the differences"""
     diff = {}
     
@@ -480,15 +610,14 @@
     plt.xticks(rotation=90)
     plt.tight_layout()
     return f
 
 def _dist_diff(ymodel, ysim):
     """
     Calculate the normalized distribution of the differences of the elements
-    of the output vectors 
     of the output vectors. 
     If difference >= original value then the normalized difference will be set to 1,
     meaning "very difference".
     If difference < original value then the normalized difference would be difference/original.
     """
 
     diff = {}
@@ -498,15 +627,15 @@
         flattened_ymodel = np.array(ymodel[key]).flatten()
 
         diff[key] = np.absolute(flattened_ymodel - flattened_ysim) / np.linalg.norm(flattened_ymodel - flattened_ysim)
         diff_vector = np.absolute(flattened_ymodel - flattened_ysim)
         abs_ymodel = np.absolute(flattened_ymodel)
 
         normalized_diff = np.zeros(diff_vector.shape)
-        normalized_diff[diff_vector >= abs_ymodel] = 1
+        normalized_diff[(diff_vector >= abs_ymodel) & (abs_ymodel>0) & (diff_vector>0)] = 1
 
         #Fill out the rest
         index = diff_vector < abs_ymodel
         normalized_diff[index] = diff_vector[index] / abs_ymodel[index]
 
         diff[key] = normalized_diff
 
@@ -524,29 +653,36 @@
     plt.tight_layout()
 
     return f
 
 def compare(keras_model, hls_model, X, plot_type = "dist_diff"):
     """
     Compare each layer's output in keras and hls model. Note that the hls_model should not be compiled before using this.
-    Params:
-    ------
-    keras_model : original keras model
-    hls_model : converted HLS model, with "Trace:True" in the configuration file.
-    X: numpy array, input for the model. 
-    plot_type : (string) different methods to visualize the y_model and y_sim differences.
-                Possible options include:
-                     - "norm_diff" : square root of the sum of the squares of the differences 
-                                    between each output vectors 
-                     - "dist_diff" : The normalized distribution of the differences of the elements
-                                    between two output vectors
+
+    Parameters
+    ----------
+    keras_model : 
+        original keras model
+    hls_model :
+        converted HLSModel, with "Trace:True" in the configuration file.
+    X : array-like 
+        Input for the model. 
+    plot_type : string
+        different methods to visualize the y_model and y_sim differences.
+        Possible options include:
+        
+        - 'norm_diff' : square root of the sum of the squares of the differences 
+          between each output vectors 
+        - 'dist_diff' : The normalized distribution of the differences of the elements
+          between two output vectors
         
-    Return:
-    ------
-        plot object of the histogram depicting the difference in each layer's ouput
+    Returns
+    -------
+    matplotlib figure
+        plot object of the histogram depicting the difference in each layer's output
     """
     
     #Take in output from both models
     #Note that each y is a dictionary with structure {"layer_name": flattened ouput array}
     ymodel = get_ymodel_keras(keras_model, X)
     _, ysim = hls_model.trace(X)
```

### Comparing `hls4ml-0.5.0b0/hls4ml/report/vivado_report.py` & `hls4ml-0.6.0/hls4ml/report/vivado_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,23 +123,23 @@
     report = {}
 
     sim_file = hls_dir + '/tb_data/csim_results.log'
     if os.path.isfile(sim_file):
         csim_results = []
         with open(sim_file, 'r') as f:
             for line in f.readlines():
-                csim_results.append([float(r) for r in line.split()])
+                csim_results.append([r for r in line.split()])
         report['CSimResults'] = csim_results
 
     sim_file = hls_dir + '/tb_data/rtl_cosim_results.log'
     if os.path.isfile(sim_file):
         cosim_results = []
         with open(sim_file, 'r') as f:
             for line in f.readlines():
-                cosim_results.append([float(r) for r in line.split()])
+                cosim_results.append([r for r in line.split()])
         report['CosimResults'] = cosim_results
 
     syn_file = sln_dir + '/' + solutions[0] + '/syn/report/{}_csynth.xml'.format(top_func_name)
     if os.path.isfile(syn_file):
         root = ET.parse(syn_file).getroot()
 
         # Performance
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/templates.py` & `hls4ml-0.6.0/hls4ml/templates/templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+import os.path
+
 
 class Backend(object):
     def __init__(self, name):
         self.name = name
         self.config_templates = {}
         self.function_templates = {}
         self.include_lists = {}
@@ -29,7 +32,13 @@
     if name in backend_map:
         raise Exception('Backend {} already registered'.format(name))
     
     backend_map[name] = backend_cls()
 
 def get_backend(name):
     return backend_map[name]
+
+def get_available_backends():
+    return list(backend_map.keys())
+
+def get_supported_boards_dict():
+    return json.load(open(os.path.dirname(__file__) + '/supported_boards.json'))
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_common.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_common.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_decl.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_decl.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed_base.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed_base.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed_ref.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed_ref.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_fixed_special.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_fixed_special.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int_base.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int_base.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int_ref.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int_ref.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/ap_int_special.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/ap_int_special.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/etc/ap_private.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/etc/ap_private.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/hls_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/hls_stream.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/ap_types/utils/x_hls_utils.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/ap_types/utils/x_hls_utils.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/build_lib.sh` & `hls4ml-0.6.0/hls4ml/templates/vivado/build_lib.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/build_prj.tcl` & `hls4ml-0.6.0/hls4ml/templates/vivado/build_prj.tcl`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/firmware/myproject.cpp` & `hls4ml-0.6.0/hls4ml/templates/vivado/firmware/myproject.cpp`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/firmware/myproject.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/firmware/myproject.h`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,13 @@
 
 #include "ap_int.h"
 #include "ap_fixed.h"
 #include "hls_stream.h"
 
 #include "defines.h"
 
-
 // Prototype of top level function for C-synthesis
 void myproject(
     //hls-fpga-machine-learning insert header
 );
 
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/myproject_bridge.cpp` & `hls4ml-0.6.0/hls4ml/templates/vivado/myproject_bridge.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 #define MYPROJECT_BRIDGE_H_
 
 #include "firmware/myproject.h"
 #include "firmware/nnet_utils/nnet_helpers.h"
 #include <algorithm>
 #include <map>
 
+//hls-fpga-machine-learning insert bram
+
+
 namespace nnet {
     bool trace_enabled = false;
     std::map<std::string, void *> *trace_outputs = NULL;
     size_t trace_type_size = sizeof(double);
 }
 
 extern "C" {
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/myproject_test.cpp` & `hls4ml-0.6.0/hls4ml/templates/vivado/myproject_test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
 
 #include "firmware/myproject.h"
 #include "firmware/nnet_utils/nnet_helpers.h"
 
+//hls-fpga-machine-learning insert bram
+
 #define CHECKPOINT 5000
 
 namespace nnet {
     bool trace_enabled = true;
     std::map<std::string, void *> *trace_outputs = NULL;
     size_t trace_type_size = sizeof(double);
 }
@@ -88,21 +90,23 @@
       //hls-fpga-machine-learning insert tb-output
 
     }
     fin.close();
     fpr.close();
   } else {
     std::cout << "INFO: Unable to open input/predictions file, using default input." << std::endl;
+
     //hls-fpga-machine-learning insert zero
 
     //hls-fpga-machine-learning insert top-level-function
 
     //hls-fpga-machine-learning insert output
 
     //hls-fpga-machine-learning insert tb-output
+
   }
 
   fout.close();
   std::cout << "INFO: Saved inference results to file: " << RESULTS_LOG << std::endl;
 
   return 0;
 }
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_activation.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_activation.h`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,15 @@
         typename CONFIG_T::inv_table_t inv_x = 1 / x;
         table_out[i] = inv_x;
     }
 }
 
 template <class data_T, class res_T, typename CONFIG_T>
 void softmax_latency(data_T data[CONFIG_T::n_in], res_T res[CONFIG_T::n_in]){
+    #pragma HLS pipeline
     // Initialize the lookup tables
 #ifdef __HLS_SYN__
     bool initialized = false;
     typename CONFIG_T::exp_table_t exp_table[CONFIG_T::table_size];
     typename CONFIG_T::inv_table_t invert_table[CONFIG_T::table_size];
 #else
     static bool initialized = false;
@@ -238,19 +239,19 @@
         // Note we are inverting the exponentials, which have type exp_table_t
         init_invert_table<typename CONFIG_T::exp_table_t, CONFIG_T>(invert_table);
         initialized = true;
     }
 
     // Calculate all the e^x's
     typename CONFIG_T::exp_table_t exp_res[CONFIG_T::n_in];
-	#pragma HLS array_partition variable=exp_res complete
+    #pragma HLS array_partition variable=exp_res complete
     typename CONFIG_T::exp_table_t exp_sum(0);
     for(unsigned i = 0; i < CONFIG_T::n_in; i++){
         #pragma HLS unroll
-    	unsigned x = softmax_idx_from_real_val<data_T, CONFIG_T>(data[i]);
+        unsigned x = softmax_idx_from_real_val<data_T, CONFIG_T>(data[i]);
         exp_res[i] = exp_table[x];
     }
 
     // Explicitly sum the results with an adder tree.
     // Rounding & Saturation mode, which improve accuracy, prevent Vivado from expression balancing
     Op_add<typename CONFIG_T::exp_table_t> op_add;
     exp_sum = reduce<typename CONFIG_T::exp_table_t, CONFIG_T::n_in, Op_add<typename CONFIG_T::exp_table_t>>(exp_res, op_add);
@@ -260,14 +261,15 @@
         #pragma HLS unroll
         res[i] = exp_res[i] * inv_exp_sum;
     }
 }
 
 template <class data_T, class res_T, typename CONFIG_T>
 void softmax_stable(data_T data[CONFIG_T::n_in], res_T res[CONFIG_T::n_in]){
+    #pragma HLS pipeline
     // Initialize the lookup tables
 #ifdef __HLS_SYN__
     bool initialized = false;
     typename CONFIG_T::exp_table_t exp_table[CONFIG_T::table_size];
     typename CONFIG_T::inv_table_t invert_table[CONFIG_T::table_size];
 #else
     static bool initialized = false;
@@ -292,19 +294,19 @@
     for(unsigned i = 0; i < CONFIG_T::n_in; i++){
         #pragma HLS unroll
         d_xi_xmax[i] = data[i] - x_max;
     }
 
     // Calculate all the e^x's
     typename CONFIG_T::exp_table_t exp_res[CONFIG_T::n_in];
-	#pragma HLS array_partition variable=exp_res complete
+    #pragma HLS array_partition variable=exp_res complete
     typename CONFIG_T::exp_table_t exp_sum(0);
     for(unsigned i = 0; i < CONFIG_T::n_in; i++){
         #pragma HLS unroll
-    	unsigned x = softmax_idx_from_real_val<data_T, CONFIG_T>(d_xi_xmax[i]);
+        unsigned x = softmax_idx_from_real_val<data_T, CONFIG_T>(d_xi_xmax[i]);
         exp_res[i] = exp_table[x];
     }
 
     // Explicitly sum the results with an adder tree.
     // Rounding & Saturation mode, which improve accuracy, prevent Vivado from expression balancing
     Op_add<typename CONFIG_T::exp_table_t> op_add;
     exp_sum = reduce<typename CONFIG_T::exp_table_t, CONFIG_T::n_in, Op_add<typename CONFIG_T::exp_table_t>>(exp_res, op_add);
@@ -331,19 +333,19 @@
 
 template<typename CONFIG_T, int N_TABLE>
 void init_invert_table_legacy(typename CONFIG_T::table_t table_out[N_TABLE])
 {
     // Inversion function:
     //   result = 1/x
     for (int ii = 0; ii < N_TABLE; ii++) {
-      // First, convert from table index to X-value (signed 8-bit, range 0 to +64)
-	float in_val = 64.0*ii/float(N_TABLE);
+        // First, convert from table index to X-value (signed 8-bit, range 0 to +64)
+        float in_val = 64.0*ii/float(N_TABLE);
         // Next, compute lookup table function
-	if (in_val > 0.0) table_out[ii] = 1.0/in_val;
-	else table_out[ii] = 0.0;
+        if (in_val > 0.0) table_out[ii] = 1.0/in_val;
+        else table_out[ii] = 0.0;
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
 void  softmax_legacy(data_T data[CONFIG_T::n_in], res_T res[CONFIG_T::n_in])
 {
     // Initialize the lookup table
@@ -370,58 +372,60 @@
     // Index into the lookup table based on data for exponentials
     typename CONFIG_T::table_t exp_res[CONFIG_T::n_in];// different, independent, fixed point precision
     typename CONFIG_T::table_t exp_diff_res;// different, independent, fixed point precision
     data_T data_cache[CONFIG_T::n_in];
     int data_round;
     int index;
     for (int ii=0; ii<CONFIG_T::n_in; ii++) {
-      data_cache[ii] = data[ii];
-      exp_res[ii] = 0;
+        data_cache[ii] = data[ii];
+        exp_res[ii] = 0;
     }
+
     for (int ii=0; ii<CONFIG_T::n_in; ii++) {
-      if (CONFIG_T::io_type == io_serial){
-          #pragma HLS PIPELINE
-      }
-      for (int jj=0; jj<CONFIG_T::n_in; jj++) {
-	if (ii==jj) exp_diff_res = 1;
-	else {
-	  data_round = (data_cache[jj]-data_cache[ii])*CONFIG_T::table_size/16;
-	  index = data_round + 8*CONFIG_T::table_size/16;
-	  if (index < 0)   index = 0;
-	  if (index > CONFIG_T::table_size-1) index = CONFIG_T::table_size-1;
-	  exp_diff_res = exp_table[index];
-	}
-	exp_res[ii] += exp_diff_res;
-      }
+        if (CONFIG_T::io_type == io_serial) {
+            #pragma HLS PIPELINE
+        }
+        for (int jj=0; jj<CONFIG_T::n_in; jj++) {
+            if (ii==jj) exp_diff_res = 1;
+            else {
+                data_round = (data_cache[jj]-data_cache[ii])*CONFIG_T::table_size/16;
+                index = data_round + 8*CONFIG_T::table_size/16;
+                if (index < 0)   index = 0;
+                if (index > CONFIG_T::table_size-1) index = CONFIG_T::table_size-1;
+                exp_diff_res = exp_table[index];
+            }
+            exp_res[ii] += exp_diff_res;
+        }
     }
 
     //Second loop to invert
     for (int ii=0; ii<CONFIG_T::n_in; ii++) {
-      int exp_res_index = exp_res[ii]*CONFIG_T::table_size/64;
-      if (exp_res_index < 0)   exp_res_index = 0;
-      if (exp_res_index > CONFIG_T::table_size-1) exp_res_index = CONFIG_T::table_size-1;
-      //typename CONFIG_T::table_t exp_res_invert = invert_table[exp_res_index];
-      res[ii] = (res_T) invert_table[exp_res_index];
+        int exp_res_index = exp_res[ii]*CONFIG_T::table_size/64;
+        if (exp_res_index < 0)   exp_res_index = 0;
+        if (exp_res_index > CONFIG_T::table_size-1) exp_res_index = CONFIG_T::table_size-1;
+        //typename CONFIG_T::table_t exp_res_invert = invert_table[exp_res_index];
+        res[ii] = (res_T) invert_table[exp_res_index];
     }
 
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
 void softmax(data_T data[CONFIG_T::n_in], res_T res[CONFIG_T::n_in]){
+    #pragma HLS inline
     switch(CONFIG_T::implementation){
     case softmax_implementation::latency:
         softmax_latency<data_T, res_T, CONFIG_T>(data, res);
         break;
     case softmax_implementation::stable:
         softmax_stable<data_T, res_T, CONFIG_T>(data, res);
         break;
     case softmax_implementation::legacy:
         softmax_legacy<data_T, res_T, CONFIG_T>(data, res);
         break;
-    }    
+    }
 }
 
 // *************************************************
 //       TanH Activation
 // *************************************************
 template<typename CONFIG_T, int N_TABLE>
 void init_tanh_table(typename CONFIG_T::table_t table_out[N_TABLE])
@@ -713,15 +717,15 @@
         }
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
 void  elu(data_T data[CONFIG_T::n_in], res_T res[CONFIG_T::n_in])
 {
-	elu<data_T, res_T, CONFIG_T>(data, 1.0, res);
+    elu<data_T, res_T, CONFIG_T>(data, 1.0, res);
 }
 
 // *************************************************
 //       SELU Activation
 // *************************************************
 inline float selu_fcn_float(float input) {
     return 1.0507009873554804934193349852946 * (1.6732632423543772848170429916717 * (std::exp(input) - 1.));
@@ -803,61 +807,55 @@
 
 // *************************************************
 //       Binary TanH Activation
 // *************************************************
 template<class data_T, class res_T, typename CONFIG_T>
 void  binary_tanh(data_T data[CONFIG_T::n_in], res_T res[CONFIG_T::n_in])
 {
+    if (CONFIG_T::io_type == io_parallel){
+        #pragma HLS PIPELINE
+    }
 
- if (CONFIG_T::io_type == io_parallel){
-     #pragma HLS PIPELINE
- }
-  
- data_T datareg;   
- res_T cache; 
- for (int ii=0; ii<CONFIG_T::n_in; ii++) {
-
-  if (CONFIG_T::io_type == io_serial){
-      #pragma HLS PIPELINE
-  }
-  datareg = data[ii];	 
-  if( datareg > 0 ) cache = 1;
-  else cache = -1;
-  
-  res[ii] = (res_T) cache;
- 
- }
- 
+    data_T datareg;
+    res_T cache;
+    for (int ii=0; ii<CONFIG_T::n_in; ii++) {
+        if (CONFIG_T::io_type == io_serial){
+            #pragma HLS PIPELINE
+        }
+        datareg = data[ii];
+        if( datareg > 0 ) cache = 1;
+        else cache = -1;
+
+        res[ii] = (res_T) cache;
+    }
 }
 
 // *************************************************
 //       Ternary TanH Activation
 // *************************************************
 template<class data_T, class res_T, typename CONFIG_T>
 void  ternary_tanh(data_T data[CONFIG_T::n_in], res_T res[CONFIG_T::n_in])
 {
 
- if (CONFIG_T::io_type == io_parallel){
-     #pragma HLS PIPELINE
- }
+    if (CONFIG_T::io_type == io_parallel){
+        #pragma HLS PIPELINE
+    }
   
- data_T datareg;   
- res_T cache; 
- for (int ii=0; ii<CONFIG_T::n_in; ii++) {
-
-  if (CONFIG_T::io_type == io_serial){
-      #pragma HLS PIPELINE
-  }
-  datareg = 2*data[ii];	 
-  if( datareg > 1 ) cache = 1;
-  else if( datareg > -1 && datareg <= 1) cache=0;
-  else cache = -1;
+    data_T datareg;   
+    res_T cache; 
+    for (int ii=0; ii<CONFIG_T::n_in; ii++) {
+        if (CONFIG_T::io_type == io_serial) {
+            #pragma HLS PIPELINE
+        }
+        datareg = 2*data[ii];
+        if( datareg > 1 ) cache = 1;
+        else if( datareg > -1 && datareg <= 1) cache=0;
+        else cache = -1;
   
-  res[ii] = (res_T) cache;
- 
- }
+        res[ii] = (res_T) cache;
+    }
  
 }
 
 }
 
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_activation_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_activation_stream.h`

 * *Files 3% similar despite different names*

```diff
@@ -135,48 +135,44 @@
         // Note we are exponentiating the inputs, which have type data_T
         init_exp_table<typename data_T::value_type, CONFIG_T>(exp_table);
         // Note we are inverting the exponentials, which have type exp_table_t
         init_invert_table<typename CONFIG_T::exp_table_t, CONFIG_T>(invert_table);
         initialized = true;
     }
 
-    constexpr unsigned multiplier_limit = DIV_ROUNDUP(CONFIG_T::n_in, CONFIG_T::reuse_factor);
-    constexpr unsigned ii = CONFIG_T::n_in / multiplier_limit;
+    constexpr unsigned multiplier_limit = DIV_ROUNDUP(data_T::size, CONFIG_T::reuse_factor);
+    constexpr unsigned ii = data_T::size / multiplier_limit;
 
     // Calculate all the e^x's
-    typename CONFIG_T::exp_table_t exp_res[CONFIG_T::n_in];
+    typename CONFIG_T::exp_table_t exp_res[data_T::size];
     #pragma HLS array_partition variable=exp_res complete
     typename CONFIG_T::exp_table_t exp_sum(0);
     SoftmaxExpLoop: for(unsigned i = 0; i < CONFIG_T::n_in / data_T::size; i++){
-        if (CONFIG_T::n_in / data_T::size > 1) {
-            #pragma HLS PIPELINE
-        }
+        #pragma HLS PIPELINE II=ii
+
         data_T in_pack = data.read();
         SoftmaxExpPackLoop: for(unsigned j = 0; j < data_T::size; j++){
             #pragma HLS UNROLL
             unsigned x = softmax_idx_from_real_val<typename data_T::value_type, CONFIG_T>(in_pack[j]);
-            exp_res[i * data_T::size + j] = exp_table[x];
+            exp_res[j] = exp_table[x];
         }
-    }
 
-    // Explicitly sum the results with an adder tree.
-    // Rounding & Saturation mode, which improve accuracy, prevent Vivado from expression balancing
-    Op_add<typename CONFIG_T::exp_table_t> op_add;
-    exp_sum = reduce<typename CONFIG_T::exp_table_t, CONFIG_T::n_in, Op_add<typename CONFIG_T::exp_table_t>>(exp_res, op_add);
+        // Explicitly sum the results with an adder tree.
+        // Rounding & Saturation mode, which improve accuracy, prevent Vivado from expression balancing
+        Op_add<typename CONFIG_T::exp_table_t> op_add;
+        exp_sum = reduce<typename CONFIG_T::exp_table_t, data_T::size, Op_add<typename CONFIG_T::exp_table_t>>(exp_res, op_add);
 
-    typename CONFIG_T::inv_table_t inv_exp_sum = invert_table[softmax_idx_from_real_val<typename CONFIG_T::exp_table_t,CONFIG_T>(exp_sum)];
-    SoftmaxInvLoop: for(unsigned i = 0; i < CONFIG_T::n_in / res_T::size; i++){
-        #pragma HLS PIPELINE II=ii
+        typename CONFIG_T::inv_table_t inv_exp_sum = invert_table[softmax_idx_from_real_val<typename CONFIG_T::exp_table_t,CONFIG_T>(exp_sum)];
 
         res_T out_pack;
         #pragma HLS DATA_PACK variable=out_pack
         SoftmaxInvPackLoop: for(unsigned j = 0; j < res_T::size; j++){
             #pragma HLS UNROLL
             #pragma HLS ALLOCATION instances=mul limit=multiplier_limit operation
-            out_pack[i * res_T::size + j] = exp_res[i * res_T::size + j] * inv_exp_sum;
+            out_pack[j] = exp_res[j] * inv_exp_sum;
         }
         res.write(out_pack);
     }
 }
 
 template <class data_T, class res_T, typename CONFIG_T>
 void softmax_stable(hls::stream<data_T> &data, hls::stream<res_T> &res){
@@ -195,66 +191,62 @@
         // Note we are exponentiating the inputs, which have type data_T
         init_exp_table<typename data_T::value_type, CONFIG_T>(exp_table);
         // Note we are inverting the exponentials, which have type exp_table_t
         init_invert_table<typename CONFIG_T::exp_table_t, CONFIG_T>(invert_table);
         initialized = true;
     }
 
-    constexpr unsigned multiplier_limit = DIV_ROUNDUP(CONFIG_T::n_in, CONFIG_T::reuse_factor);
-    constexpr unsigned ii = CONFIG_T::n_in / multiplier_limit;
+    constexpr unsigned multiplier_limit = DIV_ROUNDUP(data_T::size, CONFIG_T::reuse_factor);
+    constexpr unsigned ii = data_T::size / multiplier_limit;
 
-    typename data_T::value_type data_array[CONFIG_T::n_in];
+    typename data_T::value_type data_array[data_T::size];
     #pragma HLS ARRAY_PARTITION variable=data_array complete
     SoftmaxArrayLoop: for(unsigned i = 0; i < CONFIG_T::n_in / data_T::size; i++){
-        if (CONFIG_T::n_in / data_T::size > 1) {
-            #pragma HLS PIPELINE
-        }
+        #pragma HLS PIPELINE II=ii
+
         data_T in_pack = data.read();
         SoftmaxArrayPackLoop: for(unsigned j = 0; j < data_T::size; j++){
             #pragma HLS UNROLL
-            data_array[i * data_T::size + j] = in_pack[j];
+            data_array[j] = in_pack[j];
         }
-    }
 
-    // Find the max and compute all delta(x_i, x_max)
-    Op_max<typename data_T::value_type> op_max;
-    typename data_T::value_type x_max = reduce<typename data_T::value_type, CONFIG_T::n_in, Op_max<typename data_T::value_type>>(data_array, op_max);
+        // Find the max and compute all delta(x_i, x_max)
+        Op_max<typename data_T::value_type> op_max;
+        typename data_T::value_type x_max = reduce<typename data_T::value_type, data_T::size, Op_max<typename data_T::value_type>>(data_array, op_max);
 
-    // For the diffs, use the same type as the input but force rounding and saturation
-    ap_fixed<data_T::value_type::width, data_T::value_type::iwidth,AP_RND,AP_SAT> d_xi_xmax[CONFIG_T::n_in];
-    for(unsigned i = 0; i < CONFIG_T::n_in; i++){
-        #pragma HLS UNROLL
-        d_xi_xmax[i] = data_array[i] - x_max;
-    }
+        // For the diffs, use the same type as the input but force rounding and saturation
+        ap_fixed<data_T::value_type::width, data_T::value_type::iwidth,AP_RND,AP_SAT> d_xi_xmax[data_T::size];
+        for(unsigned j = 0; j < data_T::size; j++){
+            #pragma HLS UNROLL
+            d_xi_xmax[j] = data_array[j] - x_max;
+        }
 
-    // Calculate all the e^x's
-    typename CONFIG_T::exp_table_t exp_res[CONFIG_T::n_in];
-    #pragma HLS ARRAY_PARTITION variable=exp_res complete
-    typename CONFIG_T::exp_table_t exp_sum(0);
-    for(unsigned i = 0; i < CONFIG_T::n_in; i++){
-        #pragma HLS UNROLL
-        unsigned x = softmax_idx_from_real_val<typename data_T::value_type, CONFIG_T>(d_xi_xmax[i]);
-        exp_res[i] = exp_table[x];
-    }
+        // Calculate all the e^x's
+        typename CONFIG_T::exp_table_t exp_res[data_T::size];
+        #pragma HLS ARRAY_PARTITION variable=exp_res complete
+        typename CONFIG_T::exp_table_t exp_sum(0);
+        for(unsigned j = 0; j < data_T::size; j++){
+            #pragma HLS UNROLL
+            unsigned x = softmax_idx_from_real_val<typename data_T::value_type, CONFIG_T>(d_xi_xmax[j]);
+            exp_res[j] = exp_table[x];
+        }
 
-    // Explicitly sum the results with an adder tree.
-    // Rounding & Saturation mode, which improve accuracy, prevent Vivado from expression balancing
-    Op_add<typename CONFIG_T::exp_table_t> op_add;
-    exp_sum = reduce<typename CONFIG_T::exp_table_t, CONFIG_T::n_in, Op_add<typename CONFIG_T::exp_table_t>>(exp_res, op_add);
+        // Explicitly sum the results with an adder tree.
+        // Rounding & Saturation mode, which improve accuracy, prevent Vivado from expression balancing
+        Op_add<typename CONFIG_T::exp_table_t> op_add;
+        exp_sum = reduce<typename CONFIG_T::exp_table_t, data_T::size, Op_add<typename CONFIG_T::exp_table_t>>(exp_res, op_add);
 
-    typename CONFIG_T::inv_table_t inv_exp_sum = invert_table[softmax_idx_from_real_val<typename CONFIG_T::exp_table_t,CONFIG_T>(exp_sum)];
-    SoftmaxInvLoop: for(unsigned i = 0; i < CONFIG_T::n_in / res_T::size; i++){
-        #pragma HLS PIPELINE II=ii
+        typename CONFIG_T::inv_table_t inv_exp_sum = invert_table[softmax_idx_from_real_val<typename CONFIG_T::exp_table_t,CONFIG_T>(exp_sum)];
 
         res_T out_pack;
         #pragma HLS DATA_PACK variable=out_pack
         SoftmaxInvPackLoop: for(unsigned j = 0; j < res_T::size; j++){
             #pragma HLS UNROLL
             #pragma HLS ALLOCATION instances=mul limit=multiplier_limit operation
-            out_pack[i * res_T::size + j] = exp_res[i * res_T::size + j] * inv_exp_sum;
+            out_pack[j] = exp_res[j] * inv_exp_sum;
         }
         res.write(out_pack);
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
 void softmax_legacy(hls::stream<data_T> &data, hls::stream<res_T> &res) {
@@ -271,67 +263,65 @@
     if (!initialized) {
         init_exp_table_legacy<CONFIG_T, CONFIG_T::table_size>(exp_table);
         init_invert_table_legacy<CONFIG_T, CONFIG_T::table_size>(invert_table);
         initialized = true;
     }
 
     // Index into the lookup table based on data for exponentials
-    typename CONFIG_T::table_t exp_res[CONFIG_T::n_in];
+    typename CONFIG_T::table_t exp_res[data_T::size];
     typename CONFIG_T::table_t exp_diff_res;
-    typename data_T::value_type data_cache[CONFIG_T::n_in];
+    typename data_T::value_type data_cache[data_T::size];
 
-    SoftmaxInitLoop: for(unsigned i = 0; i < CONFIG_T::n_in / data_T::size; i++) {
+    SoftmaxInitLoop: for(unsigned s = 0; s < CONFIG_T::n_in / data_T::size; s++) {
         #pragma HLS PIPELINE
         data_T in_pack = data.read();
         SoftmaxInitPackLoop: for(unsigned j = 0; j < data_T::size; j++) {
             #pragma HLS UNROLL
-            data_cache[i * data_T::size + j] = in_pack[j];
-            exp_res[i * data_T::size + j] = 0;
+            data_cache[j] = in_pack[j];
+            exp_res[j] = 0;
         }
-    }
 
-    SoftmaxExpLoop: for (int i = 0; i < CONFIG_T::n_in; i++) {
-        #pragma HLS PIPELINE
-        SoftmaxExpInner: for (int j = 0; j < CONFIG_T::n_in; j++) {
+        SoftmaxExpLoop: for (int i = 0; i < data_T::size; i++) {
             #pragma HLS UNROLL
-            
-            if (i == j) {
-                exp_diff_res = 1;
-            } else {
-                int data_round = (data_cache[j] - data_cache[i]) * CONFIG_T::table_size / 16;
-                int index = data_round + 8 * CONFIG_T::table_size / 16;
-                if (index < 0) index = 0;
-                if (index > CONFIG_T::table_size - 1) index = CONFIG_T::table_size - 1;
-                exp_diff_res = exp_table[index];
+            SoftmaxExpInner: for (int j = 0; j < data_T::size; j++) {
+                #pragma HLS UNROLL
+
+                if (i == j) {
+                    exp_diff_res = 1;
+                } else {
+                    int data_round = (data_cache[j] - data_cache[i]) * CONFIG_T::table_size / 16;
+                    int index = data_round + 8 * CONFIG_T::table_size / 16;
+                    if (index < 0) index = 0;
+                    if (index > CONFIG_T::table_size - 1) index = CONFIG_T::table_size - 1;
+                    exp_diff_res = exp_table[index];
+                }
+
+                exp_res[i] += exp_diff_res;
             }
-            
-            exp_res[i] += exp_diff_res;
         }
-    }
-
-    SoftmaxInvLoop: for(unsigned i = 0; i < CONFIG_T::n_in / res_T::size; i++) {
-        #pragma HLS PIPELINE
 
         res_T out_pack;
         #pragma HLS DATA_PACK variable=out_pack
         SoftmaxInvPackLoop: for(unsigned j = 0; j < res_T::size; j++) {
             #pragma HLS UNROLL
-            
-            int exp_res_index = exp_res[i * res_T::size + j] * CONFIG_T::table_size / 64;
+
+            int exp_res_index = exp_res[j] * CONFIG_T::table_size / 64;
             if (exp_res_index < 0) exp_res_index = 0;
             if (exp_res_index > CONFIG_T::table_size - 1) exp_res_index = CONFIG_T::table_size - 1;
-            
-            out_pack[i * res_T::size + j] = (typename res_T::value_type) invert_table[exp_res_index];
+
+            out_pack[j] = (typename res_T::value_type) invert_table[exp_res_index];
         }
         res.write(out_pack);
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
 void softmax(hls::stream<data_T> &data, hls::stream<res_T> &res){
+    assert(CONFIG_T::axis == -1);
+
     switch(CONFIG_T::implementation){
     case softmax_implementation::latency:
         softmax_latency<data_T, res_T, CONFIG_T>(data, res);
         break;
     case softmax_implementation::stable:
         softmax_stable<data_T, res_T, CONFIG_T>(data, res);
         break;
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_array.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_array.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 #ifndef NNET_ARRAY_H_
 #define NNET_ARRAY_H_
 
 #include <math.h>
 
 namespace nnet {
 
-struct transpose3d_config {
+struct transpose_config {
     static const unsigned height = 10;
     static const unsigned width = 10;
     static const unsigned depth = 10;
-    static const unsigned perm[3];
+    static constexpr unsigned perm[3] = {2, 0, 1};
 };
 
 template<class data_T, typename CONFIG_T>
+void transpose_2d(
+    data_T data[CONFIG_T::height * CONFIG_T::width],
+    data_T data_t[CONFIG_T::height * CONFIG_T::width]
+) {
+    #pragma HLS PIPELINE
+
+    for (int i = 0; i < CONFIG_T::height; i++) {
+        for (int j = 0; j < CONFIG_T::width; j++) {
+            data_t[j * CONFIG_T::height + i] = data[i * CONFIG_T::width + j];
+        }
+    }
+}
+
+template<class data_T, typename CONFIG_T>
 void transpose_3d(
     data_T data[CONFIG_T::depth * CONFIG_T::height * CONFIG_T::width],
     data_T data_t[CONFIG_T::depth * CONFIG_T::height * CONFIG_T::width]
 ) {
     unsigned dims[3] = { CONFIG_T::depth, CONFIG_T::height, CONFIG_T::width };
     unsigned dims_t[3];
     dims_t[0] = dims[CONFIG_T::perm[0]];
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm.h`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
 
         // #pragma HLS ARRAY_PARTITION variable=weights complete // remove this line for now, it breaks compression sometimes
         #pragma HLS ARRAY_PARTITION variable=scale complete
         #pragma HLS ARRAY_PARTITION variable=bias complete
 
         int multiplier_limit  = ceil(float(CONFIG_T::n_in) / float(CONFIG_T::reuse_factor));
-        #pragma HLS ALLOCATION instances=mul limit=multiplier_limit operation
+        CONFIG_T::template product<data_T, typename CONFIG_T::scale_t, res_T>::limit(multiplier_limit);
 
     } else if (CONFIG_T::io_type == io_serial) {
         #pragma HLS ARRAY_RESHAPE variable=scale complete dim=1
         #pragma HLS ARRAY_RESHAPE variable=bias complete dim=1
         #pragma HLS DATAFLOW
     }
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_batchnorm_stream.h`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     typename CONFIG_T::bias_t  bias[CONFIG_T::n_in]
 ) {
     #pragma HLS ARRAY_PARTITION variable=scale complete
     #pragma HLS ARRAY_PARTITION variable=bias complete
 
     constexpr unsigned multiplier_limit = DIV_ROUNDUP(CONFIG_T::n_in, CONFIG_T::reuse_factor);
     constexpr unsigned ii = CONFIG_T::n_in / multiplier_limit;
-    #pragma HLS ALLOCATION instances=mul limit=multiplier_limit operation
+    CONFIG_T::template product<typename data_T::value_type, typename CONFIG_T::scale_t, typename res_T::value_type>::limit(multiplier_limit);
 
     BatchNormLoop: for (int i = 0; i < CONFIG_T::n_in / data_T::size; i++) {
         #pragma HLS PIPELINE II=ii
 
         data_T in_data = data.read();
         res_T out_data;
         #pragma HLS DATA_PACK variable=out_data
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_common.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_common.h`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #define NNET_COMMON_H_
 
 #include "ap_fixed.h"
 
 // This is a substitute for "ceil(n/(float)d)".
 #define DIV_ROUNDUP(n,d) ((n + d - 1) / d)
 #define MIN(n,d) (n > d ? d : n)
+#define MAX(n,d) (n > d ? n : d)
 
 namespace nnet {
 
 // Common type definitions
 enum io_type {io_parallel = 0, io_serial, io_stream};
 enum strategy { latency, resource };
 
@@ -37,35 +38,26 @@
   * For use in scenarios where Vivado cannot expression balance
   * Reduces an array of inputs to a single value using the template binary operator 'Op',
   * for example summing all elements with Op_add, or finding the maximum with Op_max
   * Use only when the input array is fully unrolled. Or, slice out a fully unrolled section
   * before applying and accumulate the result over the rolled dimension.
   * --- */
  template<class T, int N, class Op>
- T reduce(T* x, Op op){
-	static constexpr int leftN = pow2(floorlog2(N - 1)) > 0 ? pow2(floorlog2(N - 1)) : 0;
-	static constexpr int rightN = N - leftN > 0 ? N - leftN : 0;
-	if(N == 1){
-		return x[0];
-	}else if(N == 2){
-		return op(x[0],x[1]);
-	}else{
-		T left[leftN];
-		T right[rightN];
-		#pragma HLS array_partition variable=left complete
-		#pragma HLS array_partition variable=right complete
-		ReduceLeft: for(int i = 0; i < leftN; i++){
-			left[i] = x[i];
-		}
-		ReduceRight: for(int i = 0; i < rightN; i++){
-			right[i] = x[i+leftN];
-		}
-		return op(reduce<T,leftN,Op>(left, op), reduce<T,rightN,Op>(right, op));
-	}
- }
+ T reduce(const T* x, Op op)
+ {
+     static constexpr int leftN = pow2(floorlog2(N - 1)) > 0 ? pow2(floorlog2(N - 1)) : 0;
+     static constexpr int rightN = N - leftN > 0 ? N - leftN : 0;
+     if (N == 1){
+         return x[0];
+     }
+     if (N == 2){
+         return op(x[0],x[1]);
+     }
+     return op(reduce<T,leftN,Op>(x, op), reduce<T,rightN,Op>(x+leftN, op));
+ } 
 
  template<class T>
  class Op_add{
  public:
 	 T operator()(T a, T b){
 		 return a + b;
 	 }
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d.h`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 template<class data_T, class res_T, typename CONFIG_T>
 void conv_1d_cl(
     data_T data[CONFIG_T::in_width * CONFIG_T::n_chan],
     res_T  res[CONFIG_T::out_width * CONFIG_T::n_filt],
     typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
 {
-    if (CONFIG_T::strategy == latency) {
+    if (CONFIG_T::strategy == nnet::latency) {
         conv_1d_latency_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     } else {
         conv_1d_resource_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     }
 }
 
 }//end namespace
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_latency.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_latency.h`

 * *Files 26% similar despite different names*

```diff
@@ -114,9 +114,82 @@
     for(int ii = 0; ii < CONFIG_T::out_width; ii++) {
         for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
             res[ii * CONFIG_T::n_filt + ff] = (res_T)(acc[ii][ff]);
         }
     }
 }
 
+template<class data_T, class res_T, typename CONFIG_T>
+void pointwise_conv_1d_cl(
+    data_T data[CONFIG_T::in_width * CONFIG_T::n_chan],
+    res_T  res[CONFIG_T::out_width * CONFIG_T::n_filt],
+    typename CONFIG_T::weight_t weights[CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
+{
+    assert(CONFIG_T::filt_width == 1);
+
+    typename CONFIG_T::accum_t mult[CONFIG_T::out_width * CONFIG_T::n_filt * CONFIG_T::n_chan];
+    typename CONFIG_T::accum_t acc[CONFIG_T::out_width][CONFIG_T::n_filt];
+
+    #pragma HLS ARRAY_PARTITION variable=mult complete dim=0
+    #pragma HLS ARRAY_PARTITION variable=acc complete dim=0
+
+    // Use a function_instantiate in case it helps to explicitly optimize unchanging weights/biases
+    #pragma HLS function_instantiate variable=weights,biases
+
+    // Parallel mode
+    #pragma HLS PIPELINE
+    #pragma HLS ARRAY_PARTITION variable=biases complete dim=0
+
+    // Limit multipliers to control parallelization
+    const int multiplier_limit = compute_multiplier_limit<CONFIG_T>(weights);
+    #pragma HLS ALLOCATION instances=mul limit=multiplier_limit operation
+
+    // Convolve, saving all multiplication results to accumulate later
+    ConvOut: for(int ii = 0; ii < CONFIG_T::out_width; ii++) {
+        ConvFilt: for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+            ConvChan: for(int cc = 0; cc < CONFIG_T::n_chan; cc++) {
+                int index_mult   = ii*CONFIG_T::n_filt*CONFIG_T::n_chan + ff*CONFIG_T::n_chan + cc;
+                int index_weight = cc*CONFIG_T::n_filt + ff;
+                int index_data   = (ii*CONFIG_T::stride_width-CONFIG_T::pad_left) * CONFIG_T::n_chan + cc;
+
+                if((ii*CONFIG_T::stride_width) < CONFIG_T::pad_left || (ii*CONFIG_T::stride_width) >= (CONFIG_T::pad_left + CONFIG_T::in_width)){
+                    mult[index_mult] = 0;
+                }
+                else {
+                    mult[index_mult] = data[index_data] * weights[index_weight];
+                }
+            }//end channel loop
+        }//end filter loop
+    }//end output loop
+
+
+    // Initialize accumulator with input biases
+    for(int ii = 0; ii < CONFIG_T::out_width; ii++) {
+        for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+            acc[ii][ff]=biases[ff];
+        }
+    }
+
+
+    // Accumulate multiplication result
+    AccumOut: for(int ii = 0; ii < CONFIG_T::out_width; ii++) {
+        AccumFilt: for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+            //Do "dot product" sum within filter and sum over channels
+            AccumChan: for(int cc = 0; cc < CONFIG_T::n_chan; cc++) {
+                int index_mult = ii*CONFIG_T::n_filt*CONFIG_T::n_chan + ff*CONFIG_T::n_chan + cc;
+                acc[ii][ff] += mult[index_mult];
+            }//end channel loop
+        }//end filter loop
+    }//end output loop
+
+
+    // Cast to "res_t" type
+    for(int ii = 0; ii < CONFIG_T::out_width; ii++) {
+        for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+            res[ii * CONFIG_T::n_filt + ff] = (res_T)(acc[ii][ff]);
+        }
+    }
+}
+
 }
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_resource.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_resource.h`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt]
 )
 {
     data_T data_conv[CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::out_width];
     data_T data_col[CONFIG_T::filt_width * CONFIG_T::n_chan];
     res_T res_col[CONFIG_T::n_filt];
-    
+
     //#pragma HLS ARRAY_PARTITION variable=data_conv complete
     #pragma HLS ARRAY_PARTITION variable=data_col complete
     #pragma HLS ARRAY_PARTITION variable=res_col complete
 
     im2col_1d<data_T, CONFIG_T>(data, data_conv);
 
     for (int i = 0; i < CONFIG_T::out_width; i++) {
@@ -138,25 +138,25 @@
         }
     }
 }
 
 template<class data_T, typename CONFIG_T>
 void im2col_1d_cl(data_T data[CONFIG_T::in_width * CONFIG_T::n_chan], data_T data_col[CONFIG_T::filt_width * CONFIG_T::n_chan], const int col) {
     int index = 0;
-    ChannelLoop:
-    for (int channel = CONFIG_T::n_chan; channel--; data++) {
-		#pragma HLS UNROLL
-        KernelLoop:
-        for (int kernel_col = 0; kernel_col < CONFIG_T::filt_width; kernel_col++) {
-            int input_col = -CONFIG_T::pad_left + kernel_col * CONFIG_T::dilation + col * CONFIG_T::stride_width;
-            if (input_col >= 0 && input_col < CONFIG_T::in_width) {
-                //*(data_col++) = data[input_col * CONFIG_T::n_chan];
-                data_col[index] = data[input_col * CONFIG_T::n_chan];
+    KernelLoop:
+    for (int kernel_col = 0; kernel_col < CONFIG_T::filt_width; kernel_col++) {
+        #pragma HLS UNROLL
+
+        ChannelLoop:
+        for (int channel = 0; channel < CONFIG_T::n_chan; channel++) {
+            int index_data = (col*CONFIG_T::stride_width+kernel_col-CONFIG_T::pad_left) * CONFIG_T::n_chan + channel;
+
+            if (index_data >= 0 && index_data < CONFIG_T::in_width*CONFIG_T::n_chan) {
+                data_col[index] = data[index_data];
             } else {
-                //*(data_col++) = 0;
                 data_col[index] = 0;
             }
             index++;
         }
     }
 }
 
@@ -187,14 +187,13 @@
     ColLoop:
     for (int i = 0; i < CONFIG_T::out_width; i++) {
         #pragma HLS PIPELINE
         im2col_1d_cl<data_T, CONFIG_T>(data, data_col, i);
         dense_resource<data_T, res_T, typename CONFIG_T::mult_config>(data_col, res_col, weights, biases);
         for (int j = 0; j < CONFIG_T::n_filt; j++) {
             res[i * CONFIG_T::n_filt + j] = res_col[j];
-            //res[j * CONFIG_T::out_width + i] = res_col[j]; // Transposed order
         }
     }
 }
 
 }
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_stream.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,70 @@
-#ifndef NNET_CONV1D_STREAM_H_
-#define NNET_CONV1D_STREAM_H_
+#ifndef NNET_DENSE_STREAM_H_
+#define NNET_DENSE_STREAM_H_
 
 #include "nnet_common.h"
-#include "nnet_conv_stream.h"
+#include "nnet_types.h"
 #include "hls_stream.h"
+#include <math.h>
+#include <assert.h>
 
 namespace nnet {
 
-template<class data_T, typename CONFIG_T>
-void compute_scaled_indices_1d(
-    const unsigned w_idx,
-    ap_uint<CONFIG_T::filt_width> *pixel_idx
+template<class data_T, class res_T, typename CONFIG_T>
+void dense_wrapper(
+    data_T data[CONFIG_T::n_in],
+    res_T  res[CONFIG_T::n_out],
+    typename CONFIG_T::weight_t weights[CONFIG_T::n_in*CONFIG_T::n_out],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_out]
 ) {
-    unsigned wp_idx = w_idx * (data_T::size / CONFIG_T::n_chan);
-
-    ComputeIndex: for (unsigned p = 0; p < data_T::size / CONFIG_T::n_chan; p++) {
-        #pragma HLS UNROLL
-
-        unsigned sw_idx = scale_index<CONFIG_T::filt_width, CONFIG_T::stride_width, CONFIG_T::in_width>(wp_idx + p);
-        pixel_idx[p] = CONFIG_T::pixels[sw_idx];
+    #pragma HLS INLINE region
+    if (CONFIG_T::strategy == nnet::latency) {
+        #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
+        dense_latency<data_T, res_T, CONFIG_T>(data, res, weights, biases);
+    } else {
+        dense_resource<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
-void conv_1d_cl(
-    hls::stream<data_T> &data,
-    hls::stream<res_T>  &res,
-    typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
-    typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
+void dense(
+    hls::stream<data_T> &data_stream,
+    hls::stream<res_T>  &res_stream,
+    typename CONFIG_T::weight_t weights[CONFIG_T::n_in*CONFIG_T::n_out],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_out])
 {
-    assert(CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
-    assert(CONFIG_T::stride_width <= CONFIG_T::filt_width);
+    typename data_T::value_type data[CONFIG_T::n_in];
+    #pragma HLS ARRAY_PARTITION variable=data complete
+
+    typename res_T::value_type res[CONFIG_T::n_out];
+    #pragma HLS ARRAY_PARTITION variable=res complete
 
-    hls::stream<typename data_T::value_type> data_window[CONFIG_T::filt_width * CONFIG_T::n_chan];
-    const int win_depth = CONFIG_T::out_width;
-    for (unsigned i_out = 0; i_out < CONFIG_T::filt_width * CONFIG_T::n_chan; i_out++) {
-        #pragma HLS STREAM variable=data_window[i_out] depth=win_depth
+    DataPrepare: for(int i_in = 0; i_in < CONFIG_T::n_in / data_T::size; i_in++) {
+        if (CONFIG_T::n_in / data_T::size > 1) {
+            #pragma HLS PIPELINE
+        }
+        data_T data_pack = data_stream.read();
+        DataPack: for (int i_pack = 0; i_pack < data_T::size; i_pack++) {
+            #pragma HLS UNROLL
+            data[i_in * data_T::size + i_pack] = data_pack[i_pack];
+        }
     }
 
-    #pragma HLS ARRAY_PARTITION variable=CONFIG_T::pixels complete
+    dense_wrapper<typename data_T::value_type, typename res_T::value_type, CONFIG_T>(data, res, weights, biases);
 
-    res_T res_pack;
-    #pragma HLS DATA_PACK variable=res_pack
-    unsigned outputs_ready = 0;
-
-    ap_uint<CONFIG_T::filt_width> pixel_idx[data_T::size / CONFIG_T::n_chan];
-    #pragma HLS ARRAY_PARTITION variable=pixel_idx complete
-
-    ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (data_T::size / CONFIG_T::n_chan); i_iw++) {
-        #pragma HLS LOOP_FLATTEN
-        if (CONFIG_T::strategy == nnet::latency && data_T::size / CONFIG_T::n_chan == 1) {
-            #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
+    ResWrite: for(unsigned i_out = 0; i_out < CONFIG_T::n_out / res_T::size; i_out++) {
+        if (CONFIG_T::n_out / res_T::size > 1) {
+            #pragma HLS PIPELINE
         }
-        compute_scaled_indices_1d<data_T, CONFIG_T>(i_iw, pixel_idx);
-        compute_output<data_T, res_T, CONFIG_T>(data.read(), data_window, res, res_pack, outputs_ready, weights, biases, pixel_idx);
+        res_T res_pack;
+        #pragma HLS DATA_PACK variable=res_pack
+        ResPack: for (int i_pack = 0; i_pack < res_T::size; i_pack++) {
+            #pragma HLS UNROLL
+            res_pack[i_pack] = res[i_out * res_T::size + i_pack];
+        }
+        res_stream.write(res_pack);
     }
 }
 
 }
+
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d.h`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,29 @@
 template<class data_T, class res_T, typename CONFIG_T>
 void conv_2d_cf(
     data_T data[CONFIG_T::in_height * CONFIG_T::in_width * CONFIG_T::n_chan],
     res_T  res[CONFIG_T::out_height * CONFIG_T::out_width * CONFIG_T::n_filt],
     typename CONFIG_T::weight_t weights[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
 {
-    if (CONFIG_T::strategy == latency) {
+    if (CONFIG_T::strategy == nnet::latency) {
         conv_2d_latency_cf<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     } else {
         conv_2d_resource_cf<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
 void conv_2d_cl(
     data_T data[CONFIG_T::in_height * CONFIG_T::in_width * CONFIG_T::n_chan],
     res_T  res[CONFIG_T::out_height * CONFIG_T::out_width * CONFIG_T::n_filt],
     typename CONFIG_T::weight_t weights[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
 {
-    if (CONFIG_T::strategy == latency) {
+    if (CONFIG_T::strategy == nnet::latency) {
         conv_2d_latency_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     } else {
         conv_2d_resource_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     }
 }
 
 }//end namespace
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_latency.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_latency.h`

 * *Files 17% similar despite different names*

```diff
@@ -277,9 +277,109 @@
                 res[index] = (res_T)(acc[index]);
             }
         }
     }
 
 }//end conv2d
 
+template<class data_T, class res_T, typename CONFIG_T>
+void pointwise_conv_2d_cl(
+    data_T data[CONFIG_T::in_height*CONFIG_T::in_width*CONFIG_T::n_chan],
+    res_T  res[CONFIG_T::out_height*CONFIG_T::out_width*CONFIG_T::n_filt],
+    typename CONFIG_T::weight_t weights[CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
+{
+
+    typename CONFIG_T::accum_t mult[CONFIG_T::out_height * CONFIG_T::out_width * CONFIG_T::n_filt * CONFIG_T::n_chan];
+    typename CONFIG_T::accum_t acc[CONFIG_T::out_height * CONFIG_T::out_width * CONFIG_T::n_filt];
+
+    #pragma HLS ARRAY_PARTITION variable=mult complete dim=0
+    #pragma HLS ARRAY_PARTITION variable=acc complete dim=0
+
+    // Use a function_instantiate in case it helps to explicitly optimize unchanging weights/biases
+    #pragma HLS function_instantiate variable=weights,biases
+
+    // Parallel mode
+    #pragma HLS PIPELINE
+    #pragma HLS ARRAY_PARTITION variable=biases complete dim=0
+
+    // Limit multipliers to control parallelization
+    const int multiplier_limit = compute_multiplier_limit_conv2d<CONFIG_T>(weights);
+    #pragma HLS ALLOCATION instances=mul limit=multiplier_limit operation
+
+    // Convolve, saving all multiplication results to accumulate later
+    ConvOutHeight: for(int oh = 0; oh < CONFIG_T::out_height; oh++) {
+        ConvOutWidth: for(int ow = 0; ow < CONFIG_T::out_width; ow++) {
+            ConvFilt: for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+                ConvChan: for(int cc = 0; cc < CONFIG_T::n_chan; cc++) {
+
+                    int index_mult = oh*CONFIG_T::out_width*CONFIG_T::n_filt*CONFIG_T::n_chan
+                                   + ow*CONFIG_T::n_filt*CONFIG_T::n_chan
+                                   + ff*CONFIG_T::n_chan
+                                   + cc;
+
+                    int index_weight = cc*CONFIG_T::n_filt + ff;
+
+                    if ((oh*CONFIG_T::stride_height) < CONFIG_T::pad_top
+                    || (oh*CONFIG_T::stride_height) >= (CONFIG_T::pad_top+CONFIG_T::in_height)
+                    || (ow*CONFIG_T::stride_width) < CONFIG_T::pad_left
+                    || (ow*CONFIG_T::stride_width) >= (CONFIG_T::pad_left+CONFIG_T::in_width)) {
+                        mult[index_mult] = 0;
+                    } else {
+                        int index_data = (oh*CONFIG_T::stride_height-CONFIG_T::pad_top)*CONFIG_T::in_width*CONFIG_T::n_chan
+                                       + (ow*CONFIG_T::stride_width-CONFIG_T::pad_left)*CONFIG_T::n_chan
+                                       + cc;
+                        mult[index_mult] = data[index_data] * weights[index_weight];
+                    }
+
+                }
+            }
+        }
+    }
+
+
+    // Initialize accumulator with input biases
+    for(int oh = 0; oh < CONFIG_T::out_height; oh++) {
+        for(int ow = 0; ow < CONFIG_T::out_width; ow++) {
+            for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+                acc[oh*CONFIG_T::out_width*CONFIG_T::n_filt + ow*CONFIG_T::n_filt + ff]=biases[ff];
+            }
+        }
+    }
+
+
+    // Accumulate multiplication result
+    AccumOutHeight: for(int oh = 0; oh < CONFIG_T::out_height; oh++) {
+        AccumOutWidth: for(int ow = 0; ow < CONFIG_T::out_width; ow++) {
+            AccumFilt: for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+                //Do "dot product" sum within filter and sum over channels
+                AccumChan: for(int cc = 0; cc < CONFIG_T::n_chan; cc++) {
+
+                    int index_mult = oh*CONFIG_T::out_width*CONFIG_T::n_filt*CONFIG_T::n_chan
+                                    + ow*CONFIG_T::n_filt*CONFIG_T::n_chan
+                                    + ff*CONFIG_T::n_chan
+                                    + cc;
+                    int index_acc = oh*CONFIG_T::out_width*CONFIG_T::n_filt
+                                    + ow*CONFIG_T::n_filt
+                                    + ff;
+
+                    acc[index_acc] += mult[index_mult];
+
+                }
+            }
+        }
+    }
+
+    // Cast to "res_t" type
+    for(int oh = 0; oh < CONFIG_T::out_height; oh++) {
+        for(int ow = 0; ow < CONFIG_T::out_width; ow++) {
+              for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+                int index = oh*CONFIG_T::out_width*CONFIG_T::n_filt + ow*CONFIG_T::n_filt + ff;
+                res[index] = (res_T)(acc[index]);
+            }
+        }
+    }
+
+}//end conv2d
+
 }
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_resource.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_resource.h`

 * *Files 2% similar despite different names*

```diff
@@ -150,28 +150,26 @@
 void im2col_2d_cl(
     data_T data[CONFIG_T::in_height * CONFIG_T::in_width * CONFIG_T::n_chan],
     data_T data_col[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan],
     const int row,
     const int col)
 {
     int index = 0;
-    for (int channel = CONFIG_T::n_chan; channel--; data++) {
+    for (int kernel_row = 0; kernel_row < CONFIG_T::filt_height; kernel_row++) {
         #pragma HLS UNROLL
-        for (int kernel_row = 0; kernel_row < CONFIG_T::filt_height; kernel_row++) {
-            int input_row = -CONFIG_T::pad_top + kernel_row * CONFIG_T::dilation_height + row * CONFIG_T::stride_height;
-            for (int kernel_col = 0; kernel_col < CONFIG_T::filt_width; kernel_col++) {
+        int input_row = -CONFIG_T::pad_top + kernel_row * CONFIG_T::dilation_height + row * CONFIG_T::stride_height;
+        for (int kernel_col = 0; kernel_col < CONFIG_T::filt_width; kernel_col++) {
+            for (int channel = 0; channel < CONFIG_T::n_chan; channel++) {
                 if (input_row < 0 || input_row >= CONFIG_T::in_height) {
                     data_col[index++] = 0;
                 } else {
                     int input_col = -CONFIG_T::pad_left + kernel_col * CONFIG_T::dilation_width + col * CONFIG_T::stride_width;
                     if (input_col >= 0 && input_col < CONFIG_T::in_width) {
-                        //*(data_col++) = data[input_row * CONFIG_T::in_width * CONFIG_T::n_chan + input_col * CONFIG_T::n_chan];
-                        data_col[index++] = data[input_row * CONFIG_T::in_width * CONFIG_T::n_chan + input_col * CONFIG_T::n_chan];
+                        data_col[index++] = data[input_row * CONFIG_T::in_width * CONFIG_T::n_chan + input_col * CONFIG_T::n_chan + channel];
                     } else {
-                        //*(data_col++) = 0;
                         data_col[index++] = 0;
                     }
                 }
             }
         }
     }
 }
@@ -205,15 +203,14 @@
         for (int j = 0; j < CONFIG_T::out_width; j++) {
             #pragma HLS PIPELINE
             im2col_2d_cl<data_T, CONFIG_T>(data, data_col, i, j);
             dense<data_T, res_T, typename CONFIG_T::mult_config>(data_col, res_col, weights, biases);
             FiltLoop:
             for (int k = 0; k < CONFIG_T::n_filt; k++) {
                 res[i * CONFIG_T::out_width * CONFIG_T::n_filt + j * CONFIG_T::n_filt + k] = res_col[k];
-                //res[k * CONFIG_T::out_height * CONFIG_T::out_width + i * CONFIG_T::out_width + j] = res_col[k]; // Transposed order
             }
         }
     }
 }
 
 }
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv1d_stream.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,96 @@
-#ifndef NNET_CONV2D_STREAM_H_
-#define NNET_CONV2D_STREAM_H_
+#ifndef NNET_CONV1D_STREAM_H_
+#define NNET_CONV1D_STREAM_H_
 
 #include "nnet_common.h"
 #include "nnet_conv_stream.h"
 #include "hls_stream.h"
 
 namespace nnet {
 
 template<class data_T, typename CONFIG_T>
-void compute_scaled_indices_2d(
-    const unsigned h_idx,
+void compute_scaled_indices_1d(
     const unsigned w_idx,
-    ap_uint<CONFIG_T::filt_height * CONFIG_T::filt_width> *pixel_idx
+    ap_uint<CONFIG_T::filt_width> *pixel_idx
 ) {
-    const unsigned sh_idx = scale_index<CONFIG_T::filt_height, CONFIG_T::stride_height, CONFIG_T::in_height>(h_idx);
     unsigned wp_idx = w_idx * (data_T::size / CONFIG_T::n_chan);
 
     ComputeIndex: for (unsigned p = 0; p < data_T::size / CONFIG_T::n_chan; p++) {
         #pragma HLS UNROLL
 
         unsigned sw_idx = scale_index<CONFIG_T::filt_width, CONFIG_T::stride_width, CONFIG_T::in_width>(wp_idx + p);
-        pixel_idx[p] = CONFIG_T::pixels[sh_idx * CONFIG_T::min_width + sw_idx];
+        pixel_idx[p] = CONFIG_T::pixels[sw_idx];
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
-void conv_2d_cl(
+void conv_1d_encoded_cl(
     hls::stream<data_T> &data,
     hls::stream<res_T>  &res,
-    typename CONFIG_T::weight_t weights[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
 {
-    assert(CONFIG_T::pad_top == 0 && CONFIG_T::pad_bottom == 0 && CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
-    assert(CONFIG_T::filt_height == CONFIG_T::filt_width);
-    assert(CONFIG_T::stride_height <= CONFIG_T::filt_height && CONFIG_T::stride_width <= CONFIG_T::filt_width);
-
-    hls::stream<typename data_T::value_type> data_window[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan];
-    const int win_depth = CONFIG_T::filt_height * CONFIG_T::out_width;
-    for (unsigned i_out = 0; i_out < CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan; i_out++) {
+    assert(CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
+
+    hls::stream<typename data_T::value_type> data_window[CONFIG_T::filt_width * CONFIG_T::n_chan];
+    const int win_depth = CONFIG_T::out_width;
+    for (unsigned i_out = 0; i_out < CONFIG_T::filt_width * CONFIG_T::n_chan; i_out++) {
         #pragma HLS STREAM variable=data_window[i_out] depth=win_depth
     }
 
     #pragma HLS ARRAY_PARTITION variable=CONFIG_T::pixels complete
 
     res_T res_pack;
     #pragma HLS DATA_PACK variable=res_pack
     unsigned outputs_ready = 0;
 
-    ap_uint<CONFIG_T::filt_height * CONFIG_T::filt_width> pixel_idx[data_T::size / CONFIG_T::n_chan];
+    ap_uint<CONFIG_T::filt_width> pixel_idx[data_T::size / CONFIG_T::n_chan];
     #pragma HLS ARRAY_PARTITION variable=pixel_idx complete
 
-    ReadInputHeight: for (unsigned i_ih = 0; i_ih < CONFIG_T::in_height; i_ih++) {
-        ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (data_T::size / CONFIG_T::n_chan); i_iw++) {
-            #pragma HLS LOOP_FLATTEN
-            if (CONFIG_T::strategy == nnet::latency && data_T::size / CONFIG_T::n_chan == 1) {
-                #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
-            }
-            compute_scaled_indices_2d<data_T, CONFIG_T>(i_ih, i_iw, pixel_idx);
-            compute_output<data_T, res_T, CONFIG_T>(data.read(), data_window, res, res_pack, outputs_ready, weights, biases, pixel_idx);
+    ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (data_T::size / CONFIG_T::n_chan); i_iw++) {
+        #pragma HLS LOOP_FLATTEN
+        if (CONFIG_T::strategy == nnet::latency && data_T::size / CONFIG_T::n_chan == 1) {
+            #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
+        }
+        compute_scaled_indices_1d<data_T, CONFIG_T>(i_iw, pixel_idx);
+        compute_output_encoded<data_T, res_T, CONFIG_T>(data.read(), data_window, res, res_pack, outputs_ready, weights, biases, pixel_idx);
+    }
+}
+
+template<class data_T, class res_T, typename CONFIG_T>
+void conv_1d_buffer_cl(
+    hls::stream<data_T> &data,
+    hls::stream<res_T>  &res,
+    typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
+{
+    assert(CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
+
+    ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width; i_iw++) {
+        #pragma HLS LOOP_FLATTEN
+        if (CONFIG_T::strategy == nnet::latency) {
+            #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
         }
+        compute_output_buffer_1d<data_T, res_T, CONFIG_T>(data.read(), res, weights, biases);
     }
 }
 
+template<class data_T, class res_T, typename CONFIG_T>
+void conv_1d_cl(
+    hls::stream<data_T> &data,
+    hls::stream<res_T>  &res,
+    typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
+{
+    #pragma HLS inline region
+    switch(CONFIG_T::implementation){
+        case conv_implementation::linebuffer:
+            conv_1d_buffer_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
+            break;
+        case conv_implementation::encoded:
+            conv_1d_encoded_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
+            break;
+    }  
+}
+
 }
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense.h`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 template<class data_T, class res_T, typename CONFIG_T>
 void dense(
     data_T    data[CONFIG_T::n_in],
     res_T     res[CONFIG_T::n_out],
     typename CONFIG_T::weight_t  weights[CONFIG_T::n_in*CONFIG_T::n_out],
     typename CONFIG_T::bias_t    biases[CONFIG_T::n_out])
 {
-    if (CONFIG_T::strategy == latency) {
+    #pragma HLS inline
+    if (CONFIG_T::strategy == nnet::latency) {
         dense_latency<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     } else {
         dense_resource<data_T, res_T, CONFIG_T>(data, res, weights, biases);
     }
 }
 
 }
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_compressed.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_compressed.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_latency.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_latency.h`

 * *Files 14% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         // #pragma HLS ARRAY_PARTITION variable=weights complete // remove this line for now, it breaks compression sometimes
         #pragma HLS ARRAY_PARTITION variable=biases complete
         #pragma HLS ARRAY_PARTITION variable=mult complete
         #pragma HLS ARRAY_PARTITION variable=acc complete
 
         int multiplier_limit  = ceil(float(CONFIG_T::n_in*CONFIG_T::n_out) / float(CONFIG_T::reuse_factor)) - floor(float(CONFIG_T::n_zeros) / float(CONFIG_T::reuse_factor));
-        #pragma HLS ALLOCATION instances=product limit=multiplier_limit function
+        CONFIG_T::template product<data_T, typename CONFIG_T::weight_t, typename CONFIG_T::accum_t>::limit(multiplier_limit);
 
     } else if (CONFIG_T::io_type == io_serial){
         // Only reduce cycle_factor if n_out is evenly divisible by reuse_factor
         // Otherwise, HLS wont be happy
         int cycle_factor = CONFIG_T::n_out / CONFIG_T::reuse_factor;
         int reused_cycle = DIV_ROUNDUP(CONFIG_T::n_out, CONFIG_T::reuse_factor);
         if (cycle_factor != reused_cycle) {
@@ -86,15 +86,15 @@
         if (CONFIG_T::io_type == io_serial){
             #pragma HLS PIPELINE
         }
         cache = data[ii];
         Product2: for(int jj = 0; jj < CONFIG_T::n_out; jj++) {
             if (CONFIG_T::io_type == io_serial) {
                 int multiplier_limit  = ceil(float(CONFIG_T::n_out) / float(CONFIG_T::reuse_factor));
-                #pragma HLS ALLOCATION instances=product limit=multiplier_limit function
+                CONFIG_T::template product<data_T, typename CONFIG_T::weight_t, typename CONFIG_T::accum_t>::limit(multiplier_limit);
             }
         int index = ii*CONFIG_T::n_out+jj;
         mult[index] = CONFIG_T::template product<data_T, typename CONFIG_T::weight_t, typename CONFIG_T::accum_t>::product(cache, weights[index]);
         }
     }
 
     // Initialize accumulator with input biases
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_resource.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_dense_resource.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_dense_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_padding_stream.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,82 @@
-#ifndef NNET_DENSE_STREAM_H_
-#define NNET_DENSE_STREAM_H_
+#ifndef NNET_PADDING_STREAM_H_
+#define NNET_PADDING_STREAM_H_
 
-#include "nnet_common.h"
-#include "nnet_types.h"
-#include "hls_stream.h"
 #include <math.h>
-#include <assert.h>
 
 namespace nnet {
 
+template<class res_T, typename CONFIG_T>
+void fill_zero(hls::stream<res_T> &res) {
+    #pragma HLS INLINE
+    res_T res_part;
+	for (int c = 0; c < CONFIG_T::n_chan; c++) {
+        #pragma HLS UNROLL
+	    res_part[c] = 0;
+    }
+    res.write(res_part);
+}
+
+template<class data_T, class res_T, typename CONFIG_T>
+void fill_data(hls::stream<data_T> &data, hls::stream<res_T> &res) {
+    #pragma HLS INLINE
+    data_T data_part = data.read();
+    res_T res_part;
+    for (int c = 0; c < CONFIG_T::n_chan; c++) {
+        #pragma HLS UNROLL
+        res_part[c] = data_part[c];
+    }
+    res.write(res_part);
+}
+
 template<class data_T, class res_T, typename CONFIG_T>
-void dense_wrapper(
-    data_T data[CONFIG_T::n_in],
-    res_T  res[CONFIG_T::n_out],
-    typename CONFIG_T::weight_t weights[CONFIG_T::n_in*CONFIG_T::n_out],
-    typename CONFIG_T::bias_t   biases[CONFIG_T::n_out]
+void zeropad1d_cl(
+    hls::stream<data_T> &data,
+    hls::stream<res_T>  &res
 ) {
-    #pragma HLS INLINE region
-    if (CONFIG_T::strategy == nnet::latency) {
-        #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
-        dense_latency<data_T, res_T, CONFIG_T>(data, res, weights, biases);
-    } else {
-        dense_resource<data_T, res_T, CONFIG_T>(data, res, weights, biases);
+    PadLeft: for (int i = 0; i < CONFIG_T::pad_left; i++) {
+        fill_zero<res_T, CONFIG_T>(res);
+    }
+
+    CopyMain: for (int i = 0; i < CONFIG_T::in_width; i++) {
+        fill_data<data_T, res_T, CONFIG_T>(data, res);
+    }
+
+    PadRight: for (int i = 0; i < CONFIG_T::pad_right; i++) {
+        fill_zero<res_T, CONFIG_T>(res);
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
-void dense(
-    hls::stream<data_T> &data_stream,
-    hls::stream<res_T>  &res_stream,
-    typename CONFIG_T::weight_t weights[CONFIG_T::n_in*CONFIG_T::n_out],
-    typename CONFIG_T::bias_t   biases[CONFIG_T::n_out])
-{
-    typename data_T::value_type data[CONFIG_T::n_in];
-    #pragma HLS ARRAY_PARTITION variable=data complete
-
-    typename res_T::value_type res[CONFIG_T::n_out];
-    #pragma HLS ARRAY_PARTITION variable=res complete
-
-    DataPrepare: for(int i_in = 0; i_in < CONFIG_T::n_in / data_T::size; i_in++) {
-        if (CONFIG_T::n_in / data_T::size > 1) {
-            #pragma HLS PIPELINE
-        }
-        data_T data_pack = data_stream.read();
-        DataPack: for (int i_pack = 0; i_pack < data_T::size; i_pack++) {
-            #pragma HLS UNROLL
-            data[i_in * data_T::size + i_pack] = data_pack[i_pack];
+void zeropad2d_cl(
+    hls::stream<data_T> &data,
+    hls::stream<res_T>  &res
+) {
+
+    PadTop: for (int i = 0; i < CONFIG_T::pad_top; i++) {
+        PadTopWidth: for (int j = 0; j < CONFIG_T::out_width; j++) {
+            fill_zero<res_T, CONFIG_T>(res);
         }
     }
 
-    dense_wrapper<typename data_T::value_type, typename res_T::value_type, CONFIG_T>(data, res, weights, biases);
-
-    ResWrite: for(unsigned i_out = 0; i_out < CONFIG_T::n_out / res_T::size; i_out++) {
-        if (CONFIG_T::n_out / res_T::size > 1) {
-            #pragma HLS PIPELINE
+    PadMain: for (int i = 0; i < CONFIG_T::in_height; i++) {
+        PadLeft: for (int j = 0; j < CONFIG_T::pad_left; j++) {
+            fill_zero<res_T, CONFIG_T>(res);
         }
-        res_T res_pack;
-        #pragma HLS DATA_PACK variable=res_pack
-        ResPack: for (int i_pack = 0; i_pack < res_T::size; i_pack++) {
-            #pragma HLS UNROLL
-            res_pack[i_pack] = res[i_out * res_T::size + i_pack];
+        CopyMain: for (int j = 0; j < CONFIG_T::in_width; j++) {
+            fill_data<data_T, res_T, CONFIG_T>(data, res);
+        }
+        PadRight: for (int j = 0; j < CONFIG_T::pad_right; j++) {
+            fill_zero<res_T, CONFIG_T>(res);
+        }
+    }
+
+    PadBottom: for (int i = 0; i < CONFIG_T::pad_bottom; i++) {
+        PadBottomWidth: for (int j = 0; j < CONFIG_T::out_width; j++) {
+            fill_zero<res_T, CONFIG_T>(res);
         }
-        res_stream.write(res_pack);
     }
 }
 
 }
 
-#endif
+#endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_garnet.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_garnet.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_helpers.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_helpers.h`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 #define NNET_HELPERS_H
 
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
 #include <fstream>
 #include <algorithm>
+#include <vector>
 #include <map>
+#include <iostream>
 #include "hls_stream.h"
 
 namespace nnet {
 
 #ifndef __SYNTHESIS__
 
 #ifndef WEIGHTS_DIR
@@ -294,14 +296,29 @@
         if (i_pack == dst_T::size) {
             i_pack = 0;
             dst.write(dst_pack);
         }
     }
 }
 
+template<class src_T, class dst_T, size_t OFFSET, size_t SIZE>
+void copy_data_axi(std::vector<src_T> src, dst_T dst[SIZE]) {
+    for(auto i = 0; i < SIZE; i++)
+    	if(i == SIZE - 1)
+    	{
+    		dst[i].data = src[i];
+    		dst[i].last = 1;
+    	}
+    	else
+    	{
+    		dst[i].data = src[i];
+    		dst[i].last = 0;
+    	}
+}
+
 template<class res_T, size_t SIZE>
 void print_result(res_T result[SIZE], std::ostream &out, bool keep = false) {
     for(int i = 0; i < SIZE; i++) {
         out << result[i] << " ";
     }
     out << std::endl;
 }
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_image.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_image.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_image_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_image_stream.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_merge.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_merge.h`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 //    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 //
 
 #ifndef NNET_MERGE_H_
 #define NNET_MERGE_H_
 
 #include "nnet_common.h"
-#include "nnet_dense.h"
+#include "nnet_mult.h"
 #include "hls_stream.h"
 #include <math.h>
 
 namespace nnet {
 
 struct merge_config
 {
@@ -33,14 +33,17 @@
 };
 
 struct dot_config {
     static const unsigned n_in = 10;
     static const unsigned n_out = 1;
     static const unsigned reuse_factor = 1;
     typedef float accum_t;
+    // Product function to use
+    template<class x_T, class y_T, class res_T>
+    using product = nnet::product::mult<x_T, y_T, res_T>;
 };
 
 struct concat_config {
     static const unsigned n_elem1_0 = 10;
     static const unsigned n_elem1_1 = 10;
     static const unsigned n_elem1_2 = 10;
     static const unsigned n_elem2_0 = 10;
@@ -49,142 +52,139 @@
 
     static const unsigned axis = -1;
 };
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void add(
     input1_T data1[CONFIG_T::n_elem],
-	input2_T data2[CONFIG_T::n_elem],
+    input2_T data2[CONFIG_T::n_elem],
     res_T res[CONFIG_T::n_elem])
 {
     for (int ii=0; ii<CONFIG_T::n_elem; ii++) {
         res[ii] = data1[ii] + data2[ii];
     }
 }
 
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void subtract(
     input1_T data1[CONFIG_T::n_elem],
-	input2_T data2[CONFIG_T::n_elem],
+    input2_T data2[CONFIG_T::n_elem],
     res_T res[CONFIG_T::n_elem])
 {
     for (int ii=0; ii<CONFIG_T::n_elem; ii++) {
         res[ii] = data1[ii] - data2[ii];
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void multiply(
     input1_T data1[CONFIG_T::n_elem],
-	input2_T data2[CONFIG_T::n_elem],
+    input2_T data2[CONFIG_T::n_elem],
     res_T res[CONFIG_T::n_elem])
 {
     for (int ii=0; ii<CONFIG_T::n_elem; ii++) {
         res[ii] = data1[ii] * data2[ii];
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void average(
     input1_T data1[CONFIG_T::n_elem],
-	input2_T data2[CONFIG_T::n_elem],
+    input2_T data2[CONFIG_T::n_elem],
     res_T res[CONFIG_T::n_elem])
 {
     for (int ii=0; ii<CONFIG_T::n_elem; ii++) {
-        res[ii] = data1[ii] * data2[ii] / (res_T) 2;
+        res[ii] = (data1[ii] + data2[ii]) / (res_T) 2;
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void maximum(
     input1_T data1[CONFIG_T::n_elem],
-	input2_T data2[CONFIG_T::n_elem],
+    input2_T data2[CONFIG_T::n_elem],
     res_T res[CONFIG_T::n_elem])
 {
     for (int ii=0; ii<CONFIG_T::n_elem; ii++) {
         res[ii] = (data1[ii] > data2[ii]) ? data1[ii] : data2[ii];
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void minimum(
     input1_T data1[CONFIG_T::n_elem],
-	input2_T data2[CONFIG_T::n_elem],
+    input2_T data2[CONFIG_T::n_elem],
     res_T res[CONFIG_T::n_elem])
 {
     for (int ii=0; ii<CONFIG_T::n_elem; ii++) {
         res[ii] = (data1[ii] < data2[ii]) ? data1[ii] : data2[ii];
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void dot1d(
     input1_T data1[CONFIG_T::n_in],
-	input2_T data2[CONFIG_T::n_in],
+    input2_T data2[CONFIG_T::n_in],
     res_T res[CONFIG_T::n_out])
 {
     #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
 
     constexpr unsigned multiplier_limit = DIV_ROUNDUP(CONFIG_T::n_in, CONFIG_T::reuse_factor);
-    #pragma HLS ALLOCATION instances=product limit=multiplier_limit function
+    CONFIG_T::template product<input1_T, input2_T, typename CONFIG_T::accum_t>::limit(multiplier_limit);
 
     typename CONFIG_T::accum_t mult[CONFIG_T::n_in];
     #pragma HLS ARRAY_PARTITION variable=mult complete
     typename CONFIG_T::accum_t acc = 0;
 
     Product: for(int i_mult=0; i_mult < CONFIG_T::n_in; i_mult++) {
         #pragma HLS UNROLL
-        mult[i_mult] = product<input1_T, input2_T, typename CONFIG_T::accum_t>(data1[i_mult], data2[i_mult]);
+        mult[i_mult] = CONFIG_T::template product<input1_T, input2_T, typename CONFIG_T::accum_t>::product(data1[i_mult], data2[i_mult]);
     }
 
     Accum: for(int i_acc = 0; i_acc < CONFIG_T::n_in; i_acc++) {
         #pragma HLS UNROLL
         acc += mult[i_acc];
     }
 
-    Result: for(int i_res = 0; i_res < CONFIG_T::n_out; i_res++) {
-        #pragma HLS_UNROLL
-        res[i_res] = cast<input1_T, res_T, CONFIG_T>(acc);
-    }
+    res[0] = cast<input1_T, res_T, CONFIG_T>(acc);
 }
 
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate1d(
     input1_T data1[CONFIG_T::n_elem1_0],
-	input2_T data2[CONFIG_T::n_elem2_0],
+    input2_T data2[CONFIG_T::n_elem2_0],
     res_T res[CONFIG_T::n_elem1_0 + CONFIG_T::n_elem2_0])
 {
     for (int ii=0; ii<CONFIG_T::n_elem1_0; ii++) {
         res[ii] = data1[ii];
     }
     for (int ii=0; ii<CONFIG_T::n_elem2_0; ii++) {
         res[CONFIG_T::n_elem1_0 + ii] = data2[ii];
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate2d_0(
     input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1],
-	input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1],
+    input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1],
     res_T res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 + CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1])
 {
     for (int ii=0; ii<CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1; ii++) {
         res[ii] = data1[ii];
     }
     for (int ii=0; ii<CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1; ii++) {
         res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 + ii] = data2[ii];
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate2d_1(
     input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1],
-	input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1],
+    input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1],
     res_T res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 + CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1])
 {
     for (int ii=0; ii<CONFIG_T::n_elem1_0; ii++) {
         for (int jj=0; jj<CONFIG_T::n_elem1_1; jj++) {
             res[ii * (CONFIG_T::n_elem1_1 + CONFIG_T::n_elem2_1) + jj] = data1[ii * CONFIG_T::n_elem1_1 + jj];
         }
         for (int jj=0; jj<CONFIG_T::n_elem2_1; jj++) {
@@ -192,42 +192,42 @@
         }
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate2d(
     input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1],
-	input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1],
+    input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1],
     res_T res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 + CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1])
 {
-    if (CONFIG_T::axis == 1 || CONFIG_T::axis == -1) {
+    if (CONFIG_T::axis == 2 || CONFIG_T::axis == -1) {
         concatenate2d_1<input1_T, input2_T, res_T, CONFIG_T>(data1, data2, res);
     } else {
         concatenate2d_0<input1_T, input2_T, res_T, CONFIG_T>(data1, data2, res);
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate3d_0(
 input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2],
-	input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
+    input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
     res_T res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2])
 {
     for (int ii=0; ii<CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2; ii++) {
         res[ii] = data1[ii];
     }
     for (int ii=0; ii<CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2; ii++) {
         res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2 + ii] = data2[ii];
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate3d_1(
 input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2],
-	input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
+    input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
     res_T res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2])
 {
     for (int ii=0; ii<CONFIG_T::n_elem1_0; ii++) {
         for (int jj=0; jj<CONFIG_T::n_elem1_1; jj++) {
             for (int kk=0; kk<CONFIG_T::n_elem1_2; kk++) {
                 int res_idx = ii * (CONFIG_T::n_elem1_1 + CONFIG_T::n_elem2_1) * CONFIG_T::n_elem1_2
                             + jj * CONFIG_T::n_elem1_2
@@ -250,31 +250,30 @@
             }
         }
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate3d_2(
-input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2],
-	input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
+    input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2],
+    input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
     res_T res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2])
 {
     for (int ii=0; ii<CONFIG_T::n_elem1_0; ii++) {
         for (int jj=0; jj<CONFIG_T::n_elem1_1; jj++) {
             for (int kk=0; kk<CONFIG_T::n_elem1_2; kk++) {
                 int res_idx = ii * CONFIG_T::n_elem1_1 * (CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_2)
                             + jj * (CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_2)
                             + kk;
                 int data_idx = ii * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2
                              + jj * CONFIG_T::n_elem1_2
                              + kk;
                 res[res_idx] = data1[data_idx];
             }
             for (int kk=0; kk<CONFIG_T::n_elem1_2; kk++) {
-                res[ii * (CONFIG_T::n_elem1_1 + CONFIG_T::n_elem2_1) + CONFIG_T::n_elem1_1 + jj] = data1[ii * CONFIG_T::n_elem2_1 + jj];
                 int res_idx = ii * CONFIG_T::n_elem1_1 * (CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_2)
                             + jj * (CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_2)
                             + kk + CONFIG_T::n_elem1_2;
                 int data_idx = ii * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2
                              + jj * CONFIG_T::n_elem2_2
                              + kk;
                 res[res_idx] = data2[data_idx];
@@ -282,20 +281,20 @@
         }
     }
 }
 
 template<class input1_T, class input2_T, class res_T, typename CONFIG_T>
 void concatenate3d(
     input1_T data1[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2],
-	input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
+    input2_T data2[CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2],
     res_T res[CONFIG_T::n_elem1_0 * CONFIG_T::n_elem1_1 * CONFIG_T::n_elem1_2 + CONFIG_T::n_elem2_0 * CONFIG_T::n_elem2_1 * CONFIG_T::n_elem2_2])
 {
-    if (CONFIG_T::axis == 2 || CONFIG_T::axis == -1) {
+    if (CONFIG_T::axis == 3 || CONFIG_T::axis == -1) {
         concatenate3d_2<input1_T, input2_T, res_T, CONFIG_T>(data1, data2, res);
-    } else if (CONFIG_T::axis == 1) {
+    } else if (CONFIG_T::axis == 2 || CONFIG_T::axis == -2) {
         concatenate3d_1<input1_T, input2_T, res_T, CONFIG_T>(data1, data2, res);
     } else {
         concatenate3d_0<input1_T, input2_T, res_T, CONFIG_T>(data1, data2, res);
     }
 }
 
 }
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_mult.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_mult.h`

 * *Files 13% similar despite different names*

```diff
@@ -16,86 +16,107 @@
  * --- */
 
 template<class x_T, class w_T, class y_T>
 class Product{
     public:
     static y_T product(x_T a, w_T w){
         // 'Normal' product
-        #pragma HLS inline off
+        #pragma HLS INLINE
         return a * w;
     }
+    static void limit(unsigned multiplier_limit) {} // Nothing to do here
 };
 
 template<class x_T, class w_T, class y_T>
 class both_binary : public Product<x_T, w_T, y_T>{
     public:
     static y_T product(x_T a, w_T w){
         // specialisation for 1-bit weights and incoming data
-        #pragma HLS inline off
+        #pragma HLS INLINE
         return a == w;
     }
 };
 
 template<class x_T, class w_T, class y_T>
 class weight_binary : public Product<x_T, w_T, y_T>{
     public:
     static y_T product(x_T a, w_T w){
         // Specialisation for 1-bit weights, arbitrary data
-        #pragma HLS inline off
+        #pragma HLS INLINE
         return w == 0 ? (x_T) -a : a;
     }
 };
 
 template<class x_T, class w_T, class y_T>
+class data_binary : public Product<x_T, w_T, y_T>{
+    public:
+    static y_T product(x_T a, w_T w){
+        // Specialisation for 1-bit data, arbitrary weight
+        #pragma HLS INLINE
+        return a == 0 ? (w_T) -w : w;
+    }
+};
+
+template<class x_T, class w_T, class y_T>
 class weight_ternary : public Product<x_T, w_T, y_T>{
     public:
     static y_T product(x_T a, w_T w){
         // Specialisation for 2-bit weights, arbitrary data
-        #pragma HLS inline off
+        #pragma HLS INLINE
         if (w == 0) return (x_T) 0;
         else if(w == -1) return (x_T) -a;
         else return (x_T) a; // if(w == 1)
     }
 };
 
 template<class x_T, class w_T, class y_T>
 class mult : public Product<x_T, w_T, y_T>{
     public:
     static y_T product(x_T a, w_T w){
         // 'Normal' product
-        #pragma HLS inline off
+        #pragma HLS INLINE
         return a * w;
     }
+    static void limit(unsigned multiplier_limit){
+        #pragma HLS INLINE
+        #pragma HLS ALLOCATION instances=mul limit=multiplier_limit operation
+    }
 };
 
 template<class x_T, class w_T, class y_T>
 class weight_exponential : public Product<x_T, w_T, y_T>{
     public:
     static y_T product(x_T a, w_T w){
         // Shift product for exponential weights
-        #pragma HLS inline off
+        #pragma HLS INLINE
         // shift by the exponent. Negative weights shift right
-        y_T ay = a;
-        y_T y = ay << w.weight;
+        y_T y = a << w.weight;
         // negate or not depending on weight sign
         return w.sign == 1 ? (y_T) y : (y_T) -y;
     }
 };
 
 } // namespace product_type
 
 template<class data_T, class res_T, typename CONFIG_T>
 inline typename std::enable_if<std::is_same<data_T, ap_uint<1>>::value
-        and std::is_same<typename CONFIG_T::weight_t, ap_uint<1>>::value, ap_int<nnet::ceillog2(CONFIG_T::n_in) + 2>>::type
+        && std::is_same<typename CONFIG_T::weight_t, ap_uint<1>>::value, ap_int<nnet::ceillog2(CONFIG_T::n_in) + 2>>::type
 cast(typename CONFIG_T::accum_t x){
   return (ap_int<nnet::ceillog2(CONFIG_T::n_in) + 2>) (x - CONFIG_T::n_in / 2) * 2;
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
-inline typename std::enable_if<(not std::is_same<data_T, ap_uint<1>>::value), res_T>::type
+inline typename std::enable_if<std::is_same<data_T, ap_uint<1>>::value
+        && ! std::is_same<typename CONFIG_T::weight_t, ap_uint<1>>::value, res_T>::type
+cast(typename CONFIG_T::accum_t x){
+  return (res_T) x;
+}
+
+template<class data_T, class res_T, typename CONFIG_T>
+inline typename std::enable_if<(! std::is_same<data_T, ap_uint<1>>::value), res_T>::type
 cast(typename CONFIG_T::accum_t x){
   return (res_T) x;
 }
 
 }
 
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_padding.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_padding.h`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_pooling.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_pooling.h`

 * *Files 11% similar despite different names*

```diff
@@ -83,29 +83,85 @@
   }
 }
 
 struct pooling1d_config{
   // IO size
   static const unsigned n_in = 10;
   static const unsigned pool_width = 2;
-  static const unsigned n_out = n_in / pool_width;
+  static const unsigned stride_width = 2;
+  static const unsigned n_out = (n_in - pool_width) / stride_width + 1;
   static const unsigned pad_left = 0;
   static const unsigned pad_right = 0;
   // Pooling function
   static const Pool_Op pool_op = Max;
 };
 
+template<typename CONFIG_T>
+constexpr int pool_op_limit_1d() {
+  return CONFIG_T::n_in * CONFIG_T::n_filt / CONFIG_T::reuse;
+}
+
 template<class data_T, class res_T, typename CONFIG_T>
-void pooling1d_cl(data_T data[CONFIG_T::n_in * CONFIG_T::n_filt], res_T res[CONFIG_T::n_out * CONFIG_T::n_filt]){
-  for(int ii = 0; ii < CONFIG_T::n_out * CONFIG_T::n_filt; ii ++){
-    data_T pool[CONFIG_T::pool_width];
-    for(int jj = 0; jj < CONFIG_T::pool_width; jj++){
-      pool[jj] = data[ii * CONFIG_T::pool_width + jj]; 
+void pooling1d_cl(data_T data[CONFIG_T::n_in * CONFIG_T::n_filt], res_T res[CONFIG_T::n_out * CONFIG_T::n_filt]) {
+
+  // TODO partition the arrays according to the reuse factor
+  const int limit = pool_op_limit_1d<CONFIG_T>();
+  #pragma HLS ALLOCATION instances=pool_op limit=limit function
+  // Add any necessary padding
+  unsigned padded_width = CONFIG_T::n_in + CONFIG_T::pad_left + CONFIG_T::pad_right;
+  if (CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0) {
+    padded_width -= padded_width - (padded_width / CONFIG_T::stride_width * CONFIG_T::stride_width);
+  }
+
+  for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+    // Loop over input image x in steps of stride
+    for(int ii = 0; ii < padded_width; ii += CONFIG_T::stride_width) {
+      data_T pool[CONFIG_T::pool_width];
+      // Keep track of number of pixels in image vs padding region
+      unsigned img_overlap = 0;
+      // Loop over pool window x
+      for(int jj = 0; jj < CONFIG_T::stride_width; jj++) {
+        if(ii+jj < CONFIG_T::pad_left || ii+jj >= (padded_width - CONFIG_T::pad_right)) {
+          // Add padding
+          pool[jj] = pad_val<data_T, CONFIG_T::pool_op>();
+        }else{
+          pool[jj] = data[(ii + jj) * CONFIG_T::n_filt + ff];
+          img_overlap++;
+        }
+      }
+      // do the pooling
+      // TODO in the case of average pooling, need to reduce width to area of pool window
+      // not overlapping padding region
+      res[(ii/CONFIG_T::stride_width)* CONFIG_T::n_filt + ff] =
+          pool_op<data_T, CONFIG_T::pool_width, CONFIG_T::pool_op>(pool);
+      // If the pool op is Average, the zero-padding needs to be removed from the results
+      if(CONFIG_T::pool_op == Average) {
+        data_T rescale = CONFIG_T::pool_width / img_overlap;
+        res[(ii/CONFIG_T::stride_width)* CONFIG_T::n_filt + ff] *= rescale;
+      }
+	  }
+  }
+}
+
+template<class data_T, class res_T, typename CONFIG_T>
+void global_pooling1d_cl(data_T data[CONFIG_T::n_in * CONFIG_T::n_filt], res_T res[CONFIG_T::n_filt]) {
+  assert(CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
+  assert(CONFIG_T::pool_width == CONFIG_T::stride_width);
+
+  // TODO partition the arrays according to the reuse factor
+  const int limit = pool_op_limit_1d<CONFIG_T>();
+  #pragma HLS ALLOCATION instances=pool_op limit=limit function
+
+  for(int ff = 0; ff < CONFIG_T::n_filt; ff++) {
+    data_T pool[CONFIG_T::n_in];
+    for(int jj = 0; jj < CONFIG_T::n_in; jj++) {
+      pool[jj] = data[jj * CONFIG_T::n_filt + ff];
     }
-    res[ii] = pool_op<data_T, CONFIG_T::pool_width, CONFIG_T::pool_op>(pool);
+  // do the pooling
+  res[ff] = pool_op<data_T, CONFIG_T::n_in, CONFIG_T::pool_op>(pool);
   }
 }
 
 struct pooling2d_config{
   // IO size
   static const unsigned in_height = 10;
   static const unsigned in_width = 10;
@@ -121,14 +177,17 @@
   static const unsigned pad_bottom = 0;
   static const unsigned pad_left = 0;
   static const unsigned pad_right = 0;
   // Pooling function
   static const Pool_Op pool_op = Max;
   // Reuse
   static const unsigned reuse = 1;
+  
+  // Internal data type definitions
+  typedef float accum_t;
 };
 
 template<typename CONFIG_T>
 constexpr int pool_op_limit(){
   return (CONFIG_T::out_height * CONFIG_T::out_width) * CONFIG_T::n_filt / CONFIG_T::reuse;
 }
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_pooling_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv_stream.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,356 +1,375 @@
-#ifndef NNET_POOLING_STREAM_H_
-#define NNET_POOLING_STREAM_H_
+#ifndef NNET_CONV_STREAM_H_
+#define NNET_CONV_STREAM_H_
 
-#include "utils/x_hls_utils.h"
+#include "ap_shift_reg.h"
 #include "nnet_common.h"
-#include "nnet_pooling.h"
 #include "hls_stream.h"
+#include "nnet_dense.h"
 
 namespace nnet {
 
+enum class conv_implementation { linebuffer=0, encoded=1};
+
 // *************************************************
-//       Max/average pooling
+//       Encoded Implementation (Vlad's)
 // *************************************************
-
-template <class T, int N, class CONFIG_T>
-T reduce_pool(T x[N]) {
+template<unsigned K, unsigned S, unsigned W>
+unsigned scale_index_K_gte_S(const unsigned idx) {
     #pragma HLS INLINE
-    if (CONFIG_T::pool_op == Max) {
-        Op_max<T> op_max;
-        return reduce<T, N, Op_max<T>>(x, op_max);
-    } else {
-        Op_add<T> op_add;
-        T sum = reduce<T, N, Op_add<T>>(x, op_add);
-        return sum / N;
-    }
-}
 
-template<unsigned TABLE_SIZE, unsigned POOL_SIZE>
-void init_pool_table(
-    unsigned table[TABLE_SIZE]
-) {
-    for (unsigned ii = 0; ii < TABLE_SIZE; ii++) {
-        table[ii] = ii % POOL_SIZE;
+    if (idx < K - S) {
+        return idx;
     }
-}
 
-template<class data_T, class res_T, typename CONFIG_T>
-void compute_pool_2d(
-    const unsigned h_idx,
-    const unsigned w_idx,
-    const data_T& in_elem,
-    hls::stream<typename data_T::value_type> data_window[CONFIG_T::pool_height * CONFIG_T::pool_width * CONFIG_T::n_filt],
-    hls::stream<res_T> &res,
-    res_T &res_pack,
-    unsigned &outputs_ready
-) {
-    // Nearest H without unused pixels on the right
-    constexpr unsigned nH = ((CONFIG_T::in_height - CONFIG_T::pool_height) / CONFIG_T::stride_height) * CONFIG_T::stride_height + CONFIG_T::pool_height;
-    // Scaled H that behaves like original H
-    constexpr unsigned sH = (DIV_ROUNDUP(CONFIG_T::pool_height, CONFIG_T::stride_height) - 1) * CONFIG_T::stride_height + CONFIG_T::pool_height;
-    // Nearest W without unused pixels on the right
-    constexpr unsigned nW = ((CONFIG_T::in_width - CONFIG_T::pool_width) / CONFIG_T::stride_width) * CONFIG_T::stride_width + CONFIG_T::pool_width;
-    // Scaled W that behaves like original W
-    constexpr unsigned sW = (DIV_ROUNDUP(CONFIG_T::pool_width, CONFIG_T::stride_width) - 1) * CONFIG_T::stride_width + CONFIG_T::pool_width;
-
-#ifdef __SYNTHESIS__
-    bool initialized = false;
-    unsigned pool_table_height[CONFIG_T::in_height];
-    unsigned pool_table_width[CONFIG_T::in_width];
-#else
-    static bool initialized = false;
-    static unsigned pool_table_height[CONFIG_T::in_height];
-    static unsigned pool_table_width[CONFIG_T::in_width];
-#endif
-    if (!initialized) {
-        init_pool_table<CONFIG_T::in_height, CONFIG_T::pool_height>(pool_table_height);
-        init_pool_table<CONFIG_T::in_width, CONFIG_T::pool_width>(pool_table_width);
-        initialized = true;
+    constexpr unsigned nW = ((W - K) / S) * S + K; // Nearest W without unused pixels on the right
+    constexpr unsigned sW = (DIV_ROUNDUP(K, S) - 1) * S + K; // Scaled W that behaves like original W
+    if (idx >= nW) {
+        return sW;
     }
 
-    #pragma HLS INLINE
-
-    if (data_T::size / CONFIG_T::n_filt > 1) {
-        #pragma HLS ARRAY_PARTITION variable=pool_table_height complete
-        #pragma HLS ARRAY_PARTITION variable=pool_table_width complete
+    const unsigned r = nW - idx;
+    if (r <= K - S) {
+        return sW - r;
     }
 
-    typename data_T::value_type pool_window[CONFIG_T::pool_height * CONFIG_T::pool_width];
-    #pragma HLS ARRAY_PARTITION variable=pool_window complete
+    return K - S + (idx - (K - S)) % S;
+}
 
-    const unsigned sh_idx = pool_table_height[h_idx] * CONFIG_T::pool_width;
-    const unsigned wp_idx = w_idx * (data_T::size / CONFIG_T::n_filt);
+template<unsigned K, unsigned S, unsigned W>
+unsigned scale_index_K_lt_S(const unsigned idx) {
+    #pragma HLS INLINE
 
-    PixelLoop: for (unsigned p = 0; p < data_T::size / CONFIG_T::n_filt; p++) {
-        #pragma HLS PIPELINE
+    if (idx < S - K) {
+        return idx;
+    }
 
-        ap_uint<CONFIG_T::pool_height * CONFIG_T::pool_width> filt_mask = 0;
-        if ((h_idx < nH) && (wp_idx + p < nW)) {
-            filt_mask = sh_idx + pool_table_width[wp_idx + p] + 1;
-        }
+    constexpr unsigned nW = ((W - K) / S) * S + K; // Nearest W without unused pixels on the right
+    constexpr unsigned sW = (DIV_ROUNDUP(S, K) - 1) * S + K; // Scaled W that behaves like original W
+    if (idx >= nW) {
+        return sW;
+    }
 
-        CopyDataFilt: for (unsigned c = 0; c < CONFIG_T::n_filt; c++) {
-            if (filt_mask > 0) data_window[c * CONFIG_T::pool_height * CONFIG_T::pool_width + filt_mask.to_uint() - 1].write(in_elem[p * CONFIG_T::n_filt + c]);
-        }
+    const unsigned r = nW - idx;
+    if (r <= S - K) {
+        return sW - r;
+    }
 
-        if (filt_mask == CONFIG_T::pool_height * CONFIG_T::pool_width) {
-            FiltLoop: for(unsigned c = 0; c < CONFIG_T::n_filt; c++) {
-                PoolLoop: for(unsigned f = 0; f < CONFIG_T::pool_height * CONFIG_T::pool_width; f++) {
-                    pool_window[f] = data_window[c * CONFIG_T::pool_height * CONFIG_T::pool_width + f].read();
-                }
-                if (res_T::size / CONFIG_T::n_filt == 1) { // Saves resources if we don't pack output, compiler will remove the else branch
-                    res_pack[c] = reduce_pool<typename data_T::value_type, CONFIG_T::pool_height * CONFIG_T::pool_width, CONFIG_T>(pool_window);
-                } else {
-                    res_pack[outputs_ready * CONFIG_T::n_filt + c] = reduce_pool<typename data_T::value_type, CONFIG_T::pool_height * CONFIG_T::pool_width, CONFIG_T>(pool_window);
-                }
+    return S - K + (idx - (S - K)) % S;
+}
 
-            }
-            if (res_T::size / CONFIG_T::n_filt == 1) { // Saves resources if we don't pack output, compiler will remove the else branch
-                res.write(res_pack);
-            } else {
-                if (outputs_ready == (res_T::size / CONFIG_T::n_filt) - 1) {
-                    res.write(res_pack);
-                    outputs_ready = 0;
-                } else {
-                    outputs_ready++;
-                }
-            }
-        }
+template<unsigned K, unsigned S, unsigned W>
+unsigned scale_index(const unsigned idx) {
+    #pragma HLS INLINE
+    
+    if (K >= S) {
+        return scale_index_K_gte_S<K, S, W>(idx);
+    } else {
+        return scale_index_K_lt_S<K, S, W>(idx);
     }
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
-void pooling2d_cl(
-    hls::stream<data_T> &data,
-    hls::stream<res_T> &res
+void mult_buffer(
+    hls::stream<typename data_T::value_type> data_window[CONFIG_T::kernel_size * CONFIG_T::n_chan],
+    res_T& res_pack,
+    hls::stream<res_T>& res_stream,
+    unsigned & outputs_ready,
+    typename CONFIG_T::weight_t weights[CONFIG_T::kernel_size * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t biases[CONFIG_T::n_filt]
 ) {
-    assert(CONFIG_T::pad_top == 0 && CONFIG_T::pad_bottom == 0 && CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
-    assert(CONFIG_T::pool_height == CONFIG_T::stride_height && CONFIG_T::pool_width == CONFIG_T::stride_width);
+    #pragma HLS INLINE
 
-    res_T res_pack;
-    #pragma HLS DATA_PACK variable=res_pack
-    unsigned outputs_ready = 0;
+    typename data_T::value_type data[CONFIG_T::kernel_size * CONFIG_T::n_chan];
+    #pragma HLS ARRAY_PARTITION variable=data complete
+    typename res_T::value_type res[CONFIG_T::n_filt];
+    #pragma HLS ARRAY_PARTITION variable=res complete
 
-    hls::stream<typename data_T::value_type> data_window[CONFIG_T::pool_height * CONFIG_T::pool_width * CONFIG_T::n_filt];
-    constexpr int win_depth = CONFIG_T::pool_height * CONFIG_T::out_width;
-    for (unsigned i_out = 0; i_out < CONFIG_T::pool_height * CONFIG_T::pool_width * CONFIG_T::n_filt; i_out++) {
-        #pragma HLS STREAM variable=data_window[i_out] depth=win_depth
+    InitData: for (int id = 0; id < CONFIG_T::kernel_size * CONFIG_T::n_chan; id++) {
+        #pragma HLS UNROLL
+        data[id] = data_window[id].read();
     }
 
-    constexpr int pack_factor = data_T::size / CONFIG_T::n_filt;
+    #pragma HLS INLINE region
+    if (CONFIG_T::strategy == nnet::latency) {
+        dense_latency<typename data_T::value_type, typename res_T::value_type, typename CONFIG_T::mult_config>(data, res, weights, biases);
+    } else {
+        dense_resource<typename data_T::value_type, typename res_T::value_type, typename CONFIG_T::mult_config>(data, res, weights, biases);
+    }
 
-    ReadInputHeight: for (unsigned i_ih = 0; i_ih < CONFIG_T::in_height; i_ih++) {
-        ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (pack_factor); i_iw++) {
-            #pragma HLS LOOP_FLATTEN
-            if (res_T::size / CONFIG_T::n_filt == 1) {
-                #pragma HLS PIPELINE II=pack_factor
-            }
-            compute_pool_2d<data_T, res_T, CONFIG_T>(i_ih, i_iw, data.read(), data_window, res, res_pack, outputs_ready);
+    CastLoop: for (unsigned jj = 0; jj < CONFIG_T::n_filt; jj++) {
+        #pragma HLS UNROLL
+        if (res_T::size / CONFIG_T::n_filt == 1) {
+            res_pack[jj] = res[jj];
+        } else {
+            res_pack[outputs_ready * CONFIG_T::n_filt + jj] = res[jj];
         }
     }
-}
 
+    if (res_T::size / CONFIG_T::n_filt == 1) {
+        res_stream.write(res_pack);
+    } else {
+        if (outputs_ready == (res_T::size / CONFIG_T::n_filt) - 1) {
+            res_stream.write(res_pack);
+            outputs_ready = 0;
+        } else {
+            outputs_ready++;
+        }
+    }
+}
 
 template<class data_T, class res_T, typename CONFIG_T>
-void compute_pool_1d(
-    const unsigned w_idx,
+void compute_output_encoded(
     const data_T& in_elem,
-    hls::stream<typename data_T::value_type> data_window[CONFIG_T::pool_width * CONFIG_T::n_filt],
+    hls::stream<typename data_T::value_type> data_window[CONFIG_T::kernel_size * CONFIG_T::n_chan],
     hls::stream<res_T> &res,
     res_T &res_pack,
-    unsigned &outputs_ready
+    unsigned &outputs_ready,
+    typename CONFIG_T::weight_t weights[CONFIG_T::kernel_size * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t biases[CONFIG_T::n_filt],
+    ap_uint<CONFIG_T::kernel_size> *pixel_idx
 ) {
-    // Nearest W without unused pixels on the right
-    constexpr unsigned nW = ((CONFIG_T::n_in - CONFIG_T::pool_width) / CONFIG_T::stride_width) * CONFIG_T::stride_width + CONFIG_T::pool_width;
-    // Scaled W that behaves like original W
-    constexpr unsigned sW = (DIV_ROUNDUP(CONFIG_T::pool_width, CONFIG_T::stride_width) - 1) * CONFIG_T::stride_width + CONFIG_T::pool_width;
-
-#ifdef __SYNTHESIS__
-    bool initialized = false;
-    unsigned pool_table_width[CONFIG_T::n_in];
-#else
-    static bool initialized = false;
-    static unsigned pool_table_width[CONFIG_T::n_in];
-#endif
-    if (!initialized) {
-        init_pool_table<CONFIG_T::n_in, CONFIG_T::pool_width>(pool_table_width);
-        initialized = true;
-    }
-
     #pragma HLS INLINE
 
-    if (data_T::size / CONFIG_T::n_filt > 1) {
-        #pragma HLS ARRAY_PARTITION variable=pool_table_width complete
+    MultLoop: for (unsigned p = 0; p < data_T::size / CONFIG_T::n_chan; p++) {
+        #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
+        CopyDataFilt: for (unsigned f = 0; f < CONFIG_T::kernel_size; f++) {
+            #pragma HLS UNROLL
+            CopyDataChan: for (unsigned c = 0; c < CONFIG_T::n_chan; c++) {
+                #pragma HLS UNROLL
+                if (pixel_idx[p][f]) data_window[f * CONFIG_T::n_chan + c].write(in_elem[p * CONFIG_T::n_chan + c]);
+            }
+        }
+        if (pixel_idx[p][CONFIG_T::kernel_size - 1]) {
+            mult_buffer<data_T, res_T, CONFIG_T>(data_window, res_pack, res, outputs_ready, weights, biases);
+        }
     }
+}
 
-    typename data_T::value_type pool_window[CONFIG_T::pool_width];
-    #pragma HLS ARRAY_PARTITION variable=pool_window complete
 
-    const unsigned wp_idx = w_idx * (data_T::size / CONFIG_T::n_filt);
 
-    PixelLoop: for (unsigned p = 0; p < data_T::size / CONFIG_T::n_filt; p++) {
-        #pragma HLS PIPELINE
+// *************************************************
+//       Line Buffer Implementation (Phil's)
+// *************************************************
+template <class data_T, typename CONFIG_T>
+void kernel_shift_1d(
+    const data_T& in_elem,
+    typename data_T::value_type kernel_window[CONFIG_T::filt_width * CONFIG_T::n_chan]
+) {
+    #pragma HLS inline
+    #pragma HLS PIPELINE II = 1
+    
+    // Shift kernel_window by one step to the left (manual shift operation)
+    static const int filt_width = CONFIG_T::filt_width - 1;
+    KernelShiftWidth: for (int i_iw = 0; i_iw < filt_width; i_iw++) {
+        #pragma HLS UNROLL
+        KernelShiftChannel: for (unsigned i_ic = 0; i_ic < CONFIG_T::n_chan; i_ic++) {
+            // Shift every element in kernel_window to the left
+            kernel_window[i_iw * CONFIG_T::n_chan + i_ic] = kernel_window[(i_iw + 1) * CONFIG_T::n_chan + i_ic];
+        }
+    }
+
+    // Insert shift_buffer column into right-most column of kernel
+    static const int lastheight = (CONFIG_T::filt_width - 1) * CONFIG_T::n_chan;
+    KernelPushChannel: for (int i_ic = 0; i_ic < CONFIG_T::n_chan; i_ic++) {
+        #pragma HLS UNROLL
+        kernel_window[lastheight + i_ic] = in_elem[i_ic];
+    }
+}
 
-        ap_uint<CONFIG_T::pool_width> filt_mask = 0;
-        if (wp_idx + p < nW) {
-            filt_mask = pool_table_width[wp_idx + p] + 1;
+template <class data_T, typename CONFIG_T>
+void kernel_shift_2d(
+    typename data_T::value_type shift_buffer[CONFIG_T::filt_height][CONFIG_T::n_chan],
+    typename data_T::value_type kernel_window[CONFIG_T::filt_width * CONFIG_T::filt_height * CONFIG_T::n_chan]
+) {
+    #pragma HLS inline
+        
+    // Shift kernel_window by one step to the left (manual shift operation)
+    static const int filt_width = CONFIG_T::filt_width - 1;
+    KernelShiftWidth: for (int i_iw = 0; i_iw < filt_width; i_iw++) {
+        #pragma HLS PIPELINE II = 1
+        KernelShiftHeight: for (unsigned i_ih = 0; i_ih < CONFIG_T::filt_height; i_ih++) {
+            KernelShiftChannel: for (unsigned i_ic = 0; i_ic < CONFIG_T::n_chan; i_ic++) {
+            // Shift every element in kernel_window to the left
+                kernel_window[i_ih * CONFIG_T::filt_width * CONFIG_T::n_chan + i_iw * CONFIG_T::n_chan + i_ic] = kernel_window[i_ih * CONFIG_T::filt_width * CONFIG_T::n_chan + (i_iw + 1) * CONFIG_T::n_chan + i_ic];
+            }
         }
+    }
 
-        CopyDataFilt: for (unsigned c = 0; c < CONFIG_T::n_filt; c++) {
-            if (filt_mask > 0) data_window[c * CONFIG_T::pool_width + filt_mask.to_uint() - 1].write(in_elem[p * CONFIG_T::n_filt + c]);
+    // Insert shift_buffer column into right-most column of kernel
+    static const int lastheight = (CONFIG_T::filt_width - 1) * CONFIG_T::n_chan;
+    KernelPushHeight: for (int i_ih = 0; i_ih < CONFIG_T::filt_height; i_ih++) {
+        #pragma HLS UNROLL
+        KernelPushChannel: for (int i_ic = 0; i_ic < CONFIG_T::n_chan; i_ic++) {
+            kernel_window[lastheight + i_ih * CONFIG_T::filt_width * CONFIG_T::n_chan + i_ic] = shift_buffer[i_ih][i_ic];
         }
+    }
+}
 
-        if (filt_mask == CONFIG_T::pool_width) {
-            FiltLoop: for(unsigned c = 0; c < CONFIG_T::n_filt; c++) {
-                PoolLoop: for(unsigned f = 0; f < CONFIG_T::pool_width; f++) {
-                    pool_window[f] = data_window[c * CONFIG_T::pool_width + f].read();
-                }
-                if (res_T::size / CONFIG_T::n_filt == 1) { // Saves resources if we don't pack output, compiler will remove the else branch
-                    res_pack[c] = reduce_pool<typename data_T::value_type, CONFIG_T::pool_width, CONFIG_T>(pool_window);
-                } else {
-                    res_pack[outputs_ready * CONFIG_T::n_filt + c] = reduce_pool<typename data_T::value_type, CONFIG_T::pool_width, CONFIG_T>(pool_window);
-                }
+template <class data_T, typename CONFIG_T>
+void shift_line_buffer(const data_T& in_elem, 
+                    ap_shift_reg<typename data_T::value_type, CONFIG_T::in_width> line_buffer[MAX(CONFIG_T::filt_height - 1,1)][CONFIG_T::n_chan],
+                    typename data_T::value_type kernel_window[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan]
+) {
+    
+    #pragma HLS PIPELINE
 
-            }
-            if (res_T::size / CONFIG_T::n_filt == 1) { // Saves resources if we don't pack output, compiler will remove the else branch
-                res.write(res_pack);
-            } else {
-                if (outputs_ready == (res_T::size / CONFIG_T::n_filt) - 1) {
-                    res.write(res_pack);
-                    outputs_ready = 0;
-                } else {
-                    outputs_ready++;
-                }
-            }
+    // Temporary buffer for popped (shifted) elements
+    typename data_T::value_type shift_buffer[CONFIG_T::filt_height][CONFIG_T::n_chan];
+    #pragma HLS ARRAY_PARTITION variable = shift_buffer complete dim = 0
+
+    UpdateBuffer: for (int i_ic = 0; i_ic < CONFIG_T::n_chan; i_ic++) {
+        #pragma HLS UNROLL
+
+        // Insert pixel(s) at end of shift buffer
+        shift_buffer[CONFIG_T::filt_height - 1][i_ic] = in_elem[i_ic];
+    }
+
+    LineBufferDataIn: for (int i_ic = 0; i_ic < CONFIG_T::n_chan; i_ic++) {
+        // Shift the shift buffer into the line buffer
+        LineBufferShift: for (unsigned i_ih = 1; i_ih < CONFIG_T::filt_height; i_ih++) {
+            #pragma HLS UNROLL
+            typename data_T::value_type pop_elem = line_buffer[i_ih - 1][i_ic].shift(shift_buffer[CONFIG_T::filt_height - i_ih][i_ic]); // Shift the line buffer, return the popped pixel
+            shift_buffer[CONFIG_T::filt_height - i_ih - 1][i_ic] = pop_elem; // Popped element placed back into shift_buffer, one row up.
         }
     }
+    kernel_shift_2d<data_T, CONFIG_T>(shift_buffer, kernel_window);
 }
 
 template<class data_T, class res_T, typename CONFIG_T>
-void pooling1d_cl(
-    hls::stream<data_T> &data,
-    hls::stream<res_T> &res
+void compute_output_buffer_2d(
+    const data_T& in_elem,
+    ap_shift_reg<typename data_T::value_type, CONFIG_T::in_width> line_buffer[MAX(CONFIG_T::filt_height - 1,1)][CONFIG_T::n_chan],
+    hls::stream<res_T> &res_stream,
+    typename CONFIG_T::weight_t weights[CONFIG_T::kernel_size * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t biases[CONFIG_T::n_filt]
 ) {
-    assert(CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
-    assert(CONFIG_T::pool_width == CONFIG_T::stride_width);
+    #pragma HLS INLINE
+
+    // Thresholds
+    const static int lShiftX = CONFIG_T::filt_width - 1;
+    const static int lShiftY = CONFIG_T::filt_height - 1;
+
+    // Counters
+    static int pX = 0; // Pixel X
+    static int pY = 0; // Pixel Y
+
+    static int sX = 0; // Stride X
+    static int sY = 0; // Stride Y
+
+    static typename data_T::value_type kernel_data[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan];
+    #pragma HLS ARRAY_PARTITION variable=kernel_data complete
+
+    typename res_T::value_type res_out[CONFIG_T::n_filt];
+    #pragma HLS ARRAY_PARTITION variable=res_out complete dim = 0
 
     res_T res_pack;
     #pragma HLS DATA_PACK variable=res_pack
-    unsigned outputs_ready = 0;
 
-    hls::stream<typename data_T::value_type> data_window[CONFIG_T::pool_width * CONFIG_T::n_filt];
-    constexpr int win_depth = CONFIG_T::n_out;
-    for (unsigned i_out = 0; i_out < CONFIG_T::pool_width * CONFIG_T::n_filt; i_out++) {
-        #pragma HLS STREAM variable=data_window[i_out] depth=win_depth
-    }
-
-    constexpr int pack_factor = data_T::size / CONFIG_T::n_filt;
+    // Add pixel to buffer
+    nnet::shift_line_buffer<data_T, CONFIG_T>(in_elem, line_buffer, kernel_data);
 
-    ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::n_in / (pack_factor); i_iw++) {
-        #pragma HLS LOOP_FLATTEN
-        if (res_T::size / CONFIG_T::n_filt == 1) {
-            #pragma HLS PIPELINE II=pack_factor
+    // Check to see if we have a full kernel
+    if ( (sX - lShiftX) == 0 && (sY - lShiftY) == 0 && pY > lShiftY - 1 && pX > lShiftX - 1) {
+        
+        // Dense multiply
+        #pragma HLS INLINE region
+        if (CONFIG_T::strategy == nnet::latency) {
+            dense_latency<typename data_T::value_type, typename res_T::value_type, typename CONFIG_T::mult_config>(kernel_data, res_out, weights, biases);
+        } else {
+            dense_resource<typename data_T::value_type, typename res_T::value_type, typename CONFIG_T::mult_config>(kernel_data, res_out, weights, biases);
         }
-        compute_pool_1d<data_T, res_T, CONFIG_T>(i_iw, data.read(), data_window, res, res_pack, outputs_ready);
-    }
-}
 
+        // Pack output
+        CastLoop: for (unsigned i_ic = 0; i_ic < CONFIG_T::n_filt; i_ic++) {
+            #pragma HLS UNROLL
+            res_pack[i_ic] = res_out[i_ic];
+        }
 
-// *************************************************
-//       Global max/average pooling
-// *************************************************
+        // Write output to stream when output ready
+        res_stream.write(res_pack);
+    }
 
-template <class T, int N, class CONFIG_T>
-T reduce_global_pool(T x, T y[N]) {
-    #pragma HLS INLINE
-    if (CONFIG_T::pool_op == Max) {
-        Op_max<T> op_max;
-        T y_max = reduce<T, N, Op_max<T>>(y, op_max);
-        return (x > y_max) ? x : y_max;
+    // Counter Housekeeping
+    if (pX + 1 == CONFIG_T::in_width)  // Includes padding, end of line (padded)
+    {
+        pX = 0; 
+        sX = 0;
+        if (pY + 1 == CONFIG_T::in_height) {  // Reached bottom of image
+            pY = 0; 
+            sY = 0;
+        } else {
+            pY = pY + 1;
+            // Update stride (threshold) ? subtract stride : increment stride
+            sY = ((sY - lShiftY) == 0) ? sY - CONFIG_T::stride_height + 1 : sY + 1; 
+        }
     } else {
-        Op_add<T> op_add;
-        T y_sum = reduce<T, N, Op_add<T>>(y, op_add);
-        return x + y_sum;
+        pX = pX + 1;
+        // Update stride (threshold) ? subtract stride : increment stride
+        sX = ((sX - lShiftX) == 0) ? sX - CONFIG_T::stride_width + 1 : sX + 1; 
     }
 }
 
+// Conv 1D compute output
 template<class data_T, class res_T, typename CONFIG_T>
-void compute_global_pool(
-    const unsigned h_idx,
-    const unsigned w_idx,
+void compute_output_buffer_1d(
     const data_T& in_elem,
-    typename data_T::value_type data_window[CONFIG_T::n_filt]
+    hls::stream<res_T> &res_stream,
+    typename CONFIG_T::weight_t weights[CONFIG_T::kernel_size * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t biases[CONFIG_T::n_filt]
 ) {
-    PoolFilt: for (unsigned c = 0; c < CONFIG_T::n_filt; c++) {
-        #pragma HLS UNROLL
+    #pragma HLS INLINE
 
-        typename data_T::value_type data_pack[data_T::size / CONFIG_T::n_filt];
-        #pragma HLS ARRAY_PARTITION variable=data_pack complete dim=0
+    // Thresholds
+    const static int lShiftX = CONFIG_T::filt_width - 1;
 
-        PixelLoop: for (unsigned p = 0; p < data_T::size / CONFIG_T::n_filt; p++) {
-            #pragma HLS UNROLL
-            data_pack[p] = in_elem[p * CONFIG_T::n_filt + c];
-        }
-        data_window[c] = reduce_global_pool<typename data_T::value_type, data_T::size / CONFIG_T::n_filt, CONFIG_T>(data_window[c], data_pack);
-    }
-}
+    // Counters
+    static int pX = 0; // pixel counter
+    static int sX = 0; // stride counter
 
-template<class data_T, class res_T, typename CONFIG_T>
-void global_pooling2d_cl(
-    hls::stream<data_T> &data,
-    hls::stream<res_T> &res
-) {
-    assert(CONFIG_T::pad_top == 0 && CONFIG_T::pad_bottom == 0 && CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
-    assert(CONFIG_T::pool_height == CONFIG_T::stride_height && CONFIG_T::pool_width == CONFIG_T::stride_width);
+    static typename data_T::value_type kernel_data[CONFIG_T::filt_width * CONFIG_T::n_chan];
+    #pragma HLS ARRAY_PARTITION variable=kernel_data complete
 
-    typename data_T::value_type data_window[CONFIG_T::n_filt];
-    #pragma HLS ARRAY_PARTITION variable=data_window complete
+    typename res_T::value_type res_out[CONFIG_T::n_filt];
+    #pragma HLS ARRAY_PARTITION variable=res_out complete dim = 0
 
-    typename data_T::value_type init = 0;
-    if (CONFIG_T::pool_op == Max) {
-        init = hls::numeric_limits<typename data_T::value_type>::min();
-    }
+    res_T res_pack;
+    #pragma HLS DATA_PACK variable=res_pack
 
-    PoolInitLoop: for (unsigned i_init = 0; i_init < CONFIG_T::n_filt; i_init++) {
-        #pragma HLS UNROLL
-        data_window[i_init] = init;
-    }
+    // Add pixel to buffer
+    nnet::kernel_shift_1d<data_T, CONFIG_T>(in_elem, kernel_data);
 
-    ReadInputHeight: for (unsigned i_ih = 0; i_ih < CONFIG_T::in_height; i_ih++) {
-        ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (data_T::size / CONFIG_T::n_filt); i_iw++) {
-            #pragma HLS LOOP_FLATTEN
-            compute_global_pool<data_T, res_T, CONFIG_T>(i_ih, i_iw, data.read(), data_window);
+    // Check to see if we have a full kernel
+    if ( (sX - lShiftX) == 0 && pX > lShiftX - 1 ) {
+        
+        // Dense multiply
+        #pragma HLS INLINE region
+        if (CONFIG_T::strategy == nnet::latency) {
+            dense_latency<typename data_T::value_type, typename res_T::value_type, typename CONFIG_T::mult_config>(kernel_data, res_out, weights, biases);
+        } else {
+            dense_resource<typename data_T::value_type, typename res_T::value_type, typename CONFIG_T::mult_config>(kernel_data, res_out, weights, biases);
         }
-    }
 
-    if (CONFIG_T::pool_op == Max) {
-        MaxPoolRes: for (unsigned i_res = 0; i_res < CONFIG_T::n_filt / res_T::size; i_res++) {
-            #pragma HLS PIPELINE
-
-            res_T res_pack;
-            #pragma HLS DATA_PACK variable=res_pack
-            MaxPoolPack: for (unsigned i_pack = 0; i_pack < res_T::size; i_pack++) {
-                #pragma HLS UNROLL
-                res_pack[i_pack] = data_window[i_pack];
-            }
-            res.write(res_pack);
+        // Pack output
+        CastLoop: for (unsigned i_ic = 0; i_ic < CONFIG_T::n_filt; i_ic++) {
+            #pragma HLS UNROLL
+            res_pack[i_ic] = res_out[i_ic];
         }
-    } else {
-        AvgPoolRes: for (unsigned i_res = 0; i_res < CONFIG_T::n_filt / res_T::size; i_res++) {
-            #pragma HLS PIPELINE
 
-            res_T res_pack;
-            #pragma HLS DATA_PACK variable=res_pack
-            AvgPoolPack: for (unsigned i_pack = 0; i_pack < res_T::size; i_pack++) {
-                #pragma HLS UNROLL
-                res_pack[i_pack] = data_window[i_pack] / (CONFIG_T::in_height * CONFIG_T::in_width);
-            }
-            res.write(res_pack);
-        }
+        // Write output to stream when output ready
+        res_stream.write(res_pack);
     }
 
+    // Counter Housekeeping
+    if (pX + 1 == CONFIG_T::in_width)  // Includes padding, end of line (padded)
+    {
+        pX = 0;
+        sX = 0;
+    } else {
+        pX = pX + 1;
+        // Update stride (threshold) ? subtract stride : increment stride
+        sX = ((sX - lShiftX) == 0) ? sX - CONFIG_T::stride_width + 1 : sX + 1; 
+    }
 }
 
 }
-
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv1d_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv1d_stream.h`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 #include "hls_stream.h"
 #include "nnet_sepconv_stream.h"
 #include "nnet_conv1d_stream.h"
 
 namespace nnet {
 
 template<class data_T, class res_T, typename CONFIG_T>
-void depthwise_conv_1d_cl(
+void depthwise_conv_1d_encoded_cl(
     hls::stream<data_T> &data,
     hls::stream<res_T>  &res,
     typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_chan])
 {
     assert(CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
-    assert(CONFIG_T::stride_width <= CONFIG_T::filt_width);
 
     hls::stream<typename data_T::value_type> data_window[CONFIG_T::filt_width * CONFIG_T::n_chan];
     const int win_depth = CONFIG_T::out_width;
     for (unsigned i_out = 0; i_out < CONFIG_T::filt_width * CONFIG_T::n_chan; i_out++) {
         #pragma HLS STREAM variable=data_window[i_out] depth=win_depth
     }
 
@@ -35,18 +34,35 @@
 
     ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (data_T::size / CONFIG_T::n_chan); i_iw++) {
         #pragma HLS LOOP_FLATTEN
         if (CONFIG_T::strategy == nnet::latency && data_T::size / CONFIG_T::n_chan == 1) {
             #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
         }
         compute_scaled_indices_1d<data_T, CONFIG_T>(i_iw, pixel_idx);
-        compute_depthwise_output<data_T, res_T, CONFIG_T>(data.read(), data_window, res, res_pack, outputs_ready, weights, biases, pixel_idx);
+        compute_depthwise_output_encoded<data_T, res_T, CONFIG_T>(data.read(), data_window, res, res_pack, outputs_ready, weights, biases, pixel_idx);
     }
 }
 
+template<class data_T, class res_T, typename CONFIG_T>
+void depthwise_conv_1d_buffer_cl(
+    hls::stream<data_T> &data,
+    hls::stream<res_T>  &res,
+    typename CONFIG_T::weight_t weights[CONFIG_T::filt_width * CONFIG_T::n_chan],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_chan])
+{
+    assert(CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
+
+    ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width; i_iw++) {
+        #pragma HLS LOOP_FLATTEN
+        if (CONFIG_T::strategy == nnet::latency) {
+            #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
+        }
+        compute_depthwise_output_buffer_1d<data_T, res_T, CONFIG_T>(data.read(), res, weights, biases);
+    }
+}
 
 template<class data_T, class res_T, typename CONFIG_T>
 void pointwise_conv_1d_cl(
     hls::stream<data_T> &data,
     hls::stream<res_T>  &res,
     typename CONFIG_T::weight_t weights[CONFIG_T::n_chan * CONFIG_T::n_filt],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
@@ -81,13 +97,20 @@
 ) {
     #pragma HLS DATAFLOW
 
     hls::stream<data_T> depthwise_res;
     unsigned res_depth = CONFIG_T::depthwise_config::out_width;
     #pragma HLS STREAM variable=depthwise_res depth=res_depth
 
-    depthwise_conv_1d_cl<data_T, data_T, typename CONFIG_T::depthwise_config>(data, depthwise_res, depthwise_weights, depthwise_biases);
+    switch(CONFIG_T::depthwise_config::implementation){
+        case conv_implementation::linebuffer:
+            depthwise_conv_1d_buffer_cl<data_T, data_T, typename CONFIG_T::depthwise_config>(data, depthwise_res, depthwise_weights, depthwise_biases);
+            break;
+        case conv_implementation::encoded:
+            depthwise_conv_1d_encoded_cl<data_T, data_T, typename CONFIG_T::depthwise_config>(data, depthwise_res, depthwise_weights, depthwise_biases);
+            break;
+    } 
     pointwise_conv_1d_cl<data_T, res_T, typename CONFIG_T::pointwise_config>(depthwise_res, res, pointwise_weights, pointwise_biases);
 }
 
 }
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_sepconv2d_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_conv2d_stream.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,43 @@
-#ifndef NNET_SEPARABLE_CONV2D_STREAM_H_
-#define NNET_SEPARABLE_CONV2D_STREAM_H_
+#ifndef NNET_CONV2D_STREAM_H_
+#define NNET_CONV2D_STREAM_H_
 
+#include "ap_shift_reg.h"
 #include "nnet_common.h"
+#include "nnet_conv_stream.h"
 #include "hls_stream.h"
-#include "nnet_sepconv_stream.h"
-#include "nnet_conv2d_stream.h"
 
 namespace nnet {
 
+template<class data_T, typename CONFIG_T>
+void compute_scaled_indices_2d(
+    const unsigned h_idx,
+    const unsigned w_idx,
+    ap_uint<CONFIG_T::filt_height * CONFIG_T::filt_width> *pixel_idx
+) {
+    const unsigned sh_idx = scale_index<CONFIG_T::filt_height, CONFIG_T::stride_height, CONFIG_T::in_height>(h_idx);
+    unsigned wp_idx = w_idx * (data_T::size / CONFIG_T::n_chan);
+
+    ComputeIndex: for (unsigned p = 0; p < data_T::size / CONFIG_T::n_chan; p++) {
+        #pragma HLS UNROLL
+
+        unsigned sw_idx = scale_index<CONFIG_T::filt_width, CONFIG_T::stride_width, CONFIG_T::in_width>(wp_idx + p);
+        pixel_idx[p] = CONFIG_T::pixels[sh_idx * CONFIG_T::min_width + sw_idx];
+    }
+}
+
 template<class data_T, class res_T, typename CONFIG_T>
-void depthwise_conv_2d_cl(
+void conv_2d_encoded_cl(
     hls::stream<data_T> &data,
     hls::stream<res_T>  &res,
-    typename CONFIG_T::weight_t weights[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan],
-    typename CONFIG_T::bias_t   biases[CONFIG_T::n_chan])
+    typename CONFIG_T::weight_t weights[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
 {
     assert(CONFIG_T::pad_top == 0 && CONFIG_T::pad_bottom == 0 && CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
     assert(CONFIG_T::filt_height == CONFIG_T::filt_width);
-    assert(CONFIG_T::stride_height <= CONFIG_T::filt_height && CONFIG_T::stride_width <= CONFIG_T::filt_width);
 
     hls::stream<typename data_T::value_type> data_window[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan];
     const int win_depth = CONFIG_T::filt_height * CONFIG_T::out_width;
     for (unsigned i_out = 0; i_out < CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan; i_out++) {
         #pragma HLS STREAM variable=data_window[i_out] depth=win_depth
     }
 
@@ -37,61 +53,60 @@
     ReadInputHeight: for (unsigned i_ih = 0; i_ih < CONFIG_T::in_height; i_ih++) {
         ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (data_T::size / CONFIG_T::n_chan); i_iw++) {
             #pragma HLS LOOP_FLATTEN
             if (CONFIG_T::strategy == nnet::latency && data_T::size / CONFIG_T::n_chan == 1) {
                 #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
             }
             compute_scaled_indices_2d<data_T, CONFIG_T>(i_ih, i_iw, pixel_idx);
-            compute_depthwise_output<data_T, res_T, CONFIG_T>(data.read(), data_window, res, res_pack, outputs_ready, weights, biases, pixel_idx);
+            compute_output_encoded<data_T, res_T, CONFIG_T>(data.read(), data_window, res, res_pack, outputs_ready, weights, biases, pixel_idx);
         }
     }
 }
 
-template<class data_T, class res_T, typename CONFIG_T>
-void pointwise_conv_2d_cl(
+// Line Buffer
+template <class data_T, class res_T, typename CONFIG_T>
+void conv_2d_buffer_cl(
     hls::stream<data_T> &data,
     hls::stream<res_T>  &res,
-    typename CONFIG_T::weight_t weights[CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::weight_t weights[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
     typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
 {
     assert(CONFIG_T::pad_top == 0 && CONFIG_T::pad_bottom == 0 && CONFIG_T::pad_left == 0 && CONFIG_T::pad_right == 0);
-    assert(CONFIG_T::filt_height == 1 && CONFIG_T::filt_width == 1);
 
-    #pragma HLS ARRAY_PARTITION variable=weights complete
-    #pragma HLS ARRAY_PARTITION variable=biases complete
+    static ap_shift_reg<typename data_T::value_type, CONFIG_T::in_width> line_buffer[MAX(CONFIG_T::filt_height - 1,1)][CONFIG_T::n_chan];
+    #pragma HLS ARRAY_PARTITION variable = line_buffer complete dim = 2
 
     ReadInputHeight: for (unsigned i_ih = 0; i_ih < CONFIG_T::in_height; i_ih++) {
-        ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width / (data_T::size / CONFIG_T::n_chan); i_iw++) {
-            if (CONFIG_T::strategy == nnet::latency && data_T::size / CONFIG_T::n_chan == 1) {
+        ReadInputWidth: for (unsigned i_iw = 0; i_iw < CONFIG_T::in_width; i_iw++) {
+            #pragma HLS LOOP_FLATTEN
+            if(CONFIG_T::strategy == nnet::latency) {
                 #pragma HLS PIPELINE II=CONFIG_T::reuse_factor
             }
-            if (i_ih % CONFIG_T::stride_height == 0 && i_iw % CONFIG_T::stride_width == 0) {
-                pointwise_mult_buffer<data_T, res_T, CONFIG_T>(data.read(), res, weights, biases);
+            if (CONFIG_T::filt_height > 1) {
+                compute_output_buffer_2d<data_T, res_T, CONFIG_T>(data.read(), line_buffer, res, weights, biases);
             } else {
-                data.read();
+                compute_output_buffer_1d<data_T, res_T, CONFIG_T>(data.read(), res, weights, biases);
             }
         }
     }
 }
 
-
-template<class data_T, class res_T, typename CONFIG_T>
-void separable_conv_2d_cl(
+template <class data_T, class res_T, typename CONFIG_T>
+void conv_2d_cl(
     hls::stream<data_T> &data,
     hls::stream<res_T>  &res,
-    typename CONFIG_T::depthwise_config::weight_t depthwise_weights[CONFIG_T::depthwise_config::filt_height * CONFIG_T::depthwise_config::filt_width * CONFIG_T::depthwise_config::n_chan],
-    typename CONFIG_T::pointwise_config::weight_t pointwise_weights[CONFIG_T::pointwise_config::n_chan * CONFIG_T::pointwise_config::n_filt],
-    typename CONFIG_T::depthwise_config::bias_t   depthwise_biases[CONFIG_T::depthwise_config::n_chan],
-    typename CONFIG_T::pointwise_config::bias_t   pointwise_biases[CONFIG_T::pointwise_config::n_filt]
-) {
-    #pragma HLS DATAFLOW
-
-    hls::stream<data_T> depthwise_res;
-    unsigned res_depth = CONFIG_T::depthwise_config::out_height * CONFIG_T::depthwise_config::out_width;
-    #pragma HLS STREAM variable=depthwise_res depth=res_depth
-
-    depthwise_conv_2d_cl<data_T, data_T, typename CONFIG_T::depthwise_config>(data, depthwise_res, depthwise_weights, depthwise_biases);
-    pointwise_conv_2d_cl<data_T, res_T, typename CONFIG_T::pointwise_config>(depthwise_res, res, pointwise_weights, pointwise_biases);
+    typename CONFIG_T::weight_t weights[CONFIG_T::filt_height * CONFIG_T::filt_width * CONFIG_T::n_chan * CONFIG_T::n_filt],
+    typename CONFIG_T::bias_t   biases[CONFIG_T::n_filt])
+{
+    #pragma HLS inline region
+    switch(CONFIG_T::implementation){
+        case conv_implementation::linebuffer:
+            conv_2d_buffer_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
+            break;
+        case conv_implementation::encoded:
+            conv_2d_encoded_cl<data_T, res_T, CONFIG_T>(data, res, weights, biases);
+            break;
+    }  
 }
 
 }
 #endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_stream.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_stream.h`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 #ifndef NNET_STREAM_H
 #define NNET_STREAM_H
 
 #include "hls_stream.h"
 
 namespace nnet {
 
+struct broadcast_config
+{
+  static const unsigned in_height = 10;
+  static const unsigned in_width = 10;
+  static const unsigned n_chan = 1;
+  static const unsigned n_dupl = 2;
+};
+
 template<class data_T, class res_T, int N>
 void clone_stream(hls::stream<data_T> &data, hls::stream<res_T> &res1, hls::stream<res_T> &res2) {
     CloneLoop: for (int i = 0; i < N / data_T::size; i++) {
         #pragma HLS PIPELINE
 
         data_T in_data = data.read();
         res_T out_data1;
@@ -86,10 +94,27 @@
             } else {
                 pack_cnt++;
             }
         }
     }
 }
 
+template<class data_T, class res_T, typename CONFIG_T>
+void broadcast_stream(hls::stream<data_T> &data, hls::stream<res_T> &res) {
+    BroadcastLoop: for (int i = 0; i < CONFIG_T::in_height * CONFIG_T::in_width * CONFIG_T::n_chan / data_T::size; i++) {
+        #pragma HLS PIPELINE
+        data_T in_data = data.read();
+        for (int j = 0; j < CONFIG_T::n_dupl; j++) {
+            #pragma HLS PIPELINE
+            res_T out_data;
+            #pragma HLS DATA_PACK variable=out_data
+            for (int k = 0; k < res_T::size; k++) {
+                #pragma HLS UNROLL
+                out_data[k] = in_data[k];
+            }
+            res.write(out_data);
+        }
+    }
+}
 }
 
-#endif
+#endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado/nnet_utils/nnet_types.h` & `hls4ml-0.6.0/hls4ml/templates/vivado/nnet_utils/nnet_types.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #ifndef NNET_TYPES_H_
 #define NNET_TYPES_H_
 
 #include <assert.h>
+#include <cstddef>
+#include <cstdio>
 
 namespace nnet {
 
 // Fixed-size array
 template<typename T, unsigned N>
 struct array {
     typedef T value_type;
@@ -33,8 +35,8 @@
         }
         return *this;
     }  
 };
 
 }
 
-#endif
+#endif
```

### Comparing `hls4ml-0.5.0b0/hls4ml/templates/vivado_template.py` & `hls4ml-0.6.0/hls4ml/templates/vivado_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,27 +46,29 @@
     static const unsigned stride_width = {stride_width};
     static const unsigned dilation = {dilation};
     static const unsigned out_width = {out_width};
     static const unsigned reuse_factor = {reuse};
     static const unsigned n_zeros = {nzeros};
     static const bool store_weights_in_bram = false;
     static const unsigned strategy = nnet::{strategy};
+    static const nnet::conv_implementation implementation = nnet::conv_implementation::{implementation};
     static const unsigned min_width = {min_width};
     static const ap_uint<filt_width> pixels[min_width];
     typedef {accum_t} accum_t;
     typedef {bias_t} bias_t;
     typedef {weight_t} weight_t;
     typedef {config_t} mult_config;
 }};
 const ap_uint<config{index}::filt_width> config{index}::pixels[] = {{{instructions}}};\n"""
 
 conv_mult_config_template = """struct config{index}_mult : nnet::dense_config {{
     static const unsigned n_in = {n_in};
     static const unsigned n_out = {n_out};
     static const unsigned reuse_factor = {reuse};
+    static const unsigned strategy = nnet::{strategy};
     typedef {accum_t} accum_t;
     typedef {bias_t} bias_t;
     typedef {weight_t} weight_t;
     template<class x_T, class y_T, class res_T>
     using product = nnet::product::{product_type}<x_T, y_T, res_T>;
 }};\n"""
 
@@ -86,14 +88,15 @@
     static const unsigned stride_width = {stride_width};
     static const unsigned out_height = {out_height};
     static const unsigned out_width = {out_width};
     static const unsigned reuse_factor = {reuse};
     static const unsigned n_zeros = {nzeros};
     static const bool store_weights_in_bram = false;
     static const unsigned strategy = nnet::{strategy};
+    static const nnet::conv_implementation implementation = nnet::conv_implementation::{implementation};
     static const unsigned min_height = {min_height};
     static const unsigned min_width = {min_width};
     static const ap_uint<filt_height * filt_width> pixels[min_height * min_width];
     typedef {accum_t} accum_t;
     typedef {bias_t} bias_t;
     typedef {weight_t} weight_t;
     typedef {config_t} mult_config;
@@ -114,63 +117,76 @@
 }};\n"""
 
 softmax_config_template = """struct {type}_config{index} : nnet::activ_config {{
     static const unsigned n_in = {n_in};
     static const unsigned table_size = {table_size};
     static const unsigned io_type = nnet::{iotype};
     static const unsigned reuse_factor = {reuse};
+    static const unsigned axis = {axis};
     static const nnet::softmax_implementation implementation = nnet::softmax_implementation::{implementation};
     typedef {exp_table_t} exp_table_t;
     typedef {inv_table_t} inv_table_t;
 }};\n"""
 
 pooling1d_config_template = """struct config{index} : nnet::pooling1d_config {{
     static const unsigned n_in = {n_in};
     static const unsigned n_out = {n_out};
     static const unsigned n_filt = {n_filt};
     static const unsigned pool_width = {pool_width};
     static const unsigned pad_left = {pad_left};
     static const unsigned pad_right = {pad_right};
     static const unsigned stride_width = {stride_width};
     static const nnet::Pool_Op pool_op = nnet::{pool_op};
+    static const nnet::conv_implementation implementation = nnet::conv_implementation::{implementation};
+    static const unsigned reuse = {reuse};
+    static const unsigned filt_width = {pool_width};
+    static const unsigned n_chan = {n_filt};
+    typedef {accum_t} accum_t;
 }};\n"""
 
 pooling2d_config_template = """struct config{index} : nnet::pooling2d_config {{
     static const unsigned in_height = {in_height};
     static const unsigned in_width = {in_width};
     static const unsigned n_filt = {n_filt};
     static const unsigned stride_height = {stride_height};
     static const unsigned stride_width = {stride_width};
     static const unsigned pool_height = {pool_height};
     static const unsigned pool_width = {pool_width};
+
+    static const unsigned filt_height = {pool_height};
+    static const unsigned filt_width = {pool_width};
+    static const unsigned n_chan = {n_filt};
+
     static const unsigned out_height = {out_height};
     static const unsigned out_width = {out_width};
     static const unsigned pad_top = {pad_top};
     static const unsigned pad_bottom = {pad_bottom};
     static const unsigned pad_left = {pad_left};
     static const unsigned pad_right = {pad_right};
     static const nnet::Pool_Op pool_op = nnet::{pool_op};
+    static const nnet::conv_implementation implementation = nnet::conv_implementation::{implementation};
     static const unsigned reuse = {reuse};
+    typedef {accum_t} accum_t;
 }};\n"""
 
 global_pooling1d_config_template = """struct config{index} : nnet::pooling1d_config {{
     static const unsigned n_in = {n_in};
-    static const unsigned n_out = {n_out};
-    static const unsigned pad_left = {pad_left};
-    static const unsigned pad_right = {pad_right};
-    static const unsigned stride = {stride};
+    static const unsigned n_filt = {n_filt};
     static const nnet::Pool_Op pool_op = nnet::{pool_op};
+    static const unsigned reuse = {reuse};
+    typedef {accum_t} accum_t;
 }};\n"""
 
 global_pooling2d_config_template = """struct config{index} : nnet::pooling2d_config {{
     static const unsigned in_height = {in_height};
     static const unsigned in_width = {in_width};
     static const unsigned n_filt = {n_filt};
     static const nnet::Pool_Op pool_op = nnet::{pool_op};
     static const unsigned reuse = {reuse};
+    typedef {accum_t} accum_t;
 }};\n"""
 
 zeropad1d_config_template = """struct config{index} : nnet::padding1d_config {{
     static const unsigned in_width = {in_width};
     static const unsigned n_chan = {n_chan};
     static const unsigned out_width = {out_width};
     static const unsigned pad_left = {pad_left};
@@ -194,40 +210,42 @@
 }};\n"""
 
 dot_config_template = """struct config{index} : nnet::dot_config {{
     static const unsigned n_in = {n_in};
     static const unsigned n_out = {n_out};
     static const unsigned reuse_factor = {reuse};
     typedef {accum_t} accum_t;
+    template<class x_T, class y_T, class res_T>
+    using product = nnet::product::{product_type}<x_T, y_T, res_T>;
 }};\n"""
 
 concat_config_template = """struct config{index} : nnet::concat_config {{
     static const unsigned n_elem1_0 = {n_elem1_0};
     static const unsigned n_elem1_1 = {n_elem1_1};
     static const unsigned n_elem1_2 = {n_elem1_2};
     static const unsigned n_elem2_0 = {n_elem2_0};
     static const unsigned n_elem2_1 = {n_elem2_1};
     static const unsigned n_elem2_2 = {n_elem2_2};
 
-    static const unsigned axis = {axis};
+    static const int axis = {axis};
 }};\n"""
 
 resize_config_template = """struct config{index} : nnet::resize_config {{
     static const unsigned height = {in_height};
     static const unsigned width = {in_width};
     static const unsigned n_chan = {n_chan};
     static const unsigned new_height = {out_height};
     static const unsigned new_width = {out_width};
 }};\n"""
 
 transpose_config_template = """struct config{index} : nnet::transpose_config {{
     static const unsigned depth = {depth};
     static const unsigned height = {height};
     static const unsigned width = {width};
-    static const unsigned perm[3] = {{{perm_str}}};
+    static constexpr unsigned perm[3] = {{{perm_str}}};
 }};\n"""
 
 garnet_common_config_template = """
     static const unsigned n_vertices = {n_vertices};
     static const unsigned n_vertices_width = {n_vertices_width};
     static const unsigned n_in_features = {n_in_features};
     static const unsigned distance_width = {distance_width};
@@ -335,21 +353,21 @@
 sepconv1d_function_template = 'nnet::separable_conv_1d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output}, {d}, {p}, {z}, {b});'
 sepconv2d_function_template = 'nnet::separable_conv_2d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output}, {d}, {p}, {z}, {b});'
 depthconv2d_function_template = 'nnet::depthwise_conv_2d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output}, {w}, {b});'
 activ_function_template = 'nnet::{activation}<{input_t}, {output_t}, {config}>({input}, {output});'
 param_activ_function_template = 'nnet::{activation}<{input_t}, {output_t}, {config}>({input}, {param}, {output});'
 pooling1d_function_template = 'nnet::pooling1d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output});'
 pooling2d_function_template = 'nnet::pooling2d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output});'
-global_pooling1d_function_template = 'nnet::global_pooling1d<{input_t}, {config}>({input}, {output});'
+global_pooling1d_function_template = 'nnet::global_pooling1d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output});'
 global_pooling2d_function_template = 'nnet::global_pooling2d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output});'
 zeropad1d_function_template = 'nnet::zeropad1d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output});'
 zeropad2d_function_template = 'nnet::zeropad2d_{data_format}<{input_t}, {output_t}, {config}>({input}, {output});'
 merge_function_template = 'nnet::{merge}<{input1_t}, {input2_t}, {output_t}, {config}>({input1}, {input2}, {output});'
 resize_function_template = 'nnet::resize_{algorithm}<{input_t}, {config}>({input}, {output});'
-transpose_function_template = 'nnet::transpose{dim}<{input_t}, {config}>({input}, {output});'
+transpose_function_template = 'nnet::transpose_{dim}<{input_t}, {config}>({input}, {output});'
 garnet_function_template = 'nnet::garnet{impl}<{input_t}, {integer_input_t}, {output_t}, {config}>({input}, {nvtx}, {output});'
 garnet_stack_function_template = 'nnet::garnet_stack<{input_t}, {integer_input_t}, {output_t}, {config}>({input}, {nvtx}, {output});'
 
 dense_include_list = ['nnet_utils/nnet_dense.h', 'nnet_utils/nnet_dense_compressed.h', 'nnet_utils/nnet_dense_stream.h']
 batchnorm_include_list = ['nnet_utils/nnet_batchnorm.h', 'nnet_utils/nnet_batchnorm_stream.h']
 conv1d_include_list = ['nnet_utils/nnet_conv1d.h', 'nnet_utils/nnet_conv1d_stream.h']
 conv2d_include_list = ['nnet_utils/nnet_conv2d.h', 'nnet_utils/nnet_conv2d_stream.h']
@@ -360,42 +378,54 @@
 padding_include_list = ['nnet_utils/nnet_padding.h', 'nnet_utils/nnet_padding_stream.h']
 merge_include_list = ['nnet_utils/nnet_merge.h', 'nnet_utils/nnet_merge_stream.h']
 resize_include_list = ['nnet_utils/nnet_image.h', 'nnet_utils/nnet_image_stream.h']
 transpose_include_list = ['nnet_utils/nnet_array.h']
 garnet_include_list = ['nnet_utils/nnet_garnet.h']
 
 class VivadoBackend(Backend):
-    def __init__(self):
-        super(VivadoBackend, self).__init__('Vivado')
+    def __init__(self, name='Vivado'):
+        super(VivadoBackend, self).__init__(name)
         self.register_templates('Dense', dense_function_template, dense_config_template, dense_include_list)
         self.register_templates('BinaryDense'            , dense_function_template,       dense_config_template, dense_include_list)
         self.register_templates('BatchNormalization'     , batchnorm_function_template,   batchnorm_config_template, batchnorm_include_list)
         self.register_templates('Conv1D'                 , conv1d_function_template,      [conv1d_config_template, conv_mult_config_template], conv1d_include_list)
         self.register_templates('Conv2D'                 , conv2d_function_template,      [conv2d_config_template, conv_mult_config_template], conv2d_include_list)
+        self.register_templates('Conv2DBatchnorm'        , conv2d_function_template,      [conv2d_config_template, conv_mult_config_template], conv2d_include_list)
         self.register_templates('SeparableConv1D'        , sepconv1d_function_template,   [sepconv_config_template, conv1d_config_template, conv1d_config_template, conv_mult_config_template, conv_mult_config_template], sepconv1d_include_list)
         self.register_templates('SeparableConv2D'        , sepconv2d_function_template,   [sepconv_config_template, conv2d_config_template, conv2d_config_template, conv_mult_config_template, conv_mult_config_template], sepconv2d_include_list)
         self.register_templates('DepthwiseConv2D'        , depthconv2d_function_template, [conv2d_config_template, conv_mult_config_template], sepconv2d_include_list)
         self.register_templates('Activation'             , activ_function_template,       activ_config_template, activ_include_list)
         self.register_templates('ParametrizedActivation' , param_activ_function_template, activ_config_template, activ_include_list)
         self.register_templates('PReLU'                  , param_activ_function_template, activ_config_template, activ_include_list)
         self.register_templates('Softmax'                , activ_function_template,       softmax_config_template, activ_include_list)
+        self.register_templates('TernaryTanh'            , activ_function_template,       activ_config_template, activ_include_list)
         self.register_templates('Pooling1D'              , pooling1d_function_template,   pooling1d_config_template, pooling_include_list)
         self.register_templates('Pooling2D'              , pooling2d_function_template,   pooling2d_config_template, pooling_include_list)
         self.register_templates('GlobalPooling1D'        , global_pooling1d_function_template,   global_pooling1d_config_template, pooling_include_list)
         self.register_templates('GlobalPooling2D'        , global_pooling2d_function_template,   global_pooling2d_config_template, pooling_include_list)
         self.register_templates('ZeroPadding1D'          , zeropad1d_function_template,   zeropad1d_config_template, padding_include_list)
         self.register_templates('ZeroPadding2D'          , zeropad2d_function_template,   zeropad2d_config_template, padding_include_list)
         self.register_templates('Merge'                  , merge_function_template,       merge_config_template, merge_include_list)
         self.register_templates('Concatenate'            , merge_function_template,       concat_config_template, merge_include_list)
         self.register_templates('Dot'                    , merge_function_template,       dot_config_template, merge_include_list)
         self.register_templates('Resize'                 , resize_function_template,      resize_config_template, resize_include_list)
         self.register_templates('Transpose'              , transpose_function_template,   transpose_config_template, transpose_include_list)
         self.register_templates('GarNet'                 , garnet_function_template,      garnet_config_template, garnet_include_list)
         self.register_templates('GarNetStack'            , garnet_stack_function_template,garnet_stack_config_template, garnet_include_list)        
     
+    def create_initial_config(self, part='xcku115-flvb2104-2-i', board=None, clock_period=5, io_type='io_parallel'):
+        config = {}
+        config['XilinxPart'] = part if part is not None else 'xcku115-flvb2104-2-i'
+        config['Board'] = board
+        config['ClockPeriod'] = clock_period
+        config['IOType'] = io_type
+        config['HLSConfig'] = {}
+
+        return config
+    
     def get_valid_reuse_factors(self, layer):
         n_in = 0
         n_out = 0
         if 'Dense' in layer.__class__.__name__:
             n_in = layer.get_attr('n_in')
             n_out = layer.get_attr('n_out')
         elif 'Conv1D' in layer.__class__.__name__:
@@ -452,14 +482,38 @@
         valid_rf = self.get_valid_reuse_factors(layer)
         chosen_rf = layer.reuse_factor
         if chosen_rf not in valid_rf:
             closest_rf = self.get_closest_reuse_factor(valid_rf, chosen_rf)
             print('WARNING: Invalid ReuseFactor={} with "Resource" strategy in layer "{}". Using ReuseFactor={} instead. Valid ReuseFactor(s): {}.'
                 .format(chosen_rf, layer.name, closest_rf, ','.join(map(str, valid_rf))))
             layer.reuse_factor = closest_rf
+    
+    def set_target_reuse_factor(self, layer):
+        targ_cycles = layer.target_cycles
+
+        shuffle_cycles = 6 # Number of clock cycles to move data around
+        if targ_cycles is not None:
+            if 'Dense' in layer.__class__.__name__: 
+                kernel_multiplies = layer.get_attr('n_out')
+            elif 'Conv1D' in layer.__class__.__name__:  
+                kernel_multiplies = layer.get_attr('out_width')
+            elif 'Conv2D' in layer.__class__.__name__: 
+                kernel_multiplies = layer.get_attr('out_height') * layer.get_attr('out_width')
+            else: 
+                print('Target cycles unsupported layer')
+                return
+
+            if targ_cycles < shuffle_cycles*kernel_multiplies: # 6 clock min (6 * out_height * out_width)
+                print("Latency can not be achieved with current target %d. Mininum %d." % (targ_cycles, shuffle_cycles*kernel_multiplies+1))
+                return
+            else: 
+                rf = targ_cycles - shuffle_cycles*kernel_multiplies # subtract data shuffling overhead
+
+            layer.reuse_factor = float(rf) / kernel_multiplies
+
 
     def convert_precision_string(self, precision):
         '''
         Convert a precision string (e.g. "ap_fixed<16,6>" to the internal IntegerPrecisionTypes etc)
         '''
         from hls4ml.model.hls_layers import IntegerPrecisionType, FixedPrecisionType
         import re
@@ -469,24 +523,24 @@
         sat_mode = None
         round_mode = None
         sat_bits = None
         if 'fixed' in precision:
             W = int(bits[0])
             I = int(bits[1])
             fields = 2
-            signed = ~('u' in precision)
+            signed = not ('u' in precision)
         elif 'int' in precision:
             W = int(bits[0])
             I = W
             fields = 1
-            signed = ~('u' in precision)
+            signed = not ('u' in precision)
         if len(bits) > fields:
-            sat_mode = bits[fields]
+            round_mode = bits[fields]
         if len(bits) > fields+1:
-            round_mode = bits[fields+1]
+            sat_mode = bits[fields+1]
         if len(bits) > fields+2:
             sat_bits = int(bits[fields+2])
         if 'fixed' in precision:
             return FixedPrecisionType(W, I, signed, round_mode, sat_mode, sat_bits)
         elif 'int' in precision:
             return IntegerPrecisionType(W, signed)
 
@@ -501,26 +555,32 @@
             product = 'weight_exponential'
         else:
             # if binary
             if isinstance(weight_T, XnorPrecisionType) and isinstance(data_T, XnorPrecisionType):
                 product = 'both_binary'
             elif isinstance(weight_T, XnorPrecisionType): # data is not xnor-binary
                 product = 'weight_binary'
+            elif isinstance(data_T, XnorPrecisionType): # data is xnor, weight is not
+                product = 'data_binary'
             elif isinstance(weight_T, IntegerPrecisionType) and weight_T.width == 2 and weight_T.signed:
                 product = 'weight_ternary'
             else:
                 product = 'mult'
         return product
 
     def compute_conv1d_instructions(self, in_W, in_C, kernel_size=3, stride=1, pad=0):
 
         # Current limitations
         assert pad == 0
 
-        min_W = (math.ceil(kernel_size / stride) - 1) * stride + kernel_size
+        if kernel_size >= stride:
+            min_W = (math.ceil(kernel_size / stride) - 1) * stride + kernel_size
+        else:
+            min_W = (math.ceil(stride / kernel_size) - 1) * stride + kernel_size
+
         min_oW = int((min_W - kernel_size) // stride + 1)
 
         out_W = int((in_W - kernel_size) // stride + 1)
         scaled_W = (out_W - 1) * stride + kernel_size
 
         if scaled_W < in_W:
             min_W += 1
@@ -556,16 +616,24 @@
             stride_width = stride
 
         # Current limitations
         assert kernel_height == kernel_width
         assert stride_height == stride_width
         assert pad == 0
 
-        min_H = (math.ceil(kernel_height / stride_height) - 1) * stride_height + kernel_height
-        min_W = (math.ceil(kernel_width / stride_width) - 1) * stride_width + kernel_width
+        if kernel_height >= stride_height:
+            min_H = (math.ceil(kernel_height / stride_height) - 1) * stride_height + kernel_height
+        else:
+            min_H = (math.ceil(stride_height / kernel_height) - 1) * stride_height + kernel_height
+        
+        if kernel_width >= stride_width:
+            min_W = (math.ceil(kernel_width / stride_width) - 1) * stride_width + kernel_width
+        else:
+            min_W = (math.ceil(stride_width / kernel_width) - 1) * stride_width + kernel_width
+
         min_oH = int((min_H - kernel_height) // stride_height + 1)
         min_oW = int((min_W - kernel_width) // stride_width + 1)
 
         out_H = int((in_H - kernel_height) // stride_height + 1)
         out_W = int((in_W - kernel_width) // stride_width + 1)
         scaled_H = (out_H - 1) * stride_height + kernel_height
         scaled_W = (out_W - 1) * stride_width + kernel_width
```

### Comparing `hls4ml-0.5.0b0/hls4ml/utils/example_models.py` & `hls4ml-0.6.0/hls4ml/utils/example_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib.request import urlretrieve
-from .config import create_vivado_config
+from .config import create_config
 import pprint
 import json
 import yaml
 
 def _load_data_config_avai(model_name):
     """
     Check data and configuration availability for each model from this file:
@@ -28,18 +28,18 @@
 
 def _config_is_available(model_name):
 
     data = _load_data_config_avai(model_name)
 
     return data['example_config']
 
-def _create_default_config(model_name, model_config):
+def _create_default_config(model_name, model_config, backend):
 
     #Initiate the configuration file
-    config = create_vivado_config()
+    config = create_config(backend=backend)
 
     #Additional configuration parameters
     config[model_config] = model_name
     config['HLSConfig']['Model'] = {}
     config['HLSConfig']['Model']['Precision'] = 'ap_fixed<16,6>'
     config['HLSConfig']['Model']['ReuseFactor'] = '1'
 
@@ -84,19 +84,19 @@
     link_to_config = 'https://raw.githubusercontent.com/hls-fpga-machine-learning/example-models/master/config-files/' + config_name
 
     #Load the configuration as dictionary from file
     urlretrieve(link_to_config, config_name)
 
     #Load the configuration from local yml file
     with open(config_name, 'r') as ymlfile:
-        config = yaml.load(ymlfile)
+        config = yaml.safe_load(ymlfile)
 
     return config
 
-def fetch_example_model(model_name):
+def fetch_example_model(model_name, backend='Vivado'):
     """
     Download an example model (and example data & configuration if available) from github repo to working directory, and return the corresponding configuration:
 
     https://github.com/hls-fpga-machine-learning/example-models
 
     Use fetch_example_list() to see all the available models.
 
@@ -126,27 +126,27 @@
         model_type = 'tensorflow'
         model_config = 'TensorFlowModel'
     else:
         raise TypeError('Model type is not supported in hls4ml.')
     
 
     download_link_model = download_link + model_type + '/' + model_name
-    
+
     #Download the example model
     print("Downloading example model files ...")
     urlretrieve(download_link_model, model_name)
 
     #Check if the example data and configuration for the model are available
     if _data_is_available(model_name):
         _load_example_data(model_name)
 
     if _config_is_available(model_name):
         config = _load_example_config(model_name)
     else:
-        config = _create_default_config(model_name, model_config)
+        config = _create_default_config(model_name, model_config, backend)
 
     #If the model is a keras model then have to download its weight file as well
     if model_type == 'keras':
         model_weight_name = model_name[:-5] + "_weights.h5"
 
         download_link_weight = download_link + model_type + '/' + model_weight_name
         urlretrieve(download_link_weight, model_weight_name)
@@ -162,8 +162,8 @@
     temp_file, _ = urlretrieve(link_to_list)
     
     # Read data from file:
     data = json.load(open(temp_file))
     
     # Print in fancy format
     pp = pprint.PrettyPrinter(indent=4)
-    pp.pprint(data)
+    pp.pprint(data)
```

### Comparing `hls4ml-0.5.0b0/hls4ml/utils/plot.py` & `hls4ml-0.6.0/hls4ml/utils/plot.py`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/hls4ml/writer/vivado_writer.py` & `hls4ml-0.6.0/hls4ml/writer/vivado_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import re
 import glob
 from collections import OrderedDict
 
 from hls4ml.writer.writers import Writer
 from hls4ml.model.hls_layers import XnorPrecisionType
 
+config_filename = 'hls4ml_config.yml'
+
 class VivadoWriter(Writer):
 
     def type_definition_cpp(self, model, atype):
         type_class = atype.__class__.__name__
         if type_class == 'HLSType':
             return 'typedef {precision} {name};\n'.format(name=atype.name, precision=atype.precision)
         elif type_class == 'CompressedType':
@@ -137,30 +139,34 @@
 
         filedir = os.path.dirname(os.path.abspath(__file__))
         f = open(os.path.join(filedir,'../templates/vivado/firmware/myproject.cpp'),'r')
         fout = open('{}/firmware/{}.cpp'.format(model.config.get_output_dir(), model.config.get_project_name()),'w')
 
         model_inputs = model.get_input_variables()
         model_outputs = model.get_output_variables()
+        model_brams   = model.get_bram_variables()
 
         indent = '    '
 
         for line in f.readlines():
             #Add headers to weights and biases
             if 'myproject' in line:
                 newline = line.replace('myproject', model.config.get_project_name())
             elif '//hls-fpga-machine-learning insert header' in line:
                 inputs_str = ', '.join([self.variable_definition_cpp(model, i, as_reference=True) for i in model_inputs])
                 outputs_str = ', '.join([self.variable_definition_cpp(model, o, as_reference=True) for o in model_outputs])
+                brams_str  = ', \n'.join([indent + self.variable_definition_cpp(model, b, as_reference=False) for b in model_brams])
                 insize_str = ', '.join(['unsigned short &const_size_in_{}'.format(i) for i in range(1, len(model_inputs) + 1)])
                 outsize_str = ', '.join(['unsigned short &const_size_out_{}'.format(i) for i in range(1, len(model_outputs) + 1)])
 
                 newline = ''
                 newline += indent + inputs_str + ',\n'
                 newline += indent + outputs_str + ',\n'
+                if len(model_brams) > 0: 
+                    newline += brams_str + ',\n'
                 newline += indent + insize_str + ',\n'
                 newline += indent + outsize_str + '\n'
 
             elif '//hls-fpga-machine-learning insert load weights' in line:
                 newline = line
                 for layer in model.get_layers():
                     for w in layer.get_weights():
@@ -172,28 +178,31 @@
                             newline += indent + '    nnet::load_weights_from_txt<{}, {}>({}, "{}.txt");\n'.format(w.type.name, w.data_length, w.name, w.name)
 
             #Add input/output type
             elif '//hls-fpga-machine-learning insert IO' in line:
                 newline = line
                 all_inputs = [i.cppname for i in model_inputs]
                 all_outputs = [o.cppname for o in model_outputs]
+                all_brams = [b.cppname for b in model_brams] 
                 io_type = model.config.get_config_value("IOType")
 
                 if io_type == 'io_parallel':
                     for i in model_inputs: newline += indent + self._make_array_pragma(i) + '\n'
                     for o in model_outputs: newline += indent + self._make_array_pragma(o) + '\n'
                     # TODO discussed adding a handle for setting the interface mode for individual input and output arrays (16.03.2020)
                     # Probably the handle doesn't need to be exposed to the user but should be just set in hls_model.py
                     newline += indent + '#pragma HLS INTERFACE ap_vld port={},{} \n'.format(','.join(all_inputs), ','.join(all_outputs))
-                    if model.config.model_strategy == 'Resource':
+                    if model.config.model_strategy.lower() == 'resource':
                         newline += indent + '#pragma HLS DATAFLOW \n'
                     else:
                         newline += indent + '#pragma HLS PIPELINE \n'
                 if io_type == 'io_serial' or io_type == 'io_stream':
                     newline += indent + '#pragma HLS INTERFACE axis port={},{} \n'.format(','.join(all_inputs), ','.join(all_outputs))
+                    if all_brams: # No BRAM ports
+                        newline += indent + '#pragma HLS INTERFACE bram port={} \n'.format(','.join(all_brams))
                     newline += indent + '#pragma HLS DATAFLOW \n'
 
                 inval_str = '\n    '.join(['const_size_in_{} = {};'.format(i, inp.size_cpp()) for i, inp in enumerate(model_inputs, 1)])
                 outval_str = '\n    '.join(['const_size_out_{} = {};'.format(i, out.size_cpp()) for i, out in enumerate(model_outputs, 1)])
                 newline += '\n' + indent + inval_str
                 newline += '\n' + indent + outval_str
                 newline += '\n'
@@ -242,32 +251,36 @@
 
         filedir = os.path.dirname(os.path.abspath(__file__))
         f = open(os.path.join(filedir,'../templates/vivado/firmware/myproject.h'),'r')
         fout = open('{}/firmware/{}.h'.format(model.config.get_output_dir(), model.config.get_project_name()),'w')
 
         model_inputs = model.get_input_variables()
         model_outputs = model.get_output_variables()
+        model_brams   = model.get_bram_variables()
 
         indent = '    '
 
         for line in f.readlines():
 
             if 'MYPROJECT' in line:
                 newline = line.replace('MYPROJECT',format(model.config.get_project_name().upper()))
             elif 'void myproject(' in line:
                 newline = 'void {}(\n'.format(model.config.get_project_name())
             elif '//hls-fpga-machine-learning insert header' in line:
                 inputs_str = ', '.join([self.variable_definition_cpp(model, i, as_reference=True) for i in model_inputs])
                 outputs_str = ', '.join([self.variable_definition_cpp(model, o, as_reference=True) for o in model_outputs])
+                brams_str  = ', \n'.join([indent + self.variable_definition_cpp(model, b, as_reference=False) for b in model_brams])
                 insize_str = ', '.join(['unsigned short &const_size_in_{}'.format(i) for i in range(1, len(model_inputs) + 1)])
                 outsize_str = ', '.join(['unsigned short &const_size_out_{}'.format(o) for o in range(1, len(model_outputs) + 1)])
 
                 newline = ''
                 newline += indent + inputs_str + ',\n'
                 newline += indent + outputs_str + ',\n'
+                if len(model_brams) > 0: 
+                    newline += brams_str + ',\n'
                 newline += indent + insize_str + ',\n'
                 newline += indent + outsize_str + '\n'
             else:
                 newline = line
             fout.write(newline)
 
         f.close()
@@ -290,15 +303,14 @@
                 newline = line
                 all_precision = OrderedDict()
                 for layer in model.get_layers():
                     layer_precision = layer.get_layer_precision()
                     all_precision.update(layer_precision)
                 for used_type in all_precision.values():
                     newline += self.type_definition_cpp(model, used_type)
-
             else:
                 newline = line
             fout.write(newline)
         f.close()
         fout.close()
 
     def write_parameters(self, model):
@@ -313,15 +325,18 @@
                 for include in sorted(set(sum((layer.include_list for layer in model.get_layers()), []))):
                     newline += '#include "%s"\n' % include
 
             elif '//hls-fpga-machine-learning insert weights' in line:
                 newline = line
                 for layer in model.get_layers():
                     for w in layer.get_weights():
-                        newline += '#include "weights/{}.h"\n'.format(w.name)
+                        if w.name not in model.bram_vars.keys():
+                            newline += '#include "weights/{}.h"\n'.format(w.name)
+                        else:
+                            newline += '// #include "weights/{}.h"\n'.format(w.name)
 
             elif "//hls-fpga-machine-learning insert layer-config" in line:
                 newline = line
                 for layer in model.get_layers():
                     config = layer.config_cpp()
                     if config:
                         newline += '// ' + layer.name + '\n'
@@ -393,17 +408,23 @@
 
         for line in f.readlines():
             indent = ' ' * (len(line) - len(line.lstrip(' ')))
 
             #Insert numbers
             if 'myproject' in line:
                 newline = line.replace('myproject', model.config.get_project_name())
+            elif '//hls-fpga-machine-learning insert bram' in line:
+                newline = line
+                for bram in model.get_bram_variables():
+                    newline += '#include \"firmware/weights/{}.h\"\n'.format(bram.cppname)
             elif '//hls-fpga-machine-learning insert data' in line:
                 newline = line
                 offset = 0
+                # for bram in model.get_bram_variables():
+                #     newline += bram.definition_cpp()+';\n'
                 for inp in model.get_input_variables():
                     newline += '      ' + self.variable_definition_cpp(model, inp) + ';\n'
                     newline += '      nnet::copy_data<float, {}, {}, {}>(in, {});\n'.format(inp.type.name, offset, inp.size_cpp(), inp.cppname)
                     offset += inp.size()
                 for out in model.get_output_variables():
                     newline += '      ' + self.variable_definition_cpp(model, out) + ';\n'
             elif '//hls-fpga-machine-learning insert zero' in line:
@@ -419,15 +440,21 @@
                 size_str = indent + 'unsigned short {},{};\n'
                 input_size_vars = ','.join(['size_in{}'.format(i) for i in range(1, len(model.get_input_variables()) + 1)])
                 output_size_vars = ','.join(['size_out{}'.format(o) for o in range(1, len(model.get_output_variables()) + 1)])
                 newline += size_str.format(input_size_vars, output_size_vars)
 
                 input_vars = ','.join([i.cppname for i in model.get_input_variables()])
                 output_vars = ','.join([o.cppname for o in model.get_output_variables()])
-                top_level = indent + '{}({},{},{},{});\n'.format(model.config.get_project_name(), input_vars, output_vars, input_size_vars, output_size_vars)
+                bram_vars   =','.join([b.cppname for b in model.get_bram_variables()]) 
+
+                # Concatenate the input, output, and bram variables. Filter out empty/null values
+                all_vars = ','.join(filter(None, [input_vars, output_vars, bram_vars]))
+
+                top_level = indent + '{}({},{},{});\n'.format(model.config.get_project_name(), all_vars, input_size_vars, output_size_vars)
+                
                 newline += top_level
             elif '//hls-fpga-machine-learning insert predictions' in line:
                 newline = line
                 for out in model.get_output_variables():
                     newline += indent + 'for(int i = 0; i < {}; i++) {{\n'.format(out.size_cpp())
                     newline += indent + '  std::cout << pr[i] << " ";\n'
                     newline += indent + '}\n'
@@ -453,23 +480,28 @@
 
         filedir = os.path.dirname(os.path.abspath(__file__))
         f = open(os.path.join(filedir,'../templates/vivado/myproject_bridge.cpp'),'r')
         fout = open('{}/{}_bridge.cpp'.format(model.config.get_output_dir(), model.config.get_project_name()),'w')
 
         model_inputs = model.get_input_variables()
         model_outputs = model.get_output_variables()
+        model_brams   = model.get_bram_variables()
 
         indent = '    '
 
         for line in f.readlines():
 
             if 'MYPROJECT' in line:
                 newline = line.replace('MYPROJECT', format(model.config.get_project_name().upper()))
             elif 'myproject' in line:
                 newline = line.replace('myproject', format(model.config.get_project_name()))
+            elif '//hls-fpga-machine-learning insert bram' in line:
+                newline = line
+                for bram in model_brams:
+                    newline += '#include \"firmware/weights/{}.h\"\n'.format(bram.cppname)
             elif '//hls-fpga-machine-learning insert header' in line:
                 dtype = line.split('#', 1)[1].strip()
                 inputs_str = ', '.join(['{type} {name}[{shape}]'.format(type=dtype, name=i.cppname, shape=i.size_cpp()) for i in model_inputs])
                 outputs_str = ', '.join(['{type} {name}[{shape}]'.format(type=dtype, name=o.cppname, shape=o.size_cpp()) for o in model_outputs])
                 insize_str = ', '.join(['unsigned short &const_size_in_{}'.format(i) for i in range(1, len(model_inputs) + 1)])
                 outsize_str = ', '.join(['unsigned short &const_size_out_{}'.format(o) for o in range(1, len(model_outputs) + 1)])
 
@@ -490,16 +522,21 @@
                     newline += indent + '{var};\n'.format(var=self.variable_definition_cpp(model, o, name_suffix='_ap'))
                 
                 newline += '\n'
 
                 input_size_vars = ','.join(['const_size_in_{}'.format(i) for i in range(1, len(model.get_input_variables()) + 1)])
                 output_size_vars = ','.join(['const_size_out_{}'.format(o) for o in range(1, len(model.get_output_variables()) + 1)])
                 input_vars = ','.join([i.cppname + '_ap' for i in model.get_input_variables()])
+                bram_vars   =','.join([b.cppname for b in model.get_bram_variables()]) 
                 output_vars = ','.join([o.cppname + '_ap' for o in model.get_output_variables()])
-                top_level = indent + '{}({}, {}, {}, {});\n'.format(model.config.get_project_name(), input_vars, output_vars, input_size_vars, output_size_vars)
+                
+                # Concatenate the input, output, and bram variables. Filter out empty/null values
+                all_vars = ','.join(filter(None, [input_vars, output_vars, bram_vars]))
+
+                top_level = indent + '{}({},{},{});\n'.format(model.config.get_project_name(), all_vars, input_size_vars, output_size_vars)
                 newline += top_level
 
                 newline += '\n'
 
                 for o in model_outputs:
                     newline += indent + 'nnet::convert_data<{}, {}, {}>({}_ap, {});\n'.format(o.type.name, dtype, o.size_cpp(), o.cppname, o.cppname)
             elif '//hls-fpga-machine-learning insert trace_outputs' in line:
@@ -599,14 +636,33 @@
         dstpath = '{}/firmware/ap_types/'.format(model.config.get_output_dir())
 
         if os.path.exists(dstpath):
             rmtree(dstpath)
 
         copytree(srcpath, dstpath)
 
+    def write_yml(self, model):
+        ###################
+        # YAML config file
+        ###################
+
+        def keras_model_representer(dumper, keras_model):
+            model_path = model.config.get_output_dir() + '/keras_model.h5'
+            keras_model.save(model_path)
+            return dumper.represent_scalar(u'!keras_model', model_path)
+
+        try:
+            from tensorflow.keras import Model as KerasModel
+            yaml.add_multi_representer(KerasModel, keras_model_representer)
+        except:
+            pass
+
+        with open(model.config.get_output_dir() + '/' + config_filename, 'w') as file:
+            yaml.dump(model.config.config, file)
+
     def write_tar(self, model):
         ###################
         # Tarball output
         ###################
 
         with tarfile.open(model.config.get_output_dir() + '.tar.gz', mode='w:gz') as archive:
             archive.add(model.config.get_output_dir(), recursive=True)
@@ -619,9 +675,10 @@
         self.write_weights(model)
         self.write_defines(model)
         self.write_parameters(model)
         self.write_test_bench(model)
         self.write_bridge(model)
         self.write_build_script(model)
         self.write_nnet_utils(model)
+        self.write_yml(model)
         self.write_tar(model)
         print('Done')
```

### Comparing `hls4ml-0.5.0b0/hls4ml.egg-info/PKG-INFO` & `hls4ml-0.6.0/hls4ml.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 Metadata-Version: 2.1
 Name: hls4ml
-Version: 0.5.0b0
+Version: 0.6.0
 Summary: Machine learning in FPGAs using HLS
 Home-page: https://github.com/hls-fpga-machine-learning/hls4ml
 Author: HLS4ML Team
 Author-email: hls4ml.help@gmail.com
 License: Apache 2.0
-Description: <p float="left">
-           <img src="https://fastmachinelearning.github.io/hls4ml/img/logo.jpg" alt="hls4ml" width="400"/>
-        </p>
-        
-        [![DOI](https://zenodo.org/badge/108329371.svg)](https://zenodo.org/badge/latestdoi/108329371)
-        [![PyPI version](https://badge.fury.io/py/hls4ml.svg)](https://badge.fury.io/py/hls4ml)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/hls4ml.svg)](https://pypi.org/project/hls4ml/)
-        
-        A package for machine learning inference in FPGAs. We create firmware implementations of machine learning algorithms using high level synthesis language (HLS). We translate traditional open-source machine learning package models into HLS that can be configured for your use-case!
-        
-        **Contact:** hls4ml.help@gmail.com
-        
-        # Documentation & Tutorial
-        
-        For more information visit the webpage: [https://fastmachinelearning.org/hls4ml/](https://fastmachinelearning.org/hls4ml/)
-        
-        Detailed tutorials on how to use `hls4ml`'s various functionalities can be found [here](https://github.com/hls-fpga-machine-learning/hls4ml-tutorial).
-        
-        # Installation
-        ```
-        pip install hls4ml
-        ```
-        
-        To install the extra dependencies for profiling: 
-        
-        ```
-        pip install hls4ml[profiling]
-        ```
-        
-        # Getting Started
-        ### Creating an HLS project
-        ```Python
-        import hls4ml
-        
-        #Fetch a keras model from our example repository
-        #This will download our example model to your working directory and return an example configuration file
-        config = hls4ml.utils.fetch_example_model('KERAS_3layer.json')
-        
-        print(config) #You can print the configuration to see some default parameters
-        
-        #Convert it to a hls project
-        hls_model = hls4ml.converters.keras_to_hls(config)
-        
-        # Print full list of example models if you want to explore more
-        hls4ml.utils.fetch_example_list()
-        ```
-        
-        ### Building a project with Xilinx Vitis (after downloading and installing from [here](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vitis.html))
-        
-        ```Python
-        #Use Vivado HLS to synthesize the model
-        #This might take several minutes
-        hls_model.build()
-        
-        #Print out the report if you want
-        hls4ml.report.read_vivado_report('my-hls-test')
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: profiling
+License-File: LICENSE
+
+<p float="left">
+   <img src="https://fastmachinelearning.github.io/hls4ml/img/logo.jpg" alt="hls4ml" width="400"/>
+</p>
+
+[![DOI](https://zenodo.org/badge/108329371.svg)](https://zenodo.org/badge/latestdoi/108329371)
+[![PyPI version](https://badge.fury.io/py/hls4ml.svg)](https://badge.fury.io/py/hls4ml)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/hls4ml.svg)](https://pypi.org/project/hls4ml/)
+
+A package for machine learning inference in FPGAs. We create firmware implementations of machine learning algorithms using high level synthesis language (HLS). We translate traditional open-source machine learning package models into HLS that can be configured for your use-case!
+
+**Contact:** hls4ml.help@gmail.com
+
+# Documentation & Tutorial
+
+For more information visit the webpage: [https://fastmachinelearning.org/hls4ml/](https://fastmachinelearning.org/hls4ml/)
+
+Detailed tutorials on how to use `hls4ml`'s various functionalities can be found [here](https://github.com/hls-fpga-machine-learning/hls4ml-tutorial).
+
+# Installation
+```
+pip install hls4ml
+```
+
+To install the extra dependencies for profiling: 
+
+```
+pip install hls4ml[profiling]
+```
+
+# Getting Started
+### Creating an HLS project
+```Python
+import hls4ml
+
+#Fetch a keras model from our example repository
+#This will download our example model to your working directory and return an example configuration file
+config = hls4ml.utils.fetch_example_model('KERAS_3layer.json')
+
+print(config) #You can print the configuration to see some default parameters
+
+#Convert it to a hls project
+hls_model = hls4ml.converters.keras_to_hls(config)
+
+# Print full list of example models if you want to explore more
+hls4ml.utils.fetch_example_list()
+```
+
+### Building a project with Xilinx Vivado HLS (after downloading and installing from [here](https://www.xilinx.com/products/design-tools/vivado/integration/esl-design.html))
+Note: Vitis HLS is not yet supported. Vivado HLS versions between 2018.2 and 2020.1 are recommended.
+
+```Python
+#Use Vivado HLS to synthesize the model
+#This might take several minutes
+hls_model.build()
+
+#Print out the report if you want
+hls4ml.report.read_vivado_report('my-hls-test')
+```
+
+
```

### Comparing `hls4ml-0.5.0b0/hls4ml.egg-info/SOURCES.txt` & `hls4ml-0.6.0/hls4ml.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -52,51 +52,68 @@
 example-prjs/sublayer/firmware/weights/w2_1.h
 example-prjs/sublayer/firmware/weights/w3.h
 example-prjs/sublayer/firmware/weights/w4.h
 hls4ml/__init__.py
 hls4ml.egg-info/PKG-INFO
 hls4ml.egg-info/SOURCES.txt
 hls4ml.egg-info/dependency_links.txt
+hls4ml.egg-info/entry_points.txt
 hls4ml.egg-info/requires.txt
 hls4ml.egg-info/top_level.txt
 hls4ml/converters/__init__.py
 hls4ml/converters/keras_to_hls.py
 hls4ml/converters/onnx_to_hls.py
 hls4ml/converters/pytorch_to_hls.py
 hls4ml/converters/tf_to_hls.py
+hls4ml/converters/utils.py
 hls4ml/converters/keras/__init__.py
 hls4ml/converters/keras/convolution.py
 hls4ml/converters/keras/core.py
 hls4ml/converters/keras/graph.py
 hls4ml/converters/keras/merge.py
 hls4ml/converters/keras/pooling.py
 hls4ml/converters/keras/qkeras.py
 hls4ml/converters/keras/qkeras_layers.py
 hls4ml/converters/keras/reshape.py
 hls4ml/converters/keras/reshaping.py
+hls4ml/converters/onnx/__init__.py
+hls4ml/converters/onnx/convolution.py
+hls4ml/converters/onnx/core.py
+hls4ml/converters/onnx/merge.py
+hls4ml/converters/onnx/pooling.py
+hls4ml/converters/onnx/reshape.py
+hls4ml/converters/pytorch/__init__.py
+hls4ml/converters/pytorch/convolution.py
+hls4ml/converters/pytorch/core.py
+hls4ml/converters/pytorch/pooling.py
 hls4ml/model/__init__.py
 hls4ml/model/hls_layers.py
 hls4ml/model/hls_model.py
 hls4ml/model/profiling.py
 hls4ml/model/optimizer/__init__.py
 hls4ml/model/optimizer/optimizer.py
 hls4ml/model/optimizer/passes/__init__.py
 hls4ml/model/optimizer/passes/bn_fuse.py
 hls4ml/model/optimizer/passes/bn_quant.py
 hls4ml/model/optimizer/passes/clone.py
 hls4ml/model/optimizer/passes/conv_same_pad.py
 hls4ml/model/optimizer/passes/fuse_biasadd.py
+hls4ml/model/optimizer/passes/multi_dense.py
 hls4ml/model/optimizer/passes/nop.py
 hls4ml/model/optimizer/passes/pointwise.py
 hls4ml/model/optimizer/passes/qkeras.py
 hls4ml/model/optimizer/passes/repack_stream.py
+hls4ml/model/optimizer/passes/transpose_opt.py
 hls4ml/report/__init__.py
 hls4ml/report/vivado_report.py
 hls4ml/templates/__init__.py
+hls4ml/templates/supported_boards.json
 hls4ml/templates/templates.py
+hls4ml/templates/vivado_accelerator_config.py
+hls4ml/templates/vivado_accelerator_template.py
 hls4ml/templates/vivado_template.py
 hls4ml/templates/vivado/build_lib.sh
 hls4ml/templates/vivado/build_prj.tcl
 hls4ml/templates/vivado/myproject_bridge.cpp
 hls4ml/templates/vivado/myproject_test.cpp
 hls4ml/templates/vivado/vivado_synth.tcl
 hls4ml/templates/vivado/ap_types/ap_common.h
@@ -105,14 +122,15 @@
 hls4ml/templates/vivado/ap_types/ap_fixed_base.h
 hls4ml/templates/vivado/ap_types/ap_fixed_ref.h
 hls4ml/templates/vivado/ap_types/ap_fixed_special.h
 hls4ml/templates/vivado/ap_types/ap_int.h
 hls4ml/templates/vivado/ap_types/ap_int_base.h
 hls4ml/templates/vivado/ap_types/ap_int_ref.h
 hls4ml/templates/vivado/ap_types/ap_int_special.h
+hls4ml/templates/vivado/ap_types/ap_shift_reg.h
 hls4ml/templates/vivado/ap_types/hls_stream.h
 hls4ml/templates/vivado/ap_types/etc/ap_private.h
 hls4ml/templates/vivado/ap_types/utils/x_hls_utils.h
 hls4ml/templates/vivado/firmware/defines.h
 hls4ml/templates/vivado/firmware/myproject.cpp
 hls4ml/templates/vivado/firmware/myproject.h
 hls4ml/templates/vivado/firmware/parameters.h
@@ -149,19 +167,28 @@
 hls4ml/templates/vivado/nnet_utils/nnet_pooling.h
 hls4ml/templates/vivado/nnet_utils/nnet_pooling_stream.h
 hls4ml/templates/vivado/nnet_utils/nnet_sepconv1d_stream.h
 hls4ml/templates/vivado/nnet_utils/nnet_sepconv2d_stream.h
 hls4ml/templates/vivado/nnet_utils/nnet_sepconv_stream.h
 hls4ml/templates/vivado/nnet_utils/nnet_stream.h
 hls4ml/templates/vivado/nnet_utils/nnet_types.h
+hls4ml/templates/vivado_accelerator/build_lib.sh
+hls4ml/templates/vivado_accelerator/myproject_axi.cpp
+hls4ml/templates/vivado_accelerator/myproject_axi.h
+hls4ml/templates/vivado_accelerator/pynq-z2/python_drivers/axi_stream_driver.py
+hls4ml/templates/vivado_accelerator/pynq-z2/tcl_scripts/axi_lite_design.tcl
+hls4ml/templates/vivado_accelerator/pynq-z2/tcl_scripts/axi_stream_design.tcl
+hls4ml/templates/vivado_accelerator/zcu102/python_drivers/axi_stream_driver.py
+hls4ml/templates/vivado_accelerator/zcu102/tcl_scripts/axi_stream_design.tcl
 hls4ml/utils/__init__.py
 hls4ml/utils/config.py
 hls4ml/utils/example_models.py
 hls4ml/utils/plot.py
 hls4ml/writer/__init__.py
+hls4ml/writer/vivado_accelerator_writer.py
 hls4ml/writer/vivado_writer.py
 hls4ml/writer/writers.py
 scripts/hls4ml
 test/build-prj.sh
 test/cleanup.sh
 test/compare-reports.sh
 test/convert-keras-models.sh
@@ -176,8 +203,17 @@
 test/onnx-models.txt
 test/onnx-to-hls.sh
 test/pytorch-models.txt
 test/pytorch-to-hls.sh
 test/docker/Dockerfile
 test/docker/README.md
 test/docker/install_config-2017.2.txt
-test/docker/install_config.txt
+test/docker/install_config.txt
+test/pytest/ci-template.yml
+test/pytest/generate_ci_yaml.py
+test/pytest/test_cnn_mnist.py
+test/pytest/test_conv1d.py
+test/pytest/test_globalpooling1d.py
+test/pytest/test_graph.py
+test/pytest/test_keras_api.py
+test/pytest/test_qkeras.py
+test/pytest/test_softmax.py
```

### Comparing `hls4ml-0.5.0b0/scripts/hls4ml` & `hls4ml-0.6.0/scripts/hls4ml`

 * *Files 4% similar despite different names*

```diff
@@ -17,33 +17,30 @@
 hls4ml_description = """
 
         ╔╧╧╧╗────o
     hls ║ 4 ║ ml   - Machine learning inference in FPGAs
    o────╚╤╤╤╝
 """
 
-def parse_config(config_file):
-    print('Loading configuration from', config_file)
-    config = open(config_file, 'r')
-    return yaml.load(config, Loader=yaml.SafeLoader)
-
 def main():
     parser = argparse.ArgumentParser(description=hls4ml_description, formatter_class=argparse.RawDescriptionHelpFormatter)
     subparsers = parser.add_subparsers()
     
     config_parser = subparsers.add_parser('config', help='Create a conversion configuration file')
     convert_parser = subparsers.add_parser('convert', help='Convert Keras or ONNX model to HLS')
     build_parser = subparsers.add_parser('build', help='Build generated HLS project')
     report_parser = subparsers.add_parser('report', help='Show synthesis report of an HLS project')
 
     config_parser.add_argument('-m', '--model', help='Model file to convert (Keras .h5 or .json file, ONNX .onnx file, or TensorFlow .pb file)', default=None)
     config_parser.add_argument('-w', '--weights', help='Optional weights file (if Keras .json file is provided))', default=None)
     config_parser.add_argument('-p', '--project', help='Project name', default='myproject')
     config_parser.add_argument('-d', '--dir', help='Project output directory', default='my-hls-test')
     config_parser.add_argument('-f', '--fpga', help='FPGA part', default='xcku115-flvb2104-2-i')
+    config_parser.add_argument('-bo', '--board', help='Board used.', default='pynq-z2')
+    config_parser.add_argument('-ba', '--backend', help='Backend to use (Vivado, VivadoAccelerator)', default='Vivado')
     config_parser.add_argument('-c', '--clock', help='Clock frequency (ns)', type=int, default=5)
     config_parser.add_argument('-g', '--granularity', help='Granularity of configuration. One of "model", "type" or "name"', default='model')
     config_parser.add_argument('-x', '--precision', help='Default precision', default='ap_fixed<16,6>')
     config_parser.add_argument('-r', '--reuse-factor', help='Default reuse factor', type=int, default=1)
     config_parser.add_argument('-o', '--output', help='Output file name', default=None)
     config_parser.set_defaults(func=config)
     
@@ -74,18 +71,20 @@
         parser.print_usage()
 
 def config(args):
     if args.model is None:
         print('Model file (-m or --model) must be provided.')
         sys.exit(1)
     
-    config = hls4ml.utils.config.create_vivado_config(
+    config = hls4ml.utils.config.create_config(
+        backend=args.backend,
         output_dir=args.dir,
         project_name=args.project,
-        fpga_part=args.fpga,
+        part=args.fpga,
+        board=args.board,
         clock_period=args.clock
     )
 
     if args.model.endswith('.h5'):
         config['KerasH5'] = args.model
 
         with h5py.File(args.model, mode='r') as h5file:
@@ -133,23 +132,19 @@
         with open(outname, 'w') as outfile:
             yaml.dump(config, outfile, default_flow_style=False, sort_keys=False)
     else:
         print('Config output:')
         yaml.dump(config, sys.stdout, default_flow_style=False, sort_keys=False)
 
 def convert(args):
-    yamlConfig = parse_config(args.config)
-    model = hls4ml.converters.convert_from_yaml_config(yamlConfig)
+    model = hls4ml.converters.convert_from_config(args.config)
 
     if model is not None:
         model.write()
 
-    # Copy the config file to the generated folder
-    copyfile(args.config, yamlConfig['OutputDir'] + '/' + config_filename)
-
 def build(args):
     if args.project is None:
         print('Project directory (-p or --project) must be provided.')
         sys.exit(1)
 
     reset = int(args.reset)
     csim = int(args.simulation)
@@ -157,30 +152,30 @@
     cosim = int(args.co_simulation)
     validation = int(args.validation)
     export = int(args.export)
     vsynth = int(args.vivado_synthesis)
     if args.all:
         csim = synth = cosim = validation = export = vsynth = 1
     
-    yamlConfig = parse_config(args.project + '/' + config_filename)
+    yamlConfig = hls4ml.converters.parse_yaml_config(args.project + '/' + config_filename)
 
     # Check if vivado_hls is available
     if 'linux' in sys.platform or 'darwin' in sys.platform:
         backend = yamlConfig.get('Backend', 'Vivado')
-        if backend == 'Vivado':
+        if backend in ['Vivado', 'VivadoAccelerator']:
             found = os.system('command -v vivado_hls > /dev/null')
-            if found is not 0:
+            if found != 0:
                 print('Vivado HLS installation not found. Make sure "vivado_hls" is on PATH.')
                 sys.exit(1)
         elif backend == 'Intel':
             raise NotImplementedError
         elif backend == 'Mentor':
             raise NotImplementedError
         else:
-            raise Exception('Backend values can be [Vivado, Intel, Mentor]')
+            raise Exception('Backend values can be [Vivado, Intel, Mentor, VivadoAccelerator]')
     
     os.system('cd {dir} && vivado_hls -f build_prj.tcl "reset={reset} csim={csim} synth={synth} cosim={cosim} validation={validation} export={export} vsynth={vsynth}"'
         .format(dir=args.project, reset=reset, csim=csim, synth=synth, cosim=cosim, validation=validation, export=export, vsynth=vsynth))
 
 def report(args):
     if args.project is None:
         print('Project directory (-p or --project) must be provided.')
```

### Comparing `hls4ml-0.5.0b0/setup.py` & `hls4ml-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
                         'pyyaml',
                         'h5py',
                         'onnx>=1.4.0'],
       extras_require={
         'profiling': [
             'pandas',
             'seaborn',
-            'matplotlib'
-        ]
+            'matplotlib']
       },
       scripts=['scripts/hls4ml'],
       include_package_data=True,
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
```

### Comparing `hls4ml-0.5.0b0/test/build-prj.sh` & `hls4ml-0.6.0/test/build-prj.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/cleanup.sh` & `hls4ml-0.6.0/test/cleanup.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/compare-reports.sh` & `hls4ml-0.6.0/test/compare-reports.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/convert-keras-models.sh` & `hls4ml-0.6.0/test/convert-pytorch-models.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/bash
 
-models_var=HLS4ML_KERAS_MODELS
+models_var=HLS4ML_PYTORCH_MODELS
 models_file=
 exec=echo
 dir=
 
 function print_usage {
    echo "Usage: `basename $0` [OPTION]"
    echo ""
@@ -51,31 +51,29 @@
    fi
 else
    readarray model_line < "${models_file}"
 fi
 
 for line in "${model_line[@]}"
 do
-   params=("" "" "" "" "" "" "" "")
+   params=("" "" "" "" "" "")
    if [[ ${line} = *[![:space:]]* ]] && ! [[ "${line}" = \#* ]] ; then
       IFS=" " read -ra model_def <<< "${line}"
       for (( i=1; i<"${#model_def[@]}"; i++ ));
       do
          if [[ "${model_def[$i]}" == x:* ]] ; then params[0]="-x ${model_def[$i]:2} "; fi
          if [[ "${model_def[$i]}" == c:* ]] ; then params[1]="-c ${model_def[$i]:2} "; fi
          if [[ "${model_def[$i]}" == io:s ]] ; then params[2]="-s "; fi
          if [[ "${model_def[$i]}" == r:* ]] ; then params[3]="-r ${model_def[$i]:2} "; fi
-         if [[ "${model_def[$i]}" == s:* ]] ; then params[4]="-g ${model_def[$i]:2} "; fi
-         if [[ "${model_def[$i]}" == i:* ]] ; then params[5]="-t ${model_def[$i]:2} "; fi
-         if [[ "${model_def[$i]}" == y:* ]] ; then params[6]="-y ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == i:* ]] ; then params[4]="-t ${model_def[$i]:2} "; fi
       done
-      params[7]=${model_def[0]}
-
-      cmd="./keras-to-hls.sh ${dir} ${params[0]}${params[1]}${params[2]}${params[3]}${params[4]}${params[5]}${params[6]}${params[7]}"
-
+      params[5]=${model_def[0]}
+      
+      cmd="./pytorch-to-hls.sh ${dir} ${params[0]}${params[1]}${params[2]}${params[3]}${params[4]}${params[5]}"
+      
       ${exec} "${cmd}"
    fi
 done
 
 #cd "${rundir}"
 
 exit ${failed}
```

### Comparing `hls4ml-0.5.0b0/test/convert-onnx-models.sh` & `hls4ml-0.6.0/test/convert-onnx-models.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/convert-pytorch-models.sh` & `hls4ml-0.6.0/test/convert-keras-models.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/bash
 
-models_var=HLS4ML_PYTORCH_MODELS
+models_var=HLS4ML_KERAS_MODELS
 models_file=
 exec=echo
 dir=
 
 function print_usage {
    echo "Usage: `basename $0` [OPTION]"
    echo ""
@@ -51,29 +51,32 @@
    fi
 else
    readarray model_line < "${models_file}"
 fi
 
 for line in "${model_line[@]}"
 do
-   params=("" "" "" "" "" "")
+   params=("" "" "" "" "" "" "" "" "" "")
    if [[ ${line} = *[![:space:]]* ]] && ! [[ "${line}" = \#* ]] ; then
       IFS=" " read -ra model_def <<< "${line}"
       for (( i=1; i<"${#model_def[@]}"; i++ ));
       do
          if [[ "${model_def[$i]}" == x:* ]] ; then params[0]="-x ${model_def[$i]:2} "; fi
-         if [[ "${model_def[$i]}" == c:* ]] ; then params[1]="-c ${model_def[$i]:2} "; fi
-         if [[ "${model_def[$i]}" == io:s ]] ; then params[2]="-s "; fi
-         if [[ "${model_def[$i]}" == r:* ]] ; then params[3]="-r ${model_def[$i]:2} "; fi
-         if [[ "${model_def[$i]}" == i:* ]] ; then params[4]="-t ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == b:* ]] ; then params[1]="-b ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == B:* ]] ; then params[2]="-B ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == c:* ]] ; then params[3]="-c ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == io:s ]] ; then params[4]="-s "; fi
+         if [[ "${model_def[$i]}" == r:* ]] ; then params[5]="-r ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == s:* ]] ; then params[6]="-g ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == i:* ]] ; then params[7]="-t ${model_def[$i]:2} "; fi
+         if [[ "${model_def[$i]}" == y:* ]] ; then params[8]="-y ${model_def[$i]:2} "; fi
       done
-      params[5]=${model_def[0]}
-      
-      cmd="./pytorch-to-hls.sh ${dir} ${params[0]}${params[1]}${params[2]}${params[3]}${params[4]}${params[5]}"
-      
+      params[9]=${model_def[0]}
+      cmd="./keras-to-hls.sh ${dir} ${params[0]}${params[1]}${params[2]}${params[3]}${params[4]}${params[5]}${params[6]}${params[7]}${params[8]}${params[9]}"
+      echo "$cmd"
       ${exec} "${cmd}"
    fi
 done
 
 #cd "${rundir}"
 
 exit ${failed}
```

### Comparing `hls4ml-0.5.0b0/test/docker/Dockerfile` & `hls4ml-0.6.0/test/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/docker/README.md` & `hls4ml-0.6.0/test/docker/README.md`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/docker/install_config-2017.2.txt` & `hls4ml-0.6.0/test/docker/install_config-2017.2.txt`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/docker/install_config.txt` & `hls4ml-0.6.0/test/docker/install_config.txt`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/gather-reports.sh` & `hls4ml-0.6.0/test/gather-reports.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/hls4ml-keras-test.sh` & `hls4ml-0.6.0/test/hls4ml-keras-test.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/hls4ml-onnx-test.sh` & `hls4ml-0.6.0/test/hls4ml-onnx-test.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/hls4ml-pytorch-test.sh` & `hls4ml-0.6.0/test/hls4ml-pytorch-test.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/keras-models.txt` & `hls4ml-0.6.0/test/keras-models.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Keras models from examples directory that will be used for testing
 #
 # Synthax:
-#    MODEL_NAME[:WEIGHTS_FILE] [x:XILINXPART] [c:CLOCK_PERIOD] [io:s] [r:REUSE_FACTOR] [t:AP_TYPE] [s:STRATEGY] [y:CONFIG_FILE]
+#    MODEL_NAME[:WEIGHTS_FILE] [x:XILINXPART] [b:BOARD] [B:BACKEND] [c:CLOCK_PERIOD] [io:s] [r:REUSE_FACTOR] [t:AP_TYPE] [s:STRATEGY] [y:CONFIG_FILE]
 # where
 #    MODEL_NAME - Name of the file containing json model (without ".json")
 #    WEIGHTS_FILE - Name of the HDF5 file containing model weights (without ".h5")
 #    x:XILINXPART - Xilinx part number to use
+#    b:BOARD - name of one board defined in supported_board.json file
+#    B:BACKEND - name of the backend to be used (Vivado, VivadoAccelerator)
 #    c:CLOCK_PERIOD - Clock period
 #    io:s - User streaming I/O, otherwise use parallel I/O
 #    r:REUSE_FACTOR - Reuse factor
 #    s:STRATEGY - Latency-optimized or Resource-optimized strategy
 #    t:AP_TYPE - Default precision
 #    y:CONFIG_FILE - YAML config file to copy HLSConfig from
 #
@@ -22,15 +24,17 @@
 #KERAS_conv1d
 #KERAS_conv1d_small
 #KERAS_conv2d_model
 #KERAS_dense_16x100x100x100x100x100x5
 KERAS_3layer_batch_norm
 KERAS_3layer_binary_smaller
 KERAS_3layer_ternary_small
- 
+
+KERAS_3layer b:pynq-z2 B:VivadoAccelerator x:xc7z020clg400-1 s:Resource
+
 garnet_1layer x:xcku115-flvb2104-2-i y:garnet_1layer_config 
 
 # Resource strategy
 KERAS_3layer r:2 s:Resource
 qkeras_mnist_dense r:112 s:Resource
 
 #Fails synthesis due to a problem with loop unrolling
@@ -40,8 +44,9 @@
 #KERAS_1layer io:s
 KERAS_3layer io:s
 KERAS_conv1d_small io:s
 KERAS_conv2d_model io:s
 jetTagger_Conv2D_Small io:s
 jetTagger_Conv2D_Small_NoBatchNorm io:s
 
-#KERAS_1layer x:xcku115-flvf1924-2-i
+
+#KERAS_1layer x:xcku115-flvf1924-2-i
```

### Comparing `hls4ml-0.5.0b0/test/keras-to-hls.sh` & `hls4ml-0.6.0/test/keras-to-hls.sh`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/bin/bash
 
 pycmd=python
 xilinxpart="xcvu9p-flgb2104-2-e"
+board="None"
+backend="Vivado"
 clock=5
 io=io_parallel
 rf=1
 strategy="Latency"
 type="ap_fixed<16,6>"
 yml=""
 basedir=vivado_prj
@@ -17,16 +19,20 @@
    echo ""
    echo "MODEL is the name of the model json file without extension. Optionally"
    echo "a H5 file with weights can be provided using the MODEL:H5FILE synthax."
    echo "By default, it is assumed that weights are stored in MODEL_weights.h5."
    echo "Multiple models can be specified."
    echo ""
    echo "Options are:"
-   echo "   -x DEVICE"
+   echo "   -x XILINXPART"
    echo "      Xilinx device part number. Defaults to 'xcvu9p-flgb2104-2-e'."
+   echo "   -b BOARD"
+   echo "      Board used. Defaults to 'pynq-z2'."
+   echo "   -B BACKEND"
+   echo "      Backend to use for the generation of the code. Defaults to 'Vivado'."
    echo "   -c CLOCK"
    echo "      Clock period to use. Defaults to 5."
    echo "   -s"
    echo "      Use streaming I/O. If not specified uses parallel I/O."
    echo "   -r FACTOR"
    echo "      Reuse factor. Defaults to 1."
    echo "   -g STRATEGY"
@@ -37,18 +43,22 @@
    echo "      Output directory."
    echo "   -y FILE"
    echo "      YAML config file to take HLS config from. If specified, -r, -g and -t are ignored."
    echo "   -h"
    echo "      Prints this help message."
 }
 
-while getopts ":x:c:sr:g:t:d:y:h" opt; do
+while getopts ":x:b:B:c:sr:g:t:d:y:h" opt; do
    case "$opt" in
    x) xilinxpart=$OPTARG
       ;;
+   b) board=$OPTARG
+      ;;
+   B) backend=$OPTARG
+      ;;
    c) clock=$OPTARG
       ;;
    s) io=io_stream
       ;;
    r) rf=$OPTARG
       ;;
    g) strategy=$OPTARG
@@ -89,26 +99,28 @@
       name="${model_h5_pair[0]}"
       h5="${model_h5_pair[1]}"
    fi
 
    echo "Creating config file for model '${model}'"
    base=`echo "${h5}" | sed -e 's/\(_weights\)*$//g'`
    file="${basedir}/${base}.yml"
-   prjdir="${basedir}/${base}-${xilinxpart//${sanitizer}/_}-c${clock}-${io}-rf${rf}-${type//${sanitizer}/_}-${strategy}"
+   prjdir="${basedir}/${base}-backend${backend}-board${board//${sanitizer}/_}-${xilinxpart//${sanitizer}/_}-c${clock}-${io}-rf${rf}-${type//${sanitizer}/_}-${strategy}"
 
    hlscfg=""
    if [ ! -z "${yml}" ]; then
       hlscfg=`sed -ne '/HLSConfig/,$p' ../example-models/config-files/${yml}`
    fi
 
    echo "KerasJson: ../example-models/keras/${name}.json" > ${file}
    echo "KerasH5:   ../example-models/keras/${h5}.h5" >> ${file}
    echo "OutputDir: ${prjdir}" >> ${file}
    echo "ProjectName: myproject" >> ${file}
    echo "XilinxPart: ${xilinxpart}" >> ${file}
+   echo "Board: ${board}" >> ${file}
+   echo "Backend: ${backend}" >> ${file}
    echo "ClockPeriod: ${clock}" >> ${file}
    echo "" >> ${file}
    echo "IOType: ${io}" >> ${file}
    
    if [ -z "${hlscfg}" ]
    then
       echo "HLSConfig:" >> ${file}
```

### Comparing `hls4ml-0.5.0b0/test/onnx-models.txt` & `hls4ml-0.6.0/test/onnx-models.txt`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/onnx-to-hls.sh` & `hls4ml-0.6.0/test/onnx-to-hls.sh`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/pytorch-models.txt` & `hls4ml-0.6.0/test/pytorch-models.txt`

 * *Files identical despite different names*

### Comparing `hls4ml-0.5.0b0/test/pytorch-to-hls.sh` & `hls4ml-0.6.0/test/pytorch-to-hls.sh`

 * *Files identical despite different names*

