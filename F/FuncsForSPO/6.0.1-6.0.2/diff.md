# Comparing `tmp/FuncsForSPO-6.0.1.tar.gz` & `tmp/FuncsForSPO-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.0.1.tar", last modified: Sun Jun 18 22:42:43 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.0.2.tar", last modified: Tue Jun 20 14:43:28 2023, max compression
```

## Comparing `FuncsForSPO-6.0.1.tar` & `FuncsForSPO-6.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.220052 FuncsForSPO-6.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.890102 FuncsForSPO-6.0.1/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.943450 FuncsForSPO-6.0.1/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.0.1/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.0.1/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.952450 FuncsForSPO-6.0.1/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.0.1/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.960449 FuncsForSPO-6.0.1/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.0.1/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.965450 FuncsForSPO-6.0.1/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.1/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.968451 FuncsForSPO-6.0.1/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.1/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-6.0.1/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.979824 FuncsForSPO-6.0.1/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.0.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.983825 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.012924 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     8120 2023-06-17 20:27:58.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.030927 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.045933 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.049930 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.074931 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.085384 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.096166 FuncsForSPO-6.0.1/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.106116 FuncsForSPO-6.0.1/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-6.0.1/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.116117 FuncsForSPO-6.0.1/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-6.0.1/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.125128 FuncsForSPO-6.0.1/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.0.1/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.135115 FuncsForSPO-6.0.1/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.1/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.0.1/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.144116 FuncsForSPO-6.0.1/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.0.1/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.0.1/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:43.149559 FuncsForSPO-6.0.1/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-6.0.1/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:42:42.933453 FuncsForSPO-6.0.1/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-18 22:42:42.000000 FuncsForSPO-6.0.1/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1886 2023-06-18 22:42:42.000000 FuncsForSPO-6.0.1/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 22:42:42.000000 FuncsForSPO-6.0.1/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-18 22:42:42.000000 FuncsForSPO-6.0.1/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      458 2023-06-18 22:42:42.000000 FuncsForSPO-6.0.1/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.0.1/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-18 22:42:43.217038 FuncsForSPO-6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-6.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-18 22:42:43.221041 FuncsForSPO-6.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2611 2023-06-18 22:42:03.000000 FuncsForSPO-6.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.456146 FuncsForSPO-6.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.045098 FuncsForSPO-6.0.2/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.105942 FuncsForSPO-6.0.2/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.0.2/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.0.2/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.117531 FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.125530 FuncsForSPO-6.0.2/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.0.2/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.133376 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.137567 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.148383 FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.155055 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.191304 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     8203 2023-06-19 21:37:07.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.211433 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.227744 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.234308 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.262342 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     8971 2023-06-18 22:41:54.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.272864 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.314948 FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.329481 FuncsForSPO-6.0.2/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-6.0.2/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.347521 FuncsForSPO-6.0.2/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-6.0.2/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.359364 FuncsForSPO-6.0.2/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.0.2/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.370694 FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.380329 FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.386213 FuncsForSPO-6.0.2/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-6.0.2/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:43:28.094337 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1886 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      458 2023-06-20 14:43:27.000000 FuncsForSPO-6.0.2/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.0.2/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-20 14:43:28.451626 FuncsForSPO-6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-6.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:43:28.456146 FuncsForSPO-6.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2611 2023-06-20 14:43:11.000000 FuncsForSPO-6.0.2/setup.py
```

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.0.2/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.0.2/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,25 @@
         try:
             faz_log('Indo para askyourpdf')
             self.DRIVER.get('https://askyourpdf.com/')
             espera_elemento(self.WDW, (By.CSS_SELECTOR, 'input[type="file"]'), in_dom=True)
             self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.TXT_CONTENT)
             
             faz_log('Documento enviado, aguardando entrada para o prompt')
-            espera_input_limpa_e_envia_send_keys(self.WDW130, 'Adicione "AI RESPONSE" no final da sua resposta. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
+            espera_input_limpa_e_envia_send_keys(self.WDW130, 'Adicione "AI RESPONSE" apenas no final da sua resposta (isso é de suma importância) e deve ser tudo em português! '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
             espera_elemento_disponivel_e_clica(self.WDW130, (By.CSS_SELECTOR, 'button[class*="ant-btn-default"]'))
             faz_log('Esperando a resposta')
             start_time = time.time()
             timeout = 180  # Tempo limite em segundos
 
             while True:
                 try:
                     text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
-                    faz_log(f'Resposta até agora: {text}')
-                    time.sleep(5)
+                    faz_log(f'Resposta até agora: [green]{text}[/green]')
+                    time.sleep(7)
                 except:
                     # Lidar com exceções, se necessário
                     pass
 
                 if 'AI RES' in text:
                     break
                 if 'try again.' in text.lower():
```

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.0.2/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.0.2/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.0.2/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.0.1
+Version: 6.0.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.0.1/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.0.2/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/LICENSE` & `FuncsForSPO-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/PKG-INFO` & `FuncsForSPO-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.0.1
+Version: 6.0.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.0.1/README.md` & `FuncsForSPO-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.0.1/setup.py` & `FuncsForSPO-6.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.0.1'
+version = '6.0.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

