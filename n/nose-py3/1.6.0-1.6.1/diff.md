# Comparing `tmp/nose-py3-1.6.0.tar.gz` & `tmp/nose_py3-1.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nose-py3-1.6.0.tar", last modified: Fri Mar 17 07:41:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

