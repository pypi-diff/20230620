# Comparing `tmp/supercells-0.0.3.tar.gz` & `tmp/supercells-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ubuntu/supercells/dist/.tmp-lavpp1f9/supercells-0.0.3.tar", last modified: Wed Mar  1 15:48:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

