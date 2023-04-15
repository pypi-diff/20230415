# Comparing `tmp/pip-9.0.2.tar.gz` & `tmp/pip-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pip-9.0.2.tar", last modified: Sat Mar 17 03:10:42 2018, max compression
+gzip compressed data, was "dist/pip-9.0.3.tar", last modified: Thu Mar 22 01:09:09 2018, max compression
```

## Comparing `pip-9.0.2.tar` & `pip-9.0.3.tar`

### file list

```diff
@@ -1,358 +1,358 @@
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/
--rw-r--r--   0 dstufft    (501) staff       (20)     2602 2018-03-17 03:10:42.000000 pip-9.0.2/PKG-INFO
--rw-r--r--   0 dstufft    (501) staff       (20)      488 2018-03-17 03:10:35.000000 pip-9.0.2/MANIFEST.in
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/docs/
--rw-r--r--   0 dstufft    (501) staff       (20)     3755 2018-03-17 03:10:35.000000 pip-9.0.2/docs/installing.rst
--rw-r--r--   0 dstufft    (501) staff       (20)      483 2018-03-17 03:10:35.000000 pip-9.0.2/docs/index.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     3425 2018-03-17 03:10:35.000000 pip-9.0.2/docs/pipext.py
--rw-r--r--   0 dstufft    (501) staff       (20)       71 2018-03-17 03:10:35.000000 pip-9.0.2/docs/news.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     6790 2018-03-17 03:10:35.000000 pip-9.0.2/docs/Makefile
--rw-r--r--   0 dstufft    (501) staff       (20)      105 2018-03-17 03:10:35.000000 pip-9.0.2/docs/configuration.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     7244 2018-03-17 03:10:35.000000 pip-9.0.2/docs/conf.py
--rw-r--r--   0 dstufft    (501) staff       (20)       14 2018-03-17 03:10:35.000000 pip-9.0.2/docs/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      122 2018-03-17 03:10:35.000000 pip-9.0.2/docs/usage.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     4487 2018-03-17 03:10:35.000000 pip-9.0.2/docs/development.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     6696 2018-03-17 03:10:35.000000 pip-9.0.2/docs/make.bat
--rw-r--r--   0 dstufft    (501) staff       (20)     1270 2018-03-17 03:10:35.000000 pip-9.0.2/docs/quickstart.rst
--rw-r--r--   0 dstufft    (501) staff       (20)      139 2018-03-17 03:10:35.000000 pip-9.0.2/docs/logic.rst
--rw-r--r--   0 dstufft    (501) staff       (20)      112 2018-03-17 03:10:35.000000 pip-9.0.2/docs/cookbook.rst
--rw-r--r--   0 dstufft    (501) staff       (20)    21716 2018-03-17 03:10:35.000000 pip-9.0.2/docs/user_guide.rst
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/docs/reference/
--rw-r--r--   0 dstufft    (501) staff       (20)     1205 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_hash.rst
--rw-r--r--   0 dstufft    (501) staff       (20)      211 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/index.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     1524 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_wheel.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     3587 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_download.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     2127 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_show.rst
--rw-r--r--   0 dstufft    (501) staff       (20)      543 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_uninstall.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     1681 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_list.rst
--rw-r--r--   0 dstufft    (501) staff       (20)    31194 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_install.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     4161 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip.rst
--rw-r--r--   0 dstufft    (501) staff       (20)      443 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_search.rst
--rw-r--r--   0 dstufft    (501) staff       (20)      602 2018-03-17 03:10:35.000000 pip-9.0.2/docs/reference/pip_freeze.rst
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/
--rw-r--r--   0 dstufft    (501) staff       (20)     2602 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/PKG-INFO
--rw-r--r--   0 dstufft    (501) staff       (20)        1 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/not-zip-safe
--rw-r--r--   0 dstufft    (501) staff       (20)     9906 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/SOURCES.txt
--rw-r--r--   0 dstufft    (501) staff       (20)       68 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/entry_points.txt
--rw-r--r--   0 dstufft    (501) staff       (20)       64 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/requires.txt
--rw-r--r--   0 dstufft    (501) staff       (20)        4 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/top_level.txt
--rw-r--r--   0 dstufft    (501) staff       (20)        1 2018-03-17 03:10:42.000000 pip-9.0.2/pip.egg-info/dependency_links.txt
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/
--rw-r--r--   0 dstufft    (501) staff       (20)    10465 2018-03-17 03:10:35.000000 pip-9.0.2/pip/baseparser.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/compat/
--rw-r--r--   0 dstufft    (501) staff       (20)     4672 2018-03-17 03:10:35.000000 pip-9.0.2/pip/compat/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    23096 2018-03-17 03:10:35.000000 pip-9.0.2/pip/compat/dictconfig.py
--rw-r--r--   0 dstufft    (501) staff       (20)    39950 2018-03-17 03:10:35.000000 pip-9.0.2/pip/index.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/
--rw-r--r--   0 dstufft    (501) staff       (20)     9972 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/retrying.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/packaging/
--rw-r--r--   0 dstufft    (501) staff       (20)    11556 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/version.py
--rw-r--r--   0 dstufft    (501) staff       (20)      513 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      421 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/utils.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4327 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/requirements.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1416 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/_structures.py
--rw-r--r--   0 dstufft    (501) staff       (20)     8230 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/markers.py
--rw-r--r--   0 dstufft    (501) staff       (20)      720 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/__about__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      860 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/_compat.py
--rw-r--r--   0 dstufft    (501) staff       (20)    28025 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0 dstufft    (501) staff       (20)      313 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/vendor.txt
--rw-r--r--   0 dstufft    (501) staff       (20)    80176 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/ipaddress.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/chardet/
--rw-r--r--   0 dstufft    (501) staff       (20)     1661 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/enums.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12592 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0 dstufft    (501) staff       (20)    25481 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11290 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0 dstufft    (501) staff       (20)      242 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/version.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1134 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/compat.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12839 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1748 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3774 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1855 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1559 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    31621 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11345 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/langhebrewmodel.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/chardet/cli/
--rw-r--r--   0 dstufft    (501) staff       (20)        1 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2738 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0 dstufft    (501) staff       (20)     9411 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5370 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5110 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1754 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3413 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    17948 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/langcyrillicmodel.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1747 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3590 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3950 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/escprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12485 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2766 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    20715 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2012 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12688 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3749 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    25777 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0 dstufft    (501) staff       (20)    10510 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/escsm.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11102 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5657 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    31254 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0 dstufft    (501) staff       (20)    13546 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1757 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    13838 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3787 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3546 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0 dstufft    (501) staff       (20)    19643 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/chardet/jpcntx.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/webencodings/
--rw-r--r--   0 dstufft    (501) staff       (20)     8979 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/webencodings/labels.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1305 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4306 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0 dstufft    (501) staff       (20)    10576 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6562 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/webencodings/tests.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4094 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/ordereddict.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/progress/
--rw-r--r--   0 dstufft    (501) staff       (20)     3023 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/progress/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2685 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/progress/bar.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1314 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/progress/spinner.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2854 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/progress/helpers.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1502 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/progress/counter.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/distlib/
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/distlib/_backport/
--rw-r--r--   0 dstufft    (501) staff       (20)    25647 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/_backport/shutil.py
--rw-r--r--   0 dstufft    (501) staff       (20)      971 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/_backport/misc.py
--rw-r--r--   0 dstufft    (501) staff       (20)      274 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/_backport/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2617 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/_backport/sysconfig.cfg
--rw-r--r--   0 dstufft    (501) staff       (20)    92628 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/_backport/tarfile.py
--rw-r--r--   0 dstufft    (501) staff       (20)    26955 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/_backport/sysconfig.py
--rw-r--r--   0 dstufft    (501) staff       (20)    85504 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/w32.exe
--rw-r--r--   0 dstufft    (501) staff       (20)    51013 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/locators.py
--rw-r--r--   0 dstufft    (501) staff       (20)    38833 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/metadata.py
--rw-r--r--   0 dstufft    (501) staff       (20)    23711 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/version.py
--rw-r--r--   0 dstufft    (501) staff       (20)    40801 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/compat.py
--rw-r--r--   0 dstufft    (501) staff       (20)    21085 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/index.py
--rw-r--r--   0 dstufft    (501) staff       (20)    14810 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/manifest.py
--rw-r--r--   0 dstufft    (501) staff       (20)    52991 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/util.py
--rw-r--r--   0 dstufft    (501) staff       (20)    49672 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/database.py
--rw-r--r--   0 dstufft    (501) staff       (20)    89088 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/t32.exe
--rw-r--r--   0 dstufft    (501) staff       (20)      581 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    94208 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/w64.exe
--rw-r--r--   0 dstufft    (501) staff       (20)     6282 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/markers.py
--rw-r--r--   0 dstufft    (501) staff       (20)    10766 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/resources.py
--rw-r--r--   0 dstufft    (501) staff       (20)    15224 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/scripts.py
--rw-r--r--   0 dstufft    (501) staff       (20)    97792 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/t64.exe
--rw-r--r--   0 dstufft    (501) staff       (20)    39115 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distlib/wheel.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/colorama/
--rw-r--r--   0 dstufft    (501) staff       (20)      240 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/colorama/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5365 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/colorama/win32.py
--rw-r--r--   0 dstufft    (501) staff       (20)     9668 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2524 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/colorama/ansi.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6290 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/colorama/winterm.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1917 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/colorama/initialise.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/lockfile/
--rw-r--r--   0 dstufft    (501) staff       (20)     5506 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/lockfile/sqlitelockfile.py
--rw-r--r--   0 dstufft    (501) staff       (20)     9371 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/lockfile/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2652 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/lockfile/linklockfile.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3096 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/lockfile/mkdirlockfile.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2616 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/lockfile/symlinklockfile.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6090 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/lockfile/pidlockfile.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/cachecontrol/
--rw-r--r--   0 dstufft    (501) staff       (20)     6536 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0 dstufft    (501) staff       (20)      498 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0 dstufft    (501) staff       (20)    13024 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0 dstufft    (501) staff       (20)      380 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2531 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4141 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4608 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0 dstufft    (501) staff       (20)      790 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0 dstufft    (501) staff       (20)      302 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1320 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/_cmd.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/cachecontrol/caches/
--rw-r--r--   0 dstufft    (501) staff       (20)     3532 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0 dstufft    (501) staff       (20)      369 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      973 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/cachecontrol/caches/redis_cache.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/idna/
--rw-r--r--   0 dstufft    (501) staff       (20)     1749 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/intranges.py
--rw-r--r--   0 dstufft    (501) staff       (20)       21 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/package_data.py
--rw-r--r--   0 dstufft    (501) staff       (20)      232 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/compat.py
--rw-r--r--   0 dstufft    (501) staff       (20)    32999 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/idnadata.py
--rw-r--r--   0 dstufft    (501) staff       (20)       58 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11390 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/core.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3299 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/codec.py
--rw-r--r--   0 dstufft    (501) staff       (20)   184944 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/idna/uts46data.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4670 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/__init__.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/requests/
--rw-r--r--   0 dstufft    (501) staff       (20)    18208 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/cookies.py
--rw-r--r--   0 dstufft    (501) staff       (20)     9728 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/auth.py
--rw-r--r--   0 dstufft    (501) staff       (20)    27546 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/sessions.py
--rw-r--r--   0 dstufft    (501) staff       (20)      767 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/hooks.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1626 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/compat.py
--rw-r--r--   0 dstufft    (501) staff       (20)    34051 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/models.py
--rw-r--r--   0 dstufft    (501) staff       (20)      465 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/certs.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3575 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3323 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/status_codes.py
--rw-r--r--   0 dstufft    (501) staff       (20)      588 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/packages.py
--rw-r--r--   0 dstufft    (501) staff       (20)      436 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/__version__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6237 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/api.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1096 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0 dstufft    (501) staff       (20)    27652 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/utils.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3115 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/exceptions.py
--rw-r--r--   0 dstufft    (501) staff       (20)   271088 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/cacert.pem
--rw-r--r--   0 dstufft    (501) staff       (20)     3012 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/structures.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3667 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/help.py
--rw-r--r--   0 dstufft    (501) staff       (20)    21016 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/requests/adapters.py
--rw-r--r--   0 dstufft    (501) staff       (20)    22368 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/appdirs.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/html5lib/
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/html5lib/filters/
--rw-r--r--   0 dstufft    (501) staff       (20)    25112 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2742 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      286 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/base.py
--rw-r--r--   0 dstufft    (501) staff       (20)      621 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0 dstufft    (501) staff       (20)    10534 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3365 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/lint.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1139 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/filters/whitespace.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/html5lib/treewalkers/
--rw-r--r--   0 dstufft    (501) staff       (20)     6309 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5544 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4684 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2309 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treewalkers/genshi.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4939 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1413 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treewalkers/dom.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/html5lib/treebuilders/
--rw-r--r--   0 dstufft    (501) staff       (20)    14161 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3406 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12764 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0 dstufft    (501) staff       (20)    13942 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0 dstufft    (501) staff       (20)     8835 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0 dstufft    (501) staff       (20)    32532 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_inputstream.py
--rw-r--r--   0 dstufft    (501) staff       (20)    16705 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0 dstufft    (501) staff       (20)    83387 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/constants.py
--rw-r--r--   0 dstufft    (501) staff       (20)   117170 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/html5parser.py
--rw-r--r--   0 dstufft    (501) staff       (20)      780 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/__init__.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/html5lib/_trie/
--rw-r--r--   0 dstufft    (501) staff       (20)      979 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1178 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_trie/datrie.py
--rw-r--r--   0 dstufft    (501) staff       (20)      289 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1775 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_trie/py.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/html5lib/treeadapters/
--rw-r--r--   0 dstufft    (501) staff       (20)     1661 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treeadapters/sax.py
--rw-r--r--   0 dstufft    (501) staff       (20)      208 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1555 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0 dstufft    (501) staff       (20)    14177 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/serializer.py
--rw-r--r--   0 dstufft    (501) staff       (20)    76580 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_tokenizer.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4096 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/html5lib/_utils.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/certifi/
--rw-r--r--   0 dstufft    (501) staff       (20)       63 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/certifi/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      836 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/certifi/core.py
--rw-r--r--   0 dstufft    (501) staff       (20)   271088 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0 dstufft    (501) staff       (20)       41 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/certifi/__main__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    30098 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/six.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/urllib3/
--rw-r--r--   0 dstufft    (501) staff       (20)     2321 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5943 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/fields.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/urllib3/util/
--rw-r--r--   0 dstufft    (501) staff       (20)     1451 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3705 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0 dstufft    (501) staff       (20)     9757 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1044 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    21147 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/selectors.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2343 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12208 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0 dstufft    (501) staff       (20)    14601 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6487 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4237 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5946 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/request.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2853 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    16345 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0 dstufft    (501) staff       (20)    22903 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/response.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/
--rw-r--r--   0 dstufft    (501) staff       (20)    30501 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6195 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0 dstufft    (501) staff       (20)    15354 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 dstufft    (501) staff       (20)    10865 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/appengine.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/_securetransport/
--rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12062 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 dstufft    (501) staff       (20)    17560 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4478 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 dstufft    (501) staff       (20)    13003 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/connection.py
--rw-r--r--   0 dstufft    (501) staff       (20)    10204 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/_collections.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/urllib3/packages/
--rw-r--r--   0 dstufft    (501) staff       (20)      109 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/packages/__init__.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/urllib3/packages/backports/
--rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1461 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0 dstufft    (501) staff       (20)     8935 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/packages/ordered_dict.py
--rw-r--r--   0 dstufft    (501) staff       (20)    30098 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/packages/six.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 dstufft    (501) staff       (20)      688 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5702 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6603 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0 dstufft    (501) staff       (20)    35358 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0 dstufft    (501) staff       (20)    38349 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/distro.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/_vendor/pkg_resources/
--rw-r--r--   0 dstufft    (501) staff       (20)   103230 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      773 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/re-vendor.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6689 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/README.rst
--rw-r--r--   0 dstufft    (501) staff       (20)   224171 2018-03-17 03:10:35.000000 pip-9.0.2/pip/_vendor/pyparsing.py
--rw-r--r--   0 dstufft    (501) staff       (20)    16474 2018-03-17 03:10:35.000000 pip-9.0.2/pip/cmdoptions.py
--rw-r--r--   0 dstufft    (501) staff       (20)    32153 2018-03-17 03:10:35.000000 pip-9.0.2/pip/download.py
--rwxr-xr-x   0 dstufft    (501) staff       (20)    11941 2018-03-17 03:10:35.000000 pip-9.0.2/pip/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)      156 2018-03-17 03:10:35.000000 pip-9.0.2/pip/status_codes.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/utils/
--rw-r--r--   0 dstufft    (501) staff       (20)     1312 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/build.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3327 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/logging.py
--rw-r--r--   0 dstufft    (501) staff       (20)      971 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/encoding.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2232 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/deprecation.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11597 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/ui.py
--rw-r--r--   0 dstufft    (501) staff       (20)      899 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/filesystem.py
--rw-r--r--   0 dstufft    (501) staff       (20)    27187 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     8811 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/appdirs.py
--rw-r--r--   0 dstufft    (501) staff       (20)      278 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/setuptools_build.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2080 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/packaging.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5455 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/outdated.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2866 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/hashes.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2939 2018-03-17 03:10:35.000000 pip-9.0.2/pip/utils/glibc.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/models/
--rw-r--r--   0 dstufft    (501) staff       (20)      487 2018-03-17 03:10:35.000000 pip-9.0.2/pip/models/index.py
--rw-r--r--   0 dstufft    (501) staff       (20)       71 2018-03-17 03:10:35.000000 pip-9.0.2/pip/models/__init__.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/operations/
--rw-r--r--   0 dstufft    (501) staff       (20)     1590 2018-03-17 03:10:35.000000 pip-9.0.2/pip/operations/check.py
--rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:35.000000 pip-9.0.2/pip/operations/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5194 2018-03-17 03:10:35.000000 pip-9.0.2/pip/operations/freeze.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/req/
--rw-r--r--   0 dstufft    (501) staff       (20)    46487 2018-03-17 03:10:35.000000 pip-9.0.2/pip/req/req_install.py
--rw-r--r--   0 dstufft    (501) staff       (20)    34462 2018-03-17 03:10:35.000000 pip-9.0.2/pip/req/req_set.py
--rw-r--r--   0 dstufft    (501) staff       (20)     6897 2018-03-17 03:10:35.000000 pip-9.0.2/pip/req/req_uninstall.py
--rw-r--r--   0 dstufft    (501) staff       (20)      276 2018-03-17 03:10:35.000000 pip-9.0.2/pip/req/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11926 2018-03-17 03:10:35.000000 pip-9.0.2/pip/req/req_file.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/vcs/
--rw-r--r--   0 dstufft    (501) staff       (20)    11197 2018-03-17 03:10:35.000000 pip-9.0.2/pip/vcs/git.py
--rw-r--r--   0 dstufft    (501) staff       (20)    12374 2018-03-17 03:10:35.000000 pip-9.0.2/pip/vcs/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3472 2018-03-17 03:10:35.000000 pip-9.0.2/pip/vcs/mercurial.py
--rw-r--r--   0 dstufft    (501) staff       (20)     3803 2018-03-17 03:10:35.000000 pip-9.0.2/pip/vcs/bazaar.py
--rw-r--r--   0 dstufft    (501) staff       (20)     9350 2018-03-17 03:10:35.000000 pip-9.0.2/pip/vcs/subversion.py
--rw-r--r--   0 dstufft    (501) staff       (20)    10980 2018-03-17 03:10:35.000000 pip-9.0.2/pip/pep425tags.py
--rw-r--r--   0 dstufft    (501) staff       (20)     8121 2018-03-17 03:10:35.000000 pip-9.0.2/pip/exceptions.py
-drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-17 03:10:42.000000 pip-9.0.2/pip/commands/
--rw-r--r--   0 dstufft    (501) staff       (20)     5891 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/show.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11369 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/list.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1382 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/check.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2453 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/completion.py
--rw-r--r--   0 dstufft    (501) staff       (20)     7810 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/download.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2244 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/__init__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     1597 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/hash.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2884 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/uninstall.py
--rw-r--r--   0 dstufft    (501) staff       (20)     2835 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/freeze.py
--rw-r--r--   0 dstufft    (501) staff       (20)     4502 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/search.py
--rw-r--r--   0 dstufft    (501) staff       (20)    17412 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/install.py
--rw-r--r--   0 dstufft    (501) staff       (20)      982 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/help.py
--rw-r--r--   0 dstufft    (501) staff       (20)     7729 2018-03-17 03:10:35.000000 pip-9.0.2/pip/commands/wheel.py
--rw-r--r--   0 dstufft    (501) staff       (20)    11910 2018-03-17 03:10:35.000000 pip-9.0.2/pip/basecommand.py
--rw-r--r--   0 dstufft    (501) staff       (20)      584 2018-03-17 03:10:35.000000 pip-9.0.2/pip/__main__.py
--rw-r--r--   0 dstufft    (501) staff       (20)     5626 2018-03-17 03:10:35.000000 pip-9.0.2/pip/locations.py
--rw-r--r--   0 dstufft    (501) staff       (20)    32010 2018-03-17 03:10:35.000000 pip-9.0.2/pip/wheel.py
--rw-r--r--   0 dstufft    (501) staff       (20)    63203 2018-03-17 03:10:35.000000 pip-9.0.2/CHANGES.txt
--rw-r--r--   0 dstufft    (501) staff       (20)     2934 2018-03-17 03:10:35.000000 pip-9.0.2/setup.py
--rw-r--r--   0 dstufft    (501) staff       (20)      135 2018-03-17 03:10:42.000000 pip-9.0.2/setup.cfg
--rw-r--r--   0 dstufft    (501) staff       (20)     1285 2018-03-17 03:10:35.000000 pip-9.0.2/README.rst
--rw-r--r--   0 dstufft    (501) staff       (20)     1090 2018-03-17 03:10:35.000000 pip-9.0.2/LICENSE.txt
--rw-r--r--   0 dstufft    (501) staff       (20)    12340 2018-03-17 03:10:35.000000 pip-9.0.2/AUTHORS.txt
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/
+-rw-r--r--   0 dstufft    (501) staff       (20)     2602 2018-03-22 01:09:09.000000 pip-9.0.3/PKG-INFO
+-rw-r--r--   0 dstufft    (501) staff       (20)      488 2018-03-22 01:09:06.000000 pip-9.0.3/MANIFEST.in
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/docs/
+-rw-r--r--   0 dstufft    (501) staff       (20)     3755 2018-03-22 01:09:06.000000 pip-9.0.3/docs/installing.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)      483 2018-03-22 01:09:06.000000 pip-9.0.3/docs/index.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     3425 2018-03-22 01:09:06.000000 pip-9.0.3/docs/pipext.py
+-rw-r--r--   0 dstufft    (501) staff       (20)       71 2018-03-22 01:09:06.000000 pip-9.0.3/docs/news.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     6790 2018-03-22 01:09:06.000000 pip-9.0.3/docs/Makefile
+-rw-r--r--   0 dstufft    (501) staff       (20)      105 2018-03-22 01:09:06.000000 pip-9.0.3/docs/configuration.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     7244 2018-03-22 01:09:06.000000 pip-9.0.3/docs/conf.py
+-rw-r--r--   0 dstufft    (501) staff       (20)       14 2018-03-22 01:09:06.000000 pip-9.0.3/docs/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      122 2018-03-22 01:09:06.000000 pip-9.0.3/docs/usage.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     4487 2018-03-22 01:09:06.000000 pip-9.0.3/docs/development.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     6696 2018-03-22 01:09:06.000000 pip-9.0.3/docs/make.bat
+-rw-r--r--   0 dstufft    (501) staff       (20)     1270 2018-03-22 01:09:06.000000 pip-9.0.3/docs/quickstart.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)      139 2018-03-22 01:09:06.000000 pip-9.0.3/docs/logic.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)      112 2018-03-22 01:09:06.000000 pip-9.0.3/docs/cookbook.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)    21716 2018-03-22 01:09:06.000000 pip-9.0.3/docs/user_guide.rst
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/docs/reference/
+-rw-r--r--   0 dstufft    (501) staff       (20)     1205 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_hash.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)      211 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/index.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     1524 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_wheel.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     3587 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_download.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     2127 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_show.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)      543 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_uninstall.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     1681 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_list.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)    31194 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_install.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     4161 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)      443 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_search.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)      602 2018-03-22 01:09:06.000000 pip-9.0.3/docs/reference/pip_freeze.rst
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/
+-rw-r--r--   0 dstufft    (501) staff       (20)     2602 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/PKG-INFO
+-rw-r--r--   0 dstufft    (501) staff       (20)        1 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/not-zip-safe
+-rw-r--r--   0 dstufft    (501) staff       (20)     9906 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/SOURCES.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)       68 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/entry_points.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)       64 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/requires.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)        4 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/top_level.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)        1 2018-03-22 01:09:09.000000 pip-9.0.3/pip.egg-info/dependency_links.txt
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/
+-rw-r--r--   0 dstufft    (501) staff       (20)    10465 2018-03-22 01:09:06.000000 pip-9.0.3/pip/baseparser.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/compat/
+-rw-r--r--   0 dstufft    (501) staff       (20)     4672 2018-03-22 01:09:06.000000 pip-9.0.3/pip/compat/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    23096 2018-03-22 01:09:06.000000 pip-9.0.3/pip/compat/dictconfig.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    39950 2018-03-22 01:09:06.000000 pip-9.0.3/pip/index.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/
+-rw-r--r--   0 dstufft    (501) staff       (20)     9972 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/retrying.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/packaging/
+-rw-r--r--   0 dstufft    (501) staff       (20)    11556 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/version.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      513 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      421 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4327 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1416 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     8230 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      720 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      860 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/_compat.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    28025 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      313 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/vendor.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)    80176 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/ipaddress.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/chardet/
+-rw-r--r--   0 dstufft    (501) staff       (20)     1661 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/enums.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12592 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    25481 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11290 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      242 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/version.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1134 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/compat.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12839 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1748 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3774 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1855 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1559 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    31621 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11345 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/langhebrewmodel.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/chardet/cli/
+-rw-r--r--   0 dstufft    (501) staff       (20)        1 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2738 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     9411 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5370 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5110 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1754 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3413 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    17948 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/langcyrillicmodel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1747 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3590 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3950 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12485 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2766 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    20715 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2012 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12688 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3749 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    25777 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    10510 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11102 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5657 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    31254 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    13546 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1757 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    13838 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3787 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3546 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    19643 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/chardet/jpcntx.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/webencodings/
+-rw-r--r--   0 dstufft    (501) staff       (20)     8979 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1305 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4306 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    10576 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6562 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4094 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/ordereddict.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/progress/
+-rw-r--r--   0 dstufft    (501) staff       (20)     3023 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/progress/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2685 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/progress/bar.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1314 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/progress/spinner.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2854 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/progress/helpers.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1502 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/progress/counter.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/distlib/
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/distlib/_backport/
+-rw-r--r--   0 dstufft    (501) staff       (20)    25647 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/_backport/shutil.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      971 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/_backport/misc.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      274 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/_backport/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2617 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/_backport/sysconfig.cfg
+-rw-r--r--   0 dstufft    (501) staff       (20)    92628 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/_backport/tarfile.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    26955 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    85504 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0 dstufft    (501) staff       (20)    51013 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    38833 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    23711 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/version.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    40801 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    21085 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/index.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    14810 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    52991 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/util.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    49672 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/database.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    89088 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0 dstufft    (501) staff       (20)      581 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    94208 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0 dstufft    (501) staff       (20)     6282 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    10766 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    15224 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    97792 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0 dstufft    (501) staff       (20)    39115 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distlib/wheel.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/colorama/
+-rw-r--r--   0 dstufft    (501) staff       (20)      240 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5365 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     9668 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2524 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6290 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1917 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/colorama/initialise.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/lockfile/
+-rw-r--r--   0 dstufft    (501) staff       (20)     5506 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/lockfile/sqlitelockfile.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     9371 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/lockfile/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2652 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/lockfile/linklockfile.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3096 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/lockfile/mkdirlockfile.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2616 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/lockfile/symlinklockfile.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6090 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/lockfile/pidlockfile.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/cachecontrol/
+-rw-r--r--   0 dstufft    (501) staff       (20)     6536 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      498 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    13024 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      380 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2531 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4141 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4608 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      790 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      302 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1320 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/_cmd.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 dstufft    (501) staff       (20)     3532 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      369 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      973 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/cachecontrol/caches/redis_cache.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/idna/
+-rw-r--r--   0 dstufft    (501) staff       (20)     1749 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/intranges.py
+-rw-r--r--   0 dstufft    (501) staff       (20)       21 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/package_data.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      232 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/compat.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    32999 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0 dstufft    (501) staff       (20)       58 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11390 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/core.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3299 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/codec.py
+-rw-r--r--   0 dstufft    (501) staff       (20)   184944 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4670 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/__init__.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/requests/
+-rw-r--r--   0 dstufft    (501) staff       (20)    18208 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     9728 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/auth.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    27546 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      767 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1626 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/compat.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    34051 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/models.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      465 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/certs.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3575 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3323 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      695 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/packages.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      436 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/__version__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6237 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/api.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1096 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    27652 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/utils.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3115 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 dstufft    (501) staff       (20)   271088 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/cacert.pem
+-rw-r--r--   0 dstufft    (501) staff       (20)     3012 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/structures.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3667 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/help.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    21016 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    22368 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/appdirs.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/html5lib/
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/html5lib/filters/
+-rw-r--r--   0 dstufft    (501) staff       (20)    25112 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2742 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      286 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/base.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      621 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    10534 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3365 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1139 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/filters/whitespace.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/html5lib/treewalkers/
+-rw-r--r--   0 dstufft    (501) staff       (20)     6309 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5544 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4684 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2309 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treewalkers/genshi.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4939 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1413 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treewalkers/dom.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/html5lib/treebuilders/
+-rw-r--r--   0 dstufft    (501) staff       (20)    14161 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3406 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12764 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    13942 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     8835 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    32532 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    16705 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    83387 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/constants.py
+-rw-r--r--   0 dstufft    (501) staff       (20)   117170 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/html5parser.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      780 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/__init__.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/html5lib/_trie/
+-rw-r--r--   0 dstufft    (501) staff       (20)      979 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1178 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_trie/datrie.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      289 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1775 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_trie/py.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/html5lib/treeadapters/
+-rw-r--r--   0 dstufft    (501) staff       (20)     1661 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treeadapters/sax.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      208 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1555 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    14177 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/serializer.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    76580 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_tokenizer.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4096 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/html5lib/_utils.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/certifi/
+-rw-r--r--   0 dstufft    (501) staff       (20)       63 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      836 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/certifi/core.py
+-rw-r--r--   0 dstufft    (501) staff       (20)   271088 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0 dstufft    (501) staff       (20)       41 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    30098 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/six.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/urllib3/
+-rw-r--r--   0 dstufft    (501) staff       (20)     2321 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5943 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/fields.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/urllib3/util/
+-rw-r--r--   0 dstufft    (501) staff       (20)     1451 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3705 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     9757 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1044 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    21147 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/selectors.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2343 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12208 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    14601 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6487 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4237 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5946 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/request.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2853 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    16345 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    22903 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/response.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/
+-rw-r--r--   0 dstufft    (501) staff       (20)    30501 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6195 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    15354 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    10865 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/appengine.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12062 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    17560 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4478 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    13003 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    10204 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/_collections.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/urllib3/packages/
+-rw-r--r--   0 dstufft    (501) staff       (20)      109 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1461 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     8935 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/packages/ordered_dict.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    30098 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/packages/six.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 dstufft    (501) staff       (20)      688 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5702 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6603 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    35358 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    38349 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/distro.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/_vendor/pkg_resources/
+-rw-r--r--   0 dstufft    (501) staff       (20)   103230 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      773 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/re-vendor.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6689 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/README.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)   224171 2018-03-22 01:09:06.000000 pip-9.0.3/pip/_vendor/pyparsing.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    16474 2018-03-22 01:09:06.000000 pip-9.0.3/pip/cmdoptions.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    32153 2018-03-22 01:09:06.000000 pip-9.0.3/pip/download.py
+-rwxr-xr-x   0 dstufft    (501) staff       (20)    11956 2018-03-22 01:09:06.000000 pip-9.0.3/pip/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      156 2018-03-22 01:09:06.000000 pip-9.0.3/pip/status_codes.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/utils/
+-rw-r--r--   0 dstufft    (501) staff       (20)     1312 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/build.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3327 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/logging.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      971 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/encoding.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2232 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/deprecation.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11597 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/ui.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      899 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/filesystem.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    27187 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     8811 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/appdirs.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      278 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/setuptools_build.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2080 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/packaging.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5455 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/outdated.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2866 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/hashes.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2939 2018-03-22 01:09:06.000000 pip-9.0.3/pip/utils/glibc.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/models/
+-rw-r--r--   0 dstufft    (501) staff       (20)      487 2018-03-22 01:09:06.000000 pip-9.0.3/pip/models/index.py
+-rw-r--r--   0 dstufft    (501) staff       (20)       71 2018-03-22 01:09:06.000000 pip-9.0.3/pip/models/__init__.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/operations/
+-rw-r--r--   0 dstufft    (501) staff       (20)     1590 2018-03-22 01:09:06.000000 pip-9.0.3/pip/operations/check.py
+-rw-r--r--   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:06.000000 pip-9.0.3/pip/operations/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5194 2018-03-22 01:09:06.000000 pip-9.0.3/pip/operations/freeze.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/req/
+-rw-r--r--   0 dstufft    (501) staff       (20)    46487 2018-03-22 01:09:06.000000 pip-9.0.3/pip/req/req_install.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    34462 2018-03-22 01:09:06.000000 pip-9.0.3/pip/req/req_set.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     6897 2018-03-22 01:09:06.000000 pip-9.0.3/pip/req/req_uninstall.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      276 2018-03-22 01:09:06.000000 pip-9.0.3/pip/req/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11926 2018-03-22 01:09:06.000000 pip-9.0.3/pip/req/req_file.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/vcs/
+-rw-r--r--   0 dstufft    (501) staff       (20)    11197 2018-03-22 01:09:06.000000 pip-9.0.3/pip/vcs/git.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    12374 2018-03-22 01:09:06.000000 pip-9.0.3/pip/vcs/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3472 2018-03-22 01:09:06.000000 pip-9.0.3/pip/vcs/mercurial.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     3803 2018-03-22 01:09:06.000000 pip-9.0.3/pip/vcs/bazaar.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     9350 2018-03-22 01:09:06.000000 pip-9.0.3/pip/vcs/subversion.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    10980 2018-03-22 01:09:06.000000 pip-9.0.3/pip/pep425tags.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     8121 2018-03-22 01:09:06.000000 pip-9.0.3/pip/exceptions.py
+drwxr-xr-x   0 dstufft    (501) staff       (20)        0 2018-03-22 01:09:09.000000 pip-9.0.3/pip/commands/
+-rw-r--r--   0 dstufft    (501) staff       (20)     5891 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/show.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11369 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/list.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1382 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/check.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2453 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/completion.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     7810 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/download.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2244 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/__init__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     1597 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/hash.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2884 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/uninstall.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     2835 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/freeze.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     4502 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/search.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    17412 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/install.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      982 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/help.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     7729 2018-03-22 01:09:06.000000 pip-9.0.3/pip/commands/wheel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    11910 2018-03-22 01:09:06.000000 pip-9.0.3/pip/basecommand.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      584 2018-03-22 01:09:06.000000 pip-9.0.3/pip/__main__.py
+-rw-r--r--   0 dstufft    (501) staff       (20)     5626 2018-03-22 01:09:06.000000 pip-9.0.3/pip/locations.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    32010 2018-03-22 01:09:06.000000 pip-9.0.3/pip/wheel.py
+-rw-r--r--   0 dstufft    (501) staff       (20)    63383 2018-03-22 01:09:06.000000 pip-9.0.3/CHANGES.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)     2934 2018-03-22 01:09:06.000000 pip-9.0.3/setup.py
+-rw-r--r--   0 dstufft    (501) staff       (20)      135 2018-03-22 01:09:09.000000 pip-9.0.3/setup.cfg
+-rw-r--r--   0 dstufft    (501) staff       (20)     1285 2018-03-22 01:09:06.000000 pip-9.0.3/README.rst
+-rw-r--r--   0 dstufft    (501) staff       (20)     1090 2018-03-22 01:09:06.000000 pip-9.0.3/LICENSE.txt
+-rw-r--r--   0 dstufft    (501) staff       (20)    12340 2018-03-22 01:09:06.000000 pip-9.0.3/AUTHORS.txt
```

### Comparing `pip-9.0.2/PKG-INFO` & `pip-9.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip
-Version: 9.0.2
+Version: 9.0.3
 Summary: The PyPA recommended tool for installing Python packages.
 Home-page: https://pip.pypa.io/
 Author: The pip developers
 Author-email: python-virtualenv@groups.google.com
 License: MIT
 Description: pip
         ===
```

### Comparing `pip-9.0.2/docs/installing.rst` & `pip-9.0.3/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/pipext.py` & `pip-9.0.3/docs/pipext.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/Makefile` & `pip-9.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/conf.py` & `pip-9.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/development.rst` & `pip-9.0.3/docs/development.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/make.bat` & `pip-9.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/quickstart.rst` & `pip-9.0.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/user_guide.rst` & `pip-9.0.3/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_hash.rst` & `pip-9.0.3/docs/reference/pip_hash.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_wheel.rst` & `pip-9.0.3/docs/reference/pip_wheel.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_download.rst` & `pip-9.0.3/docs/reference/pip_download.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_show.rst` & `pip-9.0.3/docs/reference/pip_show.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_uninstall.rst` & `pip-9.0.3/docs/reference/pip_uninstall.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_list.rst` & `pip-9.0.3/docs/reference/pip_list.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_install.rst` & `pip-9.0.3/docs/reference/pip_install.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip.rst` & `pip-9.0.3/docs/reference/pip.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/docs/reference/pip_freeze.rst` & `pip-9.0.3/docs/reference/pip_freeze.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip.egg-info/PKG-INFO` & `pip-9.0.3/pip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip
-Version: 9.0.2
+Version: 9.0.3
 Summary: The PyPA recommended tool for installing Python packages.
 Home-page: https://pip.pypa.io/
 Author: The pip developers
 Author-email: python-virtualenv@groups.google.com
 License: MIT
 Description: pip
         ===
```

### Comparing `pip-9.0.2/pip.egg-info/SOURCES.txt` & `pip-9.0.3/pip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/baseparser.py` & `pip-9.0.3/pip/baseparser.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/compat/__init__.py` & `pip-9.0.3/pip/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/compat/dictconfig.py` & `pip-9.0.3/pip/compat/dictconfig.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/index.py` & `pip-9.0.3/pip/index.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/retrying.py` & `pip-9.0.3/pip/_vendor/retrying.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/version.py` & `pip-9.0.3/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/__init__.py` & `pip-9.0.3/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/requirements.py` & `pip-9.0.3/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/_structures.py` & `pip-9.0.3/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/markers.py` & `pip-9.0.3/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/__about__.py` & `pip-9.0.3/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/_compat.py` & `pip-9.0.3/pip/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/packaging/specifiers.py` & `pip-9.0.3/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/ipaddress.py` & `pip-9.0.3/pip/_vendor/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/enums.py` & `pip-9.0.3/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/langhungarianmodel.py` & `pip-9.0.3/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/mbcssm.py` & `pip-9.0.3/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/langthaimodel.py` & `pip-9.0.3/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/compat.py` & `pip-9.0.3/pip/_vendor/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/langbulgarianmodel.py` & `pip-9.0.3/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/euckrprober.py` & `pip-9.0.3/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/sjisprober.py` & `pip-9.0.3/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/cp949prober.py` & `pip-9.0.3/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/__init__.py` & `pip-9.0.3/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/euctwfreq.py` & `pip-9.0.3/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/langhebrewmodel.py` & `pip-9.0.3/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/cli/chardetect.py` & `pip-9.0.3/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/chardistribution.py` & `pip-9.0.3/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/latin1prober.py` & `pip-9.0.3/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/charsetprober.py` & `pip-9.0.3/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/gb2312prober.py` & `pip-9.0.3/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/mbcharsetprober.py` & `pip-9.0.3/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/langcyrillicmodel.py` & `pip-9.0.3/pip/_vendor/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/euctwprober.py` & `pip-9.0.3/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/codingstatemachine.py` & `pip-9.0.3/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/escprober.py` & `pip-9.0.3/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/universaldetector.py` & `pip-9.0.3/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/utf8prober.py` & `pip-9.0.3/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/gb2312freq.py` & `pip-9.0.3/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/mbcsgroupprober.py` & `pip-9.0.3/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/langgreekmodel.py` & `pip-9.0.3/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/eucjpprober.py` & `pip-9.0.3/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/jisfreq.py` & `pip-9.0.3/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/escsm.py` & `pip-9.0.3/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/langturkishmodel.py` & `pip-9.0.3/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/sbcharsetprober.py` & `pip-9.0.3/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/big5freq.py` & `pip-9.0.3/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/euckrfreq.py` & `pip-9.0.3/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/big5prober.py` & `pip-9.0.3/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/hebrewprober.py` & `pip-9.0.3/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/charsetgroupprober.py` & `pip-9.0.3/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/sbcsgroupprober.py` & `pip-9.0.3/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/chardet/jpcntx.py` & `pip-9.0.3/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/webencodings/labels.py` & `pip-9.0.3/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/webencodings/mklabels.py` & `pip-9.0.3/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/webencodings/x_user_defined.py` & `pip-9.0.3/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/webencodings/__init__.py` & `pip-9.0.3/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/webencodings/tests.py` & `pip-9.0.3/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/ordereddict.py` & `pip-9.0.3/pip/_vendor/ordereddict.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/progress/__init__.py` & `pip-9.0.3/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/progress/bar.py` & `pip-9.0.3/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/progress/spinner.py` & `pip-9.0.3/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/progress/helpers.py` & `pip-9.0.3/pip/_vendor/progress/helpers.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/progress/counter.py` & `pip-9.0.3/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/_backport/shutil.py` & `pip-9.0.3/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/_backport/misc.py` & `pip-9.0.3/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/_backport/sysconfig.cfg` & `pip-9.0.3/pip/_vendor/distlib/_backport/sysconfig.cfg`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/_backport/tarfile.py` & `pip-9.0.3/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/_backport/sysconfig.py` & `pip-9.0.3/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/w32.exe` & `pip-9.0.3/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/locators.py` & `pip-9.0.3/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/metadata.py` & `pip-9.0.3/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/version.py` & `pip-9.0.3/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/compat.py` & `pip-9.0.3/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/index.py` & `pip-9.0.3/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/manifest.py` & `pip-9.0.3/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/util.py` & `pip-9.0.3/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/database.py` & `pip-9.0.3/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/t32.exe` & `pip-9.0.3/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/__init__.py` & `pip-9.0.3/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/w64.exe` & `pip-9.0.3/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/markers.py` & `pip-9.0.3/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/resources.py` & `pip-9.0.3/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/scripts.py` & `pip-9.0.3/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/t64.exe` & `pip-9.0.3/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distlib/wheel.py` & `pip-9.0.3/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/colorama/win32.py` & `pip-9.0.3/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/colorama/ansitowin32.py` & `pip-9.0.3/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/colorama/ansi.py` & `pip-9.0.3/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/colorama/winterm.py` & `pip-9.0.3/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/colorama/initialise.py` & `pip-9.0.3/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/lockfile/sqlitelockfile.py` & `pip-9.0.3/pip/_vendor/lockfile/sqlitelockfile.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/lockfile/__init__.py` & `pip-9.0.3/pip/_vendor/lockfile/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/lockfile/linklockfile.py` & `pip-9.0.3/pip/_vendor/lockfile/linklockfile.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/lockfile/mkdirlockfile.py` & `pip-9.0.3/pip/_vendor/lockfile/mkdirlockfile.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/lockfile/symlinklockfile.py` & `pip-9.0.3/pip/_vendor/lockfile/symlinklockfile.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/lockfile/pidlockfile.py` & `pip-9.0.3/pip/_vendor/lockfile/pidlockfile.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/serialize.py` & `pip-9.0.3/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/controller.py` & `pip-9.0.3/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/filewrapper.py` & `pip-9.0.3/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/heuristics.py` & `pip-9.0.3/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/adapter.py` & `pip-9.0.3/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/cache.py` & `pip-9.0.3/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/_cmd.py` & `pip-9.0.3/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/caches/file_cache.py` & `pip-9.0.3/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pip-9.0.3/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/idna/intranges.py` & `pip-9.0.3/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/idna/idnadata.py` & `pip-9.0.3/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/idna/core.py` & `pip-9.0.3/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/idna/codec.py` & `pip-9.0.3/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/idna/uts46data.py` & `pip-9.0.3/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/__init__.py` & `pip-9.0.3/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/cookies.py` & `pip-9.0.3/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/auth.py` & `pip-9.0.3/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/sessions.py` & `pip-9.0.3/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/hooks.py` & `pip-9.0.3/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/compat.py` & `pip-9.0.3/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/models.py` & `pip-9.0.3/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/__init__.py` & `pip-9.0.3/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/status_codes.py` & `pip-9.0.3/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/api.py` & `pip-9.0.3/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/_internal_utils.py` & `pip-9.0.3/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/utils.py` & `pip-9.0.3/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/exceptions.py` & `pip-9.0.3/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/cacert.pem` & `pip-9.0.3/pip/_vendor/requests/cacert.pem`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/structures.py` & `pip-9.0.3/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/help.py` & `pip-9.0.3/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/requests/adapters.py` & `pip-9.0.3/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/appdirs.py` & `pip-9.0.3/pip/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/filters/sanitizer.py` & `pip-9.0.3/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `pip-9.0.3/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `pip-9.0.3/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/filters/optionaltags.py` & `pip-9.0.3/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/filters/lint.py` & `pip-9.0.3/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/filters/whitespace.py` & `pip-9.0.3/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `pip-9.0.3/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treewalkers/__init__.py` & `pip-9.0.3/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treewalkers/etree.py` & `pip-9.0.3/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treewalkers/genshi.py` & `pip-9.0.3/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treewalkers/base.py` & `pip-9.0.3/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treewalkers/dom.py` & `pip-9.0.3/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `pip-9.0.3/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treebuilders/__init__.py` & `pip-9.0.3/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treebuilders/etree.py` & `pip-9.0.3/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treebuilders/base.py` & `pip-9.0.3/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treebuilders/dom.py` & `pip-9.0.3/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/_inputstream.py` & `pip-9.0.3/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/_ihatexml.py` & `pip-9.0.3/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/constants.py` & `pip-9.0.3/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/html5parser.py` & `pip-9.0.3/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/__init__.py` & `pip-9.0.3/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/_trie/_base.py` & `pip-9.0.3/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/_trie/datrie.py` & `pip-9.0.3/pip/_vendor/html5lib/_trie/datrie.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/_trie/py.py` & `pip-9.0.3/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treeadapters/sax.py` & `pip-9.0.3/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/treeadapters/genshi.py` & `pip-9.0.3/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/serializer.py` & `pip-9.0.3/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/_tokenizer.py` & `pip-9.0.3/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/html5lib/_utils.py` & `pip-9.0.3/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/certifi/core.py` & `pip-9.0.3/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/certifi/cacert.pem` & `pip-9.0.3/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/six.py` & `pip-9.0.3/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/filepost.py` & `pip-9.0.3/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/fields.py` & `pip-9.0.3/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/wait.py` & `pip-9.0.3/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/request.py` & `pip-9.0.3/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/timeout.py` & `pip-9.0.3/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/__init__.py` & `pip-9.0.3/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/selectors.py` & `pip-9.0.3/pip/_vendor/urllib3/util/selectors.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/response.py` & `pip-9.0.3/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/ssl_.py` & `pip-9.0.3/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/retry.py` & `pip-9.0.3/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/url.py` & `pip-9.0.3/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/util/connection.py` & `pip-9.0.3/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/request.py` & `pip-9.0.3/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/__init__.py` & `pip-9.0.3/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/poolmanager.py` & `pip-9.0.3/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/response.py` & `pip-9.0.3/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/contrib/securetransport.py` & `pip-9.0.3/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/contrib/socks.py` & `pip-9.0.3/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pip-9.0.3/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/contrib/appengine.py` & `pip-9.0.3/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pip-9.0.3/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pip-9.0.3/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pip-9.0.3/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/connection.py` & `pip-9.0.3/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/_collections.py` & `pip-9.0.3/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/packages/backports/makefile.py` & `pip-9.0.3/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/packages/ordered_dict.py` & `pip-9.0.3/pip/_vendor/urllib3/packages/ordered_dict.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/packages/six.py` & `pip-9.0.3/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py` & `pip-9.0.3/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py` & `pip-9.0.3/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/exceptions.py` & `pip-9.0.3/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/urllib3/connectionpool.py` & `pip-9.0.3/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/distro.py` & `pip-9.0.3/pip/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/pkg_resources/__init__.py` & `pip-9.0.3/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/re-vendor.py` & `pip-9.0.3/pip/_vendor/re-vendor.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/README.rst` & `pip-9.0.3/pip/_vendor/README.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/_vendor/pyparsing.py` & `pip-9.0.3/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/cmdoptions.py` & `pip-9.0.3/pip/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/download.py` & `pip-9.0.3/pip/download.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/__init__.py` & `pip-9.0.3/pip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # OpenSSL is too old to handle TLSv1.2
 try:
     import ssl
 except ImportError:
     pass
 else:
     if (sys.platform == "darwin" and
-            ssl.OPENSSL_VERSION_NUMBER < 0x1000100f):  # OpenSSL 1.0.1
+            getattr(ssl, "OPENSSL_VERSION_NUMBER", 0) < 0x1000100f):  # OpenSSL 1.0.1
         try:
             from pip._vendor.urllib3.contrib import securetransport
         except (ImportError, OSError):
             pass
         else:
             securetransport.inject_into_urllib3()
 
@@ -54,15 +54,15 @@
 # This fixes a peculiarity when importing via __import__ - as we are
 # initialising the pip module, "from pip import cmdoptions" is recursive
 # and appears not to work properly in that situation.
 import pip.cmdoptions
 cmdoptions = pip.cmdoptions
 
 # The version as used in the setup.py and the docs conf.py
-__version__ = "9.0.2"
+__version__ = "9.0.3"
 
 
 logger = logging.getLogger(__name__)
 
 # Hide the InsecureRequestWarning from urllib3
 warnings.filterwarnings("ignore", category=InsecureRequestWarning)
```

### Comparing `pip-9.0.2/pip/utils/build.py` & `pip-9.0.3/pip/utils/build.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/logging.py` & `pip-9.0.3/pip/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/encoding.py` & `pip-9.0.3/pip/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/deprecation.py` & `pip-9.0.3/pip/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/ui.py` & `pip-9.0.3/pip/utils/ui.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/filesystem.py` & `pip-9.0.3/pip/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/__init__.py` & `pip-9.0.3/pip/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/appdirs.py` & `pip-9.0.3/pip/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/packaging.py` & `pip-9.0.3/pip/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/outdated.py` & `pip-9.0.3/pip/utils/outdated.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/hashes.py` & `pip-9.0.3/pip/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/utils/glibc.py` & `pip-9.0.3/pip/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/operations/check.py` & `pip-9.0.3/pip/operations/check.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/operations/freeze.py` & `pip-9.0.3/pip/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/req/req_install.py` & `pip-9.0.3/pip/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/req/req_set.py` & `pip-9.0.3/pip/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/req/req_uninstall.py` & `pip-9.0.3/pip/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/req/req_file.py` & `pip-9.0.3/pip/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/vcs/git.py` & `pip-9.0.3/pip/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/vcs/__init__.py` & `pip-9.0.3/pip/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/vcs/mercurial.py` & `pip-9.0.3/pip/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/vcs/bazaar.py` & `pip-9.0.3/pip/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/vcs/subversion.py` & `pip-9.0.3/pip/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/pep425tags.py` & `pip-9.0.3/pip/pep425tags.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/exceptions.py` & `pip-9.0.3/pip/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/show.py` & `pip-9.0.3/pip/commands/show.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/list.py` & `pip-9.0.3/pip/commands/list.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/check.py` & `pip-9.0.3/pip/commands/check.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/completion.py` & `pip-9.0.3/pip/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/download.py` & `pip-9.0.3/pip/commands/download.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/__init__.py` & `pip-9.0.3/pip/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/hash.py` & `pip-9.0.3/pip/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/uninstall.py` & `pip-9.0.3/pip/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/freeze.py` & `pip-9.0.3/pip/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/search.py` & `pip-9.0.3/pip/commands/search.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/install.py` & `pip-9.0.3/pip/commands/install.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/help.py` & `pip-9.0.3/pip/commands/help.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/commands/wheel.py` & `pip-9.0.3/pip/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/basecommand.py` & `pip-9.0.3/pip/basecommand.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/__main__.py` & `pip-9.0.3/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/locations.py` & `pip-9.0.3/pip/locations.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/pip/wheel.py` & `pip-9.0.3/pip/wheel.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/CHANGES.txt` & `pip-9.0.3/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-**9.0.2 (2017-03-16)**
+**9.0.3 (2018-03-21)**
+
+* Fix an error where the vendored requests was not correctly containing itself
+  to only the internal vendored prefix.
+
+* Restore compatability with 2.6.
+
+
+**9.0.2 (2018-03-16)**
 
 * Fallback to using SecureTransport on macOS when the linked OpenSSL is too old
   to support TLSv1.2.
 
 
 **9.0.1 (2016-11-06)**
```

### Comparing `pip-9.0.2/setup.py` & `pip-9.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/README.rst` & `pip-9.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/LICENSE.txt` & `pip-9.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pip-9.0.2/AUTHORS.txt` & `pip-9.0.3/AUTHORS.txt`

 * *Files identical despite different names*

