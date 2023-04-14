# Comparing `tmp/mss-8.0.2.tar.gz` & `tmp/mss-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mss-8.0.2.tar", last modified: Sun Apr  9 22:01:04 2023, max compression
+gzip compressed data, was "mss-8.0.3.tar", last modified: Fri Apr 14 22:53:22 2023, max compression
```

## Comparing `mss-8.0.2.tar` & `mss-8.0.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-04-05 04:26:59.000000 mss-8.0.2/LICENSE
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       88 2022-10-27 01:33:30.000000 mss-8.0.2/MANIFEST.in
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 22:01:04.133612 mss-8.0.2/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2199 2023-04-08 22:53:33.000000 mss-8.0.2/README.rst
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/docs/
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/docs/source/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2417 2023-04-09 20:16:52.000000 mss-8.0.2/docs/source/conf.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/docs/source/examples/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      550 2022-10-27 02:45:16.000000 mss-8.0.2/docs/source/examples/callback.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      729 2022-10-27 03:01:57.000000 mss-8.0.2/docs/source/examples/custom_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1356 2022-10-27 02:44:18.000000 mss-8.0.2/docs/source/examples/fps.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1113 2022-10-27 02:47:31.000000 mss-8.0.2/docs/source/examples/fps_multiprocessing.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      751 2022-10-27 02:46:10.000000 mss-8.0.2/docs/source/examples/from_pil_tuple.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      240 2022-10-27 02:08:04.000000 mss-8.0.2/docs/source/examples/linux_display_keyword.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      885 2022-10-27 02:08:14.000000 mss-8.0.2/docs/source/examples/opencv_numpy.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      526 2022-10-27 02:08:22.000000 mss-8.0.2/docs/source/examples/part_of_screen.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      792 2022-10-27 02:08:18.000000 mss-8.0.2/docs/source/examples/part_of_screen_monitor_2.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      712 2022-10-27 02:08:45.000000 mss-8.0.2/docs/source/examples/pil.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      755 2022-10-27 02:08:36.000000 mss-8.0.2/docs/source/examples/pil_pixels.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-09 20:16:52.000000 mss-8.0.2/mss/__init__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2659 2023-04-09 20:52:13.000000 mss-8.0.2/mss/__main__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-09 20:16:52.000000 mss-8.0.2/mss/base.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-08 22:53:33.000000 mss-8.0.2/mss/darwin.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-09 12:48:59.000000 mss-8.0.2/mss/exception.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-04-08 14:16:44.000000 mss-8.0.2/mss/factory.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    14900 2023-04-09 21:49:42.000000 mss-8.0.2/mss/linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2022-10-27 02:52:39.000000 mss-8.0.2/mss/models.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-08 22:53:33.000000 mss-8.0.2/mss/screenshot.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss/tests/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2022-10-27 02:10:59.000000 mss-8.0.2/mss/tests/bench_bgra2rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2022-10-27 02:11:02.000000 mss-8.0.2/mss/tests/bench_general.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1577 2023-04-09 21:56:53.000000 mss-8.0.2/mss/tests/conftest.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss/tests/res/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    37834 2023-04-09 21:56:53.000000 mss-8.0.2/mss/tests/res/monitor-1024x768.raw.zip
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-04-09 21:29:44.000000 mss-8.0.2/mss/tests/test_bgra_to_rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_find_monitors.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_get_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-09 12:48:59.000000 mss-8.0.2/mss/tests/test_gnu_linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6602 2023-04-09 20:52:13.000000 mss-8.0.2/mss/tests/test_implementation.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1521 2023-04-09 21:56:55.000000 mss-8.0.2/mss/tests/test_issue_220.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_leaks.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2022-10-27 02:12:18.000000 mss-8.0.2/mss/tests/test_macos.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_save.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      666 2023-04-05 14:07:14.000000 mss-8.0.2/mss/tests/test_setup.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_third_party.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2022-10-27 02:12:50.000000 mss-8.0.2/mss/tests/test_windows.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-08 22:53:33.000000 mss-8.0.2/mss/tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-09 21:08:05.000000 mss-8.0.2/mss/windows.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss.egg-info/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1583 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/SOURCES.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/dependency_links.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/entry_points.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-08 05:42:35.000000 mss-8.0.2/mss.egg-info/not-zip-safe
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/top_level.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1904 2023-04-09 22:01:04.133612 mss-8.0.2/setup.cfg
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-8.0.2/setup.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/venv/
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/venv/bin/
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      627 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2html.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      749 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2html4.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)     1094 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2html5.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      826 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2latex.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      649 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2man.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      815 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2odt.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)     1753 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      634 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      670 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2s5.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      906 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2xetex.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      635 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2xml.py
--rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      703 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.671195 mss-8.0.3/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    10881 2023-04-14 22:51:49.000000 mss-8.0.3/CHANGELOG.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5575 2023-04-14 22:52:22.000000 mss-8.0.3/CHANGES.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      668 2023-04-10 12:52:20.000000 mss-8.0.3/CONTRIBUTORS.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-04-10 14:19:05.000000 mss-8.0.3/LICENSE.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      276 2023-04-14 22:47:09.000000 mss-8.0.3/MANIFEST.in
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-14 22:53:22.671195 mss-8.0.3/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2109 2023-04-14 22:53:15.000000 mss-8.0.3/README.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       43 2023-04-11 07:35:16.000000 mss-8.0.3/dev-requirements.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.663195 mss-8.0.3/docs/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/docs/source/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8751 2023-04-09 20:16:52.000000 mss-8.0.3/docs/source/api.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2417 2023-04-10 11:05:18.000000 mss-8.0.3/docs/source/conf.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      858 2023-04-10 20:36:40.000000 mss-8.0.3/docs/source/developers.rst
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/docs/source/examples/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      550 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/callback.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      729 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/custom_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1356 2022-10-27 02:44:18.000000 mss-8.0.3/docs/source/examples/fps.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1113 2022-10-27 02:47:31.000000 mss-8.0.3/docs/source/examples/fps_multiprocessing.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      751 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/from_pil_tuple.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      240 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/linux_display_keyword.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      885 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/opencv_numpy.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      526 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/part_of_screen.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      792 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/part_of_screen_monitor_2.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      712 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/pil.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      755 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/pil_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     4332 2022-10-27 01:33:30.000000 mss-8.0.3/docs/source/examples.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1689 2023-04-10 19:48:35.000000 mss-8.0.3/docs/source/index.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      494 2022-10-27 01:33:30.000000 mss-8.0.3/docs/source/installation.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      735 2023-04-09 20:16:52.000000 mss-8.0.3/docs/source/support.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2216 2023-04-09 20:16:52.000000 mss-8.0.3/docs/source/usage.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3293 2023-04-09 22:30:36.000000 mss-8.0.3/docs/source/where.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2427 2023-04-14 22:53:22.671195 mss-8.0.3/setup.cfg
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-8.0.3/setup.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.663195 mss-8.0.3/src/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/src/mss/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/__init__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2659 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/__main__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/base.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/darwin.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/exception.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/factory.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    16933 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/models.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/py.typed
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/screenshot.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/windows.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/src/mss.egg-info/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1647 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/entry_points.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/top_level.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.671195 mss-8.0.3/src/tests/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/bench_bgra2rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/bench_general.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1577 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/conftest.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.671195 mss-8.0.3/src/tests/res/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    37834 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/res/monitor-1024x768.raw.zip
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_bgra_to_rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_find_monitors.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_get_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_gnu_linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6612 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_implementation.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1366 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_issue_220.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_leaks.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_macos.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_save.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6674 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_setup.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_third_party.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_windows.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       75 2023-04-11 07:36:50.000000 mss-8.0.3/tests-requirements.txt
```

### Comparing `mss-8.0.2/LICENSE` & `mss-8.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/PKG-INFO` & `mss-8.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,95 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.2
+Version: 8.0.3
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
 Project-URL: Tracker, https://github.com/BoboTiG/python-mss/issues
 Keywords: screen,screenshot,screencapture,screengrab
 Platform: Darwin
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: MacOS X
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
+Description-Content-Type: text/markdown
 
-Python MSS
-==========
-
-.. image:: https://badge.fury.io/py/mss.svg
-    :target: https://pypi.org/project/mss/
-.. image:: https://anaconda.org/conda-forge/python-mss/badges/version.svg
-    :target: https://anaconda.org/conda-forge/python-mss
-.. image:: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=master
-    :target: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml
-.. image:: https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
-    :target: https://pepy.tech/project/mss
-
-
-.. code-block:: python
-
-    from mss import mss
-
-    # The simplest use, save a screen shot of the 1st monitor
-    with mss() as sct:
-        sct.shot()
+# Python MSS
 
+[![PyPI version](https://badge.fury.io/py/mss.svg)](https://badge.fury.io/py/mss)
+[![Anaconda version](https://anaconda.org/conda-forge/python-mss/badges/version.svg)](https://anaconda.org/conda-forge/python-mss)
+[![Tests workflow](https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml)
+[![Downloads](https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mss)
+
+```python
+from mss import mss
+
+# The simplest use, save a screen shot of the 1st monitor
+with mss() as sct:
+    sct.shot()
+```
 
 An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 
-- **Python 3.8+** and PEP8 compliant, no dependency, thread-safe;
+- **Python 3.8+**, PEP8 compliant, no dependency, thread-safe;
 - very basic, it will grab one screen shot by monitor or a screen shot of all monitors and save it to a PNG file;
 - but you can use PIL and benefit from all its formats (or add yours directly);
 - integrate well with Numpy and OpenCV;
 - it could be easily embedded into games and other software which require fast and platform optimized methods to grab screen shots (like AI, Computer Vision);
-- get the `source code on GitHub <https://github.com/BoboTiG/python-mss>`_;
-- learn with a `bunch of examples <https://python-mss.readthedocs.io/examples.html>`_;
-- you can `report a bug <https://github.com/BoboTiG/python-mss/issues>`_;
-- need some help? Use the tag *python-mss* on `StackOverflow <https://stackoverflow.com/questions/tagged/python-mss>`_;
-- and there is a `complete, and beautiful, documentation <https://python-mss.readthedocs.io>`_ :)
+- get the [source code on GitHub](https://github.com/BoboTiG/python-mss);
+- learn with a [bunch of examples](https://python-mss.readthedocs.io/examples.html);
+- you can [report a bug](https://github.com/BoboTiG/python-mss/issues);
+- need some help? Use the tag *python-mss* on [StackOverflow](https://stackoverflow.com/questions/tagged/python-mss);
+- and there is a [complete, and beautiful, documentation](https://python-mss.readthedocs.io) :)
 - **MSS** stands for Multiple Screen Shots;
 
 
-Installation
-------------
+## Installation
 
-You can install it with pip::
+You can install it with pip:
 
-    python -m pip install -U --user mss
+```shell
+python -m pip install -U --user mss
+```
 
-Or you can install it with conda::
+Or you can install it with conda:
 
-    conda install -c conda-forge python-mss
+```shell
+conda install -c conda-forge python-mss
+```
 
-Maintenance
------------
+## Maintenance
 
-For the maintainers, here are commands to upload a new release::
+For the maintainers, here are commands to upload a new release:
 
-    rm -rf build dist
-    python -m build --sdist --wheel
-    twine check dist/*
-    twine upload dist/*
+```shell
+rm -rf build dist
+python -m build
+twine check dist/*
+twine upload dist/*
+```
```

### Comparing `mss-8.0.2/README.rst` & `mss-8.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-Python MSS
-==========
-
-.. image:: https://badge.fury.io/py/mss.svg
-    :target: https://pypi.org/project/mss/
-.. image:: https://anaconda.org/conda-forge/python-mss/badges/version.svg
-    :target: https://anaconda.org/conda-forge/python-mss
-.. image:: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=master
-    :target: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml
-.. image:: https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
-    :target: https://pepy.tech/project/mss
-
-
-.. code-block:: python
-
-    from mss import mss
-
-    # The simplest use, save a screen shot of the 1st monitor
-    with mss() as sct:
-        sct.shot()
+# Python MSS
 
+[![PyPI version](https://badge.fury.io/py/mss.svg)](https://badge.fury.io/py/mss)
+[![Anaconda version](https://anaconda.org/conda-forge/python-mss/badges/version.svg)](https://anaconda.org/conda-forge/python-mss)
+[![Tests workflow](https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml)
+[![Downloads](https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mss)
+
+```python
+from mss import mss
+
+# The simplest use, save a screen shot of the 1st monitor
+with mss() as sct:
+    sct.shot()
+```
 
 An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 
-- **Python 3.8+** and PEP8 compliant, no dependency, thread-safe;
+- **Python 3.8+**, PEP8 compliant, no dependency, thread-safe;
 - very basic, it will grab one screen shot by monitor or a screen shot of all monitors and save it to a PNG file;
 - but you can use PIL and benefit from all its formats (or add yours directly);
 - integrate well with Numpy and OpenCV;
 - it could be easily embedded into games and other software which require fast and platform optimized methods to grab screen shots (like AI, Computer Vision);
-- get the `source code on GitHub <https://github.com/BoboTiG/python-mss>`_;
-- learn with a `bunch of examples <https://python-mss.readthedocs.io/examples.html>`_;
-- you can `report a bug <https://github.com/BoboTiG/python-mss/issues>`_;
-- need some help? Use the tag *python-mss* on `StackOverflow <https://stackoverflow.com/questions/tagged/python-mss>`_;
-- and there is a `complete, and beautiful, documentation <https://python-mss.readthedocs.io>`_ :)
+- get the [source code on GitHub](https://github.com/BoboTiG/python-mss);
+- learn with a [bunch of examples](https://python-mss.readthedocs.io/examples.html);
+- you can [report a bug](https://github.com/BoboTiG/python-mss/issues);
+- need some help? Use the tag *python-mss* on [StackOverflow](https://stackoverflow.com/questions/tagged/python-mss);
+- and there is a [complete, and beautiful, documentation](https://python-mss.readthedocs.io) :)
 - **MSS** stands for Multiple Screen Shots;
 
 
-Installation
-------------
+## Installation
 
-You can install it with pip::
+You can install it with pip:
 
-    python -m pip install -U --user mss
+```shell
+python -m pip install -U --user mss
+```
 
-Or you can install it with conda::
+Or you can install it with conda:
 
-    conda install -c conda-forge python-mss
+```shell
+conda install -c conda-forge python-mss
+```
 
-Maintenance
------------
+## Maintenance
 
-For the maintainers, here are commands to upload a new release::
+For the maintainers, here are commands to upload a new release:
 
-    rm -rf build dist
-    python -m build --sdist --wheel
-    twine check dist/*
-    twine upload dist/*
+```shell
+rm -rf build dist
+python -m build
+twine check dist/*
+twine upload dist/*
+```
```

### Comparing `mss-8.0.2/docs/source/conf.py` & `mss-8.0.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 author = "Tiger-222"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "8.0.2"
+version = "8.0.3"
 
 # The full version, including alpha/beta/rc tags.
 release = "latest"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
```

### Comparing `mss-8.0.2/docs/source/examples/callback.py` & `mss-8.0.3/docs/source/examples/callback.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/custom_cls_image.py` & `mss-8.0.3/docs/source/examples/custom_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/fps.py` & `mss-8.0.3/docs/source/examples/fps.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/fps_multiprocessing.py` & `mss-8.0.3/docs/source/examples/fps_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/from_pil_tuple.py` & `mss-8.0.3/docs/source/examples/from_pil_tuple.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/opencv_numpy.py` & `mss-8.0.3/docs/source/examples/opencv_numpy.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/part_of_screen.py` & `mss-8.0.3/docs/source/examples/part_of_screen.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/part_of_screen_monitor_2.py` & `mss-8.0.3/docs/source/examples/part_of_screen_monitor_2.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/pil.py` & `mss-8.0.3/docs/source/examples/pil.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/docs/source/examples/pil_pixels.py` & `mss-8.0.3/docs/source/examples/pil_pixels.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/__init__.py` & `mss-8.0.3/src/mss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/python-mss
 If that URL should fail, try contacting the author.
 """
 from .exception import ScreenShotError
 from .factory import mss
 
-__version__ = "8.0.2"
+__version__ = "8.0.3"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
 Copyright (c) 2013-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
```

### Comparing `mss-8.0.2/mss/__main__.py` & `mss-8.0.3/src/mss/__main__.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/base.py` & `mss-8.0.3/src/mss/base.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/darwin.py` & `mss-8.0.3/src/mss/darwin.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/factory.py` & `mss-8.0.3/src/mss/factory.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/linux.py` & `mss-8.0.3/src/mss/linux.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,34 +40,39 @@
 ZPIXMAP = 2
 
 
 class Display(Structure):
     """
     Structure that serves as the connection to the X server
     and that contains all the information about that X server.
+    https://github.com/garrybodsworth/pyxlib-ctypes/blob/master/pyxlib/xlib.py#L831
     """
 
 
-class Event(Structure):
+class XErrorEvent(Structure):
     """
     XErrorEvent to debug eventual errors.
     https://tronche.com/gui/x/xlib/event-handling/protocol-errors/default-handlers.html
     """
 
     _fields_ = [
         ("type", c_int),
-        ("display", POINTER(Display)),
-        ("serial", c_ulong),
-        ("error_code", c_ubyte),
-        ("request_code", c_ubyte),
-        ("minor_code", c_ubyte),
-        ("resourceid", c_void_p),
+        ("display", POINTER(Display)),  # Display the event was read from
+        ("serial", c_ulong),  # serial number of failed request
+        ("error_code", c_ubyte),  # error code of failed request
+        ("request_code", c_ubyte),  # major op-code of failed request
+        ("minor_code", c_ubyte),  # minor op-code of failed request
+        ("resourceid", c_void_p),  # resource ID
     ]
 
 
+# TODO: remove in v9.0.0
+Event = XErrorEvent
+
+
 class XFixesCursorImage(Structure):
     """
     Cursor structure.
     /usr/include/X11/extensions/Xfixes.h
     https://github.com/freedesktop/xorg-libXfixes/blob/libXfixes-6.0.0/include/X11/extensions/Xfixes.h#L96
     """
 
@@ -88,59 +93,63 @@
 class XImage(Structure):
     """
     Description of an image as it exists in the client's memory.
     https://tronche.com/gui/x/xlib/graphics/images.html
     """
 
     _fields_ = [
-        ("width", c_int),
-        ("height", c_int),
-        ("xoffset", c_int),
-        ("format", c_int),
-        ("data", c_void_p),
-        ("byte_order", c_int),
-        ("bitmap_unit", c_int),
-        ("bitmap_bit_order", c_int),
-        ("bitmap_pad", c_int),
-        ("depth", c_int),
-        ("bytes_per_line", c_int),
-        ("bits_per_pixel", c_int),
-        ("red_mask", c_ulong),
-        ("green_mask", c_ulong),
-        ("blue_mask", c_ulong),
+        ("width", c_int),  # size of image
+        ("height", c_int),  # size of image
+        ("xoffset", c_int),  # number of pixels offset in X direction
+        ("format", c_int),  # XYBitmap, XYPixmap, ZPixmap
+        ("data", c_void_p),  # pointer to image data
+        ("byte_order", c_int),  # data byte order, LSBFirst, MSBFirst
+        ("bitmap_unit", c_int),  # quant. of scanline 8, 16, 32
+        ("bitmap_bit_order", c_int),  # LSBFirst, MSBFirst
+        ("bitmap_pad", c_int),  # 8, 16, 32 either XY or ZPixmap
+        ("depth", c_int),  # depth of image
+        ("bytes_per_line", c_int),  # accelarator to next line
+        ("bits_per_pixel", c_int),  # bits per pixel (ZPixmap)
+        ("red_mask", c_ulong),  # bits in z arrangment
+        ("green_mask", c_ulong),  # bits in z arrangment
+        ("blue_mask", c_ulong),  # bits in z arrangment
     ]
 
 
 class XRRCrtcInfo(Structure):
-    """Structure that contains CRTC information."""
+    """
+    Structure that contains CRTC information.
+    https://gitlab.freedesktop.org/xorg/lib/libxrandr/-/blob/master/include/X11/extensions/Xrandr.h#L360
+    """
 
     _fields_ = [
         ("timestamp", c_ulong),
         ("x", c_int),
         ("y", c_int),
-        ("width", c_int),
-        ("height", c_int),
+        ("width", c_uint),
+        ("height", c_uint),
         ("mode", c_long),
         ("rotation", c_int),
         ("noutput", c_int),
         ("outputs", POINTER(c_long)),
         ("rotations", c_ushort),
         ("npossible", c_int),
         ("possible", POINTER(c_long)),
     ]
 
 
 class XRRModeInfo(Structure):
-    """Voilà, voilà."""
+    """https://gitlab.freedesktop.org/xorg/lib/libxrandr/-/blob/master/include/X11/extensions/Xrandr.h#L248"""
 
 
 class XRRScreenResources(Structure):
     """
     Structure that contains arrays of XIDs that point to the
     available outputs and associated CRTCs.
+    https://gitlab.freedesktop.org/xorg/lib/libxrandr/-/blob/master/include/X11/extensions/Xrandr.h#L265
     """
 
     _fields_ = [
         ("timestamp", c_ulong),
         ("configTimestamp", c_ulong),
         ("ncrtc", c_int),
         ("crtcs", POINTER(c_long)),
@@ -151,63 +160,48 @@
     ]
 
 
 class XWindowAttributes(Structure):
     """Attributes for the specified window."""
 
     _fields_ = [
-        ("x", c_int32),
-        ("y", c_int32),
-        ("width", c_int32),
-        ("height", c_int32),
-        ("border_width", c_int32),
-        ("depth", c_int32),
-        ("visual", c_ulong),
-        ("root", c_ulong),
-        ("class", c_int32),
-        ("bit_gravity", c_int32),
-        ("win_gravity", c_int32),
-        ("backing_store", c_int32),
-        ("backing_planes", c_ulong),
-        ("backing_pixel", c_ulong),
-        ("save_under", c_int32),
-        ("colourmap", c_ulong),
-        ("mapinstalled", c_uint32),
-        ("map_state", c_uint32),
-        ("all_event_masks", c_ulong),
-        ("your_event_mask", c_ulong),
-        ("do_not_propagate_mask", c_ulong),
-        ("override_redirect", c_int32),
-        ("screen", c_ulong),
+        ("x", c_int32),  # location of window
+        ("y", c_int32),  # location of window
+        ("width", c_int32),  # width of window
+        ("height", c_int32),  # height of window
+        ("border_width", c_int32),  # border width of window
+        ("depth", c_int32),  # depth of window
+        ("visual", c_ulong),  # the associated visual structure
+        ("root", c_ulong),  # root of screen containing window
+        ("class", c_int32),  # InputOutput, InputOnly
+        ("bit_gravity", c_int32),  # one of bit gravity values
+        ("win_gravity", c_int32),  # one of the window gravity values
+        ("backing_store", c_int32),  # NotUseful, WhenMapped, Always
+        ("backing_planes", c_ulong),  # planes to be preserved if possible
+        ("backing_pixel", c_ulong),  # value to be used when restoring planes
+        ("save_under", c_int32),  # boolean, should bits under be saved?
+        ("colormap", c_ulong),  # color map to be associated with window
+        ("mapinstalled", c_uint32),  # boolean, is color map currently installed
+        ("map_state", c_uint32),  # IsUnmapped, IsUnviewable, IsViewable
+        ("all_event_masks", c_ulong),  # set of events all people have interest in
+        ("your_event_mask", c_ulong),  # my event mask
+        ("do_not_propagate_mask", c_ulong),  # set of events that should not propagate
+        ("override_redirect", c_int32),  # boolean value for override-redirect
+        ("screen", c_ulong),  # back pointer to correct screen
     ]
 
 
 _ERROR = {}
 _X11 = find_library("X11")
 _XFIXES = find_library("Xfixes")
 _XRANDR = find_library("Xrandr")
 
 
-@CFUNCTYPE(c_int, POINTER(Display), POINTER(Event))
-def _default_error_handler(display: Display, event: Event) -> int:
-    """
-    Specifies the default program's supplied error handler.
-    It's useful when exiting MSS to prevent letting `_error_handler()` as default handler.
-    Doing so would crash when using Tk/Tkinter, see issue #220.
-
-    Interesting technical stuff can be found here:
-        https://core.tcl-lang.org/tk/file?name=generic/tkError.c&ci=a527ef995862cb50
-        https://github.com/tcltk/tk/blob/b9cdafd83fe77499ff47fa373ce037aff3ae286a/generic/tkError.c
-    """
-    # pylint: disable=unused-argument
-    return 0  # pragma: nocover
-
-
-@CFUNCTYPE(c_int, POINTER(Display), POINTER(Event))
-def _error_handler(display: Display, event: Event) -> int:
+@CFUNCTYPE(c_int, POINTER(Display), POINTER(XErrorEvent))
+def _error_handler(display: Display, event: XErrorEvent) -> int:
     """Specifies the program's supplied error handler."""
 
     # Get the specific error message
     xlib = cdll.LoadLibrary(_X11)  # type: ignore[arg-type]
     get_error = xlib.XGetErrorText
     get_error.argtypes = [POINTER(Display), c_int, c_char_p, c_int]
     get_error.restype = c_void_p
@@ -262,15 +256,15 @@
     "XOpenDisplay": ("xlib", [c_char_p], POINTER(Display)),
     "XQueryExtension": ("xlib", [POINTER(Display), c_char_p, POINTER(c_int), POINTER(c_int), POINTER(c_int)], c_uint),
     "XRRFreeCrtcInfo": ("xrandr", [POINTER(XRRCrtcInfo)], c_void_p),
     "XRRFreeScreenResources": ("xrandr", [POINTER(XRRScreenResources)], c_void_p),
     "XRRGetCrtcInfo": ("xrandr", [POINTER(Display), POINTER(XRRScreenResources), c_long], POINTER(XRRCrtcInfo)),
     "XRRGetScreenResources": ("xrandr", [POINTER(Display), POINTER(Display)], POINTER(XRRScreenResources)),
     "XRRGetScreenResourcesCurrent": ("xrandr", [POINTER(Display), POINTER(Display)], POINTER(XRRScreenResources)),
-    "XSetErrorHandler": ("xlib", [c_void_p], c_int),
+    "XSetErrorHandler": ("xlib", [c_void_p], c_void_p),
 }
 
 
 class MSS(MSSBase):
     """
     Multiple ScreenShots implementation for GNU/Linux.
     It uses intensively the Xlib and its Xrandr extension.
@@ -279,14 +273,21 @@
     __slots__ = {"xfixes", "xlib", "xrandr", "_handles"}
 
     def __init__(self, /, **kwargs: Any) -> None:
         """GNU/Linux initialisations."""
 
         super().__init__(**kwargs)
 
+        # Available thread-specific variables
+        self._handles = local()
+        self._handles.display = None
+        self._handles.drawable = None
+        self._handles.original_error_handler = None
+        self._handles.root = None
+
         display = kwargs.get("display", b"")
         if not display:
             try:
                 display = os.environ["DISPLAY"].encode("utf-8")
             except KeyError:
                 raise ScreenShotError("$DISPLAY not set.") from None
 
@@ -296,50 +297,57 @@
         if b":" not in display:
             raise ScreenShotError(f"Bad display value: {display!r}.")
 
         if not _X11:
             raise ScreenShotError("No X11 library found.")
         self.xlib = cdll.LoadLibrary(_X11)
 
-        # Install the error handler to prevent interpreter crashes:
-        # any error will raise a ScreenShotError exception.
-        self.xlib.XSetErrorHandler(_error_handler)
-
         if not _XRANDR:
             raise ScreenShotError("No Xrandr extension found.")
         self.xrandr = cdll.LoadLibrary(_XRANDR)
 
         if self.with_cursor:
             if _XFIXES:
                 self.xfixes = cdll.LoadLibrary(_XFIXES)
             else:
                 self.with_cursor = False
 
         self._set_cfunctions()
 
-        self._handles = local()
+        # Install the error handler to prevent interpreter crashes: any error will raise a ScreenShotError exception
+        self._handles.original_error_handler = self.xlib.XSetErrorHandler(_error_handler)
+
         self._handles.display = self.xlib.XOpenDisplay(display)
 
         if not self._is_extension_enabled("RANDR"):
             raise ScreenShotError("Xrandr not enabled.")
 
         self._handles.root = self.xlib.XDefaultRootWindow(self._handles.display)
 
         # Fix for XRRGetScreenResources and XGetImage:
         #     expected LP_Display instance instead of LP_XWindowAttributes
         self._handles.drawable = cast(self._handles.root, POINTER(Display))
 
     def close(self) -> None:
         # Remove our error handler
-        self.xlib.XSetErrorHandler(_default_error_handler)
+        if self._handles.original_error_handler is not None:
+            # It's required when exiting MSS to prevent letting `_error_handler()` as default handler.
+            # Doing so would crash when using Tk/Tkinter, see issue #220.
+            # Interesting technical stuff can be found here:
+            #     https://core.tcl-lang.org/tk/file?name=generic/tkError.c&ci=a527ef995862cb50
+            #     https://github.com/tcltk/tk/blob/b9cdafd83fe77499ff47fa373ce037aff3ae286a/generic/tkError.c
+            self.xlib.XSetErrorHandler(self._handles.original_error_handler)
+            self._handles.original_error_handler = None
 
         # Clean-up
         if self._handles.display is not None:
             self.xlib.XCloseDisplay(self._handles.display)
             self._handles.display = None
+            self._handles.drawable = None
+            self._handles.root = None
 
         # Also empty the error dict
         _ERROR.clear()
 
     def _is_extension_enabled(self, name: str, /) -> bool:
         """Return True if the given *extension* is enabled on the server."""
         with lock:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mss-8.0.2/mss/screenshot.py` & `mss-8.0.3/src/mss/screenshot.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/bench_bgra2rgb.py` & `mss-8.0.3/src/tests/bench_bgra2rgb.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/bench_general.py` & `mss-8.0.3/src/tests/bench_general.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/conftest.py` & `mss-8.0.3/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/res/monitor-1024x768.raw.zip` & `mss-8.0.3/src/tests/res/monitor-1024x768.raw.zip`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_cls_image.py` & `mss-8.0.3/src/tests/test_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_find_monitors.py` & `mss-8.0.3/src/tests/test_find_monitors.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_get_pixels.py` & `mss-8.0.3/src/tests/test_get_pixels.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_gnu_linux.py` & `mss-8.0.3/src/tests/test_gnu_linux.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_implementation.py` & `mss-8.0.3/src/tests/test_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         assert not out
         assert not err
     else:
         with pytest.raises(ScreenShotError):
             main()
 
 
-def test_grab_with_tuple(pixel_ratio):
+def test_grab_with_tuple(pixel_ratio: int):
     left = 100
     top = 100
     right = 500
     lower = 500
     width = right - left  # 400px width
     height = lower - top  # 400px height
 
@@ -186,15 +186,15 @@
         box2 = {"left": left, "top": top, "width": width, "height": height}
         im2 = sct.grab(box2)
         assert im.size == im2.size
         assert im.pos == im2.pos
         assert im.rgb == im2.rgb
 
 
-def test_grab_with_tuple_percents(pixel_ratio):
+def test_grab_with_tuple_percents(pixel_ratio: int):
     with mss(display=os.getenv("DISPLAY")) as sct:
         monitor = sct.monitors[1]
         left = monitor["left"] + monitor["width"] * 5 // 100  # 5% from the left
         top = monitor["top"] + monitor["height"] * 5 // 100  # 5% from the top
         right = left + 500  # 500px
         lower = top + 500  # 500px
         width = right - left
```

### Comparing `mss-8.0.2/mss/tests/test_issue_220.py` & `mss-8.0.3/src/tests/test_issue_220.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
-import platform
-
 import pytest
 
 import mss
 
 tkinter = pytest.importorskip("tkinter")
 
-if platform.system().lower() == "darwin" and platform.python_implementation() == "PyPy":
-    # [macOS] PyPy 7.3.11 [Python 3.9.16] fails on GitHub:
-    #     RuntimeError: tk.h version (8.5) doesn't match libtk.a version (8.6)
-    pytestmark = pytest.mark.skip
-
 
 @pytest.fixture
 def root() -> tkinter.Tk:
-    master = tkinter.Tk()
+    try:
+        master = tkinter.Tk()
+    except RuntimeError:
+        pytest.skip(reason="tk.h version (8.5) doesn't match libtk.a version (8.6)")
+
     try:
         yield master
     finally:
         master.destroy()
 
 
 def take_screenshot():
```

### Comparing `mss-8.0.2/mss/tests/test_leaks.py` & `mss-8.0.3/src/tests/test_leaks.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_macos.py` & `mss-8.0.3/src/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_save.py` & `mss-8.0.3/src/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_third_party.py` & `mss-8.0.3/src/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_tools.py` & `mss-8.0.3/src/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tests/test_windows.py` & `mss-8.0.3/src/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/tools.py` & `mss-8.0.3/src/mss/tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss/windows.py` & `mss-8.0.3/src/mss/windows.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.2/mss.egg-info/PKG-INFO` & `mss-8.0.3/src/mss.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,95 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.2
+Version: 8.0.3
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
 Project-URL: Tracker, https://github.com/BoboTiG/python-mss/issues
 Keywords: screen,screenshot,screencapture,screengrab
 Platform: Darwin
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: MacOS X
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
+Description-Content-Type: text/markdown
 
-Python MSS
-==========
-
-.. image:: https://badge.fury.io/py/mss.svg
-    :target: https://pypi.org/project/mss/
-.. image:: https://anaconda.org/conda-forge/python-mss/badges/version.svg
-    :target: https://anaconda.org/conda-forge/python-mss
-.. image:: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=master
-    :target: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml
-.. image:: https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
-    :target: https://pepy.tech/project/mss
-
-
-.. code-block:: python
-
-    from mss import mss
-
-    # The simplest use, save a screen shot of the 1st monitor
-    with mss() as sct:
-        sct.shot()
+# Python MSS
 
+[![PyPI version](https://badge.fury.io/py/mss.svg)](https://badge.fury.io/py/mss)
+[![Anaconda version](https://anaconda.org/conda-forge/python-mss/badges/version.svg)](https://anaconda.org/conda-forge/python-mss)
+[![Tests workflow](https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml)
+[![Downloads](https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/mss)
+
+```python
+from mss import mss
+
+# The simplest use, save a screen shot of the 1st monitor
+with mss() as sct:
+    sct.shot()
+```
 
 An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 
-- **Python 3.8+** and PEP8 compliant, no dependency, thread-safe;
+- **Python 3.8+**, PEP8 compliant, no dependency, thread-safe;
 - very basic, it will grab one screen shot by monitor or a screen shot of all monitors and save it to a PNG file;
 - but you can use PIL and benefit from all its formats (or add yours directly);
 - integrate well with Numpy and OpenCV;
 - it could be easily embedded into games and other software which require fast and platform optimized methods to grab screen shots (like AI, Computer Vision);
-- get the `source code on GitHub <https://github.com/BoboTiG/python-mss>`_;
-- learn with a `bunch of examples <https://python-mss.readthedocs.io/examples.html>`_;
-- you can `report a bug <https://github.com/BoboTiG/python-mss/issues>`_;
-- need some help? Use the tag *python-mss* on `StackOverflow <https://stackoverflow.com/questions/tagged/python-mss>`_;
-- and there is a `complete, and beautiful, documentation <https://python-mss.readthedocs.io>`_ :)
+- get the [source code on GitHub](https://github.com/BoboTiG/python-mss);
+- learn with a [bunch of examples](https://python-mss.readthedocs.io/examples.html);
+- you can [report a bug](https://github.com/BoboTiG/python-mss/issues);
+- need some help? Use the tag *python-mss* on [StackOverflow](https://stackoverflow.com/questions/tagged/python-mss);
+- and there is a [complete, and beautiful, documentation](https://python-mss.readthedocs.io) :)
 - **MSS** stands for Multiple Screen Shots;
 
 
-Installation
-------------
+## Installation
 
-You can install it with pip::
+You can install it with pip:
 
-    python -m pip install -U --user mss
+```shell
+python -m pip install -U --user mss
+```
 
-Or you can install it with conda::
+Or you can install it with conda:
 
-    conda install -c conda-forge python-mss
+```shell
+conda install -c conda-forge python-mss
+```
 
-Maintenance
------------
+## Maintenance
 
-For the maintainers, here are commands to upload a new release::
+For the maintainers, here are commands to upload a new release:
 
-    rm -rf build dist
-    python -m build --sdist --wheel
-    twine check dist/*
-    twine upload dist/*
+```shell
+rm -rf build dist
+python -m build
+twine check dist/*
+twine upload dist/*
+```
```

### Comparing `mss-8.0.2/setup.cfg` & `mss-8.0.3/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 [metadata]
 name = mss
-version = 8.0.2
+version = 8.0.3
 author = Mickaël 'Tiger-222' Schoentgen
 author_email = contact@tiger-222.fr
 description = An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 url = https://github.com/BoboTiG/python-mss
 home_page = https://pypi.org/project/mss/
 project_urls = 
 	Documentation = https://python-mss.readthedocs.io
 	Source = https://github.com/BoboTiG/python-mss
 	Tracker = https://github.com/BoboTiG/python-mss/issues
 keywords = screen, screenshot, screencapture, screengrab
 license = MIT
 license_files = 
 	LICENSE
 platforms = Darwin, Linux, Windows
 classifiers = 
 	Development Status :: 5 - Production/Stable
+	Environment :: MacOS X
+	Intended Audience :: Developers
+	Intended Audience :: Education
+	Intended Audience :: End Users/Desktop
+	Intended Audience :: Information Technology
+	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
+	Operating System :: MacOS
+	Operating System :: Microsoft :: Windows
+	Operating System :: Unix
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 	Topic :: Software Development :: Libraries
 
 [options]
-zip_safe = False
-include_package_data = True
-packages = find_namespace:
 python_requires = >=3.8
+package_dir = 
+	= src
+packages = find:
 
 [options.packages.find]
-include = 
-	mss
-	mss.*
+where = src
+
+[options.package_data]
+mss = py.typed
 
 [options.entry_points]
 console_scripts = 
 	mss = mss.__main__:main
 
 [coverage:run]
 omit = 
@@ -60,22 +71,29 @@
 [isort]
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 line_length = 120
 
+[pylint.MESSAGES CONTROL]
+disable = locally-disabled, too-few-public-methods, too-many-instance-attributes, duplicate-code
+
+[pylint.REPORTS]
+max-line-length = 120
+output-format = colorized
+reports = no
+
 [tool:pytest]
+pythonpath = src
 addopts = 
 	--showlocals
 	--strict-markers
 	-r fE
 	-v
 	--cov=mss
 	--cov-report=term-missing
-	--force-flaky
-	--no-success-flaky-report
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

