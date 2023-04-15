# Comparing `tmp/clarinpl-embeddings-0.0.1rc8.tar.gz` & `tmp/clarinpl-embeddings-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarinpl-embeddings-0.0.1rc8.tar", max compression
+gzip compressed data, was "clarinpl-embeddings-0.0.1rc9.tar", max compression
```

## Comparing `clarinpl-embeddings-0.0.1rc8.tar` & `clarinpl-embeddings-0.0.1rc9.tar`

### file list

```diff
@@ -1,46 +1,57 @@
--rw-r--r--   0        0        0     1066 2021-05-10 09:49:10.016390 clarinpl-embeddings-0.0.1rc8/LICENSE
--rw-r--r--   0        0        0       22 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/__init__.py
--rw-r--r--   0        0        0      351 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/data/DataLoader.py
--rw-r--r--   0        0        0      162 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/data/Dataset.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/data/__init__.py
--rw-r--r--   0        0        0      295 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/embedding/Embedding.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/embedding/__init__.py
--rw-r--r--   0        0        0      298 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/evaluator/Evaluator.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/evaluator/__init__.py
--rw-r--r--   0        0        0      679 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/model/BaseModel.py
--rw-r--r--   0        0        0      291 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/model/Model.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/model/__init__.py
--rw-r--r--   0        0        0      201 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/pipeline/Pipeline.py
--rw-r--r--   0        0        0     4154 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/pipeline/PipelineBuilder.py
--rw-r--r--   0        0        0     1535 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/pipeline/StandardPipeline.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/pipeline/__init__.py
--rw-r--r--   0        0        0      289 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/task/Task.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/task/__init__.py
--rw-r--r--   0        0        0      304 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/transformation/Transformation.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/embeddings/transformation/__init__.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/__init__.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/data/__init__.py
--rw-r--r--   0        0        0       77 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/data/io.py
--rw-r--r--   0        0        0      109 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/datasets/__init__.py
--rw-r--r--   0        0        0      189 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/datasets/base.py
--rw-r--r--   0        0        0     5562 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/datasets/hugging_face_dataset.py
--rw-r--r--   0        0        0     2126 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/datasets/promises_elections_twitter.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/datasets/utils/__init__.py
--rw-r--r--   0        0        0      715 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/datasets/utils/converters.py
--rw-r--r--   0        0        0     2869 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/datasets/utils/misc.py
--rw-r--r--   0        0        0      265 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/defaults.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/__init__.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/language_models/__init__.py
--rw-r--r--   0        0        0      352 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/language_models/long_former.py
--rw-r--r--   0        0        0      388 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/language_models/roberta.py
--rw-r--r--   0        0        0     1389 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/scripts/evaluate_document_classification.py
--rw-r--r--   0        0        0     1993 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/scripts/evaluate_sequence_tagging.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/tasks/__init__.py
--rw-r--r--   0        0        0     1709 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/tasks/base_task.py
--rw-r--r--   0        0        0     1813 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/tasks/sequence_tagging.py
--rw-r--r--   0        0        0     3480 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/embeddings/tasks/text_classification.py
--rw-r--r--   0        0        0        0 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/utils/__init__.py
--rw-r--r--   0        0        0      541 2021-05-10 09:49:10.020390 clarinpl-embeddings-0.0.1rc8/experimental/utils/loggers.py
--rw-r--r--   0        0        0     1135 2021-05-10 09:50:33.053382 clarinpl-embeddings-0.0.1rc8/pyproject.toml
--rw-r--r--   0        0        0     1334 2021-05-10 09:50:33.609738 clarinpl-embeddings-0.0.1rc8/setup.py
--rw-r--r--   0        0        0      896 2021-05-10 09:50:33.610033 clarinpl-embeddings-0.0.1rc8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/LICENSE
+-rw-r--r--   0        0        0       22 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/data/__init__.py
+-rw-r--r--   0        0        0      305 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/data/data_loader.py
+-rw-r--r--   0        0        0      183 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/data/dataset.py
+-rw-r--r--   0        0        0      565 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/data/hugging_face_data_loader.py
+-rw-r--r--   0        0        0      340 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/data/hugging_face_dataset.py
+-rw-r--r--   0        0        0       77 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/data/io.py
+-rw-r--r--   0        0        0      265 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/defaults.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/embedding/__init__.py
+-rw-r--r--   0        0        0      295 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/embedding/embedding.py
+-rw-r--r--   0        0        0     1196 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/embedding/flair_embedding.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/evaluator/__init__.py
+-rw-r--r--   0        0        0      298 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/evaluator/evaluator.py
+-rw-r--r--   0        0        0      625 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/evaluator/metrics_evaluator.py
+-rw-r--r--   0        0        0      350 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/evaluator/sequence_tagging_evaluator.py
+-rw-r--r--   0        0        0      530 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/evaluator/text_classification_evaluator.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/model/__init__.py
+-rw-r--r--   0        0        0      679 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/model/base_model.py
+-rw-r--r--   0        0        0      689 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/model/flair_model.py
+-rw-r--r--   0        0        0      291 2021-06-18 16:15:08.314570 clarinpl-embeddings-0.0.1rc9/embeddings/model/model.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/__init__.py
+-rw-r--r--   0        0        0     1606 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/hugging_face_classification.py
+-rw-r--r--   0        0        0     1608 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/hugging_face_sequence_tagging.py
+-rw-r--r--   0        0        0      201 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/pipeline.py
+-rw-r--r--   0        0        0     4093 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/pipeline_builder.py
+-rw-r--r--   0        0        0     1475 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/standard_pipeline.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/task/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/task/flair_task/__init__.py
+-rw-r--r--   0        0        0     2821 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/task/flair_task/flair_task.py
+-rw-r--r--   0        0        0     2108 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/task/flair_task/sequence_tagging.py
+-rw-r--r--   0        0        0     2013 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/task/flair_task/text_classification.py
+-rw-r--r--   0        0        0      289 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/task/task.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/transformation/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/transformation/flair_transformation/__init__.py
+-rw-r--r--   0        0        0     1377 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/transformation/flair_transformation/classification_corpus_transformation.py
+-rw-r--r--   0        0        0     2903 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/transformation/flair_transformation/column_corpus_transformation.py
+-rw-r--r--   0        0        0     3452 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/transformation/flair_transformation/corpus_transformation.py
+-rw-r--r--   0        0        0      816 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/transformation/flair_transformation/downsample_corpus_transformation.py
+-rw-r--r--   0        0        0      968 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/transformation/transformation.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/utils/__init__.py
+-rw-r--r--   0        0        0      541 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/embeddings/utils/loggers.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/__init__.py
+-rw-r--r--   0        0        0      109 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/datasets/__init__.py
+-rw-r--r--   0        0        0      189 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/datasets/base.py
+-rw-r--r--   0        0        0     2124 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/datasets/promises_elections_twitter.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/datasets/utils/__init__.py
+-rw-r--r--   0        0        0      715 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/datasets/utils/converters.py
+-rw-r--r--   0        0        0     2867 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/datasets/utils/misc.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/embeddings/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/embeddings/language_models/__init__.py
+-rw-r--r--   0        0        0      352 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/embeddings/language_models/long_former.py
+-rw-r--r--   0        0        0      388 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/embeddings/language_models/roberta.py
+-rw-r--r--   0        0        0     1941 2021-06-18 16:15:08.318570 clarinpl-embeddings-0.0.1rc9/experimental/embeddings/scripts/evaluate_promises_sequence_tagging.py
+-rw-r--r--   0        0        0     1154 2021-06-18 16:16:35.495305 clarinpl-embeddings-0.0.1rc9/pyproject.toml
+-rw-r--r--   0        0        0     1384 2021-06-18 16:16:36.061709 clarinpl-embeddings-0.0.1rc9/setup.py
+-rw-r--r--   0        0        0      936 2021-06-18 16:16:36.061998 clarinpl-embeddings-0.0.1rc9/PKG-INFO
```

### Comparing `clarinpl-embeddings-0.0.1rc8/LICENSE` & `clarinpl-embeddings-0.0.1rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `clarinpl-embeddings-0.0.1rc8/embeddings/model/BaseModel.py` & `clarinpl-embeddings-0.0.1rc9/embeddings/model/base_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from typing import TypeVar, Generic
-from embeddings.model.Model import Model
-from embeddings.task.Task import Task
-from embeddings.embedding.Embedding import Embedding
+from embeddings.model.model import Model
+from embeddings.task.task import Task
+from embeddings.embedding.embedding import Embedding
 
 Input = TypeVar("Input")
 EmbeddingResult = TypeVar("EmbeddingResult")
 Output = TypeVar("Output")
 
 
 class BaseModel(Model[Input, Output], Generic[Input, EmbeddingResult, Output]):
```

### Comparing `clarinpl-embeddings-0.0.1rc8/embeddings/pipeline/PipelineBuilder.py` & `clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/pipeline_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import TypeVar, Generic
 from abc import ABC
-from embeddings.pipeline.Pipeline import Pipeline
-from embeddings.pipeline.StandardPipeline import StandardPipeline
-from embeddings.data.Dataset import Dataset
-from embeddings.data.DataLoader import DataLoader
-from embeddings.transformation.Transformation import Transformation
-from embeddings.model.Model import Model
-from embeddings.task.Task import Task
-from embeddings.evaluator.Evaluator import Evaluator
 from typing import Optional
-from copy import deepcopy
+from typing import TypeVar, Generic
+
+from embeddings.data.data_loader import DataLoader
+from embeddings.data.dataset import Dataset
+from embeddings.evaluator.evaluator import Evaluator
+from embeddings.model.model import Model
+from embeddings.pipeline.pipeline import Pipeline
+from embeddings.pipeline.standard_pipeline import StandardPipeline
+from embeddings.transformation.transformation import Transformation
 
 Data = TypeVar("Data")
 CreationData = TypeVar("CreationData")
 LoaderResult = TypeVar("LoaderResult")
 CreationLoaderResult = TypeVar("CreationLoaderResult")
 TransformationResult = TypeVar("TransformationResult")
 CreationTransformationResult = TypeVar("CreationTransformationResult")
```

### Comparing `clarinpl-embeddings-0.0.1rc8/embeddings/pipeline/StandardPipeline.py` & `clarinpl-embeddings-0.0.1rc9/embeddings/pipeline/standard_pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from typing import TypeVar, Generic
-from abc import ABC
-from embeddings.pipeline.Pipeline import Pipeline
-from embeddings.data.Dataset import Dataset
-from embeddings.data.DataLoader import DataLoader
-from embeddings.transformation.Transformation import Transformation
-from embeddings.model.Model import Model
-from embeddings.task.Task import Task
-from embeddings.evaluator.Evaluator import Evaluator
+
+from embeddings.data.data_loader import DataLoader
+from embeddings.data.dataset import Dataset
+from embeddings.evaluator.evaluator import Evaluator
+from embeddings.model.model import Model
+from embeddings.pipeline.pipeline import Pipeline
+from embeddings.transformation.transformation import Transformation
 
 EvaluationResult = TypeVar("EvaluationResult")
 Data = TypeVar("Data")
 LoaderResult = TypeVar("LoaderResult")
 TransformationResult = TypeVar("TransformationResult")
 ModelResult = TypeVar("ModelResult")
 
 
 class StandardPipeline(
     Pipeline[EvaluationResult],
     Generic[Data, LoaderResult, TransformationResult, ModelResult, EvaluationResult],
 ):
     def __init__(
         self,
-        data_set: Dataset[Data],
+        dataset: Dataset[Data],
         data_loader: DataLoader[Data, LoaderResult],
         transformation: Transformation[LoaderResult, TransformationResult],
         model: Model[TransformationResult, ModelResult],
         evaluator: Evaluator[ModelResult, EvaluationResult],
     ) -> None:
-        self.data_set = data_set
+        self.dataset = dataset
         self.data_loader = data_loader
         self.transformation = transformation
         self.model = model
         self.evaluator = evaluator
 
     def run(self) -> EvaluationResult:
-        loaded_data = self.data_loader.load(self.data_set)
+        loaded_data = self.data_loader.load(self.dataset)
         transformed_data = self.transformation.transform(loaded_data)
         model_result = self.model.model(transformed_data)
         return self.evaluator.evaluate(model_result)
```

### Comparing `clarinpl-embeddings-0.0.1rc8/experimental/datasets/promises_elections_twitter.py` & `clarinpl-embeddings-0.0.1rc9/experimental/datasets/promises_elections_twitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import Optional
 
 import srsly
-from experimental.data.io import T_path
+from embeddings.data.io import T_path
 from experimental.datasets.base import BaseDataset
 from experimental.datasets.utils.converters import convert_spacy_jsonl_to_connl_bilou
 from experimental.datasets.utils.misc import (
     split_train_test_dev,
     DatasetDownloader,
     all_files_exists,
 )
```

### Comparing `clarinpl-embeddings-0.0.1rc8/experimental/datasets/utils/converters.py` & `clarinpl-embeddings-0.0.1rc9/experimental/datasets/utils/converters.py`

 * *Files identical despite different names*

### Comparing `clarinpl-embeddings-0.0.1rc8/experimental/datasets/utils/misc.py` & `clarinpl-embeddings-0.0.1rc9/experimental/datasets/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tempfile import NamedTemporaryFile
 from typing import List, Any, Dict, Tuple, Optional
 
 import requests
 from sklearn.model_selection import train_test_split
 from tqdm.auto import tqdm
 
-from experimental.data.io import T_path
+from embeddings.data.io import T_path
 
 
 def split_train_test_dev(data: List[Any]) -> Dict[str, List[Any]]:
     train, test = train_test_split(data, test_size=0.4, random_state=1)
     dev, test = train_test_split(test, test_size=0.5, random_state=1)
     return {"train": train, "dev": dev, "test": test}
```

### Comparing `clarinpl-embeddings-0.0.1rc8/experimental/embeddings/scripts/evaluate_sequence_tagging.py` & `clarinpl-embeddings-0.0.1rc9/experimental/embeddings/scripts/evaluate_promises_sequence_tagging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import pickle
 from pathlib import Path
 from typing import Optional
 
 import experimental.datasets.utils.misc
 import flair
 import torch
 import typer
-from experimental.defaults import RESULTS_PATH
-from experimental.embeddings.tasks import sequence_tagging as st
+from embeddings.defaults import RESULTS_PATH
 from flair.embeddings import TransformerWordEmbeddings
 
 
 app = typer.Typer()
 
 
 def setup(device: str) -> None:
@@ -42,23 +40,23 @@
 
     test_sentences = corpus.test.sentences.copy()
 
     print("Loading embeddings...")
     embeddings = TransformerWordEmbeddings(embedding)
 
     print("Training model...")
-    tagger = st.FlairSequenceTagger(
-        embeddings=embeddings,
-        hidden_dim=256,
-        tag_dictionary=tag_dictionary,
-        output_path=str(out_dir),
-    )
-
-    training_log = tagger.fit(corpus)
-    evaluation_log = tagger.evaluate(test_sentences)
-    with out_dir.joinpath("results.pkl").open(mode="wb") as f:
-        pickle.dump(obj={"training_log": training_log, "evaluation_log": evaluation_log}, file=f)
-
-    print("Done!", training_log)
+    # tagger = FlairSequenceTagger(
+    #     embeddings=embeddings,
+    #     hidden_dim=256,
+    #     tag_dictionary=tag_dictionary,
+    #     output_path=str(out_dir),
+    # )
+    #
+    # training_log = tagger.fit(corpus)
+    # evaluation_log = tagger.evaluate(test_sentences)
+    # with out_dir.joinpath("results.pkl").open(mode="wb") as f:
+    #     pickle.dump(obj={"training_log": training_log, "evaluation_log": evaluation_log}, file=f)
+    #
+    # print("Done!", training_log)
 
 
 typer.run(evaluate_sequence_tagging)
```

### Comparing `clarinpl-embeddings-0.0.1rc8/experimental/utils/loggers.py` & `clarinpl-embeddings-0.0.1rc9/embeddings/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `clarinpl-embeddings-0.0.1rc8/pyproject.toml` & `clarinpl-embeddings-0.0.1rc9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clarinpl-embeddings"
-version = "0.0.1rc8"
+version = "0.0.1rc9"
 description = ""
 license="MIT"
 authors = [
     "Roman Bartusiak <riomus@gmail.com>",
     "Łukasz Augustyniak <luk.augustyniak@gmail.com>",
     "Albert Sawczyn <albertsawczyn@gmail.com>",
     "Kamil Tagowski <kamil.tagowski@gmail.com>"
@@ -26,14 +26,15 @@
 scikit-learn = "^0.24.1"
 srsly = "^2.4.0"
 datasets = "^1.6.1"
 Pillow = "^8.2.0"
 tensorboard = "^2.4.1"
 typer = "^0.3.2"
 spacy = "^3.0.0"
+seqeval = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 mypy = "^0.812"
 black = "^20.8b1"
 typing-extensions = "^3.7.4"
```

### Comparing `clarinpl-embeddings-0.0.1rc8/setup.py` & `clarinpl-embeddings-0.0.1rc9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,44 +5,45 @@
 ['embeddings',
  'embeddings.data',
  'embeddings.embedding',
  'embeddings.evaluator',
  'embeddings.model',
  'embeddings.pipeline',
  'embeddings.task',
+ 'embeddings.task.flair_task',
  'embeddings.transformation',
+ 'embeddings.transformation.flair_transformation',
+ 'embeddings.utils',
  'experimental',
- 'experimental.data',
  'experimental.datasets',
  'experimental.datasets.utils',
  'experimental.embeddings',
  'experimental.embeddings.language_models',
- 'experimental.embeddings.scripts',
- 'experimental.embeddings.tasks',
- 'experimental.utils']
+ 'experimental.embeddings.scripts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=8.2.0,<9.0.0',
  'datasets>=1.6.1,<2.0.0',
  'flair>=0.8.0,<0.9.0',
  'requests>=2.25.1,<3.0.0',
  'scikit-learn>=0.24.1,<0.25.0',
+ 'seqeval>=1.2.2,<2.0.0',
  'spacy>=3.0.0,<4.0.0',
  'srsly>=2.4.0,<3.0.0',
  'tensorboard>=2.4.1,<3.0.0',
  'torch>=1.8.0,<2.0.0',
  'transformers>=4.4.2,<5.0.0',
  'typer>=0.3.2,<0.4.0']
 
 setup_kwargs = {
     'name': 'clarinpl-embeddings',
-    'version': '0.0.1rc8',
+    'version': '0.0.1rc9',
     'description': '',
     'long_description': None,
     'author': 'Roman Bartusiak',
     'author_email': 'riomus@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/CLARIN-PL/embeddings',
```

### Comparing `clarinpl-embeddings-0.0.1rc8/PKG-INFO` & `clarinpl-embeddings-0.0.1rc9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarinpl-embeddings
-Version: 0.0.1rc8
+Version: 0.0.1rc9
 Summary: 
 Home-page: https://github.com/CLARIN-PL/embeddings
 License: MIT
 Author: Roman Bartusiak
 Author-email: riomus@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,13 +13,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: developer
 Requires-Dist: Pillow (>=8.2.0,<9.0.0)
 Requires-Dist: datasets (>=1.6.1,<2.0.0)
 Requires-Dist: flair (>=0.8.0,<0.9.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: scikit-learn (>=0.24.1,<0.25.0)
+Requires-Dist: seqeval (>=1.2.2,<2.0.0)
 Requires-Dist: spacy (>=3.0.0,<4.0.0)
 Requires-Dist: srsly (>=2.4.0,<3.0.0)
 Requires-Dist: tensorboard (>=2.4.1,<3.0.0)
 Requires-Dist: torch (>=1.8.0,<2.0.0)
 Requires-Dist: transformers (>=4.4.2,<5.0.0)
 Requires-Dist: typer (>=0.3.2,<0.4.0)
```

