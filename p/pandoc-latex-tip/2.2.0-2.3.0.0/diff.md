# Comparing `tmp/pandoc-latex-tip-2.2.0.tar.gz` & `tmp/pandoc_latex_tip-2.3.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-latex-tip-2.2.0.tar", last modified: Sun Jan 30 14:24:56 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

