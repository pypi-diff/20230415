# Comparing `tmp/extr-ds-0.0.4.tar.gz` & `tmp/extr-ds-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.4.tar", last modified: Fri Apr 14 12:30:19 2023, max compression
+gzip compressed data, was "extr-ds-0.0.5.tar", last modified: Sat Apr 15 13:15:49 2023, max compression
```

## Comparing `extr-ds-0.0.4.tar` & `extr-ds-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.435400 extr-ds-0.0.4/
--rw-rw-rw-   0        0        0     2591 2023-04-14 12:30:19.417144 extr-ds-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1732 2023-04-14 12:29:13.000000 extr-ds-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 12:30:19.444048 extr-ds-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-04-14 12:30:15.000000 extr-ds-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.016054 extr-ds-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.099971 extr-ds-0.0.4/src/extr_ds/
--rw-rw-rw-   0        0        0       28 2023-04-14 09:40:56.000000 extr-ds-0.0.4/src/extr_ds/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-04-13 12:42:40.000000 extr-ds-0.0.4/src/extr_ds/labellers.py
--rw-rw-rw-   0        0        0      698 2023-04-13 12:44:06.000000 extr-ds-0.0.4/src/extr_ds/models.py
--rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.4/src/extr_ds/tokenizer.py
--rw-rw-rw-   0        0        0     1527 2023-04-14 12:22:51.000000 extr-ds-0.0.4/src/extr_ds/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.389322 extr-ds-0.0.4/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     2591 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.968478 extr-ds-0.0.5/
+-rw-rw-rw-   0        0        0     2645 2023-04-15 13:15:48.963504 extr-ds-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2023-04-14 20:27:48.000000 extr-ds-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 13:15:48.978852 extr-ds-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      607 2023-04-15 13:15:11.000000 extr-ds-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.558726 extr-ds-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.848479 extr-ds-0.0.5/src/extr_ds/
+-rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.5/src/extr_ds/__init__.py
+-rw-rw-rw-   0        0        0     1602 2023-04-15 13:14:58.000000 extr-ds-0.0.5/src/extr_ds/labelers.py
+-rw-rw-rw-   0        0        0      938 2023-04-15 12:50:19.000000 extr-ds-0.0.5/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.5/src/extr_ds/tokenizer.py
+-rw-rw-rw-   0        0        0     1561 2023-04-15 12:51:08.000000 extr-ds-0.0.5/src/extr_ds/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.954479 extr-ds-0.0.5/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     2645 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.4/PKG-INFO` & `extr-ds-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -36,16 +36,16 @@
             ]),
         ])
         
         sentence_tokenizer = ## 3rd party tokenizer ##
         labels = IOB(sentence_tokenizer, entity_extractor).label(text)
         
         ## labels ==  [
-        ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
-        ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
+        ##     <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>,
+        ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
         ## ]
         ```
         
         ### 2. Find and define the type of difference between labels
         
         ```python
         from extr_ds.validators import check_for_differences
```

### Comparing `extr-ds-0.0.4/README.md` & `extr-ds-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     ]),
 ])
 
 sentence_tokenizer = ## 3rd party tokenizer ##
 labels = IOB(sentence_tokenizer, entity_extractor).label(text)
 
 ## labels ==  [
-##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
-##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
+##     <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>,
+##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
 ## ]
 ```
 
 ### 2. Find and define the type of difference between labels
 
 ```python
 from extr_ds.validators import check_for_differences
```

### Comparing `extr-ds-0.0.4/setup.py` & `extr-ds-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr-ds',
-    version='0.0.4',
+    version='0.0.5',
     keywords='',
     description='Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
-        'extr==0.0.5'
+        'extr==0.0.6'
     ],
     url='https://github.com/dpasse/extr-ds',
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

### Comparing `extr-ds-0.0.4/src/extr_ds/labellers.py` & `extr-ds-0.0.5/src/extr_ds/labelers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List, Callable, Generator, Iterator, cast
 from extr import Entity, EntityExtractor
-from .models import TokenGroup
+from .models import TokenGroup, Label
 from .tokenizer import tokenizer
 
 
 class IOB():
     def __init__(self, sentence_tokenizer: Callable[[str], List[List[str]]], entity_extractor: EntityExtractor) -> None:
         self._sentence_tokenizer = sentence_tokenizer
         self._entity_extractor = entity_extractor
 
-    def label(self, text: str) -> Generator[List[str], None, None]:
+    def label(self, text: str) -> Generator[Label, None, None]:
         entities = self._entity_extractor.get_entities(text)
         token_groups = tokenizer(text, self._sentence_tokenizer(text))
 
         return self.__merge(token_groups, entities)
 
-    def __merge(self, token_groups: Generator[TokenGroup, None, None], entities: List[Entity]) -> Generator[List[str], None, None]:
+    def __merge(self, token_groups: Generator[TokenGroup, None, None], entities: List[Entity]) -> Generator[Label, None, None]:
         for token_group in token_groups:
             tokens = list(enumerate(token_group.tokens))
             labels = ['O' for _ in range(len(tokens))]
             for entity in cast(Iterator[Entity], filter(token_group.contains, entities)):
                 used_counter = 0
 
                 for i, token in tokens:
@@ -27,10 +27,12 @@
                         continue
 
                     assert labels[i] == 'O', f'bad tokenizer? multiple entities belong to the same token - {labels[i]}'
 
                     labels[i] = 'B-' if used_counter == 0 else 'I-'
                     labels[i] += entity.label
 
+                    token.add_entity(entity)
+
                     used_counter += 1
 
-            yield labels
+            yield Label(token_group.tokens, labels)
```

### Comparing `extr-ds-0.0.4/src/extr_ds/models.py` & `extr-ds-0.0.5/src/extr_ds/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,31 @@
 @dataclass(frozen=True)
 class Token(ILocation):
     text: str
     location: Location
     order: int
     entities: List[Entity] = field(default_factory=lambda: [])
 
-    def add_token(self, entity: Entity):
+    def add_entity(self, entity: Entity):
         self.entities.append(entity)
 
     def __len__(self) -> int:
         return len(self.entities)
 
+    def __str__(self) -> str:
+        return self.text
+
     def __repr__(self) -> str:
         return f'<Token text="{self.text}", location={repr(self.location)}, order={self.order}>'
 
 @dataclass(frozen=True)
 class TokenGroup(ILocation):
     location: Location
     tokens: List[Token]
+
+@dataclass
+class Label:
+    tokens: List[Token]
+    labels: List[str]
+
+    def __repr__(self) -> str:
+        return f'<Label tokens={self.tokens}, labels={self.labels}>'
```

### Comparing `extr-ds-0.0.4/src/extr_ds/tokenizer.py` & `extr-ds-0.0.5/src/extr_ds/tokenizer.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.4/src/extr_ds/validators.py` & `extr-ds-0.0.5/src/extr_ds/validators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 from dataclasses import dataclass
-
 from enum import Enum
 
+
 # class syntax
 class DifferenceTypes(Enum):
     NONE = 0
     MISMATCH = 1
     S1_MISSING = 2
     S2_MISSING = 3
 
@@ -24,31 +24,32 @@
     sentence_labels_2: List[str]
     diffs_between_labels: List[Difference]
 
     @property
     def has_diffs(self) -> bool:
         return len(self.diffs_between_labels) > 0
 
-def check_for_differences(sentence_labels_1: List[str], sentence_labels_2: List[str]) -> Differences:
-    assert len(sentence_labels_1) == len(sentence_labels_2)
+def check_for_differences(labels_1: List[str], labels_2: List[str]) -> Differences:
+    def get_difference_type(label_1: str, label_2: str) -> DifferenceTypes:
+        diff_type = DifferenceTypes.NONE
+        if label_2 == 'O' or len(label_2) == 0:
+            diff_type = DifferenceTypes.S2_MISSING
+        elif label_1 == 'O' or len(label_1) == 0:
+            diff_type = DifferenceTypes.S1_MISSING
+        else:
+            diff_type = DifferenceTypes.MISMATCH
 
-    diffs_between_labels = []
-    for i, [label_1, label_2] in enumerate(zip(sentence_labels_1, sentence_labels_2)):
+        return diff_type
 
+    assert len(labels_1) == len(labels_2)
+
+    diffs_between_labels = []
+    for i, [label_1, label_2] in enumerate(zip(labels_1, labels_2)):
         if label_1 != label_2:
-            diff_type = DifferenceTypes.NONE
-            if label_2 == 'O' or len(label_2) == 0:
-                diff_type = DifferenceTypes.S2_MISSING
-            elif label_1 == 'O' or len(label_1) == 0:
-                diff_type = DifferenceTypes.S1_MISSING
-            else:
-                diff_type = DifferenceTypes.MISMATCH
-
-            diffs_between_labels.append(
-                Difference(i, diff_type)
-            )
+            diff_type = get_difference_type(label_1, label_2)
+            diffs_between_labels.append(Difference(i, diff_type))
 
     return Differences(
-        sentence_labels_1,
-        sentence_labels_2,
+        labels_1,
+        labels_2,
         diffs_between_labels
     )
```

### Comparing `extr-ds-0.0.4/src/extr_ds.egg-info/PKG-INFO` & `extr-ds-0.0.5/src/extr_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -36,16 +36,16 @@
             ]),
         ])
         
         sentence_tokenizer = ## 3rd party tokenizer ##
         labels = IOB(sentence_tokenizer, entity_extractor).label(text)
         
         ## labels ==  [
-        ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
-        ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
+        ##     <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>,
+        ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
         ## ]
         ```
         
         ### 2. Find and define the type of difference between labels
         
         ```python
         from extr_ds.validators import check_for_differences
```

