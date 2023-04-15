# Comparing `tmp/PyTimbre-0.6.6.tar.gz` & `tmp/PyTimbre-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTimbre-0.6.6.tar", last modified: Fri Apr  7 01:44:38 2023, max compression
+gzip compressed data, was "PyTimbre-0.6.7.tar", last modified: Sat Apr 15 00:04:57 2023, max compression
```

## Comparing `PyTimbre-0.6.6.tar` & `PyTimbre-0.6.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 01:44:38.850644 PyTimbre-0.6.6/
--rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.6/LICENSE.txt
--rw-rw-rw-   0        0        0    12383 2023-04-07 01:44:38.849645 PyTimbre-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     4557 2023-04-07 01:44:36.000000 PyTimbre-0.6.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-07 01:44:38.850644 PyTimbre-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-07 01:41:59.000000 PyTimbre-0.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:44:38.816634 PyTimbre-0.6.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 01:44:38.841322 PyTimbre-0.6.6/src/PyTimbre.egg-info/
--rw-rw-rw-   0        0        0    12383 2023-04-07 01:44:38.000000 PyTimbre-0.6.6/src/PyTimbre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2023-04-07 01:44:38.000000 PyTimbre-0.6.6/src/PyTimbre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 01:44:38.000000 PyTimbre-0.6.6/src/PyTimbre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-07 01:44:38.000000 PyTimbre-0.6.6/src/PyTimbre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 01:44:38.000000 PyTimbre-0.6.6/src/PyTimbre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-07 01:44:38.844137 PyTimbre-0.6.6/src/pytimbre/
--rw-rw-rw-   0        0        0       94 2023-04-07 01:28:28.000000 PyTimbre-0.6.6/src/pytimbre/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:44:38.846645 PyTimbre-0.6.6/src/pytimbre/audio_files/
--rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.6/src/pytimbre/audio_files/__init__.py
--rw-rw-rw-   0        0        0    23192 2023-03-31 16:13:47.000000 PyTimbre-0.6.6/src/pytimbre/audio_files/ansi_standard_formatted_files.py
--rw-rw-rw-   0        0        0    15323 2023-04-04 13:59:30.000000 PyTimbre-0.6.6/src/pytimbre/audio_files/calibrated_binary_files.py
--rw-rw-rw-   0        0        0    70669 2023-03-31 16:13:47.000000 PyTimbre-0.6.6/src/pytimbre/audio_files/wavefile.py
-drwxrwxrwx   0        0        0        0 2023-04-07 01:44:38.849645 PyTimbre-0.6.6/src/pytimbre/spectral/
--rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.6/src/pytimbre/spectral/__init__.py
--rw-rw-rw-   0        0        0    16085 2023-03-31 16:13:47.000000 PyTimbre-0.6.6/src/pytimbre/spectral/acoustic_weights.py
--rw-rw-rw-   0        0        0    15571 2023-03-03 22:01:28.000000 PyTimbre-0.6.6/src/pytimbre/spectral/fractional_octave_band.py
--rw-rw-rw-   0        0        0    38821 2023-03-31 16:13:47.000000 PyTimbre-0.6.6/src/pytimbre/spectral/spectra.py
--rw-rw-rw-   0        0        0     6647 2023-03-31 16:13:47.000000 PyTimbre-0.6.6/src/pytimbre/spectral/spectrogram.py
--rw-rw-rw-   0        0        0    30872 2023-03-31 16:13:47.000000 PyTimbre-0.6.6/src/pytimbre/spectral/time_histories.py
--rw-rw-rw-   0        0        0    10655 2023-04-07 00:06:51.000000 PyTimbre-0.6.6/src/pytimbre/swipe.py
--rw-rw-rw-   0        0        0    84900 2023-04-07 01:39:58.000000 PyTimbre-0.6.6/src/pytimbre/waveform.py
--rw-rw-rw-   0        0        0     7680 2023-04-07 00:21:00.000000 PyTimbre-0.6.6/src/pytimbre/yin.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.865787 PyTimbre-0.6.7/
+-rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    13118 2023-04-15 00:04:57.865787 PyTimbre-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5289 2023-04-13 01:01:21.000000 PyTimbre-0.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 00:04:57.865787 PyTimbre-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-04-15 00:03:14.000000 PyTimbre-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.808221 PyTimbre-0.6.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.823559 PyTimbre-0.6.7/src/PyTimbre.egg-info/
+-rw-rw-rw-   0        0        0    13118 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.836414 PyTimbre-0.6.7/src/pytimbre/
+-rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.7/src/pytimbre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.843499 PyTimbre-0.6.7/src/pytimbre/audio_files/
+-rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/__init__.py
+-rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/ansi_standard_formatted_files.py
+-rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/calibrated_binary_files.py
+-rw-rw-rw-   0        0        0    70669 2023-03-31 16:13:47.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/wavefile.py
+drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.864799 PyTimbre-0.6.7/src/pytimbre/spectral/
+-rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.7/src/pytimbre/spectral/__init__.py
+-rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.7/src/pytimbre/spectral/acoustic_weights.py
+-rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.7/src/pytimbre/spectral/fractional_octave_band.py
+-rw-rw-rw-   0        0        0    16760 2023-04-14 02:05:08.000000 PyTimbre-0.6.7/src/pytimbre/spectral/fundamental_frequency.py
+-rw-rw-rw-   0        0        0    57407 2023-04-14 23:59:24.000000 PyTimbre-0.6.7/src/pytimbre/spectral/spectra.py
+-rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.7/src/pytimbre/spectral/spectrogram.py
+-rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.7/src/pytimbre/spectral/swipe.py
+-rw-rw-rw-   0        0        0    30655 2023-04-14 23:54:59.000000 PyTimbre-0.6.7/src/pytimbre/spectral/time_histories.py
+-rw-rw-rw-   0        0        0    84616 2023-04-13 01:25:20.000000 PyTimbre-0.6.7/src/pytimbre/waveform.py
+-rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.7/src/pytimbre/yin.py
```

### Comparing `PyTimbre-0.6.6/LICENSE.txt` & `PyTimbre-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.6/PKG-INFO` & `PyTimbre-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -43,51 +43,58 @@
 These represent the sound quality metrics extracted from the Mosqito project (https://github.com/Eomys/MoSQITo).
 
 In addition to this code, PyTimbre has taken the code from libf0 (https://github.com/groupmm/libf0) that assists with 
 the computation of the fundamental frequency. There are a number of methods that exist within the libf0 module, but the
 package contains a number of dependencies that are not required for the other calculations and computations within
 PyTimbre. To facilitate the calculation of the fundamental frequency, the swipe class and associated functions were
 extracted and placed into PyTimbre. The code was extracted from the 1.0.2 version of the code on 1 April 2023. This is 
-based on the report: __*Justin Salamon and Emilia GÃ³mez: Melody Extraction From Polyphonic Music Signals Using Pitch 
+based on the report: __*Justin Salamon and Emilia Gomez: Melody Extraction From Polyphonic Music Signals Using Pitch 
 Contour Characteristics, IEEE Transactions on Audio, Speech, and Language Processing, vol. 20, no. 6, pp. 1759â€“1770, 
 2012.*__ Unfortunately, this method became unstable with further development and required the use of librosa. Due to 
 these limitations, the yin function replaced the swipe function to determine the fundamental frequency.
 
 
+Additionally, this version of PyTimbre included the code for the determination of waveform clipping taken from 
+clipdetect (https://pypi.org/project/clipdetect/#description). In similar manner as libf0, there were dependencies that
+were required by this package that increased the load of the PyTimbre installation. This code is incorporated within the
+Waveform class to make it available to all Waveform children classes. Usage of this code can be referenced this paper:
+__*Hansen, John H. L., Allen Stauffer, and Wei Xia. Nonlinear Waveform Distortion: Assessment and Detection of Clipping
+on Speech Data and Systems. Speech Communication 134 (2021): 20â€“31.*__
+
 # Usage Example
 ## 1. Defining a waveform from an array of values
 
-from pytimbre.waveform import Waveform
+    from pytimbre.waveform import Waveform
 
-fs = 48000
-w = 2 * np.pi * f
-t = np.arange(0, 10, 1/fs)
+    fs = 48000
+    w = 2 * np.pi * f
+    t = np.arange(0, 10, 1/fs)
 
-wfm = Waveform(0.75 * np.sin(w*t), fs, 0.0)
+    wfm = Waveform(0.75 * np.sin(w*t), fs, 0.0)
 
 ## 2. Define a waveform from a wav file
 
-from pytimbre.audio_files.wavefile import WaveFile
-wfm = wave_file(filename)
+    from pytimbre.audio_files.wavefile import WaveFile
+    wfm = wave_file(filename)
 
 ## 3. Obtain global temporal attributes
 
-from pytimbre.audio_files.wavefile import WaveFile
+    from pytimbre.audio_files.wavefile import WaveFile
 
-wfm = WaveFile(filename)
-print(wfm.amplitude_modulation)
+    wfm = WaveFile(filename)
+    print(wfm.amplitude_modulation)
 
 ## 4. Create single spectrogram and get a feature
 
-from pytimbre.audio_files.wavefile import WaveFile
-from pytimbre.spectra import SpectrumByFFT
+    from pytimbre.audio_files.wavefile import WaveFile
+    from pytimbre.spectra import SpectrumByFFT
 
-wfm = wave_file(filename)
-spectrum = SpectrumByFFT(wfm)
-print(spectrum.spectral_roll_off)
+    wfm = wave_file(filename)
+    spectrum = SpectrumByFFT(wfm)
+    print(spectrum.spectral_roll_off)
 
 # Clearance review and publication permission
 
 This software was developed in conjunction with research into the human perception of sound at the 711th Human 
 Performance Wing, Airman Systems Directorate.  
 
 It is approved for Distribution A, 88ABW-2020-2147.
```

### Comparing `PyTimbre-0.6.6/setup.py` & `PyTimbre-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         HISTORY = history_file.read()
 
         with open('LICENSE.txt') as license_file:
             LICENSE = license_file.read()
 
 setup(
     name='PyTimbre',
-    version='0.6.6',
+    version='0.6.7',
     description='Python conversion of Timbre Toolbox',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY + '\n\n' + LICENSE,
     license='MIT',
     packages=find_packages('src'),
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
```

### Comparing `PyTimbre-0.6.6/src/PyTimbre.egg-info/PKG-INFO` & `PyTimbre-0.6.7/src/PyTimbre.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -43,51 +43,58 @@
 These represent the sound quality metrics extracted from the Mosqito project (https://github.com/Eomys/MoSQITo).
 
 In addition to this code, PyTimbre has taken the code from libf0 (https://github.com/groupmm/libf0) that assists with 
 the computation of the fundamental frequency. There are a number of methods that exist within the libf0 module, but the
 package contains a number of dependencies that are not required for the other calculations and computations within
 PyTimbre. To facilitate the calculation of the fundamental frequency, the swipe class and associated functions were
 extracted and placed into PyTimbre. The code was extracted from the 1.0.2 version of the code on 1 April 2023. This is 
-based on the report: __*Justin Salamon and Emilia GÃ³mez: Melody Extraction From Polyphonic Music Signals Using Pitch 
+based on the report: __*Justin Salamon and Emilia Gomez: Melody Extraction From Polyphonic Music Signals Using Pitch 
 Contour Characteristics, IEEE Transactions on Audio, Speech, and Language Processing, vol. 20, no. 6, pp. 1759â€“1770, 
 2012.*__ Unfortunately, this method became unstable with further development and required the use of librosa. Due to 
 these limitations, the yin function replaced the swipe function to determine the fundamental frequency.
 
 
+Additionally, this version of PyTimbre included the code for the determination of waveform clipping taken from 
+clipdetect (https://pypi.org/project/clipdetect/#description). In similar manner as libf0, there were dependencies that
+were required by this package that increased the load of the PyTimbre installation. This code is incorporated within the
+Waveform class to make it available to all Waveform children classes. Usage of this code can be referenced this paper:
+__*Hansen, John H. L., Allen Stauffer, and Wei Xia. Nonlinear Waveform Distortion: Assessment and Detection of Clipping
+on Speech Data and Systems. Speech Communication 134 (2021): 20â€“31.*__
+
 # Usage Example
 ## 1. Defining a waveform from an array of values
 
-from pytimbre.waveform import Waveform
+    from pytimbre.waveform import Waveform
 
-fs = 48000
-w = 2 * np.pi * f
-t = np.arange(0, 10, 1/fs)
+    fs = 48000
+    w = 2 * np.pi * f
+    t = np.arange(0, 10, 1/fs)
 
-wfm = Waveform(0.75 * np.sin(w*t), fs, 0.0)
+    wfm = Waveform(0.75 * np.sin(w*t), fs, 0.0)
 
 ## 2. Define a waveform from a wav file
 
-from pytimbre.audio_files.wavefile import WaveFile
-wfm = wave_file(filename)
+    from pytimbre.audio_files.wavefile import WaveFile
+    wfm = wave_file(filename)
 
 ## 3. Obtain global temporal attributes
 
-from pytimbre.audio_files.wavefile import WaveFile
+    from pytimbre.audio_files.wavefile import WaveFile
 
-wfm = WaveFile(filename)
-print(wfm.amplitude_modulation)
+    wfm = WaveFile(filename)
+    print(wfm.amplitude_modulation)
 
 ## 4. Create single spectrogram and get a feature
 
-from pytimbre.audio_files.wavefile import WaveFile
-from pytimbre.spectra import SpectrumByFFT
+    from pytimbre.audio_files.wavefile import WaveFile
+    from pytimbre.spectra import SpectrumByFFT
 
-wfm = wave_file(filename)
-spectrum = SpectrumByFFT(wfm)
-print(spectrum.spectral_roll_off)
+    wfm = wave_file(filename)
+    spectrum = SpectrumByFFT(wfm)
+    print(spectrum.spectral_roll_off)
 
 # Clearance review and publication permission
 
 This software was developed in conjunction with research into the human perception of sound at the 711th Human 
 Performance Wing, Airman Systems Directorate.  
 
 It is approved for Distribution A, 88ABW-2020-2147.
```

### Comparing `PyTimbre-0.6.6/src/PyTimbre.egg-info/SOURCES.txt` & `PyTimbre-0.6.7/src/PyTimbre.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 setup.py
 src/PyTimbre.egg-info/PKG-INFO
 src/PyTimbre.egg-info/SOURCES.txt
 src/PyTimbre.egg-info/dependency_links.txt
 src/PyTimbre.egg-info/requires.txt
 src/PyTimbre.egg-info/top_level.txt
 src/pytimbre/__init__.py
-src/pytimbre/swipe.py
 src/pytimbre/waveform.py
 src/pytimbre/yin.py
 src/pytimbre/audio_files/__init__.py
 src/pytimbre/audio_files/ansi_standard_formatted_files.py
 src/pytimbre/audio_files/calibrated_binary_files.py
 src/pytimbre/audio_files/wavefile.py
 src/pytimbre/spectral/__init__.py
 src/pytimbre/spectral/acoustic_weights.py
 src/pytimbre/spectral/fractional_octave_band.py
+src/pytimbre/spectral/fundamental_frequency.py
 src/pytimbre/spectral/spectra.py
 src/pytimbre/spectral/spectrogram.py
+src/pytimbre/spectral/swipe.py
 src/pytimbre/spectral/time_histories.py
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/audio_files/ansi_standard_formatted_files.py` & `PyTimbre-0.6.7/src/pytimbre/audio_files/ansi_standard_formatted_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,117 +63,138 @@
         20230201 - FSM - Updated the methods to read the header information so that a variety of formatted
         information can be used in definition of the StandardBinaryFile object.
         """
 
         self._header = None
 
         if filename is not None:
-            #   Get the header and the location of the binary data
-            f_in, header = StandardBinaryFile.read_header(filename, header_element_count)
-            self._header = header
-
-            if header_only:
-                self._samples = None
-                return
-
-            #   Now to effectively understand how to read the data from the binary portion, we must determine
-            #   where specific data within the header exist. So look for the elements that were defined within
-            #   the function prototype.
-            #
-            #   The sample rate
-            if not (sample_rate_key in self.header.keys()):
-                raise ValueError("The name of the sample rate element of the waveform is not located within the "
-                                 "header dictionary. Please provide the correct name of the sample rate property")
-            else:
-                self.fs = float(header[sample_rate_key])
-
-            #   The start time of the audio file
-            if not (start_time_key in self.header.keys()):
-                raise ValueError(
-                    "The name of the start time element of the waveform is not located within the "
-                    "header dictionary. Please provide the correct name of the start time property")
-            else:
-                self.time0 = parser.parse(self.header[start_time_key])
-
-            #   The number of samples in the waveform
-            if not (sample_count_key in self.header.keys()):
-                raise ValueError("The number of samples must be provided, and the expected header element is not "
-                                 "found within the list of objects in the header.")
-            else:
-                self.sample_count = int(self.header[sample_count_key])
-
-            #   At this point there should be no reason for the data to be stored as anything other than REAL*4
-            #   Little Endian, but we do not account for any other formats, so we must now examine what is in the
-            #   header and exit if it is not what we expect.
-            if not (sample_format_key in self.header.keys()):
-                raise ValueError(
-                    "The name of the sample format element of the waveform is not located within the "
-                    "header dictionary. Please provide the correct name of the sample format property")
-            else:
-                if self.header[sample_format_key].upper() != "LITTLE ENDIAN":
-                    raise ValueError("The expected format is not present in the header.")
-
-            if not (data_format_key in self.header.keys()):
-                raise ValueError(
-                    "The name of the data format element of the waveform is not located within the "
-                    "header dictionary. Please provide the correct name of the data format property")
-            else:
-                if self.header[data_format_key].upper() != "REAL*4":
-                    raise ValueError("The required sample formate is not present in the header.")
-
-            self._data_offset = f_in.tell()
-
-            if s0 is not None:
-                if s0 > 0:
-                    # At this point we should interrogate the header to determine the size of the data sample,
-                    # but we are only supporting floating point values, so we can just increment the current location
-                    # by four times the desired start sample. So let's move the counter from the current position.
-                    f_in.seek(s0 * 4, 1)
-
-            #   Now we need to determine how many sample to read
-            samples_to_read = self.sample_count
-
-            if s0 is None and s1 is None:
-                samples_to_read = samples_to_read
-            elif s0 is not None and s1 is None:
-                samples_to_read -= s0
-                if isinstance(self.start_time, datetime):
-                    self.start_time += timedelta(seconds=s0 / self.sample_rate)
-                elif isinstance(self.start_time, float):
-                    self.start_time += s0 / self.sample_rate
-            elif s0 is None and s1 is not None:
-                samples_to_read = s1
-            elif s0 is not None and s1 is not None:
-                samples_to_read = s1 - s0
-                if isinstance(self.start_time, datetime):
-                    self.start_time += timedelta(seconds=s0 / self.sample_rate)
-                elif isinstance(self.start_time, float):
-                    self.start_time += s0 / self.sample_rate
-
-            #   Read the data - At this point we only support 32-bit/4-byte data samples
-            data = f_in.read(4 * samples_to_read)
-
-            #   Now unpack the data from the array of bytes into an array of floating point data
-            self._samples = np.asarray(struct.unpack('f'*samples_to_read, data))
-
-            if samples_to_read < self.sample_count:
-                self.sample_count = samples_to_read
-                self._samples -= np.mean(self.samples)
-
-            #   close the file
-            f_in.close()
+            self._read_file(filename, header_element_count, sample_rate_key, start_time_key, sample_format_key,
+                            data_format_key, sample_count_key, header_only, s0, s1)
         elif wfm is not None:
             super().__init__(wfm.samples, wfm.sample_rate, wfm.start_time)
             self._header = None
         else:
             self._samples = None
             self.fs = None
             self.time0 = None
             self._header = None
 
+    def _read_sample_rate(self, key):
+        if key not in self.header.keys():
+            raise ValueError("The name of the sample rate element of the waveform is not located within the "
+                             "header dictionary. Please provide the correct name of the sample rate property")
+        else:
+            self.fs = float(self.header[key])
+
+    def _read_start_time(self, key):
+        if key not in self.header.keys():
+            raise ValueError(
+                "The name of the start time element of the waveform is not located within the "
+                "header dictionary. Please provide the correct name of the start time property")
+        else:
+            self.time0 = parser.parse(self.header[key])
+
+    def _read_sample_count(self, key):
+        if key not in self.header.keys():
+            raise ValueError("The number of samples must be provided, and the expected header element is not "
+                             "found within the list of objects in the header.")
+        else:
+            self.sample_count = int(self.header[key])
+
+    def _read_format(self, sample_format_key, data_format_key):
+        if sample_format_key not in self.header.keys():
+            raise ValueError(
+                "The name of the sample format element of the waveform is not located within the "
+                "header dictionary. Please provide the correct name of the sample format property")
+        else:
+            if self.header[sample_format_key].upper() != "LITTLE ENDIAN":
+                raise ValueError("The expected format is not present in the header.")
+
+        if data_format_key not in self.header.keys():
+            raise ValueError(
+                "The name of the data format element of the waveform is not located within the "
+                "header dictionary. Please provide the correct name of the data format property")
+        else:
+            if self.header[data_format_key].upper() != "REAL*4":
+                raise ValueError("The required sample formate is not present in the header.")
+
+    def _define_samples_to_read(self, s0, s1):
+        samples_to_read = self.sample_count
+
+        if s0 is not None and s1 is None:
+            samples_to_read -= s0
+            if isinstance(self.start_time, datetime):
+                self.start_time += timedelta(seconds=s0 / self.sample_rate)
+            elif isinstance(self.start_time, float):
+                self.start_time += s0 / self.sample_rate
+        elif s0 is None and s1 is not None:
+            samples_to_read = s1
+        elif s0 is not None and s1 is not None:
+            samples_to_read = s1 - s0
+            if isinstance(self.start_time, datetime):
+                self.start_time += timedelta(seconds=s0 / self.sample_rate)
+            elif isinstance(self.start_time, float):
+                self.start_time += s0 / self.sample_rate
+
+        return samples_to_read
+
+    def _read_file(self, filename, header_element_count: int = None,
+                   sample_rate_key: str = 'SAMPLE RATE (HZ)', start_time_key: str = 'TIME (UTC ZULU)',
+                   sample_format_key: str = 'SAMPLE FORMAT', data_format_key: str = 'DATA FORMAT',
+                   sample_count_key: str = 'SAMPLES TOTAL', header_only: bool = False, s0=None, s1=None):
+        #   Get the header and the location of the binary data
+        f_in, header = StandardBinaryFile.read_header(filename, header_element_count)
+        self._header = header
+
+        if header_only:
+            self._samples = None
+            return
+
+        #   Now to effectively understand how to read the data from the binary portion, we must determine
+        #   where specific data within the header exist. So look for the elements that were defined within
+        #   the function prototype.
+        #
+        #   The sample rate
+        self._read_sample_rate(sample_rate_key)
+
+        #   The start time of the audio file
+        self._read_start_time(start_time_key)
+
+        #   The number of samples in the waveform
+        self._read_sample_count(sample_count_key)
+
+        #   At this point there should be no reason for the data to be stored as anything other than REAL*4
+        #   Little Endian, but we do not account for any other formats, so we must now examine what is in the
+        #   header and exit if it is not what we expect.
+        self._read_format(sample_format_key, data_format_key)
+
+        self._data_offset = f_in.tell()
+
+        if s0 is not None and s0 > 0:
+            # At this point we should interrogate the header to determine the size of the data sample,
+            # but we are only supporting floating point values, so we can just increment the current location
+            # by four times the desired start sample. So let's move the counter from the current position.
+            f_in.seek(s0 * 4, 1)
+
+        #   Now we need to determine how many sample to read
+        samples_to_read = self._define_samples_to_read(s0, s1)
+
+        #   Read the data - At this point we only support 32-bit/4-byte data samples
+        data = f_in.read(4 * samples_to_read)
+
+        #   Now unpack the data from the array of bytes into an array of floating point data
+        self._samples = np.asarray(struct.unpack('f' * samples_to_read, data))
+
+        if samples_to_read < self.sample_count:
+            self.sample_count = samples_to_read
+            self._samples -= np.mean(self.samples)
+
+        #   close the file
+        f_in.close()
+
     @staticmethod
     def convert_header(header_line):
         """
         This function will take the information within the header line and remove
         the semicolon in the front and all ellipsoid markers to determine the name
         of the property.  It also splits based on the colon to determine the value
 
@@ -502,15 +523,15 @@
         else:
             wav.title = os.path.basename(wav_path)
         if subject_name is not None:
             wav.subject_name = subject_name
         if description is not None:
             wav.description = description
 
-        wav.creation_software = "Python, AFRL_Physical_Acoustics "
+        wav.creation_software = "Python, PyTimbre "
 
         if data_source is not None:
             wav.data_source = data_source
         if original_form is not None:
             wav.original_form = original_form
         if digitizing_engineer is not None:
             wav.digitizing_engineer = digitizing_engineer
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/audio_files/calibrated_binary_files.py` & `PyTimbre-0.6.7/src/pytimbre/audio_files/calibrated_binary_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os.path
+
 import pandas as pd
 from datetime import datetime, timedelta
 from dateutil import parser
 import numpy as np
 import struct
 from pytimbre.waveform import Waveform
 
@@ -14,187 +16,34 @@
 
         :param filename: string
             the location of the file that will be read
 
         :param irig_ch: int or str (optional)
             the channel of the IRIG recording on the specific recorder
         """
+        self.CHANNEL_INDEX_NAME = "Channel Index"
+        self.DEVICE_NUMBER_NAME = 'Device Number'
+        self.SENSOR_SENSITIVITY = 'Sensitivity (mv/EU)'
+        self.EXTERNAL_GAIN = 'Ext. Gain (Lin.)'
+        self.INPUT_VOLTAGE_RANGE = 'Input Range (+/- V)'
+        self.IEPE_POWER_SOURCE = 'IEPE Source'
+        self.IEPE_POWER_LEVEL = 'IEPE Value (mA)'
 
+        self.filename = os.path.basename(filename)[:-4].split('_')[0]
         self._duration = 0
 
         f = open(filename, 'rt')
 
         fileline = f.readline()
         if 'STANDARD LOG FILE PARAMETERS' in fileline:
-            fileline = " "
-            while fileline != "":
-                fileline = f.readline()
-                if fileline.find(':') >= 0:
-                        command = fileline.split(':')[0]
-                        command = fileline.split('.')[0]
-                        data = fileline.split(':')[1]
-
-                        if command == 'FILENAME':
-                            self.Filename = data[1:-1]
-                        elif command == "DATE (mm/dd/yyyy)":
-                            self._start_time = parser.parse(data[1:-1])
-                        elif command == "START TIME":
-                            data = fileline.split(':',1)[1]
-                            dt = parser.parse(data)
-                            self._start_time += timedelta(seconds=60 * (60 * dt.hour + dt.minute) + dt.second +
-                                                                  dt.microsecond * 1e-6)
-                        elif command == "OFFSET FRM UTC (hrs)":
-                            self.GMT_Offset = float(data[1:-1])
-                        elif command == "TIME ZONE":
-                            self.time_zone = data[1:-1]
-                        elif command == "FILE COMMENTS":
-                            self.comments = data[1:-1]
-                        elif command == "NUMBER CHANNELS":
-                            self._channel_no = int(data[1:-1])
-                        elif command == "SAMPLE RATE (Hz)":
-                            self.fs = float(data[1:-1])
-                        # elif command == "Block Size":
-                        #     self.block_size = float(data[1:-1])
-                        elif command == "AFR SOFTWARE VERSION":
-                            self.AFR_Version = data[1:-1]
-                        elif command == "CONFIGURED CHANNEL SETTINGS":
-                            fileline = f.readline()
-                            fileline = f.readline()
-                            fileline = f.readline()
-
-                            self.channel_settings = pd.DataFrame(columns=['Channel Index', 'Device Number',
-                                                                          'Sensitivity (mv/EU)', 'Ext. Gain (Lin.)',
-                                                                          'Input Range (+/- V)', 'IEPE Source',
-                                                                          'IEPE Value (mA)'])
-
-                            for i in range(self._channel_no):
-                                fileline = f.readline()
-
-                                data = fileline.split('\t')
-
-                                row = {'Channel Index': int(data[0]),
-                                       'Device Number': data[1],
-                                       'Sensitivity (mv/EU)': float(data[2]),
-                                       'Ext. Gain (Lin.)': float(data[3]),
-                                       'Input Range (+/- V)': float(data[5]),
-                                       'IEPE Source': data[6],
-                                       'IEPE Value (mA)': float(data[7])}
-
-                                self.channel_settings = self.channel_settings.append(row, ignore_index=True)
+            self._read_standard_file(f)
         elif fileline.upper() == "AIR FORCE RESEARCH LABORATORY LOG FILE PARAMETERS\n":
-            while fileline != "":
-                fileline = f.readline()
-                if fileline.find(':') >= 0:
-                        command = fileline.split(':')[0].upper()
-                        data = fileline.split(':')[1]
-
-                        if command == 'FILE NAME':
-                            self.Filename = data[:-1]
-                        elif command == "DATE":
-                            self._start_time = parser.parse(data[:-1])
-                        elif command == "TIME":
-                            data = fileline.split(':', 1)[1]
-                            dt = parser.parse(data)
-                            self._start_time += timedelta(seconds=60 * (60 * dt.hour + dt.minute) + dt.second +
-                                                                  dt.microsecond * 1e-6)
-                        elif command == "OFFSET FROM GMT (H)":
-                            self.GMT_Offset = float(data[1:-1])
-                        elif command == "COMMENTS":
-                            self.comments = data[:-1]
-                        elif command == "NUMBER OF CHANNELS":
-                            self._channel_no = int(data[:-1])
-                        elif command == "SAMPLING FREQUENCY (HZ)":
-                            self.fs = float(data[:-1])
-                        elif command == "BLOCK SIZE":
-                            self.block_size = float(data[:-1])
-                        # elif command == "AFR SOFTWARE VERSION":
-                        #     self.AFR_Version = data[1:-1]
-                        elif command == "ACTUAL RECORD LENGTH":
-                            duration = float(data)
-                            self._duration = duration
-                        elif command == "CONFIGURATION":
-                            #   Get the column names and create the DataFrame for the configuration
-
-                            column_names = f.readline().split(',')
-                            self.channel_settings = pd.DataFrame(columns=column_names)
-
-                            #   Loop through the file until we have read a line for each channel within the measurement
-
-                            channels_read = 0
-                            while channels_read < self._channel_no:
-                                fileline = f.readline()
-
-                                if fileline != "":
-                                    data = fileline.split(',')
-
-                                    row = dict()
-
-                                    for i in range(len(column_names)):
-                                        row[column_names[i]] = data[i]
-
-                                    self.channel_settings = self.channel_settings.append(row, ignore_index=True)
-
-                                    channels_read += 1
-
+            self._read_afrl_file(f)
         else:
-            fileline = " "
-            while fileline != "":
-                fileline = f.readline()
-
-                if fileline.find(':') >= 0:
-                    command = fileline.split(':')[0]
-                    data = fileline.split(':')[1]
-
-                    if command == 'File Name':
-                        self.Filename = data[1:-1]
-                    elif command == "Date":
-                        self._start_time = parser.parse(data[1:-1])
-                    elif command == "Start Time" or command == "Time":
-                        data = fileline.split('\t')[1]
-                        dt = parser.parse(data)
-                        self._start_time += timedelta(seconds=60 * (60 * dt.hour + dt.minute) + dt.second +
-                                                      dt.microsecond * 1e-6)
-                    elif command == "Offset from GMT (h)":
-                        self.GMT_Offset = float(data[1:-1])
-                    elif command == "Time Zone":
-                        self.time_zone = data[1:-1]
-                    elif command == "File Comments":
-                        self.comments = data[1:-1]
-                    elif command == "Number of Channels":
-                        self._channel_no = int(data[1:-1])
-                    elif command == "Sampling Frequency (Hz)":
-                        self.fs = float(data[1:-1])
-                    elif command == "Block Size":
-                        self.block_size = float(data[1:-1])
-                    elif command == "AFR Software Version":
-                        self.AFR_Version = data[1:-1]
-                    elif command == "Configured Channel Settings":
-                        fileline = f.readline()
-                        fileline = f.readline()
-                        fileline = f.readline()
-
-                        self.channel_settings = pd.DataFrame(columns=['Channel Index', 'Device Number',
-                                                                      'Sensitivity (mv/EU)', 'Ext. Gain (Lin.)',
-                                                                      'Input Range (+/- V)', 'IEPE Source',
-                                                                      'IEPE Value (mA)'])
-
-                        for i in range(self._channel_no):
-                            fileline = f.readline()
-
-                            data = fileline.split('\t')
-
-                            row = {'Channel Index': int(data[0]),
-                                   'Device Number': data[1],
-                                   'Sensitivity (mv/EU)': float(data[2]),
-                                   'Ext. Gain (Lin.)': float(data[3]),
-                                   'Input Range (+/- V)': float(data[5]),
-                                   'IEPE Source': data[6],
-                                   'IEPE Value (mA)': float(data[7])}
-
-                            self.channel_settings = self.channel_settings.append(row, ignore_index=True)
+            self._read_miscellaneous(f)
         f.close()
 
         self.irig_ch = irig_ch
 
     @property
     def channel_number(self):
         return self._channel_no
@@ -211,14 +60,186 @@
     def record_duration(self):
         return self._duration
 
     @property
     def stop_time(self):
         return self.start_time + timedelta(seconds=self.record_duration)
 
+    def _read_standard_file(self, f):
+        fileline = " "
+        while fileline != "":
+            fileline = f.readline()
+            if fileline.find(':') >= 0:
+                command = fileline.split('.')[0]
+                data = fileline.split(':')[1]
+
+                if command == 'FILENAME':
+                    self.filename = data[1:-1]
+                elif command == "DATE (mm/dd/yyyy)":
+                    self._start_time = parser.parse(data[1:-1])
+                elif command == "START TIME":
+                    data = fileline.split(':', 1)[1]
+                    dt = parser.parse(data)
+                    self._start_time += timedelta(seconds=60 * (60 * dt.hour + dt.minute) + dt.second +
+                                                          dt.microsecond * 1e-6)
+                elif command == "OFFSET FRM UTC (hrs)":
+                    self.gmt_offset = float(data[1:-1])
+                elif command == "TIME ZONE":
+                    self.time_zone = data[1:-1]
+                elif command == "FILE COMMENTS":
+                    self.comments = data[1:-1]
+                elif command == "NUMBER CHANNELS":
+                    self._channel_no = int(data[1:-1])
+                elif command == "SAMPLE RATE (Hz)":
+                    self.fs = float(data[1:-1])
+                # elif command == "Block Size":
+                #     self.block_size = float(data[1:-1])
+                elif command == "AFR SOFTWARE VERSION":
+                    self.acquisition_software_version = data[1:-1]
+                elif command == "CONFIGURED CHANNEL SETTINGS":
+                    _ = f.readline()
+                    _ = f.readline()
+                    fileline = f.readline()
+
+                    self.channel_settings = pd.DataFrame(columns=[self.CHANNEL_INDEX_NAME,
+                                                                  self.DEVICE_NUMBER_NAME,
+                                                                  self.SENSOR_SENSITIVITY,
+                                                                  self.EXTERNAL_GAIN,
+                                                                  self.INPUT_VOLTAGE_RANGE,
+                                                                  self.IEPE_POWER_SOURCE,
+                                                                  self.IEPE_POWER_LEVEL])
+
+                    for i in range(self._channel_no):
+                        fileline = f.readline()
+
+                        data = fileline.split('\t')
+
+                        row = {self.CHANNEL_INDEX_NAME: int(data[0]),
+                               self.DEVICE_NUMBER_NAME: data[1],
+                               self.SENSOR_SENSITIVITY: float(data[2]),
+                               self.EXTERNAL_GAIN: float(data[3]),
+                               self.INPUT_VOLTAGE_RANGE: float(data[5]),
+                               self.IEPE_POWER_SOURCE: data[6],
+                               self.IEPE_POWER_LEVEL: float(data[7])}
+
+                        self.channel_settings = self.channel_settings.append(row, ignore_index=True)
+
+    def _read_afrl_file(self, f):
+        fileline = " "
+        while fileline != "":
+            fileline = f.readline()
+            if fileline.find(':') >= 0:
+                command = fileline.split(':')[0].upper()
+                data = fileline.split(':')[1]
+
+                if command == 'FILE NAME':
+                    self.filename = data[:-1]
+                elif command == "DATE":
+                    self._start_time = parser.parse(data[:-1])
+                elif command == "TIME":
+                    data = fileline.split(':', 1)[1]
+                    dt = parser.parse(data)
+                    self._start_time += timedelta(seconds=60 * (60 * dt.hour + dt.minute) + dt.second +
+                                                          dt.microsecond * 1e-6)
+                elif command == "OFFSET FROM GMT (H)":
+                    self.gmt_offset = float(data[1:-1])
+                elif command == "COMMENTS":
+                    self.comments = data[:-1]
+                elif command == "NUMBER OF CHANNELS":
+                    self._channel_no = int(data[:-1])
+                elif command == "SAMPLING FREQUENCY (HZ)":
+                    self.fs = float(data[:-1])
+                elif command == "BLOCK SIZE":
+                    self.block_size = float(data[:-1])
+                # elif command == "AFR SOFTWARE VERSION":
+                #     self.AFR_Version = data[1:-1]
+                elif command == "ACTUAL RECORD LENGTH":
+                    duration = float(data)
+                    self._duration = duration
+                elif command == "CONFIGURATION":
+                    #   Get the column names and create the DataFrame for the configuration
+
+                    column_names = f.readline().split(',')
+                    self.channel_settings = pd.DataFrame(columns=column_names)
+
+                    #   Loop through the file until we have read a line for each channel within the measurement
+
+                    channels_read = 0
+                    while channels_read < self._channel_no:
+                        fileline = f.readline()
+
+                        if fileline != "":
+                            data = fileline.split(',')
+
+                            row = dict()
+
+                            for i in range(len(column_names)):
+                                row[column_names[i]] = data[i]
+
+                            self.channel_settings = self.channel_settings.append(row, ignore_index=True)
+
+                            channels_read += 1
+
+    def _read_miscellaneous(self, f):
+        fileline = " "
+        while fileline != "":
+            fileline = f.readline()
+
+            if fileline.find(':') >= 0:
+                command = fileline.split(':')[0]
+                data = fileline.split(':')[1]
+
+                if command == 'File Name':
+                    self.filename = data[1:-1]
+                elif command == "Date":
+                    self._start_time = parser.parse(data[1:-1])
+                elif command == "Start Time" or command == "Time":
+                    data = fileline.split('\t')[1]
+                    dt = parser.parse(data)
+                    self._start_time += timedelta(seconds=60 * (60 * dt.hour + dt.minute) + dt.second +
+                                                          dt.microsecond * 1e-6)
+                elif command == "Offset from GMT (h)":
+                    self.gmt_offset = float(data[1:-1])
+                elif command == "Time Zone":
+                    self.time_zone = data[1:-1]
+                elif command == "File Comments":
+                    self.comments = data[1:-1]
+                elif command == "Number of Channels":
+                    self._channel_no = int(data[1:-1])
+                elif command == "Sampling Frequency (Hz)":
+                    self.fs = float(data[1:-1])
+                elif command == "Block Size":
+                    self.block_size = float(data[1:-1])
+                elif command == "AFR Software Version":
+                    self.acquisition_software_version = data[1:-1]
+                elif command == "Configured Channel Settings":
+                    _ = f.readline()
+                    _ = f.readline()
+                    fileline = f.readline()
+
+                    self.channel_settings = pd.DataFrame(columns=[self.CHANNEL_INDEX_NAME, self.DEVICE_NUMBER_NAME,
+                                                                  self.SENSOR_SENSITIVITY, self.EXTERNAL_GAIN,
+                                                                  self.INPUT_VOLTAGE_RANGE, self.IEPE_POWER_SOURCE,
+                                                                  self.IEPE_POWER_LEVEL])
+
+                    for i in range(self._channel_no):
+                        fileline = f.readline()
+
+                        data = fileline.split('\t')
+
+                        row = {self.CHANNEL_INDEX_NAME: int(data[0]),
+                               self.DEVICE_NUMBER_NAME: data[1],
+                               self.SENSOR_SENSITIVITY: float(data[2]),
+                               self.EXTERNAL_GAIN: float(data[3]),
+                               self.INPUT_VOLTAGE_RANGE: float(data[5]),
+                               self.IEPE_POWER_SOURCE: data[6],
+                               self.IEPE_POWER_LEVEL: float(data[7])}
+
+                        self.channel_settings = self.channel_settings.append(row, ignore_index=True)
+
 
 class CalibratedBinaryFile(Waveform):
     def __init__(self, log, path, run_id=None, ch_id=None, s0=None, s1=None, sync='log_start_time'):
         """
         This function loads the waveform from the legacy measurement and adjusts for the DC offset
         :param path: string
             The path to the binary audio file
@@ -234,32 +255,33 @@
             the end sample to read from the file
         :param sync: string {'log_start_time' (default), 'irig_start_time'}
             log_start_time defines the waveform start time by the documented time in the log file.
             irig_start_time defines the waveform start time via an IRIG-B signal, and requires that log.irig_ch be populated with the appropriate IRIG channel number on the recorder.
         """
 
         if not isinstance(log, MeasurementLogFile):
-            raise Exception("Arugment invalid")
+            raise ValueError("Arugment invalid")
 
         if run_id is not None and ch_id is not None:
             run_str = CalibratedBinaryFile.set_record_id_to_legacy_format(run_id)
             ch_str = CalibratedBinaryFile.set_channel_to_legacy_format(ch_id)
             data_path = "{}/{}_{}.bin".format(path, run_str, ch_str)
         else:
             data_path = path
 
         y = CalibratedBinaryFile.read_bin_file(data_path, s0, s1)
 
         if sync == 'log_start_time':
             t0 = log.start_time
         elif sync == 'irig_start_time':
             tpm_s = CalibratedBinaryFile.sync_to_irig(log, data_path)
-            t0 = datetime(year=log.start_time.year, month=log.start_time.month, day=log.start_time.day) + timedelta(seconds=tpm_s)
+            t0 = datetime(year=log.start_time.year, month=log.start_time.month, day=log.start_time.day) + timedelta(
+                seconds=tpm_s)
         elif sync == 'zero':
-            t0 = datetime(year=1, month=1, day=1,hour=0, minute=0,second=0)
+            t0 = datetime(year=1, month=1, day=1, hour=0, minute=0, second=0)
         else:
             raise ValueError('Input sync must be "log_start_time" or "irig_start_time" or "zero".')
 
         if s0 is not None:
             t0 += timedelta(seconds=s0 / log.sample_rate)
 
         super().__init__(y, log.sample_rate, t0)
@@ -310,17 +332,15 @@
             f.seek(s0 * 4)
 
         #   Determine the number of samples - the data is stored as a single precision floating point value
         #   We need to determine the number that we want to read.  If the starting sample is the beginning and the
         #   ending sample is none, then we read the entire file
         N = int(byte_count / 4)
 
-        if s0 is None and s1 is None:
-            N = N
-        elif s0 is not None and s1 is None:
+        if s0 is not None and s1 is None:
             N -= s0
         elif s0 is None and s1 is not None:
             N = s1
         elif s0 is not None and s1 is not None:
             N = s1 - s0
 
         #   Read the contents of the file and unpack them as a single
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/audio_files/wavefile.py` & `PyTimbre-0.6.7/src/pytimbre/audio_files/wavefile.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.6/src/pytimbre/spectral/acoustic_weights.py` & `PyTimbre-0.6.7/src/pytimbre/spectral/acoustic_weights.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     FSM - the math module was replaced with references to the numpy module to facilitate use with numpy arrays and the
     pandas DataFrame objects
     """
 
     #TODO: Frank - make this more generic
     @staticmethod
-    def sound_exposure_level(times, levels, dB_down):
+    def sound_exposure_level(times, levels, decibel_down):
         """
         The sound exposure level attempts to determine the equivalent level of the acoustic energy placed within a
         single second of the acoustic level.  The dB_down parameter determines how far below the peak that the algorithm
         seeks to integrate the data.
 
         times : datetime, array-like
             a collection of datetime objects that represent the times for the acoustic levels
@@ -29,15 +29,15 @@
 
         returns : double
             the integrated level between the times marking the location of the dB_down levels.
         """
 
         #   Find the indices for the integration
 
-        start_index, stop_index = AcousticWeights.find_dB_down_limits(levels, dB_down)
+        start_index, stop_index = AcousticWeights.find_decibel_down_limits(levels, decibel_down)
 
         #   Determine the equivalent level between these times
         if isinstance(times[0], datetime.datetime):
             tin = (times[stop_index] - times[start_index]).total_seconds()
         else:
             tin = times[stop_index] - times[start_index]
 
@@ -45,15 +45,15 @@
             levels,
             tin,
             1,
             start_index,
             stop_index)
 
     @staticmethod
-    def find_dB_down_limits(levels, dB_down_level):
+    def find_decibel_down_limits(levels, decibel_down_level):
         """
         Examine the array of levels and determine the points that were above the peak - dB_down_level
 
         levels : double, array-like
             the acoustic levels in an array that will be examined
         dB_down_level : double
             the level below the peak that will set the limits of the integration
@@ -70,23 +70,23 @@
 
         max_index = np.argmax(levels)
 
         #   Determine the start_index
 
         start_index = -1
         for i in range(max_index, -1, -1):
-            if levels[i] <= (max_level - dB_down_level):
+            if levels[i] <= (max_level - decibel_down_level):
                 start_index = i
                 break
 
         #   Determine the stop_index
 
         stop_index = -1
         for i in range(max_index, len(levels), 1):
-            if levels[i] <= (max_level - dB_down_level):
+            if levels[i] <= (max_level - decibel_down_level):
                 stop_index = i
                 break
 
         #   Apply some constraints to ensure that we are within the limits of the array
 
         if start_index < 0:
             start_index = 0
@@ -207,222 +207,170 @@
         f1 = 20.598997
         f4 = 12194.22
         K1 = 2.24e16
         numerator = K1 * frequency**4
         denominator = ((frequency**2 + f1**2)**2.0) * ((frequency**2 + f4**2)**2.0)
 
         frac = numerator / denominator
-        # frac[frac <= 0] = np.nextafter(0, 1)
         return 10 * numpy.log10(frac)
 
     @staticmethod
-    def pnl(dSPL):
+    def pnl(sound_pressure_level):
         """
         Determine the single number perceived noise level (PNL) based on the conversion from dB to Noys
 
         dSPL : double, array-like
             the sound pressure levels from 10 Hz to 10 kHz
 
         returns : double
             returns the perceived noise level in NOYS
 
         Remarks:
         2022-12-13 - FSM - Changed the end of the code to ensure that there is a non-infinite results when the sume of
             the levels is zero because the level is too quiet.
         """
 
-        Ld = [49, 44, 39, 34, 30, 27, 24, 21, 18, 16, 16, 16, 16, 16, 15, 12, 9, 5, 4, 5, 6, 10, 17, 21]
-        Le = [55, 51, 46, 42, 39, 36, 33, 30, 27, 25, 25, 25, 25, 25, 23, 21, 18, 15, 14, 14, 15, 17, 23, 29]
-        Lb = [64, 60, 56, 53, 51, 48, 46, 44, 42, 40, 40, 40, 40, 40, 38, 34, 32, 30, 29, 29, 30, 31, 37, 41]
-        La = [91.01, 85.88, 87.32, 79.85, 79.76, 75.96, 73.96, 74.91, 94.63, 1000, 1000, 1000, 1000, 1000, 1000, 1000,
+        ld = [49, 44, 39, 34, 30, 27, 24, 21, 18, 16, 16, 16, 16, 16, 15, 12, 9, 5, 4, 5, 6, 10, 17, 21]
+        le = [55, 51, 46, 42, 39, 36, 33, 30, 27, 25, 25, 25, 25, 25, 23, 21, 18, 15, 14, 14, 15, 17, 23, 29]
+        lb = [64, 60, 56, 53, 51, 48, 46, 44, 42, 40, 40, 40, 40, 40, 38, 34, 32, 30, 29, 29, 30, 31, 37, 41]
+        la = [91.01, 85.88, 87.32, 79.85, 79.76, 75.96, 73.96, 74.91, 94.63, 1000, 1000, 1000, 1000, 1000, 1000, 1000,
               1000, 1000, 1000, 1000, 1000, 1000, 44.29, 50.72]
-        Lc = [52, 51, 49, 47, 46, 45, 43, 42, 41, 40, 40, 40, 40, 40, 38, 34, 32, 30, 29, 29, 30, 31, 34, 37]
-        Md = [0.079520, 0.068160, 0.068160, 0.059640, 0.053013, 0.053013, 0.053013, 0.053013, 0.053013, 0.053013,
+        lc = [52, 51, 49, 47, 46, 45, 43, 42, 41, 40, 40, 40, 40, 40, 38, 34, 32, 30, 29, 29, 30, 31, 34, 37]
+        md = [0.079520, 0.068160, 0.068160, 0.059640, 0.053013, 0.053013, 0.053013, 0.053013, 0.053013, 0.053013,
               0.053013, 0.053013, 0.053013, 0.053013, 0.059640, 0.053013, 0.053013, 0.047712, 0.047712, 0.053013,
               0.053013, 0.068160, 0.079520, 0.059640]
-        Me = [0.058098, 0.058098, 0.052288, 0.047534, 0.043573, 0.043573, 0.040221, 0.037349, 0.034859, 0.034859,
+        me = [0.058098, 0.058098, 0.052288, 0.047534, 0.043573, 0.043573, 0.040221, 0.037349, 0.034859, 0.034859,
               0.034859, 0.034859, 0.034859, 0.034859, 0.034859, 0.040221, 0.037349, 0.034859, 0.034859, 0.034859,
               0.034859, 0.037349, 0.037349, 0.043573]
-        Mc = [0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0, 0, 0, 0, 0,
+        mc = [0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0, 0, 0, 0, 0,
               0, 0, 0, 0, 0, 0, 0, 0, 0.02996, 0.02996]
-        Mb = [0.043478, 0.04057, 0.036831, 0.036831, 0.035336, 0.033333, 0.033333, 0.032051, 0.030675, 0.030103,
+        mb = [0.043478, 0.04057, 0.036831, 0.036831, 0.035336, 0.033333, 0.033333, 0.032051, 0.030675, 0.030103,
               0.030103, 0.030103, 0.030103, 0.030103, 0.030103, 0.02996, 0.02996, 0.02996, 0.02996, 0.02996, 0.02996,
               0.02996, 0.042285, 0.042285]
-        dfn = [0.0 for i in range(31)]
-        d_sum = 0.0
-        fFJ = 0.15
+        dfn = np.zeros((31,))
         for j in range(0, 7, 1):
             dfn[j] = 0
         for i in range(7, 31, 1):
-            if dSPL[i] > 250:
+            if sound_pressure_level[i] > 250:
                 return -1000
 
-            if dSPL[i] >= La[i - 7]:
-                dfn[i] = AcousticWeights.ILOG10(Mc[i - 7] * (dSPL[i] - Lc[i - 7]))
+            if sound_pressure_level[i] >= la[i - 7]:
+                dfn[i] = AcousticWeights.inverse_log_base_10(mc[i - 7] * (sound_pressure_level[i] - lc[i - 7]))
 
-            elif Lb[i - 7] <= dSPL[i] < La[i - 7]:
-                dfn[i] = AcousticWeights.ILOG10(Mb[i - 7] * (dSPL[i] - Lb[i - 7]))
+            elif lb[i - 7] <= sound_pressure_level[i] < la[i - 7]:
+                dfn[i] = AcousticWeights.inverse_log_base_10(mb[i - 7] * (sound_pressure_level[i] - lb[i - 7]))
 
-            elif Le[i - 7] <= dSPL[i] < Lb[i - 7]:
-                dfn[i] = AcousticWeights.ILOG10(Me[i - 7] * (dSPL[i] - Lb[i - 7]))
+            elif le[i - 7] <= sound_pressure_level[i] < lb[i - 7]:
+                dfn[i] = AcousticWeights.inverse_log_base_10(me[i - 7] * (sound_pressure_level[i] - lb[i - 7]))
 
-            elif Ld[i - 7] <= dSPL[i] < Le[i - 7]:
-                dfn[i] = 0.1 * AcousticWeights.ILOG10(Md[i - 7] * (dSPL[i] - Ld[i - 7]))
+            elif ld[i - 7] <= sound_pressure_level[i] < le[i - 7]:
+                dfn[i] = 0.1 * AcousticWeights.inverse_log_base_10(md[i - 7] * (sound_pressure_level[i] - ld[i - 7]))
 
-            if abs(dfn[i]) > 300:
-                dfn[i] = 0
-
-            if abs(dfn[i]) < -300:
-                dfn[i] = 0
-
-            if abs(dfn[i]) < 1e-10:
+            if abs(dfn[i]) > 300 or abs(dfn[i]) < -300 or abs(dfn[i]) < 1e-10:
                 dfn[i] = 0
 
             if dfn[i] > 2048:
                 return -2000
 
-        for i in range(0, 31, 1):
-            if dfn[i] == float('inf'):
-                dfn[i] = 0.0
-        damx = dfn[7]
+        dfn[np.isinf(dfn)[0]] = 0
+        d_max = np.max(dfn[7:])
+        d_sum = np.sum(dfn[7:])
 
-        for i in range(7, 31, 1):
-            if dfn[i] > damx:
-                damx = dfn[i]
-            d_sum += dfn[i]
-        d_sum = (d_sum - damx) * fFJ + damx
+        d_sum = (d_sum - d_max) * 0.15 + d_max
 
         if d_sum == 0:
             d_sum = 1
         return 40 + 33.22 * numpy.log10(d_sum)
 
     @staticmethod
-    def ILOG10(x):
+    def inverse_log_base_10(x):
         """
         Determine the inverse log10, or 10**x
         """
 
         return 10.0 ** x
 
     @staticmethod
-    def tone_correction(dSPL):
+    def tone_correction(sound_pressure_levels):
+        import copy
         """
         This function determines the tone correction applied to the sound pressure level spectrum.  It is based on the
         description of the calculation within the FAR part 36, Appendix A36.4.3.1.
 
-        dSPL : double, array-like
+        :param sound_pressure_levels: double, array-like
             the collection of sound pressure levels from 10 Hz to 10 kHz
 
         returns : double
             the single value tone correction for the spectrum to be applied to the integrated acoustic levels.
         """
 
         #   Step 1 - Calculate the changes in adjacent sound pressure levels (or slopes)
-
-        slopes = [0.0 for x in range(len(dSPL))]
-        for i in range(0, len(slopes), 1):
-            if i < 10:
-                slopes[i] = 0.0
-            else:
-                slopes[i] = dSPL[i] - dSPL[i - 1]
+        slopes = np.zeros(len(sound_pressure_levels))
+        slopes[10:] = np.diff(sound_pressure_levels)[9:]
 
         #   Step 2 - find any slope changes greater than 5
-
-        large_slope_changes = [False for x in range(len(dSPL))]
-        for i in range(0, len(large_slope_changes), 1):
-            if abs(slopes[i]) > 5:
-                large_slope_changes[i] = True
-            else:
-                large_slope_changes[i] = False
+        large_slope_changes = abs(slopes) > 5
 
         #   Step 3 - select the sound pressure level that needs to be corrected
-
-        select_sound_pressure_level = [False for x in range(len(dSPL))]
+        select_sound_pressure_level = np.zeros((len(sound_pressure_levels),), dtype=bool)
         for i in range(1, len(select_sound_pressure_level), 1):
             if large_slope_changes[i]:
                 if slopes[i] > 0 and slopes[i] > slopes[i - 1]:
                     select_sound_pressure_level[i] = True
-                elif slopes[i] <= 0 and slopes[i - 1] > 0:
+                elif slopes[i] <= 0 < slopes[i - 1]:
                     select_sound_pressure_level[i - 1] = True
-                else:
-                    select_sound_pressure_level[i] = False
-            else:
-                select_sound_pressure_level[i] = False
 
         #   Step 4 - Adjust selected sound pressure levels
-
-        spl_prime = [0.0 for x in range(len(dSPL))]
+        spl_prime = np.zeros(len(sound_pressure_levels))
         for i in range(0, len(select_sound_pressure_level), 1):
             if not select_sound_pressure_level[i]:
-                spl_prime[i] = dSPL[i]
+                spl_prime[i] = sound_pressure_levels[i]
             else:
                 if 8 < i < 30:
-                    spl_prime[i] = 0.5 * (dSPL[i - 1] + dSPL[i + 1])
-                elif i == 30:
-                    spl_prime[i] = dSPL[i - 1] + slopes[i - 1]
+                    spl_prime[i] = 0.5 * (sound_pressure_levels[i - 1] + sound_pressure_levels[i + 1])
+                # elif i ==30:
+                #     spl_pr ime[i] = sound_pressure_levels[i - 1] + slopes[i - 1]
 
-        #   Step 5 - recompute new slopes
+        if select_sound_pressure_level[-1]:
+            spl_prime[-1] = sound_pressure_levels[-2] + slopes[-2]
 
-        slope_prime = [0.0 for x in range(len(dSPL) + 1)]
-        for i in range(1, len(spl_prime), 1):
-            slope_prime[i] = spl_prime[i] - spl_prime[i - 1]
-        slope_prime[31] = slope_prime[30]
+        #   Step 5 - recompute new slopes
+        slope_prime = np.zeros(len(sound_pressure_levels)+1)
+        slope_prime[1:-1] = np.diff(spl_prime)
+        slope_prime[-1] = slope_prime[-2]
 
         #   Step 6 - compute the arithmetic mean of adjacent three slopes
-
-        mean_slope = [0.0 for i in range(30)]
+        mean_slope = np.zeros((30,))
         for i in range(0, len(mean_slope), 1):
             mean_slope[i] = (1.0 / 3.0) * (slope_prime[i] + slope_prime[i + 1] + slope_prime[i + 2])
 
         # Step 7 - compute the final one-third-octave sound pressure levels
-
-        final_spl = [0.0 for x in range(31)]
-        for i in range(0, len(final_spl), 1):
-            if i < 10:
-                final_spl[i] = dSPL[i]
-            else:
-                final_spl[i] = final_spl[i - 1] + mean_slope[i - 1]
+        final_spl = np.zeros((31,))
+        final_spl[:10] = sound_pressure_levels[:10]
+        for i in range(10, len(final_spl), 1):
+            final_spl[i] = final_spl[i - 1] + mean_slope[i - 1]
 
         #   Step 8 - calculate the differences between the original and final SPL values
-
-        F = [0.0 for x in range(len(dSPL))]
-        for i in range(0, len(F), 1):
-            F[i] = dSPL[i] - final_spl[i]
+        final_sound_pressure_level_difference = np.asarray(sound_pressure_levels) - np.asarray(final_spl)
 
         #   Step 9 - for each of the relevant one-third-octave bands, determine tone correction factors from the sound
         #   pressure level differences (F[i]) and the table in the FAR
-
-        tone_corrections = [0.0 for x in range(len(dSPL))]
-        for i in range(0, len(dSPL), 1):
-            if i < 9:
-                tone_corrections[i] = 0.0
-            elif 9 <= i < 17:
-                if F[i] < 1.5:
-                    tone_corrections[i] = 0.0
-                elif 1.5 <= F[i] < 3:
-                    tone_corrections[i] = 0.5
-                elif 3 <= F[i] < 20:
-                    tone_corrections[i] = F[i] / 6.0
-                elif 20 <= F[i]:
-                    tone_corrections[i] = 3.0 + (1.0 / 3.0)
-            elif 17 <= i <= 27:
-                if F[i] < 1.5:
-                    tone_corrections[i] = 0.0
-                elif 1.5 <= F[i] < 3:
+        tone_corrections = np.zeros(len(sound_pressure_levels))
+        for i in range(0, len(sound_pressure_levels), 1):
+            if 17 <= i <= 27:
+                if 1.5 <= final_sound_pressure_level_difference[i] < 3:
                     tone_corrections[i] = 1
-                elif 3 <= F[i] < 20:
-                    tone_corrections[i] = F[i] / 3
-                elif 20 <= F[i]:
+                elif 3 <= final_sound_pressure_level_difference[i] < 20:
+                    tone_corrections[i] = final_sound_pressure_level_difference[i] / 3
+                elif 20 <= final_sound_pressure_level_difference[i]:
                     tone_corrections[i] = 2 * (3.0 + (1.0 / 3.0))
-            elif i > 27:
-                if F[i] < 1.5:
-                    tone_corrections[i] = 0.0
-                elif 1.5 <= F[i] < 3:
+            else:
+                if 1.5 <= final_sound_pressure_level_difference[i] < 3:
                     tone_corrections[i] = 0.5
-                elif 3 <= F[i] < 20:
-                    tone_corrections[i] = F[i] / 6.0
-                elif 20 <= F[i]:
+                elif 3 <= final_sound_pressure_level_difference[i] < 20:
+                    tone_corrections[i] = final_sound_pressure_level_difference[i] / 6.0
+                elif 20 <= final_sound_pressure_level_difference[i]:
                     tone_corrections[i] = 3.0 + (1.0 / 3.0)
 
         #   Return the maximum of the corrections
-
         return max(tone_corrections)
+
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/spectral/fractional_octave_band.py` & `PyTimbre-0.6.7/src/pytimbre/spectral/fractional_octave_band.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,16 @@
         """
         if isinstance(start_band, int) and isinstance(end_band, int) and isinstance(resolution, int):
             f = []
             for index in range(start_band, end_band + 1):
                 f.append(FractionalOctaveBandTools.center_frequency(resolution, index))
             return f
         else:
-            raise Exception
+            raise ValueError("You must supply integer values for the start and stop bands, and the frequency "
+                             "resolution")
 
     @staticmethod
     def min_audible_field(frequency):
         """
         This function calculates a curve fit to the minimum audible field according to an equation provided
         by NASA in the AUDIB code.  Reference USAAMRDL-TR-74-102A.
 
@@ -288,22 +289,24 @@
 
         returns : double
             the bandwidth of the ERB at the selected center frequency
         """
         return 24.7 * (0.00437 * frequency + 1)
 
     @staticmethod
+    def erb_to_center_frequency(erb):
+        return ((erb / 24.7) - 1) / 0.00437
+
+    @staticmethod
     def get_frequency_array(band_width: int = 3, f0: float = 10, f1: float = 10000):
 
         # Build the collection of frequencies based on the input parameters from the argument list
         accepted_bandwidths = np.array([1, 3, 6, 12, 24], dtype=float)
 
-        if band_width in accepted_bandwidths:
-            pass
-        else:
+        if band_width not in accepted_bandwidths:
             raise ValueError("You did not provide a valid bandwidth")
 
         band0 = int(np.floor(FractionalOctaveBandTools.nearest_band(band_width, f0)))
 
         freqs = list()
 
         f1_upper = f1 * 2 ** (1 / (2 * band_width))
@@ -324,24 +327,24 @@
 
         #   Define the band edges of the frequency band
         b = 2 * bandwidth
         f_low = center_frequency * 2 ** (-1 / b)
         f_high = center_frequency * 2 ** (1 / b)
 
         #   Get the ratio of the bandwidth to the frequency
-        Qr = center_frequency / (f_high - f_low)
-        Qd = (np.pi / b) / (np.sin(np.pi / b)) * Qr
-        Qd = Qd ** 6
+        qr = center_frequency / (f_high - f_low)
+        qd = (np.pi / b) / (np.sin(np.pi / b)) * qr
+        qd = qd ** 6
 
         #   Define the squared weighted shape of the band at these frequencies
         delta_f_psd = narrowband_frequencies / (center_frequency + sys.float_info.epsilon)
         delta_f_fob = center_frequency / (narrowband_frequencies + sys.float_info.epsilon)
         frequency_delta = (delta_f_psd - delta_f_fob) ** 6
 
-        return abs(1 / (1 + Qd * frequency_delta))
+        return abs(1 / (1 + qd * frequency_delta))
 
     @staticmethod
     def ansi_band_limits(class_: int = 0, fc: float = 1000, nth_oct: int = 3):
         """
         This function will calculate the constant percentage bandwidth description of the accepted shape based on the
         ANSI S1.11 standard.
 
@@ -366,15 +369,12 @@
                                   1.05594, 1.08776, 1.12246, 1.29565, 1.88695, 3.06955, 5.43474]) * fc
 
         if class_ == 0:
             lo = np.array([-75, -62, -42.5, -18, -2.3, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, 0.15, -2.3, -18, -42.5, -62,
                            -75])
             hi = np.array([-np.infty, -np.infty, -np.infty, -np.infty, -4.5, -1.1, -.4, -.2, -.15, -.2, -.4, -1.1, -4.5,
                            -np.infty, -np.infty, -np.infty, -np.infty])
-        elif class_ == 1:
-            lo = []
-            hi = []
-        elif class_ == 2:
+        elif class_ >= 1:
             lo = []
             hi = []
 
         return frequency, lo, hi
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/spectral/spectra.py` & `PyTimbre-0.6.7/src/pytimbre/spectral/spectra.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import datetime
 import numpy as np
 import scipy.fft
 import scipy.signal
 from .fractional_octave_band import FractionalOctaveBandTools as fob_tools
 from ..waveform import Waveform
 from .acoustic_weights import AcousticWeights
+from scipy.signal import find_peaks
 
 
 class Spectrum:
     """
     This is the base class that defines the structure of the spectrum object. It does not calculate the frequency
     spectrum from a waveform, but can be used to represent a single spectrum that was previously created.
 
     Remarks
     2022-12-13 - FSM - Added a function to calculate the sound quality metrics based on the frequency spectrum
 
     """
+
     def __init__(self, a: Waveform = None):
         """
         The default constructor that builds the information within the Spectrum class based on the contents of the
         object "a".
 
         Parameters
         ----------
@@ -68,14 +70,24 @@
         self.energy = None
         self.flatness = None
         self.crest = None
         self.probability_distribution = None
         self.integration_variable = None
         self.geometric_mean = None
         self.arithmetic_mean = None
+        self.pitch_threshold = 0.01
+        self.partial_frequencies_indices = None
+        self._fundamental_frequency = None
+        self._harmonic_energy = None
+        self._noise_energy = None
+        self._noisiness = None
+        self._tri_stimulus = None
+        self._harmonic_spectral_deviation = None
+        self._odd_even_ratio = None
+        self._inharmonicity = None
 
     #   ------------------------------------------ Protected functions -------------------------------------------------
 
     def _calculate_spectrum(self):
         import warnings
 
         warnings.warn("This function does nothing. You will need to implement this function in the child class to build"
@@ -118,15 +130,15 @@
     @property
     def time_past_midnight(self):
         if self._time0 is None:
             raise AttributeError("No time has been provided to the Spectrum object.")
 
         if isinstance(self._time0, datetime.datetime):
             return 60 * (60 * self._time0.hour + self._time0.minute) + self._time0.second + \
-                   float(self._time0.microsecond / 1e6)
+                float(self._time0.microsecond / 1e6)
         else:
             return self._time0
 
     @property
     def frequencies(self):
         if self._frequencies is None:
             self._calculate_spectrum()
@@ -167,15 +179,18 @@
         of the A-weighted power spectrum.
         """
 
         return AcousticWeights.la(self.pressures_decibels, self.frequencies)[0]
 
     @property
     def perceived_noise_level(self):
-        return AcousticWeights.pnl(self.pressures_decibels)
+        spl = self.pressures_decibels
+        while len(spl) < 31:
+            spl = np.concatenate([[0], self.pressures_pascals])
+        return AcousticWeights.pnl(spl)
 
     @property
     def fractional_octave_bandwidth(self):
         return self._bandwidth
 
     @fractional_octave_bandwidth.setter
     def fractional_octave_bandwidth(self, value):
@@ -269,30 +284,30 @@
         """
 
         if self.centroid is None:
             if self._acoustic_pressures_pascals is None and self._frequencies is None:
                 self._calculate_spectrum()
 
             if self.probability_distribution is None or self.integration_variable is None:
-                self.calculate_normalized_distribution()
+                self._calculate_normalized_distribution()
 
             self.centroid = np.sum(self.integration_variable * self.probability_distribution, axis=0)
 
         return self.centroid
 
     @property
     def spectral_spread(self):
         """
         Spectral spread or spectral standard-deviation represents the spread of the spectrum around its mean value.
         """
         if self.mean_center is None:
             self._calculate_mean_center()
 
         if self.probability_distribution is None or self.integration_variable is None:
-            self.calculate_normalized_distribution()
+            self._calculate_normalized_distribution()
 
         if self.spread is None:
             self.spread = np.sqrt(np.sum(self.mean_center ** 2 * self.probability_distribution, axis=0))
 
         return self.spread
 
     @property
@@ -302,15 +317,15 @@
         a symmetric distribution, a value < 0 more energy at frequencies lower than the mean value, and values > 0 more
         energy at higher frequencies.
         """
         if self.mean_center is None:
             self._calculate_mean_center()
 
         if self.probability_distribution is None or self.integration_variable is None:
-            self.calculate_normalized_distribution()
+            self._calculate_normalized_distribution()
 
         if self.skewness is None:
             self.skewness = np.sum(self.mean_center ** 3 * self.probability_distribution, axis=0) / \
                             self.spectral_spread ** 3
 
         return self.skewness
 
@@ -321,15 +336,15 @@
         indicate a normal (Gaussian) distribution, values less than 3 indicate a flatter distributions, and values
         greater than 3 indicate a peakier distribution.
         """
         if self.mean_center is None:
             self._calculate_mean_center()
 
         if self.probability_distribution is None or self.integration_variable is None:
-            self.calculate_normalized_distribution()
+            self._calculate_normalized_distribution()
 
         if self.kurtosis is None:
             self.kurtosis = np.sum(self.mean_center ** 4 * self.probability_distribution, axis=0) / \
                             self.spectral_spread ** 4
 
         return self.kurtosis
 
@@ -339,15 +354,15 @@
         Spectral slope is computed using a linear regression over the spectral amplitude values. It should be noted that
         the spectral slope is linearly dependent on the spectral centroid.
         """
         if self._acoustic_pressures_pascals is None and self._frequencies is None:
             self._calculate_spectrum()
 
         if self.probability_distribution is None or self.integration_variable is None:
-            self.calculate_normalized_distribution()
+            self._calculate_normalized_distribution()
 
         if self.slope is None:
             numerator = len(self._frequencies) * (self._frequencies.transpose().dot(self.probability_distribution))
             numerator -= np.sum(self._frequencies) * np.sum(self.probability_distribution, axis=0)
             denominator = len(self._frequencies) * sum(self._frequencies ** 2) - np.sum(self._frequencies) ** 2
             self.slope = numerator / denominator
 
@@ -359,15 +374,15 @@
         Spectral decrease was proposed by Krimphoff (1993) in relation to perceptual studies. It averages the set of
         slopes between frequency f[k] and f[1]. It therefore emphasizes the slopes of the lowest frequencies.
         """
         if self._acoustic_pressures_pascals is None and self._frequencies is None:
             self._calculate_spectrum()
 
         if self.probability_distribution is None or self.integration_variable is None:
-            self.calculate_normalized_distribution()
+            self._calculate_normalized_distribution()
 
         if self.decrease is None:
             numerator = self._acoustic_pressures_pascals[1:] - self._acoustic_pressures_pascals[0]
             denominator = (1 / np.arange(1, len(self._frequencies)))
             self.decrease = (denominator.dot(numerator)).transpose().reshape((-1,))
             self.decrease /= np.sum(self.probability_distribution[1:], axis=0)
 
@@ -382,33 +397,33 @@
         """
         if self._acoustic_pressures_pascals is None and self._frequencies is None:
             self._calculate_spectrum()
 
         if self.roll_off is None:
             threshold = 0.95
             cum_sum = np.cumsum(self._acoustic_pressures_pascals, axis=0)
-            sum = np.ones((len(self.frequencies), )) * (threshold * np.sum(self._acoustic_pressures_pascals))
+            _sum = np.ones((len(self.frequencies),)) * (threshold * np.sum(self._acoustic_pressures_pascals))
 
-            bin = np.cumsum(1 * (cum_sum > sum), axis=0)
-            idx = np.where(bin == 1)[0]
+            _bin = np.cumsum(1 * (cum_sum > _sum), axis=0)
+            idx = np.where(_bin == 1)[0]
 
             self.roll_off = self.frequencies[idx][0]
 
         return self.roll_off
 
     @property
     def spectral_energy(self):
         """
         A summation of the energy within the spectrum
         """
         if self._acoustic_pressures_pascals is None and self._frequencies is None:
             self._calculate_spectrum()
 
         if self.energy is None:
-            self.energy = np.sum(self._acoustic_pressures_pascals, axis=0)
+            self.energy = np.sum(self._acoustic_pressures_pascals ** 2, axis=0)
 
         return self.energy
 
     @property
     def spectral_flatness(self):
         """
         Spectral flatness is obtained by comparing the geometrical mean and the arithmetical mean of the spectrum. The
@@ -417,15 +432,16 @@
         tonal signals, the spectral flatness is close to 0( a peaky spectrum), whereas for noisy signals it is close to
         1 (flat spectrum).
         """
         if self._acoustic_pressures_pascals is None and self._frequencies is None:
             self._calculate_spectrum()
 
         if self.flatness is None:
-            self.geometric_mean = np.exp((1 / len(self._frequencies)) * np.sum(np.log(self._acoustic_pressures_pascals), axis=0))
+            self.geometric_mean = np.exp((1 / len(self._frequencies)) * np.sum(np.log(self._acoustic_pressures_pascals),
+                                                                               axis=0))
             self.arithmetic_mean = np.mean(self._acoustic_pressures_pascals, axis=0)
             self.flatness = self.geometric_mean / self.arithmetic_mean
 
         return self.flatness
 
     @property
     def spectral_crest(self):
@@ -446,14 +462,174 @@
     @property
     def mean_center(self):
         if self._mean_center is None:
             self._calculate_mean_center()
 
         return self._mean_center
 
+    @property
+    def harmonic_energy(self):
+        """
+        This is the energy within the signal that is explained by the harmonic partial frequencies and amplitudes. It
+        is the square of all the amplitudes determined for the harmonic frequencies.
+        """
+
+        if self.partial_frequencies_indices is None:
+            if self.fundamental_frequency is None:
+                self._calculate_fundamental_frequency()
+            self._calculate_partial_pressures()
+
+        if self._harmonic_energy is not None:
+            return self._harmonic_energy
+
+        self._harmonic_energy = 0
+
+        for idx in self.partial_frequencies_indices:
+            self._harmonic_energy += self.pressures_pascals[idx] ** 2
+
+        return self._harmonic_energy
+
+    @property
+    def noise_energy(self):
+        """
+        This is the energy of the signal not represented by the harmonic frequencies. It is simply the difference
+        between the total energy and the energy explained by the harmonics.
+        """
+        if self.partial_frequencies_indices is None:
+            if self.fundamental_frequency is None:
+                self._calculate_fundamental_frequency()
+            self._calculate_partial_pressures()
+
+        if self._noise_energy is not None:
+            return self._noise_energy
+
+        self._noise_energy = self.spectral_energy - self.harmonic_energy
+
+        return self._noise_energy
+
+    @property
+    def noisiness(self):
+        """
+        This is the ratio of the noise energy to the total energy. The higher the noisiness, the more noise-like the
+        signal must be.
+        """
+        if self.partial_frequencies_indices is None:
+            if self.fundamental_frequency is None:
+                self._calculate_fundamental_frequency()
+            self._calculate_partial_pressures()
+
+        if self._noisiness is not None:
+            return self._noisiness
+
+        self._noisiness = self.noise_energy / self.spectral_energy
+
+        return self._noisiness
+
+    @property
+    def tri_stimulus(self):
+        """
+        This is a set of values that were first introduced by H. Pollard (Pollard, H. and Jansson, E. (1982) "A
+        tristimulus method for the specification of musical timbre," Acustica 51, 162-171) as a timbral equivalent to
+        visual color attributes. It is three different energy ratios based on the description of the fundamental
+        frequency.
+        """
+        if self._tri_stimulus is None:
+            if self.partial_frequencies_indices is None:
+                if self.fundamental_frequency is None:
+                    self._calculate_fundamental_frequency()
+                self._calculate_partial_pressures()
+
+            harmonic_pressure_sum = np.sum(self.pressures_pascals[self.partial_frequencies_indices])
+            t01 = self.pressures_pascals[self.partial_frequencies_indices[0]] / harmonic_pressure_sum
+
+            t02 = np.sum(self.pressures_pascals[self.partial_frequencies_indices[1:4]]) / harmonic_pressure_sum
+            t03 = np.sum(self.pressures_pascals[self.partial_frequencies_indices[4:]]) / harmonic_pressure_sum
+
+            self._tri_stimulus = [t01, t02, t03]
+
+        return self._tri_stimulus
+
+    @property
+    def harmonic_spectral_deviation(self):
+        """
+        This measures the deviation of the amplitudes of the partials from the harmonics from the global or smoothed
+        spectral envelope.
+        """
+        if self._harmonic_spectral_deviation is None:
+            if self.partial_frequencies_indices is None:
+                if self.fundamental_frequency is None:
+                    self._calculate_fundamental_frequency()
+                self._calculate_partial_pressures()
+
+            self._harmonic_spectral_deviation = 0
+            for h in range(1, len(self.partial_frequencies_indices) - 1):
+                self._harmonic_spectral_deviation += self.pressures_pascals[self.partial_frequencies_indices[h]] - (
+                        self.pressures_pascals[self.partial_frequencies_indices[h - 1]] +
+                        self.pressures_pascals[self.partial_frequencies_indices[h]] +
+                        self.pressures_pascals[self.partial_frequencies_indices[h + 1]]
+                ) / 3
+
+            self._harmonic_spectral_deviation /= len(self.partial_frequencies_indices)
+
+        return self._harmonic_spectral_deviation
+
+    @property
+    def odd_even_ratio(self):
+        """
+        In musical instruments, certain signals contain mostly even (trumpet) or odd (clarinet) harmonics. This ratio
+        determines where the system is mostly odd or even.
+        """
+        if self._odd_even_ratio is None:
+            if self.partial_frequencies_indices is None:
+                if self.fundamental_frequency is None:
+                    self._calculate_fundamental_frequency()
+                self._calculate_partial_pressures()
+
+            odd_energy = 0
+            even_energy = 0
+            for i in range(1, len(self.partial_frequencies_indices)):
+                if (i + 1) % 2 == 0:
+                    even_energy += self.pressures_pascals[self.partial_frequencies_indices[i]] ** 2
+                else:
+                    odd_energy += self.pressures_pascals[self.partial_frequencies_indices[i]] ** 2
+
+            self._odd_even_ratio = odd_energy / even_energy
+
+        return self._odd_even_ratio
+
+    @property
+    def inharmonicity(self):
+        """
+        This is a measure of the deviation of the partial frequencies from the purely harmonic frequency.
+        """
+        if self._inharmonicity is None:
+            if self.partial_frequencies_indices is None:
+                if self.fundamental_frequency is None:
+                    self._calculate_fundamental_frequency()
+                self._calculate_partial_pressures()
+
+            f0 = self.fundamental_frequency
+
+            frequency_departure = 0
+            for i in range(1, len(self.partial_frequencies_indices)):
+                frequency_departure += (self.frequencies[self.partial_frequencies_indices[i]] - (i + 1) * f0) * \
+                                       self.pressures_pascals[self.partial_frequencies_indices[i]]
+
+            self._inharmonicity = (2 / f0) * frequency_departure / np.sum(self.pressures_pascals[
+                                                                              self.partial_frequencies_indices] ** 2)
+
+        return self._inharmonicity
+
+    @property
+    def fundamental_frequency(self):
+        if self._fundamental_frequency is None:
+            self._calculate_fundamental_frequency()
+
+        return self._fundamental_frequency
+
     def calculate_engineering_unit_scale_factor(self, calibration_level: float = 94, calibration_frequency=1000):
         """
         This will take the data within the class and build the spectral time history and then determine the value of the
         scale factor to get a specific sound pressure level at a certain frequency.
 
         Parameters
         ----------
@@ -467,19 +643,18 @@
 
         if self.fractional_octave_bandwidth is None:
             raise ValueError("This analysis cannot be accomplished on a narrowband spectrum")
 
         #   Now determine the index of the band within the spectral time history that should be examined for the
         #   calculation of the engineering scaling units.
 
-        # idx = int(np.floor(fob_tools.nearest_band(3, calibration_frequency))) - 10
         idx = np.argmin(np.abs(self.frequencies - calibration_frequency))
 
-        # #   Now this may select the nearest band as the band just above the actual band.  So ensure that the lower band
-        # #   is below the desired center frequency
+        #   Now this may select the nearest band as the band just above the actual band.  So ensure that the lower band
+        #   is below the desired center frequency
         #
         # if fob_tools.lower_frequency(3, idx + 10) > calibration_frequency:
         #     idx -= 1
 
         #   From the spectrum obtain the values of the frequency
 
         calibration_values = self.pressures_decibels[idx]
@@ -489,72 +664,282 @@
         sens = calibration_level - calibration_values
         sens /= 20
         sens *= -1
         sens = 10.0 ** sens
 
         return sens
 
-    def get_average_features(self, include_sq_metrics: bool = True):
-        import numpy as np
+    def get_average_features(self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
+                             include_spectral_features: bool = True, include_harmonic_features: bool = True):
         """
         This will return a dict of the various elements within the spectrum and waveform (if it was used to create the
         spectrogram object) with any time variant elements averaged.
         """
 
+        #   Create the dictionary that will hold the data
         features = dict()
 
-        if self.waveform is not None:
+        #   If there is a waveform inside the Spectrum object, and we desire the temporal statistics
+        if self.waveform is not None and include_temporal_features:
             features = self.waveform.get_features(include_sq_metrics)
             features['zero_crossing_rate'] = np.mean(features['zero crossing rate'])
             auto_correlation_coefficients = np.mean(features['auto-correlation'], axis=0)
+
             if include_sq_metrics:
                 features['loudness'] = np.mean(features['loudness'])
                 features['sharpness'] = np.mean(features['sharpness'])
                 features['roughness'] = np.mean(features['roughness'])
 
             for i in range(12):
                 features['auto_correlation_{:02.0f}'.format(i)] = auto_correlation_coefficients[i]
 
             del features['zero crossing rate']
             del features['auto-correlation']
 
-        features['spectral_centroid'] = np.mean(self.spectral_centroid)
-        features['spectral_spread'] = np.mean(self.spectral_spread)
-        features['spectral_skewness'] = np.mean(self.spectral_skewness)
-        features['spectral_kurtosis'] = np.mean(self.spectral_kurtosis)
-        features['spectral_slope'] = np.mean(self.spectral_slope)
-        features['spectral_decrease'] = np.mean(self.spectral_decrease)
-        features['spectral_roll_off'] = np.mean(self.spectral_roll_off)
-        features['spectral_energy'] = np.mean(self.spectral_energy)
-        features['spectral_flatness'] = np.mean(self.spectral_flatness)
-        features['spectral_crest'] = np.mean(self.spectral_crest)
+        #   If we desire the spectral statistics
+        if include_spectral_features:
+            features['spectral_centroid'] = np.mean(self.spectral_centroid)
+            features['spectral_spread'] = np.mean(self.spectral_spread)
+            features['spectral_skewness'] = np.mean(self.spectral_skewness)
+            features['spectral_kurtosis'] = np.mean(self.spectral_kurtosis)
+            features['spectral_slope'] = np.mean(self.spectral_slope)
+            features['spectral_decrease'] = np.mean(self.spectral_decrease)
+            features['spectral_roll_off'] = np.mean(self.spectral_roll_off)
+            features['spectral_energy'] = np.mean(self.spectral_energy)
+            features['spectral_flatness'] = np.mean(self.spectral_flatness)
+            features['spectral_crest'] = np.mean(self.spectral_crest)
+
+        if include_harmonic_features:
+            features['fundamental_frequency'] = np.mean(self.fundamental_frequency)
+            features['harmonic_energy'] = self.harmonic_energy
+            features['noise_energy'] = self.noise_energy
+            features['noisiness'] = self.noisiness
+            features['tri_stimulus_01'] = self.tri_stimulus[0]
+            features['tri_stimulus_02'] = self.tri_stimulus[1]
+            features['tri_stimulus_03'] = self.tri_stimulus[2]
+            features['harmonic_spectral_deviation'] = self.harmonic_spectral_deviation
+            features['odd_even_ratio'] = self.odd_even_ratio
+            features['inharmonicity'] = self.inharmonicity
 
         return features
 
-    def calculate_normalized_distribution(self):
+    def get_feature_names(self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
+                          include_spectral_features: bool = True, include_harmonic_features: bool = True):
+        return self.get_average_features(include_sq_metrics=include_sq_metrics,
+                                         include_harmonic_features=include_harmonic_features,
+                                         include_spectral_features=include_spectral_features,
+                                         include_temporal_features=include_temporal_features).keys()
+
+    def _calculate_normalized_distribution(self):
         if self._acoustic_pressures_pascals is None:
             self._calculate_spectrum()
 
         self.probability_distribution = self._acoustic_pressures_pascals
         self.probability_distribution /= np.sum(self._acoustic_pressures_pascals, axis=0)
 
         self.integration_variable = self.frequencies
 
     def _calculate_mean_center(self):
         if self._acoustic_pressures_pascals is None:
             self._calculate_spectrum()
 
         if self.probability_distribution is None or self.integration_variable is None:
-            self.calculate_normalized_distribution()
+            self._calculate_normalized_distribution()
 
         if self._mean_center is None:
             self._mean_center = self.integration_variable - self.spectral_centroid
 
         return self._mean_center
 
+    def _calculate_fundamental_frequency(self):
+        from .fundamental_frequency import FundamentalFrequencyCalculator
+
+        calculator = FundamentalFrequencyCalculator(frequency_window_size=self._fft_size)
+
+        f0 = list()
+        f0.append(calculator.fundamental_swipe(self))
+        f0.append(calculator.fundamental_by_peaks(self))
+        if self._waveform is not None:
+            f0.append(calculator.fundamental_by_time(self.waveform))
+
+        self._fundamental_frequency = np.median(np.asarray(f0))
+
+    def _calculate_partial_pressures(self):
+        """
+        We need to locate the partial pressure frequencies and amplitudes by calculating the index of each integer
+        multiple of the fundamental frequency.
+        """
+
+        #   Determine the ratio of the frequencies to the fundamental frequencies. We want to keep only the values
+        #   that are close to a whole integer multiple.
+        f_ratio = self.frequencies / self.fundamental_frequency
+
+        #   Using the last ratio, determine the maximum number of partial pressure that might exist within this spectrum
+        max_partial_frequencies = int(np.floor(f_ratio[-1]))
+        self.partial_frequencies_indices = np.zeros((max_partial_frequencies,), dtype=int)
+
+        for i in range(0, max_partial_frequencies):
+            self.partial_frequencies_indices[i] = np.where(f_ratio >= i + 1)[0][0]
+
+    def _calculate_harmonic_features(self):
+        from ..yin import yin
+        # self.stft = STFT.STFT(sound, self.config)
+        # self.t_support = self.stft.t_support
+        # maxSwipepWinSize = self.stft.hop_size * np.ceil(
+        #     2 ** (round(np.log2(8 * self.sound.reps['AudioSignal'].sampleRate / 50)) - 1) / self.stft.hop_size)
+        # freqCorrs = np.linspace(-5, 5, 101)
+        # nFreqCorrs = len(freqCorrs)
+        # inharmCoeffs = np.linspace(0, 0.001, 21)
+        # nInharmCoeffs = 21
+        # tSupport = np.subtract(self.t_support, self.t_support[0])
+        # tSize = len(tSupport)
+        # distr = self.stft.value
+        # signalChunk = a.value
+        # pitchLims = np.array([50, 500])
+        # estimated_pitches, estimated_times, estStrengths = self.swipep(signalChunk, self.sound.reps['AudioSignal'].sampleRate,
+        #                                                  pitchLims, (self.stft.hop_size / self.sound.reps[
+        #         'AudioSignal'].sampleRate), 1 / 48, 0.1, 0.2, -np.inf)
+
+        estimated_pitches, estimated_times, estimated_pitch_strengths = yin(
+            self.waveform.samples,
+            self.waveform.sample_rate,
+            F_max=10000,
+            F_min=10,
+            N=int(np.floor(self.sample_rate / 10)),
+            H=int(np.floor(self.sample_rate / 10 / 4)))
+
+        try:
+            current_maximum = np.nanmax(estimated_pitch_strengths)
+        except ValueError:
+            current_maximum = np.max(estimated_pitch_strengths)
+        nans = np.isnan(estimated_pitches)
+        anyy = any(nans)
+        if anyy:
+            estimated_pitches[np.isnan(estimated_pitches)] = np.median(
+                estimated_pitches[not np.isnan(estimated_pitches)])
+        fundamental_frequencies = None
+        if current_maximum > self.pitch_threshold:
+            estimated_time_pitch_pairs = np.zeros((len(estimated_times), 2))
+            estimated_time_pitch_pairs[:, 0] = estimated_times
+            estimated_time_pitch_pairs[:, 1] = estimated_pitches
+            fundamental_frequencies = Harmonic.Fevalbp(estimated_time_pitch_pairs, tSupport)
+            fundamental_frequencies = np.transpose(fundamental_frequencies)
+        else:
+            logging.warning('Sound deemed not harmonic. Setting f0 estimate to 0.')
+            self.partialFreqs = np.zeros((self.config['n_harms'], tSize))
+            self.partialAmps = np.zeros((self.config['n_harms'], tSize))
+            self.fundamentalFreqs = np.zeros((1, tSize))
+            return
+        a = np.empty((len(fundamental_frequencies), nFreqCorrs))
+        for column in range(np.shape(a)[1]):
+            a[:, column] = fundamental_frequencies
+        b = np.empty((tSize, len(freqCorrs)))
+        for row in range(np.shape(b)[0]):
+            b[row, :] = freqCorrs
+        corrFreqsTF = np.add(a, b)
+
+        a = np.empty((self.config['n_harms'], nInharmCoeffs))
+        for column in range(np.shape(a)[1]):
+            a[:, column] = [*range(1, self.config['n_harms'] + 1)]
+        b = np.power([*range(1, self.config['n_harms'] + 1)], 2)
+        b1 = b[:, None]
+        b2 = inharmCoeffs[None, :]
+        c = np.matmul(b1, b2)
+        d = np.add(1, c)
+        inharmFactorsHI = np.multiply(a, np.sqrt(d))
+        shape1 = np.reshape(corrFreqsTF, (tSize * nFreqCorrs, 1), order='F')
+        shape2 = np.reshape(inharmFactorsHI, (1, self.config['n_harms'] * nInharmCoeffs), order='F')
+        shape3 = np.reshape(np.multiply(shape1, shape2), (tSize, nFreqCorrs, self.config['n_harms'], nInharmCoeffs),
+                            order='F')
+        shape4 = np.divide(1, self.stft.bin_size)
+        shape5 = np.multiply(shape4, shape3)
+        shape6 = np.round(shape5)
+        fSupIdcsTFHI = np.add(1, shape6)
+        fSupIdcsTFHI[fSupIdcsTFHI > self.stft.f_size] = self.stft.f_size
+
+        a = np.array([*range(0, tSize)])
+        a2 = a[:, None, None, None]
+        b = np.tile(a2, (1, nFreqCorrs, self.config['n_harms'], nInharmCoeffs))
+        c = np.multiply(self.stft.f_size, b)
+        d = np.add(fSupIdcsTFHI, c)
+        e = d.astype(int)
+        distrIdcsTFHI = np.subtract(e, 1)
+        shape = np.shape(distrIdcsTFHI)
+
+        _0 = distr.flatten('F')
+        _1 = distrIdcsTFHI.flatten('F')
+        _2 = np.take(_0, _1)
+
+        a = np.reshape(_2, shape, order='F')
+        totalErgTFI = np.sum(a, axis=2)
+
+        scoreTI = np.max(totalErgTFI, 1)
+        inharmCoeffIdcsT = np.argmax(scoreTI, 1)
+        maxScoreTI = np.array([scoreTI[i, inharmCoeffIdcsT[i]] for i in range(len(inharmCoeffIdcsT))])
+        a = np.subtract(maxScoreTI, scoreTI[:, 0])
+        b = np.divide(a, scoreTI[:, 0])
+        c = b <= 0.01
+        inharmCoeffIdcsT[c] = 0
+        tile1 = np.add([*range(1, tSize + 1)], np.multiply(tSize * nFreqCorrs, inharmCoeffIdcsT))
+        repmat1 = np.tile(tile1, (nFreqCorrs, 1)).transpose()
+        tile2 = [tSize * (x) for x in range(nFreqCorrs)]
+        repmat2 = np.tile(tile2, (tSize, 1))
+        colIdcs = np.reshape(np.add(repmat1, repmat2), (tSize * nFreqCorrs, 1), order='F')
+        totalErgTFI_flat = totalErgTFI.flatten('F')
+        totalErgTF = np.take(totalErgTFI_flat, np.subtract(colIdcs, 1))
+        totalErgTF = np.reshape(totalErgTF, (tSize, nFreqCorrs), order='F')
+
+        reshape1 = np.reshape(
+            np.add([*range(1, tSize + 1)], np.multiply(tSize * nFreqCorrs * self.config['n_harms'], inharmCoeffIdcsT)),
+            (tSize, 1, 1), order='F')
+        repmat1 = np.tile(reshape1, (1, nFreqCorrs, self.config['n_harms']))
+        reshape2 = np.reshape([*range(1, nFreqCorrs + 1)], (1, nFreqCorrs, 1), order='F')
+        repmat2 = np.tile(reshape2, (tSize, 1, self.config['n_harms']))
+        reshape3 = np.reshape([*range(1, self.config['n_harms'] + 1)], (1, 1, self.config['n_harms']), order='F')
+        repmat3 = np.tile(reshape3, (tSize, nFreqCorrs, 1))
+
+        a = np.subtract(repmat3, 1)
+        b = np.multiply(nFreqCorrs, a)
+        c = np.subtract(np.add(repmat2, b), 1)  # ???? Switch
+        d = np.multiply(tSize, c)
+        e = np.add(repmat1, d)
+        colIdcs = np.reshape(e, (tSize * nFreqCorrs * self.config['n_harms'], 1), order='F')
+        fSupIdcsTFHI_flat = fSupIdcsTFHI.flatten('F')
+        fSupIdcsHTF = np.take(fSupIdcsTFHI_flat, np.subtract(colIdcs, 1))
+        fSupIdcsHTF = np.reshape(fSupIdcsHTF, (tSize, nFreqCorrs, self.config['n_harms']), order='F')
+        fSupIdcsHTF = np.transpose(fSupIdcsHTF, [2, 0, 1])
+        freqCorrIdcsT = np.argmax(totalErgTF, 1)
+
+        repmat1 = np.tile([*range(1, self.config['n_harms'] + 1)], (tSize, 1)).transpose()
+        a = freqCorrIdcsT
+        b = np.multiply(tSize, a)
+        c = np.subtract(np.add([*range(1, tSize + 1)], b), 1)
+        d = np.multiply(self.config['n_harms'], c)
+        repmat2 = np.tile(d, (self.config['n_harms'], 1))
+        colIdcs = np.reshape(np.add(repmat1, repmat2), (self.config['n_harms'] * tSize, 1), order='F')
+
+        fSupIdcsHTF_flat = fSupIdcsHTF.flatten('F')
+        fSup = np.take(fSupIdcsHTF_flat, np.subtract(colIdcs, 1)).astype(int)
+        partialFreqs = np.take(self.stft.f_support, np.subtract(fSup, 1))
+        partialFreqs = np.reshape(partialFreqs, (self.config['n_harms'], tSize), order='F')
+
+        repmat1 = np.tile([*range(0, tSize)], (self.config['n_harms'], 1))
+        reshape1 = np.reshape(repmat1, (self.config['n_harms'] * tSize, 1), order='F')
+        aa = fSup
+        bb = np.multiply(self.stft.f_size, reshape1)
+        cc = np.add(aa, bb)
+        distr_flat = distr.flatten('F')
+        partialAmps = np.take(distr_flat, np.subtract(cc, 1))
+        partialAmps = np.reshape(partialAmps, (self.config['n_harms'], tSize), order='F')
+        aaa = np.concatenate((partialFreqs, partialAmps))
+        self.fundamentalFreqs = aaa[0, :]
+        self.partialFreqs = aaa[:self.config['n_harms'], :]
+        self.partialAmps = aaa[self.config['n_harms']:(2 * self.config['n_harms']), :]
+        self.value = aaa
+
 
 class SpectrumByFFT(Spectrum):
     """
     This class is a specialization of the spectrum class that implements the way to define the spectrum. This is
     accomplished with the Fourier Transform, using a chunked overlapping representation of the data within the
     calculation.
 
@@ -739,15 +1124,14 @@
         s.fractional_octave_bandwidth = bandwidth
         s._time0 = self.time
 
         return s
 
 
 class SpectrumByDigitalFilters(Spectrum):
-
     """
     This class differs from the previous classes in that the determination of the spectrum is accomplished through an
     application of digital filters. A set of filters describing the collection of filters at the highest desired full
     octave band will be constructed. These coefficients will be applied as the signal is recursively down sampled at
     half the sample rate. The minimum number of elements required to generate the filtered data require three times
     the number of coefficients, doubled until we reach the maximum sample rate of the system.
 
@@ -900,9 +1284,7 @@
                                                                   self.start_fractional_octave_frequency)))[0][0]
         idx1 = np.where(frequency < fob_tools.upper_frequency(self.fractional_octave_bandwidth,
                                                               fob_tools.nearest_band(
                                                                   self.fractional_octave_bandwidth,
                                                                   self.stop_fractional_octave_frequency)))[0][-1]
         self._frequencies = frequency[np.arange(idx0, idx1 + 1)]
         self._acoustic_pressures_pascals = pressures[np.arange(idx0, idx1 + 1)]
-
-
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/spectral/spectrogram.py` & `PyTimbre-0.6.7/src/pytimbre/spectral/spectrogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         last_index = np.floor((len(self.signal) -
                                (right_hand_window_size + 1)) / self._hop_size) * self._hop_size + 1
 
         #   Define some support vectors
         index = np.arange(0, last_index, self._hop_size, dtype=int) - left_hand_window_size
         size_x = len(index)
         size_y = self.fft_size / 2
-        self._times = np.arange(0, size_x) / (self.sample_rate / self._hop_size)
+        self._times = np.arange(0, size_x) / (self.waveform_sample_rate / self._hop_size)
         normalized_frequency = np.arange(0, size_y) / size_y / 2
 
         #   Create the windowed signal
         window = np.hamming(int(self._window_size + 1))
         distribution_pts = np.zeros((self.fft_size, size_x), dtype='complex')
         for i in range(size_x):
             rng = np.arange(0, int(self._window_size + 1), dtype=int) + (index[i] + left_hand_window_size)
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/spectral/time_histories.py` & `PyTimbre-0.6.7/src/pytimbre/spectral/time_histories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 import abc
 from enum import Enum
 import pandas as pd
-
-from .spectra import Spectrum, SpectrumByDigitalFilters, SpectrumByFFT, Waveform
-from .acoustic_weights import AcousticWeights
-from ..audio_files.wavefile import WaveFile
 import numpy as np
 import warnings
 import datetime
 
-
-class LeqDurationMode(Enum):
-    """
-    The available types of time scaling for conversion of a signal to equivalent levels
-    """
-
-    steady_state = 0
-    transient = 1
+from ..waveform import Waveform, LeqDurationMode
+from .spectra import Spectrum, SpectrumByDigitalFilters, SpectrumByFFT
+from .acoustic_weights import AcousticWeights
+from ..audio_files.wavefile import WaveFile
 
 
-class weighting_function(Enum):
+class WeightingFunction(Enum):
     """
     This class provides the options on how to weight the calculation of the overall level values
     """
 
     unweighted = 0
     a_weighted = 1
     c_weighted = 2
@@ -73,14 +65,143 @@
 
     @abc.abstractmethod
     def _calculate_spectrogram(self):
         warnings.warn("This function must be implemented in any child class to create the collection of spectra objects"
                       " that define the time history")
         pass
 
+    def equivalent_level(self,
+                         weighting: WeightingFunction = WeightingFunction.a_weighted,
+                         equivalent_duration: float = 8 * 3600,
+                         start_sample: int = 0,
+                         stop_sample: int = None,
+                         leq_mode: LeqDurationMode = None,
+                         exposure_duration: float = None):
+        """
+        This function computes the equivalent level on the spectral time history. If there is a weighting
+        function specified this is applied to the spectra. Additionally, the duration of the summation
+        is specified (in seconds) for the new value with a default of 8 hours. Finally, if there is a cause to exclude
+        portions of the data (i.e. calculating the SEL for the 10 dB down points in community noise) you can specify
+        the start and stop index. If the stop index is None, then the last pressure defines the limit of the summation.
+
+        Parameters
+        ----------
+        weighting   :   WeightingFunction
+            The enumeration to determine filtering function applied to the waveform
+        equivalent_duration :   float
+            The denominator of the summation - in seconds - representing the desired length of total exposure
+            time (e.g. an 8-hour duty day, or a 1-second sound exposure level)
+        start_sample    :   int
+            default = 0. The start sample of the pressure summation
+        stop_sample :   int
+            default = None. The stop sample, if the value is None, then it is replaces with the last sample index
+        leq_mode    :   LeqDurationMode
+            The enumeration to determine whether the input signal contains all energy
+            of an exposure to the listener (transient) or the signal represents a sample of a longer-duration
+            (steady_state) exposure
+        exposure_duration   :   float
+            If leq_mode is steady_state, this is the actual time of noise exposure to the
+            listener in seconds
+
+        """
+
+        if stop_sample is None:
+            stop_sample = len(self.times)
+
+        number_of_samples = stop_sample - start_sample
+        signal_duration = number_of_samples * np.mean(np.diff(self.times))
+
+        weights = []
+        if weighting == WeightingFunction.unweighted:
+            weights = np.zeros(np.size(self.frequencies))
+        elif weighting == WeightingFunction.a_weighted:
+            weights = AcousticWeights.aw(self.frequencies)
+        elif weighting == WeightingFunction.c_weighted:
+            weights = AcousticWeights.cw(self.frequencies)
+
+        spectrogram_array_decibels_weighted = self.spectrogram_array_decibels + \
+                                              np.tile(weights, (len(self.times), 1))
+
+        spectrogram_array_pascals_weighted = 10 ** (spectrogram_array_decibels_weighted / 20) * 20e-6
+
+        s = np.sum(np.sum(spectrogram_array_pascals_weighted[start_sample:stop_sample, :] ** 2))
+
+        total_energy_in_signal = s / self.time_history_sample_rate
+
+        total_energy_of_exposure = []
+        if leq_mode == LeqDurationMode.transient:
+            total_energy_of_exposure = total_energy_in_signal
+        elif leq_mode == LeqDurationMode.steady_state:
+            if exposure_duration is None:
+                exposure_duration = signal_duration
+            total_energy_of_exposure = total_energy_in_signal * (exposure_duration / signal_duration)
+        elif leq_mode is None:
+            raise ValueError("User must specify a signal duration mode of class LeqDurationMode.")
+
+        average_energy_over_equivalent_duration = total_energy_of_exposure / equivalent_duration
+
+        return 10.0 * np.log10(average_energy_over_equivalent_duration / 20e-6 / 20e-6)
+
+    def get_features(self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
+                     include_spectral_features: bool = True, include_harmonic_features: bool = True):
+        """
+        This function will obtain the temporal, spectral, sound quality, and level metrics from the waveform and the
+        spectra within the time history.
+
+        Parameters
+        :param include_harmonic_features: bool
+            Flag to determine whether to include the harmonic features in the output
+        :param include_spectral_features: bool
+            Flag to determine whether to include the spectral features in the output
+        :param include_temporal_features: bool
+            Flag to determine whether to include the temporal features in the output
+        :param include_sq_metrics: bool
+            Flag to determine whether to include the sound quality features in the output
+        Returns
+        -------
+        A Pandas.DataFrame with the information from each spectrum
+        """
+
+        #   Create the DataFrame that will hold the data from the waveform and the spectrum objects
+        names = ['time', 'lf', 'la', 'pnl']
+        for f in self.frequencies:
+            names.append('F{:06.0f}Hz'.format(f))
+
+        for key in self.spectra[0].get_feature_names(include_sq_metrics=include_sq_metrics,
+                                                     include_harmonic_features=include_harmonic_features,
+                                                     include_spectral_features=include_spectral_features,
+                                                     include_temporal_features=include_temporal_features):
+            names.append(key)
+
+        df = pd.DataFrame(columns=names, index=np.arange(len(self.times)))
+
+        for i in range(df.shape[0]):
+            s = self.spectra[i]
+            if isinstance(s, Spectrum):
+                df.iloc[i, :4] = [s.time_past_midnight, s.overall_level, s.overall_a_weighted_level,
+                                  s.perceived_noise_level]
+
+                for band_index in range(len(self.frequencies)):
+                    df.iloc[i, 4 + band_index] = s.pressures_decibels[band_index]
+
+                n = 4 + len(self.frequencies)
+
+                for key in s.get_feature_names(include_sq_metrics=include_sq_metrics,
+                                               include_harmonic_features=include_harmonic_features,
+                                               include_spectral_features=include_spectral_features,
+                                               include_temporal_features=include_temporal_features):
+                    df.iloc[i, n] = s.get_average_features(include_sq_metrics=include_sq_metrics,
+                                                           include_harmonic_features=include_harmonic_features,
+                                                           include_spectral_features=include_spectral_features,
+                                                           include_temporal_features=include_temporal_features)[key]
+
+                    n += 1
+
+        return df
+
     def save(self, filename: str):
         from ..audio_files.ansi_standard_formatted_files import StandardBinaryFile
         import datetime
         """
         This function saves the data from the waveform's header and the spectral information to a file 
 
         Parameters:
@@ -259,15 +380,19 @@
         return self._waveform
 
     @property
     def signal(self):
         return self.waveform.samples
 
     @property
-    def sample_rate(self):
+    def waveform_sample_rate(self):
+        return self.waveform.sample_rate
+
+    @property
+    def time_history_sample_rate(self):
         """
         The number of samples per second of evey TimeHistory metric.
         """
         return 1 / self._integration_time
 
     @property
     def integration_time(self):
@@ -298,15 +423,15 @@
                     t[i] = self.spectra[i].time_past_midnight
 
             self._times = t
 
         return self._times
 
     @property
-    def sample_size(self):
+    def waveform_sample_size(self):
         return int(np.floor(self.integration_time * self._waveform.sample_rate))
 
     @property
     def frequencies(self):
         if self._spectra is None:
             self._calculate_spectrogram()
 
@@ -354,86 +479,14 @@
         levels = np.zeros((len(self.times)), )
 
         for i in range(len(self.spectra)):
             levels[i] = self.spectra[i].overall_a_weighted_level
 
         return levels
 
-    def equivalent_level(self,
-                         weighting: weighting_function = weighting_function.a_weighted,
-                         equivalent_duration: float = 8 * 3600,
-                         start_sample: int = 0,
-                         stop_sample: int = None,
-                         leq_mode: LeqDurationMode = None,
-                         exposure_duration: float = None):
-        """
-        This function computes the equivalent level on the spectral time history. If there is a weighting
-        function specified this is applied to the spectra. Additionally, the duration of the summation
-        is specified (in seconds) for the new value with a default of 8 hours. Finally, if there is a cause to exclude
-        portions of the data (i.e. calculating the SEL for the 10 dB down points in community noise) you can specify
-        the start and stop index. If the stop index is None, then the last pressure defines the limit of the summation.
-
-        Parameters
-        ----------
-        weighting   :   weighting_function
-            The enumeration to determine filtering function applied to the waveform
-        equivalent_duration :   float
-            The denominator of the summation - in seconds - representing the desired length of total exposure
-            time (e.g. an 8-hour duty day, or a 1-second sound exposure level)
-        start_sample    :   int
-            default = 0. The start sample of the pressure summation
-        stop_sample :   int
-            default = None. The stop sample, if the value is None, then it is replaces with the last sample index
-        leq_mode    :   LeqDurationMode
-            The enumeration to determine whether the input signal contains all energy
-            of an exposure to the listener (transient) or the signal represents a sample of a longer-duration
-            (steady_state) exposure
-        exposure_duration   :   float
-            If leq_mode is steady_state, this is the actual time of noise exposure to the
-            listener in seconds
-
-        """
-
-        if stop_sample is None:
-            stop_sample = len(self.times)
-
-        number_of_samples = stop_sample - start_sample
-        signal_duration = number_of_samples * np.mean(np.diff(self.times))
-
-        weights=[]
-        if weighting == weighting_function.unweighted:
-            weights = np.zeros(np.size(self.frequencies))
-        elif weighting == weighting_function.a_weighted:
-            weights = AcousticWeights.aw(self.frequencies)
-        elif weighting == weighting_function.c_weighted:
-            weights = AcousticWeights.cw(self.frequencies)
-
-        spectrogram_array_decibels_weighted = self.spectrogram_array_decibels + \
-                                              np.tile(weights, (len(self.times), 1))
-
-        spectrogram_array_pascals_weighted = 10 ** (spectrogram_array_decibels_weighted / 20) * 20e-6
-
-        s = np.sum(np.sum(spectrogram_array_pascals_weighted[start_sample:stop_sample, :] ** 2))
-
-        total_energy_in_signal = s / self.sample_rate
-
-        total_energy_of_exposure = []
-        if leq_mode == LeqDurationMode.transient:
-            total_energy_of_exposure = total_energy_in_signal
-        elif leq_mode == LeqDurationMode.steady_state:
-            if exposure_duration is None:
-                exposure_duration = signal_duration
-            total_energy_of_exposure = total_energy_in_signal * (exposure_duration / signal_duration)
-        elif leq_mode is None:
-            raise ValueError("User must specify a signal duration mode of class LeqDurationMode.")
-
-        average_energy_over_equivalent_duration = total_energy_of_exposure / equivalent_duration
-
-        return 10.0 * np.log10(average_energy_over_equivalent_duration / 20e-6 / 20e-6)
-
     @property
     def header(self):
         return self._header
 
     @header.setter
     def header(self, value):
         self._header = value
@@ -591,90 +644,34 @@
 
         for i in range(len(r)):
             r[i] = self.spectra[i].spectral_crest
 
         return r
 
     @property
+    def fundamental_frequency(self):
+        if self.spectra is None:
+            self._calculate_spectrogram()
+
+        r = np.zeros((len(self.times),))
+
+        for i in range(len(r)):
+            r[i] = self.spectra[i].fundamental_frequency
+
+        return r
+
+    @property
     def times_past_midnight(self):
         tpm = np.zeros((len(self.spectra),))
 
         for i in range(len(tpm)):
             tpm[i] = self.spectra[i].time_past_midnight
 
         return tpm
 
-    @property
-    def get_features(self):
-        """
-        This function will obtain the temporal, spectral, sound quality, and level metrics from the waveform and the
-        spectra within the time history.
-
-        Returns
-        -------
-        A Pandas.DataFrame with the information from each spectrum
-        """
-
-        #   Create the DataFrame that will hold the data from the waveform and the spectrum objects
-        names = ['attack', 'decrease', 'release', 'log_attack', 'attack_slope', 'decrease_slope', 'temporal_centroid',
-                 'effective_duration', 'amplitude_modulation', 'frequency_modulation', 'loudness', 'roughness',
-                 'sharpness', 'zero_crossing_rate', 'auto_correlation_00', 'auto_correlation_01', 'auto_correlation_02',
-                 'auto_correlation_03', 'auto_correlation_04', 'auto_correlation_05', 'auto_correlation_06',
-                 'auto_correlation_07', 'auto_correlation_08', 'auto_correlation_09', 'auto_correlation_10',
-                 'auto_correlation_11', 'spectral_centroid', 'spectral_spread', 'spectral_skewness',
-                 'spectral_kurtosis', 'spectral_slope', 'spectral_decrease', 'spectral_roll_off', 'spectral_energy',
-                 'spectral_flatness', 'spectral_crest', 'lf', 'la']
-        for f in self.frequencies:
-            names.append('F{:06.0f}Hz'.format(f))
-
-        names.append('time')
-
-        df = pd.DataFrame(columns=names, index=np.arange(len(self.times)))
-
-        for i in range(df.shape[0]):
-            s = self.spectra[i]
-            if isinstance(s, Spectrum):
-                if s.waveform is None:
-                    df.iloc[i, :14+12] = [np.nan] * (14 + 12)
-                else:
-                    df.iloc[i, :14] = [s.waveform.attack,
-                                       s.waveform.decrease,
-                                       s.waveform.release,
-                                       s.waveform.log_attack,
-                                       s.waveform.attack_slope,
-                                       s.waveform.decrease_slope,
-                                       s.waveform.temporal_centroid,
-                                       s.waveform.effective_duration,
-                                       s.waveform.amplitude_modulation,
-                                       s.waveform.frequency_modulation,
-                                       np.mean(s.waveform.loudness),
-                                       np.mean(s.waveform.roughness),
-                                       np.mean(s.waveform.sharpness),
-                                       np.mean(s.waveform.zero_crossing_rate)]
-                    df.iloc[i, 14:14 + 12] = np.mean(s.waveform.auto_correlation, axis=0)
-
-                df.iloc[i, 26:38] = [s.spectral_centroid,
-                                     s.spectral_spread,
-                                     s.spectral_skewness,
-                                     s.spectral_kurtosis,
-                                     s.spectral_slope,
-                                     s.spectral_decrease,
-                                     s.spectral_roll_off,
-                                     s.spectral_energy,
-                                     s.spectral_flatness,
-                                     s.spectral_crest,
-                                     s.overall_level,
-                                     s.overall_a_weighted_level]
-                for band_index in range(len(self.frequencies)):
-                    df.iloc[i, 38 + band_index] = s.pressures_decibels[band_index]
-
-                df.iloc[i, -1] = s.time_past_midnight
-
-        return df
-
 
 class NarrowbandTimeHistory(TimeHistory):
     """
     This class implements the _calculate_spectrogram function using the Narrowband_Spectrum class
     """
 
     def __init__(self, a: Waveform, integration_time: float = 0.25, fft_size: int = None):
@@ -687,15 +684,15 @@
         if self._fft_size is None:
 
             #   Set the default block size
             sub_wfm_length = self.integration_time * self.waveform.sample_rate
             self._fft_size = int(2 ** np.floor(np.log2(sub_wfm_length)))
 
         elif (self._fft_size > len(self.waveform.samples)) or \
-                (self.fft_size > self.integration_time * self.sample_rate):
+                (self.fft_size > self.integration_time * self.waveform.sample_rate):
             raise ValueError('FFT block size cannot be greater than the total length of the signal.')
 
     @property
     def fft_size(self):
         return self._fft_size
 
     def _calculate_spectrogram(self):
@@ -713,21 +710,21 @@
 
         #   Set the starting sample
         s0 = 0
 
         #   Loop through the elements and create the spectral object
         for n in range(N):
             #   get the subset of data from the waveform
-            subset = self.waveform.trim(s0, s0 + self.sample_size, TrimmingMethods.samples)
+            subset = self.waveform.trim(s0, s0 + self.waveform_sample_size, TrimmingMethods.samples)
 
             #   Create the spectrum object and add it as the ith element in the array
             self._spectra[n] = SpectrumByFFT(subset, self.fft_size)
 
             #   increment the starting sample
-            s0 += self.sample_size
+            s0 += self.waveform_sample_size
 
     def to_logarithmic_band_time_history(self, fob_band_width: int = 3, f0: float = 10, f1: float = 10000):
         """
         This function utilizes the functions within the SpectrumByFFT to generate a collection of
         Spectrum objects within a TimeHistory object.
 
         Parameters
@@ -777,15 +774,15 @@
 
     @property
     def stop_frequency(self):
         return self._stop_frequency
 
     @property
     def settle_time(self):
-        return self.settle_samples / self.sample_rate
+        return self.settle_samples / self.waveform.sample_rate
 
     @property
     def settle_samples(self):
         """
         Based on requirements of Matlab filtering, you must have at least 3 times the number of coefficients to
         accurately filter data. So this will start with that minimum, and then move through the full octave frequency
         band numbers to determine the minimum number of samples that are required for the filter to adequately settle.
@@ -808,22 +805,22 @@
 
         #   Set the starting sample
         s0 = 0
 
         #   Loop through the elements and create the spectral object
         for n in range(N):
             #   get the subset of data from the waveform
-            subset = self.waveform.trim(s0, s0 + self.sample_size, TrimmingMethods.samples)
+            subset = self.waveform.trim(s0, s0 + self.waveform_sample_size, TrimmingMethods.samples)
 
             #   Create the spectrum object and add it as the ith element in the array
             self._spectra[n] = SpectrumByDigitalFilters(subset, self.bandwidth, self.start_frequency,
                                                         self.stop_frequency)
 
             #   increment the starting sample
-            s0 += self.sample_size
+            s0 += self.waveform_sample_size
 
     def calculate_engineering_scale_factor(self, calibration_level: float = 94, calibration_frequency=1000):
         sensitivities = np.zeros((len(self.spectra),))
 
         for i in range(len(self.spectra)):
             sensitivities[i] = self.spectra[i].calculate_engineering_unit_scale_factor(calibration_level,
                                                                                        calibration_frequency)
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/swipe.py` & `PyTimbre-0.6.7/src/pytimbre/spectral/swipe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from scipy import interpolate
 import numpy as np
 # import librosa
 import scipy.signal
+from .spectra import Spectrum
 
 """
 | Description: libf0 SWIPE implementation
 | Contributors: Sebastian Rosenzweig, Vojtěch Pešek, Simon Schwär, Meinard Müller
 | License: The MIT license, https://opensource.org/licenses/MIT
 | This file is part of libf0.
 """
@@ -16,14 +17,68 @@
 
 2023_04_01 - FSM - Function arguments were normalized to the standard Python rules.
 2023-04-06 - FSM - Updated the swipe function to use the SciPy.Signal.STFT function rather than librosa
 2023-04-06 - FSM - Removed all functions that rely on librosa
 """
 
 
+def swipe_spectral_estimation(x: Spectrum, hop_size: float = 256, minimum_frequency: float = 10.0,
+                              maximum_frequency: float = 10000, pitch_resolution: float = 1 / 100,
+                              erb_resolution: float = 0.1,
+                              strength_threshold: float = 0):
+    if x.waveform is None:
+        raise ValueError("At this point, you must provide a Spectrum object that has been created from a waveform")
+    t = x.time
+
+    # Compute pitch candidates
+    pc = 2 ** np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
+
+    # Pitch strength matrix
+    S = np.zeros((len(pc),))
+
+    # Determine P2-WSs [max, min]
+    log_ws = np.round(np.log2(np.divide(8 * x.waveform.sample_rate, [minimum_frequency, maximum_frequency])))
+
+    # P2-WSs - window sizes in samples
+    ws = len(x.frequencies)
+
+    # Determine window sizes used by each pitch candidate
+    log2pc = np.arange(np.log2(minimum_frequency), np.log2(maximum_frequency), pitch_resolution)
+    d = log2pc - np.log2(np.divide(8 * x.waveform.sample_rate, ws))
+
+    # Create ERBs spaced frequencies (in Hertz)
+    f_erbs = erbs2hz(np.arange(hz2erbs(pc[0] / 4), hz2erbs(x.waveform.sample_rate / 2), erb_resolution))
+
+    #   Resample the frequency spectrum to the ERB frequencies
+    loudness = interpolate.splev(f_erbs, interpolate.splrep(x.frequencies, x.pressures_pascals ** 2))
+    # loudness = np.sqrt(magnitude)
+
+    pc_to_compute = pc
+
+    # Normalize loudness
+    normalization_loudness = np.full_like(loudness, np.sqrt(np.sum(loudness * loudness, axis=0)))
+    with np.errstate(divide='ignore', invalid='ignore'):
+        loudness = loudness / normalization_loudness
+
+    # Create pitch salience matrix
+    S = np.zeros((len(pc_to_compute),))
+
+    for j in range(0, len(pc_to_compute)):
+        S[j] = pitch_strength_one(f_erbs, loudness, pc_to_compute[j])
+
+    # pitch_strength = pitch_strength_all_candidates(f_erbs, loudness, pc_to_compute)
+
+    pitches, strength = parabolic_interpolation(S, strength_threshold, pc)
+
+    if np.isnan(pitches):
+        pitches = 0  # avoid NaN output
+
+    return pitches, t, strength
+
+
 def swipe(samples, sample_rate: float = 22050, hop_size: float = 256, minimum_frequency: float = 55.0,
           maximum_frequency: float = 1760.0, pitch_resolution: float = 1 / 96, erb_resolution: float = 0.1,
           strength_threshold: float = 0):
     """
     Implementation of a sawtooth waveform inspired pitch estimator (SWIPE).
     This version of the algorithm follows the original implementation, see `swipe_slim` for a more efficient
     alternative.
@@ -206,14 +261,15 @@
     # Compute pitch strength
     S = np.dot(k, normalized_loudness)
     return S
 
 
 def resample_ferbs(spectrum, f, ferbs):
     """Resample to ERB scale"""
+
     magnitude = np.zeros((len(ferbs), spectrum.shape[1]))
 
     for t in range(spectrum.shape[1]):
         spl = interpolate.splrep(f, spectrum[:, t])
         interpolate.splev(ferbs, spl)
 
         magnitude[:, t] = interpolate.splev(ferbs, spl)
@@ -271,14 +327,45 @@
                 poly = np.polyval(c, nftc)
                 k = np.argmax(poly)
                 s[j] = poly[k]
                 p[j] = 2 ** (np.log2(pc[I[0]]) + k / 12 / 64)
     return p, s
 
 
+def parabolic_interpolation(pitch_strength, strength_threshold, pc):
+    """Parabolic interpolation between pitch candidates using pitch strength"""
+
+    i = np.argmax(pitch_strength)
+    strength = pitch_strength[i]
+
+    if strength < strength_threshold:
+        return np.nan, np.nan
+
+    if i == 0:
+        return pc[0], pitch_strength[0]
+    elif i == len(pc) - 1:
+        return pc[-1], pitch_strength[-1]
+    else:
+        I = np.arange(i - 1, i + 2)
+        tc = 1 / pc[I]
+        ntc = np.dot((tc / tc[1] - 1), 2 * np.pi)
+        if np.any(np.isnan(pitch_strength[I])):
+            s = np.nan
+            p = np.nan
+        else:
+            c = np.polyfit(ntc, pitch_strength[I], 2)
+            ftc = 1 / 2 ** np.arange(np.log2(pc[I[0]]), np.log2(pc[I[2]]), 1 / 12 / 64)
+            nftc = np.dot((ftc / tc[1] - 1), 2 * np.pi)
+            poly = np.polyval(c, nftc)
+            k = np.argmax(poly)
+            s = poly[k]
+            p = 2 ** (np.log2(pc[I[0]]) + k / 12 / 64)
+        return p, s
+
+
 def primes(n):
     """Returns a set of n prime numbers"""
     small_primes = np.array([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89,
                              97, 101, 103, 107, 109, 113, 127, 131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181,
                              191, 193, 197, 199, 211, 223, 227, 229, 233, 239, 241, 251, 257, 263, 269, 271, 277, 281,
                              283, 293, 307, 311, 313, 317, 331, 337, 347, 349, 353, 359, 367, 373, 379, 383, 389, 397,
                              401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487, 491, 499, 503,
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/waveform.py` & `PyTimbre-0.6.7/src/pytimbre/waveform.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from datetime import datetime, timedelta
 from enum import Enum
 from scipy.signal.windows import hamming, tukey
 import scipy.signal
 import statsmodels.api as sm
 import colorednoise as cn
 import warnings
-from .swipe import swipe
-from .yin import yin
 from typing import Dict, Tuple
 import numpy.typing as npt
+from .yin import yin
 
 
 class WindowingMethods(Enum):
     """
     The available windowing methods for the waveform
     """
 
@@ -441,24 +440,21 @@
 
         clipped_sections, total_clipped_samples = Waveform._detect_clipping(self.samples)
 
         return not ((total_clipped_samples / len(self.samples)) < 0.01)
 
     @property
     def fundamental_frequency(self):
-        # return np.median(swipe(self.samples, self.sample_rate, minimum_frequency=10, maximum_frequency=10000,
-        #                        strength_threshold=0.25, hop_size=0.25 * self.sample_rate)[0])
-
         return np.median(yin(
             self.samples,
             self.sample_rate,
             F_max=10000,
             F_min=10,
-            N=int(np.floor(self.sample_rate/10)),
-            H=int(np.floor(self.sample_rate/10/4))
+            N=int(np.floor(self.sample_rate / 10)),
+            H=int(np.floor(self.sample_rate / 10 / 4))
         )[0])
 
     # ------------------ Static functions for the calculation of filter shapes and timbre features ---------------------
     @staticmethod
     def _detect_clipping(
             samples_array: npt.NDArray, max_threshold=0.995, min_threshold=0.995
     ) -> Tuple[Dict[str, int], int]:
@@ -1565,16 +1561,15 @@
                     'attack slope': self.attack_slope,
                     'decrease slope': self.decrease_slope,
                     'temporal centroid': self.temporal_centroid,
                     'effective duration': self.effective_duration,
                     'amplitude modulation': self.amplitude_modulation,
                     'frequency modulation': self.frequency_modulation,
                     'auto-correlation': self.auto_correlation,
-                    'zero crossing rate': self.zero_crossing_rate,
-                    'fundamental_frequency': np.mean(self.fundamental_frequency)}
+                    'zero crossing rate': self.zero_crossing_rate}
 
         if include_sq_metrics:
             features['loudness'] = self.loudness
             features['roughness'] = self.roughness
             features['sharpness'] = self.sharpness
 
         return features
@@ -1903,28 +1898,28 @@
         function specified this is applied before the pressures are summed. Additionally, the duration of the summation
         is specified (in seconds) for the new value with a default of 8 hours. Finally, if there is a cause to exclude
         portions of the data (i.e. calculating the SEL for the 10 dB down points in community noise) you can specify
         the start and stop index. If the stop index is None, then the last pressure defines the limit of the summation.
 
         Parameters
         ----------
-        weighting   :   WeightingFunctions
+        :param weighting:   WeightingFunctions
             The enumeration to determine filtering function applied to the waveform
-        equivalent_duration :   float
+        :param equivalent_duration :   float
             The denominator of the summation - in seconds - representing the desired length of total exposure
             time (e.g. an 8-hour duty day, or a 1-second sound exposure level)
-        start_sample    :   int
+        :param start_sample :   int
             default = 0. The start sample of the pressure summation
-        stop_sample :   int
+        :param stop_sample :   int
             default = None. The stop sample, if the value is None, then it is replaces with the last sample index
-        leq_mode    :   LeqDurationMode
+        :param leq_mode :   LeqDurationMode
             The enumeration to determine whether the input signal contains all energy
             of an exposure to the listener (transient) or the signal represents a sample of a longer-duration
             (steady_state) exposure
-        exposure_duration   :   float
+        :param exposure_duration :   float
             If leq_mode is steady_state, this is the actual time of noise exposure to the
             listener in seconds
 
         """
 
         if stop_sample is None:
             stop_sample = len(self.samples)
```

### Comparing `PyTimbre-0.6.6/src/pytimbre/yin.py` & `PyTimbre-0.6.7/src/pytimbre/yin.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,19 @@
     t : ndarray
         Time axis
     ap: ndarray
         Aperiodicity (indicator for voicing: the lower, the more reliable the estimate)
     """
 
     if F_min > F_max:
-        raise Exception("F_min must be smaller than F_max!")
+        raise ValueError("F_min must be smaller than F_max!")
 
     if F_min < Fs/N:        
-        raise Exception(f"The condition (F_min >= Fs/N) was not met. With Fs = {Fs}, N = {N} and F_min = {F_min} you have the following options: \n1) Set F_min >= {np.ceil(Fs/N)} Hz. \n2) Set N >= {np.ceil(Fs/F_min).astype(int)}. \n3) Set Fs <= {np.floor(F_min * N)} Hz.")
+        raise ValueError(f"The condition (F_min >= Fs/N) was not met. With Fs = {Fs}, N = {N} and F_min = {F_min} you have "
+                 f"the following options: \n1) Set F_min >= {np.ceil(Fs/N)} Hz. \n2) Set N >= {np.ceil(Fs/F_min).astype(int)}. \n3) Set Fs <= {np.floor(F_min * N)} Hz.")
 
     x_pad = np.concatenate((np.zeros(N//2), x, np.zeros(N//2)))  # Add zeros for centered estimates
     M = int(np.floor((len(x_pad) - N) / H)) + 1  # Compute number of estimates that will be generated
     f0 = np.zeros(M)  # Estimated fundamental frequencies (0 for unspecified frames)
     t = np.arange(M)*H/Fs  # Time axis
     ap = np.zeros(M)  # Aperiodicity
```

