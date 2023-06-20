# Comparing `tmp/hotpot-zzy-0.3.0.1.tar.gz` & `tmp/hotpot-zzy-0.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zzy/hotpot/dist/.tmp-1p3ukjc0/hotpot-zzy-0.3.0.1.tar", last modified: Tue Jun 20 05:04:05 2023, max compression
+gzip compressed data, was "/home/zzy/hotpot/dist/.tmp-otos8jai/hotpot-zzy-0.3.0.2.tar", last modified: Tue Jun 20 08:29:51 2023, max compression
```

## Comparing `hotpot-zzy-0.3.0.1.tar` & `hotpot-zzy-0.3.0.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/
--rwxrwx---   0 zzy       (1002) zzy       (1002)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/MANIFEST.in
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       56 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/PKG-INFO
--rwxrwx---   0 zzy       (1002) zzy       (1002)     6765 2023-06-14 13:37:58.000000 hotpot-zzy-0.3.0.1/README.md
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      437 2023-06-19 12:37:49.000000 hotpot-zzy-0.3.0.1/hotpot/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)    40667 2023-06-16 06:34:10.000000 hotpot-zzy-0.3.0.1/hotpot/_io.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)    19026 2023-06-16 06:43:48.000000 hotpot-zzy-0.3.0.1/hotpot/bundle.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)   103045 2023-06-19 12:12:28.000000 hotpot-zzy-0.3.0.1/hotpot/cheminfo.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/
--rwxrwx---   0 zzy       (1002) zzy       (1002)       71 2023-06-16 12:44:21.000000 hotpot-zzy-0.3.0.1/hotpot/data/atom_single_point.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/force_field/
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/force_field/UFF/
--rwxrwx---   0 zzy       (1002) zzy       (1002)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.596787 hotpot-zzy-0.3.0.1/hotpot/data/force_field/aMaterials/
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/force_field/aMaterials/SiC.tersoff
--rwxrwx---   0 zzy       (1002) zzy       (1002)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/force_field/contents.json
--rwxrwx---   0 zzy       (1002) zzy       (1002)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/periodic_table.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/data/solvents/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      973 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1068 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      783 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dichloroethene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2586 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1447 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      970 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1731 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1558 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,4-dioxane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-butanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1912 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-pentanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1342 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-propanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-butanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1727 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-ethoxyethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1443 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methoxyethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1636 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1760 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      670 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/DCM.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1335 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMF.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1146 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMSO.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1638 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1756 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1455 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/THF.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      963 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1149 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      774 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetonitrile.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1364 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/benzene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2104 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/butylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      687 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/carbon_tetrachloride.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1370 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/chlorobenzene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      677 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/chloroform.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2218 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/cumene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/cyclohexane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1629 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/diethylether.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2298 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/diisopropylamine.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1054 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyl_formate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1534 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1156 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyleneglycol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      771 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/formamide.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      678 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/formic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2384 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/heptane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2098 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/hexane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2108 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isobutyl_acetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2671 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isooctane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1343 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1823 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2201 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylether.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/meta-xylene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      770 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1751 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methoxybenzene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2014 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylbutylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2229 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylcyclohexane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1444 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylethylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisobutylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1733 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisopropylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1652 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/morpholine.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      869 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/nitromethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1939 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/ortho-xylene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/para-xylene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1814 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/pentane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1820 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/propylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1270 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/pyridine.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1651 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/sulfolane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/t-butylmethylether.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2340 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/tetralin.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1649 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/toluene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/trichloroacetic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      482 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/solvents/water.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/data/units.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/tanks/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     9488 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/cc.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/features.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/base.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     8789 2023-06-14 00:55:16.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/gcmc.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     9577 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/materials.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     8528 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.1/hotpot/tanks/quantum.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tmo.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/tools.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot/utils/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/utils/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1717 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/utils/load_chem_lib.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       56 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     3854 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)        1 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       51 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)        7 2023-06-20 05:04:05.000000 hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/top_level.txt
--rwxrwx---   0 zzy       (1002) zzy       (1002)      314 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.1/pyproject.toml
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       38 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/setup.cfg
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 05:04:05.604787 hotpot-zzy-0.3.0.1/test/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/test/test_amorphous_maker.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1157 2023-06-14 09:02:54.000000 hotpot-zzy-0.3.0.1/test/test_bundle.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2419 2023-06-16 02:14:06.000000 hotpot-zzy-0.3.0.1/test/test_chemif.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.1/test/test_lmp.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/MANIFEST.in
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       56 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/PKG-INFO
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     6765 2023-06-14 13:37:58.000000 hotpot-zzy-0.3.0.2/README.md
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.655512 hotpot-zzy-0.3.0.2/hotpot/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      437 2023-06-19 12:37:49.000000 hotpot-zzy-0.3.0.2/hotpot/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)    40740 2023-06-20 08:25:13.000000 hotpot-zzy-0.3.0.2/hotpot/_io.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)    19026 2023-06-16 06:43:48.000000 hotpot-zzy-0.3.0.2/hotpot/bundle.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)   105362 2023-06-20 08:15:55.000000 hotpot-zzy-0.3.0.2/hotpot/cheminfo.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.655512 hotpot-zzy-0.3.0.2/hotpot/data/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)       71 2023-06-16 12:44:21.000000 hotpot-zzy-0.3.0.2/hotpot/data/atom_single_point.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.655512 hotpot-zzy-0.3.0.2/hotpot/data/force_field/
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.655512 hotpot-zzy-0.3.0.2/hotpot/data/force_field/UFF/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.655512 hotpot-zzy-0.3.0.2/hotpot/data/force_field/aMaterials/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rwxrwx---   0 zzy       (1002) zzy       (1002)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/force_field/contents.json
+-rwxrwx---   0 zzy       (1002) zzy       (1002)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/hotpot/data/solvents/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      973 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1068 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      783 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2586 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1447 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      970 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1731 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1558 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,4-dioxane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1-butanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1912 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1-pentanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1342 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/1-propanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-butanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1727 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1443 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-methoxyethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1636 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1760 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      670 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/DCM.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1335 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/DMF.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1146 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/DMSO.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1638 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1756 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1455 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/THF.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      963 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/acetic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1149 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/acetone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      774 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/acetonitrile.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1364 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/benzene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2104 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/butylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      687 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1370 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/chlorobenzene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      677 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/chloroform.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2218 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/cumene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/cyclohexane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1629 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/diethylether.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2298 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/diisopropylamine.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1054 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethyl_formate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1534 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1156 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethyleneglycol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      771 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/formamide.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      678 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/formic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2384 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/heptane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2098 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/hexane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2108 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/isobutyl_acetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2671 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/isooctane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1343 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/isopropanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1823 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/isopropylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2201 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/isopropylether.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/meta-xylene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      770 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methanol.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1751 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methoxybenzene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2014 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylbutylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2229 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylcyclohexane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1444 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylethylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylisobutylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1733 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylisopropylketone.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1652 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/morpholine.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      869 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/nitromethane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1939 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/ortho-xylene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/para-xylene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1814 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/pentane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1820 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/propylacetate.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1270 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/pyridine.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1651 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/sulfolane.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/t-butylmethylether.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2340 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/tetralin.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1649 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/toluene.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      482 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/solvents/water.mol2
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/data/units.json
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/hotpot/tanks/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     9488 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/cc.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/features.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/base.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     8789 2023-06-14 00:55:16.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/gcmc.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     9577 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/materials.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     8528 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.2/hotpot/tanks/quantum.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/tmo.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/tools.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/hotpot/utils/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/utils/__init__.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1717 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/utils/load_chem_lib.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       56 2023-06-20 08:29:51.000000 hotpot-zzy-0.3.0.2/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)     3854 2023-06-20 08:29:51.000000 hotpot-zzy-0.3.0.2/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)        1 2023-06-20 08:29:51.000000 hotpot-zzy-0.3.0.2/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       51 2023-06-20 08:29:51.000000 hotpot-zzy-0.3.0.2/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)        7 2023-06-20 08:29:51.000000 hotpot-zzy-0.3.0.2/hotpot_zzy.egg-info/top_level.txt
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      314 2023-06-20 08:20:28.000000 hotpot-zzy-0.3.0.2/pyproject.toml
+-rw-rw-r--   0 zzy       (1002) zzy       (1002)       38 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/setup.cfg
+drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 08:29:51.663512 hotpot-zzy-0.3.0.2/test/
+-rwxrwx---   0 zzy       (1002) zzy       (1002)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/test/test_amorphous_maker.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     1157 2023-06-14 09:02:54.000000 hotpot-zzy-0.3.0.2/test/test_bundle.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     2419 2023-06-16 02:14:06.000000 hotpot-zzy-0.3.0.2/test/test_chemif.py
+-rwxrwx---   0 zzy       (1002) zzy       (1002)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.2/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.3.0.1/README.md` & `hotpot-zzy-0.3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/_io.py` & `hotpot-zzy-0.3.0.2/hotpot/_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,14 +431,16 @@
 
         if self.src.crystal().space_group:
             self.src.crystal().space_group = 'P1'
 
     def _pre_gjf(self):
         """ Assign the Molecule charge before to dump to gjf file """
         self.src.determine_mol_charge()
+        if not self.src.has_3d:
+            self.src.build_conformer()
 
     def _io_dpmd_sys(self):
         """ convert molecule information to numpy arrays """
         required_items = ['coord', 'type']
         check_atom_num = ['coord', 'force', 'charge']
         share_same_configures = ['type', 'coord', 'energy', 'force', 'charge', 'virial']
         need_reshape = ['coord', 'force']
```

### Comparing `hotpot-zzy-0.3.0.1/hotpot/bundle.py` & `hotpot-zzy-0.3.0.2/hotpot/bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/cheminfo.py` & `hotpot-zzy-0.3.0.2/hotpot/cheminfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,24 @@
 
 
 class AddBondFail(OperateOBMolFail):
     """ Raise when add a bond into Molecule fail """
 
 
 periodic_table = json.load(open(ptj(data_root, 'periodic_table.json'), encoding='utf-8'))
-# periodic_table = {d['symbol']: d for d in periodic_table}
 _symbols = ['unknown'] + list(periodic_table.keys())
 _max_valences = {n: v['max_valence'] for n, v in periodic_table.items()}
 _max_total_bond_order = {n: v['max_total_bond_order'] for n, v in periodic_table.items()}
 
 _stable_charges = {
     'H': 1, 'He': 0,
     'Li': 1, 'Be': 2,
     'Na': 1, 'Mg': 2,
-    'K': 1, 'Ca': 2,
-    'Rb': 1, 'Sr': 2,
+    'K': 1, 'Ca': 2, 'Sc': 3, 'Ti': 4,
+    'Rb': 1, 'Sr': 2, '?': '', 'Zr': 4,
     'Cs': 1, 'Ba': 2
 }
 
 _bond_type = {
     'Unknown': 0,
     'Single': 1,
     'Double': 2,
@@ -500,14 +499,31 @@
 
         return self
 
     @property
     def _protected_data(self):
         return 'ob_obj', 'atoms', 'bonds', 'angles'
 
+    def _reorder_atom_ob_id(self):
+        """ Reorder the ob id of atoms """
+        new_atom_dict = {}
+        for ob_id, atom in enumerate(self.atoms):
+            atom.ob_atom.SetId(ob_id)
+            new_atom_dict[ob_id] = atom
+
+        self._data['atoms'] = new_atom_dict
+
+    def _reorder_bond_ob_id(self):
+        new_atom_dict = {}
+        for ob_id, bond in enumerate(self.bonds):
+            bond.ob_bond.SetId(ob_id)
+            new_atom_dict[ob_id] = bond
+
+        self._data['bonds'] = new_atom_dict
+
     def _reorganize_atom_indices(self):
         """ reorganize or rearrange the indices for all atoms """
         for i, ob_atom in enumerate(ob.OBMolAtomIter(self.ob_mol)):
             ob_atom.SetId(i)
 
     def _set_atoms(self, atoms_kwargs: List[Dict[str, Any]]):
         """ add a list of atoms by a list atoms attributes dict """
@@ -667,15 +683,15 @@
     def _set_spin_multiplicity(self, spin):
         self.ob_mol.SetTotalSpinMultiplicity(spin)
 
     @property
     def acentric_factor(self):
         return self._get_critical_params('acentric_factor')
 
-    def add_atom(self, atom: Union["Atom", str, int], **atom_kwargs):
+    def add_atom(self, atom: Union["Atom", str, int], **atom_attrs):
         """
         Add a new atom out of the molecule into the molecule.
         Args:
             atom(Atom|str|int):
 
         atom_kwargs(kwargs for this added atom):
             atomic_number(int): set atomic number
@@ -685,17 +701,17 @@
             label:
             spin_density:
 
         Returns:
             the copy of atom in the molecule
         """
         if isinstance(atom, str):
-            atom = Atom(symbol=atom, **atom_kwargs)
+            atom = Atom(symbol=atom, **atom_attrs)
         elif isinstance(atom, int):
-            atom = Atom(atomic_number=atom, **atom_kwargs)
+            atom = Atom(atomic_number=atom, **atom_attrs)
         elif isinstance(atom, Atom):
             data = atom.data  # copy the atom's data dict
 
             data.pop('ob_obj')  # delete the ob_atom item in data dict
             if data.get('mol'):
                 data.pop('mol')  # delete the _mol item in data dict
 
@@ -759,16 +775,16 @@
         # the `Id` of `OBAtom` from 0; but the `Idx` of `OBAtom` from 1.
         # To meet the convention, the `Id` is selected to be the unique `index` to specify `Atom`.
         # However, when try to add a `OBBond` to link each two `OBAtoms`, the `Idx` is the only method
         # to specify the atoms, so our `index` in `Atom` are added 1 to match the 'Idx'
         success = self.ob_mol.AddBond(atoms[0].ob_idx, atoms[1].ob_idx, bond_type)
 
         if success:
-            new_ob_bond_idx = [obb for obb in (ob.OBMolBondIter(self.ob_mol))][-1].GetIdx()
-            bond = self._load_bonds()[new_ob_bond_idx]  # the new atoms should place in the terminal of the bond list
+            new_bond_ob_id = [obb for obb in (ob.OBMolBondIter(self.ob_mol))][-1].GetId()
+            bond = self._load_bonds()[new_bond_ob_id]  # the new atoms should place in the terminal of the bond list
 
         elif atoms[0].ob_id not in self.atom_indices:
             raise KeyError("the start atom1 doesn't exist in molecule")
 
         elif atoms[1].ob_id not in self.atom_indices:
             raise KeyError("the end atom2 doesn't exist in molecule")
 
@@ -783,14 +799,17 @@
         add hydrogens for the molecule
         Args:
             ph: add hydrogen in which PH environment
             polar_only: Whether to add hydrogens only to polar atoms (i.e., not to C atoms)
             correct_for_ph: Correct for pH by applying the OpenBabel::OBPhModel transformations
         """
         self.ob_mol.AddHydrogens(polar_only, correct_for_ph, ph)
+        # TODO: Beta, test feature
+        for atom in self.atoms:
+            atom.remove_redundant_hydrogen()
 
     def add_pseudo_atom(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
         """ Add pseudo atom into the molecule """
         list_pseudo_atom = self._data.setdefault('pseudo_atoms', [])
         pa = PseudoAtom(symbol, mass, coordinates, mol=self, molecule=self, **kwargs)
         list_pseudo_atom.append(pa)
 
@@ -1044,14 +1063,17 @@
         where the row index point to the atom index;
         the column index point to the (x, y, z)
         """
         return np.array([atom.coordinates for atom in self.atoms], dtype=np.float64)
 
     def copy(self) -> 'Molecule':
         """ Get a clone of this Molecule """
+        self._reorder_atom_ob_id()
+        self._reorder_bond_ob_id()
+
         clone = Molecule(self.ob_copy())
         clone._load_atoms()
         clone._load_bonds()
 
         # Copy the Molecule's attr data to the clone one
         clone.update_attr_data(self.data)
         # Copy the Atoms' attr data to the clone ones
@@ -1335,24 +1357,26 @@
         from tanks.lmp.gcmc import LjGCMC
         gcmc = LjGCMC(self, force_field, *guest, work_dir=work_dir, T=T, P=P, **kwargs)
         return gcmc.run()
 
     def generate_metal_ligand_pair(
             self, metal_symbol: str,
             acceptor_atoms: Sequence = ('O',),
-            opti_force_field: str = 'UFF'
+            opti_force_field: str = 'UFF',
+            assign_metal_charge: bool = False
     ) -> Generator['Molecule', None, None]:
         """
         This method could work if the molecule is an organic ligand, or raise AttributeError.
         Generate metal-ligand pair by link metal with acceptor atoms in the organic ligand.
 
         Args:
             metal_symbol: which metal element link to the ligand
             acceptor_atoms: which elements to be acceptor atom to link to metal
             opti_force_field: which force field could be used to optimize the configuration of ligand and M-L pair.
+            assign_metal_charge: whether to assign the stable charge to metal cation
 
         Return:
             A generator for M-L pair
         """
         ligand = self.copy()
         for atom in ligand.atoms:
             if atom.symbol in acceptor_atoms:
@@ -1365,53 +1389,67 @@
                 # assign the initial coordinates, if the pair has 3d conformer
                 # the sum of vector of relative position relate to the accepting atom
                 if pair.has_3d:
                     sum_relative_coordinates = sum([c for _, c in acc_atom.neighbours_position])
                     metal_init_coordinates = acc_atom.coordinates_array - sum_relative_coordinates
 
                     # add metal atom into the acceptor_ligand
-                    added_metal = pair.add_atom(metal_symbol, coordinates=metal_init_coordinates)
+                    added_metal = pair.add_atom(
+                        metal_symbol,
+                        coordinates=metal_init_coordinates,
+                        formal_charge=_stable_charges[metal_symbol] if assign_metal_charge else 0
+                    )
 
                 else:  # If the pair has not 3d conformer, add the metal directly
-                    added_metal = pair.add_atom(metal_symbol)
+                    added_metal = pair.add_atom(
+                        metal_symbol,
+                        formal_charge=_stable_charges[metal_symbol] if assign_metal_charge else 0
+                    )
 
                 # add the coordinating bond between metal atom and acceptor atoms
                 pair.add_bond(added_metal, acc_atom, 1)
 
-                # remove redundant hydrogen
-                while acc_atom.valence > acc_atom.valence_max and acc_atom.neighbours_hydrogen:
-                    pair.remove_atoms(acc_atom.neighbours_hydrogen[0], remove_hydrogens=True)
+                # Add hydrogens
+                pair.add_hydrogens()
 
                 # localize optimization of M-L pair by classical force field, if the pair has 3d
                 if pair.has_3d:
                     pair.localed_optimize(opti_force_field)
 
                 pair.identifier = pair.smiles
-
                 yield pair
 
     def generate_pairs_bundle(
-            self, metal_symbol: str, acceptor_atoms: Sequence = ('O',), opti_force_field: str = 'UFF'
+            self, metal_symbol: str,
+            acceptor_atoms: Sequence = ('O',),
+            opti_force_field: str = 'UFF',
+            assign_metal_charge: bool = False
     ) -> 'PairBundle':
         """
         Generate metal-ligand pairs by bind this ligand with proposed, and put this ligand, metal and all pairs,
         which are assembled by the ligand and metal, into a PairBundle objects.
         Args:
             metal_symbol(str): the symbol of proposed metal
             acceptor_atoms(Sequence): the atoms to form bond with the proposed metal, the default is Oxygen
             opti_force_field(str): the force field to optimize the conformer of this ligand and the generated
              pairs.
+            assign_metal_charge: whether to assign stable charge for metal cation
 
         Returns:
             PairBundle with this ligand, proposed metal and the pairs
         """
         return PairBundle(
             metal=Atom(symbol=metal_symbol),
             ligand=self,
-            pairs=list(self.generate_metal_ligand_pair(metal_symbol, acceptor_atoms, opti_force_field))
+            pairs=list(self.generate_metal_ligand_pair(
+                metal_symbol,
+                acceptor_atoms,
+                opti_force_field,
+                assign_metal_charge
+            )),
         )
 
     def graph_representation(self, *feature_names):
         return self.identifier, self.feature_matrix(*feature_names), self.link_matrix
 
     @property
     def has_3d(self):
@@ -1493,24 +1531,24 @@
             raise TypeError('the ob_mol should be OBMol object')
 
         atoms = self._data.get('atoms')
         bonds = self._data.get('bonds')
 
         if any(oba.GetId() not in atoms for oba in ob.OBMolAtomIter(ob_mol)):
             raise ValueError('the atom number between the wrapper and the core OBMol is not match')
-        if any(obb.GetIdx() not in bonds for obb in ob.OBMolBondIter(ob_mol)):
+        if any(obb.GetId() not in bonds for obb in ob.OBMolBondIter(ob_mol)):
             raise ValueError('the bond number between the wrapper and the core OBMol is not match')
 
         self._data['ob_obj'] = ob_mol
         for ob_atom in ob.OBMolAtomIter(ob_mol):
             atom = atoms.get(ob_atom.GetId())
             atom.ob_atom_rewrap(ob_atom)
 
         for ob_bond in ob.OBMolBondIter(ob_mol):
-            bond = bonds.get(ob_bond.GetIdx())
+            bond = bonds.get(ob_bond.GetId())
             bond.ob_bond_rewrap(ob_bond)
 
     @property
     def labels(self):
         return [a.label for a in self.atoms]
 
     @property
@@ -2094,14 +2132,15 @@
         return {
             '_mol': self._set_molecule,
             'mol': self._set_molecule,
             'molecule': self._set_molecule,
             'atomic_number': self._set_atomic_number,
             'symbol': self._set_atomic_symbol,
             'coordinates': self._set_coordinate,
+            'formal_charge': self._set_formal_charge,
             'partial_charge': self._set_partial_charge,
             'label': self._set_label,
             'ob_id': self._set_ob_id,
             'spin_density': self._set_spin_density
         }
 
     def _set_atomic_number(self, atomic_number: int):
@@ -2123,14 +2162,17 @@
         elif isinstance(force_vector, np.ndarray):
             force_vector = force_vector.flatten()
         else:
             raise TypeError('the force vector should be Sequence or np.ndarray')
 
         self._data['force_vector'] = force_vector
 
+    def _set_formal_charge(self, charge: float):
+        self.ob_atom.SetFormalCharge(charge)
+
     def _set_ob_id(self, ob_id):
         self.ob_atom.SetId(ob_id)
 
     def _set_label(self, label):
         label_data = ob.OBCommentData()
 
         label_data.SetAttribute('label')
@@ -2148,22 +2190,31 @@
         self._data['spin_density'] = spin_density
 
     @property
     def atom_type(self):
         """ Some atom have specific type, such as Carbon with sp1, sp2 and sp3, marked as C1, C2 and C3 """
         return self.ob_atom.GetType()
 
+    def add_atom(self, symbol: str, bond_type=1, **atom_attrs):
+        """ add atom to link with this atom """
+        new_atom = self.molecule.add_atom(symbol, **atom_attrs)
+        self.molecule.add_bond(self, new_atom, bond_type)
+
     @property
     def atomic_number(self):
         return self.ob_atom.GetAtomicNum()
 
     @property
+    def bond_valence(self) -> int:
+        return sum(b.type for b in self.bonds)
+
+    @property
     def bonds(self):
         """ Get all bonds link with the atoms """
-        return [self.molecule.bonds_dict[obb.GetIdx()] for obb in ob.OBAtomBondIter(self.ob_atom)]
+        return [self.molecule.bonds_dict[obb.GetId()] for obb in ob.OBAtomBondIter(self.ob_atom)]
 
     @property
     def coordinates(self) -> (float, float, float):
         return self.ob_atom.GetX(), self.ob_atom.GetY(), self.ob_atom.GetZ()
 
     @coordinates.setter
     def coordinates(self, value):
@@ -2377,14 +2428,24 @@
         for neigh_atom in self.neighbours:
             yield neigh_atom, neigh_atom.coordinates_array - self.coordinates_array
 
     @property
     def partial_charge(self):
         return self.ob_atom.GetPartialCharge()
 
+    def remove_redundant_hydrogen(self):
+        """ Remove hydrogens link with this atom, if the bond valence is more than the max allowed valence"""
+        if self.is_hydrogen:
+            return None
+
+        # remove redundant hydrogen
+        while self.bond_valence > abs(self.valence_max) and self.neighbours_hydrogen:
+            self.molecule.remove_atoms(self.neighbours_hydrogen[0])
+            self.formal_charge += self.formal_charge - 1
+
     @partial_charge.setter
     def partial_charge(self, value: float):
         # This is necessary to take effect to the assignment.
         # the reason is unknown
         self.ob_atom.GetPartialCharge()
         self._set_partial_charge(value)
 
@@ -2416,24 +2477,28 @@
         return self._data.get('spin_density', 0.0)
 
     @spin_density.setter
     def spin_density(self, spin_density: float):
         self._set_spin_density(spin_density)
 
     @property
-    def symbol(self):
+    def stable_valence(self) -> int:
+        return _stable_charges.get(self.symbol, None)
+
+    @property
+    def symbol(self) -> str:
         return _symbols[self.atomic_number]
 
     @property
     def valence(self) -> int:
         """ The current number of explicit connections """
         return self.ob_atom.GetTotalValence()
 
     @property
-    def valence_max(self):
+    def valence_max(self) -> int:
         """ The implicit valence of this atom type (i.e. maximum number of connections expected) """
         return _max_valences[self.symbol]
 
 
 class PseudoAtom(Wrapper, ABC):
     """ A data wrapper for pseudo atom """
```

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.0.2/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.0.2/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.0.2/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.0.2/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/tanks/cc.py` & `hotpot-zzy-0.3.0.2/hotpot/tanks/cc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.0.2/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/tanks/quantum.py` & `hotpot-zzy-0.3.0.2/hotpot/tanks/quantum.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/tmo.py` & `hotpot-zzy-0.3.0.2/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/tools.py` & `hotpot-zzy-0.3.0.2/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/utils/load_chem_lib.py` & `hotpot-zzy-0.3.0.2/hotpot/utils/load_chem_lib.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.0.2/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.3.0.2/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/test/test_amorphous_maker.py` & `hotpot-zzy-0.3.0.2/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/test/test_bundle.py` & `hotpot-zzy-0.3.0.2/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/test/test_chemif.py` & `hotpot-zzy-0.3.0.2/test/test_chemif.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.1/test/test_lmp.py` & `hotpot-zzy-0.3.0.2/test/test_lmp.py`

 * *Files identical despite different names*

