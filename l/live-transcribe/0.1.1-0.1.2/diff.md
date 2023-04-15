# Comparing `tmp/live-transcribe-0.1.1.tar.gz` & `tmp/live-transcribe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-transcribe-0.1.1.tar", max compression
+gzip compressed data, was "live-transcribe-0.1.2.tar", max compression
```

## Comparing `live-transcribe-0.1.1.tar` & `live-transcribe-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      985 2023-04-15 02:00:48.899346 live-transcribe-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-14 19:27:09.059000 live-transcribe-0.1.1/live_transcribe/__init__.py
--rw-r--r--   0        0        0     2069 2023-04-15 01:37:53.195052 live-transcribe-0.1.1/live_transcribe/__main__.py
--rw-r--r--   0        0        0     6069 2023-04-15 00:21:24.661903 live-transcribe-0.1.1/live_transcribe/_poc.py
--rw-r--r--   0        0        0     2162 2023-04-15 01:49:09.210252 live-transcribe-0.1.1/live_transcribe/audio_pasimple.py
--rw-r--r--   0        0        0      475 2023-04-14 22:02:22.933468 live-transcribe-0.1.1/live_transcribe/qt.py
--rw-r--r--   0        0        0     6421 2023-04-15 00:21:52.870027 live-transcribe-0.1.1/live_transcribe/text.py
--rw-r--r--   0        0        0     2558 2023-04-15 00:24:11.218644 live-transcribe-0.1.1/live_transcribe/transcribe.py
--rw-r--r--   0        0        0      584 2023-04-15 01:55:48.603074 live-transcribe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1927 2023-04-15 02:01:01.877183 live-transcribe-0.1.1/setup.py
--rw-r--r--   0        0        0     1708 2023-04-15 02:01:01.877399 live-transcribe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      987 2023-04-15 02:03:18.663420 live-transcribe-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 19:27:09.059000 live-transcribe-0.1.2/live_transcribe/__init__.py
+-rw-r--r--   0        0        0     2069 2023-04-15 01:37:53.195052 live-transcribe-0.1.2/live_transcribe/__main__.py
+-rw-r--r--   0        0        0     6069 2023-04-15 00:21:24.661903 live-transcribe-0.1.2/live_transcribe/_poc.py
+-rw-r--r--   0        0        0     2162 2023-04-15 01:49:09.210252 live-transcribe-0.1.2/live_transcribe/audio_pasimple.py
+-rw-r--r--   0        0        0      475 2023-04-14 22:02:22.933468 live-transcribe-0.1.2/live_transcribe/qt.py
+-rw-r--r--   0        0        0     6421 2023-04-15 00:21:52.870027 live-transcribe-0.1.2/live_transcribe/text.py
+-rw-r--r--   0        0        0     2558 2023-04-15 00:24:11.218644 live-transcribe-0.1.2/live_transcribe/transcribe.py
+-rw-r--r--   0        0        0      584 2023-04-15 02:03:36.871426 live-transcribe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1930 2023-04-15 02:03:43.637043 live-transcribe-0.1.2/setup.py
+-rw-r--r--   0        0        0     1710 2023-04-15 02:03:43.637258 live-transcribe-0.1.2/PKG-INFO
```

### Comparing `live-transcribe-0.1.1/README.md` & `live-transcribe-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Live Transcribe
 
-Live Transcribe is a Python package that provides live, real-time transcription of audio based on OpenAI's Whisper API.
+Live Transcribe is a Python package that provides live, real-time transcription based on OpenAI's Whisper. Works
+offline.
 
 Currently, Live Transcribe supports only PulseAudio as an audio backend.
 
 # Installation
 
 1. **optional but highly recommended for low latency** Refer to the [Pytorch documentation guide](https://pytorch.org/)
    to install Pytorch **with CUDA support**.
```

### Comparing `live-transcribe-0.1.1/live_transcribe/__main__.py` & `live-transcribe-0.1.2/live_transcribe/__main__.py`

 * *Files identical despite different names*

### Comparing `live-transcribe-0.1.1/live_transcribe/_poc.py` & `live-transcribe-0.1.2/live_transcribe/_poc.py`

 * *Files identical despite different names*

### Comparing `live-transcribe-0.1.1/live_transcribe/audio_pasimple.py` & `live-transcribe-0.1.2/live_transcribe/audio_pasimple.py`

 * *Files identical despite different names*

### Comparing `live-transcribe-0.1.1/live_transcribe/text.py` & `live-transcribe-0.1.2/live_transcribe/text.py`

 * *Files identical despite different names*

### Comparing `live-transcribe-0.1.1/live_transcribe/transcribe.py` & `live-transcribe-0.1.2/live_transcribe/transcribe.py`

 * *Files identical despite different names*

### Comparing `live-transcribe-0.1.1/pyproject.toml` & `live-transcribe-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "live-transcribe"
-version = "0.1.1"
+version = "0.1.2"
 description = "Real-time audio transcription. Runs OpenAI's Whisper locally."
 authors = ["Tomasz Łakota <tomasz.lakota@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "live_transcribe" }]
 
 [tool.poetry.dependencies]
```

### Comparing `live-transcribe-0.1.1/setup.py` & `live-transcribe-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'pulsectl>=22.3.2,<23.0.0']
 
 entry_points = \
 {'console_scripts': ['live-transcribe = live_transcribe:__main__']}
 
 setup_kwargs = {
     'name': 'live-transcribe',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': "Real-time audio transcription. Runs OpenAI's Whisper locally.",
-    'long_description': 'Live Transcribe\n\nLive Transcribe is a Python package that provides live, real-time transcription of audio based on OpenAI\'s Whisper API.\n\nCurrently, Live Transcribe supports only PulseAudio as an audio backend.\n\n# Installation\n\n1. **optional but highly recommended for low latency** Refer to the [Pytorch documentation guide](https://pytorch.org/)\n   to install Pytorch **with CUDA support**.\n1. `pip install live-transcribe`\n\n# Usage\n\nJust run:\n\n    python -m live_transcribe\n\nor\n\n    live_transcribe\n\nIf you want to transcribe from another audio device, than the default, use the `--device` option, e.g.:\n\n    live_transcribe --list-devices\n    live_transcribe --device "alsa_input.usb-046d_HD_Pro_Webcam_C920_8C0B5B0F-02.analog-stereo\n\nOn the first usage, the OpenAI\'s Whisper model will be downloaded and cached.\n\nSee `live_transcribe --help` for options.\n\n# Dependencies\n\nLive Transcribe has the following dependencies:\n\n    Python 3.8 or higher\n    OpenAI-Whisper\n    PulseAudio\n',
+    'long_description': 'Live Transcribe\n\nLive Transcribe is a Python package that provides live, real-time transcription based on OpenAI\'s Whisper. Works\noffline.\n\nCurrently, Live Transcribe supports only PulseAudio as an audio backend.\n\n# Installation\n\n1. **optional but highly recommended for low latency** Refer to the [Pytorch documentation guide](https://pytorch.org/)\n   to install Pytorch **with CUDA support**.\n1. `pip install live-transcribe`\n\n# Usage\n\nJust run:\n\n    python -m live_transcribe\n\nor\n\n    live_transcribe\n\nIf you want to transcribe from another audio device, than the default, use the `--device` option, e.g.:\n\n    live_transcribe --list-devices\n    live_transcribe --device "alsa_input.usb-046d_HD_Pro_Webcam_C920_8C0B5B0F-02.analog-stereo\n\nOn the first usage, the OpenAI\'s Whisper model will be downloaded and cached.\n\nSee `live_transcribe --help` for options.\n\n# Dependencies\n\nLive Transcribe has the following dependencies:\n\n    Python 3.8 or higher\n    OpenAI-Whisper\n    PulseAudio\n',
     'author': 'Tomasz Łakota',
     'author_email': 'tomasz.lakota@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `live-transcribe-0.1.1/PKG-INFO` & `live-transcribe-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-transcribe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Real-time audio transcription. Runs OpenAI's Whisper locally.
 License: MIT
 Author: Tomasz Łakota
 Author-email: tomasz.lakota@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,16 @@
 Requires-Dist: openai-whisper (>=20230314,<20230315)
 Requires-Dist: pasimple (>=0.0.1,<0.0.2)
 Requires-Dist: pulsectl (>=22.3.2,<23.0.0)
 Description-Content-Type: text/markdown
 
 Live Transcribe
 
-Live Transcribe is a Python package that provides live, real-time transcription of audio based on OpenAI's Whisper API.
+Live Transcribe is a Python package that provides live, real-time transcription based on OpenAI's Whisper. Works
+offline.
 
 Currently, Live Transcribe supports only PulseAudio as an audio backend.
 
 # Installation
 
 1. **optional but highly recommended for low latency** Refer to the [Pytorch documentation guide](https://pytorch.org/)
    to install Pytorch **with CUDA support**.
```

