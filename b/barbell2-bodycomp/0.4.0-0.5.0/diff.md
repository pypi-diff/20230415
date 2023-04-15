# Comparing `tmp/barbell2_bodycomp-0.4.0.tar.gz` & `tmp/barbell2_bodycomp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barbell2_bodycomp-0.4.0.tar", last modified: Sat Apr 15 07:09:24 2023, max compression
+gzip compressed data, was "dist/barbell2_bodycomp-0.5.0.tar", last modified: Sat Apr 15 10:50:04 2023, max compression
```

## Comparing `barbell2_bodycomp-0.4.0.tar` & `barbell2_bodycomp-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.467263 barbell2_bodycomp-0.4.0/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 07:09:24.466997 barbell2_bodycomp-0.4.0/PKG-INFO
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.462636 barbell2_bodycomp-0.4.0/barbell2_bodycomp/
--rw-r--r--   0 ralph      (501) staff       (20)      392 2023-04-15 07:09:19.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     4465 2023-04-13 12:43:05.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/calculator.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.466278 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/
--rw-r--r--   0 ralph      (501) staff       (20)      403 2023-04-13 11:54:27.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2nifti.py
--rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2npy.py
--rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2nrrd.py
--rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2png.py
--rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/tag2dcm.py
--rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/tag2npy.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.466627 barbell2_bodycomp-0.4.0/barbell2_bodycomp/pipeline/
--rw-r--r--   0 ralph      (501) staff       (20)        0 2023-04-13 11:55:38.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/pipeline/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     3152 2023-04-15 07:05:04.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/pipeline/bodycomp.py
--rw-r--r--   0 ralph      (501) staff       (20)     6054 2023-04-13 11:59:22.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/seg.py
--rw-r--r--   0 ralph      (501) staff       (20)     1394 2023-04-13 12:19:43.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectroi.py
--rw-r--r--   0 ralph      (501) staff       (20)     5804 2023-04-13 12:19:18.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectslice.py
--rw-r--r--   0 ralph      (501) staff       (20)     1586 2023-04-13 11:15:28.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/totalseg.py
--rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp/utils.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 07:09:24.464418 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      882 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/not-zip-safe
--rw-r--r--   0 ralph      (501) staff       (20)       68 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/requires.txt
--rw-r--r--   0 ralph      (501) staff       (20)       18 2023-04-15 07:09:24.000000 barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 07:09:24.467342 barbell2_bodycomp-0.4.0/setup.cfg
--rw-r--r--   0 ralph      (501) staff       (20)     1456 2023-04-13 12:44:51.000000 barbell2_bodycomp-0.4.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.725824 barbell2_bodycomp-0.5.0/
+-rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 10:50:04.725562 barbell2_bodycomp-0.5.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.720772 barbell2_bodycomp-0.5.0/barbell2_bodycomp/
+-rw-r--r--   0 ralph      (501) staff       (20)      392 2023-04-15 10:50:00.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     4447 2023-04-15 10:49:32.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/calculator.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.724652 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/
+-rw-r--r--   0 ralph      (501) staff       (20)      403 2023-04-13 11:54:27.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2200 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2nifti.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1485 2023-04-13 10:26:30.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2npy.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1405 2023-04-13 10:39:19.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      853 2023-04-13 10:16:54.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2nrrd.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2030 2023-04-13 10:40:43.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2png.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1059 2023-04-13 10:41:23.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/tag2dcm.py
+-rw-r--r--   0 ralph      (501) staff       (20)      435 2023-04-13 10:41:41.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/tag2npy.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.725060 barbell2_bodycomp-0.5.0/barbell2_bodycomp/pipeline/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2023-04-13 11:55:38.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/pipeline/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     3434 2023-04-15 08:57:42.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/pipeline/bodycomp.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6054 2023-04-13 11:59:22.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/seg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1394 2023-04-13 12:19:43.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectroi.py
+-rw-r--r--   0 ralph      (501) staff       (20)     5804 2023-04-13 12:19:18.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectslice.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1586 2023-04-13 11:15:28.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/totalseg.py
+-rw-r--r--   0 ralph      (501) staff       (20)     6246 2023-04-13 10:17:39.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2023-04-15 10:50:04.722759 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)      802 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      882 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       20 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-04-13 10:43:22.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)       68 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       18 2023-04-15 10:50:04.000000 barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2023-04-15 10:50:04.725902 barbell2_bodycomp-0.5.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1456 2023-04-13 12:44:51.000000 barbell2_bodycomp-0.5.0/setup.py
```

### Comparing `barbell2_bodycomp-0.4.0/PKG-INFO` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: barbell2_bodycomp
-Version: 0.4.0
+Name: barbell2-bodycomp
+Version: 0.5.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/calculator.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/calculator.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,19 +69,19 @@
                 'sat_area': calculate_area(segmentations, BodyCompositionCalculator.SAT, pixel_spacing),
                 'muscle_ra': calculate_mean_radiation_attenuation(image, segmentations, BodyCompositionCalculator.MUSCLE),
                 'vat_ra': calculate_mean_radiation_attenuation(image, segmentations, BodyCompositionCalculator.VAT),
                 'sat_ra': calculate_mean_radiation_attenuation(image, segmentations, BodyCompositionCalculator.SAT),
             }
             logger.info(f'{file_pair[0]}:')
             logger.info(' - muscle_area: {}'.format(self.output_metrics[file_pair[0]]['muscle_area']))
-            logger.info(' - vat_area: {}'.format(self.output_metrics[file_pair[0]]['muscle_area']))
-            logger.info(' - sat_area: {}'.format(self.output_metrics[file_pair[0]]['muscle_area']))
-            logger.info(' - muscle_ra: {}'.format(self.output_metrics[file_pair[0]]['muscle_area']))
-            logger.info(' - vat_ra: {}'.format(self.output_metrics[file_pair[0]]['muscle_area']))
-            logger.info(' - sat_ra: {}'.format(self.output_metrics[file_pair[0]]['muscle_area']))
+            logger.info(' - vat_area: {}'.format(self.output_metrics[file_pair[0]]['vat_area']))
+            logger.info(' - sat_area: {}'.format(self.output_metrics[file_pair[0]]['sat_area']))
+            logger.info(' - muscle_ra: {}'.format(self.output_metrics[file_pair[0]]['muscle_ra']))
+            logger.info(' - vat_ra: {}'.format(self.output_metrics[file_pair[0]]['vat_ra']))
+            logger.info(' - sat_ra: {}'.format(self.output_metrics[file_pair[0]]['sat_ra']))
         return self.output_metrics
 
 
 if __name__ == '__main__':
     def main():
         calculator = BodyCompositionCalculator()
         calculator.input_files = ['/mnt/localscratch/cds/rbrecheisen/raw/pancreas-demo-1/1.dcm']
```

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2nifti.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/dcm2npy.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/dcm2npy.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2dcm.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2nrrd.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2nrrd.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/npy2png.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/npy2png.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/convert/tag2dcm.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/convert/tag2dcm.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/pipeline/bodycomp.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/pipeline/bodycomp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
+import argparse
 
 from barbell2_bodycomp.convert import DicomToNifti
-from barbell2_bodycomp import TotalSegmentator, RoiSelector, SliceSelector, MuscleFatSegmentator
+from barbell2_bodycomp import TotalSegmentator, RoiSelector, SliceSelector, MuscleFatSegmentator, BodyCompositionCalculator
 
 
 class BodyCompositionPipeline:
 
     """
-    purpose of this component is to easily run the whole body composition pipeline from 
-    beginning to end. under the hood, the components handling the different steps are
+    Purpose of this component is to easily run the whole body composition pipeline from 
+    beginning to end. Under the hood, the components handling the different steps are
     executed in sequence.
+
+    TODO: If output already exists, skip it unless overwrite=True
     """
 
     def __init__(self, 
                  input_directory, 
                  output_directory, 
                  model_files, 
                  mode=MuscleFatSegmentator.ARGMAX
@@ -54,28 +57,33 @@
         segmentator.image_dimensions = (512, 512)
         segmentator.model_files = self.model_files
         segmentator.mode = self.mode
         segmentator.output_directory = os.path.join(self.output_directory, 'segmentator')
         output_files = segmentator.execute()
         for f in output_files:
             print(f)
+        # calculte body composition metrics
+        calculator = BodyCompositionCalculator()
+        calculator.input_files = segmentator.input_files
+        calculator.input_segmentation_files = output_files
+        output_metrics = calculator.execute()
+        print(output_metrics)
 
 
 if __name__ == '__main__':
     def main():
-        # update package path
-        import sys
-        root_dir = '/home/local/UNIMAAS/r.brecheisen/barbell2_bodycomp'
-        if root_dir not in sys.path:
-            sys.path.append(root_dir)
-        # run pipeline
+
+        parser = argparse.ArgumentParser()
+        parser.add_argument('input_directory')
+        parser.add_argument('output_directory')
+        parser.add_argument('model_files', nargs='+', default=[])
+        parser.add_argument('mode', choices=['ARGMAX', 'PROBABILITIES'])
+        args = parser.parse_args()
+
         pipeline = BodyCompositionPipeline(
-            '/mnt/localscratch/cds/rbrecheisen/raw/tlodewick-ct-noise-1/AL_100%/101816478/2-Abdomen',
-            '/mnt/localscratch/cds/rbrecheisen/processed/out', [
-                '/mnt/localscratch/cds/rbrecheisen/models/v2/model.zip',
-                '/mnt/localscratch/cds/rbrecheisen/models/v2/contour_model.zip',
-                '/mnt/localscratch/cds/rbrecheisen/models/v2/params.json',            
-            ],
-            MuscleFatSegmentator.ARGMAX,
+            input_directory=args.input_directory,
+            output_directory=args.output_directory, 
+            model_files=args.model_files,
+            mode=MuscleFatSegmentator.ARGMAX if args.mode == 'ARGMAX' else MuscleFatSegmentator.PROBABILITIES,
         )
         pipeline.execute()
     main()
```

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/seg.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/seg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectroi.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectroi.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/selectslice.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/selectslice.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/totalseg.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/totalseg.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp/utils.py` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp/utils.py`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/PKG-INFO` & `barbell2_bodycomp-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: barbell2-bodycomp
-Version: 0.4.0
+Name: barbell2_bodycomp
+Version: 0.5.0
 Summary: components for command-line body composition analysis
 Home-page: https://github.com/rbrecheisen/barbell2_bodycomp
 Author: Ralph Brecheisen
 Author-email: r.brecheisen@maastrichtuniversity.nl
 License: MIT license
 Description: UNKNOWN
 Keywords: barbell2_bodycomp
```

### Comparing `barbell2_bodycomp-0.4.0/barbell2_bodycomp.egg-info/SOURCES.txt` & `barbell2_bodycomp-0.5.0/barbell2_bodycomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barbell2_bodycomp-0.4.0/setup.py` & `barbell2_bodycomp-0.5.0/setup.py`

 * *Files identical despite different names*

