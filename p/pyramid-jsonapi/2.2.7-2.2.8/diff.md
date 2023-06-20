# Comparing `tmp/pyramid_jsonapi-2.2.7.tar.gz` & `tmp/pyramid_jsonapi-2.2.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramid_jsonapi-2.2.7.tar", last modified: Wed May 24 09:42:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

