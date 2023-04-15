# Comparing `tmp/quom-4.0.0.tar.gz` & `tmp/quom-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quom-4.0.0.tar", last modified: Sat Apr 15 10:54:33 2023, max compression
+gzip compressed data, was "quom-4.0.1.tar", last modified: Sat Apr 15 11:10:53 2023, max compression
```

## Comparing `quom-4.0.0.tar` & `quom-4.0.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-15 10:54:20.000000 quom-4.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-15 10:54:20.000000 quom-4.0.0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-15 10:54:20.000000 quom-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 10:54:20.000000 quom-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-15 10:54:33.201320 quom-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-15 10:54:20.000000 quom-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/artwork/
--rw-r--r--   0 runner    (1001) docker     (123)   313993 2023-04-15 10:54:20.000000 quom-4.0.0/artwork/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   180297 2023-04-15 10:54:20.000000 quom-4.0.0/artwork/logo_banner.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/examples/flat_structure/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/foobar_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/examples/flat_structure/libfoobar/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/bar.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/bar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/foo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/foo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/foobar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/util.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 10:54:20.000000 quom-4.0.0/examples/flat_structure/libfoobar/util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.197320 quom-4.0.0/examples/include_directory/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/foobar_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/examples/include_directory/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/examples/include_directory/include/libfoobar/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/bar.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/bar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/foo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/foo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/foobar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/util.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 10:54:20.000000 quom-4.0.0/examples/include_directory/include/libfoobar/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-15 10:54:33.205320 quom-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 10:54:20.000000 quom-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.193320 quom-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/src/quom/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/quom.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/quom_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/src/quom/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/comment_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/number_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/preprocessor_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/quote_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/remaining_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/tokenize_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-15 10:54:20.000000 quom-4.0.0/src/quom/tokenizer/whitespace_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/src/quom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 10:54:33.000000 quom-4.0.0/src/quom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:20.000000 quom-4.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:54:33.201320 quom-4.0.0/tests/test_quom/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/same_file_different_include.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_file_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_file_without_include_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_include_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_last_source_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_line_breaks_when_stitching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_quom/test_source_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-15 10:54:20.000000 quom-4.0.0/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 10:54:20.000000 quom-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.436357 quom-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.424357 quom-4.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-15 11:10:40.000000 quom-4.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-15 11:10:40.000000 quom-4.0.1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-15 11:10:40.000000 quom-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-15 11:10:40.000000 quom-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-15 11:10:53.436357 quom-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-15 11:10:40.000000 quom-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/artwork/
+-rw-r--r--   0 runner    (1001) docker     (123)   313993 2023-04-15 11:10:40.000000 quom-4.0.1/artwork/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   180297 2023-04-15 11:10:40.000000 quom-4.0.1/artwork/logo_banner.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/examples/flat_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/foobar_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/examples/flat_structure/libfoobar/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/bar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/bar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/foo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/foo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/foobar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 11:10:40.000000 quom-4.0.1/examples/flat_structure/libfoobar/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/examples/include_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/foobar_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/examples/include_directory/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.432357 quom-4.0.1/examples/include_directory/include/libfoobar/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/bar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/bar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/foo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/foo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/foobar.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 11:10:40.000000 quom-4.0.1/examples/include_directory/include/libfoobar/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-15 11:10:53.436357 quom-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 11:10:40.000000 quom-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.428357 quom-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.432357 quom-4.0.1/src/quom/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/quom.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/quom_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.432357 quom-4.0.1/src/quom/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/comment_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/number_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/preprocessor_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/quote_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/remaining_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/tokenize_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-15 11:10:40.000000 quom-4.0.1/src/quom/tokenizer/whitespace_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.432357 quom-4.0.1/src/quom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-15 11:10:53.000000 quom-4.0.1/src/quom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-15 11:10:53.000000 quom-4.0.1/src/quom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:10:53.000000 quom-4.0.1/src/quom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 11:10:53.000000 quom-4.0.1/src/quom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:10:53.000000 quom-4.0.1/src/quom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-15 11:10:53.000000 quom-4.0.1/src/quom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 11:10:53.000000 quom-4.0.1/src/quom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.432357 quom-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:40.000000 quom-4.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:10:53.436357 quom-4.0.1/tests/test_quom/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/same_file_different_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/test_file_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/test_file_without_include_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/test_include_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/test_last_source_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/test_line_breaks_when_stitching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/test_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_quom/test_source_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-15 11:10:40.000000 quom-4.0.1/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 11:10:40.000000 quom-4.0.1/tox.ini
```

### Comparing `quom-4.0.0/.github/workflows/publish.yml` & `quom-4.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/.github/workflows/testing.yml` & `quom-4.0.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/.gitignore` & `quom-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/LICENSE` & `quom-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/PKG-INFO` & `quom-4.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: quom
-Version: 4.0.0
+Version: 4.0.1
 Summary: Quom is a single header generator for C/C++ libraries.
 Home-page: https://github.com/Viatorus/quom
 Author: Toni Neubert
 Author-email: lutztonineubert@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Viatorus/quom
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE
 
 ![logo](https://raw.githubusercontent.com/Viatorus/quom/master/artwork/logo_banner.png)
 
 [![Build Status](https://github.com/Viatorus/quom/workflows/Testing/badge.svg)](https://github.com/viatorus/quom/actions)
@@ -35,15 +35,15 @@
 
 ## Installation
 
 ```
 pip install --user quom
 ```
 
-Only **Python 3.6+** is supported.
+Requires Python 3.7 or later.
 
 ## How to use it
 
 ```
 usage: quom [-h] [--stitch format] [--include_guard format] [--trim]
             input output
```

### Comparing `quom-4.0.0/README.md` & `quom-4.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ## Installation
 
 ```
 pip install --user quom
 ```
 
-Only **Python 3.6+** is supported.
+Requires Python 3.7 or later.
 
 ## How to use it
 
 ```
 usage: quom [-h] [--stitch format] [--include_guard format] [--trim]
             input output
```

### Comparing `quom-4.0.0/artwork/logo.png` & `quom-4.0.1/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/artwork/logo_banner.png` & `quom-4.0.1/artwork/logo_banner.png`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/examples/flat_structure/foobar_gen.hpp` & `quom-4.0.1/examples/flat_structure/foobar_gen.hpp`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/examples/include_directory/foobar_gen.hpp` & `quom-4.0.1/examples/include_directory/foobar_gen.hpp`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/setup.cfg` & `quom-4.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools_scm
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `quom-4.0.0/setup.py` & `quom-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/__init__.py` & `quom-4.0.1/src/quom/__init__.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/__main__.py` & `quom-4.0.1/src/quom/__main__.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/quom.py` & `quom-4.0.1/src/quom/quom.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/__init__.py` & `quom-4.0.1/src/quom/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/comment_tokenizer.py` & `quom-4.0.1/src/quom/tokenizer/comment_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/iterator.py` & `quom-4.0.1/src/quom/tokenizer/iterator.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/number_tokenizer.py` & `quom-4.0.1/src/quom/tokenizer/number_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/preprocessor_tokenizer.py` & `quom-4.0.1/src/quom/tokenizer/preprocessor_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/quote_tokenizer.py` & `quom-4.0.1/src/quom/tokenizer/quote_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/remaining_tokenizer.py` & `quom-4.0.1/src/quom/tokenizer/remaining_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/token.py` & `quom-4.0.1/src/quom/tokenizer/token.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/tokenize.py` & `quom-4.0.1/src/quom/tokenizer/tokenize.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom/tokenizer/whitespace_tokenizer.py` & `quom-4.0.1/src/quom/tokenizer/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/src/quom.egg-info/PKG-INFO` & `quom-4.0.1/src/quom.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: quom
-Version: 4.0.0
+Version: 4.0.1
 Summary: Quom is a single header generator for C/C++ libraries.
 Home-page: https://github.com/Viatorus/quom
 Author: Toni Neubert
 Author-email: lutztonineubert@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Viatorus/quom
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE
 
 ![logo](https://raw.githubusercontent.com/Viatorus/quom/master/artwork/logo_banner.png)
 
 [![Build Status](https://github.com/Viatorus/quom/workflows/Testing/badge.svg)](https://github.com/viatorus/quom/actions)
@@ -35,15 +35,15 @@
 
 ## Installation
 
 ```
 pip install --user quom
 ```
 
-Only **Python 3.6+** is supported.
+Requires Python 3.7 or later.
 
 ## How to use it
 
 ```
 usage: quom [-h] [--stitch format] [--include_guard format] [--trim]
             input output
```

### Comparing `quom-4.0.0/src/quom.egg-info/SOURCES.txt` & `quom-4.0.1/src/quom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_iterator.py` & `quom-4.0.1/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/same_file_different_include.py` & `quom-4.0.1/tests/test_quom/same_file_different_include.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/test_file_encoding.py` & `quom-4.0.1/tests/test_quom/test_file_encoding.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/test_file_without_include_guard.py` & `quom-4.0.1/tests/test_quom/test_file_without_include_guard.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/test_include_directory.py` & `quom-4.0.1/tests/test_quom/test_include_directory.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/test_last_source_file.py` & `quom-4.0.1/tests/test_quom/test_last_source_file.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/test_line_breaks_when_stitching.py` & `quom-4.0.1/tests/test_quom/test_line_breaks_when_stitching.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/test_normal.py` & `quom-4.0.1/tests/test_quom/test_normal.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_quom/test_source_directory.py` & `quom-4.0.1/tests/test_quom/test_source_directory.py`

 * *Files identical despite different names*

### Comparing `quom-4.0.0/tests/test_tokenizer.py` & `quom-4.0.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

