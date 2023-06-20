# Comparing `tmp/subseq-1.0.3.tar.gz` & `tmp/subseq-1.0.4-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subseq-1.0.3.tar", last modified: Tue May  3 14:03:16 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

