# Comparing `tmp/skyalmanac-1.3.8.tar.gz` & `tmp/skyalmanac-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyalmanac-1.3.8.tar", last modified: Sat Apr 23 16:01:51 2022, max compression
+gzip compressed data, was "skyalmanac-1.3.9.tar", last modified: Sun Jul  3 18:21:15 2022, max compression
```

## Comparing `skyalmanac-1.3.8.tar` & `skyalmanac-1.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-04-23 16:01:51.085471 skyalmanac-1.3.8/
--rw-rw-rw-   0        0        0    35149 2019-09-02 18:38:48.000000 skyalmanac-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     6933 2022-04-23 16:01:51.086472 skyalmanac-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5909 2021-05-06 14:28:09.000000 skyalmanac-1.3.8/README.rst
--rw-rw-rw-   0        0        0      115 2021-02-15 20:39:50.000000 skyalmanac-1.3.8/pyproject.toml
--rw-rw-rw-   0        0        0     1091 2022-04-23 16:01:51.086472 skyalmanac-1.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-04-23 16:01:51.015956 skyalmanac-1.3.8/skyalmanac/
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.8/skyalmanac/__init__.py
--rw-rw-rw-   0        0        0    11080 2022-04-23 16:00:08.000000 skyalmanac-1.3.8/skyalmanac/__main__.py
-drwxrwxrwx   0        0        0        0 2022-04-23 16:01:51.020956 skyalmanac-1.3.8/skyalmanac/astro-data/
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.8/skyalmanac/astro-data/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-23 16:01:51.033263 skyalmanac-1.3.8/skyalmanac/data/
--rw-rw-rw-   0        0        0   130123 2020-02-28 19:27:47.000000 skyalmanac-1.3.8/skyalmanac/data/A4chart0-180_P.pdf
--rw-rw-rw-   0        0        0   128042 2020-02-28 19:34:01.000000 skyalmanac-1.3.8/skyalmanac/data/A4chart180-360_P.pdf
--rw-rw-rw-   0        0        0    24577 2019-02-02 20:33:26.000000 skyalmanac-1.3.8/skyalmanac/data/Ra.JPG
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.8/skyalmanac/data/__init__.py
--rw-rw-rw-   0        0        0   133928 2020-02-12 20:36:26.000000 skyalmanac-1.3.8/skyalmanac/data/croppedmoon.png
-drwxrwxrwx   0        0        0        0 2022-04-23 16:01:51.073471 skyalmanac-1.3.8/skyalmanac/docs/
--rw-rw-rw-   0        0        0  1743971 2020-03-06 07:11:00.000000 skyalmanac-1.3.8/skyalmanac/docs/Explanation.pdf
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.8/skyalmanac/docs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-23 16:01:51.085471 skyalmanac-1.3.8/skyalmanac/lib/
--rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.8/skyalmanac/lib/__init__.py
--rw-rw-rw-   0        0        0    25143 2022-04-22 17:40:01.000000 skyalmanac-1.3.8/skyalmanac/lib/alma_ephem.py
--rw-rw-rw-   0        0        0    42684 2022-04-23 15:31:38.000000 skyalmanac-1.3.8/skyalmanac/lib/alma_skyfield.py
--rw-rw-rw-   0        0        0     2357 2022-04-22 17:40:35.000000 skyalmanac-1.3.8/skyalmanac/lib/config.py
--rw-rw-rw-   0        0        0    11450 2021-05-01 16:23:57.000000 skyalmanac-1.3.8/skyalmanac/lib/increments.py
--rw-rw-rw-   0        0        0    16645 2022-04-22 17:40:56.000000 skyalmanac-1.3.8/skyalmanac/lib/suntables.py
--rw-rw-rw-   0        0        0    48781 2022-04-22 17:41:07.000000 skyalmanac-1.3.8/skyalmanac/lib/tables.py
-drwxrwxrwx   0        0        0        0 2022-04-23 16:01:51.019956 skyalmanac-1.3.8/skyalmanac.egg-info/
--rw-rw-rw-   0        0        0     6933 2022-04-23 16:01:50.000000 skyalmanac-1.3.8/skyalmanac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2022-04-23 16:01:50.000000 skyalmanac-1.3.8/skyalmanac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-23 16:01:50.000000 skyalmanac-1.3.8/skyalmanac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-02-17 21:10:28.000000 skyalmanac-1.3.8/skyalmanac.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2022-04-23 16:01:50.000000 skyalmanac-1.3.8/skyalmanac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-04-23 16:01:50.000000 skyalmanac-1.3.8/skyalmanac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-03 18:21:15.275833 skyalmanac-1.3.9/
+-rw-rw-rw-   0        0        0    35149 2019-09-02 18:38:48.000000 skyalmanac-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     7115 2022-07-03 18:21:15.275833 skyalmanac-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6112 2022-07-03 18:09:44.000000 skyalmanac-1.3.9/README.rst
+-rw-rw-rw-   0        0        0      115 2021-02-15 20:39:50.000000 skyalmanac-1.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1091 2022-07-03 18:21:15.276833 skyalmanac-1.3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-07-03 18:21:15.258829 skyalmanac-1.3.9/skyalmanac/
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.9/skyalmanac/__init__.py
+-rw-rw-rw-   0        0        0    11103 2022-04-24 17:38:38.000000 skyalmanac-1.3.9/skyalmanac/__main__.py
+drwxrwxrwx   0        0        0        0 2022-07-03 18:21:15.262830 skyalmanac-1.3.9/skyalmanac/astro-data/
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.9/skyalmanac/astro-data/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-03 18:21:15.267831 skyalmanac-1.3.9/skyalmanac/data/
+-rw-rw-rw-   0        0        0   130123 2020-02-28 19:27:47.000000 skyalmanac-1.3.9/skyalmanac/data/A4chart0-180_P.pdf
+-rw-rw-rw-   0        0        0   128042 2020-02-28 19:34:01.000000 skyalmanac-1.3.9/skyalmanac/data/A4chart180-360_P.pdf
+-rw-rw-rw-   0        0        0    24577 2019-02-02 20:33:26.000000 skyalmanac-1.3.9/skyalmanac/data/Ra.JPG
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.9/skyalmanac/data/__init__.py
+-rw-rw-rw-   0        0        0   133928 2020-02-12 20:36:26.000000 skyalmanac-1.3.9/skyalmanac/data/croppedmoon.png
+drwxrwxrwx   0        0        0        0 2022-07-03 18:21:15.270831 skyalmanac-1.3.9/skyalmanac/docs/
+-rw-rw-rw-   0        0        0  1743971 2020-03-06 07:11:00.000000 skyalmanac-1.3.9/skyalmanac/docs/Explanation.pdf
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.9/skyalmanac/docs/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-03 18:21:15.274833 skyalmanac-1.3.9/skyalmanac/lib/
+-rw-rw-rw-   0        0        0        0 2021-02-03 17:12:49.000000 skyalmanac-1.3.9/skyalmanac/lib/__init__.py
+-rw-rw-rw-   0        0        0    25143 2022-04-22 17:40:01.000000 skyalmanac-1.3.9/skyalmanac/lib/alma_ephem.py
+-rw-rw-rw-   0        0        0    42700 2022-04-24 09:10:04.000000 skyalmanac-1.3.9/skyalmanac/lib/alma_skyfield.py
+-rw-rw-rw-   0        0        0     2363 2022-04-24 08:54:19.000000 skyalmanac-1.3.9/skyalmanac/lib/config.py
+-rw-rw-rw-   0        0        0    11450 2021-05-01 16:23:57.000000 skyalmanac-1.3.9/skyalmanac/lib/increments.py
+-rw-rw-rw-   0        0        0    16645 2022-04-22 17:40:56.000000 skyalmanac-1.3.9/skyalmanac/lib/suntables.py
+-rw-rw-rw-   0        0        0    48781 2022-04-22 17:41:07.000000 skyalmanac-1.3.9/skyalmanac/lib/tables.py
+drwxrwxrwx   0        0        0        0 2022-07-03 18:21:15.262830 skyalmanac-1.3.9/skyalmanac.egg-info/
+-rw-rw-rw-   0        0        0     7115 2022-07-03 18:21:14.000000 skyalmanac-1.3.9/skyalmanac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2022-07-03 18:21:15.000000 skyalmanac-1.3.9/skyalmanac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-03 18:21:14.000000 skyalmanac-1.3.9/skyalmanac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-02-17 21:10:28.000000 skyalmanac-1.3.9/skyalmanac.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2022-07-03 18:21:15.000000 skyalmanac-1.3.9/skyalmanac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-07-03 18:21:15.000000 skyalmanac-1.3.9/skyalmanac.egg-info/top_level.txt
```

### Comparing `skyalmanac-1.3.8/LICENSE` & `skyalmanac-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/PKG-INFO` & `skyalmanac-1.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: skyalmanac
-Version: 1.3.8
+Version: 1.3.9
 Summary: Creates the daily pages of a Nautical Almanac using Skyfield and Ephem
 Home-page: https://github.com/aendie/SkyAlmanac-Py3
 Author: Andrew Bauer
 Author-email: aendie.bauer@gmail.com
 License: GPL-3.0 License
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -60,17 +59,19 @@
 | Astronomical computation is done by the free Ephem and Skyfield libraries.
 | Typesetting is done typically by MiKTeX or TeX Live.
 | These need to be installed:
 
 * `python <https://www.python.org/downloads/>`_ >= 3.4 (the latest version is recommended)
 * `skyfield <https://pypi.org/project/skyfield/>`__ >= v1.15 (see the `Skyfield Changelog <https://rhodesmill.org/skyfield/installation.html#changelog>`_)
 * `pandas <https://pandas.pydata.org/>`_ >= 1.0 (to decode the Hipparcos catalog)
-* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6
+* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6 (4.1 is good; 4.1.1, 4.1.2 and 4.1.3 are faulty)
 * `MiKTeX <https://miktex.org/>`_ |nbsp| |nbsp| or |nbsp| |nbsp| `TeX Live <http://www.tug.org/texlive/>`_
 
+The fault with ``Ephem 4.1.1, 4.1.2 or 4.1.3`` is an `Endless loop in computing moon rise/set <https://github.com/brandon-rhodes/pyephem/issues/232>`_
+
 Installation
 ============
 
 Install a TeX/LaTeX program on your operating system so that 'pdflatex' is available.
 
 Ensure that the `pip Python installer tool <https://pip.pypa.io/en/latest/installing.html>`_ is installed. 
 Then ensure that old versions of PyEphem, Ephem and Skyalmanac are not installed before installing SkyAlmanac from PyPI::
@@ -116,8 +117,7 @@
     initexmf --admin --edit-config-file=pdflatex
 
 This opens pdflatex.ini in Notepad. Add the following line: ::
 
     extra_mem_top = 1000000
 
 and save the file. Problem solved. For more details look `here <https://tex.stackexchange.com/questions/438902/how-to-increase-memory-size-for-xelatex-in-miktex/438911#438911>`_.
-
```

### Comparing `skyalmanac-1.3.8/README.rst` & `skyalmanac-1.3.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,19 @@
 | Astronomical computation is done by the free Ephem and Skyfield libraries.
 | Typesetting is done typically by MiKTeX or TeX Live.
 | These need to be installed:
 
 * `python <https://www.python.org/downloads/>`_ >= 3.4 (the latest version is recommended)
 * `skyfield <https://pypi.org/project/skyfield/>`__ >= v1.15 (see the `Skyfield Changelog <https://rhodesmill.org/skyfield/installation.html#changelog>`_)
 * `pandas <https://pandas.pydata.org/>`_ >= 1.0 (to decode the Hipparcos catalog)
-* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6
+* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6 (4.1 is good; 4.1.1, 4.1.2 and 4.1.3 are faulty)
 * `MiKTeX <https://miktex.org/>`_ |nbsp| |nbsp| or |nbsp| |nbsp| `TeX Live <http://www.tug.org/texlive/>`_
 
+The fault with ``Ephem 4.1.1, 4.1.2 or 4.1.3`` is an `Endless loop in computing moon rise/set <https://github.com/brandon-rhodes/pyephem/issues/232>`_
+
 Installation
 ============
 
 Install a TeX/LaTeX program on your operating system so that 'pdflatex' is available.
 
 Ensure that the `pip Python installer tool <https://pip.pypa.io/en/latest/installing.html>`_ is installed. 
 Then ensure that old versions of PyEphem, Ephem and Skyalmanac are not installed before installing SkyAlmanac from PyPI::
```

### Comparing `skyalmanac-1.3.8/setup.cfg` & `skyalmanac-1.3.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6b79 616c 6d61 6e61 630d 0a76   = skyalmanac..v
-00000020: 6572 7369 6f6e 203d 2031 2e33 2e38 0d0a  ersion = 1.3.8..
+00000020: 6572 7369 6f6e 203d 2031 2e33 2e39 0d0a  ersion = 1.3.9..
 00000030: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
 00000040: 7468 7562 2e63 6f6d 2f61 656e 6469 652f  thub.com/aendie/
 00000050: 536b 7941 6c6d 616e 6163 2d50 7933 0d0a  SkyAlmanac-Py3..
 00000060: 6175 7468 6f72 203d 2041 6e64 7265 7720  author = Andrew 
 00000070: 4261 7565 720d 0a61 7574 686f 725f 656d  Bauer..author_em
 00000080: 6169 6c20 3d20 6165 6e64 6965 2e62 6175  ail = aendie.bau
 00000090: 6572 4067 6d61 696c 2e63 6f6d 0d0a 636c  er@gmail.com..cl
```

### Comparing `skyalmanac-1.3.8/skyalmanac/__main__.py` & `skyalmanac-1.3.9/skyalmanac/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,17 +39,17 @@
             os.remove(filename + ".pdf")
         except PermissionError:
             print("ERROR: please close '{}' so it can be re-created".format(filename + ".pdf"))
             sys.exit(0)
     if os.path.exists(filename + ".tex"):
         os.remove(filename + ".tex")
 
-def makePDF(args, fn, msg = ""):
-    command = 'pdflatex {}'.format(args + fn + ".tex")
-    if args == "":
+def makePDF(pdfcmd, fn, msg = ""):
+    command = 'pdflatex {}'.format(pdfcmd + fn + ".tex")
+    if pdfcmd == "":
         os.system(command)
         print("finished" + msg)
     else:
         returned_value = os.system(command)
         if returned_value != 0:
             if msg != "":
                 print("ERROR detected while" + msg)
@@ -71,37 +71,33 @@
     if os.path.isfile(fn + ".aux"):
         os.remove(fn + ".aux")
     return
 
 
 ##Main##
 if sys.version_info[0] < 3:
-    raise Exception("Must be using Python 3")
+    raise Exception("This runs only with Python 3")
 
 if config.ephndx not in set([0, 1, 2, 3, 4]):
     print("Error - Please choose a valid ephemeris in config.py")
     sys.exit(0)
 
-try:
-    arg = sys.argv[1]
-except IndexError:
-    arg = ""
-if len(sys.argv) > 2 or not (arg == "" or arg == "-v" or arg == "-log" or arg == "-tex"):
-    print("One optional command line parameter is permitted:")
-    print(" python -m skyalmanac -v")
-    print(" ... to send pdfTeX output to the terminal")
-    print(" python -m skyalmanac -log")
-    print(" ... to keep the log file")
-    print(" python -m skyalmanac -tex")
-    print(" ... to keep the tex file")
-    sys.exit(0)
-
-args = "" if arg == "-v" else "-interaction=batchmode -halt-on-error "
-keeplog = True if arg == "-log" else False
-keeptex = True if arg == "-tex" else False
+# command line arguments...
+validargs = ['-v', '-log', '-tex']
+for i in list(range(1, len(sys.argv))):
+    if sys.argv[i] not in validargs:
+        print("Invalid argument: {}".format(sys.argv[i]))
+        print("\nValid command line arguments are:")
+        print(" -v   ... to send pdfTeX output to the terminal")
+        print(" -log ... to keep the log file")
+        print(" -tex ... to keep the tex file")
+        sys.exit(0)
+listarg = "" if "-v" in set(sys.argv[1:]) else "-interaction=batchmode -halt-on-error "
+keeplog = True if "-log" in set(sys.argv[1:]) else False
+keeptex = True if "-tex" in set(sys.argv[1:]) else False
 
 d = datetime.datetime.utcnow().date()
 first_day = datetime.date(d.year, d.month, d.day)
 
 #first_day = datetime.date(2023, 6, 24)	# for testing a specific date
 #d = first_day							# for testing a specific date
 
@@ -226,30 +222,30 @@
             outfile.write(tables.almanac(first_day,122,df180,df360,dfcm))
             outfile.close()
             stop = time.time()
             msg = "execution time = {:0.2f} seconds".format(stop-start) # msg = "execution time = %0.2f seconds" %(stop-start)
             print(msg)
 ##            config.writeLOG("\n\n" + msg + "\n")
             print()
-            makePDF(args, fn, " creating nautical almanac for {}".format(year))
+            makePDF(listarg, fn, " creating nautical almanac for {}".format(year))
             tidy_up(fn)
 ##        config.closeLOG()     # close log after the for-loop
 
     elif s == '2':      # Sun Tables (for a year)
         for yearint in range(int(yearfr),int(yearto)+1):
             year = "{:4d}".format(yearint)  # year = "%4d" %yearint
             msg = "\nCreating the sun tables for the year {}\n".format(year)
             print(msg)
             first_day = datetime.date(yearint, 1, 1)
             ff = "STtrad_" if config.tbls != 'm' else "STmod_"
             fn = "{}{}".format(ff,year+DecFmt)
             outfile = open(fn + ".tex", mode="w", encoding="utf8")
             outfile.write(suntables.almanac(first_day,25,dfra))
             outfile.close()
-            makePDF(args, fn, " creating sun tables for {}".format(year))
+            makePDF(listarg, fn, " creating sun tables for {}".format(year))
             tidy_up(fn)
 
     elif s == '3':      # Nautical almanac   -  6 days from today
 ##        config.initLOG()		# initialize log file
         start = time.time()
         msg = "\nCreating nautical almanac tables - from {}\n".format(sdmy)
         print(msg)
@@ -261,35 +257,35 @@
         outfile.close()
         stop = time.time()
         msg = "execution time = {:0.2f} seconds".format(stop-start) # msg = "execution time = %0.2f seconds" %(stop-start)
         print(msg)
 ##        config.writeLOG('\n\n' + msg)
 ##        config.closeLOG()
         print()
-        makePDF(args, fn)
+        makePDF(listarg, fn)
         tidy_up(fn)
 
     elif s == '4':      # Sun tables only    - 30 days from today
         msg = "\nCreating the sun tables - from {}\n".format(sdmy)
         print(msg)
         ff = "STtrad_" if config.tbls != 'm' else "STmod_"
         fn = "{}{}".format(ff,symd+DecFmt)
         deletePDF(fn)
         outfile = open(fn + ".tex", mode="w", encoding="utf8")
         outfile.write(suntables.almanac(first_day,2,dfra))
         outfile.close()
-        makePDF(args, fn)
+        makePDF(listarg, fn)
         tidy_up(fn)
 
     elif s == '5':
         msg = "\nCreating the Increments and Corrections tables\n"
         print(msg)
         fn = "inc"
         deletePDF(fn)
         outfile = open(fn + ".tex", mode="w", encoding="utf8")
         outfile.write(increments.makelatex())
         outfile.close()
-        makePDF(args, fn)
+        makePDF(listarg, fn)
         tidy_up(fn)
 
 else:
     print("Error! Choose 1, 2, 3, 4 or 5")
```

### Comparing `skyalmanac-1.3.8/skyalmanac/data/A4chart0-180_P.pdf` & `skyalmanac-1.3.9/skyalmanac/data/A4chart0-180_P.pdf`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/data/A4chart180-360_P.pdf` & `skyalmanac-1.3.9/skyalmanac/data/A4chart180-360_P.pdf`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/data/Ra.JPG` & `skyalmanac-1.3.9/skyalmanac/data/Ra.JPG`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/data/croppedmoon.png` & `skyalmanac-1.3.9/skyalmanac/data/croppedmoon.png`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/docs/Explanation.pdf` & `skyalmanac-1.3.9/skyalmanac/docs/Explanation.pdf`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/lib/alma_ephem.py` & `skyalmanac-1.3.9/skyalmanac/lib/alma_ephem.py`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/lib/alma_skyfield.py` & `skyalmanac-1.3.9/skyalmanac/lib/alma_skyfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,23 +90,23 @@
         e2 = IOError('cannot download {0} because {1}'.format(url, e))
         e2.__cause__ = None
 #        raise e2
         return False
     return True     # server works
 
 def downloadUSNO(path, filename):
-    print("Downloading EOP from USNO...", end ="")
+    print("Downloading EOP data from USNO...", end ="")
     filepath = os.path.join(path, filename)
     url = "https://maia.usno.navy.mil/ser7/" + filename
     connection = urlopen(url)
     blocksize = 128*1024
 
     # Claim our own unique download filename.
 
-    tempbase = tempname = path + '.download'
+    tempbase = tempname = path + filename + '.download'
     flags = getattr(os, 'O_BINARY', 0) | os.O_CREAT | os.O_EXCL | os.O_RDWR
     i = 1
     while True:
         try:
             fd = os.open(tempname, flags, 0o666)
         except OSError as e:  # "FileExistsError" is not supported by Python 2
             if e.errno != errno.EEXIST:
```

### Comparing `skyalmanac-1.3.8/skyalmanac/lib/config.py` & `skyalmanac-1.3.9/skyalmanac/lib/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #   GNU General Public License for more details.
 # 
 #   You should have received a copy of the GNU General Public License along
 #   with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # ================ EDIT LINES IN THIS SECTION ONLY ================
 
-# choose an ephemeris (ephndx = 0, 1 or 2):
+# choose an ephemeris (ephndx = 0, 1, 2, 3 or 4):
 #   0   de421.bsp   1900 to 2050
 #   1   de405.bsp   1600 to 2200
 #   2   de406.bsp   1000 to 2750 (Equation of Time may show ??:?? after 2750)
 #   3   de430t.bsp  1550 to 2650
 #   4   de440.bsp   1550 to 2650
 ephndx = 0
```

### Comparing `skyalmanac-1.3.8/skyalmanac/lib/increments.py` & `skyalmanac-1.3.9/skyalmanac/lib/increments.py`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/lib/suntables.py` & `skyalmanac-1.3.9/skyalmanac/lib/suntables.py`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac/lib/tables.py` & `skyalmanac-1.3.9/skyalmanac/lib/tables.py`

 * *Files identical despite different names*

### Comparing `skyalmanac-1.3.8/skyalmanac.egg-info/PKG-INFO` & `skyalmanac-1.3.9/skyalmanac.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: skyalmanac
-Version: 1.3.8
+Version: 1.3.9
 Summary: Creates the daily pages of a Nautical Almanac using Skyfield and Ephem
 Home-page: https://github.com/aendie/SkyAlmanac-Py3
 Author: Andrew Bauer
 Author-email: aendie.bauer@gmail.com
 License: GPL-3.0 License
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -60,17 +59,19 @@
 | Astronomical computation is done by the free Ephem and Skyfield libraries.
 | Typesetting is done typically by MiKTeX or TeX Live.
 | These need to be installed:
 
 * `python <https://www.python.org/downloads/>`_ >= 3.4 (the latest version is recommended)
 * `skyfield <https://pypi.org/project/skyfield/>`__ >= v1.15 (see the `Skyfield Changelog <https://rhodesmill.org/skyfield/installation.html#changelog>`_)
 * `pandas <https://pandas.pydata.org/>`_ >= 1.0 (to decode the Hipparcos catalog)
-* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6
+* `ephem <https://pypi.org/project/ephem/>`__ >= 3.7.6 (4.1 is good; 4.1.1, 4.1.2 and 4.1.3 are faulty)
 * `MiKTeX <https://miktex.org/>`_ |nbsp| |nbsp| or |nbsp| |nbsp| `TeX Live <http://www.tug.org/texlive/>`_
 
+The fault with ``Ephem 4.1.1, 4.1.2 or 4.1.3`` is an `Endless loop in computing moon rise/set <https://github.com/brandon-rhodes/pyephem/issues/232>`_
+
 Installation
 ============
 
 Install a TeX/LaTeX program on your operating system so that 'pdflatex' is available.
 
 Ensure that the `pip Python installer tool <https://pip.pypa.io/en/latest/installing.html>`_ is installed. 
 Then ensure that old versions of PyEphem, Ephem and Skyalmanac are not installed before installing SkyAlmanac from PyPI::
@@ -116,8 +117,7 @@
     initexmf --admin --edit-config-file=pdflatex
 
 This opens pdflatex.ini in Notepad. Add the following line: ::
 
     extra_mem_top = 1000000
 
 and save the file. Problem solved. For more details look `here <https://tex.stackexchange.com/questions/438902/how-to-increase-memory-size-for-xelatex-in-miktex/438911#438911>`_.
-
```

### Comparing `skyalmanac-1.3.8/skyalmanac.egg-info/SOURCES.txt` & `skyalmanac-1.3.9/skyalmanac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

