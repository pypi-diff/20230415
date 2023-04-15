# Comparing `tmp/jkh011120_randmat-0.0.1-py3-none-any.whl.zip` & `tmp/jkh011120_randmat-0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1527 bytes, number of entries: 5
--rw-r--r--  2.0 unx      379 b- defN 23-Apr-15 04:33 randmat/randmat.py
--rw-r--r--  2.0 unx      282 b- defN 23-Apr-15 04:33 jkh011120_randmat-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 04:33 jkh011120_randmat-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-15 04:33 jkh011120_randmat-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      410 b- defN 23-Apr-15 04:33 jkh011120_randmat-0.0.1.dist-info/RECORD
-5 files, 1171 bytes uncompressed, 753 bytes compressed:  35.7%
+Zip file size: 1630 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      378 b- defN 23-Apr-15 04:59 randmat/randmat.py
+-rw-r--r--  2.0 unx      721 b- defN 23-Apr-15 04:59 jkh011120_randmat-0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 04:59 jkh011120_randmat-0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-15 04:59 jkh011120_randmat-0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      402 b- defN 23-Apr-15 04:59 jkh011120_randmat-0.1.dist-info/RECORD
+5 files, 1601 bytes uncompressed, 872 bytes compressed:  45.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: randmat/randmat.py
 Comment: 
 
-Filename: jkh011120_randmat-0.0.1.dist-info/METADATA
+Filename: jkh011120_randmat-0.1.dist-info/METADATA
 Comment: 
 
-Filename: jkh011120_randmat-0.0.1.dist-info/WHEEL
+Filename: jkh011120_randmat-0.1.dist-info/WHEEL
 Comment: 
 
-Filename: jkh011120_randmat-0.0.1.dist-info/top_level.txt
+Filename: jkh011120_randmat-0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jkh011120_randmat-0.0.1.dist-info/RECORD
+Filename: jkh011120_randmat-0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## randmat/randmat.py

```diff
@@ -1,13 +1,13 @@
 import numpy as np 
 import matplotlib.pyplot as plt 
 
 def randhist(n_bins:int, around:int)->None:
     x = np.random.randn(around)
-    plt.hist(x, n_bins, histtype='bar', color= "red");
+    plt.hist(x, n_bins, histtype='bar', color= "red")
     plt.show()
 
 def randscatter(start_x:int,end_x:int,y:int)->None:
     xData = np.arange(start_x, end_x) 
     yData = xData + 2*np.random.randn(y)
     plt.scatter(xData, yData) 
     plt.show()
```

