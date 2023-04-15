# Comparing `tmp/theme-label-0.2.0.tar.gz` & `tmp/theme-label-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theme-label-0.2.0.tar", last modified: Sun Feb 12 20:48:43 2023, max compression
+gzip compressed data, was "theme-label-0.2.1.tar", last modified: Sat Apr 15 15:59:39 2023, max compression
```

## Comparing `theme-label-0.2.0.tar` & `theme-label-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-02-12 20:48:43.653589 theme-label-0.2.0/
--rw-r--r--   0 ilia      (1000) ilia      (1000)     1080 2023-02-12 15:59:47.000000 theme-label-0.2.0/LICENSE
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2421 2023-02-12 20:48:43.653589 theme-label-0.2.0/PKG-INFO
--rw-r--r--   0 ilia      (1000) ilia      (1000)     2054 2023-02-12 15:59:52.000000 theme-label-0.2.0/README.md
--rw-r--r--   0 ilia      (1000) ilia      (1000)       86 2023-02-12 15:59:47.000000 theme-label-0.2.0/pyproject.toml
--rw-rw-r--   0 ilia      (1000) ilia      (1000)       38 2023-02-12 20:48:43.653589 theme-label-0.2.0/setup.cfg
--rw-r--r--   0 ilia      (1000) ilia      (1000)      709 2023-02-12 20:46:11.000000 theme-label-0.2.0/setup.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-02-12 20:48:43.649589 theme-label-0.2.0/theme/
--rw-r--r--   0 ilia      (1000) ilia      (1000)      122 2023-02-12 15:59:52.000000 theme-label-0.2.0/theme/__init__.py
--rw-r--r--   0 ilia      (1000) ilia      (1000)    11992 2023-02-12 16:06:54.000000 theme-label-0.2.0/theme/theme.py
-drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-02-12 20:48:43.653589 theme-label-0.2.0/theme_label.egg-info/
--rw-rw-r--   0 ilia      (1000) ilia      (1000)     2421 2023-02-12 20:48:43.000000 theme-label-0.2.0/theme_label.egg-info/PKG-INFO
--rw-rw-r--   0 ilia      (1000) ilia      (1000)      252 2023-02-12 20:48:43.000000 theme-label-0.2.0/theme_label.egg-info/SOURCES.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        1 2023-02-12 20:48:43.000000 theme-label-0.2.0/theme_label.egg-info/dependency_links.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)       13 2023-02-12 20:48:43.000000 theme-label-0.2.0/theme_label.egg-info/requires.txt
--rw-rw-r--   0 ilia      (1000) ilia      (1000)        6 2023-02-12 20:48:43.000000 theme-label-0.2.0/theme_label.egg-info/top_level.txt
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-15 15:59:39.862366 theme-label-0.2.1/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     1080 2023-02-12 15:59:47.000000 theme-label-0.2.1/LICENSE
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2421 2023-04-15 15:59:39.862366 theme-label-0.2.1/PKG-INFO
+-rw-r--r--   0 ilia      (1000) ilia      (1000)     2054 2023-02-12 15:59:52.000000 theme-label-0.2.1/README.md
+-rw-r--r--   0 ilia      (1000) ilia      (1000)       86 2023-02-12 15:59:47.000000 theme-label-0.2.1/pyproject.toml
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)       38 2023-04-15 15:59:39.862366 theme-label-0.2.1/setup.cfg
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      709 2023-04-15 15:35:51.000000 theme-label-0.2.1/setup.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-15 15:59:39.858366 theme-label-0.2.1/theme/
+-rw-r--r--   0 ilia      (1000) ilia      (1000)      122 2023-04-15 15:35:55.000000 theme-label-0.2.1/theme/__init__.py
+-rw-r--r--   0 ilia      (1000) ilia      (1000)    12334 2023-04-15 15:45:04.000000 theme-label-0.2.1/theme/theme.py
+drwxrwxr-x   0 ilia      (1000) ilia      (1000)        0 2023-04-15 15:59:39.862366 theme-label-0.2.1/theme_label.egg-info/
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)     2421 2023-04-15 15:59:39.000000 theme-label-0.2.1/theme_label.egg-info/PKG-INFO
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)      252 2023-04-15 15:59:39.000000 theme-label-0.2.1/theme_label.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        1 2023-04-15 15:59:39.000000 theme-label-0.2.1/theme_label.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)       13 2023-04-15 15:59:39.000000 theme-label-0.2.1/theme_label.egg-info/requires.txt
+-rw-rw-r--   0 ilia      (1000) ilia      (1000)        6 2023-04-15 15:59:39.000000 theme-label-0.2.1/theme_label.egg-info/top_level.txt
```

### Comparing `theme-label-0.2.0/LICENSE` & `theme-label-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `theme-label-0.2.0/PKG-INFO` & `theme-label-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theme-label
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple CLI labeling tool for text classification
 Author: Ilia Moiseev
 Author-email: ilia.moiseev.5@yandex.ru
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `theme-label-0.2.0/README.md` & `theme-label-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `theme-label-0.2.0/setup.py` & `theme-label-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="theme-label",
-    version='0.2.0',
+    version='0.2.1',
     author='Ilia Moiseev',
     author_email='ilia.moiseev.5@yandex.ru',
     license='MIT',
     description="Simple CLI labeling tool for text classification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `theme-label-0.2.0/theme/theme.py` & `theme-label-0.2.1/theme/theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,25 +147,36 @@
         np.random.shuffle(self._unmarked_indices)
 
         self._marked_indices = []
 
         self._check_values()
 
     def _check_values(self) -> None:
-        for col in self._show_cols + [self._text_col, self._id_col]:
-            if col not in self._unmarked:
-                raise ValueError(
-                    f'\'{col}\' not in the table columns: {list(self._unmarked.columns)}')
         for inp in self._id2label:
             if inp in self._input_map:
                 raise ValueError(
                     f'\'{inp}\' string from id2label already present in commands. '
                     f'Either change the \'{self._input_map[inp]}\' command or a value in id2label'
                 )
 
+        missing_cols = []
+        for col in self._show_cols + [self._text_col, self._id_col]:
+            if col not in self._unmarked:
+                missing_cols.append(col)
+
+        if len(missing_cols):
+            raise ValueError(
+                f'{missing_cols} from id2label not in the table columns: {list(self._unmarked.columns)}')
+
+        for inp in self._id2label:
+            if not isinstance(inp, str):
+                raise ValueError(
+                    f'{inp} in id2label is not string. Please, pass values that the user will type as strings'
+                )
+
     def _load_data(self) -> None:
         self._unmarked = pd.read_csv(self._unmarked_table)
         if self._label_col in self._unmarked and self._select_label is not None:
             self._unmarked = self._unmarked[self._unmarked[self._label_col] == self._select_label]
         else:
             self._unmarked[self._label_col] = None
 
@@ -273,17 +284,17 @@
         else:
             cprint('R', 'HISTORY IS EMPTY')
 
     def _more(self, row) -> None:
         if pd.notna(row[self._text_col]):
             text = row[self._text_col]
             start = self._chars_showed
-            end = min(start + self._show_chars, len(text) - 1)
+            end = min(start + self._show_chars, len(text))
 
-            if start == len(text) - 1:
+            if start == len(text):
                 cprint('R', 'END')
             elif end <= len(text):
                 print(text[start:end])
                 self._chars_showed = end
         else:
             cprint('R', 'CAN\'T SHOW MORE')
```

### Comparing `theme-label-0.2.0/theme_label.egg-info/PKG-INFO` & `theme-label-0.2.1/theme_label.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theme-label
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple CLI labeling tool for text classification
 Author: Ilia Moiseev
 Author-email: ilia.moiseev.5@yandex.ru
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

