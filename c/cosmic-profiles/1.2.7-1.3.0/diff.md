# Comparing `tmp/cosmic_profiles-1.2.7.tar.gz` & `tmp/cosmic_profiles-1.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_profiles-1.2.7.tar", last modified: Tue Aug 30 12:08:17 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

