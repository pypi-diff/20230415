# Comparing `tmp/mash-shell-0.2.2.tar.gz` & `tmp/mash-shell-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mash-shell-0.2.2.tar", last modified: Tue Apr 11 19:58:05 2023, max compression
+gzip compressed data, was "mash-shell-0.2.3.tar", last modified: Sat Apr 15 11:45:22 2023, max compression
```

## Comparing `mash-shell-0.2.2.tar` & `mash-shell-0.2.3.tar`

### file list

```diff
@@ -1,73 +1,83 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.767710 mash-shell-0.2.2/
--rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.2/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)     8174 2023-04-11 19:58:05.767215 mash-shell-0.2.2/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     7606 2023-04-11 19:57:54.000000 mash-shell-0.2.2/README.md
--rw-r--r--   0 mark       (501) staff       (20)      736 2023-04-11 19:57:54.000000 mash-shell-0.2.2/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.2/requirements.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-11 19:58:05.767826 mash-shell-0.2.2/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.722658 mash-shell-0.2.2/src/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.732631 mash-shell-0.2.2/src/examples/
--rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/_extend_path.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/discoverable.py
--rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-22 06:58:11.000000 mash-shell-0.2.2/src/examples/discoverable_api.py
--rw-r--r--   0 mark       (501) staff       (20)     1004 2023-04-08 06:46:34.000000 mash-shell-0.2.2/src/examples/discoverable_with_oas.py
--rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     1126 2023-03-24 06:51:08.000000 mash-shell-0.2.2/src/examples/ms_graph_api.py
--rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/examples/object_parser.py
--rwxr-xr-x   0 mark       (501) staff       (20)     1324 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/examples/shell_example.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.743519 mash-shell-0.2.2/src/mash/
--rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/__main__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.2/src/mash/cli.py
--rw-r--r--   0 mark       (501) staff       (20)     2479 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/doc_inference.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.746314 mash-shell-0.2.2/src/mash/filesystem/
--rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/filesystem/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     6953 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/filesystem/discoverable.py
--rw-r--r--   0 mark       (501) staff       (20)    10629 2023-04-10 07:54:42.000000 mash-shell-0.2.2/src/mash/filesystem/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.2/src/mash/filesystem/scope.py
--rw-r--r--   0 mark       (501) staff       (20)     4627 2023-03-24 08:15:55.000000 mash-shell-0.2.2/src/mash/filesystem/view.py
--rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/html_table_data.py
--rw-r--r--   0 mark       (501) staff       (20)     5161 2023-03-24 07:32:34.000000 mash-shell-0.2.2/src/mash/io_util.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.750594 mash-shell-0.2.2/src/mash/object_parser/
--rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/factory.py
--rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/oas.py
--rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.2/src/mash/object_parser/object_parser.py
--rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/object_parser_standards.py
--rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser/spec.py
--rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/object_parser_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/parallel.py
--rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/parallel_requests.py
--rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.760913 mash-shell-0.2.2/src/mash/shell/
--rw-r--r--   0 mark       (501) staff       (20)      215 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    11161 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/base.py
--rw-r--r--   0 mark       (501) staff       (20)     6357 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/cmd2.py
--rw-r--r--   0 mark       (501) staff       (20)     1035 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/delimiters.py
--rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.2/src/mash/shell/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     2140 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/function.py
--rw-r--r--   0 mark       (501) staff       (20)     2310 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/if_statement.py
--rw-r--r--   0 mark       (501) staff       (20)    13323 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/lex_parser.py
--rw-r--r--   0 mark       (501) staff       (20)    25476 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/model.py
--rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-10 18:49:45.000000 mash-shell-0.2.2/src/mash/shell/parsetab.py
--rw-r--r--   0 mark       (501) staff       (20)     4083 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/parsing.py
--rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/shell/progress_bar.py
--rwxr-xr-x   0 mark       (501) staff       (20)    11434 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/shell.py
--rw-r--r--   0 mark       (501) staff       (20)     6367 2023-04-11 19:57:54.000000 mash-shell-0.2.2/src/mash/shell/with_filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3229 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/subshell.py
--rw-r--r--   0 mark       (501) staff       (20)    18188 2023-04-11 18:51:45.000000 mash-shell-0.2.2/src/mash/util.py
--rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.2/src/mash/verify_server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.763275 mash-shell-0.2.2/src/mash_shell.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     8174 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1695 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       18 2023-04-11 19:58:05.000000 mash-shell-0.2.2/src/mash_shell.egg-info/top_level.txt
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-11 19:58:05.766685 mash-shell-0.2.2/test/
--rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.2/test/test_html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.2/test/test_parallel.py
--rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.2/test/test_pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.2/test/test_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.2/test/test_util.py
--rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.2/test/test_verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.619166 mash-shell-0.2.3/
+-rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.3/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)     8540 2023-04-15 11:45:22.618536 mash-shell-0.2.3/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     7972 2023-04-15 11:43:13.000000 mash-shell-0.2.3/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      736 2023-04-15 11:45:13.000000 mash-shell-0.2.3/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.3/requirements.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-15 11:45:22.619287 mash-shell-0.2.3/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.575105 mash-shell-0.2.3/src/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.584105 mash-shell-0.2.3/src/examples/
+-rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/examples/_extend_path.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/examples/discoverable.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-22 06:58:11.000000 mash-shell-0.2.3/src/examples/discoverable_api.py
+-rw-r--r--   0 mark       (501) staff       (20)     1004 2023-04-08 06:46:34.000000 mash-shell-0.2.3/src/examples/discoverable_with_oas.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/examples/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     1126 2023-03-24 06:51:08.000000 mash-shell-0.2.3/src/examples/ms_graph_api.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/examples/object_parser.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     1324 2023-04-11 19:57:54.000000 mash-shell-0.2.3/src/examples/shell_example.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.593268 mash-shell-0.2.3/src/mash/
+-rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/__main__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.3/src/mash/cli.py
+-rw-r--r--   0 mark       (501) staff       (20)     2479 2023-04-11 19:57:54.000000 mash-shell-0.2.3/src/mash/doc_inference.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.596269 mash-shell-0.2.3/src/mash/filesystem/
+-rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/filesystem/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     6953 2023-04-11 19:57:54.000000 mash-shell-0.2.3/src/mash/filesystem/discoverable.py
+-rw-r--r--   0 mark       (501) staff       (20)    10629 2023-04-10 07:54:42.000000 mash-shell-0.2.3/src/mash/filesystem/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.3/src/mash/filesystem/scope.py
+-rw-r--r--   0 mark       (501) staff       (20)     4627 2023-03-24 08:15:55.000000 mash-shell-0.2.3/src/mash/filesystem/view.py
+-rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/html_table_data.py
+-rw-r--r--   0 mark       (501) staff       (20)     5161 2023-03-24 07:32:34.000000 mash-shell-0.2.3/src/mash/io_util.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.599605 mash-shell-0.2.3/src/mash/object_parser/
+-rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/object_parser/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/object_parser/factory.py
+-rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/object_parser/oas.py
+-rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.3/src/mash/object_parser/object_parser.py
+-rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/object_parser/object_parser_standards.py
+-rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/object_parser/spec.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/object_parser_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/parallel_requests.py
+-rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.605173 mash-shell-0.2.3/src/mash/shell/
+-rw-r--r--   0 mark       (501) staff       (20)      215 2023-04-11 19:57:54.000000 mash-shell-0.2.3/src/mash/shell/__init__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.609562 mash-shell-0.2.3/src/mash/shell/ast/
+-rw-r--r--   0 mark       (501) staff       (20)      880 2023-04-15 11:14:26.000000 mash-shell-0.2.3/src/mash/shell/ast/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     4676 2023-04-15 11:25:07.000000 mash-shell-0.2.3/src/mash/shell/ast/conditions.py
+-rw-r--r--   0 mark       (501) staff       (20)     1740 2023-04-15 11:25:14.000000 mash-shell-0.2.3/src/mash/shell/ast/function_definition.py
+-rw-r--r--   0 mark       (501) staff       (20)     5562 2023-04-15 11:24:16.000000 mash-shell-0.2.3/src/mash/shell/ast/infix.py
+-rw-r--r--   0 mark       (501) staff       (20)     4715 2023-04-15 11:22:48.000000 mash-shell-0.2.3/src/mash/shell/ast/node.py
+-rw-r--r--   0 mark       (501) staff       (20)     2779 2023-04-15 11:24:58.000000 mash-shell-0.2.3/src/mash/shell/ast/nodes.py
+-rw-r--r--   0 mark       (501) staff       (20)     3138 2023-04-15 11:24:48.000000 mash-shell-0.2.3/src/mash/shell/ast/term.py
+-rw-r--r--   0 mark       (501) staff       (20)    10999 2023-04-15 11:22:15.000000 mash-shell-0.2.3/src/mash/shell/base.py
+-rw-r--r--   0 mark       (501) staff       (20)     6330 2023-04-15 10:44:24.000000 mash-shell-0.2.3/src/mash/shell/cmd2.py
+-rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.3/src/mash/shell/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     2140 2023-04-15 11:17:46.000000 mash-shell-0.2.3/src/mash/shell/function.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.611675 mash-shell-0.2.3/src/mash/shell/grammer/
+-rw-r--r--   0 mark       (501) staff       (20)     1018 2023-04-15 08:36:37.000000 mash-shell-0.2.3/src/mash/shell/grammer/delimiters.py
+-rw-r--r--   0 mark       (501) staff       (20)    13517 2023-04-15 11:21:14.000000 mash-shell-0.2.3/src/mash/shell/grammer/lex_yacc.py
+-rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-15 11:17:58.000000 mash-shell-0.2.3/src/mash/shell/grammer/parsetab.py
+-rw-r--r--   0 mark       (501) staff       (20)     4085 2023-04-15 11:21:01.000000 mash-shell-0.2.3/src/mash/shell/grammer/parsing.py
+-rw-r--r--   0 mark       (501) staff       (20)     4560 2023-04-15 11:25:31.000000 mash-shell-0.2.3/src/mash/shell/helpers.py
+-rw-r--r--   0 mark       (501) staff       (20)     2348 2023-04-15 11:24:38.000000 mash-shell-0.2.3/src/mash/shell/if_statement.py
+-rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-10 18:49:45.000000 mash-shell-0.2.3/src/mash/shell/parsetab.py
+-rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/shell/progress_bar.py
+-rwxr-xr-x   0 mark       (501) staff       (20)    11576 2023-04-15 11:21:55.000000 mash-shell-0.2.3/src/mash/shell/shell.py
+-rw-r--r--   0 mark       (501) staff       (20)     6367 2023-04-11 19:57:54.000000 mash-shell-0.2.3/src/mash/shell/with_filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3229 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/subshell.py
+-rw-r--r--   0 mark       (501) staff       (20)    18188 2023-04-11 18:51:45.000000 mash-shell-0.2.3/src/mash/util.py
+-rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.3/src/mash/verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.614071 mash-shell-0.2.3/src/mash_shell.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     8540 2023-04-15 11:45:22.000000 mash-shell-0.2.3/src/mash_shell.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1970 2023-04-15 11:45:22.000000 mash-shell-0.2.3/src/mash_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-15 11:45:22.000000 mash-shell-0.2.3/src/mash_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-04-15 11:45:22.000000 mash-shell-0.2.3/src/mash_shell.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       18 2023-04-15 11:45:22.000000 mash-shell-0.2.3/src/mash_shell.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-15 11:45:22.617816 mash-shell-0.2.3/test/
+-rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.3/test/test_html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.3/test/test_parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.3/test/test_pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.3/test/test_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.3/test/test_util.py
+-rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.3/test/test_verify_server.py
```

### Comparing `mash-shell-0.2.2/LICENSE` & `mash-shell-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/PKG-INFO` & `mash-shell-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mash-shell
-Version: 0.2.2
+Version: 0.2.3
 Summary: A shell and other utils
 Author-email: voschezang <mark.voschezang@student.uva.nl>
 Project-URL: Homepage, https://github.com/voschezang/mash
 Project-URL: Bug Tracker, https://github.com/voschezang/mash/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -36,14 +36,15 @@
 - A **REST client** to browse APIs with a programmatic yet intuitive interface: `examples/discoverable_api.py`.
 - An **object parser** which converts JSON data to Python classes: `object_parser.py`.
 - An **OAS-generator** for Python classes: `oas.py`.
 - A subshell wrapper, to redirect the output of shell scripts: `subshell.py`.
 - A parallelization framework for load testing: `parallel.py`.
 
 Links
+- [Mash language reference](SHELL_REFERENCE.md)
 - [PyPI](https://pypi.org/project/mash-shell)
 - [github](https://github.com/voschezang/mash)
 
 ## Shell
 
 <img src="https://github.com/voschezang/mash/blob/main/img/shell_dropdown.png?raw=true" style="max-height: 180px;" alt="Example of a shell with a dropdown completion menu"></img>
 
@@ -56,15 +57,23 @@
 See [`src/examples`](src/examples) for advances usage examples.
 
 **Documentation**
 
 - Implementation: [SHELL.md](https://github.com/voschezang/mash/blob/main/SHELL.md)
 - Language: [REFERENCE.md](https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md).
 
+**Table of Contents**
 
+- [Usage](#Usage)
+    - [CLI](#CLI)
+    - [Filesystem (CRUD Operations)](#Filesystem%20(CRUD%20Operations))
+    - [Usage Examples](#Usage%20Examples)
+- [Library & Tools](#Library%20&%20Tools)
+    - [Parallelization Utilities](#Parallelization%20Utilities)
+    - [Object Parser](#Object%20Parser)
 
 # Usage
 
 See [reference](SHELL_REFERENCE.md).
 
 ### CLI
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mash-shell Version: 0.2.2 Summary: A shell and
+Metadata-Version: 2.1 Name: mash-shell Version: 0.2.3 Summary: A shell and
 other utils Author-email: voschezang
 voschezang@student.uva.nl> Project-URL: Homepage, https://github.com/
 voschezang/mash Project-URL: Bug Tracker, https://github.com/voschezang/mash/
 issues Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 System :: Shells Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE !
@@ -24,21 +24,26 @@
 utilities. Features: - A **DSL** that can interpret user-defined commands:
 `shell.py`. - A **file-browser**. Query both static datastructures and REST
 APIs: `examples/filesystem.py`, - A **REST client** to browse APIs with a
 programmatic yet intuitive interface: `examples/discoverable_api.py`. - An
 **object parser** which converts JSON data to Python classes:
 `object_parser.py`. - An **OAS-generator** for Python classes: `oas.py`. - A
 subshell wrapper, to redirect the output of shell scripts: `subshell.py`. - A
-parallelization framework for load testing: `parallel.py`. Links - [PyPI]
-(https://pypi.org/project/mash-shell) - [github](https://github.com/voschezang/
-mash) ## Shell [Example of a shell with a dropdown completion menu] ```sh pip
-install mash-shell python -m mash ``` See [`src/examples`](src/examples) for
-advances usage examples. **Documentation** - Implementation: [SHELL.md](https:/
-/github.com/voschezang/mash/blob/main/SHELL.md) - Language: [REFERENCE.md]
-(https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md). # Usage See
+parallelization framework for load testing: `parallel.py`. Links - [Mash
+language reference](SHELL_REFERENCE.md) - [PyPI](https://pypi.org/project/mash-
+shell) - [github](https://github.com/voschezang/mash) ## Shell [Example of a
+shell with a dropdown completion menu] ```sh pip install mash-shell python -
+m mash ``` See [`src/examples`](src/examples) for advances usage examples.
+**Documentation** - Implementation: [SHELL.md](https://github.com/voschezang/
+mash/blob/main/SHELL.md) - Language: [REFERENCE.md](https://github.com/
+voschezang/mash/blob/main/SHELL_REFERENCE.md). **Table of Contents** - [Usage]
+(#Usage) - [CLI](#CLI) - [Filesystem (CRUD Operations)](#Filesystem%20
+(CRUD%20Operations)) - [Usage Examples](#Usage%20Examples) - [Library & Tools]
+(#Library%20&%20Tools) - [Parallelization Utilities]
+(#Parallelization%20Utilities) - [Object Parser](#Object%20Parser) # Usage See
 [reference](SHELL_REFERENCE.md). ### CLI ```sh â¶ python -m mash -h usage:
 shell.py [-hvsr][-f FILE] [--session SESSION] [cmd [cmd ...]] If no positional
 arguments are given then an interactive subshell is started. positional
 arguments: cmd A comma- or newline-separated list of commands optional
 arguments: -h, --help show this help message and exit -v, --verbose -s, --safe
 Safe-mode. Ask for confirmation before executing commands. -f FILE, --file FILE
 Read and run FILE as a commands -r, --reload Reload last session --session
```

### Comparing `mash-shell-0.2.2/README.md` & `mash-shell-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 - A **REST client** to browse APIs with a programmatic yet intuitive interface: `examples/discoverable_api.py`.
 - An **object parser** which converts JSON data to Python classes: `object_parser.py`.
 - An **OAS-generator** for Python classes: `oas.py`.
 - A subshell wrapper, to redirect the output of shell scripts: `subshell.py`.
 - A parallelization framework for load testing: `parallel.py`.
 
 Links
+- [Mash language reference](SHELL_REFERENCE.md)
 - [PyPI](https://pypi.org/project/mash-shell)
 - [github](https://github.com/voschezang/mash)
 
 ## Shell
 
 <img src="https://github.com/voschezang/mash/blob/main/img/shell_dropdown.png?raw=true" style="max-height: 180px;" alt="Example of a shell with a dropdown completion menu"></img>
 
@@ -41,15 +42,23 @@
 See [`src/examples`](src/examples) for advances usage examples.
 
 **Documentation**
 
 - Implementation: [SHELL.md](https://github.com/voschezang/mash/blob/main/SHELL.md)
 - Language: [REFERENCE.md](https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md).
 
+**Table of Contents**
 
+- [Usage](#Usage)
+    - [CLI](#CLI)
+    - [Filesystem (CRUD Operations)](#Filesystem%20(CRUD%20Operations))
+    - [Usage Examples](#Usage%20Examples)
+- [Library & Tools](#Library%20&%20Tools)
+    - [Parallelization Utilities](#Parallelization%20Utilities)
+    - [Object Parser](#Object%20Parser)
 
 # Usage
 
 See [reference](SHELL_REFERENCE.md).
 
 ### CLI
```

#### html2text {}

```diff
@@ -16,21 +16,26 @@
 utilities. Features: - A **DSL** that can interpret user-defined commands:
 `shell.py`. - A **file-browser**. Query both static datastructures and REST
 APIs: `examples/filesystem.py`, - A **REST client** to browse APIs with a
 programmatic yet intuitive interface: `examples/discoverable_api.py`. - An
 **object parser** which converts JSON data to Python classes:
 `object_parser.py`. - An **OAS-generator** for Python classes: `oas.py`. - A
 subshell wrapper, to redirect the output of shell scripts: `subshell.py`. - A
-parallelization framework for load testing: `parallel.py`. Links - [PyPI]
-(https://pypi.org/project/mash-shell) - [github](https://github.com/voschezang/
-mash) ## Shell [Example of a shell with a dropdown completion menu] ```sh pip
-install mash-shell python -m mash ``` See [`src/examples`](src/examples) for
-advances usage examples. **Documentation** - Implementation: [SHELL.md](https:/
-/github.com/voschezang/mash/blob/main/SHELL.md) - Language: [REFERENCE.md]
-(https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md). # Usage See
+parallelization framework for load testing: `parallel.py`. Links - [Mash
+language reference](SHELL_REFERENCE.md) - [PyPI](https://pypi.org/project/mash-
+shell) - [github](https://github.com/voschezang/mash) ## Shell [Example of a
+shell with a dropdown completion menu] ```sh pip install mash-shell python -
+m mash ``` See [`src/examples`](src/examples) for advances usage examples.
+**Documentation** - Implementation: [SHELL.md](https://github.com/voschezang/
+mash/blob/main/SHELL.md) - Language: [REFERENCE.md](https://github.com/
+voschezang/mash/blob/main/SHELL_REFERENCE.md). **Table of Contents** - [Usage]
+(#Usage) - [CLI](#CLI) - [Filesystem (CRUD Operations)](#Filesystem%20
+(CRUD%20Operations)) - [Usage Examples](#Usage%20Examples) - [Library & Tools]
+(#Library%20&%20Tools) - [Parallelization Utilities]
+(#Parallelization%20Utilities) - [Object Parser](#Object%20Parser) # Usage See
 [reference](SHELL_REFERENCE.md). ### CLI ```sh â¶ python -m mash -h usage:
 shell.py [-hvsr][-f FILE] [--session SESSION] [cmd [cmd ...]] If no positional
 arguments are given then an interactive subshell is started. positional
 arguments: cmd A comma- or newline-separated list of commands optional
 arguments: -h, --help show this help message and exit -v, --verbose -s, --safe
 Safe-mode. Ask for confirmation before executing commands. -f FILE, --file FILE
 Read and run FILE as a commands -r, --reload Reload last session --session
```

### Comparing `mash-shell-0.2.2/pyproject.toml` & `mash-shell-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mash-shell"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="voschezang", email="mark.voschezang@student.uva.nl" },
 ]
 description = "A shell and other utils"
 dynamic = ["dependencies"]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mash-shell-0.2.2/src/examples/discoverable.py` & `mash-shell-0.2.3/src/examples/discoverable.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/examples/discoverable_api.py` & `mash-shell-0.2.3/src/examples/discoverable_api.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/examples/discoverable_with_oas.py` & `mash-shell-0.2.3/src/examples/discoverable_with_oas.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/examples/filesystem.py` & `mash-shell-0.2.3/src/examples/filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/examples/ms_graph_api.py` & `mash-shell-0.2.3/src/examples/ms_graph_api.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/examples/object_parser.py` & `mash-shell-0.2.3/src/examples/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/examples/shell_example.py` & `mash-shell-0.2.3/src/examples/shell_example.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/cli.py` & `mash-shell-0.2.3/src/mash/cli.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/doc_inference.py` & `mash-shell-0.2.3/src/mash/doc_inference.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/filesystem/discoverable.py` & `mash-shell-0.2.3/src/mash/filesystem/discoverable.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/filesystem/filesystem.py` & `mash-shell-0.2.3/src/mash/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/filesystem/scope.py` & `mash-shell-0.2.3/src/mash/filesystem/scope.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/filesystem/view.py` & `mash-shell-0.2.3/src/mash/filesystem/view.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/html_table.py` & `mash-shell-0.2.3/src/mash/html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/html_table_data.py` & `mash-shell-0.2.3/src/mash/html_table_data.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/io_util.py` & `mash-shell-0.2.3/src/mash/io_util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/object_parser/errors.py` & `mash-shell-0.2.3/src/mash/object_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/object_parser/factory.py` & `mash-shell-0.2.3/src/mash/object_parser/factory.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/object_parser/oas.py` & `mash-shell-0.2.3/src/mash/object_parser/oas.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/object_parser/object_parser.py` & `mash-shell-0.2.3/src/mash/object_parser/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/object_parser/object_parser_standards.py` & `mash-shell-0.2.3/src/mash/object_parser/object_parser_standards.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/object_parser/spec.py` & `mash-shell-0.2.3/src/mash/object_parser/spec.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/object_parser_server.py` & `mash-shell-0.2.3/src/mash/object_parser_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/parallel.py` & `mash-shell-0.2.3/src/mash/parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/parallel_requests.py` & `mash-shell-0.2.3/src/mash/parallel_requests.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/pipeline.py` & `mash-shell-0.2.3/src/mash/pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/server.py` & `mash-shell-0.2.3/src/mash/server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/shell/base.py` & `mash-shell-0.2.3/src/mash/shell/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,45 +4,41 @@
 from typing import Any, Callable, Dict, List
 import logging
 
 from mash.shell.cmd2 import Cmd2
 from mash.filesystem.filesystem import FileSystem
 from mash.filesystem.scope import Scope, show
 from mash.io_util import log, print_shell_ready_signal
-from mash.shell import delimiters
-from mash.shell.delimiters import FALSE, IF, TRUE
+from mash.shell.grammer import delimiters
+from mash.shell.grammer.delimiters import FALSE, IF, TRUE
 from mash.shell.errors import ShellError
 from mash.shell.function import LAST_RESULTS, LAST_RESULTS_INDEX, InlineFunction, scope
 from mash.shell.function import ShellFunction as Function
-from mash.shell.parsing import to_bool
+from mash.shell.grammer.parsing import to_bool
 from mash.util import has_method, identity
 
 
 default_session_filename = '.shell_session.json'
 default_function_group_key = '_'
 
 ENV = 'env'
 CHAR = 'char'
 
 Command = Callable[[Cmd2, str], str]
 FunctionGroup = Dict[str, Dict[str, Function]]
 
 
 class BaseShell(Cmd2):
-    """Extend CMD with various capabilities.
-    This class is restricted to functionality that requires Cmd methods to be overrride.
+    """Extend Cmd with various capabilities.
+    This class is restricted to functionality that requires Cmd methods to be overrriden.
 
     Features:
-    - Parsing of multi-line and multi-segment commands.
-        - Chain commands using pipes.
-        - Interop between Python and e.g. Bash using pipes.
-    - Parsing of single commands.
-        - Set/unset variables, retrieve variable values.
-    - Confirmation mode to allow a user to accept or decline commands.
-    - Error handling.
+    - An environment with local and global variable scopes.
+    - Save/load sessions.
+    - Decotion with functions, both at runtime and compile time.
     """
 
     def __init__(self, *args, env: Dict[str, Any] = None,
                  use_model=True,
                  save_session_prehook=identity,
                  load_session_posthook=identity, **kwds):
         """
```

### Comparing `mash-shell-0.2.2/src/mash/shell/cmd2.py` & `mash-shell-0.2.3/src/mash/shell/cmd2.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,14 @@
     ----------
         strict : bool
             Raise exceptions when encountering invalid syntax.
     """
     if strict is not None:
         shell.ignore_invalid_syntax = not strict
 
-    # TODO skip splitlines
     for line in command.splitlines():
         if line:
             shell.onecmd(line)
 
 
 def run_commands_from_file(filename: str, shell: Cmd2):
     command = read_file(filename)
```

### Comparing `mash-shell-0.2.2/src/mash/shell/delimiters.py` & `mash-shell-0.2.3/src/mash/shell/grammer/delimiters.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 RETURN = Python.RETURN.value
 DEFINE_FUNCTION = Python.DEFINE_FUNCTION.value
 RIGHT_ASSIGNMENT = Python.RIGHT_ASSIGNMENT.value
 LEFT_ASSIGNMENT = Python.LEFT_ASSIGNMENT.value
 IF = Python.IF.value
 THEN = Python.THEN.value
 ELSE = Python.ELSE.value
-# AND = Python.AND.value
-# OR = Python.OR.value
+ELSE_IF_THEN = 'else-if-then'
+
 INLINE_THEN = 'inline-then'
 INLINE_ELSE = 'inline-else'
 
 
 class KeyWords(Enum):
     AND = 'and'
     OR = 'or'
```

### Comparing `mash-shell-0.2.2/src/mash/shell/function.py` & `mash-shell-0.2.3/src/mash/shell/function.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/shell/if_statement.py` & `mash-shell-0.2.3/src/mash/shell/if_statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from operator import contains
-from typing import Tuple
-from mash.shell.delimiters import ELSE, IF, INLINE_THEN, THEN
+from mash.shell.grammer.delimiters import ELSE, IF, THEN
 from mash.shell.errors import ShellError
 
 LINE_INDENT = 'line_indent'
 RAW_LINE_INDENT = 'raw_line_indent'
 
 
 class Abort(RuntimeError):
@@ -40,19 +38,21 @@
     for state in self.locals[IF][:-1]:
         if (state['value'] and state['branch'] == ELSE) or \
                 (not state['value'] and state['branch'] == THEN):
             raise Abort()
 
 
 def handle_else_statement(self, transparent=False):
-    if self._last_if['value'] is None:
-        raise Abort()
+    if not self.locals[IF]:
+        raise ShellError(f'Else clasue requires an {IF}-statement')
     elif self._last_if['branch'] is None:
         raise ShellError(
             f'If-then-else clause requires a {THEN} statement (3)')
+    elif self._last_if['value'] is None:
+        raise Abort()
 
     if not transparent:
         if not self.locals[IF]:
             raise ShellError(
                 f'If-then-else clause requires an {IF} statement (4)')
 
         self._last_if['branch'] = ELSE
```

### Comparing `mash-shell-0.2.2/src/mash/shell/lex_parser.py` & `mash-shell-0.2.3/src/mash/shell/grammer/lex_yacc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from logging import getLogger
 import ply.lex as lex
 import ply.yacc as yacc
-from mash.shell.model import Assign, BashPipe, BinaryExpression, Else, ElseIf, ElseIfThen, FunctionDefinition, If, IfThen, IfThenElse, Indent, InlineFunctionDefinition, Lines, LogicExpression, Map, Math, Method, Pipe, Quoted, Return, Shell, Terms, Then, Variable, Word
-from mash.shell.parsing import indent_width
+from mash.shell.ast import Assign, BashPipe, BinaryExpression, Else, ElseIf, ElseIfThen, FunctionDefinition, If, IfThen, IfThenElse, Indent, InlineFunctionDefinition, Lines, LogicExpression, Map, Math, Method, Pipe, Quoted, Return, Shell, Terms, Then, Variable, Word
+from mash.shell.grammer.parsing import indent_width
 from mash.shell.errors import ShellSyntaxError
 
 lexer = None
 
 tokens = (
     'BASH',  # | >>
     'SHELL',  # !
@@ -149,15 +149,20 @@
         return t
 
     def t_LONG_SYMBOL(t):
         r'\+\+|::|=>|~>|\|->'
         return t
 
     def t_MAP(t):
-        r'>>='
+        r'>>=|\|>\smap'
+        """Syntax for "map":
+            `f x >>= g`
+        or
+            `f x |> map g`
+        """
         return t
 
     def t_PIPE(t):
         r'\|>'
         return t
 
     def t_BASH(t):
@@ -354,15 +359,15 @@
     def p_then(p):
         """conditional : THEN final_statement
                        | THEN
         """
         if len(p) == 2:
             p[0] = Then()
         else:
-            p[0] = Then(p[2])
+            p[0] = Then(then=p[2])
 
     def p_else_if_then(p):
         """conditional : ELSE IF conjunction THEN final_statement
                       | ELSE IF conjunction THEN
         """
         if len(p) == 6:
             p[0] = ElseIfThen(p[3], p[5])
@@ -376,15 +381,15 @@
     def p_else(p):
         """conditional : ELSE final_statement
                        | ELSE
         """
         if len(p) == 2:
             p[0] = Else()
         else:
-            p[0] = Else(p[2])
+            p[0] = Else(otherwise=p[2])
 
     def p_conditional(p):
         """conditional : conjunction
                        | full_conditional
         """
         p[0] = p[1]
 
@@ -540,14 +545,17 @@
         global lexer
         lexer = init_lex()
     else:
         lexer.clone()
 
     log = getLogger()
     parser = yacc.yacc(debug=log)
+    if not isinstance(text, str):
+        text
+        raise
 
     # add a newline to allow empty strings to be matched
     return parser.parse('\n' + text)
 
 
 if __name__ == '__main__':
     data = """
```

### Comparing `mash-shell-0.2.2/src/mash/shell/parsetab.py` & `mash-shell-0.2.3/src/mash/shell/parsetab.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/shell/parsing.py` & `mash-shell-0.2.3/src/mash/shell/grammer/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from logging import debug
 from typing import Any, Iterable, List, Tuple
 import shlex
 
 from mash.io_util import log
-from mash.shell import delimiters
-from mash.shell.delimiters import FALSE, TRUE
+from mash.shell.grammer import delimiters
+from mash.shell.grammer.delimiters import FALSE, TRUE
 from mash.shell.errors import ShellError
-from mash.util import is_globbable, is_valid_method_name, match_words, quote, quote_all, removeprefix, glob
+from mash.util import is_globbable, is_valid_method_name, match_words, quote, quote_all, glob
 
 
 def expand_variables(terms: List[str], env: dict,
                      completenames_options: List[str],
                      ignore_invalid_syntax: bool,
                      wildcard_value='$',
                      escape=False) -> Iterable[str]:
```

### Comparing `mash-shell-0.2.2/src/mash/shell/shell.py` & `mash-shell-0.2.3/src/mash/shell/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from typing import Callable, Dict, Iterable, List, Tuple
 import logging
 import os
 import sys
 
 from mash import io_util
 from mash.io_util import ArgparseWrapper, bold, has_argument, has_output, log, log_once
-from mash.shell.model import LAST_RESULTS, ElseCondition, Indent, Lines, Map, Math, Node, Term, Terms
+from mash.shell.function import LAST_RESULTS
+from mash.shell.ast import ElseCondition, Indent, Lines, Map, Math, Node, Term, Terms
 from mash.shell.base import BaseShell
 from mash.shell.cmd2 import default_prompt, run
-from mash.shell.delimiters import DEFINE_FUNCTION
+from mash.shell.grammer.delimiters import DEFINE_FUNCTION
 from mash.shell.errors import ShellError, ShellPipeError, ShellSyntaxError
 from mash.shell.errors import ShellSyntaxError
 from mash.shell.function import ShellFunction as Function
 from mash.shell.if_statement import Abort, handle_prev_then_else_statements
-from mash.shell.lex_parser import parse
+from mash.shell.grammer.lex_yacc import parse
 from mash.util import has_method, is_valid_method_name
 
 description = 'If no positional arguments are given then an interactive subshell is started.'
 epilog = f"""
 --------------------------------------------------------------------------------
 {bold('Default Commands')}
 Run shell commands by prefixing them with `!`.
@@ -57,17 +58,14 @@
     ./shell.py print abc # Python
     ./shell.py 'print abc | echo'
     ./shell.py 'print abc |> print'
 """
 
 
 class Shell(BaseShell):
-    """Extend BaseShell(Cmd) with helper functions.
-    """
-
     def onecmd_inner(self, lines: str):
         if not self.use_model:
             return super().onecmd_inner(lines)
 
         ast = parse(lines)
         if ast is None:
             raise ShellError('Invalid syntax: AST is empty')
@@ -153,28 +151,38 @@
         # SMELL avoid circular import: base => model => lex_parser => model
         return parse(results)
 
     ############################################################################
     # Commands: do_*
     ############################################################################
 
-    def do_map(self, args=''):
-        """Apply a function to every line.
+    def do_map(self, line=''):
+        """Apply a function to each item.
+        It can be used as prefix or infix operator.
+
+        Usage (prefix)
+        --------------
+            `map f x y z` 
+
+        Usage (infix)
+        -------------
+            `f x |> map g`
+            `f x |> map g $ a b`
+            `f x >>= g`
+
         If `$` is present, then each line from stdin is inserted there.
         Otherwise each line is appended.
-
-        Usage
-        -----
-        ```sh
-        println a b |> map echo
-        println a b |> map echo prefix $ suffix
-        ```
         """
-        log('Expected arguments')
-        return ''
+        items = line.split(' ')
+        if len(items) < 2:
+            raise ShellError('Expected multiple arguments')
+
+        f, *args = items
+        for arg in args:
+            self.onecmd(f'{f} {arg}')
 
     def _do_foreach(self, ast: tuple, prev_results: str) -> Iterable:
         """Apply a function to every term or word.
 
         Usage
         ```sh
         echo a b |> foreach echo
@@ -259,20 +267,15 @@
     """
     if shell is None:
         shell = Shell()
 
     if strict is not None:
         shell.ignore_invalid_syntax = not strict
 
-    # TODO avoid splitines
-    # shell.onecmd(command)
-
-    for line in command.splitlines():
-        if line:
-            shell.onecmd(line)
+    shell.onecmd(command)
 
 
 def add_cli_args(parser: ArgumentParser):
     if not has_argument(parser, 'cmd'):
         parser.add_argument('cmd', nargs='*',
                             help='A comma- or newline-separated list of commands')
     if not has_argument(parser, 'safe'):
```

### Comparing `mash-shell-0.2.2/src/mash/shell/with_filesystem.py` & `mash-shell-0.2.3/src/mash/shell/with_filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/subshell.py` & `mash-shell-0.2.3/src/mash/subshell.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/util.py` & `mash-shell-0.2.3/src/mash/util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash/verify_server.py` & `mash-shell-0.2.3/src/mash/verify_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/src/mash_shell.egg-info/PKG-INFO` & `mash-shell-0.2.3/src/mash_shell.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mash-shell
-Version: 0.2.2
+Version: 0.2.3
 Summary: A shell and other utils
 Author-email: voschezang <mark.voschezang@student.uva.nl>
 Project-URL: Homepage, https://github.com/voschezang/mash
 Project-URL: Bug Tracker, https://github.com/voschezang/mash/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -36,14 +36,15 @@
 - A **REST client** to browse APIs with a programmatic yet intuitive interface: `examples/discoverable_api.py`.
 - An **object parser** which converts JSON data to Python classes: `object_parser.py`.
 - An **OAS-generator** for Python classes: `oas.py`.
 - A subshell wrapper, to redirect the output of shell scripts: `subshell.py`.
 - A parallelization framework for load testing: `parallel.py`.
 
 Links
+- [Mash language reference](SHELL_REFERENCE.md)
 - [PyPI](https://pypi.org/project/mash-shell)
 - [github](https://github.com/voschezang/mash)
 
 ## Shell
 
 <img src="https://github.com/voschezang/mash/blob/main/img/shell_dropdown.png?raw=true" style="max-height: 180px;" alt="Example of a shell with a dropdown completion menu"></img>
 
@@ -56,15 +57,23 @@
 See [`src/examples`](src/examples) for advances usage examples.
 
 **Documentation**
 
 - Implementation: [SHELL.md](https://github.com/voschezang/mash/blob/main/SHELL.md)
 - Language: [REFERENCE.md](https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md).
 
+**Table of Contents**
 
+- [Usage](#Usage)
+    - [CLI](#CLI)
+    - [Filesystem (CRUD Operations)](#Filesystem%20(CRUD%20Operations))
+    - [Usage Examples](#Usage%20Examples)
+- [Library & Tools](#Library%20&%20Tools)
+    - [Parallelization Utilities](#Parallelization%20Utilities)
+    - [Object Parser](#Object%20Parser)
 
 # Usage
 
 See [reference](SHELL_REFERENCE.md).
 
 ### CLI
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mash-shell Version: 0.2.2 Summary: A shell and
+Metadata-Version: 2.1 Name: mash-shell Version: 0.2.3 Summary: A shell and
 other utils Author-email: voschezang
 voschezang@student.uva.nl> Project-URL: Homepage, https://github.com/
 voschezang/mash Project-URL: Bug Tracker, https://github.com/voschezang/mash/
 issues Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 System :: Shells Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE !
@@ -24,21 +24,26 @@
 utilities. Features: - A **DSL** that can interpret user-defined commands:
 `shell.py`. - A **file-browser**. Query both static datastructures and REST
 APIs: `examples/filesystem.py`, - A **REST client** to browse APIs with a
 programmatic yet intuitive interface: `examples/discoverable_api.py`. - An
 **object parser** which converts JSON data to Python classes:
 `object_parser.py`. - An **OAS-generator** for Python classes: `oas.py`. - A
 subshell wrapper, to redirect the output of shell scripts: `subshell.py`. - A
-parallelization framework for load testing: `parallel.py`. Links - [PyPI]
-(https://pypi.org/project/mash-shell) - [github](https://github.com/voschezang/
-mash) ## Shell [Example of a shell with a dropdown completion menu] ```sh pip
-install mash-shell python -m mash ``` See [`src/examples`](src/examples) for
-advances usage examples. **Documentation** - Implementation: [SHELL.md](https:/
-/github.com/voschezang/mash/blob/main/SHELL.md) - Language: [REFERENCE.md]
-(https://github.com/voschezang/mash/blob/main/SHELL_REFERENCE.md). # Usage See
+parallelization framework for load testing: `parallel.py`. Links - [Mash
+language reference](SHELL_REFERENCE.md) - [PyPI](https://pypi.org/project/mash-
+shell) - [github](https://github.com/voschezang/mash) ## Shell [Example of a
+shell with a dropdown completion menu] ```sh pip install mash-shell python -
+m mash ``` See [`src/examples`](src/examples) for advances usage examples.
+**Documentation** - Implementation: [SHELL.md](https://github.com/voschezang/
+mash/blob/main/SHELL.md) - Language: [REFERENCE.md](https://github.com/
+voschezang/mash/blob/main/SHELL_REFERENCE.md). **Table of Contents** - [Usage]
+(#Usage) - [CLI](#CLI) - [Filesystem (CRUD Operations)](#Filesystem%20
+(CRUD%20Operations)) - [Usage Examples](#Usage%20Examples) - [Library & Tools]
+(#Library%20&%20Tools) - [Parallelization Utilities]
+(#Parallelization%20Utilities) - [Object Parser](#Object%20Parser) # Usage See
 [reference](SHELL_REFERENCE.md). ### CLI ```sh â¶ python -m mash -h usage:
 shell.py [-hvsr][-f FILE] [--session SESSION] [cmd [cmd ...]] If no positional
 arguments are given then an interactive subshell is started. positional
 arguments: cmd A comma- or newline-separated list of commands optional
 arguments: -h, --help show this help message and exit -v, --verbose -s, --safe
 Safe-mode. Ask for confirmation before executing commands. -f FILE, --file FILE
 Read and run FILE as a commands -r, --reload Reload last session --session
```

### Comparing `mash-shell-0.2.2/src/mash_shell.egg-info/SOURCES.txt` & `mash-shell-0.2.3/src/mash_shell.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,25 +34,33 @@
 src/mash/object_parser/oas.py
 src/mash/object_parser/object_parser.py
 src/mash/object_parser/object_parser_standards.py
 src/mash/object_parser/spec.py
 src/mash/shell/__init__.py
 src/mash/shell/base.py
 src/mash/shell/cmd2.py
-src/mash/shell/delimiters.py
 src/mash/shell/errors.py
 src/mash/shell/function.py
+src/mash/shell/helpers.py
 src/mash/shell/if_statement.py
-src/mash/shell/lex_parser.py
-src/mash/shell/model.py
 src/mash/shell/parsetab.py
-src/mash/shell/parsing.py
 src/mash/shell/progress_bar.py
 src/mash/shell/shell.py
 src/mash/shell/with_filesystem.py
+src/mash/shell/ast/__init__.py
+src/mash/shell/ast/conditions.py
+src/mash/shell/ast/function_definition.py
+src/mash/shell/ast/infix.py
+src/mash/shell/ast/node.py
+src/mash/shell/ast/nodes.py
+src/mash/shell/ast/term.py
+src/mash/shell/grammer/delimiters.py
+src/mash/shell/grammer/lex_yacc.py
+src/mash/shell/grammer/parsetab.py
+src/mash/shell/grammer/parsing.py
 src/mash_shell.egg-info/PKG-INFO
 src/mash_shell.egg-info/SOURCES.txt
 src/mash_shell.egg-info/dependency_links.txt
 src/mash_shell.egg-info/requires.txt
 src/mash_shell.egg-info/top_level.txt
 test/test_html_table.py
 test/test_parallel.py
```

### Comparing `mash-shell-0.2.2/test/test_html_table.py` & `mash-shell-0.2.3/test/test_html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/test/test_parallel.py` & `mash-shell-0.2.3/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/test/test_pipeline.py` & `mash-shell-0.2.3/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/test/test_server.py` & `mash-shell-0.2.3/test/test_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/test/test_util.py` & `mash-shell-0.2.3/test/test_util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.2/test/test_verify_server.py` & `mash-shell-0.2.3/test/test_verify_server.py`

 * *Files identical despite different names*

