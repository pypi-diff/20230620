# Comparing `tmp/narm2_SBU-1.0.tar.gz` & `tmp/narm2_SBU-1.1-py3.11.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "narm2_SBU-1.0.tar", last modified: Sun Jun 18 12:05:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

