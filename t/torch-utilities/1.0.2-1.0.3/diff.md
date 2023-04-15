# Comparing `tmp/torch_utilities-1.0.2.tar.gz` & `tmp/torch_utilities-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_utilities-1.0.2.tar", last modified: Tue Apr 11 21:00:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

