# Comparing `tmp/Scopul-1.0.2.tar.gz` & `tmp/Scopul-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scopul-1.0.2.tar", last modified: Tue Apr 11 03:19:33 2023, max compression
+gzip compressed data, was "Scopul-1.0.3.tar", last modified: Sat Apr 15 15:01:44 2023, max compression
```

## Comparing `Scopul-1.0.2.tar` & `Scopul-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.294281 Scopul-1.0.2/
--rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      873 2023-04-11 03:19:33.295271 Scopul-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.2/README.md
--rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.2/long_desc.md
--rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      730 2023-04-11 03:19:33.297779 Scopul-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.250658 Scopul-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.277904 Scopul-1.0.2/src/Scopul/
--rw-rw-rw-   0        0        0    16368 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/Sequence.py
--rw-rw-rw-   0        0        0      441 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/Tempo.py
--rw-rw-rw-   0        0        0      663 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/TimeSignature.py
--rw-rw-rw-   0        0        0      470 2023-03-15 00:29:53.000000 Scopul-1.0.2/src/Scopul/__init__.py
--rw-rw-rw-   0        0        0       90 2023-02-17 20:20:00.000000 Scopul-1.0.2/src/Scopul/config_musescore.py
--rw-rw-rw-   0        0        0     4011 2023-02-12 20:39:00.000000 Scopul-1.0.2/src/Scopul/conversions.py
--rw-rw-rw-   0        0        0     3560 2023-03-15 00:13:32.000000 Scopul-1.0.2/src/Scopul/helpers.py
--rw-rw-rw-   0        0        0    15336 2023-03-19 00:09:53.000000 Scopul-1.0.2/src/Scopul/scopul.py
--rw-rw-rw-   0        0        0      449 2023-02-21 00:22:42.000000 Scopul-1.0.2/src/Scopul/scopul_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.287732 Scopul-1.0.2/src/Scopul.egg-info/
--rw-rw-rw-   0        0        0      873 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 03:19:33.000000 Scopul-1.0.2/src/Scopul.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 03:19:33.293273 Scopul-1.0.2/tests/
--rw-rw-rw-   0        0        0     5380 2023-03-19 00:09:53.000000 Scopul-1.0.2/tests/test_sequence.py
--rw-rw-rw-   0        0        0     1150 2023-03-15 22:35:22.000000 Scopul-1.0.2/tests/test_tempo.py
--rw-rw-rw-   0        0        0     1384 2023-03-15 00:11:19.000000 Scopul-1.0.2/tests/test_time_sig.py
+drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.239095 Scopul-1.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-02-16 01:23:44.000000 Scopul-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      188 2023-02-16 01:24:10.000000 Scopul-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      873 2023-04-15 15:01:44.240206 Scopul-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2893 2023-03-19 00:09:53.000000 Scopul-1.0.3/README.md
+-rw-rw-rw-   0        0        0      283 2023-03-19 00:09:53.000000 Scopul-1.0.3/long_desc.md
+-rw-rw-rw-   0        0        0      108 2023-03-19 00:09:53.000000 Scopul-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-04-15 15:01:44.242205 Scopul-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.182871 Scopul-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.223331 Scopul-1.0.3/src/Scopul/
+-rw-rw-rw-   0        0        0    16368 2023-03-19 00:09:53.000000 Scopul-1.0.3/src/Scopul/Sequence.py
+-rw-rw-rw-   0        0        0      441 2023-03-19 00:09:53.000000 Scopul-1.0.3/src/Scopul/Tempo.py
+-rw-rw-rw-   0        0        0      663 2023-04-15 00:33:29.000000 Scopul-1.0.3/src/Scopul/TimeSignature.py
+-rw-rw-rw-   0        0        0      470 2023-04-15 14:56:04.000000 Scopul-1.0.3/src/Scopul/__init__.py
+-rw-rw-rw-   0        0        0       90 2023-02-17 20:20:00.000000 Scopul-1.0.3/src/Scopul/config_musescore.py
+-rw-rw-rw-   0        0        0     4011 2023-02-12 20:39:00.000000 Scopul-1.0.3/src/Scopul/conversions.py
+-rw-rw-rw-   0        0        0     3560 2023-03-15 00:13:32.000000 Scopul-1.0.3/src/Scopul/helpers.py
+-rw-rw-rw-   0        0        0    15336 2023-04-15 15:00:33.000000 Scopul-1.0.3/src/Scopul/scopul.py
+-rw-rw-rw-   0        0        0      449 2023-02-21 00:22:42.000000 Scopul-1.0.3/src/Scopul/scopul_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-15 15:01:44.238099 Scopul-1.0.3/src/Scopul.egg-info/
+-rw-rw-rw-   0        0        0      873 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 15:01:44.000000 Scopul-1.0.3/src/Scopul.egg-info/top_level.txt
```

### Comparing `Scopul-1.0.2/LICENSE` & `Scopul-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.2/PKG-INFO` & `Scopul-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.2
+Version: 1.0.3
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Scopul-1.0.2/README.md` & `Scopul-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.2/setup.cfg` & `Scopul-1.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 636f 7075 6c0d 0a76 6572 7369   = Scopul..versi
-00000020: 6f6e 203d 2031 2e30 2e32 0d0a 6175 7468  on = 1.0.2..auth
+00000020: 6f6e 203d 2031 2e30 2e33 0d0a 6175 7468  on = 1.0.3..auth
 00000030: 6f72 203d 2053 7761 7961 6d20 5361 686f  or = Swayam Saho
 00000040: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000050: 3d20 7377 6179 616d 7361 3031 4067 6d61  = swayamsa01@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 4120 4d49 4449 2066 696c  ion = A MIDI fil
 00000080: 6520 616e 616c 797a 6572 2077 6869 6368  e analyzer which
 00000090: 2061 6c6c 6f77 7320 796f 7520 746f 2067   allows you to g
```

### Comparing `Scopul-1.0.2/src/Scopul/Sequence.py` & `Scopul-1.0.3/src/Scopul/Sequence.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.2/src/Scopul/TimeSignature.py` & `Scopul-1.0.3/src/Scopul/TimeSignature.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.2/src/Scopul/conversions.py` & `Scopul-1.0.3/src/Scopul/conversions.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.2/src/Scopul/helpers.py` & `Scopul-1.0.3/src/Scopul/helpers.py`

 * *Files identical despite different names*

### Comparing `Scopul-1.0.2/src/Scopul/scopul.py` & `Scopul-1.0.3/src/Scopul/scopul.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     def generate_pdf(
         self,
         output: str,
         fp: str = "",
         overwrite: bool = False,
         remove_defects: bool = False,
     ) -> None:
+        print("HIIIIIIIIII")
         """Generates a pdf of the midi
 
         Creates a pdf by turning it into musicxml then to pdf
 
         Args:
             output: a str that represents the name of the file
             fp: a str that represents the file path as to where to save the pdf. Default is '', which will save to the current working directory
@@ -125,15 +126,15 @@
             )
 
         # Check for correct file format
         ext = pathlib.Path(output).suffix
         if ext != ".pdf":
             raise InvalidFileFormatError(f"Expected .pdf, got {ext}")
 
-        midi = self.music21.makeMeasures()
+        midi = self.music21
 
         if remove_defects:
             for part in midi.parts:
                 try:
                     part.write("musicxml.pdf")
                 except:
                     midi.remove(part)
@@ -230,15 +231,15 @@
         Can also be called with a setter to the midi property. For example:
 
         testmidi.music21 = "test.mid"
 
         """
 
         self._audio = audio
-        self.music21 = converter.parse(audio).makeMeasures()
+        self.music21 = converter.parse(audio)
         self._parts = []
         for part in self.music21.parts:
             self._parts.append(Part(part))
 
     def save_midi(self, output, fp="", overwrite=False):
         """
         Save the MIDI file to the specified output file path.
```

### Comparing `Scopul-1.0.2/src/Scopul.egg-info/PKG-INFO` & `Scopul-1.0.3/src/Scopul.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scopul
-Version: 1.0.2
+Version: 1.0.3
 Summary: A MIDI file analyzer which allows you to go through components of a MIDI file and extract data.
 Home-page: https://github.com/SwayamSahoo11742/Scopul
 Author: Swayam Sahoo
 Author-email: swayamsa01@gmail.com
 Project-URL: Bug Tracker, https://github.com/SwayamSahoo11742/Scopul/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

