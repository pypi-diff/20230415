# Comparing `tmp/novauniverse-2.1.1.tar.gz` & `tmp/novauniverse-2.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novauniverse-2.1.1.tar", last modified: Thu Apr 13 16:04:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

