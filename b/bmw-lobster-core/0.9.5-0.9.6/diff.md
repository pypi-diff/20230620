# Comparing `tmp/bmw-lobster-core-0.9.5.tar.gz` & `tmp/bmw_lobster_core-0.9.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-core-0.9.5.tar", last modified: Wed Jun 14 14:03:19 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

