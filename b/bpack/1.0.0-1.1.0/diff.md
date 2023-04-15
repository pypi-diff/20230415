# Comparing `tmp/bpack-1.0.0.tar.gz` & `tmp/bpack-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpack-1.0.0.tar", last modified: Sun Feb  5 08:38:47 2023, max compression
+gzip compressed data, was "bpack-1.1.0.tar", last modified: Sat Apr 15 09:24:15 2023, max compression
```

## Comparing `bpack-1.0.0.tar` & `bpack-1.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.412659 bpack-1.0.0/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11357 2020-11-29 07:59:12.000000 bpack-1.0.0/LICENSE
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      292 2021-06-04 06:15:22.000000 bpack-1.0.0/MANIFEST.in
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2758 2023-02-05 08:38:47.412659 bpack-1.0.0/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1719 2023-02-04 09:43:16.000000 bpack-1.0.0/README.rst
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.392659 bpack-1.0.0/bpack/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      467 2023-02-05 08:38:06.000000 bpack-1.0.0/bpack/__init__.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6003 2023-02-04 16:47:19.000000 bpack-1.0.0/bpack/ba.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     7511 2023-02-04 18:37:18.000000 bpack-1.0.0/bpack/bs.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     9963 2023-02-04 18:37:59.000000 bpack-1.0.0/bpack/codecs.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    20876 2023-02-04 18:38:44.000000 bpack-1.0.0/bpack/descriptors.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      908 2023-02-04 15:55:45.000000 bpack-1.0.0/bpack/enums.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    11665 2023-02-04 18:38:51.000000 bpack-1.0.0/bpack/np.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6355 2023-02-04 16:47:19.000000 bpack-1.0.0/bpack/st.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.400659 bpack-1.0.0/bpack/tests/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       23 2020-11-29 16:57:09.000000 bpack-1.0.0/bpack/tests/__init__.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    56154 2023-02-04 18:41:04.000000 bpack-1.0.0/bpack/tests/test_backends_codec.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1714 2023-02-04 16:47:19.000000 bpack-1.0.0/bpack/tests/test_codecs.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2435 2023-02-04 18:41:21.000000 bpack-1.0.0/bpack/tests/test_decoder_ba.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      957 2023-02-04 18:41:42.000000 bpack-1.0.0/bpack/tests/test_decoder_np.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    13639 2023-02-04 18:41:55.000000 bpack-1.0.0/bpack/tests/test_desctiptor_utils.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    19923 2023-02-04 18:42:46.000000 bpack-1.0.0/bpack/tests/test_field_descriptor.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    13667 2023-02-04 18:43:02.000000 bpack-1.0.0/bpack/tests/test_packbits.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    15410 2023-02-04 18:43:53.000000 bpack-1.0.0/bpack/tests/test_record_descriptor.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     4294 2023-02-04 17:33:41.000000 bpack-1.0.0/bpack/tests/test_typing.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5310 2023-02-04 18:44:39.000000 bpack-1.0.0/bpack/tests/test_utils.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     6847 2023-02-04 18:39:36.000000 bpack-1.0.0/bpack/typing.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     4950 2023-02-04 18:40:21.000000 bpack-1.0.0/bpack/utils.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.396659 bpack-1.0.0/bpack.egg-info/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2758 2023-02-05 08:38:47.000000 bpack-1.0.0/bpack.egg-info/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1305 2023-02-05 08:38:47.000000 bpack-1.0.0/bpack.egg-info/SOURCES.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-02-05 08:38:47.000000 bpack-1.0.0/bpack.egg-info/dependency_links.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      174 2023-02-05 08:38:47.000000 bpack-1.0.0/bpack.egg-info/requires.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        6 2023-02-05 08:38:47.000000 bpack-1.0.0/bpack.egg-info/top_level.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-02-05 08:38:46.000000 bpack-1.0.0/bpack.egg-info/zip-safe
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.404659 bpack-1.0.0/docs/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      634 2020-11-29 16:57:09.000000 bpack-1.0.0/docs/Makefile
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      456 2022-03-20 09:25:09.000000 bpack-1.0.0/docs/TODO.rst
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.384658 bpack-1.0.0/docs/_templates/
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.404659 bpack-1.0.0/docs/_templates/apidoc/
--rw-r--r--   0 antonio   (1000) antonio   (1000)     1151 2020-12-30 09:56:56.000000 bpack-1.0.0/docs/_templates/apidoc/package.rst_t
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.408659 bpack-1.0.0/docs/api/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.ba.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.bs.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.codecs.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      139 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.descriptors.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      121 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.enums.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.np.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      312 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.st.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.typing.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      121 2022-03-20 09:14:51.000000 bpack-1.0.0/docs/api/bpack.utils.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      475 2023-02-04 09:43:13.000000 bpack-1.0.0/docs/bpack.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3278 2023-02-04 19:40:20.000000 bpack-1.0.0/docs/conf.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3099 2023-02-05 08:38:06.000000 bpack-1.0.0/docs/development.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      603 2020-12-30 20:41:51.000000 bpack-1.0.0/docs/index.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2020-12-30 21:05:37.000000 bpack-1.0.0/docs/indices.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      841 2021-06-03 05:41:25.000000 bpack-1.0.0/docs/installation.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      723 2023-02-04 09:43:31.000000 bpack-1.0.0/docs/license.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      800 2023-02-04 18:16:05.000000 bpack-1.0.0/docs/make.bat
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2625 2021-06-03 05:41:25.000000 bpack-1.0.0/docs/overview.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     3923 2023-02-05 08:38:06.000000 bpack-1.0.0/docs/release_notes.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      257 2023-02-05 08:38:06.000000 bpack-1.0.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    26353 2023-02-04 14:07:35.000000 bpack-1.0.0/docs/userguide.rst
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-05 08:38:47.412659 bpack-1.0.0/examples/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1863 2023-02-04 19:32:31.000000 bpack-1.0.0/examples/packet_decoding.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     8835 2023-02-04 19:43:59.000000 bpack-1.0.0/examples/s1isp.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1790 2023-02-04 19:26:04.000000 bpack-1.0.0/pyproject.toml
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      172 2023-02-04 19:21:26.000000 bpack-1.0.0/requirements-dev.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2023-02-05 08:38:47.412659 bpack-1.0.0/setup.cfg
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1542 2023-02-04 14:00:25.000000 bpack-1.0.0/tox.ini
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.358030 bpack-1.1.0/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11357 2020-11-29 07:59:12.000000 bpack-1.1.0/LICENSE
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      292 2021-06-04 06:15:22.000000 bpack-1.1.0/MANIFEST.in
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2758 2023-04-15 09:24:15.342029 bpack-1.1.0/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1719 2023-02-04 09:43:16.000000 bpack-1.1.0/README.rst
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.314027 bpack-1.1.0/bpack/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      467 2023-04-15 09:21:40.000000 bpack-1.1.0/bpack/__init__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6003 2023-02-04 16:47:19.000000 bpack-1.1.0/bpack/ba.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     7511 2023-02-04 18:37:18.000000 bpack-1.1.0/bpack/bs.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     9963 2023-02-04 18:37:59.000000 bpack-1.1.0/bpack/codecs.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    21762 2023-02-20 07:52:19.000000 bpack-1.1.0/bpack/descriptors.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      908 2023-02-04 15:55:45.000000 bpack-1.1.0/bpack/enums.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    17330 2023-04-15 08:48:48.000000 bpack-1.1.0/bpack/np.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6355 2023-02-04 16:47:19.000000 bpack-1.1.0/bpack/st.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.318027 bpack-1.1.0/bpack/tests/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       23 2020-11-29 16:57:09.000000 bpack-1.1.0/bpack/tests/__init__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    56154 2023-02-04 18:41:04.000000 bpack-1.1.0/bpack/tests/test_backends_codec.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1714 2023-02-04 16:47:19.000000 bpack-1.1.0/bpack/tests/test_codecs.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2435 2023-02-04 18:41:21.000000 bpack-1.1.0/bpack/tests/test_decoder_ba.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      957 2023-02-04 18:41:42.000000 bpack-1.1.0/bpack/tests/test_decoder_np.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    13639 2023-02-04 18:41:55.000000 bpack-1.1.0/bpack/tests/test_desctiptor_utils.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    19923 2023-02-04 18:42:46.000000 bpack-1.1.0/bpack/tests/test_field_descriptor.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    15305 2023-02-27 07:43:44.000000 bpack-1.1.0/bpack/tests/test_packbits.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    15410 2023-02-04 18:43:53.000000 bpack-1.1.0/bpack/tests/test_record_descriptor.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     4294 2023-02-04 17:33:41.000000 bpack-1.1.0/bpack/tests/test_typing.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5310 2023-02-25 17:46:04.000000 bpack-1.1.0/bpack/tests/test_utils.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6898 2023-02-27 07:43:44.000000 bpack-1.1.0/bpack/typing.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     4950 2023-02-04 18:40:21.000000 bpack-1.1.0/bpack/utils.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.314027 bpack-1.1.0/bpack.egg-info/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2758 2023-04-15 09:24:15.000000 bpack-1.1.0/bpack.egg-info/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1305 2023-04-15 09:24:15.000000 bpack-1.1.0/bpack.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-04-15 09:24:15.000000 bpack-1.1.0/bpack.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      174 2023-04-15 09:24:15.000000 bpack-1.1.0/bpack.egg-info/requires.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        6 2023-04-15 09:24:15.000000 bpack-1.1.0/bpack.egg-info/top_level.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-04-15 09:24:14.000000 bpack-1.1.0/bpack.egg-info/zip-safe
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.330028 bpack-1.1.0/docs/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      634 2020-11-29 16:57:09.000000 bpack-1.1.0/docs/Makefile
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      456 2022-03-20 09:25:09.000000 bpack-1.1.0/docs/TODO.rst
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.306026 bpack-1.1.0/docs/_templates/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.334028 bpack-1.1.0/docs/_templates/apidoc/
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     1151 2020-12-30 09:56:56.000000 bpack-1.1.0/docs/_templates/apidoc/package.rst_t
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.342029 bpack-1.1.0/docs/api/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.ba.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.bs.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.codecs.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      139 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.descriptors.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      121 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.enums.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.np.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      312 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      112 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.st.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      124 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.typing.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      121 2023-02-26 19:15:49.000000 bpack-1.1.0/docs/api/bpack.utils.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      475 2023-02-04 09:43:13.000000 bpack-1.1.0/docs/bpack.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3278 2023-02-04 19:40:20.000000 bpack-1.1.0/docs/conf.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3099 2023-02-05 08:38:06.000000 bpack-1.1.0/docs/development.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      603 2020-12-30 20:41:51.000000 bpack-1.1.0/docs/index.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      122 2020-12-30 21:05:37.000000 bpack-1.1.0/docs/indices.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      841 2021-06-03 05:41:25.000000 bpack-1.1.0/docs/installation.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      723 2023-02-04 09:43:31.000000 bpack-1.1.0/docs/license.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      800 2023-02-04 18:16:05.000000 bpack-1.1.0/docs/make.bat
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2675 2023-02-20 07:52:46.000000 bpack-1.1.0/docs/overview.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     4253 2023-04-15 09:21:40.000000 bpack-1.1.0/docs/release_notes.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      265 2023-04-15 08:36:53.000000 bpack-1.1.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    26353 2023-02-19 16:56:43.000000 bpack-1.1.0/docs/userguide.rst
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-04-15 09:24:15.342029 bpack-1.1.0/examples/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1863 2023-02-04 19:32:31.000000 bpack-1.1.0/examples/packet_decoding.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     8835 2023-02-25 17:45:42.000000 bpack-1.1.0/examples/s1isp.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1790 2023-02-04 19:26:04.000000 bpack-1.1.0/pyproject.toml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      172 2023-02-04 19:21:26.000000 bpack-1.1.0/requirements-dev.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2023-04-15 09:24:15.358030 bpack-1.1.0/setup.cfg
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1542 2023-02-26 20:28:16.000000 bpack-1.1.0/tox.ini
```

### Comparing `bpack-1.0.0/LICENSE` & `bpack-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/PKG-INFO` & `bpack-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpack
-Version: 1.0.0
+Version: 1.1.0
 Summary: Binary data structures (un-)packing library
 Author-email: Antonio Valentino <antonio.valentino@tiscali.it>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/avalentino/bpack
 Project-URL: documentation, https://bpack.readthedocs.io
 Project-URL: repository, https://github.com/avalentino/bpack.git
 Project-URL: changelog, https://github.com/avalentino/bpack/blob/main/docs/release_notes.rst
```

### Comparing `bpack-1.0.0/README.rst` & `bpack-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/ba.py` & `bpack-1.1.0/bpack/ba.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/bs.py` & `bpack-1.1.0/bpack/bs.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/codecs.py` & `bpack-1.1.0/bpack/codecs.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/descriptors.py` & `bpack-1.1.0/bpack/descriptors.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,26 +68,29 @@
     else:
         rtype = type_
     return rtype
 
 
 @dataclasses.dataclass
 class BinFieldDescriptor:
-    """Descriptor for bpack fields."""
+    """Descriptor for bpack fields.
+
+    See also :func:`bpack.filed` for a description of the attributes.
+    """
 
     type: Optional[Type] = None  # noqa: A003
     size: Optional[int] = None  #: item size
     offset: Optional[int] = None
     signed: Optional[bool] = None
     repeat: Optional[int] = None  #: number of items
     # converter: Optional[Callable] = None
 
     def _validate_type(self):
         if self.type is None:
-            raise TypeError(f'invalid type "{self.type}"')
+            raise TypeError(f"invalid type '{self.type}'")
 
     def _validate_size(self):
         msg = f"invalid size: {self.size!r} (must be a positive integer)"
         if not isinstance(self.size, int):
             raise TypeError(msg)
         if self.size <= 0:
             raise ValueError(msg)
@@ -152,15 +155,15 @@
                     f"repeat parameter specified for non-sequence type: "
                     f"{self.type}"
                 )
         if bpack.utils.is_enum_type(self.type):
             self._validate_enum_type()
         elif self.is_sequence_type() and self.repeat is None:
             raise TypeError(
-                f"no 'repeat? parameter specified for sequence type "
+                f"no 'repeat' parameter specified for sequence type "
                 f"{self.type}"
             )
 
     def is_int_type(self) -> bool:
         """Return True if the field is an integer or a sub-type of integer."""
         return bpack.utils.is_int_type(self.type)
 
@@ -226,14 +229,34 @@
     metadata=None,
     **kwargs,
 ) -> Field:
     """Initialize a field descriptor.
 
     Returned object is a :class:`Field` instance with metadata properly
     initialized to describe the field of a binary record.
+
+    :param size: int
+        size of the field in :class:`EBaseUnits`
+    :param offset: int
+        offset of the field w.r.t. the beginning of the record
+        (expressed in :class:`EBaseUnits`)
+    :param signed: bool
+        True if an `int` field is signed, False otherwise.
+        This parameter must not be specified for non `int` fields.
+    :param repeat: int
+        length of the sequence for `sequence` fields, i.e. fields
+        consisting in multiple items having the same data type.
+        This parameter must not be specified if the data type is not a
+        sequence type (e.g. `List`).
+    :param metadata:
+        additional metadata to be attached the the field descriptor.
+    :param kwargs:
+        additional keyword arguments for the :func:`dataclasses.field`
+        function.
+
     """
     field_descr = BinFieldDescriptor(
         size=size, offset=offset, signed=signed, repeat=repeat
     )
     metadata = metadata.copy() if metadata is not None else {}
     metadata[METADATA_KEY] = types.MappingProxyType(
         dataclasses.asdict(field_descr)
```

### Comparing `bpack-1.0.0/bpack/enums.py` & `bpack-1.1.0/bpack/enums.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/st.py` & `bpack-1.1.0/bpack/st.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_backends_codec.py` & `bpack-1.1.0/bpack/tests/test_backends_codec.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_codecs.py` & `bpack-1.1.0/bpack/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_decoder_ba.py` & `bpack-1.1.0/bpack/tests/test_decoder_ba.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_decoder_np.py` & `bpack-1.1.0/bpack/tests/test_decoder_np.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_desctiptor_utils.py` & `bpack-1.1.0/bpack/tests/test_desctiptor_utils.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_field_descriptor.py` & `bpack-1.1.0/bpack/tests/test_field_descriptor.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_packbits.py` & `bpack-1.1.0/bpack/tests/test_packbits.py`

 * *Files 6% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         pytest.param(
             bpack_np,
             id="np",
             marks=pytest.mark.skipif(not bpack_np, reason="not available"),
         ),
     ],
 )
-def test_unpackbits_1(backend):
+def test_unpackbits_1_bit_per_sample(backend):
     bits_per_sample = 1
     values = [1, 0, 1, 0, 1, 0, 1, 0]
     data = bytes([0b10101010])
     ovalues = backend.unpackbits(data, bits_per_sample)
     assert list(ovalues) == values
 
 
@@ -228,38 +228,62 @@
     values = [item % (2**bits_per_sample) for item in range(nsamples)]
     data = bpack_bs.packbits(values, bits_per_sample)
     ovalues = backend.unpackbits(data, bits_per_sample)
     assert list(ovalues) == values
 
 
 def _make_sample_data_block(
-    header_size, bits_per_sample, samples_per_block, bit_offset=0, nblocks=1
+    header_size,
+    bits_per_sample,
+    samples_per_block,
+    bit_offset=0,
+    nblocks=1,
+    sign_mode=0,
 ):
     bits_per_block = header_size + bits_per_sample * samples_per_block
     nbytes = math.ceil((bit_offset + bits_per_block) / 8)
 
-    block_fmt = f"u{bits_per_sample}" * samples_per_block
+    typechar = "s" if sign_mode == 1 else "u"
+    block_fmt = f"{typechar}{bits_per_sample}" * samples_per_block
     if header_size > 0:
         block_fmt = f"u{header_size}" + block_fmt
 
     leading_pad = f"p{bit_offset}" if bit_offset > 0 else ""
     trailing_pad = nbytes * 8 - bits_per_block * nblocks - bit_offset
     trailing_pad = f"p{trailing_pad}" if trailing_pad > 0 else ""
     fmt = f"{leading_pad}{block_fmt * nblocks}{trailing_pad}"
 
     n = 2**bits_per_sample
-
-    ramp_values = list(range(n)) * math.ceil(samples_per_block / n)
+    if sign_mode == 0:
+        ramp_values = list(range(n)) * math.ceil(samples_per_block / n)
+        out_values = ramp_values
+    elif sign_mode == 1:
+        hs = 2 ** (bits_per_sample - 1)
+        ramp_values = list(range(-hs, hs)) * math.ceil(samples_per_block / n)
+        out_values = ramp_values
+    elif sign_mode == 2:
+        hs = 2 ** (bits_per_sample - 1)
+        ramp_values = list(range(hs))
+        out_values = ramp_values + [-item for item in ramp_values]
+        out_values *= math.ceil(samples_per_block / n)
+        sign_mask = 2 ** (bits_per_sample - 1)
+        ramp_values += [item | sign_mask for item in ramp_values]
+        ramp_values *= math.ceil(samples_per_block / n)
+    else:
+        raise ValueError(f"Unexpected 'sign_mode': {sign_mode}")
     values = ramp_values[:samples_per_block]
+    out_values = out_values[:samples_per_block]
     if header_size > 0:
         values = [113] + values
+        out_values = [113] + out_values
     values *= nblocks
+    out_values *= nblocks
     data = bitstruct.pack(fmt, *values)
 
-    return data, values
+    return data, out_values
 
 
 @pytest.mark.skipif(not bitstruct, reason="bitstruct not available")
 @pytest.mark.skipif(not np, reason="numpy not available")
 @pytest.mark.parametrize("bit_offset", [0, 1, 2])
 @pytest.mark.parametrize("header_size", [9, 13])
 @pytest.mark.parametrize("bits_per_sample", [3, 4, 5, 6, 12, 13, 14])
@@ -289,36 +313,48 @@
     assert all(headers == values[0])
 
 
 @pytest.mark.skipif(not bitstruct, reason="bitstruct not available")
 @pytest.mark.skipif(not np, reason="numpy not available")
 @pytest.mark.parametrize("bit_offset", [0, 1, 2])
 @pytest.mark.parametrize("header_size", [0, 9, 13])
-@pytest.mark.parametrize("bits_per_sample", [3, 4, 5, 6, 12, 13, 14])
-@pytest.mark.parametrize("samples_per_block", [64, 128, 256])
+@pytest.mark.parametrize("bits_per_sample", [3, 4, 5, 8, 13])
+@pytest.mark.parametrize("samples_per_block", [64, 128])
 @pytest.mark.parametrize("nblocks", [1, 3, 20])
+@pytest.mark.parametrize("sign_mode", [0, 1, 2])
 def test_data(
-    bit_offset, header_size, bits_per_sample, samples_per_block, nblocks
+    bit_offset,
+    header_size,
+    bits_per_sample,
+    samples_per_block,
+    nblocks,
+    sign_mode,
 ):
     data, values = _make_sample_data_block(
         header_size,
         bits_per_sample,
         samples_per_block,
         bit_offset,
         nblocks=nblocks,
+        sign_mode=sign_mode,
+    )
+
+    assert len(values) == (
+        samples_per_block * nblocks + (nblocks if header_size else 0)
     )
 
     block_size = header_size + bits_per_sample * samples_per_block
 
     odata = bpack_np.unpackbits(
         data,
         bits_per_sample,
         samples_per_block,
         bit_offset=bit_offset + header_size,
         blockstride=block_size,
+        sign_mode=sign_mode,
     )
 
     extra_bits = len(data) * 8 - bit_offset - block_size * nblocks
     extra_bits = max(extra_bits - header_size, 0)
     extra_samples = extra_bits // bits_per_sample
     assert len(odata) == nblocks * samples_per_block + extra_samples
     k = 1 if header_size > 0 else 0
@@ -398,7 +434,23 @@
 
     with pytest.raises(ValueError):
         bpack_np.unpackbits(
             data,
             bits_per_sample,
             blockstride=bits_per_sample * samples_per_block,
         )
+
+
+@pytest.mark.skipif(not np, reason="numpy not available")
+@pytest.mark.parametrize(
+    ["bits_per_sample", "mode", "ref_mask"],
+    [
+        (3, 0, 0b00000111),
+        (20, 0, 0b000011111111111111111111),
+        (34, 0, 0b0000001111111111111111111111111111111111),
+        (3, 1, 0b11111000),
+        (3, 2, 0b00000100),
+    ],
+)
+def test_make_bitmask(bits_per_sample, mode, ref_mask):
+    mask = bpack_np.make_bitmask(bits_per_sample, mode=mode)
+    assert mask == ref_mask
```

### Comparing `bpack-1.0.0/bpack/tests/test_record_descriptor.py` & `bpack-1.1.0/bpack/tests/test_record_descriptor.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_typing.py` & `bpack-1.1.0/bpack/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack/tests/test_utils.py` & `bpack-1.1.0/bpack/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         class EFlagEnumType(enum.IntFlag):
             A = 1
             B = 2
 
         class EEnumType(enum.Enum):
             A = EFlagEnumType.A
             B = 0
-            c = EFlagEnumType.B
+            C = EFlagEnumType.B
 
         assert bpack.utils.enum_item_type(EEnumType) is int
 
 
 def test_effective_type():
     assert bpack.utils.effective_type(bool) is bool
     assert bpack.utils.effective_type(int) is int
```

### Comparing `bpack-1.0.0/bpack/typing.py` & `bpack-1.1.0/bpack/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """bpack support for type annotations."""
 
 import re
 from typing import NamedTuple, Optional, Type, Union
 
+# @COMPATIBILITY: available in Python 3.7 ... 3.11
 try:
     from typing import _tp_cache
 except ImportError:
 
     def _tp_cache(x):
         return x
```

### Comparing `bpack-1.0.0/bpack/utils.py` & `bpack-1.1.0/bpack/utils.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/bpack.egg-info/PKG-INFO` & `bpack-1.1.0/bpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpack
-Version: 1.0.0
+Version: 1.1.0
 Summary: Binary data structures (un-)packing library
 Author-email: Antonio Valentino <antonio.valentino@tiscali.it>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/avalentino/bpack
 Project-URL: documentation, https://bpack.readthedocs.io
 Project-URL: repository, https://github.com/avalentino/bpack.git
 Project-URL: changelog, https://github.com/avalentino/bpack/blob/main/docs/release_notes.rst
```

### Comparing `bpack-1.0.0/bpack.egg-info/SOURCES.txt` & `bpack-1.1.0/bpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/Makefile` & `bpack-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/_templates/apidoc/package.rst_t` & `bpack-1.1.0/docs/_templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/conf.py` & `bpack-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/development.rst` & `bpack-1.1.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/index.rst` & `bpack-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/installation.rst` & `bpack-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/license.rst` & `bpack-1.1.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/make.bat` & `bpack-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/docs/overview.rst` & `bpack-1.1.0/docs/overview.rst`

 * *Files 12% similar despite different names*

```diff
@@ -61,13 +61,14 @@
 
 
 Possible additional features still not implemented
 --------------------------------------------------
 
 * user defined converters
 * support for complex and datetime data types
+* conversion to CSV, HDF5 and :func:`numpy.dtype`
 
 
 .. _Python: https://www.python.org
 .. _bitstruct: https://github.com/eerimoq/bitstruct
 .. _numpy: https://numpy.org
 .. _bitarray: https://github.com/ilanschnell/bitarray
```

### Comparing `bpack-1.0.0/docs/release_notes.rst` & `bpack-1.1.0/docs/release_notes.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Release Notes
 =============
 
-bpack v1.0.0 (UNRELEASED)
+bpack v1.1.0 (15/04/2023)
+-------------------------
+
+* Added support for signed integers to :func:`bpack.np.unpackbits`.
+  Both standard signed integers and integers encoded with sign and module
+  are now supported.
+* Use uppercase enums in `s1isp.py` example.
+* Improved docstrings in  :mod:`bpack.np`.
+* Fixed several typos. 
+
+
+bpack v1.0.0 (05/02/2023)
 -------------------------
 
 * Fix compatibility with Python v3.11.
 * Move setup configuration form `setup.cfg` to `pyproject.toml`.
 
 
 bpack v0.8.2 (20/03/2022)
```

### Comparing `bpack-1.0.0/docs/userguide.rst` & `bpack-1.1.0/docs/userguide.rst`

 * *Files 0% similar despite different names*

```diff
@@ -755,15 +755,15 @@
 bitarray_ package.
 
 .. _bitstruct: https://github.com/eerimoq/bitstruct
 .. _bitarray: https://github.com/ilanschnell/bitarray
 .. _numpy: https://numpy.org
 
 
-Coded objects
+Codec objects
 ~~~~~~~~~~~~~
 
 Each backend provides a ``Codec`` class that can be used to instantiate
 a *codec* objects.
 
 Please refer to the `Codecs`_ section for a description of basic concepts
 of how decoders work.
```

### Comparing `bpack-1.0.0/examples/packet_decoding.py` & `bpack-1.1.0/examples/packet_decoding.py`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/examples/s1isp.py` & `bpack-1.1.0/examples/s1isp.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,94 +17,94 @@
 
 
 class SyncMarkerException(RuntimeError):
     pass
 
 
 class EEccNumber(enum.IntEnum):
-    # TODO: check "not_set"
-    not_set = 0  # contingency: reserved for ground testing or mode upgrading
-    s1 = 1
-    s2 = 2
-    s3 = 3
-    s4 = 4
-    s5_n = 5
-    s6 = 6
-    iw = 8
-    wm = 9
-    s5_s = 10
-    s1_no_ical = 11
-    s2_no_ical = 12
-    s3_no_ical = 13
-    s4_no_ical = 14
-    rfc = 15
-    test = 16
-    en_s3 = 17
-    an_s1 = 18
-    an_s2 = 19
-    an_s3 = 20
-    an_s4 = 21
-    an_s5_n = 22
-    an_s5_s = 23
-    an_s6 = 24
-    s5_n_no_ical = 25
-    s5_s_no_ical = 26
-    s6_no_ical = 27
-    en_s3_no_ical = 31
-    en = 32
-    an_s1_no_ical = 33
-    an_s3_no_ical = 34
-    an_s6_no_ical = 35
-    nc_s1 = 37
-    nc_s2 = 38
-    nc_s3 = 39
-    nc_s4 = 40
-    nc_s5_n = 41
-    nc_s5_s = 42
-    nc_s6 = 43
-    nc_ew = 44
-    nc_iw = 45
-    nc_wm = 46
+    # TODO: check "NOT_SET"
+    NOT_SET = 0  # CONTINGENCY: RESERVED FOR GROUND TESTING OR MODE UPGRADING
+    S1 = 1
+    S2 = 2
+    S3 = 3
+    S4 = 4
+    S5_N = 5
+    S6 = 6
+    IW = 8
+    WM = 9
+    S5_S = 10
+    S1_NO_ICAL = 11
+    S2_NO_ICAL = 12
+    S3_NO_ICAL = 13
+    S4_NO_ICAL = 14
+    RFC = 15
+    TEST = 16
+    EN_S3 = 17
+    AN_S1 = 18
+    AN_S2 = 19
+    AN_S3 = 20
+    AN_S4 = 21
+    AN_S5_N = 22
+    AN_S5_S = 23
+    AN_S6 = 24
+    S5_N_NO_ICAL = 25
+    S5_S_NO_ICAL = 26
+    S6_NO_ICAL = 27
+    EN_S3_NO_ICAL = 31
+    EN = 32
+    AN_S1_NO_ICAL = 33
+    AN_S3_NO_ICAL = 34
+    AN_S6_NO_ICAL = 35
+    NC_S1 = 37
+    NC_S2 = 38
+    NC_S3 = 39
+    NC_S4 = 40
+    NC_S5_N = 41
+    NC_S5_S = 42
+    NC_S6 = 43
+    NC_EW = 44
+    NC_IW = 45
+    NC_WM = 46
 
 
 class ETestMode(enum.IntEnum):
-    default = 0
-    contingency_rxm_fully_operational = 4  # 100
-    contingency_rxm_fully_bypassed = 5  # 101
-    oper = 6  # 110
-    bypass = 7  # 111
+    DEFAULT = 0
+    CONTINGENCY_RXM_FULLY_OPERATIONAL = 4  # 100
+    CONTINGENCY_RXM_FULLY_BYPASSED = 5  # 101
+    OPER = 6  # 110
+    BYPASS = 7  # 111
 
 
 class ERxChannelId(enum.IntEnum):
     V = 0
     H = 1
 
 
 class EBaqMode(enum.IntEnum):
-    bypass = 0
-    baq3 = 3
-    baq4 = 4
-    baq5 = 5
-    fdbaq_mode_0 = 12
-    fdbaq_mode_1 = 13
-    fdbaq_mode_2 = 14
+    BYPASS = 0
+    BAQ3 = 3
+    BAQ4 = 4
+    BAQ5 = 5
+    FDBAQ_MODE_0 = 12
+    FDBAQ_MODE_1 = 13
+    FDBAQ_MODE_2 = 14
 
 
 class ERangeDecimation(enum.IntEnum):
-    x3_on_4 = 0
-    x2_on_3 = 1
-    x5_on_9 = 3
-    x4_on_9 = 4
-    x3_on_8 = 5
-    x1_on_3 = 6
-    x1_on_6 = 7
-    x3_on_7 = 8
-    x5_on_16 = 9
-    x3_on_26 = 10
-    x4_on_11 = 11
+    X3_ON_4 = 0
+    X2_ON_3 = 1
+    X5_ON_9 = 3
+    X4_ON_9 = 4
+    X3_ON_8 = 5
+    X1_ON_3 = 6
+    X1_ON_6 = 7
+    X3_ON_7 = 8
+    X5_ON_16 = 9
+    X3_ON_26 = 10
+    X4_ON_11 = 11
 
 
 @bpack.bs.decoder
 @bpack.descriptor(baseunits=BITS, byteorder=BE)
 class PacketPrimaryHeader:
     version: T["u3"] = 0
     packet_type: T["u1"] = 0
@@ -124,18 +124,18 @@
 
 
 @bpack.bs.decoder
 @bpack.descriptor(baseunits=BITS, byteorder=BE)
 class FixedAncillaryDataService:
     sync_marker: T["u32"] = SYNK_MARKER
     data_take_id: T["u32"] = 0
-    ecc_num: EEccNumber = bpack.field(size=8, default=EEccNumber.not_set)
+    ecc_num: EEccNumber = bpack.field(size=8, default=EEccNumber.NOT_SET)
     # n. 1 bit n/a
     test_mode: ETestMode = bpack.field(
-        size=3, offset=73, default=ETestMode.default
+        size=3, offset=73, default=ETestMode.DEFAULT
     )
     rx_channel_id: ERxChannelId = bpack.field(size=4, default=ERxChannelId.V)
     instrument_configuration_id: T["u32"] = 0  # NOTE: the data type is TBD
 
 
 @bpack.bs.decoder
 @bpack.descriptor(baseunits=BITS, byteorder=BE)
@@ -151,15 +151,15 @@
     pri_count: T["u32"] = 0
 
 
 @bpack.bs.decoder
 @bpack.descriptor(baseunits=BITS, byteorder=BE)
 class RadarConfigurationSupportService:
     error_flag: bool = False
-    baq_mode: EBaqMode = bpack.field(size=5, offset=3, default=EBaqMode.bypass)
+    baq_mode: EBaqMode = bpack.field(size=5, offset=3, default=EBaqMode.BYPASS)
     baq_block_len: T["u8"] = 0
     # n. 8 bits padding
     range_decimation: ERangeDecimation = bpack.field(
         size=8, offset=24, default=0
     )
     rx_gain: T["u8"] = 0
     tx_ramp_rate: T["u16"] = 0
```

### Comparing `bpack-1.0.0/pyproject.toml` & `bpack-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bpack-1.0.0/tox.ini` & `bpack-1.1.0/tox.ini`

 * *Files identical despite different names*

