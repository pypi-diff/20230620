# Comparing `tmp/aicssegmentation-0.5.2.tar.gz` & `tmp/aicssegmentation-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicssegmentation-0.5.2.tar", last modified: Tue Jul 26 21:02:54 2022, max compression
+gzip compressed data, was "aicssegmentation-0.5.3.tar", last modified: Tue Jun 20 16:18:51 2023, max compression
```

## Comparing `aicssegmentation-0.5.2.tar` & `aicssegmentation-0.5.3.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.879475 aicssegmentation-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6295 2022-07-26 21:02:54.879475 aicssegmentation-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4965 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.851474 aicssegmentation-0.5.2/aicssegmentation/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.851474 aicssegmentation-0.5.2/aicssegmentation/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.859475 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/
--rw-r--r--   0 runner    (1001) docker     (121)   119957 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/actb.png
--rw-r--r--   0 runner    (1001) docker     (121)   119284 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/actn1.png
--rw-r--r--   0 runner    (1001) docker     (121)   105165 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/atp2a2.png
--rw-r--r--   0 runner    (1001) docker     (121)   196144 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/cetn2.png
--rw-r--r--   0 runner    (1001) docker     (121)   103485 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/ctnnb1.png
--rw-r--r--   0 runner    (1001) docker     (121)   144903 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/dsp.png
--rw-r--r--   0 runner    (1001) docker     (121)   225879 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/fbl.png
--rw-r--r--   0 runner    (1001) docker     (121)   102554 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/gja1.png
--rw-r--r--   0 runner    (1001) docker     (121)   118205 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/h2b_interphase.png
--rw-r--r--   0 runner    (1001) docker     (121)   198065 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/lamp1.png
--rw-r--r--   0 runner    (1001) docker     (121)   251616 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/lmnb1_interphase.png
--rw-r--r--   0 runner    (1001) docker     (121)   109769 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/lmnb1_mitotic.png
--rw-r--r--   0 runner    (1001) docker     (121)   119504 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/myh10.png
--rw-r--r--   0 runner    (1001) docker     (121)   281131 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/npm1.png
--rw-r--r--   0 runner    (1001) docker     (121)   100628 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/nup153.png
--rw-r--r--   0 runner    (1001) docker     (121)   131886 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/pxn.png
--rw-r--r--   0 runner    (1001) docker     (121)   125306 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/rab5a.png
--rw-r--r--   0 runner    (1001) docker     (121)   105641 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/sec61b.png
--rw-r--r--   0 runner    (1001) docker     (121)   112810 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/slc25a17.png
--rw-r--r--   0 runner    (1001) docker     (121)   102251 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/smc1a.png
--rw-r--r--   0 runner    (1001) docker     (121)   194421 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/son.png
--rw-r--r--   0 runner    (1001) docker     (121)   259901 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/st6gal1.png
--rw-r--r--   0 runner    (1001) docker     (121)   105065 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/tjp1.png
--rw-r--r--   0 runner    (1001) docker     (121)   106508 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/tomm20.png
--rw-r--r--   0 runner    (1001) docker     (121)   103294 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/tuba1b.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.863474 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (121)    13694 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actb_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    40440 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actb_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    12840 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actn1_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    43915 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actn1_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    51634 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/atp2a2_post.png
--rw-r--r--   0 runner    (1001) docker     (121)   120036 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/atp2a2_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/cetn2_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    34859 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/cetn2_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     9946 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/ctnnb1_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    36703 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/ctnnb1_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     5619 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/dsp_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    29108 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/dsp_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     8659 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/fbl_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    28524 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/fbl_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     6163 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/gja1_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    25011 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/gja1_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    57305 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/h2b_interphase_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    92240 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/h2b_interphase_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     9011 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lamp1_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    37958 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lamp1_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     8499 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_interphase_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    29282 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_interphase_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    12450 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_mitotic_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    42177 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_mitotic_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    13686 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/myh10_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    42805 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/myh10_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     7288 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/npm1_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    28015 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/npm1_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    19476 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/nup153_post.png
--rw-r--r--   0 runner    (1001) docker     (121)   101130 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/nup153_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    13199 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/pxn_post.png
--rw-r--r--   0 runner    (1001) docker     (121)   134198 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/pxn_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/rab5a_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    79082 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/rab5a_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    14119 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/sec61b_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    44418 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/sec61b_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/slc25a17_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    49684 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/slc25a17_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    19657 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/smc1a_post.png
--rw-r--r--   0 runner    (1001) docker     (121)   122528 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/smc1a_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    27776 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/son_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    80160 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/son_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/st6gal1_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    44103 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/st6gal1_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)     8946 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tjp1_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    27919 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tjp1_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    10766 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tomm20_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    40641 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tomm20_pre.png
--rw-r--r--   0 runner    (1001) docker     (121)    22002 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tuba1b_post.png
--rw-r--r--   0 runner    (1001) docker     (121)    36865 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tuba1b_pre.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.867475 aicssegmentation-0.5.2/aicssegmentation/bin/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12168 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/bin/batch_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.867475 aicssegmentation-0.5.2/aicssegmentation/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/cli/to_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.867475 aicssegmentation-0.5.2/aicssegmentation/core/
--rw-r--r--   0 runner    (1001) docker     (121)     7252 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/MO_threshold.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/hessian.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/output_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7127 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/pre_processing_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/seg_dot.py
--rw-r--r--   0 runner    (1001) docker     (121)    16761 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11997 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/vessel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5789 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/core/visual.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.871475 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_actb.py
--rw-r--r--   0 runner    (1001) docker     (121)     5734 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_actn1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_atp2a2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_actn2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_atp2a2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_fbl.py
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_fbl_100x.py
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_myl7.py
--rw-r--r--   0 runner    (1001) docker     (121)     5941 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_npm1.py
--rw-r--r--   0 runner    (1001) docker     (121)     5950 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_npm1_100x.py
--rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_tnni1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4106 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_ttn.py
--rw-r--r--   0 runner    (1001) docker     (121)     5710 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cetn2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4307 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_ctnnb1.py
--rw-r--r--   0 runner    (1001) docker     (121)     5521 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_drug_npm1.py
--rw-r--r--   0 runner    (1001) docker     (121)     5119 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_dsp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5723 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_fbl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_fbl_labelfree_4dn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4549 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_gja1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_h2b_interphase.py
--rw-r--r--   0 runner    (1001) docker     (121)     5654 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_lamp1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_lmnb1_interphase.py
--rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_lmnb1_mitotic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_myh10.py
--rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_npm1.py
--rw-r--r--   0 runner    (1001) docker     (121)     5951 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_npm1_SR.py
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_npm_labelfree_4dn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_nup153.py
--rw-r--r--   0 runner    (1001) docker     (121)     5410 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_polr2a.py
--rw-r--r--   0 runner    (1001) docker     (121)     5260 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_polr2a_blob.py
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_pxn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_rab5a.py
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_sec61b.py
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_sec61b_dual.py
--rw-r--r--   0 runner    (1001) docker     (121)     5318 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_slc25a17.py
--rw-r--r--   0 runner    (1001) docker     (121)     3996 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_smc1a.py
--rw-r--r--   0 runner    (1001) docker     (121)     4706 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_son.py
--rw-r--r--   0 runner    (1001) docker     (121)     5494 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_st6gal1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     4818 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_terf2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4375 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_tjp1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_tomm20.py
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_tuba1b.py
--rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_ubtf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/structure_segmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.875475 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13838 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/all_functions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_actb.json
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_actn1.json
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_atp2a2.json
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_cetn2.json
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_ctnnb1.json
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_dsp.json
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_fbl.json
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_gja1.json
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_h2b_interphase.json
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_lamp1.json
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_lmnb1_interphase.json
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_lmnb1_mitotic.json
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_myh10.json
--rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_npm1.json
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_nup153.json
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_pxn.json
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_rab5a.json
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_sec61b.json
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_slc25a17.json
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_smc1a.json
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_son.json
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_st6gal1.json
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_tjp1.json
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_tomm20.json
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_tuba1b.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.875475 aicssegmentation-0.5.2/aicssegmentation/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/util/directories.py
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/util/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.875475 aicssegmentation-0.5.2/aicssegmentation/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6743 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/batch_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/segmenter_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     6346 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     7824 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     5368 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.851474 aicssegmentation-0.5.2/aicssegmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6295 2022-07-26 21:02:54.000000 aicssegmentation-0.5.2/aicssegmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9192 2022-07-26 21:02:54.000000 aicssegmentation-0.5.2/aicssegmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 21:02:54.000000 aicssegmentation-0.5.2/aicssegmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-26 21:02:54.000000 aicssegmentation-0.5.2/aicssegmentation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 21:02:54.000000 aicssegmentation-0.5.2/aicssegmentation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-07-26 21:02:54.000000 aicssegmentation-0.5.2/aicssegmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-26 21:02:54.000000 aicssegmentation-0.5.2/aicssegmentation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:54.875475 aicssegmentation-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5375 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/doc.rst
--rw-r--r--   0 runner    (1001) docker     (121)   155579 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/full.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   167525 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/full_mem.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   259125 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/full_str.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)    26263 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/rab5a_raw.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    49747 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/step1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    39781 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/step2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    25995 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/step3_p1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    61424 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/docs/step3_p2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-07-26 21:02:54.879475 aicssegmentation-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-07-26 21:02:50.000000 aicssegmentation-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.348363 aicssegmentation-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-20 16:18:51.348363 aicssegmentation-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.324363 aicssegmentation-0.5.3/aicssegmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.324363 aicssegmentation-0.5.3/aicssegmentation/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.328363 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)   119957 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/actb.png
+-rw-r--r--   0 runner    (1001) docker     (123)   119284 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/actn1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105165 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/atp2a2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196144 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/cetn2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   103485 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/ctnnb1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   144903 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/dsp.png
+-rw-r--r--   0 runner    (1001) docker     (123)   225879 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/fbl.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102554 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/gja1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118205 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/h2b_interphase.png
+-rw-r--r--   0 runner    (1001) docker     (123)   198065 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/lamp1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   251616 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/lmnb1_interphase.png
+-rw-r--r--   0 runner    (1001) docker     (123)   109769 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/lmnb1_mitotic.png
+-rw-r--r--   0 runner    (1001) docker     (123)   119504 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/myh10.png
+-rw-r--r--   0 runner    (1001) docker     (123)   281131 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/npm1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100628 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/nup153.png
+-rw-r--r--   0 runner    (1001) docker     (123)   131886 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/pxn.png
+-rw-r--r--   0 runner    (1001) docker     (123)   125306 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/rab5a.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105641 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/sec61b.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112810 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/slc25a17.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102251 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/smc1a.png
+-rw-r--r--   0 runner    (1001) docker     (123)   194421 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/son.png
+-rw-r--r--   0 runner    (1001) docker     (123)   259901 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/st6gal1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105065 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/tjp1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106508 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/tomm20.png
+-rw-r--r--   0 runner    (1001) docker     (123)   103294 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/tuba1b.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.336363 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actb_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actb_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actn1_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43915 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actn1_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51634 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/atp2a2_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)   120036 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/atp2a2_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/cetn2_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34859 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/cetn2_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/ctnnb1_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36703 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/ctnnb1_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/dsp_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29108 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/dsp_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/fbl_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/fbl_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/gja1_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/gja1_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57305 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/h2b_interphase_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    92240 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/h2b_interphase_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lamp1_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37958 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lamp1_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_interphase_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29282 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_interphase_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_mitotic_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42177 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_mitotic_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/myh10_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42805 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/myh10_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/npm1_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28015 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/npm1_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/nup153_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)   101130 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/nup153_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/pxn_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)   134198 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/pxn_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/rab5a_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79082 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/rab5a_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/sec61b_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44418 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/sec61b_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/slc25a17_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49684 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/slc25a17_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19657 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/smc1a_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)   122528 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/smc1a_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27776 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/son_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80160 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/son_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/st6gal1_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44103 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/st6gal1_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tjp1_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tjp1_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tomm20_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40641 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tomm20_pre.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22002 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tuba1b_post.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36865 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tuba1b_pre.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.336363 aicssegmentation-0.5.3/aicssegmentation/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/bin/batch_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.336363 aicssegmentation-0.5.3/aicssegmentation/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/cli/to_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.336363 aicssegmentation-0.5.3/aicssegmentation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/MO_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/pre_processing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/seg_dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/vessel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/core/visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.340363 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_actb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_actn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_atp2a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_actn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_atp2a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_fbl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_fbl_100x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_myl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_npm1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_npm1_100x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_tnni1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_ttn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cetn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_ctnnb1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_drug_npm1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_fbl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_fbl_labelfree_4dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_gja1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_h2b_interphase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_lamp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_lmnb1_interphase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_lmnb1_mitotic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_myh10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_npm1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_npm1_SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_npm_labelfree_4dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_nup153.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_polr2a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_polr2a_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_pxn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_rab5a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_sec61b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_sec61b_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_slc25a17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_smc1a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_son.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_st6gal1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_terf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_tjp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_tomm20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_tuba1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_ubtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/structure_segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.344363 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/all_functions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_actb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_actn1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_atp2a2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_cetn2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_ctnnb1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_dsp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_fbl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_gja1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_h2b_interphase.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_lamp1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_lmnb1_interphase.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_lmnb1_mitotic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_myh10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_npm1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_nup153.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_pxn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_rab5a.json
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_sec61b.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_slc25a17.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_smc1a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_son.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_st6gal1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_tjp1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_tomm20.json
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_tuba1b.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.344363 aicssegmentation-0.5.3/aicssegmentation/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/util/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/util/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.344363 aicssegmentation-0.5.3/aicssegmentation/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/batch_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/segmenter_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.324363 aicssegmentation-0.5.3/aicssegmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-20 16:18:51.000000 aicssegmentation-0.5.3/aicssegmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-06-20 16:18:51.000000 aicssegmentation-0.5.3/aicssegmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:18:51.000000 aicssegmentation-0.5.3/aicssegmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 16:18:51.000000 aicssegmentation-0.5.3/aicssegmentation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:18:51.000000 aicssegmentation-0.5.3/aicssegmentation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 16:18:51.000000 aicssegmentation-0.5.3/aicssegmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 16:18:51.000000 aicssegmentation-0.5.3/aicssegmentation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:51.348363 aicssegmentation-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/doc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   155579 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/full.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   167525 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/full_mem.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   259125 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/full_str.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    26263 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/rab5a_raw.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    49747 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/step1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39781 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/step2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    25995 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/step3_p1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    61424 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/docs/step3_p2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 16:18:51.348363 aicssegmentation-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-20 16:18:45.000000 aicssegmentation-0.5.3/setup.py
```

### Comparing `aicssegmentation-0.5.2/CONTRIBUTING.md` & `aicssegmentation-0.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/LICENSE` & `aicssegmentation-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/PKG-INFO` & `aicssegmentation-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicssegmentation
-Version: 0.5.2
+Version: 0.5.3
 Summary: Part 1 of Allen Cell and Structure Segmenter
 Home-page: https://github.com/AllenCell/aicssegmentation
 Author: Jianxu Chen
 Author-email: jianxuc@alleninstitute.org
 License: Allen Institute Software License
 Description: # aicssegmentation
```

### Comparing `aicssegmentation-0.5.2/README.md` & `aicssegmentation-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/actb.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/actb.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/actn1.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/actn1.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/atp2a2.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/atp2a2.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/cetn2.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/cetn2.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/ctnnb1.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/ctnnb1.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/dsp.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/dsp.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/fbl.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/fbl.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/gja1.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/gja1.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/h2b_interphase.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/h2b_interphase.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/lamp1.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/lamp1.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/lmnb1_interphase.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/lmnb1_interphase.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/lmnb1_mitotic.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/lmnb1_mitotic.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/myh10.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/myh10.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/npm1.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/npm1.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/nup153.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/nup153.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/pxn.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/pxn.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/rab5a.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/rab5a.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/sec61b.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/sec61b.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/slc25a17.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/slc25a17.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/smc1a.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/smc1a.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/son.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/son.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/st6gal1.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/st6gal1.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/tjp1.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/tjp1.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/tomm20.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/tomm20.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/diagrams/tuba1b.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/diagrams/tuba1b.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actb_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actb_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actb_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actb_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actn1_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actn1_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/actn1_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/actn1_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/atp2a2_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/atp2a2_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/atp2a2_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/atp2a2_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/cetn2_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/cetn2_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/cetn2_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/cetn2_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/ctnnb1_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/ctnnb1_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/ctnnb1_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/ctnnb1_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/dsp_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/dsp_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/dsp_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/dsp_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/fbl_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/fbl_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/fbl_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/fbl_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/gja1_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/gja1_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/gja1_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/gja1_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/h2b_interphase_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/h2b_interphase_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/h2b_interphase_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/h2b_interphase_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lamp1_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lamp1_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lamp1_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lamp1_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_interphase_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_interphase_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_interphase_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_interphase_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_mitotic_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_mitotic_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/lmnb1_mitotic_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/lmnb1_mitotic_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/myh10_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/myh10_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/myh10_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/myh10_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/npm1_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/npm1_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/npm1_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/npm1_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/nup153_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/nup153_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/nup153_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/nup153_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/pxn_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/pxn_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/pxn_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/pxn_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/rab5a_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/rab5a_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/rab5a_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/rab5a_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/sec61b_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/sec61b_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/sec61b_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/sec61b_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/slc25a17_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/slc25a17_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/slc25a17_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/slc25a17_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/smc1a_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/smc1a_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/smc1a_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/smc1a_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/son_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/son_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/son_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/son_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/st6gal1_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/st6gal1_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/st6gal1_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/st6gal1_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tjp1_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tjp1_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tjp1_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tjp1_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tomm20_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tomm20_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tomm20_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tomm20_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tuba1b_post.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tuba1b_post.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/assets/thumbnails/tuba1b_pre.png` & `aicssegmentation-0.5.3/aicssegmentation/assets/thumbnails/tuba1b_pre.png`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/bin/batch_processing.py` & `aicssegmentation-0.5.3/aicssegmentation/bin/batch_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,24 +165,23 @@
 
     def show_info(self):
         log.debug("Working Dir:")
         log.debug("\t{}".format(os.getcwd()))
         log.debug("Command Line:")
         log.debug("\t{}".format(" ".join(sys.argv)))
         log.debug("Args:")
-        for (k, v) in self.__dict__.items():
+        for k, v in self.__dict__.items():
             log.debug("\t{}: {}".format(k, v))
 
 
 ###############################################################################
 
 
 class Executor(object):
     def __init__(self, args):
-
         standard_xy = 0.108
 
         if args.rescale > 0:
             self.rescale_ratio = args.rescale
         else:
             if args.xy != standard_xy:
                 self.rescale_ratio = args.xy / standard_xy
@@ -270,15 +269,14 @@
 
         if not os.path.exists(output_path):
             os.mkdir(output_path)
 
         ##########################################################################
         batch_mode = False
         if args.mode == PER_IMAGE:
-
             fname = os.path.basename(os.path.splitext(args.input_fname)[0])
 
             image_reader = aicsimageio.AICSImage(args.input_fname)
             img = image_reader.data
             if len(img.shape) == 6:
                 struct_img = img[0, 0, args.struct_ch, :, :, :].astype(np.float32)
             else:
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/cli/to_analysis.py` & `aicssegmentation-0.5.3/aicssegmentation/cli/to_analysis.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/MO_threshold.py` & `aicssegmentation-0.5.3/aicssegmentation/core/MO_threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         th_low_level = np.percentile(structure_img_smooth, 50)
     elif global_thresh_method == "ave" or global_thresh_method == "ave_tri_med":
         global_tri = threshold_triangle(structure_img_smooth)
         global_median = np.percentile(structure_img_smooth, 50)
         th_low_level = (global_tri + global_median) / 2
 
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=object_minArea, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=object_minArea, connectivity=1, out=bw_low_level)
     if dilate:
-        bw_low_level = dilation(bw_low_level, selem=ball(2))
+        bw_low_level = dilation(bw_low_level, footprint=ball(2))
 
     return bw_low_level
 
 
 def MO_high_level(
     structure_img_smooth: np.ndarray,
     bw_low_level: np.ndarray,
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/hessian.py` & `aicssegmentation-0.5.3/aicssegmentation/core/hessian.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/output_utils.py` & `aicssegmentation-0.5.3/aicssegmentation/core/output_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         out_fn = str(output_path / (fn + suffix + "_contour.tiff"))
         OmeTiffWriter.save(data=bd, uri=out_fn, dim_order="ZYX")
 
 
 def generate_segmentation_contour(im):
     """generate the contour of the segmentation"""
 
-    bd = np.logical_xor(erosion(im > 0, selem=ball(1)), im > 0)
+    bd = np.logical_xor(erosion(im > 0, footprint=ball(1)), im > 0)
 
     bd = bd.astype(np.uint8)
     bd[bd > 0] = 255
 
     return bd
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/pre_processing_utils.py` & `aicssegmentation-0.5.3/aicssegmentation/core/pre_processing_utils.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/seg_dot.py` & `aicssegmentation-0.5.3/aicssegmentation/core/seg_dot.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/utils.py` & `aicssegmentation-0.5.3/aicssegmentation/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,37 +80,36 @@
     method: str
         either "3D" or "slice_by_slice", default is "3D"
     connnectivity: int
         the connectivity to use when computing object size
     """
     assert len(img.shape) == 3, "image has to be 3D"
     if method == "3D":
-        return remove_small_objects(img > 0, min_size=min_size, connectivity=connectivity, in_place=False)
+        return remove_small_objects(img > 0, min_size=min_size, connectivity=connectivity)
     elif method == "slice_by_slice":
         seg = np.zeros(img.shape, dtype=bool)
         for zz in range(img.shape[0]):
             seg[zz, :, :] = remove_small_objects(
                 img[zz, :, :] > 0,
                 min_size=min_size,
                 connectivity=connectivity,
-                in_place=False,
             )
         return seg
     else:
         raise NotImplementedError(f"unsupported method {method}")
 
 
 def topology_preserving_thinning(bw: np.ndarray, min_thickness: int = 1, thin: int = 1) -> np.ndarray:
     """perform thinning on segmentation without breaking topology
 
     Parameters:
     --------------
     bw: np.ndarray
         the 3D binary image to be thinned
-    min_thinkness: int
+    min_thickness: int
         Half of the minimum width you want to keep from being thinned.
         For example, when the object width is smaller than 4, you don't
         want to make this part even thinner (may break the thin object
         and alter the topology), you can set this value as 2.
     thin: int
         the amount to thin (has to be an positive integer). The number of
          pixels to be removed from outter boundary towards center.
@@ -419,16 +418,15 @@
     seg: List
         a list of segmentations, should all have the same shape
     """
 
     return np.logical_xor.reduce(seg)
 
 
-def remove_index_object(label: np.ndarray, id_to_remove: List[int] = [1], in_place=False):
-
+def remove_index_object(label: np.ndarray, id_to_remove: List[int] = [1], in_place: bool = False) -> np.ndarray:
     if in_place:
         img = label
     else:
         img = label.copy()
 
     for id in id_to_remove:
         img[img == id] = 0
@@ -450,15 +448,15 @@
     from skimage.measure import label
     from skimage.morphology import dilation, ball
     from skimage.segmentation import watershed
 
     distance = distance_transform_edt(bw)
     im_watershed = watershed(
         -distance,
-        label(dilation(local_maxi, selem=ball(1))),
+        label(dilation(local_maxi, footprint=ball(1))),
         mask=bw,
         watershed_line=True,
     )
     return im_watershed
 
 
 def prune_z_slices(bw: np.ndarray):
@@ -504,16 +502,16 @@
     from skimage.filters import threshold_triangle, threshold_otsu
     from skimage.morphology import dilation
 
     # cell-wise local adaptive thresholding
     th_low_level = threshold_triangle(structure_img_smooth)
 
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=cell_wise_min_area, connectivity=1, in_place=True)
-    bw_low_level = dilation(bw_low_level, selem=ball(2))
+    bw_low_level = remove_small_objects(bw_low_level, min_size=cell_wise_min_area, connectivity=1, out=bw_low_level)
+    bw_low_level = dilation(bw_low_level, footprint=ball(2))
 
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
 
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(structure_img_smooth[single_obj > 0])
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/vessel.py` & `aicssegmentation-0.5.3/aicssegmentation/core/vessel.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/core/visual.py` & `aicssegmentation-0.5.3/aicssegmentation/core/visual.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_actb.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_actb.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     response_1 = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma_1, tau=1, whiteonblack=True)
     response_2 = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma_2, tau=1, whiteonblack=True)
     bw = np.logical_or(response_1 > vesselness_cutoff_1, response_2 > vesselness_cutoff_2)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_actn1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_actn1.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     response_1 = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma_1, tau=1, whiteonblack=True)
     response_2 = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma_2, tau=1, whiteonblack=True)
     bw = np.logical_or(response_1 > vesselness_cutoff_1, response_2 > vesselness_cutoff_2)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_atp2a2.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_sec61b.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_atp2a2(
+def Workflow_sec61b(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure ATP2A2
+    classic segmentation workflow wrapper for structure SEC61B
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -44,17 +44,17 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [2.5, 9.0]
+    intensity_norm_param = [2.5, 7.5]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.25
+    vesselness_cutoff = 0.15
     minArea = 15
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
@@ -85,19 +85,19 @@
     # 2d vesselness slice by slice
     response = vesselnessSliceBySlice(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
     for zz in range(bw.shape[0]):
-        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1, in_place=False)
+        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1)
 
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_actn2.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_myl7.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_cardio_actn2(
+def Workflow_cardio_myl7(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure Cardio ACTN2
+    classic segmentation workflow wrapper for structure Cardio MYL7
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -44,17 +44,17 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [1, 19]
+    intensity_norm_param = [8, 15.5]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.02
+    vesselness_cutoff = 0.01
     minArea = 15
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
@@ -85,15 +85,15 @@
     # vesselness 3d
     response = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_atp2a2.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_actn2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_cardio_atp2a2(
+def Workflow_cardio_actn2(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure Cardio ATP2A2
+    classic segmentation workflow wrapper for structure Cardio ACTN2
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -44,17 +44,17 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [1, 20]
+    intensity_norm_param = [1, 19]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.002
+    vesselness_cutoff = 0.02
     minArea = 15
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
@@ -85,15 +85,15 @@
     # vesselness 3d
     response = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_fbl.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_fbl_100x.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_cardio_fbl(
+def Workflow_cardio_fbl_100x(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure Cardio FBL
+    classic segmentation workflow wrapper for structure Cardio FBL 100x
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -46,21 +46,21 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [0.5, 140]
+    intensity_norm_param = [0.5, 3]
     gaussian_smoothing_sigma = 1
     gaussian_smoothing_truncate_range = 3.0
     dot_2d_sigma = 1
     dot_2d_cutoff = 0.015
     minArea = 1
-    low_level_min_size = 1000
+    low_level_min_size = 600
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
@@ -95,45 +95,45 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(structure_img_smooth)
     global_median = np.percentile(structure_img_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
 
     # step 2: high level thresholding
     local_cutoff = 0.333 * threshold_otsu(structure_img_smooth)
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(structure_img_smooth[single_obj])
         if local_otsu > local_cutoff:
-            bw_high_level[np.logical_and(structure_img_smooth > local_otsu, single_obj)] = 1
+            bw_high_level[np.logical_and(structure_img_smooth > 1.1 * local_otsu, single_obj)] = 1
 
     out_img_list.append(bw_high_level.copy())
     out_name_list.append("interm_high")
 
     # step 3: finer segmentation
     response2d = dot_slice_by_slice(structure_img_smooth, log_sigma=dot_2d_sigma)
 
-    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1, in_place=True)
+    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1)
 
     out_img_list.append(bw_finer.copy())
     out_name_list.append("bw_fine")
 
-    # merge finer level detection into high level coarse segmentation to include
-    # outside dim parts
+    # merge finer level detection into high level coarse segmentation
+    # to include outside dim parts
     bw_high_level[bw_finer > 0] = 1
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_fbl_100x.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_fbl.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_cardio_fbl_100x(
+def Workflow_cardio_fbl(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure Cardio FBL 100x
+    classic segmentation workflow wrapper for structure Cardio FBL
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -46,21 +46,21 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [0.5, 3]
+    intensity_norm_param = [0.5, 140]
     gaussian_smoothing_sigma = 1
     gaussian_smoothing_truncate_range = 3.0
     dot_2d_sigma = 1
     dot_2d_cutoff = 0.015
     minArea = 1
-    low_level_min_size = 600
+    low_level_min_size = 1000
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
@@ -95,45 +95,45 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(structure_img_smooth)
     global_median = np.percentile(structure_img_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
 
     # step 2: high level thresholding
     local_cutoff = 0.333 * threshold_otsu(structure_img_smooth)
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(structure_img_smooth[single_obj])
         if local_otsu > local_cutoff:
-            bw_high_level[np.logical_and(structure_img_smooth > 1.1 * local_otsu, single_obj)] = 1
+            bw_high_level[np.logical_and(structure_img_smooth > local_otsu, single_obj)] = 1
 
     out_img_list.append(bw_high_level.copy())
     out_name_list.append("interm_high")
 
     # step 3: finer segmentation
     response2d = dot_slice_by_slice(structure_img_smooth, log_sigma=dot_2d_sigma)
 
-    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1, in_place=True)
+    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1)
 
     out_img_list.append(bw_finer.copy())
     out_name_list.append("bw_fine")
 
-    # merge finer level detection into high level coarse segmentation
-    # to include outside dim parts
+    # merge finer level detection into high level coarse segmentation to include
+    # outside dim parts
     bw_high_level[bw_finer > 0] = 1
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_myl7.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_tuba1b.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import numpy as np
 from typing import Union
 from pathlib import Path
-from skimage.morphology import remove_small_objects
+from aicssegmentation.core.vessel import vesselness3D
 from aicssegmentation.core.pre_processing_utils import (
     intensity_normalization,
     edge_preserving_smoothing_3d,
 )
-from aicssegmentation.core.vessel import vesselness3D
+from skimage.morphology import remove_small_objects
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_cardio_myl7(
+def Workflow_tuba1b(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure Cardio MYL7
+    classic segmentation workflow wrapper for structure TUBA1B
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -40,22 +40,23 @@
         3. array_with_contour: segmentation result will be returned together with
             the contour of the segmentation
         4. customize: pass in an extra output_func to do a special save. All the
             intermediate results, names of these results, the output_path, and the
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
+    ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [8, 15.5]
+    intensity_norm_param = [1.5, 8.0]
     vesselness_sigma = [1]
     vesselness_cutoff = 0.01
-    minArea = 15
+    minArea = 20
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
@@ -68,15 +69,15 @@
 
     # rescale if needed
     if rescale_ratio > 0:
         struct_img = zoom(struct_img, (1, rescale_ratio, rescale_ratio), order=2)
 
         struct_img = (struct_img - struct_img.min() + 1e-8) / (struct_img.max() - struct_img.min() + 1e-8)
 
-    # smoothing with gaussian filter
+    # smoothing with boundary preserving smoothing
     structure_img_smooth = edge_preserving_smoothing_3d(struct_img)
 
     out_img_list.append(structure_img_smooth.copy())
     out_name_list.append("im_smooth")
 
     ###################
     # core algorithm
@@ -85,15 +86,15 @@
     # vesselness 3d
     response = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_npm1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_npm1.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 
     # print(global_median)
     # print(global_tri)
     # print(th_low_level)
     # imsave('img_smooth.tiff', structure_img_smooth)
 
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
-    bw_low_level = dilation(bw_low_level, selem=ball(2))
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
+    bw_low_level = dilation(bw_low_level, footprint=ball(2))
 
     # step 2: high level thresholding
     local_cutoff = 0.333 * threshold_otsu(structure_img_smooth)
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
@@ -131,15 +131,15 @@
 
     bw_final = np.logical_or(bw_extra, bw_high_level)
     # bw_final[holes]=0
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1, in_place=True)
+    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_npm1_100x.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_npm1_100x.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 
     # print(global_median)
     # print(global_tri)
     # print(th_low_level)
     # imsave('img_smooth.tiff', structure_img_smooth)
 
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
-    bw_low_level = dilation(bw_low_level, selem=ball(2))
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
+    bw_low_level = dilation(bw_low_level, footprint=ball(2))
 
     # step 2: high level thresholding
     local_cutoff = 0.333 * threshold_otsu(structure_img_smooth)
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
@@ -131,15 +131,15 @@
 
     bw_final = np.logical_or(bw_extra, bw_high_level)
     # bw_final[holes]=0
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1, in_place=True)
+    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_tnni1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_atp2a2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import numpy as np
 from typing import Union
 from pathlib import Path
-from aicssegmentation.core.vessel import vesselness3D
+from skimage.morphology import remove_small_objects
 from aicssegmentation.core.pre_processing_utils import (
     intensity_normalization,
     edge_preserving_smoothing_3d,
 )
-from skimage.morphology import remove_small_objects
+from aicssegmentation.core.vessel import vesselness3D
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_cardio_tnni1(
+def Workflow_cardio_atp2a2(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure Cardio TNNI1
+    classic segmentation workflow wrapper for structure Cardio ATP2A2
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -44,17 +44,17 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [2, 11]
+    intensity_norm_param = [1, 20]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.01
+    vesselness_cutoff = 0.002
     minArea = 15
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
@@ -68,15 +68,15 @@
 
     # rescale if needed
     if rescale_ratio > 0:
         struct_img = zoom(struct_img, (1, rescale_ratio, rescale_ratio), order=2)
 
         struct_img = (struct_img - struct_img.min() + 1e-8) / (struct_img.max() - struct_img.min() + 1e-8)
 
-    # smoothing
+    # smoothing with gaussian filter
     structure_img_smooth = edge_preserving_smoothing_3d(struct_img)
 
     out_img_list.append(structure_img_smooth.copy())
     out_name_list.append("im_smooth")
 
     ###################
     # core algorithm
@@ -85,15 +85,15 @@
     # vesselness 3d
     response = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cardio_ttn.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_tnni1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import numpy as np
 from typing import Union
 from pathlib import Path
-from skimage.morphology import remove_small_objects
+from aicssegmentation.core.vessel import vesselness3D
 from aicssegmentation.core.pre_processing_utils import (
     intensity_normalization,
     edge_preserving_smoothing_3d,
 )
-from aicssegmentation.core.vessel import vesselness3D
+from skimage.morphology import remove_small_objects
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_cardio_ttn(
+def Workflow_cardio_tnni1(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure Cardio TTN
+    classic segmentation workflow wrapper for structure Cardio TNNI1
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -44,17 +44,17 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [8, 15.5]
+    intensity_norm_param = [2, 11]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.02
+    vesselness_cutoff = 0.01
     minArea = 15
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
@@ -68,15 +68,15 @@
 
     # rescale if needed
     if rescale_ratio > 0:
         struct_img = zoom(struct_img, (1, rescale_ratio, rescale_ratio), order=2)
 
         struct_img = (struct_img - struct_img.min() + 1e-8) / (struct_img.max() - struct_img.min() + 1e-8)
 
-    # smoothing with gaussian filter
+    # smoothing
     structure_img_smooth = edge_preserving_smoothing_3d(struct_img)
 
     out_img_list.append(structure_img_smooth.copy())
     out_name_list.append("im_smooth")
 
     ###################
     # core algorithm
@@ -85,15 +85,15 @@
     # vesselness 3d
     response = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_cetn2.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cetn2.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,37 +103,37 @@
     ###################
     # core algorithm
     ###################
 
     # step 1: LOG 3d
     response = dot_3d(structure_img_smooth_for_seg, log_sigma=dot_3d_sigma)
     bw = response > dot_3d_cutoff
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     out_img_list.append(bw.copy())
     out_name_list.append("interm_mask")
 
     # step 2: 'local_maxi + watershed' for cell cutting
     local_maxi = peak_local_max_wrapper(struct_img_for_peak, bw)
 
     out_img_list.append(local_maxi.copy())
     out_name_list.append("interm_local_max")
 
     distance = distance_transform_edt(bw)
     im_watershed = watershed(
         -distance,
-        label(dilation(local_maxi, selem=ball(1))),
+        label(dilation(local_maxi, footprint=ball(1))),
         mask=bw,
         watershed_line=True,
     )
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(im_watershed, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(im_watershed, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_ctnnb1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_ctnnb1.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     response = dot_slice_by_slice(structure_img_smooth, log_sigma=dot_2d_sigma)
     bw = response > dot_2d_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_drug_npm1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_drug_npm1.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(structure_img_smooth)
     global_median = np.percentile(structure_img_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
 
     # step 2: high level thresholding
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(structure_img_smooth[single_obj])
@@ -121,15 +121,15 @@
     # merge finer level detection into high level coarse segmentation to
     # include outside dim parts
     bw_high_level[bw_finer > 0] = 1
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_dsp.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_dsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,37 +94,37 @@
     ###################
     # core algorithm
     ###################
 
     # step 1: LOG 3d
     response = dot_3d(structure_img_smooth, log_sigma=dot_3d_sigma)
     bw = response > dot_3d_cutoff
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     out_img_list.append(bw.copy())
     out_name_list.append("interm_mask")
 
     # step 2: 'local_maxi + watershed' for cell cutting
     local_maxi = peak_local_max_wrapper(struct_img, bw)
 
     out_img_list.append(local_maxi.copy())
     out_name_list.append("interm_local_max")
 
     distance = distance_transform_edt(bw)
     im_watershed = watershed(
         -distance,
-        label(dilation(local_maxi, selem=ball(1))),
+        label(dilation(local_maxi, footprint=ball(1))),
         mask=bw,
         watershed_line=True,
     )
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(im_watershed, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(im_watershed, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_fbl.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_ubtf.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_fbl(
+def Workflow_ubtf(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure FBL
+    classic segmentation workflow wrapper for structure UBTF
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -46,30 +46,30 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [0.5, 18]
+    intensity_norm_param = [0.5, 30]
     gaussian_smoothing_sigma = 1
     gaussian_smoothing_truncate_range = 3.0
     dot_2d_sigma = 1
-    dot_2d_cutoff = 0.01  # 0.01 as default
+    dot_2d_cutoff = 0.03  # 0.01 as default
     minArea = 5
     low_level_min_size = 700
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
     ###################
-    # intenisty normalization
+    # intenisty normalization (min/max)
     struct_img = intensity_normalization(struct_img, scaling_param=intensity_norm_param)
 
     out_img_list.append(struct_img.copy())
     out_name_list.append("im_norm")
 
     # rescale if needed
     if rescale_ratio > 0:
@@ -95,42 +95,48 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(structure_img_smooth)
     global_median = np.percentile(structure_img_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
 
     # step 2: high level thresholding
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(structure_img_smooth[single_obj])
         bw_high_level[np.logical_and(structure_img_smooth > local_otsu, single_obj)] = 1
 
     out_img_list.append(bw_high_level.copy())
     out_name_list.append("interm_high")
 
     # step 3: finer segmentation
     response2d = dot_slice_by_slice(structure_img_smooth, log_sigma=dot_2d_sigma)
-    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1, in_place=True)
+    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1)
 
     out_img_list.append(bw_finer.copy())
     out_name_list.append("bw_fine")
 
+    if output_type == "return":
+        seg = bw_finer > 0
+        seg = seg.astype(np.uint8)
+        seg[seg > 0] = 255
+        return seg
+
     # merge finer level detection into high level coarse segmentation
     # to include outside dim parts
     bw_high_level[bw_finer > 0] = 1
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_fbl_labelfree_4dn.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_fbl_labelfree_4dn.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,37 +78,37 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(struct_smooth)
     global_median = np.percentile(struct_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = struct_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
 
     # step 2: high level thresholding
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(struct_smooth[single_obj])
         bw_high_level[np.logical_and(struct_smooth > local_otsu * 1.2, single_obj)] = 1
 
     # step 3: finer segmentation
     response2d = dot_2d_slice_by_slice_wrapper(struct_smooth, s2_param)
-    bw_finer = remove_small_objects(response2d, min_size=minArea, connectivity=1, in_place=True)
+    bw_finer = remove_small_objects(response2d, min_size=minArea, connectivity=1)
 
     # merge finer level detection into high level coarse segmentation
     # to include outside dim parts
     bw_high_level[bw_finer > 0] = 1
 
     ###################
     # POST-PROCESSING
     # make sure the variable name of final segmentation is 'seg'
     ###################
-    seg = remove_small_objects(bw_high_level, min_size=minArea, connectivity=1, in_place=True)
+    seg = remove_small_objects(bw_high_level, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_gja1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_gja1.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,20 +91,20 @@
     ###################
     # core algorithm
     ###################
 
     # step 1: LOG 3d
     response = dot_3d(structure_img_smooth, log_sigma=dot_3d_sigma)
     bw = response > dot_3d_cutoff
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_h2b_interphase.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_h2b_interphase.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     ###################
 
     bw = dot_2d_slice_by_slice_wrapper(structure_img_smooth, s2_param)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_lamp1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_lamp1.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         # too_small_mask = too_small[background_lab]
         # out[too_small_mask] = 0
 
         holes[zz, :, :] = out
 
     full_fill = np.logical_or(partial_fill, holes)
 
-    seg = remove_small_objects(full_fill, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(full_fill, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_lmnb1_interphase.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_lmnb1_interphase.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_lmnb1_mitotic.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_lmnb1_mitotic.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     # 2d filament filter on the middle frame
     bw = filament_2d_wrapper(structure_img_smooth, f2_param)
 
     ###################
     # POST-PROCESSING
     ###################
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = bw > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_myh10.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_myh10.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     response_1 = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma_1, tau=1, whiteonblack=True)
     response_2 = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma_2, tau=1, whiteonblack=True)
     bw = np.logical_or(response_1 > vesselness_cutoff_1, response_2 > vesselness_cutoff_2)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_npm1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_npm1.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,16 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(structure_img_smooth)
     global_median = np.percentile(structure_img_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
-    bw_low_level = dilation(bw_low_level, selem=ball(2))
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
+    bw_low_level = dilation(bw_low_level, footprint=ball(2))
 
     # step 2: high level thresholding
     local_cutoff = 0.333 * threshold_otsu(structure_img_smooth)
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
@@ -134,15 +134,15 @@
 
     bw_final = np.logical_or(bw_extra, bw_high_level)
     bw_final[holes] = 0
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1, in_place=True)
+    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_npm1_SR.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_npm1_SR.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,16 @@
 
     # step 1: low level thresholding
     global_tri = threshold_triangle(structure_img_smooth)
     global_median = np.percentile(structure_img_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
-    bw_low_level = dilation(bw_low_level, selem=ball(2))
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
+    bw_low_level = dilation(bw_low_level, footprint=ball(2))
 
     # step 2: high level thresholding
     local_cutoff = 0.333 * threshold_otsu(structure_img_smooth)
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
@@ -127,15 +127,15 @@
 
     bw_final = np.logical_or(bw_extra, bw_high_level)
     bw_final[holes] = 0
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1, in_place=True)
+    seg = remove_small_objects(bw_final, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_npm_labelfree_4dn.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_npm_labelfree_4dn.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,37 +80,37 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(struct_smooth)
     global_median = np.percentile(struct_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = struct_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
 
     # step 2: high level thresholding
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(struct_smooth[single_obj])
         bw_high_level[np.logical_and(struct_smooth > local_otsu * 1.2, single_obj)] = 1
 
     # step 3: finer segmentation
     response2d = dot_2d_slice_by_slice_wrapper(struct_smooth, s2_param)
-    bw_finer = remove_small_objects(response2d, min_size=minArea, connectivity=1, in_place=True)
+    bw_finer = remove_small_objects(response2d, min_size=minArea, connectivity=1)
 
     # merge finer level detection into high level coarse segmentation
     # to include outside dim parts
     bw_high_level[bw_finer > 0] = 1
 
     ###################
     # POST-PROCESSING
     # make sure the variable name of final segmentation is 'seg'
     ###################
-    seg = remove_small_objects(bw_high_level, min_size=minArea, connectivity=1, in_place=True)
+    seg = remove_small_objects(bw_high_level, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_nup153.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_nup153.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     bw = dot_3d_wrapper(structure_img_smooth, s3_param)
 
     # bw = dot_2d_slice_by_slice_wrapper(structure_img_smooth, s2_param)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint16)
     seg[seg > 0] = 65535
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_polr2a.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_polr2a.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,19 @@
     bw_large = np.logical_or(response_s3_3 > 0.2, response_f3 > 0.25)
     bw_dots = np.logical_or(np.logical_or(bw_small, bw_medium), bw_large)
     bw = np.logical_and(bw_dots, bw_otsu_mask)
 
     ###################
     # POST-PROCESSING
     ###################
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
     for zz in range(bw.shape[0]):
-        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1, in_place=False)
+        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1)
 
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     from aicssegmentation.core.utils import remove_hot_pixel
 
     seg = seg > 0
     seg_clean = remove_hot_pixel(seg)
     seg = seg_clean.astype(np.uint8)
     seg[seg > 0] = 255
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_polr2a_blob.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_polr2a_blob.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,37 +93,37 @@
     ###################
     # core algorithm
     ###################
 
     # step 1: LOG 3d
     response = dot_3d(structure_img_smooth, log_sigma=dot_3d_sigma)
     bw = response > dot_3d_cutoff
-    bw = remove_small_objects(bw > 0, min_size=min_area, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=min_area, connectivity=1)
 
     out_img_list.append(bw.copy())
     out_name_list.append("interm_mask")
 
     # step 2: 'local_maxi + watershed' for splitting objects
     local_maxi = peak_local_max_wrapper(struct_img, bw)
 
     out_img_list.append(local_maxi.copy())
     out_name_list.append("interm_local_max")
 
     distance = distance_transform_edt(bw)
     im_watershed = watershed(
         -distance,
-        label(dilation(local_maxi, selem=ball(1))),
+        label(dilation(local_maxi, footprint=ball(1))),
         mask=bw,
         watershed_line=True,
     )
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(im_watershed, min_size=min_area, connectivity=1, in_place=False)
+    seg = remove_small_objects(im_watershed, min_size=min_area, connectivity=1)
 
     # remove hot pixels from segmentation output
     seg = seg > 0
     seg_clean = remove_hot_pixel(seg)
     seg = seg_clean.astype(np.uint8)
     seg[seg > 0] = 255
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_pxn.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_pxn.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,17 @@
 
     ###################
     # POST-PROCESSING
     ###################
 
     seg = np.zeros_like(bw)
     for zz in range(bw.shape[0]):
-        seg[zz, :, :] = remove_small_objects(bw[zz, :, :] > 0, min_size=minArea2D, connectivity=1, in_place=False)
+        seg[zz, :, :] = remove_small_objects(bw[zz, :, :] > 0, min_size=minArea2D, connectivity=1)
 
-    seg = remove_small_objects(seg > 0, min_size=minArea3D, connectivity=1, in_place=False)
+    seg = remove_small_objects(seg > 0, min_size=minArea3D, connectivity=1)
 
     # determine z-range
     bw_z = np.zeros(bw.shape[0], dtype=np.uint16)
     for zz in range(bw.shape[0]):
         bw_z[zz] = np.count_nonzero(seg[zz, :, :] > 0)
 
     mid_z = np.argmax(bw_z)
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_rab5a.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_rab5a.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     # step 1: LOG 3d
     response = dot_3d(structure_img_smooth, log_sigma=dot_3d_sigma)
     bw = response > dot_3d_cutoff
 
     # step 2: fill holes and remove small objects
     bw_filled = hole_filling(bw, hole_min, hole_max, True)
-    seg = remove_small_objects(bw_filled, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw_filled, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_sec61b.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_sec61b_dual.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_sec61b(
+def Workflow_sec61b_dual(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure SEC61B
+    classic segmentation workflow wrapper for structure SEC61B dual
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -44,18 +44,18 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [2.5, 7.5]
+    intensity_norm_param = [2.0, 7.0]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.15
-    minArea = 15
+    vesselness_cutoff = 0.17
+    minArea = 20
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
@@ -85,19 +85,19 @@
     # 2d vesselness slice by slice
     response = vesselnessSliceBySlice(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
     for zz in range(bw.shape[0]):
-        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1, in_place=False)
+        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1)
 
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_sec61b_dual.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_atp2a2.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_sec61b_dual(
+def Workflow_atp2a2(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure SEC61B dual
+    classic segmentation workflow wrapper for structure ATP2A2
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -44,18 +44,18 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [2.0, 7.0]
+    intensity_norm_param = [2.5, 9.0]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.17
-    minArea = 20
+    vesselness_cutoff = 0.25
+    minArea = 15
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
@@ -85,19 +85,19 @@
     # 2d vesselness slice by slice
     response = vesselnessSliceBySlice(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
     for zz in range(bw.shape[0]):
-        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1, in_place=False)
+        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1)
 
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_slc25a17.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_slc25a17.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,37 +93,37 @@
     # core algorithm
     ###################
 
     # step 1: LOG 3d
     response = dot_3d(structure_img_smooth, log_sigma=dot_3d_sigma)
     bw = response > dot_3d_cutoff
 
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     out_img_list.append(bw.copy())
     out_name_list.append("interm_mask")
 
     # step 2: 'local_maxi + watershed' for cell cutting
     local_maxi = peak_local_max_wrapper(struct_img, bw)
 
     out_img_list.append(local_maxi.copy())
     out_name_list.append("interm_local_max")
 
     distance = distance_transform_edt(bw)
     im_watershed = watershed(
         -1 * distance,
-        label(dilation(local_maxi, selem=ball(1))),
+        label(dilation(local_maxi, footprint=ball(1))),
         mask=bw,
         watershed_line=True,
     )
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(im_watershed, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(im_watershed, min_size=minArea, connectivity=1)
 
     # HACK: Only for 2019 April Release #####
     if np.count_nonzero(seg > 0) < 50000:
         print("FLAG: please check the meta data of the original CZI for QC")
 
     # output
     seg = seg > 0
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_smc1a.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_smc1a.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     ###################
 
     bw = dot_2d_slice_by_slice_wrapper(structure_img_smooth, s2_param)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_son.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_son.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,19 +92,19 @@
     bw_medium = np.logical_or(bw_small, response_s3_1 > 0.07)
     bw_large = np.logical_or(response_s3_3 > 0.2, response_f3 > 0.25)
     bw = np.logical_or(np.logical_or(bw_small, bw_medium), bw_large)
 
     ###################
     # POST-PROCESSING
     ###################
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
     for zz in range(bw.shape[0]):
-        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1, in_place=False)
+        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1)
 
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
     out_name_list.append("bw_final")
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_st6gal1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_st6gal1.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,16 @@
     # core algorithm
     ###################
 
     # cell-wise local adaptive thresholding
     th_low_level = threshold_triangle(structure_img_smooth)
 
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=cell_wise_min_area, connectivity=1, in_place=True)
-    bw_low_level = dilation(bw_low_level, selem=ball(2))
+    bw_low_level = remove_small_objects(bw_low_level, min_size=cell_wise_min_area, connectivity=1)
+    bw_low_level = dilation(bw_low_level, footprint=ball(2))
 
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
 
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(structure_img_smooth[single_obj > 0])
@@ -119,15 +119,15 @@
 
     # combine the two parts
     bw = np.logical_or(bw_high_level, bw_extra)
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_template.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_template.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_terf2.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_terf2.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,19 +92,19 @@
     bw_medium = np.logical_or(bw_small, response_s3_1 > 0.07)
     bw_large = np.logical_or(response_s3_3 > 0.2, response_f3 > 0.25)
     bw = np.logical_or(np.logical_or(bw_small, bw_medium), bw_large)
 
     ###################
     # POST-PROCESSING
     ###################
-    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    bw = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
     for zz in range(bw.shape[0]):
-        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1, in_place=False)
+        bw[zz, :, :] = remove_small_objects(bw[zz, :, :], min_size=3, connectivity=1)
 
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     from aicssegmentation.core.utils import remove_hot_pixel
 
     seg = seg > 0
     seg_clean = remove_hot_pixel(seg)
     seg = seg_clean.astype(np.uint8)
     seg[seg > 0] = 255
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_tjp1.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_tjp1.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     # vesselness 3d
     response = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_tomm20.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_tomm20.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     # 2d vesselness slice by slice
     response = vesselnessSliceBySlice(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_tuba1b.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_cardio_ttn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import numpy as np
 from typing import Union
 from pathlib import Path
-from aicssegmentation.core.vessel import vesselness3D
+from skimage.morphology import remove_small_objects
 from aicssegmentation.core.pre_processing_utils import (
     intensity_normalization,
     edge_preserving_smoothing_3d,
 )
-from skimage.morphology import remove_small_objects
+from aicssegmentation.core.vessel import vesselness3D
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_tuba1b(
+def Workflow_cardio_ttn(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure TUBA1B
+    classic segmentation workflow wrapper for structure Cardio TTN
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -40,23 +40,22 @@
         3. array_with_contour: segmentation result will be returned together with
             the contour of the segmentation
         4. customize: pass in an extra output_func to do a special save. All the
             intermediate results, names of these results, the output_path, and the
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
-    ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [1.5, 8.0]
+    intensity_norm_param = [8, 15.5]
     vesselness_sigma = [1]
-    vesselness_cutoff = 0.01
-    minArea = 20
+    vesselness_cutoff = 0.02
+    minArea = 15
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
@@ -69,15 +68,15 @@
 
     # rescale if needed
     if rescale_ratio > 0:
         struct_img = zoom(struct_img, (1, rescale_ratio, rescale_ratio), order=2)
 
         struct_img = (struct_img - struct_img.min() + 1e-8) / (struct_img.max() - struct_img.min() + 1e-8)
 
-    # smoothing with boundary preserving smoothing
+    # smoothing with gaussian filter
     structure_img_smooth = edge_preserving_smoothing_3d(struct_img)
 
     out_img_list.append(structure_img_smooth.copy())
     out_name_list.append("im_smooth")
 
     ###################
     # core algorithm
@@ -86,15 +85,15 @@
     # vesselness 3d
     response = vesselness3D(structure_img_smooth, sigmas=vesselness_sigma, tau=1, whiteonblack=True)
     bw = response > vesselness_cutoff
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/seg_ubtf.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/seg_fbl.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from aicssegmentation.core.output_utils import (
     save_segmentation,
     generate_segmentation_contour,
 )
 from scipy.ndimage import zoom
 
 
-def Workflow_ubtf(
+def Workflow_fbl(
     struct_img: np.ndarray,
     rescale_ratio: float = -1,
     output_type: str = "default",
     output_path: Union[str, Path] = None,
     fn: Union[str, Path] = None,
     output_func=None,
 ):
     """
-    classic segmentation workflow wrapper for structure UBTF
+    classic segmentation workflow wrapper for structure FBL
 
     Parameter:
     -----------
     struct_img: np.ndarray
         the 3D image to be segmented
     rescale_ratio: float
         an optional parameter to allow rescale the image before running the
@@ -46,30 +46,30 @@
             original filename (without extension) will be passed in to output_func.
     """
     ##########################################################################
     # PARAMETERS:
     #   note that these parameters are supposed to be fixed for the structure
     #   and work well accross different datasets
 
-    intensity_norm_param = [0.5, 30]
+    intensity_norm_param = [0.5, 18]
     gaussian_smoothing_sigma = 1
     gaussian_smoothing_truncate_range = 3.0
     dot_2d_sigma = 1
-    dot_2d_cutoff = 0.03  # 0.01 as default
+    dot_2d_cutoff = 0.01  # 0.01 as default
     minArea = 5
     low_level_min_size = 700
     ##########################################################################
 
     out_img_list = []
     out_name_list = []
 
     ###################
     # PRE_PROCESSING
     ###################
-    # intenisty normalization (min/max)
+    # intenisty normalization
     struct_img = intensity_normalization(struct_img, scaling_param=intensity_norm_param)
 
     out_img_list.append(struct_img.copy())
     out_name_list.append("im_norm")
 
     # rescale if needed
     if rescale_ratio > 0:
@@ -95,48 +95,42 @@
     # step 1: low level thresholding
     # global_otsu = threshold_otsu(structure_img_smooth)
     global_tri = threshold_triangle(structure_img_smooth)
     global_median = np.percentile(structure_img_smooth, 50)
 
     th_low_level = (global_tri + global_median) / 2
     bw_low_level = structure_img_smooth > th_low_level
-    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, in_place=True)
+    bw_low_level = remove_small_objects(bw_low_level, min_size=low_level_min_size, connectivity=1, out=bw_low_level)
 
     # step 2: high level thresholding
     bw_high_level = np.zeros_like(bw_low_level)
     lab_low, num_obj = label(bw_low_level, return_num=True, connectivity=1)
     for idx in range(num_obj):
         single_obj = lab_low == (idx + 1)
         local_otsu = threshold_otsu(structure_img_smooth[single_obj])
         bw_high_level[np.logical_and(structure_img_smooth > local_otsu, single_obj)] = 1
 
     out_img_list.append(bw_high_level.copy())
     out_name_list.append("interm_high")
 
     # step 3: finer segmentation
     response2d = dot_slice_by_slice(structure_img_smooth, log_sigma=dot_2d_sigma)
-    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1, in_place=True)
+    bw_finer = remove_small_objects(response2d > dot_2d_cutoff, min_size=minArea, connectivity=1)
 
     out_img_list.append(bw_finer.copy())
     out_name_list.append("bw_fine")
 
-    if output_type == "return":
-        seg = bw_finer > 0
-        seg = seg.astype(np.uint8)
-        seg[seg > 0] = 255
-        return seg
-
     # merge finer level detection into high level coarse segmentation
     # to include outside dim parts
     bw_high_level[bw_finer > 0] = 1
 
     ###################
     # POST-PROCESSING
     ###################
-    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1, in_place=False)
+    seg = remove_small_objects(bw_high_level > 0, min_size=minArea, connectivity=1)
 
     # output
     seg = seg > 0
     seg = seg.astype(np.uint8)
     seg[seg > 0] = 255
 
     out_img_list.append(seg.copy())
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper/structure_segmenter.py` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper/structure_segmenter.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/all_functions.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/all_functions.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.838508064516129%*

 * *Differences: {"'absolute_3d_hessian_eigenvalues'": "OrderedDict([('name', 'Absolute 3d hessian eigenvalues'), "*

 * *                                      "('python::module', 'aicssegmentation.core.hessian'), "*

 * *                                      "('python::function', 'absolute_3d_hessian_eigenvalues'), "*

 * *                                      "('parameters', OrderedDict([('sigma', "*

 * *                                      "OrderedDict([('widget_type', 'slider'), ('data_type', "*

 * *                                      "'float') […]*

```diff
@@ -1,14 +1,80 @@
 {
+    "absolute_3d_hessian_eigenvalues": {
+        "name": "Absolute 3d hessian eigenvalues",
+        "parameters": {
+            "scale": {
+                "data_type": "bool",
+                "options": [
+                    true,
+                    false
+                ],
+                "widget_type": "drop-down"
+            },
+            "sigma": {
+                "data_type": "float",
+                "increment": 0.5,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "whiteonblack": {
+                "data_type": "bool",
+                "options": [
+                    true,
+                    false
+                ],
+                "widget_type": "drop-down"
+            }
+        },
+        "python::function": "absolute_3d_hessian_eigenvalues",
+        "python::module": "aicssegmentation.core.hessian"
+    },
+    "compute_3d_hessian_matrix": {
+        "name": "Compute 3D Hessian Matrix",
+        "parameters": {
+            "scale": {
+                "data_type": "bool",
+                "options": [
+                    true,
+                    false
+                ],
+                "widget_type": "drop-down"
+            },
+            "sigma": {
+                "data_type": "float",
+                "increment": 0.5,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "whiteonblack": {
+                "data_type": "bool",
+                "options": [
+                    true,
+                    false
+                ],
+                "widget_type": "drop-down"
+            }
+        },
+        "python::function": "compute_3d_hessian_matrix",
+        "python::module": "aicssegmentation.core.hessian"
+    },
     "edge_preserving_smoothing": {
         "name": "Edge Preserving Smoothing",
         "parameters": null,
         "python::function": "edge_preserving_smoothing_3d",
         "python::module": "aicssegmentation.core.pre_processing_utils"
     },
+    "erosion": {
+        "name": "Erosion",
+        "parameters": null,
+        "python::function": "erosion",
+        "python::module": "skimage.morphology"
+    },
     "extract_boundary_of_objects": {
         "name": "Extract Boundary of Objects",
         "parameters": {
             "connectivity": {
                 "data_type": "int",
                 "options": [
                     1,
@@ -258,14 +324,68 @@
                 "min": 0,
                 "widget_type": "slider"
             }
         },
         "python::function": "mask_image",
         "python::module": "aicssegmentation.core.utils"
     },
+    "masked_object_treshold_combined": {
+        "name": "Masked Object Threshold - Combined",
+        "parameters": {
+            "dilate": {
+                "data_type": "bool",
+                "options": [
+                    true,
+                    false
+                ],
+                "widget_type": "drop-down"
+            },
+            "extra_criteria": {
+                "data_type": "bool",
+                "options": [
+                    true,
+                    false
+                ],
+                "widget_type": "drop-down"
+            },
+            "global_thresh_method": {
+                "data_type": "str",
+                "options": [
+                    "triangle",
+                    "median",
+                    "ave_tri_med"
+                ],
+                "widget_type": "drop-down"
+            },
+            "local_adjust": {
+                "data_type": "float",
+                "increment": 0.02,
+                "max": 2,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "object_minArea": {
+                "data_type": "int",
+                "increment": 50,
+                "max": 2000,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "return_object": {
+                "data_type": "bool",
+                "options": [
+                    true,
+                    false
+                ],
+                "widget_type": "drop-down"
+            }
+        },
+        "python::function": "MO",
+        "python::module": "aicssegmentation.core.MO_threshold"
+    },
     "masked_object_treshold_high_level": {
         "name": "Masked Object Threshold - Part 2: high level",
         "parameters": {
             "extra_criteria": {
                 "data_type": "bool",
                 "options": [
                     true,
@@ -323,14 +443,20 @@
     },
     "prune_z_slices": {
         "name": "Prune Z-Slices",
         "parameters": null,
         "python::function": "prune_z_slices",
         "python::module": "aicssegmentation.core.utils"
     },
+    "remove_hot_pixel": {
+        "name": "Remove Hot Pixel",
+        "parameters": {},
+        "python::function": "remove_hot_pixel",
+        "python::module": "aicssegmentation.core.utils"
+    },
     "remove_index_object": {
         "name": "Remove Index Object",
         "parameters": null,
         "python::function": "remove_index_object",
         "python::module": "aicssegmentation.core.utils"
     },
     "segmentation_xor": {
@@ -404,24 +530,24 @@
         "python::module": "aicssegmentation.core.seg_dot"
     },
     "topology_preserving_thinning": {
         "name": "Topology Preserving Thinning",
         "parameters": {
             "min_thickness": {
                 "data_type": "int",
-                "increment": 0.2,
+                "increment": 1,
                 "max": 10,
-                "min": 0,
+                "min": 1,
                 "widget_type": "slider"
             },
             "thin": {
                 "data_type": "int",
                 "increment": 1,
-                "max": 50,
-                "min": 0,
+                "max": 200,
+                "min": 1,
                 "widget_type": "slider"
             }
         },
         "python::function": "topology_preserving_thinning",
         "python::module": "aicssegmentation.core.utils"
     },
     "watershed_for_cutting": {
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_actb.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_actb.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_actn1.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_actn1.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_atp2a2.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_atp2a2.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_cetn2.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_cetn2.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_ctnnb1.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_ctnnb1.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_dsp.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_dsp.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_fbl.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_fbl.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_gja1.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_gja1.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_h2b_interphase.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_h2b_interphase.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_lamp1.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_lamp1.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_lmnb1_interphase.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_lmnb1_interphase.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_lmnb1_mitotic.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_lmnb1_mitotic.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_myh10.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_myh10.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_npm1.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_npm1.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_nup153.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_nup153.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_pxn.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_pxn.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_rab5a.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_rab5a.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_sec61b.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_sec61b.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_slc25a17.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_slc25a17.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_smc1a.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_smc1a.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_son.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_son.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_st6gal1.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_st6gal1.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_tjp1.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_tjp1.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_tomm20.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_tomm20.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/structure_wrapper_config/conf_tuba1b.json` & `aicssegmentation-0.5.3/aicssegmentation/structure_wrapper_config/conf_tuba1b.json`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/util/directories.py` & `aicssegmentation-0.5.3/aicssegmentation/util/directories.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/workflow/batch_workflow.py` & `aicssegmentation-0.5.3/aicssegmentation/workflow/batch_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
         """
         if self._processed_files == 0:
             report = (
                 f"There were no files to process in the input directory to process \n "
                 f"Using the Workflow: {self._workflow_definition.name}"
             )
         else:
-
             files_processed = self._processed_files - self._failed_files
             report = (
                 f"{files_processed}/{self._processed_files} files were successfully processed \n "
                 f"Using the Workflow: {self._workflow_definition.name}"
             )
         self._write_to_log_file(report)
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation/workflow/segmenter_function.py` & `aicssegmentation-0.5.3/aicssegmentation/workflow/segmenter_function.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/workflow/workflow.py` & `aicssegmentation-0.5.3/aicssegmentation/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_config.py` & `aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_definition.py` & `aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_definition.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_engine.py` & `aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation/workflow/workflow_step.py` & `aicssegmentation-0.5.3/aicssegmentation/workflow/workflow_step.py`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation.egg-info/PKG-INFO` & `aicssegmentation-0.5.3/aicssegmentation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicssegmentation
-Version: 0.5.2
+Version: 0.5.3
 Summary: Part 1 of Allen Cell and Structure Segmenter
 Home-page: https://github.com/AllenCell/aicssegmentation
 Author: Jianxu Chen
 Author-email: jianxuc@alleninstitute.org
 License: Allen Institute Software License
 Description: # aicssegmentation
```

### Comparing `aicssegmentation-0.5.2/aicssegmentation.egg-info/SOURCES.txt` & `aicssegmentation-0.5.3/aicssegmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/aicssegmentation.egg-info/requires.txt` & `aicssegmentation-0.5.3/aicssegmentation.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 aicsimageio>=4.0.5
 scipy>=1.1.0
 numpy>=1.15.1
-scikit-image<0.19.0,>=0.18.0
+scikit-image
 pandas>=0.23.4
 itk
 itkwidgets
 jupyter
 matplotlib
 dask
 napari
 
 [all]
 aicsimageio>=4.0.5
 scipy>=1.1.0
 numpy>=1.15.1
-scikit-image<0.19.0,>=0.18.0
+scikit-image
 pandas>=0.23.4
 itk
 itkwidgets
 jupyter
 matplotlib
 dask
 napari
```

### Comparing `aicssegmentation-0.5.2/docs/Makefile` & `aicssegmentation-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/conf.py` & `aicssegmentation-0.5.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,17 @@
     ".md": "markdown",
 }
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"aicssegmentation"
-copyright = u"2020, Jianxu Chen"
-author = u"Jianxu Chen"
+project = "aicssegmentation"
+copyright = "2020, Jianxu Chen"
+author = "Jianxu Chen"
 
 # The version info for the project you"re documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = aicssegmentation.__version__
@@ -146,34 +146,34 @@
     # "figure_align": "htbp",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, "aicssegmentation.tex", u"aicssegmentation Documentation", u"Jianxu Chen", "manual"),
+    (master_doc, "aicssegmentation.tex", "aicssegmentation Documentation", "Jianxu Chen", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "aicssegmentation", u"aicssegmentation Documentation", [author], 1)]
+man_pages = [(master_doc, "aicssegmentation", "aicssegmentation Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
         "aicssegmentation",
-        u"aicssegmentation Documentation",
+        "aicssegmentation Documentation",
         author,
         "aicssegmentation",
         "One line description of project.",
         "Miscellaneous",
     ),
 ]
```

### Comparing `aicssegmentation-0.5.2/docs/full.jpg` & `aicssegmentation-0.5.3/docs/full.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/full_mem.jpg` & `aicssegmentation-0.5.3/docs/full_mem.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/full_str.jpg` & `aicssegmentation-0.5.3/docs/full_str.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/installation.rst` & `aicssegmentation-0.5.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/make.bat` & `aicssegmentation-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/rab5a_raw.jpg` & `aicssegmentation-0.5.3/docs/rab5a_raw.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/step1.jpg` & `aicssegmentation-0.5.3/docs/step1.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/step2.jpg` & `aicssegmentation-0.5.3/docs/step2.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/step3_p1.jpg` & `aicssegmentation-0.5.3/docs/step3_p1.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/docs/step3_p2.jpg` & `aicssegmentation-0.5.3/docs/step3_p2.jpg`

 * *Files identical despite different names*

### Comparing `aicssegmentation-0.5.2/setup.py` & `aicssegmentation-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "napari",
 ]
 
 requirements = [
     "aicsimageio>=4.0.5",
     "scipy>=1.1.0",
     "numpy>=1.15.1",
-    "scikit-image>=0.18.0,<0.19.0",
+    "scikit-image",
     "pandas>=0.23.4",
     "itk",
     "itkwidgets",
     "jupyter",
     "matplotlib",
     "dask",
     "napari",
@@ -92,10 +92,10 @@
     setup_requires=setup_requirements,
     test_suite="aicssegmentation/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/AllenCell/aicssegmentation",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="0.5.2",
+    version="0.5.3",
     zip_safe=False,
 )
```

