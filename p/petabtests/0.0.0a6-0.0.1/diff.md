# Comparing `tmp/petabtests-0.0.0a6.tar.gz` & `tmp/petabtests-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/petabtests-0.0.0a6.tar", last modified: Sat Nov 28 21:08:05 2020, max compression
+gzip compressed data, was "petabtests-0.0.1.tar", last modified: Tue Jun 20 10:10:25 2023, max compression
```

## Comparing `petabtests-0.0.0a6.tar` & `petabtests-0.0.1.tar`

### file list

```diff
@@ -1,537 +1,661 @@
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.544874 petabtests-0.0.0a6/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      102 2020-11-28 20:59:35.000000 petabtests-0.0.0a6/MANIFEST.in
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3268 2020-11-28 21:08:05.544874 petabtests-0.0.0a6/PKG-INFO
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2116 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/README.md
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.484874 petabtests-0.0.0a6/petabtests/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      661 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/C.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      245 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/__init__.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.484874 petabtests-0.0.0a6/petabtests/cases/
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.488874 petabtests-0.0.0a6/petabtests/cases/0001/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      228 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/0001.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1360 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/0001.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_0001.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_0001_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       98 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0001/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.488874 petabtests-0.0.0a6/petabtests/cases/0002/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      318 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/0002.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1510 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/0002.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_0002.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_0002_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       29 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       54 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      125 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0002/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.488874 petabtests-0.0.0a6/petabtests/cases/0003/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      480 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/0003.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1503 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/0003.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_0003.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_0003_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      116 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0003/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.488874 petabtests-0.0.0a6/petabtests/cases/0004/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      538 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/0004.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1426 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/0004.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_0004.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      139 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_0004_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       77 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      192 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       96 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0004/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.492874 petabtests-0.0.0a6/petabtests/cases/0005/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      473 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/0005.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1471 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/0005.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_0005.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_0005_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       51 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3195 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       65 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      197 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      113 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3195 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0005/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.492874 petabtests-0.0.0a6/petabtests/cases/0006/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      375 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/0006.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1440 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/0006.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_0006.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_0006_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      110 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      123 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0006/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.496874 petabtests-0.0.0a6/petabtests/cases/0007/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      439 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/0007.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1414 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/0007.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_0007.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_0007_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      103 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0007/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.496874 petabtests-0.0.0a6/petabtests/cases/0008/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      353 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/0008.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1385 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/0008.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_0008.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_0008_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       99 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      130 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0008/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.496874 petabtests-0.0.0a6/petabtests/cases/0009/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      283 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/0009.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1637 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/0009.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_0009.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_0009_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       35 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      125 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      160 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0009/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.500874 petabtests-0.0.0a6/petabtests/cases/0010/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      401 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0010/0010.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1556 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/0010/0010.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0010/_0010.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/0010/_0010_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       41 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/0010/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0010/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0010/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0010/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       89 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0010/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      159 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/0010/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0010/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.500874 petabtests-0.0.0a6/petabtests/cases/0011/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      356 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/0011.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1365 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/0011.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_0011.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      138 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_0011_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       19 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      107 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0011/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.504874 petabtests-0.0.0a6/petabtests/cases/0012/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/0012.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1504 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/0012.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_0012.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      139 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_0012_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       29 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      107 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0012/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.504874 petabtests-0.0.0a6/petabtests/cases/0013/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      219 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/0013.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1517 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/0013.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_0013.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_0013_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       21 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0013/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.504874 petabtests-0.0.0a6/petabtests/cases/0014/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      221 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/0014.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1448 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/0014.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_0014.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_0014_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      111 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       98 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0014/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.508874 petabtests-0.0.0a6/petabtests/cases/0015/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      224 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/0015.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1436 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/0015.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_0015.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_0015_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      111 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       74 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      164 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0015/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.508874 petabtests-0.0.0a6/petabtests/cases/0016/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      436 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/0016.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1413 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/0016.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_0016.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_0016_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      101 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/0016/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.480874 petabtests-0.0.0a6/petabtests/cases/pysb/
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.512874 petabtests-0.0.0a6/petabtests/cases/pysb/0001/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_0001.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_0001_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       98 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0001/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.512874 petabtests-0.0.0a6/petabtests/cases/pysb/0002/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_0002.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_0002_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       29 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       54 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      125 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0002/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.512874 petabtests-0.0.0a6/petabtests/cases/pysb/0003/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_0003.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_0003_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      116 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0003/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.512874 petabtests-0.0.0a6/petabtests/cases/pysb/0004/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_0004.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      139 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_0004_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       77 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      192 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       96 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0004/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.516874 petabtests-0.0.0a6/petabtests/cases/pysb/0005/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_0005.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_0005_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       51 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       65 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      197 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      113 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0005/conversion_modified_pysb.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.516874 petabtests-0.0.0a6/petabtests/cases/pysb/0006/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_0006.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_0006_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      110 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      123 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0006/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.516874 petabtests-0.0.0a6/petabtests/cases/pysb/0007/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_0007.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_0007_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      103 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0007/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.516874 petabtests-0.0.0a6/petabtests/cases/pysb/0008/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_0008.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_0008_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       99 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      130 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0008/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.520874 petabtests-0.0.0a6/petabtests/cases/pysb/0009/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_0009.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_0009_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       35 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      125 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      160 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0009/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.520874 petabtests-0.0.0a6/petabtests/cases/pysb/0010/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_0010.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_0010_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       41 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       89 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      159 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0010/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.520874 petabtests-0.0.0a6/petabtests/cases/pysb/0011/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_0011.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      138 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_0011_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       19 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      107 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0011/conversion_modified_pysb.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.520874 petabtests-0.0.0a6/petabtests/cases/pysb/0012/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_0012.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      139 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_0012_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       29 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      107 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0012/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.524874 petabtests-0.0.0a6/petabtests/cases/pysb/0013/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_0013.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_0013_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       21 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0013/conversion_modified_pysb.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.524874 petabtests-0.0.0a6/petabtests/cases/pysb/0014/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_0014.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_0014_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      111 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       98 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0014/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.524874 petabtests-0.0.0a6/petabtests/cases/pysb/0015/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_0015.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_0015_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      111 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       74 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      164 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0015/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.524874 petabtests-0.0.0a6/petabtests/cases/pysb/0016/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_0016.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_0016_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      101 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/pysb/0016/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.484874 petabtests-0.0.0a6/petabtests/cases/sbml/
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.524874 petabtests-0.0.0a6/petabtests/cases/sbml/0001/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      228 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/0001.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1360 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/0001.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_0001.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_0001_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       98 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0001/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.528874 petabtests-0.0.0a6/petabtests/cases/sbml/0002/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      318 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/0002.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1510 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/0002.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_0002.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_0002_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       29 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       54 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      125 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0002/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.528874 petabtests-0.0.0a6/petabtests/cases/sbml/0003/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      480 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/0003.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1503 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/0003.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_0003.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_0003_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      116 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0003/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.528874 petabtests-0.0.0a6/petabtests/cases/sbml/0004/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      538 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/0004.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1426 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/0004.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_0004.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      139 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_0004_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       77 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      192 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       96 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0004/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.528874 petabtests-0.0.0a6/petabtests/cases/sbml/0005/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      473 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/0005.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1471 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/0005.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_0005.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_0005_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       51 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3195 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       65 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      197 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      113 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3195 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0005/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.532874 petabtests-0.0.0a6/petabtests/cases/sbml/0006/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      375 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/0006.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1440 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/0006.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_0006.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_0006_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      110 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      123 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0006/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.532874 petabtests-0.0.0a6/petabtests/cases/sbml/0007/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      439 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/0007.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1414 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/0007.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_0007.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_0007_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      103 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0007/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.532874 petabtests-0.0.0a6/petabtests/cases/sbml/0008/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      353 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/0008.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1385 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/0008.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_0008.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_0008_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       99 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      130 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0008/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.532874 petabtests-0.0.0a6/petabtests/cases/sbml/0009/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      283 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/0009.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1637 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/0009.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_0009.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_0009_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       35 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      125 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      160 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0009/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.536874 petabtests-0.0.0a6/petabtests/cases/sbml/0010/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      401 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/0010.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1556 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/0010.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_0010.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_0010_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       41 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      129 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       89 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      159 2020-11-28 20:59:04.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0010/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.536874 petabtests-0.0.0a6/petabtests/cases/sbml/0011/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      356 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/0011.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1365 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/0011.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_0011.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      138 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_0011_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       19 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      107 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0011/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.540874 petabtests-0.0.0a6/petabtests/cases/sbml/0012/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      211 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/0012.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1504 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/0012.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_0012.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      139 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_0012_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       29 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      107 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0012/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.540874 petabtests-0.0.0a6/petabtests/cases/sbml/0013/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      219 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/0013.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1517 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/0013.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_0013.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      140 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_0013_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       21 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       83 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       56 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       97 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2859 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0013/conversion_modified.xml
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.544874 petabtests-0.0.0a6/petabtests/cases/sbml/0014/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      221 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/0014.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1448 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/0014.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_0014.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      141 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_0014_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      111 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       98 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0014/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.544874 petabtests-0.0.0a6/petabtests/cases/sbml/0015/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      224 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/0015.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1436 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/0015.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_0015.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_0015_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      111 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       74 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      164 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      126 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0015/_simulations.tsv
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.544874 petabtests-0.0.0a6/petabtests/cases/sbml/0016/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      436 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/0016.md
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1413 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/0016.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      212 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_0016.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      142 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_0016_solution.yaml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       15 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_conditions.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       84 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_measurements.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_model.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      101 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_observables.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      143 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_parameters.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      114 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/petabtests/cases/sbml/0016/_simulations.tsv
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3102 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/petabtests/conversion.xml
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      417 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/petabtests/conversion_pysb.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     2044 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/petabtests/core.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3694 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/petabtests/evaluate.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     6265 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/petabtests/file.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      392 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/petabtests/model.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       24 2020-11-28 20:59:41.000000 petabtests-0.0.0a6/petabtests/version.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.484874 petabtests-0.0.0a6/petabtests.egg-info/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     3268 2020-11-28 21:08:05.000000 petabtests-0.0.0a6/petabtests.egg-info/PKG-INFO
--rw-rw-r--   0 yannik    (1000) yannik    (1000)    18892 2020-11-28 21:08:05.000000 petabtests-0.0.0a6/petabtests.egg-info/SOURCES.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)        1 2020-11-28 21:08:05.000000 petabtests-0.0.0a6/petabtests.egg-info/dependency_links.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      103 2020-11-28 21:08:05.000000 petabtests-0.0.0a6/petabtests.egg-info/entry_points.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       31 2020-11-28 21:08:05.000000 petabtests-0.0.0a6/petabtests.egg-info/requires.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       11 2020-11-28 21:08:05.000000 petabtests-0.0.0a6/petabtests.egg-info/top_level.txt
--rw-rw-r--   0 yannik    (1000) yannik    (1000)       38 2020-11-28 21:08:05.544874 petabtests-0.0.0a6/setup.cfg
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1635 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/setup.py
-drwxrwxr-x   0 yannik    (1000) yannik    (1000)        0 2020-11-28 21:08:05.544874 petabtests-0.0.0a6/test/
--rw-rw-r--   0 yannik    (1000) yannik    (1000)     1101 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/test/test_evaluate.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      244 2020-11-26 09:23:28.000000 petabtests-0.0.0a6/test/test_general.py
--rw-rw-r--   0 yannik    (1000) yannik    (1000)      327 2020-11-22 21:55:30.000000 petabtests-0.0.0a6/test/test_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.964854 petabtests-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-20 10:10:15.000000 petabtests-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 10:10:15.000000 petabtests-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-20 10:10:25.964854 petabtests-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-20 10:10:15.000000 petabtests-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.872851 petabtests-0.0.1/petabtests/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/C.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.864851 petabtests-0.0.1/petabtests/cases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.864851 petabtests-0.0.1/petabtests/cases/v1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.872851 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.872851 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/0001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_0001.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_0001_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.876852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/0002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_0002.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_0002_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.876852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/0003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_0003.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_0003_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.876852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/0004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_0004.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_0004_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.880852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/0005.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_0005.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_0005_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.880852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/0006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_0006.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_0006_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.884852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/0007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_0007.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_0007_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.884852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/0008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_0008.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_0008_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.884852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/0009.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_0009.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_0009_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.884852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/0010.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_0010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_0010_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.888852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/0011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_0011.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_0011_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.892852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/0012.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_0012.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_0012_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.892852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/0013.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_0013.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_0013_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.892852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/0014.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_0014.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_0014_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.896852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/0015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_0015.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_0015_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.896852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/0016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_0016.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_0016_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.896852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/0017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_0017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_0017_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.896852 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/0018.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_0018.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_0018_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0018/model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.868852 petabtests-0.0.1/petabtests/cases/v2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.896852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.900852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/0001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_0001.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_0001_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.900852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/0002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_0002.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_0002_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.900852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/0003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_0003.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_0003_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.904852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/0004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_0004.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_0004_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.904852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/0005.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_0005.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_0005_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/conversion_modified_pysb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.904852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/0006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_0006.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_0006_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.908852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/0007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_0007.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_0007_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0007/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.908852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/0008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_0008.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_0008_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.912852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/0009.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_0009.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_0009_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.912852 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/0010.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_0010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_0010_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0010/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.916853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/0011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_0011.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_0011_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/conversion_modified_pysb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.916853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/0012.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_0012.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_0012_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0012/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.920853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/0013.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_0013.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_0013_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/conversion_modified_pysb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.920853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/0014.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_0014.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_0014_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.924853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/0015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_0015.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_0015_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.924853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/0016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_0016.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_0016_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0016/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.928853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/0017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_0017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_0017_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0017/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.928853 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/0018.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_0018.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_0018_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.928853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.932853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/0001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_0001.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_0001_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.932853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/0002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_0002.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_0002_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.932853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/0003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_0003.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_0003_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.936853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/0004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_0004.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_0004_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.936853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/0005.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_0005.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_0005_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.940853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/0006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_0006.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_0006_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.940853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/0007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_0007.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_0007_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.944853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/0008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_0008.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_0008_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.944853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/0009.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_0009.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_0009_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.948853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/0010.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_0010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_0010_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.948853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/0011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_0011.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_0011_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.952853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/0012.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_0012.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_0012_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.952853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/0013.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_0013.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_0013_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/conversion_modified.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.956853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/0014.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_0014.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_0014_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.956853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/0015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_0015.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_0015_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.960853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/0016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_0016.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_0016_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.960853 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/0017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_0017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_0017_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0017/_simulations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.964854 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/0018.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_0018.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_0018_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0018/model.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.964854 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/0019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_0019.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_0019_solution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_conditions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_measurements.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_model.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_observables.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_parameters.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/_simulations.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/conversion.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/conversion_pysb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 10:10:15.000000 petabtests-0.0.1/petabtests/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.872851 petabtests-0.0.1/petabtests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-20 10:10:25.000000 petabtests-0.0.1/petabtests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28246 2023-06-20 10:10:25.000000 petabtests-0.0.1/petabtests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:10:25.000000 petabtests-0.0.1/petabtests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 10:10:25.000000 petabtests-0.0.1/petabtests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 10:10:25.000000 petabtests-0.0.1/petabtests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 10:10:25.000000 petabtests-0.0.1/petabtests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:10:25.964854 petabtests-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-20 10:10:15.000000 petabtests-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:10:25.964854 petabtests-0.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-20 10:10:15.000000 petabtests-0.0.1/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 10:10:15.000000 petabtests-0.0.1/test/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-20 10:10:15.000000 petabtests-0.0.1/test/test_generate.py
```

### Comparing `petabtests-0.0.0a6/PKG-INFO` & `petabtests-0.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 Metadata-Version: 2.1
 Name: petabtests
-Version: 0.0.0a6
+Version: 0.0.1
 Summary: PEtab testsuite library
 Home-page: https://github.com/PEtab-dev/petab_test_suite
 Author: PEtab-dev
 Author-email: yannik.schaelte@gmail.com
 Maintainer: PEtab-dev
 Maintainer-email: yannik.schaelte@gmail.com
-License: UNKNOWN
-Description: # PEtab test suite
-        
-        The PEtab test suite is a collection of test models for the
-        [PEtab](https://github.com/petab-dev/petab) parameter estimation data format.
-        It is intended to be used to verify and quantify PEtab-support by developers
-        of tools for model simulation and parameter estimation.
-        
-        ## Download and install the test suite
-        
-        The PEtab test suite can be downloaded from GitHub via
-        
-            git clone https://github.com/petab-dev/petab_test_suite
-        
-        The test suite comes with all necessary files pregenerated. 
-        In the [petabtests](petabtests) subdirectory, it contains a python module for
-        generating the tests and evaluating results. This can be installed via
-        
-            cd petab_test_suite
-            pip3 install -e .
-        
-        ## Use the test suite
-        
-        The [cases](cases) subdirectory contains a collection of enumerated tests.
-        Each test contains a descriptive `wxyz.md` file, and a script file `wxyz.py`
-        file that can be used to generate all problem and solution files for the test.
-        The necessary files are in the same case specific folder, starting with an
-        underscore. 
-        In each case folder, there is a file `_wxyz.yaml` containing the parameter
-        estimation problem description, and a file `_wxyz_solution.yaml` containing
-        information on the expected results: chi2 value, log-likelihood, simulation
-        table reference, and tolerances.
-        
-        After download, all necessary files are already pregenerated.
-        
-        Further, installation of the petabtests module installs a routine to recreate
-        the problem and solution files for all test problems. It can be invoked via
-        
-            cd petab_test_suite
-            petabtests_create
-        
-        ## Evaluate results
-        
-        To evaluate how a tool performs on a given test problem, three metrics are
-        employed: Simulations, chi2 value and log-likelihood. A tool can be said to
-        cover a test problem if any of those values matches the ground truth values
-        up to some tolerance.
-        
-        The python module provides convenience functions for evaluation in
-        [petabtests/evaluate.py](petabtests/evaluate.py).
-        
-        -> [Overview of passed test cases for different tools supporting PEtab](https://github.com/PEtab-dev/PEtab#petab-features-supported-in-different-tools)
-        
 Keywords: PEtab testsuite
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PEtab test suite
+
+The PEtab test suite is a collection of test models for the
+[PEtab](https://github.com/petab-dev/petab) parameter estimation data format.
+It is intended to be used to verify and quantify PEtab-support by developers
+of tools for model simulation and parameter estimation.
+
+## Download and install the test suite
+
+The PEtab test suite can be downloaded from GitHub via
+
+    git clone https://github.com/petab-dev/petab_test_suite
+
+The test suite comes with all necessary files pregenerated. 
+In the [petabtests](petabtests) subdirectory, it contains a python module for
+generating the tests and evaluating results. This can be installed via
+
+    cd petab_test_suite
+    pip3 install -e .
+
+## Use the test suite
+
+The [cases](cases) subdirectory contains a collection of enumerated tests.
+Each test contains a descriptive `wxyz.md` file, and a script file `wxyz.py`
+file that can be used to generate all problem and solution files for the test.
+The necessary files are in the same case specific folder, starting with an
+underscore. 
+In each case folder, there is a file `_wxyz.yaml` containing the parameter
+estimation problem description, and a file `_wxyz_solution.yaml` containing
+information on the expected results: chi2 value, log-likelihood, simulation
+table reference, and tolerances.
+
+After download, all necessary files are already pregenerated.
+
+Further, installation of the petabtests module installs a routine to recreate
+the problem and solution files for all test problems. It can be invoked via
+
+    cd petab_test_suite
+    petabtests_create
+
+## Evaluate results
+
+To evaluate how a tool performs on a given test problem, three metrics are
+employed: Simulations, chi2 value and log-likelihood. A tool can be said to
+cover a test problem if any of those values matches the ground truth values
+up to some tolerance.
+
+The python module provides convenience functions for evaluation in
+[petabtests/evaluate.py](petabtests/evaluate.py).
+
+-> [Overview of passed test cases for different tools supporting PEtab](https://github.com/PEtab-dev/PEtab#petab-features-supported-in-different-tools)
```

### Comparing `petabtests-0.0.0a6/README.md` & `petabtests-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `petabtests-0.0.0a6/petabtests/cases/0001/0001.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/0015.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,65 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 1
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests parametric noise parameter overrides in the measurement table.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1]
+    MEASUREMENT: [0.7, 0.1],
+    NOISE_PARAMETERS: ['noise', 'noise']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: [0.5]
+    NOISE_FORMULA: ['noiseParameter1_obs_a']
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 4,
-    LOWER_BOUND: [0] * 4,
-    UPPER_BOUND: [10] * 4,
-    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
-    ESTIMATE: [1] * 4,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'noise'],
+    PARAMETER_SCALE: [LIN] * 5,
+    LOWER_BOUND: [0] * 5,
+    UPPER_BOUND: [10] * 5,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 5],
+    ESTIMATE: [1] * 5,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=15,
+    brief="Simulation. Single parametric noise parameter override.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0001/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_model.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0001/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/_model.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0002/0002.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/0015.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,65 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 2
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests parametric noise parameter overrides in the measurement table.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
-    CONDITION_ID: ['c0', 'c1'],
-    'a0': [0.8, 0.9]
+    CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a'] * 4,
-    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c1', 'c1'],
-    TIME: [0, 10, 0, 10],
-    MEASUREMENT: [0.7, 0.1, 0.8, 0.2]
+    OBSERVABLE_ID: ['obs_a', 'obs_a'],
+    SIMULATION_CONDITION_ID: ['c0', 'c0'],
+    TIME: [0, 10],
+    MEASUREMENT: [0.7, 0.1],
+    NOISE_PARAMETERS: ['noise', 'noise']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: [1]
+    NOISE_FORMULA: ['noiseParameter1_obs_a']
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['b0', 'k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 3,
-    LOWER_BOUND: [0] * 3,
-    UPPER_BOUND: [10] * 3,
-    NOMINAL_VALUE: [0, 0.8, 0.6],
-    ESTIMATE: [1] * 3,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'noise'],
+    PARAMETER_SCALE: [LIN] * 5,
+    LOWER_BOUND: [0] * 5,
+    UPPER_BOUND: [10] * 5,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 5],
+    ESTIMATE: [1] * 5,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [*[analytical_a(t, 0.8, 0, 0.8, 0.6)
-                               for t in [0, 10]],
-                             *[analytical_a(t, 0.9, 0, 0.8, 0.6)
-                               for t in [0, 10]]]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+                             for t in simulation_df[TIME]]
+
+case = PetabTestCase(
+    id=15,
+    brief="Simulation. Single parametric noise parameter override.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0002/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/conversion_modified.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0002/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0011/conversion_modified.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0003/0003.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0014/0014.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 3
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests numeric noise parameter overrides in the measurement table.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1],
-    OBSERVABLE_PARAMETERS: ['0.5;2', '0.5;2']
+    NOISE_PARAMETERS: ['0.5;2', '0.5;2']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A + '
-                         'observableParameter2_obs_a'],
-    NOISE_FORMULA: [0.5]
+    OBSERVABLE_FORMULA: ['A'],
+    NOISE_FORMULA: ['noiseParameter1_obs_a + noiseParameter2_obs_a']
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
@@ -39,16 +45,21 @@
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=14,
+    brief="Simulation. Multiple numeric noise parameter overrides.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0003/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_model.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0003/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/_model.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0004/0004.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0015/0015.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,65 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 4
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests parametric noise parameter overrides in the measurement table.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1],
+    NOISE_PARAMETERS: ['noise', 'noise']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['scaling_A * A + offset_A'],
-    NOISE_FORMULA: [1]
+    OBSERVABLE_FORMULA: ['A'],
+    NOISE_FORMULA: ['noiseParameter1_obs_a']
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'scaling_A', 'offset_A'],
-    PARAMETER_SCALE: [LIN] * 6,
-    LOWER_BOUND: [0] * 6,
-    UPPER_BOUND: [10] * 6,
-    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 0.5, 2],
-    ESTIMATE: [1] * 6,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'noise'],
+    PARAMETER_SCALE: [LIN] * 5,
+    LOWER_BOUND: [0] * 5,
+    UPPER_BOUND: [10] * 5,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 5],
+    ESTIMATE: [1] * 5,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=15,
+    brief="Simulation. Single parametric noise parameter override.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0004/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/conversion_modified.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0004/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0013/conversion_modified.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0005/0005.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0005/0005.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,31 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import PetabTestCase, analytical_a
 
-test_id = 5
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for parametric overrides from condition table.
+
+The model is to be simulated for two different experimental conditions
+(here: different initial concentrations). The observable is offsetted by
+a parametric override in the condition table (i.e. the actual value has
+to be taken from the parameter table).
+
+## Model
 
-model = 'conversion_modified.xml'
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0', 'c1'],
     'offset_A': ['offset_A_c0', 'offset_A_c1'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
@@ -34,21 +46,26 @@
     PARAMETER_SCALE: [LIN] * 6,
     LOWER_BOUND: [0] * 6,
     UPPER_BOUND: [10] * 6,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6, 2, 3],
     ESTIMATE: [1] * 6,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 simulation_df[SIMULATION] = [analytical_a(10, 1, 0, 0.8, 0.6) + offset
                              for offset in [2, 3]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=5,
+    brief="Simulation. Condition-specific parameters only defined in "
+          "parameter table.",
+    description=DESCRIPTION,
+    model='conversion_modified_pysb.py',
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0005/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/_model.xml`

 * *Files identical despite different names*

### Comparing `petabtests-0.0.0a6/petabtests/cases/0005/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/conversion_modified.xml`

 * *Files identical despite different names*

### Comparing `petabtests-0.0.0a6/petabtests/cases/0006/0006.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/0014.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,65 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 6
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests numeric noise parameter overrides in the measurement table.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1],
-    OBSERVABLE_PARAMETERS: [10, 15]
+    NOISE_PARAMETERS: ['0.5;2', '0.5;2']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A'],
-    NOISE_FORMULA: [1]
+    OBSERVABLE_FORMULA: ['A'],
+    NOISE_FORMULA: ['noiseParameter1_obs_a + noiseParameter2_obs_a']
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [10 * analytical_a(0, 1, 0, 0.8, 0.6),
-                             15 * analytical_a(10, 1, 0, 0.8, 0.6)]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+                             for t in simulation_df[TIME]]
 
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=14,
+    brief="Simulation. Multiple numeric noise parameter overrides.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0006/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_model.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0006/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/_model.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0007/0007.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/0014.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,65 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 7
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests numeric noise parameter overrides in the measurement table.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_b'],
+    OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [10, 10],
-    MEASUREMENT: [0.2, 0.8]
+    TIME: [0, 10],
+    MEASUREMENT: [0.7, 0.1],
+    NOISE_PARAMETERS: ['0.5;2', '0.5;2']
 })
 
 observable_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_b'],
-    OBSERVABLE_FORMULA: ['A', 'B'],
-    OBSERVABLE_TRANSFORMATION: [LIN, LOG10],
-    NOISE_FORMULA: [0.5, 0.6]
+    OBSERVABLE_ID: ['obs_a'],
+    OBSERVABLE_FORMULA: ['A'],
+    NOISE_FORMULA: ['noiseParameter1_obs_a + noiseParameter2_obs_a']
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [
-    analytical_a(10, 1, 0, 0.8, 0.6),
-    analytical_b(10, 1, 0, 0.8, 0.6),
-]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+                             for t in simulation_df[TIME]]
+
+case = PetabTestCase(
+    id=14,
+    brief="Simulation. Multiple numeric noise parameter overrides.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0007/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/conversion_modified.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0007/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0011/conversion_modified.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0008/0008.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0003/0003.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,74 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 8
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for numeric observable parameter overrides in
+measurement tables
+
+Simulated data describes measurements with different offset and scaling
+parameters for a single observable. These respective numeric
+`observableParameters`
+from the measurement table have to be applied to the placeholders in
+observableFormula.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_a', 'obs_a'],
-    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c0'],
-    TIME: [0, 10, 10],
-    MEASUREMENT: [0.7, 0.1, 0.2]
+    OBSERVABLE_ID: ['obs_a', 'obs_a'],
+    SIMULATION_CONDITION_ID: ['c0', 'c0'],
+    TIME: [0, 10],
+    MEASUREMENT: [0.7, 0.1],
+    OBSERVABLE_PARAMETERS: ['0.5;2', '0.5;2']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['A'],
+    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A + '
+                         'observableParameter2_obs_a'],
     NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=3,
+    brief="Simulation. Numeric observable parameter overrides in measurement "
+          "table.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0008/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_model.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0008/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/_model.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0009/0009.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0009/0009.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import (DEFAULT_PYSB_FILE, PetabTestCase, analytical_a,
+                        analytical_b)
 
-test_id = 9
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for preequilibration.
+
+The model is to be simulated for a preequilibration condition and a
+simulation condition.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['preeq_c0', 'c0'],
     'k1': [0.3, 0.8],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
@@ -35,26 +46,30 @@
     PARAMETER_SCALE: [LIN] * 3,
     LOWER_BOUND: [0] * 3,
     UPPER_BOUND: [10] * 3,
     NOMINAL_VALUE: [1, 0, 0.6],
     ESTIMATE: [1] * 3,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 # simulate for far time point as steady state
 steady_state_a = analytical_a(1000, 1, 0, 0.3, 0.6)
 steady_state_b = analytical_b(1000, 1, 0, 0.3, 0.6)
 # use steady state as initial state
 simulation_df[SIMULATION] = [
     analytical_a(t, steady_state_a, steady_state_b, 0.8, 0.6)
     for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=9,
+    brief="Simulation. Preequilibration.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0009/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/conversion_modified.xml`

 * *Files 2% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0009/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0013/conversion_modified.xml`

```diff
@@ -18,29 +18,23 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
-      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
-      <initialAssignment symbol="B">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>b0</ci>
-        </math>
-      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0010/0010.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/0008.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,67 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 10
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for replicate measurements.
+
+The model is to be simulated for a single experimental condition. The single
+model output has multiple measurements for the same condition and timepoint.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
-    CONDITION_ID: ['preeq_c0', 'c0'],
-    'k1': [0.3, 0.8],
-    'B': [0, 0],
+    CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_a'],
-    PREEQUILIBRATION_CONDITION_ID: ['preeq_c0', 'preeq_c0'],
-    SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [1, 10],
-    MEASUREMENT: [0.7, 0.1]
+    OBSERVABLE_ID: ['obs_a', 'obs_a', 'obs_a'],
+    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c0'],
+    TIME: [0, 10, 10],
+    MEASUREMENT: [0.7, 0.1, 0.2]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
     NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['k2'],
-    PARAMETER_SCALE: [LIN],
-    LOWER_BOUND: [0],
-    UPPER_BOUND: [10],
-    NOMINAL_VALUE: [0.6],
-    ESTIMATE: [1],
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 4,
+    LOWER_BOUND: [0] * 4,
+    UPPER_BOUND: [10] * 4,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
+    ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-# simulate for far time point as steady state
-steady_state_a = analytical_a(1000, 1, 0, 0.3, 0.6)
-# use steady state as initial state
-simulation_df[SIMULATION] = [
-    analytical_a(t, steady_state_a, 0, 0.8, 0.6)
-    for t in simulation_df[TIME]]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+                             for t in simulation_df[TIME]]
+
+case = PetabTestCase(
+    id=8,
+    brief="Simulation. Replicate measurements.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0010/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/conversion_modified.xml`

 * *Files 3% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0010/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/conversion_modified.xml`

```diff
@@ -17,25 +17,19 @@
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
-      <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
-      <initialAssignment symbol="A">
-        <math xmlns="http://www.w3.org/1998/Math/MathML">
-          <ci>a0</ci>
-        </math>
-      </initialAssignment>
       <initialAssignment symbol="B">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>b0</ci>
         </math>
       </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0010/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/conversion_modified.xml`

 * *Files identical despite different names*

### Comparing `petabtests-0.0.0a6/petabtests/cases/0011/0011.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/0006.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,70 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 11
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for time-point specific overrides in the measurement
+table.
+
+The model is to be simulated for a single experimental condition. The single
+model output is scaled by a different parameter at each timepoint.
+
+## Model
 
-model = 'conversion_modified.xml'
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
-    'B': [2]
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1]
+    MEASUREMENT: [0.7, 0.1],
+    OBSERVABLE_PARAMETERS: [10, 15]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: [0.5]
+    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A'],
+    NOISE_FORMULA: [1]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 2,
-    LOWER_BOUND: [0] * 2,
-    UPPER_BOUND: [10] * 2,
-    NOMINAL_VALUE: [0.8, 0.6],
-    ESTIMATE: [1] * 2,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 4,
+    LOWER_BOUND: [0] * 4,
+    UPPER_BOUND: [10] * 4,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
+    ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [analytical_a(t, 1, 2, 0.8, 0.6)
-                             for t in simulation_df[TIME]]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
+simulation_df[SIMULATION] = [10 * analytical_a(0, 1, 0, 0.8, 0.6),
+                             15 * analytical_a(10, 1, 0, 0.8, 0.6)]
 
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=6,
+    brief="Simulation. Time-point specific numeric observable parameter "
+          "overrides.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0011/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_model.xml`

 * *Files 4% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0011/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/_model.xml`

```diff
@@ -18,23 +18,30 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
+      <parameter id="offset_A" name="offset_A" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0011/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/conversion_modified.xml`

 * *Files 4% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0011/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/conversion_modified.xml`

```diff
@@ -18,23 +18,30 @@
     </listOfCompartments>
     <listOfSpecies>
       <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
       <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
+      <parameter id="offset_A" name="offset_A" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0012/0012.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/0008.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,67 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 12
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for replicate measurements.
+
+The model is to be simulated for a single experimental condition. The single
+model output has multiple measurements for the same condition and timepoint.
 
-model = DEFAULT_SBML_FILE
+## Model
+
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
-    'compartment': [3],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_a'],
-    SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1]
+    OBSERVABLE_ID: ['obs_a', 'obs_a', 'obs_a'],
+    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c0'],
+    TIME: [0, 10, 10],
+    MEASUREMENT: [0.7, 0.1, 0.2]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
     NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 2,
-    LOWER_BOUND: [0] * 2,
-    UPPER_BOUND: [10] * 2,
-    NOMINAL_VALUE: [0.8, 0.6],
-    ESTIMATE: [1] * 2,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 4,
+    LOWER_BOUND: [0] * 4,
+    UPPER_BOUND: [10] * 4,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
+    ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-# in the model, concentrations are used, which do not depend on the
-#  compartment size, so that the species values should stay the same
-simulation_df[SIMULATION] = [analytical_a(t, 1, 1, 0.8, 0.6)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=8,
+    brief="Simulation. Replicate measurements.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0012/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0012/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0013/0013.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0013/0013.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,26 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import PetabTestCase, analytical_a
 
-test_id = 13
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests parametric initial concentrations in the condition table.
+
+## Model
 
-model = 'conversion_modified.xml'
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
     'B': ['par'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
@@ -34,23 +41,34 @@
     PARAMETER_SCALE: [LIN] * 3,
     LOWER_BOUND: [0] * 3,
     UPPER_BOUND: [10] * 3,
     NOMINAL_VALUE: [0.8, 0.6, 7],
     ESTIMATE: [1] * 3,
 }).set_index(PARAMETER_ID)
 
+mapping_df = pd.DataFrame(data={
+    PETAB_ENTITY_ID: ['A', 'B'],
+    MODEL_ENTITY_ID: ['A_() ** compartment', 'B_() ** compartment'],
+}).set_index(PETAB_ENTITY_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 # in the model, concentrations are used, which do not depend on the
 #  compartment size, so that the species values should stay the same
 simulation_df[SIMULATION] = [analytical_a(t, 1, 7, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=13,
+    brief="Simulation. Species with InitialAssignment overridden by "
+          "parameter.",
+    description=DESCRIPTION,
+    model='conversion_modified_pysb.py',
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+    mapping_df=mapping_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0013/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_model.xml`

 * *Files 6% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0013/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0002/_model.xml`

```diff
@@ -13,28 +13,34 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0013/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_model.xml`

 * *Files 6% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0013/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/_model.xml`

```diff
@@ -13,28 +13,34 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0014/0014.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0008/0008.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,67 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 14
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for replicate measurements.
+
+The model is to be simulated for a single experimental condition. The single
+model output has multiple measurements for the same condition and timepoint.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_a'],
-    SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1],
-    NOISE_PARAMETERS: ['0.5;2', '0.5;2']
+    OBSERVABLE_ID: ['obs_a', 'obs_a', 'obs_a'],
+    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c0'],
+    TIME: [0, 10, 10],
+    MEASUREMENT: [0.7, 0.1, 0.2]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: ['noiseParameter1_obs_a + noiseParameter2_obs_a']
+    NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=8,
+    brief="Simulation. Replicate measurements.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0014/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0014/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0015/0015.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0003/0003.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,74 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 15
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for numeric observable parameter overrides in
+measurement tables
+
+Simulated data describes measurements with different offset and scaling
+parameters for a single observable. These respective numeric
+`observableParameters`
+from the measurement table have to be applied to the placeholders in
+observableFormula.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1],
-    NOISE_PARAMETERS: ['noise', 'noise']
+    OBSERVABLE_PARAMETERS: ['0.5;2', '0.5;2']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: ['noiseParameter1_obs_a']
+    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A + '
+                         'observableParameter2_obs_a'],
+    NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'noise'],
-    PARAMETER_SCALE: [LIN] * 5,
-    LOWER_BOUND: [0] * 5,
-    UPPER_BOUND: [10] * 5,
-    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 5],
-    ESTIMATE: [1] * 5,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 4,
+    LOWER_BOUND: [0] * 4,
+    UPPER_BOUND: [10] * 4,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
+    ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=3,
+    brief="Simulation. Numeric observable parameter overrides in measurement "
+          "table.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0015/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0015/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0006/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0016/0016.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/0006.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,70 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 16
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for time-point specific overrides in the measurement
+table.
+
+The model is to be simulated for a single experimental condition. The single
+model output is scaled by a different parameter at each timepoint.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_b'],
+    OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [10, 10],
-    MEASUREMENT: [0.2, 0.8]
+    TIME: [0, 10],
+    MEASUREMENT: [0.7, 0.1],
+    OBSERVABLE_PARAMETERS: [10, 15]
 })
 
 observable_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_b'],
-    OBSERVABLE_FORMULA: ['A', 'B'],
-    OBSERVABLE_TRANSFORMATION: [LIN, LOG],
-    NOISE_FORMULA: [0.5, 0.7]
+    OBSERVABLE_ID: ['obs_a'],
+    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A'],
+    NOISE_FORMULA: [1]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [
-    analytical_a(10, 1, 0, 0.8, 0.6),
-    analytical_b(10, 1, 0, 0.8, 0.6),
-]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [10 * analytical_a(0, 1, 0, 0.8, 0.6),
+                             15 * analytical_a(10, 1, 0, 0.8, 0.6)]
+
+case = PetabTestCase(
+    id=6,
+    brief="Simulation. Time-point specific numeric observable parameter "
+          "overrides.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/0016/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/0016/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0007/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0001/0001.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/0003.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,50 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 1
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for numeric observable parameter overrides in
+measurement tables
+
+Simulated data describes measurements with different offset and scaling
+parameters for a single observable. These respective numeric
+`observableParameters`
+from the measurement table have to be applied to the placeholders in
+observableFormula.
 
-model = DEFAULT_SBML_FILE
+## Model
+
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1]
+    MEASUREMENT: [0.7, 0.1],
+    OBSERVABLE_PARAMETERS: ['0.5;2', '0.5;2']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['A'],
+    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A + '
+                         'observableParameter2_obs_a'],
     NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
@@ -37,16 +53,22 @@
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=3,
+    brief="Simulation. Numeric observable parameter overrides in measurement "
+          "table.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0001/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0001/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0008/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0002/0002.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0006/0006.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,70 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 2
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for time-point specific overrides in the measurement
+table.
+
+The model is to be simulated for a single experimental condition. The single
+model output is scaled by a different parameter at each timepoint.
 
-model = DEFAULT_SBML_FILE
+## Model
+
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
-    CONDITION_ID: ['c0', 'c1'],
-    'a0': [0.8, 0.9]
+    CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a'] * 4,
-    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c1', 'c1'],
-    TIME: [0, 10, 0, 10],
-    MEASUREMENT: [0.7, 0.1, 0.8, 0.2]
+    OBSERVABLE_ID: ['obs_a', 'obs_a'],
+    SIMULATION_CONDITION_ID: ['c0', 'c0'],
+    TIME: [0, 10],
+    MEASUREMENT: [0.7, 0.1],
+    OBSERVABLE_PARAMETERS: [10, 15]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['A'],
+    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A'],
     NOISE_FORMULA: [1]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['b0', 'k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 3,
-    LOWER_BOUND: [0] * 3,
-    UPPER_BOUND: [10] * 3,
-    NOMINAL_VALUE: [0, 0.8, 0.6],
-    ESTIMATE: [1] * 3,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 4,
+    LOWER_BOUND: [0] * 4,
+    UPPER_BOUND: [10] * 4,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
+    ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [*[analytical_a(t, 0.8, 0, 0.8, 0.6)
-                               for t in [0, 10]],
-                             *[analytical_a(t, 0.9, 0, 0.8, 0.6)
-                               for t in [0, 10]]]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [10 * analytical_a(0, 1, 0, 0.8, 0.6),
+                             15 * analytical_a(10, 1, 0, 0.8, 0.6)]
+
+case = PetabTestCase(
+    id=6,
+    brief="Simulation. Time-point specific numeric observable parameter "
+          "overrides.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0002/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0002/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0003/0003.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0004/0004.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,71 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 3
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for parametric observable parameter overrides in
+measurement tables
+
+Simulated data describes measurements with different offset and scaling
+parameters for a single observable. These values of the respective
+(non-estimated) parameters referenced in `observableParameters` need to be
+looked up in the parameter table to replace the placeholders in
+`observableFormula`.
 
-model = DEFAULT_SBML_FILE
+## Model
+
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1],
-    OBSERVABLE_PARAMETERS: ['0.5;2', '0.5;2']
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A + '
-                         'observableParameter2_obs_a'],
-    NOISE_FORMULA: [0.5]
+    OBSERVABLE_FORMULA: ['scaling_A * A + offset_A'],
+    NOISE_FORMULA: [1]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 4,
-    LOWER_BOUND: [0] * 4,
-    UPPER_BOUND: [10] * 4,
-    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
-    ESTIMATE: [1] * 4,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'scaling_A', 'offset_A'],
+    PARAMETER_SCALE: [LIN] * 6,
+    LOWER_BOUND: [0] * 6,
+    UPPER_BOUND: [10] * 6,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 0.5, 2],
+    ESTIMATE: [1] * 6,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=4,
+    brief="Simulation. Observable parameters only defined in parameter table.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0003/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0003/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0010/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0004/0004.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0004/0004.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,33 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 4
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for parametric observable parameter overrides in
+measurement tables
+
+Simulated data describes measurements with different offset and scaling
+parameters for a single observable. These values of the respective
+(non-estimated) parameters referenced in `observableParameters` need to be
+looked up in the parameter table to replace the placeholders in
+`observableFormula`.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
@@ -33,21 +47,25 @@
     PARAMETER_SCALE: [LIN] * 6,
     LOWER_BOUND: [0] * 6,
     UPPER_BOUND: [10] * 6,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6, 0.5, 2],
     ESTIMATE: [1] * 6,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=4,
+    brief="Simulation. Observable parameters only defined in parameter table.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0004/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0004/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0012/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0005/0005.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0005/0005.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,32 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
+from pathlib import Path
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import PetabTestCase, analytical_a
 
-test_id = 5
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for parametric overrides from condition table.
+
+The model is to be simulated for two different experimental conditions
+(here: different initial concentrations). The observable is offsetted by
+a parametric override in the condition table (i.e. the actual value has
+to be taken from the parameter table).
+
+## Model
 
-model = 'conversion_modified.xml'
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0', 'c1'],
     'offset_A': ['offset_A_c0', 'offset_A_c1'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
@@ -34,21 +47,26 @@
     PARAMETER_SCALE: [LIN] * 6,
     LOWER_BOUND: [0] * 6,
     UPPER_BOUND: [10] * 6,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6, 2, 3],
     ESTIMATE: [1] * 6,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 simulation_df[SIMULATION] = [analytical_a(10, 1, 0, 0.8, 0.6) + offset
                              for offset in [2, 3]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=5,
+    brief="Simulation. Condition-specific parameters only defined in "
+          "parameter table.",
+    description=DESCRIPTION,
+    model=Path('conversion_modified.xml'),
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0005/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_model.xml`

 * *Files 7% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0005/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0014/_model.xml`

```diff
@@ -13,23 +13,22 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
-      <parameter id="offset_A" name="offset_A" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0005/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_model.xml`

 * *Files 7% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0005/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0015/_model.xml`

```diff
@@ -13,23 +13,22 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
-      <parameter id="offset_A" name="offset_A" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0006/0006.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0001/0001.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 6
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case features a simple test with two data points and no particular
+features.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1],
-    OBSERVABLE_PARAMETERS: [10, 15]
+    MEASUREMENT: [0.7, 0.1]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['observableParameter1_obs_a * A'],
-    NOISE_FORMULA: [1]
+    OBSERVABLE_FORMULA: ['A'],
+    NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [10 * analytical_a(0, 1, 0, 0.8, 0.6),
-                             15 * analytical_a(10, 1, 0, 0.8, 0.6)]
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+                             for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
 
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=1,
+    brief="Simulation. Nothing special.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0006/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0006/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0016/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0007/0007.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0019/0019.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,74 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 7
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+Test different model entities inside the mapping table.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
 
+# problem --------------------------------------------------------------------
+# TODO use mapping here
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_b'],
+    OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [10, 10],
-    MEASUREMENT: [0.2, 0.8]
+    TIME: [0, 10],
+    MEASUREMENT: [0.7, 0.1]
 })
 
 observable_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_b'],
-    OBSERVABLE_FORMULA: ['A', 'B'],
-    OBSERVABLE_TRANSFORMATION: [LIN, LOG10],
-    NOISE_FORMULA: [0.5, 0.6]
+    OBSERVABLE_ID: ['obs_a'],
+    OBSERVABLE_FORMULA: ['maps_to_A'],
+    NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
+    PARAMETER_ID: ['a0', 'maps_to_b0', 'k1', 'maps_to_k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [
-    analytical_a(10, 1, 0, 0.8, 0.6),
-    analytical_b(10, 1, 0, 0.8, 0.6),
-]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+                             for t in simulation_df[TIME]]
+
+mapping_df = pd.DataFrame(data={
+    PETAB_ENTITY_ID:
+        ['maps_to_a0', 'maps_to_b0', 'maps_to_k1',
+         'maps_to_k2', 'maps_to_A', 'maps_to_B'],
+    MODEL_ENTITY_ID:
+        ['a0', 'b0', 'k1', 'k2', 'A', 'B'],
+}).set_index(PETAB_ENTITY_ID)
+
+case = PetabTestCase(
+    id=19,
+    brief="Mapping table.",
+    description=DESCRIPTION,
+    # TODO add local parameter and use in mapping table
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+    mapping_df=mapping_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0007/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0007/_model.xml` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0017/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0008/0008.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/0004.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,71 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 8
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for parametric observable parameter overrides in
+measurement tables
+
+Simulated data describes measurements with different offset and scaling
+parameters for a single observable. These values of the respective
+(non-estimated) parameters referenced in `observableParameters` need to be
+looked up in the parameter table to replace the placeholders in
+`observableFormula`.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_a', 'obs_a'],
-    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c0'],
-    TIME: [0, 10, 10],
-    MEASUREMENT: [0.7, 0.1, 0.2]
+    OBSERVABLE_ID: ['obs_a', 'obs_a'],
+    SIMULATION_CONDITION_ID: ['c0', 'c0'],
+    TIME: [0, 10],
+    MEASUREMENT: [0.7, 0.1],
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: [0.5]
+    OBSERVABLE_FORMULA: ['scaling_A * A + offset_A'],
+    NOISE_FORMULA: [1]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 4,
-    LOWER_BOUND: [0] * 4,
-    UPPER_BOUND: [10] * 4,
-    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
-    ESTIMATE: [1] * 4,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'scaling_A', 'offset_A'],
+    PARAMETER_SCALE: [LIN] * 6,
+    LOWER_BOUND: [0] * 6,
+    UPPER_BOUND: [10] * 6,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 0.5, 2],
+    ESTIMATE: [1] * 6,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
+simulation_df[SIMULATION] = [0.5 * analytical_a(t, 1, 0, 0.8, 0.6) + 2
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=4,
+    brief="Simulation. Observable parameters only defined in parameter table.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0008/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0008/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0009/0009.py` & `petabtests-0.0.1/petabtests/cases/v1.0.0/sbml/0009/0009.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import (DEFAULT_SBML_FILE, PetabTestCase, analytical_a,
+                        analytical_b)
 
-test_id = 9
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for preequilibration.
+
+The model is to be simulated for a preequilibration condition and a
+simulation condition.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['preeq_c0', 'c0'],
     'k1': [0.3, 0.8],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
@@ -35,26 +46,30 @@
     PARAMETER_SCALE: [LIN] * 3,
     LOWER_BOUND: [0] * 3,
     UPPER_BOUND: [10] * 3,
     NOMINAL_VALUE: [1, 0, 0.6],
     ESTIMATE: [1] * 3,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 # simulate for far time point as steady state
 steady_state_a = analytical_a(1000, 1, 0, 0.3, 0.6)
 steady_state_b = analytical_b(1000, 1, 0, 0.3, 0.6)
 # use steady state as initial state
 simulation_df[SIMULATION] = [
     analytical_a(t, steady_state_a, steady_state_b, 0.8, 0.6)
     for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=9,
+    brief="Simulation. Preequilibration.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0009/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0009/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0002/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0010/0010.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0011/0011.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,73 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import PetabTestCase, analytical_a
 
-test_id = 10
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests initial concentrations in the condition table.
+For species `B`, the initial concentration is specified in the condition
+table, while for `A` it is given via an assignment rule in the SBML model.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
-    CONDITION_ID: ['preeq_c0', 'c0'],
-    'k1': [0.3, 0.8],
-    'B': [0, 0],
+    CONDITION_ID: ['c0'],
+    'B': [2]
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
-    PREEQUILIBRATION_CONDITION_ID: ['preeq_c0', 'preeq_c0'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [1, 10],
+    TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
     NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['k2'],
-    PARAMETER_SCALE: [LIN],
-    LOWER_BOUND: [0],
-    UPPER_BOUND: [10],
-    NOMINAL_VALUE: [0.6],
-    ESTIMATE: [1],
+    PARAMETER_ID: ['k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 2,
+    LOWER_BOUND: [0] * 2,
+    UPPER_BOUND: [10] * 2,
+    NOMINAL_VALUE: [0.8, 0.6],
+    ESTIMATE: [1] * 2,
 }).set_index(PARAMETER_ID)
 
+mapping_df = pd.DataFrame(data={
+    PETAB_ENTITY_ID: ['A', 'B'],
+    MODEL_ENTITY_ID: ['A_() ** compartment', 'B_() ** compartment'],
+}).set_index(PETAB_ENTITY_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-# simulate for far time point as steady state
-steady_state_a = analytical_a(1000, 1, 0, 0.3, 0.6)
-# use steady state as initial state
-simulation_df[SIMULATION] = [
-    analytical_a(t, steady_state_a, 0, 0.8, 0.6)
-    for t in simulation_df[TIME]]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 2, 0.8, 0.6)
+                             for t in simulation_df[TIME]]
+
+case = PetabTestCase(
+    id=11,
+    brief="Simulation. InitialAssignment to species overridden.",
+    description=DESCRIPTION,
+    model='conversion_modified_pysb.py',
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+    mapping_df=mapping_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0010/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0010/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0003/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0010/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_model.xml`

 * *Files 12% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0010/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0004/_model.xml`

```diff
@@ -13,23 +13,29 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
+      <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
+      <initialAssignment symbol="A">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>a0</ci>
+        </math>
+      </initialAssignment>
       <initialAssignment symbol="B">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>b0</ci>
         </math>
       </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0011/0011.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0018/0018.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 11
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests parameters in mapping table.
+
+## Model
 
-model = 'conversion_modified.xml'
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
-    'B': [2]
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1]
@@ -26,29 +32,41 @@
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
     NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 2,
-    LOWER_BOUND: [0] * 2,
-    UPPER_BOUND: [10] * 2,
-    NOMINAL_VALUE: [0.8, 0.6],
-    ESTIMATE: [1] * 2,
+    PARAMETER_ID: ['maps_to_a0', 'b0', 'maps_to_k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 4,
+    LOWER_BOUND: [0] * 4,
+    UPPER_BOUND: [10] * 4,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
+    ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
+mapping_df = pd.DataFrame(data={
+    PETAB_ENTITY_ID: ['maps_to_a0', 'maps_to_b0', 'maps_to_k1', 'maps_to_k2'],
+    MODEL_ENTITY_ID: ['a0', 'b0', 'k1', 'k2'],
+}).set_index(PETAB_ENTITY_ID)
+
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [analytical_a(t, 1, 2, 0.8, 0.6)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
 
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=18,
+    brief="Parameters in mapping table.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+    mapping_df=mapping_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0011/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_model.xml`

 * *Files 6% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0011/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0006/_model.xml`

```diff
@@ -13,28 +13,34 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0011/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_model.xml`

 * *Files 6% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0011/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0007/_model.xml`

```diff
@@ -13,28 +13,34 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0012/0012.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0001/0001.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 12
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case features a simple test with two data points and no particular
+features.
 
-model = DEFAULT_SBML_FILE
+## Model
+
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
-    'compartment': [3],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
     MEASUREMENT: [0.7, 0.1]
@@ -26,30 +33,34 @@
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
     NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['k1', 'k2'],
-    PARAMETER_SCALE: [LIN] * 2,
-    LOWER_BOUND: [0] * 2,
-    UPPER_BOUND: [10] * 2,
-    NOMINAL_VALUE: [0.8, 0.6],
-    ESTIMATE: [1] * 2,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 4,
+    LOWER_BOUND: [0] * 4,
+    UPPER_BOUND: [10] * 4,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6],
+    ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-# in the model, concentrations are used, which do not depend on the
-#  compartment size, so that the species values should stay the same
-simulation_df[SIMULATION] = [analytical_a(t, 1, 1, 0.8, 0.6)
+simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
 
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=1,
+    brief="Simulation. Nothing special.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0012/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0012/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0008/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0013/0013.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/pysb/0002/0002.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,75 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
+from math import nan
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_PYSB_FILE, PetabTestCase, analytical_a
 
-test_id = 13
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for multiple simulation conditions
+
+The model is to be simulated for two different experimental conditions
+(here: different initial concentrations).
+
+For `b0`, `nan` is used in the condition table, indicating that the default
+model values for `b0` should be used for either condition.
 
-model = 'conversion_modified.xml'
+## Model
+
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
-    CONDITION_ID: ['c0'],
-    'B': ['par'],
+    CONDITION_ID: ['c0', 'c1'],
+    'a0': [0.8, 0.9],
+    'b0': [nan, nan],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
-    OBSERVABLE_ID: ['obs_a', 'obs_a'],
-    SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1]
+    OBSERVABLE_ID: ['obs_a'] * 4,
+    SIMULATION_CONDITION_ID: ['c0', 'c0', 'c1', 'c1'],
+    TIME: [0, 10, 0, 10],
+    MEASUREMENT: [0.7, 0.1, 0.8, 0.2]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: [0.5]
+    NOISE_FORMULA: [1]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['k1', 'k2', 'par'],
-    PARAMETER_SCALE: [LIN] * 3,
-    LOWER_BOUND: [0] * 3,
-    UPPER_BOUND: [10] * 3,
-    NOMINAL_VALUE: [0.8, 0.6, 7],
-    ESTIMATE: [1] * 3,
+    PARAMETER_ID: ['k1', 'k2'],
+    PARAMETER_SCALE: [LIN] * 2,
+    LOWER_BOUND: [0] * 2,
+    UPPER_BOUND: [10] * 2,
+    NOMINAL_VALUE: [0.8, 0.6],
+    ESTIMATE: [1] * 2,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-# in the model, concentrations are used, which do not depend on the
-#  compartment size, so that the species values should stay the same
-simulation_df[SIMULATION] = [analytical_a(t, 1, 7, 0.8, 0.6)
-                             for t in simulation_df[TIME]]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
-
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+simulation_df[SIMULATION] = [*[analytical_a(t, 0.8, 1, 0.8, 0.6)
+                               for t in [0, 10]],
+                             *[analytical_a(t, 0.9, 1, 0.8, 0.6)
+                               for t in [0, 10]]]
+
+case = PetabTestCase(
+    id=2,
+    brief="Simulation. Two conditions. Numeric parameter override.",
+    description=DESCRIPTION,
+    model=DEFAULT_PYSB_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0013/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_model.xml`

 * *Files 6% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0013/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0009/_model.xml`

```diff
@@ -13,28 +13,34 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0013/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_model.xml`

 * *Files 6% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0013/conversion_modified.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0010/_model.xml`

```diff
@@ -13,28 +13,34 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
+      <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
     <listOfInitialAssignments>
       <initialAssignment symbol="A">
         <math xmlns="http://www.w3.org/1998/Math/MathML">
           <ci>a0</ci>
         </math>
       </initialAssignment>
+      <initialAssignment symbol="B">
+        <math xmlns="http://www.w3.org/1998/Math/MathML">
+          <ci>b0</ci>
+        </math>
+      </initialAssignment>
     </listOfInitialAssignments>
     <listOfReactions>
       <reaction id="fwd" name="fwd" reversible="false">
         <listOfReactants>
           <speciesReference species="A" stoichiometry="1"/>
         </listOfReactants>
         <listOfProducts>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0014/0014.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0001/0001.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import DEFAULT_SBML_FILE, PetabTestCase, analytical_a
 
-test_id = 14
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case features a simple test with two data points and no particular
+features.
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
     CONDITION_ID: ['c0'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
     SIMULATION_CONDITION_ID: ['c0', 'c0'],
     TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1],
-    NOISE_PARAMETERS: ['0.5;2', '0.5;2']
+    MEASUREMENT: [0.7, 0.1]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
     OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: ['noiseParameter1_obs_a + noiseParameter2_obs_a']
+    NOISE_FORMULA: [0.5]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
     PARAMETER_ID: ['a0', 'b0', 'k1', 'k2'],
     PARAMETER_SCALE: [LIN] * 4,
     LOWER_BOUND: [0] * 4,
     UPPER_BOUND: [10] * 4,
     NOMINAL_VALUE: [1, 0, 0.8, 0.6],
     ESTIMATE: [1] * 4,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
 simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
                              for t in simulation_df[TIME]]
 
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
 
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=1,
+    brief="Simulation. Nothing special.",
+    description=DESCRIPTION,
+    model=DEFAULT_SBML_FILE,
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0014/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0014/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0012/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0015/0015.py` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0005/0005.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,72 @@
-from petabtests import *
-from petab.C import *
-import petab
+from inspect import cleandoc
+from pathlib import Path
 
 import pandas as pd
+from petab.C import *
 
+from petabtests import PetabTestCase, analytical_a
 
-test_id = 15
+DESCRIPTION = cleandoc("""
+## Objective
 
-# problem --------------------------------------------------------------------
+This case tests support for parametric overrides from condition table.
+
+The model is to be simulated for two different experimental conditions
+(here: different initial concentrations). The observable is offsetted by
+a parametric override in the condition table (i.e. the actual value has
+to be taken from the parameter table).
+
+## Model
 
-model = DEFAULT_SBML_FILE
+A simple conversion reaction `A <=> B` in a single compartment, following
+mass action kinetics.
+""")
+
+# problem --------------------------------------------------------------------
 
 condition_df = pd.DataFrame(data={
-    CONDITION_ID: ['c0'],
+    CONDITION_ID: ['c0', 'c1'],
+    'offset_A': ['offset_A_c0', 'offset_A_c1'],
 }).set_index([CONDITION_ID])
 
 measurement_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a', 'obs_a'],
-    SIMULATION_CONDITION_ID: ['c0', 'c0'],
-    TIME: [0, 10],
-    MEASUREMENT: [0.7, 0.1],
-    NOISE_PARAMETERS: ['noise', 'noise']
+    SIMULATION_CONDITION_ID: ['c0', 'c1'],
+    TIME: [10, 10],
+    MEASUREMENT: [2.1, 3.2]
 })
 
 observable_df = pd.DataFrame(data={
     OBSERVABLE_ID: ['obs_a'],
-    OBSERVABLE_FORMULA: ['A'],
-    NOISE_FORMULA: ['noiseParameter1_obs_a']
+    OBSERVABLE_FORMULA: ['A + offset_A'],
+    NOISE_FORMULA: [1]
 }).set_index([OBSERVABLE_ID])
 
 parameter_df = pd.DataFrame(data={
-    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'noise'],
-    PARAMETER_SCALE: [LIN] * 5,
-    LOWER_BOUND: [0] * 5,
-    UPPER_BOUND: [10] * 5,
-    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 5],
-    ESTIMATE: [1] * 5,
+    PARAMETER_ID: ['a0', 'b0', 'k1', 'k2', 'offset_A_c0', 'offset_A_c1'],
+    PARAMETER_SCALE: [LIN] * 6,
+    LOWER_BOUND: [0] * 6,
+    UPPER_BOUND: [10] * 6,
+    NOMINAL_VALUE: [1, 0, 0.8, 0.6, 2, 3],
+    ESTIMATE: [1] * 6,
 }).set_index(PARAMETER_ID)
 
-
 # solutions ------------------------------------------------------------------
 
 simulation_df = measurement_df.copy(deep=True).rename(
     columns={MEASUREMENT: SIMULATION})
-simulation_df[SIMULATION] = [analytical_a(t, 1, 0, 0.8, 0.6)
-                             for t in simulation_df[TIME]]
-
-chi2 = petab.calculate_chi2(
-    measurement_df, simulation_df, observable_df, parameter_df)
+simulation_df[SIMULATION] = [analytical_a(10, 1, 0, 0.8, 0.6) + offset
+                             for offset in [2, 3]]
 
-llh = petab.calculate_llh(
-    measurement_df, simulation_df, observable_df, parameter_df)
-print(llh)
+case = PetabTestCase(
+    id=5,
+    brief="Simulation. Condition-specific parameters only defined in "
+          "parameter table.",
+    description=DESCRIPTION,
+    model=Path('conversion_modified.xml'),
+    condition_dfs=[condition_df],
+    observable_dfs=[observable_df],
+    measurement_dfs=[measurement_df],
+    simulation_dfs=[simulation_df],
+    parameter_df=parameter_df,
+)
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0015/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0015/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0014/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0016/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/cases/sbml/0016/_model.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0015/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/conversion.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_model.xml`

 * *Files 5% similar despite different names*

#### Comparing `petabtests-0.0.0a6/petabtests/conversion.xml` & `petabtests-0.0.1/petabtests/cases/v2.0.0/sbml/0016/_model.xml`

```diff
@@ -13,16 +13,16 @@
         </listOfUnits>
       </unitDefinition>
     </listOfUnitDefinitions>
     <listOfCompartments>
       <compartment id="compartment" name="compartment" spatialDimensions="3" size="1" constant="true"/>
     </listOfCompartments>
     <listOfSpecies>
-      <species id="A" name="A" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
-      <species id="B" name="B" compartment="compartment" initialConcentration="1" boundaryCondition="false" constant="false"/>
+      <species id="A" name="A" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
+      <species id="B" name="B" compartment="compartment" initialConcentration="2" boundaryCondition="false" constant="false"/>
     </listOfSpecies>
     <listOfParameters>
       <parameter id="a0" name="a0" value="1" constant="true"/>
       <parameter id="b0" name="b0" value="1" constant="true"/>
       <parameter id="k1" name="k1" value="0" constant="true"/>
       <parameter id="k2" name="k2" value="0" constant="true"/>
     </listOfParameters>
```

### Comparing `petabtests-0.0.0a6/petabtests/evaluate.py` & `petabtests-0.0.1/petabtests/evaluate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from typing import List, Union
 import numpy as np
 import pandas as pd
 from petab.C import *
 from .C import *  # noqa: F403
 
+__all__ = ['evaluate_llh', 'evaluate_chi2', 'evaluate_simulations',
+           'absolute_simulations_distance_for_tables',
+           'absolute_simulations_distance_for_array',
+           'absolute_simulations_distance_for_table']
+
 
 def evaluate_chi2(chi2: float, gt_chi2: float, tol: float = 1e-3):
     """Evaluate whether chi square values match."""
     if chi2 is None:
         return False
     return abs(chi2 - gt_chi2) < tol
 
@@ -59,20 +64,20 @@
     return distance
 
 
 def absolute_simulations_distance_for_table(
         simulations: pd.DataFrame,
         gt_simulations: pd.DataFrame):
     """Compute absolute normalized distance between simulations."""
-    # gropuing columns
+    # grouping columns
     grouping_cols = [OBSERVABLE_ID, SIMULATION_CONDITION_ID, TIME]
     if PREEQUILIBRATION_CONDITION_ID in simulations:
         grouping_cols.append(PREEQUILIBRATION_CONDITION_ID)
     relevant_cols = grouping_cols.copy()
-    # append simulation columng last for correct sorting
+    # append simulation column last for correct sorting
     relevant_cols.append(SIMULATION)
 
     # restrict tables
     simulations = simulations[relevant_cols]
     gt_simulations = gt_simulations[relevant_cols]
 
     # sort both in the same way to enable direct comparison
```

### Comparing `petabtests-0.0.0a6/petabtests.egg-info/PKG-INFO` & `petabtests-0.0.1/petabtests.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 Metadata-Version: 2.1
 Name: petabtests
-Version: 0.0.0a6
+Version: 0.0.1
 Summary: PEtab testsuite library
 Home-page: https://github.com/PEtab-dev/petab_test_suite
 Author: PEtab-dev
 Author-email: yannik.schaelte@gmail.com
 Maintainer: PEtab-dev
 Maintainer-email: yannik.schaelte@gmail.com
-License: UNKNOWN
-Description: # PEtab test suite
-        
-        The PEtab test suite is a collection of test models for the
-        [PEtab](https://github.com/petab-dev/petab) parameter estimation data format.
-        It is intended to be used to verify and quantify PEtab-support by developers
-        of tools for model simulation and parameter estimation.
-        
-        ## Download and install the test suite
-        
-        The PEtab test suite can be downloaded from GitHub via
-        
-            git clone https://github.com/petab-dev/petab_test_suite
-        
-        The test suite comes with all necessary files pregenerated. 
-        In the [petabtests](petabtests) subdirectory, it contains a python module for
-        generating the tests and evaluating results. This can be installed via
-        
-            cd petab_test_suite
-            pip3 install -e .
-        
-        ## Use the test suite
-        
-        The [cases](cases) subdirectory contains a collection of enumerated tests.
-        Each test contains a descriptive `wxyz.md` file, and a script file `wxyz.py`
-        file that can be used to generate all problem and solution files for the test.
-        The necessary files are in the same case specific folder, starting with an
-        underscore. 
-        In each case folder, there is a file `_wxyz.yaml` containing the parameter
-        estimation problem description, and a file `_wxyz_solution.yaml` containing
-        information on the expected results: chi2 value, log-likelihood, simulation
-        table reference, and tolerances.
-        
-        After download, all necessary files are already pregenerated.
-        
-        Further, installation of the petabtests module installs a routine to recreate
-        the problem and solution files for all test problems. It can be invoked via
-        
-            cd petab_test_suite
-            petabtests_create
-        
-        ## Evaluate results
-        
-        To evaluate how a tool performs on a given test problem, three metrics are
-        employed: Simulations, chi2 value and log-likelihood. A tool can be said to
-        cover a test problem if any of those values matches the ground truth values
-        up to some tolerance.
-        
-        The python module provides convenience functions for evaluation in
-        [petabtests/evaluate.py](petabtests/evaluate.py).
-        
-        -> [Overview of passed test cases for different tools supporting PEtab](https://github.com/PEtab-dev/PEtab#petab-features-supported-in-different-tools)
-        
 Keywords: PEtab testsuite
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PEtab test suite
+
+The PEtab test suite is a collection of test models for the
+[PEtab](https://github.com/petab-dev/petab) parameter estimation data format.
+It is intended to be used to verify and quantify PEtab-support by developers
+of tools for model simulation and parameter estimation.
+
+## Download and install the test suite
+
+The PEtab test suite can be downloaded from GitHub via
+
+    git clone https://github.com/petab-dev/petab_test_suite
+
+The test suite comes with all necessary files pregenerated. 
+In the [petabtests](petabtests) subdirectory, it contains a python module for
+generating the tests and evaluating results. This can be installed via
+
+    cd petab_test_suite
+    pip3 install -e .
+
+## Use the test suite
+
+The [cases](cases) subdirectory contains a collection of enumerated tests.
+Each test contains a descriptive `wxyz.md` file, and a script file `wxyz.py`
+file that can be used to generate all problem and solution files for the test.
+The necessary files are in the same case specific folder, starting with an
+underscore. 
+In each case folder, there is a file `_wxyz.yaml` containing the parameter
+estimation problem description, and a file `_wxyz_solution.yaml` containing
+information on the expected results: chi2 value, log-likelihood, simulation
+table reference, and tolerances.
+
+After download, all necessary files are already pregenerated.
+
+Further, installation of the petabtests module installs a routine to recreate
+the problem and solution files for all test problems. It can be invoked via
+
+    cd petab_test_suite
+    petabtests_create
+
+## Evaluate results
+
+To evaluate how a tool performs on a given test problem, three metrics are
+employed: Simulations, chi2 value and log-likelihood. A tool can be said to
+cover a test problem if any of those values matches the ground truth values
+up to some tolerance.
+
+The python module provides convenience functions for evaluation in
+[petabtests/evaluate.py](petabtests/evaluate.py).
+
+-> [Overview of passed test cases for different tools supporting PEtab](https://github.com/PEtab-dev/PEtab#petab-features-supported-in-different-tools)
```

### Comparing `petabtests-0.0.0a6/setup.py` & `petabtests-0.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """PEtab test suite python package"""
 
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 
 def read(fname):
     with open(fname, encoding='utf-8') as f:
@@ -30,25 +30,28 @@
     maintainer_email='yannik.schaelte@gmail.com',
     # author_email='',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     keywords='PEtab testsuite',
-    packages=find_packages(),
-    install_requires=['numpy',
-                      'pandas',
-                      'petab>=0.1.4',
-                      'pysb'],
-    python_requires='>=3.6',
+    packages=find_namespace_packages(),
+    install_requires=[
+        'numpy',
+        'pandas',
+        'petab>=0.1.4',
+        'pysb',
+        'simplesbml',
+    ],
+    python_requires='>=3.9',
     entry_points={
         'console_scripts': [
             'petabtests_create = petabtests.core:create',
             'petabtests_clear = petabtests.core:clear',
         ]
     },
     include_package_data=True,
```

### Comparing `petabtests-0.0.0a6/test/test_evaluate.py` & `petabtests-0.0.1/test/test_evaluate.py`

 * *Files identical despite different names*

