# Comparing `tmp/vmklib-1.8.2.tar.gz` & `tmp/vmklib-1.8.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmklib-1.8.2.tar", last modified: Fri May 26 06:27:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

