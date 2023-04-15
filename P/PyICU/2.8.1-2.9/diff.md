# Comparing `tmp/PyICU-2.8.1.tar.gz` & `tmp/PyICU-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyICU-2.8.1.tar", last modified: Tue Feb  1 02:11:26 2022, max compression
+gzip compressed data, was "PyICU-2.9.tar", last modified: Tue Apr 12 21:52:41 2022, max compression
```

## Comparing `PyICU-2.8.1.tar` & `PyICU-2.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-02-01 02:11:26.065261 PyICU-2.8.1/
--rw-r--r--   0 vajda      (501) wheel        (0)    19962 2022-02-01 02:09:40.000000 PyICU-2.8.1/CHANGES
--rw-r--r--   0 vajda      (501) wheel        (0)      938 2021-05-21 19:00:11.000000 PyICU-2.8.1/CREDITS
--rw-r--r--   0 vajda      (501) wheel        (0)     1289 2022-01-23 02:07:04.000000 PyICU-2.8.1/LICENSE
--rw-r--r--   0 vajda      (501) wheel        (0)      796 2021-05-21 19:49:12.000000 PyICU-2.8.1/MANIFEST.in
--rw-r--r--   0 vajda      (501) wheel        (0)    13797 2022-02-01 02:11:26.064986 PyICU-2.8.1/PKG-INFO
--rw-r--r--   0 vajda      (501) wheel        (0)    12843 2021-10-22 23:14:18.000000 PyICU-2.8.1/README.md
--rw-r--r--   0 vajda      (501) wheel        (0)     9180 2022-01-23 02:44:39.000000 PyICU-2.8.1/_icu_.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)    76072 2021-04-01 21:28:41.000000 PyICU-2.8.1/bases.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     2918 2021-04-01 21:28:41.000000 PyICU-2.8.1/bases.h
--rw-r--r--   0 vajda      (501) wheel        (0)    34270 2021-04-01 21:28:41.000000 PyICU-2.8.1/bidi.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1368 2021-04-01 21:28:41.000000 PyICU-2.8.1/bidi.h
--rw-r--r--   0 vajda      (501) wheel        (0)    29835 2021-04-10 19:14:19.000000 PyICU-2.8.1/calendar.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1469 2021-04-10 19:01:13.000000 PyICU-2.8.1/calendar.h
--rw-r--r--   0 vajda      (501) wheel        (0)    47795 2021-04-01 21:28:41.000000 PyICU-2.8.1/casemap.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1385 2021-04-01 21:28:41.000000 PyICU-2.8.1/casemap.h
--rw-r--r--   0 vajda      (501) wheel        (0)    85011 2021-10-29 17:48:10.000000 PyICU-2.8.1/char.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1375 2021-04-01 21:28:41.000000 PyICU-2.8.1/char.h
--rw-r--r--   0 vajda      (501) wheel        (0)    10539 2021-04-01 21:28:41.000000 PyICU-2.8.1/charset.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1388 2021-04-01 21:28:41.000000 PyICU-2.8.1/charset.h
--rw-r--r--   0 vajda      (501) wheel        (0)    45560 2021-06-17 14:10:37.000000 PyICU-2.8.1/collator.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1511 2021-04-01 21:28:41.000000 PyICU-2.8.1/collator.h
--rw-r--r--   0 vajda      (501) wheel        (0)    45370 2021-05-01 22:38:33.000000 PyICU-2.8.1/common.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)    13735 2021-10-04 18:06:02.000000 PyICU-2.8.1/common.h
--rw-r--r--   0 vajda      (501) wheel        (0)    88277 2021-04-10 20:11:11.000000 PyICU-2.8.1/dateformat.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1681 2021-04-01 21:28:41.000000 PyICU-2.8.1/dateformat.h
--rw-r--r--   0 vajda      (501) wheel        (0)    14427 2021-10-04 17:43:18.000000 PyICU-2.8.1/errors.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1384 2021-04-01 21:28:41.000000 PyICU-2.8.1/errors.h
--rw-r--r--   0 vajda      (501) wheel        (0)    70808 2021-04-06 21:39:38.000000 PyICU-2.8.1/format.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     2429 2021-04-01 21:28:41.000000 PyICU-2.8.1/format.h
--rw-r--r--   0 vajda      (501) wheel        (0)     3269 2021-04-01 21:28:41.000000 PyICU-2.8.1/gender.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1378 2021-04-01 21:28:41.000000 PyICU-2.8.1/gender.h
--rw-r--r--   0 vajda      (501) wheel        (0)     9320 2021-04-01 21:28:41.000000 PyICU-2.8.1/idna.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1442 2021-04-01 21:28:41.000000 PyICU-2.8.1/idna.h
--rw-r--r--   0 vajda      (501) wheel        (0)    49407 2021-05-13 19:36:29.000000 PyICU-2.8.1/iterators.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1607 2021-04-01 21:28:41.000000 PyICU-2.8.1/iterators.h
--rw-r--r--   0 vajda      (501) wheel        (0)    30298 2021-04-01 21:28:41.000000 PyICU-2.8.1/layoutengine.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1407 2021-04-01 21:28:41.000000 PyICU-2.8.1/layoutengine.h
--rw-r--r--   0 vajda      (501) wheel        (0)    83938 2021-05-03 15:08:30.000000 PyICU-2.8.1/locale.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1514 2021-04-01 21:28:41.000000 PyICU-2.8.1/locale.h
--rw-r--r--   0 vajda      (501) wheel        (0)    27468 2021-04-01 21:28:41.000000 PyICU-2.8.1/macros.h
--rw-r--r--   0 vajda      (501) wheel        (0)    58772 2021-10-04 18:56:19.000000 PyICU-2.8.1/measureunit.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1569 2021-04-01 21:28:41.000000 PyICU-2.8.1/measureunit.h
--rw-r--r--   0 vajda      (501) wheel        (0)    17254 2021-05-21 20:11:20.000000 PyICU-2.8.1/messagepattern.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1413 2021-05-21 19:48:20.000000 PyICU-2.8.1/messagepattern.h
--rw-r--r--   0 vajda      (501) wheel        (0)    24575 2021-04-01 21:28:41.000000 PyICU-2.8.1/normalizer.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1399 2021-04-01 21:28:41.000000 PyICU-2.8.1/normalizer.h
--rw-r--r--   0 vajda      (501) wheel        (0)   181025 2021-10-22 18:09:01.000000 PyICU-2.8.1/numberformat.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     2337 2021-04-01 21:28:41.000000 PyICU-2.8.1/numberformat.h
-drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-02-01 02:11:26.035581 PyICU-2.8.1/py/
-drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-02-01 02:11:26.057587 PyICU-2.8.1/py/PyICU.egg-info/
--rw-r--r--   0 vajda      (501) wheel        (0)    13797 2022-02-01 02:11:26.000000 PyICU-2.8.1/py/PyICU.egg-info/PKG-INFO
--rw-r--r--   0 vajda      (501) wheel        (0)     1652 2022-02-01 02:11:26.000000 PyICU-2.8.1/py/PyICU.egg-info/SOURCES.txt
--rw-r--r--   0 vajda      (501) wheel        (0)        1 2022-02-01 02:11:26.000000 PyICU-2.8.1/py/PyICU.egg-info/dependency_links.txt
--rw-r--r--   0 vajda      (501) wheel        (0)        4 2022-02-01 02:11:26.000000 PyICU-2.8.1/py/PyICU.egg-info/top_level.txt
-drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-02-01 02:11:26.057783 PyICU-2.8.1/py/icu/
--rw-r--r--   0 vajda      (501) wheel        (0)     1547 2022-01-25 02:10:08.000000 PyICU-2.8.1/py/icu/__init__.py
--rw-r--r--   0 vajda      (501) wheel        (0)      102 2021-10-21 23:42:21.000000 PyICU-2.8.1/pyproject.toml
--rw-r--r--   0 vajda      (501) wheel        (0)    29220 2021-04-01 21:28:41.000000 PyICU-2.8.1/regex.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1379 2021-04-01 21:28:41.000000 PyICU-2.8.1/regex.h
-drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-02-01 02:11:26.058171 PyICU-2.8.1/samples/
--rw-r--r--   0 vajda      (501) wheel        (0)     3950 2021-04-01 21:28:41.000000 PyICU-2.8.1/samples/break.py
--rw-r--r--   0 vajda      (501) wheel        (0)     6660 2021-04-01 21:28:41.000000 PyICU-2.8.1/samples/strsrch.py
--rw-r--r--   0 vajda      (501) wheel        (0)    24008 2021-10-04 17:33:06.000000 PyICU-2.8.1/script.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1383 2021-04-01 21:28:41.000000 PyICU-2.8.1/script.h
--rw-r--r--   0 vajda      (501) wheel        (0)    20255 2021-04-01 21:28:41.000000 PyICU-2.8.1/search.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1384 2021-04-01 21:28:41.000000 PyICU-2.8.1/search.h
--rw-r--r--   0 vajda      (501) wheel        (0)       38 2022-02-01 02:11:26.065342 PyICU-2.8.1/setup.cfg
--rw-r--r--   0 vajda      (501) wheel        (0)     8925 2022-02-01 02:09:47.000000 PyICU-2.8.1/setup.py
--rw-r--r--   0 vajda      (501) wheel        (0)     7527 2021-04-01 21:28:41.000000 PyICU-2.8.1/shape.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1379 2021-04-01 21:28:41.000000 PyICU-2.8.1/shape.h
--rw-r--r--   0 vajda      (501) wheel        (0)    12469 2021-04-01 21:28:41.000000 PyICU-2.8.1/spoof.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1424 2021-04-01 21:28:41.000000 PyICU-2.8.1/spoof.h
-drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-02-01 02:11:26.064672 PyICU-2.8.1/test/
--rw-r--r--   0 vajda      (501) wheel        (0)      818 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/__init__.py
--rw-r--r--   0 vajda      (501) wheel        (0)    87277 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/collation-rules.txt
--rw-r--r--   0 vajda      (501) wheel        (0)    81484 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/lohit_hi.ttf
--rw-r--r--   0 vajda      (501) wheel        (0)       49 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/noms.txt
--rw-r--r--   0 vajda      (501) wheel        (0)     4413 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Bidi.py
--rw-r--r--   0 vajda      (501) wheel        (0)     2739 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_BreakIterator.py
--rw-r--r--   0 vajda      (501) wheel        (0)     2787 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_BytesTrie.py
--rw-r--r--   0 vajda      (501) wheel        (0)     2555 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Charset.py
--rw-r--r--   0 vajda      (501) wheel        (0)     6096 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Collator.py
--rw-r--r--   0 vajda      (501) wheel        (0)     5182 2021-10-02 00:07:36.000000 PyICU-2.8.1/test/test_DateTimePatternGenerator.py
--rw-r--r--   0 vajda      (501) wheel        (0)     4382 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_LayoutEngine.py
--rw-r--r--   0 vajda      (501) wheel        (0)     1821 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_ListFormatter.py
--rw-r--r--   0 vajda      (501) wheel        (0)     1802 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Locale.py
--rw-r--r--   0 vajda      (501) wheel        (0)    10107 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_LocaleData.py
--rw-r--r--   0 vajda      (501) wheel        (0)     4156 2021-05-03 15:13:28.000000 PyICU-2.8.1/test/test_LocaleMatcher.py
--rw-r--r--   0 vajda      (501) wheel        (0)     3909 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_MessageFormat.py
--rw-r--r--   0 vajda      (501) wheel        (0)     3560 2021-05-21 20:13:58.000000 PyICU-2.8.1/test/test_MessagePattern.py
--rw-r--r--   0 vajda      (501) wheel        (0)     2584 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Normalizer.py
--rw-r--r--   0 vajda      (501) wheel        (0)     2154 2021-10-22 23:04:54.000000 PyICU-2.8.1/test/test_NumberFormat.py
--rw-r--r--   0 vajda      (501) wheel        (0)     7933 2021-10-04 18:48:52.000000 PyICU-2.8.1/test/test_NumberFormatter.py
--rw-r--r--   0 vajda      (501) wheel        (0)     3341 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_PythonReplaceable.py
--rw-r--r--   0 vajda      (501) wheel        (0)     3794 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Script.py
--rw-r--r--   0 vajda      (501) wheel        (0)     1732 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_SimpleFormatter.py
--rw-r--r--   0 vajda      (501) wheel        (0)     7486 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Spoof.py
--rw-r--r--   0 vajda      (501) wheel        (0)     3304 2021-10-29 17:38:26.000000 PyICU-2.8.1/test/test_TimeZone.py
--rw-r--r--   0 vajda      (501) wheel        (0)     3701 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_Transliterator.py
--rw-r--r--   0 vajda      (501) wheel        (0)     1957 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_UCS4.py
--rw-r--r--   0 vajda      (501) wheel        (0)     2791 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_UCharsTrie.py
--rw-r--r--   0 vajda      (501) wheel        (0)     1938 2021-04-01 21:28:41.000000 PyICU-2.8.1/test/test_UDate.py
--rw-r--r--   0 vajda      (501) wheel        (0)    56937 2021-10-04 16:04:12.000000 PyICU-2.8.1/timezone.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1693 2021-04-10 19:03:03.000000 PyICU-2.8.1/timezone.h
--rw-r--r--   0 vajda      (501) wheel        (0)    24683 2021-04-01 21:28:41.000000 PyICU-2.8.1/transliterator.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     2808 2021-04-01 21:28:41.000000 PyICU-2.8.1/transliterator.h
--rw-r--r--   0 vajda      (501) wheel        (0)    25656 2021-04-01 21:28:41.000000 PyICU-2.8.1/tries.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1374 2021-04-01 21:28:41.000000 PyICU-2.8.1/tries.h
--rw-r--r--   0 vajda      (501) wheel        (0)    23491 2021-04-10 19:10:25.000000 PyICU-2.8.1/tzinfo.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1383 2021-04-01 21:28:41.000000 PyICU-2.8.1/tzinfo.h
--rw-r--r--   0 vajda      (501) wheel        (0)    40332 2021-04-01 21:28:41.000000 PyICU-2.8.1/unicodeset.cpp
--rw-r--r--   0 vajda      (501) wheel        (0)     1577 2021-04-01 21:28:41.000000 PyICU-2.8.1/unicodeset.h
+drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-04-12 21:52:41.476041 PyICU-2.9/
+-rw-r--r--   0 vajda      (501) wheel        (0)    20259 2022-04-12 21:51:49.000000 PyICU-2.9/CHANGES
+-rw-r--r--   0 vajda      (501) wheel        (0)      938 2021-05-21 19:00:11.000000 PyICU-2.9/CREDITS
+-rw-r--r--   0 vajda      (501) wheel        (0)     1289 2022-01-23 02:07:04.000000 PyICU-2.9/LICENSE
+-rw-r--r--   0 vajda      (501) wheel        (0)      796 2021-05-21 19:49:12.000000 PyICU-2.9/MANIFEST.in
+-rw-r--r--   0 vajda      (501) wheel        (0)    13795 2022-04-12 21:52:41.475682 PyICU-2.9/PKG-INFO
+-rw-r--r--   0 vajda      (501) wheel        (0)    12843 2021-10-22 23:14:18.000000 PyICU-2.9/README.md
+-rw-r--r--   0 vajda      (501) wheel        (0)     9180 2022-01-23 02:44:39.000000 PyICU-2.9/_icu_.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)    76072 2021-04-01 21:28:41.000000 PyICU-2.9/bases.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     2918 2021-04-01 21:28:41.000000 PyICU-2.9/bases.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    34270 2021-04-01 21:28:41.000000 PyICU-2.9/bidi.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1368 2021-04-01 21:28:41.000000 PyICU-2.9/bidi.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    29835 2021-04-10 19:14:19.000000 PyICU-2.9/calendar.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1469 2021-04-10 19:01:13.000000 PyICU-2.9/calendar.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    47795 2021-04-01 21:28:41.000000 PyICU-2.9/casemap.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1385 2021-04-01 21:28:41.000000 PyICU-2.9/casemap.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    85011 2021-10-29 17:48:10.000000 PyICU-2.9/char.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1375 2021-04-01 21:28:41.000000 PyICU-2.9/char.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    10539 2021-04-01 21:28:41.000000 PyICU-2.9/charset.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1388 2021-04-01 21:28:41.000000 PyICU-2.9/charset.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    45560 2021-06-17 14:10:37.000000 PyICU-2.9/collator.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1511 2021-04-01 21:28:41.000000 PyICU-2.9/collator.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    45370 2021-05-01 22:38:33.000000 PyICU-2.9/common.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)    13735 2021-10-04 18:06:02.000000 PyICU-2.9/common.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    88277 2021-04-10 20:11:11.000000 PyICU-2.9/dateformat.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1681 2021-04-01 21:28:41.000000 PyICU-2.9/dateformat.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    14427 2021-10-04 17:43:18.000000 PyICU-2.9/errors.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1384 2021-04-01 21:28:41.000000 PyICU-2.9/errors.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    70808 2021-04-06 21:39:38.000000 PyICU-2.9/format.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     2429 2021-04-01 21:28:41.000000 PyICU-2.9/format.h
+-rw-r--r--   0 vajda      (501) wheel        (0)     3269 2021-04-01 21:28:41.000000 PyICU-2.9/gender.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1378 2021-04-01 21:28:41.000000 PyICU-2.9/gender.h
+-rw-r--r--   0 vajda      (501) wheel        (0)     9320 2021-04-01 21:28:41.000000 PyICU-2.9/idna.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1442 2021-04-01 21:28:41.000000 PyICU-2.9/idna.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    49407 2021-05-13 19:36:29.000000 PyICU-2.9/iterators.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1607 2021-04-01 21:28:41.000000 PyICU-2.9/iterators.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    30298 2021-04-01 21:28:41.000000 PyICU-2.9/layoutengine.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1407 2021-04-01 21:28:41.000000 PyICU-2.9/layoutengine.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    83938 2021-05-03 15:08:30.000000 PyICU-2.9/locale.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1514 2021-04-01 21:28:41.000000 PyICU-2.9/locale.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    27468 2021-04-01 21:28:41.000000 PyICU-2.9/macros.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    61911 2022-03-22 16:39:10.000000 PyICU-2.9/measureunit.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1569 2021-04-01 21:28:41.000000 PyICU-2.9/measureunit.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    17254 2021-05-21 20:11:20.000000 PyICU-2.9/messagepattern.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1413 2021-05-21 19:48:20.000000 PyICU-2.9/messagepattern.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    24575 2021-04-01 21:28:41.000000 PyICU-2.9/normalizer.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1399 2021-04-01 21:28:41.000000 PyICU-2.9/normalizer.h
+-rw-r--r--   0 vajda      (501) wheel        (0)   183533 2022-03-22 17:04:31.000000 PyICU-2.9/numberformat.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     2337 2021-04-01 21:28:41.000000 PyICU-2.9/numberformat.h
+drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-04-12 21:52:30.303090 PyICU-2.9/py/
+drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-04-12 21:52:41.446911 PyICU-2.9/py/PyICU.egg-info/
+-rw-r--r--   0 vajda      (501) wheel        (0)    13795 2022-04-12 21:52:29.000000 PyICU-2.9/py/PyICU.egg-info/PKG-INFO
+-rw-r--r--   0 vajda      (501) wheel        (0)     1652 2022-04-12 21:52:30.000000 PyICU-2.9/py/PyICU.egg-info/SOURCES.txt
+-rw-r--r--   0 vajda      (501) wheel        (0)        1 2022-04-12 21:52:29.000000 PyICU-2.9/py/PyICU.egg-info/dependency_links.txt
+-rw-r--r--   0 vajda      (501) wheel        (0)        4 2022-04-12 21:52:30.000000 PyICU-2.9/py/PyICU.egg-info/top_level.txt
+drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-04-12 21:52:41.447313 PyICU-2.9/py/icu/
+-rw-r--r--   0 vajda      (501) wheel        (0)     1547 2022-01-25 02:10:08.000000 PyICU-2.9/py/icu/__init__.py
+-rw-r--r--   0 vajda      (501) wheel        (0)      102 2021-10-21 23:42:21.000000 PyICU-2.9/pyproject.toml
+-rw-r--r--   0 vajda      (501) wheel        (0)    29220 2021-04-01 21:28:41.000000 PyICU-2.9/regex.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1379 2021-04-01 21:28:41.000000 PyICU-2.9/regex.h
+drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-04-12 21:52:41.449005 PyICU-2.9/samples/
+-rw-r--r--   0 vajda      (501) wheel        (0)     3950 2021-04-01 21:28:41.000000 PyICU-2.9/samples/break.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     6660 2021-04-01 21:28:41.000000 PyICU-2.9/samples/strsrch.py
+-rw-r--r--   0 vajda      (501) wheel        (0)    24008 2021-10-04 17:33:06.000000 PyICU-2.9/script.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1383 2021-04-01 21:28:41.000000 PyICU-2.9/script.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    20255 2021-04-01 21:28:41.000000 PyICU-2.9/search.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1384 2021-04-01 21:28:41.000000 PyICU-2.9/search.h
+-rw-r--r--   0 vajda      (501) wheel        (0)       38 2022-04-12 21:52:41.476152 PyICU-2.9/setup.cfg
+-rw-r--r--   0 vajda      (501) wheel        (0)     8923 2022-04-12 21:51:58.000000 PyICU-2.9/setup.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     7527 2021-04-01 21:28:41.000000 PyICU-2.9/shape.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1379 2021-04-01 21:28:41.000000 PyICU-2.9/shape.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    12469 2021-04-01 21:28:41.000000 PyICU-2.9/spoof.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1424 2021-04-01 21:28:41.000000 PyICU-2.9/spoof.h
+drwxr-xr-x   0 vajda      (501) wheel        (0)        0 2022-04-12 21:52:41.475166 PyICU-2.9/test/
+-rw-r--r--   0 vajda      (501) wheel        (0)      818 2021-04-01 21:28:41.000000 PyICU-2.9/test/__init__.py
+-rw-r--r--   0 vajda      (501) wheel        (0)    87277 2021-04-01 21:28:41.000000 PyICU-2.9/test/collation-rules.txt
+-rw-r--r--   0 vajda      (501) wheel        (0)    81484 2021-04-01 21:28:41.000000 PyICU-2.9/test/lohit_hi.ttf
+-rw-r--r--   0 vajda      (501) wheel        (0)       49 2021-04-01 21:28:41.000000 PyICU-2.9/test/noms.txt
+-rw-r--r--   0 vajda      (501) wheel        (0)     4413 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Bidi.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     2739 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_BreakIterator.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     2787 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_BytesTrie.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     2555 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Charset.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     6096 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Collator.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     5230 2022-03-22 16:11:00.000000 PyICU-2.9/test/test_DateTimePatternGenerator.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     4382 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_LayoutEngine.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     1821 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_ListFormatter.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     1802 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Locale.py
+-rw-r--r--   0 vajda      (501) wheel        (0)    10107 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_LocaleData.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     4156 2021-05-03 15:13:28.000000 PyICU-2.9/test/test_LocaleMatcher.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     3909 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_MessageFormat.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     3560 2021-05-21 20:13:58.000000 PyICU-2.9/test/test_MessagePattern.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     2584 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Normalizer.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     2154 2021-10-22 23:04:54.000000 PyICU-2.9/test/test_NumberFormat.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     7933 2021-10-04 18:48:52.000000 PyICU-2.9/test/test_NumberFormatter.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     3341 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_PythonReplaceable.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     3794 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Script.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     1732 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_SimpleFormatter.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     7486 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Spoof.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     3304 2021-10-29 17:38:26.000000 PyICU-2.9/test/test_TimeZone.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     3701 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_Transliterator.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     1957 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_UCS4.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     2791 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_UCharsTrie.py
+-rw-r--r--   0 vajda      (501) wheel        (0)     1938 2021-04-01 21:28:41.000000 PyICU-2.9/test/test_UDate.py
+-rw-r--r--   0 vajda      (501) wheel        (0)    56937 2021-10-04 16:04:12.000000 PyICU-2.9/timezone.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1693 2021-04-10 19:03:03.000000 PyICU-2.9/timezone.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    24683 2021-04-01 21:28:41.000000 PyICU-2.9/transliterator.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     2808 2021-04-01 21:28:41.000000 PyICU-2.9/transliterator.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    25656 2021-04-01 21:28:41.000000 PyICU-2.9/tries.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1374 2021-04-01 21:28:41.000000 PyICU-2.9/tries.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    23491 2021-04-10 19:10:25.000000 PyICU-2.9/tzinfo.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1383 2021-04-01 21:28:41.000000 PyICU-2.9/tzinfo.h
+-rw-r--r--   0 vajda      (501) wheel        (0)    40332 2021-04-01 21:28:41.000000 PyICU-2.9/unicodeset.cpp
+-rw-r--r--   0 vajda      (501) wheel        (0)     1577 2021-04-01 21:28:41.000000 PyICU-2.9/unicodeset.h
```

### Comparing `PyICU-2.8.1/CHANGES` & `PyICU-2.9/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Version 2.8.1 -> 2.9
+--------------------
+  - added support for ICU 71.1
+  - added wrappers for UMeasurePrefix, MeasureUnit.withPrefix()|getPrefix()
+  - added UNumberRoundingPriority, FractionPrecision.withSignificantDigits()
+  - added UNumberTrailingZeroDisplay, Precision.trailingZeroDisplay()
+
 Version 2.8 -> 2.8.1
 --------------------
   - renamed _icu extension module to _icu_ and moved it into icu module
   - moved icu python module sources into py directory
   - deleted long deprecated PyICU.py file
 
 Version 2.7.4 -> 2.8
```

### Comparing `PyICU-2.8.1/CREDITS` & `PyICU-2.9/CREDITS`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/LICENSE` & `PyICU-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/MANIFEST.in` & `PyICU-2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/PKG-INFO` & `PyICU-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyICU
-Version: 2.8.1
+Version: 2.9
 Summary: Python extension wrapping the ICU C++ API
 Home-page: https://gitlab.pyicu.org/main/pyicu
 Author: Andi Vajda
 Author-email: vajda@pyicu.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyICU-2.8.1/README.md` & `PyICU-2.9/README.md`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/_icu_.cpp` & `PyICU-2.9/_icu_.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/bases.cpp` & `PyICU-2.9/bases.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/bases.h` & `PyICU-2.9/bases.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/bidi.cpp` & `PyICU-2.9/bidi.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/bidi.h` & `PyICU-2.9/bidi.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/calendar.cpp` & `PyICU-2.9/calendar.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/calendar.h` & `PyICU-2.9/calendar.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/casemap.cpp` & `PyICU-2.9/casemap.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/casemap.h` & `PyICU-2.9/casemap.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/char.cpp` & `PyICU-2.9/char.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/char.h` & `PyICU-2.9/char.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/charset.cpp` & `PyICU-2.9/charset.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/charset.h` & `PyICU-2.9/charset.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/collator.cpp` & `PyICU-2.9/collator.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/collator.h` & `PyICU-2.9/collator.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/common.cpp` & `PyICU-2.9/common.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/common.h` & `PyICU-2.9/common.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/dateformat.cpp` & `PyICU-2.9/dateformat.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/dateformat.h` & `PyICU-2.9/dateformat.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/errors.cpp` & `PyICU-2.9/errors.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/errors.h` & `PyICU-2.9/errors.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/format.cpp` & `PyICU-2.9/format.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/format.h` & `PyICU-2.9/format.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/gender.cpp` & `PyICU-2.9/gender.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/gender.h` & `PyICU-2.9/gender.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/idna.cpp` & `PyICU-2.9/idna.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/idna.h` & `PyICU-2.9/idna.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/iterators.cpp` & `PyICU-2.9/iterators.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/iterators.h` & `PyICU-2.9/iterators.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/layoutengine.cpp` & `PyICU-2.9/layoutengine.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/layoutengine.h` & `PyICU-2.9/layoutengine.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/locale.cpp` & `PyICU-2.9/locale.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/locale.h` & `PyICU-2.9/locale.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/macros.h` & `PyICU-2.9/macros.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/measureunit.cpp` & `PyICU-2.9/measureunit.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /* ====================================================================
- * Copyright (c) 2004-2019 Open Source Applications Foundation.
+ * Copyright (c) 2004-2022 Open Source Applications Foundation.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a
  * copy of this software and associated documentation files (the "Software"),
  * to deal in the Software without restriction, including without limitation
  * the rights to use, copy, modify, merge, publish, distribute, sublicense,
  * and/or sell copies of the Software, and to permit persons to whom the
  * Software is furnished to do so, subject to the following conditions:
@@ -33,14 +33,18 @@
 DECLARE_CONSTANTS_TYPE(UTimeUnitFields)
 #endif
 
 #if U_ICU_VERSION_HEX >= VERSION_HEX(67, 0, 0)
 DECLARE_CONSTANTS_TYPE(UMeasureUnitComplexity)
 #endif
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+DECLARE_CONSTANTS_TYPE(UMeasurePrefix)
+#endif
+
 DECLARE_CONSTANTS_TYPE(UCurrNameStyle)
 
 /* MeasureUnit */
 
 class t_measureunit : public _wrapper {
 public:
     MeasureUnit *object;
@@ -57,14 +61,19 @@
 static PyObject *t_measureunit_getComplexity(t_measureunit *self);
 static PyObject *t_measureunit_getDimensionality(t_measureunit *self);
 static PyObject *t_measureunit_product(t_measureunit *self, PyObject *arg);
 static PyObject *t_measureunit_reciprocal(t_measureunit *self);
 static PyObject *t_measureunit_forIdentifier(PyTypeObject *type, PyObject *arg);
 #endif
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+static PyObject *t_measureunit_withPrefix(t_measureunit *self, PyObject *arg);
+static PyObject *t_measureunit_getPrefix(t_measureunit *self);
+#endif
+
 #if U_ICU_VERSION_HEX >= VERSION_HEX(53, 0, 0)
 static PyObject *t_measureunit_createAcre(PyTypeObject *type);
 static PyObject *t_measureunit_createArcMinute(PyTypeObject *type);
 static PyObject *t_measureunit_createArcSecond(PyTypeObject *type);
 static PyObject *t_measureunit_createCelsius(PyTypeObject *type);
 static PyObject *t_measureunit_createCentimeter(PyTypeObject *type);
 static PyObject *t_measureunit_createCubicKilometer(PyTypeObject *type);
@@ -284,14 +293,19 @@
     DECLARE_METHOD(t_measureunit, getComplexity, METH_NOARGS),
     DECLARE_METHOD(t_measureunit, getDimensionality, METH_NOARGS),
     DECLARE_METHOD(t_measureunit, product, METH_O),
     DECLARE_METHOD(t_measureunit, reciprocal, METH_NOARGS),
     DECLARE_METHOD(t_measureunit, forIdentifier, METH_CLASS | METH_O),
 #endif
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+    DECLARE_METHOD(t_measureunit, withPrefix, METH_O),
+    DECLARE_METHOD(t_measureunit, getPrefix, METH_NOARGS),
+#endif
+
 #if U_ICU_VERSION_HEX >= VERSION_HEX(53, 0, 0)
     DECLARE_METHOD(t_measureunit, createAcre, METH_NOARGS | METH_CLASS),
     DECLARE_METHOD(t_measureunit, createArcMinute, METH_NOARGS | METH_CLASS),
     DECLARE_METHOD(t_measureunit, createArcSecond, METH_NOARGS | METH_CLASS),
     DECLARE_METHOD(t_measureunit, createCelsius, METH_NOARGS | METH_CLASS),
     DECLARE_METHOD(t_measureunit, createCentimeter, METH_NOARGS | METH_CLASS),
     DECLARE_METHOD(t_measureunit, createCubicKilometer, METH_NOARGS | METH_CLASS),
@@ -851,14 +865,41 @@
 
         return wrap_MeasureUnit((MeasureUnit *) mu.clone(), T_OWNED);
     }
 
     return PyErr_SetArgsError(type, "forIdentifier", arg);
 }
 
+#endif  // ICU >= 67
+
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+
+static PyObject *t_measureunit_withPrefix(t_measureunit *self, PyObject *arg)
+{
+    UMeasurePrefix prefix;
+
+    if (!parseArg(arg, "i", &prefix))
+    {
+        MeasureUnit mu;
+        STATUS_CALL(mu = self->object->withPrefix(prefix, status));
+
+        return wrap_MeasureUnit((MeasureUnit *) mu.clone(), T_OWNED);
+    }
+
+    return PyErr_SetArgsError((PyObject *) self, "withPrefix", arg);
+}
+
+static PyObject *t_measureunit_getPrefix(t_measureunit *self)
+{
+    UMeasurePrefix prefix;
+    STATUS_CALL(prefix = self->object->getPrefix(status));
+
+    return PyInt_FromLong(prefix);
+}
+
 #endif
 
 
 #if U_ICU_VERSION_HEX >= VERSION_HEX(53, 0, 0)
 
 #define createMU(unit) \
     static PyObject *t_measureunit_create ## unit(PyTypeObject *type) \
@@ -1473,14 +1514,17 @@
 
 #if U_ICU_VERSION_HEX >= 0x04020000
     INSTALL_CONSTANTS_TYPE(UTimeUnitFields, m);
 #endif
 #if U_ICU_VERSION_HEX >= VERSION_HEX(67, 0, 0)
     INSTALL_CONSTANTS_TYPE(UMeasureUnitComplexity, m);
 #endif
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+    INSTALL_CONSTANTS_TYPE(UMeasurePrefix, m);
+#endif
     INSTALL_CONSTANTS_TYPE(UCurrNameStyle, m);
 
     INSTALL_TYPE(MeasureUnit, m);
     INSTALL_TYPE(Measure, m);
 #if U_ICU_VERSION_HEX >= VERSION_HEX(60, 0, 0)
 #if U_ICU_VERSION_HEX < VERSION_HEX(68, 0, 0)
     REGISTER_TYPE(NoUnit, m);
@@ -1516,8 +1560,40 @@
 #if U_ICU_VERSION_HEX >= VERSION_HEX(61, 0, 0)
     INSTALL_ENUM(UCurrNameStyle, "NARROW_SYMBOL_NAME", UCURR_NARROW_SYMBOL_NAME);
 #endif
 #if U_ICU_VERSION_HEX >= VERSION_HEX(68, 0, 0)
     INSTALL_ENUM(UCurrNameStyle, "FORMAL_SYMBOL_NAME", UCURR_FORMAL_SYMBOL_NAME);
     INSTALL_ENUM(UCurrNameStyle, "VARIANT_SYMBOL_NAME", UCURR_VARIANT_SYMBOL_NAME);
 #endif    
+
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+    INSTALL_ENUM(UMeasurePrefix, "ONE", UMEASURE_PREFIX_ONE);
+    INSTALL_ENUM(UMeasurePrefix, "YOTTA", UMEASURE_PREFIX_YOTTA);
+    INSTALL_ENUM(UMeasurePrefix, "ZETTA", UMEASURE_PREFIX_ZETTA);
+    INSTALL_ENUM(UMeasurePrefix, "EXA", UMEASURE_PREFIX_EXA);
+    INSTALL_ENUM(UMeasurePrefix, "PETA", UMEASURE_PREFIX_PETA);
+    INSTALL_ENUM(UMeasurePrefix, "TERA", UMEASURE_PREFIX_TERA);
+    INSTALL_ENUM(UMeasurePrefix, "GIGA", UMEASURE_PREFIX_GIGA);
+    INSTALL_ENUM(UMeasurePrefix, "MEGA", UMEASURE_PREFIX_MEGA);
+    INSTALL_ENUM(UMeasurePrefix, "KILO", UMEASURE_PREFIX_KILO);
+    INSTALL_ENUM(UMeasurePrefix, "HECTO", UMEASURE_PREFIX_HECTO);
+    INSTALL_ENUM(UMeasurePrefix, "DEKA", UMEASURE_PREFIX_DEKA);
+    INSTALL_ENUM(UMeasurePrefix, "DECI", UMEASURE_PREFIX_DECI);
+    INSTALL_ENUM(UMeasurePrefix, "CENTI", UMEASURE_PREFIX_CENTI);
+    INSTALL_ENUM(UMeasurePrefix, "MILLI", UMEASURE_PREFIX_MILLI);
+    INSTALL_ENUM(UMeasurePrefix, "MICRO", UMEASURE_PREFIX_MICRO);
+    INSTALL_ENUM(UMeasurePrefix, "NANO", UMEASURE_PREFIX_NANO);
+    INSTALL_ENUM(UMeasurePrefix, "PICO", UMEASURE_PREFIX_PICO);
+    INSTALL_ENUM(UMeasurePrefix, "FEMTO", UMEASURE_PREFIX_FEMTO);
+    INSTALL_ENUM(UMeasurePrefix, "ATTO", UMEASURE_PREFIX_ATTO);
+    INSTALL_ENUM(UMeasurePrefix, "ZEPTO", UMEASURE_PREFIX_ZEPTO);
+    INSTALL_ENUM(UMeasurePrefix, "YOCTO", UMEASURE_PREFIX_YOCTO);
+    INSTALL_ENUM(UMeasurePrefix, "KIBI", UMEASURE_PREFIX_KIBI);
+    INSTALL_ENUM(UMeasurePrefix, "MEBI", UMEASURE_PREFIX_MEBI);
+    INSTALL_ENUM(UMeasurePrefix, "GIBI", UMEASURE_PREFIX_GIBI);
+    INSTALL_ENUM(UMeasurePrefix, "TEBI", UMEASURE_PREFIX_TEBI);
+    INSTALL_ENUM(UMeasurePrefix, "PEBI", UMEASURE_PREFIX_PEBI);
+    INSTALL_ENUM(UMeasurePrefix, "EXBI", UMEASURE_PREFIX_EXBI);
+    INSTALL_ENUM(UMeasurePrefix, "ZEBI", UMEASURE_PREFIX_ZEBI);
+    INSTALL_ENUM(UMeasurePrefix, "YOBI", UMEASURE_PREFIX_YOBI);
+#endif
 }
```

### Comparing `PyICU-2.8.1/measureunit.h` & `PyICU-2.9/measureunit.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/messagepattern.cpp` & `PyICU-2.9/messagepattern.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/messagepattern.h` & `PyICU-2.9/messagepattern.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/normalizer.cpp` & `PyICU-2.9/normalizer.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/normalizer.h` & `PyICU-2.9/normalizer.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/numberformat.cpp` & `PyICU-2.9/numberformat.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,19 @@
 
 #if U_ICU_VERSION_HEX >= VERSION_HEX(63, 0, 0)
     DECLARE_CONSTANTS_TYPE(UNumberRangeIdentityFallback)
     DECLARE_CONSTANTS_TYPE(UNumberRangeIdentityResult)
     DECLARE_CONSTANTS_TYPE(UNumberRangeCollapse)
 #endif
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+    DECLARE_CONSTANTS_TYPE(UNumberRoundingPriority)
+    DECLARE_CONSTANTS_TYPE(UNumberTrailingZeroDisplay)
+#endif
+
 /* DecimalFormatSymbols */
 
 class t_decimalformatsymbols : public _wrapper {
 public:
     DecimalFormatSymbols *object;
 };
 
@@ -1041,27 +1046,34 @@
 static PyObject *t_precision_fixedSignificantDigits(PyTypeObject *type, PyObject *arg);
 static PyObject *t_precision_minSignificantDigits(PyTypeObject *type, PyObject *arg);
 static PyObject *t_precision_maxSignificantDigits(PyTypeObject *type, PyObject *arg);
 static PyObject *t_precision_minMaxSignificantDigits(PyTypeObject *type, PyObject *args);
 static PyObject *t_precision_increment(PyTypeObject *type, PyObject *arg);
 static PyObject *t_precision_currency(PyTypeObject *type, PyObject *arg);
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+static PyObject *t_precision_trailingZeroDisplay(t_precision *self, PyObject *arg);
+#endif
+
 static PyMethodDef t_precision_methods[] = {
     DECLARE_METHOD(t_precision, unlimited, METH_NOARGS | METH_CLASS),
     DECLARE_METHOD(t_precision, integer, METH_NOARGS | METH_CLASS),
     DECLARE_METHOD(t_precision, fixedFraction, METH_O | METH_CLASS),
     DECLARE_METHOD(t_precision, minFraction, METH_O | METH_CLASS),
     DECLARE_METHOD(t_precision, maxFraction, METH_O | METH_CLASS),
     DECLARE_METHOD(t_precision, minMaxFraction, METH_VARARGS | METH_CLASS),
     DECLARE_METHOD(t_precision, fixedSignificantDigits, METH_O | METH_CLASS),
     DECLARE_METHOD(t_precision, minSignificantDigits, METH_O | METH_CLASS),
     DECLARE_METHOD(t_precision, maxSignificantDigits, METH_O | METH_CLASS),
     DECLARE_METHOD(t_precision, minMaxSignificantDigits, METH_VARARGS | METH_CLASS),
     DECLARE_METHOD(t_precision, increment, METH_O | METH_CLASS),
     DECLARE_METHOD(t_precision, currency, METH_O | METH_CLASS),
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+    DECLARE_METHOD(t_precision, trailingZeroDisplay, METH_O),
+#endif
     { NULL, NULL, 0, NULL }
 };
 
 DECLARE_BY_VALUE_TYPE(Precision, t_precision, UMemory, Precision, abstract_init)
 
 /* FractionPrecision */
 
@@ -1071,17 +1083,25 @@
 };
 
 static PyObject *t_fractionprecision_minSignificantDigits(
     t_fractionprecision *self, PyObject *arg);
 static PyObject *t_fractionprecision_maxSignificantDigits(
     t_fractionprecision *self, PyObject *arg);
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+static PyObject *t_fractionprecision_withSignificantDigits(
+    t_fractionprecision *self, PyObject *args);
+#endif
+
 static PyMethodDef t_fractionprecision_methods[] = {
     DECLARE_METHOD(t_fractionprecision, minSignificantDigits, METH_O),
     DECLARE_METHOD(t_fractionprecision, maxSignificantDigits, METH_O),
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+    DECLARE_METHOD(t_fractionprecision, withSignificantDigits, METH_VARARGS),
+#endif
     { NULL, NULL, 0, NULL }
 };
 
 DECLARE_BY_VALUE_TYPE(FractionPrecision, t_fractionprecision, Precision,
                       FractionPrecision, abstract_init)
 
 
@@ -4640,14 +4660,31 @@
     {
         return wrap_CurrencyPrecision(Precision::currency((UCurrencyUsage) n));
     }
 
     return PyErr_SetArgsError(type, "currency", arg);
 }
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+
+static PyObject *t_precision_trailingZeroDisplay(t_precision *self, PyObject *arg)
+{
+    UNumberTrailingZeroDisplay tzd;
+
+    if (!parseArg(arg, "i", &tzd))
+    {
+        return wrap_Precision(self->object->trailingZeroDisplay(tzd));
+    }
+
+    return PyErr_SetArgsError((PyObject *) self, "trailingZeroDisplay", arg);
+}
+
+#endif
+
+
 /* FractionPrecision */
 
 static PyObject *t_fractionprecision_minSignificantDigits(
     t_fractionprecision *self, PyObject *arg)
 {
     int n;
 
@@ -4668,14 +4705,46 @@
     {
         return wrap_Precision(self->object->maxSignificantDigits(n));
     }
 
     return PyErr_SetArgsError((PyObject *) self, "maxSignificantDigits", arg);
 }
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+
+static PyObject *t_fractionprecision_withSignificantDigits(
+    t_fractionprecision *self, PyObject *args)
+{
+    int minDigits, maxDigits;
+    UNumberRoundingPriority priority = UNUM_ROUNDING_PRIORITY_RELAXED;
+
+    switch (PyTuple_Size(args)) {
+      case 2:
+        if (!parseArgs(args, "ii", &minDigits, &maxDigits))
+        {
+            return wrap_Precision(
+                self->object->withSignificantDigits(
+                    minDigits, maxDigits, priority));
+        }
+        break;
+      case 3:
+        if (!parseArgs(args, "iii", &minDigits, &maxDigits, &priority))
+        {
+            return wrap_Precision(
+                self->object->withSignificantDigits(
+                    minDigits, maxDigits, priority));
+        }
+        break;
+    }
+
+    return PyErr_SetArgsError((PyObject *) self, "withSignificantDigits", args);
+}
+
+#endif
+
 
 /* IncrementPrecision */
 
 static PyObject *t_incrementprecision_withMinFraction(
     t_incrementprecision *self, PyObject *arg)
 {
     int n;
@@ -5438,14 +5507,24 @@
 #endif
 #if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
     INSTALL_ENUM(UNumberFormatRoundingMode, "HALF_CEILING", UNUM_ROUND_HALF_CEILING);
     INSTALL_ENUM(UNumberFormatRoundingMode, "HALF_FLOOR", UNUM_ROUND_HALF_FLOOR);
     INSTALL_ENUM(UNumberFormatRoundingMode, "HALF_ODD", UNUM_ROUND_HALF_ODD);
 #endif
 
+#if U_ICU_VERSION_HEX >= VERSION_HEX(69, 0, 0)
+    INSTALL_CONSTANTS_TYPE(UNumberRoundingPriority, m);
+    INSTALL_ENUM(UNumberRoundingPriority, "RELAXED", UNUM_ROUNDING_PRIORITY_RELAXED);
+    INSTALL_ENUM(UNumberRoundingPriority, "STRICT", UNUM_ROUNDING_PRIORITY_STRICT);
+
+    INSTALL_CONSTANTS_TYPE(UNumberTrailingZeroDisplay, m);
+    INSTALL_ENUM(UNumberRoundingPriority, "AUTO", UNUM_TRAILING_ZERO_AUTO);
+    INSTALL_ENUM(UNumberRoundingPriority, "HIDE_IF_WHOLE", UNUM_TRAILING_ZERO_HIDE_IF_WHOLE);
+#endif
+
     INSTALL_CONSTANTS_TYPE(UNumberFormatStyle, m);
     INSTALL_ENUM(UNumberFormatStyle, "PATTERN_DECIMAL", UNUM_PATTERN_DECIMAL);
     INSTALL_ENUM(UNumberFormatStyle, "DECIMAL", UNUM_DECIMAL);
     INSTALL_ENUM(UNumberFormatStyle, "CURRENCY", UNUM_CURRENCY);
     INSTALL_ENUM(UNumberFormatStyle, "PERCENT", UNUM_PERCENT);
     INSTALL_ENUM(UNumberFormatStyle, "SCIENTIFIC", UNUM_SCIENTIFIC);
     INSTALL_ENUM(UNumberFormatStyle, "SPELLOUT", UNUM_SPELLOUT);
```

### Comparing `PyICU-2.8.1/numberformat.h` & `PyICU-2.9/numberformat.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/py/PyICU.egg-info/PKG-INFO` & `PyICU-2.9/py/PyICU.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyICU
-Version: 2.8.1
+Version: 2.9
 Summary: Python extension wrapping the ICU C++ API
 Home-page: https://gitlab.pyicu.org/main/pyicu
 Author: Andi Vajda
 Author-email: vajda@pyicu.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyICU-2.8.1/py/PyICU.egg-info/SOURCES.txt` & `PyICU-2.9/py/PyICU.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/py/icu/__init__.py` & `PyICU-2.9/py/icu/__init__.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/regex.cpp` & `PyICU-2.9/regex.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/regex.h` & `PyICU-2.9/regex.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/samples/break.py` & `PyICU-2.9/samples/break.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/samples/strsrch.py` & `PyICU-2.9/samples/strsrch.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/script.cpp` & `PyICU-2.9/script.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/script.h` & `PyICU-2.9/script.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/search.cpp` & `PyICU-2.9/search.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/search.h` & `PyICU-2.9/search.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/setup.py` & `PyICU-2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 try:
     from setuptools import setup, Extension
 except ImportError:
     from distutils.core import setup, Extension
 
 from distutils.spawn import find_executable
 
-VERSION = '2.8.1'
-ICU_MAX_MAJOR_VERSION = '70'  # max supported major version of ICU
+VERSION = '2.9'
+ICU_MAX_MAJOR_VERSION = '71'  # max supported major version of ICU
 
 try:
     from subprocess import check_output as subprocess_check_output
 
     def check_output(popenargs):
         print("(running '%s')" %(' '.join(popenargs)))
         return subprocess_check_output(popenargs)
```

### Comparing `PyICU-2.8.1/shape.cpp` & `PyICU-2.9/shape.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/shape.h` & `PyICU-2.9/shape.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/spoof.cpp` & `PyICU-2.9/spoof.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/spoof.h` & `PyICU-2.9/spoof.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/__init__.py` & `PyICU-2.9/test/__init__.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/collation-rules.txt` & `PyICU-2.9/test/collation-rules.txt`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/lohit_hi.ttf` & `PyICU-2.9/test/lohit_hi.ttf`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Bidi.py` & `PyICU-2.9/test/test_Bidi.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_BreakIterator.py` & `PyICU-2.9/test/test_BreakIterator.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_BytesTrie.py` & `PyICU-2.9/test/test_BytesTrie.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Charset.py` & `PyICU-2.9/test/test_Charset.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Collator.py` & `PyICU-2.9/test/test_Collator.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_DateTimePatternGenerator.py` & `PyICU-2.9/test/test_DateTimePatternGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,25 @@
     def testAddPattern(self):
         """Test overwriting a pattern with the same skeleton."""
         locale = Locale.getFrance()
         dtpg = DateTimePatternGenerator.createInstance(locale)
 
         sdf = SimpleDateFormat(dtpg.getBestPattern('MMMMddHmm'), locale)
         sdf.setTimeZone(self.tz)
-        if ICU_VERSION < '68.0':
+        if ICU_VERSION < '68.0' or ICU_VERSION > '71.0':
             self.assertEqual(sdf.format(self.date), u'09 mai à 17:30')
             self.assertEqual(sdf.toPattern(), u"dd MMMM 'à' HH:mm")
         else:
             self.assertEqual(sdf.format(self.date), u'09 mai, 17:30')
             self.assertEqual(sdf.toPattern(), u"dd MMMM, HH:mm")
 
         dtpg.addPattern("dd'. von' MMMM", True)
         sdf.applyPattern(dtpg.getBestPattern('MMMMddHmm'))
         sdf.setTimeZone(self.tz)
-        if ICU_VERSION < '68.0':
+        if ICU_VERSION < '68.0' or ICU_VERSION > '71.0':
             self.assertEqual(sdf.format(self.date), u'09. von mai à 17:30')
             self.assertEqual(sdf.toPattern(), u"dd'. von' MMMM 'à' HH:mm")
         else:
             self.assertEqual(sdf.format(self.date), u'09. von mai, 17:30')
             self.assertEqual(sdf.toPattern(), u"dd'. von' MMMM, HH:mm")
 
     def testGetBestPattern(self):
```

### Comparing `PyICU-2.8.1/test/test_LayoutEngine.py` & `PyICU-2.9/test/test_LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_ListFormatter.py` & `PyICU-2.9/test/test_ListFormatter.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Locale.py` & `PyICU-2.9/test/test_Locale.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_LocaleData.py` & `PyICU-2.9/test/test_LocaleData.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_LocaleMatcher.py` & `PyICU-2.9/test/test_LocaleMatcher.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_MessageFormat.py` & `PyICU-2.9/test/test_MessageFormat.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_MessagePattern.py` & `PyICU-2.9/test/test_MessagePattern.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Normalizer.py` & `PyICU-2.9/test/test_Normalizer.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_NumberFormat.py` & `PyICU-2.9/test/test_NumberFormat.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_NumberFormatter.py` & `PyICU-2.9/test/test_NumberFormatter.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_PythonReplaceable.py` & `PyICU-2.9/test/test_PythonReplaceable.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Script.py` & `PyICU-2.9/test/test_Script.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_SimpleFormatter.py` & `PyICU-2.9/test/test_SimpleFormatter.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Spoof.py` & `PyICU-2.9/test/test_Spoof.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_TimeZone.py` & `PyICU-2.9/test/test_TimeZone.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_Transliterator.py` & `PyICU-2.9/test/test_Transliterator.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_UCS4.py` & `PyICU-2.9/test/test_UCS4.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_UCharsTrie.py` & `PyICU-2.9/test/test_UCharsTrie.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/test/test_UDate.py` & `PyICU-2.9/test/test_UDate.py`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/timezone.cpp` & `PyICU-2.9/timezone.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/timezone.h` & `PyICU-2.9/timezone.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/transliterator.cpp` & `PyICU-2.9/transliterator.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/transliterator.h` & `PyICU-2.9/transliterator.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/tries.cpp` & `PyICU-2.9/tries.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/tries.h` & `PyICU-2.9/tries.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/tzinfo.cpp` & `PyICU-2.9/tzinfo.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/tzinfo.h` & `PyICU-2.9/tzinfo.h`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/unicodeset.cpp` & `PyICU-2.9/unicodeset.cpp`

 * *Files identical despite different names*

### Comparing `PyICU-2.8.1/unicodeset.h` & `PyICU-2.9/unicodeset.h`

 * *Files identical despite different names*

