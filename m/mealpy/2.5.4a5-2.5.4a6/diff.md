# Comparing `tmp/mealpy-2.5.4a5.tar.gz` & `tmp/mealpy-2.5.4a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mealpy-2.5.4a5.tar", last modified: Fri Jun 16 15:41:02 2023, max compression
+gzip compressed data, was "mealpy-2.5.4a6.tar", last modified: Tue Jun 20 16:10:44 2023, max compression
```

## Comparing `mealpy-2.5.4a5.tar` & `mealpy-2.5.4a6.tar`

### file list

```diff
@@ -1,176 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.273996 mealpy-2.5.4a5/
--rw-r--r--   0 runner    (1001) docker     (123)    58180 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    90711 2023-06-16 15:41:02.273996 mealpy-2.5.4a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    88172 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.241996 mealpy-2.5.4a5/mealpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.245996 mealpy-2.5.4a5/mealpy/bio_based/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/BBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/BBOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/BMO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/EOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/IWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/SBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/SMA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/SOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/SOS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/TPO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/TSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/VCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/WHO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/bio_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.249996 mealpy-2.5.4a5/mealpy/evolutionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/CRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/DE.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/EP.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/ES.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/FPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    38895 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/GA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/MA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/evolutionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.253996 mealpy-2.5.4a5/mealpy/human_based/
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/BRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/BSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/CA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/CHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/FBIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/GSKA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/HBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/HCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/ICA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/LCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/QSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/SARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/SPBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/SSDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/TLO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/TOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/WarSO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/human_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.253996 mealpy-2.5.4a5/mealpy/math_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/AOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/CEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/CGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/CircleSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/GBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/HC.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/PSS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/RUN.py
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/SCA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/SHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/math_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/multitask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.253996 mealpy-2.5.4a5/mealpy/music_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/music_based/HS.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/music_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33913 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.257996 mealpy-2.5.4a5/mealpy/physics_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/ASO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/ArchOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/CDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/EFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/EO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/EVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/FLA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/HGSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/MVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/NRO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/RIME.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/SA.py
--rw-r--r--   0 runner    (1001) docker     (123)    20830 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/TWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/WDO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/physics_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.269997 mealpy-2.5.4a5/mealpy/swarm_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/ABC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/ACOR.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/AGTO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/ALO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/AO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/ARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/AVOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/BA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/BES.py
--rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/BFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/BSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/BeesA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/COA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/CSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/CSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/CoatiOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/DMOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/DO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/EHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/ESOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/FA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/FFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/FFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/FOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/FOX.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/GJO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/GOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/GTO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/GWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/HBA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/HGS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/HHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/JA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/MFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/MGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/MPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/MRFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/MSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/NGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/NMRA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/OOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/PFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/POA.py
--rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/PSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SCSO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SHO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SLO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SRSR.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SSpiderA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SSpiderO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/STO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/SeaHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/ServalOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/TDO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/TSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/WOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/WaOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/ZOA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/swarm_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.269997 mealpy-2.5.4a5/mealpy/system_based/
--rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/system_based/AEO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/system_based/GCO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/system_based/WCA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/system_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.269997 mealpy-2.5.4a5/mealpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.269997 mealpy-2.5.4a5/mealpy/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/mealpy/utils/visualize/linechart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.245996 mealpy-2.5.4a5/mealpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    90711 2023-06-16 15:41:02.000000 mealpy-2.5.4a5/mealpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-16 15:41:02.000000 mealpy-2.5.4a5/mealpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:41:02.000000 mealpy-2.5.4a5/mealpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 15:41:02.000000 mealpy-2.5.4a5/mealpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 15:41:02.000000 mealpy-2.5.4a5/mealpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:41:02.273996 mealpy-2.5.4a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:41:02.273996 mealpy-2.5.4a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-16 15:38:14.000000 mealpy-2.5.4a5/tests/test_tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.345373 mealpy-2.5.4a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    91128 2023-06-20 16:10:44.345373 mealpy-2.5.4a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    88589 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.321371 mealpy-2.5.4a6/mealpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.325372 mealpy-2.5.4a6/mealpy/bio_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/BBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/BBOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/BMO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/EOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/IWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/SBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/SOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/SOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/TPO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/TSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/VCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/WHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/bio_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.325372 mealpy-2.5.4a6/mealpy/evolutionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/CRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/DE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/EP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/ES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/FPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38895 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/MA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/SHADE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/evolutionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.329372 mealpy-2.5.4a6/mealpy/human_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/BRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/BSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/CA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/CHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/FBIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/GSKA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/HBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/HCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/ICA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/LCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/QSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/SARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/SPBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/SSDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/TLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/TOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/WarSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/human_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.333372 mealpy-2.5.4a6/mealpy/math_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/AOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/CEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/CGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/CircleSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/GBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/HC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/PSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/RUN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/SCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/SHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/math_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/multitask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.333372 mealpy-2.5.4a6/mealpy/music_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/music_based/HS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/music_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33913 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.333372 mealpy-2.5.4a6/mealpy/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/ASO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/ArchOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/CDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/EFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/EO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/EVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/FLA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/HGSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/MVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/NRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/RIME.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20830 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/TWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/WDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.341373 mealpy-2.5.4a6/mealpy/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/ACOR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/AGTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/ALO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/AO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/ARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/AVOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/BA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/BES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/BFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/BSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/BeesA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/COA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/CSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/CSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/CoatiOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/DMOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/DO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/EHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/ESOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/FA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/FFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/FFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/FOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/FOX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/GJO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/GOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/GTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/GWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/HBA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/HGS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/HHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/JA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/MFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/MGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/MPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/MRFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/MSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/NGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/NMRA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/OOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/PFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/POA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SCSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SRSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SSpiderA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SSpiderO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/STO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/SeaHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/ServalOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/TDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/TSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/WOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/WaOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/ZOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/swarm_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.345373 mealpy-2.5.4a6/mealpy/system_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/system_based/AEO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/system_based/GCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/system_based/WCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/system_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.345373 mealpy-2.5.4a6/mealpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.345373 mealpy-2.5.4a6/mealpy/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/mealpy/utils/visualize/linechart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.325372 mealpy-2.5.4a6/mealpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    91128 2023-06-20 16:10:44.000000 mealpy-2.5.4a6/mealpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-20 16:10:44.000000 mealpy-2.5.4a6/mealpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:10:44.000000 mealpy-2.5.4a6/mealpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 16:10:44.000000 mealpy-2.5.4a6/mealpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:10:44.000000 mealpy-2.5.4a6/mealpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:10:44.345373 mealpy-2.5.4a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:10:44.345373 mealpy-2.5.4a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-20 16:08:33.000000 mealpy-2.5.4a6/tests/test_tuner.py
```

### Comparing `mealpy-2.5.4a5/ChangeLog.md` & `mealpy-2.5.4a6/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 + Remove ILA optimizer 
 + Rename "amend_position()" definition in some algorithms to "bounded_position()".
 + Add a "amend_position()" function in Optimizer class. This function will call two functions.
   + bounded_position() from optimizer. This means for optimizer level (get in valid range of position)
   + amend_position() from problem. This means for problem level (transform to the correct solution)
 + Fix bugs coefficients in GWO-based optimizers.
 + Fig bug self.epoch in SCSO optimizer.
++ Fix bug self.dyn_pop_size when pop_size is small value
++ Move SHADE-based optimizers from DE to SHADE module in evolutionary_based group
++ Add Improved Grey Wolf Optimization (IGWO) in GWO algorithm
++ Add Tabu Search (TS) to math-based group
++ Add get_all_optimizers() and get_optimizer_by_name() in Mealpy
+
 
 
 # Version 2.5.3
 
 ### Update 
 + Fix bug in roulette-wheel-selection in Optimizer
 + Update multitask with input modes and terminations
```

### Comparing `mealpy-2.5.4a5/LICENSE` & `mealpy-2.5.4a6/LICENSE`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/PKG-INFO` & `mealpy-2.5.4a6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,7 @@
-Metadata-Version: 2.1
-Name: mealpy
-Version: 2.5.4a5
-Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
-Home-page: https://github.com/thieu1995/mealpy
-Author: Thieu
-Author-email: nguyenthieu2102@gmail.com
-License: GPLv3
-Project-URL: Documentation, https://mealpy.readthedocs.io/
-Project-URL: Source Code, https://github.com/thieu1995/mealpy
-Project-URL: Bug Tracker, https://github.com/thieu1995/mealpy/issues
-Project-URL: Change Log, https://github.com/thieu1995/mealpy/blob/master/ChangeLog.md
-Project-URL: Forum, https://t.me/+fRVCJGuGJg1mNDg1
-Keywords: optimization,metaheuristics,MHA,mathematical optimization,nature-inspired algorithms,evolutionary computation,soft computing,population-based algorithms,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Black-box optimization,Robust optimization,Hybrid algorithms,Benchmark functions,Metaheuristic design,Performance analysis,Exploration versus exploitation,Self-adaptation,Constrained optimization,Intelligent optimization,Adaptive search,Simulations,Algorithm selection
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Benchmark
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 
 <p align="center">
 <img style="height:400px;" 
 src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy5-nobg.png" 
 alt="MEALPY"/>
 </p>
 
@@ -70,15 +27,15 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MEALPY is the largest python library for most of the cutting-edge nature-inspired meta-heuristic algorithms (population-based). Population meta-heuristic algorithms (PMA) are the most popular algorithms in the field of 
 approximate optimization.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total algorithms**: 174 (102 original, 45 official variants, 27 developed variants)
+* **Total algorithms**: 175 (102 original, 46 official variants, 27 developed variants)
 * **Documentation:** https://mealpy.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, pandas, matplotlib
 
 
 # Goals
 
@@ -99,15 +56,15 @@
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
 $ pip install mealpy==2.5.3
 ```
 
 ### Install the alpha/beta version
 ```sh 
-$ pip install mealpy==2.5.4a5
+$ pip install mealpy==2.5.4a6
 ```
 
 ### Install the pre-release version
 You can install pre-release directly from the source code:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
@@ -119,14 +76,17 @@
 
 After installation, you can import Mealpy as any other Python module:
 
 ```sh
 $ python
 >>> import mealpy
 >>> mealpy.__version__
+
+>>> print(mealpy.get_all_optimizers())
+>>> model = mealpy.get_optimizer_by_name("OriginalWOA")(epoch=100, pop_size=50)
 ```
 
 Let's go through a basic and advanced example.
 
 
 ## Examples
 
@@ -403,44 +363,46 @@
 
 * Official source code repo: https://github.com/thieu1995/mealpy
 * Official document: https://mealpy.readthedocs.io/
 * Download releases: https://pypi.org/project/mealpy/
 * Issue tracker: https://github.com/thieu1995/mealpy/issues
 * Notable changes log: https://github.com/thieu1995/mealpy/blob/master/ChangeLog.md
 * Examples with different meapy version: https://github.com/thieu1995/mealpy/blob/master/EXAMPLES.md
+* Official chat/support group: https://t.me/+fRVCJGuGJg1mNDg1
 
 * This project also related to our another projects which are "meta-heuristics" and "neural-network", check it here
     * https://github.com/thieu1995/opfunu
     * https://github.com/thieu1995/metaheuristics
     * https://github.com/aiir-team
-
-**Want to have an instant assistant? Join our telegram community at [link](https://t.me/+fRVCJGuGJg1mNDg1)**
-We share lots of information, questions, and answers there. You will get more support and knowledge there.
+    * https://github.com/mafese
+    * https://github.com/permetrics
 
 ### Cite Us
 
 If you are using mealpy in your project, we would appreciate citations:
 
 ```bibtex 
 @article{van2023mealpy,
   title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
   author={Van Thieu, Nguyen and Mirjalili, Seyedali},
   journal={Journal of Systems Architecture},
   year={2023},
-  publisher={Elsevier}
+  publisher={Elsevier},
+  doi={10.1016/j.sysarc.2023.102871}
 }
 
 @article{van2023groundwater,
   title={Groundwater level modeling using Augmented Artificial Ecosystem Optimization},
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
   pages={129034},
   year={2023},
-  publisher={Elsevier}
+  publisher={Elsevier},
+  doi={10.1016/j.jhydrol.2022.129034}
 }
 ```
 
 
 
 # List of papers used MEALPY
 
@@ -567,14 +529,15 @@
 | Swarm        | -                                               | -          | ModifiedBA       | -        | 5         | medium         |
 | Swarm        | Fruit-fly Optimization Algorithm                | FOA        | OriginalFOA      | 2012     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseFOA          | -        | 2         | easy           |
 | Swarm        | -                                               | -          | WhaleFOA         | 2020     | 2         | medium         |
 | Swarm        | Social Spider Optimization                      | SSpiderO   | OriginalSSpiderO | 2018     | 4         | hard*          |
 | Swarm        | Grey Wolf Optimizer                             | GWO        | OriginalGWO      | 2014     | 2         | easy           |
 | Swarm        | -                                               | -          | RW_GWO           | 2019     | 2         | easy           |
+| Swarm        | -                                               | -          | IGWO             | 2017     | 4         | easy           |
 | Swarm        | Social Spider Algorithm                         | SSpiderA   | OriginalSSpiderA | 2015     | 5         | medium         |
 | Swarm        | Ant Lion Optimizer                              | ALO        | OriginalALO      | 2015     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseALO          | -        | 2         | easy           |
 | Swarm        | Moth Flame Optimization                         | MFO        | OriginalMFO      | 2015     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseMFO          | -        | 2         | easy           |
 | Swarm        | Elephant Herding Optimization                   | EHO        | OriginalEHO      | 2015     | 5         | easy           |
 | Swarm        | Jaya Algorithm                                  | JA         | OriginalJA       | 2016     | 2         | easy           |
@@ -896,14 +859,15 @@
   * **EliteSingleGA**: Elite version of Single-point mutation GA
   * **EliteMultiGA**: Elite version of Multiple-point mutation GA
 
 * **GWO - Grey Wolf Optimizer** 
   * **OriginalGWO**: Mirjalili, S., Mirjalili, S. M., & Lewis, A. (2014). Grey wolf optimizer. Advances in engineering software, 69, 46-61.
   * **RW_GWO**: Gupta, S., & Deep, K. (2019). A novel random walk grey wolf optimizer. Swarm and evolutionary computation, 44, 101-112.
   * **GWO_WOA**: Obadina, O. O., Thaha, M. A., Althoefer, K., & Shaheed, M. H. (2022). Dynamic characterization of a master–slave robotic manipulator using a hybrid grey wolf–whale optimization algorithm. Journal of Vibration and Control, 28(15-16), 1992-2003.
+  * **IGWO**: Kaveh, A. & Zakian, P.. (2018). Improved GWO algorithm for optimal design of truss structures. Engineering with Computers. 34. 10.1007/s00366-017-0567-1.
 
 * **GOA - Grasshopper Optimisation Algorithm** 
   * **OriginalGOA**: Saremi, S., Mirjalili, S., & Lewis, A. (2017). Grasshopper optimisation algorithm: theory and application. Advances in Engineering Software, 105, 30-47.
 
 * **GCO - Germinal Center Optimization** 
   * **OriginalGCO**: Villaseñor, C., Arana-Daniel, N., Alanis, A. Y., López-Franco, C., & Hernandez-Vargas, E. A. (2018). Germinal center optimization algorithm. International Journal of Computational Intelligence Systems, 12(1), 13-27.
   * **BaseGCO**: The developed version
```

### Comparing `mealpy-2.5.4a5/README.md` & `mealpy-2.5.4a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,50 @@
+Metadata-Version: 2.1
+Name: mealpy
+Version: 2.5.4a6
+Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
+Home-page: https://github.com/thieu1995/mealpy
+Author: Thieu
+Author-email: nguyenthieu2102@gmail.com
+License: GPLv3
+Project-URL: Documentation, https://mealpy.readthedocs.io/
+Project-URL: Source Code, https://github.com/thieu1995/mealpy
+Project-URL: Bug Tracker, https://github.com/thieu1995/mealpy/issues
+Project-URL: Change Log, https://github.com/thieu1995/mealpy/blob/master/ChangeLog.md
+Project-URL: Forum, https://t.me/+fRVCJGuGJg1mNDg1
+Keywords: optimization,metaheuristics,MHA,mathematical optimization,nature-inspired algorithms,evolutionary computation,soft computing,population-based algorithms,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Black-box optimization,Robust optimization,Hybrid algorithms,Benchmark functions,Metaheuristic design,Performance analysis,Exploration versus exploitation,Self-adaptation,Constrained optimization,Intelligent optimization,Adaptive search,Simulations,Algorithm selection
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Benchmark
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 
 <p align="center">
 <img style="height:400px;" 
 src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy5-nobg.png" 
 alt="MEALPY"/>
 </p>
 
@@ -27,15 +70,15 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MEALPY is the largest python library for most of the cutting-edge nature-inspired meta-heuristic algorithms (population-based). Population meta-heuristic algorithms (PMA) are the most popular algorithms in the field of 
 approximate optimization.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total algorithms**: 174 (102 original, 45 official variants, 27 developed variants)
+* **Total algorithms**: 175 (102 original, 46 official variants, 27 developed variants)
 * **Documentation:** https://mealpy.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, pandas, matplotlib
 
 
 # Goals
 
@@ -56,15 +99,15 @@
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
 $ pip install mealpy==2.5.3
 ```
 
 ### Install the alpha/beta version
 ```sh 
-$ pip install mealpy==2.5.4a5
+$ pip install mealpy==2.5.4a6
 ```
 
 ### Install the pre-release version
 You can install pre-release directly from the source code:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
@@ -76,14 +119,17 @@
 
 After installation, you can import Mealpy as any other Python module:
 
 ```sh
 $ python
 >>> import mealpy
 >>> mealpy.__version__
+
+>>> print(mealpy.get_all_optimizers())
+>>> model = mealpy.get_optimizer_by_name("OriginalWOA")(epoch=100, pop_size=50)
 ```
 
 Let's go through a basic and advanced example.
 
 
 ## Examples
 
@@ -360,44 +406,46 @@
 
 * Official source code repo: https://github.com/thieu1995/mealpy
 * Official document: https://mealpy.readthedocs.io/
 * Download releases: https://pypi.org/project/mealpy/
 * Issue tracker: https://github.com/thieu1995/mealpy/issues
 * Notable changes log: https://github.com/thieu1995/mealpy/blob/master/ChangeLog.md
 * Examples with different meapy version: https://github.com/thieu1995/mealpy/blob/master/EXAMPLES.md
+* Official chat/support group: https://t.me/+fRVCJGuGJg1mNDg1
 
 * This project also related to our another projects which are "meta-heuristics" and "neural-network", check it here
     * https://github.com/thieu1995/opfunu
     * https://github.com/thieu1995/metaheuristics
     * https://github.com/aiir-team
-
-**Want to have an instant assistant? Join our telegram community at [link](https://t.me/+fRVCJGuGJg1mNDg1)**
-We share lots of information, questions, and answers there. You will get more support and knowledge there.
+    * https://github.com/mafese
+    * https://github.com/permetrics
 
 ### Cite Us
 
 If you are using mealpy in your project, we would appreciate citations:
 
 ```bibtex 
 @article{van2023mealpy,
   title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
   author={Van Thieu, Nguyen and Mirjalili, Seyedali},
   journal={Journal of Systems Architecture},
   year={2023},
-  publisher={Elsevier}
+  publisher={Elsevier},
+  doi={10.1016/j.sysarc.2023.102871}
 }
 
 @article{van2023groundwater,
   title={Groundwater level modeling using Augmented Artificial Ecosystem Optimization},
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
   pages={129034},
   year={2023},
-  publisher={Elsevier}
+  publisher={Elsevier},
+  doi={10.1016/j.jhydrol.2022.129034}
 }
 ```
 
 
 
 # List of papers used MEALPY
 
@@ -524,14 +572,15 @@
 | Swarm        | -                                               | -          | ModifiedBA       | -        | 5         | medium         |
 | Swarm        | Fruit-fly Optimization Algorithm                | FOA        | OriginalFOA      | 2012     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseFOA          | -        | 2         | easy           |
 | Swarm        | -                                               | -          | WhaleFOA         | 2020     | 2         | medium         |
 | Swarm        | Social Spider Optimization                      | SSpiderO   | OriginalSSpiderO | 2018     | 4         | hard*          |
 | Swarm        | Grey Wolf Optimizer                             | GWO        | OriginalGWO      | 2014     | 2         | easy           |
 | Swarm        | -                                               | -          | RW_GWO           | 2019     | 2         | easy           |
+| Swarm        | -                                               | -          | IGWO             | 2017     | 4         | easy           |
 | Swarm        | Social Spider Algorithm                         | SSpiderA   | OriginalSSpiderA | 2015     | 5         | medium         |
 | Swarm        | Ant Lion Optimizer                              | ALO        | OriginalALO      | 2015     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseALO          | -        | 2         | easy           |
 | Swarm        | Moth Flame Optimization                         | MFO        | OriginalMFO      | 2015     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseMFO          | -        | 2         | easy           |
 | Swarm        | Elephant Herding Optimization                   | EHO        | OriginalEHO      | 2015     | 5         | easy           |
 | Swarm        | Jaya Algorithm                                  | JA         | OriginalJA       | 2016     | 2         | easy           |
@@ -853,14 +902,15 @@
   * **EliteSingleGA**: Elite version of Single-point mutation GA
   * **EliteMultiGA**: Elite version of Multiple-point mutation GA
 
 * **GWO - Grey Wolf Optimizer** 
   * **OriginalGWO**: Mirjalili, S., Mirjalili, S. M., & Lewis, A. (2014). Grey wolf optimizer. Advances in engineering software, 69, 46-61.
   * **RW_GWO**: Gupta, S., & Deep, K. (2019). A novel random walk grey wolf optimizer. Swarm and evolutionary computation, 44, 101-112.
   * **GWO_WOA**: Obadina, O. O., Thaha, M. A., Althoefer, K., & Shaheed, M. H. (2022). Dynamic characterization of a master–slave robotic manipulator using a hybrid grey wolf–whale optimization algorithm. Journal of Vibration and Control, 28(15-16), 1992-2003.
+  * **IGWO**: Kaveh, A. & Zakian, P.. (2018). Improved GWO algorithm for optimal design of truss structures. Engineering with Computers. 34. 10.1007/s00366-017-0567-1.
 
 * **GOA - Grasshopper Optimisation Algorithm** 
   * **OriginalGOA**: Saremi, S., Mirjalili, S., & Lewis, A. (2017). Grasshopper optimisation algorithm: theory and application. Advances in Engineering Software, 105, 30-47.
 
 * **GCO - Germinal Center Optimization** 
   * **OriginalGCO**: Villaseñor, C., Arana-Daniel, N., Alanis, A. Y., López-Franco, C., & Hernandez-Vargas, E. A. (2018). Germinal center optimization algorithm. International Journal of Computational Intelligence Systems, 12(1), 13-27.
   * **BaseGCO**: The developed version
```

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/BBO.py` & `mealpy-2.5.4a6/mealpy/bio_based/BBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/BBOA.py` & `mealpy-2.5.4a6/mealpy/bio_based/BBOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/BMO.py` & `mealpy-2.5.4a6/mealpy/bio_based/BMO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/EOA.py` & `mealpy-2.5.4a6/mealpy/bio_based/EOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/IWO.py` & `mealpy-2.5.4a6/mealpy/bio_based/IWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/SBO.py` & `mealpy-2.5.4a6/mealpy/bio_based/SBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/SMA.py` & `mealpy-2.5.4a6/mealpy/bio_based/SMA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/SOA.py` & `mealpy-2.5.4a6/mealpy/bio_based/SOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/SOS.py` & `mealpy-2.5.4a6/mealpy/bio_based/SOS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/TPO.py` & `mealpy-2.5.4a6/mealpy/bio_based/TPO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/TSA.py` & `mealpy-2.5.4a6/mealpy/bio_based/TSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/VCS.py` & `mealpy-2.5.4a6/mealpy/bio_based/VCS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/bio_based/WHO.py` & `mealpy-2.5.4a6/mealpy/bio_based/WHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/evolutionary_based/CRO.py` & `mealpy-2.5.4a6/mealpy/evolutionary_based/CRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/evolutionary_based/DE.py` & `mealpy-2.5.4a6/mealpy/evolutionary_based/GA.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,903 +1,794 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 09:48, 16/03/2020 ----------%
+# Created by "Thieu" at 09:33, 16/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
-from scipy.stats import cauchy
-from copy import deepcopy
 
 
-class BaseDE(Optimizer):
+class BaseGA(Optimizer):
     """
-    The original version of: Differential Evolution (DE)
+    The original version of: Genetic Algorithm (GA)
 
     Links:
-        1. https://doi.org/10.1016/j.swevo.2018.10.006
+        1. https://blog.sicara.com/getting-started-genetic-algorithms-python-tutorial-81ffa1dd72f9
+        2. https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_quick_guide.htm
+        3. https://www.analyticsvidhya.com/blog/2017/07/introduction-to-genetic-algorithm/
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + wf (float): [0.5, 0.95], weighting factor, default = 0.8
-        + cr (float): [0.5, 0.95], crossover rate, default = 0.9
-        + strategy (int): [0, 5], there are lots of variant version of DE algorithm,
-            + 0: DE/current-to-rand/1/bin
-            + 1: DE/best/1/bin
-            + 2: DE/best/2/bin
-            + 3: DE/rand/2/bin
-            + 4: DE/current-to-best/1/bin
-            + 5: DE/current-to-rand/1/bin
+        + pc (float): [0.7, 0.95], cross-over probability, default = 0.95
+        + pm (float): [0.01, 0.2], mutation probability, default = 0.025
+        + selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+        + k_way (float): Optional, set it when use "tournament" selection, default = 0.2
+        + crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+        + mutation_multipoints (bool): Optional, True or False, effect on mutation process, default = True
+        + mutation (str): Optional, can be ["flip", "swap"] for multipoints and can be ["flip", "swap", "scramble", "inversion"] for one-point
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.evolutionary_based.DE import BaseDE
+    >>> from mealpy.evolutionary_based.GA import BaseGA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> wf = 0.7
-    >>> cr = 0.9
-    >>> strategy = 0
-    >>> model = BaseDE(epoch, pop_size, wf, cr, strategy)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
+    >>> pc = 0.9
+    >>> pm = 0.05
+    >>> model1 = BaseGA(epoch, pop_size, pc, pm)
+    >>> best_position, best_fitness = model1.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+    >>>
+    >>> model2 = BaseGA(epoch, pop_size, pc, pm, selection="tournament", k_way=0.4, crossover="multi_points")
+    >>>
+    >>> model3 = BaseGA(epoch, pop_size, pc, pm, crossover="one_point", mutation="scramble")
+    >>>
+    >>> model4 = BaseGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation_multipoints=True, mutation="swap")
+    >>>
+    >>> model5 = BaseGA(epoch, pop_size, pc, pm, selection="roulette", crossover="multi_points")
+    >>>
+    >>> model6 = BaseGA(epoch, pop_size, pc, pm, selection="random", mutation="inversion")
+    >>>
+    >>> model7 = BaseGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation="flip")
 
     References
     ~~~~~~~~~~
-    [1] Mohamed, A.W., Hadi, A.A. and Jambi, K.M., 2019. Novel mutation strategy for enhancing SHADE and
-    LSHADE algorithms for global numerical optimization. Swarm and Evolutionary Computation, 50, p.100455.
+    [1] Whitley, D., 1994. A genetic algorithm tutorial. Statistics and computing, 4(2), pp.65-85.
     """
 
-    def __init__(self, epoch=10000, pop_size=100, wf=1.0, cr=0.9, strategy=0, **kwargs):
+    def __init__(self, epoch=10000, pop_size=100, pc=0.95, pm=0.025, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
-            wf (float): weighting factor, default = 1.5
-            cr (float): crossover rate, default = 0.9
-            strategy (int): Different variants of DE, default = 0
+            pc (float): cross-over probability, default = 0.95
+            pm (float): mutation probability, default = 0.025
+            selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+            k_way (float): Optional, set it when use "tournament" selection, default = 0.2
+            crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+            mutation_multipoints (bool): Optional, True or False, effect on mutation process, default = False
+            mutation (str): Optional, can be ["flip", "swap"] for multipoints and can be ["flip", "swap", "scramble", "inversion"] for one-point, default="flip"
         """
         super().__init__(**kwargs)
+
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.wf = self.validator.check_float("wf", wf, (0, 3.0))
-        self.cr = self.validator.check_float("cr", cr, (0, 1.0))
-        self.strategy = self.validator.check_int("strategy", strategy, [0, 5])
-        self.set_parameters(["epoch", "pop_size", "wf", "cr", "strategy"])
+        self.pc = self.validator.check_float("pc", pc, (0, 1.0))
+        self.pm = self.validator.check_float("pm", pm, (0, 1.0))
+        self.set_parameters(["epoch", "pop_size", "pc", "pm"])
         self.sort_flag = False
+        self.selection = "tournament"
+        self.k_way = 0.2
+        self.crossover = "uniform"
+        self.mutation = "flip"
+        self.mutation_multipoints = True
+
+        if "selection" in kwargs:
+            self.selection = self.validator.check_str("selection", kwargs["selection"], ["tournament", "random", "roulette"])
+        if "k_way" in kwargs:
+            self.k_way = self.validator.check_float("k_way", kwargs["k_way"], (0, 1.0))
+        if "crossover" in kwargs:
+            self.crossover = self.validator.check_str("crossover", kwargs["crossover"], ["one_point", "multi_points", "uniform", "arithmetic"])
+        if "mutation_multipoints" in kwargs:
+            self.mutation_multipoints = self.validator.check_bool("mutation_multipoints", kwargs["mutation_multipoints"])
+        if self.mutation_multipoints:
+            if "mutation" in kwargs:
+                self.mutation = self.validator.check_str("mutation", kwargs["mutation"], ["flip", "swap"])
+        else:
+            if "mutation" in kwargs:
+                self.mutation = self.validator.check_str("mutation", kwargs["mutation"], ["flip", "swap", "scramble", "inversion"])
 
-    def mutation__(self, current_pos, new_pos):
-        condition = np.random.random(self.problem.n_dims) < self.cr
-        pos_new = np.where(condition, new_pos, current_pos)
-        return self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+    def selection_process__(self, list_fitness):
+        """
+        Notes
+        ~~~~~
+        + https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_parent_selection.htm
+        + Default selection strategy is Tournament with k% = 0.2.
+        + Other strategy like "roulette" and "random" can be selected via Optional parameter "selection"
 
-    def evolve(self, epoch):
+        Args:
+            list_fitness (np.array): list of fitness values.
+
+        Returns:
+            list: The position of dad and mom
         """
-        The main operations (equations) of algorithm. Inherit from Optimizer class
+        if self.selection == "roulette":
+            id_c1 = self.get_index_roulette_wheel_selection(list_fitness)
+            id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
+            while id_c2 == id_c1:
+                id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
+        elif self.selection == "random":
+            id_c1, id_c2 = np.random.choice(range(self.pop_size), 2, replace=False)
+        else:   ## tournament
+            id_c1, id_c2 = self.get_index_kway_tournament_selection(self.pop, k_way=self.k_way, output=2)
+        return self.pop[id_c1][self.ID_POS], self.pop[id_c2][self.ID_POS]
+
+    def selection_process_00__(self, pop_selected):
+        """
+        Notes
+        ~~~~~
+        + https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_parent_selection.htm
+        + Default selection strategy is Tournament with k% = 0.2.
+        + Other strategy like "roulette" and "random" can be selected via Optional parameter "selection"
 
         Args:
-            epoch (int): The current iteration
+            pop_selected (np.array): a population that will be selected
+
+        Returns:
+            list: The position of dad and mom
         """
-        pop = []
-        if self.strategy == 0:
-            # Choose 3 random element and different to i
-            for idx in range(0, self.pop_size):
-                idx_list = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 3, replace=False)
-                pos_new = self.pop[idx_list[0]][self.ID_POS] + self.wf * \
-                          (self.pop[idx_list[1]][self.ID_POS] - self.pop[idx_list[2]][self.ID_POS])
-                pos_new = self.mutation__(self.pop[idx][self.ID_POS], pos_new)
-                pop.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    target = self.get_target_wrapper(pos_new)
-                    self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        elif self.strategy == 1:
-            for idx in range(0, self.pop_size):
-                idx_list = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
-                pos_new = self.g_best[self.ID_POS] + self.wf * (self.pop[idx_list[0]][self.ID_POS] - self.pop[idx_list[1]][self.ID_POS])
-                pos_new = self.mutation__(self.pop[idx][self.ID_POS], pos_new)
-                pop.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    target = self.get_target_wrapper(pos_new)
-                    self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        elif self.strategy == 2:
-            for idx in range(0, self.pop_size):
-                idx_list = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 4, replace=False)
-                pos_new = self.g_best[self.ID_POS] + self.wf * (self.pop[idx_list[0]][self.ID_POS] - self.pop[idx_list[1]][self.ID_POS]) + \
-                          self.wf * (self.pop[idx_list[2]][self.ID_POS] - self.pop[idx_list[3]][self.ID_POS])
-                pos_new = self.mutation__(self.pop[idx][self.ID_POS], pos_new)
-                pop.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    target = self.get_target_wrapper(pos_new)
-                    self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        elif self.strategy == 3:
-            for idx in range(0, self.pop_size):
-                idx_list = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 5, replace=False)
-                pos_new = self.pop[idx_list[0]][self.ID_POS] + self.wf * \
-                          (self.pop[idx_list[1]][self.ID_POS] - self.pop[idx_list[2]][self.ID_POS]) + \
-                          self.wf * (self.pop[idx_list[3]][self.ID_POS] - self.pop[idx_list[4]][self.ID_POS])
-                pos_new = self.mutation__(self.pop[idx][self.ID_POS], pos_new)
-                pop.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    target = self.get_target_wrapper(pos_new)
-                    self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        elif self.strategy == 4:
-            for idx in range(0, self.pop_size):
-                idx_list = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
-                pos_new = self.pop[idx][self.ID_POS] + self.wf * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]) + \
-                          self.wf * (self.pop[idx_list[0]][self.ID_POS] - self.pop[idx_list[1]][self.ID_POS])
-                pos_new = self.mutation__(self.pop[idx][self.ID_POS], pos_new)
-                pop.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    target = self.get_target_wrapper(pos_new)
-                    self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        else:
-            for idx in range(0, self.pop_size):
-                idx_list = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 3, replace=False)
-                pos_new = self.pop[idx][self.ID_POS] + self.wf * (self.pop[idx_list[0]][self.ID_POS] - self.pop[idx][self.ID_POS]) + \
-                          self.wf * (self.pop[idx_list[1]][self.ID_POS] - self.pop[idx_list[2]][self.ID_POS])
-                pos_new = self.mutation__(self.pop[idx][self.ID_POS], pos_new)
-                pop.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    target = self.get_target_wrapper(pos_new)
-                    self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        if self.mode in self.AVAILABLE_MODES:
-            pop = self.update_target_wrapper_population(pop)
-            self.pop = self.greedy_selection_population(self.pop, pop)
+        if self.selection == "roulette":
+            list_fitness = np.array([agent[self.ID_TAR][self.ID_FIT] for agent in pop_selected])
+            id_c1 = self.get_index_roulette_wheel_selection(list_fitness)
+            id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
+            while id_c2 == id_c1:
+                id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
+        elif self.selection == "random":
+            id_c1, id_c2 = np.random.choice(range(len(pop_selected)), 2, replace=False)
+        else:   ## tournament
+            id_c1, id_c2 = self.get_index_kway_tournament_selection(pop_selected, k_way=self.k_way, output=2)
+        return pop_selected[id_c1][self.ID_POS], pop_selected[id_c2][self.ID_POS]
+
+    def selection_process_01__(self, pop_dad, pop_mom):
+        """
+        Notes
+        ~~~~~
+        + https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_parent_selection.htm
+        + Default selection strategy is Tournament with k% = 0.2.
+        + Other strategy like "roulette" and "random" can be selected via Optional parameter "selection"
 
+        Returns:
+            list: The position of dad and mom
+        """
+        if self.selection == "roulette":
+            list_fit_dad = np.array([agent[self.ID_TAR][self.ID_FIT] for agent in pop_dad])
+            list_fit_mom = np.array([agent[self.ID_TAR][self.ID_FIT] for agent in pop_mom])
+            id_c1 = self.get_index_roulette_wheel_selection(list_fit_dad)
+            id_c2 = self.get_index_roulette_wheel_selection(list_fit_mom)
+        elif self.selection == "random":
+            id_c1 = np.random.choice(range(len(pop_dad)))
+            id_c2 = np.random.choice(range(len(pop_mom)))
+        else:   ## tournament
+            id_c1 = self.get_index_kway_tournament_selection(pop_dad, k_way=self.k_way, output=1)[0]
+            id_c2 = self.get_index_kway_tournament_selection(pop_mom, k_way=self.k_way, output=1)[0]
+        return pop_dad[id_c1][self.ID_POS], pop_mom[id_c2][self.ID_POS]
+
+    def crossover_process__(self, dad, mom):
+        """
+        Notes
+        ~~~~~
+        + https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_crossover.htm
+        + Default crossover strategy is "uniform"
+        + Other strategy like "arithmetic", "one_point", "multi_points" can be selected via parameter: crossover
 
-class JADE(Optimizer):
-    """
-    The original version of: Differential Evolution (JADE)
+        Args:
+            dad (np.array): The position of dad
+            mom (np.array): The position of mom
 
-    Links:
-        1. https://doi.org/10.1109/TEVC.2009.2014613
+        Returns:
+            list: The position of child 1 and child 2
+        """
+        if self.crossover == "arithmetic":
+            w1, w2 = self.crossover_arithmetic(dad, mom)
+        elif self.crossover == "one_point":
+            cut = np.random.randint(1, self.problem.n_dims-1)
+            w1 = np.concatenate([ dad[:cut], mom[cut:] ])
+            w2 = np.concatenate([ mom[:cut], dad[cut:] ])
+        elif self.crossover == "multi_points":
+            idxs = np.random.choice(range(1, self.problem.n_dims-1), 2, replace=False)
+            cut1, cut2 = np.min(idxs), np.max(idxs)
+            w1 = np.concatenate([ dad[:cut1], mom[cut1:cut2], dad[cut2:] ])
+            w2 = np.concatenate([ mom[:cut1], dad[cut1:cut2], mom[cut2:] ])
+        else:           # uniform
+            flip = np.random.randint(0, 2, self.problem.n_dims)
+            w1 = dad * flip + mom * (1 - flip)
+            w2 = mom * flip + dad * (1 - flip)
+        return w1, w2
+
+    def mutation_process__(self, child):
+        """
+        Notes
+        ~~~~~
+        + https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_mutation.htm
+        + There are 2 strategies that effects by the mutation probability: Mutated on single point or the whole vector.
+            + Multiple points (whole vector) has 2 strategies selected via parameter: mutation
+                + flip --> (default in this case) should set the pm small such as: [0.01 -> 0.2]
+                + swap --> should set the pm small such as: [0.01 -> 0.2]
+            + Single point has 4 strategies:
+                + flip --> should set the pm large such as: [0.5 -> 0.9]
+                + swap --> same as flip: pm in range [0.5 -> 0.9]
+                + scramble --> should set the pm small enough such as: [0.4 -> 0.6]
+                + inversion --> like scramble [0.4 -> 0.6]
 
-    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + miu_f (float): [0.4, 0.6], initial adaptive f, default = 0.5
-        + miu_cr (float): [0.4, 0.6], initial adaptive cr, default = 0.5
-        + pt (float): [0.05, 0.2], The percent of top best agents (p in the paper), default = 0.1
-        + ap (float): [0.05, 0.2], The Adaptation Parameter control value of f and cr (c in the paper), default=0.1
+        Args:
+            child (np.array): The position of the child
 
-    Examples
-    ~~~~~~~~
-    >>> import numpy as np
-    >>> from mealpy.evolutionary_based.DE import JADE
-    >>>
-    >>> def fitness_function(solution):
-    >>>     return np.sum(solution**2)
-    >>>
-    >>> problem_dict1 = {
-    >>>     "fit_func": fitness_function,
-    >>>     "lb": [-10, -15, -4, -2, -8],
-    >>>     "ub": [10, 15, 12, 8, 20],
-    >>>     "minmax": "min",
-    >>> }
-    >>>
-    >>> epoch = 1000
-    >>> pop_size = 50
-    >>> miu_f = 0.5
-    >>> miu_cr = 0.5
-    >>> pt = 0.1
-    >>> ap = 0.1
-    >>> model = JADE(epoch, pop_size, miu_f, miu_cr, pt, ap)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
-    >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+        Returns:
+            np.array: The mutated vector of the child
+        """
 
-    References
-    ~~~~~~~~~~
-    [1] Zhang, J. and Sanderson, A.C., 2009. JADE: adaptive differential evolution with optional
-    external archive. IEEE Transactions on evolutionary computation, 13(5), pp.945-958.
-    """
+        if self.mutation_multipoints:
+            if self.mutation == "swap":
+                for idx in range(self.problem.n_dims):
+                    idx_swap = np.random.choice(list(set(range(0, self.problem.n_dims)) - {idx}))
+                    child[idx], child[idx_swap] = child[idx_swap], child[idx]
+                    return child
+            else:       # "flip"
+                mutation_child = self.generate_position(self.problem.lb, self.problem.ub)
+                flag_child = np.random.uniform(0, 1, self.problem.n_dims) < self.pm
+                return np.where(flag_child, mutation_child, child)
+        else:
+            if self.mutation == "swap":
+                idx1, idx2 = np.random.choice(range(0, self.problem.n_dims), 2, replace=False)
+                child[idx1], child[idx2] = child[idx2], child[idx1]
+                return child
+            elif self.mutation == "inversion":
+                cut1, cut2 = np.random.choice(range(0, self.problem.n_dims), 2, replace=False)
+                temp = child[cut1:cut2]
+                temp = temp[::-1]
+                child[cut1:cut2] = temp
+                return child
+            elif self.mutation == "scramble":
+                cut1, cut2 = np.random.choice(range(0, self.problem.n_dims), 2, replace=False)
+                temp = child[cut1:cut2]
+                np.random.shuffle(temp)
+                child[cut1:cut2] = temp
+                return child
+            else:   # "flip"
+                idx = np.random.randint(0, self.problem.n_dims)
+                child[idx] = np.random.uniform(self.problem.lb[idx], self.problem.ub[idx])
+                return child
 
-    def __init__(self, epoch=10000, pop_size=100, miu_f=0.5, miu_cr=0.5, pt=0.1, ap=0.1, **kwargs):
+    def survivor_process__(self, pop, pop_child):
         """
+        The current survivor process is select the worst solution out of k-way solutions (tournament selection) and
+        compare with child solutions. The better solution will be kept for the next generation.
+
         Args:
-            epoch (int): maximum number of iterations, default = 10000
-            pop_size (int): number of population size, default = 100
-            miu_f (float): initial adaptive f, default = 0.5
-            miu_cr (float): initial adaptive cr, default = 0.5
-            pt (float): The percent of top best agents (p in the paper), default = 0.1
-            ap (float): The Adaptation Parameter control value of f and cr (c in the paper), default=0.1
-        """
-        super().__init__(**kwargs)
-        self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
-        self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.miu_f = self.validator.check_float("miu_f", miu_f, (0, 1.0))
-        self.miu_cr = self.validator.check_float("miu_cr", miu_cr, (0, 1.0))
-        # np.random.uniform(0.05, 0.2) # the x_best is select from the top 100p % solutions
-        self.pt = self.validator.check_float("pt", pt, (0, 1.0))
-        # np.random.uniform(1/20, 1/5) # the adaptation parameter control value of f and cr
-        self.ap = self.validator.check_float("ap", ap, (0, 1.0))
-        self.set_parameters(["epoch", "pop_size", "miu_f", "miu_cr", "pt", "ap"])
-        self.sort_flag = False
+            pop: The old population
+            pop_child: The new population
 
-    def initialize_variables(self):
-        self.dyn_miu_cr = self.miu_cr
-        self.dyn_miu_f = self.miu_f
-        self.dyn_pop_archive = list()
-
-    ### Survivor Selection
-    def lehmer_mean(self, list_objects):
-        temp = sum(list_objects)
-        return 0 if temp == 0 else sum(list_objects ** 2) / temp
+        Returns:
+            The new population
+        """
+        pop_new = []
+        for idx in range(0, self.pop_size):
+            id_child = self.get_index_kway_tournament_selection(pop, k_way=0.1, output=1, reverse=True)[0]
+            pop_new.append(self.get_better_solution(pop_child[idx], pop[id_child]))
+        return pop_new
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        list_f = list()
-        list_cr = list()
-        temp_f = list()
-        temp_cr = list()
+        list_fitness = np.array([agent[self.ID_TAR][self.ID_FIT] for agent in self.pop])
+        pop_new = []
+        for i in range(0, int(self.pop_size/2)):
+            ### Selection
+            child1, child2 = self.selection_process__(list_fitness)
+
+            ### Crossover
+            if np.random.uniform() < self.pc:
+                child1, child2 = self.crossover_process__(child1, child2)
+
+            ### Mutation
+            child1 = self.mutation_process__(child1)
+            child2 = self.mutation_process__(child2)
+
+            child1 = self.amend_position(child1, self.problem.lb, self.problem.ub)
+            child2 = self.amend_position(child2, self.problem.lb, self.problem.ub)
+
+            pop_new.append([child1, None])
+            pop_new.append([child2, None])
 
-        pop_sorted = self.get_sorted_strim_population(self.pop)
-        pop = []
-        for idx in range(0, self.pop_size):
-            ## Calculate adaptive parameter cr and f
-            cr = np.random.normal(self.dyn_miu_cr, 0.1)
-            cr = np.clip(cr, 0, 1)
-            while True:
-                f = cauchy.rvs(self.dyn_miu_f, 0.1)
-                if f < 0:
-                    continue
-                elif f > 1:
-                    f = 1
-                break
-            temp_f.append(f)
-            temp_cr.append(cr)
-            top = int(self.pop_size * self.pt)
-            x_best = pop_sorted[np.random.randint(0, top)]
-            x_r1 = self.pop[np.random.choice(list(set(range(0, self.pop_size)) - {idx}))]
-            new_pop = self.pop + self.dyn_pop_archive
-            while True:
-                x_r2 = new_pop[np.random.randint(0, len(new_pop))]
-                if np.any(x_r2[self.ID_POS] - x_r1[self.ID_POS]) and np.any(x_r2[self.ID_POS] - self.pop[idx][self.ID_POS]):
-                    break
-            x_new = self.pop[idx][self.ID_POS] + f * (x_best[self.ID_POS] - self.pop[idx][self.ID_POS]) + f * (x_r1[self.ID_POS] - x_r2[self.ID_POS])
-            pos_new = np.where(np.random.random(self.problem.n_dims) < cr, x_new, self.pop[idx][self.ID_POS])
-            j_rand = np.random.randint(0, self.problem.n_dims)
-            pos_new[j_rand] = x_new[j_rand]
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
-                pop[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-        pop = self.update_target_wrapper_population(pop)
-        for idx in range(0, self.pop_size):
-            if self.compare_agent(pop[idx], self.pop[idx]):
-                self.dyn_pop_archive.append(deepcopy(self.pop[idx]))
-                list_cr.append(temp_cr[idx])
-                list_f.append(temp_f[idx])
-                self.pop[idx] = deepcopy(pop[idx])
-
-        # Randomly remove solution
-        temp = len(self.dyn_pop_archive) - self.pop_size
-        if temp > 0:
-            idx_list = np.random.choice(range(0, len(self.dyn_pop_archive)), temp, replace=False)
-            archive_pop_new = []
-            for idx, solution in enumerate(self.dyn_pop_archive):
-                if idx not in idx_list:
-                    archive_pop_new.append(solution)
-            self.dyn_pop_archive = deepcopy(archive_pop_new)
-
-        # Update miu_cr and miu_f
-        if len(list_cr) == 0:
-            self.dyn_miu_cr = (1 - self.ap) * self.dyn_miu_cr + self.ap * 0.5
-        else:
-            self.dyn_miu_cr = (1 - self.ap) * self.dyn_miu_cr + self.ap * np.mean(np.array(list_cr))
-        if len(list_f) == 0:
-            self.dyn_miu_f = (1 - self.ap) * self.dyn_miu_f + self.ap * 0.5
-        else:
-            self.dyn_miu_f = (1 - self.ap) * self.dyn_miu_f + self.ap * self.lehmer_mean(np.array(list_f))
+                pop_new[-2][self.ID_TAR] = self.get_target_wrapper(child1)
+                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(child2)
+        if self.mode in self.AVAILABLE_MODES:
+            pop_new = self.update_target_wrapper_population(pop_new)
+        ### Survivor Selection
+        self.pop = self.survivor_process__(self.pop, pop_new)
 
 
-class SADE(Optimizer):
+class SingleGA(BaseGA):
     """
-    The original version of: Self-Adaptive Differential Evolution (SADE)
+    The developed single-point mutation of: Genetic Algorithm (GA)
 
     Links:
-        1. https://doi.org/10.1109/CEC.2005.1554904
+        1. https://blog.sicara.com/getting-started-genetic-algorithms-python-tutorial-81ffa1dd72f9
+        2. https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_quick_guide.htm
+        3. https://www.analyticsvidhya.com/blog/2017/07/introduction-to-genetic-algorithm/
+
+    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
+        + pc (float): [0.7, 0.95], cross-over probability, default = 0.95
+        + pm (float): [0.01, 0.2], mutation probability, default = 0.025
+        + selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+        + crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+        + mutation (str): Optional, can be ["flip", "swap", "scramble", "inversion"] for one-point
+        + k_way (float): Optional, set it when use "tournament" selection, default = 0.2
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.evolutionary_based.DE import SADE
+    >>> from mealpy.evolutionary_based.GA import SingleGA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = SADE(epoch, pop_size)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
+    >>> pc = 0.9
+    >>> pm = 0.8
+    >>> selection = "roulette"
+    >>> crossover = "uniform"
+    >>> mutation = "swap"
+    >>> model1 = SingleGA(epoch, pop_size, pc, pm, selection, crossover, mutation)
+    >>> best_position, best_fitness = model1.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+    >>>
+    >>> model2 = SingleGA(epoch, pop_size, pc, pm, selection="tournament", k_way=0.4, crossover="multi_points")
+    >>>
+    >>> model3 = SingleGA(epoch, pop_size, pc, pm, crossover="one_point", mutation="scramble")
+    >>>
+    >>> model4 = SingleGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation="swap")
+    >>>
+    >>> model5 = SingleGA(epoch, pop_size, pc, pm, selection="roulette", crossover="multi_points")
+    >>>
+    >>> model6 = SingleGA(epoch, pop_size, pc, pm, selection="random", mutation="inversion")
+    >>>
+    >>> model7 = SingleGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation="flip")
 
     References
     ~~~~~~~~~~
-    [1] Qin, A.K. and Suganthan, P.N., 2005, September. Self-adaptive differential evolution algorithm for
-    numerical optimization. In 2005 IEEE congress on evolutionary computation (Vol. 2, pp. 1785-1791). IEEE.
+    [1] Whitley, D., 1994. A genetic algorithm tutorial. Statistics and computing, 4(2), pp.65-85.
     """
 
-    def __init__(self, epoch=10000, pop_size=100, **kwargs):
+    def __init__(self, epoch=10000, pop_size=100, pc=0.95, pm=0.8, selection="roulette",
+                 crossover="uniform", mutation="swap", k_way=0.2, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
-        """
-        super().__init__(**kwargs)
-        self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
-        self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.set_parameters(["epoch", "pop_size"])
+            pc (float): cross-over probability, default = 0.95
+            pm (float): mutation probability, default = 0.8
+            selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+            crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+            mutation (str): Optional, can be ["flip", "swap", "scramble", "inversion"], default="flip"
+            k_way (float): Optional, set it when use "tournament" selection, default = 0.2
+        """
+        super().__init__(epoch, pop_size, pc, pm, **kwargs)
+        self.selection = self.validator.check_str("selection", selection, ["tournament", "random", "roulette"])
+        self.crossover = self.validator.check_str("crossover", crossover, ["one_point", "multi_points", "uniform", "arithmetic"])
+        self.mutation = self.validator.check_str("mutation", mutation, ["flip", "swap", "scramble", "inversion"])
+        self.k_way = self.validator.check_float("k_way", k_way, (0, 1.0))
+        self.set_parameters(["epoch", "pop_size", "pc", "pm", "selection", "crossover", "mutation", "k_way"])
         self.sort_flag = False
 
-    def initialize_variables(self):
-        self.loop_probability = 50
-        self.loop_cr = 5
-        self.ns1 = self.ns2 = self.nf1 = self.nf2 = 0
-        self.crm = 0.5
-        self.p1 = 0.5
-        self.dyn_list_cr = list()
-
-    def evolve(self, epoch):
+    def mutation_process__(self, child):
         """
-        The main operations (equations) of algorithm. Inherit from Optimizer class
+        + https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_mutation.htm
+        + The mutation process is effected by parameter: pm
+            + flip --> should set the pm large such as: [0.5 -> 0.9]
+            + swap --> same as flip: pm in range [0.5 -> 0.9]
+            + scramble --> should set the pm small enough such as: [0.4 -> 0.6]
+            + inversion --> like scramble [0.4 -> 0.6]
 
         Args:
-            epoch (int): The current iteration
-        """
-        pop = []
-        list_probability = []
-        list_cr = []
-        for idx in range(0, self.pop_size):
-            ## Calculate adaptive parameter cr and f
-            cr = np.random.normal(self.crm, 0.1)
-            cr = np.clip(cr, 0, 1)
-            list_cr.append(cr)
-            while True:
-                f = np.random.normal(0.5, 0.3)
-                if f < 0:
-                    continue
-                elif f > 1:
-                    f = 1
-                break
-
-            id1, id2, id3 = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 3, replace=False)
-            if np.random.rand() < self.p1:
-                x_new = self.pop[id1][self.ID_POS] + f * (self.pop[id2][self.ID_POS] - self.pop[id3][self.ID_POS])
-                pos_new = np.where(np.random.random(self.problem.n_dims) < cr, x_new, self.pop[idx][self.ID_POS])
-                j_rand = np.random.randint(0, self.problem.n_dims)
-                pos_new[j_rand] = x_new[j_rand]
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                list_probability.append(True)
-            else:
-                x_new = self.pop[idx][self.ID_POS] + f * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]) + \
-                        f * (self.pop[id1][self.ID_POS] - self.pop[id2][self.ID_POS])
-                pos_new = np.where(np.random.random(self.problem.n_dims) < cr, x_new, self.pop[idx][self.ID_POS])
-                j_rand = np.random.randint(0, self.problem.n_dims)
-                pos_new[j_rand] = x_new[j_rand]
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                list_probability.append(False)
-            pop.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                pop[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-        pop = self.update_target_wrapper_population(pop)
+            child (np.array): The position of the child
 
-        for idx in range(0, self.pop_size):
-            if list_probability[idx]:
-                if self.compare_agent(pop[idx], self.pop[idx]):
-                    self.ns1 += 1
-                    self.pop[idx] = deepcopy(pop[idx])
-                else:
-                    self.nf1 += 1
-            else:
-                if self.compare_agent(pop[idx], self.pop[idx]):
-                    self.ns2 += 1
-                    self.dyn_list_cr.append(list_cr[idx])
-                    self.pop[idx] = deepcopy(pop[idx])
-                else:
-                    self.nf2 += 1
-
-        # Update cr and p1
-        if (epoch + 1) / self.loop_cr == 0:
-            self.crm = np.mean(self.dyn_list_cr)
-            self.dyn_list_cr = list()
-
-        if (epoch + 1) / self.loop_probability == 0:
-            self.p1 = self.ns1 * (self.ns2 + self.nf2) / (self.ns2 * (self.ns1 + self.nf1) + self.ns1 * (self.ns2 + self.nf2))
-            self.ns1 = self.ns2 = self.nf1 = self.nf2 = 0
+        Returns:
+            np.array: The mutated vector of the child
+        """
+        if self.mutation == "swap":
+            idx1, idx2 = np.random.choice(range(0, self.problem.n_dims), 2, replace=False)
+            child[idx1], child[idx2] = child[idx2], child[idx1]
+            return child
+        elif self.mutation == "inversion":
+            cut1, cut2 = np.random.choice(range(0, self.problem.n_dims), 2, replace=False)
+            temp = child[cut1:cut2]
+            temp = temp[::-1]
+            child[cut1:cut2] = temp
+            return child
+        elif self.mutation == "scramble":
+            cut1, cut2 = np.random.choice(range(0, self.problem.n_dims), 2, replace=False)
+            temp = child[cut1:cut2]
+            np.random.shuffle(temp)
+            child[cut1:cut2] = temp
+            return child
+        else:   # "flip"
+            idx = np.random.randint(0, self.problem.n_dims)
+            child[idx] = np.random.uniform(self.problem.lb[idx], self.problem.ub[idx])
+            return child
 
 
-class SHADE(Optimizer):
+class EliteSingleGA(SingleGA):
     """
-    The original version of: Success-History Adaptation Differential Evolution (SHADE)
+    The developed elite single-point mutation of: Genetic Algorithm (GA)
 
     Links:
-        1. https://doi.org/10.1109/CEC.2013.6557555
+        1. https://www.baeldung.com/cs/elitism-in-evolutionary-algorithms
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + miu_f (float): [0.4, 0.6], initial weighting factor, default = 0.5
-        + miu_cr (float): [0.4, 0.6], initial cross-over probability, default = 0.5
+        + pc (float): [0.7, 0.95], cross-over probability, default = 0.95
+        + pm (float): [0.01, 0.2], mutation probability, default = 0.025
+        + selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+        + crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+        + mutation (str): Optional, can be ["flip", "swap", "scramble", "inversion"] for one-point
+        + k_way (float): Optional, set it when use "tournament" selection, default = 0.2
+        + elite_best (float/int): Optional, can be float (percentage of the best in elite group), or int (the number of best elite), default = 0.1
+        + elite_worst (float/int): Opttional, can be float (percentage of the worst in elite group), or int (the number of worst elite), default = 0.3
+        + strategy (int): Optional, can be 0 or 1. If = 0, the selection is select parents from (elite_worst + non_elite_group).
+            Else, the selection will select dad from elite_worst and mom from non_elite_group.
+        + pop_size = elite_group (elite_best + elite_worst) + non_elite_group
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.evolutionary_based.DE import SHADE
+    >>> from mealpy.evolutionary_based.GA import EliteSingleGA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> miu_f = 0.5
-    >>> miu_cr = 0.5
-    >>> model = SHADE( epoch, pop_size, miu_f, miu_cr)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
+    >>> pc = 0.9
+    >>> pm = 0.8
+    >>> selection = "roulette"
+    >>> crossover = "uniform"
+    >>> mutation = "swap"
+    >>> elite_best = 0.1
+    >>> elite_worst = 0.3
+    >>> strategy = 0
+    >>> model1 = EliteSingleGA(epoch, pop_size, pc, pm, selection, crossover, mutation, elite_best, elite_worst, strategy)
+    >>> best_position, best_fitness = model1.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+    >>>
+    >>> model2 = EliteSingleGA(epoch, pop_size, pc, pm, selection="tournament", k_way=0.4, crossover="multi_points")
+    >>>
+    >>> model3 = EliteSingleGA(epoch, pop_size, pc, pm, crossover="one_point", mutation="scramble")
+    >>>
+    >>> model4 = EliteSingleGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation="swap")
+    >>>
+    >>> model5 = EliteSingleGA(epoch, pop_size, pc, pm, selection="roulette", crossover="multi_points")
+    >>>
+    >>> model6 = EliteSingleGA(epoch, pop_size, pc, pm, selection="random", mutation="inversion")
+    >>>
+    >>> model7 = EliteSingleGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation="flip")
 
     References
     ~~~~~~~~~~
-    [1] Tanabe, R. and Fukunaga, A., 2013, June. Success-history based parameter adaptation for
-    differential evolution. In 2013 IEEE congress on evolutionary computation (pp. 71-78). IEEE.
+    [1] Whitley, D., 1994. A genetic algorithm tutorial. Statistics and computing, 4(2), pp.65-85.
     """
 
-    def __init__(self, epoch=750, pop_size=100, miu_f=0.5, miu_cr=0.5, **kwargs):
-        """
-        Args:
-            epoch (int): maximum number of iterations, default = 10000
-            pop_size (int): number of population size, default = 100
-            miu_f (float): initial weighting factor, default = 0.5
-            miu_cr (float): initial cross-over probability, default = 0.5
-        """
-        super().__init__(**kwargs)
-        self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
-        self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        # the initial f, location is changed then that f is good
-        self.miu_f = self.validator.check_float("miu_f", miu_f, (0, 1.0))
-        # the initial cr,
-        self.miu_cr = self.validator.check_float("miu_cr", miu_cr, (0, 1.0))
-        self.set_parameters(["epoch", "pop_size", "miu_f", "miu_cr"])
-        self.sort_flag = False
-
-    def initialize_variables(self):
-        self.dyn_miu_f = self.miu_f * np.ones(self.pop_size)  # list the initial f,
-        self.dyn_miu_cr = self.miu_cr * np.ones(self.pop_size)  # list the initial cr,
-        self.dyn_pop_archive = list()
-        self.k_counter = 0
-
-    ### Survivor Selection
-    def weighted_lehmer_mean__(self, list_objects, list_weights):
-        up = list_weights * list_objects ** 2
-        down = list_weights * list_objects
-        return np.sum(up) / np.sum(down)
+    def __init__(self, epoch=10000, pop_size=100, pc=0.95, pm=0.8, selection="roulette",
+                 crossover="uniform", mutation="swap", k_way=0.2,
+                 elite_best=0.1, elite_worst=0.3, strategy=0, **kwargs):
+        super().__init__(epoch, pop_size, pc, pm, selection, crossover, mutation, k_way, **kwargs)
+        self.elite_best = self.validator.check_is_int_and_float("elite_best", elite_best, [1, int(self.pop_size / 2)-1], (0, 0.5))
+        self.n_elite_best = int(self.elite_best * self.pop_size) if self.elite_best < 1 else self.elite_best
+        if self.n_elite_best < 1:
+            self.n_elite_best = 1
+
+        self.elite_worst = self.validator.check_is_int_and_float("elite_worst", elite_worst, [1, int(self.pop_size / 2)-1], (0, 0.5))
+        self.n_elite_worst = int(self.elite_worst * self.pop_size) if self.elite_worst < 1 else self.elite_worst
+        if self.n_elite_worst < 1:
+            self.n_elite_worst = 1
+
+        self.strategy = self.validator.check_int("strategy", strategy, [0, 1])
+        self.set_parameters(["epoch", "pop_size", "pc", "pm", "selection", "crossover", "mutation", "k_way",
+                             "elite_best", "elite_worst", "strategy"])
+        self.sort_flag = True
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        list_f = list()
-        list_cr = list()
-        list_f_index = list()
-        list_cr_index = list()
-
-        list_f_new = np.ones(self.pop_size)
-        list_cr_new = np.ones(self.pop_size)
-        pop_old = deepcopy(self.pop)
-        pop_sorted = self.get_sorted_strim_population(self.pop)
+        pop_new = self.pop[:self.n_elite_best]
 
-        pop = []
-        for idx in range(0, self.pop_size):
-            ## Calculate adaptive parameter cr and f
-            idx_rand = np.random.randint(0, self.pop_size)
-            cr = np.random.normal(self.dyn_miu_cr[idx_rand], 0.1)
-            cr = np.clip(cr, 0, 1)
-            while True:
-                f = cauchy.rvs(self.dyn_miu_f[idx_rand], 0.1)
-                if f < 0:
-                    continue
-                elif f > 1:
-                    f = 1
-                break
-            list_cr_new[idx] = cr
-            list_f_new[idx] = f
-            p = np.random.uniform(2 / self.pop_size, 0.2)
-            top = int(self.pop_size * p)
-            x_best = pop_sorted[np.random.randint(0, top)]
-            x_r1 = self.pop[np.random.choice(list(set(range(0, self.pop_size)) - {idx}))]
-            new_pop = self.pop + self.dyn_pop_archive
-            while True:
-                x_r2 = new_pop[np.random.randint(0, len(new_pop))]
-                if np.any(x_r2[self.ID_POS] - x_r1[self.ID_POS]) and np.any(x_r2[self.ID_POS] - self.pop[idx][self.ID_POS]):
-                    break
-            x_new = self.pop[idx][self.ID_POS] + f * (x_best[self.ID_POS] - self.pop[idx][self.ID_POS]) + f * (x_r1[self.ID_POS] - x_r2[self.ID_POS])
-            condition = np.random.random(self.problem.n_dims) < cr
-            pos_new = np.where(condition, x_new, self.pop[idx][self.ID_POS])
-            j_rand = np.random.randint(0, self.problem.n_dims)
-            pos_new[j_rand] = x_new[j_rand]
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                pop[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-        pop = self.update_target_wrapper_population(pop)
-
-        for i in range(0, self.pop_size):
-            if self.compare_agent(pop[i], self.pop[i]):
-                list_cr.append(list_cr_new[i])
-                list_f.append(list_f_new[i])
-                list_f_index.append(i)
-                list_cr_index.append(i)
-                self.pop[i] = deepcopy(pop[i])
-                self.dyn_pop_archive.append(deepcopy(pop[i]))
-
-        # Randomly remove solution
-        temp = len(self.dyn_pop_archive) - self.pop_size
-        if temp > 0:
-            idx_list = np.random.choice(range(0, len(self.dyn_pop_archive)), temp, replace=False)
-            archive_pop_new = []
-            for idx, solution in enumerate(self.dyn_pop_archive):
-                if idx not in idx_list:
-                    archive_pop_new.append(solution)
-            self.dyn_pop_archive = deepcopy(archive_pop_new)
-
-        # Update miu_cr and miu_f
-        if len(list_f) != 0 and len(list_cr) != 0:
-            # Eq.13, 14, 10
-            list_fit_old = np.ones(len(list_cr_index))
-            list_fit_new = np.ones(len(list_cr_index))
-            idx_increase = 0
-            for i in range(0, self.pop_size):
-                if i in list_cr_index:
-                    list_fit_old[idx_increase] = pop_old[i][self.ID_TAR][self.ID_FIT]
-                    list_fit_new[idx_increase] = self.pop[i][self.ID_TAR][self.ID_FIT]
-                    idx_increase += 1
-            temp = np.sum(np.abs(list_fit_new - list_fit_old))
-            if temp == 0:
-                list_weights = 1.0 / len(list_fit_new) * np.ones(len(list_fit_new))
-            else:
-                list_weights = np.abs(list_fit_new - list_fit_old) / temp
-            self.dyn_miu_cr[self.k_counter] = np.sum(list_weights * np.array(list_cr))
-            self.dyn_miu_f[self.k_counter] = self.weighted_lehmer_mean__(np.array(list_f), list_weights)
-            self.k_counter += 1
-            if self.k_counter >= self.pop_size:
-                self.k_counter = 0
+        if self.strategy == 0:
+            pop_old = self.pop[self.n_elite_best:]
+            for idx in range(self.n_elite_best, self.pop_size):
+                ### Selection
+                child1, child2 = self.selection_process_00__(pop_old)
+                ### Crossover
+                if np.random.uniform() < self.pc:
+                    child1, child2 = self.crossover_process__(child1, child2)
+                child = child1 if np.random.random() <= 0.5 else child2
+                ### Mutation
+                child = self.mutation_process__(child)
+                ### Survivor Selection
+                pos_new = self.amend_position(child, self.problem.lb, self.problem.ub)
+                pop_new.append([pos_new, None])
+                if self.mode not in self.AVAILABLE_MODES:
+                    pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+            self.pop = self.update_target_wrapper_population(pop_new)
+        else:
+            pop_dad = self.pop[self.n_elite_best:self.n_elite_best+self.n_elite_worst]
+            pop_mom = self.pop[self.n_elite_best+self.n_elite_worst:]
+            for idx in range(self.n_elite_best, self.pop_size):
+                ### Selection
+                child1, child2 = self.selection_process_01__(pop_dad, pop_mom)
+                ### Crossover
+                if np.random.uniform() < self.pc:
+                    child1, child2 = self.crossover_process__(child1, child2)
+                child = child1 if np.random.random() <= 0.5 else child2
+                ### Mutation
+                child = self.mutation_process__(child)
+                ### Survivor Selection
+                pos_new = self.amend_position(child, self.problem.lb, self.problem.ub)
+                pop_new.append([pos_new, None])
+                if self.mode not in self.AVAILABLE_MODES:
+                    pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+            self.pop = self.update_target_wrapper_population(pop_new)
 
 
-class L_SHADE(Optimizer):
+class MultiGA(BaseGA):
     """
-    The original version of: Linear Population Size Reduction Success-History Adaptation Differential Evolution (LSHADE)
+    The developed multipoints-mutation version of: Genetic Algorithm (GA)
 
     Links:
-        1. https://metahack.org/CEC2014-Tanabe-Fukunaga.pdf
+        1. https://blog.sicara.com/getting-started-genetic-algorithms-python-tutorial-81ffa1dd72f9
+        2. https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_quick_guide.htm
+        3. https://www.analyticsvidhya.com/blog/2017/07/introduction-to-genetic-algorithm/
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + miu_f (float): [0.4, 0.6], initial weighting factor, default = 0.5
-        + miu_cr (float): [0.4, 0.6], initial cross-over probability, default = 0.5
+        + pc (float): [0.7, 0.95], cross-over probability, default = 0.95
+        + pm (float): [0.01, 0.2], mutation probability, default = 0.025
+        + selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+        + k_way (float): Optional, set it when use "tournament" selection, default = 0.2
+        + crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+        + mutation (str): Optional, can be ["flip", "swap"] for multipoints
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.evolutionary_based.DE import L_SHADE
+    >>> from mealpy.evolutionary_based.GA import MultiGA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> miu_f = 0.5
-    >>> miu_cr = 0.5
-    >>> model = L_SHADE(epoch, pop_size, miu_f, miu_cr)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
+    >>> pc = 0.9
+    >>> pm = 0.05
+    >>> selection = "roulette"
+    >>> crossover = "uniform"
+    >>> mutation = "swap"
+    >>> model1 = MultiGA(epoch, pop_size, pc, pm, selection, crossover, mutation)
+    >>> best_position, best_fitness = model1.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+    >>>
+    >>> model2 = MultiGA(epoch, pop_size, pc, pm, selection="tournament", k_way=0.4, crossover="multi_points")
+    >>>
+    >>> model3 = MultiGA(epoch, pop_size, pc, pm, crossover="one_point", mutation="flip")
+    >>>
+    >>> model4 = MultiGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation_multipoints=True, mutation="swap")
+    >>>
+    >>> model5 = MultiGA(epoch, pop_size, pc, pm, selection="roulette", crossover="multi_points")
+    >>>
+    >>> model6 = MultiGA(epoch, pop_size, pc, pm, selection="random", mutation="swap")
+    >>>
+    >>> model7 = MultiGA(epoch, pop_size, pc, pm, crossover="arithmetic", mutation="flip")
 
     References
     ~~~~~~~~~~
-    [1] Tanabe, R. and Fukunaga, A.S., 2014, July. Improving the search performance of SHADE using
-    linear population size reduction. In 2014 IEEE congress on evolutionary computation (CEC) (pp. 1658-1665). IEEE.
+    [1] Whitley, D., 1994. A genetic algorithm tutorial. Statistics and computing, 4(2), pp.65-85.
     """
 
-    def __init__(self, epoch=750, pop_size=100, miu_f=0.5, miu_cr=0.5, **kwargs):
+    def __init__(self, epoch=10000, pop_size=100, pc=0.95, pm=0.025,
+                 selection="roulette", crossover="arithmetic", mutation="flip", k_way=0.2, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
-            miu_f (float): initial weighting factor, default = 0.5
-            miu_cr (float): initial cross-over probability, default = 0.5
-        """
-        super().__init__(**kwargs)
-        self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
-        self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.miu_f = self.validator.check_float("miu_f", miu_f, (0, 1.0))
-        self.miu_cr = self.validator.check_float("miu_cr", miu_cr, (0, 1.0))
-        self.set_parameters(["epoch", "pop_size", "miu_f", "miu_cr"])
-        self.sort_flag = False
-
-    def initialize_variables(self):
-        # Dynamic variable
-        self.dyn_miu_f = self.miu_f * np.ones(self.pop_size)  # list the initial f,
-        self.dyn_miu_cr = self.miu_cr * np.ones(self.pop_size)  # list the initial cr,
-        self.dyn_pop_archive = list()
-        self.dyn_pop_size = self.pop_size
-        self.k_counter = 0
-        self.n_min = int(self.pop_size / 5)
-
-    ### Survivor Selection
-    def weighted_lehmer_mean__(self, list_objects, list_weights):
-        up = np.sum(list_weights * list_objects ** 2)
-        down = np.sum(list_weights * list_objects)
-        return up / down if down != 0 else 0.5
-
-    def evolve(self, epoch):
-        """
-        The main operations (equations) of algorithm. Inherit from Optimizer class
+            pc (float): cross-over probability, default = 0.95
+            pm (float): mutation probability, default = 0.025
+            selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+            crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+            mutation (str): Optional, can be ["flip", "swap"] for multipoints
+            k_way (float): Optional, set it when use "tournament" selection, default = 0.2
+        """
+        super().__init__(epoch, pop_size, pc, pm, **kwargs)
+        self.selection = self.validator.check_str("selection", selection, ["tournament", "random", "roulette"])
+        self.crossover = self.validator.check_str("crossover", crossover, ["one_point", "multi_points", "uniform", "arithmetic"])
+        self.mutation = self.validator.check_str("mutation", mutation, ["flip", "swap"])
+        self.k_way = self.validator.check_float("k_way", k_way, (0, 1.0))
+        self.set_parameters(["epoch", "pop_size", "pc", "pm", "selection", "crossover", "mutation", "k_way"])
+
+    def mutation_process__(self, child):
+        """
+        + https://www.tutorialspoint.com/genetic_algorithms/genetic_algorithms_mutation.htm
+        + Mutated on the whole vector is effected by parameter: pm
+            + flip --> (default in this case) should set the pm small such as: [0.01 -> 0.2]
+            + swap --> should set the pm small such as: [0.01 -> 0.2]
 
         Args:
-            epoch (int): The current iteration
-        """
-        list_f = list()
-        list_cr = list()
-        list_f_index = list()
-        list_cr_index = list()
-
-        list_f_new = np.ones(self.pop_size)
-        list_cr_new = np.ones(self.pop_size)
-        pop_old = deepcopy(self.pop)
-        pop_sorted = self.get_sorted_strim_population(self.pop)
-
-        pop = []
-        for idx in range(0, self.pop_size):
-            ## Calculate adaptive parameter cr and f
-            idx_rand = np.random.randint(0, self.pop_size)
-            cr = np.random.normal(self.dyn_miu_cr[idx_rand], 0.1)
-            cr = np.clip(cr, 0, 1)
-            while True:
-                f = cauchy.rvs(self.dyn_miu_f[idx_rand], 0.1)
-                if f < 0:
-                    continue
-                elif f > 1:
-                    f = 1
-                break
-            list_cr_new[idx] = cr
-            list_f_new[idx] = f
-            p = np.random.uniform(0.15, 0.2)
-            top = int(self.dyn_pop_size * p)
-            x_best = pop_sorted[np.random.randint(0, top)]
-            x_r1 = self.pop[np.random.choice(list(set(range(0, self.dyn_pop_size)) - {idx}))]
-            new_pop = self.pop + self.dyn_pop_archive
-            while True:
-                x_r2 = new_pop[np.random.randint(0, len(new_pop))]
-                if np.any(x_r2[self.ID_POS] - x_r1[self.ID_POS]) and np.any(x_r2[self.ID_POS] - self.pop[idx][self.ID_POS]):
-                    break
-            x_new = self.pop[idx][self.ID_POS] + f * (x_best[self.ID_POS] - self.pop[idx][self.ID_POS]) + f * (x_r1[self.ID_POS] - x_r2[self.ID_POS])
-            pos_new = np.where(np.random.random(self.problem.n_dims) < cr, x_new, self.pop[idx][self.ID_POS])
-            j_rand = np.random.randint(0, self.problem.n_dims)
-            pos_new[j_rand] = x_new[j_rand]
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                pop[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-        pop = self.update_target_wrapper_population(pop)
-
-        for i in range(0, self.pop_size):
-            if self.compare_agent(pop[i], self.pop[i]):
-                list_cr.append(list_cr_new[i])
-                list_f.append(list_f_new[i])
-                list_f_index.append(i)
-                list_cr_index.append(i)
-                self.pop[i] = deepcopy(pop[i])
-                self.dyn_pop_archive.append(deepcopy(self.pop[i]))
-
-        # Randomly remove solution
-        temp = len(self.dyn_pop_archive) - self.pop_size
-        if temp > 0:
-            idx_list = np.random.choice(range(0, len(self.dyn_pop_archive)), temp, replace=False)
-            archive_pop_new = []
-            for idx, solution in enumerate(self.dyn_pop_archive):
-                if idx not in idx_list:
-                    archive_pop_new.append(solution)
-            self.dyn_pop_archive = deepcopy(archive_pop_new)
-
-        # Update miu_cr and miu_f
-        if len(list_f) != 0 and len(list_cr) != 0:
-            # Eq.13, 14, 10
-            list_fit_old = np.ones(len(list_cr_index))
-            list_fit_new = np.ones(len(list_cr_index))
-            idx_increase = 0
-            for i in range(0, self.dyn_pop_size):
-                if i in list_cr_index:
-                    list_fit_old[idx_increase] = pop_old[i][self.ID_TAR][self.ID_FIT]
-                    list_fit_new[idx_increase] = self.pop[i][self.ID_TAR][self.ID_FIT]
-                    idx_increase += 1
-            total_fit = np.sum(np.abs(list_fit_new - list_fit_old))
-            list_weights = 0 if total_fit == 0 else np.abs(list_fit_new - list_fit_old) / total_fit
-            self.dyn_miu_cr[self.k_counter] = np.sum(list_weights * np.array(list_cr))
-            self.dyn_miu_f[self.k_counter] = self.weighted_lehmer_mean__(np.array(list_f), list_weights)
-            self.k_counter += 1
-            if self.k_counter >= self.dyn_pop_size:
-                self.k_counter = 0
+            child (np.array): The position of the child
 
-        # Linear Population Size Reduction
-        self.dyn_pop_size = round(self.pop_size + epoch * ((self.n_min - self.pop_size) / self.epoch))
+        Returns:
+            np.array: The mutated vector of the child
+        """
+        if self.mutation == "swap":
+            for idx in range(self.problem.n_dims):
+                idx_swap = np.random.choice(list(set(range(0, self.problem.n_dims)) - {idx}))
+                child[idx], child[idx_swap] = child[idx_swap], child[idx]
+                return child
+        else:       # "flip"
+            mutation_child = self.generate_position(self.problem.lb, self.problem.ub)
+            flag_child = np.random.uniform(0, 1, self.problem.n_dims) < self.pm
+            return np.where(flag_child, mutation_child, child)
 
 
-class SAP_DE(Optimizer):
+class EliteMultiGA(MultiGA):
     """
-    The original version of: Differential Evolution with Self-Adaptive Populations (SAP_DE)
+    The developed elite multipoints-mutation version of: Genetic Algorithm (GA)
 
     Links:
-        1. https://doi.org/10.1007/s00500-005-0537-1
+        1. https://www.baeldung.com/cs/elitism-in-evolutionary-algorithms
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + branch (str): ["ABS" or "REL"], gaussian (absolute) or uniform (relative) method
+        + pc (float): [0.7, 0.95], cross-over probability, default = 0.95
+        + pm (float): [0.01, 0.2], mutation probability, default = 0.025
+        + selection (str): Optional, can be ["roulette", "tournament", "random"], default = "tournament"
+        + k_way (float): Optional, set it when use "tournament" selection, default = 0.2
+        + crossover (str): Optional, can be ["one_point", "multi_points", "uniform", "arithmetic"], default = "uniform"
+        + mutation (str): Optional, can be ["flip", "swap"] for multipoints
+        + elite_best (float/int): Optional, can be float (percentage of the best in elite group), or int (the number of best elite), default = 0.1
+        + elite_worst (float/int): Opttional, can be float (percentage of the worst in elite group), or int (the number of worst elite), default = 0.3
+        + strategy (int): Optional, can be 0 or 1. If = 0, the selection is select parents from (elite_worst + non_elite_group).
+            Else, the selection will select dad from elite_worst and mom from non_elite_group.
+        + pop_size = elite_group (elite_best + elite_worst) + non_elite_group
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.evolutionary_based.DE import SAP_DE
+    >>> from mealpy.evolutionary_based.GA import MultiGA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> branch = "ABS"
-    >>> model = SAP_DE(epoch, pop_size, branch)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
+    >>> pc = 0.9
+    >>> pm = 0.05
+    >>> selection = "roulette"
+    >>> crossover = "uniform"
+    >>> mutation = "swap"
+    >>> model1 = MultiGA(epoch, pop_size, pc, pm, selection, crossover, mutation)
+    >>> best_position, best_fitness = model1.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+    >>>
+    >>> model2 = MultiGA(epoch, pop_size, pc, pm, selection="tournament", k_way=0.4, crossover="multi_points")
 
     References
     ~~~~~~~~~~
-    [1] Teo, J., 2006. Exploring dynamic self-adaptive populations in differential evolution. Soft Computing, 10(8), pp.673-686.
+    [1] Whitley, D., 1994. A genetic algorithm tutorial. Statistics and computing, 4(2), pp.65-85.
     """
 
-    ID_CR = 2
-    ID_MR = 3
-    ID_PS = 4
-
-    def __init__(self, epoch=750, pop_size=100, branch="ABS", **kwargs):
-        """
-        Args:
-            epoch (int): maximum number of iterations, default = 10000
-            pop_size (int): number of population size, default = 100
-            branch (str): gaussian (absolute) or uniform (relative) method
-        """
-        super().__init__(**kwargs)
-        self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
-        self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.branch = self.validator.check_str("branch", branch, ["ABS", "REL"])
-        self.set_parameters(["epoch", "pop_size", "branch"])
-        self.fixed_pop_size = self.pop_size
-        self.sort_flag = False
-
-    def create_solution(self, lb=None, ub=None, pos=None):
-        """
-        Overriding method in Optimizer class
-
-        Returns:
-            list: solution with format [position, target, crossover_rate, mutation_rate, pop_size]
-        """
-        if pos is None:
-            pos = self.generate_position(lb, ub)
-        position = self.amend_position(pos, lb, ub)
-        target = self.get_target_wrapper(position)
-        crossover_rate = np.random.uniform(0, 1)
-        mutation_rate = np.random.uniform(0, 1)
-        if self.branch == "ABS":
-            pop_size = int(10 * self.problem.n_dims + np.random.normal(0, 1))
-        else:  # elif self.branch == "REL":
-            pop_size = int(10 * self.problem.n_dims + np.random.uniform(-0.5, 0.5))
-        return [position, target, crossover_rate, mutation_rate, pop_size]
-
-    def edit_to_range(self, var=None, lower=0, upper=1, func_value=None):
-        while var <= lower or var >= upper:
-            if var <= lower:
-                var += func_value()
-            if var >= upper:
-                var -= func_value()
-        return var
+    def __init__(self, epoch=10000, pop_size=100, pc=0.95, pm=0.8, selection="roulette",
+                 crossover="uniform", mutation="swap", k_way=0.2,
+                 elite_best=0.1, elite_worst=0.3, strategy=0, **kwargs):
+        super().__init__(epoch, pop_size, pc, pm, selection, crossover, mutation, k_way, **kwargs)
+        self.elite_best = self.validator.check_is_int_and_float("elite_best", elite_best, [1, int(self.pop_size / 2) - 1], (0, 0.5))
+        self.n_elite_best = int(self.elite_best * self.pop_size) if self.elite_best < 1 else self.elite_best
+        if self.n_elite_best < 1:
+            self.n_elite_best = 1
+
+        self.elite_worst = self.validator.check_is_int_and_float("elite_worst", elite_worst, [1, int(self.pop_size / 2) - 1], (0, 0.5))
+        self.n_elite_worst = int(self.elite_worst * self.pop_size) if self.elite_worst < 1 else self.elite_worst
+        if self.n_elite_worst < 1:
+            self.n_elite_worst = 1
+
+        self.strategy = self.validator.check_int("strategy", strategy, [0, 1])
+        self.set_parameters(["epoch", "pop_size", "pc", "pm", "selection", "crossover", "mutation", "k_way",
+                             "elite_best", "elite_worst", "strategy"])
+        self.sort_flag = True
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop = []
-        for idx in range(0, self.pop_size):
-            # Choose 3 random element and different to idx
-            idxs = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 3, replace=False)
-            j = np.random.randint(0, self.pop_size)
-            self.F = np.random.normal(0, 1)
-
-            ## Crossover
-            if np.random.uniform(0, 1) < self.pop[idx][self.ID_CR] or idx == j:
-                pos_new = self.pop[idxs[0]][self.ID_POS] + self.F * (self.pop[idxs[1]][self.ID_POS] - self.pop[idxs[2]][self.ID_POS])
-                cr_new = self.pop[idxs[0]][self.ID_CR] + self.F * (self.pop[idxs[1]][self.ID_CR] - self.pop[idxs[2]][self.ID_CR])
-                mr_new = self.pop[idxs[0]][self.ID_MR] + self.F * (self.pop[idxs[1]][self.ID_MR] - self.pop[idxs[2]][self.ID_MR])
-                if self.branch == "ABS":
-                    ps_new = self.pop[idxs[0]][self.ID_PS] + int(self.F * (self.pop[idxs[1]][self.ID_PS] - self.pop[idxs[2]][self.ID_PS]))
-                else:  # elif self.branch == "REL":
-                    ps_new = self.pop[idxs[0]][self.ID_PS] + self.F * (self.pop[idxs[1]][self.ID_PS] - self.pop[idxs[2]][self.ID_PS])
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                cr_new = self.edit_to_range(cr_new, 0, 1, np.random.random)
-                mr_new = self.edit_to_range(mr_new, 0, 1, np.random.random)
-                pop.append([pos_new, None, cr_new, mr_new, ps_new])
-                if self.mode not in self.AVAILABLE_MODES:
-                    pop[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-            else:
-                pop.append(deepcopy(self.pop[idx]))
-            ## Mutation
-            if np.random.uniform(0, 1) < self.pop[idxs[0]][self.ID_MR]:
-                pos_new = self.pop[idx][self.ID_POS] + np.random.normal(0, self.pop[idxs[0]][self.ID_MR])
-                cr_new = np.random.normal(0, 1)
-                mr_new = np.random.normal(0, 1)
-                if self.branch == "ABS":
-                    ps_new = self.pop[idx][self.ID_PS] + int(np.random.normal(0.5, 1))
-                else:  # elif self.branch == "REL":
-                    ps_new = self.pop[idx][self.ID_PS] + np.random.normal(0, self.pop[idxs[0]][self.ID_MR])
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                pop.append([pos_new, None, cr_new, mr_new, ps_new])
-                if self.mode not in self.AVAILABLE_MODES:
-                    pop[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-        pop = self.update_target_wrapper_population(pop)
+        pop_new = self.pop[:self.n_elite_best]
 
-        # Calculate new population size
-        total = sum([pop[i][self.ID_PS] for i in range(0, self.pop_size)])
-        if self.branch == "ABS":
-            m_new = int(total / self.pop_size)
-        else:  # elif self.branch == "REL":
-            m_new = int(self.pop_size + total)
-        if m_new <= 4:
-            m_new = self.fixed_pop_size + int(np.random.uniform(0, 4))
-        elif m_new > 4 * self.fixed_pop_size:
-            m_new = self.fixed_pop_size - int(np.random.uniform(0, 4))
-
-        ## Change population by population size
-        if m_new <= self.pop_size:
-            self.pop = pop[:m_new]
+        if self.strategy == 0:
+            pop_old = self.pop[self.n_elite_best:]
+            for idx in range(self.n_elite_best, self.pop_size):
+                ### Selection
+                child1, child2 = self.selection_process_00__(pop_old)
+                ### Crossover
+                if np.random.uniform() < self.pc:
+                    child1, child2 = self.crossover_process__(child1, child2)
+                child = child1 if np.random.random() <= 0.5 else child2
+                ### Mutation
+                child = self.mutation_process__(child)
+                ### Survivor Selection
+                pos_new = self.amend_position(child, self.problem.lb, self.problem.ub)
+                pop_new.append([pos_new, None])
+                if self.mode not in self.AVAILABLE_MODES:
+                    pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+            self.pop = self.update_target_wrapper_population(pop_new)
         else:
-            pop_sorted = self.get_sorted_strim_population(pop)
-            self.pop = pop + pop_sorted[:m_new - self.pop_size]
-        self.pop_size = len(self.pop)
+            pop_dad = self.pop[self.n_elite_best:self.n_elite_best+self.n_elite_worst]
+            pop_mom = self.pop[self.n_elite_best+self.n_elite_worst:]
+            for idx in range(self.n_elite_best, self.pop_size):
+                ### Selection
+                child1, child2 = self.selection_process_01__(pop_dad, pop_mom)
+                ### Crossover
+                if np.random.uniform() < self.pc:
+                    child1, child2 = self.crossover_process__(child1, child2)
+                child = child1 if np.random.random() <= 0.5 else child2
+                ### Mutation
+                child = self.mutation_process__(child)
+                ### Survivor Selection
+                pos_new = self.amend_position(child, self.problem.lb, self.problem.ub)
+                pop_new.append([pos_new, None])
+                if self.mode not in self.AVAILABLE_MODES:
+                    pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+            self.pop = self.update_target_wrapper_population(pop_new)
```

### Comparing `mealpy-2.5.4a5/mealpy/evolutionary_based/EP.py` & `mealpy-2.5.4a6/mealpy/evolutionary_based/EP.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/evolutionary_based/ES.py` & `mealpy-2.5.4a6/mealpy/evolutionary_based/ES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/evolutionary_based/FPA.py` & `mealpy-2.5.4a6/mealpy/evolutionary_based/FPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/evolutionary_based/MA.py` & `mealpy-2.5.4a6/mealpy/evolutionary_based/MA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/BRO.py` & `mealpy-2.5.4a6/mealpy/human_based/BRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/BSO.py` & `mealpy-2.5.4a6/mealpy/human_based/BSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/CA.py` & `mealpy-2.5.4a6/mealpy/human_based/CA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/CHIO.py` & `mealpy-2.5.4a6/mealpy/human_based/CHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/FBIO.py` & `mealpy-2.5.4a6/mealpy/human_based/FBIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/GSKA.py` & `mealpy-2.5.4a6/mealpy/human_based/GSKA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/HBO.py` & `mealpy-2.5.4a6/mealpy/human_based/HBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/HCO.py` & `mealpy-2.5.4a6/mealpy/human_based/HCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/ICA.py` & `mealpy-2.5.4a6/mealpy/human_based/ICA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/LCO.py` & `mealpy-2.5.4a6/mealpy/human_based/LCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/QSA.py` & `mealpy-2.5.4a6/mealpy/human_based/QSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/SARO.py` & `mealpy-2.5.4a6/mealpy/human_based/SARO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/SPBO.py` & `mealpy-2.5.4a6/mealpy/human_based/SPBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/SSDO.py` & `mealpy-2.5.4a6/mealpy/human_based/SSDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/TLO.py` & `mealpy-2.5.4a6/mealpy/human_based/TLO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/TOA.py` & `mealpy-2.5.4a6/mealpy/human_based/TOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/human_based/WarSO.py` & `mealpy-2.5.4a6/mealpy/human_based/WarSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/AOA.py` & `mealpy-2.5.4a6/mealpy/math_based/AOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/CEM.py` & `mealpy-2.5.4a6/mealpy/math_based/CEM.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/CGO.py` & `mealpy-2.5.4a6/mealpy/math_based/CGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/CircleSA.py` & `mealpy-2.5.4a6/mealpy/math_based/CircleSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/GBO.py` & `mealpy-2.5.4a6/mealpy/math_based/GBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/HC.py` & `mealpy-2.5.4a6/mealpy/math_based/HC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/INFO.py` & `mealpy-2.5.4a6/mealpy/math_based/INFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/PSS.py` & `mealpy-2.5.4a6/mealpy/math_based/PSS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/RUN.py` & `mealpy-2.5.4a6/mealpy/math_based/RUN.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/SCA.py` & `mealpy-2.5.4a6/mealpy/math_based/SCA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/math_based/SHIO.py` & `mealpy-2.5.4a6/mealpy/math_based/SHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/multitask.py` & `mealpy-2.5.4a6/mealpy/multitask.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/music_based/HS.py` & `mealpy-2.5.4a6/mealpy/music_based/HS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/optimizer.py` & `mealpy-2.5.4a6/mealpy/optimizer.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/ASO.py` & `mealpy-2.5.4a6/mealpy/physics_based/ASO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/ArchOA.py` & `mealpy-2.5.4a6/mealpy/physics_based/ArchOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/CDO.py` & `mealpy-2.5.4a6/mealpy/physics_based/CDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/EFO.py` & `mealpy-2.5.4a6/mealpy/physics_based/EFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/EO.py` & `mealpy-2.5.4a6/mealpy/physics_based/EO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/EVO.py` & `mealpy-2.5.4a6/mealpy/physics_based/EVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/FLA.py` & `mealpy-2.5.4a6/mealpy/physics_based/FLA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/HGSO.py` & `mealpy-2.5.4a6/mealpy/physics_based/HGSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/MVO.py` & `mealpy-2.5.4a6/mealpy/physics_based/MVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/NRO.py` & `mealpy-2.5.4a6/mealpy/physics_based/NRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/RIME.py` & `mealpy-2.5.4a6/mealpy/physics_based/RIME.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/SA.py` & `mealpy-2.5.4a6/mealpy/physics_based/SA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/TWO.py` & `mealpy-2.5.4a6/mealpy/physics_based/TWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/physics_based/WDO.py` & `mealpy-2.5.4a6/mealpy/physics_based/WDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/ABC.py` & `mealpy-2.5.4a6/mealpy/swarm_based/ABC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/ACOR.py` & `mealpy-2.5.4a6/mealpy/swarm_based/ACOR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/AGTO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/AGTO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/ALO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/ALO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/AO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/AO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/ARO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/ARO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/AVOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/AVOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/BA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/BA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/BES.py` & `mealpy-2.5.4a6/mealpy/swarm_based/BES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/BFO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/BFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/BSA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/BSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/BeesA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/BeesA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/COA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/COA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/CSA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/CSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/CSO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/CSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/CoatiOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/CoatiOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/DMOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/DMOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/DO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/DO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/EHO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/EHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/ESOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/ESOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/FA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/FA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/FFA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/FFA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/FFO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/FFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/FOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/FOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/FOX.py` & `mealpy-2.5.4a6/mealpy/swarm_based/FOX.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/GJO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/GJO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/GOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/GOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/GTO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/GTO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/GWO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/GWO.py`

 * *Files 17% similar despite different names*

```diff
@@ -257,7 +257,110 @@
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
+
+
+class IGWO(OriginalGWO):
+    """
+    The original version of: Improved Grey Wolf Optimization (IGWO)
+
+    Notes:
+        1. Link: https://doi.org/10.1007/s00366-017-0567-1
+        2. Implemented by: Mohammadtaher Abbasi (https://github.com/mtabbasi)
+
+    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
+        + a_min (float): Lower bound of a, default = 0.02
+        + a_max (float): Upper bound of a, default = 2.2
+
+    Examples
+    ~~~~~~~~
+    >>> import numpy as np
+    >>> from mealpy.swarm_based.GWO import IGWO
+    >>>
+    >>> def fitness_function(solution):
+    >>>     return np.sum(solution**2)
+    >>>
+    >>> problem_dict1 = {
+    >>>     "fit_func": fitness_function,
+    >>>     "lb": [-10, -15, -4, -2, -8],
+    >>>     "ub": [10, 15, 12, 8, 20],
+    >>>     "minmax": "min",
+    >>> }
+    >>>
+    >>> epoch = 1000
+    >>> pop_size = 50
+    >>> a_min = 0.02
+    >>> a_max = 2.2
+    >>> model = IGWO(epoch, pop_size, a_min, a_max)
+    >>> best_position, best_fitness = model.solve(problem_dict1)
+    >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+
+    References
+    ~~~~~~~~~~
+    [1] Kaveh, A. & Zakian, P.. (2018). Improved GWO algorithm for optimal design of truss structures.
+    Engineering with Computers. 34. 10.1007/s00366-017-0567-1.
+    """
+
+    def __init__(self, epoch=10000, pop_size=100, a_min=0.02, a_max=2.2, **kwargs):
+        """
+        Args:
+            epoch (int): maximum number of iterations, default = 10000
+            pop_size (int): number of population size, default = 100
+            a_min (float): Lower bound of a, default = 0.02
+            a_max (float): Upper bound of a, default = 2.2
+        """
+        super().__init__(epoch, pop_size, **kwargs)
+        self.a_min = self.validator.check_float("a_min", a_min, (0.0, 1.6))
+        self.a_max = self.validator.check_float("a_max", a_max, [1., 4.])
+        self.set_parameters(["epoch", "pop_size", "a_min", "a_max"])
+        self.growth_alpha = 2
+        self.growth_delta = 3
+
+    def evolve(self, epoch):
+        """
+        The main operations (equations) of algorithm.
+
+        Args:
+            epoch (int): The current iteration
+        """
+        _, list_best, _ = self.get_special_solutions(self.pop, best=3)
+
+        pop_new = []
+        for idx in range(0, self.pop_size):
+            # IGWO functions
+            a_alpha = self.a_max * np.exp(
+                (epoch / self.epoch) ** self.growth_alpha
+                * np.log(self.a_min / self.a_max)
+            )
+            a_delta = self.a_max * np.exp(
+                (epoch / self.epoch) ** self.growth_delta
+                * np.log(self.a_min / self.a_max)
+            )
+            a_beta = (a_alpha + a_delta) * 0.5
+            A1 = a_alpha * (2 * np.random.rand(self.problem.n_dims) - 1)
+            A2 = a_beta * (2 * np.random.rand(self.problem.n_dims) - 1)
+            A3 = a_delta * (2 * np.random.rand(self.problem.n_dims) - 1)
+            C1 = 2 * np.random.rand(self.problem.n_dims)
+            C2 = 2 * np.random.rand(self.problem.n_dims)
+            C3 = 2 * np.random.rand(self.problem.n_dims)
+            X1 = list_best[0][self.ID_POS] - A1 * np.abs(
+                C1 * list_best[0][self.ID_POS] - self.pop[idx][self.ID_POS]
+            )
+            X2 = list_best[1][self.ID_POS] - A2 * np.abs(
+                C2 * list_best[1][self.ID_POS] - self.pop[idx][self.ID_POS]
+            )
+            X3 = list_best[2][self.ID_POS] - A3 * np.abs(
+                C3 * list_best[2][self.ID_POS] - self.pop[idx][self.ID_POS]
+            )
+            pos_new = (X1 + X2 + X3) / 3.0
+            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+            pop_new.append([pos_new, None])
+            if self.mode not in self.AVAILABLE_MODES:
+                target = self.get_target_wrapper(pos_new)
+                self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
+        if self.mode in self.AVAILABLE_MODES:
+            pop_new = self.update_target_wrapper_population(pop_new)
+            self.pop = self.greedy_selection_population(self.pop, pop_new)
```

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/HBA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/HBA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/HGS.py` & `mealpy-2.5.4a6/mealpy/swarm_based/HGS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/HHO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/HHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/JA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/JA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/MFO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/MFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/MGO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/MGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/MPA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/MPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/MRFO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/MRFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/MSA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/MSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/NGO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/NGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/NMRA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/NMRA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/OOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/OOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/PFA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/PFA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/POA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/POA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/PSO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/PSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SCSO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SCSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SFO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SHO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SLO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SLO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SRSR.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SRSR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SSA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SSO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SSpiderA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SSpiderA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SSpiderO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SSpiderO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/STO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/STO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/SeaHO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/SeaHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/ServalOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/ServalOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/TDO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/TDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/TSO.py` & `mealpy-2.5.4a6/mealpy/swarm_based/TSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/WOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/WOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/WaOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/WaOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/swarm_based/ZOA.py` & `mealpy-2.5.4a6/mealpy/swarm_based/ZOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/system_based/AEO.py` & `mealpy-2.5.4a6/mealpy/system_based/AEO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/system_based/GCO.py` & `mealpy-2.5.4a6/mealpy/system_based/GCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/system_based/WCA.py` & `mealpy-2.5.4a6/mealpy/system_based/WCA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/tuner.py` & `mealpy-2.5.4a6/mealpy/tuner.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/utils/history.py` & `mealpy-2.5.4a6/mealpy/utils/history.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/utils/io.py` & `mealpy-2.5.4a6/mealpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/utils/logger.py` & `mealpy-2.5.4a6/mealpy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/utils/problem.py` & `mealpy-2.5.4a6/mealpy/utils/problem.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/utils/termination.py` & `mealpy-2.5.4a6/mealpy/utils/termination.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/utils/validator.py` & `mealpy-2.5.4a6/mealpy/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy/utils/visualize/linechart.py` & `mealpy-2.5.4a6/mealpy/utils/visualize/linechart.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/mealpy.egg-info/PKG-INFO` & `mealpy-2.5.4a6/mealpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.4a5
+Version: 2.5.4a6
 Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
@@ -70,15 +70,15 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MEALPY is the largest python library for most of the cutting-edge nature-inspired meta-heuristic algorithms (population-based). Population meta-heuristic algorithms (PMA) are the most popular algorithms in the field of 
 approximate optimization.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total algorithms**: 174 (102 original, 45 official variants, 27 developed variants)
+* **Total algorithms**: 175 (102 original, 46 official variants, 27 developed variants)
 * **Documentation:** https://mealpy.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, pandas, matplotlib
 
 
 # Goals
 
@@ -99,15 +99,15 @@
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
 $ pip install mealpy==2.5.3
 ```
 
 ### Install the alpha/beta version
 ```sh 
-$ pip install mealpy==2.5.4a5
+$ pip install mealpy==2.5.4a6
 ```
 
 ### Install the pre-release version
 You can install pre-release directly from the source code:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
@@ -119,14 +119,17 @@
 
 After installation, you can import Mealpy as any other Python module:
 
 ```sh
 $ python
 >>> import mealpy
 >>> mealpy.__version__
+
+>>> print(mealpy.get_all_optimizers())
+>>> model = mealpy.get_optimizer_by_name("OriginalWOA")(epoch=100, pop_size=50)
 ```
 
 Let's go through a basic and advanced example.
 
 
 ## Examples
 
@@ -403,44 +406,46 @@
 
 * Official source code repo: https://github.com/thieu1995/mealpy
 * Official document: https://mealpy.readthedocs.io/
 * Download releases: https://pypi.org/project/mealpy/
 * Issue tracker: https://github.com/thieu1995/mealpy/issues
 * Notable changes log: https://github.com/thieu1995/mealpy/blob/master/ChangeLog.md
 * Examples with different meapy version: https://github.com/thieu1995/mealpy/blob/master/EXAMPLES.md
+* Official chat/support group: https://t.me/+fRVCJGuGJg1mNDg1
 
 * This project also related to our another projects which are "meta-heuristics" and "neural-network", check it here
     * https://github.com/thieu1995/opfunu
     * https://github.com/thieu1995/metaheuristics
     * https://github.com/aiir-team
-
-**Want to have an instant assistant? Join our telegram community at [link](https://t.me/+fRVCJGuGJg1mNDg1)**
-We share lots of information, questions, and answers there. You will get more support and knowledge there.
+    * https://github.com/mafese
+    * https://github.com/permetrics
 
 ### Cite Us
 
 If you are using mealpy in your project, we would appreciate citations:
 
 ```bibtex 
 @article{van2023mealpy,
   title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
   author={Van Thieu, Nguyen and Mirjalili, Seyedali},
   journal={Journal of Systems Architecture},
   year={2023},
-  publisher={Elsevier}
+  publisher={Elsevier},
+  doi={10.1016/j.sysarc.2023.102871}
 }
 
 @article{van2023groundwater,
   title={Groundwater level modeling using Augmented Artificial Ecosystem Optimization},
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
   pages={129034},
   year={2023},
-  publisher={Elsevier}
+  publisher={Elsevier},
+  doi={10.1016/j.jhydrol.2022.129034}
 }
 ```
 
 
 
 # List of papers used MEALPY
 
@@ -567,14 +572,15 @@
 | Swarm        | -                                               | -          | ModifiedBA       | -        | 5         | medium         |
 | Swarm        | Fruit-fly Optimization Algorithm                | FOA        | OriginalFOA      | 2012     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseFOA          | -        | 2         | easy           |
 | Swarm        | -                                               | -          | WhaleFOA         | 2020     | 2         | medium         |
 | Swarm        | Social Spider Optimization                      | SSpiderO   | OriginalSSpiderO | 2018     | 4         | hard*          |
 | Swarm        | Grey Wolf Optimizer                             | GWO        | OriginalGWO      | 2014     | 2         | easy           |
 | Swarm        | -                                               | -          | RW_GWO           | 2019     | 2         | easy           |
+| Swarm        | -                                               | -          | IGWO             | 2017     | 4         | easy           |
 | Swarm        | Social Spider Algorithm                         | SSpiderA   | OriginalSSpiderA | 2015     | 5         | medium         |
 | Swarm        | Ant Lion Optimizer                              | ALO        | OriginalALO      | 2015     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseALO          | -        | 2         | easy           |
 | Swarm        | Moth Flame Optimization                         | MFO        | OriginalMFO      | 2015     | 2         | easy           |
 | Swarm        | -                                               | -          | BaseMFO          | -        | 2         | easy           |
 | Swarm        | Elephant Herding Optimization                   | EHO        | OriginalEHO      | 2015     | 5         | easy           |
 | Swarm        | Jaya Algorithm                                  | JA         | OriginalJA       | 2016     | 2         | easy           |
@@ -896,14 +902,15 @@
   * **EliteSingleGA**: Elite version of Single-point mutation GA
   * **EliteMultiGA**: Elite version of Multiple-point mutation GA
 
 * **GWO - Grey Wolf Optimizer** 
   * **OriginalGWO**: Mirjalili, S., Mirjalili, S. M., & Lewis, A. (2014). Grey wolf optimizer. Advances in engineering software, 69, 46-61.
   * **RW_GWO**: Gupta, S., & Deep, K. (2019). A novel random walk grey wolf optimizer. Swarm and evolutionary computation, 44, 101-112.
   * **GWO_WOA**: Obadina, O. O., Thaha, M. A., Althoefer, K., & Shaheed, M. H. (2022). Dynamic characterization of a master–slave robotic manipulator using a hybrid grey wolf–whale optimization algorithm. Journal of Vibration and Control, 28(15-16), 1992-2003.
+  * **IGWO**: Kaveh, A. & Zakian, P.. (2018). Improved GWO algorithm for optimal design of truss structures. Engineering with Computers. 34. 10.1007/s00366-017-0567-1.
 
 * **GOA - Grasshopper Optimisation Algorithm** 
   * **OriginalGOA**: Saremi, S., Mirjalili, S., & Lewis, A. (2017). Grasshopper optimisation algorithm: theory and application. Advances in Engineering Software, 105, 30-47.
 
 * **GCO - Germinal Center Optimization** 
   * **OriginalGCO**: Villaseñor, C., Arana-Daniel, N., Alanis, A. Y., López-Franco, C., & Hernandez-Vargas, E. A. (2018). Germinal center optimization algorithm. International Journal of Computational Intelligence Systems, 12(1), 13-27.
   * **BaseGCO**: The developed version
```

### Comparing `mealpy-2.5.4a5/mealpy.egg-info/SOURCES.txt` & `mealpy-2.5.4a6/mealpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 mealpy/evolutionary_based/CRO.py
 mealpy/evolutionary_based/DE.py
 mealpy/evolutionary_based/EP.py
 mealpy/evolutionary_based/ES.py
 mealpy/evolutionary_based/FPA.py
 mealpy/evolutionary_based/GA.py
 mealpy/evolutionary_based/MA.py
+mealpy/evolutionary_based/SHADE.py
 mealpy/evolutionary_based/__init__.py
 mealpy/human_based/BRO.py
 mealpy/human_based/BSO.py
 mealpy/human_based/CA.py
 mealpy/human_based/CHIO.py
 mealpy/human_based/FBIO.py
 mealpy/human_based/GSKA.py
@@ -59,14 +60,15 @@
 mealpy/math_based/GBO.py
 mealpy/math_based/HC.py
 mealpy/math_based/INFO.py
 mealpy/math_based/PSS.py
 mealpy/math_based/RUN.py
 mealpy/math_based/SCA.py
 mealpy/math_based/SHIO.py
+mealpy/math_based/TS.py
 mealpy/math_based/__init__.py
 mealpy/music_based/HS.py
 mealpy/music_based/__init__.py
 mealpy/physics_based/ASO.py
 mealpy/physics_based/ArchOA.py
 mealpy/physics_based/CDO.py
 mealpy/physics_based/EFO.py
```

### Comparing `mealpy-2.5.4a5/setup.py` & `mealpy-2.5.4a6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mealpy",
-    version="2.5.4-alpha.5",
+    version="2.5.4-alpha.6",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["optimization", "metaheuristics", "MHA", "mathematical optimization", "nature-inspired algorithms",
               "evolutionary computation", "soft computing", "population-based algorithms",
```

### Comparing `mealpy-2.5.4a5/tests/test_optimizer.py` & `mealpy-2.5.4a6/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a5/tests/test_tuner.py` & `mealpy-2.5.4a6/tests/test_tuner.py`

 * *Files identical despite different names*

