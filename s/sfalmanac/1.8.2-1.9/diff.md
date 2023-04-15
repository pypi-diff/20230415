# Comparing `tmp/sfalmanac-1.8.2.tar.gz` & `tmp/sfalmanac-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfalmanac-1.8.2.tar", last modified: Wed Aug 10 20:14:56 2022, max compression
+gzip compressed data, was "sfalmanac-1.9.tar", last modified: Thu Sep  1 18:49:30 2022, max compression
```

## Comparing `sfalmanac-1.8.2.tar` & `sfalmanac-1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-08-10 20:14:56.248250 sfalmanac-1.8.2/
--rw-rw-rw-   0        0        0    35149 2019-09-02 18:42:29.000000 sfalmanac-1.8.2/LICENSE
--rw-rw-rw-   0        0        0     8424 2022-08-10 20:14:56.248250 sfalmanac-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     7369 2022-08-10 20:11:06.000000 sfalmanac-1.8.2/README.rst
--rw-rw-rw-   0        0        0      115 2021-02-15 20:39:50.000000 sfalmanac-1.8.2/pyproject.toml
--rw-rw-rw-   0        0        0     1140 2022-08-10 20:14:56.249251 sfalmanac-1.8.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-10 20:14:56.069724 sfalmanac-1.8.2/sfalmanac/
--rw-rw-rw-   0        0        0        0 2021-06-17 20:46:28.000000 sfalmanac-1.8.2/sfalmanac/__init__.py
--rw-rw-rw-   0        0        0    41526 2022-08-09 17:44:21.000000 sfalmanac-1.8.2/sfalmanac/__main__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 20:14:56.075725 sfalmanac-1.8.2/sfalmanac/astro-data/
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.8.2/sfalmanac/astro-data/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 20:14:56.115734 sfalmanac-1.8.2/sfalmanac/data/
--rw-rw-rw-   0        0        0   137935 2021-11-04 20:14:15.000000 sfalmanac-1.8.2/sfalmanac/data/A4chart0-180_P.pdf
--rw-rw-rw-   0        0        0   135960 2021-11-09 08:58:21.000000 sfalmanac-1.8.2/sfalmanac/data/A4chart180-360_P.pdf
--rw-rw-rw-   0        0        0    24577 2019-02-02 20:33:26.000000 sfalmanac-1.8.2/sfalmanac/data/Ra.JPG
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.8.2/sfalmanac/data/__init__.py
--rw-rw-rw-   0        0        0   133928 2020-02-12 20:36:26.000000 sfalmanac-1.8.2/sfalmanac/data/croppedmoon.png
-drwxrwxrwx   0        0        0        0 2022-08-10 20:14:56.153900 sfalmanac-1.8.2/sfalmanac/docs/
--rw-rw-rw-   0        0        0  1743971 2020-03-06 07:11:00.000000 sfalmanac-1.8.2/sfalmanac/docs/Explanation.pdf
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.8.2/sfalmanac/docs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-10 20:14:56.247250 sfalmanac-1.8.2/sfalmanac/lib/
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.8.2/sfalmanac/lib/__init__.py
--rw-rw-rw-   0        0        0     2174 2022-04-26 13:23:35.000000 sfalmanac-1.8.2/sfalmanac/lib/alma_ephem.py
--rw-rw-rw-   0        0        0    75714 2022-05-12 16:08:34.000000 sfalmanac-1.8.2/sfalmanac/lib/alma_skyfield.py
--rw-rw-rw-   0        0        0     4915 2022-05-12 16:02:53.000000 sfalmanac-1.8.2/sfalmanac/lib/config.py
--rw-rw-rw-   0        0        0    24534 2022-08-09 19:14:53.000000 sfalmanac-1.8.2/sfalmanac/lib/eventtables.py
--rw-rw-rw-   0        0        0    11993 2022-04-26 13:25:52.000000 sfalmanac-1.8.2/sfalmanac/lib/increments.py
--rw-rw-rw-   0        0        0   118981 2022-05-14 20:32:26.000000 sfalmanac-1.8.2/sfalmanac/lib/ld_charts.py
--rw-rw-rw-   0        0        0    44934 2022-05-19 18:40:45.000000 sfalmanac-1.8.2/sfalmanac/lib/ld_skyfield.py
--rw-rw-rw-   0        0        0    26131 2022-04-26 13:12:10.000000 sfalmanac-1.8.2/sfalmanac/lib/ld_stardata.py
--rw-rw-rw-   0        0        0    28838 2022-08-09 19:06:58.000000 sfalmanac-1.8.2/sfalmanac/lib/ld_tables.py
--rw-rw-rw-   0        0        0    25675 2022-04-26 13:28:11.000000 sfalmanac-1.8.2/sfalmanac/lib/mp_eventtables.py
--rw-rw-rw-   0        0        0    42465 2022-04-26 13:29:03.000000 sfalmanac-1.8.2/sfalmanac/lib/mp_nautical.py
--rw-rw-rw-   0        0        0    65468 2022-08-10 16:34:58.000000 sfalmanac-1.8.2/sfalmanac/lib/nautical.py
--rw-rw-rw-   0        0        0    20178 2022-08-09 18:55:13.000000 sfalmanac-1.8.2/sfalmanac/lib/suntables.py
-drwxrwxrwx   0        0        0        0 2022-08-10 20:14:56.075725 sfalmanac-1.8.2/sfalmanac.egg-info/
--rw-rw-rw-   0        0        0     8424 2022-08-10 20:14:56.000000 sfalmanac-1.8.2/sfalmanac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2022-08-10 20:14:56.000000 sfalmanac-1.8.2/sfalmanac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-10 20:14:56.000000 sfalmanac-1.8.2/sfalmanac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-02-18 20:32:26.000000 sfalmanac-1.8.2/sfalmanac.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2022-08-10 20:14:56.000000 sfalmanac-1.8.2/sfalmanac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-10 20:14:56.000000 sfalmanac-1.8.2/sfalmanac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-01 18:49:30.218165 sfalmanac-1.9/
+-rw-rw-rw-   0        0        0    35149 2019-09-02 18:42:29.000000 sfalmanac-1.9/LICENSE
+-rw-rw-rw-   0        0        0     8462 2022-09-01 18:49:30.218165 sfalmanac-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7421 2022-09-01 18:40:06.000000 sfalmanac-1.9/README.rst
+-rw-rw-rw-   0        0        0      115 2021-02-15 20:39:50.000000 sfalmanac-1.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1126 2022-09-01 18:49:30.219164 sfalmanac-1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-09-01 18:49:30.195735 sfalmanac-1.9/sfalmanac/
+-rw-rw-rw-   0        0        0        0 2021-06-17 20:46:28.000000 sfalmanac-1.9/sfalmanac/__init__.py
+-rw-rw-rw-   0        0        0    43002 2022-09-01 18:20:51.000000 sfalmanac-1.9/sfalmanac/__main__.py
+drwxrwxrwx   0        0        0        0 2022-09-01 18:49:30.201149 sfalmanac-1.9/sfalmanac/astro-data/
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.9/sfalmanac/astro-data/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-01 18:49:30.204162 sfalmanac-1.9/sfalmanac/data/
+-rw-rw-rw-   0        0        0   137935 2021-11-04 20:14:15.000000 sfalmanac-1.9/sfalmanac/data/A4chart0-180_P.pdf
+-rw-rw-rw-   0        0        0   135960 2021-11-09 08:58:21.000000 sfalmanac-1.9/sfalmanac/data/A4chart180-360_P.pdf
+-rw-rw-rw-   0        0        0    24577 2019-02-02 20:33:26.000000 sfalmanac-1.9/sfalmanac/data/Ra.JPG
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.9/sfalmanac/data/__init__.py
+-rw-rw-rw-   0        0        0   133928 2020-02-12 20:36:26.000000 sfalmanac-1.9/sfalmanac/data/croppedmoon.png
+drwxrwxrwx   0        0        0        0 2022-09-01 18:49:30.207162 sfalmanac-1.9/sfalmanac/docs/
+-rw-rw-rw-   0        0        0  1743971 2020-03-06 07:11:00.000000 sfalmanac-1.9/sfalmanac/docs/Explanation.pdf
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.9/sfalmanac/docs/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-01 18:49:30.217164 sfalmanac-1.9/sfalmanac/lib/
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 sfalmanac-1.9/sfalmanac/lib/__init__.py
+-rw-rw-rw-   0        0        0     2172 2022-09-01 18:09:29.000000 sfalmanac-1.9/sfalmanac/lib/alma_ephem.py
+-rw-rw-rw-   0        0        0    79842 2022-09-01 18:09:56.000000 sfalmanac-1.9/sfalmanac/lib/alma_skyfield.py
+-rw-rw-rw-   0        0        0     5174 2022-09-01 18:07:57.000000 sfalmanac-1.9/sfalmanac/lib/config.py
+-rw-rw-rw-   0        0        0    30979 2022-09-01 18:18:58.000000 sfalmanac-1.9/sfalmanac/lib/eventtables.py
+-rw-rw-rw-   0        0        0    13592 2022-09-01 18:06:28.000000 sfalmanac-1.9/sfalmanac/lib/increments.py
+-rw-rw-rw-   0        0        0   118850 2022-09-01 18:11:16.000000 sfalmanac-1.9/sfalmanac/lib/ld_charts.py
+-rw-rw-rw-   0        0        0    49093 2022-09-01 18:18:19.000000 sfalmanac-1.9/sfalmanac/lib/ld_skyfield.py
+-rw-rw-rw-   0        0        0    26129 2022-09-01 18:14:04.000000 sfalmanac-1.9/sfalmanac/lib/ld_stardata.py
+-rw-rw-rw-   0        0        0    36942 2022-09-01 18:12:17.000000 sfalmanac-1.9/sfalmanac/lib/ld_tables.py
+-rw-rw-rw-   0        0        0    25663 2022-09-01 18:15:35.000000 sfalmanac-1.9/sfalmanac/lib/mp_eventtables.py
+-rw-rw-rw-   0        0        0    42453 2022-09-01 18:17:09.000000 sfalmanac-1.9/sfalmanac/lib/mp_nautical.py
+-rw-rw-rw-   0        0        0    80676 2022-09-01 18:26:51.000000 sfalmanac-1.9/sfalmanac/lib/nautical.py
+-rw-rw-rw-   0        0        0    26522 2022-09-01 18:14:40.000000 sfalmanac-1.9/sfalmanac/lib/suntables.py
+drwxrwxrwx   0        0        0        0 2022-09-01 18:49:30.201149 sfalmanac-1.9/sfalmanac.egg-info/
+-rw-rw-rw-   0        0        0     8462 2022-09-01 18:49:30.000000 sfalmanac-1.9/sfalmanac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2022-09-01 18:49:30.000000 sfalmanac-1.9/sfalmanac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-01 18:49:30.000000 sfalmanac-1.9/sfalmanac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-02-18 20:32:26.000000 sfalmanac-1.9/sfalmanac.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2022-09-01 18:49:30.000000 sfalmanac-1.9/sfalmanac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-09-01 18:49:30.000000 sfalmanac-1.9/sfalmanac.egg-info/top_level.txt
```

### Comparing `sfalmanac-1.8.2/LICENSE` & `sfalmanac-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sfalmanac-1.8.2/PKG-INFO` & `sfalmanac-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sfalmanac
-Version: 1.8.2
-Summary: Creates the daily pages of a Nautical Almanac using Skyfield (and Ephem)
+Version: 1.9
+Summary: Creates the daily pages of a Nautical Almanac using Skyfield
 Home-page: https://github.com/aendie/SFalmanac-Py3
 Author: Andrew Bauer
 Author-email: aendie.bauer@gmail.com
 License: GPL-3.0 License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -54,49 +54,52 @@
 Windows 10 uses up to 8 threads; Linux uses up to 12 threads in parallel. Testing was performed on a PC with an AMD Ryzen 7 3700X 8-Core (16 threads) Processor. Windows & Mac OS spawn new processes; Linux forks new processes (the code is compatible with both techniques and will also run on CPUs with fewer cores/threads).
 
 This performance gain shows that there is practically no justification in using Skyalmanac, which was an interim solution to overcome the poor single-processing performance in SFalmanac at the cost of marginally poorer accuracy in event times (sunset/twilight/sunrise; moonrise/moonset).
 
 Quick Overview
 --------------
 
-This is the **PyPI edition** of `SFalmanac-Py3 <https://github.com/aendie/SFalmanac-Py3>`_ (a Changelog can be viewed here). Version numbering here started from 1.0 as the previous well-tested versions that are on github since 2015 were never published in PyPI. Version numbering follows the scheme *Major.Minor.Patch*, whereby the *Patch* number represents some small correction to the intended release.
+This is the **PyPI edition** of `SFalmanac-Py3 <https://github.com/aendie/SFalmanac-Py3>`_ (a Changelog can be viewed here). Version numbering follows the scheme *Major.Minor.Patch*, whereby the *Patch* number represents some small correction to the intended release.
+
+| **NOTE:** Version numbering in PyPI restarted from 1.0 as the previous well-tested versions that exist since early 2019 were never published in PyPI.
 
 Two astronomical libraries are employed: `Skyfield <https://rhodesmill.org/skyfield/>`_ and `Ephem <https://rhodesmill.org/pyephem/>`_.
 Ephem is only used to calculate a few planet magnitudes (Venus and Jupiter are available in Skyfield).
 
 SFalmanac uses the Hipparcos catalog as its star database. If a current version of Skyfield (>= 1.31) is used, you have two options (which one, you specify by manually editing *config.py*):
 
 * if "useIERS = False", the built-in UT1 tables in the installed version of Skyfield will be employed.
-* if "useIERS = True", for optimal accuracy (especially for all GHA data), Earth orientation data from IERS (International Earth Rotation and Reference Systems Service) is downloaded and then used until it 'expires'. It expires after a chosen number of days (also specifiable in *config.py*). Note that IERS specifies the range of Earth Orientation Parameter (EOP) data currently as "from 2nd January 1973 to 1st October 2023 (continuously advancing)". Refer to the `IERS web site <https://www.iers.org/IERS/EN/Home/home_node.html>`_ for current information.
+* if "useIERS = True", for optimal accuracy (especially for all GHA data), Earth orientation data from IERS (International Earth Rotation and Reference Systems Service) is downloaded and then used until it 'expires'. It expires after a chosen number of days (also specifiable in *config.py*). Note that IERS specifies the range of Earth Orientation Parameter (EOP) data currently as "from 2nd January 1973 to 22nd October 2023 (continuously advancing)". Refer to the `IERS web site <https://www.iers.org/IERS/EN/Home/home_node.html>`_ for current information.
 
 If your Skyfield version is somewhat older (<= 1.30), Skyfield will have downloaded the older files it then used: *deltat.data, deltat.preds* and *Leap_Second.dat*, which are slightly less accurate than the IERS EOP data (which is updated weekly!).
 
 Software Requirements
 =====================
 
 |
 | Nearly all of the astronomical computation is done by the free Skyfield library.
 | Typesetting is done typically by MiKTeX or TeX Live.
 | Here are the requirements/recommendations:
 
 * `python <https://www.python.org/downloads/>`_ >= 3.4 (the latest version is recommended)
 * `skyfield <https://pypi.org/project/skyfield/>`__ >= v1.15 (the latest is recommended; see the `Skyfield Changelog <https://rhodesmill.org/skyfield/installation.html#changelog>`_)
 * `pandas <https://pandas.pydata.org/>`_ >= 1.0 (to decode the Hipparcos catalog)
-* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6 (required for some planet magnitudes)
+* `ephem <https://pypi.org/project/ephem/>`__ = 4.1 (required for some planet magnitudes)
 * `MiKTeX <https://miktex.org/>`_ |nbsp| |nbsp| or |nbsp| |nbsp| `TeX Live <http://www.tug.org/texlive/>`_
 
 Installation
 ============
 
 Install a TeX/LaTeX program on your operating system so that 'pdflatex' is available.
 
 Ensure that the `pip Python installer tool <https://pip.pypa.io/en/latest/installation/>`_ is installed.
 Then ensure that old versions of PyEphem, Ephem and SFalmanac are not installed before installing SFalmanac from PyPI as follows::
 
   python -m pip uninstall pyephem ephem sfalmanac
+  python -m pip install ephem==4.1
   python -m pip install sfalmanac
 
 Installing SFalmanac ensures that Ephem, Skyfield and Pandas (and their dependencies) are also installed. If previous versions of SFalmanac were installed, consider upgrading Skyfield and Pandas thus::
 
   python -m pip install --upgrade skyfield pandas
 
 Thereafter run it with::
```

### Comparing `sfalmanac-1.8.2/README.rst` & `sfalmanac-1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,49 +29,52 @@
 Windows 10 uses up to 8 threads; Linux uses up to 12 threads in parallel. Testing was performed on a PC with an AMD Ryzen 7 3700X 8-Core (16 threads) Processor. Windows & Mac OS spawn new processes; Linux forks new processes (the code is compatible with both techniques and will also run on CPUs with fewer cores/threads).
 
 This performance gain shows that there is practically no justification in using Skyalmanac, which was an interim solution to overcome the poor single-processing performance in SFalmanac at the cost of marginally poorer accuracy in event times (sunset/twilight/sunrise; moonrise/moonset).
 
 Quick Overview
 --------------
 
-This is the **PyPI edition** of `SFalmanac-Py3 <https://github.com/aendie/SFalmanac-Py3>`_ (a Changelog can be viewed here). Version numbering here started from 1.0 as the previous well-tested versions that are on github since 2015 were never published in PyPI. Version numbering follows the scheme *Major.Minor.Patch*, whereby the *Patch* number represents some small correction to the intended release.
+This is the **PyPI edition** of `SFalmanac-Py3 <https://github.com/aendie/SFalmanac-Py3>`_ (a Changelog can be viewed here). Version numbering follows the scheme *Major.Minor.Patch*, whereby the *Patch* number represents some small correction to the intended release.
+
+| **NOTE:** Version numbering in PyPI restarted from 1.0 as the previous well-tested versions that exist since early 2019 were never published in PyPI.
 
 Two astronomical libraries are employed: `Skyfield <https://rhodesmill.org/skyfield/>`_ and `Ephem <https://rhodesmill.org/pyephem/>`_.
 Ephem is only used to calculate a few planet magnitudes (Venus and Jupiter are available in Skyfield).
 
 SFalmanac uses the Hipparcos catalog as its star database. If a current version of Skyfield (>= 1.31) is used, you have two options (which one, you specify by manually editing *config.py*):
 
 * if "useIERS = False", the built-in UT1 tables in the installed version of Skyfield will be employed.
-* if "useIERS = True", for optimal accuracy (especially for all GHA data), Earth orientation data from IERS (International Earth Rotation and Reference Systems Service) is downloaded and then used until it 'expires'. It expires after a chosen number of days (also specifiable in *config.py*). Note that IERS specifies the range of Earth Orientation Parameter (EOP) data currently as "from 2nd January 1973 to 1st October 2023 (continuously advancing)". Refer to the `IERS web site <https://www.iers.org/IERS/EN/Home/home_node.html>`_ for current information.
+* if "useIERS = True", for optimal accuracy (especially for all GHA data), Earth orientation data from IERS (International Earth Rotation and Reference Systems Service) is downloaded and then used until it 'expires'. It expires after a chosen number of days (also specifiable in *config.py*). Note that IERS specifies the range of Earth Orientation Parameter (EOP) data currently as "from 2nd January 1973 to 22nd October 2023 (continuously advancing)". Refer to the `IERS web site <https://www.iers.org/IERS/EN/Home/home_node.html>`_ for current information.
 
 If your Skyfield version is somewhat older (<= 1.30), Skyfield will have downloaded the older files it then used: *deltat.data, deltat.preds* and *Leap_Second.dat*, which are slightly less accurate than the IERS EOP data (which is updated weekly!).
 
 Software Requirements
 =====================
 
 |
 | Nearly all of the astronomical computation is done by the free Skyfield library.
 | Typesetting is done typically by MiKTeX or TeX Live.
 | Here are the requirements/recommendations:
 
 * `python <https://www.python.org/downloads/>`_ >= 3.4 (the latest version is recommended)
 * `skyfield <https://pypi.org/project/skyfield/>`__ >= v1.15 (the latest is recommended; see the `Skyfield Changelog <https://rhodesmill.org/skyfield/installation.html#changelog>`_)
 * `pandas <https://pandas.pydata.org/>`_ >= 1.0 (to decode the Hipparcos catalog)
-* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6 (required for some planet magnitudes)
+* `ephem <https://pypi.org/project/ephem/>`__ = 4.1 (required for some planet magnitudes)
 * `MiKTeX <https://miktex.org/>`_ |nbsp| |nbsp| or |nbsp| |nbsp| `TeX Live <http://www.tug.org/texlive/>`_
 
 Installation
 ============
 
 Install a TeX/LaTeX program on your operating system so that 'pdflatex' is available.
 
 Ensure that the `pip Python installer tool <https://pip.pypa.io/en/latest/installation/>`_ is installed.
 Then ensure that old versions of PyEphem, Ephem and SFalmanac are not installed before installing SFalmanac from PyPI as follows::
 
   python -m pip uninstall pyephem ephem sfalmanac
+  python -m pip install ephem==4.1
   python -m pip install sfalmanac
 
 Installing SFalmanac ensures that Ephem, Skyfield and Pandas (and their dependencies) are also installed. If previous versions of SFalmanac were installed, consider upgrading Skyfield and Pandas thus::
 
   python -m pip install --upgrade skyfield pandas
 
 Thereafter run it with::
```

### Comparing `sfalmanac-1.8.2/setup.cfg` & `sfalmanac-1.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6661 6c6d 616e 6163 0d0a 7665   = sfalmanac..ve
-00000020: 7273 696f 6e20 3d20 312e 382e 320d 0a75  rsion = 1.8.2..u
-00000030: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000040: 6875 622e 636f 6d2f 6165 6e64 6965 2f53  hub.com/aendie/S
-00000050: 4661 6c6d 616e 6163 2d50 7933 0d0a 6175  Falmanac-Py3..au
-00000060: 7468 6f72 203d 2041 6e64 7265 7720 4261  thor = Andrew Ba
-00000070: 7565 720d 0a61 7574 686f 725f 656d 6169  uer..author_emai
-00000080: 6c20 3d20 6165 6e64 6965 2e62 6175 6572  l = aendie.bauer
-00000090: 4067 6d61 696c 2e63 6f6d 0d0a 636c 6173  @gmail.com..clas
-000000a0: 7369 6669 6572 7320 3d20 0d0a 094e 6174  sifiers = ...Nat
-000000b0: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
-000000c0: 2045 6e67 6c69 7368 0d0a 094f 7065 7261   English...Opera
-000000d0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000000e0: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-000000f0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000100: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
-00000110: 7469 6f6e 2f53 7461 626c 650d 0a09 4c69  tion/Stable...Li
-00000120: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000130: 726f 7665 6420 3a3a 2047 4e55 2047 656e  roved :: GNU Gen
-00000140: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00000150: 6e73 6520 7633 2028 4750 4c76 3329 0d0a  nse v3 (GPLv3)..
-00000160: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000170: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000180: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001a0: 7974 686f 6e20 3a3a 2033 2e34 0d0a 0950  ython :: 3.4...P
-000001b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001d0: 2033 2e35 0d0a 0950 726f 6772 616d 6d69   3.5...Programmi
-000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001f0: 7974 686f 6e20 3a3a 2033 2e36 0d0a 0950  ython :: 3.6...P
-00000200: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000210: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000220: 2033 2e37 0d0a 0950 726f 6772 616d 6d69   3.7...Programmi
-00000230: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000240: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000270: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-00000280: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000290: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
-000002a0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-000002b0: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
-000002c0: 3a3a 2041 7374 726f 6e6f 6d79 0d0a 6465  :: Astronomy..de
-000002d0: 7363 7269 7074 696f 6e20 3d20 4372 6561  scription = Crea
-000002e0: 7465 7320 7468 6520 6461 696c 7920 7061  tes the daily pa
-000002f0: 6765 7320 6f66 2061 204e 6175 7469 6361  ges of a Nautica
-00000300: 6c20 416c 6d61 6e61 6320 7573 696e 6720  l Almanac using 
-00000310: 536b 7966 6965 6c64 2028 616e 6420 4570  Skyfield (and Ep
-00000320: 6865 6d29 0d0a 6c69 6365 6e73 6520 3d20  hem)..license = 
-00000330: 4750 4c2d 332e 3020 4c69 6365 6e73 650d  GPL-3.0 License.
-00000340: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000350: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-00000360: 2e72 7374 0d0a 6c6f 6e67 5f64 6573 6372  .rst..long_descr
-00000370: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000380: 7970 6520 3d20 7465 7874 2f78 2d72 7374  ype = text/x-rst
-00000390: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-000003a0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-000003b0: 203e 3d33 2e34 0d0a 7a69 702d 7361 6665   >=3.4..zip-safe
-000003c0: 203d 2046 616c 7365 0d0a 7061 636b 6167   = False..packag
-000003d0: 6573 203d 2066 696e 643a 0d0a 696e 7374  es = find:..inst
-000003e0: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-000003f0: 0a09 4570 6865 6d0d 0a09 5061 6e64 6173  ..Ephem...Pandas
-00000400: 0d0a 0953 6b79 6669 656c 640d 0a09 4e75  ...Skyfield...Nu
-00000410: 6d70 790d 0a0d 0a5b 6f70 7469 6f6e 732e  mpy....[options.
-00000420: 7061 636b 6167 655f 6461 7461 5d0d 0a2a  package_data]..*
-00000430: 203d 202a 2e70 6466 2c20 2a2e 6a70 672c   = *.pdf, *.jpg,
-00000440: 202a 2e70 6e67 0d0a 0d0a 5b65 6767 5f69   *.png....[egg_i
-00000450: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000460: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000470: 0d0a 0d0a                                ....
+00000020: 7273 696f 6e20 3d20 312e 390d 0a75 726c  rsion = 1.9..url
+00000030: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000040: 622e 636f 6d2f 6165 6e64 6965 2f53 4661  b.com/aendie/SFa
+00000050: 6c6d 616e 6163 2d50 7933 0d0a 6175 7468  lmanac-Py3..auth
+00000060: 6f72 203d 2041 6e64 7265 7720 4261 7565  or = Andrew Baue
+00000070: 720d 0a61 7574 686f 725f 656d 6169 6c20  r..author_email 
+00000080: 3d20 6165 6e64 6965 2e62 6175 6572 4067  = aendie.bauer@g
+00000090: 6d61 696c 2e63 6f6d 0d0a 636c 6173 7369  mail.com..classi
+000000a0: 6669 6572 7320 3d20 0d0a 094e 6174 7572  fiers = ...Natur
+000000b0: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
+000000c0: 6e67 6c69 7368 0d0a 094f 7065 7261 7469  nglish...Operati
+000000d0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+000000e0: 496e 6465 7065 6e64 656e 740d 0a09 4465  Independent...De
+000000f0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000100: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
+00000110: 6f6e 2f53 7461 626c 650d 0a09 4c69 6365  on/Stable...Lice
+00000120: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000130: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
+00000140: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
+00000150: 6520 7633 2028 4750 4c76 3329 0d0a 0950  e v3 (GPLv3)...P
+00000160: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000170: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000180: 2033 0d0a 0950 726f 6772 616d 6d69 6e67   3...Programming
+00000190: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001a0: 686f 6e20 3a3a 2033 2e34 0d0a 0950 726f  hon :: 3.4...Pro
+000001b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001d0: 2e35 0d0a 0950 726f 6772 616d 6d69 6e67  .5...Programming
+000001e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001f0: 686f 6e20 3a3a 2033 2e36 0d0a 0950 726f  hon :: 3.6...Pro
+00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000220: 2e37 0d0a 0950 726f 6772 616d 6d69 6e67  .7...Programming
+00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000240: 686f 6e20 3a3a 2033 2e38 0d0a 0950 726f  hon :: 3.8...Pro
+00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000270: 2e39 0d0a 0950 726f 6772 616d 6d69 6e67  .9...Programming
+00000280: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000290: 686f 6e20 3a3a 2033 2e31 300d 0a09 546f  hon :: 3.10...To
+000002a0: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
+000002b0: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
+000002c0: 2041 7374 726f 6e6f 6d79 0d0a 6465 7363   Astronomy..desc
+000002d0: 7269 7074 696f 6e20 3d20 4372 6561 7465  ription = Create
+000002e0: 7320 7468 6520 6461 696c 7920 7061 6765  s the daily page
+000002f0: 7320 6f66 2061 204e 6175 7469 6361 6c20  s of a Nautical 
+00000300: 416c 6d61 6e61 6320 7573 696e 6720 536b  Almanac using Sk
+00000310: 7966 6965 6c64 0d0a 6c69 6365 6e73 6520  yfield..license 
+00000320: 3d20 4750 4c2d 332e 3020 4c69 6365 6e73  = GPL-3.0 Licens
+00000330: 650d 0a6c 6f6e 675f 6465 7363 7269 7074  e..long_descript
+00000340: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+00000350: 4d45 2e72 7374 0d0a 6c6f 6e67 5f64 6573  ME.rst..long_des
+00000360: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+00000370: 5f74 7970 6520 3d20 7465 7874 2f78 2d72  _type = text/x-r
+00000380: 7374 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  st....[options].
+00000390: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+000003a0: 203d 203e 3d33 2e34 0d0a 7a69 705f 7361   = >=3.4..zip_sa
+000003b0: 6665 203d 2046 616c 7365 0d0a 7061 636b  fe = False..pack
+000003c0: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
+000003d0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+000003e0: 200d 0a09 4570 6865 6d0d 0a09 5061 6e64   ...Ephem...Pand
+000003f0: 6173 0d0a 0953 6b79 6669 656c 640d 0a09  as...Skyfield...
+00000400: 4e75 6d70 790d 0a0d 0a5b 6f70 7469 6f6e  Numpy....[option
+00000410: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
+00000420: 0a2a 203d 202a 2e70 6466 2c20 2a2e 6a70  .* = *.pdf, *.jp
+00000430: 672c 202a 2e70 6e67 0d0a 0d0a 5b65 6767  g, *.png....[egg
+00000440: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000450: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000460: 2030 0d0a 0d0a                            0....
```

### Comparing `sfalmanac-1.8.2/sfalmanac/__main__.py` & `sfalmanac-1.9/sfalmanac/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,49 +4,50 @@
 #   Copyright (C) 2022  Andrew Bauer
 #   Copyright (C) 2014  Enno Rodegerdts
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 ###### Standard library imports ######
 import os
 import sys, site
-from sysconfig import get_path  # new in python 3.2
 import time
-import datetime
+from sysconfig import get_path  # new in python 3.2
+from datetime import date, datetime, timedelta
 from multiprocessing import cpu_count
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 # !! execute the next 3 lines before importing from nautical/eventtables !!
 config.WINpf = True if sys.platform.startswith('win') else False
 config.LINUXpf = True if sys.platform.startswith('linux') else False
 config.MACOSpf = True if sys.platform == 'darwin' else False
+config.FANCYhd = False  # default for TeX Live <= "TeX Live 2019/Debian"
 config.CPUcores = cpu_count()
 # NOTE: Multiprocessing on Windows using 'spawn' requires all variables modified
 #       and stored in config.py to be re-calculated for every spawned process!
 # NOTE: multiprocessing is supported in modules: nautical, eventtables
-from sfalmanac.lib.alma_skyfield import init_sf as init_sf
-from sfalmanac.lib.ld_skyfield import ld_init_sf as ld_init_sf
-from sfalmanac.lib.nautical import almanac as almanac
-from sfalmanac.lib.suntables import sunalmanac as sunalmanac
-from sfalmanac.lib.eventtables import makeEVtables as makeEVtables
-from sfalmanac.lib.ld_tables import makeLDtables as makeLDtables
-from sfalmanac.lib.ld_charts import makeLDcharts as makeLDcharts
-from sfalmanac.lib.increments import makelatex as makelatex
+from sfalmanac.lib.alma_skyfield import init_sf
+from sfalmanac.lib.ld_skyfield import ld_init_sf
+from sfalmanac.lib.nautical import almanac
+from sfalmanac.lib.suntables import sunalmanac
+from sfalmanac.lib.eventtables import makeEVtables
+from sfalmanac.lib.ld_tables import makeLDtables
+from sfalmanac.lib.ld_charts import makeLDcharts
+from sfalmanac.lib.increments import makelatex
 
 #   Some modules in SFalmanac have been ported from the original source code ...
 #   this may explain why sections of code are not consolidated. Furthermore two
 #   separate Skyfield modules are used with obvious repetition of code. This
 #   simplifies porting from the original code for development and testing.
 
 def toUnix(fn):
@@ -116,25 +117,25 @@
         sys.exit(0)
 
 def check_years(yearfr, yearto):
     global yrmin, yrmax
 
     if str(yearfr).isnumeric():
         if yrmin <= int(yearfr) <= yrmax:
-            first_day = datetime.date(int(yearfr), 1, 1)
+            first_day = date(int(yearfr), 1, 1)
         else:
             print("!! Please pick a year between {} and {} !!".format(yrmin,yrmax))
             sys.exit(0)
     else:
         print("Error! First year is not numeric")
         sys.exit(0)
 
     if str(yearto).isnumeric():
         if yrmin <= int(yearto) <= yrmax:
-            first_day_to = datetime.date(int(yearto), 1, 1)
+            first_day_to = date(int(yearto), 1, 1)
         else:
             print("!! Please pick a year between {} and {} !!".format(yrmin,yrmax))
             sys.exit(0)
         if int(yearto) < int(yearfr):
             print("Error! The LAST year must be later than the FIRST year")
             sys.exit(0)
     else:
@@ -211,40 +212,76 @@
         print("\nNOTE: only {} logical processors are available for parallel processessing".format(config.CPUcores))
 
 
 ###### Main Program ######
 
 if __name__ == '__main__':      # required for Windows multiprocessing compatibility
     if sys.version_info[0] < 3:
-        raise Exception("This runs only with Python 3")
+        print("This runs only with Python 3")
+        sys.exit(0)
+
+    # check if TeX Live is compatible with the 'fancyhdr' package...
+    process = os.popen("tex --version")
+    returned_value = process.read()
+    process.close()
+    if returned_value == "":
+        print("- - - Neither TeX Live nor MiKTeX is installed - - -")
+        sys.exit(0)
+    pos1 = returned_value.find("(") 
+    pos2 = returned_value.find(")")
+    if pos1 != -1 and pos2 != -1:
+        texver = returned_value[pos1+1:pos2]
+        # e.g. "TeX Live 2019/Debian", "TeX Live 2022/dev/Debian", "MiKTeX 22.7.30"
+        if texver[:8] == "TeX Live":
+            yrtxt = texver[9:13]
+            if yrtxt.isnumeric():
+                yr = int(yrtxt)
+                if yr >= 2020:
+                    config.FANCYhd = True  # TeX Live can handle the 'fancyhdr' package
+        else:
+            config.FANCYhd = True  # assume MiKTeX can handle the 'fancyhdr' package
 
     # command line arguments...
-    validargs = ['-v', '-q', '-log', '-tex', '-sky', '-d1', '-d2', '-d3', '-d4']
+    validargs = ['-v', '-q', '-log', '-tex', '-sky', '-old', 'a4', '-let', '-dpo', '-nmg', '-d1', '-d2', '-d3', '-d4']
     # (the 4 dummy arguments d1 d2 d3 d4 are specified in 'dockerfile')
     for i in list(range(1, len(sys.argv))):
         if sys.argv[i] not in validargs:
             print("Invalid argument: {}".format(sys.argv[i]))
             print("\nValid command line arguments are:")
-            print(" -v   ... to send pdfTeX output to the terminal")
+            print(" -v   ... 'verbose': to send pdfTeX output to the terminal")
             print(" -q   ... quiet mode for LD charts")
             print(" -log ... to keep the log file")
             print(" -tex ... to keep the tex file")
             print(" -sky ... stars only in LD charts")
+            print(" -old ... old formatting without the 'fancyhdr' package")
+            print(" -a4  ... A4 papersize")
+            print(" -let ... Letter papersize")
+            print(" -dpo ... data pages only")
             sys.exit(0)
 
     # NOTE: pdfTeX 3.14159265-2.6-1.40.21 (TeX Live 2020/Debian), as used in the Docker
     #       Image, does not have the options "-quiet" or "-verbose".
     listarg = "" if "-v" in set(sys.argv[1:]) else "-interaction=batchmode -halt-on-error "
     keeplog = True if "-log" in set(sys.argv[1:]) else False
     keeptex = True if "-tex" in set(sys.argv[1:]) else False
     quietmode = True if "-q" in set(sys.argv[1:]) else False
     onlystars = True if "-sky" in set(sys.argv[1:]) else False
+    if "-nmg" in set(sys.argv[1:]): config.moonimg = False  # only for debugging
+    config.DPonly = True if "-dpo" in set(sys.argv[1:]) else False
+    if "-old" in set(sys.argv[1:]): config.FANCYhd = False  # don't use the 'fancyhdr' package
+    forcepgsz = False
+    if not("-a4" in set(sys.argv[1:]) and "-let" in set(sys.argv[1:])):
+        if "-a4" in set(sys.argv[1:]): forcepgsz = True
+        if "-let" in set(sys.argv[1:]): forcepgsz = True
+    if forcepgsz:
+        if "-a4" in set(sys.argv[1:]): config.pgsz = "A4"
+        if "-let" in set(sys.argv[1:]): config.pgsz = "Letter"
 
-    d = datetime.datetime.utcnow().date()
-    first_day = datetime.date(d.year, d.month, d.day)
+    d = datetime.utcnow().date()
+    first_day = date(d.year, d.month, d.day)
     yy = "%s" % d.year
 
     # if this code runs locally (not in Docker), the settings in config.py are used.
     # if this code runs in Docker without use of an environment file, the settings in config.py apply.
     # if this code runs in Docker with an environment file ("--env-file ./.env"), then its values apply.
     ageERR = False
     ephERR = False
@@ -314,15 +351,15 @@
 
     mfp = sys.modules['__main__'].__file__  # main module filepath
     pkg = mfp.split(os.path.sep)[-2]        # this package name
 
     spad = ""
     spdf = ""
     spcf = ""
-    if sys.platform.startswith('win'):  # Windows 10 (also in 'venv' virtual environment)
+    if config.WINpf:  # Windows 10 (also in 'venv' virtual environment)
         syspf = sys.exec_prefix.replace("\\","/")
         spad = syspf + "/Lib/site-packages/" + pkg + "/astro-data/"  # path to downloaded data
         spdf = syspf + "/Lib/site-packages/" + pkg + "/data/"  # path to data files
         spcf = syspf + "/Lib/site-packages/" + pkg + "/lib/"   # path to config.py
         spcf = spcf.replace("/","\\")
         spad = spad.replace("/","\\")
     else:                               # POSIX (Linux & Mac OS X)
@@ -432,20 +469,20 @@
                 elif len(ss) == 8:
                     dd = ss[:2]
                     mm = ss[2:4]
                     check_mth(mm)
                     yy = ss[4:]
                     check_date(yy,mm,dd)
                 
-                first_day = datetime.date(int(yy), int(mm), int(dd))
+                first_day = date(int(yy), int(mm), int(dd))
                 d = first_day
 
                 if len(ss) in [2,3]:    # process entire month
                     entireMth = True
-                    daystoprocess = (d.replace(month = d.month%12 + 1, day = 1)-datetime.timedelta(days=1)).day
+                    daystoprocess = (d.replace(month = d.month%12 + 1, day = 1)-timedelta(days=1)).day
 
                 if not entireYr and not entireMth and daystoprocess == 0:
                     daystoprocess = 1       # default
                     nn = input("""  Enter number of days to process from starting date:
 """)
                     if len(nn) > 0:
                         if not nn.isnumeric():
@@ -500,20 +537,20 @@
                 check_mth(mm)
                 check_date(yy,mm,dd)
 
                 if not (yrmin <= int(yy) <= yrmax):
                     print("!! Please pick a year between {} and {} !!".format(yrmin,yrmax))
                     sys.exit(0)
 
-                first_day = datetime.date(int(yy), int(mm), int(dd))
+                first_day = date(int(yy), int(mm), int(dd))
                 d = first_day
 
                 if len(ss) in [2,3]:     # process entire month
                     entireMth = True
-                    daystoprocess = (d.replace(month = d.month%12 + 1, day = 1)-datetime.timedelta(days=1)).day
+                    daystoprocess = (d.replace(month = d.month%12 + 1, day = 1)-timedelta(days=1)).day
 
                 if daystoprocess == 0:
                     daystoprocess = 1       # default
                     nn = input("""  Enter number of days to process from starting date:
 """)
                     if len(nn) > 0:
                         if not nn.isnumeric():
@@ -583,15 +620,15 @@
                 config.moonDataFound = 0
                 config.moonHorizonSeeks = 0
                 config.moonHorizonFound = 0
                 year = "{:4d}".format(yearint)  # year = "%4d" %yearint
                 msg = "\nCreating the nautical almanac for the year {}".format(year)
                 print(msg)
     ##            config.writeLOG(msg)
-                first_day = datetime.date(yearint, 1, 1)
+                first_day = date(yearint, 1, 1)
                 ff = "NAtrad" if config.tbls != 'm' else "NAmod"
                 fn = toUnix("{}({})_{}".format(ff,papersize,year+DecFmt))
                 deletePDF(f_prefix + fn)
                 # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
                 outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
                 outfile.write(almanac(first_day,0,ts,spad,df180,df360,dfcm))
                 outfile.close()
@@ -646,15 +683,15 @@
             txt = "from" if daystoprocess > 1 else "for"
             msg = "\nCreating the nautical almanac {} {}".format(txt,first_day.strftime("%d %B %Y"))
             print(msg)
     ##            config.writeLOG(msg)
             ff = "NAtrad" if config.tbls != 'm' else "NAmod"
             dto = ""
             if daystoprocess > 1:   # filename as 'from date'-'to date'
-                lastdate = d + datetime.timedelta(days=daystoprocess-1)
+                lastdate = d + timedelta(days=daystoprocess-1)
                 dto = lastdate.strftime("-%Y%m%d")
             fn = toUnix("{}({})_{}".format(ff,papersize,symd+dto+DecFmt))
             deletePDF(f_prefix + fn)
             # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
             outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
             outfile.write(almanac(first_day,daystoprocess,ts,spad,df180,df360,dfcm))
             outfile.close()
@@ -669,15 +706,15 @@
 
         elif s == '2' and entireYr:     # Sun Tables (for a year/years)
             check_exists(spdf + "Ra.jpg")
             for yearint in range(int(yearfr),int(yearto)+1):
                 year = "{:4d}".format(yearint)  # year = "%4d" %yearint
                 msg = "\nCreating the sun tables for the year {}".format(year)
                 print(msg)
-                first_day = datetime.date(yearint, 1, 1)
+                first_day = date(yearint, 1, 1)
                 ff = "STtrad" if config.tbls != 'm' else "STmod"
                 fn = toUnix("{}({})_{}".format(ff,papersize,year+DecFmt))
                 deletePDF(f_prefix + fn)
                 # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
                 outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
                 outfile.write(sunalmanac(first_day,0,dfra))
                 outfile.close()
@@ -708,15 +745,15 @@
             check_exists(spdf + "Ra.jpg")
             txt = "from" if daystoprocess > 1 else "for"
             msg = "\nCreating the sun tables {} {}".format(txt,first_day.strftime("%d %B %Y"))
             print(msg)
             ff = "STtrad" if config.tbls != 'm' else "STmod"
             dto = ""
             if daystoprocess > 1:   # filename as 'from date'-'to date'
-                lastdate = d + datetime.timedelta(days=daystoprocess-1)
+                lastdate = d + timedelta(days=daystoprocess-1)
                 dto = lastdate.strftime("-%Y%m%d")
             fn = toUnix("{}({})_{}".format(ff,papersize,symd+dto+DecFmt))
             deletePDF(f_prefix + fn)
             # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
             outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
             outfile.write(sunalmanac(first_day,daystoprocess,dfra))
             outfile.close()
@@ -732,15 +769,15 @@
             print("Take a break - this computer needs some time for cosmic meditation.")
             for yearint in range(int(yearfr),int(yearto)+1):
                 if config.MULTIpr: checkCoreCount()
                 start = timer_start()
                 year = "{:4d}".format(yearint)  # year = "%4d" %yearint
                 msg = "\nCreating the event time tables for the year {}".format(year)
                 print(msg)
-                first_day = datetime.date(yearint, 1, 1)
+                first_day = date(yearint, 1, 1)
                 fn = toUnix("Event-Times({})_{}".format(papersize,year))
                 deletePDF(f_prefix + fn)
                 # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
                 outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
                 outfile.write(makeEVtables(first_day,0,ts,spad,df180,df360))
                 outfile.close()
                 # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
@@ -776,15 +813,15 @@
             if config.MULTIpr: checkCoreCount()
             start = timer_start()
             txt = "from" if daystoprocess > 1 else "for"
             msg = "\nCreating the event time tables {} {}".format(txt,first_day.strftime("%d %B %Y"))
             print(msg)
             fn = toUnix("Event-Times({})_{}".format(papersize,symd))
             if daystoprocess > 1:   # filename as 'from date'-'to date'
-                lastdate = d + datetime.timedelta(days=daystoprocess-1)
+                lastdate = d + timedelta(days=daystoprocess-1)
                 fn += lastdate.strftime("-%Y%m%d")
             deletePDF(f_prefix + fn)
             # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
             outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
             outfile.write(makeEVtables(first_day,daystoprocess,ts,spad,df180,df360))
             outfile.close()
             # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
@@ -799,46 +836,46 @@
             check_exists(spdf + "A4chart180-360_P.pdf")
             if entireYr: # Lunar Distance tables (for a year/years)
                 for yearint in range(int(yearfr),int(yearto)+1):
                     start = time.time()
                     year = "{:4d}".format(yearint)  # year = "%4d" %yearint
                     msg = "\nCreating the lunar distance tables for the year {}".format(year)
                     print(msg)
-                    daystoprocess = (datetime.date(yearint+1, 1, 1) - datetime.date(yearint, 1, 1)).days
+                    daystoprocess = (date(yearint+1, 1, 1) - date(yearint, 1, 1)).days
                     fn = toUnix("LDtable({})_{}".format(papersize,year))
-                    first_day = datetime.date(yearint, 1, 1)
+                    first_day = date(yearint, 1, 1)
                     # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
                     outfile = open(fn + ".tex", mode="w", encoding="utf8")
-                    outfile.write(makeLDtables(first_day,strat,daystoprocess,entireMth,entireYr,spad,df180,df360))
+                    outfile.write(makeLDtables(first_day,0,strat,df180,df360))
                     outfile.close()
                     # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
                     if config.dockerized: os.chdir(os.getcwd() + f_postfix)     # DOCKER ONLY
                     stop = time.time()
                     msg2 = "execution time = {:0.2f} seconds".format(stop-start)
                     print(msg2)
                     makePDF(listarg, fn)
                     tidy_up(fn, keeplog, keeptex)
             else:
                 start = time.time()
                 if entireMth:
                     fn = toUnix("LDtable({})_{}".format(papersize,syr + '-' + smth))
-                    msg = "\nCreating the lunar distance tables for {}".format(syr + '-' + smth)
+                    msg = "\nCreating the lunar distance tables for {}".format(first_day.strftime("%B %Y"))
+                    daystoprocess = -1
                 else:
                     fn = toUnix("LDtable({})_{}".format(papersize,symd))
                     if daystoprocess > 1:   # filename as 'from date'-'to date'
-                        lastdate = first_day + datetime.timedelta(days=daystoprocess-1)
-                        lymd = lastdate.strftime("-%Y%m%d")
-                        fn += lymd
-                        msg = "\nCreating the lunar distance tables from {}".format(symd)
-                    else: msg = "\nCreating the lunar distance table for {}".format(symd)
+                        lastdate = first_day + timedelta(days=daystoprocess-1)
+                        fn += lastdate.strftime("-%Y%m%d")
+                    txt = "from" if daystoprocess > 1 else "for"
+                    msg = "\nCreating the lunar distance tables {} {}".format(txt,symd)
                 print(msg)
                 deletePDF(f_prefix + fn)
                 # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
                 outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
-                outfile.write(makeLDtables(first_day,strat,daystoprocess,entireMth,entireYr,spad,df180,df360))
+                outfile.write(makeLDtables(first_day,daystoprocess,strat,df180,df360))
                 outfile.close()
                 # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
                 if config.dockerized: os.chdir(os.getcwd() + f_postfix)     # DOCKER ONLY
                 stop = time.time()
                 msg2 = "execution time = {:0.2f} seconds".format(stop-start)
                 print(msg2)
                 makePDF(listarg, fn)
@@ -846,42 +883,41 @@
 
         elif s == '5':  # Lunar Distance charts
             if entireMth:
                 fn = toUnix("LDchart({})_{}".format(papersize,syr + '-' + smth))
             else:
                 fn = toUnix("LDchart({})_{}".format(papersize,symd))
                 if daystoprocess > 1:   # filename as 'from date'-'to date'
-                    lastdate = first_day + datetime.timedelta(days=daystoprocess-1)
-                    lymd = lastdate.strftime("-%Y%m%d")
-                    fn += lymd
+                    lastdate = first_day + timedelta(days=daystoprocess-1)
+                    fn += lastdate.strftime("-%Y%m%d")
             deletePDF(f_prefix + fn)
 
             start = time.time()
             if entireYr: msg = "\nCreating the lunar distance charts for the year {}".format(syr)
             elif entireMth: msg = "\nCreating the lunar distance charts for {}".format(syr + '-' + smth)
             elif daystoprocess > 1: msg = "\nCreating the lunar distance charts from {}".format(symd)
             else: msg = "\nCreating the lunar distance chart for {}".format(symd)
             print(msg)
             # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
             outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
-            makeLDcharts(first_day,strat,daystoprocess,outfile,spad,ts,onlystars,quietmode)
+            makeLDcharts(first_day,strat,daystoprocess,outfile,ts,onlystars,quietmode)
             outfile.close()
             # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
             if config.dockerized: os.chdir(os.getcwd() + f_postfix)     # DOCKER ONLY
             stop = time.time()
             msg2 = "\nexecution time = {:0.2f} seconds".format(stop-start)
             print(msg2)
             msg = " creating {}".format(fn + ".pdf")
             makePDF(listarg, fn, msg)
             tidy_up(fn, keeplog, keeptex)
 
-        elif s == '6':
+        elif s == '6':  # Increments and Corrections tables
             msg = "\nCreating the Increments and Corrections tables"
             print(msg)
-            fn = toUnix("Inc(A4)")
+            fn = toUnix("Inc({})").format(papersize)
             deletePDF(f_prefix + fn)
             # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
             outfile = open(f_prefix + fn + ".tex", mode="w", encoding="utf8")
             outfile.write(makelatex())
             outfile.close()
             # :::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
             if config.dockerized: os.chdir(os.getcwd() + f_postfix)     # DOCKER ONLY
```

### Comparing `sfalmanac-1.8.2/sfalmanac/data/A4chart0-180_P.pdf` & `sfalmanac-1.9/sfalmanac/data/A4chart0-180_P.pdf`

 * *Files identical despite different names*

### Comparing `sfalmanac-1.8.2/sfalmanac/data/A4chart180-360_P.pdf` & `sfalmanac-1.9/sfalmanac/data/A4chart180-360_P.pdf`

 * *Files identical despite different names*

### Comparing `sfalmanac-1.8.2/sfalmanac/data/Ra.JPG` & `sfalmanac-1.9/sfalmanac/data/Ra.JPG`

 * *Files identical despite different names*

### Comparing `sfalmanac-1.8.2/sfalmanac/data/croppedmoon.png` & `sfalmanac-1.9/sfalmanac/data/croppedmoon.png`

 * *Files identical despite different names*

### Comparing `sfalmanac-1.8.2/sfalmanac/docs/Explanation.pdf` & `sfalmanac-1.9/sfalmanac/docs/Explanation.pdf`

 * *Files identical despite different names*

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/alma_ephem.py` & `sfalmanac-1.9/sfalmanac/lib/alma_ephem.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #   Copyright (C) 2022  Andrew Bauer
 #   Copyright (C) 2014  Enno Rodegerdts
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # This contains one function to calculate planet magnitudes...
 # ... because these are not in Skyfield yet
 
 ###### Third party imports ######
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/alma_skyfield.py` & `sfalmanac-1.9/sfalmanac/lib/alma_skyfield.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,52 +3,61 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # This contains the majority of functions that calculate values for the Nautical Almanac
 
 ###### Standard library imports ######
-import datetime
-import time         # 00000 - stopwatch elements
-import math
+# don't confuse the 'date' method with the 'Date' variable!
+#   the following line includes 'datetime.combine' class method:
+from datetime import date, time, datetime, timedelta
+# don't confuse the 'time' instance method in the 'datetime' object with the 'Time' module:
+import time as Time # 00000 - stopwatch elements
+from math import pi, cos, tan, atan, degrees, copysign
 import os
 import errno
 import socket
 import sys			# required for .stdout.write()
+import urllib.error # used in 'download_EOP' function
 from urllib.request import urlopen
+from collections import deque
 
 ###### Third party imports ######
 from skyfield import VERSION
 from skyfield.api import Loader
 from skyfield.api import Topos, Star
 from skyfield import almanac
 from skyfield.nutationlib import iau2000b
 from skyfield.data import hipparcos
 from skyfield.magnitudelib import planetary_magnitude
 import numpy as np
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 
 #---------------------------
 #   Module initialization
 #---------------------------
 
+urlIERS = "ftp://ftp.iers.org/products/eop/rapid/standard/"
+urlUSNO = "https://maia.usno.navy.mil/ser7/"        # alternate location
+urlDCIERS = "https://datacenter.iers.org/data/9/"   # alternate location
+
 hour_of_day = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23]
 next_hour_of_day = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24]
 degree_sign= u'\N{DEGREE SIGN}'
 
 def compareVersion(versions1, version2):
     #versions1 = [int(v) for v in version1.split(".")]
     versions2 = [int(v) for v in version2.split(".")]
@@ -79,31 +88,38 @@
         pass
     return False    # if neither is reachable
 
 # NOTE: the IERS server is unavailable (due to maintenance work in the first 3 weeks, at least, of April 2022)
 #       however, although the USNO server currently works, it was previously down for 2.5 years!
 #       So it is still best to try using the IERS server as first oprion, and USNO as second.
 
-def testIERSserver(filename):
-    url = "ftp://ftp.iers.org/products/eop/rapid/standard/" + filename
+def testServer(filename, url):
+    url += filename
     try:
         connection2 = urlopen(url)
     except Exception as e:
         e2 = IOError('cannot download {0} because {1}'.format(url, e))
         e2.__cause__ = None
 #        raise e2
         return False
     return True     # server works
 
-def downloadUSNO(path, filename):
-    sys.stdout.write("Downloading EOP data from USNO...")
+def download_EOP(path, filename, url, loc):
+    # NOTE: the following 'print' statement does not print immediately in Linux!
+    #print("Downloading EOP data from USNO...", end ="")
+    sys.stdout.write("Downloading EOP data from {}...".format(loc))
     sys.stdout.flush()
     filepath = os.path.join(path, filename)
-    url = "https://maia.usno.navy.mil/ser7/" + filename
-    connection = urlopen(url)
+    url += filename
+    try:
+        connection = urlopen(url)
+    except urllib.error.URLError as e:
+        #raise IOError('error getting {0} - {1}'.format(url, e))
+        print('\nError getting {0} - {1}'.format(url, e))
+        sys.exit(0)
     blocksize = 128*1024
 
     # Claim our own unique download filename.
 
     tempbase = tempname = path + filename + '.download'
     flags = getattr(os, 'O_BINARY', 0) | os.O_CREAT | os.O_EXCL | os.O_RDWR
     i = 1
@@ -146,37 +162,107 @@
     sys.stdout.flush()
 
 def init_sf(spad):
     global ts, eph, earth, moon, sun, venus, mars, jupiter, saturn, df
     load = Loader(spad)         # spad = folder to store the downloaded files
     EOPdf  = "finals2000A.all"  # Earth Orientation Parameters data file
     dfIERS = spad + EOPdf
+    config.useIERSEOP = False
+    config.txtIERSEOP = ""
 
     if config.useIERS:
         if compareVersion(VERSION, "1.31") >= 0:
             if os.path.isfile(dfIERS):
                 if load.days_old(EOPdf) > float(config.ageIERS):
                     if isConnected():
-                        if testIERSserver(EOPdf): load.download(EOPdf)
-                        else: downloadUSNO(spad,EOPdf)
+                        if testServer(EOPdf, urlIERS):  # first try downloading via FTP
+                            load.download(EOPdf)
+                        elif testServer(EOPdf, urlUSNO):# then try the USNO server
+                            download_EOP(spad,EOPdf,urlUSNO,"USNO")
+                        else:   # finally try the IERS datacenter (available in more countries)
+                            download_EOP(spad,EOPdf,urlDCIERS,"IERS datacenter")
                     else: print("NOTE: no Internet connection... using existing '{}'".format(EOPdf))
                 ts = load.timescale(builtin=False)	# timescale object
+                config.useIERSEOP = True
             else:
                 if isConnected():
-                    if testIERSserver(EOPdf): load.download(EOPdf)
-                    else: downloadUSNO(spad,EOPdf)
+                    if testServer(EOPdf, urlIERS):  # first try downloading via FTP
+                        load.download(EOPdf)
+                    elif testServer(EOPdf, urlUSNO):# then try the USNO server
+                        download_EOP(spad,EOPdf,urlUSNO,"USNO")
+                    else:   # finally try the IERS datacenter (available in more countries)
+                        download_EOP(spad,EOPdf,urlDCIERS,"IERS datacenter")
                     ts = load.timescale(builtin=False)	# timescale object
+                    config.useIERSEOP = True
                 else:
                     print("NOTE: no Internet connection... using built-in UT1-tables")
                     ts = load.timescale()	# timescale object with built-in UT1-tables
         else:
             ts = load.timescale()	# timescale object with built-in UT1-tables
     else:
         ts = load.timescale()	# timescale object with built-in UT1-tables
 
+    if config.useIERSEOP and os.path.isfile(dfIERS):
+# get the IERS EOP data "release date" according to these rules:
+#   - begin searching within this millenium (ignoring data from 02 Jan 1973 to 31 Dec 1999)
+#   - halt when the following value is "P", i.e. predicted as opposed to measured:
+#       - flag for Bull. A UT1-UTC values
+#   - step back one day to the record that has "I", i.e. measured data.
+#
+# the date of this record is the last date with IERS measured data.
+#   [the more recent the date, the more accurate/reliable are both the past IERS
+#   Earth Orientation Parameters as well as the future (predicted) EOP data values.]
+
+# IERS EOP data format definition:
+# https://maia.usno.navy.mil/ser7/readme.finals2000A
+
+        queue = deque(["a", "b", "c", "d"])
+        PredData = False    # True when Prediction data flagged
+        PredEnd  = False    # True when Prediction data no longer flagged
+
+        with open(dfIERS) as file:
+            for line in file:
+                mjd = int(line[7:12])
+
+                if not PredData and mjd >= 51544:    # skip data in previous  millenium
+                    queue.append(line)
+                    queue.popleft()
+                    c1 = line[16:17]    # IERS (I) or Prediction (P) flag for Bull. A polar motion values
+                    c2 = line[57:58]    # IERS (I) or Prediction (P) flag for Bull. A UT1-UTC values
+                    c3 = line[95:96]    # IERS (I) or Prediction (P) flag for Bull. A nutation values
+                    if not PredData and c2 == "P":
+                        PredData = True
+                        iers = ""
+                        while queue:
+                            iersdata = queue.pop()
+                            if iersdata[57:58] == "I":
+                                iers = iersdata
+                                break
+                        if iers == "": iers = iersdata
+                        year = int(iers[0:2]) + 2000
+                        mth  = int(iers[2:4])
+                        day  = int(iers[4:6])
+                        dt = date(year, mth, day)
+                        config.txtIERSEOP = "IERS Earth Orientation data as of " + dt.strftime("%d-%b-%Y")
+                elif PredData:    # search for end of Prediction data
+                    c2 = line[57:58]    # IERS (I) or Prediction (P) flag for Bull. A UT1-UTC values
+                    if c2 == "P":
+                        iers = line
+                    else:
+                        PredEnd = True
+                        break
+
+        # detect end of Prediction data even if file ends with c2 == "P" ...
+        year = int(iers[0:2]) + 2000
+        mth  = int(iers[2:4])
+        day  = int(iers[4:6])
+        dt2 = date(year, mth, day)
+        config.endIERSEOP = "IERS Earth Orientation predictions end " + dt2.strftime("%d-%b-%Y")
+        config.dt_IERSEOP = dt2
+
     if config.ephndx in set([0, 1, 2, 3, 4]):
     
         eph = load(config.ephemeris[config.ephndx][0])	# load chosen ephemeris
         earth   = eph['earth']
         moon    = eph['moon']
         sun     = eph['sun']
         venus   = eph['venus']
@@ -340,15 +426,15 @@
     msg = "rise_set {} values for {}: {}".format(len(y),lats, y[0])
     if len(y) > 1:
         msg = msg + " {}".format(y[1])
     if len(y) > 2:
         msg = msg + " {}".format(y[2])
     if len(y) > 3:
         msg = msg + " {}".format(y[3])
-    dt = t0.utc_datetime() + datetime.timedelta(seconds = t0.dut1)
+    dt = t0.utc_datetime() + timedelta(seconds = t0.dut1)
 
     if config.logfileopen:
         # write to log file
         config.writeLOG("\n{}".format(dt.isoformat()))
         config.writeLOG("   " + msg)
     else:
         # print to console
@@ -392,16 +478,16 @@
 def sunSD(d):               # used in sunmoontab(m)
     # compute semi-diameter of sun and sun's declination change per hour (in minutes)
     t00 = ts.ut1(d.year, d.month, d.day, 0, 0, 0)
     #t12 = ts.ut1(d.year, d.month, d.day, 12, 0, 0)
     position = earth.at(t00).observe(sun)
     distance = position.apparent().radec(epoch='date')[2]
     dist_km = distance.km
-# OLD:  sds = math.degrees(math.atan(695500.0 / dist_km))   # radius of sun = 695500 km
-    sds = math.degrees(math.atan(695700.0 / dist_km))   # volumetric mean radius of sun = 695700 km
+# OLD:  sds = degrees(atan(695500.0 / dist_km))   # radius of sun = 695500 km
+    sds = degrees(atan(695700.0 / dist_km))   # volumetric mean radius of sun = 695700 km
     sdsm = "{:0.1f}".format(sds * 60)   # convert to minutes of arc
 
     t0 = ts.ut1(d.year, d.month, d.day, 0, 0, 0)
     position0 = earth.at(t0).observe(sun)
     dec0 = position0.apparent().radec(epoch='date')[1]
     t1= ts.ut1(d.year, d.month, d.day, 1, 0, 0)
     position1 = earth.at(t1).observe(sun)
@@ -413,16 +499,16 @@
 def moonSD(d):              # used in sunmoontab(m)
     # compute semi-diameter of moon (in minutes)
     t00 = ts.ut1(d.year, d.month, d.day, 0, 0, 0)
     #t12 = ts.ut1(d.year, d.month, d.day, 12, 0, 0)
     position = earth.at(t00).observe(moon)
     distance = position.apparent().radec(epoch='date')[2]
     dist_km = distance.km
-# OLD: sdm = math.degrees(math.atan(1738.1/dist_km))   # equatorial radius of moon = 1738.1 km
-    sdm = math.degrees(math.atan(1737.4/dist_km))   # volumetric mean radius of moon = 1737.4 km
+# OLD: sdm = degrees(atan(1738.1/dist_km))   # equatorial radius of moon = 1738.1 km
+    sdm = degrees(atan(1737.4/dist_km))   # volumetric mean radius of moon = 1737.4 km
     sdmm = "{:0.1f}".format(sdm * 60)  # convert to minutes of arc
     return sdmm
 
 def moonGHA(d, round2seconds = False):  # used in sunmoontab(m) & equationtab (in eventtables.py)
     # compute moon's GHA, DEC and HP per hour of day
     t = ts.ut1(d.year, d.month, d.day, hour_of_day, 0, 0)
     position = earth.at(t).observe(moon)
@@ -458,16 +544,16 @@
 ##        if raIDL > 24: raIDL = raIDL - 24
         GHAupper[i] = gha2deg(t[i].gast, ra.hours[i])   # GHA as float
         GHAlower[i] = GHAcolong(GHAupper[i])
         gham[i] = fmtgha(t[i].gast, ra.hours[i])
         decm[i] = fmtdeg(dec.degrees[i],2)
         degm[i] = dec.degrees[i]
         dist_km = distance.km[i]
-# OLD:  HP = math.degrees(math.atan(6378.0/dist_km))	# radius of earth = 6378.0 km
-        HP = math.degrees(math.atan(6371.0/dist_km))	# volumetric mean radius of earth = 6371.0 km
+# OLD:  HP = degrees(atan(6378.0/dist_km))	# radius of earth = 6378.0 km
+        HP = degrees(atan(6371.0/dist_km))	# volumetric mean radius of earth = 6371.0 km
         HPm[i] = "{:0.1f}'".format(HP * 60)     # convert to minutes of arc
 
     # degm has been added for the sunmoontab function
     # GHAupper is an array of GHA per hour as float
     # ghaSoD, ghaEoD = GHA at Start/End of Day as time is rounded to hh:mm (or hh:mm:ss)
 
     return gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD
@@ -683,87 +769,87 @@
     #min = tup[-2] + int(round(tup[-1]/60+0.00001))
     min = int(round((trans - hr) * 60))
     if min == 60:
         min = 0
         hr += 1
         if hr == 24:
             hr = 0
-    time = '{:02d}:{:02d}'.format(hr,min)
-    return time
+    ttime = '{:02d}:{:02d}'.format(hr,min)
+    return ttime
     
 def planetstransit(d, round2seconds = False):      # used in starstab & meridiantab (in eventtables.py)
     # returns SHA and Meridian Passage for the navigational planets
-    d1 = d + datetime.timedelta(days=1)
+    d1 = d + timedelta(days=1)
     
 # Venus
     t0 = ts.ut1(d.year, d.month, d.day, 0, 0, 0)
     position0 = earth.at(t0).observe(venus)
     ra0 = position0.apparent().radec(epoch='date')[0]	# RA
     vau = position0.apparent().radec(epoch='date')[2]	# distance
     vsha = fmtgha(0, ra0.hours)
-    hpvenus = "{:0.1f}".format((math.tan(6371/(vau.au*149597870.7)))*60*180/math.pi)
+    hpvenus = "{:0.1f}".format((tan(6371/(vau.au*149597870.7)))*60*180/pi)
 
     # calculate planet transit
     tfr = t0
     tto = ts.ut1(d1.year, d1.month, d1.day, 0, 0, 0)
     position = earth.at(tfr).observe(venus)
     ra = position.apparent().radec(epoch='date')[0]
     #print('Venus transit: ', tfr.gast, ra.hours)
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     transit_time, y = almanac.find_discrete(tfr, tto, planet_transit(venus))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     #if len(transit_time) != 1:
     #    print('returned %s values' %len(transit_time))
     vtrans = rise_set(transit_time,y,u'Venus   0{} E transit'.format(degree_sign),round2seconds)[0]
 
 # Mars
     position0 = earth.at(t0).observe(mars)
     ra0 = position0.apparent().radec(epoch='date')[0]	# RA
     mau = position0.apparent().radec(epoch='date')[2]	# distance
     marssha = fmtgha(0, ra0.hours)
-    hpmars = "{:0.1f}".format((math.tan(6371/(mau.au*149597870.7)))*60*180/math.pi)
+    hpmars = "{:0.1f}".format((tan(6371/(mau.au*149597870.7)))*60*180/pi)
 
     # calculate planet transit
     tfr = t0
     tto = ts.ut1(d1.year, d1.month, d1.day, 0, 0, 0)
     position = earth.at(tfr).observe(mars)
     ra = position.apparent().radec(epoch='date')[0]
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     transit_time, y = almanac.find_discrete(tfr, tto, planet_transit(mars))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     marstrans = rise_set(transit_time,y,u'Mars    0{} E transit'.format(degree_sign),round2seconds)[0]
 
 # Jupiter
     position0 = earth.at(t0).observe(jupiter)
     ra0 = position0.apparent().radec(epoch='date')[0]	# RA
     jsha = fmtgha(0, ra0.hours)
 
     # calculate planet transit
     tfr = t0
     tto = ts.ut1(d1.year, d1.month, d1.day, 0, 0, 0)
     position = earth.at(tfr).observe(jupiter)
     ra = position.apparent().radec(epoch='date')[0]
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     transit_time, y = almanac.find_discrete(tfr, tto, planet_transit(jupiter))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     jtrans = rise_set(transit_time,y,u'Jupiter 0{} E transit'.format(degree_sign),round2seconds)[0]
     
 # Saturn
     position0 = earth.at(t0).observe(saturn)
     ra0 = position0.apparent().radec(epoch='date')[0]	# RA
     satsha = fmtgha(0, ra0.hours)
 
     # calculate planet transit
     tfr = t0
     tto = ts.ut1(d1.year, d1.month, d1.day, 0, 0, 0)
     position = earth.at(tfr).observe(saturn)
     ra = position.apparent().radec(epoch='date')[0]
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     transit_time, y = almanac.find_discrete(tfr, tto, planet_transit(saturn))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     sattrans = rise_set(transit_time,y,u'Saturn  0{} E transit'.format(degree_sign),round2seconds)[0]
     
     return [vsha,vtrans,marssha,marstrans,jsha,jtrans,satsha,sattrans,hpmars,hpvenus]
 
 def planet_transit(planet_name):
     # Build a function of time that returns a planet's upper transit time.
 
@@ -883,50 +969,50 @@
     # naut. and civil twilight (before sunrise), sunrise, meridian passage, sunset, civil and nautical twilight (after sunset).
     # NOTE: 'twilight' is only called for every third day in the Full Almanac...
     #       ...therefore daily tracking of the sun state is not possible.
 
     out = [0,0,0,0,0,0]
     lats = "{:3.1f} {}".format(abs(lat), hemisph)
     locn = Topos(lats, "0.0 E")
-    dt = datetime.datetime(d.year, d.month, d.day, 0, 0, 0)
+    dt = datetime(d.year, d.month, d.day, 0, 0, 0)
 
     if round2seconds:
-        dt -= datetime.timedelta(seconds=0.5)      # search from 0.5 seconds before midnight
+        dt -= timedelta(seconds=0.5)      # search from 0.5 seconds before midnight
     else:
-        dt -= datetime.timedelta(seconds=30)       # search from 30 seconds before midnight
+        dt -= timedelta(seconds=30)       # search from 30 seconds before midnight
 
     t0 = ts.ut1(dt.year, dt.month, dt.day,   dt.hour, dt.minute, dt.second)
     t1 = ts.ut1(dt.year, dt.month, dt.day+1, dt.hour, dt.minute, dt.second)
     abhd = False                                # above/below horizon display NOT enabled
 
     # Sunrise/Sunset...
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     actual, y = almanac.find_discrete(t0, t1, daylength(locn, 0.8333))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     out[2], out[3], r2, s2, fs = rise_set(actual,y,lats,round2seconds)
     if out[2] == '--:--' and out[3] == '--:--':	# if neither sunrise nor sunset...
         abhd = True                             # enable above/below horizon display
         yn = midnightsun(d, hemisph)
         out[2] = yn
         out[3] = yn
 
     # Civil Twilight...
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     civil, y = almanac.find_discrete(t0, t1, daylength(locn, 6.0))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     out[1], out[4], r2, s2, fs = rise_set(civil,y,lats,round2seconds)
     if abhd and out[1] == '--:--' and out[4] == '--:--':	# if neither begin nor end...
         yn = midnightsun(d, hemisph)
         out[1] = yn
         out[4] = yn
 
     # Nautical Twilight...
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     naut, y = almanac.find_discrete(t0, t1, daylength(locn, 12.0))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     out[0], out[5], r2, s2, fs = rise_set(naut,y,lats,round2seconds)
     if abhd and out[0] == '--:--' and out[5] == '--:--':	# if neither begin nor end...
         yn = midnightsun(d, hemisph)
         out[0] = yn
         out[5] = yn
     
     return out
@@ -992,16 +1078,16 @@
 
 def getHorizon(t):
     # calculate the angle of the moon below the horizon at moonrise/set
 
     position = earth.at(t).observe(moon)   # at noontime (for daily average distance)
     distance = position.apparent().radec(epoch='date')[2]
     dist_km = distance.km
-# OLD: sdm = math.degrees(math.atan(1738.1/dist_km))   # equatorial radius of moon = 1738.1 km
-    sdm = math.degrees(math.atan(1737.4/dist_km))   # volumetric mean radius of moon = 1737.4 km
+# OLD: sdm = degrees(atan(1738.1/dist_km))   # equatorial radius of moon = 1738.1 km
+    sdm = degrees(atan(1737.4/dist_km))   # volumetric mean radius of moon = 1737.4 km
     horizon = sdm + 0.5666667	# moon's equatorial radius + 34' (atmospheric refraction)
 
     return horizon
 
 def fetchMoonData(d, tFrom, tNoon, tTo, i, lats, hFlag = False, round2seconds=False):
     # calculate & store moon data (rise/set times) or fetch data if pre-calculated.
     # --- THIS IMPROVES PERFORMANCE BY AVOIDING DUPLICATE COSTLY CALCULATIONS AS ---
@@ -1038,17 +1124,17 @@
             np_array[ndx][k][1] = b''
 
     # check the transient data store...
     if round2seconds or len(np_array[ndx][i-1][0]) == 0:     # no data stored - calculate new values
 
         locn = Topos(lats, "0.0 E")
         horizon = getHorizon(tNoon)
-        start00 = time.time()                   # 00000
+        start00 = Time.time()                   # 00000
         moonrise, y = almanac.find_discrete(tFrom, tTo, moonday(locn, horizon))
-        time00 = time.time()-start00 # 00000
+        time00 = Time.time()-start00 # 00000
         rise, sett, ris2, set2, fs = rise_set(moonrise,y,lats,round2seconds)
 
         # only store single events (not double events, which are very rare)
         if ris2 == '--:--' and set2 == '--:--':
             # save 'sett' with moon's finalstate (above/below horizon or currently unknown)
             if fs == True:
                 set9 = sett[0:2] + 'n' + sett[3:5]
@@ -1095,29 +1181,29 @@
     # Additionally it also tracks the current state of the moon (above or below horizon)
 
     i = 1 + config.lat.index(lat)   # index 0 is reserved to enable an explicit setting
     out  = ['--:--','--:--','--:--','--:--','--:--','--:--']	# first event
     out2 = ['--:--','--:--','--:--','--:--','--:--','--:--']	# second event on same day (rare)
     lats = "{:3.1f} {}".format(abs(lat), hemisph)
     locn = Topos(lats, "0.0 E")
-    dt = datetime.datetime(d.year, d.month, d.day, 0, 0, 0)
-    dt -= datetime.timedelta(seconds=30)       # search from 30 seconds before midnight
+    dt = datetime(d.year, d.month, d.day, 0, 0, 0)
+    dt -= timedelta(seconds=30)       # search from 30 seconds before midnight
 
-    d9 = d + datetime.timedelta(days=-1)
+    d9 = d + timedelta(days=-1)
     t9 = ts.ut1(dt.year, dt.month, dt.day-1, dt.hour, dt.minute, dt.second)
 
     t0 = ts.ut1(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second)
 
-    d1 = d + datetime.timedelta(days=1)
+    d1 = d + timedelta(days=1)
     t1 = ts.ut1(dt.year, dt.month, dt.day+1, dt.hour, dt.minute, dt.second)
 
-    d2 = d + datetime.timedelta(days=2)
+    d2 = d + timedelta(days=2)
     t2 = ts.ut1(dt.year, dt.month, dt.day+2, dt.hour, dt.minute, dt.second)
 
-    d3 = d + datetime.timedelta(days=3)
+    d3 = d + timedelta(days=3)
     t3 = ts.ut1(dt.year, dt.month, dt.day+3, dt.hour, dt.minute, dt.second)
 
     t4 = ts.ut1(dt.year, dt.month, dt.day+4, dt.hour, dt.minute, dt.second)
 
     # get the angle of the moon below the horizon at noontime (for daily average distance)
     t9noon = ts.ut1(dt.year, dt.month, dt.day, dt.hour-12, dt.minute, dt.second)
     t0noon = ts.ut1(dt.year, dt.month, dt.day, dt.hour+12, dt.minute, dt.second)
@@ -1164,15 +1250,15 @@
 
     if fs != None:
         moonvisible[i] = fs
 
     if out[1] == '--:--' and out[4] == '--:--':	# if neither moonrise nor moonset...
         config.moonDataSeeks -= 1
         if moonvisible[i] == None:
-            getmoonstate(dt+datetime.timedelta(days=1), lat, hemisph)    # ...get moon state if unknown
+            getmoonstate(dt+timedelta(days=1), lat, hemisph)    # ...get moon state if unknown
         out[1] = moonstate(i)
         out[4] = moonstate(i)
 
     if out[1] == '--:--' and out[4] != '--:--':	# if moonset but no moonrise...
         out[1] = moonset_no_rise(d1, lat, d, t0, t0noon, t1, d2, t2, t2noon, t3, i, lats)
 
     if out[1] != '--:--' and out[4] == '--:--':	# if moonrise but no moonset...
@@ -1190,15 +1276,15 @@
 
     if fs != None:
         moonvisible[i] = fs
 
     if out[2] == '--:--' and out[5] == '--:--':	# if neither moonrise nor moonset...
         config.moonDataSeeks -= 1
         if moonvisible[i] == None:
-            getmoonstate(dt+datetime.timedelta(days=2), lat, hemisph)    # ...get moon state if unknown
+            getmoonstate(dt+timedelta(days=2), lat, hemisph)    # ...get moon state if unknown
         out[2] = moonstate(i)
         out[5] = moonstate(i)
 
     if out[2] == '--:--' and out[5] != '--:--':	# if moonset but no moonrise...
         out[2] = moonset_no_rise(d2, lat, d1, t1, t1noon, t2, d3, t3, t3noon, t4, i, lats)
 
     if out[2] != '--:--' and out[5] == '--:--':	# if moonrise but no moonset...
@@ -1249,60 +1335,60 @@
     locn = Topos(lats, '0.0 E')
     t0 = ts.ut1(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second)
     horizon = 0.8333
 
     # search for the next moonrise or moonset (returned in moonrise[0] and y[0])
     while moonvisible[i] == None:
         t0 = ts.ut1(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second)
-        dt += datetime.timedelta(days=1)
+        dt += timedelta(days=1)
         t9 = ts.ut1(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second)
-        start00 = time.time()                   # 00000
+        start00 = Time.time()                   # 00000
         moonrise, y = almanac.find_discrete(t0, t9, moonday(locn, horizon))
-        config.stopwatch2 += time.time()-start00 # 00000
+        config.stopwatch2 += Time.time()-start00 # 00000
 #        for n in range(len(moonrise)):
 #            print(y[n], moonrise[n].utc_datetime())
         if len(moonrise) > 0:
 #            print()
             if y[0]:
                 moonvisible[i] = False
             else:
                 moonvisible[i] = True
 
     return
 
-def moonset_no_rise(date, lat, prday, t9, t9noon, t0, nxday, t1, t1noon, t2, i, lats, round2seconds=False):
+def moonset_no_rise(Date, lat, prday, t9, t9noon, t0, nxday, t1, t1noon, t2, i, lats, round2seconds=False):
     # if moonset but no moonrise...
     msg = ""
     n = seek_moonrise(prday, t9, t9noon, t0, nxday, t1, t1noon, t2, i, lats, round2seconds)
     if n == 1:
         out = moonstate(i)       # moonrise "below horizon"
         msg = "below horizon (start)"
     if n == -1:
         #print("UP")
         moonvisible[0] = True
         out = moonstate(0)       # moonrise "above horizon"
         msg = "above horizon (end)"
         #print(out[0])
-    #if msg != "": print("no moonrise on {} at lat {} => {}".format(date.strftime("%Y-%m-%d"), lat, msg))
+    #if msg != "": print("no moonrise on {} at lat {} => {}".format(Date.strftime("%Y-%m-%d"), lat, msg))
     if n == 0:
         out = r'''\raisebox{0.24ex}{\boldmath$\cdot\cdot$~\boldmath$\cdot\cdot$}'''
     return out
 
-def moonrise_no_set(date, lat, prday, t9, t9noon, t0, nxday, t1, t1noon, t2, i, lats, round2seconds=False):
+def moonrise_no_set(Date, lat, prday, t9, t9noon, t0, nxday, t1, t1noon, t2, i, lats, round2seconds=False):
     # if moonrise but no moonset...
     msg = ""
     n = seek_moonset(prday, t9, t9noon, t0, nxday, t1, t1noon, t2, i, lats, round2seconds)
     if n == 1:
         out = moonstate(i)       # moonset "above horizon"
         msg = "above horizon (start)"
     if n == -1:
         moonvisible[0] = False
         out = moonstate(0)       # moonset "below horizon"
         msg = "below horizon (end)"
-    #if msg != "": print("no moonset on  {} at lat {} => {}".format(date.strftime("%Y-%m-%d"), lat, msg))
+    #if msg != "": print("no moonset on  {} at lat {} => {}".format(Date.strftime("%Y-%m-%d"), lat, msg))
     if n == 0:
         out = r'''\raisebox{0.24ex}{\boldmath$\cdot\cdot$~\boldmath$\cdot\cdot$}'''
     return out
 
 def seek_moonset(prday, t9, t9noon, t0, nxday, t1, t1noon, t2, i, lats, round2seconds=False):
     # for the specified date & latitude ...
     # return -1 if there is NO MOONSET yesterday
@@ -1360,23 +1446,23 @@
 
     i = 1 + config.lat.index(lat)   # index 0 is reserved to enable an explicit setting
     out  = ['--:--','--:--']	# first event
     out2 = ['--:--','--:--']	# second event on same day (rare)
 
     lats = "{:3.1f} {}".format(abs(lat), hemisph)
     locn = Topos(lats, "0.0 E")
-    dt = datetime.datetime(d.year, d.month, d.day, 0, 0, 0)
-    dt -= datetime.timedelta(seconds=0.5)   # search from 0.5 seconds before midnight
+    dt = datetime(d.year, d.month, d.day, 0, 0, 0)
+    dt -= timedelta(seconds=0.5)   # search from 0.5 seconds before midnight
 
-    d9 = d + datetime.timedelta(days=-1)
+    d9 = d + timedelta(days=-1)
     t9 = ts.ut1(dt.year, dt.month, dt.day-1, dt.hour, dt.minute, dt.second)
 
     t0 = ts.ut1(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second)
 
-    d1 = d + datetime.timedelta(days=1)
+    d1 = d + timedelta(days=1)
     t1 = ts.ut1(dt.year, dt.month, dt.day+1, dt.hour, dt.minute, dt.second)
 
     t2 = ts.ut1(dt.year, dt.month, dt.day+2, dt.hour, dt.minute, dt.second)
 
     t9noon = ts.ut1(dt.year, dt.month, dt.day, dt.hour-12, dt.minute, dt.second)
     t0noon = ts.ut1(dt.year, dt.month, dt.day, dt.hour+12, dt.minute, dt.second)
     t1noon = ts.ut1(dt.year, dt.month, dt.day+1, dt.hour+12, dt.minute, dt.second)
@@ -1677,17 +1763,17 @@
     return transit_time
 
 
 def moonphase(d):           # used in twilighttab (section 3)
     # returns the moon's elongation (angle to the sun)
 
     # convert python 'date' to 'date with time' ...
-    dt = datetime.datetime(d.year, d.month, d.day, 0, 0, 0)
+    dt = datetime(d.year, d.month, d.day, 0, 0, 0)
     # phase is calculated at noon
-    dt += datetime.timedelta(hours=12)
+    dt += timedelta(hours=12)
 
     t00 = ts.ut1(d.year, d.month, d.day, 0, 0, 0)
     #t12 = ts.ut1(d.year, d.month, d.day, 12, 0, 0)
     phase_angle = almanac.phase_angle(eph, 'moon', t00)     # OLD: t12
     elong = phase_angle.radians
 
     # phase_angle.degrees is ...
@@ -1695,37 +1781,37 @@
     
     #pnm = PreviousNewMoon.replace(tzinfo=None)
     #nfm = NextFullMoon.replace(tzinfo=None)
     #pfm = PreviousFullMoon.replace(tzinfo=None)
     #nnm = NextNewMoon.replace(tzinfo=None)
 
     if WaxingMoon:
-        phase = math.pi - phase_angle.radians
+        phase = pi - phase_angle.radians
     else:
-        phase = math.pi + phase_angle.radians
+        phase = pi + phase_angle.radians
 
     return phase
 
 def moonage(d, d1):         # used in twilighttab (section 3)
     # return the moon's 'age' and percent illuminated
 
     # percent illumination is calculated at midnight
     t00 = ts.ut1(d.year, d.month, d.day, 0, 0, 0)
     #t12 = ts.ut1(d.year, d.month, d.day, 12, 0, 0)
     phase_angle = almanac.phase_angle(eph, 'moon', t00)     # OLD: t12
-    pctrad = 50 * (1.0 + math.cos(phase_angle.radians))
+    pctrad = 50 * (1.0 + cos(phase_angle.radians))
     pct = "{:.0f}".format(pctrad)
 
     # calculate age of moon
 
     pnm = PreviousNewMoon
     nnm = NextNewMoon
-    #dt0 = datetime.date(pnm.year, pnm.month, pnm.day)
-    #dt1 = datetime.date(nnm.year, nnm.month, nnm.day)
-    dt  = datetime.datetime.combine(d1, datetime.time(0, 0))
+    #dt0 = date(pnm.year, pnm.month, pnm.day)
+    #dt1 = date(nnm.year, nnm.month, nnm.day)
+    dt = datetime.combine(d1, time(0, 0))
     age1td = dt-pnm.replace(tzinfo=None)
     age2td = dt-nnm.replace(tzinfo=None)
     age1 = age1td.days
     age2 = age2td.days
     age = age1
     if age2 >= 0:
         age = age2
@@ -1777,24 +1863,24 @@
         mp_lower = find_transit(d, LowerList, True)
 
     if not(extras):     # omit 'age' and 'pct'
         return eqt00,eqt12,mpa12,mp_upper,mp_lower
 
     # percent illumination is calculated at midnight
     phase_angle = almanac.phase_angle(eph, 'moon', t00)     # OLD: t12
-    pctrad = 50 * (1.0 + math.cos(phase_angle.radians))
+    pctrad = 50 * (1.0 + cos(phase_angle.radians))
     pct = "{:.0f}".format(pctrad)
 
     # calculate age of moon
 
     pnm = PreviousNewMoon
     nnm = NextNewMoon
-    #dt0 = datetime.date(pnm.year, pnm.month, pnm.day)
-    #dt1 = datetime.date(nnm.year, nnm.month, nnm.day)
-    dt  = datetime.datetime.combine(d1, datetime.time(0, 0))
+    #dt0 = date(pnm.year, pnm.month, pnm.day)
+    #dt1 = date(nnm.year, nnm.month, nnm.day)
+    dt = datetime.combine(d1, time(0, 0))
     age1td = dt-pnm.replace(tzinfo=None)
     age2td = dt-nnm.replace(tzinfo=None)
     age1 = age1td.days
     age2 = age2td.days
     age = age1
     if age2 >= 0:
         age = age2
@@ -1875,35 +1961,35 @@
     NextNewMoon      = None
     PreviousFullMoon = None
     NextFullMoon     = None
     WaxingMoon = None
     # note: the python datetimes above are timezone 'aware' (not 'naive')
 
     # search from 30 days earlier than noon... till noon on this day
-    d0 = d - datetime.timedelta(days=30)
+    d0 = d - timedelta(days=30)
     t0 = ts.utc(d0.year, d0.month, d0.day, 12, 0, 0)
     t1 = ts.utc(d.year, d.month, d.day, 12, 0, 0)
-    start00 = time.time()                   # 00000
+    start00 = Time.time()                   # 00000
     t, y = almanac.find_discrete(t0, t1, almanac.moon_phases(eph))
-    config.stopwatch += time.time()-start00 # 00000
+    config.stopwatch += Time.time()-start00 # 00000
     for i in range(len(t)):
         if y[i] == 0:       # 0=New Moon, 1=First Quarter, 2=Full Moon, 3=Last Quarter
             PreviousNewMoon = t[i].utc_datetime()
         if y[i] == 2:       # 2 = Full Moon
             PreviousFullMoon = t[i].utc_datetime()
     # note: if two PreviousNewMoons are found within the range, the last is stored
     # note: if two PreviousFullMoons are found within the range, the last is stored
 
     if PreviousNewMoon != None and PreviousFullMoon != None:
         # synodic month = about 29.53 days
-        t2 = ts.utc(PreviousNewMoon + datetime.timedelta(days=28))
-        t3 = ts.utc(PreviousNewMoon + datetime.timedelta(days=30))
-        start00 = time.time()                   # 00000
+        t2 = ts.utc(PreviousNewMoon + timedelta(days=28))
+        t3 = ts.utc(PreviousNewMoon + timedelta(days=30))
+        start00 = Time.time()                   # 00000
         t, y = almanac.find_discrete(t2, t3, almanac.moon_phases(eph))
-        config.stopwatch += time.time()-start00 # 00000
+        config.stopwatch += Time.time()-start00 # 00000
         for i in range(len(t)):
             if y[i] == 0:       # 0 = New Moon
                 NextNewMoon = t[i].utc_datetime()
 
         WaxingMoon = True
         if PreviousFullMoon > PreviousNewMoon:
             WaxingMoon = False
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/config.py` & `sfalmanac-1.9/sfalmanac/lib/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # ================ EDIT LINES IN THIS SECTION ONLY ================
 
 # choose an ephemeris (ephndx = 0, 1, 2, 3 or 4):
 #   0   de421.bsp   1900 to 2050
@@ -55,17 +55,23 @@
 # --------------------------------------------------------------
 
 # global variables initialized during main program startup (and on every spawned process)
 CPUcores = 1        # CPU core count
 WINpf = False       # system platform
 LINUXpf = False     # system platform
 MACOSpf = False     # system platform
+FANCYhd = False     # 'True' if compatible with 'fancyhdr' package
+DPonly = False      # output data pages only
 
 # define global variables
 logfileopen = False
+useIERSEOP = False
+txtIERSEOP = ""     # footer text (using 'fancyhdr')
+endIERSEOP = ""     # footer text (using 'fancyhdr')
+dt_IERSEOP = None
 ephemeris = [['de421.bsp',1900,2050],['de405.bsp',1600,2200],['de406.bsp',1000,2750],['de430t.bsp',1550,2650],['de440.bsp',1550,2650]]
 tbls = ''		# table style (global variable)
 decf = ''		# Declination format (global variable)
 stopwatch = 0.0     # time spent in a section of code
 stopwatch2 = 0.0    # time spent in a section of code
 moonDaysCount = 0   # count of days processed by moonrise_set (alma_skyfield.py)
 moonDataSeeks = 0   # count of moon daily data seeks
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/eventtables.py` & `sfalmanac-1.9/sfalmanac/lib/eventtables.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # NOTE: the new format statement requires a literal '{' to be entered as '{{',
 #       and a literal '}' to be entered as '}}'. The old '%' format specifier
 #       will be removed from Python at some later time. See:
 # https://docs.python.org/3/whatsnew/3.0.html#pep-3101-a-new-approach-to-string-formatting
 
 ###### Standard library imports ######
-from datetime import datetime, timedelta
+# don't confuse the 'date' method with the 'Date' variable!
+from datetime import date, datetime, timedelta
 import sys			# required for .stdout.write()
 import signal       # for init_worker
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 if config.MULTIpr:      # in multi-processing mode ...
     # ------------------------------------------------------
     # EITHER comment next 2 lines out to invoke executor.map
     MPmode = 0
     import multiprocessing as mp
     #  *OR*  comment next 2 lines out to invoke pool.map
 ##    MPmode = 1
@@ -98,66 +99,66 @@
     dbl = False
     for i in range(len(m1)):
         if m2[i] != '--:--':
             dbl = True
     return dbl
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def mp_twilight_worker(date, ts, spad, lat):
+def mp_twilight_worker(Date, ts, spad, lat):
     #print(" mp_twilight_worker Start {}".format(lat))
     hemisph = 'N' if lat >= 0 else 'S'
-    twi = mp_twilight(date, lat, hemisph, ts, spad, True) # ===>>> mp_eventtables.py
+    twi = mp_twilight(Date, lat, hemisph, ts, spad, True) # ===>>> mp_eventtables.py
     #print(" mp_twilight_worker Finish {}".format(lat))
     return twi      # return list for all latitudes
 
-def mp_moonlight_worker(date, ts, spad, lat):
+def mp_moonlight_worker(Date, ts, spad, lat):
     #print(" mp_moonlight_worker Start  {}".format(lat))
     hemisph = 'N' if lat >= 0 else 'S'
-    ml = mp_moonrise_set(date, lat, hemisph, ts, spad)    # ===>>> mp_eventtables.py
+    ml = mp_moonrise_set(Date, lat, hemisph, ts, spad)    # ===>>> mp_eventtables.py
     #print(" mp_moonlight_worker Finish {}".format(lat))
     return ml       # return list for all latitudes
 
-def twilighttab(date, ts, spad):
+def twilighttab(Date, ts, spad):
     # returns the twilight and moonrise tables
 
     if config.MULTIpr:
         # multiprocess twilight values per latitude simultaneously
         if MPmode == 0:      # with pool.map
-            partial_func = partial(mp_twilight_worker, date, ts, spad)
+            partial_func = partial(mp_twilight_worker, Date, ts, spad)
 
             try:
                 # RECOMMENDED: chunksize = 1
                 listoftwi = pool.map(partial_func, config.lat, 1)
             except KeyboardInterrupt:
                 print(msg0)
                 sys.exit(0)
 
         if MPmode == 1:      # with executor.map
-            partial_func = partial(mp_twilight_worker, date, ts, spad)
+            partial_func = partial(mp_twilight_worker, Date, ts, spad)
             future_value = executor.map(partial_func, config.lat)
             listoftwi = list(future_value)
 
         for k in range(len(listoftwi)):
             config.stopwatch += listoftwi[k][6]     # accumulate multiprocess processing time
             del listoftwi[k][-1]
         #print("listoftwi = {}".format(listoftwi))
 
         # multiprocess moonrise/moonset values per latitude simultaneously
         if MPmode == 0:      # with pool.map
-            partial_func2 = partial(mp_moonlight_worker, date, ts, spad)
+            partial_func2 = partial(mp_moonlight_worker, Date, ts, spad)
 
             try:
                 # RECOMMENDED: chunksize = 1
                 listmoon = pool.map(partial_func2, config.lat, 1)
             except KeyboardInterrupt:
                 print(msg0)
                 sys.exit(0)
 
         if MPmode == 1:      # with executor.map
-            partial_func2 = partial(mp_moonlight_worker, date, ts, spad)
+            partial_func2 = partial(mp_moonlight_worker, Date, ts, spad)
             future_val = executor.map(partial_func2, config.lat)
             listmoon = list(future_val)
 
         for k in range(len(listmoon)):
             tuple_times = listmoon[k][-1]
             config.stopwatch  += tuple_times[0]         # accumulate multiprocess processing time
             config.stopwatch2 += tuple_times[1]         # accumulate multiprocess processing time
@@ -168,15 +169,15 @@
     #lat = [72,70,68,66,64,62,60,58,56,54,52,50,45,40,35,30,20,10,0, -10,-20,-30,-35,-40,-45,-50,-52,-54,-56,-58,-60]
     latNS = [72, 70, 58, 40, 10, -10, -50, -60]
 #    tab = r'''\begin{tabular*}{0.72\textwidth}[t]{@{\extracolsep{\fill}}|r|ccc|ccc|cc|}
     tab = r'''\begin{tabular}[t]{|r|ccc|ccc|cc|}
 %%%\multicolumn{9}{c}{\normalsize{}}\\
 '''
 
-    ondate = date.strftime("%d %B %Y")
+    ondate = Date.strftime("%d %B %Y")
     tab = tab + r'''\hline
 \multicolumn{{9}}{{|c|}}{{\rule{{0pt}}{{2.4ex}}{{\textbf{{{}}}}}}}\\
 '''.format(ondate)
 
     tab = tab + r'''\hline
 \multicolumn{1}{|c|}{\rule{0pt}{2.4ex}\multirow{2}{*}{\textbf{Lat.}}} & 
 \multicolumn{2}{c}{\textbf{Twilight}} & 
@@ -209,16 +210,16 @@
         lasthemisph = hemisph
 
         if config.MULTIpr:
             twi = listoftwi[j-5]
             moon = listmoon[j-5][0]
             moon2 = listmoon[j-5][1]
         else:
-            twi = twilight(date, lat, hemisph, True)
-            moon, moon2 = moonrise_set2(date, lat, hemisph)
+            twi = twilight(Date, lat, hemisph, True)
+            moon, moon2 = moonrise_set2(Date, lat, hemisph)
 
         if not(double_events_found(moon,moon2)):
             line = r'''\textbf{{{}}}'''.format(hs) + r''' {}$^\circ$'''.format(abs(lat))
             line = line + r''' & {} & {} & {} & {} & {} & {} & {} & {} \\
 '''.format(twi[0],twi[1],twi[2],twi[3],twi[4],twi[5],moon[0],moon[1])
         else:
             # print a row with two moonrise/moonset events on the same day & latitude
@@ -254,29 +255,29 @@
     tab = tab + r'''\hline\multicolumn{9}{c}{}\\
 '''
     tab = tab + r'''\end{tabular}
 '''
     return tab
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def mp_planets_worker(date, ts, spad, obj):
+def mp_planets_worker(Date, ts, spad, obj):
     #print(" mp_planets_worker Start  {}".format(obj))
-    sha = mp_planetstransit(date, ts, spad, obj, True)    # ===>>> mp_eventtables.py
+    sha = mp_planetstransit(Date, ts, spad, obj, True)    # ===>>> mp_eventtables.py
     #print(" mp_planets_worker Finish {}".format(obj))
     return sha      # return list for four planets
 
-def meridiantab(date, ts, spad):
+def meridiantab(Date, ts, spad):
     # returns a table with ephemerides for the navigational stars
     # LaTeX SPACING: \enskip \quad \qquad
 
     if config.MULTIpr and config.WINpf and MPmode == 0:
         # multiprocess 'SHA + transit times' simultaneously
         objlist = ['venus', 'mars', 'jupiter', 'saturn']
         # set constant values to all arguments which are not changed during parallel processing
-        partial_func2 = partial(mp_planets_worker, date, ts, spad)
+        partial_func2 = partial(mp_planets_worker, Date, ts, spad)
 
         try:
             listofsha = pool.map(partial_func2, objlist, 1)     # RECOMMENDED: chunksize = 1
         except KeyboardInterrupt:
             print(msg0)
             sys.exit(0)
 
@@ -287,25 +288,25 @@
 
     out = r'''\quad
 \begin{tabular*}{0.25\textwidth}[t]{@{\extracolsep{\fill}}|rrr|}
 %%%\multicolumn{3}{c}{\normalsize{}}\\
 '''
     m = ""
     # returns a table with SHA & Mer.pass for Venus, Mars, Jupiter and Saturn
-    datestr = r'''{} {}'''.format(date.strftime("%b"), date.strftime("%d"))
+    datestr = r'''{} {}'''.format(Date.strftime("%b"), Date.strftime("%d"))
     m = m + r'''\hline
 & & \multicolumn{{1}}{{r|}}{{}}\\[-2.0ex]
 \textbf{{{}}} & \textbf{{SHA}} & \textbf{{Mer.pass}}\\
 \hline\multicolumn{{3}}{{|r|}}{{}}\\[-2.0ex]
 '''.format(datestr)
 
     if config.MULTIpr and config.WINpf and MPmode == 0:
         p = [item for sublist in listofsha for item in sublist]
     else:
-        p = planetstransit(date, True)
+        p = planetstransit(Date, True)
 
     m = m + r'''Venus & {} & {} \\
 '''.format(p[0],p[1])
     m = m + r'''Mars & {} & {} \\
 '''.format(p[2],p[3])
     m = m + r'''Jupiter & {} & {} \\
 '''.format(p[4],p[5])
@@ -317,18 +318,18 @@
 
     out = out + r'''\end{tabular*}
 \par    % put next table below here
 '''
     return out
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def equationtab(date, dpp):
-    # returns the Equation of Time section for 'date' and 'date+1'
+def equationtab(Date, dpp):
+    # returns the Equation of Time section for 'Date' and 'Date+1'
 
-    d = date
+    d = Date
     # first create the UpperLists & LowerLists arrays ...
     nn = 0
     while nn < dpp:
         gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD = moonGHA(d, True)
 
         buildUPlists2(nn, ghaSoD, GHAupper, ghaEoD)
         buildLOWlists2(nn, ghaSoD, GHAupper, ghaEoD)
@@ -342,60 +343,83 @@
 \multicolumn{3}{c|}{\textbf{Sun}} & \multicolumn{3}{c|}{\textbf{Moon}}\\
 \multicolumn{1}{|c|}{} & \multicolumn{2}{c}{Eqn.of Time} & \multicolumn{1}{|c|}{Mer.} & \multicolumn{2}{c}{Mer.Pass.} & \multicolumn{1}{|c|}{}\\
 \multicolumn{1}{|c|}{} & \multicolumn{1}{c}{00\textsuperscript{h}} & \multicolumn{1}{c}{12\textsuperscript{h}} & \multicolumn{1}{|c|}{Pass} & \multicolumn{1}{c}{Upper} & \multicolumn{1}{c}{Lower} &\multicolumn{1}{|c|}{Age}\\
 \multicolumn{1}{|c|}{} & \multicolumn{1}{c}{mm:ss} & \multicolumn{1}{c}{mm:ss} & \multicolumn{1}{|c|}{hh:mm:ss} & \multicolumn{1}{c}{hh:mm:ss} & \multicolumn{1}{c}{hh:mm:ss} &\multicolumn{1}{|c|}{}\\
 \cline{1-7}\rule{0pt}{3.0ex}\noindent
 '''
 
-    d = date
+    d = Date
     for k in range(dpp):
         eq = equation_of_time(d,d + timedelta(days=1),UpperLists[k],LowerLists[k],True,True)
         tab = tab + r'''{} & {} & {} & {} & {} & {} & {}({}\%) \\
 '''.format(d.strftime("%d"),eq[0],eq[1],eq[2],eq[3],eq[4],eq[5],eq[6])
         d += timedelta(days=1)
 
     tab = tab + r'''\cline{1-7}
 \end{tabular}'''
     return tab
 
 #----------------------
 #   page preparation
 #----------------------
 
-def page(date, ts, dpp, spad):
+def page(Date, ts, dpp, spad):
 
     # time delta values for the initial date&time...
-    dut1, deltat = getDUT1(date)
+    dut1, deltat = getDUT1(Date)
     timeDUT1 = r"DUT1 = UT1-UTC = {:+.4f} sec\quad$\Delta$T = TT-UT1 = {:+.4f} sec".format(dut1, deltat)
 
-    find_new_moon(date)     # required for 'moonage' and 'equation_of_time"
+    Lfoot_IERSEOP = ""
+    if config.dt_IERSEOP != None:
+        # the IERS EOP data start date is 2nd January 1973
+        if Date + timedelta(days=1) >= date(1973, 1, 2):
+            Lfoot_IERSEOP = config.txtIERSEOP
+        if Date + timedelta(days=1) >= config.dt_IERSEOP:
+            Lfoot_IERSEOP = config.endIERSEOP
+        if Date > config.dt_IERSEOP:
+            Lfoot_IERSEOP = r'''\textbf{No IERS EOP prediction data available}'''
+
+    find_new_moon(Date)     # required for 'moonage' and 'equation_of_time"
     #leftindent = ""
     #rightindent = ""
 
     if dpp > 1:
-        str2 = r'''\textbf{{{} to {} UT}}'''.format(date.strftime("%Y %B %d"),(date+timedelta(days=dpp-1)).strftime("%b. %d"))
+        str2 = r'''\textbf{{{} to {} UT}}'''.format(Date.strftime("%Y %B %d"),(Date+timedelta(days=dpp-1)).strftime("%b. %d"))
     else:
-        str2 = r'''\textbf{{{} UT}}'''.format(date.strftime("%Y %B %d"))
+        str2 = r'''\textbf{{{} UT}}'''.format(Date.strftime("%Y %B %d"))
 
-    page = r'''
+    if config.FANCYhd:
+        page = r'''
 % ------------------ N E W   P A G E ------------------
 \newpage
 \sffamily
-\lhead{{\noindent\textsf{{\footnotesize{{{}}}}}}}
+\lhead{{\textsf{{\footnotesize{{{}}}}}}}
 \rhead{{\textsf{{\textbf{{{}}}}}}}
+\lfoot{{\textsf{{\footnotesize{{{}}}}}}}
+\begin{{scriptsize}}
+'''.format(timeDUT1, str2, Lfoot_IERSEOP)
+    else:   # old formatting
+        page = r'''
+% ------------------ N E W   P A G E ------------------
+\newpage
+\sffamily
+\noindent
+\begin{{flushleft}}     % required so that \par works
+{{\footnotesize {}}}\hfill{}
+\end{{flushleft}}\par
 \begin{{scriptsize}}
 '''.format(timeDUT1, str2)
 
-    date2 = date+timedelta(days=1)
-    page += twilighttab(date,ts,spad)
-    page += meridiantab(date,ts,spad)
+    Date2 = Date+timedelta(days=1)
+    page += twilighttab(Date,ts,spad)
+    page += meridiantab(Date,ts,spad)
     if dpp == 2:
-        page += twilighttab(date2,ts,spad)
-        page += meridiantab(date2,ts,spad)
-    page += equationtab(date,dpp)
+        page += twilighttab(Date2,ts,spad)
+        page += meridiantab(Date2,ts,spad)
+    page += equationtab(Date,dpp)
 
     # to avoid "Overfull \hbox" messages, leave a paragraph end before the end of a size change. (This may only apply to tabular* table style) See lines below...
     page = page + r'''
 
 \end{scriptsize}'''
     return page
 
@@ -444,14 +468,15 @@
                 pmth = cmth
             else:
                 sys.stdout.write('.')	# progress indicator
                 sys.stdout.flush()
             out += page(day1,ts,dpp,spad)
             day1 += timedelta(days=2)
             year = day1.year
+
     elif dtp == -1:     # if entire month
         mth = first_day.month
         m = mth
         while mth == m:
             cmth = day1.strftime("%b ")
             day2 = day1 + timedelta(days=1)
             if day2.month != m:
@@ -465,14 +490,15 @@
                 pmth = cmth
             else:
                 sys.stdout.write('.')	# progress indicator
                 sys.stdout.flush()
             out += page(day1,ts,dpp,spad)
             day1 += timedelta(days=2)
             mth = day1.month
+
     else:           # print 'dtp' days beginning with first_day
         i = dtp   # don't decrement dtp
         while i > 0:
             if i < 2: dpp = i
             out += page(day1,ts,dpp,spad)
             i -= 2
             day1 += timedelta(days=2)
@@ -490,150 +516,314 @@
     return out
 
 #--------------------------
 #   external entry point
 #--------------------------
 
 def makeEVtables(first_day, dtp, ts, spad, df180, df360):
+    # make tables starting from first_day
     # dtp = 0 if for entire year; = -1 if for entire month; else days to print
 
+    if config.FANCYhd:
+        return makeEVnew(first_day, dtp, ts, spad, df180, df360) # use the 'fancyhdr' package
+    else:
+        return makeEVold(first_day, dtp, ts, spad, df180, df360) # use old formatting
+
+#   The following functions are intentionally separate functions.
+#   'makeEVold' is required for TeX Live 2019, which is the standard
+#   version in Ubuntu 20.04 LTS which expires in April 2030.
+
+def hdrEVnew(first_day, dtp, vsep1, vsep2, df180, df360):
+    # build the front page
+
+    tex = r'''
+    \begin{titlepage}
+    \begin{center}
+    \textsc{\Large Generated using Skyfield}\\
+    \large http://rhodesmill.org/skyfield/\\[0.7cm]'''
+
+    if config.dockerized:   # DOCKER ONLY
+        df180 = "../A4chart0-180_P.pdf"
+        df360 = "../A4chart180-360_P.pdf"
+
+    tex += r'''
+    % TRIM values: left bottom right top
+    \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\[0.3cm]
+    \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\'''.format(df180,df360)
+
+    tex += r'''[{}]
+    \textsc{{\huge Event Time Tables}}\\[{}]'''.format(vsep1,vsep2)
+
+    if dtp == 0:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(first_day.year)
+    elif dtp == -1:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(first_day.strftime("%B %Y"))
+    elif dtp > 1:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdates(first_day,first_day+timedelta(days=dtp-1)))
+    else:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdate(first_day))
+
+    tex += r'''
+    \begin{center}\begin{tabular}[t]{rl}
+    \large\emph{Author:} & \large Andrew \textsc{Bauer}\\
+    \end{tabular}\end{center}'''
+
+    tex += r'''
+    {\large \today}
+    \HRule \\[0.2cm]
+    \end{center}
+    \begin{description}[leftmargin=5.5em,style=nextline]\footnotesize
+    \item[Disclaimer:] These are computer generated tables. They focus on times of rising and setting events and are rounded to the second (not primarily intended for navigation). Meridian Passage times of the sun, moon and four planets are included. All times are in UT (=UT1).
+    The author claims no liability for any consequences arising from use of these tables.
+    \end{description}
+\end{titlepage}'''
+
+    return tex
+
+def makeEVnew(first_day, dtp, ts, spad, df180, df360):
     # make tables starting from first_day
-    year = first_day.year
-    mth = first_day.month
-    day = first_day.day
+    # dtp = 0 if for entire year; = -1 if for entire month; else days to print
 
     # page size specific parameters
     # NOTE: 'bm' (bottom margin) is an unrealistic value used only to determine the vertical size of 'body' (textheight), which must be large enough to include all the tables. 'tm' (top margin) and 'hs' (headsep) determine the top of body. Finally use 'fs' (footskip) to position the footer.
     if config.pgsz == "A4":
         # A4 ... pay attention to the limited page width
         paper = "a4paper"
         # title page...
         vsep1 = "1.5cm"
         vsep2 = "1.0cm"
         tm1 = "21mm"
         bm1 = "15mm"
         lm1 = "10mm"
         rm1 = "10mm"
         # data pages...
-        tm = "34.5mm"       # was "21mm" [v2q]
-        bm = "10mm"         # was "18mm" [v2q]
+        tm = "26.6mm"       # was "21mm" [v2q]
+        bm = "18mm"         # was "18mm" [v2q]
         hs = "2.6pt"        # headsep  (page 3 onwards) [v2q]
-        fs = "36pt"         # footskip (page 3 onwards) [v2q]
+        fs = "15pt"         # footskip (page 3 onwards) [v2q]
         lm = "16mm"
         rm = "16mm"
     else:
         # LETTER ... pay attention to the limited page height
         paper = "letterpaper"
         # title page...
         vsep1 = "0.8cm"
         vsep2 = "0.7cm"
         tm1 = "12mm"
         bm1 = "15mm"
         lm1 = "12mm"
         rm1 = "12mm"
         # data pages...
-        tm = "25.7mm"       # was "12.2mm" [v2q]
-        bm = "9.5mm"        # was "13mm"
+        tm = "17.8mm"       # was "12.2mm" [v2q]
+        bm = "17mm"         # was "13mm"
         hs = "2.6pt"        # headsep  (page 3 onwards) [v2q]
-        fs = "28pt"         # footskip (page 3 onwards) [v2q]
+        fs = "15pt"         # footskip (page 3 onwards) [v2q]
         lm = "15mm"
         rm = "11mm"
 
     # default is 'oneside'...
-    alm = r'''\documentclass[10pt, {}]{{report}}'''.format(paper)
+    tex = r'''\documentclass[10pt, {}]{{report}}'''.format(paper)
 
-    alm = alm + r'''
+    tex += r'''
 %\usepackage[utf8]{inputenc}
 \usepackage[english]{babel}
 \usepackage{fontenc}
 \usepackage{enumitem} % used to customize the {description} environment'''
 
     # to troubleshoot add "showframe, verbose," below:
-    alm = alm + r'''
-\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}
-\setlength{{\headsep}}{{{}}} % [v2q]'''.format(tm,bm,lm,rm,hs)
+    tex += r'''
+\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm1,bm1,lm1,rm1)
+
+    # define page styles
+    # CAUTION: putting '\fancyhf{}' in frontpage style also clears the footer in page2!
+    tex += r'''
+%------------ page styles ------------
+\usepackage{fancyhdr}
+\renewcommand{\headrulewidth}{0pt}
+\renewcommand{\footrulewidth}{0pt}
+\fancypagestyle{frontpage}{
+}
+\fancypagestyle{page2}[frontpage]{
+  \fancyfootoffset[R]{0pt}% recalculate \headwidth
+  \lfoot{\textsf{\footnotesize{https://thenauticalalmanac.com/}}}
+  \cfoot{\centerline{Page \thepage}}
+}
+\fancypagestyle{datapage}[page2]{'''
+    tex += r'''
+  \newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}, headsep={}, footskip={}}}'''.format(tm,bm,lm,rm,hs,fs)
+    tex += r'''
+  \rfoot{\textsf{\footnotesize{https://pypi.org/project/sfalmanac/}}}
+} %-----------------------------------'''
 
     # Note: \DeclareUnicodeCharacter is not compatible with some versions of pdflatex
-    alm = alm + r'''
+    tex += r'''
 \usepackage{xcolor}  % highlight double moon events on same day
 \definecolor{khaki}{rgb}{0.76, 0.69, 0.57}
 \usepackage{multirow}
 \newcommand{\HRule}{\rule{\linewidth}{0.5mm}}
-\usepackage{fancyhdr}   % [v2q]
-\pagestyle{fancy}       % [v2q]
-\renewcommand{\headrulewidth}{0pt}  % [v2q]
-\setlength{\footskip}{15pt}
 \usepackage[pdftex]{graphicx}	% for \includegraphics
 \usepackage{tikz}				% for \draw  (load after 'graphicx')
 %\showboxbreadth=50  % use for logging
 %\showboxdepth=50    % use for logging
 %\DeclareUnicodeCharacter{00B0}{\ensuremath{{}^\circ}}
 \setlength\fboxsep{1.5pt}       % ONLY used by \colorbox in alma_skyfield.py
-\begin{document}'''
+\begin{document}
+\pagestyle{frontpage}'''
+
+    if not config.DPonly:
+        tex += hdrEVnew(first_day,dtp,vsep1,vsep2,df180,df360)
+
+    tex += r'''
+\pagestyle{datapage}  % page style for data pages'''
+
+    tex += pages(first_day,dtp,ts,spad)
+    tex += r'''
+\end{document}'''
+    return tex
+
+# ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===
+# ===   ===   ===   ===   O L D   F O R M A T T I N G   ===   ===   ===   ===
+# ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===
 
-    alm = alm + r'''
+def hdrEVold(first_day, dtp, tm1, bm1, lm1, rm1, vsep1, vsep2, df180, df360):
+    # build the front page
+
+    tex = r'''
 % for the title page only...
 \newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}}}'''.format(tm1,bm1,lm1,rm1)
 
-    alm = alm + r'''
+    tex += r'''
     \begin{titlepage}
     \begin{center}
     \textsc{\Large Generated using Skyfield}\\
     \large http://rhodesmill.org/skyfield/\\[0.7cm]'''
 
     if config.dockerized:   # DOCKER ONLY
         df180 = "../A4chart0-180_P.pdf"
         df360 = "../A4chart180-360_P.pdf"
 
-    alm = alm + r'''
+    tex += r'''
     % TRIM values: left bottom right top
     \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\[0.3cm]
     \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\'''.format(df180,df360)
 
-    alm = alm + r'''[{}]
+    tex += r'''[{}]
     \textsc{{\huge Event Time Tables}}\\[{}]'''.format(vsep1,vsep2)
 
     if dtp == 0:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
-    \HRule \\'''.format(year)
+    \HRule \\'''.format(first_day.year)
     elif dtp == -1:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
     \HRule \\'''.format(first_day.strftime("%B %Y"))
     elif dtp > 1:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
     \HRule \\'''.format(fmtdates(first_day,first_day+timedelta(days=dtp-1)))
     else:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
     \HRule \\'''.format(fmtdate(first_day))
 
-    alm = alm + r'''
+    tex += r'''
     \begin{center}\begin{tabular}[t]{rl}
     \large\emph{Author:} & \large Andrew \textsc{Bauer}\\
     \end{tabular}\end{center}'''
 
-    alm = alm + r'''
+    tex += r'''
     {\large \today}
     \HRule \\[0.2cm]
     \end{center}
     \begin{description}[leftmargin=5.5em,style=nextline]\footnotesize
     \item[Disclaimer:] These are computer generated tables. They focus on times of rising and setting events and are rounded to the second (not primarily intended for navigation). Meridian Passage times of the sun, moon and four planets are included. All times are in UT (=UT1).
     The author claims no liability for any consequences arising from use of these tables.
     \end{description}
 \end{titlepage}
-% DO NOT SPECIFY lfoot, cfoot & rfoot BEFORE restoregeometry!
-\restoregeometry    % so it does not affect the rest of the pages
-\lfoot{\textsf{\footnotesize{https://thenauticalalmanac.com/}}}
-\cfoot{\centerline{Page \thepage}}
-\rfoot{\textsf{\footnotesize{https://pypi.org/project/sfalmanac/}}}'''
+\restoregeometry    % so it does not affect the rest of the pages'''
+
+    return tex
+
+def makeEVold(first_day, dtp, ts, spad, df180, df360):
+    # make tables starting from first_day
+    # dtp = 0 if for entire year; = -1 if for entire month; else days to print
+
+    # page size specific parameters
+    if config.pgsz == "A4":
+        # pay attention to the limited page width
+        paper = "a4paper"
+        vsep1 = "1.5cm"
+        vsep2 = "1.0cm"
+        tm1 = "21mm"    # title page...
+        bm1 = "15mm"
+        lm1 = "10mm"
+        rm1 = "10mm"
+        tm = "21mm"     # data pages...
+        bm = "18mm"
+        lm = "16mm"
+        rm = "16mm"
+    else:
+        # pay attention to the limited page height
+        paper = "letterpaper"
+        vsep1 = "0.8cm"
+        vsep2 = "0.7cm"
+        tm1 = "12mm"    # title page...
+        bm1 = "15mm"
+        lm1 = "12mm"
+        rm1 = "12mm"
+        tm = "12.2mm"   # data pages...
+        bm = "13mm"
+        lm = "15mm"
+        rm = "11mm"
+
+    # default is 'oneside'...
+    tex = r'''\documentclass[10pt, {}]{{report}}'''.format(paper)
+
+    tex += r'''
+%\usepackage[utf8]{inputenc}
+\usepackage[english]{babel}
+\usepackage{fontenc}
+\usepackage{enumitem} % used to customize the {description} environment'''
+
+    # to troubleshoot add "showframe, verbose," below:
+    tex += r'''
+\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm,bm,lm,rm)
+
+    # Note: \DeclareUnicodeCharacter is not compatible with some versions of pdflatex
+    tex += r'''
+\usepackage{xcolor}  % highlight double moon events on same day
+\definecolor{khaki}{rgb}{0.76, 0.69, 0.57}
+\usepackage{multirow}
+\newcommand{\HRule}{\rule{\linewidth}{0.5mm}}
+\setlength{\footskip}{15pt}
+\usepackage[pdftex]{graphicx}	% for \includegraphics
+\usepackage{tikz}				% for \draw  (load after 'graphicx')
+%\showboxbreadth=50  % use for logging
+%\showboxdepth=50    % use for logging
+%\DeclareUnicodeCharacter{00B0}{\ensuremath{{}^\circ}}
+\setlength\fboxsep{1.5pt}       % ONLY used by \colorbox in alma_skyfield.py
+\begin{document}'''
+
+    if not config.DPonly:
+        tex += hdrEVold(first_day,dtp,tm1,bm1,lm1,rm1,vsep1,vsep2,df180,df360)
 
-    alm = alm + pages(first_day,dtp,ts,spad)
-    alm = alm + '''
+    tex += pages(first_day,dtp,ts,spad)
+    tex += r'''
 \end{document}'''
-    return alm
+    return tex
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/increments.py` & `sfalmanac-1.9/sfalmanac/lib/increments.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 
 #   Copyright (C) 2014  Enno Rodegerdts
+#   Copyright (C) 2022  Andrew Bauer
 
-#  This program is free software; you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation; either version 2 of the License, or
-#     (at your option) any later version.
-# 
-#     This program is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-# 
-#     You should have received a copy of the GNU General Public License along
-#     with this program; if not, write to the Free Software Foundation, Inc.,
-#     51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+#   This program is free software; you can redistribute it and/or modify
+#   it under the terms of the GNU General Public License as published by
+#   the Free Software Foundation; either version 2 of the License, or
+#   (at your option) any later version.
+#
+#   This program is distributed in the hope that it will be useful,
+#   but WITHOUT ANY WARRANTY; without even the implied warranty of
+#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#   GNU General Public License for more details.
+#
+#   You should have received a copy of the GNU General Public License along
+#   with this program; if not, write to the Free Software Foundation, Inc.,
+#   51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 ###### Standard library imports ######
 import os
 import sys
-from math import pi as pi
-from math import cos as cos
-from math import tan as tan
-from math import sqrt as sqrt
+from math import pi, cos, tan, sqrt
+
+###### Local application imports ######
+from sfalmanac.lib import config
 
 def degmin(deg):
     #changes decimal degrees to the format usually used in the nautical almanac. (ddd°mm.m')
     theminus = ""
     if deg < 0:
         theminus = "-"
     deg = abs(deg)
@@ -39,270 +40,313 @@
         mf -= 60
         di += 1
         if di == 360:
             di = 0
     gm = "{}{}$^\circ${:04.1f}".format(theminus,di,mf)
     return gm
 
-def decdeg(d,min):
-	# returns decimal degrees from deg. and min.
-	d=d*1.0
-	min=min*1.0
-	deg=d+(min/60)
-	return deg
+def decdeg(d,mmm):
+    # returns decimal degrees from deg. and min.
+    d=d*1.0
+    mmm=mmm*1.0
+    deg=d+(mmm/60)
+    return deg
 	
-def rad(d,min):
-	#returns radiands from deg. and min.
-	rad=decdeg(d,min)/180*pi
-	return rad
+def rad(d,mmm):
+    #returns radians from deg. and min.
+    rad=decdeg(d,mmm)/180*pi
+    return rad
 
 def suninc(m,s):
-	# returns the increment for the sun.
-	min=m*1.0
-	sec=s/60.0
-	hour=(sec+min)/60
-	inc=degmin(15*hour)
-	return inc
+    # returns the increment for the sun.
+    mmm=m*1.0
+    sec=s/60.0
+    hour=(sec+mmm)/60
+    inc=degmin(15*hour)
+    return inc
 
 def ariesinc(m,s):
-	# returns the increment for aries
-	min= m*1.0
-	sec=s/60.0
-	hour=(sec+min)/60
-	inc=degmin(decdeg(15,2.46)*hour)
-	return inc
+    # returns the increment for aries
+    mmm= m*1.0
+    sec=s/60.0
+    hour=(sec+mmm)/60
+    inc=degmin(decdeg(15,2.46)*hour)
+    return inc
 
 def mooninc(m,s):
-	# returns the increment for the Moon
-	min= m*1.0
-	sec=s/60.0
-	hour=(sec+min)/60
-	inc=degmin(decdeg(14,19.0)*hour)
-	return inc
+    # returns the increment for the Moon
+    mmm= m*1.0
+    sec=s/60.0
+    hour=(sec+mmm)/60
+    inc=degmin(decdeg(14,19.0)*hour)
+    return inc
 	
 def vcorr(m,v):
-	# returns the v correction for a given minute and tabular v.
-	h=(m+0.5)/60.0
-	corr=round(v*h,1)
-	return corr
-
-def inctab(min):
-    """generates a latex table for increments"""
-    tab = r'''\noindent
+    # returns the v correction for a given minute and tabular v.
+    h=(m+0.5)/60.0
+    corr=round(v*h,1)
+    return corr
+
+def inctab(mmm):
+    # generates a latex table for increments
+
+    tab = r'''
+    \noindent
     \begin{tabular*}{0.33\textwidth}[t]{@{\extracolsep{\fill}}|>{\bfseries}p{0.3cm}|>{\hspace{-3pt}}r|>{\hspace{-3pt}}r|>{\hspace{-3pt}}r||>{\hspace{-3pt}}c>{\hspace{-3pt}}c>{\hspace{-3pt}}c<{\hspace{-3pt}}|}
     \hline
     {\tiny m} \textbf{'''
     
-    tab = tab+"{}".format(int(min))
+    tab += "{}".format(int(mmm))
     
-    tab=tab+ r'''} & \multicolumn{1}{p{0.5cm}|}{\textbf{Sun Plan.}} & \multicolumn{1}{c|}{\textbf{Aries}} & \multicolumn{1}{c||}{\textbf{Moon}} & \multicolumn{3}{c|}{\textit{\textbf{v and d corr}}}\\ 
-    \hline'''
+    tab += r'''} & \multicolumn{1}{p{0.5cm}|}{\textbf{Sun Plan.}} & \multicolumn{1}{c|}{\multirow{2}{*}{\textbf{Aries}}} & 
+    \multicolumn{1}{c||}{\multirow{2}{*}{\textbf{Moon}}} & 
+    \multicolumn{3}{c|}{\multirow{2}{*}{\textit{\textbf{v and d corr}}}}\\ 
+    \hline
+'''
    
     sec = 0
     while sec < 60:
-        line = "{} & {} & {} & {} & {} - {} & {} - {} & {} - {} \\\ \n".format(sec,suninc(min,sec),ariesinc(min,sec),mooninc(min,sec),str(round(0.1*sec,1)),vcorr(min,0.1*sec),str(round(6+0.1*sec,1)),vcorr(min,6+0.1*sec),str(round(12+0.1*sec,1)),vcorr(min,12+0.1*sec))
-        tab = tab + line
+        line = "{} & {} & {} & {} & {} - {} & {} - {} & {} - {} \\\ \n".format(sec,suninc(mmm,sec),ariesinc(mmm,sec),mooninc(mmm,sec),str(round(0.1*sec,1)),vcorr(mmm,0.1*sec),str(round(6+0.1*sec,1)),vcorr(mmm,6+0.1*sec),str(round(12+0.1*sec,1)),vcorr(mmm,12+0.1*sec))
+        tab += line
         sec += 1
         
-    tab = tab+r"""\hline \end{tabular*}
-    """
+    tab = tab + r'''\hline \end{tabular*}'''
     return tab
 
-def allinctabs():
-	# iterates throu 60 minutes
-	min=0
-	tab=""
-	while min < 60:
-		tab = tab + inctab(min)
-		min += 1
-	return tab
+def allinctabs(colsep):
+    tab = ""
+    if colsep != "":
+        # change tabcolsep just for the inctabs
+        tab += r'''
+\newlength{{\oldtabcolsep}}
+\setlength{{\oldtabcolsep}}{{\tabcolsep}}
+\setlength{{\tabcolsep}}{{{}}}'''.format(colsep)
+
+    # iterates through 60 minutes
+    mmm=0
+    while mmm < 60:
+        tab += inctab(mmm)
+        mmm += 1
+
+    if colsep != "":
+        # reset tabcolsep to the previous value (= 6.0pt)
+        tab += r'''
+\setlength{\tabcolsep}{\oldtabcolsep}'''
+
+    return tab
 
 def dip(meter):
-	dip=60*0.0293*sqrt(meter)
-	return dip
+    dip=60*0.0293*sqrt(meter)
+    return dip
 
 def diptab():
-	meter=1
-	tab = r'''\noindent 
-	\begin{tabular}[t]{|c c c|} 
-	\multicolumn{3}{c}{\textbf{DIP}}\\
-	\hline 
-	\textit{m} & \textit{dip} & \textit{ft}\\ 
-	\hline
-	'''
-	while meter < 25.5:
-		line = "{} &  {:.1f} & {:.1f}\\\ \n".format(meter, dip(meter), meter/0.3084)
-		tab = tab + line
-		meter += 0.5
-	tab = tab + r"""\hline
-	\end{tabular}
-	"""
-	
-	return tab
+    meter=1
+    tab = r'''\noindent 
+    \begin{tabular}[t]{|c c c|} 
+    \multicolumn{3}{c}{\textbf{DIP}}\\
+    \hline 
+    \textit{m} & \textit{dip} & \textit{ft}\\ 
+    \hline
+'''
+    while meter < 25.5:
+        line = "{} &  {:.1f} & {:.1f}\\\ \n".format(meter, dip(meter), meter/0.3084)
+        tab = tab + line
+        meter += 0.5
+    tab = tab + r'''\hline
+    \end{tabular}
+'''
+
+    return tab
 
 def refrac(h):
-	r = 1/tan((h+7.31/(h+4.4))/180*pi)
-	return r
+    r = 1/tan((h+7.31/(h+4.4))/180*pi)
+    return r
 
 def refractab():
-	ho=5
-	tab = r'''\noindent 
-	\begin{tabular}[t]{|c c|} 
-	\multicolumn{2}{c}{\textbf{Refract.}}\\
-	\hline 
-	\textit{$H_{a}$} & \textit{ref} \\ 
-	\hline
-	'''
-	while ho < 20:
-		line = "{}$^\circ$ &  {:.1f}\\\ \n".format(ho, refrac(ho))
-		tab = tab + line
-		ho += 0.5
-	while ho < 40:
-		line = "{}$^\circ$ &  {:.1f}\\\ \n".format(ho, refrac(ho))
-		tab = tab + line
-		ho += 1
-	while ho < 90:
-		line = "{}$^\circ$ &  {:.1f}\\\ \n".format(ho, refrac(ho))
-		tab = tab + line
-		ho += 5
-	tab = tab + r"""\hline
-	\end{tabular}
-	"""
-	return tab
-
-def parallax(hp, deg, min):
-	#returns parallax in dec minutes from horizontal parallax, and Ha
-	p = rad(0, hp) * cos(rad(deg, min)) * 180/pi *60
-	return p 
+    ho=5
+    tab = r'''
+    \noindent 
+    \begin{tabular}[t]{|c c|} 
+    \multicolumn{2}{c}{\textbf{Refract.}}\\
+    \hline 
+    \textit{$H_{a}$} & \textit{ref} \\ 
+    \hline
+'''
+    while ho < 20:
+        line = "{}$^\circ$ &  {:.1f}\\\ \n".format(ho, refrac(ho))
+        tab = tab + line
+        ho += 0.5
+    while ho < 40:
+        line = "{}$^\circ$ &  {:.1f}\\\ \n".format(ho, refrac(ho))
+        tab = tab + line
+        ho += 1
+    while ho < 90:
+        line = "{}$^\circ$ &  {:.1f}\\\ \n".format(ho, refrac(ho))
+        tab = tab + line
+        ho += 5
+    tab = tab + r'''\hline
+    \end{tabular}
+'''
+    return tab
+
+def parallax(hp, deg, mmm):
+    #returns parallax in dec minutes from horizontal parallax, and Ha
+    p = rad(0, hp) * cos(rad(deg, mmm)) * 180/pi *60
+    return p 
 	
 def parallaxtab():
-	Hdeg=0 
-	
-	HP=54.0
-	tab = r'''\noindent 
-	\begin{tabular}[t]{|c|rrrrrrrrrrrrrrrrrr|}
-	\multicolumn{19}{c}{\textbf{Parallax of the Moon}}\\
-	\hline
-	'''
-	d = 0
-	line = r"\textbf{$H_{a}$} "
-	while d<90:
-		line += r"& \multicolumn{{1}}{{>{{\hspace{{-4pt}}}}c<{{\hspace{{-4pt}}}}|}}{{\textbf{{{}-{}$^\circ$}}}}".format(d, d+5)
-		d+= 5
-	line += " \\\ \n \\hline"
-	tab += line
-	
-	while Hdeg < 5 :
-		#line = " \u0027 "        # DOCKER ONLY
-		line = " $'$ "
-		dd = Hdeg
-		while dd < 90:
-			line += r"& \multicolumn{{1}}{{l}}{{\textbf{{{}$^\circ$}}}}".format(dd)
-			dd += 5
-		line += "\\vline \\\ \n"
-		tab = tab + line
-		Hmin=0
-		while Hmin < 60:
-			dd = Hdeg
-			line = r"\textbf{{{}}} ".format(Hmin)
-			while dd < 90:
-				line += " & {:.1f} ".format(parallax(HP,dd,Hmin))
-				dd += 5
-			line += "\\\ \n"
-			tab = tab + line
-			Hmin += 10	
-		Hdeg += 1
-		
-	tab += r"""\hline 
+    Hdeg=0 
+
+    HP=54.0
+    tab = r'''\noindent 
+    \begin{tabular}[t]{|c|rrrrrrrrrrrrrrrrrr|}
+    \multicolumn{19}{c}{\textbf{Parallax of the Moon}}\\
+    \hline
+'''
+    d = 0
+    line = r"\textbf{$H_{a}$} "
+    while d<90:
+        line += r"& \multicolumn{{1}}{{>{{\hspace{{-4pt}}}}c<{{\hspace{{-4pt}}}}|}}{{\textbf{{{}-{}$^\circ$}}}}".format(d, d+5)
+        d+= 5
+    line += " \\\ \n \\hline"
+    tab += line
+
+    while Hdeg < 5 :
+        #line = " \u0027 "        # DOCKER ONLY
+        line = " $'$ "
+        dd = Hdeg
+        while dd < 90:
+            line += r"& \multicolumn{{1}}{{l}}{{\textbf{{{}$^\circ$}}}}".format(dd)
+            dd += 5
+        line += "\\vline \\\ \n"
+        tab = tab + line
+        Hmin=0
+        while Hmin < 60:
+            dd = Hdeg
+            line = r"\textbf{{{}}} ".format(Hmin)
+            while dd < 90:
+                line += " & {:.1f} ".format(parallax(HP,dd,Hmin))
+                dd += 5
+            line += "\\\ \n"
+            tab = tab + line
+            Hmin += 10	
+        Hdeg += 1
+
+    tab += r'''\hline 
 	\multicolumn{1}{|c|}{\textbf{HP}} & \multicolumn{18}{c|}{correction for HP per column}\\
 	\hline
-	"""
-	hp = 54.3
-	while hp<61.5:
-		line = r"\textbf{{ {:.1f}}} ".format(hp)
-		d = 2
-		while d<90:
-			line += "& {:.1f} ".format(parallax(hp, d, 30) - parallax(54, d, 30))
-			d += 5
-		line += "\\\ \n"
-		tab += line
-		hp += 0.3
-			
-		
-	tab = tab + r"""\hline
-	\end{tabular}
-	"""
-	return tab
+'''
+    hp = 54.3
+    while hp<61.5:
+        line = r"\textbf{{ {:.1f}}} ".format(hp)
+        d = 2
+        while d<90:
+            line += "& {:.1f} ".format(parallax(hp, d, 30) - parallax(54, d, 30))
+            d += 5
+        line += "\\\ \n"
+        tab += line
+        hp += 0.3
 	
+
+    tab = tab + r'''\hline
+    \end{tabular}
+'''
+    return tab
+
 def venparallax():
-	Hdeg=10 
-	
-	tab = r'''\noindent 
-	\begin{tabular}[t]{|c|cccccc|}
-	\multicolumn{7}{c}{\textbf{Parallax of Venus and Mars}}\\
-	'''
-	tab += r"""\hline 
-	$H_{a}$ HP & \textbf{.1$'$} & \textbf{.2$'$} & \textbf{.3$'$} & \textbf{.4$'$} & \textbf{.5$'$} & \textbf{.6$'$} \\
-	\hline
-	"""
-	while Hdeg<90:
-		hp = 0.1
-		line = r"\textbf{{ {}$^\circ$}} ".format(Hdeg)
-		while hp < 0.7:
-			line += "& {:.1f} ".format(parallax(hp, Hdeg, 0))
-			hp += 0.1
-		line += "\\\ \n"
-		tab += line
-		Hdeg += 10		
-	tab = tab + r"""\hline
-	\end{tabular}
-	"""
-	return tab
+    Hdeg=10 
+
+    tab = r'''\noindent 
+    \begin{tabular}[t]{|c|cccccc|}
+    \multicolumn{7}{c}{\textbf{Parallax of Venus and Mars}}\\
+'''
+    tab += r'''\hline 
+    $H_{a}$ HP & \textbf{.1$'$} & \textbf{.2$'$} & \textbf{.3$'$} & \textbf{.4$'$} & \textbf{.5$'$} & \textbf{.6$'$} \\
+    \hline
+'''
+    while Hdeg<90:
+        hp = 0.1
+        line = r"\textbf{{ {}$^\circ$}} ".format(Hdeg)
+        while hp < 0.7:
+            line += "& {:.1f} ".format(parallax(hp, Hdeg, 0))
+            hp += 0.1
+        line += "\\\ \n"
+        tab += line
+        Hdeg += 10		
+    tab = tab + r'''\hline
+    \end{tabular}
+'''
+    return tab
 
 #--------------------------
 #   external entry point
 #--------------------------
 
 def makelatex():
-	lx = r"""\documentclass[ 10pt, a4paper]{scrreprt}
-	\usepackage[automark]{scrlayer-scrpage}
-	\pagestyle{scrheadings}
-	\clearpairofpagestyles
-	\chead{\large \textbf{Increments and Corrections}}
+
+    if config.pgsz == "A4":
+        # A4 ... pay attention to the limited page width
+        paper = "a4paper"
+        tm = "15mm"
+        bm = "15mm"
+        lm = "8mm"
+        rm = "8mm"
+        colsep = ""
+    else:
+        # LETTER ... pay attention to the limited page height
+        paper = "letterpaper"
+        tm = "15mm"
+        bm = "15mm"
+        lm = "8mm"
+        rm = "8mm"
+        colsep = "5pt"
+
+    lx = r'''\documentclass[10pt, {}]{{scrreprt}}'''.format(paper)
+
+    lx += r'''
+    \usepackage[automark]{scrlayer-scrpage}
+    \pagestyle{scrheadings}
+    \clearpairofpagestyles
+    \chead{\large \textbf{Increments and Corrections}}
     %\usepackage[utf8]{inputenc}
     \usepackage[english]{babel}
     \usepackage{fontenc}
     %\usepackage{upquote}
-    \usepackage{array, multicol, blindtext}
-    \usepackage[landscape,headsep=0mm, headheight=5mm, top=15mm, bottom=15mm, left=8mm, right=8mm]{geometry}
-	\newcommand{\HRule}{\rule{\linewidth}{0.9mm}}
-	\usepackage[pdftex]{graphicx}
+    \usepackage{multirow}
+    \usepackage{array, multicol, blindtext}'''
+
+    lx += r'''
+    \usepackage[landscape,headsep=0mm, headheight=5mm, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm,bm,lm,rm)
+
+    lx += r'''
+    \newcommand{\HRule}{\rule{\linewidth}{0.9mm}}
+    \usepackage[pdftex]{graphicx}
     %\DeclareUnicodeCharacter{00B0}{\ensuremath{{}^\circ}}
 \begin{document}
 % ----------------------
 % CAUTION: the next 2 lines suppress Overfull \hbox (badness 10000) messages
 \hbadness=10000
 \newcount\hbadness
 % CAUTION: the next 2 lines suppress Overfull \hbox (too wide) messages below 6.5Pt
 \hfuzz=6.5Pt
 \newdimen\hfuzz
 % ----------------------
-\begin{scriptsize}"""
-	lx = lx + allinctabs()
-	lx = lx + refractab()
-	lx = lx + parallaxtab()
-	lx = lx + diptab()
-	lx += r''' \end{scriptsize} \newpage
-	\begin{multicols}{2} \begin{scriptsize}
-	'''
-	lx = lx + venparallax()
-	lx = lx + r'''\end{scriptsize} \newpage
-	\section*{About these tables}
-	The preceding static tables are independent from the year. They differ from the tables found in the official paper versions of the Nautical almanac in two important considerations. 
-\begin{itemize}
+\begin{scriptsize}'''
+    lx += allinctabs(colsep)
+    lx += refractab()
+    lx += parallaxtab()
+    lx += diptab()
+    lx += r''' \end{scriptsize} \newpage
+    \begin{multicols}{2} \begin{scriptsize}
+'''
+    lx += venparallax()
+    lx += r'''\end{scriptsize} \newpage
+    \section*{About these tables}
+    The preceding static tables are independent from the year. They differ from the tables found in the official paper versions of the Nautical almanac in two important considerations. 
+    \begin{itemize}
       \item My tables are not arranged as \textit{critical} tables. So chose the value that fits best to your value and interpolate in the rare cases where this should be necessary.
       \item My tables do not combine multiple corrections as some tables in the paper Nautical Almanac do. Each correction has to be applied separately. 
     \end{itemize}
 All tables that are specific for a year are contained in the Nautical Almanac daily pages for the corresponding year.
 \subsubsection*{Increments}
 The large increment table is is nothing but a linear interpolation between the tabulated values in the daily pages of the Nautical almanac. This table is basically identical with the official one.
 \subsubsection*{DIP}
@@ -327,20 +371,20 @@
 \subsubsection*{Sight reduction}
 Sight reduction tables can be downloaded from the US government's internet pages. Search for HO-229 or HO-249.  These values can also be calculated with two, relatively simple, formulas:
 \[ \sin H_c= \sin L \sin d + \cos L \cos d \cos LHA\]
 and
 \[\cos A = \frac{\sin d - \sin L \sin H_c}{\cos L \cos H_c}\]
 where $A$ is the azimuth angle, $L$ is the latitude, $d$ is the declination and $LHA$ is the local hour angle. The azimuth ($Z_n$) is given by the following rule:
 \begin{itemize}
-      \item if the $LHA$ is greater than $180^\circ$,\quad$Z_n=A$
-      \item if the $LHA$ is less than $180^\circ$,\quad$Z_n = 360^\circ - A$
+    \item if the $LHA$ is greater than $180^\circ$,\quad$Z_n=A$
+    \item if the $LHA$ is less than $180^\circ$,\quad$Z_n = 360^\circ - A$
 \end{itemize}
-
-	\end{multicols} \end{document}'''
-	return lx
+\end{multicols}
+\end{document}'''
+    return lx
 
 #if sys.version_info[0] != 3:
 #    raise Exception("This runs with Python 3")
 
 #fn = "inc"
 #filename = fn + ".tex"
 #outfile = open(filename, mode="w", encoding="utf8")
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/ld_charts.py` & `sfalmanac-1.9/sfalmanac/lib/ld_charts.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # NOTE: the new format statement requires a literal '{' to be entered as '{{',
 #       and a literal '}' to be entered as '}}'. The old '%' format specifier
 #       will be removed from Python at some later time. See:
 # https://docs.python.org/3/whatsnew/3.0.html#pep-3101-a-new-approach-to-string-formatting
 
 ###### Standard library imports ######
 import ephem
 from datetime import datetime, timedelta
 import math
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 import sfalmanac.lib.ld_stardata as ld_stardata
 from sfalmanac.lib.ld_skyfield import sunGHA, moonGHA, venusGHA, marsGHA, jupiterGHA, saturnGHA, ld_planets, ld_stars, getHipparcos
 
 #   My apologies to those who read this . . .
 #   Although use of global variables is frowned upon by the Python community,
 #   I have chosen to employ global variables in this module to reduce the
 #   number of arguments passed to some functions, so that the function
@@ -57,15 +57,15 @@
 PREVobjects = []        # list of LD objects from previous day
 PREVobjColour = []      # list of LD object-colour tuples from previous day
 
 #---------------------------
 #   Module initialization
 #---------------------------
 
-def init_A4(spad, ts, d0=None):
+def init_A4(ts, d0=None):
     # initialize variables for this module
 
     global sf
     if config.pgsz == "A4":
         sf = 1.39               # scale factor (1.39cm to 10 degrees SHA/DEC)
     else:
         sf = 1.31               # scale factor (1.31cm to 10 degrees SHA/DEC)
@@ -2363,19 +2363,18 @@
 """
     return tex
 
 #--------------------------
 #   external entry point
 #--------------------------
 
-# global variables >>> d00, decmin, decmax, PREVobjColour, PREVobjects, shamin, shamax, sharng, t00
-def makeLDcharts(first_day, strat, daystoprocess, outfile, spad, ts, onlystars, quietmode):
+def makeLDcharts(first_day, strat, daystoprocess, outfile, ts, onlystars, quietmode):
 
     global d00, t00, shamin, shamax, sharng, decmin, decmax, PREVobjColour, PREVobjects
-    init_A4(spad, ts, first_day)    # initialize variables
+    init_A4(ts, first_day)    # initialize variables
 
     DEBUG_m2 = False            # 'True' to print each LD object
 
     PREVobjects = []        # list of LD objects from previous day
     PREVobjColour = []      # list of LD object-colour tuples from previous day
 
     d00 = first_day
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/ld_skyfield.py` & `sfalmanac-1.9/sfalmanac/lib/ld_skyfield.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,50 +3,56 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # Skyfield functions for Lunar Distance tables and charts
 
 ###### Standard library imports ######
-import datetime
-import math
+from datetime import date
+from math import atan, degrees, copysign
 import os
 import errno
 import socket
 import sys			# required for .stdout.write()
+import urllib.error # used in 'download_EOP' function
 from urllib.request import urlopen
+from collections import deque
 
 ###### Third party imports ######
 from skyfield import VERSION
 from skyfield.api import Loader
 from skyfield.api import Topos, Star
 from skyfield import almanac
 from skyfield.nutationlib import iau2000b
 from skyfield.data import hipparcos
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 from sfalmanac.lib import ld_stardata
 
 #---------------------------
 #   Module initialization
 #---------------------------
 
+urlIERS = "ftp://ftp.iers.org/products/eop/rapid/standard/"
+urlUSNO = "https://maia.usno.navy.mil/ser7/"        # alternate location
+urlDCIERS = "https://datacenter.iers.org/data/9/"   # alternate location
+
 hour_of_day3 = [0, 12, 24]
 hour_of_day5 = [0, 6, 12, 18, 24]
 hour_of_day = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23]
 next_hour_of_day = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24]
 hour_of_day26 = [-2, -1, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23]
 degree_sign= u'\N{DEGREE SIGN}'
 
@@ -80,31 +86,37 @@
         pass
     return False    # if neither is reachable
 
 # NOTE: the IERS server is unavailable (due to maintenance work in the first 3 weeks, at least, of April 2022)
 #       however, although the USNO server currently works, it was previously down for 2.5 years!
 #       So it is still best to try using the IERS server as first oprion, and USNO as second.
 
-def testIERSserver(filename):
-    url = "ftp://ftp.iers.org/products/eop/rapid/standard/" + filename
+def testServer(filename, url):
     try:
         connection2 = urlopen(url)
     except Exception as e:
         e2 = IOError('cannot download {0} because {1}'.format(url, e))
         e2.__cause__ = None
 #        raise e2
         return False
     return True     # server works
 
-def downloadUSNO(path, filename):
-    sys.stdout.write("Downloading EOP data from USNO...")
+def download_EOP(path, filename, url, loc):
+    # NOTE: the following 'print' statement does not print immediately in Linux!
+    #print("Downloading EOP data from USNO...", end ="")
+    sys.stdout.write("Downloading EOP data from {}...".format(loc))
     sys.stdout.flush()
     filepath = os.path.join(path, filename)
-    url = "https://maia.usno.navy.mil/ser7/" + filename
-    connection = urlopen(url)
+    url += filename
+    try:
+        connection = urlopen(url)
+    except urllib.error.URLError as e:
+        #raise IOError('error getting {0} - {1}'.format(url, e))
+        print('\nError getting {0} - {1}'.format(url, e))
+        sys.exit(0)
     blocksize = 128*1024
 
     # Claim our own unique download filename.
 
     tempbase = tempname = path + filename + '.download'
     flags = getattr(os, 'O_BINARY', 0) | os.O_CREAT | os.O_EXCL | os.O_RDWR
     i = 1
@@ -147,37 +159,107 @@
     sys.stdout.flush()
 
 def ld_init_sf(spad):
     global ts, pandasDF, eph, earth, moon, sun, venus, mars, jupiter, saturn
     load = Loader(spad)         # spad = folder to store the downloaded files
     EOPdf  = "finals2000A.all"  # Earth Orientation Parameters data file
     dfIERS = spad + EOPdf
+    config.useIERSEOP = False
+    config.txtIERSEOP = ""
 
     if config.useIERS:
         if compareVersion(VERSION, "1.31") >= 0:
             if os.path.isfile(dfIERS):
                 if load.days_old(EOPdf) > float(config.ageIERS):
                     if isConnected():
-                        if testIERSserver(EOPdf): load.download(EOPdf)
-                        else: downloadUSNO(spad,EOPdf)
+                        if testServer(EOPdf, urlIERS):  # first try downloading via FTP
+                            load.download(EOPdf)
+                        elif testServer(EOPdf, urlUSNO):# then try the USNO server
+                            download_EOP(spad,EOPdf,urlUSNO,"USNO")
+                        else:   # finally try the IERS datacenter (available in more countries)
+                            download_EOP(spad,EOPdf,urlDCIERS,"IERS datacenter")
                     else: print("NOTE: no Internet connection... using existing '{}'".format(EOPdf))
                 ts = load.timescale(builtin=False)	# timescale object
+                config.useIERSEOP = True
             else:
                 if isConnected():
-                    if testIERSserver(EOPdf): load.download(EOPdf)
-                    else: downloadUSNO(spad,EOPdf)
+                    if testServer(EOPdf, urlIERS):  # first try downloading via FTP
+                        load.download(EOPdf)
+                    elif testServer(EOPdf, urlUSNO):# then try the USNO server
+                        download_EOP(spad,EOPdf,urlUSNO,"USNO")
+                    else:   # finally try the IERS datacenter (available in more countries)
+                        download_EOP(spad,EOPdf,urlDCIERS,"IERS datacenter")
                     ts = load.timescale(builtin=False)	# timescale object
+                    config.useIERSEOP = True
                 else:
                     print("NOTE: no Internet connection... using built-in UT1-tables")
                     ts = load.timescale()	# timescale object with built-in UT1-tables
         else:
             ts = load.timescale()	# timescale object with built-in UT1-tables
     else:
         ts = load.timescale()	# timescale object with built-in UT1-tables
 
+    if config.useIERSEOP and os.path.isfile(dfIERS):
+# get the IERS EOP data "release date" according to these rules:
+#   - begin searching within this millenium (ignoring data from 02 Jan 1973 to 31 Dec 1999)
+#   - halt when the following value is "P", i.e. predicted as opposed to measured:
+#       - flag for Bull. A UT1-UTC values
+#   - step back one day to the record that has "I", i.e. measured data.
+#
+# the date of this record is the last date with IERS measured data.
+#   [the more recent the date, the more accurate/reliable are both the past IERS
+#   Earth Orientation Parameters as well as the future (predicted) EOP data values.]
+
+# IERS EOP data format definition:
+# https://maia.usno.navy.mil/ser7/readme.finals2000A
+
+        queue = deque(["a", "b", "c", "d"])
+        PredData = False    # True when Prediction data flagged
+        PredEnd  = False    # True when Prediction data no longer flagged
+
+        with open(dfIERS) as file:
+            for line in file:
+                mjd = int(line[7:12])
+
+                if not PredData and mjd >= 51544:    # skip data in previous  millenium
+                    queue.append(line)
+                    queue.popleft()
+                    c1 = line[16:17]    # IERS (I) or Prediction (P) flag for Bull. A polar motion values
+                    c2 = line[57:58]    # IERS (I) or Prediction (P) flag for Bull. A UT1-UTC values
+                    c3 = line[95:96]    # IERS (I) or Prediction (P) flag for Bull. A nutation values
+                    if not PredData and c2 == "P":
+                        PredData = True
+                        iers = ""
+                        while queue:
+                            iersdata = queue.pop()
+                            if iersdata[57:58] == "I":
+                                iers = iersdata
+                                break
+                        if iers == "": iers = iersdata
+                        year = int(iers[0:2]) + 2000
+                        mth  = int(iers[2:4])
+                        day  = int(iers[4:6])
+                        dt = date(year, mth, day)
+                        config.txtIERSEOP = "IERS Earth Orientation data as of " + dt.strftime("%d-%b-%Y")
+                elif PredData:    # search for end of Prediction data
+                    c2 = line[57:58]    # IERS (I) or Prediction (P) flag for Bull. A UT1-UTC values
+                    if c2 == "P":
+                        iers = line
+                    else:
+                        PredEnd = True
+                        break
+
+        # detect end of Prediction data even if file ends with c2 == "P" ...
+        year = int(iers[0:2]) + 2000
+        mth  = int(iers[2:4])
+        day  = int(iers[4:6])
+        dt2 = date(year, mth, day)
+        config.endIERSEOP = "IERS Earth Orientation predictions end " + dt2.strftime("%d-%b-%Y")
+        config.dt_IERSEOP = dt2
+
     if config.ephndx in set([0, 1, 2, 3, 4]):
     
         eph = load(config.ephemeris[config.ephndx][0])	# load chosen ephemeris
         earth   = eph['earth']
         moon    = eph['moon']
         sun     = eph['sun']
         venus   = eph['venus']
@@ -269,16 +351,16 @@
 def moon_SD(d):         # used in moontab
     # compute semi-diameter of moon (in minutes)
     t00 = ts.ut1(d.year, d.month, d.day, 0, 0, 0)
     #t12 = ts.ut1(d.year, d.month, d.day, 12, 0, 0)
     position = earth.at(t00).observe(moon)
     distance = position.apparent().radec(epoch='date')[2]
     dist_km = distance.km
-# OLD: sdm = math.degrees(math.atan(1738.1/dist_km))   # equatorial radius of moon = 1738.1 km
-    sdm = math.degrees(math.atan(1737.4/dist_km))   # volumetric mean radius of moon = 1737.4 km
+# OLD: sdm = degrees(atan(1738.1/dist_km))   # equatorial radius of moon = 1738.1 km
+    sdm = degrees(atan(1737.4/dist_km))   # volumetric mean radius of moon = 1737.4 km
     sdmm = "{:0.1f}".format(sdm * 60)  # convert to minutes of arc
     return sdmm
 
 def moon_GHA(d):        # used in moontab
     # compute moon's GHA, DEC and HP per hour of day
     t = ts.ut1(d.year, d.month, d.day, hour_of_day, 0, 0)
     position = earth.at(t).observe(moon)
@@ -307,16 +389,16 @@
 ##        if raIDL > 24: raIDL = raIDL - 24
         GHAupper[i] = gha2deg(t[i].gast, ra.hours[i])   # GHA as float
         GHAlower[i] = GHAcolong(GHAupper[i])
         gham[i] = fmtgha(t[i].gast, ra.hours[i])
         decm[i] = fmtdeg(dec.degrees[i],2)
         degm[i] = dec.degrees[i]
         dist_km = distance.km[i]
-# OLD:  HP = math.degrees(math.atan(6378.0/dist_km))	# radius of earth = 6378.0 km
-        HP = math.degrees(math.atan(6371.0/dist_km))	# volumetric mean radius of earth = 6371.0 km
+# OLD:  HP = degrees(atan(6378.0/dist_km))	# radius of earth = 6378.0 km
+        HP = degrees(atan(6371.0/dist_km))	# volumetric mean radius of earth = 6371.0 km
         HPm[i] = "{:0.1f}'".format(HP * 60)     # convert to minutes of arc
 
     # degm has been added for the sunmoontab function
     # GHAupper is an array of GHA per hour as float
     # ghaSoD, ghaEoD = GHA at Start/End of Day assuming time is rounded to hh:mm
 
     return gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD
@@ -498,15 +580,15 @@
     i = 0
     for hh in [0, 23]:
         t00 = ts.ut1(d.year, d.month, d.day, hh, 0, 0)
         position = earth.at(t00).observe(sun)
         distance = position.apparent().radec(epoch='date')[2]
         dist_km = distance.km
         # volumetric mean radius of sun = 695700 km
-        sds = math.degrees(math.atan(695700.0 / dist_km))
+        sds = degrees(atan(695700.0 / dist_km))
         sdsm[i] = "{:0.1f}".format(sds * 60)   # convert to minutes of arc
         i += 1
 
     return sdsm
 
 #-------------------------------------------------------------
 #   Sun and Moon calculations  (Lunar Distance charts only)
@@ -803,18 +885,18 @@
         # Unless we have a New Moon, choose to include 3 hour-values minimum per sun/planet per day
         # (because a day could have 22 hours of New Moon, thus 2 valid LD values would be excluded)
         if len(NewMoonHours) == 0 and n < 3: n = 0
         maxLDdelta_per_planet[idx] = ld_delta_max
         LDhours_per_planet[idx] = n
         mag_per_planet[idx] = Vmag
         if n > 0:
-            firstLD_per_planet[idx] = math.copysign(ld_first, ld_first_ra_diff)
-            lastLD_per_planet[idx] = math.copysign(ld_last, ld_last_ra_diff)
-            maxLD_per_planet[idx] = math.copysign(ld_max, ld_max_ra)
-            minLD_per_planet[idx] = math.copysign(ld_min, ld_min_ra)
+            firstLD_per_planet[idx] = copysign(ld_first, ld_first_ra_diff)
+            lastLD_per_planet[idx] = copysign(ld_last, ld_last_ra_diff)
+            maxLD_per_planet[idx] = copysign(ld_max, ld_max_ra)
+            minLD_per_planet[idx] = copysign(ld_min, ld_min_ra)
             #print("Moon {:2d}h RA: {}   {} RA: {}".format(ld_max_i, ra_moon_max, name, ra_planet_max))
         else:       # if no valid LD data
             firstLD_per_planet[idx] = 1000.0    # invalid value
             maxLD_per_planet[idx] = 1000.0      # invalid value
             minLD_per_planet[idx] = 1000.0      # invalid value
 
         # List with these values per planet ...
@@ -1029,18 +1111,18 @@
         # Unless we have a New Moon, choose to include 3 hour-values minimum per sun/planet per day
         # (because a day could have 22 hours of New Moon, thus 2 valid LD values would be excluded)
         if len(NewMoonHours) == 0 and n < 3: n = 0
         maxLDdelta_per_star[ns_idx] = ld_delta_max
         LDhours_per_star[ns_idx] = n
         mag_per_star[ns_idx] = Hpmag
         if n > 0:
-            firstLD_per_star[ns_idx] = math.copysign(ld_first, ld_first_ra_diff)
-            lastLD_per_star[ns_idx] = math.copysign(ld_last, ld_last_ra_diff)
-            maxLD_per_star[ns_idx] = math.copysign(ld_max, ld_max_ra)
-            minLD_per_star[ns_idx] = math.copysign(ld_min, ld_min_ra)
+            firstLD_per_star[ns_idx] = copysign(ld_first, ld_first_ra_diff)
+            lastLD_per_star[ns_idx] = copysign(ld_last, ld_last_ra_diff)
+            maxLD_per_star[ns_idx] = copysign(ld_max, ld_max_ra)
+            minLD_per_star[ns_idx] = copysign(ld_min, ld_min_ra)
             #print("Moon {:2d}h RA: {}   {} RA: {}".format(ld_max_i, ra_moon_max, name, ra_star_max))
         else:       # if no valid LD data
             firstLD_per_star[ns_idx] = 1000.0   # invalid value
             maxLD_per_star[ns_idx] = 1000.0     # invalid value
             minLD_per_star[ns_idx] = 1000.0     # invalid value
 
         # List with these values per star ...
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/ld_stardata.py` & `sfalmanac-1.9/sfalmanac/lib/ld_stardata.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # List of navigational stars with data from Hipparcos, e.g.:
 # http://vizier.u-strasbg.fr/viz-bin/VizieR-5?-source=I/311&-out.all&-out.max=10&HIP==677
 # The format corresponds to an XEphem database file:
 # http://www.clearskyinstitute.com/xephem/help/xephem.html#mozTocId468501
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/ld_tables.py` & `sfalmanac-1.9/sfalmanac/lib/ld_tables.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,39 +3,51 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # NOTE: the new format statement requires a literal '{' to be entered as '{{',
 #       and a literal '}' to be entered as '}}'. The old '%' format specifier
 #       will be removed from Python at some later time. See:
 # https://docs.python.org/3/whatsnew/3.0.html#pep-3101-a-new-approach-to-string-formatting
 
 ###### Standard library imports ######
-import datetime     #from datetime import datetime, timedelta
-import math
-import sys			# required for .stdout.write()
+# don't confuse the 'date' method with the 'Date' variable!
+from datetime import date, datetime, timedelta
+from math import copysign
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 from sfalmanac.lib.ld_skyfield import getDUT1, moon_GHA, moon_SD, moon_VD, ld_planets, ld_stars, find_transit, sunSD
 
 UpperLists = [[], [], []]    # moon GHA per hour for 3 days
 
+#------------------------
+#   internal functions
+#------------------------
+
+def fmtdate(d):
+    if config.pgsz == 'Letter': return d.strftime("%m/%d/%Y")
+    return d.strftime("%d.%m.%Y")
+
+def fmtdates(d1,d2):
+    if config.pgsz == 'Letter': return d1.strftime("%m/%d/%Y") + " - " + d2.strftime("%m/%d/%Y")
+    return d1.strftime("%d.%m.%Y") + " - " + d2.strftime("%d.%m.%Y")
+
 def buildUPlists(n, ghaSoD, ghaPerHour, ghaEoD):
     # build list of hourly GHA values with modified start and end time to
     #  account for rounding times to the minute where 23:59:>30 rounds up
     #  00:00 the next day.
     UpperLists[n] = [-1.0 for x in range(25)]
     UpperLists[n][0] = ghaSoD
     for i in range(23):
@@ -59,34 +71,38 @@
         if forceNS or hr%6 == 0:
             sdeg = r'''\textbf{{{}}}'''.format(hemisph) + deg
         else:
             sdeg = deg
     return sdeg, hemisph
 
 
-def moontab(date, strat, dop):
+#---------------------------------
+#   create Lunar Distance table
+#---------------------------------
+
+def moontab(Date, dpp, strat):
     # generates LaTeX table for moon and Lunar Distance (traditional style)
 
     tab = r'''\setlength{\tabcolsep}{5pt}  % default 6pt
 \noindent'''
     n = 0
-    while n < dop:      # maximum 3 days on a page
+    while n < dpp:      # maximum 3 days on a page
 
 # >>>>>>>>>>>> Calculate all required data <<<<<<<<<<<<
 
         if config.debug_strategy:
             print("=" * 70)
-        date0 = date - datetime.timedelta(days=1)
-        gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD = moon_GHA(date)
-        vmin, dmin = moon_VD(date0,date)
+        Date0 = Date - timedelta(days=1)
+        gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD = moon_GHA(Date)
+        vmin, dmin = moon_VD(Date0,Date)
 
         buildUPlists(n, ghaSoD, GHAupper, ghaEoD)
 
-        out2, tup2, NMhours, ra_m = ld_planets(date)   # planets & sun
-        out, tup = ld_stars(date, NMhours, out2[0][1].hours)
+        out2, tup2, NMhours, ra_m = ld_planets(Date)   # planets & sun
+        out, tup = ld_stars(Date, NMhours, out2[0][1].hours)
         tup = tup + tup2
         tup.sort(key = lambda x: x[1])  # sort by signed first valid LD
         if config.debug_strategy:
             print("New Moon hours:\n{}".format(NMhours))
             for i in range(len(out2)):
                 print("{}:\n{}".format(out2[i][0], out2[i][5]))
             for i in range(len(out)):
@@ -99,16 +115,16 @@
 # >>>>>>>>>>>> Decide which LD lists to print (8 maximum) <<<<<<<<<<<<
 
         if strat == "C":
             LDtxt = " (objects with highest brightness)"
             # build list of objects sorted by largest hourly LD delta first
             tuple_list = [None] * 27
             for i in range(len(tup)):
-##                tuple_list[i] = (tup[i][0], tup[i][4], math.copysign(1, tup[i][1]), tup[i][3])
-                tuple_list[i] = (tup[i][0], tup[i][5], math.copysign(1, tup[i][1]), tup[i][4])
+##                tuple_list[i] = (tup[i][0], tup[i][4], copysign(1, tup[i][1]), tup[i][3])
+                tuple_list[i] = (tup[i][0], tup[i][5], copysign(1, tup[i][1]), tup[i][4])
             tuple_list.sort(key = lambda x: x[1])   # sort by object magnitude
             if config.debug_strategy:
                 print("--- tuples with highest brightness first ---")
                 print(tuple_list)
 ##                print([y[0] for y in tuple_list].index(3))  # find index of star in tuple_list
 
 # =================================================================
@@ -118,16 +134,16 @@
 # >>>>>>>>>>>> Decide which LD lists to print (8 maximum) <<<<<<<<<<<<
 
         if strat == "B":
             LDtxt = " (objects with largest hourly LD delta)"
             # build list of objects sorted by largest hourly LD delta first
             tuple_list = [None] * 27
             for i in range(len(tup)):
-##                tuple_list[i] = (tup[i][0], tup[i][2], math.copysign(1, tup[i][1]), tup[i][3])
-                tuple_list[i] = (tup[i][0], tup[i][3], math.copysign(1, tup[i][1]), tup[i][4])
+##                tuple_list[i] = (tup[i][0], tup[i][2], copysign(1, tup[i][1]), tup[i][3])
+                tuple_list[i] = (tup[i][0], tup[i][3], copysign(1, tup[i][1]), tup[i][4])
             tuple_list.sort(key = lambda x: -x[1])  # sort by max hourly LD delta
             if config.debug_strategy:
                 print("--- tuples with largest ld_delta_max first ---")
                 print(tuple_list)
 ##                print([y[0] for y in tuple_list].index(3))  # find index of star in tuple_list
 
 # =================================================================
@@ -266,15 +282,15 @@
         for objX in obj:
             if objX[1:] == "Sun":
                 sunSDrqrd = True
                 break
             iC += 1
 
         if sunSDrqrd:
-            sdsm = sunSD(date)  # get sun's SD at 0h and 23h
+            sdsm = sunSD(Date)  # get sun's SD at 0h and 23h
             ldx00 = ld[iC][0]
             ldx23 = ld[iC][23]
             if ldx00.find("circ") == -1: ldx00 = ''
             if ldx23.find("circ") == -1: ldx23 = ''
             sdsval = sdsm[0]
             if ldx00 == '': sdsval = sdsm[1]
             if ldx00 != '' and ldx23 != '': # if we have LD at 0h and 23h
@@ -300,15 +316,15 @@
 \multicolumn{1}{c}{\normalsize{h}} & \multicolumn{5}{c}{\normalsize{Moon}}'''
 
         if iCols > 0:
             tab = tab + r''' & \multicolumn{{{}}}{{c}}{{\normalsize{{Lunar Distance{}}}}}'''.format(iCols,LDtxt)
 
         tab = tab + r'''\\
 \hline
-\multicolumn{{1}}{{|c|}}{{\rule{{0pt}}{{2.6ex}}\textbf{{{}}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\(\nu\)}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} & \multicolumn{{1}}{{c}}{{\textit{{d}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{HP}}}}'''.format(date.strftime("%a"))
+\multicolumn{{1}}{{|c|}}{{\rule{{0pt}}{{2.6ex}}\textbf{{{}}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\(\nu\)}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} & \multicolumn{{1}}{{c}}{{\textit{{d}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{HP}}}}'''.format(Date.strftime("%a"))
 
         for iC in range(iCols):
             tab = tab + r''' & \multicolumn{{1}}{{c|}}{{\textbf{{{}}}}}'''.format(obj[iC])
         if len(NMhours) == 24:      # add fake column (iCols == 0)
             tab = tab + r''' & \multicolumn{1}{c|}{}'''
         tab = tab + r'''\\
 \hline\rule{0pt}{2.6ex}\noindent
@@ -323,15 +339,15 @@
                 prevDECm = degm[0]		# hour -1 = hour 0
             if h < 23:
                 nextDECm = degm[h+1]
             else:
                 nextDECm = degm[23]	    # hour 24 = hour 23
 
             mdec, mNS = NSdeg(decm[h],False,h)
-            if mNS != mlastNS or math.copysign(1.0,prevDECm) != math.copysign(1.0,nextDECm):
+            if mNS != mlastNS or copysign(1.0,prevDECm) != copysign(1.0,nextDECm):
                 mdec, mNS = NSdeg(decm[h],False,h,True)	# force N/S
             mlastNS = mNS
 
             line = r'''{} & {} & {} & {} & {} & {}'''.format(h,gham[h],vmin[h],mdec,dmin[h],HPm[h])
 
             if h in set(NMhours):       # better than "if ld[0][h] == "newMoon":"
                 txt = "New Moon"
@@ -351,16 +367,16 @@
 '''
             if h < 23 and (h+1)%6 == 0:
                 lineterminator = r'''\\[2Pt]
 '''
             tab = tab + line + lineterminator
             h += 1
 
-        sdmm = moon_SD(date)
-        mp_upper = find_transit(date, UpperLists[n], False)    # calculate moon upper transit
+        sdmm = moon_SD(Date)
+        mp_upper = find_transit(Date, UpperLists[n], False)    # calculate moon upper transit
         tab = tab + r'''\hline
 \rule{{0pt}}{{2.4ex}} & \multicolumn{{5}}{{c|}}{{SD = {}$'$ \quad Mer. pass. {}}}'''.format(sdmm,mp_upper)
         if iCols > 0:
             if sunSDrqrd:
                 tab = tab + r''' & \multicolumn{{{}}}{{c|}}{{{}}}'''.format(iCols,sdstxt)
             else:
                 tab = tab + r''' & \multicolumn{{{}}}{{c|}}{{}}'''.format(iCols)
@@ -370,262 +386,491 @@
 \hline
 '''
         if n < 2:
             # add space between tables...
             tab = tab + r'''\multicolumn{5}{c}{}\\[-1.5ex]
 '''
         n += 1
-        date += datetime.timedelta(days=1)
+        Date += timedelta(days=1)
         tab = tab + r'''\end{tabular}
 \par\noindent    % put next table below here'''
     return tab
 
 #----------------------
 #   page preparation
 #----------------------
 
-def page(date, strat, dop):
+def page(Date, dpp, strat):
     # creates a page (max. 3 days) of tables
 
     # time delta values for the initial date&time...
-    dut1, deltat = getDUT1(date)
+    dut1, deltat = getDUT1(Date)
     timeDUT1 = r"DUT1 = UT1-UTC = {:+.4f} sec\quad$\Delta$T = TT-UT1 = {:+.4f} sec".format(dut1, deltat)
 
+    Lfoot_IERSEOP = ""
+    if config.dt_IERSEOP != None:
+        # the IERS EOP data start date is 2nd January 1973
+        if Date + timedelta(days=2) >= date(1973, 1, 2):
+            Lfoot_IERSEOP = config.txtIERSEOP
+        if Date + timedelta(days=2) >= config.dt_IERSEOP:
+            Lfoot_IERSEOP = config.endIERSEOP
+        if Date > config.dt_IERSEOP:
+            Lfoot_IERSEOP = r'''\textbf{No IERS EOP prediction data available}'''
+
     page = ''
 
-    if dop > 1:
+    if dpp > 1:
         str2 = r'''\textbf{{{} to {} UT}}
-'''.format(date.strftime("%Y %B %d"),(date+datetime.timedelta(days=dop-1)).strftime("%b. %d"))
+'''.format(Date.strftime("%Y %B %d"),(Date+timedelta(days=dpp-1)).strftime("%b. %d"))
     else:
         str2 = r'''\textbf{{{} UT}}
-'''.format(date.strftime("%Y %B %d"))
+'''.format(Date.strftime("%Y %B %d"))
 
-    str1 = r'''
+    if config.FANCYhd:
+        str1 = r'''
 % ------------------ N E W   P A G E ------------------
 \newpage
 \sffamily
-\lhead{{\noindent\textsf{{\footnotesize{{{}}}}}}}
+\lhead{{\textsf{{\footnotesize{{{}}}}}}}
 \rhead{{\textsf{{\textbf{{{}}}}}}}
+\lfoot{{\textsf{{\footnotesize{{{}}}}}}}
+\begin{{scriptsize}}
+'''.format(timeDUT1, str2, Lfoot_IERSEOP)
+    else:   # old formatting
+        str1 = r'''
+% ------------------ N E W   P A G E ------------------
+\newpage
+\sffamily
+\noindent
+\begin{{flushleft}}     % required so that \par works
+{{\footnotesize {}}}\hfill{}
+\end{{flushleft}}\par
 \begin{{scriptsize}}
 '''.format(timeDUT1, str2)
 
     page = page + str1
 
-    page = page + moontab(date,strat,dop)
+    page = page + moontab(Date,dpp,strat)
     page = page + r'''
 \end{scriptsize}'''
     # to avoid "Overfull \hbox" messages, leave a paragraph end before the end of a size change. (See lines above)
     return page
 
 
-def pages(first_day, strat, daysnum):
+def pages(first_day, dtp, strat):
     # make pages beginning with first_day
+    # dtp = 0 if for entire year; = -1 if for entire month; else days to print
+
     out = ''
     pmth = ''
+    dpp = 3         # 3 days per page maximum
+    day1 = first_day
+
+    if dtp == 0:        # if entire year
+        year = first_day.year
+        yr = year
+        while year == yr:
+            day3 = day1 + timedelta(days=2)
+            if day3.year != yr:
+                dpp -= day3.day
+                if dpp <= 0: return out
+            out += page(day1,dpp,strat)
+            day1 += timedelta(days=3)
+            year = day1.year
+
+    elif dtp == -1:     # if entire month
+        mth = first_day.month
+        m = mth
+        while mth == m:
+            day3 = day1 + timedelta(days=2)
+            if day3.month != m:
+                dpp -= day3.day
+                if dpp <= 0: return out
+            out += page(day1,dpp,strat)
+            day1 += timedelta(days=3)
+            mth = day1.month
+
+    else:           # print 'dtp' days beginning with first_day
+        i = dtp   # don't decrement dtp
+        while i > 0:
+            if i < 3: dpp = i
+            out += page(day1,dpp,strat)
+            i -= 3
+            day1 += timedelta(days=3)
 
-    while daysnum > 0:
-        daysnum -= 3
-        dop = 3 if daysnum >= 0 else daysnum+3      # days to print on page
-        out += page(first_day,strat,dop)
-        first_day += datetime.timedelta(days=3)
     return out
 
+def page2():
+    return r'''
+\setcounter{page}{2}    % otherwise it's 1
+    %\vspace*{5mm}
+    \noindent
+    \textbf{Lunar Distance}\\[12pt]
+    \noindent
+    The Lunar Distance method (or the old method of ``lunars'') is an 18th century technique to find the time, typically to reset ship's clocks or as an emergency procedure.
+    The method uses the Moon's apparent motion relative to the Sun, planets or stars like a clock to find a reference time (e.g. GMT).
+    ``Until 1906, the Nautical Almanac included lunar distance tables showing predicted geocentric angular distances between the Moon and selected bodies in 3-hour intervals. After the tables were dropped, lunar distances fell more or less into oblivion.''\footnote{Henning Umland, Chapter 7 - Finding Time and Longitude by Lunar Distances}\\[12pt]
+    \noindent
+    ``The methods are a good deal more laborious than the more commonplace procedures of celestial navigation. 
+    It is perhaps the most difficult possible operation within the discipline of celestial navigation.
+    However, one argument for maintaining celestial skills is the utility of celestial navigation as an emergency substitute for electronic navigation.''\footnote{Eric Romelczyk, The Journal of Navigation, Volume 72, Issue 6}
+    ``Nothing else comes close to the lunar for developing skill with a sextant - and the observation is demanding enough to hold one's interest for a lifetime.''\footnote{Bruce Stark, page vi, Tables For Clearing the Lunar Distance and Finding Universal Time by Sextant Observation}
+    Thus it is still a valuable process to learn and indeed worthwhile mastering.
+    (A practised user can routinely find the correct time to within ±30 seconds.)\\[12pt]
+    \noindent
+    ``Because the Moon moves much slower across the sky than the stars, its changing position can be used in sort of a reverse process of sight reduction to find the time.''\footnote{Bruce Stark, https://www.celestaire.com/product/tables-for-clearing-the-lunar-distance/}
+    ``The basic idea of the lunar distance method is easy to comprehend. Since the Moon moves across the celestial sphere at a rate of about 0.5$^\circ$ per hour, the angular distance between the Moon and a celestial body in her path varies at a similar rate and rapidly enough to be used to measure the time. The time corresponding with an observed lunar distance can be found by comparison with tabulated values.''\footnote{Henning Umland, Chapter 7 - Finding Time and Longitude by Lunar Distances}
+    (The continuous motion of the Moon through the sky day-by-day implies that different celestial bodies will be selected for LD measurements on different days.)\\[12pt]
+    \noindent
+    The following Lunar Distance tables can contain up to 8 celestial bodies per day (due to the page width limitation).
+    Generally, an attempt is made to include an even number of objects to the east and west of the Moon. 
+    The maximum LD angle chosen for inclusion in the tables is 120$^\circ$, which is about the maximum angle a sextant can measure.\\[12pt]
+    \noindent
+    The celestial bodies available for LD measurement include the Sun, four planets (Venus, Mars, Jupiter, Saturn), 21 navigational stars (with magnitude $\leq$ 1.5) and Polaris.\\[12pt]
+    \noindent
+    Three different strategies are available to select suitable celestial bodies for inclusion in a daily LD table:
+    \begin{itemize}
+    \item pick celestial bodies closest to the Moon
+    \item pick celestial bodies with the highest hourly LD delta (for best accuracy in time determination)
+    \item pick the brightest celestial bodies (possibly easier to locate in the sky)
+    \end{itemize}
+    The celestial body LD angle at a particular hour of day still needs to fulfill several requirements:
+    \begin{itemize}
+    \item the LD of the Sun is \textgreater 10$^\circ$ as the Moon is hardly visible during New Moon. (This applies to \underline{all} celestial bodies)
+    \item the LD of the Sun is \textgreater 40$^\circ$ (otherwise the Moon is not visible)
+    \item only LD angles \textless 120$^\circ$ are tabulated
+    \item the angle between the celestial body and the Sun (``Solar Distance'') is \textgreater 10$^\circ$ (otherwise the celestial body might not be visible)
+    \item the Sun is not between the celestial body and the Moon (based on the Right Ascenscion of all three)
+    \item the hourly LD delta is \textgreater 15$'$ of arc (to avoid measurement errors).
+    ``The rate of change of LD becomes zero when LD passes through a minimum or maximum, making an observation useless.''\footnote{Henning Umland, Chapter 7 - Finding Time and Longitude by Lunar Distances}
+    \item the rate of change of the hourly LD delta does not exceed 0.016$^\circ$ (= 0.96$'$). This empirical figure removes LD values where linear interpolation (between hours) becomes unreliable.
+    \end{itemize}
+    Suggested further reading: ``Stark Tables: For Clearing the Lunar Distance and Finding Universal Time by Sextant Observation'' by Bruce Stark, ISBN 978-0-914025-21-4'''
+
 #--------------------------
 #   external entry point
 #--------------------------
 
-def makeLDtables(first_day, strat, daysnum, entireMth, entireYr, spad, df180, df360):
+def makeLDtables(first_day, dtp, strat, df180, df360):
 
-    # make tables starting from first_day
+    if config.FANCYhd:
+        return makeLDnew(first_day, dtp, strat, df180, df360) # use the 'fancyhdr' package
+    else:
+        return makeLDold(first_day, dtp, strat, df180, df360) # use old formatting
+
+#   The following functions are intentionally separate functions.
+#   'makeEVold' is required for TeX Live 2019, which is the standard
+#   version in Ubuntu 20.04 LTS which expires in April 2030.
+
+def hdrEVnew(first_day,dtp,vsep1,vsep2,df180,df360):
+    # build the front page
     year = first_day.year
     mth = first_day.month
     day = first_day.day
 
+    tex = r'''
+\pagestyle{frontpage}
+    \begin{titlepage}
+    \begin{center}
+    \textsc{\Large Generated using Skyfield}\\
+    \large http://rhodesmill.org/skyfield/\\[0.7cm]'''
+
+    if config.dockerized:   # DOCKER ONLY
+        df180 = "../A4chart0-180_P.pdf"
+        df360 = "../A4chart180-360_P.pdf"
+
+    tex += r'''
+    % TRIM values: left bottom right top
+    \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\[0.3cm]
+    \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\'''.format(df180,df360)
+    
+    tex += r'''[{}]
+    \textsc{{\huge Lunar Distance}}\\[{}]'''.format(vsep1,vsep2)
+
+    if dtp == 0:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(first_day.year)
+    elif dtp == -1:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(first_day.strftime("%B %Y"))
+    elif dtp > 1:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdates(first_day,first_day+timedelta(days=dtp-1)))
+    else:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdate(first_day))
+
+    tex += r'''
+    \begin{center}\begin{tabular}[t]{rl}
+    \large\emph{Author:} & \large Andrew \textsc{Bauer}\\
+    \end{tabular}\end{center}'''
+
+    tex += r'''
+    {\large \today}
+    \HRule \\[0.2cm]
+    \end{center}
+    \begin{description}[leftmargin=5.5em,style=nextline]\footnotesize
+    \item[Disclaimer:] These are computer generated tables - use them at your own risk. They replicate Lunar Distance algorithms with no guarantee of accuracy. They are intended to encourage the use of sextants, be it as a hobby or as a backup when electronics fail. The author claims no liability for any consequences arising from use of these tables and accompanying charts.
+    \end{description}
+\end{titlepage}
+\pagestyle{page2}  % page style for page 2'''
+
+    tex += page2()
+
+    return tex
+
+def makeLDnew(first_day, dtp, strat, df180, df360):
+    # make tables starting from first_day
+
     # page size specific parameters
     # NOTE: 'bm' (bottom margin) is an unrealistic value used only to determine the vertical size of 'body' (textheight), which must be large enough to include all the tables. 'tm' (top margin) and 'hs' (headsep) determine the top of body. Finally use 'fs' (footskip) to position the footer.
     if config.pgsz == "A4":
         # A4 ... pay attention to the limited page width
         paper = "a4paper"
         # title page...
         vsep1 = "1.5cm"
         vsep2 = "1.0cm"
         tm1 = "21mm"
         bm1 = "15mm"
         lm1 = "10mm"
         rm1 = "10mm"
-        # description text...
+        # page 2 text...
         tm2 = "21mm"
         bm2 = "18mm"
+        fs2 = "20pt"
         # data pages...
-        tm = "34.5mm"       # was "21mm" [v2q]
-        bm = "12mm"         # was "18mm" [v2q]
-        hs = "5.1pt"        # headsep  (page 3 onwards) [v2q]
-        fs = "24pt"         # footskip (page 3 onwards) [v2q]
+        tm = "27.6mm"       # was "21mm"
+        bm = "16mm"         # was "18mm"
+        hs = "4.9pt"        # headsep  (page 3 onwards)
+        fs = "12pt"         # footskip (page 3 onwards)
         lm = "16mm"
         rm = "12mm"
     else:
         # LETTER ... pay attention to the limited page height
         paper = "letterpaper"
         # title page...
         vsep1 = "0.8cm"
         vsep2 = "0.7cm"
         tm1 = "12mm"
         bm1 = "15mm"
         lm1 = "12mm"
         rm1 = "12mm"
-        # description text...
+        # page 2 text...
         tm2 = "12mm"
         bm2 = "13mm"
+        fs2 = "20pt"
         # data pages...
-        tm = "25.6mm"       # was "12mm" [v2q]
-        bm = "5mm"          # was "12mm" [v2q]
-        hs = "2.6pt"        # headsep  (page 3 onwards) [v2q]
-        fs = "21pt"         # footskip (page 3 onwards) [v2q]
+        tm = "17.8mm"       # was "12mm"
+        bm = "10.5mm"       # was "12mm"
+        hs = "2.6pt"        # headsep  (page 3 onwards)
+        fs = "12pt"         # footskip (page 3 onwards)
         lm = "16mm"
         rm = "14mm"
 
     # default is 'oneside'...
-    alm = r'''\documentclass[10pt, {}]{{report}}'''.format(paper)
+    tex = r'''\documentclass[10pt, {}]{{report}}'''.format(paper)
 
-    alm = alm + r'''
+    tex += r'''
 %\usepackage[utf8]{inputenc}
 \usepackage[english]{babel}
 \usepackage{fontenc}
 \usepackage{enumitem} % used to customize the {description} environment'''
 
     # to troubleshoot add "showframe, verbose," below:
-    alm = alm + r'''
-\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}
-\setlength{{\headsep}}{{{}}} % [v2q]'''.format(tm,bm,lm,rm,hs)
+    tex += r'''
+\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm1,bm1,lm1,rm1)
+
+    # define page styles
+    # CAUTION: putting '\fancyhf{}' in frontpage style also clears the footer in page2!
+    tex += r'''
+%------------ page styles ------------
+\usepackage{fancyhdr}
+\renewcommand{\headrulewidth}{0pt}
+\renewcommand{\footrulewidth}{0pt}
+\fancypagestyle{frontpage}{
+}
+\fancypagestyle{page2}[frontpage]{'''
+    tex += r'''
+  \newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}, headsep={}, footskip={}}}'''.format(tm2,bm2,lm,rm,hs,fs2)
+    tex += r'''
+  \cfoot{\centerline{Page \thepage}}
+  \fancyfootoffset[R]{0pt}% recalculate \headwidth
+}
+\fancypagestyle{datapage}[page2]{'''
+    tex += r'''
+  \newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}, headsep={}, footskip={}}}'''.format(tm,bm,lm,rm,hs,fs)
+    tex += r'''
+  \rfoot{\textsf{\footnotesize{https://pypi.org/project/sfalmanac/}}}
+} %-----------------------------------'''
 
     # Note: \DeclareUnicodeCharacter is not compatible with some versions of pdflatex
-    alm = alm + r'''
+    tex += r'''
 \usepackage{xcolor}  % highlight double moon events on same day
 \definecolor{khaki}{rgb}{0.76, 0.69, 0.57}
 \usepackage{multirow}
 \newcommand{\HRule}{\rule{\linewidth}{0.5mm}}
-\usepackage{fancyhdr}   % [v2q]
-\pagestyle{fancy}       % [v2q]
-\renewcommand{\headrulewidth}{0pt}  % [v2q]
-\setlength{\footskip}{20pt}
 \usepackage[pdftex]{graphicx}	% for \includegraphics
 \usepackage{tikz}				% for \draw  (load after 'graphicx')
 %\showboxbreadth=50  % use for logging
 %\showboxdepth=50    % use for logging
 %\DeclareUnicodeCharacter{00B0}{\ensuremath{{}^\circ}}
 \setlength\fboxsep{1.5pt}       % ONLY used by \colorbox in ldist_skyfield.py
 \begin{document}'''
 
-    alm = alm + r'''
+    if not config.DPonly:
+        tex += hdrEVnew(first_day,dtp,vsep1,vsep2,df180,df360)
+
+    tex += r'''
+\pagestyle{datapage}  % the default page style for the document'''
+
+    tex += pages(first_day,dtp,strat)
+    tex += r'''
+\end{document}'''
+    return tex
+
+# ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===
+# ===   ===   ===   ===   O L D   F O R M A T T I N G   ===   ===   ===   ===
+# ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===
+
+def hdrEVold(first_day,dtp,tm1,bm1,lm1,rm1,vsep1,vsep2,df180,df360):
+    # build the front page
+    year = first_day.year
+    mth = first_day.month
+    day = first_day.day
+
+    tex = r'''
 % for the title page only...
 \newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}}}'''.format(tm1,bm1,lm1,rm1)
 
-    alm = alm + r'''
+    tex += r'''
     \begin{titlepage}
     \begin{center}
     \textsc{\Large Generated using Skyfield}\\
     \large http://rhodesmill.org/skyfield/\\[0.7cm]'''
 
     if config.dockerized:   # DOCKER ONLY
         df180 = "../A4chart0-180_P.pdf"
         df360 = "../A4chart180-360_P.pdf"
 
-    alm = alm + r'''
+    tex += r'''
     % TRIM values: left bottom right top
     \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\[0.3cm]
     \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\'''.format(df180,df360)
     
-    alm = alm + r'''[{}]
+    tex += r'''[{}]
     \textsc{{\huge Lunar Distance}}\\[{}]'''.format(vsep1,vsep2)
 
-    if entireYr:
-        alm = alm + r'''
+    if dtp == 0:
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
-    \HRule \\'''.format(year)
-    elif entireMth:
-        alm = alm + r'''
+    \HRule \\'''.format(first_day.year)
+    elif dtp == -1:
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
     \HRule \\'''.format(first_day.strftime("%B %Y"))
+    elif dtp > 1:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdates(first_day,first_day+timedelta(days=dtp-1)))
     else:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
-    {{ \Huge \bfseries from {}.{}.{}}}\\[0.2cm]
-    \HRule \\'''.format(day,mth,year)
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdate(first_day))
 
-    alm = alm + r'''
+    tex += r'''
     \begin{center}\begin{tabular}[t]{rl}
     \large\emph{Author:} & \large Andrew \textsc{Bauer}\\
     \end{tabular}\end{center}'''
 
-    alm = alm + r'''
+    tex += r'''
     {\large \today}
     \HRule \\[0.2cm]
     \end{center}
     \begin{description}[leftmargin=5.5em,style=nextline]\footnotesize
     \item[Disclaimer:] These are computer generated tables - use them at your own risk. They replicate Lunar Distance algorithms with no guarantee of accuracy. They are intended to encourage the use of sextants, be it as a hobby or as a backup when electronics fail. The author claims no liability for any consequences arising from use of these tables and accompanying charts.
     \end{description}
-\end{titlepage}'''
-
-    alm = alm + r'''
-% for the description text only...
-\newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}}}'''.format(tm2,bm2,lm,rm)
-
-    alm = alm + r'''
-\lfoot{\textsf{\footnotesize{https://thenauticalalmanac.com/}}}
-\cfoot{\centerline{Page \thepage}}
-\rfoot{\textsf{\footnotesize{https://pypi.org/project/sfalmanac/}}}
-\setcounter{page}{2}    % otherwise it's 1
-    %\vspace*{5mm}
-    \noindent
-    \textbf{Lunar Distance}\\[12pt]
-    \noindent
-    The Lunar Distance method (or the old method of ``lunars'') is an 18th century technique to find the time, typically to reset ship's clocks or as an emergency procedure.
-    The method uses the Moon's apparent motion relative to the Sun, planets or stars like a clock to find a reference time (e.g. GMT).
-    ``Until 1906, the Nautical Almanac included lunar distance tables showing predicted geocentric angular distances between the Moon and selected bodies in 3-hour intervals. After the tables were dropped, lunar distances fell more or less into oblivion.''\footnote{Henning Umland, Chapter 7 - Finding Time and Longitude by Lunar Distances}\\[12pt]
-    \noindent
-    ``The methods are a good deal more laborious than the more commonplace procedures of celestial navigation. 
-    It is perhaps the most difficult possible operation within the discipline of celestial navigation.
-    However, one argument for maintaining celestial skills is the utility of celestial navigation as an emergency substitute for electronic navigation.''\footnote{Eric Romelczyk, The Journal of Navigation, Volume 72, Issue 6}
-    ``Nothing else comes close to the lunar for developing skill with a sextant - and the observation is demanding enough to hold one's interest for a lifetime.''\footnote{Bruce Stark, page vi, Tables For Clearing the Lunar Distance and Finding Universal Time by Sextant Observation}
-    Thus it is still a valuable process to learn and indeed worthwhile mastering.
-    (A practised user can routinely find the correct time to within ±30 seconds.)\\[12pt]
-    \noindent
-    ``Because the Moon moves much slower across the sky than the stars, its changing position can be used in sort of a reverse process of sight reduction to find the time.''\footnote{Bruce Stark, https://www.celestaire.com/product/tables-for-clearing-the-lunar-distance/}
-    ``The basic idea of the lunar distance method is easy to comprehend. Since the Moon moves across the celestial sphere at a rate of about 0.5$^\circ$ per hour, the angular distance between the Moon and a celestial body in her path varies at a similar rate and rapidly enough to be used to measure the time. The time corresponding with an observed lunar distance can be found by comparison with tabulated values.''\footnote{Henning Umland, Chapter 7 - Finding Time and Longitude by Lunar Distances}
-    (The continuous motion of the Moon through the sky day-by-day implies that different celestial bodies will be selected for LD measurements on different days.)\\[12pt]
-    \noindent
-    The following Lunar Distance tables can contain up to 8 celestial bodies per day (due to the page width limitation).
-    Generally, an attempt is made to include an even number of objects to the east and west of the Moon. 
-    The maximum LD angle chosen for inclusion in the tables is 120$^\circ$, which is about the maximum angle a sextant can measure.\\[12pt]
-    \noindent
-    The celestial bodies available for LD measurement include the Sun, four planets (Venus, Mars, Jupiter, Saturn), 21 navigational stars (with magnitude $\leq$ 1.5) and Polaris.\\[12pt]
-    \noindent
-    Three different strategies are available to select suitable celestial bodies for inclusion in a daily LD table:
-    \begin{itemize}
-    \item pick celestial bodies closest to the Moon
-    \item pick celestial bodies with the highest hourly LD delta (for best accuracy in time determination)
-    \item pick the brightest celestial bodies (possibly easier to locate in the sky)
-    \end{itemize}
-    The celestial body LD angle at a particular hour of day still needs to fulfill several requirements:
-    \begin{itemize}
-    \item the LD of the Sun is \textgreater 10$^\circ$ as the Moon is hardly visible during New Moon. (This applies to \underline{all} celestial bodies)
-    \item the LD of the Sun is \textgreater 40$^\circ$ (otherwise the Moon is not visible)
-    \item only LD angles \textless 120$^\circ$ are tabulated
-    \item the angle between the celestial body and the Sun (``Solar Distance'') is \textgreater 10$^\circ$ (otherwise the celestial body might not be visible)
-    \item the Sun is not between the celestial body and the Moon (based on the Right Ascenscion of all three)
-    \item the hourly LD delta is \textgreater 15$'$ of arc (to avoid measurement errors).
-    ``The rate of change of LD becomes zero when LD passes through a minimum or maximum, making an observation useless.''\footnote{Henning Umland, Chapter 7 - Finding Time and Longitude by Lunar Distances}
-    \item the rate of change of the hourly LD delta does not exceed 0.016$^\circ$ (= 0.96$'$). This empirical figure removes LD values where linear interpolation (between hours) becomes unreliable.
-    \end{itemize}
-    Suggested further reading: ``Stark Tables: For Clearing the Lunar Distance and Finding Universal Time by Sextant Observation'' by Bruce Stark, ISBN 978-0-914025-21-4
+\end{titlepage}
 \restoregeometry    % so it does not affect the rest of the pages'''
 
-    # footskip = distance of footer baseline below body [v2q]
-    alm = alm + r'''
-\setlength{{\footskip}}{{{}}}'''.format(fs)
+    tex += page2()
+
+    return tex
+
+def makeLDold(first_day, dtp, strat, df180, df360):
+    # make tables starting from first_day
+    # dtp = 0 if for entire year; = -1 if for entire month; else days to print
+
+    # page size specific parameters
+    if config.pgsz == "A4":
+        # pay attention to the limited page width
+        paper = "a4paper"
+        vsep1 = "1.5cm"
+        vsep2 = "1.0cm"
+        tm1 = "21mm"    # title page...
+        bm1 = "15mm"
+        lm1 = "10mm"
+        rm1 = "10mm"
+        tm = "21mm"     # data pages...
+        bm = "18mm"
+        lm = "16mm"
+        rm = "12mm"
+    else:
+        # pay attention to the limited page height
+        paper = "letterpaper"
+        vsep1 = "0.8cm"
+        vsep2 = "0.7cm"
+        tm1 = "12mm"    # title page...
+        bm1 = "15mm"
+        lm1 = "12mm"
+        rm1 = "12mm"
+        tm = "12mm"   # data pages...
+        bm = "12mm"
+        lm = "16mm"
+        rm = "14mm"
+
+    # default is 'oneside'...
+    tex = r'''\documentclass[10pt, {}]{{report}}'''.format(paper)
+
+    tex += r'''
+%\usepackage[utf8]{inputenc}
+\usepackage[english]{babel}
+\usepackage{fontenc}
+\usepackage{enumitem} % used to customize the {description} environment'''
+
+    # to troubleshoot add "showframe, verbose," below:
+    tex += r'''
+\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm,bm,lm,rm)
+
+    # Note: \DeclareUnicodeCharacter is not compatible with some versions of pdflatex
+    tex += r'''
+\usepackage{xcolor}  % highlight double moon events on same day
+\definecolor{khaki}{rgb}{0.76, 0.69, 0.57}
+\usepackage{multirow}
+\newcommand{\HRule}{\rule{\linewidth}{0.5mm}}
+\setlength{\footskip}{15pt}
+\usepackage[pdftex]{graphicx}	% for \includegraphics
+\usepackage{tikz}				% for \draw  (load after 'graphicx')
+%\showboxbreadth=50  % use for logging
+%\showboxdepth=50    % use for logging
+%\DeclareUnicodeCharacter{00B0}{\ensuremath{{}^\circ}}
+\setlength\fboxsep{1.5pt}       % ONLY used by \colorbox in ldist_skyfield.py
+\begin{document}'''
+
+    if not config.DPonly:
+        tex += hdrEVold(first_day,dtp,tm1,bm1,lm1,rm1,vsep1,vsep2,df180,df360)
 
-    alm = alm + pages(first_day,strat,daysnum)
-    alm = alm + '''
+    tex += pages(first_day,dtp,strat)
+    tex += r'''
 \end{document}'''
-    return alm
+    return tex
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/mp_eventtables.py` & `sfalmanac-1.9/sfalmanac/lib/mp_eventtables.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # ----------------------------------------------------------------------------------
 # THIS MODULE IS OPTIMIZED SPECIFICALLY FOR MULTIPROCESSING (DATA BASED PARALELLISM)
 # Except for 4 functions this replaces alma_skyfield.py
 #     Note: 6 worker processes are sufficient
@@ -37,15 +37,15 @@
 from skyfield.api import Loader     # rqrd for PyPI version
 from skyfield.api import Topos, Star
 from skyfield import almanac
 from skyfield.nutationlib import iau2000b
 #from skyfield.data import hipparcos
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 
 #----------------------
 #   initialization
 #----------------------
 
 hour_of_day = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23]
 degree_sign= u'\N{DEGREE SIGN}'
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/mp_nautical.py` & `sfalmanac-1.9/sfalmanac/lib/mp_nautical.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 #   Copyright (C) 2022  Andrew Bauer
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # ----------------------------------------------------------------------------------
 # THIS MODULE IS OPTIMIZED SPECIFICALLY FOR MULTIPROCESSING (DATA BASED PARALELLISM)
 #     Note: 6 worker processes are sufficient
 #     Note: read/write to a global variable will occur randomly and give false
@@ -36,15 +36,15 @@
 from skyfield.api import Loader     # rqrd for PyPI version
 from skyfield.api import Topos, Star
 from skyfield import almanac
 from skyfield.nutationlib import iau2000b
 #from skyfield.data import hipparcos
 
 ###### Local application imports ######
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 
 #----------------------
 #   initialization
 #----------------------
 
 hour_of_day = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23]
 next_hour_of_day = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24]
```

### Comparing `sfalmanac-1.8.2/sfalmanac/lib/nautical.py` & `sfalmanac-1.9/sfalmanac/lib/nautical.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #   Copyright (C) 2022  Andrew Bauer
 #   Copyright (C) 2014  Enno Rodegerdts
 
 #   This program is free software; you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
 #   (at your option) any later version.
-# 
+#
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
-# 
+#
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # NOTE: the new format statement requires a literal '{' to be entered as '{{',
 #       and a literal '}' to be entered as '}}'. The old '%' format specifier
 #       will be removed from Python at some later time. See:
 # https://docs.python.org/3/whatsnew/3.0.html#pep-3101-a-new-approach-to-string-formatting
@@ -38,24 +38,23 @@
 #       is possible: https://de.wikibooks.org/wiki/LaTeX-W%C3%B6rterbuch:_tabular
 #       This works, but again increases the overall table width unnecessarily.
 #       Conclusion/Resolution:
 #       The following code now uses the 'tabular' table style without any
 #       column width specifiers - thus table widths vary slightly from page to page.
 
 ###### Standard library imports ######
-from datetime import datetime, timedelta
+# don't confuse the 'date' method with the 'Date' variable!
+from datetime import date, datetime, timedelta
 import sys			# required for .stdout.write()
 import signal       # for init_worker
-from math import cos as cos
-from math import copysign as copysign
-from math import pi as pi
+from math import cos, copysign, pi
 
 ###### Local application imports ######
 from sfalmanac.lib.alma_ephem import magnitudes
-from sfalmanac.lib import config as config
+from sfalmanac.lib import config
 if config.MULTIpr:  # in multi-processing mode ...
     # ! DO NOT PLACE imports IN CONDITIONAL 'if'-STATEMENTS WHEN MULTI-PROCESSING !
     import multiprocessing as mp
     from functools import partial
     # ... following is still required for SINGLE-PROCESSING (in multi-processing mode):
     from sfalmanac.lib.alma_skyfield import ariesGHA, venusGHA, marsGHA, jupiterGHA, saturnGHA, sunGHA, moonGHA, moonVD, sunSD, moonSD, vdm_Venus, vdm_Mars, vdm_Jupiter, vdm_Saturn, ariestransit, stellar_info, planetstransit, moonage, moonphase, equation_of_time, getDUT1, find_new_moon
     # ... following is required for MULTI-PROCESSING:
@@ -256,41 +255,41 @@
     dbl = False
     for i in range(len(m1)):
         if m2[i] != '--:--':
             dbl = True
     return dbl
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def mp_planetGHA_worker(date, ts, spad, obj):
+def mp_planetGHA_worker(Date, ts, spad, obj):
     #print(" mp_planetGHA_worker Start  {}".format(obj))
-    gha = mp_planetGHA(date, ts, spad, obj)    # ===>>> mp_nautical.py
+    gha = mp_planetGHA(Date, ts, spad, obj)    # ===>>> mp_nautical.py
     #print(" mp_planetGHA_worker Finish {}".format(obj))
     return gha      # return list for four planets and Aries
 
-def planetstab(date, ts, spad):
+def planetstab(Date, ts, spad):
     # generates a LaTeX table for the navigational plantets (traditional style)
     # OLD: \begin{tabular*}{0.74\textwidth}[t]{@{\extracolsep{\fill}}|c|r|rr|rr|rr|rr|}
     tab = r'''\noindent
 \setlength{\tabcolsep}{5.8pt}  % default 6pt
 \begin{tabular}[t]{|c|r|rr|rr|rr|rr|}
 \multicolumn{1}{c}{\normalsize{}} & \multicolumn{1}{c}{\normalsize{Aries}} &  \multicolumn{2}{c}{\normalsize{Venus}}& \multicolumn{2}{c}{\normalsize{Mars}} & \multicolumn{2}{c}{\normalsize{Jupiter}} & \multicolumn{2}{c}{\normalsize{Saturn}}\\
 '''
     # note: 74% table width above removes "Overfull \hbox (1.65279pt too wide)"
     n = 0
     while n < 3:
         tab = tab + r'''\hline
 \rule{{0pt}}{{2.4ex}}\textbf{{{}}} & \multicolumn{{1}}{{c|}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{Dec}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{Dec}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{Dec}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{Dec}}}}\\
 \hline\rule{{0pt}}{{2.6ex}}\noindent
-'''.format(date.strftime("%a"))
+'''.format(Date.strftime("%a"))
 
         if config.MULTIpr and config.WINpf:
             global pool
             # multiprocess 'SHA + transit times' simultaneously
             objlist = ['aries', 'venus', 'mars', 'jupiter', 'saturn']
-            partial_func2 = partial(mp_planetGHA_worker, date, ts, spad)
+            partial_func2 = partial(mp_planetGHA_worker, Date, ts, spad)
 
             try:
                 # RECOMMENDED: chunksize = 1
                 listofGHA = pool.map(partial_func2, objlist, 1)
             except KeyboardInterrupt:
                 print(msg0)
                 sys.exit(0)
@@ -305,19 +304,19 @@
             jGHA = listofGHA[3][0]
             jDEC = listofGHA[3][1]
             jDEG = listofGHA[3][2]
             sGHA = listofGHA[4][0]
             sDEC = listofGHA[4][1]
             sDEG = listofGHA[4][2]
         else:
-            aGHA             = ariesGHA(date)
-            vGHA, vDEC, vDEG = venusGHA(date)
-            mGHA, mDEC, mDEG = marsGHA(date)
-            jGHA, jDEC, jDEG = jupiterGHA(date)
-            sGHA, sDEC, sDEG = saturnGHA(date)
+            aGHA             = ariesGHA(Date)
+            vGHA, vDEC, vDEG = venusGHA(Date)
+            mGHA, mDEC, mDEG = marsGHA(Date)
+            jGHA, jDEC, jDEG = jupiterGHA(Date)
+            sGHA, sDEC, sDEG = saturnGHA(Date)
         h = 0
 
         if config.decf != '+':	# USNO format for Declination
             while h < 24:
                 if h > 0:
                     prevDECv = vDEG[h-1]
                     prevDECm = mDEG[h-1]
@@ -368,36 +367,36 @@
 '''
                 if h < 23 and (h+1)%6 == 0:
                     lineterminator = r'''\\[2Pt]
 '''
                 tab = tab + line + lineterminator
                 h += 1
 
-        mag_v, mag_m, mag_j, mag_s = magnitudes(date)   # magnitudes from Ephem
-        RAc_v, Dc_v, mag_v = vdm_Venus(date)
-        RAc_m, Dc_m = vdm_Mars(date)
-        RAc_j, Dc_j, mag_j = vdm_Jupiter(date)
-        RAc_s, Dc_s = vdm_Saturn(date)
+        mag_v, mag_m, mag_j, mag_s = magnitudes(Date)   # magnitudes from Ephem
+        RAc_v, Dc_v, mag_v = vdm_Venus(Date)
+        RAc_m, Dc_m = vdm_Mars(Date)
+        RAc_j, Dc_j, mag_j = vdm_Jupiter(Date)
+        RAc_s, Dc_s = vdm_Saturn(Date)
         tab = tab + r'''\hline
 \multicolumn{{2}}{{|c|}}{{\rule{{0pt}}{{2.4ex}}Mer.pass. {}}} & 
 \multicolumn{{2}}{{c|}}{{\(\nu\) {}$'$ \emph{{d}} {}$'$ m {}}} & 
 \multicolumn{{2}}{{c|}}{{\(\nu\) {}$'$ \emph{{d}} {}$'$ m {}}} & 
 \multicolumn{{2}}{{c|}}{{\(\nu\) {}$'$ \emph{{d}} {}$'$ m {}}} & 
 \multicolumn{{2}}{{c|}}{{\(\nu\) {}$'$ \emph{{d}} {}$'$ m {}}}\\
 \hline
 \multicolumn{{10}}{{c}}{{}}\\
-'''.format(ariestransit(date+timedelta(days=1)),RAc_v,Dc_v,mag_v,RAc_m,Dc_m,mag_m,RAc_j,Dc_j,mag_j,RAc_s,Dc_s,mag_s)
+'''.format(ariestransit(Date+timedelta(days=1)),RAc_v,Dc_v,mag_v,RAc_m,Dc_m,mag_m,RAc_j,Dc_j,mag_j,RAc_s,Dc_s,mag_s)
         n += 1
-        date += timedelta(days=1)
+        Date += timedelta(days=1)
     tab = tab + r'''\end{tabular}
 '''
     return tab
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def planetstabm(date, ts, spad):
+def planetstabm(Date, ts, spad):
     # generates a LaTeX table for the navigational plantets (modern style)
 
     tab = r'''\vspace{6Pt}\noindent
 \renewcommand{\arraystretch}{1.1}
 \setlength{\tabcolsep}{4pt}  % default 6pt
 \begin{tabular}[t]{crcrrcrrcrrcrr}
 \multicolumn{1}{c}{\normalsize{h}} & 
@@ -408,19 +407,19 @@
 \multicolumn{2}{c}{\normalsize{Saturn}}\\
 \cmidrule{2-2} \cmidrule{4-5} \cmidrule{7-8} \cmidrule{10-11} \cmidrule{13-14}'''
     n = 0
     while n < 3:
         tab = tab + r'''
 \multicolumn{{1}}{{c}}{{\textbf{{{}}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} && 
 \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} &&  \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} &&  \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} &&  \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}}\\
-'''.format(date.strftime("%a"))
+'''.format(Date.strftime("%a"))
         if config.MULTIpr and config.WINpf:
             # multiprocess 'SHA + transit times' simultaneously
             objlist = ['aries', 'venus', 'mars', 'jupiter', 'saturn']
-            partial_func2 = partial(mp_planetGHA_worker, date, ts, spad)
+            partial_func2 = partial(mp_planetGHA_worker, Date, ts, spad)
 
             try:
                 # RECOMMENDED: chunksize = 1
                 listofGHA = pool.map(partial_func2, objlist, 1)
             except KeyboardInterrupt:
                 print(msg0)
                 sys.exit(0)
@@ -435,19 +434,19 @@
             jGHA = listofGHA[3][0]
             jDEC = listofGHA[3][1]
             jDEG = listofGHA[3][2]
             sGHA = listofGHA[4][0]
             sDEC = listofGHA[4][1]
             sDEG = listofGHA[4][2]
         else:
-            aGHA             = ariesGHA(date)
-            vGHA, vDEC, vDEG = venusGHA(date)
-            mGHA, mDEC, mDEG = marsGHA(date)
-            jGHA, jDEC, jDEG = jupiterGHA(date)
-            sGHA, sDEC, sDEG = saturnGHA(date)
+            aGHA             = ariesGHA(Date)
+            vGHA, vDEC, vDEG = venusGHA(Date)
+            mGHA, mDEC, mDEG = marsGHA(Date)
+            jGHA, jDEC, jDEG = jupiterGHA(Date)
+            sGHA, sDEC, sDEG = saturnGHA(Date)
         h = 0
 
         if config.decf != '+':	# USNO format for Declination
             while h < 24:
                 band = int(h/6)
                 group = band % 2
                 if h > 0:
@@ -502,54 +501,55 @@
 '''.format(aGHA[h],vGHA[h],vDEC[h],mGHA[h],mDEC[h],jGHA[h],jDEC[h],sGHA[h],sDEC[h])
                 if group == 1:
                     tab = tab + r'''\rowcolor{LightCyan}
 '''
                 tab = tab + line
                 h += 1
 
-        mag_v, mag_m, mag_j, mag_s = magnitudes(date)   # magnitudes from Ephem
-        RAc_v, Dc_v, mag_v = vdm_Venus(date)
-        RAc_m, Dc_m = vdm_Mars(date)
-        RAc_j, Dc_j, mag_j = vdm_Jupiter(date)
-        RAc_s, Dc_s = vdm_Saturn(date)
+        mag_v, mag_m, mag_j, mag_s = magnitudes(Date)   # magnitudes from Ephem
+        RAc_v, Dc_v, mag_v = vdm_Venus(Date)
+        RAc_m, Dc_m = vdm_Mars(Date)
+        RAc_j, Dc_j, mag_j = vdm_Jupiter(Date)
+        RAc_s, Dc_s = vdm_Saturn(Date)
         tab = tab + r'''\cmidrule{{1-2}} \cmidrule{{4-5}} \cmidrule{{7-8}} \cmidrule{{10-11}} \cmidrule{{13-14}}
 \multicolumn{{2}}{{c}}{{\footnotesize{{Mer.pass. {}}}}} && 
 \multicolumn{{2}}{{c}}{{\footnotesize{{\(\nu\){}$'$ \emph{{d}}{}$'$ m{}}}}} && 
 \multicolumn{{2}}{{c}}{{\footnotesize{{\(\nu\){}$'$ \emph{{d}}{}$'$ m{}}}}} && 
 \multicolumn{{2}}{{c}}{{\footnotesize{{\(\nu\){}$'$ \emph{{d}}{}$'$ m{}}}}} && 
 \multicolumn{{2}}{{c}}{{\footnotesize{{\(\nu\){}$'$ \emph{{d}}{}$'$ m{}}}}}\\
 \cmidrule{{1-2}} \cmidrule{{4-5}} \cmidrule{{7-8}} \cmidrule{{10-11}} \cmidrule{{13-14}}
-'''.format(ariestransit(date+timedelta(days=1)),RAc_v,Dc_v,mag_v,RAc_m,Dc_m,mag_m,RAc_j,Dc_j,mag_j,RAc_s,Dc_s,mag_s)
+'''.format(ariestransit(Date+timedelta(days=1)),RAc_v,Dc_v,mag_v,RAc_m,Dc_m,mag_m,RAc_j,Dc_j,mag_j,RAc_s,Dc_s,mag_s)
         if n < 2:
             vsep = ""
             if config.pgsz == "Letter":
                 vsep = "[-2.0ex]"
             # add space between tables...
             tab = tab + r'''\multicolumn{{10}}{{c}}{{}}\\{}'''.format(vsep)
         n += 1
-        date += timedelta(days=1)
+        Date += timedelta(days=1)
 
     tab = tab+r'''\end{tabular}\quad
 '''
     return tab
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def mp_planets_worker(date, ts, spad, obj):
+def mp_planets_worker(Date, ts, spad, obj):
     #print(" mp_planets_worker Start  {}".format(obj))
-    sha = mp_planetstransit(date, ts, spad, obj)    # ===>>> mp_nautical.py
+    sha = mp_planetstransit(Date, ts, spad, obj)    # ===>>> mp_nautical.py
     #print(" mp_planets_worker Finish {}".format(obj))
     return sha      # return list for four planets
 
-def starstab(date, ts, spad):
+def starstab(Date, ts, spad):
     # returns a table with ephemerides for the navigational stars
     # OLD: \begin{tabular*}{0.251\textwidth}[t]{@{\extracolsep{\fill}}|rrr|}
     # OLD: note: 0.251 instead of 0.25 (above) prevents an "Overfull \hbox (0.14297pt too wide)" message on about 5 specific pages in the full year (moonimg=True)
 
     if config.tbls == "m":
-        out = r'''\setlength{\tabcolsep}{4pt}  % default 6pt
+        out = r'''\renewcommand{\arraystretch}{1.1}
+\setlength{\tabcolsep}{4pt}  % default 6pt
 \begin{tabular}[t]{|rrr|}
 \multicolumn{3}{c}{\normalsize{Stars}}\\
 \hline
 & \multicolumn{1}{c}{\multirow{2}{*}{\textbf{SHA}}} 
 & \multicolumn{1}{c|}{\multirow{2}{*}{\textbf{Dec}}}\\
 & & \multicolumn{1}{c|}{} \\
 '''
@@ -557,39 +557,39 @@
         out = r'''\setlength{\tabcolsep}{5pt}  % default 6pt
 \begin{tabular}[t]{|rrr|}
 \multicolumn{3}{c}{\normalsize{Stars}}\\
 \hline
 \rule{0pt}{2.4ex} & \multicolumn{1}{c}{\textbf{SHA}} & \multicolumn{1}{c|}{\textbf{Dec}}\\
 \hline\rule{0pt}{2.6ex}\noindent
 '''
-    stars = stellar_info(date + timedelta(days=1))
+    stars = stellar_info(Date + timedelta(days=1))
 
     for i in range(len(stars)):
         out = out + r'''{} & {} & {} \\
 '''.format(stars[i][0],stars[i][1],stars[i][2])
     m = r'''\hline
 '''
 
     # returns 3 tables with SHA & Mer.pass for Venus, Mars, Jupiter and Saturn
     for i in range(3):
-        dt = date + timedelta(days=i)
+        dt = Date + timedelta(days=i)
         datestr = r'''{} {} {}'''.format(dt.strftime("%b"), dt.strftime("%d"), dt.strftime("%a"))
         m = m + '''\hline
 '''
         if config.tbls == "m":
             m = m + r'''& & \multicolumn{{1}}{{r|}}{{}}\\[-2.0ex]
 \multicolumn{{1}}{{|r}}{{\textbf{{{}}}}} 
 & \multicolumn{{1}}{{c}}{{\textbf{{SHA}}}} 
 & \multicolumn{{1}}{{r|}}{{\textbf{{Mer.pass}}}}\\
 '''.format(datestr)
         else:
             m = m + r'''& & \multicolumn{{1}}{{r|}}{{}}\\[-2.0ex]
 \textbf{{{}}} & \textbf{{SHA}} & \textbf{{Mer.pass}}\\
 '''.format(datestr)
-        datex = date + timedelta(days=i)
+        datex = Date + timedelta(days=i)
 
         if config.MULTIpr and config.WINpf:
             # multiprocess 'SHA + transit times' simultaneously
             objlist = ['venus', 'mars', 'jupiter', 'saturn']
             partial_func2 = partial(mp_planets_worker, datex, ts, spad)
 
             try:
@@ -633,31 +633,31 @@
 '''
     out = out + hp
     
     out = out + r'''\end{tabular}'''
     return out
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def mp_sunmoon_worker(date, ts, spad, n):
+def mp_sunmoon_worker(Date, ts, spad, n):
     # split the work by date into 3 separate days
-    sunmoondata = mp_sunmoon(date, ts, spad, n)      # ===>>> mp_nautical.py
+    sunmoondata = mp_sunmoon(Date, ts, spad, n)      # ===>>> mp_nautical.py
     return sunmoondata
 
-def sunmoontab(date, ts, spad):
+def sunmoontab(Date, ts, spad):
     # generates LaTeX table for sun and moon (traditional style)
     # OLD: \begin{tabular*}{0.54\textwidth}[t]{@{\extracolsep{\fill}}|c|rr|rrrrr|}
     # OLD note: 54% table width above removes "Overfull \hbox (1.65279pt too wide)"
     #                 and "Underfull \hbox (badness 10000)"
     # note: table may have different widths due to the 1st column (e.g. Fri versus Wed)
     # note: table may have different widths due to the 'v' column (e.g. 6.9' versus 15.3')
     # note: table may have different widths due to the 'd' column (e.g. 8.2' versus -13.9')
 
     if config.MULTIpr and config.WINpf:
-        # multiprocess sunmoontab values per "date" simultaneously
-        partial_func = partial(mp_sunmoon_worker, date, ts, spad)
+        # multiprocess sunmoontab values per "Date" simultaneously
+        partial_func = partial(mp_sunmoon_worker, Date, ts, spad)
 
         try:
             sunmoonlist = pool.map(partial_func, [nn for nn in range(3)], 1)
         except KeyboardInterrupt:
             print(msg0)
             sys.exit(0)
 
@@ -667,15 +667,15 @@
 \multicolumn{1}{c}{\normalsize{h}}& \multicolumn{2}{c}{\normalsize{Sun}} & \multicolumn{5}{c}{\normalsize{Moon}}\\
 '''
     n = 0
     while n < 3:
         tab = tab + r'''\hline
 \multicolumn{{1}}{{|c|}}{{\rule{{0pt}}{{2.6ex}}\textbf{{{}}}}} &\multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{Dec}}}}  & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\(\nu\)}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} & \multicolumn{{1}}{{c}}{{\textit{{d}}}} & \multicolumn{{1}}{{c|}}{{\textbf{{HP}}}}\\
 \hline\rule{{0pt}}{{2.6ex}}\noindent
-'''.format(date.strftime("%a"))
+'''.format(Date.strftime("%a"))
         # note: inline math mode is used to typeset the greek character 'nu'
 
         if config.MULTIpr and config.WINpf:
             ghas = sunmoonlist[n][0]
             decs = sunmoonlist[n][1]
             degs = sunmoonlist[n][2]
             gham = sunmoonlist[n][3]
@@ -685,18 +685,18 @@
             GHAupper = sunmoonlist[n][7]
             GHAlower = sunmoonlist[n][8]
             ghaSoD = sunmoonlist[n][9]
             ghaEoD = sunmoonlist[n][10]
             vmin = sunmoonlist[n][11]
             dmin = sunmoonlist[n][12]
         else:
-            date0 = date - timedelta(days=1)
-            ghas, decs, degs = sunGHA(date)
-            gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD = moonGHA(date)
-            vmin, dmin = moonVD(date0,date)
+            Date0 = Date - timedelta(days=1)
+            ghas, decs, degs = sunGHA(Date)
+            gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD = moonGHA(Date)
+            vmin, dmin = moonVD(Date0,Date)
 
         buildUPlists(n, ghaSoD, GHAupper, ghaEoD)
         buildLOWlists(n, ghaSoD, GHAupper, ghaEoD)
 
         h = 0
         if config.decf != '+':	# USNO format for Declination
             mlastNS = ''
@@ -739,36 +739,36 @@
 '''
                 if h < 23 and (h+1)%6 == 0:
                     lineterminator = r'''\\[2Pt]
 '''
                 tab = tab + line + lineterminator
                 h += 1
 
-        sds, dsm = sunSD(date)
-        sdmm = moonSD(date)
+        sds, dsm = sunSD(Date)
+        sdmm = moonSD(Date)
         tab = tab + r'''\hline
 \rule{{0pt}}{{2.4ex}} & \multicolumn{{1}}{{c}}{{SD = {}$'$}} & \multicolumn{{1}}{{c|}}{{\textit{{d}} = {}$'$}} & \multicolumn{{5}}{{c|}}{{SD = {}$'$}}\\
 \hline
 '''.format(sds,dsm,sdmm)
         if n < 2:
             # add space between tables...
             tab = tab + r'''\multicolumn{7}{c}{}\\[-1.5ex]'''
         n += 1
-        date += timedelta(days=1)
+        Date += timedelta(days=1)
     tab = tab + r'''\end{tabular}
 '''
     return tab
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
-def sunmoontabm(date, ts, spad):
+def sunmoontabm(Date, ts, spad):
     # generates LaTeX table for sun and moon (modern style)
 
     if config.MULTIpr and config.WINpf:
-        # multiprocess sunmoontab values per "date" simultaneously
-        partial_func = partial(mp_sunmoon_worker, date, ts, spad)
+        # multiprocess sunmoontab values per "Date" simultaneously
+        partial_func = partial(mp_sunmoon_worker, Date, ts, spad)
 
         try:
             sunmoonlist = pool.map(partial_func, [nn for nn in range(3)], 1)
         except KeyboardInterrupt:
             print(msg0)
             sys.exit(0)
 
@@ -782,15 +782,15 @@
 \multicolumn{5}{c}{\normalsize{Moon}}\\
 \cmidrule{2-3} \cmidrule{5-9}'''
     # note: \quad\quad above shifts all tables to the right (still within margins)
     n = 0
     while n < 3:
         tab = tab + r'''
 \multicolumn{{1}}{{c}}{{\textbf{{{}}}}} & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} & & \multicolumn{{1}}{{c}}{{\textbf{{GHA}}}} & \multicolumn{{1}}{{c}}{{\(\nu\)}} & \multicolumn{{1}}{{c}}{{\textbf{{Dec}}}} & \multicolumn{{1}}{{c}}{{\textit{{d}}}} & \multicolumn{{1}}{{c}}{{\textbf{{HP}}}}\\
-'''.format(date.strftime("%a"))
+'''.format(Date.strftime("%a"))
 
         if config.MULTIpr and config.WINpf:
             ghas = sunmoonlist[n][0]
             decs = sunmoonlist[n][1]
             degs = sunmoonlist[n][2]
             gham = sunmoonlist[n][3]
             decm = sunmoonlist[n][4]
@@ -799,18 +799,18 @@
             GHAupper = sunmoonlist[n][7]
             GHAlower = sunmoonlist[n][8]
             ghaSoD = sunmoonlist[n][9]
             ghaEoD = sunmoonlist[n][10]
             vmin = sunmoonlist[n][11]
             dmin = sunmoonlist[n][12]
         else:
-            date0 = date - timedelta(days=1)
-            ghas, decs, degs = sunGHA(date)
-            gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD = moonGHA(date)
-            vmin, dmin = moonVD(date0,date)
+            Date0 = Date - timedelta(days=1)
+            ghas, decs, degs = sunGHA(Date)
+            gham, decm, degm, HPm, GHAupper, GHAlower, ghaSoD, ghaEoD = moonGHA(Date)
+            vmin, dmin = moonVD(Date0,Date)
 
         buildUPlists(n, ghaSoD, GHAupper, ghaEoD)
         buildLOWlists(n, ghaSoD, GHAupper, ghaEoD)
 
         h = 0
         if config.decf != '+':	# USNO format for Declination
             mlastNS = ''
@@ -858,78 +858,78 @@
 '''.format(ghas[h],decs[h],gham[h],vmin[h],decm[h],dmin[h],HPm[h])
                 if group == 1:
                     tab = tab + r'''\rowcolor{LightCyan}
 '''
                 tab = tab + line
                 h += 1
 
-        sds, dsm = sunSD(date)
-        sdmm = moonSD(date)
+        sds, dsm = sunSD(Date)
+        sdmm = moonSD(Date)
         tab = tab + r'''\cmidrule{{2-3}} \cmidrule{{5-9}}
 \multicolumn{{1}}{{c}}{{}} & \multicolumn{{1}}{{c}}{{\footnotesize{{SD = {}$'$}}}} & 
 \multicolumn{{1}}{{c}}{{\footnotesize{{\textit{{d}} = {}$'$}}}} && \multicolumn{{5}}{{c}}{{\footnotesize{{SD = {}$'$}}}}\\
 \cmidrule{{2-3}} \cmidrule{{5-9}}
 '''.format(sds,dsm,sdmm)
         if n < 2:
             vsep = "[-1.5ex]"
             if config.pgsz == "Letter":
                 vsep = "[-2.0ex]"
             # add space between tables...
             tab = tab + r'''\multicolumn{{7}}{{c}}{{}}\\{}'''.format(vsep)
         n += 1
-        date += timedelta(days=1)
+        Date += timedelta(days=1)
     tab = tab + r'''\end{tabular}\quad\quad
 '''
     return tab
 
 # >>>>>>>>>>>>>>>>>>>>>>>>
 # create a list of 'moon above/below horizon' states per Latitude...
 #    None = unknown; True = above horizon (visible); False = below horizon (not visible)
 # The moon above/below status is stored at 3-day intervals, i.e. when multiprocessing "1st day",
 #    the previous day's status is stored here (except on the first day to be processed).
 #    Multiprocessing does not confuse the states as every three days it waits for all data.
 # Note: the size of moonvisible MUST equal the size of config.lat
 moonvisible = [None] * 31       # moonvisible[0] up to moonvisible[30]
 
-def mp_twilight_worker(date, ts, spad, lat):
+def mp_twilight_worker(Date, ts, spad, lat):
     #print(" mp_twilight_worker Start {}".format(lat))
     hemisph = 'N' if lat >= 0 else 'S'
-    twi = mp_twilight(date, lat, hemisph, ts, spad)       # ===>>> mp_nautical.py
+    twi = mp_twilight(Date, lat, hemisph, ts, spad)       # ===>>> mp_nautical.py
     #print(" mp_twilight_worker Finish {}".format(lat))
     return twi      # return list for all latitudes
 
-def mp_moonlight_worker(date, ts, spad, lat, mstate):
+def mp_moonlight_worker(Date, ts, spad, lat, mstate):
     #print(" mp_moonlight_worker Start  {}".format(lat))
     hemisph = 'N' if lat >= 0 else 'S'
-    ml = mp_moonrise_set(date, lat, mstate, hemisph, ts, spad)    # ===>>> mp_nautical.py
+    ml = mp_moonrise_set(Date, lat, mstate, hemisph, ts, spad)    # ===>>> mp_nautical.py
     #print(" mp_moonlight_worker Finish {}".format(lat))
     return ml       # return list for all latitudes
 
-def twilighttab(date, ts, spad, dfcm):
+def twilighttab(Date, ts, spad, dfcm):
     # returns the twilight and moonrise tables, finally EoT data
 
     if config.MULTIpr:
-        # multiprocess twilight values for "date+1" per latitude simultaneously
-        # date+1 to calculate for the second day (three days are printed on one page)
-        partial_func = partial(mp_twilight_worker, date+timedelta(days=1), ts, spad)
+        # multiprocess twilight values for "Date+1" per latitude simultaneously
+        # Date+1 to calculate for the second day (three days are printed on one page)
+        partial_func = partial(mp_twilight_worker, Date+timedelta(days=1), ts, spad)
 
         try:
             # RECOMMENDED: chunksize = 1
             listoftwi = pool.map(partial_func, config.lat, 1)
         except KeyboardInterrupt:
             print(msg0)
             sys.exit(0)
 
         for k in range(len(listoftwi)):
             config.stopwatch += listoftwi[k][6]     # accumulate multiprocess processing time
             del listoftwi[k][-1]
 
-        # multiprocess moonlight values for "date, date+1, date+2" per latitude simultaneously
+        # multiprocess moonlight values for "Date, Date+1, Date+2" per latitude simultaneously
         data = [(config.lat[ii], moonvisible[ii]) for ii in range(len(config.lat))]
-        partial_func2 = partial(mp_moonlight_worker, date, ts, spad)  # list of tuples
+        partial_func2 = partial(mp_moonlight_worker, Date, ts, spad)  # list of tuples
 
         try:
             # RECOMMENDED: chunksize = 1
             listmoon = pool.starmap(partial_func2, data, 1)
         except KeyboardInterrupt:
             print(msg0)
             sys.exit(0)
@@ -950,15 +950,16 @@
     #lat = [72,70,68,66,64,62,60,58,56,54,52,50,45,40,35,30,20,10,0, -10,-20,-30,-35,-40,-45,-50,-52,-54,-56,-58,-60]
     latNS = [72, 70, 58, 40, 10, -10, -50, -60]
     # OLD: \begin{tabular*}{0.45\textwidth}[t]{@{\extracolsep{\fill}}|r|ccc|ccc|}
 
     if config.tbls == "m":
     # The header begins with a thin empty row as top padding; and the top row with
     # bold text has some padding below it. This result gives a balanced impression.
-        tab = r'''\setlength{\tabcolsep}{5pt}  % default 6pt
+        tab = r'''\renewcommand{\arraystretch}{1.05}
+\setlength{\tabcolsep}{5pt}  % default 6pt
 \begin{tabular}[t]{|r|ccc|ccc|}
 \multicolumn{7}{c}{\normalsize{}}\\
 \hline
 \multicolumn{1}{|c|}{} & & & \multicolumn{1}{|c|}{} & \multicolumn{1}{c|}{} & & \multicolumn{1}{c|}{}\\[-2.0ex]
 \multicolumn{1}{|c|}{\multirow{2}{*}{\textbf{Lat.}}} & 
 \multicolumn{2}{c}{\footnotesize{\textbf{Twilight}}} & 
 \multicolumn{1}{|c|}{\multirow{2}{*}{\textbf{Sunrise}}} & 
@@ -992,29 +993,29 @@
 \multicolumn{1}{c|}{Naut.}\\
 \hline\rule{0pt}{2.6ex}\noindent
 '''
     lasthemisph = ""
     j = 5
     for lat in config.lat:
         hemisph = 'N' if lat >= 0 else 'S'
-        hs = ""
+        hsph = ""
         if (lat in latNS):
-            hs = hemisph
+            hsph = hemisph
             if j%6 == 0:
                 tab = tab + r'''\rule{0pt}{2.6ex}
 '''
         lasthemisph = hemisph
 
         if config.MULTIpr:
             twi = listoftwi[j-5]
         else:
             # day+1 to calculate for the second day (three days are printed on one page)
-            twi = twilight(date+timedelta(days=1), lat, hemisph)
+            twi = twilight(Date+timedelta(days=1), lat, hemisph)
 
-        line = r'''\textbf{{{}}}'''.format(hs) + " " + r'''{}$^\circ$'''.format(abs(lat))
+        line = r'''\textbf{{{}}}'''.format(hsph) + " " + r'''{}$^\circ$'''.format(abs(lat))
         line = line + r''' & {} & {} & {} & {} & {} & {} \\
 '''.format(twi[0],twi[1],twi[2],twi[3],twi[4],twi[5])
         tab = tab + line
         j += 1
     # add space between tables...
     tab = tab + r'''\hline\multicolumn{7}{c}{}\\[-1.5ex]
 '''
@@ -1030,15 +1031,15 @@
     else:
         tab = tab + r'''\hline
 \multicolumn{1}{|c|}{\rule{0pt}{2.4ex}\multirow{2}{*}{\textbf{Lat.}}} & 
 \multicolumn{3}{c|}{\textbf{Moonrise}} & 
 \multicolumn{3}{c|}{\textbf{Moonset}}\\
 '''
 
-    weekday = [date.strftime("%a"),(date+timedelta(days=1)).strftime("%a"),(date+timedelta(days=2)).strftime("%a")]
+    weekday = [Date.strftime("%a"),(Date+timedelta(days=1)).strftime("%a"),(Date+timedelta(days=2)).strftime("%a")]
     tab = tab + r'''\multicolumn{{1}}{{|c|}}{{}} & 
 \multicolumn{{1}}{{c}}{{{}}} & 
 \multicolumn{{1}}{{c}}{{{}}} & 
 \multicolumn{{1}}{{c|}}{{{}}} & 
 \multicolumn{{1}}{{c}}{{{}}} & 
 \multicolumn{{1}}{{c}}{{{}}} & 
 \multicolumn{{1}}{{c|}}{{{}}} \\
@@ -1047,35 +1048,35 @@
 
     moon = [0,0,0,0,0,0]
     moon2 = [0,0,0,0,0,0]
     lasthemisph = ""
     j = 5
     for lat in config.lat:
         hemisph = 'N' if lat >= 0 else 'S'
-        hs = ""
+        hsph = ""
         if (lat in latNS):
-            hs = hemisph
+            hsph = hemisph
             if j%6 == 0:
                 tab = tab + r'''\rule{0pt}{2.6ex}
 '''
         lasthemisph = hemisph
 
         if config.MULTIpr:
             moon = listmoon[j-5][0]
             moon2 = listmoon[j-5][1]
         else:
-            moon, moon2 = moonrise_set(date,lat,hemisph)
+            moon, moon2 = moonrise_set(Date,lat,hemisph)
 
         if not(double_events_found(moon,moon2)):
-            tab = tab + r'''\textbf{{{}}}'''.format(hs) + " " + r'''{}$^\circ$'''.format(abs(lat))
+            tab = tab + r'''\textbf{{{}}}'''.format(hsph) + " " + r'''{}$^\circ$'''.format(abs(lat))
             tab = tab + r''' & {} & {} & {} & {} & {} & {} \\
 '''.format(moon[0],moon[1],moon[2],moon[3],moon[4],moon[5])
         else:
 # print a row with two moonrise/moonset events on the same day & latitude
-            tab = tab + r'''\multirow{{2}}{{*}}{{\textbf{{{}}} {}$^\circ$}}'''.format(hs,abs(lat))
+            tab = tab + r'''\multirow{{2}}{{*}}{{\textbf{{{}}} {}$^\circ$}}'''.format(hsph,abs(lat))
 # top row...
             for k in range(len(moon)):
                 if moon2[k] != '--:--':
                     #tab = tab + r''' & {}'''.format(moon[k])
                     tab = tab + r''' & \colorbox{{khaki!45}}{{{}}}'''.format(moon[k])
                 else:
                     tab = tab + r''' & \multirow{{2}}{{*}}{{{}}}'''.format(moon[k])
@@ -1094,15 +1095,15 @@
     # add space between tables...
     tab = tab + r'''\hline\multicolumn{7}{c}{}\\[-1.5ex]
 '''
 
 # Equation of Time section ...........................................
     #------------------  if moon image displayed... ------------------
     if config.moonimg:
-        d = date
+        d = Date
         d1 = d + timedelta(days=1)
         d2 = d + timedelta(days=2)
         d3 = d + timedelta(days=3)
         age0, pct0 = moonage(d, d1)
         phase = moonphase(d1)       # moon phase (0:new to π:full to 2π:new)
         age2, pct2 = moonage(d2, d3)
         ages = '{}-{}'.format(age0,age2)
@@ -1138,15 +1139,15 @@
 '''.format(ages)
             tab = tab + r'''\multicolumn{1}{|c|}{} & \multicolumn{1}{c}{mm:ss} & \multicolumn{1}{c}{mm:ss} & 
 \multicolumn{1}{|c|}{hh:mm} & \multicolumn{1}{c}{hh:mm} & \multicolumn{1}{c}{hh:mm} & '''
             tab = tab + r'''\multicolumn{{1}}{{|c|}}{{{}}}\\
 \hline\rule{{0pt}}{{3.0ex}}\noindent
 '''.format(pcts)
 
-        d = date
+        d = Date
         for k in range(3):
             eq = equation_of_time(d,d + timedelta(days=1),UpperLists[k],LowerLists[k], False)
             if k == 0:
                 tab = tab + r'''%s & %s & %s & %s & %s & %s & ''' %(d.strftime("%d"),eq[0],eq[1],eq[2],eq[3],eq[4])
                 tab = tab + lunatikz(phase,dfcm)
             elif k == 1:
                 tab = tab + r'''{} & {} & {} & {} & {} & {} & \multicolumn{{1}}{{|c|}}{{}}\\
@@ -1180,15 +1181,15 @@
 \multicolumn{3}{c|}{\textbf{Sun}} & \multicolumn{3}{c|}{\textbf{Moon}}\\
 \multicolumn{1}{|c|}{} & \multicolumn{2}{c}{Eqn.of Time} & \multicolumn{1}{|c|}{Mer.} & \multicolumn{2}{c}{Mer.Pass.} & \multicolumn{1}{|c|}{}\\
 \multicolumn{1}{|c|}{} & \multicolumn{1}{c}{00\textsuperscript{h}} & \multicolumn{1}{c}{12\textsuperscript{h}} & \multicolumn{1}{|c|}{Pass} & \multicolumn{1}{c}{Upper} & \multicolumn{1}{c}{Lower} &\multicolumn{1}{|c|}{Age}\\
 \multicolumn{1}{|c|}{} & \multicolumn{1}{c}{mm:ss} & \multicolumn{1}{c}{mm:ss} & \multicolumn{1}{|c|}{hh:mm} & \multicolumn{1}{c}{hh:mm} & \multicolumn{1}{c}{hh:mm} &\multicolumn{1}{|c|}{}\\
 \hline\rule{0pt}{3.0ex}\noindent
 '''
 
-        d = date
+        d = Date
         for k in range(3):
             eq = equation_of_time(d,d + timedelta(days=1),UpperLists[k],LowerLists[k], True)
             if k == 2:
                 tab = tab + r'''{} & {} & {} & {} & {} & {} & {}({}\%) \\[0.3ex]
 '''.format(d.strftime("%d"),eq[0],eq[1],eq[2],eq[3],eq[4],eq[5],eq[6])
             else:
                 tab = tab + r'''{} & {} & {} & {} & {} & {} & {}({}\%) \\
@@ -1198,77 +1199,135 @@
 \end{tabular}'''
     return tab
 
 #----------------------
 #   page preparation
 #----------------------
 
-def doublepage(date, page1, ts, spad, dfcm):
+def doublepage(Date, page1, ts, spad, dfcm):
     # creates a doublepage (3 days) of the nautical almanac
 
     # time delta values for the initial date&time...
-    dut1, deltat = getDUT1(date)
+    dut1, deltat = getDUT1(Date)
     timeDUT1 = r"DUT1 = UT1-UTC = {:+.4f} sec\quad$\Delta$T = TT-UT1 = {:+.4f} sec".format(dut1, deltat)
 
-    find_new_moon(date)     # required for 'moonage' and 'equation_of_time"
+    LOfoot_IERSEOP = ""
+    if config.dt_IERSEOP != None:
+        # the IERS EOP data start date is 2nd January 1973
+        if Date + timedelta(days=2) >= date(1973, 1, 2):
+            LOfoot_IERSEOP = config.txtIERSEOP
+        if Date + timedelta(days=2) >= config.dt_IERSEOP:
+            LOfoot_IERSEOP = config.endIERSEOP
+        if Date > config.dt_IERSEOP:
+            LOfoot_IERSEOP = r'''\textbf{No IERS EOP prediction data available}'''
+
+    find_new_moon(Date)     # required for 'moonage' and 'equation_of_time"
     #from alma_skyfield import PreviousNewMoon, PreviousFullMoon, NextNewMoon, NextFullMoon
     #print("previous  new moon: %s" %PreviousNewMoon)
     #print("previous full moon: %s" %PreviousFullMoon)
     #print("next      new moon: %s" %NextNewMoon)
     #print("next     full moon: %s" %NextFullMoon)
 
-    page = ''
-    if not(page1):
-        page = r'''
-% ------------------ N E W   E V E N   P A G E ------------------
-\newpage
-\restoregeometry    % reset to even-page margins'''
-
     leftindent = ""
     rightindent = ""
     if config.tbls == "m":
         leftindent = "\quad"
         rightindent = "\hphantom{\quad}"
 
-    page = page + r'''
+# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+    if config.FANCYhd:
+        page = r'''
+% ------------------ N E W   E V E N   P A G E ------------------
+\newpage'''
+
+        page += r'''
+  \newgeometry{{nomarginpar, top={}, bottom={}, outer={}, inner={}, headsep={}, footskip={}}}'''.format(eventm,evenbm,evenom,evenim,evenhs,evenfs)
+# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+    else:   # old formatting
+        page = ''
+        if not(page1):
+            page = r'''
+% ------------------ N E W   E V E N   P A G E ------------------
+\newpage
+\restoregeometry    % reset to even-page margins'''
+# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+
+# ...........................................................
+    if config.FANCYhd:
+        page += r'''
 \sffamily
-\fancyhead[LE]{{{}\textsf{{\textbf{{{}, {}, {} UT ({}.,  {}.,  {}.)}}}}}}
-\setlength{{\headsep}}{{{}}} % [v2q]'''.format(leftindent, date.strftime("%B %d"), (date+timedelta(days=1)).strftime("%d"), (date+timedelta(days=2)).strftime("%d"), date.strftime("%a"), (date+timedelta(days=1)).strftime("%a"), (date+timedelta(days=2)).strftime("%a"), hds)
+\fancyhead[LE]{{{}\textsf{{\textbf{{{}, {}, {} UT ({}.,  {}.,  {}.)}}}}}}'''.format(leftindent, Date.strftime("%B %d"), (Date+timedelta(days=1)).strftime("%d"), (Date+timedelta(days=2)).strftime("%d"), Date.strftime("%a"), (Date+timedelta(days=1)).strftime("%a"), (Date+timedelta(days=2)).strftime("%a"))
 
-    page = page + r'''
+        page += r'''
 \begin{scriptsize}
 '''
+# ...........................................................
+    else:   # old formatting
+        page += r'''
+\sffamily
+\noindent
+{}\textbf{{{}, {}, {} UT ({}.,  {}.,  {}.)}}'''.format(leftindent,Date.strftime("%B %d"),(Date+timedelta(days=1)).strftime("%d"),(Date+timedelta(days=2)).strftime("%d"),Date.strftime("%a"),(Date+timedelta(days=1)).strftime("%a"),(Date+timedelta(days=2)).strftime("%a"))
+
+        if config.tbls == "m":
+            page += r'\\[1.0ex]'  # \par leaves about 1.2ex
+        else:
+            page += r'\\[0.7ex]'
+
+        page += r'''
+\begin{scriptsize}
+'''
+# ...........................................................
 
     if config.tbls == "m":
-        page = page + planetstabm(date,ts,spad)
+        page += planetstabm(Date,ts,spad)
     else:
-        page = page + planetstab(date,ts,spad) + r'''\enskip
+        page += planetstab(Date,ts,spad) + r'''\enskip
 '''
-    page = page + starstab(date,ts,spad)
-    str1 = r'''
+    page += starstab(Date,ts,spad)
+
+# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+    if config.FANCYhd:
+        str1 = r'''
+\end{scriptsize}
+% ------------------ N E W   O D D   P A G E ------------------
+\newpage'''
+        str1 += r'''
+  \newgeometry{{nomarginpar, top={}, bottom={}, inner={}, outer={}, headsep={}, footskip={}}}'''.format(oddtm,oddbm,oddim,oddom,oddhs,oddfs)
+        str1 += r'''
+\fancyhead[LO]{{\textsf{{\footnotesize{{{}}}}}}}
+\fancyhead[RO]{{\textsf{{\textbf{{{} to {} UT}}}}}}
+\fancyfoot[LO]{{\textsf{{\footnotesize{{{}}}}}}}
+\fancyfootoffset[R]{{0pt}}% recalculate \headwidth
+\setlength{{\headsep}}{{{}}}
+\begin{{scriptsize}}
+'''.format(timeDUT1, Date.strftime("%Y %B %d"), (Date+timedelta(days=2)).strftime("%b. %d"), LOfoot_IERSEOP, oddhs)
+# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+    else:   # old formatting
+        str1 = r'''
 \end{{scriptsize}}
 % ------------------ N E W   O D D   P A G E ------------------
 \newpage
 \newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}}}
-\fancyhead[LO]{{\textsf{{\footnotesize{{{}}}}}}}
-\fancyhead[RO]{{\textsf{{\textbf{{{} to {} UT}}}}}}
-\fancyheadoffset[RO]{{0pt}}  % bugfix - otherwise its shifted right
-\setlength{{\headsep}}{{{}}} % [v2q]
+\begin{{flushleft}}     % required so that \par works
+{{\footnotesize {}}}\hfill\textbf{{{} to {} UT}}
+\end{{flushleft}}\par
 \begin{{scriptsize}}
-'''.format(oddtm, oddbm, oddim, oddom, timeDUT1, date.strftime("%Y %B %d"), (date+timedelta(days=2)).strftime("%b. %d"), oddhds)
-    page = page + str1
+'''.format(oddtm, bm, oddim, oddom, timeDUT1, Date.strftime("%Y %B %d"), (Date+timedelta(days=2)).strftime("%b. %d"), rightindent)
+# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+
+    page += str1
+
     if config.tbls == "m":
-        page = page + sunmoontabm(date,ts,spad)
+        page += sunmoontabm(Date,ts,spad)
     else:
-        page = page + sunmoontab(date,ts,spad) + r'''\enskip
+        page += sunmoontab(Date,ts,spad) + r'''\enskip
 '''
-    page = page + twilighttab(date,ts,spad,dfcm)
+    page += twilighttab(Date,ts,spad,dfcm)
     # to avoid "Overfull \hbox" messages, leave a paragraph end before the end of a size change. (This may only apply to tabular* table style) See lines below...
-    page = page + r'''
-
+    page += r'''
 \end{scriptsize}'''
     return page
 
 #   This simple but effective function eliminates endless keyboard interrupts
 #   each time Ctrl-C is issued, while none actually kill the parent process
 #   ... and this causes the Command Prompt window (in Windows, MPmode=0) to hang.
 def init_worker():
@@ -1284,15 +1343,15 @@
         n = config.CPUcores
         if n > 12: n = 12   # use 12 cores maximum
         if (config.WINpf or config.MACOSpf) and n > 8: n = 8   # 8 maximum if Windows or Mac OS
         global pool
         pool = mp.Pool(n, init_worker)   # start 8 max. worker processes
 
     out = ''
-    page1 = True
+    page01 = True
     pmth = ''
     dpp = 3         # 3 days per page
     day1 = first_day
 
     if dtp == 0:        # if entire year
         year = first_day.year
         yr = year
@@ -1304,16 +1363,16 @@
                 #print(cmth, end='')
                 sys.stdout.write(cmth)	# next month
                 sys.stdout.flush()
                 pmth = cmth
             else:
                 sys.stdout.write('.')	# progress indicator
                 sys.stdout.flush()
-            out += doublepage(day1,page1,ts,spad,dfcm)
-            page1 = False
+            out += doublepage(day1,page01,ts,spad,dfcm)
+            page01 = False
             day1 += timedelta(days=3)
             year = day1.year
     elif dtp == -1:     # if entire month
         mth = first_day.month
         m = mth
         while mth == m:
             cmth = day1.strftime("%b ")
@@ -1323,229 +1382,487 @@
                 #print(cmth, end='')
                 sys.stdout.write(cmth)	# next month
                 sys.stdout.flush()
                 pmth = cmth
             else:
                 sys.stdout.write('.')	# progress indicator
                 sys.stdout.flush()
-            out += doublepage(day1,page1,ts,spad,dfcm)
-            page1 = False
+            out += doublepage(day1,page01,ts,spad,dfcm)
+            page01 = False
             day1 += timedelta(days=3)
             mth = day1.month
     else:           # print 'dtp' days beginning with first_day
         i = dtp   # don't decrement dtp
         while i > 0:
-            out += doublepage(day1,page1,ts,spad,dfcm)
-            page1 = False
+            out += doublepage(day1,page01,ts,spad,dfcm)
+            page01 = False
             i -= 3
             day1 += timedelta(days=3)
 
     if dtp <= 0:        # if Full Almanac for a whole month/year...
         print("\n")		# 2 x newline to terminate progress indicator
 
     if config.MULTIpr:
         pool.close()    # close all worker processes
         pool.join()
 
     return out
 
+def page1():
+    return r'''
+\setcounter{page}{1}    % otherwise it's 2
+    \noindent
+    {\large\textbf{Information in the data page footers}}\\[12pt]
+    Information pertaining to the IERS EOP data has been added to the odd data page footers if using MiKTeX or TeX Live (2020 or later). The International Earth Rotation Service (IERS) provides accurate data (updated weekly) on the Earth Orientation Parameters (EOP).\\[12pt]
+    Earth's speed of rotation is not constant, i.e. the day length fluctuates.\footnote{https://en.wikipedia.org/wiki/Day\_length\_fluctuations} This is due to \textit{internal torques} caused by relative movements and mass redistribution of Earth's core, mantle, oceans, atmosphere, and cryosphere.
+    This has an immediate impact on the GHA values of all celestial objects.\\[12pt]
+    The IERS monitors and measures several parameters taking the actual speed of Earth's rotation into account. Their measured data begins on 2nd Januaray 1973. Predictive data begins following the last day of (obtained) data and extends about 360 days into the future.
+    (The IERS results are published with a delay of about 18-hours between the date of publication and the last available date with measured EOP.\footnote{https://hpiers.obspm.fr/eoppc/bul/bulb/explanatory.html})
+    These Nautical Almanac daily pages take the (measured or predicted) UT1-UTC values into account providing highly accurate navigational data especially if the predictions are fairly recent.\\[12pt]
+    As long as either measured or predicted data is available the footer will show:\\
+    \textcolor{blue}{\textsf{IERS Earth Orientation data as of dd-mmm-yyyy}}\\
+    This indicates that IERS EOP data is in use - older dates are measured; newer dates are predictions.\\[12pt]
+    If the final date of IERS prediction data is on the current data page, the footer shows:\\
+    \textcolor{blue}{\textsf{IERS Earth Orientation predictions end dd-mmm-yyyy}}\\[12pt]
+    Pages with dates beyond the final date of IERS prediction data have the following footer:\\
+    \textcolor{blue}{\textbf{\textsf{No IERS EOP prediction data available}}}\\
+    Skyfield then defaults to using the $\Delta$T and leap second files that ship with Skyfield internally.\\[12pt]
+    The footers mentioned are only displayed as long as \textbf{\textsf{'useIERS = True'}} is set in \textit{config.py} to enable use of IERS EOP data.\\[20pt]
+    {\large\textbf{Brief historical overview}}\\[12pt]
+    The story begins with the XEphem astronomical library, which is declared 'end of life' by its author, Elwood Charles Downey, as no further updates are planned. He generously gave permission for use of XEphem code in Ephem (also known as Pyephem), an astronomical library authored by Brandon Rhodes.
+    Enno Rodegerdts (\textcolor{blue}{\textsf{https://sv-inua.net/}}) created the original Nautical Almanac 'daily pages' in Pyalmanac using Python 2 and LaTeX. After contacting him I obtained permission for its future enhancement and maintenance. Pyalmanac uses Ephem.\\[12pt]
+    Meanwhile Brandon Rhodes was working on a far more sophisticated astronomical library, Skyfield. This was 'state of the art' and clearly surpassed the 'Jean Meeus'-based Pyephem/Ephem. Skyfield uses NASA's NAIF (Navigation and Ancillary Information Facility) SPICE algorithms. The results agree with those from the HORIZONS System (\textit{operated by NASA JPL (Jet Propulsion Laboratory) SSD (Solar System Dynamics) group, not by NAIF}). This in turn implies that celestial positions calculated by Skyfield agree with those generated by the United States Naval Observatory and their \textit{Astronomical Almanac} to within 0.0005 arcseconds (half a milliarcsecond).\\[12pt]
+    Pyephem was then in 'maintenance mode'. Clearly Pyalmanac needed adaptation to use Skyfield, and thus SFalmanac was born. However its performance was poor regarding the calculation of 'events' such as: sunrise, sunset, moonrise, moonset, civil twilight start/end and nautical twilight start/end. An interim (faster) solution was required.\\[12pt]
+    Skyalmanac was the result: a hybrid application using Ephem to calculate 'events' and Skyfield for the rest. This was indeed much faster at the cost of poorer 'event' time data. It took a while to find a better solution: multiprocessing, which was built into SFalmanac. This now could compare to the execution times in Pyalmanac but with improved results.\\[12pt]    
+    New functionality was added to SFalmanac: lunar phase as a graphic; Lunar Distance tables and charts. The original Skyalmanac is deprecated and will soon be replaced with the latest SFalmanac code.
+    Since April 2019 \textcolor{blue}{\textsf{http://thenauticalalmanac.com}} has been publishing Celestial Navigation related material with software provided here.
+\newpage'''
+
 #--------------------------
 #   external entry point
 #--------------------------
 
 def almanac(first_day, dtp, ts, spad, df180, df360, dfcm):
+    # make almanac starting from first_day
     # dtp = 0 if for entire year; = -1 if for entire month; else days to print
 
+    if config.FANCYhd:
+        return makeNAnew(first_day, dtp, ts, spad, df180, df360, dfcm) # use the 'fancyhdr' package
+    else:
+        return makeNAold(first_day, dtp, ts, spad, df180, df360, dfcm) # use old formatting
+
+#   The following functions are intentionally separate functions.
+#   'makeEVold' is required for TeX Live 2019, which is the standard
+#   version in Ubuntu 20.04 LTS which expires in April 2030.
+
+def hdrNAnew(first_day, dtp, tm1, bm1, lm1, rm1, vsep1, vsep2, df180, df360):
+    # build the front page
+
+    tex = r'''
+\pagestyle{frontpage}
+    \begin{titlepage}
+    \begin{center}
+    \textsc{\Large Generated using Skyfield}\\
+    \large http://rhodesmill.org/skyfield/\\[0.7cm]'''
+    
+    if config.dockerized:   # DOCKER ONLY
+        df180 = "../A4chart0-180_P.pdf"
+        df360 = "../A4chart180-360_P.pdf"
+
+    tex += r'''
+    % TRIM values: left bottom right top
+    \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\[0.3cm]
+    \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\'''.format(df180,df360)
+
+    tex += r'''[{}]
+    \textsc{{\huge The Nautical Almanac}}\\[{}]'''.format(vsep1,vsep2)
+
+    if dtp == 0:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(first_day.year)
+    elif dtp == -1:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(first_day.strftime("%B %Y"))
+    elif dtp > 1:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdates(first_day,first_day+timedelta(days=dtp-1)))
+    else:
+        tex += r'''
+    \HRule \\[0.5cm]
+    {{ \Huge \bfseries {}}}\\[0.2cm]
+    \HRule \\'''.format(fmtdate(first_day))
+
+    tex += r'''
+    \begin{center}\begin{tabular}[t]{rl}
+    \large\emph{Author:} & \large Andrew \textsc{Bauer}\\
+    \large\emph{Original concept from:} & \large Enno \textsc{Rodegerdts}\\
+    \end{tabular}\end{center}'''
+
+    tex += r'''
+    {\large \today}
+    \HRule \\[0.2cm]
+    \end{center}
+    \begin{description}[leftmargin=5.5em,style=nextline]\footnotesize
+    \item[Disclaimer:] These are computer generated tables - use them at your own risk.
+    The accuracy has been randomly checked with JPL HORIZONS System, but cannot be guaranteed.
+    The author claims no liability for any consequences arising from use of these tables.
+    Besides, this publication only contains the 'daily pages' of the Nautical Almanac: an official version of the Nautical Almanac is indispensable.
+    \end{description}
+\end{titlepage}
+\pagestyle{page1}'''
+
+    tex += page1()
+
+    return tex
+
+def makeNAnew(first_day, dtp, ts, spad, df180, df360, dfcm):
     # make almanac starting from first_day
-    global tm, bm, hds, oddim, oddom, oddtm, oddbm, oddhds
-    year = first_day.year
-    mth = first_day.month
-    day = first_day.day
+    global oddtm,  oddbm,  oddim,  oddom,  oddhs,  oddfs  # required by doublepage
+    global eventm, evenbm, evenim, evenom, evenhs, evenfs
+
+    # NOTE: 'bm' (bottom margin) is an unrealistic value used only to determine the vertical size of 'body' (textheight), which must be large enough to include all the tables. 'tm' (top margin) and 'hds' (headsep) determine the top of body. Note: 'fs' (footskip) does not position the footer.
 
     # page size specific parameters
-    # NOTE: 'bm' (bottom margin) is an unrealistic value used only to determine the vertical size of 'body' (textheight), which must be large enough to include all the tables. 'tm' (top margin) and 'hds' (headsep) determine the top of body. Finally use 'fs' (footskip) to position the footer.
     if config.pgsz == "A4":
         # A4 ... pay attention to the limited page width
         paper = "a4paper"
         # title page...
         vsep1 = "1.5cm"
         vsep2 = "1.0cm"
         tm1 = "21mm"
         bm1 = "15mm"
         lm1 = "10mm"
         rm1 = "10mm"
-        # data pages...
-        tm = "34.5mm"       # data pages... was "21mm" [v2q]
-        bm = "10mm"         # was "18mm" [v2q]
-        hds = "1.8pt"       # headsep  (page 3 onwards) [v2q]
-        fs = "36pt"         # footskip (page 3 onwards) [v2q]
         # even data pages...
-        im = "10mm"         # inner margin (right side on even pages)
-        om = "9mm"          # outer margin (left side on even pages)
+        eventm = "25mm"     # data pages... was "21mm"
+        evenbm = "16mm"     # was "18mm"
+        evenhs = "1.8pt"    # headsep  (page 2 onwards)
+        evenfs = "12pt"     # footskip (page 2 onwards)
+        evenim = "10mm"     # inner margin (right side on even pages)
+        evenom = "9mm"      # outer margin (left side on even pages)
         # odd data pages...
-        oddtm = "34.5mm"    # was "21mm" [v2q]
-        oddbm = "12mm"      # was "18mm" [v2q]
-        oddhds = "6.5pt"    # headsep  (page 3 onwards) [v2q]
+        oddtm = "27.5mm"    # was "21mm"
+        oddbm = "16mm"      # was "18mm"
+        oddhs = "6.5pt"     # headsep  (page 3 onwards)
+        oddfs = "12pt"      # footskip (page 3 onwards)
         oddim = "14mm"      # inner margin (left side on odd pages)
         oddom = "11mm"      # outer margin (right side on odd pages)
         if config.tbls == "m":
-            tm = "23.5mm"   # was "10mm" [v2q]
-            bm = "8mm"      # was "15mm" [v2q]
-            hds = "3.0pt"   # headsep  (page 3 onwards) [v2q]
-            fs = "36pt"     # footskip (page 3 onwards) [v2q]
-            im = "10mm"
-            om = "10mm"
+            # even data pages...
+            eventm = "15.8mm"   # was "10mm"
+            evenbm = "12mm"     # was "15mm"
+            evenhs = "3.0pt"    # headsep  (page 2 onwards)
+            evenfs = "12pt"     # footskip (page 2 onwards)
+            evenim = "10mm"
+            evenom = "10mm"
             # odd data pages...
-            oddtm = "23.5mm"    # was "10mm" [v2q]
-            oddbm = "8mm"       # was "15mm" [v2q]
-            oddhds = "4.6pt"    # headsep  (page 3 onwards) [v2q]
+            oddtm = "16mm"      # was "10mm"
+            oddbm = "13mm"      # was "15mm"
+            oddhs = "4.6pt"     # headsep  (page 3 onwards)
+            oddfs = "12pt"      # footskip (page 3 onwards)
             oddim = "14mm"
             oddom = "11mm"
     else:
         # LETTER ... pay attention to the limited page height
         paper = "letterpaper"
         # title page...
         vsep1 = "0.8cm"
         vsep2 = "0.7cm"
         tm1 = "12mm"
         bm1 = "15mm"
         lm1 = "12mm"
         rm1 = "12mm"
-        # data pages...
-        tm = "25.8mm"       # data pages... was "12.2mm" [v2q]
-        bm = "5mm"          # was "13mm" [v2q]
-        hds = "1.5pt"       # headsep  (page 3 onwards) [v2q]
-        fs = "28pt"         # footskip (page 3 onwards) [v2q]
         # even data pages...
-        im = "13mm"         # inner margin (right side on even pages)
-        om = "13mm"         # outer margin (left side on even pages)
+        eventm = "17.2mm"   # data pages... was "12.2mm"
+        evenbm = "12mm"     # was "13mm"
+        evenhs = "1.5pt"    # headsep  (page 2 onwards)
+        evenfs = "12pt"     # footskip (page 2 onwards)
+        evenim = "13mm"     # inner margin (right side on even pages)
+        evenom = "13mm"     # outer margin (left side on even pages)
         # odd data pages...
-        oddtm = "25.8mm"    # was "12.2mm" [v2q]
-        oddbm = "6.5mm"     # was "13mm" [v2q]
-        oddhds = "6.1pt"    # headsep  (page 3 onwards) [v2q]
+        oddtm = "19mm"      # was "12.2mm"
+        oddbm = "12mm"      # was "13mm"
+        oddhs = "6.1pt"     # headsep  (page 3 onwards)
+        oddfs = "12pt"      # footskip (page 3 onwards)
         oddim = "14mm"      # inner margin (left side on odd pages)
         oddom = "11mm"      # outer margin (right side on odd pages)
         if config.tbls == "m":
-            tm = "17.6mm"   # was "4mm" [v2q]
-            bm = "2mm"      # was "8mm" [v2q]
-            hds = "2.8pt"   # headsep  (page 3 onwards) [v2q]
-            fs = "36pt"     # footskip (page 3 onwards) [v2q]
-            im = "13mm"
-            om = "13mm"
-            # odd data pages...
-            oddtm = "17.6mm"    # was "4mm" [v2q]
-            oddbm = "2mm"       # was "8mm" [v2q]
-            oddhds = "2.5pt"    # headsep  (page 3 onwards) [v2q]
-            oddim = "14mm"
-            oddom = "14mm"
+            # even data pages...
+            eventm = "9.4mm"    # was "4mm"
+            evenbm = "8mm"      # was "8mm"
+            evenhd = "2.8pt"    # headsep  (page 2 onwards)
+            evenfs = "12pt"     # footskip (page 2 onwards)
+            evenim = "12.5mm"
+            evenom = "12.5mm"
+            # odd data pages... use 26.06.2024 as a testcase
+            oddtm = "8mm"       # was "4mm"
+            oddbm = "8mm"       # was "8mm"
+            oddhs = "0pt"       # headsep  (page 3 onwards)
+            oddfs = "12pt"      # footskip (page 3 onwards)
+            oddim = "13mm"
+            oddom = "13mm"
+
+#------------------------------------------------------------------------------
+#   This edition employs the 'fancyhdr' v4.0.3 package
+#   CAUTION: do not use '\newgeometry' & '\restoregeometry' as advised here:
+#   https://tex.stackexchange.com/questions/247972/top-margin-fancyhdr
+#------------------------------------------------------------------------------
 
-    alm = r'''\documentclass[10pt, twoside, {}]{{report}}'''.format(paper)
+    tex = r'''\documentclass[10pt, twoside, {}]{{report}}'''.format(paper)
 
-    alm = alm + r'''
+    tex += r'''
 %\usepackage[utf8]{inputenc}
 \usepackage[english]{babel}
 \usepackage{fontenc}
 \usepackage{enumitem} % used to customize the {description} environment'''
 
     # to troubleshoot add "showframe, verbose," below:
-    alm = alm + r'''
-\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm,bm,im,om)
+    tex += r'''
+\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm1,bm1,lm1,rm1)
+
+    # define page styles
+    tex += r'''
+%------------ page styles ------------
+\usepackage{fancyhdr}
+\renewcommand{\headrulewidth}{0pt}
+\renewcommand{\footrulewidth}{0pt}
+\fancypagestyle{frontpage}{
+  \fancyhf{}% clear all header and footer fields
+}
+\fancypagestyle{page1}[frontpage]{
+  \fancyfootoffset[R]{0pt}% recalculate \headwidth
+  \cfoot{\centerline{Page \thepage}}
+\setlength{\footskip}{12pt}
+}
+\fancypagestyle{datapage}[page1]{'''
+    tex += r'''
+  \fancyfoot[LE,RO]{\textsf{\footnotesize{https://pypi.org/project/sfalmanac/}}}
+} %-----------------------------------'''
 
     if config.tbls == "m":
-        alm = alm + r'''
+        tex += r'''
 \usepackage[table]{xcolor}
 % [table] option loads the colortbl package for coloring rows, columns, and cells within tables.
 \definecolor{LightCyan}{rgb}{0.88,1,1}
-\definecolor{darknight}{rgb}{0.18, 0.27, 0.33}
 \usepackage{booktabs}'''
     else:
-        alm = alm + r'''
+        tex += r'''
 \usepackage{xcolor}  % highlight double moon events on same day'''
 
     # Note: \DeclareUnicodeCharacter is not compatible with some versions of pdflatex
-    alm = alm + r'''
+    tex += r'''
 \definecolor{darknight}{rgb}{0.18, 0.27, 0.33}
 \definecolor{khaki}{rgb}{0.76, 0.69, 0.57}
 \usepackage{multirow}
 \newcommand{\HRule}{\rule{\linewidth}{0.5mm}}
-\usepackage{fancyhdr}   % [v2q]
-\pagestyle{fancy}       % [v2q]
-\renewcommand{\headrulewidth}{0pt}  % [v2q]
-\setlength{\footskip}{15pt}
 \usepackage[pdftex]{graphicx}	% for \includegraphics
 \usepackage{tikz}				% for \draw  (load after 'graphicx')
 %\showboxbreadth=50  % use for logging
 %\showboxdepth=50    % use for logging
 %\DeclareUnicodeCharacter{00B0}{\ensuremath{{}^\circ}}
 \setlength\fboxsep{1.5pt}       % ONLY used by \colorbox in alma_skyfield.py
 \begin{document}'''
 
-    alm = alm + r'''
+    if not config.DPonly:
+        tex += hdrNAnew(first_day,dtp,tm1,bm1,lm1,rm1,vsep1,vsep2,df180,df360)
+
+# NOTE: the first data page must be even (otherwise there's no header)
+    tex += r'''
+\pagestyle{datapage}  % the default page style for the document
+\setcounter{page}{2}'''
+
+    tex += pages(first_day,dtp,ts,spad,dfcm)
+    tex += r'''
+\end{document}'''
+    return tex
+
+# ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===
+# ===   ===   ===   ===   O L D   F O R M A T T I N G   ===   ===   ===   ===
+# ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===   ===
+
+def hdrNAold(first_day, dtp, tm1, bm1, lm1, rm1, vsep1, vsep2, df180, df360):
+    # build the front page
+
+    tex = r'''
 % for the title page only...
 \newgeometry{{nomarginpar, top={}, bottom={}, left={}, right={}}}'''.format(tm1,bm1,lm1,rm1)
 
-    alm = alm + r'''
+    tex += r'''
     \begin{titlepage}
     \begin{center}
     \textsc{\Large Generated using Skyfield}\\
     \large http://rhodesmill.org/skyfield/\\[0.7cm]'''
     
     if config.dockerized:   # DOCKER ONLY
         df180 = "../A4chart0-180_P.pdf"
         df360 = "../A4chart180-360_P.pdf"
 
-    alm = alm + r'''
+    tex += r'''
     % TRIM values: left bottom right top
     \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\[0.3cm]
     \includegraphics[clip, trim=12mm 20cm 12mm 21mm, width=0.92\textwidth]{{{}}}\\'''.format(df180,df360)
 
-    alm = alm + r'''[{}]
+    tex += r'''[{}]
     \textsc{{\huge The Nautical Almanac}}\\[{}]'''.format(vsep1,vsep2)
 
     if dtp == 0:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
-    \HRule \\'''.format(year)
+    \HRule \\'''.format(first_day.year)
     elif dtp == -1:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
     \HRule \\'''.format(first_day.strftime("%B %Y"))
     elif dtp > 1:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
     \HRule \\'''.format(fmtdates(first_day,first_day+timedelta(days=dtp-1)))
     else:
-        alm = alm + r'''
+        tex += r'''
     \HRule \\[0.5cm]
     {{ \Huge \bfseries {}}}\\[0.2cm]
     \HRule \\'''.format(fmtdate(first_day))
 
-    alm = alm + r'''
+    tex += r'''
     \begin{center}\begin{tabular}[t]{rl}
     \large\emph{Author:} & \large Andrew \textsc{Bauer}\\
     \large\emph{Original concept from:} & \large Enno \textsc{Rodegerdts}\\
     \end{tabular}\end{center}'''
 
-    alm = alm + r'''
+    tex += r'''
     {\large \today}
     \HRule \\[0.2cm]
     \end{center}
     \begin{description}[leftmargin=5.5em,style=nextline]\footnotesize
     \item[Disclaimer:] These are computer generated tables - use them at your own risk.
     The accuracy has been randomly checked with JPL HORIZONS System, but cannot be guaranteed.
     The author claims no liability for any consequences arising from use of these tables.
     Besides, this publication only contains the 'daily pages' of the Nautical Almanac: an official version of the Nautical Almanac is indispensable.
     \end{description}
-\end{titlepage}
-% DO NOT SPECIFY lfoot, cfoot & rfoot BEFORE restoregeometry!
-\restoregeometry    % so it does not affect the rest of the pages
-\lfoot{\textsf{\footnotesize{https://thenauticalalmanac.com/}}}
-\cfoot{\centerline{Page \thepage}}
-\rfoot{\textsf{\footnotesize{https://pypi.org/project/sfalmanac/}}}'''
+\end{titlepage}'''
+
+    tex += page1()
+
+    tex += r'''
+\restoregeometry    % so it does not affect the rest of the pages'''
+
+    return tex
+
+def makeNAold(first_day, dtp, ts, spad, df180, df360, dfcm):
+    # make almanac starting from first_day
+    global tm, bm, oddtm, oddim, oddom     # required by doublepage
+
+    # page size specific parameters
+    if config.pgsz == "A4":
+        # A4 ... pay attention to the limited page width
+        paper = "a4paper"
+        vsep1 = "1.5cm"
+        vsep2 = "1.0cm"
+        tm1 = "21mm"    # title page...
+        bm1 = "15mm"
+        lm1 = "10mm"
+        rm1 = "10mm"
+        tm = "21mm"     # data pages...
+        bm = "18mm"
+        # even data pages...
+        im = "10mm"     # inner margin (right side on even pages)
+        om = "9mm"      # outer margin (left side on even pages)
+        # odd data pages...
+        oddtm = tm
+        oddim = "14mm"  # inner margin (left side on odd pages)
+        oddom = "11mm"  # outer margin (right side on odd pages)
+        if config.tbls == "m":
+            # even data pages...
+            tm = "10mm"
+            bm = "15mm"
+            im = "10mm"
+            om = "10mm"
+            # odd data pages...
+            oddtm = tm
+            oddim = "14mm"
+            oddom = "11mm"
+    else:
+        # LETTER ... pay attention to the limited page height
+        paper = "letterpaper"
+        vsep1 = "0.8cm"
+        vsep2 = "0.7cm"
+        tm1 = "12mm"    # title page...
+        bm1 = "15mm"
+        lm1 = "12mm"
+        rm1 = "12mm"
+        tm = "12.2mm"   # data pages...
+        bm = "13mm"
+        # even data pages...
+        im = "13mm"     # inner margin (right side on even pages)
+        om = "13mm"     # outer margin (left side on even pages)
+        # odd data pages...
+        oddtm = tm
+        oddim = "14mm"  # inner margin (left side on odd pages)
+        oddom = "11mm"  # outer margin (right side on odd pages)
+        if config.tbls == "m":
+            # even data pages...
+            tm = "4mm"
+            bm = "8mm"
+            im = "12mm"
+            om = "12mm"
+            # odd data pages... use 26.06.2024 & 18.06.2025 as testcases
+            oddtm = "2.6mm"
+            oddim = "14mm"
+            oddom = "14mm"
+
+    tex = r'''\documentclass[10pt, twoside, {}]{{report}}'''.format(paper)
+
+    tex += r'''
+%\usepackage[utf8]{inputenc}
+\usepackage[english]{babel}
+\usepackage{fontenc}
+\usepackage{enumitem} % used to customize the {description} environment'''
+
+    # to troubleshoot add "showframe, verbose," below:
+    tex += r'''
+\usepackage[nomarginpar, top={}, bottom={}, left={}, right={}]{{geometry}}'''.format(tm,bm,im,om)
+
+    if config.tbls == "m":
+        tex += r'''
+\usepackage[table]{xcolor}
+% [table] option loads the colortbl package for coloring rows, columns, and cells within tables.
+\definecolor{LightCyan}{rgb}{0.88,1,1}
+\usepackage{booktabs}'''
+    else:
+        tex += r'''
+\usepackage{xcolor}  % highlight double moon events on same day'''
+
+    # Note: \DeclareUnicodeCharacter is not compatible with some versions of pdflatex
+    tex += r'''
+\definecolor{darknight}{rgb}{0.18, 0.27, 0.33}
+\definecolor{khaki}{rgb}{0.76, 0.69, 0.57}
+\usepackage{multirow}
+\newcommand{\HRule}{\rule{\linewidth}{0.5mm}}
+\setlength{\footskip}{15pt}
+\usepackage[pdftex]{graphicx}	% for \includegraphics
+\usepackage{tikz}				% for \draw  (load after 'graphicx')
+%\showboxbreadth=50  % use for logging
+%\showboxdepth=50    % use for logging
+%\DeclareUnicodeCharacter{00B0}{\ensuremath{{}^\circ}}
+\setlength\fboxsep{1.5pt}       % ONLY used by \colorbox in alma_skyfield.py
+\begin{document}'''
+
+    if not config.DPonly:
+        tex += hdrNAold(first_day,dtp,tm1,bm1,lm1,rm1,vsep1,vsep2,df180,df360)
+
+    # Nautical Almanac pages begin with a left page (page 2)
+    tex += r'''
+\setcounter{page}{2}'''
 
-    alm = alm + pages(first_day,dtp,ts,spad,dfcm)
-    alm = alm + '''
+    tex += pages(first_day,dtp,ts,spad,dfcm)
+    tex += r'''
 \end{document}'''
-    return alm
+    return tex
```

### Comparing `sfalmanac-1.8.2/sfalmanac.egg-info/PKG-INFO` & `sfalmanac-1.9/sfalmanac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sfalmanac
-Version: 1.8.2
-Summary: Creates the daily pages of a Nautical Almanac using Skyfield (and Ephem)
+Version: 1.9
+Summary: Creates the daily pages of a Nautical Almanac using Skyfield
 Home-page: https://github.com/aendie/SFalmanac-Py3
 Author: Andrew Bauer
 Author-email: aendie.bauer@gmail.com
 License: GPL-3.0 License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -54,49 +54,52 @@
 Windows 10 uses up to 8 threads; Linux uses up to 12 threads in parallel. Testing was performed on a PC with an AMD Ryzen 7 3700X 8-Core (16 threads) Processor. Windows & Mac OS spawn new processes; Linux forks new processes (the code is compatible with both techniques and will also run on CPUs with fewer cores/threads).
 
 This performance gain shows that there is practically no justification in using Skyalmanac, which was an interim solution to overcome the poor single-processing performance in SFalmanac at the cost of marginally poorer accuracy in event times (sunset/twilight/sunrise; moonrise/moonset).
 
 Quick Overview
 --------------
 
-This is the **PyPI edition** of `SFalmanac-Py3 <https://github.com/aendie/SFalmanac-Py3>`_ (a Changelog can be viewed here). Version numbering here started from 1.0 as the previous well-tested versions that are on github since 2015 were never published in PyPI. Version numbering follows the scheme *Major.Minor.Patch*, whereby the *Patch* number represents some small correction to the intended release.
+This is the **PyPI edition** of `SFalmanac-Py3 <https://github.com/aendie/SFalmanac-Py3>`_ (a Changelog can be viewed here). Version numbering follows the scheme *Major.Minor.Patch*, whereby the *Patch* number represents some small correction to the intended release.
+
+| **NOTE:** Version numbering in PyPI restarted from 1.0 as the previous well-tested versions that exist since early 2019 were never published in PyPI.
 
 Two astronomical libraries are employed: `Skyfield <https://rhodesmill.org/skyfield/>`_ and `Ephem <https://rhodesmill.org/pyephem/>`_.
 Ephem is only used to calculate a few planet magnitudes (Venus and Jupiter are available in Skyfield).
 
 SFalmanac uses the Hipparcos catalog as its star database. If a current version of Skyfield (>= 1.31) is used, you have two options (which one, you specify by manually editing *config.py*):
 
 * if "useIERS = False", the built-in UT1 tables in the installed version of Skyfield will be employed.
-* if "useIERS = True", for optimal accuracy (especially for all GHA data), Earth orientation data from IERS (International Earth Rotation and Reference Systems Service) is downloaded and then used until it 'expires'. It expires after a chosen number of days (also specifiable in *config.py*). Note that IERS specifies the range of Earth Orientation Parameter (EOP) data currently as "from 2nd January 1973 to 1st October 2023 (continuously advancing)". Refer to the `IERS web site <https://www.iers.org/IERS/EN/Home/home_node.html>`_ for current information.
+* if "useIERS = True", for optimal accuracy (especially for all GHA data), Earth orientation data from IERS (International Earth Rotation and Reference Systems Service) is downloaded and then used until it 'expires'. It expires after a chosen number of days (also specifiable in *config.py*). Note that IERS specifies the range of Earth Orientation Parameter (EOP) data currently as "from 2nd January 1973 to 22nd October 2023 (continuously advancing)". Refer to the `IERS web site <https://www.iers.org/IERS/EN/Home/home_node.html>`_ for current information.
 
 If your Skyfield version is somewhat older (<= 1.30), Skyfield will have downloaded the older files it then used: *deltat.data, deltat.preds* and *Leap_Second.dat*, which are slightly less accurate than the IERS EOP data (which is updated weekly!).
 
 Software Requirements
 =====================
 
 |
 | Nearly all of the astronomical computation is done by the free Skyfield library.
 | Typesetting is done typically by MiKTeX or TeX Live.
 | Here are the requirements/recommendations:
 
 * `python <https://www.python.org/downloads/>`_ >= 3.4 (the latest version is recommended)
 * `skyfield <https://pypi.org/project/skyfield/>`__ >= v1.15 (the latest is recommended; see the `Skyfield Changelog <https://rhodesmill.org/skyfield/installation.html#changelog>`_)
 * `pandas <https://pandas.pydata.org/>`_ >= 1.0 (to decode the Hipparcos catalog)
-* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6 (required for some planet magnitudes)
+* `ephem <https://pypi.org/project/ephem/>`__ = 4.1 (required for some planet magnitudes)
 * `MiKTeX <https://miktex.org/>`_ |nbsp| |nbsp| or |nbsp| |nbsp| `TeX Live <http://www.tug.org/texlive/>`_
 
 Installation
 ============
 
 Install a TeX/LaTeX program on your operating system so that 'pdflatex' is available.
 
 Ensure that the `pip Python installer tool <https://pip.pypa.io/en/latest/installation/>`_ is installed.
 Then ensure that old versions of PyEphem, Ephem and SFalmanac are not installed before installing SFalmanac from PyPI as follows::
 
   python -m pip uninstall pyephem ephem sfalmanac
+  python -m pip install ephem==4.1
   python -m pip install sfalmanac
 
 Installing SFalmanac ensures that Ephem, Skyfield and Pandas (and their dependencies) are also installed. If previous versions of SFalmanac were installed, consider upgrading Skyfield and Pandas thus::
 
   python -m pip install --upgrade skyfield pandas
 
 Thereafter run it with::
```

### Comparing `sfalmanac-1.8.2/sfalmanac.egg-info/SOURCES.txt` & `sfalmanac-1.9/sfalmanac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

