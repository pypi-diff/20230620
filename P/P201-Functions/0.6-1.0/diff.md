# Comparing `tmp/P201_Functions-0.6.tar.gz` & `tmp/P201_Functions-1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "P201_Functions-0.6.tar", last modified: Thu Aug 25 13:17:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

