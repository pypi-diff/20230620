# Comparing `tmp/pyxtal-0.5.6.tar.gz` & `tmp/pyxtal-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/.tmp-ad4xrg8r/pyxtal-0.5.6.tar", last modified: Fri Jun  9 17:12:42 2023, max compression
+gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/.tmp-hw7pnauu/pyxtal-0.5.7.tar", last modified: Tue Jun 20 14:43:17 2023, max compression
```

## Comparing `pyxtal-0.5.6.tar` & `pyxtal-0.5.7.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.6/LICENSE.txt
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       82 2022-06-15 16:30:37.000000 pyxtal-0.5.6/MANIFEST.in
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-09 17:12:42.000000 pyxtal-0.5.6/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.6/README.md
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.6/pyxtal/XRD.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   100907 2023-06-09 15:11:50.000000 pyxtal-0.5.6/pyxtal/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.6/pyxtal/block_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.6/pyxtal/constants.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2022-06-21 13:41:23.000000 pyxtal-0.5.6/pyxtal/crystal.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/database/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.6/pyxtal/database/HM_Full.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/atomic_scattering_params.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.6/pyxtal/database/bonds.json
--rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.6/pyxtal/database/bug.json
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/database/cifs/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.6/pyxtal/database/cifs/0-G62.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.6/pyxtal/database/cifs/1-G59.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/191.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.6/pyxtal/database/cifs/2-G71.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.6/pyxtal/database/cifs/3-G139.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.6/pyxtal/database/cifs/4-G225.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/ACBNZA01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/AXOSOW01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/BTO-Amm2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/BTO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.6/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.6/pyxtal/database/cifs/FAU.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/Fd3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.6/pyxtal/database/cifs/Fd3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.6/pyxtal/database/cifs/Fd3m.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/GUMMUW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/GeF2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/HAHCOI.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.6/pyxtal/database/cifs/I41amd.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/I4_132.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/JAPWIH.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/LAGNAL.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/LUFHAW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/LiCs.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/MERQIM.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/MPWO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NaCl.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NaSb3F10.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NbO2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/NiS-Cm.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/P3_112.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/P4_332.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.6/pyxtal/database/cifs/P4nmm.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/P6_422.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/PAHYON01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/PPO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/PVO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pm3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pmmn.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pn3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.6/pyxtal/database/cifs/Pn3m.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/R-3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/R-3c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/cifs/R32.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/TMPPIO03.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/WEXBOS.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.6/pyxtal/database/cifs/YICMOP.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.6/pyxtal/database/cifs/anthracene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/aspirin-c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/aspirin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.6/pyxtal/database/cifs/benzene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/bug.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/coumarin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.6/pyxtal/database/cifs/dist_6_0.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.6/pyxtal/database/cifs/dist_6_1.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/gdh.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.6/pyxtal/database/cifs/ht_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.6/pyxtal/database/cifs/ht_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.6/pyxtal/database/cifs/ht_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/ice.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.6/pyxtal/database/cifs/lt_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/lt_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/lt_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.6/pyxtal/database/cifs/naphthalene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.6/pyxtal/database/cifs/resorcinol.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.6/pyxtal/database/cifs/sim-0.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.6/pyxtal/database/cifs/sim-1.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/cifs/xxvi.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/clusters.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.6/pyxtal/database/collection.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.6/pyxtal/database/element.py
--rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/k_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/layer.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/layer_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/layer_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/molecules.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/point.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/point_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/point_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/rod.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/rod_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/rod_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/symbols.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/t_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_list.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_sets.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/database/wyckoff_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2023-06-03 17:11:12.000000 pyxtal-0.5.6/pyxtal/db.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18767 2023-01-09 17:49:14.000000 pyxtal-0.5.6/pyxtal/descriptor.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2023-04-04 17:06:21.000000 pyxtal-0.5.6/pyxtal/elasticity.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/interface/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/LJ.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    27549 2023-01-11 02:44:28.000000 pyxtal-0.5.6/pyxtal/interface/dftb.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    10599 2023-06-05 08:33:21.000000 pyxtal-0.5.6/pyxtal/interface/gulp.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.6/pyxtal/interface/lammpslib.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/vasp.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/interface/vasprun.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.6/pyxtal/io.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    67422 2023-06-05 17:26:36.000000 pyxtal-0.5.6/pyxtal/lattice.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17952 2022-09-15 04:47:12.000000 pyxtal-0.5.6/pyxtal/molecular_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.6/pyxtal/molecule.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.6/pyxtal/msg.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2022-08-15 15:30:42.000000 pyxtal-0.5.6/pyxtal/operations.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/optimize/
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/fire.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/fire2.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/optimize/myscipy_optimize.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal/potentials/
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/CuAg.eam.alloy
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/LJ_cluster.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/Si.tersoff
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/SiCGe.tersoff
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.6/pyxtal/potentials/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    16730 2023-06-03 11:57:07.000000 pyxtal-0.5.6/pyxtal/representation.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    46380 2023-06-05 08:59:34.000000 pyxtal-0.5.6/pyxtal/supergroup.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   127177 2023-06-06 20:16:19.000000 pyxtal-0.5.6/pyxtal/symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    42070 2023-06-05 08:51:40.000000 pyxtal-0.5.6/pyxtal/test_all.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2022-06-20 18:26:47.000000 pyxtal-0.5.6/pyxtal/tolerance.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    16025 2023-04-04 16:58:20.000000 pyxtal-0.5.6/pyxtal/util.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-06-01 23:30:13.000000 pyxtal-0.5.6/pyxtal/version.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.6/pyxtal/viz.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    39382 2023-06-09 13:57:18.000000 pyxtal-0.5.6/pyxtal/wyckoff_site.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21212 2023-06-05 08:57:39.000000 pyxtal-0.5.6/pyxtal/wyckoff_split.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4217 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/SOURCES.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/dependency_links.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)      158 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/requires.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2023-06-09 17:12:42.000000 pyxtal-0.5.6/pyxtal.egg-info/top_level.txt
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-09 17:12:42.000000 pyxtal-0.5.6/scripts/
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     3973 2021-08-17 15:48:09.000000 pyxtal-0.5.6/scripts/pyxtal_main.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.6/scripts/pyxtal_symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-06-09 17:12:42.000000 pyxtal-0.5.6/setup.cfg
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1796 2022-09-15 04:14:56.000000 pyxtal-0.5.6/setup.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.7/LICENSE.txt
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       82 2022-06-15 16:30:37.000000 pyxtal-0.5.7/MANIFEST.in
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-20 14:43:17.000000 pyxtal-0.5.7/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.7/README.md
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.7/pyxtal/XRD.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   101275 2023-06-14 20:14:43.000000 pyxtal-0.5.7/pyxtal/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.7/pyxtal/block_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.7/pyxtal/constants.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2022-06-21 13:41:23.000000 pyxtal-0.5.7/pyxtal/crystal.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/database/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.7/pyxtal/database/HM_Full.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/atomic_scattering_params.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.7/pyxtal/database/bonds.json
+-rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.7/pyxtal/database/bug.json
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/database/cifs/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.7/pyxtal/database/cifs/0-G62.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.7/pyxtal/database/cifs/1-G59.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/191.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.7/pyxtal/database/cifs/2-G71.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.7/pyxtal/database/cifs/3-G139.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.7/pyxtal/database/cifs/4-G225.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/ACBNZA01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/AXOSOW01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.7/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/BTO-Amm2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/BTO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.7/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.7/pyxtal/database/cifs/FAU.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/Fd3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.7/pyxtal/database/cifs/Fd3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.7/pyxtal/database/cifs/Fd3m.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/GUMMUW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/GeF2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/HAHCOI.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.7/pyxtal/database/cifs/I41amd.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/I4_132.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/JAPWIH.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/LAGNAL.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/LUFHAW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/LiCs.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/MERQIM.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/MPWO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NaCl.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NaSb3F10.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NbO2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NiS-Cm.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/P3_112.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/P4_332.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.7/pyxtal/database/cifs/P4nmm.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/P6_422.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/PAHYON01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/PPO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/PVO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pm3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pmmn.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pn3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pn3m.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/R-3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/R-3c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/R32.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/TMPPIO03.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/WEXBOS.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.7/pyxtal/database/cifs/YICMOP.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.7/pyxtal/database/cifs/anthracene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/aspirin-c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/aspirin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.7/pyxtal/database/cifs/benzene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/bug.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/coumarin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.7/pyxtal/database/cifs/dist_6_0.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.7/pyxtal/database/cifs/dist_6_1.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/gdh.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.7/pyxtal/database/cifs/ht_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.7/pyxtal/database/cifs/ht_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.7/pyxtal/database/cifs/ht_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/ice.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.7/pyxtal/database/cifs/lt_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/lt_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/lt_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.7/pyxtal/database/cifs/naphthalene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.7/pyxtal/database/cifs/resorcinol.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.7/pyxtal/database/cifs/sim-0.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.7/pyxtal/database/cifs/sim-1.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/xxvi.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/clusters.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.7/pyxtal/database/collection.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.7/pyxtal/database/element.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/k_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/layer.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/layer_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/layer_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/molecules.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/point.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/point_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/point_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/rod.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/rod_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/rod_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/symbols.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/t_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_list.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_sets.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2023-06-13 10:12:21.000000 pyxtal-0.5.7/pyxtal/db.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18767 2023-01-09 17:49:14.000000 pyxtal-0.5.7/pyxtal/descriptor.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2023-04-04 17:06:21.000000 pyxtal-0.5.7/pyxtal/elasticity.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/interface/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/LJ.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    27549 2023-01-11 02:44:28.000000 pyxtal-0.5.7/pyxtal/interface/dftb.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12441 2023-06-20 14:35:57.000000 pyxtal-0.5.7/pyxtal/interface/gulp.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.7/pyxtal/interface/lammpslib.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/vasp.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/vasprun.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.7/pyxtal/io.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    67422 2023-06-12 20:57:05.000000 pyxtal-0.5.7/pyxtal/lattice.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17952 2022-09-15 04:47:12.000000 pyxtal-0.5.7/pyxtal/molecular_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.7/pyxtal/molecule.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.7/pyxtal/msg.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2022-08-15 15:30:42.000000 pyxtal-0.5.7/pyxtal/operations.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/optimize/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/fire.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/fire2.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/myscipy_optimize.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/potentials/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/CuAg.eam.alloy
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/LJ_cluster.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/Si.tersoff
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/SiCGe.tersoff
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    16972 2023-06-12 20:43:44.000000 pyxtal-0.5.7/pyxtal/representation.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    46380 2023-06-05 08:59:34.000000 pyxtal-0.5.7/pyxtal/supergroup.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   130450 2023-06-15 07:38:47.000000 pyxtal-0.5.7/pyxtal/symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    42484 2023-06-12 09:31:13.000000 pyxtal-0.5.7/pyxtal/test_all.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2022-06-20 18:26:47.000000 pyxtal-0.5.7/pyxtal/tolerance.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17439 2023-06-15 07:58:40.000000 pyxtal-0.5.7/pyxtal/util.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-06-20 14:38:04.000000 pyxtal-0.5.7/pyxtal/version.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.7/pyxtal/viz.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    39382 2023-06-09 13:57:18.000000 pyxtal-0.5.7/pyxtal/wyckoff_site.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21212 2023-06-05 08:57:39.000000 pyxtal-0.5.7/pyxtal/wyckoff_split.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4217 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/SOURCES.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/dependency_links.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      158 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/requires.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/top_level.txt
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/scripts/
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     3973 2021-08-17 15:48:09.000000 pyxtal-0.5.7/scripts/pyxtal_main.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.7/scripts/pyxtal_symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-06-20 14:43:17.000000 pyxtal-0.5.7/setup.cfg
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1796 2023-06-09 17:27:30.000000 pyxtal-0.5.7/setup.py
```

### Comparing `pyxtal-0.5.6/LICENSE.txt` & `pyxtal-0.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/PKG-INFO` & `pyxtal-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.5.6/README.md` & `pyxtal-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/XRD.py` & `pyxtal-0.5.7/pyxtal/XRD.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/__init__.py` & `pyxtal-0.5.7/pyxtal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1470,14 +1470,15 @@
         self.PBC = [1, 1, 1]
         self.numIons = numIons
         self.species = species
         numIons_added = np.zeros(len(numIons), dtype=int)
         _sites = []
 
         if len(sites) != len(species):
+            print(len(sites), len(species))
             raise RuntimeError("Inconsistency between sites and species")
 
         for sp, wps in zip(species, sites):
             if type(wps) is dict:
                 for pair in wps.items():
                     (key, pos) = pair
                     _wp = choose_wyckoff(self.group, site=key)
@@ -1698,32 +1699,35 @@
         special = False
         for msite in self.mol_sites:
             if msite.wp.index > 0:
                 special = True
                 break
         return special
 
-    def to_subgroup(self):
+    def to_subgroup(self, path=None):
         """
-        Transform a molecular crystal with speical sites to subgroup
+        Transform a crystal with speical sites to subgroup
         represenatation with general sites
         """
         if not self.standard_setting:
             self.optimize_lattice(standard=True)
 
-        if self.molecular:
-            sites = self.mol_sites
-        else:
-            sites = self.atom_sites
+        # Compute the path is needed
+        if path is None:
+            if self.molecular:
+                sites = self.mol_sites
+            else:
+                sites = self.atom_sites
+
+            max_index = max([site.wp.index for site in sites])
+            if self.molecular:
+                path = self.group.short_path_to_general_wp(max_index, True)
+            else:
+                path = self.group.short_path_to_general_wp(max_index)
 
-        max_index = max([site.wp.index for site in sites])
-        if self.molecular:
-            path = self.group.short_path_to_general_wp(max_index, True)
-        else:
-            path = self.group.short_path_to_general_wp(max_index)
         if path is not None:
             gtypes, ids = [], []
             for p in path:
                 gtypes.append(p[0])
                 ids.append(p[1])
             sub = self.subgroup_by_path(gtypes, ids, eps=0)
             sub.optimize_lattice()
@@ -2208,15 +2212,15 @@
         # resort sites_H based on elements0
         seq = list(map(lambda x: elements1.index(x), elements0))
         sites_H = [sites_H[i] for i in seq]
         numIons_H = []
         for site in sites_H:
             numIons_H.append(sum([int(l[:-1]) for l in site]))
 
-        # enumerate all possible solution space
+        # enumerate all possible solutions
         ids = []
         g_types = []
         G = self.group
         for p in path[1:]:
             dicts, g_type = G.get_max_subgroup(p)
             _ids = []
             for i, sub in enumerate(dicts['subgroup']):
@@ -2520,21 +2524,21 @@
         return display_cluster(molecules, self.lattice.matrix, engs, cmap, **kwargs)
 
     def substitute(self, dicts):
         """
         A quick function to apply substitution
         For molecule only
 
-
         Args:
-            dicts: {"F": "Cl"}
+            dicts: e.g., {"F": "Cl"}
         """
         pmg = self.to_pymatgen()
-        pmg.replace_species({'F': 'Cl'})
-        smi = [m.smile.replace('F', 'Cl') + '.smi' for m in self.molecules]
+        pmg.replace_species(dicts)
+        for e1e in dicts.keys():
+            smi = [m.smile.replace(ele, dicts[ele]) + '.smi' for m in self.molecules]
         self.from_seed(pmg, smi)
 
     def remove_water(self):
         """
         Remove water from hydrates
         """
         molecules = []
@@ -2557,38 +2561,42 @@
                     #print("add sites", i, m)
                     break
 
         self.molecules = molecules
         self.numMols = numMols
         self.mol_sites = sites
 
-    def set_cutoff(self):
+    def set_cutoff(self, exclude_ii=False):
         """
         get the cutoff dictionary
         """
         cutoff = {}
         tm = Tol_matrix(prototype="molecular")
         for i in range(len(self.species)):
             s1 = self.species[i]
             for j in range(i, len(self.species)):
                 s2 = self.species[j]
-                tuple_elements = (s1, s2)
-                cutoff[tuple_elements] = tm.get_tol(s1, s2)
+                select = True
+                if exclude_ii and s1 == s2:
+                    select = False
+                if select:
+                    tuple_elements = (s1, s2)
+                    cutoff[tuple_elements] = tm.get_tol(s1, s2)
 
         self.cutoff = cutoff
 
-    def set_site_coordination(self, cutoff=None, verbose=False):
+    def set_site_coordination(self, cutoff=None, verbose=False, exclude_ii=False):
         """
         Compute the coordination number from each atomic site 
         """
         from ase.neighborlist import neighbor_list
 
         if cutoff is None:
-            if not hasattr(self, 'cutoff'):
-                self.set_cutoff()
+            #if not hasattr(self, 'cutoff'):
+            self.set_cutoff(exclude_ii)
             cutoff = self.cutoff
 
         if verbose:
             print("\n The cutoff values for CN calculation are")
             print(cutoff)
 
         atoms = self.to_ase(resort=False)
```

### Comparing `pyxtal-0.5.6/pyxtal/block_crystal.py` & `pyxtal-0.5.7/pyxtal/block_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/constants.py` & `pyxtal-0.5.7/pyxtal/constants.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/crystal.py` & `pyxtal-0.5.7/pyxtal/crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/HM_Full.csv` & `pyxtal-0.5.7/pyxtal/database/HM_Full.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/atomic_scattering_params.json` & `pyxtal-0.5.7/pyxtal/database/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/bonds.json` & `pyxtal-0.5.7/pyxtal/database/bonds.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/bug.json` & `pyxtal-0.5.7/pyxtal/database/bug.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/0-G62.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/0-G62.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/1-G59.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/1-G59.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/2-G71.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/2-G71.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/3-G139.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/3-G139.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/4-G225.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/4-G225.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/ACBNZA01.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/ACBNZA01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/AXOSOW01.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/AXOSOW01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/BTO-Amm2.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/BTO-Amm2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/BTO.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/BTO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/FAU.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/FAU.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/Fd3.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/Fd3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/Fd3.vasp` & `pyxtal-0.5.7/pyxtal/database/cifs/Fd3.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/Fd3m.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/Fd3m.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/GUMMUW.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/GUMMUW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/GeF2.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/GeF2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/HAHCOI.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/HAHCOI.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/I4_132.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/I4_132.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/JAPWIH.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/JAPWIH.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/LAGNAL.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/LAGNAL.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/LUFHAW.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/LUFHAW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/LiCs.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/LiCs.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/MERQIM.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/MERQIM.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/MPWO.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/MPWO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/NaCl.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/NaCl.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/NaSb3F10.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/NaSb3F10.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/NbO2.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/NbO2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/NiS-Cm.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/NiS-Cm.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/P3_112.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/P3_112.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/P4_332.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/P4_332.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/P6_422.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/P6_422.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/PAHYON01.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/PAHYON01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/PPO.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/PPO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/PVO.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/PVO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/Pm3.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/Pm3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/R-3.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/R-3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/R-3c.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/R-3c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/R32.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/R32.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/TMPPIO03.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/TMPPIO03.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/WEXBOS.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/WEXBOS.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/YICMOP.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/YICMOP.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/anthracene.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/anthracene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/aspirin-c.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/aspirin-c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/aspirin.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/aspirin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/benzene.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/benzene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/bug.vasp` & `pyxtal-0.5.7/pyxtal/database/cifs/bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/coumarin.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/coumarin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/dist_6_0.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/dist_6_0.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/dist_6_1.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/dist_6_1.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/gdh.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/gdh.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/ht_KNbBO.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/ht_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/ht_cristobalite.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/ht_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/ht_quartz.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/ht_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/ice.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/ice.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/lt_KNbBO.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/lt_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/lt_cristobalite.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/lt_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/lt_quartz.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/lt_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/naphthalene.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/naphthalene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/resorcinol.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/resorcinol.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/cifs/xxvi.cif` & `pyxtal-0.5.7/pyxtal/database/cifs/xxvi.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/clusters.json` & `pyxtal-0.5.7/pyxtal/database/clusters.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/collection.py` & `pyxtal-0.5.7/pyxtal/database/collection.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/element.py` & `pyxtal-0.5.7/pyxtal/database/element.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/k_subgroup.json` & `pyxtal-0.5.7/pyxtal/database/k_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/layer.csv` & `pyxtal-0.5.7/pyxtal/database/layer.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/layer_generators.csv` & `pyxtal-0.5.7/pyxtal/database/layer_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/layer_symmetry.csv` & `pyxtal-0.5.7/pyxtal/database/layer_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/molecules.json` & `pyxtal-0.5.7/pyxtal/database/molecules.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/point.csv` & `pyxtal-0.5.7/pyxtal/database/point.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/point_generators.csv` & `pyxtal-0.5.7/pyxtal/database/point_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/point_symmetry.csv` & `pyxtal-0.5.7/pyxtal/database/point_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/rod.csv` & `pyxtal-0.5.7/pyxtal/database/rod.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/rod_generators.csv` & `pyxtal-0.5.7/pyxtal/database/rod_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/rod_symmetry.csv` & `pyxtal-0.5.7/pyxtal/database/rod_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/symbols.json` & `pyxtal-0.5.7/pyxtal/database/symbols.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/t_subgroup.json` & `pyxtal-0.5.7/pyxtal/database/t_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/wyckoff_generators.csv` & `pyxtal-0.5.7/pyxtal/database/wyckoff_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/wyckoff_list.csv` & `pyxtal-0.5.7/pyxtal/database/wyckoff_list.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/wyckoff_sets.json` & `pyxtal-0.5.7/pyxtal/database/wyckoff_sets.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/database/wyckoff_symmetry.csv` & `pyxtal-0.5.7/pyxtal/database/wyckoff_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/db.py` & `pyxtal-0.5.7/pyxtal/db.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/descriptor.py` & `pyxtal-0.5.7/pyxtal/descriptor.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/elasticity.py` & `pyxtal-0.5.7/pyxtal/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/interface/LJ.py` & `pyxtal-0.5.7/pyxtal/interface/LJ.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/interface/dftb.py` & `pyxtal-0.5.7/pyxtal/interface/dftb.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/interface/gulp.py` & `pyxtal-0.5.7/pyxtal/interface/gulp.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,32 +12,40 @@
     At the moment, only inorganic crystal is considered
 
     Args:
 
     struc: structure object generated by Pyxtal
     ff: path of forcefield lib
     opt: `conv`, `conp`, `single`
+    pstress (float): external pressure
+    steps (int): relaxation steps
+    symm (bool): whether or not impose the symmetry
     """
 
     def __init__(self, struc, label="_", path='tmp', ff='reax', \
                  pstress=None, opt='conp', steps=1000, exe='gulp',\
-                 input='gulp.in', output='gulp.log', dump=None):
+                 input='gulp.in', output='gulp.log', dump=None,
+                 symmetry=False):
 
         if isinstance(struc, pyxtal):
+            self.pyxtal = struc
             self.species = struc.species
             struc = struc.to_ase(resort=False)
+        else:
+            self.pyxtal = None
 
         if isinstance(struc, Atoms):
             self.lattice = Lattice.from_matrix(struc.cell)
             self.frac_coords = struc.get_scaled_positions()
             self.sites = struc.get_chemical_symbols()
             self.species = None
         else:
             raise NotImplementedError("only support ASE atoms object")
-
+        
+        self.symmetry = symmetry
         self.structure = struc
         self.pstress= pstress
         self.label = label
         self.ff = ff
         self.opt = opt
         self.exe = exe
         self.steps = steps
@@ -95,28 +103,39 @@
         return struc
 
     def write(self):
         a, b, c, alpha, beta, gamma = self.lattice.get_para(degree=True)
         
         with open(self.input, 'w') as f:
             if self.opt == 'conv':
-                f.write('opti stress {:s} conjugate nosymmetry\n'.format(self.opt))
+                f.write('opti stress {:s} conjugate '.format(self.opt))
             elif self.opt == "single":
-                f.write('grad conp stress\n')
+                f.write('grad conp stress ')
             else:
-                f.write('opti stress {:s} conjugate nosymmetry\n'.format(self.opt))
+                f.write('opti stress {:s} conjugate '.format(self.opt))
+
+            if not self.symmetry:
+                f.write('nosymmetry\n')
 
             f.write('\ncell\n')
             f.write('{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}\n'.format(\
                     a, b, c, alpha, beta, gamma))
             f.write('\nfractional\n')
             
             symbols = []
-            for coord, site in zip(self.frac_coords, self.sites):
-                f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} core \n'.format(site, *coord))
+            if self.symmetry and self.pyxtal is not None:
+                # Use pyxta here
+                for site in self.pyxtal.atom_sites:
+                    symbol, coord = site.specie, site.position
+                    f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} core \n'.format(symbol, *coord))
+                f.write('\nspace\n{:d}\n'.format(self.pyxtal.group.number))
+            else:
+                # all coordinates
+                for coord, site in zip(self.frac_coords, self.sites):
+                    f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} core \n'.format(site, *coord))
             if self.species is not None:
                 species = self.structure.species
             else:
                 species = list(set(self.sites))
 
             f.write('\nSpecies\n')
             for specie in species:
@@ -135,15 +154,17 @@
 
 
     def read(self):
         with open(self.output, 'r') as f:
             lines = f.readlines()
         try: 
             for i, line in enumerate(lines):
-                if self.pstress is None or self.pstress == 0:
+                if self.symmetry and self.pyxtal.group.symbol[0] != 'P':
+                    m = re.match(r'\s*Non-primitive unit cell\s*=\s*(\S+)\s*eV', line)
+                elif self.pstress is None or self.pstress == 0:
                     m = re.match(r'\s*Total lattice energy\s*=\s*(\S+)\s*eV', line)
                 else:
                     m = re.match(r'\s*Total lattice enthalpy\s*=\s*(\S+)\s*eV', line)
                 #print(line.find('Final asymmetric unit coord'), line)
                 if m:
                     self.energy = float(m.group(1))
                     self.energy_per_atom = self.energy/len(self.frac_coords)
@@ -194,14 +215,24 @@
                         G = [-float(x) * eV / Ang for x in g]
                         forces.append(G)
                     forces = np.array(forces)
                     self.forces = forces
 
                 elif line.find(' Cycle: ') != -1:
                     self.iter = int(line.split()[1])
+    
+                # asymmetric unit
+                elif line.find('Final asymmetric unit coordinates') != -1:
+                    s = i + 6
+                    positions = []
+                    for _i in range(len(self.pyxtal.atom_sites)):
+                        xyz = lines[s+_i].split()[3:6]
+                        XYZ = [float(x) for x in xyz]
+                        #print(XYZ)
+                        self.pyxtal.atom_sites[_i].update(XYZ)
 
                 elif line.find('Final fractional coordinates of atoms') != -1:
                     s = i + 5
                     positions = []
                     species = []
                     while True:
                         s = s + 1
@@ -219,41 +250,56 @@
                     lattice_vectors = np.zeros((3,3))
                     s = i + 2
                     for j in range(s, s+3):
                         temp=lines[j].split()
                         for k in range(3):
                             lattice_vectors[j-s][k]=float(temp[k])
                     self.lattice = Lattice.from_matrix(lattice_vectors)
+                    if self.pyxtal is not None:
+                        self.pyxtal.lattice = self.lattice
             if np.isnan(self.energy):
                 self.error = True
                 self.energy = None
                 print("GULP calculation is wrong, reading------")
         except:
             self.error = True
             self.energy = None
             print("GULP calculation is wrong")
 
-def single_optimize(struc, ff, steps=1000, pstress=None, opt="conp", exe="gulp", path="tmp", label="_", clean=True):
-    calc = GULP(struc, steps=steps, label=label, path=path, pstress=pstress, ff=ff, opt=opt)
+def single_optimize(struc, ff, steps=1000, pstress=None, opt="conp", 
+                    exe="gulp", path="tmp", label="_", clean=True,
+                    symmetry=False):
+
+    calc = GULP(struc, steps=steps, label=label, path=path, 
+                pstress=pstress, ff=ff, opt=opt, symmetry=symmetry)
+
     calc.run(clean=clean)
+
     if calc.error:
         print("GULP error in single optimize")
         return None, None, 0, True
     else:
-        struc = calc.to_pyxtal()
-        #if sum(struc.numIons) == 42:
-        #    print("SSSSSSSSSSSSSS")
-        #    import sys; sys.exit()   
+        if calc.pyxtal is None:
+            struc = calc.to_pyxtal()
+        else:
+            struc = calc.pyxtal
+        #if sum(struc.numIons) == 42: print("SSSSS"); import sys; sys.exit()   
         return struc, calc.energy_per_atom, calc.cputime, calc.error
 
 def optimize(struc, ff, optimizations=["conp", "conp"], exe="gulp", 
             pstress=None, path="tmp", label="_", clean=True, adjust=False):
+    """
+    Multiple calls
+
+    """
     time_total = 0
     for opt in optimizations:
-        struc, energy, time, error = single_optimize(struc, ff, pstress, opt, exe, path, label, clean)
+        struc, energy, time, error = single_optimize(struc, ff, 
+        pstress=pstress, opt=opt, exe=exe, path=path, label=label, clean=clean)
+
         time_total += time
         if error:
             return None, None, 0, True
         elif adjust and abs(energy)<1e-8:
             matrix = struc.lattice.matrix
             struc.lattice.set_matrix(matrix*0.8)
             
@@ -263,22 +309,26 @@
 if __name__ == "__main__":
 
     while True:
         struc = pyxtal()
         struc.from_random(3, 19, ["C"], [4])
         if struc.valid:
             break
-
+    print(struc)
     pmg1 = struc.to_pymatgen()
     calc = GULP(struc, opt="single", ff="tersoff.lib")
-    calc.run()
+    calc.run(clean=False)#; import sys; sys.exit()
     print(calc.energy)
     print(calc.stress)
     print(calc.forces)
     pmg2 = calc.to_pymatgen()
+    #xtal = calc.pyxtal #calc.to_pyxtal()
+    #print(calc.iter)
+    #print(xtal)
+
     import pymatgen.analysis.structure_matcher as sm
     print(sm.StructureMatcher().fit(pmg1, pmg2))
 
     struc, eng, time, _ = optimize(struc, ff="tersoff.lib")
     print(struc)
     print(eng)
     print(time)
```

### Comparing `pyxtal-0.5.6/pyxtal/interface/lammpslib.py` & `pyxtal-0.5.7/pyxtal/interface/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/interface/vasp.py` & `pyxtal-0.5.7/pyxtal/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/interface/vasprun.py` & `pyxtal-0.5.7/pyxtal/interface/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/io.py` & `pyxtal-0.5.7/pyxtal/io.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/lattice.py` & `pyxtal-0.5.7/pyxtal/lattice.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/molecular_crystal.py` & `pyxtal-0.5.7/pyxtal/molecular_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/molecule.py` & `pyxtal-0.5.7/pyxtal/molecule.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/msg.py` & `pyxtal-0.5.7/pyxtal/msg.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/operations.py` & `pyxtal-0.5.7/pyxtal/operations.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/optimize/fire.py` & `pyxtal-0.5.7/pyxtal/optimize/fire.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/optimize/fire2.py` & `pyxtal-0.5.7/pyxtal/optimize/fire2.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/optimize/myscipy_optimize.py` & `pyxtal-0.5.7/pyxtal/optimize/myscipy_optimize.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/potentials/CuAg.eam.alloy` & `pyxtal-0.5.7/pyxtal/potentials/CuAg.eam.alloy`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/potentials/LJ_cluster.py` & `pyxtal-0.5.7/pyxtal/potentials/LJ_cluster.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/potentials/Si.tersoff` & `pyxtal-0.5.7/pyxtal/potentials/Si.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/potentials/SiCGe.tersoff` & `pyxtal-0.5.7/pyxtal/potentials/SiCGe.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/representation.py` & `pyxtal-0.5.7/pyxtal/representation.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,23 @@
         struc._get_formula()
         struc.source = '1D rep.'
         struc.valid = True
         struc.standard_setting = site.wp.is_standard_setting()
 
         return struc
     
+    def to_array(self):
+        """
+        Export only varibles to a 1d numpy array
+        """
+        cells, xyzs = self.x[0][1:], self.x[1:]
+        x = cells
+        for xyz in xyzs: x = np.hstack((x, xyz[2:]))
+        return x
+        
     def to_string(self, time=None, eng=None, tag=None):
         """
         Export string representation
 
         Args:
             time: float
             eng: float
```

### Comparing `pyxtal-0.5.6/pyxtal/supergroup.py` & `pyxtal-0.5.7/pyxtal/supergroup.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/symmetry.py` & `pyxtal-0.5.7/pyxtal/symmetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,25 +180,28 @@
     x+1/2, -y+1, z+1/2
     -x+1/2, y+1/2, z
 
     We also provide several utilities functions, e.g.,
     one can search the possible wyckoff_combinations by a formula
 
     >>> g.list_wyckoff_combinations([4, 2])
-    (None, False)
+    ([], [], [])
     >>> g.list_wyckoff_combinations([4, 8])
     ([[['4a'], ['8c']],
     [['4a'], ['8d']],
     [['4a'], ['8e']],
     [['4a'], ['8f']],
     [['4b'], ['8c']],
     [['4b'], ['8d']],
     [['4b'], ['8e']],
     [['4b'], ['8f']]],
-    [False, True, True, True, False, True, True, True])
+    [False, True, True, True, False, True, True, True],
+    [[[6], [4]], [[6], [3]], [[6], [2]], [[6], [1]], 
+    [[5], [4]], [[5], [3]], [[5], [2]], [[5], [1]]]
+    )
 
     or search the subgroup information
 
     >>> g.get_max_t_subgroup()['subgroup']
     [12, 14, 15, 20, 36, 39, 41]
 
     or check if a given composition is compatible with Wyckoff positions
@@ -341,14 +344,32 @@
                 site = site[-1]
             id = len(self) - letters.index(site) - 1
             string = self[id].ops[0].as_xyz_string()
             dof[i] = len(set(re.sub('[^a-z]+', '', string)))
 
         return dof
 
+    def get_lattice_dof(self):
+        """
+        compute the degree of freedom for the lattice
+        """
+        if self.lattice_type in ["triclinic"]:
+            dof = 6
+        elif self.lattice_type in ["monoclinic"]:
+            dof = 4
+        elif self.lattice_type in ['orthorhombic']:
+            dof = 3
+        elif self.lattice_type in ['tetragonal', 'hexagonal', 'trigonal']:
+            dof = 2
+        else:
+            dof = 1
+       
+        return dof
+
+
     def is_valid_combination(self, sites):
         """
         check if the solutions are valid. A special WP with zero freedom (0,0,0)
         cannot be occupied twice.
 
         Args:
             sites: list, e.g. ['4a', '8b'] or ['a', 'b']
@@ -365,15 +386,15 @@
             letter = wp.letter
             if sites.count(letter)>1:
                 freedom = np.trace(wp.ops[0].rotation_matrix) > 0
                 if not freedom:
                     return False
         return True
 
-    def list_wyckoff_combinations(self, numIons, quick=False):
+    def list_wyckoff_combinations(self, numIons, quick=False, max_wp=None, min_wp=None, Nmax=10000000):
         """
         List all possible wyckoff combinations for the given formula. Note this
         is really designed for a light weight calculation. If the solution space
         is big, set quick as True.
 
         Args:
             numIons: [12, 8]
@@ -381,19 +402,24 @@
 
         Returns:
             Combinations: list of possible sites
             has_freedom: list of boolean numbers
         """
 
         numIons = np.array(numIons)
+        # Must be greater than the number of smallest wp multiplicity
+        if numIons.min() < self[-1].multiplicity:
+            return [], [], []
+        elif max_wp is not None and sum(numIons) > self[0].multiplicity*max_wp:
+            return [], [], []
 
         basis = [] # [8, 4, 4]
         letters = [] # ['c', 'b', 'a']
         freedoms = [] # [False, False, False]
-
+        ids = [] # [2, 3, 4]
         # obtain the basis
         for i, wp in enumerate(self):
             mul = wp.multiplicity
             letter = wp.letter
             freedom = np.trace(wp.ops[0].rotation_matrix) > 0
             if mul <= max(numIons):
                 if quick:
@@ -405,89 +431,120 @@
                         basis.append(mul)
                         letters.append(letter)
                         freedoms.append(freedom)
                 else:
                     basis.append(mul)
                     letters.append(letter)
                     freedoms.append(freedom)
+                    ids.append(i)
 
         basis = np.array(basis)
 
         # quickly exit
         if np.min(numIons) < np.min(basis):
             #print(numIons, basis)
-            return None, False
+            return [], []
         # odd and even
         elif np.mod(numIons, 2).sum()>0 and np.mod(basis, 2).sum()==0:
             #print("odd-even", numIons, basis)
-            return None, False
+            #return None, False
+            return [], [], []
 
+        #print("basis", basis)
+        #print("numIons", numIons)
         # obtain the maximum numbers for each basis
-        max_solutions = np.floor(numIons[:,None]/basis)
         # reset the maximum to 1 if there is no freedom
+        # find the integer solutions
+        # reset solutions according to max_wp
+        max_solutions = np.floor(numIons[:, None]/basis)
         for i in range(len(freedoms)):
             if not freedoms[i]:
-                max_solutions[:,i] = 1
+                max_solutions[:, i] = 1
 
-        # find the integer solutions
-        max_arrays = max_solutions.flatten()
-        lists = []
-        for a in max_arrays:
-            d = int(a) + 1
-            lists.append(list(range(d)))
-        if len(lists) > 20:
-            msg = "Solution space is big, rerun it by setting quick as True"
-            raise RuntimeError(msg)
-
-        solutions = np.array(list(itertools.product(*lists)))
-        big_basis = np.tile(basis, len(numIons))
-
-        for i in range(len(numIons)):
-            N = solutions[:,i*len(basis):(i+1)*len(basis)].dot(basis)
-            solutions = solutions[N == numIons[i]]
-            if len(solutions) == 0:
-                #print("No solution is available")
-                return None, False
+        if max_wp is not None:
+            N_max = max_wp - (len(numIons) - 1)
+            max_solutions[max_solutions > N_max] = N_max 
+
+        list_solutions = []
+        for i, numIon in enumerate(numIons):
+            lists = []
+            prod = 1
+            for a in max_solutions[i]:
+                if prod <= Nmax: #10000000:
+                    d = int(a) + 1
+                    lists.append(list(range(d)))
+                    prod *= d
+                else:
+                    # If the size is too big, we terminate it asap
+                    lists.append([0])
+                    # Terminate the list
+                    # break
+            #print(len(lists), prod)
+
+            sub_solutions = np.array(list(itertools.product(*lists)))
+            N = sub_solutions.dot(basis)
+            sub_solutions = sub_solutions[N == numIon]
+            list_solutions.append(sub_solutions.tolist())
+            #print(i)
+            #print(sub_solutions)#; import sys; sys.exit()
+            if len(sub_solutions) == 0:
+                return [], [], []
+        
+        # Gather all solutions and remove very large number solutions
+        solutions = np.array(list(itertools.product(*list_solutions))) 
+        dim1 = solutions.shape[0]
+        dim2 = np.prod(solutions.shape[1:])
+        solutions = solutions.reshape([dim1, dim2])
+        if max_wp is not None:
+            solutions_total = solutions.sum(axis=1)
+            solutions = solutions[solutions_total <= max_wp]
+        if min_wp is not None:
+            solutions_total = solutions.sum(axis=1)
+            solutions = solutions[solutions_total >= min_wp]
 
         # convert the results to list
         combinations = []
         has_freedom = []
+        indices = []
         for solution in solutions:
             res = solution.reshape([len(numIons), len(basis)])
             _com = []
             _free = []
+            _ids = []
+
+            # QZ: check what's going on
             for i, numIon in enumerate(numIons):
                 tmp = []
                 bad_resolution = False
                 frozen = []
+                ids_in = []
                 for j, b in enumerate(basis):
                     if not freedoms[j] and (res[:, j]).sum() > 1:
                         bad_resolution = True
                         break
                     else:
                         if res[i, j] > 0:
-                            symbols = [str(b) + letters[j]] * res[i,j]
+                            symbols = [str(b) + letters[j]] * res[i, j]
                             tmp.extend(symbols)
                             frozen.extend([freedoms[j]])
+                            ids_in.extend([ids[j]] * res[i, j])
                 if not bad_resolution:
                     _com.append(tmp)
                     _free.extend(frozen)
+                    _ids.append(ids_in)
 
             if len(_com) == len(numIons):
                 combinations.append(_com)
+                indices.append(_ids)
                 if True in _free:
                     has_freedom.append(True)
                 else:
                     has_freedom.append(False)
 
-        if len(combinations) == 0:
-            #print("No solution is available")
-            return None, False
-        else:
-            return combinations, has_freedom
+        return combinations, has_freedom, indices
 
     def get_wyckoff_position(self, index):
         """
         Returns a single Wyckoff_position object.
 
         Args:
             index: the index of the Wyckoff position within the group.
@@ -531,14 +588,18 @@
         if self.dim == 3:
             return t_subgroup[str(self.number)]
         else:
             msg = "Only supports the subgroups for space group"
             raise NotImplementedError(msg)
 
     def get_max_subgroup(self, H):
+        """
+        Returns the dicts for both t and k subgroup, H is just track the type
+        QZ: the function name is not instructive, need to revise later
+        """
         if self.point_group == Group(H, quick=True).point_group:
             g_type = 'k'
             dicts = self.get_max_k_subgroup()
         else:
             g_type = 't'
             dicts = self.get_max_t_subgroup()
         return dicts, g_type
@@ -947,14 +1008,41 @@
 
             traversed.extend(groups)
             layers[l] = {'groups': deepcopy(groups),
                          'subgroups':[]}
             layers[l-1]['subgroups'] = deepcopy(subgroups)
         return final
 
+    def path_to_subgroup(self, H):
+        """
+        For a given a path, extract the 
+            a list of (g_types, subgroup_id, spg_number, wp_list (optional))
+        """
+        path_list = []
+        paths = self.search_subgroup_paths(H)
+        if len(paths) > 0:
+            path = paths[0]
+            g0 = Group(path[0], quick=True)
+            for p in path[1:]:
+                g1 = Group(p, quick=True)
+                if g0.point_group == g1.point_group:
+                    g_type = 'k'
+                    spgs = g0.get_max_k_subgroup()['subgroup']
+                else:
+                    g_type = 't'
+                    spgs = g0.get_max_t_subgroup()['subgroup']
+                for id, spg in enumerate(spgs):
+                    if spg == p:
+                        break
+                #print(id, spgs, spgs[id])
+                path_list.append((g_type, id, p))
+                g0 = g1
+        return path_list
+
+
     def search_subgroup_paths(self, G, max_layer=5):
         """
         Search paths to transit to subgroup H. if
         - path1 is a>>e
         - path2 is a>>b>>c>>e
         path 2 will not be counted since path 1 exists
```

### Comparing `pyxtal-0.5.6/pyxtal/test_all.py` & `pyxtal-0.5.7/pyxtal/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,33 +15,43 @@
 from pyxtal.lattice import Lattice
 from pyxtal.molecule import pyxtal_molecule
 from pyxtal.symmetry import Group, Wyckoff_position, get_wyckoffs, Hall
 from pyxtal.XRD import Similarity
 from pyxtal.operations import get_inverse
 from pyxtal.supergroup import supergroups, supergroup
 from pyxtal.descriptor import spherical_image
+from pyxtal.util import generate_wp_lib
 
 cif_path = resource_filename("pyxtal", "database/cifs/")
 l01 = Lattice.from_matrix([[4.08, 0, 0], [0, 9.13, 0], [0, 0, 5.50]])
 l02 = Lattice.from_para(4.08, 9.13, 5.50, 90, 90, 90)
 wp1 = Wyckoff_position.from_group_and_index(36, 0)
 wp2 = Wyckoff_position.from_group_and_letter(36, "4a")
 
 class TestGroup(unittest.TestCase):
+
+    def test_generate_wp_lib(self):
+        wps = generate_wp_lib([227, 228], composition=[1, 2])
+        self.assertTrue(len(wps) == 18)
+        wps = generate_wp_lib([227, 228], composition=[1, 1, 3])
+        self.assertTrue(len(wps) == 9)
+
     def test_list_wyckoff_combinations(self):
         g = Group(64)
-        a1, _ = g.list_wyckoff_combinations([4, 2])
-        self.assertTrue(a1 is None)
-        a2, _ = g.list_wyckoff_combinations([4, 8], quick=False) 
+        a1, _, _ = g.list_wyckoff_combinations([4, 2])
+        self.assertTrue(len(a1) == 0)
+        a2, _, _ = g.list_wyckoff_combinations([4, 8], quick=False) 
         self.assertTrue(len(a2) == 8)
 
-    def test_print_group(self):
-        for sg in [1, 15, 60, 143, 188]:
+    def test_print_group_and_dof(self):
+        for d in [(1, 6), (15, 4), (60, 3), (143, 2), (208, 1)]:
+            (sg, dof_ref) = d
             g = Group(sg)
-            #print(g)
+            dof = g.get_lattice_dof()
+            self.assertTrue(dof == dof_ref)
 
     def test_short_path(self):
         g = Group(217)
         path = g.short_path_to_general_wp(7)
         self.assertTrue(path[-1][2] == 145)
 
     def test_spg_symmetry(self):
```

### Comparing `pyxtal-0.5.6/pyxtal/tolerance.py` & `pyxtal-0.5.7/pyxtal/tolerance.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/util.py` & `pyxtal-0.5.7/pyxtal/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -483,14 +483,53 @@
     for i, id in enumerate(orders):
         s1, e1 = id*N_atoms, (id+1)*N_atoms
         s2, e2 = i*N_atoms, (i+1)*N_atoms
         pos1[s2:e2, :] += pos0[s1:e1, :] - shifts[i].dot(atoms.cell[:])
 
     atoms.set_positions(pos1)
     return atoms
+
+def generate_wp_lib(spg_list, composition, max_wp=None, min_wp=None):
+    """
+    Generate wps according to the composition constraint (e.g., SiO2)
+
+    Args;
+        - spg_list: list of space group choices
+        - composition: chemical compositions [1, 2]
+        - max_wp: the number of maximum wp sites
+        - min_wp: the number of minimum wp sites
+
+    Returns:
+        a list of wps [spg, ([wp1, ...], ... [wp1, ...]), wp_dof]
+    """
+
+    from pyxtal.symmetry import Group
+
+    composition = np.array(composition, dtype=int)
+    if max_wp is None: max_wp = len(composition)
+    if min_wp is None: min_wp = len(composition)
+    #print(max_wp, min_wp)
+    wps = []
+    for sg in spg_list:
+        g = Group(sg)
+        lat_dof = g.get_lattice_dof()
+        # determine the upper and lower limit 
+        min_repeat = max([int(len(g[-1])/min(composition)), 1])
+        max_repeat = max([int(len(g[0])/max(composition)), 1])
+        for i in range(min_repeat, max_repeat+1):
+            letters, _, wp_ids = g.list_wyckoff_combinations(
+                    composition*i, max_wp=max_wp, min_wp=min_wp)
+            for j, wp in enumerate(wp_ids):
+                wp_dofs = 0
+                for wp0 in wp:
+                    for id in wp0:
+                        wp_dofs += g[id].get_dof()
+                #print(sg, wp, letters[i])
+                wps.append((sg, wp, lat_dof + wp_dofs))
+    return wps 
  
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     parser = ArgumentParser()
     parser.add_argument(
```

### Comparing `pyxtal-0.5.6/pyxtal/viz.py` & `pyxtal-0.5.7/pyxtal/viz.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/wyckoff_site.py` & `pyxtal-0.5.7/pyxtal/wyckoff_site.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal/wyckoff_split.py` & `pyxtal-0.5.7/pyxtal/wyckoff_split.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/pyxtal.egg-info/PKG-INFO` & `pyxtal-0.5.7/pyxtal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.5.6/pyxtal.egg-info/SOURCES.txt` & `pyxtal-0.5.7/pyxtal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/scripts/pyxtal_main.py` & `pyxtal-0.5.7/scripts/pyxtal_main.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/scripts/pyxtal_symmetry.py` & `pyxtal-0.5.7/scripts/pyxtal_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.6/setup.py` & `pyxtal-0.5.7/setup.py`

 * *Files identical despite different names*

