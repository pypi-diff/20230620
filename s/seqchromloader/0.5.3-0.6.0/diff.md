# Comparing `tmp/seqchromloader-0.5.3.tar.gz` & `tmp/seqchromloader-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.5.3.tar", last modified: Tue May 30 17:03:04 2023, max compression
+gzip compressed data, was "seqchromloader-0.6.0.tar", last modified: Tue Jun 20 15:14:13 2023, max compression
```

## Comparing `seqchromloader-0.5.3.tar` & `seqchromloader-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.504793 seqchromloader-0.5.3/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1374 2023-05-30 17:03:04.504229 seqchromloader-0.5.3/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.3/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.492703 seqchromloader-0.5.3/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.5.3/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-05-30 04:51:02.000000 seqchromloader-0.5.3/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12391 2023-05-30 04:41:31.000000 seqchromloader-0.5.3/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6693 2023-05-30 16:57:25.000000 seqchromloader-0.5.3/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.497095 seqchromloader-0.5.3/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1374 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-05-30 17:03:04.504893 seqchromloader-0.5.3/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-05-30 17:02:33.000000 seqchromloader-0.5.3/setup.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.503274 seqchromloader-0.5.3/tests/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    10950 2023-05-30 05:34:50.000000 seqchromloader-0.5.3/tests/test_writer_loader.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.169778 seqchromloader-0.6.0/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-20 15:14:13.169450 seqchromloader-0.6.0/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.0/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.152544 seqchromloader-0.6.0/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.0/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12423 2023-06-20 14:51:56.000000 seqchromloader-0.6.0/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14272 2023-06-20 14:56:57.000000 seqchromloader-0.6.0/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7280 2023-06-20 14:39:51.000000 seqchromloader-0.6.0/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.162922 seqchromloader-0.6.0/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-06-20 15:14:13.169876 seqchromloader-0.6.0/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-06-20 14:48:49.000000 seqchromloader-0.6.0/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.168493 seqchromloader-0.6.0/tests/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12376 2023-06-20 15:03:21.000000 seqchromloader-0.6.0/tests/test_writer_loader.py
```

### Comparing `seqchromloader-0.5.3/PKG-INFO` & `seqchromloader-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.3
+Version: 0.6.0
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
-License: UNKNOWN
-Description: # seqchromloader
-        
-        seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
-        
-        Plan to support dataset formats including:
-        - webdataset (done)
-        - tfrecord (x)
-        
-        Training framework support:
-        - pytorch dataloader (done)
-        - pytorch-lightning datamodule (done)
-        - NVIDIA-DALI (x)
-        
-        ## Installation
-        
-        ### conda (suggested):
-        
-        `mamba install -c bioconda -c conda-forge seqchromloader`
-        
-        or
-        
-        `conda install -c bioconda -c conda-forge seqchromloader`
-        
-        ### pip
-        
-        `pip install seqchromloader`
-        
-        ## Usage
-        
-        For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
-        
 Keywords: dataloder,pytorch,webdataset
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
+
+# seqchromloader
+
+seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
+
+Plan to support dataset formats including:
+- webdataset (done)
+- tfrecord (x)
+
+Training framework support:
+- pytorch dataloader (done)
+- pytorch-lightning datamodule (done)
+- NVIDIA-DALI (x)
+
+## Installation
+
+### conda (suggested):
+
+`mamba install -c bioconda -c conda-forge seqchromloader`
+
+or
+
+`conda install -c bioconda -c conda-forge seqchromloader`
+
+### pip
+
+`pip install seqchromloader`
+
+## Usage
+
+For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
```

### Comparing `seqchromloader-0.5.3/README.md` & `seqchromloader-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.3/seqchromloader/loader.py` & `seqchromloader-0.6.0/seqchromloader/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             feature = utils.extract_info(
                 item.chrom,
                 item.start,
                 item.end,
                 item.label,
                 genome_pyfaidx=self.genome_pyfaidx,
                 bigwigs=self.bigwigs,
-                target_bam=self.target_pysam,
+                target=self.target_pysam,
                 strand=item.strand,
                 transforms=self.transforms
             )
         except utils.BigWigInaccessible as e:
             raise e
 
         return feature['seq'], feature['chrom'], feature['target'], feature['label']
```

### Comparing `seqchromloader-0.5.3/seqchromloader/utils.py` & `seqchromloader-0.6.0/seqchromloader/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 Utilities for iterating constructing data sets and iterating over
 DNA sequence data.
 """
+import math
 import pandas as pd
 import numpy as np
 import logging
+import pysam
+import pyBigWig
 from multiprocessing import Pool
 from pybedtools import Interval, BedTool
 from pybedtools.helpers import chromsizes
 
 def get_genome_sizes(gs=None, genome=None, to_filter=None, to_keep=None):
     """
     Loads the genome sizes file, filter or keep chromosomes
@@ -201,14 +204,53 @@
     genome_chops_bdt = BedTool.from_dataframe(genome_chops)
     
     if incl: genome_chops_bdt = genome_chops_bdt.intersect(incl, wa=True)
     if excl: genome_chops_bdt = genome_chops_bdt.intersect(excl, v=True)
 
     return genome_chops_bdt.to_dataframe()[["chrom", "start", "end"]]
 
+def compute_mean_std_bigwig(bigwig):
+    """
+    
+    Compute the overall mean and standard deviation of a given bigwig file
+
+    :param bigwig: bigwig file path
+    :type bigwig: str
+    :rtype: (mean, stddev)
+    """
+    bw = pyBigWig.open(bigwig)
+    
+    # get chrom length list
+    chroms = bw.chroms()
+    
+    # iterate chrom list to get mean and std
+    ns = []; means = []; stds = []
+    for chrom, length in chroms.items():
+        # iterate all intervals to get the covered length
+        length = sum([i[1]-i[0] for i in bw.intervals(chrom)])
+        ns.append(length)
+        means.append(bw.stats(chrom, type="mean", exact=True)[0])
+        try:
+            stds.append(bw.stats(chrom, type="std", exact=True)[0])
+        except RuntimeError:
+            print(chrom)
+            print(length)
+            raise Exception
+    
+    # compute overall metrics
+    std_all = 0
+    ns_sum = sum(ns); mean_all = sum([n*means[i] for i, n in enumerate(ns)])/ns_sum
+    for i, n in enumerate(ns):
+        std_all += n* math.pow(means[i]- mean_all, 2)
+        std_all += n* math.pow(stds[i], 2)
+    std_all /= ns_sum
+    std_all = math.sqrt(std_all)
+    
+    return mean_all, std_all
+
 class DNA2OneHot(object):
     def __init__(self):
         self.DNA2Index = {
             "A": 0,
             "C": 1, 
             "G": 2,
             "T": 3,
@@ -279,42 +321,62 @@
         super().__init__(*args)
         self.chrom = chrom
         self.start = start
         self.end = end
 
     def __str__(self) -> str:
         return f'Chromatin Info Inaccessible in region {self.chrom}:{self.start}-{self.end}'
+    
+def extract_bw(chrom, start, end, strand, bigwigs):
+    chroms_array = []
+    try:
+        for idx, bigwig in enumerate(bigwigs):
+            c = (np.nan_to_num(bigwig.values(chrom, start, end))).astype(np.float32)
+            if strand=="-":
+                c = c[::-1] 
+            chroms_array.append(c)
+    except RuntimeError as e:
+        logging.warning(e)
+        logging.warning(f"RuntimeError happened when accessing {chrom}:{start}-{end}, it's probably due to at least one chromatin track bigwig doesn't have information in this region")
+        raise BigWigInaccessible(chrom, start, end)
+    chroms_array = np.vstack(chroms_array)  # create the chromatin track array, shape (num_tracks, length)
+    
+    return chroms_array
 
-def extract_info(chrom, start, end, label, genome_pyfaidx, bigwigs, target_bam, strand="+", transforms:dict=None):
+def extract_dnaOneHot(chrom, start, end, strand, genome_pyfaidx):
     seq = genome_pyfaidx[chrom][int(start):int(end)].seq
     if strand=="-":
         seq = rev_comp(seq)
     seq_array = dna2OneHot(seq)
+    
+    return seq_array
+
+def extract_target(chrom, start, end, strand, target):
+    if isinstance(target, pysam.AlignmentFile):
+        target_array = np.array(target.count(chrom, start, end), dtype=np.float32)[np.newaxis]
+    elif isinstance(target, pyBigWig.pyBigWig):
+        target_array = np.nan_to_num(target.values(chrom, start, end)).astype(np.float32)
+        if strand=="-":
+            target_array = target_array[::-1]
+    else:
+        target_array = None
+    return target_array
+
+def extract_info(chrom, start, end, label, genome_pyfaidx, bigwigs, target, strand="+", transforms:dict=None):
+    seq_array = extract_dnaOneHot(chrom, start, end, strand, genome_pyfaidx)
 
     #chromatin track
-    chroms_array = []
     if bigwigs is not None and len(bigwigs)>0:
-        try:
-            for idx, bigwig in enumerate(bigwigs):
-                c = (np.nan_to_num(bigwig.values(chrom, start, end))).astype(np.float32)
-                if strand=="-":
-                    c = c[::-1] 
-                chroms_array.append(c)
-        except RuntimeError as e:
-            logging.warning(e)
-            logging.warning(f"RuntimeError happened when accessing {chrom}:{start}-{end}, it's probably due to at least one chromatin track bigwig doesn't have information in this region")
-            raise BigWigInaccessible(chrom, start, end)
-        chroms_array = np.vstack(chroms_array)  # create the chromatin track array, shape (num_tracks, length)
+        chroms_array = extract_bw(chrom, start, end, strand, bigwigs)
     else:
         chroms_array = None
     # label
     label_array = np.array(label, dtype=np.int32)[np.newaxis]
     # counts
-    target_array = target_bam.count(chrom, start, end) if target_bam is not None else np.nan
-    target_array = np.array(target_array, dtype=np.float32)[np.newaxis]
+    target_array = extract_target(chrom, start, end, strand, target)
 
     feature = {
         'seq': seq_array,
         'chrom': chroms_array,
         'target': target_array,
         'label': label_array
     }
```

### Comparing `seqchromloader-0.5.3/seqchromloader/writer.py` & `seqchromloader-0.6.0/seqchromloader/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         feature_dict["chrom.npy"] = chrom
         feature_dict["target.npy"] = target
         feature_dict["label.npy"] = label
         sink.write(feature_dict)
     sink.close()
     
 def dump_data_webdataset(coords, genome_fasta, bigwig_filelist,
-                        target_bam=None, 
+                        target_bam=None,
+                        target_bw=None, 
                         outdir="dataset/", outprefix="seqchrom", 
                         compress=True, 
                         numProcessors=1,
                         transforms=None,
                         braceexpand=False,
                         DALI=False):
     """
@@ -60,16 +61,18 @@
 
     :param coords: pandas DataFrame containing genomic coordinates with columns **[chrom, start, end, label]**
     :type coords: pandas DataFrame
     :param genome_fasta: Genome fasta file.
     :type genome_fasta: str
     :param bigwig_filelist: A list of bigwig files containing track information (e.g., histone modifications)
     :type bigwig_filelist: list of str or None
-    :param target_bam: bam file to get # reads in each region
+    :param target_bam: bam file to get # reads in each region, mutually exclusive with `target_bw`
     :type target_bam: str or None
+    :param target_bw: bigwig file to get # reads in each region, mutually exclusive with `target_bam`
+    :type target_bw: str or None
     :param transforms: A dictionary of functions to transform the output data, accepted keys are *["seq", "chrom", "target", "label"]*
     :type transforms: dict of functions
     :param outdir: output directory to save files in
     :type outdir: str
     :param outprefix: prefix of output files
     :type outprefix: str
     :param compress: whether to compress the output files
@@ -77,26 +80,30 @@
     :param numProcessors: number of processors
     :type numProcessors: int
     :param braceexpand: if use brace to simplify the wds file list into a string
     :param braceexpand: boolean
     :param DALI: Set to True if you want to use the dataset for NVIDIA DALI, it would save all arrays in bytes, which results in losing the array shape info
     :param DALI: boolean
     """
+    # check parameters
+    if (target_bam is not None and target_bw is not None):
+        raise Exception("Only one of target_bam and target_bw should be provided!")
 
     # split coordinates and assign chunks to workers
     num_chunks = math.ceil(len(coords) / 7000)
     chunks = np.array_split(coords, num_chunks)
     
     # freeze the common parameters
     ## create a scaler to get statistics for normalizing chromatin marks input
     ## also create a multiprocessing lock
     dump_data_worker_freeze = functools.partial(dump_data_webdataset_worker, 
                                                     fasta=genome_fasta, 
                                                     bigwig_files=bigwig_filelist,
                                                     target_bam=target_bam,
+                                                    target_bw=target_bw,
                                                     compress=compress,
                                                     outdir=outdir,
                                                     transforms=transforms,
                                                     DALI=DALI)
     
     count_of_digits = 0
     nc = num_chunks
@@ -115,23 +122,29 @@
     else:
         return files
 
 def dump_data_webdataset_worker(coords, 
                                 outprefix, 
                                 fasta, 
                                 bigwig_files,
-                                target_bam=None, 
+                                target_bam=None,
+                                target_bw=None,
                                 outdir="dataset/", 
                                 compress=True,
                                 transforms=None,
                                 DALI=False):
     # get handlers
     genome_pyfaidx = pyfaidx.Fasta(fasta)
     bigwigs = [pyBigWig.open(bw) for bw in bigwig_files]
-    target_pysam = pysam.AlignmentFile(target_bam) if target_bam is not None else None
+    if target_bam is not None:
+        target = pysam.AlignmentFile(target_bam)
+    elif target_bw is not None:
+        target = pyBigWig.open(target_bw)
+    else:
+        target = None
 
     # iterate all records
     filename = os.path.join(outdir, f"{outprefix}.tar.gz" if compress else f"{outprefix}.tar")
     sink = wds.TarWriter(filename, compress=compress)
     for rindex, item in enumerate(coords.itertuples()):
         feature_dict = defaultdict()
         feature_dict["__key__"] = f"{rindex}_{item.chrom}:{item.start}-{item.end}_{item.strand}" 
@@ -140,15 +153,15 @@
             feature = utils.extract_info(
                 item.chrom,
                 item.start,
                 item.end,
                 item.label,
                 genome_pyfaidx=genome_pyfaidx,
                 bigwigs=bigwigs,
-                target_bam=target_pysam,
+                target=target,
                 strand=item.strand,
                 transforms=transforms,
             )
         except utils.BigWigInaccessible as e:
             continue
         
         if not DALI:
```

### Comparing `seqchromloader-0.5.3/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.6.0/seqchromloader.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.3
+Version: 0.6.0
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
-License: UNKNOWN
-Description: # seqchromloader
-        
-        seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
-        
-        Plan to support dataset formats including:
-        - webdataset (done)
-        - tfrecord (x)
-        
-        Training framework support:
-        - pytorch dataloader (done)
-        - pytorch-lightning datamodule (done)
-        - NVIDIA-DALI (x)
-        
-        ## Installation
-        
-        ### conda (suggested):
-        
-        `mamba install -c bioconda -c conda-forge seqchromloader`
-        
-        or
-        
-        `conda install -c bioconda -c conda-forge seqchromloader`
-        
-        ### pip
-        
-        `pip install seqchromloader`
-        
-        ## Usage
-        
-        For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
-        
 Keywords: dataloder,pytorch,webdataset
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
+
+# seqchromloader
+
+seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
+
+Plan to support dataset formats including:
+- webdataset (done)
+- tfrecord (x)
+
+Training framework support:
+- pytorch dataloader (done)
+- pytorch-lightning datamodule (done)
+- NVIDIA-DALI (x)
+
+## Installation
+
+### conda (suggested):
+
+`mamba install -c bioconda -c conda-forge seqchromloader`
+
+or
+
+`conda install -c bioconda -c conda-forge seqchromloader`
+
+### pip
+
+`pip install seqchromloader`
+
+## Usage
+
+For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
```

### Comparing `seqchromloader-0.5.3/setup.py` & `seqchromloader-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.5.3",
+    version="0.6.0",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

### Comparing `seqchromloader-0.5.3/tests/test_writer_loader.py` & `seqchromloader-0.6.0/tests/test_writer_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import numpy as np
 import pandas as pd
+from functools import partial
 from seqchromloader import SeqChromDatasetByDataFrame, SeqChromDatasetByBed, SeqChromDatasetByWds, SeqChromDataModule
 from seqchromloader import dump_data_webdataset, convert_data_webdataset
 from seqchromloader import get_genome_sizes, make_random_shift, make_flank, random_coords, chop_genome
 
 import unittest
 import tempfile
 import shutil
@@ -78,15 +79,15 @@
         coords_excl = chop_genome(chroms=["chr2", "chr12"], genome="mm10", stride=1000, l=500, excl=interval)
         for c in ['chr2', 'chr12']:
             df = coords_incl[coords_incl.chrom==c]
             self.assertTrue(np.all([df.start.iloc[i] - df.start.iloc[i-1] == 1000 for i in range(1, len(df))]))
         self.assertTrue(BedTool().from_dataframe(coords_incl).intersect(interval).count()==len(coords_incl))
         self.assertTrue(BedTool().from_dataframe(coords_excl).intersect(interval).count()==0)
 
-    def test_writer(self):
+    def test_writer_target_bam(self):
         coords = pd.DataFrame({
             'chrom': ["chr19", "chr19"],
             'start': [0, 3],
             'end': [5, 8],
             'label': [0, 1],
             'score': [".", "."],
             'strand': ["+", "+"]
@@ -121,14 +122,47 @@
         )
         seq, chrom, target, label = next(iter(ds))
         self.assertEqual(seq[1,0,4].item(), 1.0)
         self.assertEqual(chrom[0,0,3].item(), 999.0)
         self.assertEqual(target[0].item(), 2.0)
         self.assertEqual(label[1].item(), 1)
     
+    def test_writer_target_bw(self):
+        coords = pd.DataFrame({
+            'chrom': ["chr19", "chr19"],
+            'start': [0, 3],
+            'end': [5, 8],
+            'label': [0, 1],
+            'score': [".", "."],
+            'strand': ["+", "+"]
+        })
+        huge_coords = pd.concat([coords] * 5000, axis=0).reset_index()
+        dump_data_webdataset(huge_coords, 
+                    genome_fasta='data/sample.fa', 
+                    bigwig_filelist=['data/sample.bw'],
+                    target_bw='data/sample.bw',
+                    outdir=self.tempdir,
+                    outprefix='test',
+                    compress=True,
+                    transforms={'target': partial(np.sum, keepdims=True)},
+                    numProcessors=2)
+        self.assertIsFile(os.path.join(self.tempdir, "test_0.tar.gz"))
+        ds = wds.DataPipeline(
+            wds.SimpleShardList([os.path.join(self.tempdir, "test_0.tar.gz")]),
+            wds.tarfile_to_samples(),
+            wds.decode(),
+            wds.to_tuple("seq.npy", "chrom.npy", "target.npy", "label.npy"),
+            wds.batched(2)
+        )
+        seq, chrom, target, label = next(iter(ds))
+        self.assertEqual(seq[1,0,4].item(), 1.0)
+        self.assertEqual(chrom[0,0,3].item(), 999.0)
+        self.assertEqual(target[0].item(), 999.0)
+        self.assertEqual(label[1].item(), 1)
+        
     def test_wds_loader(self):
         it = iter(SeqChromDatasetByWds(["data/test_0.tar.gz"], dataloader_kws={"batch_size":3}))
         seq, chrom, target, label = next(it)
 
         self.assertEqual(seq[0,0,3].item(), 1.0)
         self.assertEqual(chrom[0,0,3].item(), 4.0)
         self.assertEqual(target[0].item(), 0.0)
```

