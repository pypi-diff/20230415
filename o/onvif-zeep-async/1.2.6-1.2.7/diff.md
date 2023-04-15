# Comparing `tmp/onvif-zeep-async-1.2.6.tar.gz` & `tmp/onvif-zeep-async-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-1.2.6.tar", last modified: Sat Apr 15 18:47:24 2023, max compression
+gzip compressed data, was "onvif-zeep-async-1.2.7.tar", last modified: Sat Apr 15 18:58:09 2023, max compression
```

## Comparing `onvif-zeep-async-1.2.6.tar` & `onvif-zeep-async-1.2.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:47:24.373389 onvif-zeep-async-1.2.6/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.6/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.6/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 18:47:24.373471 onvif-zeep-async-1.2.6/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:47:24.365007 onvif-zeep-async-1.2.6/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:47:24.365576 onvif-zeep-async-1.2.6/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    19250 2023-04-15 18:46:52.000000 onvif-zeep-async-1.2.6/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 18:47:04.000000 onvif-zeep-async-1.2.6/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:47:24.372342 onvif-zeep-async-1.2.6/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:47:24.373174 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 18:47:24.000000 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1417 2023-04-15 18:47:24.000000 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-15 18:47:24.000000 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-04-15 18:47:24.000000 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-04-15 18:47:24.000000 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 18:47:24.000000 onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-04-15 18:47:24.373763 onvif-zeep-async-1.2.6/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:47:24.373276 onvif-zeep-async-1.2.6/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.6/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:58:09.065404 onvif-zeep-async-1.2.7/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.7/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.7/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 18:58:09.065459 onvif-zeep-async-1.2.7/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:58:09.056523 onvif-zeep-async-1.2.7/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:58:09.057244 onvif-zeep-async-1.2.7/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    19246 2023-04-15 18:57:44.000000 onvif-zeep-async-1.2.7/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 18:57:50.000000 onvif-zeep-async-1.2.7/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:58:09.064393 onvif-zeep-async-1.2.7/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:58:09.065160 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 18:58:09.000000 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1417 2023-04-15 18:58:09.000000 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-15 18:58:09.000000 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-04-15 18:58:09.000000 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-04-15 18:58:09.000000 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 18:58:09.000000 onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-04-15 18:58:09.065710 onvif-zeep-async-1.2.7/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 18:58:09.065261 onvif-zeep-async-1.2.7/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.7/tests/test.py
```

### Comparing `onvif-zeep-async-1.2.6/.gitignore` & `onvif-zeep-async-1.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/.pre-commit-config.yaml` & `onvif-zeep-async-1.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/LICENSE` & `onvif-zeep-async-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/Makefile` & `onvif-zeep-async-1.2.7/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/PKG-INFO` & `onvif-zeep-async-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.2.6
+Version: 1.2.7
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.6/README.rst` & `onvif-zeep-async-1.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/examples/events.py` & `onvif-zeep-async-1.2.7/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/examples/rotate_image.py` & `onvif-zeep-async-1.2.7/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/examples/streaming.py` & `onvif-zeep-async-1.2.7/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/__init__.py` & `onvif-zeep-async-1.2.7/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/client.py` & `onvif-zeep-async-1.2.7/onvif/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
 
     async def create_pullpoint_subscription(
         self, config: Optional[Dict[str, Any]] = None
     ) -> bool:
         """Create a pullpoint subscription."""
         try:
             events = self.create_events_service()
-            pullpoint = await events.CreatePullPointSubscription(**(config or {}))
+            pullpoint = await events.CreatePullPointSubscription(config or {})
             # pylint: disable=protected-access
             self.xaddrs[
                 "http://www.onvif.org/ver10/events/wsdl/PullPointSubscription"
             ] = pullpoint.SubscriptionReference.Address._value_1
         except Fault:
             return False
         return True
```

### Comparing `onvif-zeep-async-1.2.6/onvif/definition.py` & `onvif-zeep-async-1.2.7/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/exceptions.py` & `onvif-zeep-async-1.2.7/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/addressing` & `onvif-zeep-async-1.2.7/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/display.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/envelope` & `onvif-zeep-async-1.2.7/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/events.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/media.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/search.wsdl` & `onvif-zeep-async-1.2.7/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/types.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/xml.xsd` & `onvif-zeep-async-1.2.7/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif/wsdl/xmlmime` & `onvif-zeep-async-1.2.7/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.2.6
+Version: 1.2.7
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.6/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-1.2.7/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/pylintrc` & `onvif-zeep-async-1.2.7/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/setup.py` & `onvif-zeep-async-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.6/tests/test.py` & `onvif-zeep-async-1.2.7/tests/test.py`

 * *Files identical despite different names*

