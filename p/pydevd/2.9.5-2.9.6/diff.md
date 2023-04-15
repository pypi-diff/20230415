# Comparing `tmp/pydevd-2.9.5.tar.gz` & `tmp/pydevd-2.9.6-cp37-cp37m-macosx_10_15_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydevd-2.9.5.tar", last modified: Fri Dec 30 20:21:47 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

