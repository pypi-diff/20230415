# Comparing `tmp/ctypeslib2-2.3.2.tar.gz` & `tmp/ctypeslib2-2.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ctypeslib2-2.3.2.tar", last modified: Wed Apr  7 03:44:05 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

