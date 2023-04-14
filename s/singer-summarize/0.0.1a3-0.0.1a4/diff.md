# Comparing `tmp/singer_summarize-0.0.1a3.tar.gz` & `tmp/singer_summarize-0.0.1a4.tar.gz`

## Comparing `singer_summarize-0.0.1a3.tar` & `singer_summarize-0.0.1a4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 singer_summarize-0.0.1a3/local_dependencies/singer_rust/Cargo.toml
--rw-r--r--   0     1001      123     4507 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/local_dependencies/singer_rust/src/lib.rs
--rw-r--r--   0     1001      123     4272 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/local_dependencies/singer_rust/src/message/io.rs
--rw-r--r--   0     1001      123      105 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/local_dependencies/singer_rust/src/message/mod.rs
--rw-r--r--   0     1001      123     4150 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/local_dependencies/singer_rust/src/message/types.rs
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 singer_summarize-0.0.1a3/Cargo.toml
--rw-r--r--   0     1001      123     1067 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/LICENSE
--rw-r--r--   0     1001      123      757 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/README.md
--rw-r--r--   0     1001      123       10 2023-04-14 23:37:30.000000 singer_summarize-0.0.1a3/dist/singer_summarize-0.0.1a3.tar.gz
--rw-r--r--   0     1001      123      905 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/pyproject.toml
--rw-r--r--   0     1001      123      453 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/src/bin/singer-summarize.rs
--rw-r--r--   0     1001      123      104 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/src/cli.rs
--rw-r--r--   0     1001      123     3597 2023-04-14 23:36:49.000000 singer_summarize-0.0.1a3/src/lib.rs
--rw-r--r--   0     1001      123     9816 2023-04-14 23:37:29.000000 singer_summarize-0.0.1a3/Cargo.lock
--rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 singer_summarize-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 singer_summarize-0.0.1a4/local_dependencies/singer_rust/Cargo.toml
+-rw-r--r--   0     1001      123     4507 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/local_dependencies/singer_rust/src/lib.rs
+-rw-r--r--   0     1001      123     4272 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/local_dependencies/singer_rust/src/message/io.rs
+-rw-r--r--   0     1001      123      105 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/local_dependencies/singer_rust/src/message/mod.rs
+-rw-r--r--   0     1001      123     4150 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/local_dependencies/singer_rust/src/message/types.rs
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 singer_summarize-0.0.1a4/Cargo.toml
+-rw-r--r--   0     1001      123     1067 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/LICENSE
+-rw-r--r--   0     1001      123      914 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/README.md
+-rw-r--r--   0     1001      123       10 2023-04-14 23:48:23.000000 singer_summarize-0.0.1a4/dist/singer_summarize-0.0.1a4.tar.gz
+-rw-r--r--   0     1001      123      905 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/pyproject.toml
+-rw-r--r--   0     1001      123      453 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/src/bin/singer-summarize.rs
+-rw-r--r--   0     1001      123      104 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/src/cli.rs
+-rw-r--r--   0     1001      123     3597 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/src/lib.rs
+-rw-r--r--   0     1001      123     9816 2023-04-14 23:47:50.000000 singer_summarize-0.0.1a4/Cargo.lock
+-rw-r--r--   0        0        0     1770 1970-01-01 00:00:00.000000 singer_summarize-0.0.1a4/PKG-INFO
```

### Comparing `singer_summarize-0.0.1a3/local_dependencies/singer_rust/src/lib.rs` & `singer_summarize-0.0.1a4/local_dependencies/singer_rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `singer_summarize-0.0.1a3/local_dependencies/singer_rust/src/message/io.rs` & `singer_summarize-0.0.1a4/local_dependencies/singer_rust/src/message/io.rs`

 * *Files identical despite different names*

### Comparing `singer_summarize-0.0.1a3/local_dependencies/singer_rust/src/message/types.rs` & `singer_summarize-0.0.1a4/local_dependencies/singer_rust/src/message/types.rs`

 * *Files identical despite different names*

### Comparing `singer_summarize-0.0.1a3/Cargo.toml` & `singer_summarize-0.0.1a4/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "singer_summarize"
-version = "0.0.1-a3"
+version = "0.0.1-a4"
 edition = "2021"
 rust-version = "1.67"
 documentation = "https://github.com/edgarrmondragon/singer-rust"
 homepage = "https://github.com/edgarrmondragon/singer-rust"
 repository = "https://github.com/edgarrmondragon/singer-rust"
 readme = "README.md"
 license = "MIT"
```

### Comparing `singer_summarize-0.0.1a3/LICENSE` & `singer_summarize-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `singer_summarize-0.0.1a3/README.md` & `singer_summarize-0.0.1a4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # singer-summarize
 
 A POC Singer target that summarizes a tap's output.
 
+## Installation
+
+### From PyPI
+
+I recommend using [pipx](https://pypa.github.io/pipx/) to install this package:
+
+```shell
+pipx install singer-summarize
+```
+
 ## Build
 
 ### Binary
 
 ```shell
 cargo build -p singer_summarize --release
 ```
```

### Comparing `singer_summarize-0.0.1a3/pyproject.toml` & `singer_summarize-0.0.1a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "maturin"
 requires = ["maturin>=0.14,<0.15"]
 
 [project]
 name = "singer_summarize"
-version = "0.0.1-a3"
+version = "0.0.1-a4"
 description = "Singer target that summarizes a tap's output"
 authors = [{ name = "Edgar Ramirez", email = "edgarrm358@gmail.com" }]
 maintainers = [{ name = "Edgar Ramirez", email = "edgarrm358@gmail.com" }]
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["singer.io", "target"]
```

### Comparing `singer_summarize-0.0.1a3/src/lib.rs` & `singer_summarize-0.0.1a4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `singer_summarize-0.0.1a3/Cargo.lock` & `singer_summarize-0.0.1a4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "singer_summarize"
-version = "0.0.1-a3"
+version = "0.0.1-a4"
 dependencies = [
  "clap",
  "serde",
  "serde_json",
  "singer_rust",
 ]
```

### Comparing `singer_summarize-0.0.1a3/PKG-INFO` & `singer_summarize-0.0.1a4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singer_summarize
-Version: 0.0.1a3
+Version: 0.0.1a4
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Rust
@@ -19,14 +19,24 @@
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/edgarrmondragon/singer-rust
 
 # singer-summarize
 
 A POC Singer target that summarizes a tap's output.
 
+## Installation
+
+### From PyPI
+
+I recommend using [pipx](https://pypa.github.io/pipx/) to install this package:
+
+```shell
+pipx install singer-summarize
+```
+
 ## Build
 
 ### Binary
 
 ```shell
 cargo build -p singer_summarize --release
 ```
```

