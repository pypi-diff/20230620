# Comparing `tmp/unigbsa-0.1.4.tar.gz` & `tmp/unigbsa-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unigbsa-0.1.4.tar", last modified: Fri Apr 14 15:52:50 2023, max compression
+gzip compressed data, was "unigbsa-0.1.5.tar", last modified: Tue Jun 20 03:22:56 2023, max compression
```

## Comparing `unigbsa-0.1.4.tar` & `unigbsa-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.982078 unigbsa-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 15:52:36.000000 unigbsa-0.1.4/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 15:52:36.000000 unigbsa-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-14 15:52:50.982078 unigbsa-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-14 15:52:36.000000 unigbsa-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.962078 unigbsa-0.1.4/launching/
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-04-14 15:52:36.000000 unigbsa-0.1.4/launching/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-14 15:52:36.000000 unigbsa-0.1.4/launching/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-14 15:52:36.000000 unigbsa-0.1.4/launching/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:52:50.982078 unigbsa-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-14 15:52:36.000000 unigbsa-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.962078 unigbsa-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-14 15:52:36.000000 unigbsa-0.1.4/tests/test_pipline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.962078 unigbsa-0.1.4/unigbsa/
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/CLI.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.970078 unigbsa-0.1.4/unigbsa/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.970078 unigbsa-0.1.4/unigbsa/data/Calibri/
--rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/Calibri/Calibri.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/Calibri/calibribold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/default.ini
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/default.json
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/mmpbsa.in
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/scan.json
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.974078 unigbsa-0.1.4/unigbsa/gbsa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/gbsarun.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.974078 unigbsa-0.1.4/unigbsa/scanparas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/scanparas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/scanparas/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.978078 unigbsa-0.1.4/unigbsa/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.978078 unigbsa-0.1.4/unigbsa/simulation/mdp/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/ions.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/md.mdp
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/mdout.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minim.mdp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.982078 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-cg.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-steep.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-cg.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-steep.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s3-steep.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s4-cg.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/npt.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/nvt.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/vaccum.mdp
--rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/openmm-em.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.966078 unigbsa-0.1.4/unigbsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.925210 unigbsa-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 03:22:41.000000 unigbsa-0.1.5/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 03:22:41.000000 unigbsa-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-06-20 03:22:56.925210 unigbsa-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-06-20 03:22:41.000000 unigbsa-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.913209 unigbsa-0.1.5/launching/
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-20 03:22:41.000000 unigbsa-0.1.5/launching/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-20 03:22:41.000000 unigbsa-0.1.5/launching/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-20 03:22:41.000000 unigbsa-0.1.5/launching/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:22:56.925210 unigbsa-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-20 03:22:41.000000 unigbsa-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.913209 unigbsa-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-20 03:22:41.000000 unigbsa-0.1.5/tests/test_pipline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.917209 unigbsa-0.1.5/unigbsa/
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.917209 unigbsa-0.1.5/unigbsa/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.917209 unigbsa-0.1.5/unigbsa/data/Calibri/
+-rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/data/Calibri/Calibri.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/data/Calibri/calibribold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/data/default.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/data/default.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/data/mmpbsa.in
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/data/scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/data/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.921210 unigbsa-0.1.5/unigbsa/gbsa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/gbsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/gbsa/gbsarun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/gbsa/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/gbsa/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/gbsa/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/gbsa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.921210 unigbsa-0.1.5/unigbsa/scanparas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/scanparas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/scanparas/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.921210 unigbsa-0.1.5/unigbsa/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.921210 unigbsa-0.1.5/unigbsa/simulation/mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/ions.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/md.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/mdout.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/minim.mdp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.921210 unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s1-cg.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s1-steep.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s2-cg.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s2-steep.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s3-steep.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s4-cg.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/npt.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/nvt.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdp/vaccum.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/mdrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/openmm-em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/simulation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 03:22:41.000000 unigbsa-0.1.5/unigbsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:22:56.917209 unigbsa-0.1.5/unigbsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-06-20 03:22:56.000000 unigbsa-0.1.5/unigbsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 03:22:56.000000 unigbsa-0.1.5/unigbsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:22:56.000000 unigbsa-0.1.5/unigbsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 03:22:56.000000 unigbsa-0.1.5/unigbsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:22:56.000000 unigbsa-0.1.5/unigbsa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 03:22:56.000000 unigbsa-0.1.5/unigbsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 03:22:56.000000 unigbsa-0.1.5/unigbsa.egg-info/top_level.txt
```

### Comparing `unigbsa-0.1.4/LICENCE.txt` & `unigbsa-0.1.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/PKG-INFO` & `unigbsa-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unigbsa
-Version: 0.1.4
+Version: 0.1.5
 Summary: MMPB(GB)SA tools for calculate energy.
 Home-page: https://github.com/dptech-corp/Uni-GBSA
 Author: dptech.net
 Author-email: hermite@dptech.net
 Keywords: MMPBSA MMGBSA
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
-Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening==============================================================================[[ChemRxiv](https://chemrxiv.org/engage/chemrxiv/article-details/63345399f764e656800664e7)]## BackgroudCalculating the binding free energy of a ligand to a protein receptor is a crucial goal in drug discovery. Molecular mechanics/Generalized-Born (Poisson–Boltzmann) surface area (MM/GB(PB)SA), which balances accuracy and efficiency, is one of the most widely used methods for evaluating ligand binding free energies in virtual screening. Uni-GBSA is an automatic workflow to perform MM/GB(PB)SA calculations. It includes several functions including but not limited to topology preparation, structure optimization, binding free energy calculation, and parameter scanning for MM/GB(PB)SA calculations. It also has a batch mode that allows the evaluation of thousands of molecules against one protein target simultaneously, enabling its application in virtual screening. ## Install### Install by condaTo run uni-GBSA, you need to install several third-party softwares including acpype, gmx_MMPBSA, lickit, etc.```Bashconda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacsconda activate gbsapip install unigbsa gmx_MMPBSA>=1.5.6 lickit```### Install by dokcer imagesYou can also build a dokcer image using this file or pull from the docker hub `docker pull dockerymh/unigbsa````PlaintextFROM continuumio/miniconda3# 1. create a enveriomentSHELL ["/bin/bash", "-c"]RUN conda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacs \&&  echo 'conda activate gbsa' >> ~/.bashrc \&&  rm -rf /opt/conda/pkgs/* # 2. install unigbsaRUN source ~/.bashrc \ &&  pip install unigbsa gmx_MMPBSA>=1.5.6 lickit \&&  rm -rf ~/.cache/*```## Usage & Example### Usage```bash$ unigbsa-pipeline -husage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD]                        [--decomp] [--verbose] [-v]GBSA Calculation. Version: 0.0.9_devoptions:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: /opt/miniconda3/envs/test/lib/python3.10/site-packages/unigbsa-0.0.9.dev0-py3.10.egg/unigbsa/data/default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.  -v, --version         show program's version number and exit```### Example```bash$ unigbsa-pipeline -i example/1ceb/1ceb_protein.pdb -l example/1ceb/1ceb_ligand.sdf -o BindingEnergy.csv10/08/2022 13:46:09 PM - INFO - Build protein topology.10/08/2022 13:46:10 PM - INFO - Build ligand topology: 1ceb_ligand1 molecule converted10/08/2022 13:46:13 PM - INFO - Running energy minimization: 1ceb_ligand10/08/2022 13:46:14 PM - INFO - Run the MMPB(GB)SA.10/08/2022 13:46:18 PM - INFO - Clean the results.================================================================================Results: Energy.csv Dec.csvFrames    mode    detal_G(kcal/mole)     1      gb              -20.4421```## Other ToolsThis packge contains many command lines: `unigbsa-scan`, `unigbsa-pipeline`, `unigbsa-traj`, `unigbsa-pbc`, `unigbsa-buildtop`, `unigbsa-buildsys`, `unigbsa-md`.### unigbsa-scan>An automatic parameter optimization prior to production MM/GB(PB)SA calculations.```Bashusage: unigbsa-scan [-h] [-i RECEPTOR] [-pd PROTDIR] [-l LIGAND [LIGAND ...]] [-ld LIGDIR] -e E -c PARASFILE [-o OUTDIR]                    [-nt THREAD] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -pd PROTDIR           Floder contains many protein files. file format: .pdb  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -ld LIGDIR            Floder contains many ligand files. file format: .mol or .sdf  -e E                  Experiment data file.  -c PARASFILE          Parameters to scan  -o OUTDIR             Output directory.  -nt THREAD            Set number of thread to run this program.  --verbose             Keep all the files.```>Example```Bashunigbsa-scan -i example/scan/protein.pdb -ld example/scan/ -e example/scan/ligands.csv -c example/scan/scan.json -o scan-demo -nt 4```### unigbsa-pipeline>A simple, automatic pipeline to perform MM/GB(PB)SA calculations. You only need to provide a protein file (in the PDB format) and ligand files (in the MOL or SDF format). This function will perform an energy minimization then calculate the PBSA/GBSA values for the each input ligand.* If you want perform energy minimization or MD simulation for the complex automatically, use the ``unigbsa-pipeline`` function.```Bashusage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD] [--decomp] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.```You can change the parameters for the MM/GB(PB)SA calculations by providing a configue file(`default.ini`). ```; parameters for simulation[simulation]; input pose process method: ;   input   -   just use input pose to calculation;   em      -   run a simple energy minimizaion for the input poses;   md      -   run a md simulation for the input posesmode = em; simulation box type: triclinic, cubic, dodecahedron, octahedronboxtype = triclinic; Distance between the solute and the simulation boxboxsize = 0.9; Specify salt concentration (mol/liter). This will add sufficient ions to reach up to the specified concentrationconc = 0.15; number of md simulation stepsnsteps = 500000; number of equilibrium simulation(nvt, npt) stepseqsteps = 50000; number of structure to save for the md simulationnframe = 100; protein forcefield (gromacs engine)proteinforcefield = amber03; ligand forcefield (acpype engine)ligandforcefield = gaff; ligand charge method: bcc, gasligandCharge = bcc; parameters for PBSA/GBSA calculation, support all the gmx_MMPBSA parameters[GBSA]; calculation namesys_name = GBSA; calculation mode, Separated by commas. gb,pb,decompositionmodes = gb; best parameters for PBSA/GBSA calculations obtained from Wang, Ercheng, et al. Chemical reviews 119.16 (2019): 9478-9508.igb = 2indi = 4.0exdi = 80.0```### unigbsa-traj>Perform a PBSA/GBSA calculation of a complex from a MD trajectory. Note: you need to prepare a gromacs `index.ndx` file which contains two groups named `RECEPTOR` and `LIGAND`.````unigbsa-traj -husage: unigbsa-traj [-h] -i INP -p TOP -ndx NDX [-m {gb,pb,pb+gb,gb+pb}] [-t TRAJ] [-indi INDI] [-dec] [-D]Free energy calcaulated by PBSA method.optional arguments:  -h, --help            show this help message and exit  -i INP                A pdb file or a tpr file for the trajectory.  -p TOP                Gromacs topol file for the system.  -ndx NDX              Gromacs index file, must contain recepror and ligand group.  -m {gb,pb,pb+gb,gb+pb}                        Method to calculate: gb, pb, pb+gb. default:gb  -t TRAJ               A trajectory file contains many structure frames. File format: xtc, pdb, gro...  -indi INDI            External dielectric constant. detault: 1.0  -dec                  Decompose the energy. default:false  -D                    DEBUG model, keep all the files.````### unigbsa-buildtop>Topology preparation for a protein receptor and ligand(s) using gromacs.```Bashunigbsa-buildtop -husage: unigbsa-buildtop [-h] [-p PROTEIN] [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-o OUTDIR] [-c] [-verbose]Build topology file for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file or directory to build topology.  -l LIGAND         Ligand file or directory to build topology.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -o OUTDIR         A output directory.  -c                Combine the protein and ligand topology. Suppport for one protein and more ligands. default:True  -verbose          Keep the directory or not.```### unigbsa-buildsys>Build a simulation box for a protein-ligand complex.```bashunigbsa-buildsys -husage: unigbsa-buildsys [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR]Build MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.```### unigbsa-md>Run a MD simulation of a protein-ligand complex.```Bashunigbsa-md -husage: unigbsa-md [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR] [-nstep NSTEP] [-nframe NFRAME] [-verbose]Run MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.  -nstep NSTEP      Simulation steps. default:2500  -nframe NFRAME    Number of frame to save for the xtc file. default:100  -verbose          Keep all the files in the simulation.```### unigbsa-pbc>Process PBC condition for a MD trajectory.```Bashunigbsa-pbc -husage: unigbsa-pbc [-h] -s TPR -f XTC [-o OUT] [-n NDX]Auto process PBC for gromacs MD trajector.optional arguments:  -h, --help  show this help message and exit  -s TPR      TPR file generated from gromacs or coordinate file.  -f XTC      Trajector file to process PBC.  -o OUT      Result file after processed PBC.  -n NDX      Index file contains the center and output group.```### More Examples* Perform a MM/GB(PB)SA calculation on a ligand file with a protein receptor with ``unigbsa-pipeline``````Bashunigbsa-pipeline -i ./example/2fvy/protein.pdb -l ./example/2fvy/BGC.mol2````* Perform a MM/GB(PB)SA calculation of a complex from a MD trajectory with ``unigbsa-traj`````Bashunigbsa-traj -i example/3f/complex.pdb -p example/3f/complex.top -ndx example/3f/index.ndx -m pb gb -t example/3f/complex.pdb```* Build topology for a protein receptor and a ligand using gromacs. ``unigbsa-buildtop`````bashunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -o topol  # build gromacs topology for a single proteinunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -l example/2fvy/BGC.mol2 -lf gaff -o 2fvy_topol -c # build gromacs topology for protein and ligand complex```* Build a simulation system with ``unigbsa-buildsys``* Run a MD simulation with ``unigbsa-md``* Process the PBC condition of a MD trjectorywith ``unigbsa-pbc``## Citation```plaintextYang M, Wang D, Zheng H. Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening. ChemRxiv. Cambridge: Cambridge Open Engage; 2022; This content is a preprint and has not been peer-reviewed.```
+Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening==============================================================================[[Briefings in Bioinformatics](https://academic.oup.com/bib/advance-article/doi/10.1093/bib/bbad218/7199492)]## BackgroudCalculating the binding free energy of a ligand to a protein receptor is a crucial goal in drug discovery. Molecular mechanics/Generalized-Born (Poisson–Boltzmann) surface area (MM/GB(PB)SA), which balances accuracy and efficiency, is one of the most widely used methods for evaluating ligand binding free energies in virtual screening. Uni-GBSA is an automatic workflow to perform MM/GB(PB)SA calculations. It includes several functions including but not limited to topology preparation, structure optimization, binding free energy calculation, and parameter scanning for MM/GB(PB)SA calculations. It also has a batch mode that allows the evaluation of thousands of molecules against one protein target simultaneously, enabling its application in virtual screening. ## Install### Install by condaTo run uni-GBSA, you need to install several third-party softwares including acpype, gmx_MMPBSA, lickit, etc.```Bashconda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacsconda activate gbsapip install unigbsa gmx_MMPBSA>=1.5.6 lickit```### Install by docker imagesYou can also build a docker image using this file or pull from the docker hub `docker pull dockerymh/unigbsa````PlaintextFROM continuumio/miniconda3# 1. create a enveriomentSHELL ["/bin/bash", "-c"]RUN conda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacs \&&  echo 'conda activate gbsa' >> ~/.bashrc \&&  rm -rf /opt/conda/pkgs/* # 2. install unigbsaRUN source ~/.bashrc \ &&  pip install unigbsa gmx_MMPBSA>=1.5.6 lickit \&&  rm -rf ~/.cache/*```## Usage & Example### Usage```bash$ unigbsa-pipeline -husage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD]                        [--decomp] [--verbose] [-v]GBSA Calculation. Version: 0.0.9_devoptions:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: /opt/miniconda3/envs/test/lib/python3.10/site-packages/unigbsa-0.0.9.dev0-py3.10.egg/unigbsa/data/default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.  -v, --version         show program's version number and exit```### Example```bash$ unigbsa-pipeline -i example/1ceb/1ceb_protein.pdb -l example/1ceb/1ceb_ligand.sdf -o BindingEnergy.csv10/08/2022 13:46:09 PM - INFO - Build protein topology.10/08/2022 13:46:10 PM - INFO - Build ligand topology: 1ceb_ligand1 molecule converted10/08/2022 13:46:13 PM - INFO - Running energy minimization: 1ceb_ligand10/08/2022 13:46:14 PM - INFO - Run the MMPB(GB)SA.10/08/2022 13:46:18 PM - INFO - Clean the results.================================================================================Results: Energy.csv Dec.csvFrames    mode    detal_G(kcal/mole)     1      gb              -20.4421```## Other ToolsThis packge contains several commands: `unigbsa-scan`, `unigbsa-pipeline`, `unigbsa-traj`, `unigbsa-pbc`, `unigbsa-buildtop`, `unigbsa-buildsys`, `unigbsa-md`.### unigbsa-scan>Perform an automatic parameter optimization prior to production MM/GB(PB)SA calculations.```Bashusage: unigbsa-scan [-h] [-i RECEPTOR] [-pd PROTDIR] [-l LIGAND [LIGAND ...]] [-ld LIGDIR] -e E -c PARASFILE [-o OUTDIR]                    [-nt THREAD] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -pd PROTDIR           Floder contains many protein files. file format: .pdb  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -ld LIGDIR            Floder contains many ligand files. file format: .mol or .sdf  -e E                  Experiment data file.  -c PARASFILE          Parameters to scan  -o OUTDIR             Output directory.  -nt THREAD            Set number of thread to run this program.  --verbose             Keep all the files.```>Example```Bashunigbsa-scan -i example/scan/protein.pdb -ld example/scan/ -e example/scan/ligands.csv -c example/scan/scan.json -o scan-demo -nt 4```### unigbsa-pipeline>A simple, automatic pipeline to perform MM/GB(PB)SA calculations. You only need to provide a protein file (in the PDB format) and ligand files (in the MOL or SDF format). This function will perform an energy minimization then calculate the PBSA/GBSA values for the each input ligand.* If you want perform energy minimization or MD simulation for the complex automatically, use the ``unigbsa-pipeline`` function.```Bashusage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD] [--decomp] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.```You can change the parameters for the MM/GB(PB)SA calculations by providing a configue file(`default.ini`). ```; parameters for simulation[simulation]; input pose process method: ;   input   -   just use input pose to calculation;   em      -   run a simple energy minimizaion for the input poses;   md      -   run a md simulation for the input posesmode = em; simulation box type: triclinic, cubic, dodecahedron, octahedronboxtype = triclinic; Distance between the solute and the simulation boxboxsize = 0.9; Specify salt concentration (mol/liter). This will add sufficient ions to reach up to the specified concentrationconc = 0.15; number of md simulation stepsnsteps = 500000; number of equilibrium simulation(nvt, npt) stepseqsteps = 50000; number of structure to save for the md simulationnframe = 100; protein forcefield (gromacs engine)proteinforcefield = amber03; ligand forcefield (acpype engine)ligandforcefield = gaff; ligand charge method: bcc, gasligandCharge = bcc; parameters for PBSA/GBSA calculation, support all the gmx_MMPBSA parameters[GBSA]; calculation namesys_name = GBSA; calculation mode, Separated by commas. gb,pb,decompositionmodes = gb; best parameters for PBSA/GBSA calculations obtained from Wang, Ercheng, et al. Chemical reviews 119.16 (2019): 9478-9508.igb = 2indi = 4.0exdi = 80.0```### unigbsa-traj>Perform a PBSA/GBSA calculation of a complex from a MD trajectory. Note: you need to prepare a gromacs `index.ndx` file which contains two groups named `RECEPTOR` and `LIGAND`.````unigbsa-traj -husage: unigbsa-traj [-h] -i INP -p TOP -ndx NDX [-m {gb,pb,pb+gb,gb+pb}] [-t TRAJ] [-indi INDI] [-dec] [-D]Free energy calcaulated by PBSA method.optional arguments:  -h, --help            show this help message and exit  -i INP                A pdb file or a tpr file for the trajectory.  -p TOP                Gromacs topol file for the system.  -ndx NDX              Gromacs index file, must contain recepror and ligand group.  -m {gb,pb,pb+gb,gb+pb}                        Method to calculate: gb, pb, pb+gb. default:gb  -t TRAJ               A trajectory file contains many structure frames. File format: xtc, pdb, gro...  -indi INDI            External dielectric constant. detault: 1.0  -dec                  Decompose the energy. default:false  -D                    DEBUG model, keep all the files.````### unigbsa-buildtop>Topology preparation for a protein receptor and ligand(s) using gromacs.```Bashunigbsa-buildtop -husage: unigbsa-buildtop [-h] [-p PROTEIN] [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-o OUTDIR] [-c] [-verbose]Build topology file for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file or directory to build topology.  -l LIGAND         Ligand file or directory to build topology.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -o OUTDIR         A output directory.  -c                Combine the protein and ligand topology. Suppport for one protein and more ligands. default:True  -verbose          Keep the directory or not.```### unigbsa-buildsys>Build a simulation box for a protein-ligand complex.```bashunigbsa-buildsys -husage: unigbsa-buildsys [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR]Build MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.```### unigbsa-md>Run a MD simulation of a protein-ligand complex.```Bashunigbsa-md -husage: unigbsa-md [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR] [-nstep NSTEP] [-nframe NFRAME] [-verbose]Run MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.  -nstep NSTEP      Simulation steps. default:2500  -nframe NFRAME    Number of frame to save for the xtc file. default:100  -verbose          Keep all the files in the simulation.```### unigbsa-pbc>Process PBC condition for a MD trajectory.```Bashunigbsa-pbc -husage: unigbsa-pbc [-h] -s TPR -f XTC [-o OUT] [-n NDX]Auto process PBC for gromacs MD trajector.optional arguments:  -h, --help  show this help message and exit  -s TPR      TPR file generated from gromacs or coordinate file.  -f XTC      Trajector file to process PBC.  -o OUT      Result file after processed PBC.  -n NDX      Index file contains the center and output group.```### More Examples* Perform a MM/GB(PB)SA calculation on a ligand file with a protein receptor with ``unigbsa-pipeline``````Bashunigbsa-pipeline -i ./example/2fvy/protein.pdb -l ./example/2fvy/BGC.mol2````* Perform a MM/GB(PB)SA calculation of a complex from a MD trajectory with ``unigbsa-traj`````Bashunigbsa-traj -i example/3f/complex.pdb -p example/3f/complex.top -ndx example/3f/index.ndx -m pb gb -t example/3f/complex.pdb```* Build topology for a protein receptor and a ligand using gromacs. ``unigbsa-buildtop`````bashunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -o topol  # build gromacs topology for a single proteinunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -l example/2fvy/BGC.mol2 -lf gaff -o 2fvy_topol -c # build gromacs topology for protein and ligand complex```* Build a simulation system with ``unigbsa-buildsys``* Run a MD simulation with ``unigbsa-md``* Process the PBC condition of a MD trjectorywith ``unigbsa-pbc``## Citation```plaintextMaohua Yang and others, Uni-GBSA: an open-source and web-based automatic workflow to perform MM/GB(PB)SA calculations for virtual screening, Briefings in Bioinformatics, 2023;, bbad218, https://doi.org/10.1093/bib/bbad218.```
```

### Comparing `unigbsa-0.1.4/README.md` & `unigbsa-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening
 ==============================================================================
 
-[[ChemRxiv](https://chemrxiv.org/engage/chemrxiv/article-details/63345399f764e656800664e7)]
+[[Briefings in Bioinformatics](https://academic.oup.com/bib/advance-article/doi/10.1093/bib/bbad218/7199492)]
 
 ## Backgroud
 
 Calculating the binding free energy of a ligand to a protein receptor is a crucial goal in drug discovery. Molecular mechanics/Generalized-Born (Poisson–Boltzmann) surface area (MM/GB(PB)SA), which balances accuracy and efficiency, is one of the most widely used methods for evaluating ligand binding free energies in virtual screening. Uni-GBSA is an automatic workflow to perform MM/GB(PB)SA calculations. It includes several functions including but not limited to topology preparation, structure optimization, binding free energy calculation, and parameter scanning for MM/GB(PB)SA calculations. It also has a batch mode that allows the evaluation of thousands of molecules against one protein target simultaneously, enabling its application in virtual screening. 
 
 ## Install
 ### Install by conda
 To run uni-GBSA, you need to install several third-party softwares including acpype, gmx_MMPBSA, lickit, etc.
 ```Bash
 conda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacs
 conda activate gbsa
 pip install unigbsa gmx_MMPBSA>=1.5.6 lickit
 ```
 
-### Install by dokcer images
-You can also build a dokcer image using this file or pull from the docker hub `docker pull dockerymh/unigbsa`
+### Install by docker images
+You can also build a docker image using this file or pull from the docker hub `docker pull dockerymh/unigbsa`
 ```Plaintext
 FROM continuumio/miniconda3
 
 # 1. create a enverioment
 SHELL ["/bin/bash", "-c"]
 RUN conda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacs \
 &&  echo 'conda activate gbsa' >> ~/.bashrc \
@@ -73,18 +73,18 @@
 Results: Energy.csv Dec.csv
 Frames    mode    detal_G(kcal/mole)
      1      gb              -20.4421
 
 ```
 
 ## Other Tools
-This packge contains many command lines: `unigbsa-scan`, `unigbsa-pipeline`, `unigbsa-traj`, `unigbsa-pbc`, `unigbsa-buildtop`, `unigbsa-buildsys`, `unigbsa-md`.
+This packge contains several commands: `unigbsa-scan`, `unigbsa-pipeline`, `unigbsa-traj`, `unigbsa-pbc`, `unigbsa-buildtop`, `unigbsa-buildsys`, `unigbsa-md`.
 
 ### unigbsa-scan
->An automatic parameter optimization prior to production MM/GB(PB)SA calculations.
+>Perform an automatic parameter optimization prior to production MM/GB(PB)SA calculations.
 ```Bash
 usage: unigbsa-scan [-h] [-i RECEPTOR] [-pd PROTDIR] [-l LIGAND [LIGAND ...]] [-ld LIGDIR] -e E -c PARASFILE [-o OUTDIR]
                     [-nt THREAD] [--verbose]
 
 GBSA Calculation.
 
 optional arguments:
@@ -306,9 +306,9 @@
 * Run a MD simulation with ``unigbsa-md``
 
 * Process the PBC condition of a MD trjectorywith ``unigbsa-pbc``
 
 
 ## Citation
 ```plaintext
-Yang M, Wang D, Zheng H. Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening. ChemRxiv. Cambridge: Cambridge Open Engage; 2022; This content is a preprint and has not been peer-reviewed.
+Maohua Yang and others, Uni-GBSA: an open-source and web-based automatic workflow to perform MM/GB(PB)SA calculations for virtual screening, Briefings in Bioinformatics, 2023;, bbad218, https://doi.org/10.1093/bib/bbad218.
 ```
```

### Comparing `unigbsa-0.1.4/launching/app.py` & `unigbsa-0.1.5/launching/app.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/launching/pipeline.py` & `unigbsa-0.1.5/launching/pipeline.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/launching/scan.py` & `unigbsa-0.1.5/launching/scan.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/setup.py` & `unigbsa-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/tests/test_pipline.py` & `unigbsa-0.1.5/tests/test_pipline.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/CLI.py` & `unigbsa-0.1.5/unigbsa/CLI.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/data/Calibri/Calibri.ttf` & `unigbsa-0.1.5/unigbsa/data/Calibri/Calibri.ttf`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/data/Calibri/calibribold.ttf` & `unigbsa-0.1.5/unigbsa/data/Calibri/calibribold.ttf`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/data/default.ini` & `unigbsa-0.1.5/unigbsa/data/default.ini`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/data/default.json` & `unigbsa-0.1.5/unigbsa/data/default.json`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/data/mmpbsa.in` & `unigbsa-0.1.5/unigbsa/data/mmpbsa.in`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/data/scan.json` & `unigbsa-0.1.5/unigbsa/data/scan.json`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/data/template.json` & `unigbsa-0.1.5/unigbsa/data/template.json`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/gbsa/gbsarun.py` & `unigbsa-0.1.5/unigbsa/gbsa/gbsarun.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/gbsa/io.py` & `unigbsa-0.1.5/unigbsa/gbsa/io.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/gbsa/parameters.py` & `unigbsa-0.1.5/unigbsa/gbsa/parameters.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/gbsa/plots.py` & `unigbsa-0.1.5/unigbsa/gbsa/plots.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/gbsa/utils.py` & `unigbsa-0.1.5/unigbsa/gbsa/utils.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/pipeline.py` & `unigbsa-0.1.5/unigbsa/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,42 +140,43 @@
         if len(ligandfiles) == 1:
             traceback.print_exc()
             logging.warning('Failed to generate forcefield for ligand: %s' % ligandName)
             exit(256)
     if len(ligandfiles) == 1:
         logging.info('Running energy minimization: %s' % ligandName)
     engine = GMXEngine()
-    try:
-        minimgro, outtop = engine.run_to_minim(grofile, topfile,
-                                               boxtype=simParas['boxtype'],
-                                               boxsize=simParas['boxsize'],
-                                               conc=simParas['conc'],
-                                               maxsol=simParas['maxsol'],
-                                               nt=1)
-        cmd = '%s editconf -f %s -o %s -resnr 1 >/dev/null 2>&1' % (GMXEXE, minimgro, grofile)
-        RC = os.system(cmd)
-        if RC != 0:
-            raise Exception('Error convert %s to %s'%(minimgro, grofile))
-        shutil.copy(topfile, outtop)
-    except Exception as e:
-        if len(ligandfiles) == 1:
-            traceback.print_exc()
-            logging.warning('Failed to run simulation for ligand: %s' % ligandName)
-            exit(256)
-        statu = 'F_md'
-    indexfile = generate_index_file(grofile)
     if statu == 'S':
         try:
+            minimgro, outtop = engine.run_to_minim(grofile, topfile,
+                                                   boxtype=simParas['boxtype'],
+                                                   boxsize=simParas['boxsize'],
+                                                   conc=simParas['conc'],
+                                                   maxsol=simParas['maxsol'],
+                                                   nt=1)
+            cmd = '%s editconf -f %s -o %s -resnr 1 >/dev/null 2>&1' % (GMXEXE, minimgro, grofile)
+            RC = os.system(cmd)
+            if RC != 0:
+                raise Exception('Error convert %s to %s'%(minimgro, grofile))
+            shutil.copy(topfile, outtop)
+        except Exception as e:
+            if len(ligandfiles) == 1:
+                traceback.print_exc()
+                logging.warning('Failed to run simulation for ligand: %s' % ligandName)
+                exit(256)
+            statu = 'F_md'
+    if statu == 'S':
+        try:
+            indexfile = generate_index_file(grofile)
             d1 = traj_pipeline(grofile, trajfile=grofile, topolfile=topfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, verbose=verbose, nt=nt, input_pdb=receptorfile)
         except:
             if len(ligandfiles) == 1:
                 logging.warning('Failed to run GBSA for ligand: %s'%ligandName)
                 traceback.print_exc()
             statu = 'F_GBSA'
-    if not verbose:
+    if not verbose and statu == 'S':
         engine.clean(pdbfile=grofile)
     os.chdir(cwd)
     d1['ligandName'] = ligandName
     d1['status'] = statu
     return d1
 
 def minim_pipeline(receptorfile, ligandfiles, paras, mmpbsafile=None, nt=1, outfile='BindingEnergy.csv', verbose=False):
```

### Comparing `unigbsa-0.1.4/unigbsa/scanparas/scan.py` & `unigbsa-0.1.5/unigbsa/scanparas/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 def calc_R2(expfile, gbsa):
     exp = pd.read_csv(expfile)
     if isinstance(gbsa, str):
         GBSA = pd.read_csv(gbsa)
     else:
         GBSA = gbsa
     df = pd.merge(exp, GBSA, on='ligandName')
-    R  = df.corr().loc['TOTAL', 'dG_exp']
+    R  = df[['TOTAL', 'dG_exp']].corr().loc['TOTAL', 'dG_exp']
     return R, R**2
 
 def iter_paras(args) -> None:
     '''
     '''
     from unigbsa.pipeline import minim_pipeline, md_pipeline, base_pipeline
     receptor, ligands, name, paras, outfile, expdatfile, verbose, nt = args
```

### Comparing `unigbsa-0.1.4/unigbsa/settings.py` & `unigbsa-0.1.5/unigbsa/settings.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/ions.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/ions.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/md.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/md.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/mdout.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/mdout.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/minim.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/minim.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-cg.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s1-cg.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-steep.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s1-steep.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-cg.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s2-cg.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-steep.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s2-steep.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s3-steep.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s3-steep.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s4-cg.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/minimization/s4-cg.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/npt.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/npt.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/nvt.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/nvt.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdp/vaccum.mdp` & `unigbsa-0.1.5/unigbsa/simulation/mdp/vaccum.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/mdrun.py` & `unigbsa-0.1.5/unigbsa/simulation/mdrun.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/openmm-em.py` & `unigbsa-0.1.5/unigbsa/simulation/openmm-em.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/topology.py` & `unigbsa-0.1.5/unigbsa/simulation/topology.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/simulation/utils.py` & `unigbsa-0.1.5/unigbsa/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa/utils.py` & `unigbsa-0.1.5/unigbsa/utils.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.4/unigbsa.egg-info/PKG-INFO` & `unigbsa-0.1.5/unigbsa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unigbsa
-Version: 0.1.4
+Version: 0.1.5
 Summary: MMPB(GB)SA tools for calculate energy.
 Home-page: https://github.com/dptech-corp/Uni-GBSA
 Author: dptech.net
 Author-email: hermite@dptech.net
 Keywords: MMPBSA MMGBSA
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
-Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening==============================================================================[[ChemRxiv](https://chemrxiv.org/engage/chemrxiv/article-details/63345399f764e656800664e7)]## BackgroudCalculating the binding free energy of a ligand to a protein receptor is a crucial goal in drug discovery. Molecular mechanics/Generalized-Born (Poisson–Boltzmann) surface area (MM/GB(PB)SA), which balances accuracy and efficiency, is one of the most widely used methods for evaluating ligand binding free energies in virtual screening. Uni-GBSA is an automatic workflow to perform MM/GB(PB)SA calculations. It includes several functions including but not limited to topology preparation, structure optimization, binding free energy calculation, and parameter scanning for MM/GB(PB)SA calculations. It also has a batch mode that allows the evaluation of thousands of molecules against one protein target simultaneously, enabling its application in virtual screening. ## Install### Install by condaTo run uni-GBSA, you need to install several third-party softwares including acpype, gmx_MMPBSA, lickit, etc.```Bashconda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacsconda activate gbsapip install unigbsa gmx_MMPBSA>=1.5.6 lickit```### Install by dokcer imagesYou can also build a dokcer image using this file or pull from the docker hub `docker pull dockerymh/unigbsa````PlaintextFROM continuumio/miniconda3# 1. create a enveriomentSHELL ["/bin/bash", "-c"]RUN conda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacs \&&  echo 'conda activate gbsa' >> ~/.bashrc \&&  rm -rf /opt/conda/pkgs/* # 2. install unigbsaRUN source ~/.bashrc \ &&  pip install unigbsa gmx_MMPBSA>=1.5.6 lickit \&&  rm -rf ~/.cache/*```## Usage & Example### Usage```bash$ unigbsa-pipeline -husage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD]                        [--decomp] [--verbose] [-v]GBSA Calculation. Version: 0.0.9_devoptions:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: /opt/miniconda3/envs/test/lib/python3.10/site-packages/unigbsa-0.0.9.dev0-py3.10.egg/unigbsa/data/default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.  -v, --version         show program's version number and exit```### Example```bash$ unigbsa-pipeline -i example/1ceb/1ceb_protein.pdb -l example/1ceb/1ceb_ligand.sdf -o BindingEnergy.csv10/08/2022 13:46:09 PM - INFO - Build protein topology.10/08/2022 13:46:10 PM - INFO - Build ligand topology: 1ceb_ligand1 molecule converted10/08/2022 13:46:13 PM - INFO - Running energy minimization: 1ceb_ligand10/08/2022 13:46:14 PM - INFO - Run the MMPB(GB)SA.10/08/2022 13:46:18 PM - INFO - Clean the results.================================================================================Results: Energy.csv Dec.csvFrames    mode    detal_G(kcal/mole)     1      gb              -20.4421```## Other ToolsThis packge contains many command lines: `unigbsa-scan`, `unigbsa-pipeline`, `unigbsa-traj`, `unigbsa-pbc`, `unigbsa-buildtop`, `unigbsa-buildsys`, `unigbsa-md`.### unigbsa-scan>An automatic parameter optimization prior to production MM/GB(PB)SA calculations.```Bashusage: unigbsa-scan [-h] [-i RECEPTOR] [-pd PROTDIR] [-l LIGAND [LIGAND ...]] [-ld LIGDIR] -e E -c PARASFILE [-o OUTDIR]                    [-nt THREAD] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -pd PROTDIR           Floder contains many protein files. file format: .pdb  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -ld LIGDIR            Floder contains many ligand files. file format: .mol or .sdf  -e E                  Experiment data file.  -c PARASFILE          Parameters to scan  -o OUTDIR             Output directory.  -nt THREAD            Set number of thread to run this program.  --verbose             Keep all the files.```>Example```Bashunigbsa-scan -i example/scan/protein.pdb -ld example/scan/ -e example/scan/ligands.csv -c example/scan/scan.json -o scan-demo -nt 4```### unigbsa-pipeline>A simple, automatic pipeline to perform MM/GB(PB)SA calculations. You only need to provide a protein file (in the PDB format) and ligand files (in the MOL or SDF format). This function will perform an energy minimization then calculate the PBSA/GBSA values for the each input ligand.* If you want perform energy minimization or MD simulation for the complex automatically, use the ``unigbsa-pipeline`` function.```Bashusage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD] [--decomp] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.```You can change the parameters for the MM/GB(PB)SA calculations by providing a configue file(`default.ini`). ```; parameters for simulation[simulation]; input pose process method: ;   input   -   just use input pose to calculation;   em      -   run a simple energy minimizaion for the input poses;   md      -   run a md simulation for the input posesmode = em; simulation box type: triclinic, cubic, dodecahedron, octahedronboxtype = triclinic; Distance between the solute and the simulation boxboxsize = 0.9; Specify salt concentration (mol/liter). This will add sufficient ions to reach up to the specified concentrationconc = 0.15; number of md simulation stepsnsteps = 500000; number of equilibrium simulation(nvt, npt) stepseqsteps = 50000; number of structure to save for the md simulationnframe = 100; protein forcefield (gromacs engine)proteinforcefield = amber03; ligand forcefield (acpype engine)ligandforcefield = gaff; ligand charge method: bcc, gasligandCharge = bcc; parameters for PBSA/GBSA calculation, support all the gmx_MMPBSA parameters[GBSA]; calculation namesys_name = GBSA; calculation mode, Separated by commas. gb,pb,decompositionmodes = gb; best parameters for PBSA/GBSA calculations obtained from Wang, Ercheng, et al. Chemical reviews 119.16 (2019): 9478-9508.igb = 2indi = 4.0exdi = 80.0```### unigbsa-traj>Perform a PBSA/GBSA calculation of a complex from a MD trajectory. Note: you need to prepare a gromacs `index.ndx` file which contains two groups named `RECEPTOR` and `LIGAND`.````unigbsa-traj -husage: unigbsa-traj [-h] -i INP -p TOP -ndx NDX [-m {gb,pb,pb+gb,gb+pb}] [-t TRAJ] [-indi INDI] [-dec] [-D]Free energy calcaulated by PBSA method.optional arguments:  -h, --help            show this help message and exit  -i INP                A pdb file or a tpr file for the trajectory.  -p TOP                Gromacs topol file for the system.  -ndx NDX              Gromacs index file, must contain recepror and ligand group.  -m {gb,pb,pb+gb,gb+pb}                        Method to calculate: gb, pb, pb+gb. default:gb  -t TRAJ               A trajectory file contains many structure frames. File format: xtc, pdb, gro...  -indi INDI            External dielectric constant. detault: 1.0  -dec                  Decompose the energy. default:false  -D                    DEBUG model, keep all the files.````### unigbsa-buildtop>Topology preparation for a protein receptor and ligand(s) using gromacs.```Bashunigbsa-buildtop -husage: unigbsa-buildtop [-h] [-p PROTEIN] [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-o OUTDIR] [-c] [-verbose]Build topology file for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file or directory to build topology.  -l LIGAND         Ligand file or directory to build topology.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -o OUTDIR         A output directory.  -c                Combine the protein and ligand topology. Suppport for one protein and more ligands. default:True  -verbose          Keep the directory or not.```### unigbsa-buildsys>Build a simulation box for a protein-ligand complex.```bashunigbsa-buildsys -husage: unigbsa-buildsys [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR]Build MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.```### unigbsa-md>Run a MD simulation of a protein-ligand complex.```Bashunigbsa-md -husage: unigbsa-md [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR] [-nstep NSTEP] [-nframe NFRAME] [-verbose]Run MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.  -nstep NSTEP      Simulation steps. default:2500  -nframe NFRAME    Number of frame to save for the xtc file. default:100  -verbose          Keep all the files in the simulation.```### unigbsa-pbc>Process PBC condition for a MD trajectory.```Bashunigbsa-pbc -husage: unigbsa-pbc [-h] -s TPR -f XTC [-o OUT] [-n NDX]Auto process PBC for gromacs MD trajector.optional arguments:  -h, --help  show this help message and exit  -s TPR      TPR file generated from gromacs or coordinate file.  -f XTC      Trajector file to process PBC.  -o OUT      Result file after processed PBC.  -n NDX      Index file contains the center and output group.```### More Examples* Perform a MM/GB(PB)SA calculation on a ligand file with a protein receptor with ``unigbsa-pipeline``````Bashunigbsa-pipeline -i ./example/2fvy/protein.pdb -l ./example/2fvy/BGC.mol2````* Perform a MM/GB(PB)SA calculation of a complex from a MD trajectory with ``unigbsa-traj`````Bashunigbsa-traj -i example/3f/complex.pdb -p example/3f/complex.top -ndx example/3f/index.ndx -m pb gb -t example/3f/complex.pdb```* Build topology for a protein receptor and a ligand using gromacs. ``unigbsa-buildtop`````bashunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -o topol  # build gromacs topology for a single proteinunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -l example/2fvy/BGC.mol2 -lf gaff -o 2fvy_topol -c # build gromacs topology for protein and ligand complex```* Build a simulation system with ``unigbsa-buildsys``* Run a MD simulation with ``unigbsa-md``* Process the PBC condition of a MD trjectorywith ``unigbsa-pbc``## Citation```plaintextYang M, Wang D, Zheng H. Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening. ChemRxiv. Cambridge: Cambridge Open Engage; 2022; This content is a preprint and has not been peer-reviewed.```
+Uni-GBSA: An Automatic Workflow to Perform MM/GB(PB)SA Calculations for Virtual Screening==============================================================================[[Briefings in Bioinformatics](https://academic.oup.com/bib/advance-article/doi/10.1093/bib/bbad218/7199492)]## BackgroudCalculating the binding free energy of a ligand to a protein receptor is a crucial goal in drug discovery. Molecular mechanics/Generalized-Born (Poisson–Boltzmann) surface area (MM/GB(PB)SA), which balances accuracy and efficiency, is one of the most widely used methods for evaluating ligand binding free energies in virtual screening. Uni-GBSA is an automatic workflow to perform MM/GB(PB)SA calculations. It includes several functions including but not limited to topology preparation, structure optimization, binding free energy calculation, and parameter scanning for MM/GB(PB)SA calculations. It also has a batch mode that allows the evaluation of thousands of molecules against one protein target simultaneously, enabling its application in virtual screening. ## Install### Install by condaTo run uni-GBSA, you need to install several third-party softwares including acpype, gmx_MMPBSA, lickit, etc.```Bashconda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacsconda activate gbsapip install unigbsa gmx_MMPBSA>=1.5.6 lickit```### Install by docker imagesYou can also build a docker image using this file or pull from the docker hub `docker pull dockerymh/unigbsa````PlaintextFROM continuumio/miniconda3# 1. create a enveriomentSHELL ["/bin/bash", "-c"]RUN conda create -n gbsa -c conda-forge acpype openmpi mpi4py gromacs \&&  echo 'conda activate gbsa' >> ~/.bashrc \&&  rm -rf /opt/conda/pkgs/* # 2. install unigbsaRUN source ~/.bashrc \ &&  pip install unigbsa gmx_MMPBSA>=1.5.6 lickit \&&  rm -rf ~/.cache/*```## Usage & Example### Usage```bash$ unigbsa-pipeline -husage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD]                        [--decomp] [--verbose] [-v]GBSA Calculation. Version: 0.0.9_devoptions:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: /opt/miniconda3/envs/test/lib/python3.10/site-packages/unigbsa-0.0.9.dev0-py3.10.egg/unigbsa/data/default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.  -v, --version         show program's version number and exit```### Example```bash$ unigbsa-pipeline -i example/1ceb/1ceb_protein.pdb -l example/1ceb/1ceb_ligand.sdf -o BindingEnergy.csv10/08/2022 13:46:09 PM - INFO - Build protein topology.10/08/2022 13:46:10 PM - INFO - Build ligand topology: 1ceb_ligand1 molecule converted10/08/2022 13:46:13 PM - INFO - Running energy minimization: 1ceb_ligand10/08/2022 13:46:14 PM - INFO - Run the MMPB(GB)SA.10/08/2022 13:46:18 PM - INFO - Clean the results.================================================================================Results: Energy.csv Dec.csvFrames    mode    detal_G(kcal/mole)     1      gb              -20.4421```## Other ToolsThis packge contains several commands: `unigbsa-scan`, `unigbsa-pipeline`, `unigbsa-traj`, `unigbsa-pbc`, `unigbsa-buildtop`, `unigbsa-buildsys`, `unigbsa-md`.### unigbsa-scan>Perform an automatic parameter optimization prior to production MM/GB(PB)SA calculations.```Bashusage: unigbsa-scan [-h] [-i RECEPTOR] [-pd PROTDIR] [-l LIGAND [LIGAND ...]] [-ld LIGDIR] -e E -c PARASFILE [-o OUTDIR]                    [-nt THREAD] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -pd PROTDIR           Floder contains many protein files. file format: .pdb  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -ld LIGDIR            Floder contains many ligand files. file format: .mol or .sdf  -e E                  Experiment data file.  -c PARASFILE          Parameters to scan  -o OUTDIR             Output directory.  -nt THREAD            Set number of thread to run this program.  --verbose             Keep all the files.```>Example```Bashunigbsa-scan -i example/scan/protein.pdb -ld example/scan/ -e example/scan/ligands.csv -c example/scan/scan.json -o scan-demo -nt 4```### unigbsa-pipeline>A simple, automatic pipeline to perform MM/GB(PB)SA calculations. You only need to provide a protein file (in the PDB format) and ligand files (in the MOL or SDF format). This function will perform an energy minimization then calculate the PBSA/GBSA values for the each input ligand.* If you want perform energy minimization or MD simulation for the complex automatically, use the ``unigbsa-pipeline`` function.```Bashusage: unigbsa-pipeline [-h] -i RECEPTOR [-l LIGAND [LIGAND ...]] [-c CONFIG] [-d LIGDIR] [-f PBSAFILE] [-o OUTFILE] [-nt THREAD] [--decomp] [--verbose]GBSA Calculation.optional arguments:  -h, --help            show this help message and exit  -i RECEPTOR           Input protein file with pdb format.  -l LIGAND [LIGAND ...]                        Ligand files to calculate binding energy.  -c CONFIG             Configue file, default: default.ini  -d LIGDIR             Floder contains many ligand files. file format: .mol or .sdf  -f PBSAFILE           gmx_MMPBSA input file. default=None  -o OUTFILE            Output file.  -nt THREAD            Set number of thread to run this program.  --decomp              Decompose the free energy. default:False  --verbose             Keep all the files.```You can change the parameters for the MM/GB(PB)SA calculations by providing a configue file(`default.ini`). ```; parameters for simulation[simulation]; input pose process method: ;   input   -   just use input pose to calculation;   em      -   run a simple energy minimizaion for the input poses;   md      -   run a md simulation for the input posesmode = em; simulation box type: triclinic, cubic, dodecahedron, octahedronboxtype = triclinic; Distance between the solute and the simulation boxboxsize = 0.9; Specify salt concentration (mol/liter). This will add sufficient ions to reach up to the specified concentrationconc = 0.15; number of md simulation stepsnsteps = 500000; number of equilibrium simulation(nvt, npt) stepseqsteps = 50000; number of structure to save for the md simulationnframe = 100; protein forcefield (gromacs engine)proteinforcefield = amber03; ligand forcefield (acpype engine)ligandforcefield = gaff; ligand charge method: bcc, gasligandCharge = bcc; parameters for PBSA/GBSA calculation, support all the gmx_MMPBSA parameters[GBSA]; calculation namesys_name = GBSA; calculation mode, Separated by commas. gb,pb,decompositionmodes = gb; best parameters for PBSA/GBSA calculations obtained from Wang, Ercheng, et al. Chemical reviews 119.16 (2019): 9478-9508.igb = 2indi = 4.0exdi = 80.0```### unigbsa-traj>Perform a PBSA/GBSA calculation of a complex from a MD trajectory. Note: you need to prepare a gromacs `index.ndx` file which contains two groups named `RECEPTOR` and `LIGAND`.````unigbsa-traj -husage: unigbsa-traj [-h] -i INP -p TOP -ndx NDX [-m {gb,pb,pb+gb,gb+pb}] [-t TRAJ] [-indi INDI] [-dec] [-D]Free energy calcaulated by PBSA method.optional arguments:  -h, --help            show this help message and exit  -i INP                A pdb file or a tpr file for the trajectory.  -p TOP                Gromacs topol file for the system.  -ndx NDX              Gromacs index file, must contain recepror and ligand group.  -m {gb,pb,pb+gb,gb+pb}                        Method to calculate: gb, pb, pb+gb. default:gb  -t TRAJ               A trajectory file contains many structure frames. File format: xtc, pdb, gro...  -indi INDI            External dielectric constant. detault: 1.0  -dec                  Decompose the energy. default:false  -D                    DEBUG model, keep all the files.````### unigbsa-buildtop>Topology preparation for a protein receptor and ligand(s) using gromacs.```Bashunigbsa-buildtop -husage: unigbsa-buildtop [-h] [-p PROTEIN] [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-o OUTDIR] [-c] [-verbose]Build topology file for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file or directory to build topology.  -l LIGAND         Ligand file or directory to build topology.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -o OUTDIR         A output directory.  -c                Combine the protein and ligand topology. Suppport for one protein and more ligands. default:True  -verbose          Keep the directory or not.```### unigbsa-buildsys>Build a simulation box for a protein-ligand complex.```bashunigbsa-buildsys -husage: unigbsa-buildsys [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR]Build MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.```### unigbsa-md>Run a MD simulation of a protein-ligand complex.```Bashunigbsa-md -husage: unigbsa-md [-h] -p PROTEIN [-l LIGAND] [-pf PROTFORCE] [-lf {gaff,gaff2}] [-bt BOXTYPE] [-box BOX BOX BOX] [-d D] [-conc CONC] [-o OUTDIR] [-nstep NSTEP] [-nframe NFRAME] [-verbose]Run MD simulation for input file.optional arguments:  -h, --help        show this help message and exit  -p PROTEIN        Protein file for the simulation.  -l LIGAND         Ligand file or directory for the simulation.  -pf PROTFORCE     Protein forcefield.  -lf {gaff,gaff2}  Ligand forcefiled: gaff or gaff2.  -bt BOXTYPE       Simulation box type, default: triclinic  -box BOX BOX BOX  Simulation box size.  -d D              Distance between the solute and the box.  -conc CONC        Specify salt concentration (mol/liter). default=0.15  -o OUTDIR         A output directory.  -nstep NSTEP      Simulation steps. default:2500  -nframe NFRAME    Number of frame to save for the xtc file. default:100  -verbose          Keep all the files in the simulation.```### unigbsa-pbc>Process PBC condition for a MD trajectory.```Bashunigbsa-pbc -husage: unigbsa-pbc [-h] -s TPR -f XTC [-o OUT] [-n NDX]Auto process PBC for gromacs MD trajector.optional arguments:  -h, --help  show this help message and exit  -s TPR      TPR file generated from gromacs or coordinate file.  -f XTC      Trajector file to process PBC.  -o OUT      Result file after processed PBC.  -n NDX      Index file contains the center and output group.```### More Examples* Perform a MM/GB(PB)SA calculation on a ligand file with a protein receptor with ``unigbsa-pipeline``````Bashunigbsa-pipeline -i ./example/2fvy/protein.pdb -l ./example/2fvy/BGC.mol2````* Perform a MM/GB(PB)SA calculation of a complex from a MD trajectory with ``unigbsa-traj`````Bashunigbsa-traj -i example/3f/complex.pdb -p example/3f/complex.top -ndx example/3f/index.ndx -m pb gb -t example/3f/complex.pdb```* Build topology for a protein receptor and a ligand using gromacs. ``unigbsa-buildtop`````bashunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -o topol  # build gromacs topology for a single proteinunigbsa-buildtop -p example/2fvy/protein.pdb -pf amber99sb -l example/2fvy/BGC.mol2 -lf gaff -o 2fvy_topol -c # build gromacs topology for protein and ligand complex```* Build a simulation system with ``unigbsa-buildsys``* Run a MD simulation with ``unigbsa-md``* Process the PBC condition of a MD trjectorywith ``unigbsa-pbc``## Citation```plaintextMaohua Yang and others, Uni-GBSA: an open-source and web-based automatic workflow to perform MM/GB(PB)SA calculations for virtual screening, Briefings in Bioinformatics, 2023;, bbad218, https://doi.org/10.1093/bib/bbad218.```
```

### Comparing `unigbsa-0.1.4/unigbsa.egg-info/SOURCES.txt` & `unigbsa-0.1.5/unigbsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

