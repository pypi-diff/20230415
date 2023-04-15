# Comparing `tmp/deepwave-0.0.8.tar.gz` & `tmp/deepwave-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepwave-0.0.8.tar", last modified: Sun Jan 24 13:32:23 2021, max compression
+gzip compressed data, was "dist/deepwave-0.0.9.tar", last modified: Tue Oct 26 10:09:46 2021, max compression
```

## Comparing `deepwave-0.0.8.tar` & `deepwave-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-01-24 13:32:23.000000 deepwave-0.0.8/
--rw-rw-r--   0 alanr     (1000) alanr     (1000)     1072 2021-01-21 16:54:48.000000 deepwave-0.0.8/LICENSE
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      118 2021-01-21 16:54:48.000000 deepwave-0.0.8/MANIFEST.in
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    11599 2021-01-24 13:32:23.000000 deepwave-0.0.8/PKG-INFO
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    10070 2021-01-24 13:28:17.000000 deepwave-0.0.8/README.md
-drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-01-24 13:32:23.000000 deepwave-0.0.8/deepwave/
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      136 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/__init__.py
-drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-01-24 13:32:23.000000 deepwave-0.0.8/deepwave/base/
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      147 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/base/__init__.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)     5265 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/base/extract.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    11431 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/base/model.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      648 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/base/pad.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)     8413 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/base/propagator.py
-drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-01-24 13:32:23.000000 deepwave-0.0.8/deepwave/scalar/
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      168 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/scalar/__init__.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    17101 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar.cpp
--rw-rw-r--   0 alanr     (1000) alanr     (1000)     9489 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar.h
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    19314 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    21302 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar_born.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    21068 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar_cpu.cpp
--rw-rw-r--   0 alanr     (1000) alanr     (1000)       27 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/scalar/scalar_cpu.h
--rw-rw-r--   0 alanr     (1000) alanr     (1000)     3286 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar_device.h
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    40560 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar_gpu.cu
--rw-rw-r--   0 alanr     (1000) alanr     (1000)       27 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/scalar/scalar_gpu.h
--rw-rw-r--   0 alanr     (1000) alanr     (1000)     4867 2021-01-24 13:28:17.000000 deepwave-0.0.8/deepwave/scalar/scalar_wrapper.cpp
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      849 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/utils.py
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      711 2021-01-21 16:54:48.000000 deepwave-0.0.8/deepwave/wavelets.py
-drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-01-24 13:32:23.000000 deepwave-0.0.8/deepwave.egg-info/
--rw-rw-r--   0 alanr     (1000) alanr     (1000)    11599 2021-01-24 13:32:22.000000 deepwave-0.0.8/deepwave.egg-info/PKG-INFO
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      703 2021-01-24 13:32:22.000000 deepwave-0.0.8/deepwave.egg-info/SOURCES.txt
--rw-rw-r--   0 alanr     (1000) alanr     (1000)        1 2021-01-24 13:32:22.000000 deepwave-0.0.8/deepwave.egg-info/dependency_links.txt
--rw-rw-r--   0 alanr     (1000) alanr     (1000)       43 2021-01-24 13:32:22.000000 deepwave-0.0.8/deepwave.egg-info/requires.txt
--rw-rw-r--   0 alanr     (1000) alanr     (1000)      162 2021-01-24 13:32:22.000000 deepwave-0.0.8/deepwave.egg-info/top_level.txt
--rw-rw-r--   0 alanr     (1000) alanr     (1000)       38 2021-01-24 13:32:23.000000 deepwave-0.0.8/setup.cfg
--rw-rw-r--   0 alanr     (1000) alanr     (1000)     2742 2021-01-24 13:28:39.000000 deepwave-0.0.8/setup.py
+drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-10-26 10:09:46.000000 deepwave-0.0.9/
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)     1072 2021-01-21 16:54:48.000000 deepwave-0.0.9/LICENSE
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      118 2021-01-21 16:54:48.000000 deepwave-0.0.9/MANIFEST.in
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    12041 2021-10-26 10:09:46.000000 deepwave-0.0.9/PKG-INFO
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    10416 2021-10-25 20:36:20.000000 deepwave-0.0.9/README.md
+drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-10-26 10:09:46.000000 deepwave-0.0.9/deepwave/
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      136 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/__init__.py
+drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-10-26 10:09:46.000000 deepwave-0.0.9/deepwave/base/
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      147 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/base/__init__.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)     5265 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/base/extract.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    11431 2021-01-24 13:28:17.000000 deepwave-0.0.9/deepwave/base/model.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      648 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/base/pad.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)     8413 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/base/propagator.py
+drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-10-26 10:09:46.000000 deepwave-0.0.9/deepwave/scalar/
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      168 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/scalar/__init__.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    18505 2021-10-25 20:25:10.000000 deepwave-0.0.9/deepwave/scalar/scalar.cpp
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)     9867 2021-10-25 20:24:48.000000 deepwave-0.0.9/deepwave/scalar/scalar.h
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    19329 2021-10-26 09:14:30.000000 deepwave-0.0.9/deepwave/scalar/scalar.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    21322 2021-10-26 09:50:54.000000 deepwave-0.0.9/deepwave/scalar/scalar_born.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    22526 2021-10-25 20:24:56.000000 deepwave-0.0.9/deepwave/scalar/scalar_cpu.cpp
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)       27 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/scalar/scalar_cpu.h
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)     3619 2021-10-25 20:24:40.000000 deepwave-0.0.9/deepwave/scalar/scalar_device.h
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    43035 2021-10-25 20:24:59.000000 deepwave-0.0.9/deepwave/scalar/scalar_gpu.cu
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)       27 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/scalar/scalar_gpu.h
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)     5182 2021-10-25 20:24:52.000000 deepwave-0.0.9/deepwave/scalar/scalar_wrapper.cpp
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      849 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/utils.py
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      711 2021-01-21 16:54:48.000000 deepwave-0.0.9/deepwave/wavelets.py
+drwxrwxr-x   0 alanr     (1000) alanr     (1000)        0 2021-10-26 10:09:46.000000 deepwave-0.0.9/deepwave.egg-info/
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)    12041 2021-10-26 10:09:45.000000 deepwave-0.0.9/deepwave.egg-info/PKG-INFO
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      703 2021-10-26 10:09:45.000000 deepwave-0.0.9/deepwave.egg-info/SOURCES.txt
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)        1 2021-10-26 10:09:45.000000 deepwave-0.0.9/deepwave.egg-info/dependency_links.txt
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)       43 2021-10-26 10:09:45.000000 deepwave-0.0.9/deepwave.egg-info/requires.txt
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)      162 2021-10-26 10:09:45.000000 deepwave-0.0.9/deepwave.egg-info/top_level.txt
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)       38 2021-10-26 10:09:46.000000 deepwave-0.0.9/setup.cfg
+-rw-rw-r--   0 alanr     (1000) alanr     (1000)     2778 2021-10-25 21:01:43.000000 deepwave-0.0.9/setup.py
```

### Comparing `deepwave-0.0.8/LICENSE` & `deepwave-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/PKG-INFO` & `deepwave-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: deepwave
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wave propagation modules for PyTorch.
 Home-page: https://github.com/ar4/deepwave
 Author: Alan Richardson
 Author-email: alan@ausargeo.com
 License: UNKNOWN
 Description: # Deepwave
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/52d27677ef0a439195d574964a6b4be4)](https://www.codacy.com/app/ar4/deepwave?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ar4/deepwave&amp;utm_campaign=Badge_Grade)
         
         Deepwave provides wave propagation modules for PyTorch (currently only for the constant density acoustic / scalar wave equation). It is primarily aimed at seismic imaging/inversion. One interesting advantage of this is that it allows you to chain operations together. You could, for example, use Deepwave to perform FWI using a custom cost function (as long as PyTorch is able to automatically differentiate it), or add some other operations before and after wave propagation and PyTorch will backpropagate through all of them.
         
         Wave propagation and FWI [can be implemented using deep neural networks](https://arxiv.org/abs/1801.07232). Deep learning tools such as TensorFlow and PyTorch are currently too slow and memory inefficient to do this with realistic seismic datasets, however. Deepwave extends PyTorch with higher performance wave propagation modules (written in C and CUDA) so that you can benefit from the conveniences of PyTorch without sacrificing performance.
         
         Deepwave runs on CPUs and NVIDIA GPUs. It should automatically detect compatible GPUs during installation and compile the GPU code if any are found. To run on the GPU you must transfer the model, source amplitude, and source and receiver location Tensors to the GPU in the standard PyTorch way (using `.cuda()` or `.to(device)`).
         
         ## Installation
         Deepwave needs NumPy, so [installing Anaconda](https://www.anaconda.com/download) first is highly recommended. It also needs [PyTorch](https://pytorch.org/), so it is also best to install that (using something like `conda install pytorch-cpu -c pytorch`) before installing Deepwave. You can then install the latest release of Deepwave using
         
         `pip install deepwave`
         
-        or the latest development version using
-        
-        `pip install git+https://github.com/ar4/deepwave.git`
-        
+        Note that this will probably take several minutes as it needs to compile the code.
         
         ## Usage
         Deepwave can do two things: forward modeling and backpropagation.
         
         ### Forward modeling
         We first need to create a wave propagation module. If you are familiar with training neural networks, this is the same as defining your network (or a portion of it) and initializing the weights.
         
@@ -131,19 +127,35 @@
         
         For an example of using Deepwave for LSRTM, see [this notebook](https://colab.research.google.com/drive/1BgQM5VGgyFp7Q--pAJX-vGb2bW9mcbM8).
         
         ## Notes
         * For a reflective free surface, set the PML width to zero at the surface. For example, in 3D and when the PML width on the other sides is 10 cells, provide the argument `pml_width=[0,10,10,10,10,10]` when creating the propagator if the free surface is at the beginning of the first dimension. The format is [z1, z2, y1, y2, x1, x2], where z1, y1, and x1 are the PML widths at the beginning of the z, y, and x dimensions, and z2, y2, and x2 are the PML widths at the ends of those dimensions.
         * To limit wave simulation to the region covered by the survey (the sources and receivers), provide the `survey_pad` keyword argument when creating the propagator. For example, to use the whole z dimension, but only up to 100m from the first and last source/receiver in the y and x dimensions, use `survey_pad=[None, None, 100, 100, 100, 100]`, where `None` means continue to the edge of the model, and the format is similar to that used for `pml_width`. The default is `None` for every entry.
         * [@LukasMosser](https://github.com/LukasMosser) discovered that GCC 4.9 or above is necessary ([#18](https://github.com/ar4/deepwave/issues/18)).
+        * [@ADharaUTEXAS123007](https://github.com/ADharaUTEXAS123007) discovered that for recent versions of PyTorch an even later release of GCC might be necessary. A warning was displayed (Your compiler (g++ 4.8.5) may be ABI-incompatible with PyTorch!
+        Please use a compiler that is ABI-compatible with GCC 5.0 and above.) and compilation failed. This was resolved with `conda install gxx_linux-64`.
         * Distributed parallelization over shots is supported, but not within a shot; each shot must run within one node.
-        * Currently, the forward source wavefield is saved in memory for use during backpropagation. This means that realistic 3D surveys will probably require more memory than is available. This will be fixed in a future release.
-        
-        ## Contributing
-        Your help to improve Deepwave would be greatly appreciated. If you encounter any difficulty using Deepwave, please report it as a Github Issue so that it can be fixed. If you have feature suggestions or other ideas to make Deepwave better, please also report those as Github Issues. If you want to help with the coding, that would be especially wonderful. The Github Issues contain a list of things that need work. If you see one that you would like to attempt, please ask for it to be assigned to you.
+        * Currently, the forward source wavefield is saved in memory for use during backpropagation. This means that realistic 3D surveys will probably require more memory than is available.
+        * [@erellaz](https://github.com/erellaz) has created [a nice tool](https://github.com/erellaz/SEGY_Wrapper) to make loading and saving SEG-Y files easier, and a demonstration of using Deepwave for forward modeling with a realistic 2D model.
+        * Your help to improve Deepwave would be greatly appreciated. If you encounter any difficulty using Deepwave, please report it as a Github Issue so that it can be fixed.
+        
+        ## Citing
+        If you would like to cite Deepwave, I suggest
+        ```
+        @software{deepwave,
+          author       = {Richardson, Alan},
+          title        = {Deepwave},
+          month        = oct,
+          year         = 2021,
+          publisher    = {Zenodo},
+          version      = {v0.0.9},
+          doi          = {10.5281/zenodo.3829886},
+          url          = {https://doi.org/10.5281/zenodo.3829886}
+        }
+        ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `deepwave-0.0.8/README.md` & `deepwave-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # Deepwave
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/52d27677ef0a439195d574964a6b4be4)](https://www.codacy.com/app/ar4/deepwave?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ar4/deepwave&amp;utm_campaign=Badge_Grade)
 
 Deepwave provides wave propagation modules for PyTorch (currently only for the constant density acoustic / scalar wave equation). It is primarily aimed at seismic imaging/inversion. One interesting advantage of this is that it allows you to chain operations together. You could, for example, use Deepwave to perform FWI using a custom cost function (as long as PyTorch is able to automatically differentiate it), or add some other operations before and after wave propagation and PyTorch will backpropagate through all of them.
 
 Wave propagation and FWI [can be implemented using deep neural networks](https://arxiv.org/abs/1801.07232). Deep learning tools such as TensorFlow and PyTorch are currently too slow and memory inefficient to do this with realistic seismic datasets, however. Deepwave extends PyTorch with higher performance wave propagation modules (written in C and CUDA) so that you can benefit from the conveniences of PyTorch without sacrificing performance.
 
 Deepwave runs on CPUs and NVIDIA GPUs. It should automatically detect compatible GPUs during installation and compile the GPU code if any are found. To run on the GPU you must transfer the model, source amplitude, and source and receiver location Tensors to the GPU in the standard PyTorch way (using `.cuda()` or `.to(device)`).
 
 ## Installation
 Deepwave needs NumPy, so [installing Anaconda](https://www.anaconda.com/download) first is highly recommended. It also needs [PyTorch](https://pytorch.org/), so it is also best to install that (using something like `conda install pytorch-cpu -c pytorch`) before installing Deepwave. You can then install the latest release of Deepwave using
 
 `pip install deepwave`
 
-or the latest development version using
-
-`pip install git+https://github.com/ar4/deepwave.git`
-
+Note that this will probably take several minutes as it needs to compile the code.
 
 ## Usage
 Deepwave can do two things: forward modeling and backpropagation.
 
 ### Forward modeling
 We first need to create a wave propagation module. If you are familiar with training neural networks, this is the same as defining your network (or a portion of it) and initializing the weights.
 
@@ -123,12 +119,28 @@
 
 For an example of using Deepwave for LSRTM, see [this notebook](https://colab.research.google.com/drive/1BgQM5VGgyFp7Q--pAJX-vGb2bW9mcbM8).
 
 ## Notes
 * For a reflective free surface, set the PML width to zero at the surface. For example, in 3D and when the PML width on the other sides is 10 cells, provide the argument `pml_width=[0,10,10,10,10,10]` when creating the propagator if the free surface is at the beginning of the first dimension. The format is [z1, z2, y1, y2, x1, x2], where z1, y1, and x1 are the PML widths at the beginning of the z, y, and x dimensions, and z2, y2, and x2 are the PML widths at the ends of those dimensions.
 * To limit wave simulation to the region covered by the survey (the sources and receivers), provide the `survey_pad` keyword argument when creating the propagator. For example, to use the whole z dimension, but only up to 100m from the first and last source/receiver in the y and x dimensions, use `survey_pad=[None, None, 100, 100, 100, 100]`, where `None` means continue to the edge of the model, and the format is similar to that used for `pml_width`. The default is `None` for every entry.
 * [@LukasMosser](https://github.com/LukasMosser) discovered that GCC 4.9 or above is necessary ([#18](https://github.com/ar4/deepwave/issues/18)).
+* [@ADharaUTEXAS123007](https://github.com/ADharaUTEXAS123007) discovered that for recent versions of PyTorch an even later release of GCC might be necessary. A warning was displayed (Your compiler (g++ 4.8.5) may be ABI-incompatible with PyTorch!
+Please use a compiler that is ABI-compatible with GCC 5.0 and above.) and compilation failed. This was resolved with `conda install gxx_linux-64`.
 * Distributed parallelization over shots is supported, but not within a shot; each shot must run within one node.
-* Currently, the forward source wavefield is saved in memory for use during backpropagation. This means that realistic 3D surveys will probably require more memory than is available. This will be fixed in a future release.
-
-## Contributing
-Your help to improve Deepwave would be greatly appreciated. If you encounter any difficulty using Deepwave, please report it as a Github Issue so that it can be fixed. If you have feature suggestions or other ideas to make Deepwave better, please also report those as Github Issues. If you want to help with the coding, that would be especially wonderful. The Github Issues contain a list of things that need work. If you see one that you would like to attempt, please ask for it to be assigned to you.
+* Currently, the forward source wavefield is saved in memory for use during backpropagation. This means that realistic 3D surveys will probably require more memory than is available.
+* [@erellaz](https://github.com/erellaz) has created [a nice tool](https://github.com/erellaz/SEGY_Wrapper) to make loading and saving SEG-Y files easier, and a demonstration of using Deepwave for forward modeling with a realistic 2D model.
+* Your help to improve Deepwave would be greatly appreciated. If you encounter any difficulty using Deepwave, please report it as a Github Issue so that it can be fixed.
+
+## Citing
+If you would like to cite Deepwave, I suggest
+```
+@software{deepwave,
+  author       = {Richardson, Alan},
+  title        = {Deepwave},
+  month        = oct,
+  year         = 2021,
+  publisher    = {Zenodo},
+  version      = {v0.0.9},
+  doi          = {10.5281/zenodo.3829886},
+  url          = {https://doi.org/10.5281/zenodo.3829886}
+}
+```
```

### Comparing `deepwave-0.0.8/deepwave/base/extract.py` & `deepwave-0.0.9/deepwave/base/extract.py`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/deepwave/base/model.py` & `deepwave-0.0.9/deepwave/base/model.py`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/deepwave/base/pad.py` & `deepwave-0.0.9/deepwave/base/pad.py`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/deepwave/base/propagator.py` & `deepwave-0.0.9/deepwave/base/propagator.py`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/deepwave/scalar/scalar.h` & `deepwave-0.0.9/deepwave/scalar/scalar.h`

 * *Files 14% similar despite different names*

```diff
@@ -174,421 +174,444 @@
 00000ad0: 6520 6474 202a 2073 7465 705f 7261 7469  e dt * step_rati
 00000ae0: 6f29 2e0a 202a 2073 6176 655f 7374 7261  o).. * save_stra
 00000af0: 7465 6779 3a20 456e 756d 2073 7065 6369  tegy: Enum speci
 00000b00: 6679 696e 6720 686f 7720 746f 2073 746f  fying how to sto
 00000b10: 7265 2077 6176 6566 6965 6c64 2066 6f72  re wavefield for
 00000b20: 2062 6163 6b70 726f 7061 6761 7469 6f6e   backpropagation
 00000b30: 2e0a 202a 2f0a 766f 6964 2066 6f72 7761  .. */.void forwa
-00000b40: 7264 2854 5950 4520 2a20 636f 6e73 7420  rd(TYPE * const 
-00000b50: 7761 7665 6669 656c 642c 0a20 2020 2020  wavefield,.     
-00000b60: 2020 2020 2020 2020 5459 5045 202a 2063          TYPE * c
-00000b70: 6f6e 7374 2061 7578 5f77 6176 6566 6965  onst aux_wavefie
-00000b80: 6c64 2c0a 2020 2020 2020 2020 2020 2020  ld,.            
-00000b90: 2054 5950 4520 2a20 636f 6e73 7420 7265   TYPE * const re
-00000ba0: 6365 6976 6572 5f61 6d70 6c69 7475 6465  ceiver_amplitude
-00000bb0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00000bc0: 5459 5045 202a 2063 6f6e 7374 2073 6176  TYPE * const sav
-00000bd0: 6564 5f77 6176 6566 6965 6c64 732c 0a20  ed_wavefields,. 
-00000be0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00000bf0: 7420 5459 5045 202a 2063 6f6e 7374 2073  t TYPE * const s
-00000c00: 6967 6d61 2c0a 2020 2020 2020 2020 2020  igma,.          
-00000c10: 2020 2063 6f6e 7374 2054 5950 4520 2a20     const TYPE * 
-00000c20: 636f 6e73 7420 6d6f 6465 6c2c 0a20 2020  const model,.   
-00000c30: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00000c40: 5459 5045 202a 2063 6f6e 7374 2066 6431  TYPE * const fd1
-00000c50: 2c0a 2020 2020 2020 2020 2020 2020 2063  ,.             c
-00000c60: 6f6e 7374 2054 5950 4520 2a20 636f 6e73  onst TYPE * cons
-00000c70: 7420 6664 322c 0a20 2020 2020 2020 2020  t fd2,.         
-00000c80: 2020 2020 636f 6e73 7420 5459 5045 202a      const TYPE *
-00000c90: 2063 6f6e 7374 2073 6f75 7263 655f 616d   const source_am
-00000ca0: 706c 6974 7564 6573 2c0a 2020 2020 2020  plitudes,.      
-00000cb0: 2020 2020 2020 2063 6f6e 7374 2070 7472         const ptr
-00000cc0: 6469 6666 5f74 202a 2063 6f6e 7374 2073  diff_t * const s
-00000cd0: 6f75 7263 655f 6c6f 6361 7469 6f6e 732c  ource_locations,
-00000ce0: 0a20 2020 2020 2020 2020 2020 2020 636f  .             co
-00000cf0: 6e73 7420 7074 7264 6966 665f 7420 2a20  nst ptrdiff_t * 
-00000d00: 636f 6e73 7420 7265 6365 6976 6572 5f6c  const receiver_l
-00000d10: 6f63 6174 696f 6e73 2c0a 2020 2020 2020  ocations,.      
-00000d20: 2020 2020 2020 2063 6f6e 7374 2070 7472         const ptr
-00000d30: 6469 6666 5f74 202a 2063 6f6e 7374 2073  diff_t * const s
-00000d40: 6861 7065 2c0a 2020 2020 2020 2020 2020  hape,.          
-00000d50: 2020 2063 6f6e 7374 2070 7472 6469 6666     const ptrdiff
-00000d60: 5f74 202a 2063 6f6e 7374 2070 6d6c 5f77  _t * const pml_w
-00000d70: 6964 7468 2c0a 2020 2020 2020 2020 2020  idth,.          
-00000d80: 2020 2063 6f6e 7374 2070 7472 6469 6666     const ptrdiff
-00000d90: 5f74 206e 756d 5f73 7465 7073 2c20 636f  _t num_steps, co
-00000da0: 6e73 7420 7074 7264 6966 665f 7420 7374  nst ptrdiff_t st
-00000db0: 6570 5f72 6174 696f 2c0a 2020 2020 2020  ep_ratio,.      
-00000dc0: 2020 2020 2020 2063 6f6e 7374 2070 7472         const ptr
-00000dd0: 6469 6666 5f74 206e 756d 5f73 686f 7473  diff_t num_shots
-00000de0: 2c20 636f 6e73 7420 7074 7264 6966 665f  , const ptrdiff_
-00000df0: 7420 6e75 6d5f 736f 7572 6365 735f 7065  t num_sources_pe
-00000e00: 725f 7368 6f74 2c0a 2020 2020 2020 2020  r_shot,.        
-00000e10: 2020 2020 2063 6f6e 7374 2070 7472 6469       const ptrdi
-00000e20: 6666 5f74 206e 756d 5f72 6563 6569 7665  ff_t num_receive
-00000e30: 7273 5f70 6572 5f73 686f 742c 2063 6f6e  rs_per_shot, con
-00000e40: 7374 2054 5950 4520 6474 2c0a 2020 2020  st TYPE dt,.    
-00000e50: 2020 2020 2020 2020 2063 6f6e 7374 2065           const e
-00000e60: 6e75 6d20 7761 7665 6669 656c 645f 7361  num wavefield_sa
-00000e70: 7665 5f73 7472 6174 6567 7920 7361 7665  ve_strategy save
-00000e80: 5f73 7472 6174 6567 7929 3b0a 0a2f 2a20  _strategy);../* 
-00000e90: 426f 726e 2066 6f72 7761 7264 206d 6f64  Born forward mod
-00000ea0: 656c 696e 670a 202a 2041 7267 756d 656e  eling. * Argumen
-00000eb0: 7473 2061 7265 2074 6865 2073 616d 6520  ts are the same 
-00000ec0: 6173 2072 6567 756c 6172 2066 6f72 7761  as regular forwa
-00000ed0: 7264 206d 6f64 656c 696e 672c 2065 7863  rd modeling, exc
-00000ee0: 6570 7420 666f 7220 7468 6520 666f 6c6c  ept for the foll
-00000ef0: 6f77 696e 670a 202a 2073 6361 7474 6572  owing. * scatter
-00000f00: 6564 5f77 6176 6566 6965 6c64 3a20 4c69  ed_wavefield: Li
-00000f10: 6b65 2077 6176 6566 6965 6c64 2c20 6275  ke wavefield, bu
-00000f20: 7420 666f 7220 7363 6174 7465 7265 6420  t for scattered 
-00000f30: 7761 7665 730a 202a 2073 6361 7474 6572  waves. * scatter
-00000f40: 6564 5f61 7578 5f77 6176 6566 6965 6c64  ed_aux_wavefield
-00000f50: 3a20 4c69 6b65 2061 7578 5f77 6176 6566  : Like aux_wavef
-00000f60: 6965 6c64 2c20 6275 7420 666f 7220 7363  ield, but for sc
-00000f70: 6174 7465 7265 6420 7761 7665 730a 202a  attered waves. *
-00000f80: 2073 6361 7474 6572 3a20 4c69 6b65 206d   scatter: Like m
-00000f90: 6f64 656c 2c20 6275 7420 636f 6e74 6169  odel, but contai
-00000fa0: 6e73 2074 6865 2073 6361 7474 6572 696e  ns the scatterin
-00000fb0: 6720 616d 706c 6974 7564 650a 202a 2f0a  g amplitude. */.
-00000fc0: 766f 6964 2066 6f72 7761 7264 5f62 6f72  void forward_bor
-00000fd0: 6e28 5459 5045 202a 2063 6f6e 7374 2077  n(TYPE * const w
-00000fe0: 6176 6566 6965 6c64 2c0a 2020 2020 2020  avefield,.      
-00000ff0: 2020 2020 2020 2054 5950 4520 2a20 636f         TYPE * co
-00001000: 6e73 7420 6175 785f 7761 7665 6669 656c  nst aux_wavefiel
-00001010: 642c 0a20 2020 2009 2020 2020 2054 5950  d,.    .     TYP
-00001020: 4520 2a20 636f 6e73 7420 7363 6174 7465  E * const scatte
-00001030: 7265 645f 7761 7665 6669 656c 642c 0a09  red_wavefield,..
-00001040: 2020 2020 2054 5950 4520 2a20 636f 6e73       TYPE * cons
-00001050: 7420 7363 6174 7465 7265 645f 6175 785f  t scattered_aux_
-00001060: 7761 7665 6669 656c 642c 0a20 2020 2020  wavefield,.     
-00001070: 2020 2020 2020 2020 5459 5045 202a 2063          TYPE * c
-00001080: 6f6e 7374 2072 6563 6569 7665 725f 616d  onst receiver_am
-00001090: 706c 6974 7564 6573 2c0a 2020 2020 2020  plitudes,.      
-000010a0: 2020 2020 2020 2054 5950 4520 2a20 636f         TYPE * co
-000010b0: 6e73 7420 7361 7665 645f 7761 7665 6669  nst saved_wavefi
-000010c0: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
-000010d0: 2020 2063 6f6e 7374 2054 5950 4520 2a20     const TYPE * 
-000010e0: 636f 6e73 7420 7369 676d 612c 0a20 2020  const sigma,.   
-000010f0: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00001100: 5459 5045 202a 2063 6f6e 7374 206d 6f64  TYPE * const mod
-00001110: 656c 2c0a 0920 2020 2020 636f 6e73 7420  el,..     const 
-00001120: 5459 5045 202a 2063 6f6e 7374 2073 6361  TYPE * const sca
-00001130: 7474 6572 2c0a 2020 2020 2020 2020 2020  tter,.          
-00001140: 2020 2063 6f6e 7374 2054 5950 4520 2a20     const TYPE * 
-00001150: 636f 6e73 7420 6664 312c 0a20 2020 2020  const fd1,.     
-00001160: 2020 2020 2020 2020 636f 6e73 7420 5459          const TY
-00001170: 5045 202a 2063 6f6e 7374 2066 6432 2c0a  PE * const fd2,.
-00001180: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001190: 7374 2054 5950 4520 2a20 636f 6e73 7420  st TYPE * const 
-000011a0: 736f 7572 6365 5f61 6d70 6c69 7475 6465  source_amplitude
-000011b0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000011c0: 636f 6e73 7420 7074 7264 6966 665f 7420  const ptrdiff_t 
-000011d0: 2a20 636f 6e73 7420 736f 7572 6365 5f6c  * const source_l
-000011e0: 6f63 6174 696f 6e73 2c0a 2020 2020 2020  ocations,.      
-000011f0: 2020 2020 2020 2063 6f6e 7374 2070 7472         const ptr
-00001200: 6469 6666 5f74 202a 2063 6f6e 7374 2072  diff_t * const r
-00001210: 6563 6569 7665 725f 6c6f 6361 7469 6f6e  eceiver_location
-00001220: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00001230: 636f 6e73 7420 7074 7264 6966 665f 7420  const ptrdiff_t 
-00001240: 2a20 636f 6e73 7420 7368 6170 652c 0a20  * const shape,. 
-00001250: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00001260: 7420 7074 7264 6966 665f 7420 2a20 636f  t ptrdiff_t * co
-00001270: 6e73 7420 706d 6c5f 7769 6474 682c 0a20  nst pml_width,. 
-00001280: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00001290: 7420 7074 7264 6966 665f 7420 6e75 6d5f  t ptrdiff_t num_
-000012a0: 7374 6570 732c 2063 6f6e 7374 2070 7472  steps, const ptr
-000012b0: 6469 6666 5f74 2073 7465 705f 7261 7469  diff_t step_rati
-000012c0: 6f2c 0a20 2020 2020 2020 2020 2020 2020  o,.             
-000012d0: 636f 6e73 7420 7074 7264 6966 665f 7420  const ptrdiff_t 
-000012e0: 6e75 6d5f 7368 6f74 732c 2063 6f6e 7374  num_shots, const
-000012f0: 2070 7472 6469 6666 5f74 206e 756d 5f73   ptrdiff_t num_s
-00001300: 6f75 7263 6573 5f70 6572 5f73 686f 742c  ources_per_shot,
-00001310: 0a20 2020 2020 2020 2020 2020 2020 636f  .             co
-00001320: 6e73 7420 7074 7264 6966 665f 7420 6e75  nst ptrdiff_t nu
-00001330: 6d5f 7265 6365 6976 6572 735f 7065 725f  m_receivers_per_
-00001340: 7368 6f74 2c20 636f 6e73 7420 5459 5045  shot, const TYPE
-00001350: 2064 742c 0a20 2020 2020 2020 2020 2020   dt,.           
-00001360: 2020 636f 6e73 7420 656e 756d 2077 6176    const enum wav
-00001370: 6566 6965 6c64 5f73 6176 655f 7374 7261  efield_save_stra
-00001380: 7465 6779 2073 6176 655f 7374 7261 7465  tegy save_strate
-00001390: 6779 293b 0a0a 2f2a 2042 6163 6b70 726f  gy);../* Backpro
-000013a0: 7061 6761 7469 6f6e 0a20 2a20 7761 7665  pagation. * wave
-000013b0: 6669 656c 643a 2054 776f 2074 696d 6520  field: Two time 
-000013c0: 7374 6570 7320 6f66 2074 6865 2077 6176  steps of the wav
-000013d0: 6566 6965 6c64 2066 6f72 2070 726f 7061  efield for propa
-000013e0: 6761 7469 6f6e 2e0a 202a 2020 2020 2020  gation.. *      
-000013f0: 3320 2a20 6e75 6d5f 7368 6f74 7320 2a20  3 * num_shots * 
-00001400: 6e75 6d65 6c5f 7065 725f 7368 6f74 2c0a  numel_per_shot,.
-00001410: 202a 2020 2020 2020 7768 6572 6520 6e75   *      where nu
-00001420: 6d65 6c5f 7065 725f 7368 6f74 2069 7320  mel_per_shot is 
-00001430: 7468 6520 6e75 6d62 6572 206f 6620 656c  the number of el
-00001440: 656d 656e 7473 2069 6e20 7468 6520 7061  ements in the pa
-00001450: 6464 6564 206d 6f64 656c 2e0a 202a 2061  dded model.. * a
-00001460: 7578 5f77 6176 6566 6965 6c64 3a20 504d  ux_wavefield: PM
-00001470: 4c20 6175 7869 6c69 6172 7920 7761 7665  L auxiliary wave
-00001480: 6669 656c 6473 2e0a 202a 2020 2020 2020  fields.. *      
-00001490: 3220 2a20 4155 585f 5349 5a45 202a 206e  2 * AUX_SIZE * n
-000014a0: 756d 5f73 686f 7473 202a 206e 756d 656c  um_shots * numel
-000014b0: 5f70 6572 5f73 686f 742c 2077 6865 7265  _per_shot, where
-000014c0: 2041 5558 5f53 495a 4520 3d20 3120 666f   AUX_SIZE = 1 fo
-000014d0: 7220 3144 2c0a 202a 2020 2020 2020 3220  r 1D,. *      2 
-000014e0: 666f 7220 3244 2c20 616e 6420 3420 666f  for 2D, and 4 fo
-000014f0: 7220 3344 2e0a 202a 206d 6f64 656c 5f67  r 3D.. * model_g
-00001500: 7261 643a 2054 6865 206f 7574 7075 7420  rad: The output 
-00001510: 696d 6167 652f 6d6f 6465 6c20 6772 6164  image/model grad
-00001520: 6965 6e74 2e0a 202a 2020 2020 2020 5468  ient.. *      Th
-00001530: 6520 7361 6d65 2073 697a 6520 6173 2074  e same size as t
-00001540: 6865 2075 6e70 6164 6465 6420 6d6f 6465  he unpadded mode
-00001550: 6c2e 204e 554c 4c20 6966 206e 6f74 2064  l. NULL if not d
-00001560: 6f69 6e67 206d 6f64 656c 2069 6e76 6572  oing model inver
-00001570: 7369 6f6e 2e0a 202a 2073 6f75 7263 655f  sion.. * source_
-00001580: 6772 6164 5f61 6d70 6c69 7475 6465 733a  grad_amplitudes:
-00001590: 2054 6865 206f 7574 7075 7420 736f 7572   The output sour
-000015a0: 6365 2061 6d70 6c69 7475 6465 7320 6772  ce amplitudes gr
-000015b0: 6164 6965 6e74 0a20 2a20 2020 2020 2054  adient. *      T
-000015c0: 6865 2073 616d 6520 7369 7a65 2061 7320  he same size as 
-000015d0: 736f 7572 6365 5f61 6d70 6c69 7475 6465  source_amplitude
-000015e0: 7320 6475 7269 6e67 2066 6f72 7761 7264  s during forward
-000015f0: 2e20 4e55 4c4c 2069 6620 6e6f 7420 646f  . NULL if not do
-00001600: 696e 670a 202a 2020 2020 2020 736f 7572  ing. *      sour
-00001610: 6365 2069 6e76 6572 7369 6f6e 2e0a 202a  ce inversion.. *
-00001620: 2061 646a 6f69 6e74 5f77 6176 6566 6965   adjoint_wavefie
-00001630: 6c64 733a 2053 6176 6564 2077 6176 6566  lds: Saved wavef
-00001640: 6965 6c64 7320 6672 6f6d 2066 6f72 7761  ields from forwa
-00001650: 7264 206d 6f64 656c 696e 672e 0a20 2a20  rd modeling.. * 
-00001660: 2020 2020 206e 756d 5f73 7465 7073 202a       num_steps *
-00001670: 206e 756d 5f73 686f 7473 202a 206e 756d   num_shots * num
-00001680: 656c 5f70 6572 5f73 686f 742e 0a20 2a20  el_per_shot.. * 
-00001690: 7363 616c 696e 673a 2054 6865 2066 6163  scaling: The fac
-000016a0: 746f 7220 7468 6174 206d 756c 7469 706c  tor that multipl
-000016b0: 6965 7320 7468 6520 7a65 726f 2d6c 6167  ies the zero-lag
-000016c0: 2063 726f 7373 2d63 6f72 7265 6c61 7469   cross-correlati
-000016d0: 6f6e 2069 6d61 6769 6e67 0a20 2a20 2020  on imaging. *   
-000016e0: 2020 2063 6f6e 6469 7469 6f6e 2074 6f20     condition to 
-000016f0: 7475 726e 2069 7420 696e 746f 2074 6865  turn it into the
-00001700: 206d 6f64 656c 2067 7261 6469 656e 742e   model gradient.
-00001710: 2054 7970 6963 616c 6c79 2032 202f 2063   Typically 2 / c
-00001720: 5e33 2e0a 202a 2020 2020 2020 5361 6d65  ^3.. *      Same
-00001730: 2073 6861 7065 2061 7320 696d 6167 652e   shape as image.
-00001740: 0a20 2a20 7369 676d 613a 2050 4d4c 2073  . * sigma: PML s
-00001750: 6967 6d61 2e20 4e75 6d62 6572 206f 6620  igma. Number of 
-00001760: 656c 656d 656e 7473 2069 7320 7468 6520  elements is the 
-00001770: 7375 6d20 6f66 2074 6865 2070 6164 6465  sum of the padde
-00001780: 6420 6c65 6e67 7468 206f 660a 202a 2020  d length of. *  
-00001790: 2020 2020 6561 6368 2064 696d 656e 7369      each dimensi
-000017a0: 6f6e 2c20 652e 672e 2073 6861 7065 5b30  on, e.g. shape[0
-000017b0: 5d20 2b20 7368 6170 655b 315d 202b 2073  ] + shape[1] + s
-000017c0: 6861 7065 5b32 5d20 696e 2033 442e 0a20  hape[2] in 3D.. 
-000017d0: 2a20 6d6f 6465 6c3a 2050 6164 6465 6420  * model: Padded 
-000017e0: 7761 7665 2073 7065 6564 206d 6f64 656c  wave speed model
-000017f0: 2e20 4c65 6e67 7468 2069 6e20 6561 6368  . Length in each
-00001800: 2064 696d 656e 7369 6f6e 2069 7320 7468   dimension is th
-00001810: 6520 756e 7061 6464 6564 0a20 2a20 2020  e unpadded. *   
-00001820: 2020 206c 656e 6774 6820 2b20 7468 6520     length + the 
-00001830: 6669 6e69 7465 2064 6966 6665 7265 6e63  finite differenc
-00001840: 6520 6163 6375 7261 6379 206f 7264 6572  e accuracy order
-00001850: 202b 2032 202a 2070 6d6c 5f77 6964 7468   + 2 * pml_width
-00001860: 2e20 5061 6464 6564 0a20 2a20 2020 2020  . Padded. *     
-00001870: 2072 6567 696f 6e73 2073 686f 756c 6420   regions should 
-00001880: 7265 706c 6963 6174 6520 7468 6520 6564  replicate the ed
-00001890: 6765 206f 6620 7468 6520 756e 7061 6464  ge of the unpadd
-000018a0: 6564 206d 6f64 656c 2e0a 202a 2066 6431  ed model.. * fd1
-000018b0: 3a20 4669 7273 7420 6465 7269 7661 7469  : First derivati
-000018c0: 7665 2066 696e 6974 6520 6469 6666 6572  ve finite differ
-000018d0: 656e 6365 2063 6f65 6666 6963 6965 6e74  ence coefficient
-000018e0: 7320 286f 6e65 2073 6964 6529 2e0a 202a  s (one side).. *
-000018f0: 2020 2020 2020 4861 6c66 2066 696e 6974        Half finit
-00001900: 6520 6469 6666 6572 656e 6365 2061 6363  e difference acc
-00001910: 7572 6163 7920 6f72 6465 7220 2a20 6e75  uracy order * nu
-00001920: 6d5f 6469 6d73 2e0a 202a 2066 6432 3a20  m_dims.. * fd2: 
-00001930: 5365 636f 6e64 2064 6572 6976 6174 6976  Second derivativ
-00001940: 6520 6669 6e69 7465 2064 6966 6665 7265  e finite differe
-00001950: 6e63 6520 636f 6566 6669 6369 656e 7473  nce coefficients
-00001960: 2028 706f 7369 7469 7665 2073 6964 6529   (positive side)
-00001970: 2e0a 202a 2020 2020 2020 4861 6c66 2066  .. *      Half f
-00001980: 696e 6974 6520 6469 6666 6572 656e 6365  inite difference
-00001990: 2061 6363 7572 6163 7920 6f72 6465 7220   accuracy order 
-000019a0: 2a20 6e75 6d5f 6469 6d73 202b 2031 2e20  * num_dims + 1. 
-000019b0: 5468 6520 222b 2031 220a 202a 2020 2020  The "+ 1". *    
-000019c0: 2020 636f 6e74 6169 6e73 2074 6865 2063    contains the c
-000019d0: 6f65 6666 6963 6965 6e74 2066 6f72 2074  oefficient for t
-000019e0: 6865 2063 656e 7472 616c 2065 6c65 6d65  he central eleme
-000019f0: 6e74 2e0a 202a 2072 6563 6569 7665 725f  nt.. * receiver_
-00001a00: 6772 6164 5f61 6d70 6c69 7475 6465 733a  grad_amplitudes:
-00001a10: 2054 6865 2067 7261 6469 656e 7420 6f66   The gradient of
-00001a20: 2074 6865 206c 6f73 7320 7772 7420 7468   the loss wrt th
-00001a30: 6520 7265 6365 6976 6572 0a20 2a20 2020  e receiver. *   
-00001a40: 2020 2061 6d70 6c69 7475 6465 732e 206e     amplitudes. n
-00001a50: 756d 5f73 7465 7073 202a 206e 756d 5f73  um_steps * num_s
-00001a60: 686f 7473 202a 206e 756d 5f72 6563 6569  hots * num_recei
-00001a70: 7665 7273 5f70 6572 5f73 686f 740a 202a  vers_per_shot. *
-00001a80: 2073 6f75 7263 655f 6c6f 6361 7469 6f6e   source_location
-00001a90: 733a 204c 6f63 6174 696f 6e73 2069 6e20  s: Locations in 
-00001aa0: 756e 6974 7320 6f66 2063 656c 6c73 2c20  units of cells, 
-00001ab0: 6672 6f6d 206f 7269 6769 6e20 6f66 206d  from origin of m
-00001ac0: 6f64 656c 2e0a 202a 2020 2020 2020 6e75  odel.. *      nu
-00001ad0: 6d5f 7368 6f74 7320 2a20 6e75 6d5f 736f  m_shots * num_so
-00001ae0: 7572 6365 735f 7065 725f 7368 6f74 202a  urces_per_shot *
-00001af0: 206e 756d 5f64 696d 730a 202a 2072 6563   num_dims. * rec
-00001b00: 6569 7665 725f 6c6f 6361 7469 6f6e 733a  eiver_locations:
-00001b10: 204c 6f63 6174 696f 6e73 2069 6e20 756e   Locations in un
-00001b20: 6974 7320 6f66 2063 656c 6c73 2c20 6672  its of cells, fr
-00001b30: 6f6d 206f 7269 6769 6e20 6f66 206d 6f64  om origin of mod
-00001b40: 656c 2e0a 202a 2020 2020 2020 6e75 6d5f  el.. *      num_
-00001b50: 7368 6f74 7320 2a20 6e75 6d5f 7265 6365  shots * num_rece
-00001b60: 6976 6572 735f 7065 725f 7368 6f74 202a  ivers_per_shot *
-00001b70: 206e 756d 5f64 696d 730a 202a 2073 6861   num_dims. * sha
-00001b80: 7065 3a20 5061 6464 6564 2073 6861 7065  pe: Padded shape
-00001b90: 206f 6620 7468 6520 6d6f 6465 6c2e 2033   of the model. 3
-00001ba0: 2065 6c65 6d65 6e74 732c 2077 6974 6820   elements, with 
-00001bb0: 6d69 6e69 6d75 6d20 7661 6c75 6520 312c  minimum value 1,
-00001bc0: 2065 2e67 2e0a 202a 2020 2020 2020 3130   e.g.. *      10
-00001bd0: 302c 2031 2c20 3120 666f 7220 3144 2e0a  0, 1, 1 for 1D..
-00001be0: 202a 2070 6d6c 5f77 6964 7468 3a20 4e75   * pml_width: Nu
-00001bf0: 6d62 6572 206f 6620 504d 4c20 6365 6c6c  mber of PML cell
-00001c00: 732e 2036 2065 6c65 6d65 6e74 732c 2062  s. 6 elements, b
-00001c10: 6567 696e 6e69 6e67 2061 6e64 2065 6e64  eginning and end
-00001c20: 206f 6620 6561 6368 0a20 2a20 2020 2020   of each. *     
-00001c30: 2064 696d 656e 7369 6f6e 2c20 7769 7468   dimension, with
-00001c40: 206d 696e 696d 756d 2076 616c 7565 2030   minimum value 0
-00001c50: 2c20 652e 672e 2031 302c 2031 302c 2030  , e.g. 10, 10, 0
-00001c60: 2c20 302c 2030 2c20 3020 666f 7220 3144  , 0, 0, 0 for 1D
-00001c70: 2e0a 202a 206e 756d 5f73 7465 7073 3a20  .. * num_steps: 
-00001c80: 4e75 6d62 6572 206f 6620 7469 6d65 2073  Number of time s
-00001c90: 616d 706c 6573 2069 6e20 736f 7572 6365  amples in source
-00001ca0: 2061 6d70 6c69 7475 6465 7320 2861 6c73   amplitudes (als
-00001cb0: 6f20 7468 6520 7361 6d65 2061 730a 202a  o the same as. *
-00001cc0: 2020 2020 2020 7468 6520 6e75 6d62 6572        the number
-00001cd0: 206f 6620 7469 6d65 2073 616d 706c 6573   of time samples
-00001ce0: 2069 6e20 6f75 7470 7574 2072 6563 6569   in output recei
-00001cf0: 7665 7220 616d 706c 6974 7564 6573 2c20  ver amplitudes, 
-00001d00: 616e 6420 7468 650a 202a 2020 2020 2020  and the. *      
-00001d10: 6e75 6d62 6572 206f 6620 7361 7665 6420  number of saved 
-00001d20: 7761 7665 6669 656c 6473 292e 0a20 2a20  wavefields).. * 
-00001d30: 7374 6570 5f72 6174 696f 3a20 5468 6520  step_ratio: The 
-00001d40: 6e75 6d62 6572 206f 6620 696e 6e65 7220  number of inner 
-00001d50: 7469 6d65 2073 7465 7073 206f 6620 7468  time steps of th
-00001d60: 6520 7072 6f70 6167 6174 6f72 2062 6574  e propagator bet
-00001d70: 7765 656e 2065 6163 680a 202a 2020 2020  ween each. *    
-00001d80: 2020 6561 6368 2073 6f75 7263 6520 616d    each source am
-00001d90: 706c 6974 7564 6520 7469 6d65 2073 616d  plitude time sam
-00001da0: 706c 652e 0a20 2a20 6e75 6d5f 7368 6f74  ple.. * num_shot
-00001db0: 730a 202a 206e 756d 5f73 6f75 7263 6573  s. * num_sources
-00001dc0: 5f70 6572 5f73 686f 740a 202a 206e 756d  _per_shot. * num
-00001dd0: 5f72 6563 6569 7665 7273 5f70 6572 5f73  _receivers_per_s
-00001de0: 686f 740a 202a 2064 743a 2054 6865 2074  hot. * dt: The t
-00001df0: 696d 6520 696e 7465 7276 616c 2062 6574  ime interval bet
-00001e00: 7765 656e 2070 726f 7061 6761 746f 7220  ween propagator 
-00001e10: 7469 6d65 2073 7465 7073 2028 4e4f 5420  time steps (NOT 
-00001e20: 7468 6520 7469 6d65 2069 6e74 6572 7661  the time interva
-00001e30: 6c0a 202a 2020 2020 2020 6265 7477 6565  l. *      betwee
-00001e40: 6e20 736f 7572 6365 2061 6d70 6c69 7475  n source amplitu
-00001e50: 6465 2073 616d 706c 6573 202d 2074 6861  de samples - tha
-00001e60: 7420 776f 756c 6420 6265 2064 7420 2a20  t would be dt * 
-00001e70: 7374 6570 5f72 6174 696f 292e 0a20 2a2f  step_ratio).. */
-00001e80: 0a76 6f69 6420 6261 636b 7761 7264 2854  .void backward(T
-00001e90: 5950 4520 2a20 636f 6e73 7420 7761 7665  YPE * const wave
-00001ea0: 6669 656c 642c 0a20 2020 2020 2020 2020  field,.         
-00001eb0: 2020 2020 2054 5950 4520 2a20 636f 6e73       TYPE * cons
-00001ec0: 7420 6175 785f 7761 7665 6669 656c 642c  t aux_wavefield,
-00001ed0: 0a20 2020 2020 2020 2020 2020 2020 2054  .              T
-00001ee0: 5950 4520 2a20 636f 6e73 7420 6d6f 6465  YPE * const mode
-00001ef0: 6c5f 6772 6164 2c0a 2020 2020 2020 2020  l_grad,.        
-00001f00: 2020 2020 2020 5459 5045 202a 2063 6f6e        TYPE * con
-00001f10: 7374 2073 6f75 7263 655f 6772 6164 5f61  st source_grad_a
-00001f20: 6d70 6c69 7475 6465 732c 0a20 2020 2020  mplitudes,.     
-00001f30: 2020 2020 2020 2020 2063 6f6e 7374 2054           const T
-00001f40: 5950 4520 2a20 636f 6e73 7420 6164 6a6f  YPE * const adjo
-00001f50: 696e 745f 7761 7665 6669 656c 642c 0a20  int_wavefield,. 
-00001f60: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001f70: 7374 2054 5950 4520 2a20 636f 6e73 7420  st TYPE * const 
-00001f80: 7363 616c 696e 672c 0a20 2020 2020 2020  scaling,.       
-00001f90: 2020 2020 2020 2063 6f6e 7374 2054 5950         const TYP
-00001fa0: 4520 2a20 636f 6e73 7420 7369 676d 612c  E * const sigma,
-00001fb0: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
-00001fc0: 6f6e 7374 2054 5950 4520 2a20 636f 6e73  onst TYPE * cons
-00001fd0: 7420 6d6f 6465 6c2c 0a20 2020 2020 2020  t model,.       
-00001fe0: 2020 2020 2020 2063 6f6e 7374 2054 5950         const TYP
-00001ff0: 4520 2a20 636f 6e73 7420 6664 312c 0a20  E * const fd1,. 
-00002000: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00002010: 7374 2054 5950 4520 2a20 636f 6e73 7420  st TYPE * const 
-00002020: 6664 322c 0a20 2020 2020 2020 2020 2020  fd2,.           
-00002030: 2020 2063 6f6e 7374 2054 5950 4520 2a20     const TYPE * 
-00002040: 636f 6e73 7420 7265 6365 6976 6572 5f67  const receiver_g
-00002050: 7261 645f 616d 706c 6974 7564 6573 2c0a  rad_amplitudes,.
-00002060: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002070: 6e73 7420 7074 7264 6966 665f 7420 2a20  nst ptrdiff_t * 
-00002080: 636f 6e73 7420 736f 7572 6365 5f6c 6f63  const source_loc
-00002090: 6174 696f 6e73 2c0a 2020 2020 2020 2020  ations,.        
-000020a0: 2020 2020 2020 636f 6e73 7420 7074 7264        const ptrd
-000020b0: 6966 665f 7420 2a20 636f 6e73 7420 7265  iff_t * const re
-000020c0: 6365 6976 6572 5f6c 6f63 6174 696f 6e73  ceiver_locations
-000020d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000020e0: 636f 6e73 7420 7074 7264 6966 665f 7420  const ptrdiff_t 
-000020f0: 2a20 636f 6e73 7420 7368 6170 652c 0a20  * const shape,. 
-00002100: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00002110: 7374 2070 7472 6469 6666 5f74 202a 2063  st ptrdiff_t * c
-00002120: 6f6e 7374 2070 6d6c 5f77 6964 7468 2c0a  onst pml_width,.
-00002130: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002140: 6e73 7420 7074 7264 6966 665f 7420 6e75  nst ptrdiff_t nu
-00002150: 6d5f 7374 6570 732c 2063 6f6e 7374 2070  m_steps, const p
-00002160: 7472 6469 6666 5f74 2073 7465 705f 7261  trdiff_t step_ra
-00002170: 7469 6f2c 0a20 2020 2020 2020 2020 2020  tio,.           
-00002180: 2020 2063 6f6e 7374 2070 7472 6469 6666     const ptrdiff
-00002190: 5f74 206e 756d 5f73 686f 7473 2c20 636f  _t num_shots, co
-000021a0: 6e73 7420 7074 7264 6966 665f 7420 6e75  nst ptrdiff_t nu
-000021b0: 6d5f 736f 7572 6365 735f 7065 725f 7368  m_sources_per_sh
-000021c0: 6f74 2c0a 2020 2020 2020 2020 2020 2020  ot,.            
-000021d0: 2020 636f 6e73 7420 7074 7264 6966 665f    const ptrdiff_
-000021e0: 7420 6e75 6d5f 7265 6365 6976 6572 735f  t num_receivers_
-000021f0: 7065 725f 7368 6f74 2c20 636f 6e73 7420  per_shot, const 
-00002200: 5459 5045 2064 7429 3b0a 0a54 5950 4520  TYPE dt);..TYPE 
-00002210: 2a73 6574 5f73 7465 705f 706f 696e 7465  *set_step_pointe
-00002220: 7228 636f 6e73 7420 5459 5045 202a 2063  r(const TYPE * c
-00002230: 6f6e 7374 206f 7269 6769 6e2c 0a20 2020  onst origin,.   
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2020 636f 6e73 7420 7074 7264 6966      const ptrdif
-00002260: 665f 7420 7374 6570 2c20 636f 6e73 7420  f_t step, const 
-00002270: 7074 7264 6966 665f 7420 6e75 6d5f 7368  ptrdiff_t num_sh
-00002280: 6f74 732c 0a20 2020 2020 2020 2020 2020  ots,.           
-00002290: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-000022a0: 7420 7074 7264 6966 665f 7420 6e75 6d65  t ptrdiff_t nume
-000022b0: 6c5f 7065 725f 7368 6f74 293b 0a0a 2f2a  l_per_shot);../*
-000022c0: 2044 696d 656e 7369 6f6e 2d73 7065 6369   Dimension-speci
-000022d0: 6669 6320 6465 6669 6e69 7469 6f6e 730a  fic definitions.
-000022e0: 202a 0a20 2a20 5a50 4144 2f59 5041 442f   *. * ZPAD/YPAD/
-000022f0: 5850 4144 3a20 4e75 6d62 6572 206f 6620  XPAD: Number of 
-00002300: 6365 6c6c 7320 6f66 2070 6164 6469 6e67  cells of padding
-00002310: 2061 7420 7468 6520 6265 6769 6e6e 696e   at the beginnin
-00002320: 6720 616e 6420 656e 6420 6f66 0a20 2a20  g and end of. * 
-00002330: 2020 2020 207a 2c20 792c 2061 6e64 2078       z, y, and x
-00002340: 2064 696d 656e 7369 6f6e 7320 746f 206d   dimensions to m
-00002350: 616b 6520 6669 6e69 7465 2064 6966 6665  ake finite diffe
-00002360: 7265 6e63 6520 6361 6c63 756c 6174 696f  rence calculatio
-00002370: 6e20 636c 6561 6e65 720a 202a 2041 5558  n cleaner. * AUX
-00002380: 5f53 495a 453a 204e 756d 6265 7220 6f66  _SIZE: Number of
-00002390: 2061 7578 696c 6961 7279 2077 6176 6566   auxiliary wavef
-000023a0: 6965 6c64 730a 202a 202a 2f0a 2369 6620  ields. * */.#if 
-000023b0: 4449 4d20 3d3d 2031 0a0a 2364 6566 696e  DIM == 1..#defin
-000023c0: 6520 5a50 4144 2032 0a23 6465 6669 6e65  e ZPAD 2.#define
-000023d0: 2059 5041 4420 300a 2364 6566 696e 6520   YPAD 0.#define 
-000023e0: 5850 4144 2030 0a0a 2364 6566 696e 6520  XPAD 0..#define 
-000023f0: 4155 585f 5349 5a45 2031 0a0a 2365 6c69  AUX_SIZE 1..#eli
-00002400: 6620 4449 4d20 3d3d 2032 0a0a 2364 6566  f DIM == 2..#def
-00002410: 696e 6520 5a50 4144 2032 0a23 6465 6669  ine ZPAD 2.#defi
-00002420: 6e65 2059 5041 4420 320a 2364 6566 696e  ne YPAD 2.#defin
-00002430: 6520 5850 4144 2030 0a0a 2364 6566 696e  e XPAD 0..#defin
-00002440: 6520 4155 585f 5349 5a45 2032 0a0a 2365  e AUX_SIZE 2..#e
-00002450: 6c69 6620 4449 4d20 3d3d 2033 0a0a 2364  lif DIM == 3..#d
-00002460: 6566 696e 6520 5a50 4144 2032 0a23 6465  efine ZPAD 2.#de
-00002470: 6669 6e65 2059 5041 4420 320a 2364 6566  fine YPAD 2.#def
-00002480: 696e 6520 5850 4144 2032 0a0a 2364 6566  ine XPAD 2..#def
-00002490: 696e 6520 4155 585f 5349 5a45 2034 0a0a  ine AUX_SIZE 4..
-000024a0: 2365 6c73 650a 2365 7272 6f72 2022 4d75  #else.#error "Mu
-000024b0: 7374 2073 7065 6369 6679 2074 6865 2064  st specify the d
-000024c0: 696d 656e 7369 6f6e 2c20 652e 672e 202d  imension, e.g. -
-000024d0: 4420 4449 4d3d 3122 0a23 656e 6469 6620  D DIM=1".#endif 
-000024e0: 2f2a 2044 494d 202a 2f0a 0a23 656e 6469  /* DIM */..#endi
-000024f0: 6620 2f2a 2044 4545 5057 4156 455f 5343  f /* DEEPWAVE_SC
-00002500: 414c 4152 5f53 4341 4c41 525f 4820 2a2f  ALAR_SCALAR_H */
-00002510: 0a                                       .
+00000b40: 7264 2844 4545 5057 4156 455f 5459 5045  rd(DEEPWAVE_TYPE
+00000b50: 202a 2063 6f6e 7374 2077 6176 6566 6965   * const wavefie
+00000b60: 6c64 2c0a 2020 2020 2020 2020 2020 2020  ld,.            
+00000b70: 2044 4545 5057 4156 455f 5459 5045 202a   DEEPWAVE_TYPE *
+00000b80: 2063 6f6e 7374 2061 7578 5f77 6176 6566   const aux_wavef
+00000b90: 6965 6c64 2c0a 2020 2020 2020 2020 2020  ield,.          
+00000ba0: 2020 2044 4545 5057 4156 455f 5459 5045     DEEPWAVE_TYPE
+00000bb0: 202a 2063 6f6e 7374 2072 6563 6569 7665   * const receive
+00000bc0: 725f 616d 706c 6974 7564 6573 2c0a 2020  r_amplitudes,.  
+00000bd0: 2020 2020 2020 2020 2020 2044 4545 5057             DEEPW
+00000be0: 4156 455f 5459 5045 202a 2063 6f6e 7374  AVE_TYPE * const
+00000bf0: 2073 6176 6564 5f77 6176 6566 6965 6c64   saved_wavefield
+00000c00: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00000c10: 636f 6e73 7420 4445 4550 5741 5645 5f54  const DEEPWAVE_T
+00000c20: 5950 4520 2a20 636f 6e73 7420 7369 676d  YPE * const sigm
+00000c30: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00000c40: 636f 6e73 7420 4445 4550 5741 5645 5f54  const DEEPWAVE_T
+00000c50: 5950 4520 2a20 636f 6e73 7420 6d6f 6465  YPE * const mode
+00000c60: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00000c70: 636f 6e73 7420 4445 4550 5741 5645 5f54  const DEEPWAVE_T
+00000c80: 5950 4520 2a20 636f 6e73 7420 6664 312c  YPE * const fd1,
+00000c90: 0a20 2020 2020 2020 2020 2020 2020 636f  .             co
+00000ca0: 6e73 7420 4445 4550 5741 5645 5f54 5950  nst DEEPWAVE_TYP
+00000cb0: 4520 2a20 636f 6e73 7420 6664 322c 0a20  E * const fd2,. 
+00000cc0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00000cd0: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+00000ce0: 2a20 636f 6e73 7420 736f 7572 6365 5f61  * const source_a
+00000cf0: 6d70 6c69 7475 6465 732c 0a20 2020 2020  mplitudes,.     
+00000d00: 2020 2020 2020 2020 636f 6e73 7420 7074          const pt
+00000d10: 7264 6966 665f 7420 2a20 636f 6e73 7420  rdiff_t * const 
+00000d20: 736f 7572 6365 5f6c 6f63 6174 696f 6e73  source_locations
+00000d30: 2c0a 2020 2020 2020 2020 2020 2020 2063  ,.             c
+00000d40: 6f6e 7374 2070 7472 6469 6666 5f74 202a  onst ptrdiff_t *
+00000d50: 2063 6f6e 7374 2072 6563 6569 7665 725f   const receiver_
+00000d60: 6c6f 6361 7469 6f6e 732c 0a20 2020 2020  locations,.     
+00000d70: 2020 2020 2020 2020 636f 6e73 7420 7074          const pt
+00000d80: 7264 6966 665f 7420 2a20 636f 6e73 7420  rdiff_t * const 
+00000d90: 7368 6170 652c 0a20 2020 2020 2020 2020  shape,.         
+00000da0: 2020 2020 636f 6e73 7420 7074 7264 6966      const ptrdif
+00000db0: 665f 7420 2a20 636f 6e73 7420 706d 6c5f  f_t * const pml_
+00000dc0: 7769 6474 682c 0a20 2020 2020 2020 2020  width,.         
+00000dd0: 2020 2020 636f 6e73 7420 7074 7264 6966      const ptrdif
+00000de0: 665f 7420 6e75 6d5f 7374 6570 732c 2063  f_t num_steps, c
+00000df0: 6f6e 7374 2070 7472 6469 6666 5f74 2073  onst ptrdiff_t s
+00000e00: 7465 705f 7261 7469 6f2c 0a20 2020 2020  tep_ratio,.     
+00000e10: 2020 2020 2020 2020 636f 6e73 7420 7074          const pt
+00000e20: 7264 6966 665f 7420 6e75 6d5f 7368 6f74  rdiff_t num_shot
+00000e30: 732c 2063 6f6e 7374 2070 7472 6469 6666  s, const ptrdiff
+00000e40: 5f74 206e 756d 5f73 6f75 7263 6573 5f70  _t num_sources_p
+00000e50: 6572 5f73 686f 742c 0a20 2020 2020 2020  er_shot,.       
+00000e60: 2020 2020 2020 636f 6e73 7420 7074 7264        const ptrd
+00000e70: 6966 665f 7420 6e75 6d5f 7265 6365 6976  iff_t num_receiv
+00000e80: 6572 735f 7065 725f 7368 6f74 2c20 636f  ers_per_shot, co
+00000e90: 6e73 7420 4445 4550 5741 5645 5f54 5950  nst DEEPWAVE_TYP
+00000ea0: 4520 6474 2c0a 2020 2020 2020 2020 2020  E dt,.          
+00000eb0: 2020 2063 6f6e 7374 2065 6e75 6d20 7761     const enum wa
+00000ec0: 7665 6669 656c 645f 7361 7665 5f73 7472  vefield_save_str
+00000ed0: 6174 6567 7920 7361 7665 5f73 7472 6174  ategy save_strat
+00000ee0: 6567 7929 3b0a 0a2f 2a20 426f 726e 2066  egy);../* Born f
+00000ef0: 6f72 7761 7264 206d 6f64 656c 696e 670a  orward modeling.
+00000f00: 202a 2041 7267 756d 656e 7473 2061 7265   * Arguments are
+00000f10: 2074 6865 2073 616d 6520 6173 2072 6567   the same as reg
+00000f20: 756c 6172 2066 6f72 7761 7264 206d 6f64  ular forward mod
+00000f30: 656c 696e 672c 2065 7863 6570 7420 666f  eling, except fo
+00000f40: 7220 7468 6520 666f 6c6c 6f77 696e 670a  r the following.
+00000f50: 202a 2073 6361 7474 6572 6564 5f77 6176   * scattered_wav
+00000f60: 6566 6965 6c64 3a20 4c69 6b65 2077 6176  efield: Like wav
+00000f70: 6566 6965 6c64 2c20 6275 7420 666f 7220  efield, but for 
+00000f80: 7363 6174 7465 7265 6420 7761 7665 730a  scattered waves.
+00000f90: 202a 2073 6361 7474 6572 6564 5f61 7578   * scattered_aux
+00000fa0: 5f77 6176 6566 6965 6c64 3a20 4c69 6b65  _wavefield: Like
+00000fb0: 2061 7578 5f77 6176 6566 6965 6c64 2c20   aux_wavefield, 
+00000fc0: 6275 7420 666f 7220 7363 6174 7465 7265  but for scattere
+00000fd0: 6420 7761 7665 730a 202a 2073 6361 7474  d waves. * scatt
+00000fe0: 6572 3a20 4c69 6b65 206d 6f64 656c 2c20  er: Like model, 
+00000ff0: 6275 7420 636f 6e74 6169 6e73 2074 6865  but contains the
+00001000: 2073 6361 7474 6572 696e 6720 616d 706c   scattering ampl
+00001010: 6974 7564 650a 202a 2f0a 766f 6964 2066  itude. */.void f
+00001020: 6f72 7761 7264 5f62 6f72 6e28 4445 4550  orward_born(DEEP
+00001030: 5741 5645 5f54 5950 4520 2a20 636f 6e73  WAVE_TYPE * cons
+00001040: 7420 7761 7665 6669 656c 642c 0a20 2020  t wavefield,.   
+00001050: 2020 2020 2020 2020 2020 4445 4550 5741            DEEPWA
+00001060: 5645 5f54 5950 4520 2a20 636f 6e73 7420  VE_TYPE * const 
+00001070: 6175 785f 7761 7665 6669 656c 642c 0a20  aux_wavefield,. 
+00001080: 2020 2009 2020 2020 2044 4545 5057 4156     .     DEEPWAV
+00001090: 455f 5459 5045 202a 2063 6f6e 7374 2073  E_TYPE * const s
+000010a0: 6361 7474 6572 6564 5f77 6176 6566 6965  cattered_wavefie
+000010b0: 6c64 2c0a 0920 2020 2020 4445 4550 5741  ld,..     DEEPWA
+000010c0: 5645 5f54 5950 4520 2a20 636f 6e73 7420  VE_TYPE * const 
+000010d0: 7363 6174 7465 7265 645f 6175 785f 7761  scattered_aux_wa
+000010e0: 7665 6669 656c 642c 0a20 2020 2020 2020  vefield,.       
+000010f0: 2020 2020 2020 4445 4550 5741 5645 5f54        DEEPWAVE_T
+00001100: 5950 4520 2a20 636f 6e73 7420 7265 6365  YPE * const rece
+00001110: 6976 6572 5f61 6d70 6c69 7475 6465 732c  iver_amplitudes,
+00001120: 0a20 2020 2020 2020 2020 2020 2020 4445  .             DE
+00001130: 4550 5741 5645 5f54 5950 4520 2a20 636f  EPWAVE_TYPE * co
+00001140: 6e73 7420 7361 7665 645f 7761 7665 6669  nst saved_wavefi
+00001150: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
+00001160: 2020 2063 6f6e 7374 2044 4545 5057 4156     const DEEPWAV
+00001170: 455f 5459 5045 202a 2063 6f6e 7374 2073  E_TYPE * const s
+00001180: 6967 6d61 2c0a 2020 2020 2020 2020 2020  igma,.          
+00001190: 2020 2063 6f6e 7374 2044 4545 5057 4156     const DEEPWAV
+000011a0: 455f 5459 5045 202a 2063 6f6e 7374 206d  E_TYPE * const m
+000011b0: 6f64 656c 2c0a 0920 2020 2020 636f 6e73  odel,..     cons
+000011c0: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+000011d0: 2a20 636f 6e73 7420 7363 6174 7465 722c  * const scatter,
+000011e0: 0a20 2020 2020 2020 2020 2020 2020 636f  .             co
+000011f0: 6e73 7420 4445 4550 5741 5645 5f54 5950  nst DEEPWAVE_TYP
+00001200: 4520 2a20 636f 6e73 7420 6664 312c 0a20  E * const fd1,. 
+00001210: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00001220: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+00001230: 2a20 636f 6e73 7420 6664 322c 0a20 2020  * const fd2,.   
+00001240: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
+00001250: 4445 4550 5741 5645 5f54 5950 4520 2a20  DEEPWAVE_TYPE * 
+00001260: 636f 6e73 7420 736f 7572 6365 5f61 6d70  const source_amp
+00001270: 6c69 7475 6465 732c 0a20 2020 2020 2020  litudes,.       
+00001280: 2020 2020 2020 636f 6e73 7420 7074 7264        const ptrd
+00001290: 6966 665f 7420 2a20 636f 6e73 7420 736f  iff_t * const so
+000012a0: 7572 6365 5f6c 6f63 6174 696f 6e73 2c0a  urce_locations,.
+000012b0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000012c0: 7374 2070 7472 6469 6666 5f74 202a 2063  st ptrdiff_t * c
+000012d0: 6f6e 7374 2072 6563 6569 7665 725f 6c6f  onst receiver_lo
+000012e0: 6361 7469 6f6e 732c 0a20 2020 2020 2020  cations,.       
+000012f0: 2020 2020 2020 636f 6e73 7420 7074 7264        const ptrd
+00001300: 6966 665f 7420 2a20 636f 6e73 7420 7368  iff_t * const sh
+00001310: 6170 652c 0a20 2020 2020 2020 2020 2020  ape,.           
+00001320: 2020 636f 6e73 7420 7074 7264 6966 665f    const ptrdiff_
+00001330: 7420 2a20 636f 6e73 7420 706d 6c5f 7769  t * const pml_wi
+00001340: 6474 682c 0a20 2020 2020 2020 2020 2020  dth,.           
+00001350: 2020 636f 6e73 7420 7074 7264 6966 665f    const ptrdiff_
+00001360: 7420 6e75 6d5f 7374 6570 732c 2063 6f6e  t num_steps, con
+00001370: 7374 2070 7472 6469 6666 5f74 2073 7465  st ptrdiff_t ste
+00001380: 705f 7261 7469 6f2c 0a20 2020 2020 2020  p_ratio,.       
+00001390: 2020 2020 2020 636f 6e73 7420 7074 7264        const ptrd
+000013a0: 6966 665f 7420 6e75 6d5f 7368 6f74 732c  iff_t num_shots,
+000013b0: 2063 6f6e 7374 2070 7472 6469 6666 5f74   const ptrdiff_t
+000013c0: 206e 756d 5f73 6f75 7263 6573 5f70 6572   num_sources_per
+000013d0: 5f73 686f 742c 0a20 2020 2020 2020 2020  _shot,.         
+000013e0: 2020 2020 636f 6e73 7420 7074 7264 6966      const ptrdif
+000013f0: 665f 7420 6e75 6d5f 7265 6365 6976 6572  f_t num_receiver
+00001400: 735f 7065 725f 7368 6f74 2c20 636f 6e73  s_per_shot, cons
+00001410: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+00001420: 6474 2c0a 2020 2020 2020 2020 2020 2020  dt,.            
+00001430: 2063 6f6e 7374 2065 6e75 6d20 7761 7665   const enum wave
+00001440: 6669 656c 645f 7361 7665 5f73 7472 6174  field_save_strat
+00001450: 6567 7920 7361 7665 5f73 7472 6174 6567  egy save_strateg
+00001460: 7929 3b0a 0a2f 2a20 4261 636b 7072 6f70  y);../* Backprop
+00001470: 6167 6174 696f 6e0a 202a 2077 6176 6566  agation. * wavef
+00001480: 6965 6c64 3a20 5477 6f20 7469 6d65 2073  ield: Two time s
+00001490: 7465 7073 206f 6620 7468 6520 7761 7665  teps of the wave
+000014a0: 6669 656c 6420 666f 7220 7072 6f70 6167  field for propag
+000014b0: 6174 696f 6e2e 0a20 2a20 2020 2020 2033  ation.. *      3
+000014c0: 202a 206e 756d 5f73 686f 7473 202a 206e   * num_shots * n
+000014d0: 756d 656c 5f70 6572 5f73 686f 742c 0a20  umel_per_shot,. 
+000014e0: 2a20 2020 2020 2077 6865 7265 206e 756d  *      where num
+000014f0: 656c 5f70 6572 5f73 686f 7420 6973 2074  el_per_shot is t
+00001500: 6865 206e 756d 6265 7220 6f66 2065 6c65  he number of ele
+00001510: 6d65 6e74 7320 696e 2074 6865 2070 6164  ments in the pad
+00001520: 6465 6420 6d6f 6465 6c2e 0a20 2a20 6175  ded model.. * au
+00001530: 785f 7761 7665 6669 656c 643a 2050 4d4c  x_wavefield: PML
+00001540: 2061 7578 696c 6961 7279 2077 6176 6566   auxiliary wavef
+00001550: 6965 6c64 732e 0a20 2a20 2020 2020 2032  ields.. *      2
+00001560: 202a 2041 5558 5f53 495a 4520 2a20 6e75   * AUX_SIZE * nu
+00001570: 6d5f 7368 6f74 7320 2a20 6e75 6d65 6c5f  m_shots * numel_
+00001580: 7065 725f 7368 6f74 2c20 7768 6572 6520  per_shot, where 
+00001590: 4155 585f 5349 5a45 203d 2031 2066 6f72  AUX_SIZE = 1 for
+000015a0: 2031 442c 0a20 2a20 2020 2020 2032 2066   1D,. *      2 f
+000015b0: 6f72 2032 442c 2061 6e64 2034 2066 6f72  or 2D, and 4 for
+000015c0: 2033 442e 0a20 2a20 6d6f 6465 6c5f 6772   3D.. * model_gr
+000015d0: 6164 3a20 5468 6520 6f75 7470 7574 2069  ad: The output i
+000015e0: 6d61 6765 2f6d 6f64 656c 2067 7261 6469  mage/model gradi
+000015f0: 656e 742e 0a20 2a20 2020 2020 2054 6865  ent.. *      The
+00001600: 2073 616d 6520 7369 7a65 2061 7320 7468   same size as th
+00001610: 6520 756e 7061 6464 6564 206d 6f64 656c  e unpadded model
+00001620: 2e20 4e55 4c4c 2069 6620 6e6f 7420 646f  . NULL if not do
+00001630: 696e 6720 6d6f 6465 6c20 696e 7665 7273  ing model invers
+00001640: 696f 6e2e 0a20 2a20 736f 7572 6365 5f67  ion.. * source_g
+00001650: 7261 645f 616d 706c 6974 7564 6573 3a20  rad_amplitudes: 
+00001660: 5468 6520 6f75 7470 7574 2073 6f75 7263  The output sourc
+00001670: 6520 616d 706c 6974 7564 6573 2067 7261  e amplitudes gra
+00001680: 6469 656e 740a 202a 2020 2020 2020 5468  dient. *      Th
+00001690: 6520 7361 6d65 2073 697a 6520 6173 2073  e same size as s
+000016a0: 6f75 7263 655f 616d 706c 6974 7564 6573  ource_amplitudes
+000016b0: 2064 7572 696e 6720 666f 7277 6172 642e   during forward.
+000016c0: 204e 554c 4c20 6966 206e 6f74 2064 6f69   NULL if not doi
+000016d0: 6e67 0a20 2a20 2020 2020 2073 6f75 7263  ng. *      sourc
+000016e0: 6520 696e 7665 7273 696f 6e2e 0a20 2a20  e inversion.. * 
+000016f0: 6164 6a6f 696e 745f 7761 7665 6669 656c  adjoint_wavefiel
+00001700: 6473 3a20 5361 7665 6420 7761 7665 6669  ds: Saved wavefi
+00001710: 656c 6473 2066 726f 6d20 666f 7277 6172  elds from forwar
+00001720: 6420 6d6f 6465 6c69 6e67 2e0a 202a 2020  d modeling.. *  
+00001730: 2020 2020 6e75 6d5f 7374 6570 7320 2a20      num_steps * 
+00001740: 6e75 6d5f 7368 6f74 7320 2a20 6e75 6d65  num_shots * nume
+00001750: 6c5f 7065 725f 7368 6f74 2e0a 202a 2073  l_per_shot.. * s
+00001760: 6361 6c69 6e67 3a20 5468 6520 6661 6374  caling: The fact
+00001770: 6f72 2074 6861 7420 6d75 6c74 6970 6c69  or that multipli
+00001780: 6573 2074 6865 207a 6572 6f2d 6c61 6720  es the zero-lag 
+00001790: 6372 6f73 732d 636f 7272 656c 6174 696f  cross-correlatio
+000017a0: 6e20 696d 6167 696e 670a 202a 2020 2020  n imaging. *    
+000017b0: 2020 636f 6e64 6974 696f 6e20 746f 2074    condition to t
+000017c0: 7572 6e20 6974 2069 6e74 6f20 7468 6520  urn it into the 
+000017d0: 6d6f 6465 6c20 6772 6164 6965 6e74 2e20  model gradient. 
+000017e0: 5479 7069 6361 6c6c 7920 3220 2f20 635e  Typically 2 / c^
+000017f0: 332e 0a20 2a20 2020 2020 2053 616d 6520  3.. *      Same 
+00001800: 7368 6170 6520 6173 2069 6d61 6765 2e0a  shape as image..
+00001810: 202a 2073 6967 6d61 3a20 504d 4c20 7369   * sigma: PML si
+00001820: 676d 612e 204e 756d 6265 7220 6f66 2065  gma. Number of e
+00001830: 6c65 6d65 6e74 7320 6973 2074 6865 2073  lements is the s
+00001840: 756d 206f 6620 7468 6520 7061 6464 6564  um of the padded
+00001850: 206c 656e 6774 6820 6f66 0a20 2a20 2020   length of. *   
+00001860: 2020 2065 6163 6820 6469 6d65 6e73 696f     each dimensio
+00001870: 6e2c 2065 2e67 2e20 7368 6170 655b 305d  n, e.g. shape[0]
+00001880: 202b 2073 6861 7065 5b31 5d20 2b20 7368   + shape[1] + sh
+00001890: 6170 655b 325d 2069 6e20 3344 2e0a 202a  ape[2] in 3D.. *
+000018a0: 206d 6f64 656c 3a20 5061 6464 6564 2077   model: Padded w
+000018b0: 6176 6520 7370 6565 6420 6d6f 6465 6c2e  ave speed model.
+000018c0: 204c 656e 6774 6820 696e 2065 6163 6820   Length in each 
+000018d0: 6469 6d65 6e73 696f 6e20 6973 2074 6865  dimension is the
+000018e0: 2075 6e70 6164 6465 640a 202a 2020 2020   unpadded. *    
+000018f0: 2020 6c65 6e67 7468 202b 2074 6865 2066    length + the f
+00001900: 696e 6974 6520 6469 6666 6572 656e 6365  inite difference
+00001910: 2061 6363 7572 6163 7920 6f72 6465 7220   accuracy order 
+00001920: 2b20 3220 2a20 706d 6c5f 7769 6474 682e  + 2 * pml_width.
+00001930: 2050 6164 6465 640a 202a 2020 2020 2020   Padded. *      
+00001940: 7265 6769 6f6e 7320 7368 6f75 6c64 2072  regions should r
+00001950: 6570 6c69 6361 7465 2074 6865 2065 6467  eplicate the edg
+00001960: 6520 6f66 2074 6865 2075 6e70 6164 6465  e of the unpadde
+00001970: 6420 6d6f 6465 6c2e 0a20 2a20 6664 313a  d model.. * fd1:
+00001980: 2046 6972 7374 2064 6572 6976 6174 6976   First derivativ
+00001990: 6520 6669 6e69 7465 2064 6966 6665 7265  e finite differe
+000019a0: 6e63 6520 636f 6566 6669 6369 656e 7473  nce coefficients
+000019b0: 2028 6f6e 6520 7369 6465 292e 0a20 2a20   (one side).. * 
+000019c0: 2020 2020 2048 616c 6620 6669 6e69 7465       Half finite
+000019d0: 2064 6966 6665 7265 6e63 6520 6163 6375   difference accu
+000019e0: 7261 6379 206f 7264 6572 202a 206e 756d  racy order * num
+000019f0: 5f64 696d 732e 0a20 2a20 6664 323a 2053  _dims.. * fd2: S
+00001a00: 6563 6f6e 6420 6465 7269 7661 7469 7665  econd derivative
+00001a10: 2066 696e 6974 6520 6469 6666 6572 656e   finite differen
+00001a20: 6365 2063 6f65 6666 6963 6965 6e74 7320  ce coefficients 
+00001a30: 2870 6f73 6974 6976 6520 7369 6465 292e  (positive side).
+00001a40: 0a20 2a20 2020 2020 2048 616c 6620 6669  . *      Half fi
+00001a50: 6e69 7465 2064 6966 6665 7265 6e63 6520  nite difference 
+00001a60: 6163 6375 7261 6379 206f 7264 6572 202a  accuracy order *
+00001a70: 206e 756d 5f64 696d 7320 2b20 312e 2054   num_dims + 1. T
+00001a80: 6865 2022 2b20 3122 0a20 2a20 2020 2020  he "+ 1". *     
+00001a90: 2063 6f6e 7461 696e 7320 7468 6520 636f   contains the co
+00001aa0: 6566 6669 6369 656e 7420 666f 7220 7468  efficient for th
+00001ab0: 6520 6365 6e74 7261 6c20 656c 656d 656e  e central elemen
+00001ac0: 742e 0a20 2a20 7265 6365 6976 6572 5f67  t.. * receiver_g
+00001ad0: 7261 645f 616d 706c 6974 7564 6573 3a20  rad_amplitudes: 
+00001ae0: 5468 6520 6772 6164 6965 6e74 206f 6620  The gradient of 
+00001af0: 7468 6520 6c6f 7373 2077 7274 2074 6865  the loss wrt the
+00001b00: 2072 6563 6569 7665 720a 202a 2020 2020   receiver. *    
+00001b10: 2020 616d 706c 6974 7564 6573 2e20 6e75    amplitudes. nu
+00001b20: 6d5f 7374 6570 7320 2a20 6e75 6d5f 7368  m_steps * num_sh
+00001b30: 6f74 7320 2a20 6e75 6d5f 7265 6365 6976  ots * num_receiv
+00001b40: 6572 735f 7065 725f 7368 6f74 0a20 2a20  ers_per_shot. * 
+00001b50: 736f 7572 6365 5f6c 6f63 6174 696f 6e73  source_locations
+00001b60: 3a20 4c6f 6361 7469 6f6e 7320 696e 2075  : Locations in u
+00001b70: 6e69 7473 206f 6620 6365 6c6c 732c 2066  nits of cells, f
+00001b80: 726f 6d20 6f72 6967 696e 206f 6620 6d6f  rom origin of mo
+00001b90: 6465 6c2e 0a20 2a20 2020 2020 206e 756d  del.. *      num
+00001ba0: 5f73 686f 7473 202a 206e 756d 5f73 6f75  _shots * num_sou
+00001bb0: 7263 6573 5f70 6572 5f73 686f 7420 2a20  rces_per_shot * 
+00001bc0: 6e75 6d5f 6469 6d73 0a20 2a20 7265 6365  num_dims. * rece
+00001bd0: 6976 6572 5f6c 6f63 6174 696f 6e73 3a20  iver_locations: 
+00001be0: 4c6f 6361 7469 6f6e 7320 696e 2075 6e69  Locations in uni
+00001bf0: 7473 206f 6620 6365 6c6c 732c 2066 726f  ts of cells, fro
+00001c00: 6d20 6f72 6967 696e 206f 6620 6d6f 6465  m origin of mode
+00001c10: 6c2e 0a20 2a20 2020 2020 206e 756d 5f73  l.. *      num_s
+00001c20: 686f 7473 202a 206e 756d 5f72 6563 6569  hots * num_recei
+00001c30: 7665 7273 5f70 6572 5f73 686f 7420 2a20  vers_per_shot * 
+00001c40: 6e75 6d5f 6469 6d73 0a20 2a20 7368 6170  num_dims. * shap
+00001c50: 653a 2050 6164 6465 6420 7368 6170 6520  e: Padded shape 
+00001c60: 6f66 2074 6865 206d 6f64 656c 2e20 3320  of the model. 3 
+00001c70: 656c 656d 656e 7473 2c20 7769 7468 206d  elements, with m
+00001c80: 696e 696d 756d 2076 616c 7565 2031 2c20  inimum value 1, 
+00001c90: 652e 672e 0a20 2a20 2020 2020 2031 3030  e.g.. *      100
+00001ca0: 2c20 312c 2031 2066 6f72 2031 442e 0a20  , 1, 1 for 1D.. 
+00001cb0: 2a20 706d 6c5f 7769 6474 683a 204e 756d  * pml_width: Num
+00001cc0: 6265 7220 6f66 2050 4d4c 2063 656c 6c73  ber of PML cells
+00001cd0: 2e20 3620 656c 656d 656e 7473 2c20 6265  . 6 elements, be
+00001ce0: 6769 6e6e 696e 6720 616e 6420 656e 6420  ginning and end 
+00001cf0: 6f66 2065 6163 680a 202a 2020 2020 2020  of each. *      
+00001d00: 6469 6d65 6e73 696f 6e2c 2077 6974 6820  dimension, with 
+00001d10: 6d69 6e69 6d75 6d20 7661 6c75 6520 302c  minimum value 0,
+00001d20: 2065 2e67 2e20 3130 2c20 3130 2c20 302c   e.g. 10, 10, 0,
+00001d30: 2030 2c20 302c 2030 2066 6f72 2031 442e   0, 0, 0 for 1D.
+00001d40: 0a20 2a20 6e75 6d5f 7374 6570 733a 204e  . * num_steps: N
+00001d50: 756d 6265 7220 6f66 2074 696d 6520 7361  umber of time sa
+00001d60: 6d70 6c65 7320 696e 2073 6f75 7263 6520  mples in source 
+00001d70: 616d 706c 6974 7564 6573 2028 616c 736f  amplitudes (also
+00001d80: 2074 6865 2073 616d 6520 6173 0a20 2a20   the same as. * 
+00001d90: 2020 2020 2074 6865 206e 756d 6265 7220       the number 
+00001da0: 6f66 2074 696d 6520 7361 6d70 6c65 7320  of time samples 
+00001db0: 696e 206f 7574 7075 7420 7265 6365 6976  in output receiv
+00001dc0: 6572 2061 6d70 6c69 7475 6465 732c 2061  er amplitudes, a
+00001dd0: 6e64 2074 6865 0a20 2a20 2020 2020 206e  nd the. *      n
+00001de0: 756d 6265 7220 6f66 2073 6176 6564 2077  umber of saved w
+00001df0: 6176 6566 6965 6c64 7329 2e0a 202a 2073  avefields).. * s
+00001e00: 7465 705f 7261 7469 6f3a 2054 6865 206e  tep_ratio: The n
+00001e10: 756d 6265 7220 6f66 2069 6e6e 6572 2074  umber of inner t
+00001e20: 696d 6520 7374 6570 7320 6f66 2074 6865  ime steps of the
+00001e30: 2070 726f 7061 6761 746f 7220 6265 7477   propagator betw
+00001e40: 6565 6e20 6561 6368 0a20 2a20 2020 2020  een each. *     
+00001e50: 2065 6163 6820 736f 7572 6365 2061 6d70   each source amp
+00001e60: 6c69 7475 6465 2074 696d 6520 7361 6d70  litude time samp
+00001e70: 6c65 2e0a 202a 206e 756d 5f73 686f 7473  le.. * num_shots
+00001e80: 0a20 2a20 6e75 6d5f 736f 7572 6365 735f  . * num_sources_
+00001e90: 7065 725f 7368 6f74 0a20 2a20 6e75 6d5f  per_shot. * num_
+00001ea0: 7265 6365 6976 6572 735f 7065 725f 7368  receivers_per_sh
+00001eb0: 6f74 0a20 2a20 6474 3a20 5468 6520 7469  ot. * dt: The ti
+00001ec0: 6d65 2069 6e74 6572 7661 6c20 6265 7477  me interval betw
+00001ed0: 6565 6e20 7072 6f70 6167 6174 6f72 2074  een propagator t
+00001ee0: 696d 6520 7374 6570 7320 284e 4f54 2074  ime steps (NOT t
+00001ef0: 6865 2074 696d 6520 696e 7465 7276 616c  he time interval
+00001f00: 0a20 2a20 2020 2020 2062 6574 7765 656e  . *      between
+00001f10: 2073 6f75 7263 6520 616d 706c 6974 7564   source amplitud
+00001f20: 6520 7361 6d70 6c65 7320 2d20 7468 6174  e samples - that
+00001f30: 2077 6f75 6c64 2062 6520 6474 202a 2073   would be dt * s
+00001f40: 7465 705f 7261 7469 6f29 2e0a 202a 2f0a  tep_ratio).. */.
+00001f50: 766f 6964 2062 6163 6b77 6172 6428 4445  void backward(DE
+00001f60: 4550 5741 5645 5f54 5950 4520 2a20 636f  EPWAVE_TYPE * co
+00001f70: 6e73 7420 7761 7665 6669 656c 642c 0a20  nst wavefield,. 
+00001f80: 2020 2020 2020 2020 2020 2020 2044 4545               DEE
+00001f90: 5057 4156 455f 5459 5045 202a 2063 6f6e  PWAVE_TYPE * con
+00001fa0: 7374 2061 7578 5f77 6176 6566 6965 6c64  st aux_wavefield
+00001fb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001fc0: 4445 4550 5741 5645 5f54 5950 4520 2a20  DEEPWAVE_TYPE * 
+00001fd0: 636f 6e73 7420 6d6f 6465 6c5f 6772 6164  const model_grad
+00001fe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ff0: 4445 4550 5741 5645 5f54 5950 4520 2a20  DEEPWAVE_TYPE * 
+00002000: 636f 6e73 7420 736f 7572 6365 5f67 7261  const source_gra
+00002010: 645f 616d 706c 6974 7564 6573 2c0a 2020  d_amplitudes,.  
+00002020: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00002030: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+00002040: 2a20 636f 6e73 7420 6164 6a6f 696e 745f  * const adjoint_
+00002050: 7761 7665 6669 656c 642c 0a20 2020 2020  wavefield,.     
+00002060: 2020 2020 2020 2020 2063 6f6e 7374 2044           const D
+00002070: 4545 5057 4156 455f 5459 5045 202a 2063  EEPWAVE_TYPE * c
+00002080: 6f6e 7374 2073 6361 6c69 6e67 2c0a 2020  onst scaling,.  
+00002090: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+000020a0: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+000020b0: 2a20 636f 6e73 7420 7369 676d 612c 0a20  * const sigma,. 
+000020c0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000020d0: 7374 2044 4545 5057 4156 455f 5459 5045  st DEEPWAVE_TYPE
+000020e0: 202a 2063 6f6e 7374 206d 6f64 656c 2c0a   * const model,.
+000020f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002100: 6e73 7420 4445 4550 5741 5645 5f54 5950  nst DEEPWAVE_TYP
+00002110: 4520 2a20 636f 6e73 7420 6664 312c 0a20  E * const fd1,. 
+00002120: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00002130: 7374 2044 4545 5057 4156 455f 5459 5045  st DEEPWAVE_TYPE
+00002140: 202a 2063 6f6e 7374 2066 6432 2c0a 2020   * const fd2,.  
+00002150: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00002160: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+00002170: 2a20 636f 6e73 7420 7265 6365 6976 6572  * const receiver
+00002180: 5f67 7261 645f 616d 706c 6974 7564 6573  _grad_amplitudes
+00002190: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000021a0: 636f 6e73 7420 7074 7264 6966 665f 7420  const ptrdiff_t 
+000021b0: 2a20 636f 6e73 7420 736f 7572 6365 5f6c  * const source_l
+000021c0: 6f63 6174 696f 6e73 2c0a 2020 2020 2020  ocations,.      
+000021d0: 2020 2020 2020 2020 636f 6e73 7420 7074          const pt
+000021e0: 7264 6966 665f 7420 2a20 636f 6e73 7420  rdiff_t * const 
+000021f0: 7265 6365 6976 6572 5f6c 6f63 6174 696f  receiver_locatio
+00002200: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00002210: 2020 636f 6e73 7420 7074 7264 6966 665f    const ptrdiff_
+00002220: 7420 2a20 636f 6e73 7420 7368 6170 652c  t * const shape,
+00002230: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
+00002240: 6f6e 7374 2070 7472 6469 6666 5f74 202a  onst ptrdiff_t *
+00002250: 2063 6f6e 7374 2070 6d6c 5f77 6964 7468   const pml_width
+00002260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002270: 636f 6e73 7420 7074 7264 6966 665f 7420  const ptrdiff_t 
+00002280: 6e75 6d5f 7374 6570 732c 2063 6f6e 7374  num_steps, const
+00002290: 2070 7472 6469 6666 5f74 2073 7465 705f   ptrdiff_t step_
+000022a0: 7261 7469 6f2c 0a20 2020 2020 2020 2020  ratio,.         
+000022b0: 2020 2020 2063 6f6e 7374 2070 7472 6469       const ptrdi
+000022c0: 6666 5f74 206e 756d 5f73 686f 7473 2c20  ff_t num_shots, 
+000022d0: 636f 6e73 7420 7074 7264 6966 665f 7420  const ptrdiff_t 
+000022e0: 6e75 6d5f 736f 7572 6365 735f 7065 725f  num_sources_per_
+000022f0: 7368 6f74 2c0a 2020 2020 2020 2020 2020  shot,.          
+00002300: 2020 2020 636f 6e73 7420 7074 7264 6966      const ptrdif
+00002310: 665f 7420 6e75 6d5f 7265 6365 6976 6572  f_t num_receiver
+00002320: 735f 7065 725f 7368 6f74 2c20 636f 6e73  s_per_shot, cons
+00002330: 7420 4445 4550 5741 5645 5f54 5950 4520  t DEEPWAVE_TYPE 
+00002340: 6474 293b 0a0a 4445 4550 5741 5645 5f54  dt);..DEEPWAVE_T
+00002350: 5950 4520 2a73 6574 5f73 7465 705f 706f  YPE *set_step_po
+00002360: 696e 7465 7228 636f 6e73 7420 4445 4550  inter(const DEEP
+00002370: 5741 5645 5f54 5950 4520 2a20 636f 6e73  WAVE_TYPE * cons
+00002380: 7420 6f72 6967 696e 2c0a 2020 2020 2020  t origin,.      
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2063 6f6e 7374 2070 7472 6469 6666 5f74   const ptrdiff_t
+000023b0: 2073 7465 702c 2063 6f6e 7374 2070 7472   step, const ptr
+000023c0: 6469 6666 5f74 206e 756d 5f73 686f 7473  diff_t num_shots
+000023d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000023e0: 2020 2020 2020 2020 2063 6f6e 7374 2070           const p
+000023f0: 7472 6469 6666 5f74 206e 756d 656c 5f70  trdiff_t numel_p
+00002400: 6572 5f73 686f 7429 3b0a 0a2f 2a20 4469  er_shot);../* Di
+00002410: 6d65 6e73 696f 6e2d 7370 6563 6966 6963  mension-specific
+00002420: 2064 6566 696e 6974 696f 6e73 0a20 2a0a   definitions. *.
+00002430: 202a 205a 5041 442f 5950 4144 2f58 5041   * ZPAD/YPAD/XPA
+00002440: 443a 204e 756d 6265 7220 6f66 2063 656c  D: Number of cel
+00002450: 6c73 206f 6620 7061 6464 696e 6720 6174  ls of padding at
+00002460: 2074 6865 2062 6567 696e 6e69 6e67 2061   the beginning a
+00002470: 6e64 2065 6e64 206f 660a 202a 2020 2020  nd end of. *    
+00002480: 2020 7a2c 2079 2c20 616e 6420 7820 6469    z, y, and x di
+00002490: 6d65 6e73 696f 6e73 2074 6f20 6d61 6b65  mensions to make
+000024a0: 2066 696e 6974 6520 6469 6666 6572 656e   finite differen
+000024b0: 6365 2063 616c 6375 6c61 7469 6f6e 2063  ce calculation c
+000024c0: 6c65 616e 6572 0a20 2a20 4155 585f 5349  leaner. * AUX_SI
+000024d0: 5a45 3a20 4e75 6d62 6572 206f 6620 6175  ZE: Number of au
+000024e0: 7869 6c69 6172 7920 7761 7665 6669 656c  xiliary wavefiel
+000024f0: 6473 0a20 2a20 2a2f 0a23 6966 2044 4545  ds. * */.#if DEE
+00002500: 5057 4156 455f 4449 4d20 3d3d 2031 0a0a  PWAVE_DIM == 1..
+00002510: 2364 6566 696e 6520 5a50 4144 2032 0a23  #define ZPAD 2.#
+00002520: 6465 6669 6e65 2059 5041 4420 300a 2364  define YPAD 0.#d
+00002530: 6566 696e 6520 5850 4144 2030 0a0a 2364  efine XPAD 0..#d
+00002540: 6566 696e 6520 4155 585f 5349 5a45 2031  efine AUX_SIZE 1
+00002550: 0a0a 2365 6c69 6620 4445 4550 5741 5645  ..#elif DEEPWAVE
+00002560: 5f44 494d 203d 3d20 320a 0a23 6465 6669  _DIM == 2..#defi
+00002570: 6e65 205a 5041 4420 320a 2364 6566 696e  ne ZPAD 2.#defin
+00002580: 6520 5950 4144 2032 0a23 6465 6669 6e65  e YPAD 2.#define
+00002590: 2058 5041 4420 300a 0a23 6465 6669 6e65   XPAD 0..#define
+000025a0: 2041 5558 5f53 495a 4520 320a 0a23 656c   AUX_SIZE 2..#el
+000025b0: 6966 2044 4545 5057 4156 455f 4449 4d20  if DEEPWAVE_DIM 
+000025c0: 3d3d 2033 0a0a 2364 6566 696e 6520 5a50  == 3..#define ZP
+000025d0: 4144 2032 0a23 6465 6669 6e65 2059 5041  AD 2.#define YPA
+000025e0: 4420 320a 2364 6566 696e 6520 5850 4144  D 2.#define XPAD
+000025f0: 2032 0a0a 2364 6566 696e 6520 4155 585f   2..#define AUX_
+00002600: 5349 5a45 2034 0a0a 2365 6c73 650a 2365  SIZE 4..#else.#e
+00002610: 7272 6f72 2022 4d75 7374 2073 7065 6369  rror "Must speci
+00002620: 6679 2074 6865 2064 696d 656e 7369 6f6e  fy the dimension
+00002630: 2c20 652e 672e 202d 4420 4445 4550 5741  , e.g. -D DEEPWA
+00002640: 5645 5f44 494d 3d31 220a 2365 6e64 6966  VE_DIM=1".#endif
+00002650: 202f 2a20 4445 4550 5741 5645 5f44 494d   /* DEEPWAVE_DIM
+00002660: 202a 2f0a 0a23 656e 6469 6620 2f2a 2044   */..#endif /* D
+00002670: 4545 5057 4156 455f 5343 414c 4152 5f53  EEPWAVE_SCALAR_S
+00002680: 4341 4c41 525f 4820 2a2f 0a              CALAR_H */.
```

### Comparing `deepwave-0.0.8/deepwave/scalar/scalar.py` & `deepwave-0.0.9/deepwave/scalar/scalar.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,17 +215,17 @@
             num_shots,
             num_receivers_per_shot,
         ) = grad_receiver_amplitudes.shape
         num_sources_per_shot = source_model_locations.shape[1]
         shape = torch.ones(3).long()
         shape[:ndim] = torch.tensor(vp2dt2.shape)
 
-        aux.fill_(0)
-        model_gradient.fill_(0)
-        source_gradient.fill_(0)
+        aux.data.fill_(0)
+        model_gradient.data.fill_(0)
+        source_gradient.data.fill_(0)
         wavefield = torch.zeros(3, *aux[0].shape, device=aux.device)
 
         grad_receiver_amplitudes_resampled = scipy.signal.resample(
             grad_receiver_amplitudes.detach().cpu().numpy(),
             num_steps * step_ratio,
         )
         grad_receiver_amplitudes_resampled = (
```

### Comparing `deepwave-0.0.8/deepwave/scalar/scalar_born.py` & `deepwave-0.0.9/deepwave/scalar/scalar_born.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,17 +252,17 @@
             num_shots,
             num_receivers_per_shot,
         ) = grad_receiver_amplitudes.shape
         num_sources_per_shot = source_model_locations.shape[1]
         shape = torch.ones(3).long()
         shape[:ndim] = torch.tensor(vp2dt2.shape)
 
-        aux.fill_(0)
-        model_gradient.fill_(0)
-        source_gradient.fill_(0)
+        aux.data.fill_(0)
+        model_gradient.data.fill_(0)
+        source_gradient.data.fill_(0)
         wavefield = torch.zeros(3, *aux[0].shape, device=aux.device)
 
         grad_receiver_amplitudes_resampled = scipy.signal.resample(
             grad_receiver_amplitudes.detach().cpu().numpy(),
             num_steps * step_ratio,
         )
         grad_receiver_amplitudes_resampled = (
@@ -305,15 +305,15 @@
 
         if not ctx.needs_input_grad[0]:
             source_gradient = None
 
         if not ctx.needs_input_grad[scatter_index]:
             model_gradient = None
 
-        zero_edges(model_gradient, pml_width.long())
+        zero_edges(model_gradient.data, pml_width.long())
 
         return_list = [
             source_gradient,
             None,
             None,
             None,
             None,
```

### Comparing `deepwave-0.0.8/deepwave/scalar/scalar_cpu.cpp` & `deepwave-0.0.9/deepwave/scalar/scalar_cpu.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -4,96 +4,96 @@
 #include <string.h>
 
 #include "scalar.h"
 
 static inline ptrdiff_t location_index(
     const ptrdiff_t * const arr,
     const ptrdiff_t * const shape, const ptrdiff_t index);
-#if DIM == 1
-static inline TYPE laplacian_1d(const TYPE * const arr,
-                                const TYPE * const fd2,
+#if DEEPWAVE_DIM == 1
+static inline DEEPWAVE_TYPE laplacian_1d(const DEEPWAVE_TYPE * const arr,
+                                const DEEPWAVE_TYPE * const fd2,
                                 const ptrdiff_t si);
 #endif
-#if DIM == 2
-static inline TYPE laplacian_2d(const TYPE * const arr,
-                                const TYPE * const fd2,
+#if DEEPWAVE_DIM == 2
+static inline DEEPWAVE_TYPE laplacian_2d(const DEEPWAVE_TYPE * const arr,
+                                const DEEPWAVE_TYPE * const fd2,
                                 const ptrdiff_t si, const ptrdiff_t size_x);
 #endif
-#if DIM == 3
-static inline TYPE laplacian_3d(const TYPE * const arr,
-                                const TYPE * const fd2,
+#if DEEPWAVE_DIM == 3
+static inline DEEPWAVE_TYPE laplacian_3d(const DEEPWAVE_TYPE * const arr,
+                                const DEEPWAVE_TYPE * const fd2,
                                 const ptrdiff_t si, const ptrdiff_t size_x,
                                 const ptrdiff_t size_xy);
 #endif
-static inline TYPE z_deriv(const TYPE * const arr,
-                           const TYPE * const fd1,
+static inline DEEPWAVE_TYPE z_deriv(const DEEPWAVE_TYPE * const arr,
+                           const DEEPWAVE_TYPE * const fd1,
                            const ptrdiff_t si, const ptrdiff_t size_xy);
-static inline TYPE y_deriv(const TYPE * const arr,
-                           const TYPE * const fd1,
+static inline DEEPWAVE_TYPE y_deriv(const DEEPWAVE_TYPE * const arr,
+                           const DEEPWAVE_TYPE * const fd1,
                            const ptrdiff_t si, const ptrdiff_t size_x);
-static inline TYPE x_deriv(const TYPE * const arr,
-                           const TYPE * const fd1,
+static inline DEEPWAVE_TYPE x_deriv(const DEEPWAVE_TYPE * const arr,
+                           const DEEPWAVE_TYPE * const fd1,
                            const ptrdiff_t si);
 
-void setup(const TYPE * const /*fd1*/,
-           const TYPE * const /*fd2*/) {}
+void setup(const DEEPWAVE_TYPE * const /*fd1*/,
+           const DEEPWAVE_TYPE * const /*fd2*/) {}
 
-#if DIM == 1
-void propagate(TYPE * const wfn,        /* next wavefield */
-               TYPE * const auxn,       /* next auxiliary */
-               const TYPE * const wfc,  /* current wavefield */
-               const TYPE * const wfp,  /* previous wavefield */
-               const TYPE * const auxc, /* current auxiliary */
-               const TYPE * const sigma,
-               const TYPE * const model,
-               const TYPE * const fd1, /* 1st difference coeffs */
-               const TYPE * const fd2, /* 2nd difference coeffs */
+#if DEEPWAVE_DIM == 1
+void propagate(DEEPWAVE_TYPE * const wfn,        /* next wavefield */
+               DEEPWAVE_TYPE * const auxn,       /* next auxiliary */
+               const DEEPWAVE_TYPE * const wfc,  /* current wavefield */
+               const DEEPWAVE_TYPE * const wfp,  /* previous wavefield */
+               const DEEPWAVE_TYPE * const auxc, /* current auxiliary */
+               const DEEPWAVE_TYPE * const sigma,
+               const DEEPWAVE_TYPE * const model,
+               const DEEPWAVE_TYPE * const fd1, /* 1st difference coeffs */
+               const DEEPWAVE_TYPE * const fd2, /* 2nd difference coeffs */
                const ptrdiff_t * const shape,
                const ptrdiff_t * const pml_width,
-               const ptrdiff_t num_shots, const TYPE dt) {
+               const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t numel_shot = shape[0];
-  TYPE * const phizn = auxn;
-  const TYPE * const phizc = auxc;
-  const TYPE * const sigmaz = sigma;
+  DEEPWAVE_TYPE * const phizn = auxn;
+  const DEEPWAVE_TYPE * const phizc = auxc;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
 
 #pragma omp parallel for collapse(2)
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
       const ptrdiff_t i = z;
       const ptrdiff_t si = shot * numel_shot + i;
 
       /* Spatial finite differences */
-      const TYPE lap = laplacian_1d(wfc, fd2, si);
-      const TYPE wfc_z = z_deriv(wfc, fd1, si, 1);
-      const TYPE phizc_z = z_deriv(phizc, fd1, si, 1);
+      const DEEPWAVE_TYPE lap = laplacian_1d(wfc, fd2, si);
+      const DEEPWAVE_TYPE wfc_z = z_deriv(wfc, fd1, si, 1);
+      const DEEPWAVE_TYPE phizc_z = z_deriv(phizc, fd1, si, 1);
 
       /* Update wavefield */
       wfn[si] = 1 / (1 + dt * sigmaz[z] / 2) *
                 (model[i] * (lap + phizc_z) + dt * sigmaz[z] * wfp[si] / 2 +
                  (2 * wfc[si] - wfp[si]));
 
       /* Update phi */
       phizn[si] = phizc[si] - dt * sigmaz[z] * (wfc_z + phizc[si]);
     }
   }
 }
 
-void imaging_condition(TYPE * const model_grad,
-                       const TYPE * const current_wavefield,
-                       const TYPE * const saved_wavefield,
-                       const TYPE * const saved_wavefield_t,
-                       const TYPE * const saved_wavefield_tt,
-                       const TYPE * const sigma,
+void imaging_condition(DEEPWAVE_TYPE * const model_grad,
+                       const DEEPWAVE_TYPE * const current_wavefield,
+                       const DEEPWAVE_TYPE * const saved_wavefield,
+                       const DEEPWAVE_TYPE * const saved_wavefield_t,
+                       const DEEPWAVE_TYPE * const saved_wavefield_tt,
+                       const DEEPWAVE_TYPE * const sigma,
                        const ptrdiff_t * const shape,
                        const ptrdiff_t * const pml_width,
                        const ptrdiff_t num_shots) {
   if (model_grad == nullptr) return; /* Not doing model inversion */
 
   const ptrdiff_t numel_shot = shape[0];
-  const TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
 
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
       const ptrdiff_t i = z;
       const ptrdiff_t si = shot * numel_shot + i;
 
       model_grad[i] +=
@@ -107,50 +107,50 @@
     const ptrdiff_t * const arr,
     const ptrdiff_t * const shape, const ptrdiff_t index) {
   const ptrdiff_t z = arr[index];
 
   return z;
 }
 
-#elif DIM == 2
+#elif DEEPWAVE_DIM == 2
 
-void propagate(TYPE * const wfn,        /* next wavefield */
-               TYPE * const auxn,       /* next auxiliary */
-               const TYPE * const wfc,  /* current wavefield */
-               const TYPE * const wfp,  /* previous wavefield */
-               const TYPE * const auxc, /* current auxiliary */
-               const TYPE * const sigma,
-               const TYPE * const model,
-               const TYPE * const fd1, /* 1st difference coeffs */
-               const TYPE * const fd2, /* 2nd difference coeffs */
+void propagate(DEEPWAVE_TYPE * const wfn,        /* next wavefield */
+               DEEPWAVE_TYPE * const auxn,       /* next auxiliary */
+               const DEEPWAVE_TYPE * const wfc,  /* current wavefield */
+               const DEEPWAVE_TYPE * const wfp,  /* previous wavefield */
+               const DEEPWAVE_TYPE * const auxc, /* current auxiliary */
+               const DEEPWAVE_TYPE * const sigma,
+               const DEEPWAVE_TYPE * const model,
+               const DEEPWAVE_TYPE * const fd1, /* 1st difference coeffs */
+               const DEEPWAVE_TYPE * const fd2, /* 2nd difference coeffs */
                const ptrdiff_t * const shape,
                const ptrdiff_t * const pml_width,
-               const ptrdiff_t num_shots, const TYPE dt) {
+               const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t numel_shot = shape[0] * shape[1];
   const ptrdiff_t size_xy = shape[1];
-  TYPE * const phizn = auxn;
-  TYPE * const phiyn = auxn + num_shots * numel_shot;
-  const TYPE * const phizc = auxc;
-  const TYPE * const phiyc = auxc + num_shots * numel_shot;
-  const TYPE * const sigmaz = sigma;
-  const TYPE * const sigmay = sigma + shape[0];
+  DEEPWAVE_TYPE * const phizn = auxn;
+  DEEPWAVE_TYPE * const phiyn = auxn + num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const phizc = auxc;
+  const DEEPWAVE_TYPE * const phiyc = auxc + num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
 
 #pragma omp parallel for collapse(2)
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
       for (ptrdiff_t y = YPAD; y < shape[1] - YPAD; y++) {
         const ptrdiff_t i = z * size_xy + y;
         const ptrdiff_t si = shot * numel_shot + i;
 
         /* Spatial finite differences */
-        const TYPE lap = laplacian_2d(wfc, fd2, si, size_xy);
-        const TYPE wfc_z = z_deriv(wfc, fd1, si, size_xy);
-        const TYPE wfc_y = y_deriv(wfc, fd1, si, 1);
-        const TYPE phizc_z = z_deriv(phizc, fd1, si, size_xy);
-        const TYPE phiyc_y = y_deriv(phiyc, fd1, si, 1);
+        const DEEPWAVE_TYPE lap = laplacian_2d(wfc, fd2, si, size_xy);
+        const DEEPWAVE_TYPE wfc_z = z_deriv(wfc, fd1, si, size_xy);
+        const DEEPWAVE_TYPE wfc_y = y_deriv(wfc, fd1, si, 1);
+        const DEEPWAVE_TYPE phizc_z = z_deriv(phizc, fd1, si, size_xy);
+        const DEEPWAVE_TYPE phiyc_y = y_deriv(phiyc, fd1, si, 1);
 
         /* Update wavefield */
         wfn[si] = 1 / (1 + dt * (sigmaz[z] + sigmay[y]) / 2) *
                   (model[i] * (lap + phizc_z + phiyc_y) +
                    dt * (sigmaz[z] + sigmay[y]) * wfp[si] / 2 +
                    (2 * wfc[si] - wfp[si]) -
                    dt * dt * sigmaz[z] * sigmay[y] * wfc[si]);
@@ -161,29 +161,29 @@
         phiyn[si] = phiyc[si] - dt * (sigmay[y] * phiyc[si] +
                                       (sigmay[y] - sigmaz[z]) * wfc_y);
       }
     }
   }
 }
 
-void imaging_condition(TYPE * const model_grad,
-                       const TYPE * const current_wavefield,
-                       const TYPE * const saved_wavefield,
-                       const TYPE * const saved_wavefield_t,
-                       const TYPE * const saved_wavefield_tt,
-                       const TYPE * const sigma,
+void imaging_condition(DEEPWAVE_TYPE * const model_grad,
+                       const DEEPWAVE_TYPE * const current_wavefield,
+                       const DEEPWAVE_TYPE * const saved_wavefield,
+                       const DEEPWAVE_TYPE * const saved_wavefield_t,
+                       const DEEPWAVE_TYPE * const saved_wavefield_tt,
+                       const DEEPWAVE_TYPE * const sigma,
                        const ptrdiff_t * const shape,
                        const ptrdiff_t * const pml_width,
                        const ptrdiff_t num_shots) {
   if (model_grad == nullptr) return; /* Not doing model inversion */
 
   const ptrdiff_t numel_shot = shape[0] * shape[1];
   const ptrdiff_t size_xy = shape[1];
-  const TYPE * const sigmaz = sigma;
-  const TYPE * const sigmay = sigma + shape[0];
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
 
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
       for (ptrdiff_t y = YPAD; y < shape[1] - YPAD; y++) {
         const ptrdiff_t i = z * size_xy + y;
         const ptrdiff_t si = shot * numel_shot + i;
 
@@ -201,62 +201,62 @@
     const ptrdiff_t * const shape, const ptrdiff_t index) {
   const ptrdiff_t z = arr[index * 2];
   const ptrdiff_t y = arr[index * 2 + 1];
 
   return z * shape[1] + y;
 }
 
-#elif DIM == 3
+#elif DEEPWAVE_DIM == 3
 
-void propagate(TYPE * const wfn,        /* next wavefield */
-               TYPE * const auxn,       /* next auxiliary */
-               const TYPE * const wfc,  /* current wavefield */
-               const TYPE * const wfp,  /* previous wavefield */
-               const TYPE * const auxc, /* current auxiliary */
-               const TYPE * const sigma,
-               const TYPE * const model,
-               const TYPE * const fd1, /* 1st difference coeffs */
-               const TYPE * const fd2, /* 2nd difference coeffs */
+void propagate(DEEPWAVE_TYPE * const wfn,        /* next wavefield */
+               DEEPWAVE_TYPE * const auxn,       /* next auxiliary */
+               const DEEPWAVE_TYPE * const wfc,  /* current wavefield */
+               const DEEPWAVE_TYPE * const wfp,  /* previous wavefield */
+               const DEEPWAVE_TYPE * const auxc, /* current auxiliary */
+               const DEEPWAVE_TYPE * const sigma,
+               const DEEPWAVE_TYPE * const model,
+               const DEEPWAVE_TYPE * const fd1, /* 1st difference coeffs */
+               const DEEPWAVE_TYPE * const fd2, /* 2nd difference coeffs */
                const ptrdiff_t * const shape,
                const ptrdiff_t * const pml_width,
-               const ptrdiff_t num_shots, const TYPE dt) {
+               const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t numel_shot = shape[0] * shape[1] * shape[2];
   const ptrdiff_t size_x = shape[2];
   const ptrdiff_t size_xy = shape[1] * shape[2];
-  TYPE * const phizn = auxn;
-  TYPE * const phiyn = auxn + num_shots * numel_shot;
-  TYPE * const phixn = auxn + 2 * num_shots * numel_shot;
-  TYPE * const psin = auxn + 3 * num_shots * numel_shot;
-  const TYPE * const phizc = auxc;
-  const TYPE * const phiyc = auxc + num_shots * numel_shot;
-  const TYPE * const phixc = auxc + 2 * num_shots * numel_shot;
-  const TYPE * const psic = auxc + 3 * num_shots * numel_shot;
-  const TYPE * const sigmaz = sigma;
-  const TYPE * const sigmay = sigma + shape[0];
-  const TYPE * const sigmax = sigma + shape[0] + shape[1];
+  DEEPWAVE_TYPE * const phizn = auxn;
+  DEEPWAVE_TYPE * const phiyn = auxn + num_shots * numel_shot;
+  DEEPWAVE_TYPE * const phixn = auxn + 2 * num_shots * numel_shot;
+  DEEPWAVE_TYPE * const psin = auxn + 3 * num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const phizc = auxc;
+  const DEEPWAVE_TYPE * const phiyc = auxc + num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const phixc = auxc + 2 * num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const psic = auxc + 3 * num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
+  const DEEPWAVE_TYPE * const sigmax = sigma + shape[0] + shape[1];
 
 #pragma omp parallel for collapse(2)
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
       for (ptrdiff_t y = YPAD; y < shape[1] - YPAD; y++) {
         for (ptrdiff_t x = XPAD; x < shape[2] - XPAD; x++) {
           const ptrdiff_t i = z * size_xy + y * size_x + x;
           const ptrdiff_t si = shot * numel_shot + i;
 
           /* Spatial finite differences */
-          const TYPE lap = laplacian_3d(wfc, fd2, si, size_x, size_xy);
-          const TYPE wfc_z = z_deriv(wfc, fd1, si, size_xy);
-          const TYPE wfc_y = y_deriv(wfc, fd1, si, size_x);
-          const TYPE wfc_x = x_deriv(wfc, fd1, si);
-          const TYPE phizc_z = z_deriv(phizc, fd1, si, size_xy);
-          const TYPE phiyc_y = y_deriv(phiyc, fd1, si, size_x);
-          const TYPE phixc_x = x_deriv(phixc, fd1, si);
-          const TYPE psic_z = z_deriv(psic, fd1, si, size_xy);
-          const TYPE psic_y = y_deriv(psic, fd1, si, size_x);
-          const TYPE psic_x = x_deriv(psic, fd1, si);
+          const DEEPWAVE_TYPE lap = laplacian_3d(wfc, fd2, si, size_x, size_xy);
+          const DEEPWAVE_TYPE wfc_z = z_deriv(wfc, fd1, si, size_xy);
+          const DEEPWAVE_TYPE wfc_y = y_deriv(wfc, fd1, si, size_x);
+          const DEEPWAVE_TYPE wfc_x = x_deriv(wfc, fd1, si);
+          const DEEPWAVE_TYPE phizc_z = z_deriv(phizc, fd1, si, size_xy);
+          const DEEPWAVE_TYPE phiyc_y = y_deriv(phiyc, fd1, si, size_x);
+          const DEEPWAVE_TYPE phixc_x = x_deriv(phixc, fd1, si);
+          const DEEPWAVE_TYPE psic_z = z_deriv(psic, fd1, si, size_xy);
+          const DEEPWAVE_TYPE psic_y = y_deriv(psic, fd1, si, size_x);
+          const DEEPWAVE_TYPE psic_x = x_deriv(psic, fd1, si);
 
           /* Update wavefield */
           wfn[si] = 1 / (1 + dt * (sigmaz[z] + sigmay[y] + sigmax[x]) / 2) *
                     (model[i] * lap +
                      dt * dt *
                          (phizc_z + phiyc_y + phixc_x -
                           sigmaz[z] * sigmay[y] * sigmax[x] * psic[si]) +
@@ -281,31 +281,31 @@
           psin[si] = psic[si] + dt * wfc[si];
         }
       }
     }
   }
 }
 
-void imaging_condition(TYPE * const model_grad,
-                       const TYPE * const current_wavefield,
-                       const TYPE * const saved_wavefield,
-                       const TYPE * const saved_wavefield_t,
-                       const TYPE * const saved_wavefield_tt,
-                       const TYPE * const sigma,
+void imaging_condition(DEEPWAVE_TYPE * const model_grad,
+                       const DEEPWAVE_TYPE * const current_wavefield,
+                       const DEEPWAVE_TYPE * const saved_wavefield,
+                       const DEEPWAVE_TYPE * const saved_wavefield_t,
+                       const DEEPWAVE_TYPE * const saved_wavefield_tt,
+                       const DEEPWAVE_TYPE * const sigma,
                        const ptrdiff_t * const shape,
                        const ptrdiff_t * const pml_width,
                        const ptrdiff_t num_shots) {
   if (model_grad == nullptr) return; /* Not doing model inversion */
 
   const ptrdiff_t numel_shot = shape[0] * shape[1] * shape[2];
   const ptrdiff_t size_x = shape[2];
   const ptrdiff_t size_xy = shape[1] * shape[2];
-  const TYPE * const sigmaz = sigma;
-  const TYPE * const sigmay = sigma + shape[0];
-  const TYPE * const sigmax = sigma + shape[0] + shape[1];
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
+  const DEEPWAVE_TYPE * const sigmax = sigma + shape[0] + shape[1];
 
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
       for (ptrdiff_t y = YPAD; y < shape[1] - YPAD; y++) {
         for (ptrdiff_t x = XPAD; x < shape[2] - XPAD; x++) {
           const ptrdiff_t i = z * size_xy + y * size_x + x;
           const ptrdiff_t si = shot * numel_shot + i;
@@ -333,63 +333,63 @@
   const ptrdiff_t y = arr[index * 3 + 1];
   const ptrdiff_t x = arr[index * 3 + 2];
 
   return z * shape[1] * shape[2] + y * shape[2] + x;
 }
 
 #else
-#error "Must specify the dimension, e.g. -D DIM=1"
-#endif /* DIM */
+#error "Must specify the dimension, e.g. -D DEEPWAVE_DIM=1"
+#endif /* DEEPWAVE_DIM */
 
-void add_sources(TYPE * const next_wavefield,
-                 const TYPE * const model,
-                 const TYPE * const source_amplitudes,
+void add_sources(DEEPWAVE_TYPE * const next_wavefield,
+                 const DEEPWAVE_TYPE * const model,
+                 const DEEPWAVE_TYPE * const source_amplitudes,
                  const ptrdiff_t * const source_locations,
                  const ptrdiff_t * const shape,
                  const ptrdiff_t num_shots,
                  const ptrdiff_t num_sources_per_shot) {
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t source = 0; source < num_sources_per_shot; source++) {
       const ptrdiff_t s = shot * num_sources_per_shot + source;
       const ptrdiff_t i = location_index(source_locations, shape, s);
       const ptrdiff_t si = shot * shape[0] * shape[1] * shape[2] + i;
       next_wavefield[si] += source_amplitudes[s] * model[i];
     }
   }
 }
 
-void add_scattering(TYPE * const next_scattered_wavefield,
-                    const TYPE * const next_wavefield,
-                    const TYPE * const current_wavefield,
-                    const TYPE * const previous_wavefield,
-                    const TYPE * const scatter,
+void add_scattering(DEEPWAVE_TYPE * const next_scattered_wavefield,
+                    const DEEPWAVE_TYPE * const next_wavefield,
+                    const DEEPWAVE_TYPE * const current_wavefield,
+                    const DEEPWAVE_TYPE * const previous_wavefield,
+                    const DEEPWAVE_TYPE * const scatter,
                     const ptrdiff_t * const shape,
                     const ptrdiff_t num_shots) {
   const ptrdiff_t numel_shot = shape[0] * shape[1] * shape[2];
   const ptrdiff_t size_x = shape[2];
   const ptrdiff_t size_xy = shape[1] * shape[2];
 
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
     for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
       for (ptrdiff_t y = YPAD; y < shape[1] - YPAD; y++) {
         for (ptrdiff_t x = XPAD; x < shape[2] - XPAD; x++) {
           const ptrdiff_t i = z * size_xy + y * size_x + x;
           const ptrdiff_t si = shot * numel_shot + i;
-          const TYPE current_wavefield_tt =
+          const DEEPWAVE_TYPE current_wavefield_tt =
               (next_wavefield[si] - 2 * current_wavefield[si] +
                previous_wavefield[si]); /* no dt^2 because of cancellation */
           next_scattered_wavefield[si] += current_wavefield_tt * scatter[i];
         }
       }
     }
   }
 }
 
-void record_receivers(TYPE * const receiver_amplitudes,
-                      const TYPE * const current_wavefield,
+void record_receivers(DEEPWAVE_TYPE * const receiver_amplitudes,
+                      const DEEPWAVE_TYPE * const current_wavefield,
                       const ptrdiff_t * const receiver_locations,
                       const ptrdiff_t * const shape,
                       const ptrdiff_t num_shots,
                       const ptrdiff_t num_receivers_per_shot) {
   if (receiver_amplitudes == nullptr) return; /* no source inversion */
 
   for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
@@ -399,30 +399,30 @@
       const ptrdiff_t si = shot * shape[0] * shape[1] * shape[2] +
                            location_index(receiver_locations, shape, r);
       receiver_amplitudes[r] = current_wavefield[si];
     }
   }
 }
 
-void save_wavefields(TYPE * const current_saved_wavefield,
-                     TYPE * const current_saved_wavefield_t,
-                     TYPE * const current_saved_wavefield_tt,
-                     const TYPE * const next_wavefield,
-                     const TYPE * const current_wavefield,
-                     const TYPE * const previous_wavefield,
+void save_wavefields(DEEPWAVE_TYPE * const current_saved_wavefield,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_t,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+                     const DEEPWAVE_TYPE * const next_wavefield,
+                     const DEEPWAVE_TYPE * const current_wavefield,
+                     const DEEPWAVE_TYPE * const previous_wavefield,
                      const ptrdiff_t * const shape,
-                     const ptrdiff_t num_shots, const TYPE dt,
+                     const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt,
                      const enum wavefield_save_strategy save_strategy) {
   if (save_strategy == STRATEGY_COPY) {
     const ptrdiff_t numel_shot = shape[0] * shape[1] * shape[2];
     const ptrdiff_t size_x = shape[2];
     const ptrdiff_t size_xy = shape[1] * shape[2];
     memcpy(current_saved_wavefield, current_wavefield,
            static_cast<size_t>(num_shots * shape[0] * shape[1] * shape[2])
-           * sizeof(TYPE));
+           * sizeof(DEEPWAVE_TYPE));
 
     for (ptrdiff_t shot = 0; shot < num_shots; shot++) {
       for (ptrdiff_t z = ZPAD; z < shape[0] - ZPAD; z++) {
         for (ptrdiff_t y = YPAD; y < shape[1] - YPAD; y++) {
           for (ptrdiff_t x = XPAD; x < shape[2] - XPAD; x++) {
             const ptrdiff_t i = z * size_xy + y * size_x + x;
             const ptrdiff_t si = shot * numel_shot + i;
@@ -435,74 +435,74 @@
           }
         }
       }
     }
   }
 }
 
-void model_grad_scaling(TYPE * const model_grad,
-                        const TYPE * const scaling,
+void model_grad_scaling(DEEPWAVE_TYPE * const model_grad,
+                        const DEEPWAVE_TYPE * const scaling,
                         const ptrdiff_t * const shape,
                         const ptrdiff_t * const pml_width) {
   if (model_grad == nullptr) return; /* Not doing model inversion */
 
   const ptrdiff_t numel_shot = shape[0] * shape[1] * shape[2];
 
   for (ptrdiff_t i = 0; i < numel_shot; i++) {
     model_grad[i] *= scaling[i];
   }
 }
 
-#if DIM == 1
-static inline TYPE laplacian_1d(const TYPE * const arr,
-                                const TYPE * const fd2,
+#if DEEPWAVE_DIM == 1
+static inline DEEPWAVE_TYPE laplacian_1d(const DEEPWAVE_TYPE * const arr,
+                                const DEEPWAVE_TYPE * const fd2,
                                 const ptrdiff_t si) {
   return fd2[0] * arr[si] + fd2[1] * (arr[si + 1] + arr[si - 1]) +
          fd2[2] * (arr[si + 2] + arr[si - 2]);
 }
 #endif
 
-#if DIM == 2
-static inline TYPE laplacian_2d(const TYPE * const arr,
-                                const TYPE * const fd2,
+#if DEEPWAVE_DIM == 2
+static inline DEEPWAVE_TYPE laplacian_2d(const DEEPWAVE_TYPE * const arr,
+                                const DEEPWAVE_TYPE * const fd2,
                                 const ptrdiff_t si, const ptrdiff_t size_x) {
   return fd2[0] * arr[si] + fd2[1] * (arr[si + size_x] + arr[si - size_x]) +
          fd2[2] * (arr[si + 2 * size_x] + arr[si - 2 * size_x]) +
          +fd2[3] * (arr[si + 1] + arr[si - 1]) +
          fd2[4] * (arr[si + 2] + arr[si - 2]);
 }
 #endif
 
-#if DIM == 3
-static inline TYPE laplacian_3d(const TYPE * const arr,
-                                const TYPE * const fd2,
+#if DEEPWAVE_DIM == 3
+static inline DEEPWAVE_TYPE laplacian_3d(const DEEPWAVE_TYPE * const arr,
+                                const DEEPWAVE_TYPE * const fd2,
                                 const ptrdiff_t si, const ptrdiff_t size_x,
                                 const ptrdiff_t size_xy) {
   return fd2[0] * arr[si] + fd2[1] * (arr[si + size_xy] + arr[si - size_xy]) +
          fd2[2] * (arr[si + 2 * size_xy] + arr[si - 2 * size_xy]) +
          +fd2[3] * (arr[si + size_x] + arr[si - size_x]) +
          fd2[4] * (arr[si + 2 * size_x] + arr[si - 2 * size_x]) +
          fd2[5] * (arr[si + 1] + arr[si - 1]) +
          fd2[6] * (arr[si + 2] + arr[si - 2]);
 }
 #endif
 
-static inline TYPE z_deriv(const TYPE * const arr,
-                           const TYPE * const fd1,
+static inline DEEPWAVE_TYPE z_deriv(const DEEPWAVE_TYPE * const arr,
+                           const DEEPWAVE_TYPE * const fd1,
                            const ptrdiff_t si, const ptrdiff_t size_xy) {
   return fd1[0] * (arr[si + size_xy] - arr[si - size_xy]) +
          fd1[1] * (arr[si + 2 * size_xy] - arr[si - 2 * size_xy]);
 }
 
-static inline TYPE y_deriv(const TYPE * const arr,
-                           const TYPE * const fd1,
+static inline DEEPWAVE_TYPE y_deriv(const DEEPWAVE_TYPE * const arr,
+                           const DEEPWAVE_TYPE * const fd1,
                            const ptrdiff_t si, const ptrdiff_t size_x) {
   return fd1[0] * (arr[si + size_x] - arr[si - size_x]) +
          fd1[1] * (arr[si + 2 * size_x] - arr[si - 2 * size_x]);
 }
 
-static inline TYPE x_deriv(const TYPE * const arr,
-                           const TYPE * const fd1,
+static inline DEEPWAVE_TYPE x_deriv(const DEEPWAVE_TYPE * const arr,
+                           const DEEPWAVE_TYPE * const fd1,
                            const ptrdiff_t si) {
   return fd1[0] * (arr[si + 1] - arr[si - 1]) +
          fd1[1] * (arr[si + 2] - arr[si - 2]);
 }
```

### Comparing `deepwave-0.0.8/deepwave/scalar/scalar_gpu.cu` & `deepwave-0.0.9/deepwave/scalar/scalar_gpu.cu`

 * *Files 13% similar despite different names*

```diff
@@ -2,186 +2,186 @@
 
 #include <stddef.h>
 #include <stdio.h>
 #include <string.h>
 
 #include "scalar.h"
 
-static __constant__ TYPE fd1[2 * DIM];
-static __constant__ TYPE fd2[2 * DIM + 1];
+static __constant__ DEEPWAVE_TYPE fd1[2 * DEEPWAVE_DIM];
+static __constant__ DEEPWAVE_TYPE fd2[2 * DEEPWAVE_DIM + 1];
 
 #define gpuErrchk(ans) \
   { gpuAssert((ans), __FILE__, __LINE__); }
 static inline void gpuAssert(cudaError_t code, const char *file, int line,
                              bool abort = true) {
   if (code != cudaSuccess) {
     fprintf(stderr, "GPUassert: %s %s %d\n", cudaGetErrorString(code), file,
             line);
     if (abort) exit(code);
   }
 }
 
-static inline __device__ TYPE laplacian_1d(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE laplacian_1d(const DEEPWAVE_TYPE * const arr,
                                            const ptrdiff_t si);
-static inline __device__ TYPE laplacian_2d(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE laplacian_2d(const DEEPWAVE_TYPE * const arr,
                                            const ptrdiff_t si,
                                            const ptrdiff_t size_x);
-static inline __device__ TYPE laplacian_3d(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE laplacian_3d(const DEEPWAVE_TYPE * const arr,
                                            const ptrdiff_t si,
                                            const ptrdiff_t size_x,
                                            const ptrdiff_t size_xy);
 static inline __device__ ptrdiff_t location_index(
     const ptrdiff_t * const arr,
     const ptrdiff_t * const shape, const ptrdiff_t index);
-static inline __device__ TYPE z_deriv(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE z_deriv(const DEEPWAVE_TYPE * const arr,
                                       const ptrdiff_t si,
                                       const ptrdiff_t size_xy);
-static inline __device__ TYPE y_deriv(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE y_deriv(const DEEPWAVE_TYPE * const arr,
                                       const ptrdiff_t si,
                                       const ptrdiff_t size_x);
-static inline __device__ TYPE x_deriv(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE x_deriv(const DEEPWAVE_TYPE * const arr,
                                       const ptrdiff_t si);
 
-#if DIM == 1
+#if DEEPWAVE_DIM == 1
 __global__ void propagate_kernel(
-    TYPE * const wfn, TYPE * const phizn,
-    const TYPE * const wfc, const TYPE * const wfp,
-    const TYPE * const phizc, const TYPE * const sigmaz,
-    const TYPE * const model, const ptrdiff_t shape_z,
+    DEEPWAVE_TYPE * const wfn, DEEPWAVE_TYPE * const phizn,
+    const DEEPWAVE_TYPE * const wfc, const DEEPWAVE_TYPE * const wfp,
+    const DEEPWAVE_TYPE * const phizc, const DEEPWAVE_TYPE * const sigmaz,
+    const DEEPWAVE_TYPE * const model, const ptrdiff_t shape_z,
     const ptrdiff_t numel_shot, const ptrdiff_t num_shots,
-    const ptrdiff_t pmlz0, const ptrdiff_t pmlz1, const TYPE dt) {
+    const ptrdiff_t pmlz0, const ptrdiff_t pmlz1, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t shot = blockIdx.y * blockDim.y + threadIdx.y;
   const ptrdiff_t z = blockIdx.x * blockDim.x + threadIdx.x + ZPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD)) {
     const ptrdiff_t i = z;
     const ptrdiff_t si = shot * numel_shot + i;
 
-    const TYPE lap = laplacian_1d(wfc, si);
+    const DEEPWAVE_TYPE lap = laplacian_1d(wfc, si);
 
     if ((z >= pmlz0 + 2 * ZPAD) && (z < shape_z - pmlz1 - 2 * ZPAD)) {
       /* Update wavefield */
       wfn[si] = model[i] * lap + 2 * wfc[si] - wfp[si];
     } else {
       /* Inside PML region */
 
-      const TYPE wfc_z = z_deriv(wfc, si, 1);
-      const TYPE phizc_z = z_deriv(phizc, si, 1);
+      const DEEPWAVE_TYPE wfc_z = z_deriv(wfc, si, 1);
+      const DEEPWAVE_TYPE phizc_z = z_deriv(phizc, si, 1);
 
       /* Update wavefield */
       wfn[si] = 1 / (1 + dt * sigmaz[z] / 2) *
                 (model[i] * (lap + phizc_z) + dt * sigmaz[z] * wfp[si] / 2 +
                  (2 * wfc[si] - wfp[si]));
 
       /* Update phi */
       phizn[si] = phizc[si] - dt * sigmaz[z] * (wfc_z + phizc[si]);
     }
   }
 }
 
-void propagate(TYPE * const wfn,        /* next wavefield */
-               TYPE * const auxn,       /* next auxiliary */
-               const TYPE * const wfc,  /* current wavefield */
-               const TYPE * const wfp,  /* previous wavefield */
-               const TYPE * const auxc, /* current auxiliary */
-               const TYPE * const sigma,
-               const TYPE * const model,
-               const TYPE * const fd1_d, /* 1st diff coeffs */
-               const TYPE * const fd2_d, /* 2nd diff coeffs */
+void propagate(DEEPWAVE_TYPE * const wfn,        /* next wavefield */
+               DEEPWAVE_TYPE * const auxn,       /* next auxiliary */
+               const DEEPWAVE_TYPE * const wfc,  /* current wavefield */
+               const DEEPWAVE_TYPE * const wfp,  /* previous wavefield */
+               const DEEPWAVE_TYPE * const auxc, /* current auxiliary */
+               const DEEPWAVE_TYPE * const sigma,
+               const DEEPWAVE_TYPE * const model,
+               const DEEPWAVE_TYPE * const fd1_d, /* 1st diff coeffs */
+               const DEEPWAVE_TYPE * const fd2_d, /* 2nd diff coeffs */
                const ptrdiff_t * const shape,
                const ptrdiff_t * const pml_width,
-               const ptrdiff_t num_shots, const TYPE dt) {
+               const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t numel_shot = shape[0];
-  TYPE * const phizn = auxn;
-  const TYPE * const phizc = auxc;
-  const TYPE * const sigmaz = sigma;
+  DEEPWAVE_TYPE * const phizn = auxn;
+  const DEEPWAVE_TYPE * const phizc = auxc;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
 
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[0] - (2 * ZPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (num_shots + dimBlock.y - 1) / dimBlock.y;
   const int gridz = 1;
   const dim3 dimGrid(gridx, gridy, gridz);
   propagate_kernel<<<dimGrid, dimBlock>>>(
       wfn, phizn, wfc, wfp, phizc, sigmaz, model, shape[0], numel_shot,
       num_shots, pml_width[0], pml_width[1], dt);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ imaging_condition_kernel(
-    TYPE * const model_grad,
-    const TYPE * const current_wavefield,
-    const TYPE * const current_saved_wavefield_t,
-    const TYPE * const current_saved_wavefield_tt,
-    const TYPE * const sigmaz, const ptrdiff_t shape_z,
+    DEEPWAVE_TYPE * const model_grad,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const sigmaz, const ptrdiff_t shape_z,
     const ptrdiff_t num_shots) {
   const ptrdiff_t shot = blockIdx.y * blockDim.y + threadIdx.y;
   const ptrdiff_t z = blockIdx.x * blockDim.x + threadIdx.x + ZPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD)) {
     const ptrdiff_t i = z;
     const ptrdiff_t si = shot * shape_z + i;
 
     atomicAdd(model_grad + i, current_wavefield[si] *
                                   (current_saved_wavefield_tt[si] +
                                    sigmaz[z] * current_saved_wavefield_t[si]));
   }
 }
 
 void imaging_condition(
-    TYPE * const model_grad,
-    const TYPE * const current_wavefield,
-    const TYPE * const current_saved_wavefield,
-    const TYPE * const current_saved_wavefield_t,
-    const TYPE * const current_saved_wavefield_tt,
-    const TYPE * const sigma,
+    DEEPWAVE_TYPE * const model_grad,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const sigma,
     const ptrdiff_t * const shape,
     const ptrdiff_t * const pml_width, const ptrdiff_t num_shots) {
   if (model_grad == NULL) return; /* Not doing model inversion */
 
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[0] - (2 * ZPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (num_shots + dimBlock.y - 1) / dimBlock.y;
   const int gridz = 1;
 
   const dim3 dimGrid(gridx, gridy, gridz);
-  const TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
 
   imaging_condition_kernel<<<dimGrid, dimBlock>>>(
       model_grad, current_wavefield, current_saved_wavefield_t,
       current_saved_wavefield_tt, sigmaz, shape[0], num_shots);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ add_scattering_kernel(
-    TYPE * const next_scattered_wavefield,
-    const TYPE * const next_wavefield,
-    const TYPE * const current_wavefield,
-    const TYPE * const previous_wavefield,
-    const TYPE * const scatter,
+    DEEPWAVE_TYPE * const next_scattered_wavefield,
+    const DEEPWAVE_TYPE * const next_wavefield,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const previous_wavefield,
+    const DEEPWAVE_TYPE * const scatter,
     const ptrdiff_t shape_z,
     const ptrdiff_t num_shots) {
   const ptrdiff_t shot = blockIdx.y * blockDim.y + threadIdx.y;
   const ptrdiff_t z = blockIdx.x * blockDim.x + threadIdx.x + ZPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD)) {
     const ptrdiff_t i = z;
     const ptrdiff_t si = shot * shape_z + i;
 
-    const TYPE current_wavefield_tt =
+    const DEEPWAVE_TYPE current_wavefield_tt =
         (next_wavefield[si] - 2 * current_wavefield[si] +
          previous_wavefield[si]); /* no dt^2 because of cancellation */
     next_scattered_wavefield[si] += current_wavefield_tt * scatter[i];
   }
 }
 
 void add_scattering(
-                     TYPE * const next_scattered_wavefield,
-                     const TYPE * const next_wavefield,
-                     const TYPE * const current_wavefield,
-                     const TYPE * const previous_wavefield,
-                     const TYPE * const scatter,
+                     DEEPWAVE_TYPE * const next_scattered_wavefield,
+                     const DEEPWAVE_TYPE * const next_wavefield,
+                     const DEEPWAVE_TYPE * const current_wavefield,
+                     const DEEPWAVE_TYPE * const previous_wavefield,
+                     const DEEPWAVE_TYPE * const scatter,
                      const ptrdiff_t * const shape,
                      const ptrdiff_t num_shots) {
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[0] - (2 * ZPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (num_shots + dimBlock.y - 1) / dimBlock.y;
   const int gridz = 1;
 
@@ -189,20 +189,20 @@
   add_scattering_kernel<<<dimGrid, dimBlock>>>(
       next_scattered_wavefield, next_wavefield,
       current_wavefield, previous_wavefield, scatter, shape[0], num_shots);
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ save_wavefields_kernel(
-    TYPE * const current_saved_wavefield_t,
-    TYPE * const current_saved_wavefield_tt,
-    const TYPE * const next_wavefield,
-    const TYPE * const current_wavefield,
-    const TYPE * const previous_wavefield, const ptrdiff_t shape_z,
-    const ptrdiff_t num_shots, const TYPE dt) {
+    DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const next_wavefield,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const previous_wavefield, const ptrdiff_t shape_z,
+    const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t shot = blockIdx.y * blockDim.y + threadIdx.y;
   const ptrdiff_t z = blockIdx.x * blockDim.x + threadIdx.x + ZPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD)) {
     const ptrdiff_t i = z;
     const ptrdiff_t si = shot * shape_z + i;
     current_saved_wavefield_t[si] =
         (current_wavefield[si] - previous_wavefield[si]) / dt;
@@ -210,27 +210,27 @@
     current_saved_wavefield_tt[si] =
         (next_wavefield[si] - 2 * current_wavefield[si] +
          previous_wavefield[si]) /
         dt / dt;
   }
 }
 
-void save_wavefields(TYPE * const current_saved_wavefield,
-                     TYPE * const current_saved_wavefield_t,
-                     TYPE * const current_saved_wavefield_tt,
-                     const TYPE * const next_wavefield,
-                     const TYPE * const current_wavefield,
-                     const TYPE * const previous_wavefield,
+void save_wavefields(DEEPWAVE_TYPE * const current_saved_wavefield,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_t,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+                     const DEEPWAVE_TYPE * const next_wavefield,
+                     const DEEPWAVE_TYPE * const current_wavefield,
+                     const DEEPWAVE_TYPE * const previous_wavefield,
                      const ptrdiff_t * const shape,
-                     const ptrdiff_t num_shots, const TYPE dt,
+                     const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt,
                      const enum wavefield_save_strategy save_strategy) {
   if (save_strategy == STRATEGY_COPY) {
     gpuErrchk(
         cudaMemcpy(current_saved_wavefield, current_wavefield,
-                   num_shots * shape[0] * shape[1] * shape[2] * sizeof(TYPE),
+                   num_shots * shape[0] * shape[1] * shape[2] * sizeof(DEEPWAVE_TYPE),
                    cudaMemcpyDeviceToDevice));
 
     const dim3 dimBlock(32, 32, 1);
     const int gridx = (shape[0] - (2 * ZPAD) + dimBlock.x - 1) / dimBlock.x;
     const int gridy = (num_shots + dimBlock.y - 1) / dimBlock.y;
     const int gridz = 1;
 
@@ -246,52 +246,52 @@
 location_index(const ptrdiff_t * const arr, const ptrdiff_t shape_y,
                const ptrdiff_t shape_x, const ptrdiff_t index) {
   const ptrdiff_t z = arr[index];
 
   return z;
 }
 
-static inline __device__ TYPE laplacian_1d(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE laplacian_1d(const DEEPWAVE_TYPE * const arr,
                                            const ptrdiff_t si) {
   return fd2[0] * arr[si] + fd2[1] * (arr[si + 1] + arr[si - 1]) +
          fd2[2] * (arr[si + 2] + arr[si - 2]);
 }
 
-#elif DIM == 2
+#elif DEEPWAVE_DIM == 2
 
 __global__ void propagate_kernel(
-    TYPE * const wfn, TYPE * const phizn,
-    TYPE * const phiyn, const TYPE * const wfc,
-    const TYPE * const wfp, const TYPE * const phizc,
-    const TYPE * const sigmaz, const TYPE * const phiyc,
-    const TYPE * const sigmay, const TYPE * const model,
+    DEEPWAVE_TYPE * const wfn, DEEPWAVE_TYPE * const phizn,
+    DEEPWAVE_TYPE * const phiyn, const DEEPWAVE_TYPE * const wfc,
+    const DEEPWAVE_TYPE * const wfp, const DEEPWAVE_TYPE * const phizc,
+    const DEEPWAVE_TYPE * const sigmaz, const DEEPWAVE_TYPE * const phiyc,
+    const DEEPWAVE_TYPE * const sigmay, const DEEPWAVE_TYPE * const model,
     const ptrdiff_t shape_z, const ptrdiff_t shape_y,
     const ptrdiff_t numel_shot, const ptrdiff_t num_shots,
     const ptrdiff_t pmlz0, const ptrdiff_t pmlz1, const ptrdiff_t pmly0,
-    const ptrdiff_t pmly1, const TYPE dt) {
+    const ptrdiff_t pmly1, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t shot = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t z = blockIdx.y * blockDim.y + threadIdx.y + ZPAD;
   const ptrdiff_t y = blockIdx.x * blockDim.x + threadIdx.x + YPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD) && (y < shape_y - YPAD)) {
     const ptrdiff_t i = z * shape_y + y;
     const ptrdiff_t si = shot * numel_shot + i;
 
-    const TYPE lap = laplacian_2d(wfc, si, shape_y);
+    const DEEPWAVE_TYPE lap = laplacian_2d(wfc, si, shape_y);
 
     if ((z >= pmlz0 + 2 * ZPAD) && (z < shape_z - pmlz1 - 2 * ZPAD) &&
         (y >= pmly0 + 2 * YPAD) && (y < shape_y - pmly1 - 2 * YPAD)) {
       /* Update wavefield */
       wfn[si] = model[i] * lap + 2 * wfc[si] - wfp[si];
     } else {
       /* Inside PML region */
 
-      const TYPE wfc_z = z_deriv(wfc, si, shape_y);
-      const TYPE phizc_z = z_deriv(phizc, si, shape_y);
-      const TYPE wfc_y = y_deriv(wfc, si, 1);
-      const TYPE phiyc_y = y_deriv(phiyc, si, 1);
+      const DEEPWAVE_TYPE wfc_z = z_deriv(wfc, si, shape_y);
+      const DEEPWAVE_TYPE phizc_z = z_deriv(phizc, si, shape_y);
+      const DEEPWAVE_TYPE wfc_y = y_deriv(wfc, si, 1);
+      const DEEPWAVE_TYPE phiyc_y = y_deriv(phiyc, si, 1);
 
       /* Update wavefield */
       wfn[si] =
           1 / (1 + dt * (sigmaz[z] + sigmay[y]) / 2) *
           (model[i] * (lap + phizc_z + phiyc_y) +
            dt * (sigmaz[z] + sigmay[y]) * wfp[si] / 2 +
            (2 * wfc[si] - wfp[si]) - dt * dt * sigmaz[z] * sigmay[y] * wfc[si]);
@@ -301,34 +301,34 @@
                                     (sigmaz[z] - sigmay[y]) * wfc_z);
       phiyn[si] = phiyc[si] - dt * (sigmay[y] * phiyc[si] +
                                     (sigmay[y] - sigmaz[z]) * wfc_y);
     }
   }
 }
 
-void propagate(TYPE * const wfn,        /* next wavefield */
-               TYPE * const auxn,       /* next auxiliary */
-               const TYPE * const wfc,  /* current wavefield */
-               const TYPE * const wfp,  /* previous wavefield */
-               const TYPE * const auxc, /* current auxiliary */
-               const TYPE * const sigma,
-               const TYPE * const model,
-               const TYPE * const fd1_d, /* 1st diff coeffs */
-               const TYPE * const fd2_d, /* 2nd diff coeffs */
+void propagate(DEEPWAVE_TYPE * const wfn,        /* next wavefield */
+               DEEPWAVE_TYPE * const auxn,       /* next auxiliary */
+               const DEEPWAVE_TYPE * const wfc,  /* current wavefield */
+               const DEEPWAVE_TYPE * const wfp,  /* previous wavefield */
+               const DEEPWAVE_TYPE * const auxc, /* current auxiliary */
+               const DEEPWAVE_TYPE * const sigma,
+               const DEEPWAVE_TYPE * const model,
+               const DEEPWAVE_TYPE * const fd1_d, /* 1st diff coeffs */
+               const DEEPWAVE_TYPE * const fd2_d, /* 2nd diff coeffs */
                const ptrdiff_t * const shape,
                const ptrdiff_t * const pml_width,
-               const ptrdiff_t num_shots, const TYPE dt) {
+               const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t numel_shot = shape[0] * shape[1];
-  TYPE * const phizn = auxn;
-  const TYPE * const phizc = auxc;
-  const TYPE * const sigmaz = sigma;
-
-  TYPE * const phiyn = auxn + num_shots * numel_shot;
-  const TYPE * const phiyc = auxc + num_shots * numel_shot;
-  const TYPE * const sigmay = sigma + shape[0];
+  DEEPWAVE_TYPE * const phizn = auxn;
+  const DEEPWAVE_TYPE * const phizc = auxc;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+
+  DEEPWAVE_TYPE * const phiyn = auxn + num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const phiyc = auxc + num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
 
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[1] - (2 * YPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (shape[0] - (2 * ZPAD) + dimBlock.y - 1) / dimBlock.y;
   const int gridz = (num_shots + dimBlock.z - 1) / dimBlock.z;
   const dim3 dimGrid(gridx, gridy, gridz);
   propagate_kernel<<<dimGrid, dimBlock>>>(
@@ -336,21 +336,21 @@
       shape[0], shape[1], numel_shot, num_shots, pml_width[0], pml_width[1],
       pml_width[2], pml_width[3], dt);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ imaging_condition_kernel(
-    TYPE * const model_grad,
-    const TYPE * const current_wavefield,
-    const TYPE * const current_saved_wavefield,
-    const TYPE * const current_saved_wavefield_t,
-    const TYPE * const current_saved_wavefield_tt,
-    const TYPE * const sigmaz,
-    const TYPE * const sigmay, const ptrdiff_t shape_z,
+    DEEPWAVE_TYPE * const model_grad,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const sigmaz,
+    const DEEPWAVE_TYPE * const sigmay, const ptrdiff_t shape_z,
     const ptrdiff_t shape_y, const ptrdiff_t numel_shot,
     const ptrdiff_t num_shots) {
   const ptrdiff_t shot = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t z = blockIdx.y * blockDim.y + threadIdx.y + ZPAD;
   const ptrdiff_t y = blockIdx.x * blockDim.x + threadIdx.x + YPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD) && (y < shape_y - YPAD)) {
     const ptrdiff_t i = z * shape_y + y;
@@ -361,70 +361,70 @@
                   (current_saved_wavefield_tt[si] +
                    (sigmaz[z] + sigmay[y]) * current_saved_wavefield_t[si] +
                    sigmaz[z] * sigmay[y] * current_saved_wavefield[si]));
   }
 }
 
 void imaging_condition(
-    TYPE * const model_grad,
-    const TYPE * const current_wavefield,
-    const TYPE * const current_saved_wavefield,
-    const TYPE * const current_saved_wavefield_t,
-    const TYPE * const current_saved_wavefield_tt,
-    const TYPE * const sigma,
+    DEEPWAVE_TYPE * const model_grad,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const sigma,
     const ptrdiff_t * const shape,
     const ptrdiff_t * const pml_width, const ptrdiff_t num_shots) {
   if (model_grad == NULL) return; /* Not doing model inversion */
 
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[1] - (2 * YPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (shape[0] - (2 * ZPAD) + dimBlock.y - 1) / dimBlock.y;
   const int gridz = (num_shots + dimBlock.z - 1) / dimBlock.z;
 
   const dim3 dimGrid(gridx, gridy, gridz);
-  const TYPE * const sigmaz = sigma;
-  const TYPE * const sigmay = sigma + shape[0];
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
 
   imaging_condition_kernel<<<dimGrid, dimBlock>>>(
       model_grad, current_wavefield, current_saved_wavefield,
       current_saved_wavefield_t, current_saved_wavefield_tt, sigmaz, sigmay,
       shape[0], shape[1], shape[0] * shape[1], num_shots);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ add_scattering_kernel(
-    TYPE * const next_scattered_wavefield,
-    const TYPE * const next_wavefield,
-    const TYPE * const current_wavefield,
-    const TYPE * const previous_wavefield,
-    const TYPE * const scatter,
+    DEEPWAVE_TYPE * const next_scattered_wavefield,
+    const DEEPWAVE_TYPE * const next_wavefield,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const previous_wavefield,
+    const DEEPWAVE_TYPE * const scatter,
     const ptrdiff_t shape_z,
     const ptrdiff_t shape_y, const ptrdiff_t numel_shot,
     const ptrdiff_t num_shots) {
   const ptrdiff_t shot = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t z = blockIdx.y * blockDim.y + threadIdx.y + ZPAD;
   const ptrdiff_t y = blockIdx.x * blockDim.x + threadIdx.x + YPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD) && (y < shape_y - YPAD)) {
     const ptrdiff_t i = z * shape_y + y;
     const ptrdiff_t si = shot * numel_shot + i;
 
-    const TYPE current_wavefield_tt =
+    const DEEPWAVE_TYPE current_wavefield_tt =
         (next_wavefield[si] - 2 * current_wavefield[si] +
          previous_wavefield[si]); /* no dt^2 because of cancellation */
     next_scattered_wavefield[si] += current_wavefield_tt * scatter[i];
   }
 }
 
 void add_scattering(
-                     TYPE * const next_scattered_wavefield,
-                     const TYPE * const next_wavefield,
-                     const TYPE * const current_wavefield,
-                     const TYPE * const previous_wavefield,
-                     const TYPE * const scatter,
+                     DEEPWAVE_TYPE * const next_scattered_wavefield,
+                     const DEEPWAVE_TYPE * const next_wavefield,
+                     const DEEPWAVE_TYPE * const current_wavefield,
+                     const DEEPWAVE_TYPE * const previous_wavefield,
+                     const DEEPWAVE_TYPE * const scatter,
                      const ptrdiff_t * const shape,
                      const ptrdiff_t num_shots) {
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[1] - (2 * YPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (shape[0] - (2 * ZPAD) + dimBlock.y - 1) / dimBlock.y;
   const int gridz = (num_shots + dimBlock.z - 1) / dimBlock.z;
 
@@ -433,21 +433,21 @@
       next_scattered_wavefield, next_wavefield,
       current_wavefield, previous_wavefield, scatter, shape[0], shape[1],
       shape[0] * shape[1], num_shots);
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ save_wavefields_kernel(
-    TYPE * const current_saved_wavefield_t,
-    TYPE * const current_saved_wavefield_tt,
-    const TYPE * const next_wavefield,
-    const TYPE * const current_wavefield,
-    const TYPE * const previous_wavefield, const ptrdiff_t shape_z,
+    DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const next_wavefield,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const previous_wavefield, const ptrdiff_t shape_z,
     const ptrdiff_t shape_y, const ptrdiff_t numel_shot,
-    const ptrdiff_t num_shots, const TYPE dt) {
+    const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t shot = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t z = blockIdx.y * blockDim.y + threadIdx.y + ZPAD;
   const ptrdiff_t y = blockIdx.x * blockDim.x + threadIdx.x + YPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD) && (y < shape_y - YPAD)) {
     const ptrdiff_t i = z * shape_y + y;
     const ptrdiff_t si = shot * numel_shot + i;
 
@@ -457,27 +457,27 @@
     current_saved_wavefield_tt[si] =
         (next_wavefield[si] - 2 * current_wavefield[si] +
          previous_wavefield[si]) /
         dt / dt;
   }
 }
 
-void save_wavefields(TYPE * const current_saved_wavefield,
-                     TYPE * const current_saved_wavefield_t,
-                     TYPE * const current_saved_wavefield_tt,
-                     const TYPE * const next_wavefield,
-                     const TYPE * const current_wavefield,
-                     const TYPE * const previous_wavefield,
+void save_wavefields(DEEPWAVE_TYPE * const current_saved_wavefield,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_t,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+                     const DEEPWAVE_TYPE * const next_wavefield,
+                     const DEEPWAVE_TYPE * const current_wavefield,
+                     const DEEPWAVE_TYPE * const previous_wavefield,
                      const ptrdiff_t * const shape,
-                     const ptrdiff_t num_shots, const TYPE dt,
+                     const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt,
                      const enum wavefield_save_strategy save_strategy) {
   if (save_strategy == STRATEGY_COPY) {
     gpuErrchk(
         cudaMemcpy(current_saved_wavefield, current_wavefield,
-                   num_shots * shape[0] * shape[1] * shape[2] * sizeof(TYPE),
+                   num_shots * shape[0] * shape[1] * shape[2] * sizeof(DEEPWAVE_TYPE),
                    cudaMemcpyDeviceToDevice));
 
     const dim3 dimBlock(32, 32, 1);
     const int gridx = (shape[1] - (2 * YPAD) + dimBlock.x - 1) / dimBlock.x;
     const int gridy = (shape[0] - (2 * ZPAD) + dimBlock.y - 1) / dimBlock.y;
     const int gridz = (num_shots + dimBlock.z - 1) / dimBlock.z;
 
@@ -495,67 +495,67 @@
                const ptrdiff_t shape_x, const ptrdiff_t index) {
   const ptrdiff_t z = arr[index * 2];
   const ptrdiff_t y = arr[index * 2 + 1];
 
   return z * shape_y + y;
 }
 
-static inline __device__ TYPE laplacian_2d(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE laplacian_2d(const DEEPWAVE_TYPE * const arr,
                                            const ptrdiff_t si,
                                            const ptrdiff_t size_x) {
   return fd2[0] * arr[si] + fd2[1] * (arr[si + size_x] + arr[si - size_x]) +
          fd2[2] * (arr[si + 2 * size_x] + arr[si - 2 * size_x]) +
          +fd2[3] * (arr[si + 1] + arr[si - 1]) +
          fd2[4] * (arr[si + 2] + arr[si - 2]);
 }
 
-#elif DIM == 3
+#elif DEEPWAVE_DIM == 3
 __global__ void propagate_kernel(
-    TYPE * const wfn, TYPE * const phizn,
-    TYPE * const phiyn, TYPE * const phixn,
-    TYPE * const psin, const TYPE * const wfc,
-    const TYPE * const wfp, const TYPE * const phizc,
-    const TYPE * const sigmaz, const TYPE * const phiyc,
-    const TYPE * const sigmay, const TYPE * const phixc,
-    const TYPE * const sigmax, const TYPE * const psic,
-    const TYPE * const model, const ptrdiff_t shape_z,
+    DEEPWAVE_TYPE * const wfn, DEEPWAVE_TYPE * const phizn,
+    DEEPWAVE_TYPE * const phiyn, DEEPWAVE_TYPE * const phixn,
+    DEEPWAVE_TYPE * const psin, const DEEPWAVE_TYPE * const wfc,
+    const DEEPWAVE_TYPE * const wfp, const DEEPWAVE_TYPE * const phizc,
+    const DEEPWAVE_TYPE * const sigmaz, const DEEPWAVE_TYPE * const phiyc,
+    const DEEPWAVE_TYPE * const sigmay, const DEEPWAVE_TYPE * const phixc,
+    const DEEPWAVE_TYPE * const sigmax, const DEEPWAVE_TYPE * const psic,
+    const DEEPWAVE_TYPE * const model, const ptrdiff_t shape_z,
     const ptrdiff_t shape_y, const ptrdiff_t shape_x,
     const ptrdiff_t numel_shot, const ptrdiff_t size_xy,
     const ptrdiff_t num_shots, const ptrdiff_t pmlz0, const ptrdiff_t pmlz1,
     const ptrdiff_t pmly0, const ptrdiff_t pmly1, const ptrdiff_t pmlx0,
-    const ptrdiff_t pmlx1, const TYPE dt) {
+    const ptrdiff_t pmlx1, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t threadz = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t shot = threadz / (shape_z - ZPAD - ZPAD + 1);
   const ptrdiff_t z = threadz % (shape_z - ZPAD - ZPAD + 1) + ZPAD;
   const ptrdiff_t y = blockIdx.y * blockDim.y + threadIdx.y + YPAD;
   const ptrdiff_t x = blockIdx.x * blockDim.x + threadIdx.x + XPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD) && (y < shape_y - YPAD) &&
       (x < shape_x - XPAD)) {
     const ptrdiff_t i = z * size_xy + y * shape_x + x;
     const ptrdiff_t si = shot * numel_shot + i;
 
-    const TYPE lap = laplacian_3d(wfc, si, size_xy, shape_x);
+    const DEEPWAVE_TYPE lap = laplacian_3d(wfc, si, size_xy, shape_x);
 
     if ((z >= pmlz0 + 2 * ZPAD) && (z < shape_z - pmlz1 - 2 * ZPAD) &&
         (y >= pmly0 + 2 * YPAD) && (y < shape_y - pmly1 - 2 * YPAD) &&
         (x >= pmlx0 + 2 * XPAD) && (x < shape_x - pmlx1 - 2 * XPAD)) {
       /* Update wavefield */
       wfn[si] = model[i] * lap + 2 * wfc[si] - wfp[si];
     } else {
       /* Inside PML region */
 
-      const TYPE wfc_z = z_deriv(wfc, si, size_xy);
-      const TYPE wfc_y = y_deriv(wfc, si, shape_x);
-      const TYPE wfc_x = x_deriv(wfc, si);
-      const TYPE phizc_z = z_deriv(phizc, si, size_xy);
-      const TYPE phiyc_y = y_deriv(phiyc, si, shape_x);
-      const TYPE phixc_x = x_deriv(phixc, si);
-      const TYPE psic_z = z_deriv(psic, si, size_xy);
-      const TYPE psic_y = y_deriv(psic, si, shape_x);
-      const TYPE psic_x = x_deriv(psic, si);
+      const DEEPWAVE_TYPE wfc_z = z_deriv(wfc, si, size_xy);
+      const DEEPWAVE_TYPE wfc_y = y_deriv(wfc, si, shape_x);
+      const DEEPWAVE_TYPE wfc_x = x_deriv(wfc, si);
+      const DEEPWAVE_TYPE phizc_z = z_deriv(phizc, si, size_xy);
+      const DEEPWAVE_TYPE phiyc_y = y_deriv(phiyc, si, shape_x);
+      const DEEPWAVE_TYPE phixc_x = x_deriv(phixc, si);
+      const DEEPWAVE_TYPE psic_z = z_deriv(psic, si, size_xy);
+      const DEEPWAVE_TYPE psic_y = y_deriv(psic, si, shape_x);
+      const DEEPWAVE_TYPE psic_x = x_deriv(psic, si);
 
       /* Update wavefield */
       wfn[si] = 1 / (1 + dt * (sigmaz[z] + sigmay[y] + sigmax[x]) / 2) *
                 (model[i] * lap +
                  dt * dt *
                      (phizc_z + phiyc_y + phixc_x -
                       sigmaz[z] * sigmay[y] * sigmax[x] * psic[si]) +
@@ -578,41 +578,41 @@
 
       /* Update psi */
       psin[si] = psic[si] + dt * wfc[si];
     }
   }
 }
 
-void propagate(TYPE * const wfn,        /* next wavefield */
-               TYPE * const auxn,       /* next auxiliary */
-               const TYPE * const wfc,  /* current wavefield */
-               const TYPE * const wfp,  /* previous wavefield */
-               const TYPE * const auxc, /* current auxiliary */
-               const TYPE * const sigma,
-               const TYPE * const model,
-               const TYPE * const fd1_d, /* 1st diff coeffs */
-               const TYPE * const fd2_d, /* 2nd diff coeffs */
+void propagate(DEEPWAVE_TYPE * const wfn,        /* next wavefield */
+               DEEPWAVE_TYPE * const auxn,       /* next auxiliary */
+               const DEEPWAVE_TYPE * const wfc,  /* current wavefield */
+               const DEEPWAVE_TYPE * const wfp,  /* previous wavefield */
+               const DEEPWAVE_TYPE * const auxc, /* current auxiliary */
+               const DEEPWAVE_TYPE * const sigma,
+               const DEEPWAVE_TYPE * const model,
+               const DEEPWAVE_TYPE * const fd1_d, /* 1st diff coeffs */
+               const DEEPWAVE_TYPE * const fd2_d, /* 2nd diff coeffs */
                const ptrdiff_t * const shape,
                const ptrdiff_t * const pml_width,
-               const ptrdiff_t num_shots, const TYPE dt) {
+               const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t numel_shot = shape[0] * shape[1] * shape[2];
   const ptrdiff_t size_xy = shape[1] * shape[2];
-  TYPE * const phizn = auxn;
-  const TYPE * const phizc = auxc;
-  const TYPE * const sigmaz = sigma;
-
-  TYPE * const phiyn = auxn + num_shots * numel_shot;
-  const TYPE * const phiyc = auxc + num_shots * numel_shot;
-  const TYPE * const sigmay = sigma + shape[0];
-
-  TYPE * const phixn = auxn + 2 * num_shots * numel_shot;
-  TYPE * const psin = auxn + 3 * num_shots * numel_shot;
-  const TYPE * const phixc = auxc + 2 * num_shots * numel_shot;
-  const TYPE * const psic = auxc + 3 * num_shots * numel_shot;
-  const TYPE * const sigmax = sigma + shape[0] + shape[1];
+  DEEPWAVE_TYPE * const phizn = auxn;
+  const DEEPWAVE_TYPE * const phizc = auxc;
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+
+  DEEPWAVE_TYPE * const phiyn = auxn + num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const phiyc = auxc + num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
+
+  DEEPWAVE_TYPE * const phixn = auxn + 2 * num_shots * numel_shot;
+  DEEPWAVE_TYPE * const psin = auxn + 3 * num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const phixc = auxc + 2 * num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const psic = auxc + 3 * num_shots * numel_shot;
+  const DEEPWAVE_TYPE * const sigmax = sigma + shape[0] + shape[1];
 
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[2] - (2 * XPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (shape[1] - (2 * YPAD) + dimBlock.y - 1) / dimBlock.y;
   const int gridz =
       (num_shots * (shape[0] - (2 * ZPAD)) + dimBlock.z - 1) / dimBlock.z;
   const dim3 dimGrid(gridx, gridy, gridz);
@@ -622,22 +622,22 @@
       size_xy, num_shots, pml_width[0], pml_width[1], pml_width[2],
       pml_width[3], pml_width[4], pml_width[5], dt);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ imaging_condition_kernel(
-    TYPE * const model_grad,
-    const TYPE * const current_wavefield,
-    const TYPE * const current_saved_wavefield,
-    const TYPE * const current_saved_wavefield_t,
-    const TYPE * const current_saved_wavefield_tt,
-    const TYPE * const sigmaz,
-    const TYPE * const sigmay,
-    const TYPE * const sigmax, const ptrdiff_t shape_z,
+    DEEPWAVE_TYPE * const model_grad,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const sigmaz,
+    const DEEPWAVE_TYPE * const sigmay,
+    const DEEPWAVE_TYPE * const sigmax, const ptrdiff_t shape_z,
     const ptrdiff_t shape_y, const ptrdiff_t shape_x,
     const ptrdiff_t numel_shot, const ptrdiff_t size_xy,
     const ptrdiff_t num_shots) {
   const ptrdiff_t threadz = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t shot = threadz / (shape_z - ZPAD - ZPAD + 1);
   const ptrdiff_t z = threadz % (shape_z - ZPAD - ZPAD + 1) + ZPAD;
   const ptrdiff_t y = blockIdx.y * blockDim.y + threadIdx.y + YPAD;
@@ -658,50 +658,50 @@
                    (sigmax[x] * sigmay[y] + sigmay[y] * sigmaz[z] +
                     sigmax[x] * sigmaz[z]) *
                        current_saved_wavefield[si]));
   }
 }
 
 void imaging_condition(
-    TYPE * const model_grad,
-    const TYPE * const current_wavefield,
-    const TYPE * const current_saved_wavefield,
-    const TYPE * const current_saved_wavefield_t,
-    const TYPE * const current_saved_wavefield_tt,
-    const TYPE * const sigma,
+    DEEPWAVE_TYPE * const model_grad,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    const DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const sigma,
     const ptrdiff_t * const shape,
     const ptrdiff_t * const pml_width, const ptrdiff_t num_shots) {
   if (model_grad == NULL) return; /* Not doing model inversion */
 
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[2] - (2 * XPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (shape[1] - (2 * YPAD) + dimBlock.y - 1) / dimBlock.y;
   const int gridz =
       (num_shots * (shape[0] - (2 * ZPAD)) + dimBlock.z - 1) / dimBlock.z;
 
   const dim3 dimGrid(gridx, gridy, gridz);
-  const TYPE * const sigmaz = sigma;
-  const TYPE * const sigmay = sigma + shape[0];
-  const TYPE * const sigmax = sigma + shape[0] + shape[1];
+  const DEEPWAVE_TYPE * const sigmaz = sigma;
+  const DEEPWAVE_TYPE * const sigmay = sigma + shape[0];
+  const DEEPWAVE_TYPE * const sigmax = sigma + shape[0] + shape[1];
 
   imaging_condition_kernel<<<dimGrid, dimBlock>>>(
       model_grad, current_wavefield, current_saved_wavefield,
       current_saved_wavefield_t, current_saved_wavefield_tt, sigmaz, sigmay,
       sigmax, shape[0], shape[1], shape[2], shape[0] * shape[1] * shape[2],
       shape[1] * shape[2], num_shots);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ add_scattering_kernel(
-    TYPE * const next_scattered_wavefield,
-    const TYPE * const next_wavefield,
-    const TYPE * const current_wavefield,
-    const TYPE * const previous_wavefield,
-    const TYPE * const scatter,
+    DEEPWAVE_TYPE * const next_scattered_wavefield,
+    const DEEPWAVE_TYPE * const next_wavefield,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const previous_wavefield,
+    const DEEPWAVE_TYPE * const scatter,
     const ptrdiff_t shape_z,
     const ptrdiff_t shape_y,
     const ptrdiff_t shape_x,
     const ptrdiff_t numel_shot, const ptrdiff_t size_xy,
     const ptrdiff_t num_shots) {
   const ptrdiff_t threadz = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t shot = threadz / (shape_z - ZPAD - ZPAD + 1);
@@ -709,27 +709,27 @@
   const ptrdiff_t y = blockIdx.y * blockDim.y + threadIdx.y + YPAD;
   const ptrdiff_t x = blockIdx.x * blockDim.x + threadIdx.x + XPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD) && (y < shape_y - YPAD) &&
       (x < shape_x - XPAD)) {
     const ptrdiff_t i = z * size_xy + y * shape_x + x;
     const ptrdiff_t si = shot * numel_shot + i;
 
-    const TYPE current_wavefield_tt =
+    const DEEPWAVE_TYPE current_wavefield_tt =
         (next_wavefield[si] - 2 * current_wavefield[si] +
          previous_wavefield[si]); /* no dt^2 because of cancellation */
     next_scattered_wavefield[si] += current_wavefield_tt * scatter[i];
   }
 }
 
 void add_scattering(
-                     TYPE * const next_scattered_wavefield,
-                     const TYPE * const next_wavefield,
-                     const TYPE * const current_wavefield,
-                     const TYPE * const previous_wavefield,
-                     const TYPE * const scatter,
+                     DEEPWAVE_TYPE * const next_scattered_wavefield,
+                     const DEEPWAVE_TYPE * const next_wavefield,
+                     const DEEPWAVE_TYPE * const current_wavefield,
+                     const DEEPWAVE_TYPE * const previous_wavefield,
+                     const DEEPWAVE_TYPE * const scatter,
                      const ptrdiff_t * const shape,
                      const ptrdiff_t num_shots) {
   const dim3 dimBlock(32, 32, 1);
   const int gridx = (shape[2] - (2 * XPAD) + dimBlock.x - 1) / dimBlock.x;
   const int gridy = (shape[1] - (2 * YPAD) + dimBlock.y - 1) / dimBlock.y;
   const int gridz =
       (num_shots * (shape[0] - (2 * ZPAD)) + dimBlock.z - 1) / dimBlock.z;
@@ -739,22 +739,22 @@
       next_scattered_wavefield, next_wavefield,
       current_wavefield, previous_wavefield, scatter, shape[0], shape[1],
       shape[2], shape[0] * shape[1] * shape[2], shape[1] * shape[2], num_shots);
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ save_wavefields_kernel(
-    TYPE * const current_saved_wavefield_t,
-    TYPE * const current_saved_wavefield_tt,
-    const TYPE * const next_wavefield,
-    const TYPE * const current_wavefield,
-    const TYPE * const previous_wavefield, const ptrdiff_t shape_z,
+    DEEPWAVE_TYPE * const current_saved_wavefield_t,
+    DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+    const DEEPWAVE_TYPE * const next_wavefield,
+    const DEEPWAVE_TYPE * const current_wavefield,
+    const DEEPWAVE_TYPE * const previous_wavefield, const ptrdiff_t shape_z,
     const ptrdiff_t shape_y, const ptrdiff_t shape_x,
     const ptrdiff_t numel_shot, const ptrdiff_t size_xy,
-    const ptrdiff_t num_shots, const TYPE dt) {
+    const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt) {
   const ptrdiff_t threadz = blockIdx.z * blockDim.z + threadIdx.z;
   const ptrdiff_t shot = threadz / (shape_z - ZPAD - ZPAD + 1);
   const ptrdiff_t z = threadz % (shape_z - ZPAD - ZPAD + 1) + ZPAD;
   const ptrdiff_t y = blockIdx.y * blockDim.y + threadIdx.y + YPAD;
   const ptrdiff_t x = blockIdx.x * blockDim.x + threadIdx.x + XPAD;
   if ((shot < num_shots) && (z < shape_z - ZPAD) && (y < shape_y - YPAD) &&
       (x < shape_x - XPAD)) {
@@ -767,27 +767,27 @@
     current_saved_wavefield_tt[si] =
         (next_wavefield[si] - 2 * current_wavefield[si] +
          previous_wavefield[si]) /
         dt / dt;
   }
 }
 
-void save_wavefields(TYPE * const current_saved_wavefield,
-                     TYPE * const current_saved_wavefield_t,
-                     TYPE * const current_saved_wavefield_tt,
-                     const TYPE * const next_wavefield,
-                     const TYPE * const current_wavefield,
-                     const TYPE * const previous_wavefield,
+void save_wavefields(DEEPWAVE_TYPE * const current_saved_wavefield,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_t,
+                     DEEPWAVE_TYPE * const current_saved_wavefield_tt,
+                     const DEEPWAVE_TYPE * const next_wavefield,
+                     const DEEPWAVE_TYPE * const current_wavefield,
+                     const DEEPWAVE_TYPE * const previous_wavefield,
                      const ptrdiff_t * const shape,
-                     const ptrdiff_t num_shots, const TYPE dt,
+                     const ptrdiff_t num_shots, const DEEPWAVE_TYPE dt,
                      const enum wavefield_save_strategy save_strategy) {
   if (save_strategy == STRATEGY_COPY) {
     gpuErrchk(
         cudaMemcpy(current_saved_wavefield, current_wavefield,
-                   num_shots * shape[0] * shape[1] * shape[2] * sizeof(TYPE),
+                   num_shots * shape[0] * shape[1] * shape[2] * sizeof(DEEPWAVE_TYPE),
                    cudaMemcpyDeviceToDevice));
     const dim3 dimBlock(32, 32, 1);
     const int gridx = (shape[2] - (2 * XPAD) + dimBlock.x - 1) / dimBlock.x;
     const int gridy = (shape[1] - (2 * YPAD) + dimBlock.y - 1) / dimBlock.y;
     const int gridz =
         (num_shots * (shape[0] - (2 * ZPAD)) + dimBlock.z - 1) / dimBlock.z;
 
@@ -806,57 +806,57 @@
   const ptrdiff_t z = arr[index * 3];
   const ptrdiff_t y = arr[index * 3 + 1];
   const ptrdiff_t x = arr[index * 3 + 2];
 
   return z * shape_y * shape_x + y * shape_x + x;
 }
 
-static inline __device__ TYPE laplacian_3d(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE laplacian_3d(const DEEPWAVE_TYPE * const arr,
                                            const ptrdiff_t si,
                                            const ptrdiff_t size_x,
                                            const ptrdiff_t size_xy) {
   return fd2[0] * arr[si] + fd2[1] * (arr[si + size_xy] + arr[si - size_xy]) +
          fd2[2] * (arr[si + 2 * size_xy] + arr[si - 2 * size_xy]) +
          +fd2[3] * (arr[si + size_x] + arr[si - size_x]) +
          fd2[4] * (arr[si + 2 * size_x] + arr[si - 2 * size_x]) +
          fd2[5] * (arr[si + 1] + arr[si - 1]) +
          fd2[6] * (arr[si + 2] + arr[si - 2]);
 }
 
 #else
-#error "Must specify the dimension, e.g. -D DIM=1"
-#endif /* DIM */
+#error "Must specify the dimension, e.g. -D DEEPWAVE_DIM=1"
+#endif /* DEEPWAVE_DIM */
 
-void setup(const TYPE * const fd1_d,
-           const TYPE * const fd2_d) {
-  gpuErrchk(cudaMemcpyToSymbol(fd1, fd1_d, 2 * DIM * sizeof(TYPE)));
-  gpuErrchk(cudaMemcpyToSymbol(fd2, fd2_d, (2 * DIM + 1) * sizeof(TYPE)));
+void setup(const DEEPWAVE_TYPE * const fd1_d,
+           const DEEPWAVE_TYPE * const fd2_d) {
+  gpuErrchk(cudaMemcpyToSymbol(fd1, fd1_d, 2 * DEEPWAVE_DIM * sizeof(DEEPWAVE_TYPE)));
+  gpuErrchk(cudaMemcpyToSymbol(fd2, fd2_d, (2 * DEEPWAVE_DIM + 1) * sizeof(DEEPWAVE_TYPE)));
 }
 
 void __global__ add_sources_kernel(
-    TYPE * const next_wavefield,
-    const TYPE * const model,
-    const TYPE * const source_amplitudes,
+    DEEPWAVE_TYPE * const next_wavefield,
+    const DEEPWAVE_TYPE * const model,
+    const DEEPWAVE_TYPE * const source_amplitudes,
     const ptrdiff_t * const source_locations,
     const ptrdiff_t shape_z, const ptrdiff_t shape_y, const ptrdiff_t shape_x,
     const ptrdiff_t num_shots, const ptrdiff_t num_sources_per_shot) {
   ptrdiff_t shot = blockIdx.y * blockDim.y + threadIdx.y;
   ptrdiff_t source = blockIdx.x * blockDim.x + threadIdx.x;
 
   if ((shot < num_shots) && (source < num_sources_per_shot)) {
     ptrdiff_t s = shot * num_sources_per_shot + source;
     ptrdiff_t i = location_index(source_locations, shape_y, shape_x, s);
     ptrdiff_t si = shot * shape_z * shape_y * shape_x + i;
     atomicAdd(next_wavefield + si, source_amplitudes[s] * model[i]);
   }
 }
 
-void add_sources(TYPE * const next_wavefield,
-                 const TYPE * const model,
-                 const TYPE * const source_amplitudes,
+void add_sources(DEEPWAVE_TYPE * const next_wavefield,
+                 const DEEPWAVE_TYPE * const model,
+                 const DEEPWAVE_TYPE * const source_amplitudes,
                  const ptrdiff_t * const source_locations,
                  const ptrdiff_t * const shape,
                  const ptrdiff_t num_shots,
                  const ptrdiff_t num_sources_per_shot) {
   dim3 dimBlock(32, 1, 1);
   int gridx = (num_sources_per_shot + dimBlock.x - 1) / dimBlock.x;
   int gridy = (num_shots + dimBlock.y - 1) / dimBlock.y;
@@ -867,32 +867,32 @@
       next_wavefield, model, source_amplitudes, source_locations, shape[0],
       shape[1], shape[2], num_shots, num_sources_per_shot);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ record_receivers_kernel(
-    TYPE * const receiver_amplitudes,
-    const TYPE * const current_wavefield,
+    DEEPWAVE_TYPE * const receiver_amplitudes,
+    const DEEPWAVE_TYPE * const current_wavefield,
     const ptrdiff_t * const receiver_locations,
     const ptrdiff_t shape_z, const ptrdiff_t shape_y, const ptrdiff_t shape_x,
     const ptrdiff_t num_shots, const ptrdiff_t num_receivers_per_shot) {
   ptrdiff_t shot = blockIdx.y * blockDim.y + threadIdx.y;
   ptrdiff_t receiver = blockIdx.x * blockDim.x + threadIdx.x;
 
   if ((shot < num_shots) && (receiver < num_receivers_per_shot)) {
     ptrdiff_t r = shot * num_receivers_per_shot + receiver;
     ptrdiff_t si = shot * shape_z * shape_y * shape_x +
                    location_index(receiver_locations, shape_y, shape_x, r);
     receiver_amplitudes[r] = current_wavefield[si];
   }
 }
 
-void record_receivers(TYPE * const receiver_amplitudes,
-                      const TYPE * const current_wavefield,
+void record_receivers(DEEPWAVE_TYPE * const receiver_amplitudes,
+                      const DEEPWAVE_TYPE * const current_wavefield,
                       const ptrdiff_t * const receiver_locations,
                       const ptrdiff_t * const shape,
                       const ptrdiff_t num_shots,
                       const ptrdiff_t num_receivers_per_shot) {
   if (receiver_amplitudes == NULL) return; /* no source inversion */
 
   dim3 dimBlock(32, 1, 1);
@@ -905,25 +905,25 @@
       receiver_amplitudes, current_wavefield, receiver_locations, shape[0],
       shape[1], shape[2], num_shots, num_receivers_per_shot);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
 void __global__ model_grad_scaling_kernel(
-    TYPE * const model_grad, const TYPE * const scaling,
+    DEEPWAVE_TYPE * const model_grad, const DEEPWAVE_TYPE * const scaling,
     const ptrdiff_t numel_shot) {
   ptrdiff_t i = blockIdx.x * blockDim.x + threadIdx.x;
 
   if (i < numel_shot) {
     model_grad[i] *= scaling[i];
   }
 }
 
-void model_grad_scaling(TYPE * const model_grad,
-                        const TYPE * const scaling,
+void model_grad_scaling(DEEPWAVE_TYPE * const model_grad,
+                        const DEEPWAVE_TYPE * const scaling,
                         const ptrdiff_t * const shape,
                         const ptrdiff_t * const pml_width) {
   if (model_grad == NULL) return; /* Not doing model inversion */
 
   const ptrdiff_t numel_shot = shape[0] * shape[1] * shape[2];
 
   dim3 dimBlock(32, 1, 1);
@@ -934,26 +934,26 @@
 
   model_grad_scaling_kernel<<<dimGrid, dimBlock>>>(model_grad, scaling,
                                                    numel_shot);
 
   gpuErrchk(cudaPeekAtLastError());
 }
 
-static inline __device__ TYPE z_deriv(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE z_deriv(const DEEPWAVE_TYPE * const arr,
                                       const ptrdiff_t si,
                                       const ptrdiff_t size_xy) {
   return fd1[0] * (arr[si + size_xy] - arr[si - size_xy]) +
          fd1[1] * (arr[si + 2 * size_xy] - arr[si - 2 * size_xy]);
 }
 
-static inline __device__ TYPE y_deriv(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE y_deriv(const DEEPWAVE_TYPE * const arr,
                                       const ptrdiff_t si,
                                       const ptrdiff_t size_x) {
   return fd1[0] * (arr[si + size_x] - arr[si - size_x]) +
          fd1[1] * (arr[si + 2 * size_x] - arr[si - 2 * size_x]);
 }
 
-static inline __device__ TYPE x_deriv(const TYPE * const arr,
+static inline __device__ DEEPWAVE_TYPE x_deriv(const DEEPWAVE_TYPE * const arr,
                                       const ptrdiff_t si) {
   return fd1[0] * (arr[si + 1] - arr[si - 1]) +
          fd1[1] * (arr[si + 2] - arr[si - 2]);
 }
```

### Comparing `deepwave-0.0.8/deepwave/scalar/scalar_wrapper.cpp` & `deepwave-0.0.9/deepwave/scalar/scalar_wrapper.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,22 @@
                      at::Tensor receiver_locations, at::Tensor shape,
                      at::Tensor pml_width, at::Tensor dt,
                      const ptrdiff_t num_steps, const ptrdiff_t step_ratio,
                      const ptrdiff_t num_shots,
                      const ptrdiff_t num_sources_per_shot,
                      const ptrdiff_t num_receivers_per_shot,
                      const enum wavefield_save_strategy save_strategy) {
-  forward(wavefield.data_ptr<TYPE>(), aux_wavefield.data_ptr<TYPE>(),
-          receiver_amplitudes.data_ptr<TYPE>(), saved_wavefields.data_ptr<TYPE>(),
-          sigma.data_ptr<TYPE>(), model.data_ptr<TYPE>(), fd1.data_ptr<TYPE>(),
-          fd2.data_ptr<TYPE>(), source_amplitudes.data_ptr<TYPE>(),
+  forward(wavefield.data_ptr<DEEPWAVE_TYPE>(), aux_wavefield.data_ptr<DEEPWAVE_TYPE>(),
+          receiver_amplitudes.data_ptr<DEEPWAVE_TYPE>(), saved_wavefields.data_ptr<DEEPWAVE_TYPE>(),
+          sigma.data_ptr<DEEPWAVE_TYPE>(), model.data_ptr<DEEPWAVE_TYPE>(), fd1.data_ptr<DEEPWAVE_TYPE>(),
+          fd2.data_ptr<DEEPWAVE_TYPE>(), source_amplitudes.data_ptr<DEEPWAVE_TYPE>(),
           source_locations.data_ptr<ptrdiff_t>(),
           receiver_locations.data_ptr<ptrdiff_t>(), shape.data_ptr<ptrdiff_t>(),
           pml_width.data_ptr<ptrdiff_t>(), num_steps, step_ratio, num_shots,
-          num_sources_per_shot, num_receivers_per_shot, dt.data_ptr<TYPE>()[0],
+          num_sources_per_shot, num_receivers_per_shot, dt.data_ptr<DEEPWAVE_TYPE>()[0],
           save_strategy);
 }
 
 void forward_born_wrapper(
     at::Tensor wavefield, at::Tensor aux_wavefield,
     at::Tensor scattered_wavefield, at::Tensor scattered_aux_wavefield,
     at::Tensor receiver_amplitudes, at::Tensor saved_wavefields,
@@ -32,24 +32,24 @@
     at::Tensor scatter, at::Tensor fd1, at::Tensor fd2,
     at::Tensor source_amplitudes, at::Tensor source_locations,
     at::Tensor receiver_locations, at::Tensor shape, at::Tensor pml_width,
     at::Tensor dt, const ptrdiff_t num_steps, const ptrdiff_t step_ratio,
     const ptrdiff_t num_shots, const ptrdiff_t num_sources_per_shot,
     const ptrdiff_t num_receivers_per_shot,
     const enum wavefield_save_strategy save_strategy) {
-  forward_born(wavefield.data_ptr<TYPE>(), aux_wavefield.data_ptr<TYPE>(),
-	       scattered_wavefield.data_ptr<TYPE>(), scattered_aux_wavefield.data_ptr<TYPE>(),
-               receiver_amplitudes.data_ptr<TYPE>(), saved_wavefields.data_ptr<TYPE>(),
-               sigma.data_ptr<TYPE>(),
-               model.data_ptr<TYPE>(), scatter.data_ptr<TYPE>(), fd1.data_ptr<TYPE>(),
-               fd2.data_ptr<TYPE>(), source_amplitudes.data_ptr<TYPE>(),
+  forward_born(wavefield.data_ptr<DEEPWAVE_TYPE>(), aux_wavefield.data_ptr<DEEPWAVE_TYPE>(),
+	       scattered_wavefield.data_ptr<DEEPWAVE_TYPE>(), scattered_aux_wavefield.data_ptr<DEEPWAVE_TYPE>(),
+               receiver_amplitudes.data_ptr<DEEPWAVE_TYPE>(), saved_wavefields.data_ptr<DEEPWAVE_TYPE>(),
+               sigma.data_ptr<DEEPWAVE_TYPE>(),
+               model.data_ptr<DEEPWAVE_TYPE>(), scatter.data_ptr<DEEPWAVE_TYPE>(), fd1.data_ptr<DEEPWAVE_TYPE>(),
+               fd2.data_ptr<DEEPWAVE_TYPE>(), source_amplitudes.data_ptr<DEEPWAVE_TYPE>(),
                source_locations.data_ptr<ptrdiff_t>(),
                receiver_locations.data_ptr<ptrdiff_t>(), shape.data_ptr<ptrdiff_t>(),
                pml_width.data_ptr<ptrdiff_t>(), num_steps, step_ratio, num_shots,
-               num_sources_per_shot, num_receivers_per_shot, dt.data_ptr<TYPE>()[0],
+               num_sources_per_shot, num_receivers_per_shot, dt.data_ptr<DEEPWAVE_TYPE>()[0],
                save_strategy);
 }
 
 void backward_wrapper(at::Tensor wavefield, at::Tensor aux_wavefield,
                       at::Tensor model_grad, at::Tensor source_grad_amplitudes,
                       at::Tensor adjoint_wavefield, at::Tensor scaling,
                       at::Tensor sigma, at::Tensor model, at::Tensor fd1,
@@ -57,23 +57,23 @@
                       at::Tensor source_locations,
                       at::Tensor receiver_locations, at::Tensor shape,
                       at::Tensor pml_width, at::Tensor dt,
                       const ptrdiff_t num_steps, const ptrdiff_t step_ratio,
                       const ptrdiff_t num_shots,
                       const ptrdiff_t num_sources_per_shot,
                       const ptrdiff_t num_receivers_per_shot) {
-  backward(wavefield.data_ptr<TYPE>(), aux_wavefield.data_ptr<TYPE>(),
-           model_grad.data_ptr<TYPE>(), source_grad_amplitudes.data_ptr<TYPE>(),
-           adjoint_wavefield.data_ptr<TYPE>(), scaling.data_ptr<TYPE>(),
-           sigma.data_ptr<TYPE>(), model.data_ptr<TYPE>(), fd1.data_ptr<TYPE>(),
-           fd2.data_ptr<TYPE>(), receiver_grad_amplitudes.data_ptr<TYPE>(),
+  backward(wavefield.data_ptr<DEEPWAVE_TYPE>(), aux_wavefield.data_ptr<DEEPWAVE_TYPE>(),
+           model_grad.data_ptr<DEEPWAVE_TYPE>(), source_grad_amplitudes.data_ptr<DEEPWAVE_TYPE>(),
+           adjoint_wavefield.data_ptr<DEEPWAVE_TYPE>(), scaling.data_ptr<DEEPWAVE_TYPE>(),
+           sigma.data_ptr<DEEPWAVE_TYPE>(), model.data_ptr<DEEPWAVE_TYPE>(), fd1.data_ptr<DEEPWAVE_TYPE>(),
+           fd2.data_ptr<DEEPWAVE_TYPE>(), receiver_grad_amplitudes.data_ptr<DEEPWAVE_TYPE>(),
            source_locations.data_ptr<ptrdiff_t>(),
            receiver_locations.data_ptr<ptrdiff_t>(), shape.data_ptr<ptrdiff_t>(),
            pml_width.data_ptr<ptrdiff_t>(), num_steps, step_ratio, num_shots,
-           num_sources_per_shot, num_receivers_per_shot, dt.data_ptr<TYPE>()[0]);
+           num_sources_per_shot, num_receivers_per_shot, dt.data_ptr<DEEPWAVE_TYPE>()[0]);
 }
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
   m.def("forward", &forward_wrapper, "forward");
   m.def("forward_born", &forward_born_wrapper, "forward_born");
   m.def("backward", &backward_wrapper, "backward");
   py::enum_<wavefield_save_strategy>(m, "wavefield_save_strategy",
```

### Comparing `deepwave-0.0.8/deepwave/utils.py` & `deepwave-0.0.9/deepwave/utils.py`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/deepwave/wavelets.py` & `deepwave-0.0.9/deepwave/wavelets.py`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/deepwave.egg-info/PKG-INFO` & `deepwave-0.0.9/deepwave.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: deepwave
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wave propagation modules for PyTorch.
 Home-page: https://github.com/ar4/deepwave
 Author: Alan Richardson
 Author-email: alan@ausargeo.com
 License: UNKNOWN
 Description: # Deepwave
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/52d27677ef0a439195d574964a6b4be4)](https://www.codacy.com/app/ar4/deepwave?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ar4/deepwave&amp;utm_campaign=Badge_Grade)
         
         Deepwave provides wave propagation modules for PyTorch (currently only for the constant density acoustic / scalar wave equation). It is primarily aimed at seismic imaging/inversion. One interesting advantage of this is that it allows you to chain operations together. You could, for example, use Deepwave to perform FWI using a custom cost function (as long as PyTorch is able to automatically differentiate it), or add some other operations before and after wave propagation and PyTorch will backpropagate through all of them.
         
         Wave propagation and FWI [can be implemented using deep neural networks](https://arxiv.org/abs/1801.07232). Deep learning tools such as TensorFlow and PyTorch are currently too slow and memory inefficient to do this with realistic seismic datasets, however. Deepwave extends PyTorch with higher performance wave propagation modules (written in C and CUDA) so that you can benefit from the conveniences of PyTorch without sacrificing performance.
         
         Deepwave runs on CPUs and NVIDIA GPUs. It should automatically detect compatible GPUs during installation and compile the GPU code if any are found. To run on the GPU you must transfer the model, source amplitude, and source and receiver location Tensors to the GPU in the standard PyTorch way (using `.cuda()` or `.to(device)`).
         
         ## Installation
         Deepwave needs NumPy, so [installing Anaconda](https://www.anaconda.com/download) first is highly recommended. It also needs [PyTorch](https://pytorch.org/), so it is also best to install that (using something like `conda install pytorch-cpu -c pytorch`) before installing Deepwave. You can then install the latest release of Deepwave using
         
         `pip install deepwave`
         
-        or the latest development version using
-        
-        `pip install git+https://github.com/ar4/deepwave.git`
-        
+        Note that this will probably take several minutes as it needs to compile the code.
         
         ## Usage
         Deepwave can do two things: forward modeling and backpropagation.
         
         ### Forward modeling
         We first need to create a wave propagation module. If you are familiar with training neural networks, this is the same as defining your network (or a portion of it) and initializing the weights.
         
@@ -131,19 +127,35 @@
         
         For an example of using Deepwave for LSRTM, see [this notebook](https://colab.research.google.com/drive/1BgQM5VGgyFp7Q--pAJX-vGb2bW9mcbM8).
         
         ## Notes
         * For a reflective free surface, set the PML width to zero at the surface. For example, in 3D and when the PML width on the other sides is 10 cells, provide the argument `pml_width=[0,10,10,10,10,10]` when creating the propagator if the free surface is at the beginning of the first dimension. The format is [z1, z2, y1, y2, x1, x2], where z1, y1, and x1 are the PML widths at the beginning of the z, y, and x dimensions, and z2, y2, and x2 are the PML widths at the ends of those dimensions.
         * To limit wave simulation to the region covered by the survey (the sources and receivers), provide the `survey_pad` keyword argument when creating the propagator. For example, to use the whole z dimension, but only up to 100m from the first and last source/receiver in the y and x dimensions, use `survey_pad=[None, None, 100, 100, 100, 100]`, where `None` means continue to the edge of the model, and the format is similar to that used for `pml_width`. The default is `None` for every entry.
         * [@LukasMosser](https://github.com/LukasMosser) discovered that GCC 4.9 or above is necessary ([#18](https://github.com/ar4/deepwave/issues/18)).
+        * [@ADharaUTEXAS123007](https://github.com/ADharaUTEXAS123007) discovered that for recent versions of PyTorch an even later release of GCC might be necessary. A warning was displayed (Your compiler (g++ 4.8.5) may be ABI-incompatible with PyTorch!
+        Please use a compiler that is ABI-compatible with GCC 5.0 and above.) and compilation failed. This was resolved with `conda install gxx_linux-64`.
         * Distributed parallelization over shots is supported, but not within a shot; each shot must run within one node.
-        * Currently, the forward source wavefield is saved in memory for use during backpropagation. This means that realistic 3D surveys will probably require more memory than is available. This will be fixed in a future release.
-        
-        ## Contributing
-        Your help to improve Deepwave would be greatly appreciated. If you encounter any difficulty using Deepwave, please report it as a Github Issue so that it can be fixed. If you have feature suggestions or other ideas to make Deepwave better, please also report those as Github Issues. If you want to help with the coding, that would be especially wonderful. The Github Issues contain a list of things that need work. If you see one that you would like to attempt, please ask for it to be assigned to you.
+        * Currently, the forward source wavefield is saved in memory for use during backpropagation. This means that realistic 3D surveys will probably require more memory than is available.
+        * [@erellaz](https://github.com/erellaz) has created [a nice tool](https://github.com/erellaz/SEGY_Wrapper) to make loading and saving SEG-Y files easier, and a demonstration of using Deepwave for forward modeling with a realistic 2D model.
+        * Your help to improve Deepwave would be greatly appreciated. If you encounter any difficulty using Deepwave, please report it as a Github Issue so that it can be fixed.
+        
+        ## Citing
+        If you would like to cite Deepwave, I suggest
+        ```
+        @software{deepwave,
+          author       = {Richardson, Alan},
+          title        = {Deepwave},
+          month        = oct,
+          year         = 2021,
+          publisher    = {Zenodo},
+          version      = {v0.0.9},
+          doi          = {10.5281/zenodo.3829886},
+          url          = {https://doi.org/10.5281/zenodo.3829886}
+        }
+        ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `deepwave-0.0.8/deepwave.egg-info/SOURCES.txt` & `deepwave-0.0.9/deepwave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepwave-0.0.8/setup.py` & `deepwave-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 scalar_gpu_file = os.path.join(scalar_dir, 'scalar_gpu.cu')
 scalar_wrapper_file = os.path.join(scalar_dir, 'scalar_wrapper.cpp')
 
 
 def _make_cpp_extension(dim, dtype):
     return CppExtension('scalar{}d_cpu_iso_4_{}'.format(dim, dtype),
                         [scalar_cpu_file, scalar_cpp_file, scalar_wrapper_file],
-                        define_macros=[('DIM', dim), ('TYPE', dtype)],
+                        define_macros=[('DEEPWAVE_DIM', dim), ('DEEPWAVE_TYPE', dtype)],
                         include_dirs=[scalar_dir],
                         extra_compile_args=['-Ofast', '-march=native',
                                             '-fopenmp'],
                         extra_link_args=['-fopenmp'])
 
 
 def _make_cuda_extension(dim, dtype):
     return CUDAExtension('scalar{}d_gpu_iso_4_{}'.format(dim, dtype),
                          [scalar_gpu_file, scalar_cpp_file, scalar_wrapper_file],
-                         define_macros=[('DIM', dim), ('TYPE', dtype)],
+                         define_macros=[('DEEPWAVE_DIM', dim), ('DEEPWAVE_TYPE', dtype)],
                          include_dirs=[scalar_dir],
                          extra_compile_args={'nvcc': ['--restrict', '-O3',
                                                       '--use_fast_math'],
                                              'cxx': ['-Ofast', '-march=native']})
 
 
 cpp_extensions = [_make_cpp_extension(dim, dtype)
@@ -43,15 +43,15 @@
                        for dim in ['1', '2', '3']
                        for dtype in ['float']]
 else:
     cuda_extensions = []
 
 setuptools.setup(
     name="deepwave",
-    version="0.0.8",
+    version="0.0.9",
     author="Alan Richardson",
     author_email="alan@ausargeo.com",
     description="Wave propagation modules for PyTorch.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ar4/deepwave",
     packages=setuptools.find_packages(),
```

