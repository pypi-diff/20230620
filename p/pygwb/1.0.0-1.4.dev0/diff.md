# Comparing `tmp/pygwb-1.0.0.tar.gz` & `tmp/pygwb-1.4.dev0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygwb-1.0.0.tar", last modified: Fri Mar 31 01:58:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

