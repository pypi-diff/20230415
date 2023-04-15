# Comparing `tmp/Scopul-1.0.3.tar.gz` & `tmp/Scopul-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scopul-1.0.3.tar", last modified: Sat Apr 15 15:01:44 2023, max compression
+gzip compressed data, was "Scopul-1.0.4.tar", last modified: Sat Apr 15 15:08:01 2023, max compression
```

## Comparing `Scopul-1.0.3.tar` & `Scopul-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.239095 Scopul-1.0.3/
--rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      873 2023-04-15 15:01:44.240206 Scopul-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.3/README.md
--rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.3/long_desc.md
--rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      730 2023-04-15 15:01:44.242205 Scopul-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.182871 Scopul-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.223331 Scopul-1.0.3/src/Scopul/
--rw-rw-rw-   0        0        0    16368 2023-03-19 00:09:53.000000 Scopul-1.0.3/src/Scopul/Sequence.py
--rw-rw-rw-   0        0        0      441 2023-03-19 00:09:53.000000 Scopul-1.0.3/src/Scopul/Tempo.py
--rw-rw-rw-   0        0        0      663 2023-04-15 00:33:29.000000 Scopul-1.0.3/src/Scopul/TimeSignature.py
--rw-rw-rw-   0        0        0      470 2023-04-15 14:56:04.000000 Scopul-1.0.3/src/Scopul/__init__.py
--rw-rw-rw-   0        0        0       90 2023-02-17 20:20:00.000000 Scopul-1.0.3/src/Scopul/config_musescore.py
--rw-rw-rw-   0        0        0     4011 2023-02-12 20:39:00.000000 Scopul-1.0.3/src/Scopul/conversions.py
--rw-rw-rw-   0        0        0     3560 2023-03-15 00:13:32.000000 Scopul-1.0.3/src/Scopul/helpers.py
--rw-rw-rw-   0        0        0    15336 2023-04-15 15:00:33.000000 Scopul-1.0.3/src/Scopul/scopul.py
--rw-rw-rw-   0        0        0      449 2023-02-21 00:22:42.000000 Scopul-1.0.3/src/Scopul/scopul_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.238099 Scopul-1.0.3/src/Scopul.egg-info/
--rw-rw-rw-   0        0        0      873 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.603704 Scopul-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      873 2023-04-15 15:08:01.604701 Scopul-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.4/README.md
+-rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.4/long_desc.md
+-rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-04-15 15:08:01.605697 Scopul-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.562908 Scopul-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.589724 Scopul-1.0.4/src/Scopul/
+-rw-rw-rw-   0        0        0    16368 2023-03-19 00:09:53.000000 Scopul-1.0.4/src/Scopul/Sequence.py
+-rw-rw-rw-   0        0        0      441 2023-03-19 00:09:53.000000 Scopul-1.0.4/src/Scopul/Tempo.py
+-rw-rw-rw-   0        0        0      663 2023-04-15 00:33:29.000000 Scopul-1.0.4/src/Scopul/TimeSignature.py
+-rw-rw-rw-   0        0        0      470 2023-04-15 14:56:04.000000 Scopul-1.0.4/src/Scopul/__init__.py
+-rw-rw-rw-   0        0        0       90 2023-02-17 20:20:00.000000 Scopul-1.0.4/src/Scopul/config_musescore.py
+-rw-rw-rw-   0        0        0     4011 2023-02-12 20:39:00.000000 Scopul-1.0.4/src/Scopul/conversions.py
+-rw-rw-rw-   0        0        0     3560 2023-03-15 00:13:32.000000 Scopul-1.0.4/src/Scopul/helpers.py
+-rw-rw-rw-   0        0        0    15321 2023-04-15 15:07:35.000000 Scopul-1.0.4/src/Scopul/scopul.py
+-rw-rw-rw-   0        0        0      449 2023-02-21 00:22:42.000000 Scopul-1.0.4/src/Scopul/scopul_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-15 15:08:01.602707 Scopul-1.0.4/src/Scopul.egg-info/
+-rw-rw-rw-   0        0        0      873 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 15:08:01.000000 Scopul-1.0.4/src/Scopul.egg-info/top_level.txt
```

### Comparing `Scopul-1.0.3/LICENSE` & `Scopul-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.3/PKG-INFO` & `Scopul-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.3
+Version: 1.0.4
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Scopul-1.0.3/README.md` & `Scopul-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.3/setup.cfg` & `Scopul-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 636f 7075 6c0d 0a76 6572 7369   = Scopul..versi
-00000020: 6f6e 203d 2031 2e30 2e33 0d0a 6175 7468  on = 1.0.3..auth
+00000020: 6f6e 203d 2031 2e30 2e34 0d0a 6175 7468  on = 1.0.4..auth
 00000030: 6f72 203d 2053 7761 7961 6d20 5361 686f  or = Swayam Saho
 00000040: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000050: 3d20 7377 6179 616d 7361 3031 4067 6d61  = swayamsa01@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 4120 4d49 4449 2066 696c  ion = A MIDI fil
 00000080: 6520 616e 616c 797a 6572 2077 6869 6368  e analyzer which
 00000090: 2061 6c6c 6f77 7320 796f 7520 746f 2067   allows you to g
```

### Comparing `Scopul-1.0.3/src/Scopul/Sequence.py` & `Scopul-1.0.4/src/Scopul/Sequence.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.3/src/Scopul/TimeSignature.py` & `Scopul-1.0.4/src/Scopul/TimeSignature.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.3/src/Scopul/conversions.py` & `Scopul-1.0.4/src/Scopul/conversions.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.3/src/Scopul/helpers.py` & `Scopul-1.0.4/src/Scopul/helpers.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.3/src/Scopul/scopul.py` & `Scopul-1.0.4/src/Scopul/scopul.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,18 +84,18 @@
         return MidiFile(self._audio).length
     
     # Generate a pdf
     def generate_pdf(
         self,
         output: str,
         fp: str = "",
+        title: str = "Scop",
         overwrite: bool = False,
         remove_defects: bool = False,
     ) -> None:
-        print("HIIIIIIIIII")
         """Generates a pdf of the midi
 
         Creates a pdf by turning it into musicxml then to pdf
 
         Args:
             output: a str that represents the name of the file
             fp: a str that represents the file path as to where to save the pdf. Default is '', which will save to the current working directory
@@ -147,15 +147,15 @@
         else:
             if pathlib.Path(fp + output).exists():
                 raise FileExistsError(
                     f"{fp + output} already exists. To overwrite, set overwrite=True"
                 )
 
         # Creates the pdf and deletes the musicxml file
-        midi.metadata.title = output.split(".")[0]
+        midi.metadata.title = title
         midi.write("musicxml.pdf", fp=fp)
         os.rename(fp + ".musicxml.pdf", fp + output)
         os.remove(fp + ".musicxml.musicxml")
 
     def generate_musicxml(
         self,
         output: str,
```

### Comparing `Scopul-1.0.3/src/Scopul.egg-info/PKG-INFO` & `Scopul-1.0.4/src/Scopul.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.3
+Version: 1.0.4
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

