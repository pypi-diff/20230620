# Comparing `tmp/finx_io-0.2.5.tar.gz` & `tmp/finx_io-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finx_io-0.2.5.tar", last modified: Mon May  1 18:40:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

