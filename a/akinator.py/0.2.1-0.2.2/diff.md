# Comparing `tmp/akinator.py-0.2.1.tar.gz` & `tmp/akinator.py-0.2.2.tar.gz`

## Comparing `akinator.py-0.2.1.tar` & `akinator.py-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 akinator.py-0.2.1/Cargo.toml
--rw-r--r--   0     1001      121     4639 2022-08-20 18:30:53.000000 akinator.py-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      121       88 2022-08-20 18:30:53.000000 akinator.py-0.2.1/.gitignore
--rw-r--r--   0     1001      121      213 2022-08-20 18:30:53.000000 akinator.py-0.2.1/.readthedocs.yml
--rw-r--r--   0     1001      121      190 2022-08-20 18:30:53.000000 akinator.py-0.2.1/.vscode/settings.json
--rw-r--r--   0     1001      121     1076 2022-08-20 18:30:53.000000 akinator.py-0.2.1/LICENSE
--rw-r--r--   0     1001      121      577 2022-08-20 18:30:53.000000 akinator.py-0.2.1/README.md
--rw-r--r--   0     1001      121     4220 2022-08-20 18:30:53.000000 akinator.py-0.2.1/akinator.pyi
--rw-r--r--   0     1001      121      146 2022-08-20 18:30:53.000000 akinator.py-0.2.1/docs/akinator.rst
--rw-r--r--   0     1001      121     2498 2022-08-20 18:30:53.000000 akinator.py-0.2.1/docs/conf.py
--rw-r--r--   0     1001      121     4170 2022-08-20 18:30:53.000000 akinator.py-0.2.1/docs/examples.rst
--rw-r--r--   0     1001      121      475 2022-08-20 18:30:53.000000 akinator.py-0.2.1/docs/index.rst
--rw-r--r--   0     1001      121      591 2022-08-20 18:30:53.000000 akinator.py-0.2.1/pyproject.toml
--rw-r--r--   0     1001      121     9925 2022-08-20 18:30:53.000000 akinator.py-0.2.1/src/async_akinator.rs
--rw-r--r--   0     1001      121     8537 2022-08-20 18:30:53.000000 akinator.py-0.2.1/src/blocking_akinator.rs
--rw-r--r--   0     1001      121     6147 2022-08-20 18:30:53.000000 akinator.py-0.2.1/src/enums.rs
--rw-r--r--   0     1001      121     3947 2022-08-20 18:30:53.000000 akinator.py-0.2.1/src/error.rs
--rw-r--r--   0     1001      121     1044 2022-08-20 18:30:53.000000 akinator.py-0.2.1/src/lib.rs
--rw-r--r--   0     1001      121     1989 2022-08-20 18:30:53.000000 akinator.py-0.2.1/src/models.rs
--rw-r--r--   0     1001      121     1612 2022-08-20 18:30:53.000000 akinator.py-0.2.1/tests/test_async.py
--rw-r--r--   0     1001      121     1543 2022-08-20 18:30:53.000000 akinator.py-0.2.1/tests/test_sync.py
--rw-r--r--   0     1001      121       10 2022-08-20 18:31:18.000000 akinator.py-0.2.1/wheelhouse/akinator.py-0.2.1.tar.gz
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 akinator.py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 akinator.py-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123     4639 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123       88 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.gitignore
+-rw-r--r--   0     1001      123      213 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.readthedocs.yml
+-rw-r--r--   0     1001      123      190 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.vscode/settings.json
+-rw-r--r--   0     1001      123     1076 2023-04-14 23:36:17.000000 akinator.py-0.2.2/LICENSE
+-rw-r--r--   0     1001      123      695 2023-04-14 23:36:17.000000 akinator.py-0.2.2/README.md
+-rw-r--r--   0     1001      123     4220 2023-04-14 23:36:17.000000 akinator.py-0.2.2/akinator.pyi
+-rw-r--r--   0     1001      123      146 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/akinator.rst
+-rw-r--r--   0     1001      123     2498 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/conf.py
+-rw-r--r--   0     1001      123     4170 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/examples.rst
+-rw-r--r--   0     1001      123      475 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/index.rst
+-rw-r--r--   0     1001      123      591 2023-04-14 23:36:17.000000 akinator.py-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123    10034 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/async_akinator.rs
+-rw-r--r--   0     1001      123     8646 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/blocking_akinator.rs
+-rw-r--r--   0     1001      123     6575 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/enums.rs
+-rw-r--r--   0     1001      123     3947 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/error.rs
+-rw-r--r--   0     1001      123     1044 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123     1996 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/models.rs
+-rw-r--r--   0     1001      123     1612 2023-04-14 23:36:17.000000 akinator.py-0.2.2/tests/test_async.py
+-rw-r--r--   0     1001      123     1543 2023-04-14 23:36:17.000000 akinator.py-0.2.2/tests/test_sync.py
+-rw-r--r--   0     1001      123       10 2023-04-14 23:36:38.000000 akinator.py-0.2.2/wheelhouse/akinator.py-0.2.2.tar.gz
+-rw-r--r--   0     1001      123    29148 2023-04-14 23:36:37.000000 akinator.py-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 akinator.py-0.2.2/PKG-INFO
```

### Comparing `akinator.py-0.2.1/Cargo.toml` & `akinator.py-0.2.2/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "akinator-py"
 authors = ["Tom-the-Bomb"]
-version = "0.2.1"
+version = "0.2.2"
 edition = "2021"
 license = "MIT"
 readme = "README.md"
 description = "Python bindings for akinator-rs"
 documentation = "https://akinatorpy.readthedocs.io/en/latest/"
 repository = "https://github.com/Tom-the-Bomb/akinator.py"
 homepage = "https://github.com/Tom-the-Bomb/akinator.py"
@@ -23,12 +23,12 @@
 ]
 
 [lib]
 name = "akinator"
 crate-type = ["cdylib"]
 
 [dependencies]
-akinator-rs = "0.1"
 lazy_static = "1.4"
 pyo3-asyncio = { version = "0.16", features = ["tokio-runtime"] }
+akinator-rs = { git = "https://github.com/Tom-the-Bomb/akinator-rs" }
 tokio = { version = "1.20", features = ["sync", "rt", "rt-multi-thread"] }
 pyo3 = { version = "0.16", features = ["extension-module", "abi3-py37"] }
```

### Comparing `akinator.py-0.2.1/.github/workflows/ci.yml` & `akinator.py-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/LICENSE` & `akinator.py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/akinator.pyi` & `akinator.py-0.2.2/akinator.pyi`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/docs/conf.py` & `akinator.py-0.2.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'akinator.py'
 copyright = '2022, Tom-the-Bomb'
 author = 'Tom-the-Bomb'
 
 # The full version, including alpha/beta/rc tags
-release = '0.2.0'
+release = '0.2.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `akinator.py-0.2.1/docs/examples.rst` & `akinator.py-0.2.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/src/async_akinator.rs` & `akinator.py-0.2.2/src/async_akinator.rs`

 * *Files 3% similar despite different names*

```diff
@@ -27,22 +27,25 @@
 ///
 /// Parameters are also set as properties which also have a setter to change the values if necessary in the future
 ///
 /// Parameters
 /// ----------
 /// theme : Optional[:class:`Theme`]
 ///     the theme of the akinator game, would be one of ``Characters``, ``Animals`` or ``Objects``
-///     pass in using an answer enum, using the ``from_str`` classmethod if necessary, defaults to ``Characters``
+///     pass in using an answer enum, using the ``from_str`` classmethod if necessary,
+///     defaults to ``Characters``
 /// language : Optional[:class:`Language`]
-///     the language for the akinator game, refer to the :class:`Language` enum
+///     the language for the akinator game, refer to the :class:`Language` enum,
+///     defaults to ``English``
 /// child_mode : Optional[:class:`bool`]
-///     when set to ``True``, NSFW content will not be provided
+///     when set to ``True``, NSFW content will not be provided,
+///     defaults to ``False``
 #[pyclass]
 #[derive(Debug, Clone)]
-#[pyo3(text_signature = "(*, theme, language, child_mode)")]
+#[pyo3(text_signature = "(*, theme = None, language = None, child_mode = None)")]
 pub struct AsyncAkinator(
     Arc<RwLock<AkinatorStruct>>,
 );
 
 #[pymethods]
 impl AsyncAkinator {
     #[new]
@@ -95,15 +98,15 @@
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - getting the starting timestamp failed
     ///         - the data required to start the game such as the server url, frontaddr or game UID could not be found
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     fn start_game<'a>(&'a mut self, py: Python<'a>) -> PyResult<&'a PyAny> {
         let cloned = self.0.clone();
 
         to_coro(py,
             async move {
@@ -135,15 +138,15 @@
     /// ------
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - missing required data to continue
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     #[pyo3(text_signature = "(self, answer)")]
     fn answer<'a>(&'a mut self, py: Python<'a>, answer: Answer) -> PyResult<&'a PyAny> {
         let cloned = self.0.clone();
 
         to_coro(py,
@@ -171,15 +174,15 @@
     /// ------
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - missing required data to continue
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     fn win<'a>(&'a mut self, py: Python<'a>) -> PyResult<&'a PyAny> {
         let cloned = self.0.clone();
 
         to_coro(py,
             async move {
@@ -210,15 +213,15 @@
     ///     Could not go back anymore, likely that we are already on the first question
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - missing required data to continue
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     fn back<'a>(&'a mut self, py: Python<'a>) -> PyResult<&'a PyAny> {
         let cloned = self.0.clone();
 
         to_coro(py,
             async move {
```

### Comparing `akinator.py-0.2.1/src/blocking_akinator.rs` & `akinator.py-0.2.2/src/blocking_akinator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 ///
 /// Parameters are also set as properties which also have a setter to change the values if necessary in the future
 ///
 /// Parameters
 /// ----------
 /// theme : Optional[:class:`Theme`]
 ///     the theme of the akinator game, would be one of ``Characters``, ``Animals`` or ``Objects``
-///     pass in using an answer enum, using the ``from_str`` classmethod if necessary, defaults to ``Characters``
+///     pass in using an answer enum, using the ``from_str`` classmethod if necessary,
+///     defaults to ``Characters``
 /// language : Optional[:class:`Language`]
-///     the language for the akinator game, refer to the ``Language`` enum
+///     the language for the akinator game, refer to the ``Language`` enum,
+///     defaults to ``English``
 /// child_mode : Optional[:class:`bool`]
-///     when set to ``True``, NSFW content will not be provided
+///     when set to ``True``, NSFW content will not be provided,
+///     defaults to ``False``
 #[pyclass]
 #[derive(Debug, Clone)]
-#[pyo3(text_signature = "(*, theme, language, child_mode)")]
+#[pyo3(text_signature = "(*, theme = None, language = None, child_mode = None)")]
 pub struct Akinator(
     AkinatorStruct,
 );
 
 #[pymethods]
 impl Akinator {
     #[new]
@@ -86,15 +89,15 @@
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - getting the starting timestamp failed
     ///         - the data required to start the game such as the server url, frontaddr or game UID could not be found
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     fn start_game<'a>(&'a mut self, _py: Python<'a>) -> PyResult<Option<String>> {
         RUNTIME.block_on(
             async move {
                 self.0.start().await
                     .map_err(|e| Error::from(e).into())
@@ -119,15 +122,15 @@
     /// ------
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - missing required data to continue
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     #[pyo3(text_signature = "(self, answer)")]
     fn answer<'a>(&'a mut self, _py: Python<'a>, answer: Answer) -> PyResult<Option<String>> {
         RUNTIME.block_on(
             async move {
                 self.0.answer(answer.into()).await
@@ -148,15 +151,15 @@
     /// ------
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - missing required data to continue
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     fn win<'a>(&'a mut self, _py: Python<'a>) -> PyResult<Option<Guess>> {
         RUNTIME.block_on(
             async move {
                 self.0.win().await
                     .map(|result| {
@@ -180,15 +183,15 @@
     ///     Could not go back anymore, likely that we are already on the first question
     /// :class:`RuntimeError`
     ///     Something internal went wrong, this could be in this case:
     ///         - missing required data to continue
     ///         - request error: any sort of error when making the HTTP requests
     ///         - updating the internal data fields errored (either a field was missing or was of the wrong type)
     /// :class:`ValueError`
-    ///     Could not parse the returned JSON properly (invalid, missing fields etc.)
+    ///     Could not parse the API returned JSON properly (invalid, missing fields etc.)
     /// ``Other api errors``
     ///     Refer to the exceptions at the bottom of the page
     fn back<'a>(&'a mut self, _py: Python<'a>) -> PyResult<Option<String>> {
         RUNTIME.block_on(
             async move {
                 self.0.back().await
                     .map_err(|e| Error::from(e).into())
```

### Comparing `akinator.py-0.2.1/src/enums.rs` & `akinator.py-0.2.2/src/enums.rs`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,19 @@
     /// aliases for answer variants are also accepted (trims ws & case-insensitive):
     ///     - ``yes | y | 0`` -> ``Answer.Yes``
     ///     - ``no | n | 1`` -> ``Answer.No``
     ///     - ``i don(')?t know | idk | 2`` -> ``Answer.Idk``
     ///     - ``probably | p | 3`` -> ``Answer.Probably``
     ///     - ``probably not | pn | 4`` -> ``Answer.ProbablyNot``
     ///
+    /// Parameters
+    /// ----------
+    /// answer : :class:`str`
+    ///     the string representation of the answer to parse from
+    ///
     /// Raises
     /// ------
     /// :class:`InvalidAnswer`
     ///     raised if the provided answer cannot match one of the above (is invalid)
     #[classmethod]
     #[pyo3(text_signature = "(self, answer)")]
     fn from_str(_cls: &PyType, answer: String) -> PyResult<Self> {
@@ -103,14 +108,19 @@
 }
 
 #[pymethods]
 impl Theme {
     /// a classmethod to return a :class:`Theme` enum variant parsing from a :class:`str`
     /// useful when you have external user input
     ///
+    /// Parameters
+    /// ----------
+    /// theme : :class:`str`
+    ///     the string representation of the theme to parse from
+    ///
     /// .. note ::
     ///     if an invalid string for the theme is given, no error will be raised
     ///     instead it will just fallback to ``Theme.Characters`` as the default
     #[classmethod]
     #[pyo3(text_signature = "(self, theme)")]
     fn from_str(_cls: &PyType, theme: String) -> Self {
         Self::from(ThemeEnum::from(theme))
@@ -128,14 +138,19 @@
 #[pymethods]
 impl Language {
     /// a classmethod to return a :class:`Language` enum variant parsing from a :class:`str`
     /// useful when you have external user input
     ///
     /// Short forms such as ``en`` or ``fr`` are also accepted along with the full name
     ///
+    /// Parameters
+    /// ----------
+    /// language : :class:`str`
+    ///     the string representation of the language to parse from
+    ///
     /// Raises
     /// ------
     /// :class:`InvalidLanguage`
     ///     Raised if the given string is of an invalid language
     #[classmethod]
     #[pyo3(text_signature = "(self, language)")]
     fn from_str(_cls: &PyType, language: String) -> PyResult<Self> {
```

### Comparing `akinator.py-0.2.1/src/error.rs` & `akinator.py-0.2.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/src/lib.rs` & `akinator.py-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/src/models.rs` & `akinator.py-0.2.2/src/models.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use pyo3::prelude::*;
 use akinator_rs::models::Guess as GuessModel;
 
 
 /// a model class representing an akinator's guess
-/// not meant for the user to construct, but is returned in various properties and methods in the `Akinator` class
+/// not meant for the user to construct, but is returned in various properties and methods in the :class:`Akinator` class
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct Guess(
     pub GuessModel,
 );
 
 #[pymethods]
```

### Comparing `akinator.py-0.2.1/tests/test_async.py` & `akinator.py-0.2.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/tests/test_sync.py` & `akinator.py-0.2.2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.1/PKG-INFO` & `akinator.py-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akinator.py
-Version: 0.2.1
+Version: 0.2.2
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: sphinxext-opengraph; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Provides-Extra: docs
 License-File: LICENSE
 Summary: Python bindings for akinator-rs
@@ -15,21 +15,23 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: documentation, https://akinatorpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/Tom-the-Bomb/akinator.py
 Project-URL: homepage, https://github.com/Tom-the-Bomb/akinator.py
 
 # Akinator-py
-python bindings for [akinator-rs](https://github.com/Tom-the-Bomb/akinator-rs) using [pyo3](https://pyo3.rs)
+Python bindings for ``akinator-rs``, a wrapper around the undocumented akinator API, made using [pyo3](https://pyo3.rs)
+
+designed for easy implementation of an akinator game in code, providing a simple and easy to use API.
 
 ### Installation
 Prebuilt wheels are uploaded onto pypi, if you platform is supported, you can install with:
 
 ```bash
 $ py -m pip install akinator.py
 ```
 
 You can also build from source yourself if you have `rust` installed
 
 ### Examples
 - refer to the [tests](https://github.com/Tom-the-Bomb/akinator.py/tree/master/tests) for full examples on usage
-- Refer to the documentation [here](https://akinatorpy.readthedocs.io/en/latest/) for more information
+- Refer to the **documentation** [here](https://akinatorpy.readthedocs.io/en/latest/) for more information
```

