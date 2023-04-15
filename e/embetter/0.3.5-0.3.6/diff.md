# Comparing `tmp/embetter-0.3.5.tar.gz` & `tmp/embetter-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/embetter-0.3.5.tar", last modified: Sun Mar 12 15:11:36 2023, max compression
+gzip compressed data, was "dist/embetter-0.3.6.tar", last modified: Sat Apr 15 12:22:07 2023, max compression
```

## Comparing `embetter-0.3.5.tar` & `embetter-0.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7451 2023-03-12 15:11:36.000000 embetter-0.3.5/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6285 2023-03-02 16:27:05.000000 embetter-0.3.5/README.md
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/embetter/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2022-12-05 09:29:24.000000 embetter-0.3.5/embetter/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      326 2022-09-17 15:40:35.000000 embetter-0.3.5/embetter/base.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      742 2022-07-16 12:25:08.000000 embetter-0.3.5/embetter/error.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/embetter/external/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      256 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/external/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2001 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/external/_cohere.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2356 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/external/_openai.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/embetter/finetune/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      401 2023-03-12 14:13:26.000000 embetter-0.3.5/embetter/finetune/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5452 2023-03-12 14:57:16.000000 embetter-0.3.5/embetter/finetune/_contrastive.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2670 2023-03-12 13:44:45.000000 embetter-0.3.5/embetter/finetune/_forward.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1922 2022-12-05 09:29:24.000000 embetter-0.3.5/embetter/grab.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/embetter/text/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      731 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/text/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3794 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/text/_bpemb.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1345 2023-03-02 16:27:05.000000 embetter-0.3.5/embetter/text/_s2v.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2658 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/text/_sbert.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2770 2023-03-02 16:27:05.000000 embetter-0.3.5/embetter/text/_spacy.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/embetter/vision/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      361 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/vision/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/vision/_colorhist.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2205 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/vision/_loader.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2056 2023-02-09 16:06:49.000000 embetter-0.3.5/embetter/vision/_torchvis.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/embetter.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7451 2023-03-12 15:11:35.000000 embetter-0.3.5/embetter.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      784 2023-03-12 15:11:35.000000 embetter-0.3.5/embetter.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-03-12 15:11:35.000000 embetter-0.3.5/embetter.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1022 2023-03-12 15:11:35.000000 embetter-0.3.5/embetter.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       15 2023-03-12 15:11:35.000000 embetter-0.3.5/embetter.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-03-12 15:11:36.000000 embetter-0.3.5/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2595 2023-03-12 15:11:16.000000 embetter-0.3.5/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-03-12 15:11:36.000000 embetter-0.3.5/tests/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2021-10-31 16:15:20.000000 embetter-0.3.5/tests/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2022-12-05 09:29:24.000000 embetter-0.3.5/tests/test_base.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       64 2022-07-16 12:25:08.000000 embetter-0.3.5/tests/test_default.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2023-02-09 16:06:49.000000 embetter-0.3.5/tests/test_docs.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2521 2023-02-09 16:06:49.000000 embetter-0.3.5/tests/test_text.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      871 2022-12-05 09:29:24.000000 embetter-0.3.5/tests/test_vision.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7621 2023-04-15 12:22:07.000000 embetter-0.3.6/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6455 2023-04-01 13:01:08.000000 embetter-0.3.6/README.md
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2022-12-05 09:29:24.000000 embetter-0.3.6/embetter/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      326 2022-09-17 15:40:35.000000 embetter-0.3.6/embetter/base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      742 2022-07-16 12:25:08.000000 embetter-0.3.6/embetter/error.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter/external/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      256 2023-02-09 16:06:49.000000 embetter-0.3.6/embetter/external/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2001 2023-02-09 16:06:49.000000 embetter-0.3.6/embetter/external/_cohere.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2356 2023-03-28 13:55:26.000000 embetter-0.3.6/embetter/external/_openai.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter/finetune/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      401 2023-03-28 13:55:26.000000 embetter-0.3.6/embetter/finetune/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5452 2023-03-28 13:55:26.000000 embetter-0.3.6/embetter/finetune/_contrastive.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2670 2023-03-12 13:44:45.000000 embetter-0.3.6/embetter/finetune/_forward.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2408 2023-04-15 11:19:18.000000 embetter-0.3.6/embetter/grab.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter/text/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2023-03-28 13:55:26.000000 embetter-0.3.6/embetter/text/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3794 2023-02-09 16:06:49.000000 embetter-0.3.6/embetter/text/_bpemb.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1579 2023-03-28 13:55:22.000000 embetter-0.3.6/embetter/text/_s2v.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3143 2023-04-15 12:06:04.000000 embetter-0.3.6/embetter/text/_sbert.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2023-03-28 13:55:22.000000 embetter-0.3.6/embetter/text/_spacy.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter/vision/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      361 2023-02-09 16:06:49.000000 embetter-0.3.6/embetter/vision/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2023-02-09 16:06:49.000000 embetter-0.3.6/embetter/vision/_colorhist.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2205 2023-02-09 16:06:49.000000 embetter-0.3.6/embetter/vision/_loader.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2056 2023-02-09 16:06:49.000000 embetter-0.3.6/embetter/vision/_torchvis.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7621 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      784 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1022 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       15 2023-04-15 12:22:07.000000 embetter-0.3.6/embetter.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-15 12:22:07.000000 embetter-0.3.6/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2595 2023-04-15 11:55:26.000000 embetter-0.3.6/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:22:07.000000 embetter-0.3.6/tests/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2021-10-31 16:15:20.000000 embetter-0.3.6/tests/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2022-12-05 09:29:24.000000 embetter-0.3.6/tests/test_base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       64 2022-07-16 12:25:08.000000 embetter-0.3.6/tests/test_default.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2023-02-09 16:06:49.000000 embetter-0.3.6/tests/test_docs.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2521 2023-02-09 16:06:49.000000 embetter-0.3.6/tests/test_text.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      871 2022-12-05 09:29:24.000000 embetter-0.3.6/tests/test_vision.py
```

### Comparing `embetter-0.3.5/PKG-INFO` & `embetter-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.3.5
+Version: 0.3.6
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
@@ -69,15 +69,15 @@
 # Helpers to grab text or image from pandas column.
 from embetter.grab import ColumnGrabber
 
 # Representations/Helpers for computer vision
 from embetter.vision import ImageLoader, TimmEncoder, ColorHistogramEncoder
 
 # Representations for text
-from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder
+from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder, spaCyEncoder
 
 # Finetuning components 
 from embetter.finetune import ForwardFinetuner
 
 # External embedding providers, typically needs an API key
 from embetter.external import CohereEncoder, OpenAIEncoder
 ```
@@ -159,17 +159,18 @@
 The goal of the library is remain small but to offer a few general tools
 that might help with bulk labelling in particular, but general scikit-learn
 pipelines as well.
 
 |       class               | link                                                 | What it does                                                                                          |
 |:-------------------------:|------------------------------------------------------|--------------------------------------------------------------|
 | `ColumnGrabber`           | [docs](https://koaning.github.io/embetter/API/grab/) | `dataframe` → `ColumnGrabber` → `list with column contents`  |
+| `KeyGrabber`              | [docs](https://koaning.github.io/embetter/API/grab/) | `list of dict` → `KeyGrabber` → `list with column contents`  |
 | `SentenceEncoder`         | [docs](https://koaning.github.io/embetter/API/text/sentence-enc/) | `list of text` → `SentenceEncoder` → `embedding array`  |
 | `Sense2VecEncoder`        | [docs](https://koaning.github.io/embetter/API/text/sense2vec/)    | `list of text` → `Sense2VecEncoder` → `embedding array` |
-| `spaCyEncoder`        | [docs](https://koaning.github.io/embetter/API/text/spacy/)    | `list of text` → `spaCyEncoder` → `embedding array` |
+| `spaCyEncoder`            | [docs](https://koaning.github.io/embetter/API/text/spacy/)    | `list of text` → `spaCyEncoder` → `embedding array` |
 | `BytePairEncoder`         | [docs](https://koaning.github.io/embetter/API/text/bytepair/)    | `list of text` → `BytePairEncoder` → `embedding array` |
 | `ImageLoader`             | [docs](https://koaning.github.io/embetter/API/vision/imageload/) | `list of paths` → `ImageLoader` → `list of PIL images` |
 | `ColorHistogramEncoder`   | [docs](https://koaning.github.io/embetter/API/vision/colorhist/) | `list of PIL images` → `ColorHistogramEncoder` → `embedding array`           |
 | `TimmEncoder`             | [docs](https://koaning.github.io/embetter/API/vision/timm/) | `list of PIL images` → `TimmEncoder` → `embedding array`                     |
 | `ForwardFinetuner`        | [docs](https://koaning.github.io/embetter/API/finetune/feedforward/) | `array + labels` → `ForwardFinetuner` → `finetuned array`                     |
 | `CohereEncoder`           | [docs](https://koaning.github.io/embetter/API/external/cohere/) | `list of text` → `CohereEncoder` → `embedding array`  |
 | `OpenAIEncoder`           | [docs](https://koaning.github.io/embetter/API/external/openai/) | `list of text` → `OpenAIEncoder` → `embedding array`  |
```

### Comparing `embetter-0.3.5/README.md` & `embetter-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # Helpers to grab text or image from pandas column.
 from embetter.grab import ColumnGrabber
 
 # Representations/Helpers for computer vision
 from embetter.vision import ImageLoader, TimmEncoder, ColorHistogramEncoder
 
 # Representations for text
-from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder
+from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder, spaCyEncoder
 
 # Finetuning components 
 from embetter.finetune import ForwardFinetuner
 
 # External embedding providers, typically needs an API key
 from embetter.external import CohereEncoder, OpenAIEncoder
 ```
@@ -127,17 +127,18 @@
 The goal of the library is remain small but to offer a few general tools
 that might help with bulk labelling in particular, but general scikit-learn
 pipelines as well.
 
 |       class               | link                                                 | What it does                                                                                          |
 |:-------------------------:|------------------------------------------------------|--------------------------------------------------------------|
 | `ColumnGrabber`           | [docs](https://koaning.github.io/embetter/API/grab/) | `dataframe` → `ColumnGrabber` → `list with column contents`  |
+| `KeyGrabber`              | [docs](https://koaning.github.io/embetter/API/grab/) | `list of dict` → `KeyGrabber` → `list with column contents`  |
 | `SentenceEncoder`         | [docs](https://koaning.github.io/embetter/API/text/sentence-enc/) | `list of text` → `SentenceEncoder` → `embedding array`  |
 | `Sense2VecEncoder`        | [docs](https://koaning.github.io/embetter/API/text/sense2vec/)    | `list of text` → `Sense2VecEncoder` → `embedding array` |
-| `spaCyEncoder`        | [docs](https://koaning.github.io/embetter/API/text/spacy/)    | `list of text` → `spaCyEncoder` → `embedding array` |
+| `spaCyEncoder`            | [docs](https://koaning.github.io/embetter/API/text/spacy/)    | `list of text` → `spaCyEncoder` → `embedding array` |
 | `BytePairEncoder`         | [docs](https://koaning.github.io/embetter/API/text/bytepair/)    | `list of text` → `BytePairEncoder` → `embedding array` |
 | `ImageLoader`             | [docs](https://koaning.github.io/embetter/API/vision/imageload/) | `list of paths` → `ImageLoader` → `list of PIL images` |
 | `ColorHistogramEncoder`   | [docs](https://koaning.github.io/embetter/API/vision/colorhist/) | `list of PIL images` → `ColorHistogramEncoder` → `embedding array`           |
 | `TimmEncoder`             | [docs](https://koaning.github.io/embetter/API/vision/timm/) | `list of PIL images` → `TimmEncoder` → `embedding array`                     |
 | `ForwardFinetuner`        | [docs](https://koaning.github.io/embetter/API/finetune/feedforward/) | `array + labels` → `ForwardFinetuner` → `finetuned array`                     |
 | `CohereEncoder`           | [docs](https://koaning.github.io/embetter/API/external/cohere/) | `list of text` → `CohereEncoder` → `embedding array`  |
 | `OpenAIEncoder`           | [docs](https://koaning.github.io/embetter/API/external/openai/) | `list of text` → `OpenAIEncoder` → `embedding array`  |
```

### Comparing `embetter-0.3.5/embetter/error.py` & `embetter-0.3.6/embetter/error.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter/external/_cohere.py` & `embetter-0.3.6/embetter/external/_cohere.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter/external/_openai.py` & `embetter-0.3.6/embetter/external/_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,10 +74,10 @@
         self.model = model
         self.batch_size = batch_size
 
     def transform(self, X, y=None):
         """Transforms the text into a numeric representation."""
         result = []
         for b in _batch(X, self.batch_size):
-            resp = openai.Embedding.create(input=X, model=self.model)  # fmt: off
+            resp = openai.Embedding.create(input=b, model=self.model)  # fmt: off
             result.extend([_["embedding"] for _ in resp["data"]])
         return np.array(result)
```

### Comparing `embetter-0.3.5/embetter/finetune/_contrastive.py` & `embetter-0.3.6/embetter/finetune/_contrastive.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter/finetune/_forward.py` & `embetter-0.3.6/embetter/finetune/_forward.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter/grab.py` & `embetter-0.3.6/embetter/grab.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,7 +61,25 @@
         self.colname = colname
 
     def transform(self, X, y=None):
         """
         Takes a column from pandas and returns it as a list.
         """
         return [x for x in X[self.colname]]
+
+
+class KeyGrabber:
+    """
+    Effectively the same thing as the ColumnGrabber, except this is
+    meant to work on generators of dictionaries instead of dataframes.
+    """
+
+    def __init__(self, colname: str) -> None:
+        self.colname = colname
+
+    def transform(self, X, y=None):
+        """
+        Takes a column from pandas and returns it as a list.
+        """
+        if isinstance(X, dict):
+            return X[self.colname]
+        return [x[self.colname] for x in X]
```

### Comparing `embetter-0.3.5/embetter/text/__init__.py` & `embetter-0.3.6/embetter/text/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from embetter.text._s2v import Sense2VecEncoder
 except ModuleNotFoundError:
     Sense2VecEncoder = NotInstalled("Sense2VecEncoder", "sense2vec")
 
 try:
     from embetter.text._bpemb import BytePairEncoder
 except ModuleNotFoundError:
-    Sense2VecEncoder = NotInstalled("BytePairEncoder", "bpemb")
+    BytePairEncoder = NotInstalled("BytePairEncoder", "bpemb")
 
 try:
     from embetter.text._spacy import spaCyEncoder
 except ModuleNotFoundError:
     spaCyEncoder = NotInstalled("spaCyEncoder", "spacy")
```

### Comparing `embetter-0.3.5/embetter/text/_bpemb.py` & `embetter-0.3.6/embetter/text/_bpemb.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter/text/_s2v.py` & `embetter-0.3.6/embetter/text/_s2v.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,11 +37,18 @@
     X = text_emb_pipeline.fit_transform(dataf, dataf['label_col'])
     ```
     """
 
     def __init__(self, path: str):
         self.path = path
         self.s2v = Sense2Vec().from_disk(self.path)
+        self.shape = self.s2v["duck|NOUN"].shape
+
+    def _to_vector(self, text):
+        sense = self.s2v.get_best_sense(text)
+        if not sense:
+            return np.zeros(shape=self.shape)
+        return self.s2v[sense]
 
     def transform(self, X, y=None):
         """Transforms the phrase text into a numeric representation."""
-        return np.array([self.s2v[x] for x in X])
+        return np.array([self._to_vector(x) for x in X])
```

### Comparing `embetter-0.3.5/embetter/text/_sbert.py` & `embetter-0.3.6/embetter/text/_sbert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import pandas as pd
 import torch
+from torch.nn import Linear
+from torch.quantization import quantize_dynamic
 from sentence_transformers import SentenceTransformer as SBERT
 
 from embetter.base import EmbetterBase
 
 
 class SentenceEncoder(EmbetterBase):
     """
     Encoder that can numerically encode sentences.
 
     Arguments:
         name: name of model, see available options
         device: manually override cpu/gpu device, tries to grab gpu automatically when available
+        quantize: turns on quantization
+        num_threads: number of treads for pytorch to use, only affects when device=cpu
 
     The following model names should be supported:
 
     - `all-mpnet-base-v2`
     - `multi-qa-mpnet-base-dot-v1`
     - `all-distilroberta-v1`
     - `all-MiniLM-L12-v2`
@@ -63,20 +67,28 @@
     )
 
     # Prediction example
     text_clf_pipeline.fit(dataf, dataf['label_col']).predict(dataf)
     ```
     """
 
-    def __init__(self, name="all-MiniLM-L6-v2", device=None):
+    def __init__(
+        self, name="all-MiniLM-L6-v2", device=None, quantize=True, num_threads=2
+    ):
         if not device:
             device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.name = name
         self.device = device
         self.tfm = SBERT(name, device=self.device)
+        self.num_threads = num_threads
+        self.quantize = quantize
+        if quantize:
+            self.tfm = quantize_dynamic(self.tfm, {Linear})
+        if self.device.type == "cpu":
+            torch.set_num_threads(num_threads)
 
     def transform(self, X, y=None):
         """Transforms the text into a numeric representation."""
         # Convert pd.Series objects to encode compatable
         if isinstance(X, pd.Series):
             X = X.to_numpy()
```

### Comparing `embetter-0.3.5/embetter/text/_spacy.py` & `embetter-0.3.6/embetter/text/_spacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     # Prediction example
     text_clf_pipeline.fit(dataf, dataf['label_col']).predict(dataf)
     ```
     """
 
     def __init__(self, nlp: Union[str, Language], agg: str = "base"):
         if isinstance(nlp, str):
-            self.nlp = spacy.load(nlp, deactivate=["ner", "tagger", "parser"])
+            self.nlp = spacy.load(nlp, disable=["ner", "tagger", "parser"])
         elif isinstance(nlp, Language):
             self.nlp = nlp
         else:
             raise ValueError("`nlp` must be `str` or spaCy-language object.")
         self.agg = agg
 
     def fit(self, X, y=None):
```

### Comparing `embetter-0.3.5/embetter/vision/_colorhist.py` & `embetter-0.3.6/embetter/vision/_colorhist.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter/vision/_loader.py` & `embetter-0.3.6/embetter/vision/_loader.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter/vision/_torchvis.py` & `embetter-0.3.6/embetter/vision/_torchvis.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter.egg-info/PKG-INFO` & `embetter-0.3.6/embetter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.3.5
+Version: 0.3.6
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
@@ -69,15 +69,15 @@
 # Helpers to grab text or image from pandas column.
 from embetter.grab import ColumnGrabber
 
 # Representations/Helpers for computer vision
 from embetter.vision import ImageLoader, TimmEncoder, ColorHistogramEncoder
 
 # Representations for text
-from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder
+from embetter.text import SentenceEncoder, Sense2VecEncoder, BytePairEncoder, spaCyEncoder
 
 # Finetuning components 
 from embetter.finetune import ForwardFinetuner
 
 # External embedding providers, typically needs an API key
 from embetter.external import CohereEncoder, OpenAIEncoder
 ```
@@ -159,17 +159,18 @@
 The goal of the library is remain small but to offer a few general tools
 that might help with bulk labelling in particular, but general scikit-learn
 pipelines as well.
 
 |       class               | link                                                 | What it does                                                                                          |
 |:-------------------------:|------------------------------------------------------|--------------------------------------------------------------|
 | `ColumnGrabber`           | [docs](https://koaning.github.io/embetter/API/grab/) | `dataframe` → `ColumnGrabber` → `list with column contents`  |
+| `KeyGrabber`              | [docs](https://koaning.github.io/embetter/API/grab/) | `list of dict` → `KeyGrabber` → `list with column contents`  |
 | `SentenceEncoder`         | [docs](https://koaning.github.io/embetter/API/text/sentence-enc/) | `list of text` → `SentenceEncoder` → `embedding array`  |
 | `Sense2VecEncoder`        | [docs](https://koaning.github.io/embetter/API/text/sense2vec/)    | `list of text` → `Sense2VecEncoder` → `embedding array` |
-| `spaCyEncoder`        | [docs](https://koaning.github.io/embetter/API/text/spacy/)    | `list of text` → `spaCyEncoder` → `embedding array` |
+| `spaCyEncoder`            | [docs](https://koaning.github.io/embetter/API/text/spacy/)    | `list of text` → `spaCyEncoder` → `embedding array` |
 | `BytePairEncoder`         | [docs](https://koaning.github.io/embetter/API/text/bytepair/)    | `list of text` → `BytePairEncoder` → `embedding array` |
 | `ImageLoader`             | [docs](https://koaning.github.io/embetter/API/vision/imageload/) | `list of paths` → `ImageLoader` → `list of PIL images` |
 | `ColorHistogramEncoder`   | [docs](https://koaning.github.io/embetter/API/vision/colorhist/) | `list of PIL images` → `ColorHistogramEncoder` → `embedding array`           |
 | `TimmEncoder`             | [docs](https://koaning.github.io/embetter/API/vision/timm/) | `list of PIL images` → `TimmEncoder` → `embedding array`                     |
 | `ForwardFinetuner`        | [docs](https://koaning.github.io/embetter/API/finetune/feedforward/) | `array + labels` → `ForwardFinetuner` → `finetuned array`                     |
 | `CohereEncoder`           | [docs](https://koaning.github.io/embetter/API/external/cohere/) | `list of text` → `CohereEncoder` → `embedding array`  |
 | `OpenAIEncoder`           | [docs](https://koaning.github.io/embetter/API/external/openai/) | `list of text` → `OpenAIEncoder` → `embedding array`  |
```

### Comparing `embetter-0.3.5/embetter.egg-info/SOURCES.txt` & `embetter-0.3.6/embetter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/embetter.egg-info/requires.txt` & `embetter-0.3.6/embetter.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/setup.py` & `embetter-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 all_packages = base_packages + text_packages + vision_packages + openai_packages
 dev_packages = all_packages + docs_packages + test_packages
 
 
 setup(
     name="embetter",
-    version="0.3.5",
+    version="0.3.6",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
     description="Just a bunch of useful embeddings to get started quickly.",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license_files=("LICENSE"),
     url="https://koaning.github.io/embetter/",
```

### Comparing `embetter-0.3.5/tests/test_docs.py` & `embetter-0.3.6/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/tests/test_text.py` & `embetter-0.3.6/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.5/tests/test_vision.py` & `embetter-0.3.6/tests/test_vision.py`

 * *Files identical despite different names*

