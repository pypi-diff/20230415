# Comparing `tmp/argparse-manpage-4.tar.gz` & `tmp/argparse-manpage-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-manpage-4.tar", last modified: Mon Oct 31 08:33:42 2022, max compression
+gzip compressed data, was "argparse-manpage-4.1.tar", last modified: Sat Apr 15 19:13:25 2023, max compression
```

## Comparing `argparse-manpage-4.tar` & `argparse-manpage-4.1.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.880494 argparse-manpage-4/
--rw-rw-r--   0 twine    (17125) twine    (17125)      136 2019-09-07 00:39:54.000000 argparse-manpage-4/AUTHORS
--rw-rw-r--   0 twine    (17125) twine    (17125)    11357 2019-09-07 00:39:54.000000 argparse-manpage-4/LICENSE
--rw-r--r--   0 twine    (17125) twine    (17125)      577 2022-04-27 07:23:03.000000 argparse-manpage-4/MANIFEST.in
--rw-r--r--   0 twine    (17125) twine    (17125)     3925 2022-10-31 08:33:07.000000 argparse-manpage-4/NEWS
--rw-r--r--   0 twine    (17125) twine    (17125)     7516 2022-10-31 08:33:42.880494 argparse-manpage-4/PKG-INFO
--rw-r--r--   0 twine    (17125) twine    (17125)     7075 2022-10-31 08:33:07.000000 argparse-manpage-4/README.md
--rwxr-xr-x   0 twine    (17125) twine    (17125)      357 2022-10-31 08:33:07.000000 argparse-manpage-4/argparse-manpage
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.871494 argparse-manpage-4/argparse_manpage/
--rw-r--r--   0 twine    (17125) twine    (17125)       52 2022-10-31 08:33:07.000000 argparse-manpage-4/argparse_manpage/__init__.py
--rw-r--r--   0 twine    (17125) twine    (17125)     3380 2022-10-31 08:33:07.000000 argparse-manpage-4/argparse_manpage/cli.py
--rw-r--r--   0 twine    (17125) twine    (17125)     1637 2022-10-31 08:33:07.000000 argparse-manpage-4/argparse_manpage/compat.py
--rw-r--r--   0 twine    (17125) twine    (17125)    16432 2022-10-31 08:33:07.000000 argparse-manpage-4/argparse_manpage/manpage.py
--rw-r--r--   0 twine    (17125) twine    (17125)     2326 2022-10-31 08:33:07.000000 argparse-manpage-4/argparse_manpage/tooling.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.872494 argparse-manpage-4/argparse_manpage.egg-info/
--rw-rw-r--   0 twine    (17125) twine    (17125)     7516 2022-10-31 08:33:42.000000 argparse-manpage-4/argparse_manpage.egg-info/PKG-INFO
--rw-rw-r--   0 twine    (17125) twine    (17125)     2455 2022-10-31 08:33:42.000000 argparse-manpage-4/argparse_manpage.egg-info/SOURCES.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        1 2022-10-31 08:33:42.000000 argparse-manpage-4/argparse_manpage.egg-info/dependency_links.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)       63 2022-10-31 08:33:42.000000 argparse-manpage-4/argparse_manpage.egg-info/entry_points.txt
--rw-r--r--   0 twine    (17125) twine    (17125)       25 2022-10-31 08:33:42.000000 argparse-manpage-4/argparse_manpage.egg-info/requires.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)       32 2022-10-31 08:33:42.000000 argparse-manpage-4/argparse_manpage.egg-info/top_level.txt
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.872494 argparse-manpage-4/build_manpages/
--rw-r--r--   0 twine    (17125) twine    (17125)      169 2022-10-31 08:33:07.000000 argparse-manpage-4/build_manpages/__init__.py
--rw-r--r--   0 twine    (17125) twine    (17125)     7252 2022-10-31 08:33:07.000000 argparse-manpage-4/build_manpages/build_manpage.py
--rw-r--r--   0 twine    (17125) twine    (17125)     5205 2022-10-31 08:33:07.000000 argparse-manpage-4/build_manpages/build_manpages.py
--rw-r--r--   0 twine    (17125) twine    (17125)      980 2022-10-31 08:33:07.000000 argparse-manpage-4/build_manpages/compat.py
--rw-r--r--   0 twine    (17125) twine    (17125)      157 2022-10-31 08:33:07.000000 argparse-manpage-4/build_manpages/manpage.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.869494 argparse-manpage-4/examples/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.872494 argparse-manpage-4/examples/argument_groups/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.872494 argparse-manpage-4/examples/argument_groups/bin/
--rwxr-xr-x   0 twine    (17125) twine    (17125)     2250 2021-11-28 22:10:08.000000 argparse-manpage-4/examples/argument_groups/bin/test
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.873494 argparse-manpage-4/examples/argument_groups/expected/
--rw-r--r--   0 twine    (17125) twine    (17125)     2126 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/argument_groups/expected/test.1
--rw-r--r--   0 twine    (17125) twine    (17125)      115 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/argument_groups/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      984 2021-11-28 22:10:08.000000 argparse-manpage-4/examples/argument_groups/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.873494 argparse-manpage-4/examples/copr/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.873494 argparse-manpage-4/examples/copr/copr_cli/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/copr_cli/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/copr_cli/build_config.py
--rw-r--r--   0 twine    (17125) twine    (17125)    49234 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/copr/copr_cli/main.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/copr_cli/util.py
--rw-r--r--   0 twine    (17125) twine    (17125)    26532 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/copr/expected-output.1
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.874494 argparse-manpage-4/examples/copr/fake-deps/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/HACK
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.874494 argparse-manpage-4/examples/copr/fake-deps/copr/
--rw-rw-r--   0 twine    (17125) twine    (17125)       35 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/copr/README
--rw-rw-r--   0 twine    (17125) twine    (17125)       43 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/copr/__init__.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.874494 argparse-manpage-4/examples/copr/fake-deps/copr/client/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/copr/client/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       29 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/copr/client/responses.py
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/copr/exceptions.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       28 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/jinja2.py
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/fake-deps/simplejson.py
--rw-r--r--   0 twine    (17125) twine    (17125)      113 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/copr/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      965 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/copr/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.875494 argparse-manpage-4/examples/old_format/
--rw-r--r--   0 twine    (17125) twine    (17125)      917 2022-01-12 01:47:25.000000 argparse-manpage-4/examples/old_format/README.md
--rw-rw-r--   0 twine    (17125) twine    (17125)      519 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/old_format/example.py
--rw-r--r--   0 twine    (17125) twine    (17125)      504 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/old_format/expected-output.1
--rw-rw-r--   0 twine    (17125) twine    (17125)       59 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/old_format/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      789 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/old_format/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.876494 argparse-manpage-4/examples/old_format_file_name/
--rw-r--r--   0 twine    (17125) twine    (17125)      585 2022-01-12 01:47:25.000000 argparse-manpage-4/examples/old_format_file_name/README.md
--rw-r--r--   0 twine    (17125) twine    (17125)      519 2022-01-12 01:47:25.000000 argparse-manpage-4/examples/old_format_file_name/example.py
--rw-r--r--   0 twine    (17125) twine    (17125)      504 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/old_format_file_name/expected-output.1
--rw-r--r--   0 twine    (17125) twine    (17125)       82 2022-01-12 01:47:25.000000 argparse-manpage-4/examples/old_format_file_name/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      789 2022-01-12 01:47:25.000000 argparse-manpage-4/examples/old_format_file_name/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.876494 argparse-manpage-4/examples/osc/
--rw-r--r--   0 twine    (17125) twine    (17125)     2247 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/osc/expected-output.1
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.877494 argparse-manpage-4/examples/osc/osc/
--rw-r--r--   0 twine    (17125) twine    (17125)        0 2022-04-27 06:51:30.000000 argparse-manpage-4/examples/osc/osc/__init__.py
--rwxr-xr-x   0 twine    (17125) twine    (17125)     4636 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/osc/osc/main.py
--rw-r--r--   0 twine    (17125) twine    (17125)      251 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/osc/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      772 2022-04-27 06:51:30.000000 argparse-manpage-4/examples/osc/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.877494 argparse-manpage-4/examples/raw-description/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.877494 argparse-manpage-4/examples/raw-description/bin/
--rwxrwxr-x   0 twine    (17125) twine    (17125)     4455 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/raw-description/bin/dg
--rw-r--r--   0 twine    (17125) twine    (17125)     2036 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/raw-description/expected-output.1
--rw-rw-r--   0 twine    (17125) twine    (17125)       69 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/raw-description/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      982 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/raw-description/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.878494 argparse-manpage-4/examples/resalloc/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.878494 argparse-manpage-4/examples/resalloc/bin/
--rwxrwxr-x   0 twine    (17125) twine    (17125)     3076 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/bin/resalloc
--rwxrwxr-x   0 twine    (17125) twine    (17125)     2070 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/bin/resalloc-maint
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.869494 argparse-manpage-4/examples/resalloc/expected/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.878494 argparse-manpage-4/examples/resalloc/expected/man/
--rw-r--r--   0 twine    (17125) twine    (17125)     1124 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/resalloc/expected/man/resalloc-maint.1
--rw-r--r--   0 twine    (17125) twine    (17125)     1352 2022-10-31 08:33:07.000000 argparse-manpage-4/examples/resalloc/expected/man/resalloc.1
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/requirements.txt
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.879494 argparse-manpage-4/examples/resalloc/resalloc/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/resalloc/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/resalloc/client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       23 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/resalloc/version.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.879494 argparse-manpage-4/examples/resalloc/resallocserver/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/resallocserver/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       27 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/resallocserver/maint.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      146 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)     2241 2019-09-07 00:39:54.000000 argparse-manpage-4/examples/resalloc/setup.py
--rw-r--r--   0 twine    (17125) twine    (17125)      133 2022-10-31 08:33:42.880494 argparse-manpage-4/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)     1390 2022-10-31 08:33:07.000000 argparse-manpage-4/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2022-10-31 08:33:42.879494 argparse-manpage-4/tests/
--rw-r--r--   0 twine    (17125) twine    (17125)      660 2022-04-27 06:51:30.000000 argparse-manpage-4/tests/argparse_testlib.py
--rw-r--r--   0 twine    (17125) twine    (17125)     2010 2022-10-31 08:33:07.000000 argparse-manpage-4/tests/test_basic.py
--rw-r--r--   0 twine    (17125) twine    (17125)     7014 2022-10-31 08:33:07.000000 argparse-manpage-4/tests/test_examples.py
--rw-r--r--   0 twine    (17125) twine    (17125)     3954 2022-10-31 08:33:07.000000 argparse-manpage-4/tests/test_script.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.044954 argparse-manpage-4.1/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      136 2019-09-07 00:39:54.000000 argparse-manpage-4.1/AUTHORS
+-rw-rw-r--   0 twine    (17125) twine    (17125)    11357 2019-09-07 00:39:54.000000 argparse-manpage-4.1/LICENSE
+-rw-r--r--   0 twine    (17125) twine    (17125)      601 2023-04-15 19:13:21.000000 argparse-manpage-4.1/MANIFEST.in
+-rw-r--r--   0 twine    (17125) twine    (17125)     4345 2023-04-15 19:13:21.000000 argparse-manpage-4.1/NEWS
+-rw-r--r--   0 twine    (17125) twine    (17125)     8490 2023-04-15 19:13:25.044954 argparse-manpage-4.1/PKG-INFO
+-rw-r--r--   0 twine    (17125) twine    (17125)     8047 2023-04-15 19:13:21.000000 argparse-manpage-4.1/README.md
+-rwxr-xr-x   0 twine    (17125) twine    (17125)      357 2022-10-31 08:33:07.000000 argparse-manpage-4.1/argparse-manpage
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.034954 argparse-manpage-4.1/argparse_manpage/
+-rw-r--r--   0 twine    (17125) twine    (17125)       54 2023-04-15 19:13:21.000000 argparse-manpage-4.1/argparse_manpage/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     3492 2023-04-15 19:13:21.000000 argparse-manpage-4.1/argparse_manpage/cli.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1637 2022-10-31 08:33:07.000000 argparse-manpage-4.1/argparse_manpage/compat.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    21030 2023-04-15 19:13:21.000000 argparse-manpage-4.1/argparse_manpage/manpage.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     2326 2022-10-31 08:33:07.000000 argparse-manpage-4.1/argparse_manpage/tooling.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.035954 argparse-manpage-4.1/argparse_manpage.egg-info/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     8490 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/PKG-INFO
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2471 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/SOURCES.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        1 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/dependency_links.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)       63 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/entry_points.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)       25 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/requires.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)       32 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/top_level.txt
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.035954 argparse-manpage-4.1/build_manpages/
+-rw-r--r--   0 twine    (17125) twine    (17125)      169 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     7364 2023-04-15 19:13:21.000000 argparse-manpage-4.1/build_manpages/build_manpage.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     5205 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/build_manpages.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      980 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/compat.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      157 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/manpage.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.032954 argparse-manpage-4.1/examples/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/argument_groups/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/argument_groups/bin/
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     2250 2021-11-28 22:10:08.000000 argparse-manpage-4.1/examples/argument_groups/bin/test
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/argument_groups/expected/
+-rw-r--r--   0 twine    (17125) twine    (17125)     2125 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/argument_groups/expected/test.1
+-rw-r--r--   0 twine    (17125) twine    (17125)      115 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/argument_groups/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      984 2021-11-28 22:10:08.000000 argparse-manpage-4.1/examples/argument_groups/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/copr/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.037954 argparse-manpage-4.1/examples/copr/copr_cli/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/copr_cli/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/copr_cli/build_config.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    49234 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/copr/copr_cli/main.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/copr_cli/util.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    26531 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/copr/expected-output.1
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.037954 argparse-manpage-4.1/examples/copr/fake-deps/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/HACK
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.038954 argparse-manpage-4.1/examples/copr/fake-deps/copr/
+-rw-rw-r--   0 twine    (17125) twine    (17125)       35 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/README
+-rw-rw-r--   0 twine    (17125) twine    (17125)       43 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/__init__.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.038954 argparse-manpage-4.1/examples/copr/fake-deps/copr/client/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/client/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       29 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/client/responses.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/exceptions.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       28 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/jinja2.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/simplejson.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      113 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/copr/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      965 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.039954 argparse-manpage-4.1/examples/old_format/
+-rw-r--r--   0 twine    (17125) twine    (17125)      917 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format/README.md
+-rw-rw-r--   0 twine    (17125) twine    (17125)      519 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/old_format/example.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/old_format/expected-output.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)       59 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/old_format/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      789 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/old_format/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.040954 argparse-manpage-4.1/examples/old_format_file_name/
+-rw-r--r--   0 twine    (17125) twine    (17125)      585 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/README.md
+-rw-r--r--   0 twine    (17125) twine    (17125)      519 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/example.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/old_format_file_name/expected-output.1
+-rw-r--r--   0 twine    (17125) twine    (17125)       82 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      789 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.040954 argparse-manpage-4.1/examples/osc/
+-rw-r--r--   0 twine    (17125) twine    (17125)     2246 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/osc/expected-output.1
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.041954 argparse-manpage-4.1/examples/osc/osc/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2022-04-27 06:51:30.000000 argparse-manpage-4.1/examples/osc/osc/__init__.py
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     4636 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/osc/osc/main.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      251 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/osc/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      772 2022-04-27 06:51:30.000000 argparse-manpage-4.1/examples/osc/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.041954 argparse-manpage-4.1/examples/raw-description/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.041954 argparse-manpage-4.1/examples/raw-description/bin/
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     4455 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/raw-description/bin/dg
+-rw-r--r--   0 twine    (17125) twine    (17125)     2035 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/raw-description/expected-output.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)       69 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/raw-description/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      982 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/raw-description/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.042954 argparse-manpage-4.1/examples/resalloc/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.042954 argparse-manpage-4.1/examples/resalloc/bin/
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     3076 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/bin/resalloc
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     2070 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/bin/resalloc-maint
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.032954 argparse-manpage-4.1/examples/resalloc/expected/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.043954 argparse-manpage-4.1/examples/resalloc/expected/man/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1123 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/resalloc/expected/man/resalloc-maint.1
+-rw-r--r--   0 twine    (17125) twine    (17125)     1351 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/resalloc/expected/man/resalloc.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/requirements.txt
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.043954 argparse-manpage-4.1/examples/resalloc/resalloc/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resalloc/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resalloc/client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       23 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resalloc/version.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.043954 argparse-manpage-4.1/examples/resalloc/resallocserver/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resallocserver/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       27 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resallocserver/maint.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      146 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2241 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/setup.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      133 2023-04-15 19:13:25.045954 argparse-manpage-4.1/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)     1390 2022-10-31 08:33:07.000000 argparse-manpage-4.1/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.044954 argparse-manpage-4.1/tests/
+-rw-r--r--   0 twine    (17125) twine    (17125)      660 2022-04-27 06:51:30.000000 argparse-manpage-4.1/tests/argparse_testlib.py
+-rw-r--r--   0 twine    (17125) twine    (17125)       80 2023-04-15 19:13:21.000000 argparse-manpage-4.1/tests/extra.man
+-rw-r--r--   0 twine    (17125) twine    (17125)     2010 2022-10-31 08:33:07.000000 argparse-manpage-4.1/tests/test_basic.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     7014 2022-10-31 08:33:07.000000 argparse-manpage-4.1/tests/test_examples.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     4165 2023-04-15 19:13:21.000000 argparse-manpage-4.1/tests/test_script.py
```

### Comparing `argparse-manpage-4/LICENSE` & `argparse-manpage-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/MANIFEST.in` & `argparse-manpage-4.1/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 include examples/resalloc/expected/man/resalloc-maint.1
 include examples/resalloc/expected/man/resalloc.1
 include examples/copr/fake-deps/HACK
 include examples/copr/fake-deps/copr/README
 include examples/raw-description/bin/dg
 include examples/resalloc/bin/resalloc
 include examples/resalloc/bin/resalloc-maint
+include tests/extra.man
```

### Comparing `argparse-manpage-4/NEWS` & `argparse-manpage-4.1/NEWS`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 WARNING: The 'build_manpage' setup.py command will be removed v5
 WARNING: We'll drop the Python 2.7 support in v5
 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+News in v4.1
+
+* A new `--include` feature, inspired by `help2man --include`.
+
+* Allow overriding build date with SOURCE_DATE_EPOCH environment variable
+  in order to make builds reproducible.  See this link for more info:
+  https://reproducible-builds.org/specs/source-date-epoch/
+
+* The AUTHORS section was changed to more standard AUTHOR.
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 News in v4
 
 * The manual page generator logic is now separated from the 'build_manpages'
   module (which provides setup.py integration helpers).  Therefore the
   argparse-manpage doesn't necessarily have to depend on setuptools.
   Projects that want to integrate using 'setup.py' should though place a new
   "extra" named 'argparse-manpage[setuptools]' into their set of build
```

### Comparing `argparse-manpage-4/PKG-INFO` & `argparse-manpage-4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-manpage
-Version: 4
+Version: 4.1
 Summary: Build manual page from python's ArgumentParser object.
 Home-page: https://github.com/praiskup/argparse-manpage
 Author: Gabriele Giammatteo
 Author-email: gabriele.giammatteo@eng.it
 Maintainer: Pavel Raiskup
 Maintainer-email: praiskup@redhat.com
 License: Apache 2.0
@@ -125,22 +125,51 @@
 - version - version of the project, visible in manual page footer
 - prog - value that substitutes %prog in ArgumentParser's usage
 - url - link to project download page
 - manual_section - section of the manual, by default 1, see man (7) man-pages
     for more info about existing sections
 - manual_title - the title of the manual, by default "Generated Python Manual",
     see man (7) man-pages for more instructions
+- include - a file of extra material to include; see below for the format
 
 The values from setup.cfg override values from setup.py's setup().
 
-
 Then run `setup.py build_manpages` to build a manpages for your project.  Also,
 if you used `get_build_py` helper, `setup.py build` then transitively builds the
 manual pages.
 
+## Include file format
+
+The include file format is based on GNU `help2man`'s `--include` format.
+
+The format is simple:
+
+```
+[section]
+text
+
+/pattern/
+text
+```
+
+Blocks of verbatim *roff text are inserted into the output either at
+the start of the given `section` (case insensitive), or after a
+paragraph matching `pattern`, a Python regular expression.
+
+Lines before the first section are silently ignored and may be used for
+comments and the like.
+
+Other sections are prepended to the automatically produced output for the
+standard sections given above, or included near the bottom of the man page,
+before the `AUTHOR` section, in the order they occur in the include file.
+
+Placement of the text within the section may be explicitly requested by
+using the syntax `[<section]`, `[=section]` or `[>section]` to place the
+additional text before, in place of, or after the default output
+respectively.
 
 ## Installation
 
 This package is distributed [in PyPI][pypi-page], can be installed by:
 
     $ pip install argparse-manpage
```

### Comparing `argparse-manpage-4/README.md` & `argparse-manpage-4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -110,22 +110,51 @@
 - version - version of the project, visible in manual page footer
 - prog - value that substitutes %prog in ArgumentParser's usage
 - url - link to project download page
 - manual_section - section of the manual, by default 1, see man (7) man-pages
     for more info about existing sections
 - manual_title - the title of the manual, by default "Generated Python Manual",
     see man (7) man-pages for more instructions
+- include - a file of extra material to include; see below for the format
 
 The values from setup.cfg override values from setup.py's setup().
 
-
 Then run `setup.py build_manpages` to build a manpages for your project.  Also,
 if you used `get_build_py` helper, `setup.py build` then transitively builds the
 manual pages.
 
+## Include file format
+
+The include file format is based on GNU `help2man`'s `--include` format.
+
+The format is simple:
+
+```
+[section]
+text
+
+/pattern/
+text
+```
+
+Blocks of verbatim *roff text are inserted into the output either at
+the start of the given `section` (case insensitive), or after a
+paragraph matching `pattern`, a Python regular expression.
+
+Lines before the first section are silently ignored and may be used for
+comments and the like.
+
+Other sections are prepended to the automatically produced output for the
+standard sections given above, or included near the bottom of the man page,
+before the `AUTHOR` section, in the order they occur in the include file.
+
+Placement of the text within the section may be explicitly requested by
+using the syntax `[<section]`, `[=section]` or `[>section]` to place the
+additional text before, in place of, or after the default output
+respectively.
 
 ## Installation
 
 This package is distributed [in PyPI][pypi-page], can be installed by:
 
     $ pip install argparse-manpage
```

### Comparing `argparse-manpage-4/argparse_manpage/cli.py` & `argparse-manpage-4.1/argparse_manpage/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
                 help="Output file. Defaults to stdout.")
 ap.add_argument("--manual-section", help=(
     "Section of the manual, by default 1.  See man (7) man-pages for more "
     "info about existing sections."))
 ap.add_argument("--manual-title", help=(
     "The title of the manual, by default \"Generated Python Manual\". "
     "See man (7) man-pages for more instructions."))
+ap.add_argument("--include", metavar="FILE", help=(
+    "File that contains extra material for the man page."))
 
 
 def args_to_manpage_data(args):
     data = {}
     for attr in MANPAGE_DATA_ATTRS:
         value = getattr(args, attr)
         data[attr] = value
```

### Comparing `argparse-manpage-4/argparse_manpage/compat.py` & `argparse-manpage-4.1/argparse_manpage/compat.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/argparse_manpage/manpage.py` & `argparse-manpage-4.1/argparse_manpage/manpage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from argparse import SUPPRESS, HelpFormatter, _SubParsersAction, _HelpAction
 from collections import OrderedDict
 import datetime
+import os
+import time
+import re
 
 
 DEFAULT_GROUP_NAMES = {
     # We replace ArgumentGroup title (value) with alias (key).
     None: [
         'positional arguments',
     ],
@@ -35,14 +38,25 @@
     "project_name",  # maps to distribution.get_name()
     "prog",
     "url",
     "version",
     "format",
     "manual_section",
     "manual_title",
+    "include",
+)
+
+# manpage sections that are handled specially, so need special treatment
+# when --include'ing extra material; see Manpage.add_section.
+SPECIAL_MANPAGE_SECTIONS = (
+    "author",
+    "comments",
+    "description",
+    "distribution",
+    "synopsis",
 )
 
 
 def _markup(text):
     """
     Escape the text for the markdown format.
     """
@@ -90,15 +104,15 @@
     ret = []
     project_name = data.get("project_name", "")
     authors = data.get("authors")
     url = data.get("url")
 
     needs_separator = False
     if authors:
-        ret.append('.SH AUTHORS')
+        ret.append('.SH AUTHOR')
         for author in authors:
             ret.append(".nf")
             ret.append(author)
             ret.append(".fi")
         needs_separator = True
 
     if url:
@@ -133,24 +147,28 @@
         argument (see https://github.com/praiskup/argparse-manpage/issues/7),
         instead override the `self.<ATTRIBUTE>` when needed.
         """
         self.prog = parser.prog
         self.parser = parser
         self.format = format
         self._data = _data or {}
+        self._match_texts = []
         if not getattr(parser, '_manpage', None):
             self.parser._manpage = []
 
         self.formatter = self.parser._get_formatter()
         self.mf = _ManpageFormatter(self.prog, self.formatter, format=self.format)
         self.synopsis = self.parser.format_usage().split(':')[-1].split()
 
         self.date = self._data.get("date")
         if not self.date:
-            self.date = datetime.datetime.now().strftime('%Y-%m-%d')
+            builddate = datetime.datetime.utcfromtimestamp(
+                int(os.environ.get('SOURCE_DATE_EPOCH', time.time()))
+            )
+            self.date = builddate.strftime('%Y-%m-%d')
 
         self.source = self._data.get("project_name")
         if not self.source:
             self.source = self.prog
 
         version = self._data.get("version")
         if version:
@@ -162,14 +180,18 @@
 
         self.section = self._data.get("manual_section")
         if not self.section:
             self.section = 1
 
         self.description = self._data.get("description")
 
+        include = self._data.get("include")
+        if include is not None:
+            self.parse_include(include)
+
     def format_text(self, text):
         # Wrap by parser formatter and convert to manpage format
         return self.mf.format_text(self.formatter._format_text(text)).strip('\n')
 
     def __str__(self):
         lines = []
 
@@ -196,34 +218,122 @@
         if self.description:
             description = self.description
         if description:
             line += " - " + description
         lines.append(_markup(line))
 
         # Synopsis
-        if self.synopsis:
+        synopsis_section = self.get_extra_section("synopsis")
+        if self.synopsis or synopsis_section:
             lines.append('.SH SYNOPSIS')
-            lines.append('.B {}'.format(_markup(self.synopsis[0])))
-            lines.append(' '.join(self.synopsis[1:]))
+            if synopsis_section:
+                lines.append(synopsis_section.content)
+            else:
+                lines.append('.B {}'.format(_markup(self.synopsis[0])))
+                lines.append(' '.join(self.synopsis[1:]))
 
-        lines.extend(self.mf.format_parser(self.parser))
+        extra_description = None
+        description_section = self.get_extra_section("description")
+        if description_section:
+            extra_description = description_section.content
+        lines.extend(self.mf.format_parser(self.parser, extra_description=extra_description))
 
-        if self.parser.epilog != None:
+        comments_section = self.get_extra_section("comments")
+        if self.parser.epilog or comments_section:
             lines.append("")
             lines.append('.SH COMMENTS')
-            lines.append(self.format_text(self.parser.epilog))
+            if comments_section:
+                lines.append(comments_section.content)
+            else:
+                lines.append(self.format_text(self.parser.epilog))
 
-        # Additional Section
-        for section in self.parser._manpage:
-            lines.append('.SH {}'.format(section['heading'].upper()))
-            lines.append(self.format_text(section['content']))
+        # Additional sections
+        for section in self.parser._manpage: # pylint: disable=protected-access
+            if section["heading"] not in SPECIAL_MANPAGE_SECTIONS:
+                lines.append('.SH {}'.format(section['heading'].upper()))
+                lines.append(section['content'])
 
         lines.append("")
         lines.extend(self.mf.format_footer(self._data))
-        return "\n".join(lines).strip("\n") + "\n"
+
+        # Finally add --include sections that match text in the page
+        final_lines = []
+        for line in lines:
+            final_lines.append(line)
+            for match in self._match_texts:
+                if re.search(match['match_text'], line):
+                    final_lines.append(match['content'])
+
+        return "\n".join(final_lines).strip("\n") + "\n"
+
+    def get_extra_section(self, heading):
+        """
+        Return supplementary section for the `Manpage` (created with
+        `--include`), or `None`
+        """
+        for section in self.parser._manpage: # pylint: disable=protected-access
+            if section["heading"] == heading:
+                return section
+        return None
+
+    def add_section(self, heading, position, content):
+        """
+        Add a supplementary section to a `Manpage`
+        """
+        # Sections that need special treatment
+        heading = heading.lower()
+        if heading in ("author", "distribution"):
+            if heading == "author":
+                self._data['authors'] = [content]
+            elif heading == "distribution":
+                self._data['url'] = content
+        section = self.get_extra_section(heading)
+        if section is None:
+            section = {"heading": heading, "content": ""}
+            self.parser._manpage.append(section) # pylint: disable=protected-access
+        if position == '<':
+            section["content"] = content + section["content"]
+        elif position == '=':
+            section["content"] = content
+        elif position == '>':
+            section["content"] += content
+        else:
+            raise ValueError("invalid position " + position)
+
+    def parse_include(self, file):
+        """
+        Parse include file and add its contents to the man page
+        """
+        def get_section(lines, n):
+            for i, line in enumerate(lines[n:]):
+                if re.match(r'[\[/]', line):
+                    return n + i, lines[n:n + i]
+            return len(lines), lines[n:]
+
+        with open(file) as f:
+            lines = f.readlines()
+            i = 0
+            while i < len(lines):
+                # Parse a header line
+                m = re.match(r"/([^/]+)/$", lines[i])
+                if m:
+                    match_text = m.group(1)
+                    i, section_lines = get_section(lines, i + 1)
+                    self._match_texts.append({"match_text": match_text, "content": "".join(section_lines).strip()})
+                else:
+                    m = re.match(r"\[([<=>])?([^\]]+)\]$", lines[i])
+                    if m:
+                        position = m.group(1) or '<'
+                        heading = m.group(2).upper()
+                        if heading == "NAME":
+                            raise ValueError("Invalid include section " + heading)
+                        i, section_lines = get_section(lines, i + 1)
+                        self.add_section(heading, position, "".join(section_lines).strip())
+                    else:
+                        raise ValueError("Invalid or missing section header in include file %s:\n%s" % (file, lines[i]))
 
 
 def underline(text):
     """
     Wrap text with \fI for underlined text
     """
     return r'\fI\,{0}\/\fR'.format(_markup(text))
@@ -271,15 +381,15 @@
             default = action.dest.upper()
             args_string = self._format_args(action, default)
             for option_string in action.option_strings:
                 parts.append('{} {}'.format(bold(option_string),
                                             underline(args_string)))
         return ', '.join(parts)
 
-    def _format_parser(self, parser, subcommand=None, aliases=None, help=None):
+    def _format_parser(self, parser, subcommand=None, aliases=None, help=None, extra_description=None):
         # The parser "tree" looks like
         # ----------------------------
         # Parser -> [ActionGroup, ActionGroup, ..]
         # Group -> [Action, Action, ..]
         # Action -> Option
         # Action -> Subparsers
         # Subparser -> [Parser, Parser, ..] So called "choices".
@@ -304,39 +414,42 @@
                 elif self.format == "single-commands-section":
                     # print help
                     lines.append(help)
                     lines.append("")
 
             lines.append(self.format_text(parser.format_usage()))
 
-        if parser.description:
+        if parser.description or extra_description:
             if subcommand:
                 lines.append("")
             else:
                 lines.append(".SH DESCRIPTION")
 
-            lines.append(self.format_text(parser.description))
+            if extra_description:
+                lines.append(extra_description)
+            if parser.description:
+                lines.append(self.format_text(parser.description))
 
         is_subsequent_ag = True
         for group in parser._action_groups:
             ag_lines = self._format_action_group(group, subcommand)
             if not ag_lines:
                 continue
             if is_subsequent_ag:
                 lines.append("")
             lines.extend(ag_lines)
             is_subsequent_ag = True
 
         return lines
 
-    def format_parser(self, parser):
+    def format_parser(self, parser, extra_description=None):
         """
         Return lines Groff formatted text for given parser
         """
-        return self._format_parser(parser)
+        return self._format_parser(parser, extra_description=extra_description)
 
     def _format_action(self, action):
         parts = []
         parts.append('.TP')
 
         action_header = self._format_action_invocation(action)
         parts.append(action_header)
```

### Comparing `argparse-manpage-4/argparse_manpage/tooling.py` & `argparse-manpage-4.1/argparse_manpage/tooling.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/argparse_manpage.egg-info/PKG-INFO` & `argparse-manpage-4.1/argparse_manpage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-manpage
-Version: 4
+Version: 4.1
 Summary: Build manual page from python's ArgumentParser object.
 Home-page: https://github.com/praiskup/argparse-manpage
 Author: Gabriele Giammatteo
 Author-email: gabriele.giammatteo@eng.it
 Maintainer: Pavel Raiskup
 Maintainer-email: praiskup@redhat.com
 License: Apache 2.0
@@ -125,22 +125,51 @@
 - version - version of the project, visible in manual page footer
 - prog - value that substitutes %prog in ArgumentParser's usage
 - url - link to project download page
 - manual_section - section of the manual, by default 1, see man (7) man-pages
     for more info about existing sections
 - manual_title - the title of the manual, by default "Generated Python Manual",
     see man (7) man-pages for more instructions
+- include - a file of extra material to include; see below for the format
 
 The values from setup.cfg override values from setup.py's setup().
 
-
 Then run `setup.py build_manpages` to build a manpages for your project.  Also,
 if you used `get_build_py` helper, `setup.py build` then transitively builds the
 manual pages.
 
+## Include file format
+
+The include file format is based on GNU `help2man`'s `--include` format.
+
+The format is simple:
+
+```
+[section]
+text
+
+/pattern/
+text
+```
+
+Blocks of verbatim *roff text are inserted into the output either at
+the start of the given `section` (case insensitive), or after a
+paragraph matching `pattern`, a Python regular expression.
+
+Lines before the first section are silently ignored and may be used for
+comments and the like.
+
+Other sections are prepended to the automatically produced output for the
+standard sections given above, or included near the bottom of the man page,
+before the `AUTHOR` section, in the order they occur in the include file.
+
+Placement of the text within the section may be explicitly requested by
+using the syntax `[<section]`, `[=section]` or `[>section]` to place the
+additional text before, in place of, or after the default output
+respectively.
 
 ## Installation
 
 This package is distributed [in PyPI][pypi-page], can be installed by:
 
     $ pip install argparse-manpage
```

### Comparing `argparse-manpage-4/argparse_manpage.egg-info/SOURCES.txt` & `argparse-manpage-4.1/argparse_manpage.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,10 +69,11 @@
 examples/resalloc/expected/man/resalloc.1
 examples/resalloc/resalloc/__init__.py
 examples/resalloc/resalloc/client.py
 examples/resalloc/resalloc/version.py
 examples/resalloc/resallocserver/__init__.py
 examples/resalloc/resallocserver/maint.py
 tests/argparse_testlib.py
+tests/extra.man
 tests/test_basic.py
 tests/test_examples.py
 tests/test_script.py
```

### Comparing `argparse-manpage-4/build_manpages/build_manpage.py` & `argparse-manpage-4.1/build_manpages/build_manpage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
 """build_manpage command -- Generate man page from setup()"""
 
 import datetime
 import optparse
 import argparse
+import os
+import time
 import warnings
 
 from distutils.core import Command
 from distutils.errors import DistutilsOptionError
 
 from argparse_manpage.manpage import (
     get_manpage_data_from_distribution,
@@ -30,15 +32,17 @@
     _parser = None
     _command = None
     _type = None
 
     def __init__(self, parser, values):
         self._parser = parser
         self.values = values
-        self._today = datetime.date.today()
+        self._today = datetime.datetime.utcfromtimestamp(
+            int(os.environ.get('SOURCE_DATE_EPOCH', time.time()))
+        )
 
         if isinstance(parser, argparse.ArgumentParser):
             self._type = 'argparse'
             if parser.formatter_class == argparse.HelpFormatter:
                 # Hack for issue #36, to have reproducible manual page content
                 # regardless the terminal window size.  Long term we should avoid
                 # using the built-in usage formatter, and generate our own.
```

### Comparing `argparse-manpage-4/build_manpages/build_manpages.py` & `argparse-manpage-4.1/build_manpages/build_manpages.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/build_manpages/compat.py` & `argparse-manpage-4.1/build_manpages/compat.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/argument_groups/bin/test` & `argparse-manpage-4.1/examples/argument_groups/bin/test`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/argument_groups/expected/test.1` & `argparse-manpage-4.1/examples/argument_groups/expected/test.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH TEST "2" "2022\-10\-26" "example 0.1.0" "Test Manual"
+.TH TEST "2" "2023\-04\-09" "example 0.1.0" "Test Manual"
 .SH NAME
 test \- templating system/generator for distributions
 .SH SYNOPSIS
 .B test
 [-h] [--group-1-option PROJECTDIR] [--group-2-option DIST] [--top-option MULTISPEC] (--template TEMPLATE | --multispec-combinations) g2arg {subparserA} ...
 
 .SH OPTIONS
@@ -65,15 +65,15 @@
 .SH COMMAND \fI\,'test subparserA sub\-subparserA'\/\fR
 usage: test g2arg subparserA sub\-subparserA [\-h] [\-\-doh DOH]
 
 .SH OPTIONS \fI\,'test subparserA sub\-subparserA'\/\fR
 .TP
 \fB\-\-doh\fR \fI\,DOH\/\fR
 
-.SH AUTHORS
+.SH AUTHOR
 .nf
 John Doe <jd@example.com>
 .fi
 
 .SH DISTRIBUTION
 The latest version of example may be downloaded from
 .UR http://example.com
```

### Comparing `argparse-manpage-4/examples/argument_groups/setup.py` & `argparse-manpage-4.1/examples/argument_groups/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/copr/copr_cli/build_config.py` & `argparse-manpage-4.1/examples/copr/copr_cli/build_config.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/copr/copr_cli/main.py` & `argparse-manpage-4.1/examples/copr/copr_cli/main.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/copr/copr_cli/util.py` & `argparse-manpage-4.1/examples/copr/copr_cli/util.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/copr/expected-output.1` & `argparse-manpage-4.1/examples/copr/expected-output.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COPR "1" "2022\-10\-26" "example setup\-py\-overriden" "Generated Python Manual"
+.TH COPR "1" "2023\-04\-09" "example setup\-py\-overriden" "Generated Python Manual"
 .SH NAME
 copr
 .SH SYNOPSIS
 .B copr
 [-h] [--debug] [--config CONFIG] [--version] {hidden,whoami,list,mock-config,create,modify,delete,fork,build,buildpypi,buildgem,buildfedpkg,buildtito,buildmock,status,download-build,cancel,watch-build,delete-build,edit-chroot,get-chroot,add-package-tito,edit-package-tito,add-package-pypi,edit-package-pypi,add-package-mockscm,edit-package-mockscm,add-package-rubygems,edit-package-rubygems,list-packages,list-package-names,get-package,delete-package,reset-package,build-package,build-module} ...
 
 .SH OPTIONS
@@ -994,15 +994,15 @@
 .TP
 \fB\-\-yaml\fR \fI\,YAML\/\fR
 Path to modulemd file in yaml format
 
 .SH COMMENTS
 dummy text
 
-.SH AUTHORS
+.SH AUTHOR
 .nf
 John Doe <jd@example.com>
 .fi
 
 .SH DISTRIBUTION
 The latest version of example may be downloaded from
 .UR http://example.com
```

### Comparing `argparse-manpage-4/examples/copr/setup.py` & `argparse-manpage-4.1/examples/copr/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/old_format/README.md` & `argparse-manpage-4.1/examples/old_format/README.md`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/old_format/example.py` & `argparse-manpage-4.1/examples/old_format/example.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/old_format/setup.py` & `argparse-manpage-4.1/examples/old_format/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/old_format_file_name/README.md` & `argparse-manpage-4.1/examples/old_format_file_name/README.md`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/old_format_file_name/example.py` & `argparse-manpage-4.1/examples/old_format_file_name/example.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/old_format_file_name/setup.py` & `argparse-manpage-4.1/examples/old_format_file_name/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/osc/expected-output.1` & `argparse-manpage-4.1/examples/osc/expected-output.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH OSC "1" "2022\-10\-26" "osc 1.0" "Generated Python Manual"
+.TH OSC "1" "2023\-04\-09" "osc 1.0" "Generated Python Manual"
 .SH NAME
 osc \- openSUSE commander command\-line
 .SH SYNOPSIS
 .B osc
 [global opts] <command> [--help] [opts] [args] osc --help
 
 .SH
@@ -87,15 +87,15 @@
 
 .TP
 \fB\-\-opt\-baz2\fR \fI\,OPT_BAZ2\/\fR
 help opt\-baz2
 .RE
 
 
-.SH AUTHORS
+.SH AUTHOR
 .nf
 Contributors to the osc project. See the project's GIT history for the complete list.
 .fi
 
 .SH DISTRIBUTION
 The latest version of osc may be downloaded from
 .UR http://en.opensuse.org/openSUSE:OSC
```

### Comparing `argparse-manpage-4/examples/osc/osc/main.py` & `argparse-manpage-4.1/examples/osc/osc/main.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/osc/setup.py` & `argparse-manpage-4.1/examples/osc/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/raw-description/bin/dg` & `argparse-manpage-4.1/examples/raw-description/bin/dg`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/raw-description/expected-output.1` & `argparse-manpage-4.1/examples/raw-description/expected-output.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH DG "1" "2022\-10\-26" "example 0.1.0" "Generated Python Manual"
+.TH DG "1" "2023\-04\-09" "example 0.1.0" "Generated Python Manual"
 .SH NAME
 dg \- templating system/generator for distributions
 .SH SYNOPSIS
 .B dg
 [-h] [--projectdir PROJECTDIR] [--distro DIST] [--multispec MULTISPEC] [--multispec-selector MULTISPEC_SELECTOR] [--spec SPEC] [--output OUTPUT] [--macros-from PROJECTDIR] [--container CONTAINER_TYPE] [--macro MACRO] [--max-passes PASSES] (--template TEMPLATE | --multispec-combinations)
 .SH DESCRIPTION
 Generate script using predefined metadata about distribution and
@@ -61,15 +61,15 @@
 \fB\-\-template\fR \fI\,TEMPLATE\/\fR
 Use TEMPLATE file, e.g. docker.tpl or a template string, e.g. "{{ config.docker.from }}"
 
 .TP
 \fB\-\-multispec\-combinations\fR
 Print available multispec combinations
 
-.SH AUTHORS
+.SH AUTHOR
 .nf
 John Doe <jd@example.com>
 .fi
 
 .SH DISTRIBUTION
 The latest version of example may be downloaded from
 .UR http://example.com
```

### Comparing `argparse-manpage-4/examples/raw-description/setup.py` & `argparse-manpage-4.1/examples/raw-description/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/resalloc/bin/resalloc` & `argparse-manpage-4.1/examples/resalloc/bin/resalloc`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/resalloc/bin/resalloc-maint` & `argparse-manpage-4.1/examples/resalloc/bin/resalloc-maint`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/examples/resalloc/expected/man/resalloc-maint.1` & `argparse-manpage-4.1/examples/resalloc/expected/man/resalloc-maint.1`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH RESALLOC\-MAINT "1" "2022\-10\-26" "resalloc 0" "Generated Python Manual"
+.TH RESALLOC\-MAINT "1" "2023\-04\-09" "resalloc 0" "Generated Python Manual"
 .SH NAME
 resalloc\-maint
 .SH SYNOPSIS
 .B resalloc\-maint
 [-h] [--duh DUH] {resource-list,resource-delete,ticket-list} ...
 
 .SH OPTIONS
@@ -36,15 +36,15 @@
 .TP
 \fBresource\fR
 The resource ID
 
 .SH COMMAND \fI\,'resalloc\-maint ticket\-list'\/\fR
 usage: resalloc\-maint ticket\-list [\-h]
 
-.SH AUTHORS
+.SH AUTHOR
 .nf
 Pavel Raiskup <praiskup@redhat.com>
 .fi
 
 .SH DISTRIBUTION
 The latest version of resalloc may be downloaded from
 .UR https://github.com/praiskup/resalloc
```

### Comparing `argparse-manpage-4/examples/resalloc/expected/man/resalloc.1` & `argparse-manpage-4.1/examples/resalloc/expected/man/resalloc.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH RESALLOC "1" "2022\-10\-26" "resalloc 0" "Generated Python Manual"
+.TH RESALLOC "1" "2023\-04\-09" "resalloc 0" "Generated Python Manual"
 .SH NAME
 resalloc
 .SH SYNOPSIS
 .B resalloc
 [-h] [--connection CONNECTION] [--version] {ticket,ticket-check,ticket-wait,ticket-close} ...
 
 .SH OPTIONS
@@ -53,15 +53,15 @@
 .SH COMMAND \fI\,'resalloc ticket\-close'\/\fR
 usage: resalloc ticket\-close [\-h] ticket
 
 .TP
 \fBticket\fR
 ID of ticket to be closed
 
-.SH AUTHORS
+.SH AUTHOR
 .nf
 Pavel Raiskup <praiskup@redhat.com>
 .fi
 
 .SH DISTRIBUTION
 The latest version of resalloc may be downloaded from
 .UR https://github.com/praiskup/resalloc
```

### Comparing `argparse-manpage-4/examples/resalloc/setup.py` & `argparse-manpage-4.1/examples/resalloc/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/setup.py` & `argparse-manpage-4.1/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/tests/argparse_testlib.py` & `argparse-manpage-4.1/tests/argparse_testlib.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/tests/test_basic.py` & `argparse-manpage-4.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/tests/test_examples.py` & `argparse-manpage-4.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4/tests/test_script.py` & `argparse-manpage-4.1/tests/test_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import datetime
 import os
 import shutil
 import sys
 import subprocess
 import tempfile
+import time
 
 SIMPLE_FILE_CONTENTS = """
 import argparse
 
 def get_parser():
         parser = argparse.ArgumentParser({ap_arguments})
         parser.add_argument("test")
@@ -40,25 +41,30 @@
 {name} \\- some description
 .SH SYNOPSIS
 .B {name}
 [-h] test
 
 .TP
 \\fBtest\\fR
+.SH EXTRA SECTION
+This is an extra section.
 
-.SH AUTHORS
+.SH AUTHOR
 .nf
 John Doe <jdoe@example.com>
+Developer extraordinaire.
 .fi
 .nf
 Mr. Foo <mfoo@example.com> and friends
 .fi
 """
 
-DATE = datetime.datetime.now().strftime("%Y\\-%m\\-%d")
+DATE = datetime.datetime.utcfromtimestamp(
+           int(os.environ.get('SOURCE_DATE_EPOCH', time.time()))
+       ).strftime("%Y\\-%m\\-%d")
 
 class TestsArgparseManpageScript:
     def setup_method(self, _):
         self.workdir = tempfile.mkdtemp(prefix="argparse-manpage-tests-")
         os.environ["PYTHON"] = sys.executable
 
     def teardown_method(self, _):
@@ -127,12 +133,13 @@
             "--manual-title", "Some-long Manual Name",
             "--version", "1.alpha",
             "--author", "John Doe <jdoe@example.com>",
             "--author", "Mr. Foo <mfoo@example.com> and friends",
             "--project-name", "Proj-On-Cmdline",
             "--description", "some description",
             "--long-description", "Some long description.",  # unused
+            "--include", "tests/extra.man",
         ]
         output = subprocess.check_output(cmd).decode("utf-8")
         name="progname"
         assert output == FULL_OUTPUT.format(name=name, NAME=name.upper(),
                                             DATE=DATE)
```

