# Comparing `tmp/fortepyan-0.1.8.tar.gz` & `tmp/fortepyan-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortepyan-0.1.8.tar", last modified: Sat Mar 11 15:39:07 2023, max compression
+gzip compressed data, was "fortepyan-0.1.9.tar", last modified: Sun Apr  2 17:21:18 2023, max compression
```

## Comparing `fortepyan-0.1.8.tar` & `fortepyan-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-03-11 15:39:07.794669 fortepyan-0.1.8/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1226 2023-03-11 15:39:07.794669 fortepyan-0.1.8/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      774 2023-02-26 14:45:22.000000 fortepyan-0.1.8/README.md
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-03-11 15:39:07.790669 fortepyan-0.1.8/fortepyan/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      468 2023-03-11 15:38:33.000000 fortepyan-0.1.8/fortepyan/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-03-11 15:39:07.790669 fortepyan-0.1.8/fortepyan/animation/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       96 2023-03-02 08:36:53.000000 fortepyan-0.1.8/fortepyan/animation/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15612 2023-03-08 21:12:29.000000 fortepyan-0.1.8/fortepyan/animation/evolution.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      756 2023-02-21 08:54:31.000000 fortepyan-0.1.8/fortepyan/animation/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     4985 2023-03-08 20:21:52.000000 fortepyan-0.1.8/fortepyan/animation/pianoroll.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-03-11 15:39:07.790669 fortepyan-0.1.8/fortepyan/audio/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.1.8/fortepyan/audio/render.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.1.8/fortepyan/audio/soundfont.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.1.8/fortepyan/config.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.1.8/fortepyan/main.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-03-11 15:39:07.794669 fortepyan-0.1.8/fortepyan/midi/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7921 2023-03-04 15:19:19.000000 fortepyan-0.1.8/fortepyan/midi/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2168 2023-03-04 16:57:37.000000 fortepyan-0.1.8/fortepyan/midi/tools.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-03-11 15:39:07.794669 fortepyan-0.1.8/fortepyan/viz/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-02-11 18:29:02.000000 fortepyan-0.1.8/fortepyan/viz/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5531 2023-03-08 21:09:31.000000 fortepyan-0.1.8/fortepyan/viz/pianoroll.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2925 2023-03-03 08:39:56.000000 fortepyan-0.1.8/fortepyan/viz/structures.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-03-11 15:39:07.790669 fortepyan-0.1.8/fortepyan.egg-info/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1226 2023-03-11 15:39:07.000000 fortepyan-0.1.8/fortepyan.egg-info/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      563 2023-03-11 15:39:07.000000 fortepyan-0.1.8/fortepyan.egg-info/SOURCES.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-03-11 15:39:07.000000 fortepyan-0.1.8/fortepyan.egg-info/dependency_links.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      119 2023-03-11 15:39:07.000000 fortepyan-0.1.8/fortepyan.egg-info/requires.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-03-11 15:39:07.000000 fortepyan-0.1.8/fortepyan.egg-info/top_level.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1301 2023-03-11 15:38:33.000000 fortepyan-0.1.8/pyproject.toml
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-03-11 15:39:07.794669 fortepyan-0.1.8/setup.cfg
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1226 2023-04-02 17:21:18.612348 fortepyan-0.1.9/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      774 2023-02-26 14:45:22.000000 fortepyan-0.1.9/README.md
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      468 2023-04-02 17:20:56.000000 fortepyan-0.1.9/fortepyan/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/animation/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       96 2023-03-02 08:36:53.000000 fortepyan-0.1.9/fortepyan/animation/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15612 2023-03-08 21:12:29.000000 fortepyan-0.1.9/fortepyan/animation/evolution.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      756 2023-02-21 08:54:31.000000 fortepyan-0.1.9/fortepyan/animation/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     4985 2023-03-08 20:21:52.000000 fortepyan-0.1.9/fortepyan/animation/pianoroll.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/audio/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.1.9/fortepyan/audio/render.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.1.9/fortepyan/audio/soundfont.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.1.9/fortepyan/config.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.1.9/fortepyan/main.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/midi/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8106 2023-04-02 17:19:30.000000 fortepyan-0.1.9/fortepyan/midi/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2168 2023-03-04 16:57:37.000000 fortepyan-0.1.9/fortepyan/midi/tools.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/viz/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-02-11 18:29:02.000000 fortepyan-0.1.9/fortepyan/viz/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5531 2023-03-08 21:09:31.000000 fortepyan-0.1.9/fortepyan/viz/pianoroll.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2925 2023-03-03 08:39:56.000000 fortepyan-0.1.9/fortepyan/viz/structures.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan.egg-info/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1226 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      563 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/SOURCES.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/dependency_links.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      137 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/requires.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/top_level.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1326 2023-04-02 17:20:56.000000 fortepyan-0.1.9/pyproject.toml
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-04-02 17:21:18.612348 fortepyan-0.1.9/setup.cfg
```

### Comparing `fortepyan-0.1.8/PKG-INFO` & `fortepyan-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.1.8
+Version: 0.1.9
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.1.8/README.md` & `fortepyan-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/animation/evolution.py` & `fortepyan-0.1.9/fortepyan/animation/evolution.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/animation/main.py` & `fortepyan-0.1.9/fortepyan/animation/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/animation/pianoroll.py` & `fortepyan-0.1.9/fortepyan/animation/pianoroll.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/audio/render.py` & `fortepyan-0.1.9/fortepyan/audio/render.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/audio/soundfont.py` & `fortepyan-0.1.9/fortepyan/audio/soundfont.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/main.py` & `fortepyan-0.1.9/fortepyan/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/midi/structures.py` & `fortepyan-0.1.9/fortepyan/midi/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,17 @@
         part = self.df[index].reset_index(drop=True)
 
         first_sound = part.start.min()
         part.start -= first_sound
         part.end -= first_sound
 
         # Make sure the piece can always be track back to the original file exactly
-        out_source = self.source
+        out_source = dict(self.source)
         out_source["start"] = self.source.get("start", 0) + index.start
-        out_source["finish"] = self.source.get("finish", 0) + index.stop
+        out_source["finish"] = self.source.get("start", 0) + index.stop
         out_source["start_time"] = self.source.get("start_time", 0) + first_sound
         out = MidiPiece(df=part, source=out_source)
 
         return out
 
     @property
     def duration(self) -> float:
@@ -124,15 +124,20 @@
 
         return track
 
     @classmethod
     def from_huggingface(cls, record: dict) -> "MidiPiece":
         df = pd.DataFrame(record["notes"])
         df["duration"] = df.end - df.start
-        that = cls(df=df)
+        source = {
+            "composer": record["composer"],
+            "title": record["title"],
+            "midi_filename": record["midi_filename"],
+        }
+        that = cls(df=df, source=source)
         return that
 
 
 @dataclass
 class MidiFile:
     path: str
     apply_sustain: bool = True
```

### Comparing `fortepyan-0.1.8/fortepyan/midi/tools.py` & `fortepyan-0.1.9/fortepyan/midi/tools.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/viz/pianoroll.py` & `fortepyan-0.1.9/fortepyan/viz/pianoroll.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan/viz/structures.py` & `fortepyan-0.1.9/fortepyan/viz/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/fortepyan.egg-info/PKG-INFO` & `fortepyan-0.1.9/fortepyan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.1.8
+Version: 0.1.9
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.1.8/fortepyan.egg-info/SOURCES.txt` & `fortepyan-0.1.9/fortepyan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.8/pyproject.toml` & `fortepyan-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fortepyan"
-version = "0.1.8"
+version = "0.1.9"
 description = "Process MIDI piano with (almost) no pain"
 readme = "README.md"
 authors = [{ name = "Piano For AI", email = "roszcz+fortepyan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -22,25 +22,26 @@
     "boto3",
     "midi2audio>=0.1.1",
     "numpy>=1.23.4",
     "pretty-midi>=0.2.9",
     "psycopg2>=2.9.5",
     "pydub>=0.25",
     "SQLAlchemy>=1.4.45",
+    "matplotlib>=3.6.2",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/Nospoko/fortepyan"
 
 [tool.setuptools]
 packages = ["fortepyan", "fortepyan.viz", "fortepyan.midi", "fortepyan.audio", "fortepyan.animation"]
 
 [tool.bumpver]
-current_version = "0.1.8"
+current_version = "0.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

