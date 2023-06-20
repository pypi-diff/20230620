# Comparing `tmp/featurExtract-0.2.5.5.tar.gz` & `tmp/featurExtract-0.2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/featurExtract-0.2.5.5.tar", last modified: Fri Jun  9 09:48:48 2023, max compression
+gzip compressed data, was "dist/featurExtract-0.2.5.6.tar", last modified: Tue Jun 20 08:00:30 2023, max compression
```

## Comparing `featurExtract-0.2.5.5.tar` & `featurExtract-0.2.5.6.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/
--rw-r--r--   0 zhusitao   (501) staff       (20)       18 2021-08-20 08:13:20.000000 featurExtract-0.2.5.5/MANIFEST.in
--rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/PKG-INFO
--rw-r--r--   0 zhusitao   (501) staff       (20)     3117 2022-08-04 14:50:42.000000 featurExtract-0.2.5.5/README.md
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/
--rw-r--r--   0 zhusitao   (501) staff       (20)      248 2021-07-22 09:50:56.000000 featurExtract-0.2.5.5/featurExtract/__init__.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      272 2021-12-19 03:41:05.000000 featurExtract-0.2.5.5/featurExtract/a.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1928 2021-08-20 07:44:38.000000 featurExtract-0.2.5.5/featurExtract/command_gb.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     2364 2021-08-24 01:51:44.000000 featurExtract-0.2.5.5/featurExtract/command_gff.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/commands/
--rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 09:48:06.000000 featurExtract-0.2.5.5/featurExtract/commands/__init__.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     8178 2023-06-09 09:32:14.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_CDS.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     4655 2022-08-10 09:02:03.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_IGR.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5057 2023-06-09 09:12:54.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_UTR.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    13110 2022-07-12 14:15:50.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_cdna.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    15336 2022-07-14 03:54:00.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_dORF.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     4035 2022-07-14 04:14:36.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_exon.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3353 2022-07-14 04:20:57.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_gene.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3342 2022-07-14 06:23:32.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_intron.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     7533 2022-07-14 06:48:00.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_mRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5160 2022-07-14 07:14:56.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_promoter.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1361 2021-08-20 09:54:37.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_rRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1360 2021-08-20 09:54:58.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_tRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5576 2022-07-14 07:30:41.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_terminator.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    31030 2023-06-09 08:49:48.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_uORF.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    33238 2023-06-09 02:52:54.000000 featurExtract-0.2.5.5/featurExtract/commands/extract_uORF_back.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/database/
--rwxr-xr-x   0 zhusitao   (501) staff       (20)      572 2021-07-22 09:50:56.000000 featurExtract-0.2.5.5/featurExtract/database/database.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    17546 2023-06-09 09:39:26.000000 featurExtract-0.2.5.5/featurExtract/feature_extract.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     7561 2021-08-20 07:50:44.000000 featurExtract-0.2.5.5/featurExtract/genBank_extract.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3152 2021-07-22 09:50:56.000000 featurExtract-0.2.5.5/featurExtract/parameter.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract/utils/
--rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 03:25:23.000000 featurExtract-0.2.5.5/featurExtract/utils/__init__.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      125 2021-08-20 09:23:21.000000 featurExtract-0.2.5.5/featurExtract/utils/coverage.py
--rw-r--r--   0 zhusitao   (501) staff       (20)     2326 2021-08-20 03:52:32.000000 featurExtract-0.2.5.5/featurExtract/utils/util.py
--rw-r--r--   0 zhusitao   (501) staff       (20)    16564 2022-09-16 07:58:22.000000 featurExtract-0.2.5.5/featurExtract/utils/visualize.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)       24 2023-06-09 09:48:33.000000 featurExtract-0.2.5.5/featurExtract/version.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/featurExtract.egg-info/
--rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/PKG-INFO
--rw-r--r--   0 zhusitao   (501) staff       (20)     1268 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/SOURCES.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)        1 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/dependency_links.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)      113 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/entry_points.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       80 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/requires.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       14 2023-06-09 09:48:47.000000 featurExtract-0.2.5.5/featurExtract.egg-info/top_level.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       38 2023-06-09 09:48:48.000000 featurExtract-0.2.5.5/setup.cfg
--rw-r--r--   0 zhusitao   (501) staff       (20)     1283 2021-08-20 10:06:18.000000 featurExtract-0.2.5.5/setup.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/
+-rw-r--r--   0 zhusitao   (501) staff       (20)       18 2021-08-20 08:13:20.000000 featurExtract-0.2.5.6/MANIFEST.in
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/PKG-INFO
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3117 2022-08-04 14:50:42.000000 featurExtract-0.2.5.6/README.md
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/
+-rw-r--r--   0 zhusitao   (501) staff       (20)      248 2021-07-22 09:50:56.000000 featurExtract-0.2.5.6/featurExtract/__init__.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      272 2021-12-19 03:41:05.000000 featurExtract-0.2.5.6/featurExtract/a.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      690 2023-06-15 02:49:42.000000 featurExtract-0.2.5.6/featurExtract/b.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      439 2023-06-15 02:52:56.000000 featurExtract-0.2.5.6/featurExtract/c.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1928 2021-08-20 07:44:38.000000 featurExtract-0.2.5.6/featurExtract/command_gb.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     2364 2021-08-24 01:51:44.000000 featurExtract-0.2.5.6/featurExtract/command_gff.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/commands/
+-rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 09:48:06.000000 featurExtract-0.2.5.6/featurExtract/commands/__init__.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     8211 2023-06-09 11:34:14.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_CDS.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     4655 2022-08-10 09:02:03.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_IGR.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     5090 2023-06-09 11:30:09.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_UTR.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    13110 2022-07-12 14:15:50.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_cdna.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    15340 2023-06-20 06:45:18.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_dORF.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     4035 2022-07-14 04:14:36.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_exon.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3353 2022-07-14 04:20:57.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_gene.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3342 2022-07-14 06:23:32.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_intron.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     7533 2022-07-14 06:48:00.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_mRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     5160 2022-07-14 07:14:56.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_promoter.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1361 2021-08-20 09:54:37.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_rRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1360 2021-08-20 09:54:58.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_tRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     5576 2022-07-14 07:30:41.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_terminator.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    28563 2023-06-20 06:50:08.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_uORF.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    32658 2023-06-15 02:27:15.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_uORF_back.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/database/
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)      572 2021-07-22 09:50:56.000000 featurExtract-0.2.5.6/featurExtract/database/database.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    18014 2023-06-20 02:34:25.000000 featurExtract-0.2.5.6/featurExtract/feature_extract.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     7561 2021-08-20 07:50:44.000000 featurExtract-0.2.5.6/featurExtract/genBank_extract.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3152 2021-07-22 09:50:56.000000 featurExtract-0.2.5.6/featurExtract/parameter.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/utils/
+-rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 03:25:23.000000 featurExtract-0.2.5.6/featurExtract/utils/__init__.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      125 2021-08-20 09:23:21.000000 featurExtract-0.2.5.6/featurExtract/utils/coverage.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)     2326 2021-08-20 03:52:32.000000 featurExtract-0.2.5.6/featurExtract/utils/util.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)    16597 2023-06-20 06:34:08.000000 featurExtract-0.2.5.6/featurExtract/utils/visualize.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)       24 2023-06-20 07:59:58.000000 featurExtract-0.2.5.6/featurExtract/version.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/PKG-INFO
+-rw-r--r--   0 zhusitao   (501) staff       (20)     1306 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/SOURCES.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)        1 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/dependency_links.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)      113 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/entry_points.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       80 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/requires.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       14 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/top_level.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       38 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/setup.cfg
+-rw-r--r--   0 zhusitao   (501) staff       (20)     1283 2021-08-20 10:06:18.000000 featurExtract-0.2.5.6/setup.py
```

### Comparing `featurExtract-0.2.5.5/PKG-INFO` & `featurExtract-0.2.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurExtract
-Version: 0.2.5.5
+Version: 0.2.5.6
 Summary: Extract genome ferature sequence for biologists
 Home-page: https://github.com/SitaoZ/featurExtract.git
 Author: zhusitao
 Author-email: zhusitao1990@163.com
 License: MIT
 Keywords: genome feature,extract
 Platform: UNKNOWN
```

### Comparing `featurExtract-0.2.5.5/README.md` & `featurExtract-0.2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/command_gb.py` & `featurExtract-0.2.5.6/featurExtract/command_gb.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/command_gff.py` & `featurExtract-0.2.5.6/featurExtract/command_gff.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_CDS.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_CDS.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,25 @@
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     '''
     # print(args)
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
+    feature_types = db.featuretypes()
     # dict
     cds_seq_list = deque()
     # cds_seq = pd.DataFrame(columns=['TranscriptID','Chrom','Start','End','Strand','CDS'])
     cds_record = deque()
     index = 0
     # assert GTF or GFF
     if args.rna_feature == 'mRNA':
         mRNA_str = mRNA_type(args.style)
     else:
-        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     # loop all transcript in genome
     if not args.transcript:
         for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
                                    total = len(list(db.features_of_type(mRNA_str, order_by='start'))),\
                                    ncols = 80, desc="CDS Processing :"):
             seq = ''
             cds_start_transcript = 0
```

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_IGR.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_IGR.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_UTR.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_UTR.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     '''
     parameters:
         args: parse from argparse
     return:
         file write to file or stdout
     '''
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
+    feature_types = db.featuretypes()
     # header
     # utr_seq = pd.DataFrame(columns=_CSV_HEADER)
     # dist fastest way 
     utr_seq_list = deque()
     # mRNA_str = mRNA_type(args.style)
     if args.rna_feature == 'mRNA':
         mRNA_str = mRNA_type(args.style)
     else:
-        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     utr3_t = utr3_type(args.style)
     utr5_t = utr5_type(args.style)
     if not args.transcript:
         # all UTR in genome 
         index = 0
         for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
                       total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
```

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_cdna.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_cdna.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_dORF.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_dORF.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
 from tqdm import tqdm 
 from Bio.Seq import Seq
-from collections import defaultdict
+from multiprocessing import Pool
+from collections import defaultdict, deque
 from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
 from featurExtract.utils.util import stop_codon_seq, add_stop_codon 
 from featurExtract.commands.extract_uORF import GFF
 from featurExtract.utils.visualize import visual_transcript, visual_transcript_genome
 
 # table header 
 _dORF_csv_header = ['TranscriptID', 'Chrom', 'Strand', \
-                    'CDS Interval', 'uORF Start', 'uORF End', \
-                    'uORF Type', 'uORF Length', 'uORF']
+                    'CDS Interval', 'dORF Start', 'dORF End', \
+                    'dORF Type', 'dORF Length', 'dORF']
 
 
 
 class dORF(object):
     """dORF finder using object-oriented
     Attributes:
         transcript_id (str): transcript id
@@ -25,16 +26,17 @@
         strand (str): transcript strand 
         matural_transcript (Seq of Biopython): matural transcript sequence
         coding_sequence (Seq of Biopython): conding sequence of specifity transcript 
     """
     START_CODON = 'ATG'
     STOP_CODON_LIST = ['TAA','TAG','TGA']
     
-    def __init__(self, transcript_id, chrom, strand, matural_transcript, coding_sequence):
+    def __init__(self, transcript_id, length, chrom, strand, matural_transcript, coding_sequence):
         self.t_id = transcript_id
+        self.length = length
         self.chrom = chrom
         self.strand = strand 
         self.mt = matural_transcript
         self.cds = coding_sequence
     def transcript_location(self):
         """Transcript start and end
         1D list regradless of strand  
@@ -53,14 +55,16 @@
         """Extract dorfs start and end in transcript
         2D list regardless strand 
         """
         d2 = []
         dORF_dict = self.dorf_parse()
         for dorf_type in dORF_dict.keys():
             for it in dORF_dict[dorf_type]:
+                if len(it[8]) <= self.length:
+                    continue
                 dorf_start, dorf_end = it[4], it[5]
                 d2.append([dorf_start, dorf_end])
         return d2
     def dorf_parse(self):
         """ dORF parse"""
         dORF_dict = defaultdict(list)
         # start_codon means the first base position in matural_transcript
@@ -76,25 +80,24 @@
         utr3_len = len(utr3)
         for i in range(0, utr3_len-3):
             # start codon find 
             if utr3[i:i+3] == dORF.START_CODON:
                 for j in range(i+3, utr3_len, 3):
                 # stop codon find
                     if utr3[j:j+3] in dORF.STOP_CODON_LIST:
-                        # type1 uORF  upstream; not unique 
                         dorf = utr3[i:j+3]
                         out1 = [self.t_id, self.chrom, self.strand, cds_intervel, stop_codon+i+1, stop_codon+j+3, 'dORF', len(dorf), dorf]
                         if not dORF_dict.get('dORF'):
                             dORF_dict['dORF'] = [out1]
                         else:
                             dORF_dict['dORF'].append(out1)
                         break
         return dORF_dict
      
-def uorf_procedure_oriented(transcript_id, chrom, strand, matural_transcript, coding_sequence):
+def dorf_procedure_oriented(transcript_id, chrom, strand, matural_transcript, coding_sequence):
     """
     Parameters:
         transcript_id:      transcript id
         matural_transcript: a Seq type (Biopython) from mature transcript without intron
         coding_sequence:    a Seq type (Biopython) from coding sequence start with ATG , 
                          end with TAA, TGA, TAG
     Return:
@@ -115,199 +118,219 @@
     utr3_len = len(utr3)
     for i in range(0, utr3_len-3):
         # start codon find 
         if utr3[i:i+3] == "ATG":
             for j in range(i+3, utr3_len, 3):
             # stop codon find
                 if utr3[j:j+3] in stop_codon_list:
-                    # type1 uORF  upstream; not unique 
                     dORF = utr3[i:j+3]
                     out1 = [transcript_id, chrom, strand, cds_intervel, stop_codon+i+1, stop_codon+j+3, 'dORF', len(dORF), dORF]
                     if not dORF_dict.get('dORF'):
                         dORF_dict['dORF'] = [out1]
                     else:
                         dORF_dict['dORF'].append(out1)
                     break 
     return dORF_dict
 
 
 
+def get_mt_cds_seq(t, db, genome, style):
+    """
+    parameters:
+        args:  
+    """
+    # primary transcript (pt) 是基因组上的转录本的序列，
+    # 有的会包括intron，所以提取的序列和matural transcript (mt) 不一致
+    # pt = t.sequence(genome, use_strand=True)
+    # matural transcript (mt)
+    # 该步骤是获取序列: 转录本序列，CDS序列, five_prime_UTR, three_prime_UTR
+    # 但是有的基因注释不正确，导致成熟转录本序列的两个来源不一致，一个是exon来源的，一个是five_prime_UTR和CDS来源的
+    # 针对这种请情况，我们使用 five_prime_UTR + CDS + three_prime_UTR 拼接形成成熟的转录本序列用于uORF/dORF的注释
+    # exon 提取的是转录本内成熟的mRNA的序列,即外显子按基因组坐标首尾相连的matural transcript
+    mt, cds = '', ''
+    exons_list = []
+    for e in db.children(t, featuretype='exon', order_by='start'):
+        exons_list.append((e.start, e.end))
+        mt += e.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+    mt = Seq(mt)
+    if t.strand == '-':
+        mt = mt.reverse_complement()
+    # CDS 提取的是编码区 ATG ... TAG
+    cds_list = []
+    for c in db.children(t, featuretype='CDS', order_by='start'):
+        cds_list.append((c.start, c.end))
+        cds += c.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+    if style == 'GTF':
+        sc_seq = stop_codon_seq(db, t, genome)
+        cds = add_stop_codon(cds, t.strand, sc_seq)
+    cds = Seq(cds)
+    ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
+    # mt from utr5/3 and cds
+    mt_from_utr_cds = ''
+    for e in db.children(t, featuretype=['five_prime_UTR', 'CDS', 'three_prime_UTR'], order_by='start'):
+        mt_from_utr_cds += e.sequence(genome, use_strand=False)
+    mt_from_utr_cds = Seq(mt_from_utr_cds)
+    if t.strand == '-':
+        mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
+    if mt != mt_from_utr_cds:
+        mt = mt_from_utr_cds
+        # error_count += 1
+    if t.strand == '-':
+        cds = cds.reverse_complement()
+    return mt, cds, exons_list, cds_list
+
+
+def dorf_filter_output(params):
+    t, database, genome, style, length, output_format = params
+    db = gffutils.FeatureDB(database, keep_order=True)
+    index = 0
+    dORF_seq_list = deque()
+    # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
+    mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, genome, style)
+    # objected-oriented
+    if mt == cds: # not contain dORF
+        return
+    if len(cds) % 3 != 0: # CDS error
+        return
+    dORF_ = dORF(t.id, length, t.chrom, t.strand, mt, cds)
+    dORF_dict = dORF_.dorf_parse()
+    if len(dORF_dict) == 0: # CDS error
+        return
+    # loop for type1, type2 and type3
+    for key in sorted(dORF_dict.keys()):
+        # print(key,len(dORF_dict[key]))
+        for it in dORF_dict[key]:
+            # dORF length filter 
+            if len(it[8]) <= length:
+                # default: 6
+                continue
+            # csv output format 
+            if output_format == 'csv':
+                # dORF_seq.loc[index] = it
+                # dict 
+                dORF_seq_list.append(dict(zip(_dORF_csv_header, it)))
+                index += 1
+            elif output_format == 'fasta':
+                uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
+                seq = it[8] # it[8] is s Seq type
+                desc='strand:%s dORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
+                                                              it[4],
+                                                              it[5],
+                                                              it[6],
+                                                              len(seq),
+                                                              it[3].split('-')[0],
+                                                              it[3].split('-')[1])
+                uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
+                dORF_seq_list.append(uorfRecord)
+
+            elif output_format == 'gff':
+                gff = GFF(exons_list, it, 'dORF')
+                uorf_gff_line,features_gff_lines = gff.parse()
+                # print(uorf_gff_line)
+                # dORF_gff.write(uorf_gff_line+"\n")
+                dORF_seq_list.append(uorf_gff_line)
+                for feature_line in features_gff_lines:
+                    # print(feature_line)
+                    dORF_seq_list.append(feature_line)
+                    # dORF_gff.write(feature_line+"\n")
+            else:
+                # csv output_format
+                dORF_seq_list.append(dict(zip(_dORF_csv_header, it)))
+                index += 1
+    return dORF_seq_list
+
 
 def get_dorf(args):
     """
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout 
     """
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
-    # csv
-    # dORF_seq = pd.DataFrame(columns=_dORF_csv_header)
-    dORF_seq_list = []
-    # gff
-    dORF_gff = open(args.output,'w')
-    # fasta
-    dorf_record = []
-
-    mRNA_str = mRNA_type(args.style)
-    index = 0
+    feature_types = db.featuretypes()
+    if args.rna_feature == 'mRNA':
+        mRNA_str = mRNA_type(args.style)
+    else:
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
+    error_count = 0
+    total_transcript_number = len(list(db.features_of_type(mRNA_str, order_by='start')))
+    # loop all transcripts in genome
     if not args.transcript:
-        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
-                      ncols = 80, desc = "dORF Processing:"):
-            # primary transcript (pt) 是基因组上的转录本的序列，
-            # 有的会包括intron，所以提取的序列和matural transcript 不一致
-            # print(t)
-            pt = t.sequence(args.genome, use_strand=True)
-            # matural transcript (mt)
-            # exon 提取的是转录本内成熟的MRNA的序列,即外显子收尾相连的matural transcript
-            mt = ''
-            exons_list = []
-            for e in db.children(t, featuretype='exon', order_by='start'):
-                exons_list.append([e.start, e.end])
-                s = e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                mt += s
-            mt = Seq(mt)
-            if t.strand == '-':
-                mt = mt.reverse_complement()
-            # CDS 提取的是编码区 ATG ... TAG
-            cds = ''
-            for c in db.children(t, featuretype='CDS', order_by='start'):
-                # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                s = c.sequence(args.genome, use_strand=False)
-                cds += s
-            if args.style == 'GTF':
-                sc_seq = stop_codon_seq(db, t, args.genome)
-                cds = add_stop_codon(cds, t.strand, sc_seq)
-            cds = Seq(cds)
-            if t.strand == '-':
-                cds = cds.reverse_complement()
-            dORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
-            # loop all dORF
-            for key in sorted(dORF_dict.keys()):
-                for it in dORF_dict[key]:
-                    # csv output format 
-                    if args.output_format == 'csv':
-                        # dORF_seq.loc[index] = it
-                        # index += 1
-                        dORF_seq_list.append(dict((_dORF_csv_header[i],it[i]) for i in range(len(_dORF_csv_header))))
-                    elif args.output_format == 'fasta':
-                        dorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
-                        seq = it[8] # it[8] is a Seq type
-                        desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
-                                                                        it[4],
-                                                                        it[5],
-                                                                        it[6],
-                                                                        len(seq),
-                                                                        it[3].split('-')[0],
-                                                                        it[3].split('-')[1])
-                        dorfRecord = SeqRecord(seq, id=dorf_id.replace('transcript:',''), description=desc)
-                        dorf_record.append(dorfRecord)
-                    elif args.output_format == 'gff':
-                        gff = GFF(exons_list, it, 'dORF')
-                        dorf_gff_line,features_gff_lines = gff.parse()
-                        ex_locations = gff.uorf_exons_location()
-                        dORF_gff.write(dorf_gff_line+"\n")
-                        for feature_line in features_gff_lines:
-                            dORF_gff.write(feature_line+"\n")
+        param_list = [(t, args.database, args.genome, args.style, args.length, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
+        print('length :', len(param_list))
+        with Pool(processes=args.process) as p:
+            dORF_seq_list = list(tqdm(p.imap(dorf_filter_output, param_list), total=len(param_list), desc='dORF Processing:'))
+        dORF_seq_list = [d for de in dORF_seq_list if de != None for d in de]
+        # output file 
         if args.output_format == 'csv':
             dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
             dORF_seq.to_csv(args.output, sep=',', index=False)
         elif args.output_format == 'gff':
-            dORF_gff.close()
+            with open(args.output,'w') as handle:
+                for record in dORF_seq_list:
+                    handle.write(record+'\n')
         elif args.output_format == 'fasta':
             with open(args.output,'w') as handle:
-                SeqIO.write(uorf_record, handle, "fasta")
+                SeqIO.write(dORF_seq_list, handle, "fasta")
+        else:
+            dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
+            dORF_seq.to_csv(args.output, sep=',', index=False)
     else:
+        # specify the transcript id; only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             # primary transcript (pt) 是基因组上的转录本的序列，
             # 有的会包括intron，所以提取的序列和matural transcript 不一致
-            # print(t)
+            # id specify
             if args.transcript in t.id:
-                pt = t.sequence(args.genome, use_strand=True)
-                # matural transcript (mt)
-                # exon 提取的是转录本内成熟的MRNA的序列,即外显子收尾相连的matural transcript
-                mt = ''
-                exons_list = []
-                for e in db.children(t, featuretype='exon', order_by='start'):
-                    exons_list.append([e.start, e.end])
-                    s = e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                    mt += s
-                mt = Seq(mt)
-                if t.strand == '-':
-                    mt = mt.reverse_complement()
-                # CDS 提取的是编码区 ATG ... TAG
-                cds = ''
-                cds_list = []
-                for c in db.children(t, featuretype='CDS', order_by='start'):
-                    # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                    cds_list.append([c.start, c.end])
-                    s = c.sequence(args.genome, use_strand=False)
-                    cds += s
-                if args.style == 'GTF':
-                    sc_seq = stop_codon_seq(db, t, args.genome)
-                    cds = add_stop_codon(cds, t.strand, sc_seq)
-                cds = Seq(cds)
-                if t.strand == '-':
-                    cds = cds.reverse_complement()
-                # precodure-oriented
-                # dORF_dict = dorf(t.id, t.chrom, t.strand, mt, cds)
-                dORF_ = dORF(t.id, t.chrom, t.strand, mt, cds)
+                params = (t, args.database, args.genome, args.style, args.length, args.output_format)
+                dORF_seq_list = dorf_filter_output(params)
+                mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, args.genome, args.style)
+                print(args)
+                dORF_ = dORF(t.id, args.length, t.chrom, t.strand, mt, cds)
                 dORF_dict = dORF_.dorf_parse()
                 dorf_location_genome = [] # for schematic on genome # 3D list 
                 for key in sorted(dORF_dict.keys()):
                     for it in dORF_dict[key]:
-                        # csv output format 
-                        if args.output_format == 'csv':
-                            # dORF_seq.loc[index] = it
-                            # index += 1
-                            dORF_seq_list.append(dict((_dORF_csv_header[i],it[i]) for i in range(len(_dORF_csv_header))))
-                        elif args.output_format == 'fasta':
-                            dorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
-                            seq = it[8] # it[8] is a Seq type
-                            desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
-                                                                        it[4],
-                                                                        it[5],
-                                                                        it[6],
-                                                                        len(seq),
-                                                                        it[3].split('-')[0],
-                                                                        it[3].split('-')[1])
-                            dorfRecord = SeqRecord(seq, id=dorf_id.replace('transcript:',''), description=desc)
-                            dorf_record.append(dorfRecord)
-                        elif args.output_format == 'gff':
-                            gff = GFF(exons_list, it, 'dORF')
-                            dorf_gff_line,features_gff_lines = gff.parse()
-                            ex_locations = gff.uorf_exons_location()
-                            dorf_location_genome.append(ex_locations) # for schematic on genome
-                            dORF_gff.write(dorf_gff_line+"\n")
-                            for feature_line in features_gff_lines:
-                                dORF_gff.write(feature_line+"\n")
+                        # dORF length filter 
+                        if len(it[8]) <= args.length:
+                            # default: 6
+                            continue
+                        # for schematic on genome
+                        gff = GFF(exons_list, it, 'dORF')
+                        ex_locations = gff.uorf_exons_location()
+                        dorf_location_genome.append(ex_locations)
                 # figure the schametic 
-                # without intron 
+                # without intron / -m 
                 if args.schematic_without_intron:
                     figure = visual_transcript(args.schematic_without_intron,
                                                args.transcript,
                                                dORF_.transcript_location(),
                                                dORF_.cds_location_transcript(),
                                                dORF_.dorf_location_transcript(),
                                                'dORF')
                     figure.draw()
-                # with intron
+                # with intron / -n 
                 if args.schematic_with_intron:
                     figure = visual_transcript_genome(t.strand,
                                                       args.schematic_with_intron,
                                                       args.transcript,
                                                       exons_list,
                                                       cds_list,
                                                       dorf_location_genome,# 3D list 
                                                       'dORF')
                     figure.draw()
-                
+                # file out
                 if args.output_format == 'csv':
                     dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
                     dORF_seq.to_csv(args.output, sep=',', index=False)
                 elif args.output_format == 'gff':
-                    dORF_gff.close()
+                    with open(args.output,'w') as handle:
+                        for record in dORF_seq_list:
+                            handle.write(record+'\n')
                 elif args.output_format == 'fasta':
                     with open(args.output,'w') as handle:
-                        SeqIO.write(uorf_record, handle, "fasta")
-                break 
+                        SeqIO.write(dORF_seq_list, handle, "fasta")
+                else:
+                    dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
+                    dORF_seq.to_csv(args.output, sep=',', index=False)
+                break
```

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_exon.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_exon.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_gene.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_gene.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_intron.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_intron.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_mRNA.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_mRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_promoter.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_promoter.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_rRNA.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_rRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_tRNA.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_tRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_terminator.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_terminator.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_uORF.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_uORF.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
-import multiprocessing
+from multiprocessing import Pool
+from multiprocessing import get_context
 from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from collections import defaultdict, deque
+from concurrent.futures import ProcessPoolExecutor
 from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
 from featurExtract.utils.util import stop_codon_seq, add_stop_codon
 from featurExtract.utils.visualize import visual_transcript, visual_transcript_genome
 
 # table header 
 _uORF_csv_header = ['TranscriptID', 'Chrom', 'Strand', 
                     'CDS Interval', 'uORF Start', 'uORF End', 
@@ -384,34 +386,33 @@
 def get_mt_cds_seq(t, db, genome, style):
     """
     parameters:
         args:  
     """
     # primary transcript (pt) 是基因组上的转录本的序列，
     # 有的会包括intron，所以提取的序列和matural transcript (mt) 不一致
-    pt = t.sequence(genome, use_strand=True)
+    # pt = t.sequence(genome, use_strand=True)
     # matural transcript (mt)
     # 该步骤是获取序列: 转录本序列，CDS序列, five_prime_UTR, three_prime_UTR
     # 但是有的基因注释不正确，导致成熟转录本序列的两个来源不一致，一个是exon来源的，一个是five_prime_UTR和CDS来源的
     # 针对这种请情况，我们使用 five_prime_UTR + CDS + three_prime_UTR 拼接形成成熟的转录本序列用于uORF的注释
     # exon 提取的是转录本内成熟的mRNA的序列,即外显子按基因组坐标首尾相连的matural transcript
-    mt = ''
+    mt, cds = '', ''
     exons_list = []
     for e in db.children(t, featuretype='exon', order_by='start'):
         exons_list.append((e.start, e.end))
-        s = e.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-        mt += s
+        mt += e.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
     mt = Seq(mt)
     if t.strand == '-':
         mt = mt.reverse_complement()
     # CDS 提取的是编码区 ATG ... TAG
-    cds = ''
+    cds_list = []
     for c in db.children(t, featuretype='CDS', order_by='start'):
-        s = c.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-        cds += s
+        cds_list.append((c.start, c.end))
+        cds += c.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
     if style == 'GTF':
         sc_seq = stop_codon_seq(db, t, genome)
         cds = add_stop_codon(cds, t.strand, sc_seq)
     cds = Seq(cds)
     ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
     # mt from utr5/3 and cds
     mt_from_utr_cds = ''
@@ -421,204 +422,173 @@
     if t.strand == '-':
         mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
     if mt != mt_from_utr_cds:
         mt = mt_from_utr_cds
         # error_count += 1
     if t.strand == '-':
         cds = cds.reverse_complement()
-    return mt, cds, exons_list
+    return mt, cds, exons_list, cds_list
     
+def uorf_filter_output(params):
+    t, database, genome, style, length, output_format = params
+    db = gffutils.FeatureDB(database, keep_order=True)
+    index = 0 
+    uORF_seq_list = deque()
+    # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
+    mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, genome, style)
+    # objected-oriented
+    if mt == cds: # not contain uORF
+        return 
+    if len(cds) % 3 != 0: # CDS error
+        return 
+    uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
+    uORF_dict = uORF_.uorf_parse()
+    if len(uORF_dict) == 0: # CDS error
+        return 
+    # loop for type1, type2 and type3
+    for key in sorted(uORF_dict.keys()):
+        # print(key,len(uORF_dict[key]))
+        for it in uORF_dict[key]:
+            # uORF length filter 
+            if len(it[8]) <= length:
+                # default: 6
+                continue
+            # csv output format 
+            if output_format == 'csv':
+                # uORF_seq.loc[index] = it
+                # dict 
+                uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
+                index += 1
+            elif output_format == 'fasta':
+                uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
+                seq = it[8] # it[8] is s Seq type
+                desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
+                                                              it[4],
+                                                              it[5],
+                                                              it[6],
+                                                              len(seq),
+                                                              it[3].split('-')[0],
+                                                              it[3].split('-')[1])
+                uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
+                uORF_seq_list.append(uorfRecord)
+
+            elif output_format == 'gff':
+                gff = GFF(exons_list, it, 'uORF')
+                uorf_gff_line,features_gff_lines = gff.parse()
+                # print(uorf_gff_line)
+                # uORF_gff.write(uorf_gff_line+"\n")
+                uORF_seq_list.append(uorf_gff_line)
+                for feature_line in features_gff_lines:
+                    # print(feature_line)
+                    uORF_seq_list.append(feature_line)
+                    # uORF_gff.write(feature_line+"\n")
+            else:
+                # csv output_format
+                uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
+                index += 1
+    return uORF_seq_list
+
 
 def get_uorf(args):
     """ Get uORF main command line entry
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     """
     db = gffutils.FeatureDB(args.database, keep_order=True)
+    feature_types = db.featuretypes()
     # csv
     # uORF_seq = pd.DataFrame(columns=_uORF_csv_header)
     # uORF_seq_list = []
-    uORF_seq_list = deque()
-    # gff
-    uORF_gff = open(args.output,'w')
+    # uORF_seq_list = deque()
     # fasta
-    # uorf_record = []
     uorf_record = deque()
-    index = 0
+    # gff 
+    uorf_gff_record = deque()
+    # index = 0
     if args.rna_feature == 'mRNA':
         mRNA_str = mRNA_type(args.style)
     else:
-        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     error_count = 0
+    total_transcript_number = len(list(db.features_of_type(mRNA_str, order_by='start')))
     # loop all transcripts in genome
     if not args.transcript:
-        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
-                      ncols = 80, desc = "uORF Processing :"):
-            # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
-            mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
-            # procedure-oriented
-            # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
-            # objected-oriented
-            if mt == cds: # not contain uORF
-                continue
-            if len(cds) % 3 != 0: # CDS error
-                continue
-            uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
-            uORF_dict = uORF_.uorf_parse()
-            if len(uORF_dict) == 0: # CDS error
-                continue
-            # loop for type1, type2 and type3
-            for key in sorted(uORF_dict.keys()):
-                # print(key,len(uORF_dict[key]))
-                for it in uORF_dict[key]:
-                    # uORF length filter 
-                    if len(it[8]) <= args.length:
-                        # default: 6
-                        continue
-                    # csv output format 
-                    if args.output_format == 'csv':
-                        # uORF_seq.loc[index] = it
-                        # dict 
-                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
-                        index += 1
-                    elif args.output_format == 'fasta':
-                        uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
-                        seq = it[8] # it[8] is s Seq type
-                        desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
-                                                                      it[4],
-                                                                      it[5],
-                                                                      it[6],
-                                                                      len(seq),
-                                                                      it[3].split('-')[0],
-                                                                      it[3].split('-')[1])
-                        uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
-                        uorf_record.append(uorfRecord)
-                        
-                    elif args.output_format == 'gff':
-                        gff = GFF(exons_list, it, 'uORF')
-                        uorf_gff_line,features_gff_lines = gff.parse() 
-                        # print(uorf_gff_line)
-                        uORF_gff.write(uorf_gff_line+"\n") 
-                        for feature_line in features_gff_lines:
-                            # print(feature_line)
-                            uORF_gff.write(feature_line+"\n")
-                    else:
-                        # csv output_format
-                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
-                        index += 1 
+        param_list = [(t, args.database, args.genome, args.style, args.length, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
+        print('length :', len(param_list))
+        with Pool(processes=args.process) as p:
+            uORF_seq_list = list(tqdm(p.imap(uorf_filter_output, param_list), total=len(param_list), desc='多进程提取uORF:'))
+        uORF_seq_list = [d for de in uORF_seq_list if de != None for d in de]
         # output file 
         if args.output_format == 'csv':
             uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
             uORF_seq.to_csv(args.output, sep=',', index=False)
         elif args.output_format == 'gff':
-            uORF_gff.close()
+            with open(args.output,'w') as handle:
+                for record in uORF_seq_list:
+                    handle.write(record+'\n')
         elif args.output_format == 'fasta':
             with open(args.output,'w') as handle:
-                SeqIO.write(uorf_record, handle, "fasta")
+                SeqIO.write(uORF_seq_list, handle, "fasta")
         else:
             uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
             uORF_seq.to_csv(args.output, sep=',', index=False)
     else:
-        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
         # specify the transcript id; only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             # primary transcript (pt) 是基因组上的转录本的序列，
             # 有的会包括intron，所以提取的序列和matural transcript 不一致
             # id specify
             if args.transcript in t.id:
-                mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
-                # procedure-oriented 
-                # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
-                # objected-oriented
-                if mt == cds:  # not contain uORF
-                    continue
-                if len(cds) % 3 != 0: # CDS error
-                    continue
+                params = (t, args.database, args.genome, args.style, args.length, args.output_format)
+                uORF_seq_list = uorf_filter_output(params)
+                mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, args.genome, args.style)
                 uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
+                print(args)
+                # figure the schametic 
                 uORF_dict = uORF_.uorf_parse()
-                if len(uORF_dict) == 0:  # CDS error
-                    continue
                 uorf_location_genome = [] # for schematic on genome # 3D list 
                 for key in sorted(uORF_dict.keys()):
-                    # print(key,len(uORF_dict[key]))
                     for it in uORF_dict[key]:
                         # uORF length filter 
                         if len(it[8]) <= args.length:
                             # default: 6
                             continue
-                        # csv output format 
-                        if args.output_format == 'csv':
-                            # uORF_seq.loc[index] = it
-                            # dict is fastest way 
-                            uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
-                            index += 1
-                            # for schematic on genome
-                            gff = GFF(exons_list, it, 'uORF')
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations)
-                        elif args.output_format == 'fasta':
-                            uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
-                            seq = it[8] # it[8] is a Seq type
-                            desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
-                                                                        it[4],
-                                                                        it[5],
-                                                                        it[6],
-                                                                        len(seq),
-                                                                        it[3].split('-')[0],
-                                                                        it[3].split('-')[1])
-                            uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
-                            uorf_record.append(uorfRecord)
-                            # for schematic on genome
-                            gff = GFF(exons_list, it, 'uORF')
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations) 
-                        elif args.output_format == 'gff':
-                            # for schematic on genome
-                            gff = GFF(exons_list, it, 'uORF')
-                            uorf_gff_line,features_gff_lines = gff.parse()
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations) # for schematic on genome
-                            uORF_gff.write(uorf_gff_line+"\n")
-                            for feature_line in features_gff_lines:
-                                uORF_gff.write(feature_line+"\n")
-                        else:
-                            uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
-                            index += 1
-                            gff = GFF(exons_list, it, 'uORF')
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations)
-                # figure the schametic 
+                        # for schematic on genome
+                        gff = GFF(exons_list, it, 'uORF')
+                        ex_locations = gff.uorf_exons_location()
+                        uorf_location_genome.append(ex_locations)
                 # without intron 
-                if args.schematic_without_intron:
+                if args.schematic_without_intron == True:
                     figure = visual_transcript(args.schematic_without_intron, 
                                                args.transcript, 
                                                uORF_.transcript_location(),
                                                uORF_.cds_location_transcript(),
                                                uORF_.uorf_location_transcript(),
                                                'uORF')
                     figure.draw()
                 # with intron
-                if args.schematic_with_intron:
+                if args.schematic_with_intron == True:
                     figure = visual_transcript_genome(t.strand, 
                                                       args.schematic_with_intron, 
                                                       args.transcript, 
                                                       exons_list, 
                                                       cds_list,
                                                       uorf_location_genome,# 3D list 
                                                       'uORF')
                     figure.draw() 
                 # file out
                 if args.output_format == 'csv':
                     uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
                     uORF_seq.to_csv(args.output, sep=',', index=False)
                 elif args.output_format == 'gff':
-                    uORF_gff.close()
+                    with open(args.output,'w') as handle:
+                        for record in uORF_seq_list:
+                            handle.write(record+'\n')
                 elif args.output_format == 'fasta':
                     with open(args.output,'w') as handle:
-                        SeqIO.write(uorf_record, handle, "fasta")
+                        SeqIO.write(uORF_seq_list, handle, "fasta")
                 else:
                     uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
                     uORF_seq.to_csv(args.output, sep=',', index=False)
                 break
```

### Comparing `featurExtract-0.2.5.5/featurExtract/commands/extract_uORF_back.py` & `featurExtract-0.2.5.6/featurExtract/commands/extract_uORF_back.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
+import multiprocessing
 from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
-from collections import defaultdict
+from collections import defaultdict, deque
 from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
 from featurExtract.utils.util import stop_codon_seq, add_stop_codon
 from featurExtract.utils.visualize import visual_transcript, visual_transcript_genome
 
 # table header 
 _uORF_csv_header = ['TranscriptID', 'Chrom', 'Strand', 
                     'CDS Interval', 'uORF Start', 'uORF End', 
@@ -105,14 +106,15 @@
                    str(exon[0]), str(exon[1]), ".", self.strand, "0", gff_9_col])
                 gff_lines.append(gff_line)
             return gff_lines
         
 
 class uORF_genome_location(object):
     """A parse for uORF location from transcript map to genome 
+    designed for GFF output format 
     uORF的起始和终止只会位于某一外显子中,锁定外显子后根据相对位置判定真实坐标,
     其中uORF的起始等于它位于的外显子的起始位置+该位置离该exon起始的距离,
     uORF的终止等于它位于的外显子的起始位置+该位置离该exon起始的距离.
     """
     def __init__(self, exons, uorf_start, uorf_end, strand, cds_interval):
         self.exons = exons
         self.uorf_start = uorf_start
@@ -257,15 +259,16 @@
             for it in uORF_dict[uorf_type]:
                 uorf_start, uorf_end = it[4], it[5]
                 d2.append([uorf_start, uorf_end])
         return d2 
         
     def uorf_parse(self):
         """uorf finder main program, return a dict"""
-        uORF_dict = defaultdict(list)
+        # uORF_dict = defaultdict(list)
+        uORF_dict = defaultdict()
         # start_codon_position means the first base position in matural_transcript
         if self.cds not in self.mt:
             return uORF_dict
         start_codon_position = self.mt.index(self.cds)
         # stop_codon_position means the last base position in matural transcript
         stop_codon_position = start_codon_position + len(self.cds)
         # CDS on mt coordinate
@@ -285,36 +288,36 @@
                 # stop codon find
                     if self.mt[j:j+3] in uORF.STOP_CODON_LIST and j < utr5_len:
                         # type1 uORF  upstream; not unique 
                         type1_uORF = self.mt[i:j+3]
                         out1 = [self.transcript_id, self.chrom, self.strand, \
                                 cds_interval, i+1, j+3, 'type1', len(type1_uORF), type1_uORF]
                         if not uORF_dict.get('type1_uORF'):
-                            uORF_dict['type1_uORF'] = [out1]
+                            uORF_dict['type1_uORF'] = deque([out1])
                         else:
                             uORF_dict['type1_uORF'].append(out1)
                         # only use the first stop codon, so break must
                         break
                     if self.mt[j:j+3] in uORF.STOP_CODON_LIST and j + 3 > utr5_len and j + 3 < stop_codon_position:
                         # type2 uORF across; the overlap region is triple or not; not unique
                         type2_uORF = self.mt[i:j+3]
                         out2 = [self.transcript_id, self.chrom, self.strand, \
                                 cds_interval, i+1, j+3, 'type2', len(type2_uORF), type2_uORF]
                         if not uORF_dict.get('type2_uORF'):
-                            uORF_dict['type2_uORF'] = [out2]
+                            uORF_dict['type2_uORF'] = deque([out2])
                         else:
                             uORF_dict['type2_uORF'].append(out2)
                         break
                     if self.mt[j:j+3] in uORF.STOP_CODON_LIST and j + 3 > utr5_len and j+3 == stop_codon_position and (utr5_len - i)%3 == 0:
                         # type3 uORF; N extention 通读; not unique 
                         type3_uORF = self.mt[i:utr5_len+cds_len]
                         out3 = [self.transcript_id, self.chrom, self.strand, \
                                 cds_interval, i+1, j+3, 'type3', len(type3_uORF), type3_uORF]
                         if not uORF_dict.get('type3_uORF'):
-                            uORF_dict['type3_uORF'] = [out3]
+                            uORF_dict['type3_uORF'] = deque([out3])
                         else:
                             uORF_dict['type3_uORF'].append(out3)
                         break
         return uORF_dict
             
 
 
@@ -374,82 +377,116 @@
                         uORF_dict['type3_uORF'] = [out3]
                     else:
                         uORF_dict['type3_uORF'].append(out3)
                     break
     return uORF_dict
 
 
-
-_uORF_csv_header = ['TranscriptID', 'Chrom', 'Strand',
-                    'CDS Interval', 'uORF Start', 'uORF End',
-                    'uORF Type', 'uORF Length', 'uORF']
+def get_mt_cds_seq(t, db, genome, style):
+    """
+    parameters:
+        args:  
+    """
+    # primary transcript (pt) 是基因组上的转录本的序列，
+    # 有的会包括intron，所以提取的序列和matural transcript (mt) 不一致
+    # pt = t.sequence(genome, use_strand=True)
+    # matural transcript (mt)
+    # 该步骤是获取序列: 转录本序列，CDS序列, five_prime_UTR, three_prime_UTR
+    # 但是有的基因注释不正确，导致成熟转录本序列的两个来源不一致，一个是exon来源的，一个是five_prime_UTR和CDS来源的
+    # 针对这种请情况，我们使用 five_prime_UTR + CDS + three_prime_UTR 拼接形成成熟的转录本序列用于uORF的注释
+    # exon 提取的是转录本内成熟的mRNA的序列,即外显子按基因组坐标首尾相连的matural transcript
+    mt, cds = '', ''
+    exons_list = []
+    for e in db.children(t, featuretype='exon', order_by='start'):
+        exons_list.append((e.start, e.end))
+        mt += e.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+    mt = Seq(mt)
+    if t.strand == '-':
+        mt = mt.reverse_complement()
+    # CDS 提取的是编码区 ATG ... TAG
+    for c in db.children(t, featuretype='CDS', order_by='start'):
+        cds += c.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+    if style == 'GTF':
+        sc_seq = stop_codon_seq(db, t, genome)
+        cds = add_stop_codon(cds, t.strand, sc_seq)
+    cds = Seq(cds)
+    ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
+    # mt from utr5/3 and cds
+    mt_from_utr_cds = ''
+    for e in db.children(t, featuretype=['five_prime_UTR', 'CDS', 'three_prime_UTR'], order_by='start'):
+        mt_from_utr_cds += e.sequence(genome, use_strand=False)
+    mt_from_utr_cds = Seq(mt_from_utr_cds)
+    if t.strand == '-':
+        mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
+    if mt != mt_from_utr_cds:
+        mt = mt_from_utr_cds
+        # error_count += 1
+    if t.strand == '-':
+        cds = cds.reverse_complement()
+    return mt, cds, exons_list
+    
 
 def get_uorf(args):
     """ Get uORF main command line entry
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     """
     db = gffutils.FeatureDB(args.database, keep_order=True)
+    feature_types = db.featuretypes()
     # csv
     # uORF_seq = pd.DataFrame(columns=_uORF_csv_header)
-    uORF_seq_list = []
+    # uORF_seq_list = []
+    uORF_seq_list = deque()
     # gff
     uORF_gff = open(args.output,'w')
     # fasta
-    uorf_record = []
+    # uorf_record = []
+    uorf_record = deque()
     index = 0
     if args.rna_feature == 'mRNA':
         mRNA_str = mRNA_type(args.style)
     else:
-        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     error_count = 0
+    total_transcript_number = len(list(db.features_of_type(mRNA_str, order_by='start')))
     # loop all transcripts in genome
     if not args.transcript:
         for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
+                      total = total_transcript_number, \
                       ncols = 80, desc = "uORF Processing :"):
-            # primary transcript (pt) 是基因组上的转录本的序列，
-            # 有的会包括intron，所以提取的序列和matural transcript (mt) 不一致
-            pt = t.sequence(args.genome, use_strand=True)
-            # matural transcript (mt)
-            # 该步骤是获取序列: 转录本序列，CDS序列, five_prime_UTR, three_prime_UTR
-            # 但是有的基因注释不正确，导致成熟转录本序列的两个来源不一致，一个是exon来源的，一个是five_prime_UTR和CDS来源的
-            # 针对这种请情况，我们使用 five_prime_UTR + CDS + three_prime_UTR 拼接形成成熟的转录本序列用于uORF的注释
-            # exon 提取的是转录本内成熟的mRNA的序列,即外显子按基因组坐标首尾相连的matural transcript
-            mt = ''
+            # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
+            # mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
+            mt, cds = '', ''
             exons_list = []
             for e in db.children(t, featuretype='exon', order_by='start'):
-                exons_list.append([e.start, e.end])
-                s = e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                mt += s
+                exons_list.append((e.start, e.end))
+                mt += e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
             mt = Seq(mt)
             if t.strand == '-':
                 mt = mt.reverse_complement()
             # CDS 提取的是编码区 ATG ... TAG
-            cds = ''
             for c in db.children(t, featuretype='CDS', order_by='start'):
-                s = c.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                cds += s
+                cds += c.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
             if args.style == 'GTF':
                 sc_seq = stop_codon_seq(db, t, args.genome)
                 cds = add_stop_codon(cds, t.strand, sc_seq)
             cds = Seq(cds)
             ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
             # mt from utr5/3 and cds
             mt_from_utr_cds = ''
-            for e in db.children(t, featuretype=['five_prime_UTR','CDS', 'three_prime_UTR'], order_by='start'):
+            for e in db.children(t, featuretype=['five_prime_UTR', 'CDS', 'three_prime_UTR'], order_by='start'):
                 mt_from_utr_cds += e.sequence(args.genome, use_strand=False)
             mt_from_utr_cds = Seq(mt_from_utr_cds)
             if t.strand == '-':
                 mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
             if mt != mt_from_utr_cds:
                 mt = mt_from_utr_cds
-                error_count += 1
+                # error_count += 1
             if t.strand == '-':
                 cds = cds.reverse_complement()
             # procedure-oriented
             # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
             # objected-oriented
             if mt == cds: # not contain uORF
                 continue
@@ -467,15 +504,15 @@
                     if len(it[8]) <= args.length:
                         # default: 6
                         continue
                     # csv output format 
                     if args.output_format == 'csv':
                         # uORF_seq.loc[index] = it
                         # dict 
-                        uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
+                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
                         index += 1
                     elif args.output_format == 'fasta':
                         uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
                         seq = it[8] # it[8] is s Seq type
                         desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
                                                                       it[4],
                                                                       it[5],
@@ -491,79 +528,38 @@
                         uorf_gff_line,features_gff_lines = gff.parse() 
                         # print(uorf_gff_line)
                         uORF_gff.write(uorf_gff_line+"\n") 
                         for feature_line in features_gff_lines:
                             # print(feature_line)
                             uORF_gff.write(feature_line+"\n")
                     else:
-                        # args.output_format == 'csv'
-                        uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
+                        # csv output_format
+                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
                         index += 1 
         # output file 
         if args.output_format == 'csv':
             uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
             uORF_seq.to_csv(args.output, sep=',', index=False)
         elif args.output_format == 'gff':
             uORF_gff.close()
         elif args.output_format == 'fasta':
             with open(args.output,'w') as handle:
                 SeqIO.write(uorf_record, handle, "fasta")
         else:
             uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
             uORF_seq.to_csv(args.output, sep=',', index=False)
     else:
-        mRNA_str = tuple([x for x in list(db.featuretypes()) if 'RNA' in x or 'trascript' in x])
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
         # specify the transcript id; only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             # primary transcript (pt) 是基因组上的转录本的序列，
             # 有的会包括intron，所以提取的序列和matural transcript 不一致
             # id specify
             if args.transcript in t.id:
-                pt = t.sequence(args.genome, use_strand=True)
-                # matural transcript (mt)
-                # exon 提取的是转录本内成熟的MRNA的序列,即外显子收尾相连的matural transcript
-                mt = ''
-                exons_list = []
-                for e in db.children(t, featuretype='exon', order_by='start'):
-                    exons_list.append([e.start, e.end]) # 1 based location 
-                    s = e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                    mt += s
-                mt = Seq(mt)
-                mt_len = len(mt)
-                if t.strand == '-':
-                    mt = mt.reverse_complement()
-                # intron for uORF locate position 
-                for i in db.children(t, featuretype='intron', order_by='start'):
-                    pass
-                # CDS 提取的是编码区 ATG ... TAG
-                cds = ''
-                cds_list = []
-                for c in db.children(t, featuretype='CDS', order_by='start'):
-                    cds_list.append([c.start, c.end])
-                    s = c.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                    # print('cds len i:', len(c))
-                    cds += s
-                if args.style == 'GTF':
-                    sc_seq = stop_codon_seq(db, t, args.genome)
-                    cds = add_stop_codon(cds, t.strand, sc_seq)
-                cds = Seq(cds)
-                ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
-                # mt from utr5/3 and cds
-                mt_from_utr_cds = ''
-                for e in db.children(t, featuretype=['five_prime_UTR','CDS', 'three_prime_UTR'], order_by='start'):
-                    mt_from_utr_cds += e.sequence(args.genome, use_strand=False)
-                mt_from_utr_cds = Seq(mt_from_utr_cds)
-                if t.strand == '-':
-                    mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
-                if mt != mt_from_utr_cds:
-                    mt = mt_from_utr_cds
-                    error_count += 1
-                cds_len = len(cds)
-                if t.strand == '-':
-                    cds = cds.reverse_complement()
+                mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
                 # procedure-oriented 
                 # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
                 # objected-oriented
                 if mt == cds:  # not contain uORF
                     continue
                 if len(cds) % 3 != 0: # CDS error
                     continue
@@ -571,14 +567,18 @@
                 uORF_dict = uORF_.uorf_parse()
                 if len(uORF_dict) == 0:  # CDS error
                     continue
                 uorf_location_genome = [] # for schematic on genome # 3D list 
                 for key in sorted(uORF_dict.keys()):
                     # print(key,len(uORF_dict[key]))
                     for it in uORF_dict[key]:
+                        # uORF length filter 
+                        if len(it[8]) <= args.length:
+                            # default: 6
+                            continue
                         # csv output format 
                         if args.output_format == 'csv':
                             # uORF_seq.loc[index] = it
                             # dict is fastest way 
                             uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
                             index += 1
                             # for schematic on genome
```

### Comparing `featurExtract-0.2.5.5/featurExtract/database/database.py` & `featurExtract-0.2.5.6/featurExtract/database/database.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/feature_extract.py` & `featurExtract-0.2.5.6/featurExtract/feature_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,112 +148,112 @@
                            help='database absolute path')
 parser_create.set_defaults(func=create)
 
 # promoter subcommand
 parser_promoter = subparsers.add_parser('promoter', help='extract promoter in genome or gene')
 parser_promoter.add_argument('-d', '--database', type=str, required=True, 
                              help='database generated by subcommand create')
-parser_promoter.add_argument('-f', '--genome', type=str, required=True,
+parser_promoter.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+                             help = 'output format')
+parser_promoter.add_argument('-g', '--genome', type=str, required=True,
                              help='genome fasta path')
-parser_promoter.add_argument('-g', '--gene', type=str, 
+parser_promoter.add_argument('-i', '--gene', type=str, 
                              help='specific gene; if not given, return whole genes')
 parser_promoter.add_argument('-l', '--promoter_length', type=int, default=100,
                              help='promoter length before TSS (default: 100)')
-parser_promoter.add_argument('-u', '--utr5_upper_length', type=int, default=10,
-                             help='5\' utr length after TSS (default: 10)')
 parser_promoter.add_argument('-o', '--output', type=str, 
                              help = 'output file path')
-parser_promoter.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'], 
-                             help = 'output format')
 parser_promoter.add_argument('-p', '--print', action="store_true", 
                              help = 'output to stdout')
+parser_promoter.add_argument('-u', '--utr5_upper_length', type=int, default=10,
+                             help='5\' utr length after TSS (default: 10)')
 parser_promoter.set_defaults(func=promoter)
 
 
 # terminator 
 parser_terminator = subparsers.add_parser('terminator', help='extract terminator in genome or gene')
 parser_terminator.add_argument('-d', '--database', type=str, required=True,
                              help='database generated by subcommand create')
-parser_terminator.add_argument('-f', '--genome', type=str, required=True,
+parser_terminator.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+                             help = 'output format')
+parser_terminator.add_argument('-g', '--genome', type=str, required=True,
                              help='genome fasta path')
-parser_terminator.add_argument('-g', '--gene', type=str,
+parser_terminator.add_argument('-i', '--gene', type=str,
                              help='specific gene; if not given, return whole genes')
 parser_terminator.add_argument('-l', '--terminator_length', type=int, default=100,
                              help='terminator length (default: 100)')
-parser_terminator.add_argument('-u', '--utr3_upper_length', type=int, default=10,
-                             help='3\' length (default: 10)')
 parser_terminator.add_argument('-o', '--output', type=str,
                              help = 'output file path')
-parser_terminator.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'],
-                             help = 'output format')
 parser_terminator.add_argument('-p', '--print', action="store_true",
                              help = 'output to stdout')
+parser_terminator.add_argument('-u', '--utr3_upper_length', type=int, default=10,
+                             help='3\' length (default: 10)')
 parser_terminator.set_defaults(func=terminator)
 
 # gene subcommand 
 parser_gene = subparsers.add_parser('gene', help='extract gene in genome or gene')
 parser_gene.add_argument('-d', '--database', type=str, required=True,
                          help='database generated by subcommand create')
-parser_gene.add_argument('-f', '--genome', type=str, required=True,
+parser_gene.add_argument('-g', '--genome', type=str, required=True,
                          help='genome fasta')
-parser_gene.add_argument('-g', '--gene', type=str, 
+parser_gene.add_argument('-i', '--gene', type=str, 
                          help='specific gene; if not given, return whole genes')
 parser_gene.add_argument('-o', '--output', type=str, 
                          help = 'output file path')
 parser_gene.add_argument('-p', '--print', action="store_true", 
                          help='output to stdout')
 parser_gene.set_defaults(func=gene)
 
 # mRNA subcommand 
 parser_mRNA = subparsers.add_parser('mRNA', help='extract mature messager RNA in genome or gene')
 parser_mRNA.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
-parser_mRNA.add_argument('-f', '--genome', type=str, required=True, 
+parser_mRNA.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+                         help = 'output format')
+parser_mRNA.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_mRNA.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript; if not given, return whole transcripts')
 parser_mRNA.add_argument('-o', '--output', type=str, 
                          help = 'output file path')
-parser_mRNA.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'], 
-                         help = 'output format')
 parser_mRNA.add_argument('-p', '--print', action="store_true", 
                          help='output to stdout')
+parser_mRNA.add_argument('-s', '--style', choices=['GFF','GTF'],
+                         help = 'GTF database or GFF database')
 parser_mRNA.add_argument('-u', '--upper', action="store_true", 
                          help='upper CDS and lower utr')
-parser_mRNA.add_argument('-s', '--style', choices=['GFF','GTF'], 
-                         help = 'GTF database or GFF database')
 parser_mRNA.set_defaults(func=mRNA)
 
 
 # cdna subcommand 
 parser_cdna = subparsers.add_parser('cdna', help='extract cdna (or refMrna) in genome or gene')
 parser_cdna.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
-parser_cdna.add_argument('-f', '--genome', type=str, required=True, 
+parser_cdna.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+                         help = 'output format')
+parser_cdna.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_cdna.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript; if not given, return whole transcripts')
 parser_cdna.add_argument('-o', '--output', type=str, 
                          help = 'output file path')
-parser_cdna.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'], 
-                         help = 'output format')
 parser_cdna.add_argument('-p', '--print', action="store_true", 
                          help='output to stdout')
+parser_cdna.add_argument('-s', '--style', choices=['GFF','GTF'],
+                         help = 'GTF database or GFF database')
 parser_cdna.add_argument('-u', '--upper', action="store_true", 
                          help='upper CDS and lower utr')
-parser_cdna.add_argument('-s', '--style', choices=['GFF','GTF'], 
-                         help = 'GTF database or GFF database')
 parser_cdna.set_defaults(func=cdna)
 
 
 # IGR subcommand 
 parser_IGR = subparsers.add_parser('IGR', help='extract IGR in genome or gene')
 parser_IGR.add_argument('-d', '--database', type=str, required=True,
                         help='database generated by subcommand create')
-parser_IGR.add_argument('-f', '--genome', type=str, required=True, 
+parser_IGR.add_argument('-g', '--genome', type=str, required=True, 
                         help='genome fasta')
 parser_IGR.add_argument('-l', '--IGR_length', type=int, default=100,
                         help='IGR length threshold')
 parser_IGR.add_argument('-o', '--output', type=str, 
                         help = 'output fasta file path')
 parser_IGR.add_argument('-p', '--print', action="store_true", 
                         help='output to stdout')
@@ -262,15 +262,15 @@
                        protein genes, while GFF database contain protein genes and nocoding genes')
 parser_IGR.set_defaults(func=IGR)
 
 # UTR subcommand
 parser_utr = subparsers.add_parser('UTR', help='extract untranslated region sequence in genome or gene')
 parser_utr.add_argument('-d', '--database', type=str, required=True, 
                         help='database generated by subcommand create')
-parser_utr.add_argument('-f', '--genome', type=str, required=True,
+parser_utr.add_argument('-g', '--genome', type=str, required=True,
                         help='genome fasta file')
 parser_utr.add_argument('-i', '--transcript', type=str, 
                         help='specific transcript id; if not given, \
                         whole transcript will return')
 parser_utr.add_argument('-o', '--output', type=str, 
                         help='output file path')
 parser_utr.add_argument('-p', '--print', action="store_true", 
@@ -281,83 +281,91 @@
                         help = 'GTF database or GFF database')
 parser_utr.set_defaults(func=UTR)
 
 # uORF subcommand
 parser_uORF = subparsers.add_parser('uORF', help='extract upper stream open reading sequence in genome or gene')
 parser_uORF.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
-parser_uORF.add_argument('-f', '--genome', type=str, required=True, 
+parser_uORF.add_argument('-f', '--output_format', choices=['csv','fasta','gff'],
+                        help='output format (default: csv)')
+parser_uORF.add_argument('-g', '--genome', type=str, required=True,
                          help='genome fasta')
 parser_uORF.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript id; if not given, \
                                whole transcript will return')
 parser_uORF.add_argument('-l', '--length', type=int, default=6,
                          help='uORF length, (default: 6)')
-parser_uORF.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
-                         help='The type of RNA used to make uORF identification (default: mRNA)')
-parser_uORF.add_argument('-t', '--output_format', choices=['csv','fasta','gff'], 
-                        help='output format (default: csv)')
-parser_uORF.add_argument('-o', '--output', type=str, 
-                         help='output file path')
-parser_uORF.add_argument('-m', '--schematic_without_intron', action='store_false',default='False',
+parser_uORF.add_argument('-m', '--schematic_without_intron', action='store_true',
                          help='schematic figure file for uORF, CDS and transcript without intron')
-parser_uORF.add_argument('-n', '--schematic_with_intron', action='store_false',default='False',
+parser_uORF.add_argument('-n', '--schematic_with_intron', action='store_true',
                          help='schematic figure file for uORF, CDS and transcript with intron')
+parser_uORF.add_argument('-o', '--output', type=str, 
+                         help='output file path')
+parser_uORF.add_argument('-p', '--process', type=int, default=1,
+                         help='number of uORF extract process, (default: 1)')
+parser_uORF.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
+                         help='The type of RNA used to make uORF identification (default: mRNA)')
 parser_uORF.add_argument('-s', '--style', choices=['GFF','GTF'], 
                          help = 'GTF database or GFF database')
 parser_uORF.set_defaults(func=uORF)
 
 # CDS subcommand
 parser_cds = subparsers.add_parser('CDS', help='extract coding sequence in genome or gene')
 parser_cds.add_argument('-d', '--database', type=str, required=True, 
                         help='database generated by subcommand create')
-parser_cds.add_argument('-f', '--genome', type=str, required=True,
+parser_cds.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+                         help = 'output format')
+parser_cds.add_argument('-g', '--genome', type=str, required=True,
                         help='genome fasta')
 parser_cds.add_argument('-i', '--transcript', type=str, 
                         help='specific transcript id; if not given, \
                         whole transcript will return')
 parser_cds.add_argument('-o', '--output', type=str, 
                         help='output file path')
 parser_cds.add_argument('-p', '--print', action="store_true", 
                         help='output to stdout')
 parser_cds.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
                          help='The type of RNA used to extract CDS, (default: mRNA)')
-parser_cds.add_argument('-t', '--output_format', type=str, choices=['csv','fasta'],
-                         help = 'output format')
 parser_cds.add_argument('-s', '--style', choices=['GFF','GTF'], 
                         help = 'GTF database or GFF database')
 parser_cds.set_defaults(func=CDS)
 
 # dORF subcommand 
 parser_dORF = subparsers.add_parser('dORF', help='extract down stream open reading frame sequence in a genome or gene')
 parser_dORF.add_argument('-d', '--database', type=str, required=True,
                          help='database generated by subcommand create')
-parser_dORF.add_argument('-f', '--genome', type=str, required=True, 
+parser_dORF.add_argument('-f', '--output_format', choices=['csv','fasta','gff'],
+                        help='output format')
+parser_dORF.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_dORF.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript id; if not given, \
                                whole transcript will return')
-parser_dORF.add_argument('-t', '--output_format', choices=['csv','fasta','gff'],
-                        help='output format ')
-parser_dORF.add_argument('-o', '--output', type=str, 
-                         help='output file path')
-parser_dORF.add_argument('-m', '--schematic_without_intron', type=str,
+parser_dORF.add_argument('-l', '--length', type=int, default=6,
+                         help='dORF length, (default: 6)')
+parser_dORF.add_argument('-m', '--schematic_without_intron', action='store_true',
                          help='schematic figure file for dORF, CDS and transcript without intron')
-parser_dORF.add_argument('-n', '--schematic_with_intron', type=str,
+parser_dORF.add_argument('-n', '--schematic_with_intron', action='store_true',
                          help='schematic figure file for dORF, CDS and transcript with intron')
+parser_dORF.add_argument('-o', '--output', type=str, 
+                         help='output file path')
+parser_dORF.add_argument('-p', '--process', type=int, default=1,
+                         help='number of dORF extract process, (default: 1)')
+parser_dORF.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
+                         help='The type of RNA used to make dORF identification (default: mRNA)')
 parser_dORF.add_argument('-s', '--style', choices=['GFF','GTF'], 
                          help = 'GTF database or GFF database')
 parser_dORF.set_defaults(func=dORF)
 
 
 # exon 
 parser_exon = subparsers.add_parser('exon', help='extract exon sequence for a given transcript')
 parser_exon.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
-parser_exon.add_argument('-f', '--genome', type=str, required=True, 
+parser_exon.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_exon.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript id; needed')
 parser_exon.add_argument('-o', '--output', type=str, 
                          help='output file path')
 parser_exon.add_argument('-p', '--print', action="store_true", 
                          help='output to stdout')
@@ -365,29 +373,24 @@
                          help = 'GTF database or GFF database')
 parser_exon.set_defaults(func=exon)
 
 # intron 
 parser_intron = subparsers.add_parser('intron', help='extract exon sequence for a given transcript')
 parser_intron.add_argument('-d', '--database', type=str, required=True, 
                            help='database generated by subcommand create')
-parser_intron.add_argument('-f', '--genome', type=str, required=True, 
+parser_intron.add_argument('-g', '--genome', type=str, required=True, 
                            help='genome fasta')
 parser_intron.add_argument('-i', '--transcript', type=str, 
                            help='specific transcript id; needed')
 parser_intron.add_argument('-o', '--output', type=str, 
                            help='output file path')
 parser_intron.add_argument('-p', '--print', action="store_true", 
                            help='output to stdout')
 parser_intron.add_argument('-s', '--style', choices=['GFF','GTF'], 
                            help = 'GTF database or GFF database')
 parser_intron.set_defaults(func=intron)
 
-
 args = parser.parse_args()
-# print('[%s runing ...]'%(time.strftime("%a %b %d %H:%M:%S %Y", time.localtime())))
-# pool = multiprocessing.Pool(4)
-# pool.apply_async(func=args.func, args=args)
-# pool.close()
-# pool.join()
+#print('[%s runing ...]'%(time.strftime("%a %b %d %H:%M:%S %Y", time.localtime())))
 args.func(args)
-# print('[%s finished ...]'%(time.strftime("%a %b %d %H:%M:%S %Y", time.localtime())))
-
+#print('[%s finished ...]'%(time.strftime("%a %b %d %H:%M:%S %Y", time.localtime())))
+
```

### Comparing `featurExtract-0.2.5.5/featurExtract/genBank_extract.py` & `featurExtract-0.2.5.6/featurExtract/genBank_extract.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/parameter.py` & `featurExtract-0.2.5.6/featurExtract/parameter.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/utils/util.py` & `featurExtract-0.2.5.6/featurExtract/utils/util.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.5/featurExtract/utils/visualize.py` & `featurExtract-0.2.5.6/featurExtract/utils/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
         '''
         intron_list_all = []
         intron_start = 0
         intron_end = 0
         # 2D list 
         for xorf in self.xorf_location:
             # wotyout intron 
+            print('xorf:', xorf)
             if len(xorf) == 1:
                 intron_list_all.append([])
             else:
                 # with intron 
                 if self.strand == '-':
                     xorf = xorf[::-1] # reverse list 
                 intron_list = []
```

### Comparing `featurExtract-0.2.5.5/featurExtract.egg-info/PKG-INFO` & `featurExtract-0.2.5.6/featurExtract.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurExtract
-Version: 0.2.5.5
+Version: 0.2.5.6
 Summary: Extract genome ferature sequence for biologists
 Home-page: https://github.com/SitaoZ/featurExtract.git
 Author: zhusitao
 Author-email: zhusitao1990@163.com
 License: MIT
 Keywords: genome feature,extract
 Platform: UNKNOWN
```

### Comparing `featurExtract-0.2.5.5/featurExtract.egg-info/SOURCES.txt` & `featurExtract-0.2.5.6/featurExtract.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 MANIFEST.in
 README.md
 setup.py
 featurExtract/__init__.py
 featurExtract/a.py
+featurExtract/b.py
+featurExtract/c.py
 featurExtract/command_gb.py
 featurExtract/command_gff.py
 featurExtract/feature_extract.py
 featurExtract/genBank_extract.py
 featurExtract/parameter.py
 featurExtract/version.py
 featurExtract.egg-info/PKG-INFO
```

### Comparing `featurExtract-0.2.5.5/setup.py` & `featurExtract-0.2.5.6/setup.py`

 * *Files identical despite different names*

