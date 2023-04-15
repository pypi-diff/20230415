# Comparing `tmp/sabledocs-0.1.43.tar.gz` & `tmp/sabledocs-0.1.46-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.1.43.tar", last modified: Sat Apr 15 20:04:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

