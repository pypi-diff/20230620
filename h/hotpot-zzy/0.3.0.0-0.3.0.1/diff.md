# Comparing `tmp/hotpot-zzy-0.3.0.0.tar.gz` & `tmp/hotpot-zzy-0.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-_8xl5tum/hotpot-zzy-0.3.0.0.tar", last modified: Mon Jun 19 12:52:24 2023, max compression
+gzip compressed data, was "/home/zzy/hotpot/dist/.tmp-1p3ukjc0/hotpot-zzy-0.3.0.1.tar", last modified: Tue Jun 20 05:04:05 2023, max compression
```

## Comparing `hotpot-zzy-0.3.0.0.tar` & `hotpot-zzy-0.3.0.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/
--rwxrwx---   0 zz1       (1005) zz1       (1008)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/MANIFEST.in
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       56 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/PKG-INFO
--rwxrwx---   0 zz1       (1005) zz1       (1008)     6765 2023-06-14 13:37:58.000000 hotpot-zzy-0.3.0.0/README.md
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/
--rwxrwx---   0 zz1       (1005) zz1       (1008)      437 2023-06-19 12:37:49.000000 hotpot-zzy-0.3.0.0/hotpot/__init__.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)    40667 2023-06-16 06:34:10.000000 hotpot-zzy-0.3.0.0/hotpot/_io.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)    19026 2023-06-16 06:43:48.000000 hotpot-zzy-0.3.0.0/hotpot/bundle.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)   103045 2023-06-19 12:12:28.000000 hotpot-zzy-0.3.0.0/hotpot/cheminfo.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/
--rwxrwx---   0 zz1       (1005) zz1       (1008)       71 2023-06-16 12:44:21.000000 hotpot-zzy-0.3.0.0/hotpot/data/atom_single_point.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/force_field/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/force_field/UFF/
--rwxrwx---   0 zz1       (1005) zz1       (1008)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/force_field/aMaterials/
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/force_field/aMaterials/SiC.tersoff
--rwxrwx---   0 zz1       (1005) zz1       (1008)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/force_field/contents.json
--rwxrwx---   0 zz1       (1005) zz1       (1008)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/periodic_table.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.150557 hotpot-zzy-0.3.0.0/hotpot/data/solvents/
--rwxrwx---   0 zz1       (1005) zz1       (1008)      973 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1068 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      783 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dichloroethene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2586 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1447 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      970 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1731 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1558 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,4-dioxane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-butanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1912 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-pentanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1342 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-propanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-butanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1727 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-ethoxyethanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1443 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methoxyethanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1636 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1760 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      670 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/DCM.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1335 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMF.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1146 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMSO.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1638 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1756 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1455 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/THF.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      963 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetic_acid.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1149 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetone.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      774 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetonitrile.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1364 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/benzene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2104 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/butylacetate.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      687 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/carbon_tetrachloride.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1370 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/chlorobenzene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      677 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/chloroform.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2218 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/cumene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/cyclohexane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1629 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/diethylether.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2298 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/diisopropylamine.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1054 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyl_formate.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1534 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethylacetate.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1156 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyleneglycol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      771 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/formamide.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      678 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/formic_acid.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2384 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/heptane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2098 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/hexane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2108 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isobutyl_acetate.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2671 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isooctane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1343 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1823 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylacetate.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2201 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylether.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/meta-xylene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      770 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methanol.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1751 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methoxybenzene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylacetate.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2014 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylbutylketone.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2229 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylcyclohexane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1444 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylethylketone.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisobutylketone.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1733 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisopropylketone.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1652 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/morpholine.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      869 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/nitromethane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1939 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ortho-xylene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/para-xylene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1814 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/pentane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1820 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/propylacetate.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1270 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/pyridine.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1651 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/sulfolane.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/t-butylmethylether.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2340 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/tetralin.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1649 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/toluene.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/trichloroacetic_acid.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      482 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/water.mol2
--rwxrwx---   0 zz1       (1005) zz1       (1008)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/units.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot/tanks/
--rwxrwx---   0 zz1       (1005) zz1       (1008)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/__init__.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     9486 2023-06-19 11:51:27.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/cc.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/features.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/
--rwxrwx---   0 zz1       (1005) zz1       (1008)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/__init__.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/base.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     8789 2023-06-14 00:55:16.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/gcmc.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     9577 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/materials.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     8286 2023-06-19 12:05:14.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/quantum.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tmo.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tools.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot/utils/
--rwxrwx---   0 zz1       (1005) zz1       (1008)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/utils/__init__.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1717 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/utils/load_chem_lib.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       56 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3854 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       51 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/top_level.txt
--rwxrwx---   0 zz1       (1005) zz1       (1008)      314 2023-06-19 12:51:44.000000 hotpot-zzy-0.3.0.0/pyproject.toml
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/setup.cfg
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/test/
--rwxrwx---   0 zz1       (1005) zz1       (1008)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/test/test_amorphous_maker.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     1157 2023-06-14 09:02:54.000000 hotpot-zzy-0.3.0.0/test/test_bundle.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     2419 2023-06-16 02:14:06.000000 hotpot-zzy-0.3.0.0/test/test_chemif.py
--rwxrwx---   0 zz1       (1005) zz1       (1008)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/test/test_lmp.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/MANIFEST.in
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       56 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/PKG-INFO
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     6765 2023-06-14 13:37:58.000000 hotpot-zzy-0.3.0.1/README.md
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      437 2023-06-19 12:37:49.000000 hotpot-zzy-0.3.0.1/hotpot/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)    40667 2023-06-16 06:34:10.000000 hotpot-zzy-0.3.0.1/hotpot/_io.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)    19026 2023-06-16 06:43:48.000000 hotpot-zzy-0.3.0.1/hotpot/bundle.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)   103045 2023-06-19 12:12:28.000000 hotpot-zzy-0.3.0.1/hotpot/cheminfo.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)       71 2023-06-16 12:44:21.000000 hotpot-zzy-0.3.0.1/hotpot/data/atom_single_point.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/force_field/
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/force_field/UFF/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/force_field/aMaterials/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rwxrwx---   0 zzy       (1002) zzy       (1002)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/force_field/contents.json
+-rwxrwx---   0 zzy       (1002) zzy       (1002)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/data/solvents/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      973 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1068 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      783 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2586 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1447 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      970 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1731 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1558 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,4-dioxane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-butanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1912 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-pentanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1342 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-propanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-butanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1727 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1443 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methoxyethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1636 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1760 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      670 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/DCM.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1335 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMF.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1146 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMSO.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1638 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1756 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1455 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/THF.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      963 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1149 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      774 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetonitrile.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1364 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/benzene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2104 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/butylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      687 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1370 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/chlorobenzene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      677 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/chloroform.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2218 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/cumene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/cyclohexane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1629 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/diethylether.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2298 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/diisopropylamine.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1054 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyl_formate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1534 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1156 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyleneglycol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      771 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/formamide.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      678 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/formic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2384 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/heptane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2098 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/hexane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2108 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isobutyl_acetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2671 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isooctane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1343 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1823 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2201 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylether.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/meta-xylene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      770 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1751 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methoxybenzene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2014 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylbutylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2229 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylcyclohexane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1444 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylethylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisobutylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1733 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisopropylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1652 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/morpholine.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      869 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/nitromethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1939 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ortho-xylene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/para-xylene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1814 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/pentane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1820 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/propylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1270 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/pyridine.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1651 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/sulfolane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/t-butylmethylether.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2340 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/tetralin.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1649 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/toluene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      482 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/water.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/units.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/tanks/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     9488 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/cc.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/features.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/base.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     8789 2023-06-14 00:55:16.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/gcmc.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     9577 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/materials.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     8528 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/quantum.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tmo.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tools.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/utils/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/utils/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1717 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/utils/load_chem_lib.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       56 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)     3854 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)        1 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       51 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)        7 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/top_level.txt
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      314 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.1/pyproject.toml
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       38 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/setup.cfg
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/test/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/test/test_amorphous_maker.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1157 2023-06-14 09:02:54.000000 hotpot-zzy-0.3.0.1/test/test_bundle.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2419 2023-06-16 02:14:06.000000 hotpot-zzy-0.3.0.1/test/test_chemif.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.3.0.0/README.md` & `hotpot-zzy-0.3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/_io.py` & `hotpot-zzy-0.3.0.1/hotpot/_io.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/bundle.py` & `hotpot-zzy-0.3.0.1/hotpot/bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/cheminfo.py` & `hotpot-zzy-0.3.0.1/hotpot/cheminfo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.0.1/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.0.1/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.0.1/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.0.1/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/tanks/cc.py` & `hotpot-zzy-0.3.0.1/hotpot/tanks/cc.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         # Energy sheet, bond dissociation energy (BDE) sheet
         e_sheet, bde_sheet = [], []
 
         # optimize the configure of ligand and calculate their total energy after optimization
         self.ligand.gaussian(
             g16root,
             link0=f'CPU=0-{os.cpu_count()-1}',
-            route=f'opt {method}/{basis_set}' + route,
+            route=f'opt {method}/{basis_set} ' + route,
             path_log_file=dirs_files.ligand_log_path,
             path_err_file=dirs_files.ligand_err_path,
             inplace_attrs=True
         )
 
         ligand_energy = self.ligand.energy  # Retrieve the energy after optimizing the conformer
         e_sheet.append(['ligand', self.ligand.smiles, ligand_energy])
@@ -166,15 +166,15 @@
         # Calculate the single point (sp) energy for metal
         try:
             metal_sp = _atom_single_point[self.metal.atoms[0].symbol][method][basis_set]
         except KeyError:
             self.metal.gaussian(
                 g16root,
                 link0=f'CPU=0-{os.cpu_count()-1}',
-                route=f'{method}/{basis_set}' + route,
+                route=f'{method}/{basis_set} ' + route,
                 path_log_file=dirs_files.metal_log_path,
                 path_err_file=dirs_files.ligand_err_path,
                 inplace_attrs=True
             )
 
             ele_dict = _atom_single_point.setdefault(self.metal.atoms[0].symbol, {})
             ele_method_dict = ele_dict.setdefault(method, {})
```

### Comparing `hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/tanks/quantum.py` & `hotpot-zzy-0.3.0.1/hotpot/tanks/quantum.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 import resource
 import subprocess
 import io
 import cclib
 from typing import *
 
 
+class GaussianRunError(BaseException):
+    """ Raise when the encounter error in run gaussian """
+
+
 class Gaussian:
     """
     A class for setting up and running Gaussian 16 calculations.
 
     Attributes:
         g16root (str): The path to the Gaussian 16 root directory.
 
@@ -173,14 +177,19 @@
         self.g16process = subprocess.Popen(
             'g16', bufsize=-1, stdin=subprocess.PIPE,
             stdout=subprocess.PIPE, stderr=subprocess.PIPE,
             env=self.envs, universal_newlines=True
         )
         stdout, stderr = self.g16process.communicate(script)
 
+        # Raise error if got standard error message
+        if stderr:
+            print(stderr)
+            raise GaussianRunError
+
         self.parse_log(stdout)
 
         return stdout, stderr
 
     def parse_log(self, stdout: str):
         """ Parse the gaussian log file and save them into self """
         string_buffer = io.StringIO(stdout)
```

### Comparing `hotpot-zzy-0.3.0.0/hotpot/tmo.py` & `hotpot-zzy-0.3.0.1/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/tools.py` & `hotpot-zzy-0.3.0.1/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/utils/load_chem_lib.py` & `hotpot-zzy-0.3.0.1/hotpot/utils/load_chem_lib.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.0.1/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/test/test_amorphous_maker.py` & `hotpot-zzy-0.3.0.1/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/test/test_bundle.py` & `hotpot-zzy-0.3.0.1/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/test/test_chemif.py` & `hotpot-zzy-0.3.0.1/test/test_chemif.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.0/test/test_lmp.py` & `hotpot-zzy-0.3.0.1/test/test_lmp.py`

 * *Files identical despite different names*

