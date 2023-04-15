# Comparing `tmp/frame_semantic_transformer-0.8.1.tar.gz` & `tmp/frame_semantic_transformer-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frame_semantic_transformer-0.8.1.tar", max compression
+gzip compressed data, was "frame_semantic_transformer-0.8.2.tar", max compression
```

## Comparing `frame_semantic_transformer-0.8.1.tar` & `frame_semantic_transformer-0.8.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1069 2023-03-15 01:41:55.153134 frame_semantic_transformer-0.8.1/LICENSE
--rw-r--r--   0        0        0     6379 2023-03-15 01:41:55.153134 frame_semantic_transformer-0.8.1/README.md
--rw-r--r--   0        0        0     8940 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/FrameSemanticTransformer.py
--rw-r--r--   0        0        0      606 2023-03-15 01:41:55.921159 frame_semantic_transformer-0.8.1/frame_semantic_transformer/__init__.py
--rw-r--r--   0        0        0      223 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/constants.py
--rw-r--r--   0        0        0     4969 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/LoaderDataCache.py
--rw-r--r--   0        0        0     3652 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/TaskSampleDataset.py
--rw-r--r--   0        0        0     1203 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/DataAugmentation.py
--rw-r--r--   0        0        0     2148 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py
--rw-r--r--   0        0        0     1946 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py
--rw-r--r--   0        0        0      465 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/LowercaseAugmentation.py
--rw-r--r--   0        0        0     1061 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py
--rw-r--r--   0        0        0     1842 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py
--rw-r--r--   0        0        0     2144 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py
--rw-r--r--   0        0        0     1433 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py
--rw-r--r--   0        0        0      809 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py
--rw-r--r--   0        0        0      932 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/__init__.py
--rw-r--r--   0        0        0      552 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/chain_augmentations.py
--rw-r--r--   0        0        0      267 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/modification_helpers/__init__.py
--rw-r--r--   0        0        0      572 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py
--rw-r--r--   0        0        0     1789 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py
--rw-r--r--   0        0        0     4141 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py
--rw-r--r--   0        0        0     2913 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/data_utils.py
--rw-r--r--   0        0        0     1335 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/frame_types.py
--rw-r--r--   0        0        0     2699 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py
--rw-r--r--   0        0        0     5659 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py
--rw-r--r--   0        0        0      209 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/__init__.py
--rw-r--r--   0        0        0      174 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/ensure_framenet_downloaded.py
--rw-r--r--   0        0        0      279 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/ensure_wordnet_downloaded.py
--rw-r--r--   0        0        0     1235 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py
--rw-r--r--   0        0        0     2582 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/loader.py
--rw-r--r--   0        0        0     1661 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py
--rw-r--r--   0        0        0     6404 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py
--rw-r--r--   0        0        0      209 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/__init__.py
--rw-r--r--   0        0        0      603 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py
--rw-r--r--   0        0        0     1296 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py
--rw-r--r--   0        0        0     2479 2023-03-15 01:41:55.161134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py
--rw-r--r--   0        0        0     2356 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py
--rw-r--r--   0        0        0     1107 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/FrameClassificationSample.py
--rw-r--r--   0        0        0     2202 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/FrameClassificationTask.py
--rw-r--r--   0        0        0      610 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/Task.py
--rw-r--r--   0        0        0      952 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/TaskSample.py
--rw-r--r--   0        0        0     2766 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py
--rw-r--r--   0        0        0      634 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py
--rw-r--r--   0        0        0      685 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/__init__.py
--rw-r--r--   0        0        0     2118 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks_from_annotated_sentences.py
--rw-r--r--   0        0        0     3443 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/predict.py
--rw-r--r--   0        0        0     1038 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/scripts/evaluate.py
--rw-r--r--   0        0        0     1195 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/scripts/train.py
--rw-r--r--   0        0        0     3400 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/ModelRecorder.py
--rw-r--r--   0        0        0     1773 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/TrainingDataModule.py
--rw-r--r--   0        0        0     8397 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/TrainingModelWrapper.py
--rw-r--r--   0        0        0      186 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/__init__.py
--rw-r--r--   0        0        0     4714 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/evaluate_batch.py
--rw-r--r--   0        0        0     1454 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/evaluate_best_val_models.py
--rw-r--r--   0        0        0     3388 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/evaluate_model.py
--rw-r--r--   0        0        0     1925 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/find_best_val_model_paths.py
--rw-r--r--   0        0        0     5400 2023-03-15 01:41:55.165134 frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/train.py
--rw-r--r--   0        0        0      982 2023-03-15 01:41:55.921159 frame_semantic_transformer-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     7384 1970-01-01 00:00:00.000000 frame_semantic_transformer-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 11:31:48.764542 frame_semantic_transformer-0.8.2/LICENSE
+-rw-r--r--   0        0        0     6650 2023-04-15 11:31:48.764542 frame_semantic_transformer-0.8.2/README.md
+-rw-r--r--   0        0        0     8667 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/FrameSemanticTransformer.py
+-rw-r--r--   0        0        0      606 2023-04-15 11:31:49.472555 frame_semantic_transformer-0.8.2/frame_semantic_transformer/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/constants.py
+-rw-r--r--   0        0        0     4969 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/LoaderDataCache.py
+-rw-r--r--   0        0        0     3652 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/TaskSampleDataset.py
+-rw-r--r--   0        0        0     1203 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DataAugmentation.py
+-rw-r--r--   0        0        0     2148 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py
+-rw-r--r--   0        0        0     1946 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py
+-rw-r--r--   0        0        0      465 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/LowercaseAugmentation.py
+-rw-r--r--   0        0        0     1061 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py
+-rw-r--r--   0        0        0     1842 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py
+-rw-r--r--   0        0        0     2144 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py
+-rw-r--r--   0        0        0     1433 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py
+-rw-r--r--   0        0        0      809 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py
+-rw-r--r--   0        0        0      932 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/chain_augmentations.py
+-rw-r--r--   0        0        0      267 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/__init__.py
+-rw-r--r--   0        0        0      572 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py
+-rw-r--r--   0        0        0     1789 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py
+-rw-r--r--   0        0        0     4141 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py
+-rw-r--r--   0        0        0     4518 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/data_utils.py
+-rw-r--r--   0        0        0     1335 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/frame_types.py
+-rw-r--r--   0        0        0     2699 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py
+-rw-r--r--   0        0        0     5659 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py
+-rw-r--r--   0        0        0      209 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/__init__.py
+-rw-r--r--   0        0        0      174 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/ensure_framenet_downloaded.py
+-rw-r--r--   0        0        0      279 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/ensure_wordnet_downloaded.py
+-rw-r--r--   0        0        0     1235 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py
+-rw-r--r--   0        0        0     2582 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/loader.py
+-rw-r--r--   0        0        0     1661 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py
+-rw-r--r--   0        0        0     6404 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py
+-rw-r--r--   0        0        0      209 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/__init__.py
+-rw-r--r--   0        0        0      603 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py
+-rw-r--r--   0        0        0     1296 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py
+-rw-r--r--   0        0        0     2479 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py
+-rw-r--r--   0        0        0     2356 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py
+-rw-r--r--   0        0        0     1107 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationSample.py
+-rw-r--r--   0        0        0     2202 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationTask.py
+-rw-r--r--   0        0        0      610 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/Task.py
+-rw-r--r--   0        0        0      952 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TaskSample.py
+-rw-r--r--   0        0        0     2766 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py
+-rw-r--r--   0        0        0      634 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py
+-rw-r--r--   0        0        0      685 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/__init__.py
+-rw-r--r--   0        0        0     2118 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks_from_annotated_sentences.py
+-rw-r--r--   0        0        0     3443 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/predict.py
+-rw-r--r--   0        0        0     1038 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/evaluate.py
+-rw-r--r--   0        0        0     1195 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/train.py
+-rw-r--r--   0        0        0     3400 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/ModelRecorder.py
+-rw-r--r--   0        0        0     1773 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingDataModule.py
+-rw-r--r--   0        0        0     8397 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingModelWrapper.py
+-rw-r--r--   0        0        0      186 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/__init__.py
+-rw-r--r--   0        0        0     4714 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_batch.py
+-rw-r--r--   0        0        0     1454 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_best_val_models.py
+-rw-r--r--   0        0        0     3388 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_model.py
+-rw-r--r--   0        0        0     1925 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/find_best_val_model_paths.py
+-rw-r--r--   0        0        0     5400 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/train.py
+-rw-r--r--   0        0        0      982 2023-04-15 11:31:49.472555 frame_semantic_transformer-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     7655 1970-01-01 00:00:00.000000 frame_semantic_transformer-0.8.2/PKG-INFO
```

### Comparing `frame_semantic_transformer-0.8.1/LICENSE` & `frame_semantic_transformer-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/README.md` & `frame_semantic_transformer-0.8.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,7 +98,19 @@
 Any contributions to improve this project are welcome! Please open an issue or pull request in this repo with any bugfixes / changes / improvements you have!
 
 This project uses [Black](https://github.com/psf/black) for code formatting, [Flake8](https://flake8.pycqa.org/en/latest/) for linting, and [Pytest](https://docs.pytest.org/) for tests. Make sure any changes you submit pass these code checks in your PR. If you have trouble getting these to run feel free to open a pull-request regardless and we can discuss further in the PR.
 
 ## License
 
 The code contained in this repo is released under a MIT license, however the pretrained models are released under an Apache 2.0 license in accordance with FrameNet training data and HuggingFace's T5 base models.
+
+## Citation
+
+If you use Frame semantic transformer in your work, please cite the following:
+```bibtex
+@article{chanin2023opensource,
+  title={Open-source Frame Semantic Parsing},
+  author={Chanin, David},
+  journal={arXiv preprint arXiv:2303.12788},
+  year={2023}
+}
+```
```

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/FrameSemanticTransformer.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/FrameSemanticTransformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -164,31 +164,31 @@
             )
         return results
 
     def detect_frames_bulk(self, sentences: Iterable[str]) -> list[DetectFramesResult]:
         tasks_queue: list[Task] = []
         # slowly build up results from each task as they complete
         results_acc: ResultsAccumulator = defaultdict(dict)
-        # T5 doesn't necessarily have to output the original sentence, even though it's supposed to
-        # This map just keeps track of the original sentence for each output sentence so we can match them up
-        parsed_sentences_map: dict[str, str] = {}
         for sentence in sentences:
             tasks_queue.append(TriggerIdentificationTask(text=sentence))
         while len(tasks_queue) > 0:
             batch = tasks_queue[: self.batch_size]
             tasks_queue = tasks_queue[self.batch_size :]
             batch_results = self._batch_predict([task.get_input() for task in batch])
             for task, preds in zip(
                 batch, chunk_list(batch_results, self.predictions_per_sample)
             ):
                 if isinstance(task, TriggerIdentificationTask):
                     # first identify triggers
-                    result = task.parse_output(preds, self.loader_cache)
-                    parsed_sent, trigger_locs = marked_string_to_locs(result)
-                    parsed_sentences_map[task.text] = parsed_sent
+                    text_with_triggers_marked = task.parse_output(
+                        preds, self.loader_cache
+                    )
+                    trigger_locs = marked_string_to_locs(
+                        task.text, text_with_triggers_marked
+                    )
                     for trigger_loc in trigger_locs:
                         tasks_queue.append(
                             FrameClassificationTask(
                                 text=task.text,
                                 trigger_loc=trigger_loc,
                                 loader_cache=self.loader_cache,
                             )
@@ -211,15 +211,14 @@
                     frame_element_tuples = task.parse_output(preds, self.loader_cache)
                     results_acc[task.text][task.trigger_loc][1].update(
                         frame_element_tuples
                     )
         results_map = self._collate_results(results_acc)
         results = []
         for sentence in sentences:
-            mapped_sentence = parsed_sentences_map[sentence]
-            if mapped_sentence in results_map:
-                results.append(results_map[mapped_sentence])
+            if sentence in results_map:
+                results.append(results_map[sentence])
             else:
                 results.append(
                     DetectFramesResult(sentence, trigger_locations=[], frames=[])
                 )
         return results
```

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/__init__.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 from .FrameSemanticTransformer import (
     FrameSemanticTransformer,
     DetectFramesResult,
     FrameElementResult,
     FrameResult,
 )
```

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/LoaderDataCache.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/LoaderDataCache.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/TaskSampleDataset.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/TaskSampleDataset.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/DataAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/__init__.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/chain_augmentations.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/chain_augmentations.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/frame_types.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/frame_types.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/loader.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/FrameClassificationSample.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/FrameClassificationTask.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationTask.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/Task.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/Task.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/TaskSample.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TaskSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks/__init__.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/data/tasks_from_annotated_sentences.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks_from_annotated_sentences.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/predict.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/predict.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/scripts/evaluate.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/scripts/train.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/train.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/ModelRecorder.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/ModelRecorder.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/TrainingDataModule.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingDataModule.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/TrainingModelWrapper.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingModelWrapper.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/evaluate_batch.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_batch.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/evaluate_best_val_models.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_best_val_models.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/evaluate_model.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/find_best_val_model_paths.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/find_best_val_model_paths.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/frame_semantic_transformer/training/train.py` & `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/train.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.1/pyproject.toml` & `frame_semantic_transformer-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frame-semantic-transformer"
-version = "0.8.1"
+version = "0.8.2"
 description = "Frame Semantic Parser based on T5 and FrameNet"
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chanind/frame-semantic-transformer"
 authors = ["David Chanin <chanindav@gmail.com>"]
 
 [tool.poetry.dependencies]
```

### Comparing `frame_semantic_transformer-0.8.1/PKG-INFO` & `frame_semantic_transformer-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frame-semantic-transformer
-Version: 0.8.1
+Version: 0.8.2
 Summary: Frame Semantic Parser based on T5 and FrameNet
 Home-page: https://github.com/chanind/frame-semantic-transformer
 License: MIT
 Author: David Chanin
 Author-email: chanindav@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -124,7 +124,19 @@
 
 This project uses [Black](https://github.com/psf/black) for code formatting, [Flake8](https://flake8.pycqa.org/en/latest/) for linting, and [Pytest](https://docs.pytest.org/) for tests. Make sure any changes you submit pass these code checks in your PR. If you have trouble getting these to run feel free to open a pull-request regardless and we can discuss further in the PR.
 
 ## License
 
 The code contained in this repo is released under a MIT license, however the pretrained models are released under an Apache 2.0 license in accordance with FrameNet training data and HuggingFace's T5 base models.
 
+## Citation
+
+If you use Frame semantic transformer in your work, please cite the following:
+```bibtex
+@article{chanin2023opensource,
+  title={Open-source Frame Semantic Parsing},
+  author={Chanin, David},
+  journal={arXiv preprint arXiv:2303.12788},
+  year={2023}
+}
+```
+
```

