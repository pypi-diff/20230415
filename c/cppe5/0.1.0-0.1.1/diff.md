# Comparing `tmp/cppe5-0.1.0.tar.gz` & `tmp/cppe5-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppe5-0.1.0.tar", last modified: Tue Dec 14 19:20:55 2021, max compression
+gzip compressed data, was "cppe5-0.1.1.tar", last modified: Sat Apr 15 00:57:58 2023, max compression
```

## Comparing `cppe5-0.1.0.tar` & `cppe5-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 19:20:55.164831 cppe5-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-14 19:20:42.000000 cppe5-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-12-14 19:20:42.000000 cppe5-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    16540 2021-12-14 19:20:55.164831 cppe5-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15325 2021-12-14 19:20:42.000000 cppe5-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 19:20:55.160831 cppe5-0.1.0/cppe5/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-12-14 19:20:42.000000 cppe5-0.1.0/cppe5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2021-12-14 19:20:42.000000 cppe5-0.1.0/cppe5/download.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-12-14 19:20:42.000000 cppe5-0.1.0/cppe5/download_tfrecords.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-12-14 19:20:42.000000 cppe5-0.1.0/cppe5/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2021-12-14 19:20:42.000000 cppe5-0.1.0/cppe5/torch.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-14 19:20:42.000000 cppe5-0.1.0/cppe5/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 19:20:55.164831 cppe5-0.1.0/cppe5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16540 2021-12-14 19:20:55.000000 cppe5-0.1.0/cppe5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-12-14 19:20:55.000000 cppe5-0.1.0/cppe5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 19:20:55.000000 cppe5-0.1.0/cppe5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-14 19:20:55.000000 cppe5-0.1.0/cppe5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-14 19:20:55.000000 cppe5-0.1.0/cppe5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-14 19:20:55.164831 cppe5-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2021-12-14 19:20:42.000000 cppe5-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:57:58.829327 cppe5-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 00:57:46.000000 cppe5-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-15 00:57:46.000000 cppe5-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-04-15 00:57:58.829327 cppe5-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-04-15 00:57:46.000000 cppe5-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:57:58.829327 cppe5-0.1.1/cppe5/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-15 00:57:46.000000 cppe5-0.1.1/cppe5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 00:57:46.000000 cppe5-0.1.1/cppe5/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-15 00:57:46.000000 cppe5-0.1.1/cppe5/download_tfrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-15 00:57:46.000000 cppe5-0.1.1/cppe5/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-15 00:57:46.000000 cppe5-0.1.1/cppe5/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 00:57:46.000000 cppe5-0.1.1/cppe5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:57:58.829327 cppe5-0.1.1/cppe5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-04-15 00:57:58.000000 cppe5-0.1.1/cppe5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-15 00:57:58.000000 cppe5-0.1.1/cppe5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:57:58.000000 cppe5-0.1.1/cppe5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-15 00:57:58.000000 cppe5-0.1.1/cppe5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 00:57:58.000000 cppe5-0.1.1/cppe5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 00:57:58.829327 cppe5-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-15 00:57:46.000000 cppe5-0.1.1/setup.py
```

### Comparing `cppe5-0.1.0/LICENSE` & `cppe5-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cppe5-0.1.0/PKG-INFO` & `cppe5-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,39 @@
-Metadata-Version: 2.1
-Name: cppe5
-Version: 0.1.0
-Summary: A library to easily download, load and work with the CPPE-5 dataset.
-Home-page: https://github.com/Rishit-dagli/CPPE-Dataset
-Author: Rishit Dagli, Ali Mustufa
-Author-email: rishit.dagli@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # CPPE - 5 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2FRishit-dagli%2Fhttps://github.com/Rishit-dagli/CPPE-Dataset)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2FRishit-dagli%2Fhttps://github.com/Rishit-dagli/CPPE-Dataset)
 
 ![GitHub Repo stars](https://img.shields.io/github/stars/Rishit-dagli/CPPE-Dataset?style=social)
+[![arXiv](https://img.shields.io/badge/paper-arXiv:2112.09569-b31b1b.svg?logo=arxiv)](https://arxiv.org/abs/2112.09569)
+[![Models TF Hub](https://img.shields.io/badge/Models-TF%20Hub-orange?style=flat&logo=tensorflow)](https://tfhub.dev/rishit-dagli/collections/cppe5)
+
 ![PyPI](https://img.shields.io/pypi/v/cppe5)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 CPPE - 5 (Medical Personal Protective Equipment) is a new challenging dataset
 with the goal to allow the study of subordinate categorization of medical
 personal protective equipments, which is not possible with other popular data
 sets that focus on broad level categories.
 
+_**Accompanying paper: [CPPE - 5: Medical Personal Protective Equipment Dataset](https://arxiv.org/abs/2112.09569)**_
+
+_**by Rishit Dagli and Ali Mustufa Shaikh.**_
+
 Some features of this dataset are:
 - high quality images and annotations (~4.6 bounding boxes per image)
 - real-life images unlike any current such dataset
 - majority of non-iconic images (allowing easy deployment to real-world environments)
 - \>15 pre-trained models in the model zoo availaible to directly use (also for mobile and edge devices)
 
 ![](media/annotation_type.png)
 
+## Updates
+
+- 06/01/2022 - Many thanks to [@mariosasko](https://github.com/mariosasko) for creating a [Hugging Face Datasets loader](https://huggingface.co/datasets/cppe-5).
+- 05/01/2022 - This paper got featured on Google Research TRC's [publication section](https://sites.research.google/trc/publications/)
+- 20/12/2021 - First public release of the CPPE - 5 dataset on arXiv
+
 ## Get the data
 
 We strongly recommend you use either the downlaoder script or the Python package
 to download the dataset however you could also download and extract it manually.
 
 | Name | Size | Drive | Bucket | MD5 checksum |
 |:----:|:----:|:----:|:----:|:------------:|
@@ -74,29 +58,91 @@
 ```
 
 ```python
 import cppe5
 cppe5.download_data()
 ```
 
+## Data Loaders
+
+We provide PyTorch and TensorFlow data loaders in this repository, the
+dataset can also be loaded from [Hugging Face Datasets](https://github.com/huggingface/datasets). To use the data
+loaders in this repository you would need to install the Python package
+first:
+
+```bash
+pip install cppe5
+```
+
+### Hugging Face Datasets
+
+Install the datasets library first:
+
+```bash
+pip install datasets
+```
+
+```py
+from datasets import load_dataset
+
+dataset = load_dataset("cppe-5")
+```
+
+### PyTorch `DataLoader`
+
+A ready to run Google Colab example can be found at [notebooks/pytorch_loader.ipynb](notebooks/pytorch_loader.ipynb).
+
+```py
+import cppe5
+from cppe5.torch import data_loader
+import os
+
+cppe5.download_data()
+os.chdir("..")
+data_loader = cppe5.torch.data_loader() # torch.utils.data.DataLoader
+
+# Fetch all images and annotations
+device = torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")
+
+# DataLoader is iterable over Dataset
+for imgs, annotations in data_loader:
+    imgs = list(img.to(device) for img in imgs)
+    annotations = [{k: v.to(device) for k, v in t.items()} for t in annotations]
+```
+
+### TensorFlow Loader
+
+A ready to run Google Colab example can be found at [notebooks/tensorflow_loader.ipynb](notebooks/tensorflow_loader.ipynb).
+
+```py
+import cppe5
+from cppe5.tensorflow import data_loader
+
+cppe5.download_tfrecords()
+os.chdir("..")
+
+dataset = cppe5.tensorflow.data_loader() # tf.data.Dataset
+iter(dataset).next()
+```
+
 ## Labels
 
 The dataset contains the following labels:
 
 | Label | Description |
 |:----:|:-------------|
 | 1 | Coverall |
 | 2 | Face_Shield |
 | 3 | Gloves |
 | 4 | Goggles |
 | 5 | Mask |
 
 ## Model Zoo
 
-More about the pre-trained models could be found in [MODEL_ZOO.md](MODEL_ZOO.md)
+More information about the pre-trained models (like modlel complexity or FPS benchmark) could be found in [MODEL_ZOO.md](MODEL_ZOO.md)
 and [LITE_MODEL_ZOO.md](LITE_MODEL_ZOO.md) includes models ready for deployment
 on mobile and edge devices.
 
 ### Baseline Models
 
 This section contains the baseline models that are trained on the CPPE-5 dataset
 . More information about how these are trained could be found in the original
@@ -110,15 +156,14 @@
 
 ### SoTA Models
 
 This section contains the SoTA models that are trained on the CPPE-5 dataset
 . More information about how these are trained could be found in the original
 paper and the config files.
 
-
 |           Method           | AP<sup>box</sup> | AP<sub>50</sub><sup>box</sup> | AP<sub>75</sub><sup>box</sup> | AP<sub>S</sub><sup>box</sup> | AP<sub>M</sub><sup>box</sup> | AP<sub>L</sub><sup>box</sup> | Configs | TensorBoard.dev                                                      | PyTorch model                                                                                                                                  | TensorFlow model                                                                               |
 |:--------------------------:|:----------:|:-----------------:|:-----------------:|:----------------:|:----------------:|:----------------:|:------------:|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------:|
 |         RepPoints          |    43.0    |        75.9       |        40.1       |       27.3       |       36.7       |       48.0       | [config](configs/reppoints_moment_r50_fpn_gn_2x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/Co6JQVe1RDmxgbMx4gD0Qg/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/reppoints/reppoints_moment_r50_fpn_gn_2x_coco-18beef36.pth)                      |                                                -                                               |
 |        Sparse RCNN         |    44.0    |        69.6       |        44.6       |       30.0       |       30.6       |       54.7       | [config](configs/sparse_rcnn_r101_fpn_300_proposals_crop_mstrain_480-800_3x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/se3w7zQ7SlyE6T8q59P79w/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/sparse_rcnn/sparse_rcnn_r101_fpn_300_proposals_crop_mstrain_480-800_3x_coco.pth) |                                                -                                               |
 |            FCOS            |    44.4    |        79.5       |        45.9       |       36.7       |       39.2       |       51.7       | [config](configs/fcos_r101_caffe_fpn_gn-head_mstrain_640-800_2x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/O343s1kRQIKTqs508jESDA/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/fcos/fcos_r101_caffe_fpn_gn-head_mstrain_640-800_2x_coco-031dc428.pth)           | [bucket](https://storage.googleapis.com/cppe-5/trained_models/fcos/tf_fcos.tar.gz)             |
 |         Grid RCNN          |    47.5    |        77.9       |        50.6       |       43.4       |       37.2       |       54.4       | [config](configs/grid_rcnn_x101_64x4d_fpn_gn-head_2x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/fgGkJ4IBSZmDQj1QEKgXqA/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/grid_rcnn/grid_rcnn_x101_64x4d_fpn_gn-head_2x_coco-65319c19.pth)                 |                                                -                                               |
 |      Deformable DETR       |    48.0    |        76.9       |        52.8       |       36.4       |       35.2       |       53.9       | [config](configs/deformable_detr_refine_r50_16x2_50e_coco.py) | [tb.dev](https://tensorboard.dev/experiment/uq80boznQY2iJVhWSXAKTw/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/deformable_detr/deformable_detr_refine_r50_16x2_50e-d36a2db1.pth)                |                                                -                                               |
@@ -160,22 +205,41 @@
 
 - [visualize.ipynb](notebooks/visualize.ipynb) <a href="https://colab.research.google.com/github/Rishit-dagli/CPPE-Dataset/blob/main/notebooks/visualize.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 In this notebook, we will visualize the CPPE-5 dataset, which could be really helpful to see some sample images and annotations from the dataset.
 
 ## Citation
 
-If you use this dataset, please cite the following paper:
+If you use this work, please cite the following paper:
+
+**BibTeX:**
+
+```bibtex
+@misc{dagli2021cppe5,
+      title={CPPE-5: Medical Personal Protective Equipment Dataset}, 
+      author={Rishit Dagli and Ali Mustufa Shaikh},
+      year={2021},
+      eprint={2112.09569},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+```
 
-[WIP]
+**MLA:**
+
+```
+Dagli, Rishit, and Ali Mustufa Shaikh. ‘CPPE-5: Medical Personal Protective Equipment Dataset’. ArXiv:2112.09569 [Cs], Dec. 2021. arXiv.org, http://arxiv.org/abs/2112.09569.
+```
+
+## Acknoweldgements
+
+The authors would like to thank Google for supporting this work by providing Google Cloud credits. The authors would also like to thank Google TPU Research Cloud (TRC) program for providing access to TPUs. The authors are also grateful to Omkar Agrawal for help with verifying the difficult annotations.
 
 ## Want to Contribute 🙋‍♂️?
 
 Awesome! If you want to contribute to this project, you're always welcome! See [Contributing Guidelines](CONTRIBUTING.md). You can also take a look at [open issues](https://github.com/Rishit-dagli/CPPE-Dataset/issues) for getting more information about current or upcoming tasks.
 
 ## Want to discuss? 💬
 
 Have any questions, doubts or want to present your opinions, views? You're always welcome. You can [start discussions](hhttps://github.com/Rishit-dagli/CPPE-Dataset/discussions).
 
 Have you used this work in your paper, blog, experiments, or more please share it with us by making a discussion under the [Show and Tell category](https://github.com/Rishit-dagli/CPPE-Dataset/discussions/categories/show-and-tell).
-
-
```

### Comparing `cppe5-0.1.0/cppe5/tensorflow.py` & `cppe5-0.1.1/cppe5/tensorflow.py`

 * *Files identical despite different names*

### Comparing `cppe5-0.1.0/cppe5/torch.py` & `cppe5-0.1.1/cppe5/torch.py`

 * *Files identical despite different names*

### Comparing `cppe5-0.1.0/cppe5.egg-info/PKG-INFO` & `cppe5-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cppe5
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to easily download, load and work with the CPPE-5 dataset.
 Home-page: https://github.com/Rishit-dagli/CPPE-Dataset
 Author: Rishit Dagli, Ali Mustufa
 Author-email: rishit.dagli@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,30 +24,43 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # CPPE - 5 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2FRishit-dagli%2Fhttps://github.com/Rishit-dagli/CPPE-Dataset)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2FRishit-dagli%2Fhttps://github.com/Rishit-dagli/CPPE-Dataset)
 
 ![GitHub Repo stars](https://img.shields.io/github/stars/Rishit-dagli/CPPE-Dataset?style=social)
+[![arXiv](https://img.shields.io/badge/paper-arXiv:2112.09569-b31b1b.svg?logo=arxiv)](https://arxiv.org/abs/2112.09569)
+[![Models TF Hub](https://img.shields.io/badge/Models-TF%20Hub-orange?style=flat&logo=tensorflow)](https://tfhub.dev/rishit-dagli/collections/cppe5)
+
 ![PyPI](https://img.shields.io/pypi/v/cppe5)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 CPPE - 5 (Medical Personal Protective Equipment) is a new challenging dataset
 with the goal to allow the study of subordinate categorization of medical
 personal protective equipments, which is not possible with other popular data
 sets that focus on broad level categories.
 
+_**Accompanying paper: [CPPE - 5: Medical Personal Protective Equipment Dataset](https://arxiv.org/abs/2112.09569)**_
+
+_**by Rishit Dagli and Ali Mustufa Shaikh.**_
+
 Some features of this dataset are:
 - high quality images and annotations (~4.6 bounding boxes per image)
 - real-life images unlike any current such dataset
 - majority of non-iconic images (allowing easy deployment to real-world environments)
 - \>15 pre-trained models in the model zoo availaible to directly use (also for mobile and edge devices)
 
 ![](media/annotation_type.png)
 
+## Updates
+
+- 06/01/2022 - Many thanks to [@mariosasko](https://github.com/mariosasko) for creating a [Hugging Face Datasets loader](https://huggingface.co/datasets/cppe-5).
+- 05/01/2022 - This paper got featured on Google Research TRC's [publication section](https://sites.research.google/trc/publications/)
+- 20/12/2021 - First public release of the CPPE - 5 dataset on arXiv
+
 ## Get the data
 
 We strongly recommend you use either the downlaoder script or the Python package
 to download the dataset however you could also download and extract it manually.
 
 | Name | Size | Drive | Bucket | MD5 checksum |
 |:----:|:----:|:----:|:----:|:------------:|
@@ -74,29 +85,91 @@
 ```
 
 ```python
 import cppe5
 cppe5.download_data()
 ```
 
+## Data Loaders
+
+We provide PyTorch and TensorFlow data loaders in this repository, the
+dataset can also be loaded from [Hugging Face Datasets](https://github.com/huggingface/datasets). To use the data
+loaders in this repository you would need to install the Python package
+first:
+
+```bash
+pip install cppe5
+```
+
+### Hugging Face Datasets
+
+Install the datasets library first:
+
+```bash
+pip install datasets
+```
+
+```py
+from datasets import load_dataset
+
+dataset = load_dataset("cppe-5")
+```
+
+### PyTorch `DataLoader`
+
+A ready to run Google Colab example can be found at [notebooks/pytorch_loader.ipynb](notebooks/pytorch_loader.ipynb).
+
+```py
+import cppe5
+from cppe5.torch import data_loader
+import os
+
+cppe5.download_data()
+os.chdir("..")
+data_loader = cppe5.torch.data_loader() # torch.utils.data.DataLoader
+
+# Fetch all images and annotations
+device = torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")
+
+# DataLoader is iterable over Dataset
+for imgs, annotations in data_loader:
+    imgs = list(img.to(device) for img in imgs)
+    annotations = [{k: v.to(device) for k, v in t.items()} for t in annotations]
+```
+
+### TensorFlow Loader
+
+A ready to run Google Colab example can be found at [notebooks/tensorflow_loader.ipynb](notebooks/tensorflow_loader.ipynb).
+
+```py
+import cppe5
+from cppe5.tensorflow import data_loader
+
+cppe5.download_tfrecords()
+os.chdir("..")
+
+dataset = cppe5.tensorflow.data_loader() # tf.data.Dataset
+iter(dataset).next()
+```
+
 ## Labels
 
 The dataset contains the following labels:
 
 | Label | Description |
 |:----:|:-------------|
 | 1 | Coverall |
 | 2 | Face_Shield |
 | 3 | Gloves |
 | 4 | Goggles |
 | 5 | Mask |
 
 ## Model Zoo
 
-More about the pre-trained models could be found in [MODEL_ZOO.md](MODEL_ZOO.md)
+More information about the pre-trained models (like modlel complexity or FPS benchmark) could be found in [MODEL_ZOO.md](MODEL_ZOO.md)
 and [LITE_MODEL_ZOO.md](LITE_MODEL_ZOO.md) includes models ready for deployment
 on mobile and edge devices.
 
 ### Baseline Models
 
 This section contains the baseline models that are trained on the CPPE-5 dataset
 . More information about how these are trained could be found in the original
@@ -110,15 +183,14 @@
 
 ### SoTA Models
 
 This section contains the SoTA models that are trained on the CPPE-5 dataset
 . More information about how these are trained could be found in the original
 paper and the config files.
 
-
 |           Method           | AP<sup>box</sup> | AP<sub>50</sub><sup>box</sup> | AP<sub>75</sub><sup>box</sup> | AP<sub>S</sub><sup>box</sup> | AP<sub>M</sub><sup>box</sup> | AP<sub>L</sub><sup>box</sup> | Configs | TensorBoard.dev                                                      | PyTorch model                                                                                                                                  | TensorFlow model                                                                               |
 |:--------------------------:|:----------:|:-----------------:|:-----------------:|:----------------:|:----------------:|:----------------:|:------------:|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------:|
 |         RepPoints          |    43.0    |        75.9       |        40.1       |       27.3       |       36.7       |       48.0       | [config](configs/reppoints_moment_r50_fpn_gn_2x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/Co6JQVe1RDmxgbMx4gD0Qg/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/reppoints/reppoints_moment_r50_fpn_gn_2x_coco-18beef36.pth)                      |                                                -                                               |
 |        Sparse RCNN         |    44.0    |        69.6       |        44.6       |       30.0       |       30.6       |       54.7       | [config](configs/sparse_rcnn_r101_fpn_300_proposals_crop_mstrain_480-800_3x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/se3w7zQ7SlyE6T8q59P79w/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/sparse_rcnn/sparse_rcnn_r101_fpn_300_proposals_crop_mstrain_480-800_3x_coco.pth) |                                                -                                               |
 |            FCOS            |    44.4    |        79.5       |        45.9       |       36.7       |       39.2       |       51.7       | [config](configs/fcos_r101_caffe_fpn_gn-head_mstrain_640-800_2x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/O343s1kRQIKTqs508jESDA/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/fcos/fcos_r101_caffe_fpn_gn-head_mstrain_640-800_2x_coco-031dc428.pth)           | [bucket](https://storage.googleapis.com/cppe-5/trained_models/fcos/tf_fcos.tar.gz)             |
 |         Grid RCNN          |    47.5    |        77.9       |        50.6       |       43.4       |       37.2       |       54.4       | [config](configs/grid_rcnn_x101_64x4d_fpn_gn-head_2x_coco.py) | [tb.dev](https://tensorboard.dev/experiment/fgGkJ4IBSZmDQj1QEKgXqA/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/grid_rcnn/grid_rcnn_x101_64x4d_fpn_gn-head_2x_coco-65319c19.pth)                 |                                                -                                               |
 |      Deformable DETR       |    48.0    |        76.9       |        52.8       |       36.4       |       35.2       |       53.9       | [config](configs/deformable_detr_refine_r50_16x2_50e_coco.py) | [tb.dev](https://tensorboard.dev/experiment/uq80boznQY2iJVhWSXAKTw/) | [bucket](https://storage.googleapis.com/cppe-5/trained_models/deformable_detr/deformable_detr_refine_r50_16x2_50e-d36a2db1.pth)                |                                                -                                               |
@@ -160,22 +232,41 @@
 
 - [visualize.ipynb](notebooks/visualize.ipynb) <a href="https://colab.research.google.com/github/Rishit-dagli/CPPE-Dataset/blob/main/notebooks/visualize.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 In this notebook, we will visualize the CPPE-5 dataset, which could be really helpful to see some sample images and annotations from the dataset.
 
 ## Citation
 
-If you use this dataset, please cite the following paper:
+If you use this work, please cite the following paper:
+
+**BibTeX:**
+
+```bibtex
+@misc{dagli2021cppe5,
+      title={CPPE-5: Medical Personal Protective Equipment Dataset}, 
+      author={Rishit Dagli and Ali Mustufa Shaikh},
+      year={2021},
+      eprint={2112.09569},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+```
 
-[WIP]
+**MLA:**
+
+```
+Dagli, Rishit, and Ali Mustufa Shaikh. ‘CPPE-5: Medical Personal Protective Equipment Dataset’. ArXiv:2112.09569 [Cs], Dec. 2021. arXiv.org, http://arxiv.org/abs/2112.09569.
+```
+
+## Acknoweldgements
+
+The authors would like to thank Google for supporting this work by providing Google Cloud credits. The authors would also like to thank Google TPU Research Cloud (TRC) program for providing access to TPUs. The authors are also grateful to Omkar Agrawal for help with verifying the difficult annotations.
 
 ## Want to Contribute 🙋‍♂️?
 
 Awesome! If you want to contribute to this project, you're always welcome! See [Contributing Guidelines](CONTRIBUTING.md). You can also take a look at [open issues](https://github.com/Rishit-dagli/CPPE-Dataset/issues) for getting more information about current or upcoming tasks.
 
 ## Want to discuss? 💬
 
 Have any questions, doubts or want to present your opinions, views? You're always welcome. You can [start discussions](hhttps://github.com/Rishit-dagli/CPPE-Dataset/discussions).
 
 Have you used this work in your paper, blog, experiments, or more please share it with us by making a discussion under the [Show and Tell category](https://github.com/Rishit-dagli/CPPE-Dataset/discussions/categories/show-and-tell).
-
-
```

### Comparing `cppe5-0.1.0/setup.py` & `cppe5-0.1.1/setup.py`

 * *Files identical despite different names*

