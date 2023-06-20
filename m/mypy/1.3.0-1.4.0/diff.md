# Comparing `tmp/mypy-1.3.0.tar.gz` & `tmp/mypy-1.4.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-1.3.0.tar", last modified: Tue May  9 14:54:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

