# Comparing `tmp/pythonBgt-0.43-py3-none-any.whl.zip` & `tmp/pythonBgt-0.44-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6719 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    18492 b- defN 23-Mar-20 20:00 pythonBgt/pythonBgt.py
+Zip file size: 6685 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-Apr-14 21:49 pythonBgt/pythonBgt.py
 -rw-rw-rw-  2.0 fat       26 b- defN 22-Mar-07 18:01 pythonBgt/__init__.py
--rw-rw-rw-  2.0 fat      632 b- defN 23-Mar-20 20:26 pythonBgt-0.43.dist-info/metadata.json
--rw-rw-rw-  2.0 fat       10 b- defN 23-Mar-20 20:26 pythonBgt-0.43.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Mar-20 20:26 pythonBgt-0.43.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      517 b- defN 23-Mar-20 20:26 pythonBgt-0.43.dist-info/METADATA
--rw-rw-rw-  2.0 fat      558 b- defN 23-Mar-20 20:26 pythonBgt-0.43.dist-info/RECORD
-7 files, 20332 bytes uncompressed, 5739 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat      632 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      517 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      558 b- defN 23-Apr-14 22:04 pythonBgt-0.44.dist-info/RECORD
+7 files, 19912 bytes uncompressed, 5705 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pythonBgt/pythonBgt.py
 Comment: 
 
 Filename: pythonBgt/__init__.py
 Comment: 
 
-Filename: pythonBgt-0.43.dist-info/metadata.json
+Filename: pythonBgt-0.44.dist-info/metadata.json
 Comment: 
 
-Filename: pythonBgt-0.43.dist-info/top_level.txt
+Filename: pythonBgt-0.44.dist-info/top_level.txt
 Comment: 
 
-Filename: pythonBgt-0.43.dist-info/WHEEL
+Filename: pythonBgt-0.44.dist-info/WHEEL
 Comment: 
 
-Filename: pythonBgt-0.43.dist-info/METADATA
+Filename: pythonBgt-0.44.dist-info/METADATA
 Comment: 
 
-Filename: pythonBgt-0.43.dist-info/RECORD
+Filename: pythonBgt-0.44.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pythonBgt/pythonBgt.py

```diff
@@ -535,17 +535,15 @@
 	getThread.start()
 	while not geted==True: wait(5)
 	return contentGet
 def serialize(dict, file):
 	pickle.dump(dict, open(file, "wb"))
 def deserialize(file):
 	return pickle.load(open(file, "rb"))
-def positionSound1d(sound, listenerX, sourceX, panStep=1, volumeStep=1):
-	positionSoundCustom1d(sound, listenerX, sourceX, panStep=panStep, volumeStep=volumeStep, startPan=0.0, startVolume=0.0)
-def positionSoundCustom1d(sound, listenerX, sourceX, panStep=1, volumeStep=1, startPan=0.0, startVolume=0.0):
+def positionSound1d(sound, listenerX, sourceX, panStep=1, volumeStep=1, startPan=0.0, startVolume=0.0):
 	finalPan=startPan
 	finalVolume=startVolume
 	if sourceX<listenerX:
 		delta=listenerX-sourceX
 		finalPan-=delta*panStep
 		finalVolume-=delta*volumeStep
 	elif sourceX>listenerX:
@@ -556,30 +554,31 @@
 	elif finalPan<-100: finalPan=-100
 	if finalVolume>100: finalVolume=100
 	elif finalVolume<-100: finalVolume=-100
 	if not sound.pan==finalPan:
 		sound.pan=finalPan
 	if not sound.volume==finalVolume:
 		sound.volume=finalVolume
-def positionSound2d(sound, listenerX, sourceX, listenerY, sourceY, panStep=1, volumeStep=1, pitchDecrease=5):
-	positionSoundCustom2d(sound, listenerX, sourceX, listenerY, sourceY, panStep=panStep, volumeStep=volumeStep, pitchDecrease=pitchDecrease, startPan=0.0, startVolume=0.0, startPitch=100.0)
-def positionSoundCustom2d(sound, listenerX, sourceX, listenerY, sourceY, panStep=1, volumeStep=1, pitchDecrease=5, startPan=0.0, startVolume=0.0, startPitch=100.0):
+def positionSound2d(sound, listenerX, listenerY, sourceX, sourceY, panStep=1, volumeStep=1, pitchDecrease=5, startPan=0.0, startVolume=0.0, startPitch=100.0):
 	finalPan=startPan
 	finalVolume=startVolume
 	finalPitch=startPitch
 	if sourceX<listenerX:
 		delta=listenerX-sourceX
 		finalPan-=delta*panStep
 		finalVolume-=delta*volumeStep
 	elif sourceX>listenerX:
 		delta=sourceX-listenerX
 		finalPan+=delta*panStep
 		finalVolume-=delta*volumeStep
-	if sourceY>listenerY:
+	if listenerY>sourceY:
 		finalPitch-=pitchDecrease
+		deltaY=listenerY-sourceY
+		finalVolume-=deltaY*volumeStep
+	elif sourceY>listenerY:
 		deltaY=sourceY-listenerY
 		finalVolume-=deltaY*volumeStep
 	if finalPan>100: finalPan=100
 	elif finalPan<-100: finalPan=-100
 	if finalVolume>100: finalVolume=100
 	elif finalVolume<-100: finalVolume=-100
 	if finalPitch>400: finalPitch=400
```

## Comparing `pythonBgt-0.43.dist-info/metadata.json` & `pythonBgt-0.44.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.44'"}*

```diff
@@ -31,9 +31,9 @@
                 "accessible-output2",
                 "pyperclip",
                 "pyenet310"
             ]
         }
     ],
     "summary": "PythonBgt is a library for Python that allows the easy and practical creation of audiogames, combining the flexibility and modernity of Python with the simplicity and practicality of BGT.",
-    "version": "0.43"
+    "version": "0.44"
 }
```

## Comparing `pythonBgt-0.43.dist-info/METADATA` & `pythonBgt-0.44.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: pythonBgt
-Version: 0.43
+Version: 0.44
 Summary: PythonBgt is a library for Python that allows the easy and practical creation of audiogames, combining the flexibility and modernity of Python with the simplicity and practicality of BGT.
 Author: Gabriel Haberkamp
 Keywords: Python,BGT,Python_Bgt,audiogame,audiogames,games
 Requires-Dist: pygame
 Requires-Dist: sound-lib
 Requires-Dist: wxpython310
 Requires-Dist: requests
```

