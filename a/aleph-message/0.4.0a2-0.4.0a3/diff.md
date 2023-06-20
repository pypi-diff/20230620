# Comparing `tmp/aleph-message-0.4.0a2.tar.gz` & `tmp/aleph_message-0.4.0a3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-message-0.4.0a2.tar", last modified: Wed May 31 13:58:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

