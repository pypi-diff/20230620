# Comparing `tmp/asap3-3.13.1.tar.gz` & `tmp/asap3-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asap3-3.13.1.tar", last modified: Tue Jun 20 12:52:59 2023, max compression
+gzip compressed data, was "dist/asap3-3.9.6.tar", last modified: Wed Oct 26 10:36:18 2016, max compression
```

## Comparing `asap3-3.13.1.tar` & `asap3-3.9.6.tar`

### file list

```diff
@@ -1,523 +1,492 @@
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.112599 asap3-3.13.1/
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.891758 asap3-3.13.1/Archive/
--rw-r--r--   0 schiotz    (501) staff       (20)    29406 2018-02-22 12:09:10.000000 asap3-3.13.1/Archive/MoPotential.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3137 2018-02-22 12:09:10.000000 asap3-3.13.1/Archive/MoPotential.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.913829 asap3-3.13.1/Basics/
--rw-r--r--   0 schiotz    (501) staff       (20)     5631 2021-04-16 18:13:02.000000 asap3-3.13.1/Basics/Asap.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1461 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/AsapNamespace.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1847 2021-03-19 16:37:03.000000 asap3-3.13.1/Basics/AsapObject.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1945 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/AsapObject.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3226 2019-08-27 09:30:33.000000 asap3-3.13.1/Basics/AsapPython.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1670 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Atoms.h
--rw-r--r--   0 schiotz    (501) staff       (20)     8662 2021-04-21 07:36:30.000000 asap3-3.13.1/Basics/AtomsBasis.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2988 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Debug.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3696 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Debug.h
--rw-r--r--   0 schiotz    (501) staff       (20)     6613 2019-08-27 09:30:33.000000 asap3-3.13.1/Basics/DynamicAtoms.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2438 2021-03-19 15:03:26.000000 asap3-3.13.1/Basics/DynamicAtoms.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3985 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/Exception.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     7303 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/Exception.h
--rw-r--r--   0 schiotz    (501) staff       (20)     4710 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/IVec.h
--rw-r--r--   0 schiotz    (501) staff       (20)     9186 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/ImageAtoms.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     9998 2020-12-18 12:17:10.000000 asap3-3.13.1/Basics/ImageAtoms.h
--rw-r--r--   0 schiotz    (501) staff       (20)     4228 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/ImagePotential.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     4563 2021-04-21 07:36:30.000000 asap3-3.13.1/Basics/ImagePotential.h
--rw-r--r--   0 schiotz    (501) staff       (20)     8614 2021-03-29 20:41:54.000000 asap3-3.13.1/Basics/Langevin.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3141 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Langevin.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1838 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Matrix3x3.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1666 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Matrix3x3.h
--rw-r--r--   0 schiotz    (501) staff       (20)     7328 2021-03-29 20:42:24.000000 asap3-3.13.1/Basics/MolecularDynamics.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2717 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/MolecularDynamics.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3718 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/MonteCarloAtoms.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1986 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/MonteCarloAtoms.h
--rw-r--r--   0 schiotz    (501) staff       (20)    45535 2021-04-21 07:36:30.000000 asap3-3.13.1/Basics/NeighborCellLocator.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)    12919 2021-04-16 17:39:49.000000 asap3-3.13.1/Basics/NeighborCellLocator.h
--rw-r--r--   0 schiotz    (501) staff       (20)    28842 2021-04-21 07:36:30.000000 asap3-3.13.1/Basics/NeighborList.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     9146 2021-04-21 07:36:30.000000 asap3-3.13.1/Basics/NeighborList.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3828 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/NeighborList2013.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1729 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/NeighborList2013.h
--rw-r--r--   0 schiotz    (501) staff       (20)     6695 2020-12-18 12:17:10.000000 asap3-3.13.1/Basics/NeighborLocator.h
--rw-r--r--   0 schiotz    (501) staff       (20)    25252 2021-04-21 07:36:30.000000 asap3-3.13.1/Basics/NormalAtoms.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)    10990 2020-12-18 12:17:10.000000 asap3-3.13.1/Basics/NormalAtoms.h
--rw-r--r--   0 schiotz    (501) staff       (20)     4296 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/RandomNumbers.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      703 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/RandomNumbers.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2859 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/SymTensor.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3095 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Timing.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     7881 2018-12-20 11:50:46.000000 asap3-3.13.1/Basics/Timing.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1694 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/TimingResults.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2874 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/TinyMatrix.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1679 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Vec.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     5241 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/Vec.h
--rw-r--r--   0 schiotz    (501) staff       (20)     6170 2021-03-19 20:02:44.000000 asap3-3.13.1/Basics/VelocityVerlet.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2173 2021-03-19 15:03:28.000000 asap3-3.13.1/Basics/VelocityVerlet.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2149 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/mass.h
--rw-r--r--   0 schiotz    (501) staff       (20)    12835 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/stacktrace.c
--rw-r--r--   0 schiotz    (501) staff       (20)     1387 2018-02-22 12:09:10.000000 asap3-3.13.1/Basics/stacktrace.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.922821 asap3-3.13.1/Brenner/
--rw-r--r--   0 schiotz    (501) staff       (20)     2207 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/AtomPairInfoState.h
--rw-r--r--   0 schiotz    (501) staff       (20)     6282 2021-04-21 07:36:30.000000 asap3-3.13.1/Brenner/BrennerPotential.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     7358 2021-04-21 07:36:30.000000 asap3-3.13.1/Brenner/BrennerPotential.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1317 2018-12-20 11:50:46.000000 asap3-3.13.1/Brenner/asapbrenner.h
--rw-r--r--   0 schiotz    (501) staff       (20)     6297 2018-12-20 11:50:46.000000 asap3-3.13.1/Brenner/bcuint.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     8833 2018-12-20 11:50:46.000000 asap3-3.13.1/Brenner/caguts.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      661 2018-12-20 11:50:46.000000 asap3-3.13.1/Brenner/expand.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      278 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/expand.h
--rw-r--r--   0 schiotz    (501) staff       (20)     9037 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/inter2d_iv.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     8997 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/mtable.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)    37763 2018-12-20 11:50:46.000000 asap3-3.13.1/Brenner/pibond.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)    11880 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/radic.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)   387465 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/radicdata.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     5695 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/sili_germ.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1631 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/spgch.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      188 2018-02-22 12:09:10.000000 asap3-3.13.1/Brenner/spgch.h
--rw-r--r--   0 schiotz    (501) staff       (20)    35147 2022-04-28 10:51:54.000000 asap3-3.13.1/COPYING
--rw-r--r--   0 schiotz    (501) staff       (20)     7651 2022-04-28 10:51:54.000000 asap3-3.13.1/COPYING.LESSER
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.931459 asap3-3.13.1/Interface/
--rw-r--r--   0 schiotz    (501) staff       (20)     8037 2019-08-27 09:30:33.000000 asap3-3.13.1/Interface/AsapModule.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1347 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/AsapModule.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1237 2019-08-27 09:30:33.000000 asap3-3.13.1/Interface/AsapSerial.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     9913 2021-03-19 20:10:44.000000 asap3-3.13.1/Interface/DynamicsInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1619 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/DynamicsInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     5974 2021-03-19 20:29:51.000000 asap3-3.13.1/Interface/EMTParameterProviderInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1902 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/EMTParameterProviderInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1474 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/ExceptionInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2752 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/ExceptionInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)    19858 2021-04-21 07:36:30.000000 asap3-3.13.1/Interface/NeighborLocatorInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2790 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/NeighborLocatorInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3751 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/OpenMPInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1764 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/OpenMPInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)    11784 2019-08-27 09:30:33.000000 asap3-3.13.1/Interface/PTMInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1484 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/PTMInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)    38914 2021-04-28 13:33:22.000000 asap3-3.13.1/Interface/PotentialInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1741 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/PotentialInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3356 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/PythonConversions.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3697 2018-12-20 11:50:46.000000 asap3-3.13.1/Interface/PythonConversions.h
--rw-r--r--   0 schiotz    (501) staff       (20)     7388 2018-12-20 11:50:46.000000 asap3-3.13.1/Interface/RDFInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1446 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/RDFInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2067 2021-03-19 21:21:52.000000 asap3-3.13.1/Interface/Templates.h
--rw-r--r--   0 schiotz    (501) staff       (20)     5593 2021-03-19 20:26:45.000000 asap3-3.13.1/Interface/ToolsInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1838 2018-02-22 12:09:10.000000 asap3-3.13.1/Interface/ToolsInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)      461 2018-02-22 12:09:10.000000 asap3-3.13.1/MANIFEST.in
--rw-r--r--   0 schiotz    (501) staff       (20)    21844 2020-12-18 12:17:15.000000 asap3-3.13.1/Makefile
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.936061 asap3-3.13.1/OpenKIMexport/
--rw-r--r--   0 schiotz    (501) staff       (20)     2421 2018-12-20 11:50:46.000000 asap3-3.13.1/OpenKIMexport/KimAsapPython.h
--rw-r--r--   0 schiotz    (501) staff       (20)     5856 2018-12-20 11:50:46.000000 asap3-3.13.1/OpenKIMexport/KimAtoms.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     6488 2018-12-20 11:50:46.000000 asap3-3.13.1/OpenKIMexport/KimAtoms.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3823 2018-12-20 11:50:46.000000 asap3-3.13.1/OpenKIMexport/KimNeighborLocator.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     5862 2020-12-18 12:17:15.000000 asap3-3.13.1/OpenKIMexport/KimNeighborLocator.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1739 2020-12-18 12:17:15.000000 asap3-3.13.1/OpenKIMexport/KimTemplates.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2162 2018-12-20 11:50:46.000000 asap3-3.13.1/OpenKIMexport/NeighborLocatorInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)    10219 2018-12-20 11:50:46.000000 asap3-3.13.1/OpenKIMexport/asap_kim_api.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     4177 2019-01-31 10:01:49.000000 asap3-3.13.1/OpenKIMexport/asap_kim_api.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.937666 asap3-3.13.1/OpenKIMimport/
--rw-r--r--   0 schiotz    (501) staff       (20)    28447 2021-04-21 07:36:30.000000 asap3-3.13.1/OpenKIMimport/OpenKIMcalculator.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     7976 2021-04-21 07:36:30.000000 asap3-3.13.1/OpenKIMimport/OpenKIMcalculator.h
--rw-r--r--   0 schiotz    (501) staff       (20)    12077 2019-08-27 09:30:33.000000 asap3-3.13.1/OpenKIMimport/OpenKIMinterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2013 2018-12-20 11:50:47.000000 asap3-3.13.1/OpenKIMimport/OpenKIMinterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1196 2023-06-20 12:52:59.112280 asap3-3.13.1/PKG-INFO
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.944908 asap3-3.13.1/PTM/
--rw-r--r--   0 schiotz    (501) staff       (20)     1845 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/alloy_types.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      233 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/alloy_types.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     4388 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/canonical.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      321 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/canonical.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     8845 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/convex_hull_incremental.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      681 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/convex_hull_incremental.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)      381 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/cpp11compat.h
--rw-r--r--   0 schiotz    (501) staff       (20)      717 2018-03-16 09:47:56.000000 asap3-3.13.1/PTM/deformation_gradient.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2442 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/deformation_gradient.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     6830 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/fundamental_mappings.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)    72726 2018-03-16 09:47:56.000000 asap3-3.13.1/PTM/graph_data.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      703 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/graph_data.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     9906 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/index_ptm.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     6019 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/index_ptm.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2534 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/initialize_data.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      957 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/initialize_data.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3020 2018-03-16 09:47:56.000000 asap3-3.13.1/PTM/neighbour_ordering.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      269 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/neighbour_ordering.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1077 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/normalize_vertices.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      225 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/normalize_vertices.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     5775 2018-03-16 09:47:56.000000 asap3-3.13.1/PTM/ptm_constants.h
--rw-r--r--   0 schiotz    (501) staff       (20)      737 2018-03-16 09:47:56.000000 asap3-3.13.1/PTM/ptm_functions.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.946646 asap3-3.13.1/PTM/qcprot/
--rw-r--r--   0 schiotz    (501) staff       (20)    10723 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/qcprot/polar.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      456 2018-05-02 10:58:20.000000 asap3-3.13.1/PTM/qcprot/polar.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     8643 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/qcprot/quat.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      913 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/qcprot/quat.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3510 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/qcprot.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.947459 asap3-3.13.1/PTM/voronoi/
--rw-r--r--   0 schiotz    (501) staff       (20)    40630 2018-12-20 11:50:47.000000 asap3-3.13.1/PTM/voronoi/cell.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)    14009 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/voronoi/cell.hpp
--rw-r--r--   0 schiotz    (501) staff       (20)     5232 2018-02-22 12:09:10.000000 asap3-3.13.1/PTM/voronoi/config.hpp
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.951637 asap3-3.13.1/Parallel/
--rw-r--r--   0 schiotz    (501) staff       (20)     9090 2020-12-18 12:17:15.000000 asap3-3.13.1/Parallel/AsapMPI.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     4604 2020-12-18 12:17:15.000000 asap3-3.13.1/Parallel/AsapMPI.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3287 2018-02-22 12:09:10.000000 asap3-3.13.1/Parallel/DomainDecomposition.h
--rw-r--r--   0 schiotz    (501) staff       (20)    36534 2022-10-04 10:29:32.000000 asap3-3.13.1/Parallel/ParallelAtoms.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)    10284 2021-04-21 07:36:30.000000 asap3-3.13.1/Parallel/ParallelAtoms.h
--rw-r--r--   0 schiotz    (501) staff       (20)     6285 2021-04-21 07:36:30.000000 asap3-3.13.1/Parallel/ParallelPotential.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     4489 2021-04-21 07:36:30.000000 asap3-3.13.1/Parallel/ParallelPotential.h
--rw-r--r--   0 schiotz    (501) staff       (20)    15163 2019-05-02 07:07:18.000000 asap3-3.13.1/Parallel/RegularGridDecomposition.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3292 2018-02-22 12:09:10.000000 asap3-3.13.1/Parallel/RegularGridDecomposition.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.955860 asap3-3.13.1/ParallelInterface/
--rw-r--r--   0 schiotz    (501) staff       (20)     1414 2020-12-18 12:17:15.000000 asap3-3.13.1/ParallelInterface/AsapParallel.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2009 2019-05-02 07:07:18.000000 asap3-3.13.1/ParallelInterface/ParallelAtomsInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1501 2019-05-02 07:07:18.000000 asap3-3.13.1/ParallelInterface/ParallelAtomsInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     1739 2021-04-21 07:36:30.000000 asap3-3.13.1/ParallelInterface/ParallelNeighborListInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)      274 2018-02-22 12:09:10.000000 asap3-3.13.1/ParallelInterface/ParallelNeighborListInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3637 2019-05-02 07:07:18.000000 asap3-3.13.1/ParallelInterface/ParallelPotentialInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1430 2018-02-22 12:09:10.000000 asap3-3.13.1/ParallelInterface/ParallelPotentialInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)    29034 2021-04-28 13:34:24.000000 asap3-3.13.1/ParallelInterface/mpimodule.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1601 2020-12-18 12:17:15.000000 asap3-3.13.1/ParallelInterface/mpimodule.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.969296 asap3-3.13.1/Potentials/
--rw-r--r--   0 schiotz    (501) staff       (20)    59537 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/EMT.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     9845 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/EMT.h
--rw-r--r--   0 schiotz    (501) staff       (20)    27371 2019-08-27 09:30:33.000000 asap3-3.13.1/Potentials/EMT2013.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1846 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/EMT2013.h
--rw-r--r--   0 schiotz    (501) staff       (20)     8774 2019-02-01 09:12:08.000000 asap3-3.13.1/Potentials/EMTDefaultParameterProvider.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3169 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/EMTDefaultParameterProvider.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3910 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/EMTParameterProvider.h
--rw-r--r--   0 schiotz    (501) staff       (20)     6595 2019-08-27 09:30:33.000000 asap3-3.13.1/Potentials/EMTPythonParameterProvider.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1933 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/EMTPythonParameterProvider.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3732 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/EMTRasmussenParameterProvider.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1772 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/EMTRasmussenParameterProvider.h
--rw-r--r--   0 schiotz    (501) staff       (20)    21641 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/LennardJones.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     8865 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/LennardJones.h
--rw-r--r--   0 schiotz    (501) staff       (20)    26026 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/MetalOxideInterface.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     4835 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/MetalOxideInterface.h
--rw-r--r--   0 schiotz    (501) staff       (20)    24277 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/MetalOxideInterface2.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     5013 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/MetalOxideInterface2.h
--rw-r--r--   0 schiotz    (501) staff       (20)    11869 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/MonteCarloEMT.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2831 2018-12-20 11:50:47.000000 asap3-3.13.1/Potentials/MonteCarloEMT.h
--rw-r--r--   0 schiotz    (501) staff       (20)    18763 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/Morse.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     7918 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/Morse.h
--rw-r--r--   0 schiotz    (501) staff       (20)     3442 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/Potential.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     7293 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/Potential.h
--rw-r--r--   0 schiotz    (501) staff       (20)    12111 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/RGL.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3345 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/RGL.h
--rw-r--r--   0 schiotz    (501) staff       (20)    19344 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/RahmanStillingerLemberg.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     8831 2021-04-21 07:36:30.000000 asap3-3.13.1/Potentials/RahmanStillingerLemberg.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.874796 asap3-3.13.1/Python/
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.976886 asap3-3.13.1/Python/asap3/
--rw-r--r--   0 schiotz    (501) staff       (20)      190 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/EMT2011Parameters.py
--rw-r--r--   0 schiotz    (501) staff       (20)    23300 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/EMT2011_py.py
--rw-r--r--   0 schiotz    (501) staff       (20)    11742 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/EMT2013Parameters.py
--rw-r--r--   0 schiotz    (501) staff       (20)      278 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/GuptaParameters.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.984718 asap3-3.13.1/Python/asap3/Internal/
--rw-r--r--   0 schiotz    (501) staff       (20)    24089 2021-04-21 07:36:30.000000 asap3-3.13.1/Python/asap3/Internal/BuiltinPotentials.py
--rw-r--r--   0 schiotz    (501) staff       (20)      580 2019-08-27 09:30:33.000000 asap3-3.13.1/Python/asap3/Internal/Builtins.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1493 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/CheckArray.py
--rw-r--r--   0 schiotz    (501) staff       (20)     6635 2021-04-19 09:25:32.000000 asap3-3.13.1/Python/asap3/Internal/Collector.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.985112 asap3-3.13.1/Python/asap3/Internal/Compatibility/
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/Compatibility/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     8779 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/EMTParameters.py
--rw-r--r--   0 schiotz    (501) staff       (20)      570 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/ListOfElements.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2466 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/MonteCarloAtoms.py
--rw-r--r--   0 schiotz    (501) staff       (20)    15745 2019-08-27 09:30:33.000000 asap3-3.13.1/Python/asap3/Internal/OpenKIMcalculator.py
--rw-r--r--   0 schiotz    (501) staff       (20)    25207 2022-04-22 14:31:57.000000 asap3-3.13.1/Python/asap3/Internal/ParallelListOfAtoms.py
--rw-r--r--   0 schiotz    (501) staff       (20)      713 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/Subject.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4731 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/Threads.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4438 2021-04-02 21:05:52.000000 asap3-3.13.1/Python/asap3/Internal/UtilityFunctions.py
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1100 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Internal/checkversion.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.987921 asap3-3.13.1/Python/asap3/MonteCarlo/
--rw-r--r--   0 schiotz    (501) staff       (20)     6052 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Base.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1308 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Basin.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1045 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Metropolis.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.989078 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/
--rw-r--r--   0 schiotz    (501) staff       (20)    10336 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Base.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.990192 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Data/
--rw-r--r--   0 schiotz    (501) staff       (20)      196 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Data/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)    10422 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Data/fcc.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2860 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Data/symmetry.py
--rw-r--r--   0 schiotz    (501) staff       (20)    15256 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Surface.py
--rw-r--r--   0 schiotz    (501) staff       (20)      307 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Moves/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2179 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/Start.py
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/MonteCarlo/__init__.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:58.994064 asap3-3.13.1/Python/asap3/Tools/
--rwxr-xr-x   0 schiotz    (501) staff       (20)     4900 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/AsapFileToTrajectory.py
--rw-r--r--   0 schiotz    (501) staff       (20)      615 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/AtomicEnergies.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3168 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/EMT_two_atom_test.py
--rw-r--r--   0 schiotz    (501) staff       (20)     8449 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ElasticConstants.py
--rw-r--r--   0 schiotz    (501) staff       (20)     5472 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/MaterialProperties.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4893 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/OptimizationDatabase.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.000026 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/
--rw-r--r--   0 schiotz    (501) staff       (20)     6337 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/EMT.py
--rw-r--r--   0 schiotz    (501) staff       (20)      856 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/GetParameters.py
--rw-r--r--   0 schiotz    (501) staff       (20)    17545 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Optimization.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2038 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Performance.py
--rw-r--r--   0 schiotz    (501) staff       (20)    36185 2019-11-14 09:46:19.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Quantities.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2541 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/RGL.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2809 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Sampling.py
--rw-r--r--   0 schiotz    (501) staff       (20)    64144 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/ScipyFmin.py
--rw-r--r--   0 schiotz    (501) staff       (20)     7726 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Search.py
--rw-r--r--   0 schiotz    (501) staff       (20)    11789 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/SearchParallel.py
--rw-r--r--   0 schiotz    (501) staff       (20)      303 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4969 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/SurfaceEnergies.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4839 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/Timing.py
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)      793 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/Tools/niflheim.py
--rw-r--r--   0 schiotz    (501) staff       (20)     5285 2020-12-18 12:17:15.000000 asap3-3.13.1/Python/asap3/__init__.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.005259 asap3-3.13.1/Python/asap3/analysis/
--rw-r--r--   0 schiotz    (501) staff       (20)      278 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/analysis/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     6218 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/analysis/averagepositions.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4063 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/analysis/clusterposition.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2401 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/analysis/cutcluster.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4933 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/analysis/findcluster.py
--rw-r--r--   0 schiotz    (501) staff       (20)    11390 2019-08-21 16:06:34.000000 asap3-3.13.1/Python/asap3/analysis/localstructure.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2975 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/analysis/particle.py
--rw-r--r--   0 schiotz    (501) staff       (20)    12466 2019-08-27 09:30:33.000000 asap3-3.13.1/Python/asap3/analysis/ptm.py
--rw-r--r--   0 schiotz    (501) staff       (20)    12199 2019-08-21 16:06:34.000000 asap3-3.13.1/Python/asap3/analysis/rdf.py
--rw-r--r--   0 schiotz    (501) staff       (20)     5998 2022-07-17 10:13:48.000000 asap3-3.13.1/Python/asap3/constraints.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1242 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/fixepydoc.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.008148 asap3-3.13.1/Python/asap3/io/
--rw-r--r--   0 schiotz    (501) staff       (20)     3135 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/io/ReadOldFiles.py
--rw-r--r--   0 schiotz    (501) staff       (20)      189 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/io/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)    19539 2020-12-18 12:17:15.000000 asap3-3.13.1/Python/asap3/io/bundletrajectory.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1536 2020-12-18 12:17:15.000000 asap3-3.13.1/Python/asap3/io/cpu_setup.py
--rw-r--r--   0 schiotz    (501) staff       (20)     6961 2020-12-18 12:17:15.000000 asap3-3.13.1/Python/asap3/io/trajectory.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.013394 asap3-3.13.1/Python/asap3/md/
--rw-r--r--   0 schiotz    (501) staff       (20)      117 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/md/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)    10212 2022-04-22 13:42:31.000000 asap3-3.13.1/Python/asap3/md/langevin.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2289 2022-04-22 13:50:17.000000 asap3-3.13.1/Python/asap3/md/md.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2731 2020-12-18 12:17:15.000000 asap3-3.13.1/Python/asap3/md/npt.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3774 2022-07-09 17:08:58.000000 asap3-3.13.1/Python/asap3/md/nptberendsen.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2299 2022-04-22 13:50:38.000000 asap3-3.13.1/Python/asap3/md/nvtberendsen.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3755 2021-03-29 12:08:48.000000 asap3-3.13.1/Python/asap3/md/velocitydistribution.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2667 2022-04-22 14:31:46.000000 asap3-3.13.1/Python/asap3/md/verlet.py
--rw-r--r--   0 schiotz    (501) staff       (20)      505 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/memory.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3268 2019-08-27 09:30:33.000000 asap3-3.13.1/Python/asap3/mpi.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.018991 asap3-3.13.1/Python/asap3/nanoparticle_mc/
--rw-r--r--   0 schiotz    (501) staff       (20)     1511 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/AdsCalc.py
--rw-r--r--   0 schiotz    (501) staff       (20)      767 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/Logger.py
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     9541 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/atommontecarlodata.py
--rw-r--r--   0 schiotz    (501) staff       (20)    17753 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/cluster.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4763 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/clusteratom.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.020568 asap3-3.13.1/Python/asap3/nanoparticle_mc/data/
--rw-r--r--   0 schiotz    (501) staff       (20)      253 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/data/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)      673 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/data/au.py
--rw-r--r--   0 schiotz    (501) staff       (20)    10413 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/data/fcc.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2860 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/data/symmetry.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1558 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/langmuirExpression.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1280 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/mc_result.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.021775 asap3-3.13.1/Python/asap3/nanoparticle_mc/montecarlo/
--rw-r--r--   0 schiotz    (501) staff       (20)      379 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/montecarlo/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)    40041 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/montecarlo/atom.py
--rw-r--r--   0 schiotz    (501) staff       (20)    25368 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/montecarlo/surface.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1809 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/nanoparticle_mc/resizecluster.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.024110 asap3-3.13.1/Python/asap3/optimize/
--rw-r--r--   0 schiotz    (501) staff       (20)       76 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/optimize/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2186 2020-05-25 16:01:27.000000 asap3-3.13.1/Python/asap3/optimize/fire.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1093 2019-04-15 16:57:05.000000 asap3-3.13.1/Python/asap3/optimize/mdmin.py
--rw-r--r--   0 schiotz    (501) staff       (20)      553 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/optimize/optimize.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.026001 asap3-3.13.1/Python/asap3/setup/
--rw-r--r--   0 schiotz    (501) staff       (20)      778 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/VelocityDistribution.py
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     9849 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/dislocation.py
--rw-r--r--   0 schiotz    (501) staff       (20)     7007 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/displacementfield.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4290 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/multidislocation.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.029044 asap3-3.13.1/Python/asap3/setup/nanocrystalline/
--rw-r--r--   0 schiotz    (501) staff       (20)      363 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2831 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/dislocated.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1372 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/energy.py
--rw-r--r--   0 schiotz    (501) staff       (20)     8521 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/grain_structures.py
--rw-r--r--   0 schiotz    (501) staff       (20)     7786 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/helpers.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1689 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/nanocrystalline.py
--rw-r--r--   0 schiotz    (501) staff       (20)    13481 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/nanocrystalline_orig.py
--rw-r--r--   0 schiotz    (501) staff       (20)      570 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/plane_utils.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4342 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/setup/nanocrystalline/quat_utils.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4548 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/testtools.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2701 2018-02-22 12:09:10.000000 asap3-3.13.1/Python/asap3/timing.py
--rw-r--r--   0 schiotz    (501) staff       (20)      643 2023-06-16 10:38:41.000000 asap3-3.13.1/Python/asap3/version.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.031237 asap3-3.13.1/Python/asap3/visualize/
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2020-09-29 12:35:59.000000 asap3-3.13.1/Python/asap3/visualize/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)    39540 2020-09-29 12:35:59.000000 asap3-3.13.1/Python/asap3/visualize/colortable.py
--rw-r--r--   0 schiotz    (501) staff       (20)    11032 2020-09-29 12:35:59.000000 asap3-3.13.1/Python/asap3/visualize/fieldplotter.py
--rw-r--r--   0 schiotz    (501) staff       (20)    35788 2023-06-16 10:38:41.000000 asap3-3.13.1/Python/asap3/visualize/primiplotter.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1953 2022-04-28 11:01:10.000000 asap3-3.13.1/README.rst
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.075210 asap3-3.13.1/Test/
--rw-r--r--   0 schiotz    (501) staff       (20)     2823 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/Berendsen.py
--rw-r--r--   0 schiotz    (501) staff       (20)    16918 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/BrennerNanotube.py
--rw-r--r--   0 schiotz    (501) staff       (20)      825 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/BrennerPullNanotube.py
--rw-r--r--   0 schiotz    (501) staff       (20)    10792 2023-06-16 10:38:41.000000 asap3-3.13.1/Test/BrennerStress.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2992 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/BundleTrajectory.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2033 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/CNAleak.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1506 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/CalculationRequired.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1717 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/ChangeAtoms.py
--rw-r--r--   0 schiotz    (501) staff       (20)      699 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/ChangeAtoms2.py
--rw-r--r--   0 schiotz    (501) staff       (20)      814 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/ChangeCalculator.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2319 2022-04-22 13:27:20.000000 asap3-3.13.1/Test/ChangeConstraint.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2621 2021-04-11 13:15:55.000000 asap3-3.13.1/Test/ChangePeriodicity.py
--rw-r--r--   0 schiotz    (501) staff       (20)      975 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/ChangeUnitCell.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1361 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/ChangeUnitCell2.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1240 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/ConstraintInTraj.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3165 2022-04-22 11:28:45.000000 asap3-3.13.1/Test/Constraints.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1048 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/EMT2013elements.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2133 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/EMTleak.py
--rw-r--r--   0 schiotz    (501) staff       (20)      752 2019-11-13 12:25:20.000000 asap3-3.13.1/Test/Exception.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1669 2021-11-08 08:40:53.000000 asap3-3.13.1/Test/ExplicitMasses.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1026 2019-08-21 16:06:34.000000 asap3-3.13.1/Test/FIRE.py
--rw-r--r--   0 schiotz    (501) staff       (20)      698 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/FieldPlotter.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1334 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/FixAtoms_Lgv.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4893 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Hydrocarbons.py
--rw-r--r--   0 schiotz    (501) staff       (20)      722 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/LJ_Stress.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1449 2021-10-08 12:17:29.000000 asap3-3.13.1/Test/Langevin.py
--rw-r--r--   0 schiotz    (501) staff       (20)      851 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/LangevinSeed.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1141 2022-02-07 17:11:04.000000 asap3-3.13.1/Test/Langevin_COM.py
--rw-r--r--   0 schiotz    (501) staff       (20)      794 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/LargeShear.py
--rw-r--r--   0 schiotz    (501) staff       (20)     6882 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Lattice.py
--rwxr-xr-x   0 schiotz    (501) staff       (20)    10062 2023-06-16 10:38:41.000000 asap3-3.13.1/Test/LennardJones.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2443 2021-02-02 09:15:27.000000 asap3-3.13.1/Test/LennardJonesDimer.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1837 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/LocalStructure.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1345 2020-09-29 12:35:59.000000 asap3-3.13.1/Test/MakeDislocation.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4853 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/MonteCarloOptim_Alloy.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4089 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/MonteCarloOptim_Energy.py
--rw-r--r--   0 schiotz    (501) staff       (20)     5159 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/MonteCarloOptim_NbList.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3065 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/Morse.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2015 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/NPT.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3475 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/NbCellLocator.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3985 2020-12-18 12:17:10.000000 asap3-3.13.1/Test/NbCellLocatorQueryPoint.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3864 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/NeighborList.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2064 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/NoInterference.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1159 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/NoMI_LeftHanded.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1261 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/NotImplemented.py
--rw-r--r--   0 schiotz    (501) staff       (20)     6458 2021-06-07 10:17:26.000000 asap3-3.13.1/Test/OpenKIM_AllModels.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1704 2018-12-20 11:50:47.000000 asap3-3.13.1/Test/OpenKIM_ArLJ.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3413 2019-11-25 11:45:09.000000 asap3-3.13.1/Test/OpenKIM_EMT.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1479 2021-03-02 14:24:58.000000 asap3-3.13.1/Test/OpenKIM_LJ_PModif.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1746 2018-12-20 11:50:47.000000 asap3-3.13.1/Test/OpenKIM_MultiNbList.py
--rw-r--r--   0 schiotz    (501) staff       (20)      796 2019-03-29 15:16:07.000000 asap3-3.13.1/Test/OpenKIM_modelname.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1704 2019-11-25 12:28:38.000000 asap3-3.13.1/Test/PBCwrap.py
--rw-r--r--   0 schiotz    (501) staff       (20)     5705 2019-11-25 11:45:09.000000 asap3-3.13.1/Test/Potentials.py
--rw-r--r--   0 schiotz    (501) staff       (20)      481 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/PrintMemory.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2071 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/RDF.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3029 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/RDF2.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2818 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/RawRDF.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2113 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/RawRDF2.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2372 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/SizeConsist_EMT.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2297 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/SizeConsist_EMT2013.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1359 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/SizeConsist_LeftHand.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1623 2018-12-20 11:50:47.000000 asap3-3.13.1/Test/SizeConsist_OpenKIM.py
--rw-r--r--   0 schiotz    (501) staff       (20)   298761 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/SpecialEMT.pickle
--rw-r--r--   0 schiotz    (501) staff       (20)     3169 2019-08-27 09:30:33.000000 asap3-3.13.1/Test/SpecialEMT.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1066 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/StdParamProv.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3337 2023-06-16 10:38:41.000000 asap3-3.13.1/Test/Stress.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1965 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/StressCrash.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1747 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/StressFilter.py
--rw-r--r--   0 schiotz    (501) staff       (20)    10668 2023-06-16 10:38:41.000000 asap3-3.13.1/Test/StressModule.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1680 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Subset.py
--rw-r--r--   0 schiotz    (501) staff       (20)     7887 2021-10-08 12:17:29.000000 asap3-3.13.1/Test/TestAll.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.082078 asap3-3.13.1/Test/Timing/
--rwxr-xr-x   0 schiotz    (501) staff       (20)     6683 2019-08-27 09:30:33.000000 asap3-3.13.1/Test/Timing/BigTiming.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3706 2019-11-14 09:48:34.000000 asap3-3.13.1/Test/Timing/MonteCarloTiming.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1840 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/Morse.py
--rw-r--r--   0 schiotz    (501) staff       (20)     6392 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/OfficialTiming.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3381 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/OpenKIM_MemLeak.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4212 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/OpenKIM_ParTiming.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3213 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/OpenKIM_Profiling.py
--rw-r--r--   0 schiotz    (501) staff       (20)     9019 2019-08-21 16:06:34.000000 asap3-3.13.1/Test/Timing/ParallelTiming.py
--rw-r--r--   0 schiotz    (501) staff       (20)      739 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/ThreadForceTiming.py
--rwxr-xr-x   0 schiotz    (501) staff       (20)     6528 2021-02-01 16:44:51.000000 asap3-3.13.1/Test/Timing/Timing.py
--rwxr-xr-x   0 schiotz    (501) staff       (20)     6522 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/TimingEMT2013.py
--rwxr-xr-x   0 schiotz    (501) staff       (20)     3498 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/TimingLangevin.py
--rwxr-xr-x   0 schiotz    (501) staff       (20)     3108 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Timing/TimingVerlet.py
--rwxr-xr-x   0 schiotz    (501) staff       (20)     6561 2020-03-15 14:32:31.000000 asap3-3.13.1/Test/Timing/Timing_OpenKIM.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3630 2022-02-07 17:27:24.000000 asap3-3.13.1/Test/TinyLangevin.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2666 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Trajectories.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2045 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/Trajectories_ase.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1715 2019-11-25 11:45:09.000000 asap3-3.13.1/Test/Verlet.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2177 2019-08-27 09:30:33.000000 asap3-3.13.1/Test/Verlet_OpenKIM.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2083 2019-11-25 11:45:09.000000 asap3-3.13.1/Test/Verlet_legacymass.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2127 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/ase_emt.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.102257 asap3-3.13.1/Test/parallel/
--rw-r--r--   0 schiotz    (501) staff       (20)     1596 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/parallel/Force1D.py
--rw-r--r--   0 schiotz    (501) staff       (20)        0 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/parallel/__init__.py
--rw-r--r--   0 schiotz    (501) staff       (20)      229 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/parallel/ase_before_asap.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1022 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/parallel/autodistribution.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2781 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/parallel/bundleTrajPreserveZ.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1914 2020-03-16 08:43:46.000000 asap3-3.13.1/Test/parallel/emptyNode.py
--rw-r--r--   0 schiotz    (501) staff       (20)     6521 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/parallel/longMelting.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2265 2019-08-21 16:06:34.000000 asap3-3.13.1/Test/parallel/makeparallel.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1722 2020-03-16 08:43:46.000000 asap3-3.13.1/Test/parallel/migration.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1963 2019-08-21 16:06:34.000000 asap3-3.13.1/Test/parallel/moveatoms.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3244 2019-08-21 16:06:34.000000 asap3-3.13.1/Test/parallel/moveatomsLJ.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3043 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/parallel/parallelBundleTrajectories.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2991 2022-04-22 13:38:45.000000 asap3-3.13.1/Test/parallel/parallelChangeConstraints.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4883 2022-07-17 09:49:05.000000 asap3-3.13.1/Test/parallel/parallelConstraints.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2351 2021-04-21 07:36:30.000000 asap3-3.13.1/Test/parallel/parallelDeleteAtoms.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1650 2019-08-21 16:06:34.000000 asap3-3.13.1/Test/parallel/parallelFIRE.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1666 2021-08-26 13:59:42.000000 asap3-3.13.1/Test/parallel/parallelFixatomTemperature.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1414 2021-04-19 09:25:32.000000 asap3-3.13.1/Test/parallel/parallelFixatomTrajectory.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3682 2021-10-08 12:17:29.000000 asap3-3.13.1/Test/parallel/parallelLangevin.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3055 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelLennardJones.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2518 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelLocalStructure.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3408 2021-10-08 12:17:29.000000 asap3-3.13.1/Test/parallel/parallelLongVerlet.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3927 2020-12-18 12:17:15.000000 asap3-3.13.1/Test/parallel/parallelNPT.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2732 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelNeighborLocator.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2119 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelOpenKIM_ArLJ.py
--rw-r--r--   0 schiotz    (501) staff       (20)     5458 2019-08-27 09:30:33.000000 asap3-3.13.1/Test/parallel/parallelOpenKIM_EMT.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2192 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelOpenKIM_MultiNbList.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1489 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelPBC.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1626 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelPBC2.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4842 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelPTM.py
--rw-r--r--   0 schiotz    (501) staff       (20)   123573 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/parallel/parallelPotentials.pickle
--rw-r--r--   0 schiotz    (501) staff       (20)     7279 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/parallel/parallelPotentials.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3456 2020-09-29 12:35:59.000000 asap3-3.13.1/Test/parallel/parallelPrimiPlot.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2680 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelRDF.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2929 2021-04-21 07:36:30.000000 asap3-3.13.1/Test/parallel/parallelSafeNbList.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3948 2023-06-16 10:38:41.000000 asap3-3.13.1/Test/parallel/parallelStress.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2903 2021-04-19 09:25:32.000000 asap3-3.13.1/Test/parallel/parallelTrajectories.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2799 2021-03-29 15:54:10.000000 asap3-3.13.1/Test/parallel/parallelVelocityDistribution.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4572 2019-08-21 16:06:35.000000 asap3-3.13.1/Test/parallel/parallelVerlet.py
--rw-r--r--   0 schiotz    (501) staff       (20)     2317 2019-10-08 11:12:11.000000 asap3-3.13.1/Test/parallel/simplempi.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3079 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/parallel/splitBundleTrajectories.py
--rw-r--r--   0 schiotz    (501) staff       (20)    36496 2018-02-22 12:09:10.000000 asap3-3.13.1/Test/potResults.py
--rw-r--r--   0 schiotz    (501) staff       (20)     3690 2019-05-02 07:18:13.000000 asap3-3.13.1/Test/ptm.py
--rw-r--r--   0 schiotz    (501) staff       (20)     4140 2019-11-25 11:45:09.000000 asap3-3.13.1/Test/test_reproducible.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.109151 asap3-3.13.1/Tools/
--rw-r--r--   0 schiotz    (501) staff       (20)     3656 2021-04-21 07:36:30.000000 asap3-3.13.1/Tools/CNA.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1345 2018-02-22 12:09:10.000000 asap3-3.13.1/Tools/CNA.h
--rw-r--r--   0 schiotz    (501) staff       (20)     2558 2021-04-11 12:40:22.000000 asap3-3.13.1/Tools/CoordinationNumbers.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1424 2018-02-22 12:09:10.000000 asap3-3.13.1/Tools/CoordinationNumbers.h
--rw-r--r--   0 schiotz    (501) staff       (20)    17922 2018-12-20 11:50:47.000000 asap3-3.13.1/Tools/FullCNA.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3419 2018-02-22 12:09:10.000000 asap3-3.13.1/Tools/FullCNA.h
--rw-r--r--   0 schiotz    (501) staff       (20)     4744 2021-04-21 07:36:30.000000 asap3-3.13.1/Tools/GetNeighborList.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     1849 2018-02-22 12:09:10.000000 asap3-3.13.1/Tools/GetNeighborList.h
--rw-r--r--   0 schiotz    (501) staff       (20)     4698 2018-12-20 11:50:47.000000 asap3-3.13.1/Tools/RawRadialDistribution.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     2780 2018-02-22 12:09:10.000000 asap3-3.13.1/Tools/RawRadialDistribution.h
--rw-r--r--   0 schiotz    (501) staff       (20)     4614 2021-04-21 07:36:30.000000 asap3-3.13.1/Tools/SecondaryNeighborLocator.cpp
--rw-r--r--   0 schiotz    (501) staff       (20)     3446 2021-04-16 17:39:43.000000 asap3-3.13.1/Tools/SecondaryNeighborLocator.h
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.110770 asap3-3.13.1/asap3.egg-info/
--rw-r--r--   0 schiotz    (501) staff       (20)     1196 2023-06-20 12:52:58.000000 asap3-3.13.1/asap3.egg-info/PKG-INFO
--rw-r--r--   0 schiotz    (501) staff       (20)    14076 2023-06-20 12:52:58.000000 asap3-3.13.1/asap3.egg-info/SOURCES.txt
--rw-r--r--   0 schiotz    (501) staff       (20)        1 2023-06-20 12:52:58.000000 asap3-3.13.1/asap3.egg-info/dependency_links.txt
--rw-r--r--   0 schiotz    (501) staff       (20)       12 2023-06-20 12:52:58.000000 asap3-3.13.1/asap3.egg-info/requires.txt
--rw-r--r--   0 schiotz    (501) staff       (20)       12 2023-06-20 12:52:58.000000 asap3-3.13.1/asap3.egg-info/top_level.txt
--rw-r--r--   0 schiotz    (501) staff       (20)      371 2018-02-22 12:09:10.000000 asap3-3.13.1/asapmpiinfo-input.py
--rwxr-xr-x   0 schiotz    (501) staff       (20)     1528 2021-10-08 12:17:29.000000 asap3-3.13.1/compile-niflheim.sh
--rw-r--r--   0 schiotz    (501) staff       (20)     4008 2021-04-21 07:36:30.000000 asap3-3.13.1/depend.CHANGES
--rwxr-xr-x   0 schiotz    (501) staff       (20)      825 2018-02-22 12:09:10.000000 asap3-3.13.1/getconfig.py
--rw-r--r--   0 schiotz    (501) staff       (20)     1002 2020-12-18 12:17:15.000000 asap3-3.13.1/makefile-Darwin-x86_64
--rw-r--r--   0 schiotz    (501) staff       (20)     1947 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Linux-x86_64-gnu
--rw-r--r--   0 schiotz    (501) staff       (20)     1701 2018-05-02 10:58:20.000000 asap3-3.13.1/makefile-Linux-x86_64-intel
--rw-r--r--   0 schiotz    (501) staff       (20)       31 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Nifl7_broadwell_foss
--rw-r--r--   0 schiotz    (501) staff       (20)       27 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Nifl7_broadwell_intel
--rw-r--r--   0 schiotz    (501) staff       (20)       31 2021-10-08 12:17:29.000000 asap3-3.13.1/makefile-Nifl7_icelake_foss
--rw-r--r--   0 schiotz    (501) staff       (20)       27 2021-10-08 12:17:29.000000 asap3-3.13.1/makefile-Nifl7_icelake_intel
--rw-r--r--   0 schiotz    (501) staff       (20)       31 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Nifl7_nehalem_foss
--rw-r--r--   0 schiotz    (501) staff       (20)       27 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Nifl7_nehalem_intel
--rw-r--r--   0 schiotz    (501) staff       (20)       31 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Nifl7_sandybridge_foss
--rw-r--r--   0 schiotz    (501) staff       (20)       27 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Nifl7_sandybridge_intel
--rw-r--r--   0 schiotz    (501) staff       (20)       31 2019-02-28 12:45:34.000000 asap3-3.13.1/makefile-Nifl7_skylake_foss
--rw-r--r--   0 schiotz    (501) staff       (20)       27 2019-02-28 12:45:34.000000 asap3-3.13.1/makefile-Nifl7_skylake_intel
--rw-r--r--   0 schiotz    (501) staff       (20)     1816 2020-12-18 12:17:15.000000 asap3-3.13.1/makefile-Niflheim7
--rw-r--r--   0 schiotz    (501) staff       (20)     1899 2018-12-20 11:50:47.000000 asap3-3.13.1/makefile-Niflheim7-gcc
--rw-r--r--   0 schiotz    (501) staff       (20)     1751 2018-05-02 10:58:20.000000 asap3-3.13.1/makefile-Niflheim7-gcc-mkl
--rw-r--r--   0 schiotz    (501) staff       (20)      348 2018-02-22 12:09:10.000000 asap3-3.13.1/makefile-default
--rw-r--r--   0 schiotz    (501) staff       (20)     1002 2021-05-27 12:16:26.000000 asap3-3.13.1/makefile-local
--rw-r--r--   0 schiotz    (501) staff       (20)     2219 2018-05-02 10:58:20.000000 asap3-3.13.1/makefile-local-gcc-svml
--rw-r--r--   0 schiotz    (501) staff       (20)     1100 2023-06-16 10:38:41.000000 asap3-3.13.1/recordversion.py
-drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2023-06-20 12:52:59.111516 asap3-3.13.1/scripts/
--rwxr-xr-x   0 schiotz    (501) staff       (20)     6577 2018-02-22 12:09:10.000000 asap3-3.13.1/scripts/asap-qsub
--rwxr-xr-x   0 schiotz    (501) staff       (20)     6423 2021-02-01 16:44:51.000000 asap3-3.13.1/scripts/asap-sbatch
--rw-r--r--   0 schiotz    (501) staff       (20)       38 2023-06-20 12:52:59.112708 asap3-3.13.1/setup.cfg
--rw-r--r--   0 schiotz    (501) staff       (20)     9358 2023-06-16 10:38:41.000000 asap3-3.13.1/setup.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Archive/
+-rw-r--r--   0 schiotz    (501) staff       (20)    29406 2016-10-18 11:47:04.000000 asap3-3.9.6/Archive/MoPotential.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3137 2016-10-18 11:47:04.000000 asap3-3.9.6/Archive/MoPotential.h
+-rw-r--r--   0 schiotz    (501) staff       (20)      371 2016-08-26 07:18:44.000000 asap3-3.9.6/asapmpiinfo-input.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Basics/
+-rw-r--r--   0 schiotz    (501) staff       (20)     4882 2016-10-10 07:26:38.000000 asap3-3.9.6/Basics/Asap.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1461 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/AsapNamespace.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1849 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/AsapObject.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1945 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/AsapObject.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3846 2016-10-14 09:28:52.000000 asap3-3.9.6/Basics/AsapPython.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1670 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Atoms.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     8967 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/AtomsBasis.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2988 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Debug.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3696 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Debug.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     6618 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/DynamicAtoms.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2150 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/DynamicAtoms.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    48208 2016-09-28 13:11:16.000000 asap3-3.9.6/Basics/EMT.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     9501 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/EMT.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    27374 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/EMT2013.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1846 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/EMT2013.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     8733 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/EMTDefaultParameterProvider.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3169 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/EMTDefaultParameterProvider.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3910 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/EMTParameterProvider.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     6680 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/EMTPythonParameterProvider.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1933 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/EMTPythonParameterProvider.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3732 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/EMTRasmussenParameterProvider.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1772 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/EMTRasmussenParameterProvider.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3384 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Exception.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     6559 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Exception.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     8327 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/ImageAtoms.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    10145 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/ImageAtoms.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4224 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/ImagePotential.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     4137 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/ImagePotential.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4710 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/IVec.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     8002 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Langevin.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3141 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Langevin.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    21330 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/LennardJones.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     8507 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/LennardJones.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2149 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/mass.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1838 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Matrix3x3.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1666 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Matrix3x3.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    21465 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/MetalOxideInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     4272 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/MetalOxideInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    20655 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/MetalOxideInterface2.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     4445 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/MetalOxideInterface2.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     7304 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/MolecularDynamics.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2673 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/MolecularDynamics.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3718 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/MonteCarloAtoms.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1986 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/MonteCarloAtoms.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    11869 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/MonteCarloEMT.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2831 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/MonteCarloEMT.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    18701 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/Morse.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     7541 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/Morse.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    40139 2016-10-14 08:58:12.000000 asap3-3.9.6/Basics/NeighborCellLocator.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    10991 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/NeighborCellLocator.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    28196 2016-09-28 13:12:03.000000 asap3-3.9.6/Basics/NeighborList.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     9018 2016-09-28 12:57:47.000000 asap3-3.9.6/Basics/NeighborList.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3772 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/NeighborList2013.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1729 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/NeighborList2013.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     6420 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/NeighborLocator.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    26273 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/NormalAtoms.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    11416 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/NormalAtoms.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     5092 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Potential.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     7155 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/Potential.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    17247 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/RahmanStillingerLemberg.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     8732 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/RahmanStillingerLemberg.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4296 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/RandomNumbers.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      703 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/RandomNumbers.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    11941 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/RGL.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2956 2016-09-25 11:57:10.000000 asap3-3.9.6/Basics/RGL.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    12835 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/stacktrace.c
+-rw-r--r--   0 schiotz    (501) staff       (20)     1387 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/stacktrace.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2859 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/SymTensor.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3095 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Timing.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     7881 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Timing.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1694 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/TimingResults.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2874 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/TinyMatrix.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1679 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Vec.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     5241 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/Vec.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3711 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/VelocityVerlet.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2133 2016-08-26 07:18:44.000000 asap3-3.9.6/Basics/VelocityVerlet.h
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Brenner/
+-rw-r--r--   0 schiotz    (501) staff       (20)     1297 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/asapbrenner.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2207 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/AtomPairInfoState.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     6617 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/bcuint.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     6083 2016-09-25 11:57:10.000000 asap3-3.9.6/Brenner/BrennerPotential.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     6980 2016-09-25 11:57:10.000000 asap3-3.9.6/Brenner/BrennerPotential.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     8842 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/caguts.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      661 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/expand.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      278 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/expand.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     9037 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/inter2d_iv.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     8997 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/mtable.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    37861 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/pibond.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    11916 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/radic.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)   387465 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/radicdata.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     5692 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/sili_germ.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1631 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/spgch.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      188 2016-08-26 07:18:44.000000 asap3-3.9.6/Brenner/spgch.h
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     1132 2016-10-14 09:06:40.000000 asap3-3.9.6/compile-niflheim.sh
+-rw-r--r--   0 schiotz    (501) staff       (20)     1951 2016-10-26 09:21:42.000000 asap3-3.9.6/customize.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3530 2016-10-11 20:08:52.000000 asap3-3.9.6/depend.CHANGES
+-rwxr-xr-x   0 schiotz    (501) staff       (20)      825 2016-10-12 12:27:01.000000 asap3-3.9.6/getconfig.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Interface/
+-rw-r--r--   0 schiotz    (501) staff       (20)     7945 2016-09-25 11:57:10.000000 asap3-3.9.6/Interface/AsapModule.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1347 2016-09-25 11:57:10.000000 asap3-3.9.6/Interface/AsapModule.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1516 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/AsapSerial.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    10024 2016-09-25 11:57:10.000000 asap3-3.9.6/Interface/DynamicsInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1619 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/DynamicsInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     5890 2016-09-25 11:57:10.000000 asap3-3.9.6/Interface/EMTParameterProviderInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1902 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/EMTParameterProviderInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1474 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/ExceptionInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2752 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/ExceptionInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    16450 2016-09-25 11:57:10.000000 asap3-3.9.6/Interface/NeighborLocatorInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2790 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/NeighborLocatorInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3751 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/OpenMPInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1764 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/OpenMPInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    36765 2016-09-25 11:57:10.000000 asap3-3.9.6/Interface/PotentialInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1741 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/PotentialInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    11762 2016-10-25 07:17:57.000000 asap3-3.9.6/Interface/PTMInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1484 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/PTMInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3356 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/PythonConversions.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3697 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/PythonConversions.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     7401 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/RDFInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1446 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/RDFInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1744 2016-09-25 11:57:16.000000 asap3-3.9.6/Interface/Templates.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     5487 2016-09-25 11:57:10.000000 asap3-3.9.6/Interface/ToolsInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1838 2016-08-26 07:18:44.000000 asap3-3.9.6/Interface/ToolsInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    35147 2016-08-26 07:18:44.000000 asap3-3.9.6/LICENSE
+-rw-r--r--   0 schiotz    (501) staff       (20)     7651 2016-08-26 07:18:44.000000 asap3-3.9.6/LICENSE.LESSER
+-rw-r--r--   0 schiotz    (501) staff       (20)    24056 2016-10-26 09:21:42.000000 asap3-3.9.6/Makefile
+-rw-r--r--   0 schiotz    (501) staff       (20)      840 2016-09-25 11:57:03.000000 asap3-3.9.6/makefile-Darwin-x86_64
+-rw-r--r--   0 schiotz    (501) staff       (20)      348 2016-08-26 07:18:44.000000 asap3-3.9.6/makefile-default
+-rw-r--r--   0 schiotz    (501) staff       (20)       27 2016-08-26 07:18:44.000000 asap3-3.9.6/makefile-dl160g6-el6
+-rw-r--r--   0 schiotz    (501) staff       (20)     1918 2016-10-12 10:47:33.000000 asap3-3.9.6/makefile-Linux-i686-gnu
+-rw-r--r--   0 schiotz    (501) staff       (20)      542 2016-08-26 07:18:44.000000 asap3-3.9.6/makefile-Linux-i686-intel
+-rw-r--r--   0 schiotz    (501) staff       (20)     1915 2016-10-12 10:47:33.000000 asap3-3.9.6/makefile-Linux-x86_64-gnu
+-rw-r--r--   0 schiotz    (501) staff       (20)     1728 2016-10-14 08:58:12.000000 asap3-3.9.6/makefile-Linux-x86_64-intel
+-rw-r--r--   0 schiotz    (501) staff       (20)     1447 2016-10-17 13:41:41.000000 asap3-3.9.6/makefile-niflheim6
+-rw-r--r--   0 schiotz    (501) staff       (20)      269 2016-10-14 08:58:12.000000 asap3-3.9.6/makefile-Niflheim7
+-rw-r--r--   0 schiotz    (501) staff       (20)       27 2016-08-26 07:18:44.000000 asap3-3.9.6/makefile-sl230s-el6
+-rw-r--r--   0 schiotz    (501) staff       (20)       27 2016-10-25 07:17:57.000000 asap3-3.9.6/makefile-sylg.fysik.dtu.dk
+-rw-r--r--   0 schiotz    (501) staff       (20)       27 2016-08-26 07:18:44.000000 asap3-3.9.6/makefile-x3455-el6
+-rw-r--r--   0 schiotz    (501) staff       (20)      461 2016-10-26 09:21:42.000000 asap3-3.9.6/MANIFEST.in
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/OpenKIMexport/
+-rw-r--r--   0 schiotz    (501) staff       (20)    10147 2016-09-25 11:57:10.000000 asap3-3.9.6/OpenKIMexport/asap_kim_api.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2845 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/asap_kim_api.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2497 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimAsapPython.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     5787 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimAtoms.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     6281 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimAtoms.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3083 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborLocator.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     5289 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborLocator.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3667 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborMIOPBCF.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3597 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborMIOPBCF.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4286 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborMIOPBCH.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3401 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborMIOPBCH.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3443 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHPUREF.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3467 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHPUREF.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3654 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHPUREH.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3419 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHPUREH.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3360 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHRVECF.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3466 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHRVECF.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3738 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHRVECH.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3457 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimNeighborNEIGHRVECH.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1738 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/KimTemplates.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2181 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMexport/NeighborLocatorInterface.cpp
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/OpenKIMimport/
+-rw-r--r--   0 schiotz    (501) staff       (20)     3348 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMimport/DummyNeighborLocator.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     5970 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMimport/DummyNeighborLocator.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    20830 2016-09-25 11:57:10.000000 asap3-3.9.6/OpenKIMimport/OpenKIMcalculator.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     6902 2016-09-25 11:57:10.000000 asap3-3.9.6/OpenKIMimport/OpenKIMcalculator.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4693 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMimport/OpenKIMinfo.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3093 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMimport/OpenKIMinfo.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    22344 2016-09-25 11:57:10.000000 asap3-3.9.6/OpenKIMimport/OpenKIMinterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2182 2016-08-26 07:18:44.000000 asap3-3.9.6/OpenKIMimport/OpenKIMinterface.h
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Parallel/
+-rw-r--r--   0 schiotz    (501) staff       (20)    10603 2016-08-26 07:18:44.000000 asap3-3.9.6/Parallel/AsapMPI.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     3287 2016-08-26 07:18:44.000000 asap3-3.9.6/Parallel/DomainDecomposition.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    35461 2016-09-25 11:57:11.000000 asap3-3.9.6/Parallel/ParallelAtoms.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    10710 2016-09-25 11:57:11.000000 asap3-3.9.6/Parallel/ParallelAtoms.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     6509 2016-08-26 07:18:44.000000 asap3-3.9.6/Parallel/ParallelPotential.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3971 2016-08-26 07:18:44.000000 asap3-3.9.6/Parallel/ParallelPotential.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    14737 2016-09-25 11:57:11.000000 asap3-3.9.6/Parallel/RegularGridDecomposition.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3292 2016-09-25 11:57:11.000000 asap3-3.9.6/Parallel/RegularGridDecomposition.h
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/ParallelInterface/
+-rw-r--r--   0 schiotz    (501) staff       (20)     2676 2016-09-25 11:57:11.000000 asap3-3.9.6/ParallelInterface/AsapParallel.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    30171 2016-09-25 11:57:16.000000 asap3-3.9.6/ParallelInterface/mpi.c
+-rw-r--r--   0 schiotz    (501) staff       (20)     1533 2016-08-26 07:18:44.000000 asap3-3.9.6/ParallelInterface/mpimodule.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1759 2016-08-26 07:18:44.000000 asap3-3.9.6/ParallelInterface/ParallelAtomsInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1478 2016-08-26 07:18:44.000000 asap3-3.9.6/ParallelInterface/ParallelAtomsInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1725 2016-08-26 07:18:44.000000 asap3-3.9.6/ParallelInterface/ParallelNeighborListInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      274 2016-08-26 07:18:44.000000 asap3-3.9.6/ParallelInterface/ParallelNeighborListInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2728 2016-09-25 11:57:11.000000 asap3-3.9.6/ParallelInterface/ParallelPotentialInterface.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1430 2016-08-26 07:18:44.000000 asap3-3.9.6/ParallelInterface/ParallelPotentialInterface.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     1127 2016-10-26 10:36:18.000000 asap3-3.9.6/PKG-INFO
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/PTM/
+-rw-r--r--   0 schiotz    (501) staff       (20)     1728 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/alloy_types.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      206 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/alloy_types.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3889 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/canonical.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      208 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/canonical.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     8668 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/convex_hull_incremental.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      591 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/convex_hull_incremental.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2769 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/deformation_gradient.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      475 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/deformation_gradient.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     6718 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/fundamental_mappings.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    72714 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/graph_data.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      612 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/graph_data.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    13512 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/index_ptm.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     6019 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/index_ptm.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2998 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/neighbour_ordering.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      269 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/neighbour_ordering.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1077 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/normalize_vertices.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      225 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/normalize_vertices.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    10166 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/polar_decomposition.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      154 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/polar_decomposition.hpp
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/PTM/qcprot/
+-rw-r--r--   0 schiotz    (501) staff       (20)     9973 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/qcprot/qcprot.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3574 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/qcprot/qcprot.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     8643 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/qcprot/quat.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      913 2016-10-11 20:08:51.000000 asap3-3.9.6/PTM/qcprot/quat.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3510 2016-08-26 07:32:09.000000 asap3-3.9.6/PTM/qcprot.h
+-rw-r--r--   0 schiotz    (501) staff       (20)       93 2016-10-11 20:08:52.000000 asap3-3.9.6/PTM/unittest.hpp
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/PTM/voronoi/
+-rw-r--r--   0 schiotz    (501) staff       (20)    40624 2016-10-11 20:08:52.000000 asap3-3.9.6/PTM/voronoi/cell.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)    14009 2016-10-11 20:08:52.000000 asap3-3.9.6/PTM/voronoi/cell.hpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     5232 2016-10-11 20:08:52.000000 asap3-3.9.6/PTM/voronoi/config.hpp
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/
+-rw-r--r--   0 schiotz    (501) staff       (20)     5012 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/__init__.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/analysis/
+-rw-r--r--   0 schiotz    (501) staff       (20)      278 2016-10-17 13:41:41.000000 asap3-3.9.6/Python/asap3/analysis/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6218 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/analysis/averagepositions.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4063 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/analysis/clusterposition.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10873 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/analysis/localstructure.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2975 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/analysis/particle.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    11078 2016-10-17 09:19:37.000000 asap3-3.9.6/Python/asap3/analysis/ptm.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    11997 2016-10-18 11:47:04.000000 asap3-3.9.6/Python/asap3/analysis/rdf.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3663 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/constraints.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    23251 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/EMT2011_py.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      190 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/EMT2011Parameters.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    11742 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/EMT2013Parameters.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1242 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/fixepydoc.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      278 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/GuptaParameters.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/Internal/
+-rw-r--r--   0 schiotz    (501) staff       (20)        0 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     9560 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/AtomsInArrays.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    19688 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/Internal/BuiltinPotentials.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      834 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/Internal/Builtins.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1493 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/CheckArray.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1100 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/checkversion.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5508 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/Collector.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/Internal/Compatibility/
+-rw-r--r--   0 schiotz    (501) staff       (20)        0 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/Compatibility/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     8779 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/EMTParameters.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      570 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/ListOfElements.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2466 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/MonteCarloAtoms.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    16545 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/OpenKIMcalculator.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    13597 2016-10-18 11:47:04.000000 asap3-3.9.6/Python/asap3/Internal/ParallelListOfAtoms.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      713 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/Subject.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4731 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/Threads.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4134 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Internal/UtilityFunctions.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/io/
+-rw-r--r--   0 schiotz    (501) staff       (20)      189 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/io/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10796 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/io/bundletrajectory.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1524 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/io/cpu_setup.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3135 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/io/ReadOldFiles.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6897 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/io/trajectory.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/md/
+-rw-r--r--   0 schiotz    (501) staff       (20)      117 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/md/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     9525 2016-10-07 13:20:49.000000 asap3-3.9.6/Python/asap3/md/langevin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1356 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/md/md.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3775 2016-09-02 12:12:45.000000 asap3-3.9.6/Python/asap3/md/npt.py
+-rw-r--r--   0 schiotz    (501) staff       (20)       73 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/md/nptberendsen.py
+-rw-r--r--   0 schiotz    (501) staff       (20)       45 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/md/nvtberendsen.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1748 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/md/velocitydistribution.py
+-rw-r--r--   0 schiotz    (501) staff       (20)       91 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/md/verlet.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1828 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/md/verlet_fast.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      505 2016-09-28 12:16:54.000000 asap3-3.9.6/Python/asap3/memory.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/MonteCarlo/
+-rw-r--r--   0 schiotz    (501) staff       (20)        0 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6052 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Base.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1308 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Basin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1045 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Metropolis.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/
+-rw-r--r--   0 schiotz    (501) staff       (20)      307 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10336 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Base.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Data/
+-rw-r--r--   0 schiotz    (501) staff       (20)      196 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Data/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10422 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Data/fcc.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2860 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Data/symmetry.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    15256 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Surface.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2179 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/MonteCarlo/Start.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3899 2016-10-07 13:20:49.000000 asap3-3.9.6/Python/asap3/mpi.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/
+-rw-r--r--   0 schiotz    (501) staff       (20)        0 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1511 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/AdsCalc.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     9541 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/atommontecarlodata.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    17753 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/cluster.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4763 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/clusteratom.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/data/
+-rw-r--r--   0 schiotz    (501) staff       (20)      253 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/data/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      673 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/data/au.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10413 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/data/fcc.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2860 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/data/symmetry.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1558 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/langmuirExpression.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      767 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/Logger.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1280 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/mc_result.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/montecarlo/
+-rw-r--r--   0 schiotz    (501) staff       (20)      379 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/montecarlo/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    40041 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/montecarlo/atom.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    25368 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/montecarlo/surface.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1809 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/nanoparticle_mc/resizecluster.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/optimize/
+-rw-r--r--   0 schiotz    (501) staff       (20)       76 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/optimize/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2020 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/optimize/fire.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1019 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/optimize/mdmin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      553 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/optimize/optimize.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/setup/
+-rw-r--r--   0 schiotz    (501) staff       (20)        0 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/setup/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10553 2016-10-12 14:20:37.000000 asap3-3.9.6/Python/asap3/setup/dislocation.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6938 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/setup/displacementfield.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5655 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/setup/make_sample.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     9256 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/setup/nanocrystalline.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      570 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/setup/plane_utils.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4445 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/setup/quat_utils.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      778 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/setup/VelocityDistribution.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4548 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/testtools.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2701 2016-09-25 11:57:11.000000 asap3-3.9.6/Python/asap3/timing.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/Tools/
+-rw-r--r--   0 schiotz    (501) staff       (20)        0 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/__init__.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     4900 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/AsapFileToTrajectory.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      615 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/AtomicEnergies.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     8449 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ElasticConstants.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3168 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/EMT_two_atom_test.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5472 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/MaterialProperties.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      793 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/niflheim.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4893 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/OptimizationDatabase.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/
+-rw-r--r--   0 schiotz    (501) staff       (20)      303 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6337 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/EMT.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      856 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/GetParameters.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    17545 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Optimization.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2038 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Performance.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    36095 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Quantities.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2541 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/RGL.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2809 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Sampling.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    64144 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/ScipyFmin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     7726 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Search.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    11789 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/SearchParallel.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4969 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/SurfaceEnergies.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4839 2016-08-26 07:18:44.000000 asap3-3.9.6/Python/asap3/Tools/Timing.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      391 2016-10-26 07:50:22.000000 asap3-3.9.6/Python/asap3/version.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1059 2016-10-26 07:50:22.000000 asap3-3.9.6/recordversion.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/scripts/
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     6535 2016-10-26 07:50:22.000000 asap3-3.9.6/scripts/asap-qsub
+-rw-r--r--   0 schiotz    (501) staff       (20)    13871 2016-10-26 09:21:42.000000 asap3-3.9.6/setup.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Test/
+-rw-r--r--   0 schiotz    (501) staff       (20)     2133 2016-10-11 20:08:52.000000 asap3-3.9.6/Test/ase_emt.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    16918 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/BrennerNanotube.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      788 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/BrennerPullNanotube.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10885 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/BrennerStress.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1506 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/CalculationRequired.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1717 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/ChangeAtoms.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      699 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/ChangeAtoms2.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      814 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/ChangeCalculator.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2240 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/ChangePeriodicity.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      975 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/ChangeUnitCell.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1361 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/ChangeUnitCell2.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2033 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/CNAleak.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1127 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/ConstraintInTraj.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3170 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Constraints.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1048 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/EMT2013elements.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2133 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/EMTleak.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      826 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Exception.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      698 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/FieldPlotter.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1019 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/FIRE.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5116 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/HooverNPT.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4893 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Hydrocarbons.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2833 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Langevin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      794 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/LargeShear.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6882 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Lattice.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     9872 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/LennardJones.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      722 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/LJ_Stress.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1837 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/LocalStructure.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     4950 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/LongLangevin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4851 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/MonteCarloOptim_Alloy.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4089 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/MonteCarloOptim_Energy.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5157 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/MonteCarloOptim_NbList.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2986 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Morse.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3475 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/NbCellLocator.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3864 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/NeighborList.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2050 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/NoInterference.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1159 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/NoMI_LeftHanded.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6249 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/OpenKIM_AllModels.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2774 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/OpenKIM_EMT.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      776 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/OpenKIM_modelname.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Test/parallel/
+-rw-r--r--   0 schiotz    (501) staff       (20)        0 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/__init__.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2776 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/bundleTrajPreserveZ.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1596 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/Force1D.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6219 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/longMelting.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2258 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/makeparallel.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1650 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/migration.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1956 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/moveatoms.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3237 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/moveatomsLJ.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3020 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelBundleTrajectories.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2905 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelConstraints.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1643 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelFIRE.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3621 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/parallel/parallelLangevin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3048 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelLennardJones.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2511 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelLocalStructure.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3285 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelLongVerlet.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2718 2016-10-18 11:47:04.000000 asap3-3.9.6/Test/parallel/parallelNeighborLocator.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3703 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelNPT.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5068 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelOpenKIM_NeighMiopbc_F.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5068 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelOpenKIM_NeighMiopbc_H.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5071 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelOpenKIM_NeighPure_F.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5071 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelOpenKIM_NeighPure_H.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5071 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelOpenKIM_NeighRvec_F.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5066 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelOpenKIM_NeighRvec_H.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1482 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelPBC.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1619 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelPBC2.py
+-rw-r--r--   0 schiotz    (501) staff       (20)   123573 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelPotentials.pickle
+-rw-r--r--   0 schiotz    (501) staff       (20)     7279 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelPotentials.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2673 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelRDF.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3988 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelStress.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2941 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelTrajectories.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4544 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/parallelVerlet.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2095 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/parallel/simplempi.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1557 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/PBCwrap.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     5358 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Potentials.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    36496 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/potResults.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      481 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/PrintMemory.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1179 2016-10-11 20:08:52.000000 asap3-3.9.6/Test/ptm.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2794 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/QuickLangevin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2818 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/RawRDF.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2113 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/RawRDF2.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2071 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/RDF.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3029 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/RDF2.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2372 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/SizeConsist_EMT.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2297 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/SizeConsist_EMT2013.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1359 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/SizeConsist_LeftHand.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1601 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/SizeConsist_OpenKIM.py
+-rw-r--r--   0 schiotz    (501) staff       (20)   298761 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/SpecialEMT.pickle
+-rw-r--r--   0 schiotz    (501) staff       (20)     3228 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/SpecialEMT.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1066 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/StdParamProv.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3379 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Stress.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1737 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/StressCrash.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1540 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/StressFilter.py
+-rw-r--r--   0 schiotz    (501) staff       (20)    10859 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/StressModule.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1680 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Subset.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4054 2016-10-26 07:50:22.000000 asap3-3.9.6/Test/test_reproducible.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     7507 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/TestAll.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)       66 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/TestParallel-openmpi.sh
+-rw-r--r--   0 schiotz    (501) staff       (20)   258002 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/testVerlet.pickle
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Test/Timing/
+-rw-r--r--   0 schiotz    (501) staff       (20)     3741 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Timing/MonteCarloTiming.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1840 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Timing/Morse.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     6392 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Timing/OfficialTiming.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3381 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Timing/OpenKIM_MemLeak.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     4212 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Timing/OpenKIM_ParTiming.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3213 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Timing/OpenKIM_Profiling.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     8924 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Timing/ParallelTiming.py
+-rw-r--r--   0 schiotz    (501) staff       (20)      739 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/Timing/ThreadForceTiming.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     6436 2016-10-25 07:17:57.000000 asap3-3.9.6/Test/Timing/Timing.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     6543 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/Timing/Timing_OpenKIM.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     6522 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/Timing/TimingEMT2013.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     3498 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/Timing/TimingLangevin.py
+-rwxr-xr-x   0 schiotz    (501) staff       (20)     3108 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/Timing/TimingVerlet.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     3506 2016-09-25 11:57:11.000000 asap3-3.9.6/Test/TinyLangevin.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2583 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Trajectories.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     2046 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Trajectories_ase.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1481 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Verlet.py
+-rw-r--r--   0 schiotz    (501) staff       (20)     1642 2016-08-26 07:18:44.000000 asap3-3.9.6/Test/Verlet_OpenKIM.py
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/Tools/
+-rw-r--r--   0 schiotz    (501) staff       (20)     3475 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/CNA.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1345 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/CNA.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     2551 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/CoordinationNumbers.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1424 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/CoordinationNumbers.h
+-rw-r--r--   0 schiotz    (501) staff       (20)    17922 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/FullCNA.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3419 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/FullCNA.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4460 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/GetNeighborList.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     1849 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/GetNeighborList.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4698 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/RawRadialDistribution.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     2780 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/RawRadialDistribution.h
+-rw-r--r--   0 schiotz    (501) staff       (20)     4079 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/SecondaryNeighborLocator.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)     3445 2016-08-26 07:18:44.000000 asap3-3.9.6/Tools/SecondaryNeighborLocator.h
+drwxr-xr-x   0 schiotz    (501) staff       (20)        0 2016-10-26 10:36:18.000000 asap3-3.9.6/VersionInfo_autogen/
+-rw-r--r--   0 schiotz    (501) staff       (20)      420 2016-10-26 08:12:04.000000 asap3-3.9.6/VersionInfo_autogen/version_demokrit.fysik.dtu.dk_p.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      418 2016-10-26 08:12:04.000000 asap3-3.9.6/VersionInfo_autogen/version_demokrit.fysik.dtu.dk_s.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      413 2016-10-25 12:55:36.000000 asap3-3.9.6/VersionInfo_autogen/version_demokrit.local_p.cpp
+-rw-r--r--   0 schiotz    (501) staff       (20)      411 2016-10-25 12:55:36.000000 asap3-3.9.6/VersionInfo_autogen/version_demokrit.local_s.cpp
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `asap3-3.13.1/Archive/MoPotential.cpp` & `asap3-3.9.6/Archive/MoPotential.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Archive/MoPotential.h` & `asap3-3.9.6/Archive/MoPotential.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Asap.h` & `asap3-3.9.6/Basics/Asap.h`

 * *Files 18% similar despite different names*

```diff
@@ -42,19 +42,15 @@
 
 // A C++ namespace is defined for all of Asap to reduce the likelihood
 // of symbol clashes.  It is defined in a separate header file so it can
 // be changed when Asap source files are used in e.g. OpenKIM
 #include "AsapNamespace.h"
 
 /// The batch-buffer size in EMT.cpp.
-///
-/// If Intel MKL is used, must be a multiple of 8 to preserve alignment,
-/// since 8 doubles is 64 bytes or 512 bits, and new Intel processors
-/// may process data in 512 bit chunks (current only use 256 bits).
-#define BUFLEN 1600
+#define BUFLEN 10000
 
 /// Maximal number of elements in a single simulation (EMT.cpp)
 #define NMAXELEMENTS 25
 
 /// Is timing enabled?
 //#define TIMING
 
@@ -70,21 +66,18 @@
 
 #ifndef _WIN32
 #ifndef __APPLE__
 //#define CATCHFLOAT
 #endif
 #endif
 
-/// Do we want to use our own assert macro, transforming assertion
-/// failure into a Python AssertionFailed exception?
-#ifndef NDEBUG        // Never if NDEBUG is defined ...
-#ifndef ASAP_FOR_KIM  // ... also keep real assert in OpenKIM
+/// Do we want to use our own assert macro?
+#ifndef NDEBUG        // Never if NDEBUG is defined
 #define ASAPASSERT
 #endif
-#endif
 
 /// Do we want asserts that cause a (small) performance penalty
 ///
 /// The performance penalty is approximately 2 percent.
 #define SLOWASSERT
 
 // Some openMP compilers (Open64 for example) turns on processor
@@ -106,45 +99,34 @@
 /// Do we want debugging info printed when objects are created or destroyed?
 //#define DEBUGOBJECTS
 
 /// Do we want to debug memory usage
 //#define ASAPMEMORYDEBUG
 
 // The following symbol definitions should not be changed
-#define CHECKNAN(x) ASSERT(!isnan(x) && !isinf(x))
+#ifdef SLOWASSERT
+#define ASSERT(x) assert(x);
+#else
+#define ASSERT(x)
+#endif
+
+#define CHECKNAN(x) assert(!isnan(x) && !isinf(x))
 
 // Define the size of the integer used to hold atomic numbers
 #define asap_z_int npy_int32
 #define ASAP_Z_ARRAYTYPE NPY_INT32
 #define ASAP_Z_SIZE NPY_SIZEOF_INT32
 
-// When compiling with Math Kernel Library (not a good idea unless
-// Intel compilers are not availabe) we must align some temporary
-// arrays.
-#ifdef ASAP_MKL
-#define ASAP_MKL_ALIGN 64
-#endif //ASAP_MKL
-
 // Macros that aid the compiler optimizing.
 #ifdef __GNUC__
 #define RESTRICT __restrict__
 #else
 #define RESTRICT
 #endif
-
-// Macro for flagging unused variables, so they are not triggering compiler warnings.
-#ifdef UNUSED
-#elif defined(__GNUC__)
-#define UNUSED(x) x __attribute__((unused))
-#elif defined(__LCLINT__)
-#define UNUSED(x) /*@unused@*/ x
-#else
-#define UNUSED(x) x
-#endif
-
+ 
 
 // Macros for controling visibility of symbols, for use with -fvisibility=hidden
 #if defined _WIN32 || defined __CYGWIN__
   // Prepare for the unlikely case that someone will try to compile for Windoze.
   #define ASAP_PUBLIC __declspec(dllexport)
   #define ASAP_LOCAL
 #else  // _WIN32
```

### Comparing `asap3-3.13.1/Basics/AsapNamespace.h` & `asap3-3.9.6/Basics/AsapNamespace.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/AsapObject.cpp` & `asap3-3.9.6/Basics/AsapObject.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
 #include "Asap.h"
 #include "AsapObject.h"
 #include <stdio.h>
 
 string AsapObject::GetRepresentation() const
 {
   char buffer[50];
-  sprintf(buffer, "%p", this);
+  sprintf(buffer, "0x%p", this);
   return "<asap." + GetName() + " object at " + buffer + ">";
 }
```

### Comparing `asap3-3.13.1/Basics/AsapObject.h` & `asap3-3.9.6/Basics/AsapObject.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/AsapPython.h` & `asap3-3.9.6/Basics/AsapPython.h`

 * *Files 24% similar despite different names*

```diff
@@ -40,21 +40,43 @@
 #define NO_IMPORT_ARRAY
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 #include <numpy/arrayobject.h>
 #ifdef __cplusplus  // Allow inclusion from mpi.c
 #include "Exception.h"
 
 // Take a PyObject and check that it is a reasonable PyArrayObject
-inline PyArrayObject *ASPYARRAY(PyObject *p, string f, int l) {
+inline PyArrayObject *AsPyArray(PyObject *p) {
   if ((p != NULL) && !PyArray_Check(p))
-    throw AsapError("Expected a numpy array, got something else! ") << f << ":" << l;
+    throw AsapError("Expected a NumPy array, got something else!");
   return (PyArrayObject *) p;
 }
-#define AsPyArray(x) ASPYARRAY((x), __FILE__, __LINE__)
-
 #endif // __cplusplus
 
 #define CHECKREF(x) assert(Py_REFCNT(x) >= 1 && Py_REFCNT(x) <= 100);
 #define XCHECKREF(x) assert((x) == NULL || (Py_REFCNT(x) >= 1 && Py_REFCNT(x) <= 100));
 #define PRINTREF(x) cerr << __FILE__ << ":" << __LINE__ << " Refcount=" << Py_REFCNT(x) << endl;
 
+
+/* Python 2 or Python 3 ? */
+#if PY_MAJOR_VERSION >= 3
+#define ASAP_PY3
+#endif
+
+#ifdef ASAP_PY3
+#define PyAsapString_Check PyUnicode_Check
+#define PyAsapString_Type PyUnicode_Type
+#define PyAsapString_FromString PyUnicode_FromString
+#define PyAsapString_AsString PyUnicode_AsUTF8
+#define PyAsapInt_AsLong PyLong_AsLong
+#define PyAsapInt_FromLong PyLong_FromLong
+#define PyAsapInt_Check PyLong_Check
+#else
+#define PyAsapString_Check PyString_Check
+#define PyAsapString_Type PyString_Type
+#define PyAsapString_FromString PyString_FromString
+#define PyAsapString_AsString PyString_AsString
+#define PyAsapInt_AsLong PyInt_AsLong
+#define PyAsapInt_FromLong PyInt_FromLong
+#define PyAsapInt_Check PyInt_Check
+#endif
+
 #endif /* _ASAPPYTHON_H */
```

### Comparing `asap3-3.13.1/Basics/Atoms.h` & `asap3-3.9.6/Basics/Atoms.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/AtomsBasis.h` & `asap3-3.9.6/Basics/AtomsBasis.h`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,15 @@
 /// This object is refcounted, see AsapAtoms_INCREF() and AsapAtoms_DECREF().
 class Atoms
 {
 protected:
   /// Delete the interface object.
   ///
   /// Protected: may only be called from AsapAtoms_DECREF() friend function.
-  virtual ~Atoms() {}
-  //virtual ~Atoms() {assert(refcount == 0);}  // Incorrect if assert is redefined.
+  virtual ~Atoms() {assert(refcount == 0);}
   
 public:
   /// Create the interface object.
   Atoms() {refcount = 1;}
 
   // Reference counting
   friend void AsapAtoms_INCREF(Atoms *atoms);
@@ -123,20 +122,21 @@
   /// Include ghosts if possible and requested.
   virtual void GetScaledPositions(vector<Vec> &scaledpos, bool ghosts=false) = 0;
 
   /// Get a copy of some positions, converted to scaled space.
   virtual void GetScaledPositions(vector<Vec> &scaledpos, const set<int> &which) = 0;
 
   /// Get the atomic numbers
-  virtual const asap_z_int *GetAtomicNumbers() = 0;
+  virtual const asap_z_int *GetAtomicNumbers() const = 0;
   
+  /// Get the cartesian momenta
+  virtual const Vec *GetMomenta() = 0;
+
   /// Get the boundary conditions.
   virtual const bool *GetBoundaryConditions() const = 0;
-  /// Get the boundary conditions. No sanity check!
-  virtual const bool *GET_BOUNDARY_CONDITIONS() const = 0;
 
   virtual bool AllFreeBoundaries() const = 0;
 
   virtual bool AllPeriodicBoundaries() const = 0;
 
   /// Get the supercell
   virtual const Vec *GetCell() const = 0;
@@ -150,15 +150,15 @@
   /// Get the height of the supercell
   virtual const double *GetCellHeights() = 0;
   
   /// Get the inverse supercell
   virtual const Vec *GetInverseCell() = 0;
   
   /// Get a set of all elements present in the simulations.
-  virtual void GetListOfElements(set<int> &elements) = 0;
+  virtual void GetListOfElements(set<int> &elements) const = 0;
 
   /// Get the masses of the atoms
   virtual const double *GetMasses() = 0;
 
   /// Set a python array on the atoms.
   virtual void SetData(const char *name, PyObject *data) = 0;
 
@@ -212,16 +212,28 @@
   virtual int GetNumbersCounter() const = 0;
   
   /// Counter showing changes to the positions.
   ///
   /// Also updated if CellCounter, NumbersCounter or AtomsCounter is updated.
   virtual int GetPositionsCounter() const = 0;
 
-  /// Throw an error if there are no atoms in the simulation.
-  virtual void NoAtomsErrorOrWarning() {throw AsapError("No atoms in simulation.");}
+  /// Counter showing changes to the momenta.
+  ///
+  /// Reading this counter will cause the momenta to be extracted from Python.
+  virtual int GetMomentaCounter() = 0;
+
+  /// Set the primary neighbor list in a PARALLEL simulation.
+  ///
+  /// Ignored in serial simulations
+  virtual void SetPrimaryNbLocator(PyObject *nblocator) {};
+
+  /// Get the primary neighbor list in a PARALLEL simulation.
+  ///
+  /// Ignored in serial simulations.  Returns a new reference.
+  virtual PyObject *GetPrimaryNbLocator(PyObject *pyatoms) {return NULL;}
 
   /// Print memory usage
   virtual long PrintMemory() const = 0;
   
 protected:
   int refcount;           ///< Number of references to this object.
 };
```

### Comparing `asap3-3.13.1/Basics/Debug.cpp` & `asap3-3.9.6/Basics/Debug.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Debug.h` & `asap3-3.9.6/Basics/Debug.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/DynamicAtoms.cpp` & `asap3-3.9.6/Basics/DynamicAtoms.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,15 @@
   return PyArray_DIM(py_data, 0);
 }
 
 double *DynamicAtoms::GetDoubleData(PyObject *name)
 {
   PyArrayObject *py_data = AsPyArray(PyDict_GetItem(arrays, name));
   if (py_data == NULL)
-      throw AsapError("Atoms.arrays has no ") << PyUnicode_AsUTF8(name);
+      throw AsapError("Atoms.arrays has no ") << PyAsapString_AsString(name);
   if (PyArray_Check(py_data) != 1           // A NumPy array
         || PyArray_TYPE(py_data) != NPY_DOUBLE  // array of double
         || !PyArray_ISCARRAY_RO(py_data))       // Contiguous etc.
       throw AsapError("Atoms data has unexpected type: ") << name;
   return (double *) PyArray_DATA(py_data);
 }
```

### Comparing `asap3-3.13.1/Basics/DynamicAtoms.h` & `asap3-3.9.6/Basics/DynamicAtoms.h`

 * *Files 17% similar despite different names*

```diff
@@ -34,26 +34,21 @@
 
 namespace ASAPSPACE {
 
 class DynamicAtoms
 {
 public:
     DynamicAtoms(PyObject *py_atoms);
-    virtual ~DynamicAtoms();
+    ~DynamicAtoms();
     
     int GetNAtoms();
     Vec *GetPositions() {return GetVecData("positions");}
     Vec *GetMomenta() {return GetVecData("momenta");}
     const asap_z_int *GetAtomicNumbers();
-
-    // GetMasses and GetInverseMasses return arrays that map from
-    // atomic numbers to (inverse) atomic masses based on data 
-    // extracted from the ase.data Python module.
-    // A Dynamics module MUST check if these need to be overruled
-    // by masses stored on the atoms.
+    
     const std::vector<double> &GetMasses() {return masses;}
     const std::vector<double> &GetInverseMasses() {return invmasses;}
 
     double *GetDoubleData(PyObject *name);
     double *GetDoubleDataMaybe(PyObject *name);  // Get data if present, or NULL
 
 private:
```

### Comparing `asap3-3.13.1/Basics/Exception.cpp` & `asap3-3.9.6/Basics/Exception.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -39,43 +39,26 @@
 }
 
 AsapError::AsapError(const AsapError& ex) : message() 
 {
   message << ex.GetMessage();
 }
 
-
+AsapError::~AsapError() 
+{
+}
 string AsapError::GetMessage() const 
 {
   return message.str();
 }
 
-#ifndef ASAP_FOR_KIM
 AsapNotImplementedError::AsapNotImplementedError(const char *m)
 {
-  // We need to raise a PropertyNotImplementedError available in the asap3
-  // Python module, either defined there or imported from ASE.
-  PyObject *asap = PyImport_ImportModule("asap3");
-  if (asap == NULL)
-  {
-    PyErr_SetString(PyExc_RuntimeError, "Failed to make a PropertyNotImplementedError (module loading)");
-    return;
-  }
-  PyObject *PropertyNIE = PyObject_GetAttrString(asap, "PropertyNotImplementedError");
-  if (PropertyNIE == NULL)
-  {
-    Py_DECREF(asap);
-    PyErr_SetString(PyExc_RuntimeError, "Failed to make a PropertyNotImplementedError (attribute)");
-    return;
-  }
-  PyErr_SetString(PropertyNIE, m);
-  Py_DECREF(PropertyNIE);
-  Py_DECREF(asap);
+  PyErr_SetString(PyExc_NotImplementedError, m);
 }
-#endif // not ASAP_FOR_KIM
 
 AssertionFailed::AssertionFailed(const char *expression, const char *file,
 				 int line, const char *func)
   : message() 
 {
   DEBUGPRINT;
   message << file << ":" << line << ": ";
@@ -89,14 +72,17 @@
 AssertionFailed::AssertionFailed(const AssertionFailed& ex)
   : message() 
 {
   DEBUGPRINT;
   message << ex.GetMessage();
 }
 
+AssertionFailed::~AssertionFailed() 
+{
+}
 string AssertionFailed::GetMessage() const 
 {
   DEBUGPRINT;
   return message.str();
 }
 
 #ifdef _OPENMP
```

### Comparing `asap3-3.13.1/Basics/Exception.h` & `asap3-3.9.6/Basics/Exception.h`

 * *Files 8% similar despite different names*

```diff
@@ -65,44 +65,39 @@
 #define _EXCEPTION_H
 
 #include "Asap.h"
 #include <sstream>
 #include <iostream>
 #ifndef ASAPASSERT
 #include <assert.h>
-#include <exception>
 #endif // ASAPASSERT
 
 using std::stringstream;
 using std::string;
 
-#ifndef _NOEXCEPT
-#define _NOEXCEPT throw()
-#endif
-
 namespace ASAPSPACE {
 
 // this AsapError class can be used as follows:
 //
 // throw AsapError("Error");
 //
 // throw AsapError("Error ") << n + 7 << " while opening file: " << filename;
 
-class ASAP_PUBLIC AsapErrorBase : std::exception
+class ASAP_PUBLIC AsapErrorBase
 {
 public:
-  virtual ~AsapErrorBase() _NOEXCEPT {};
+  virtual ~AsapErrorBase() {};
 };
 
 class ASAP_PUBLIC AsapError : public AsapErrorBase
 {
 public:
   AsapError(const char *m);
   AsapError(const AsapError& ex);
-  virtual ~AsapError() _NOEXCEPT {};
+  virtual ~AsapError();
   template<class T> AsapError& operator<<(const T& x) 
     {
       message << x;
       return *this;
     }
   string GetMessage() const;
 private:
@@ -111,81 +106,61 @@
 
 /// An exception for indicating that a Python error has occurred and
 /// should be propagated.
 class ASAP_PUBLIC AsapPythonError : public AsapErrorBase
 {
 public:
   AsapPythonError() {};
-  virtual ~AsapPythonError() _NOEXCEPT {};
 };
 
-#ifdef ASAP_FOR_KIM
-// This definition is used when an ASAP potential is exported to OpenKIM,
-// where there is no Python.
-class ASAP_PUBLIC AsapNotImplementedError : public AsapError
-{
-public:
-  AsapNotImplementedError(const char *m) : AsapError(m) {};
-};
-#else // ASAP_FOR_KIM
-// The NORMAL version is here !
 /// An exception mapping to a Python NotImplementedError
 class ASAP_PUBLIC AsapNotImplementedError : public AsapPythonError
 {
 public:
   AsapNotImplementedError(const char *m);
 };
-#endif //ASAP_FOR_KIM
+
 
 class ASAP_PUBLIC AssertionFailed : public AsapErrorBase
 {
 public:
   AssertionFailed(const char *expression, const char *file, int line,
 		  const char *func = NULL);
   AssertionFailed(const AssertionFailed& ex);
-  ~AssertionFailed() _NOEXCEPT {};
+  ~AssertionFailed();
   string GetMessage() const;
 private:
   stringstream message;
 };
 
 /// A helper define
 #define NOTHREADSERROR throw AsapError("Threads not supported. ") << __FILE__ << ":" << __LINE__
 
 /// Defining our own assert macro that throws an exception
 #ifdef ASAPASSERT
+#undef assert
 #ifdef __GNUC__
-#define ASSERT(EX) if (!(EX)) \
+#define assert(EX) if (!(EX)) \
     throw AssertionFailed(#EX, __FILE__, __LINE__, __PRETTY_FUNCTION__)
 #else // __GNUC__
-#define ASSERT(EX) if (!(EX)) \
+#define assert(EX) if (!(EX)) \
     throw AssertionFailed(#EX, __FILE__, __LINE__, __func__)
 #endif // __GNUC__
-#else // ASAPASSERT
-#define ASSERT(EX) assert(EX)
 #endif // ASAPASSERT
 
-#ifdef SLOWASSERT
-// We need the semicolon below, although it looks wrong, to allow SASSERT to vanish altogether.
-#define SASSERT(x) ASSERT(x);
-#else  // SLOWASSERT
-#define SASSERT(x)
-#endif // SLOWASSERT
-
-
 // Define macros and helper functions for throwing exceptions within OpenMP constructs.
 #ifdef _OPENMP
 
 extern AsapErrorBase *AsapGlobalException;
 void AsapThrowHelper(const AsapError &err);
 void AsapThrowHelper(const AsapPythonError &err);
 
 #define THROW(x) AsapThrowHelper(x)
 #define THROW_RETURN(x) {AsapThrowHelper(x); return;}
-#define CHECKNOASAPERROR ASSERT(AsapGlobalException == NULL)
+#define CHECKNOASAPERROR assert(AsapGlobalException == NULL)
 #define RETURNIFASAPERROR if (AsapGlobalException != NULL) return
 #define RETURNIFASAPERROR2(x) if (AsapGlobalException != NULL) return (x)
 #define PROPAGATEASAPERROR if (AsapGlobalException != NULL) { \
     AsapError *err = dynamic_cast<AsapError*>(AsapGlobalException); \
     AsapPythonError *perr = dynamic_cast<AsapPythonError*>(AsapGlobalException); \
     AsapGlobalException = NULL; \
     std::cerr << "Propagating ASAP error [" << __FILE__ << ":" << __LINE__ << "] ..." << std::endl; \
```

### Comparing `asap3-3.13.1/Basics/IVec.h` & `asap3-3.9.6/Basics/IVec.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/ImageAtoms.cpp` & `asap3-3.9.6/Basics/ImageAtoms.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   AsapAtoms_INCREF(realatoms);
 }
 
 ImageAtoms::~ImageAtoms()
 {
   DESTRUCTOR;
   AsapAtoms_DECREF(realatoms);
-  ASSERT(refcount == 0);
+  assert(refcount == 0);
 }
 
 bool ImageAtoms::UpdateBeforeCalculation(bool flag, double range)
 {
   DEBUGPRINT;
   bool update = realatoms->UpdateBeforeCalculation(flag, range);
   if (update)
@@ -64,60 +64,68 @@
     }
   DEBUGPRINT;
   return update;
 }
 
 void ImageAtoms::Begin(PyObject *pyatoms, bool expect_reopen /*=false*/)
 {
+  DEBUGPRINT;
   realatoms->Begin(pyatoms, expect_reopen);
   if ((nAtoms != realatoms->GetNumberOfAtoms())
       || (nGhosts != realatoms->GetNumberOfGhostAtoms()))
     make_images(last_range);
   update_images();
+  DEBUGPRINT;
 }
 
 void ImageAtoms::GetPositions(vector<Vec> &pos, bool ghosts /* = false */) const
 {
+  DEBUGPRINT;
   pos.clear();
   int nTot = ghosts ? (nAtoms + nGhosts + nImages) : nAtoms;
   if (pos.capacity() < nTot)
     pos.reserve(nTot + nTot/25);  // 4% extra
-  ASSERT(allpositions.size() >= nTot);
+  assert(allpositions.size() >= nTot);
   pos.insert(pos.begin(), allpositions.begin(), allpositions.begin() + nTot);
-  ASSERT(pos.size() == nTot);
+  assert(pos.size() == nTot);
+  DEBUGPRINT;
 }
 
 
 void ImageAtoms::GetScaledPositions(vector<Vec> &pos, bool ghosts /* = false */)
 {
+  DEBUGPRINT;
   int n = nAtoms;
   if (ghosts)
     n += nGhosts + nImages;
-  ASSERT(allpositions.size() >= n);
+  assert(allpositions.size() >= n);
   const Vec *inv = GetInverseCell();
   if (pos.capacity() < n)
     pos.reserve(n + n/25);  // Reserve 4% extra.
   pos.resize(n);
   for (int i = 0; i < n; i++)
     for (int j = 0; j < 3; j++)
       pos[i][j] = allpositions[i][0] * inv[0][j]
                 + allpositions[i][1] * inv[1][j]
                 + allpositions[i][2] * inv[2][j];
+  DEBUGPRINT;
 }
 
 void ImageAtoms::GetScaledPositions(vector<Vec> &scaledpos, const set<int> &which)
 {
-  ASSERT(scaledpos.size() == which.size());
+  DEBUGPRINT;
+  assert(scaledpos.size() == which.size());
   const Vec *inv = GetInverseCell();
   vector<Vec>::iterator spi = scaledpos.begin();
   for (set<int>::const_iterator i = which.begin(); i != which.end(); ++i,++spi)
     for (int j = 0; j < 3; j++)
       (*spi)[j] = allpositions[*i][0] * inv[0][j]
                 + allpositions[*i][1] * inv[1][j]
                 + allpositions[*i][2] * inv[2][j];
+  DEBUGPRINT;
 }
 
 void ImageAtoms::make_images(double range)
 {
   DEBUGPRINT;
   initialized = true;
   translations.clear();
@@ -138,62 +146,47 @@
       else
         nbox[i] = 0;
     }
 
 
   // Now create the images.  We loop over each replica of the system
   // that may contain images.
+  const Vec *positions = realatoms->GetPositions();
   nAtoms = realatoms->GetNumberOfAtoms();
   nGhosts = realatoms->GetNumberOfGhostAtoms();
   const Vec *cell = realatoms->GetCell();
   Vec toppoint(cell[0] + cell[1] + cell[2]);
 
-  DEBUGPRINT;
-
   // Normalize and make sure the sign is right (we cannot assume
   // a right-handed unit cell.
   Vec directions[3];
   for (int i = 0; i < 3; i++)
     {
       int j = (i + 1) % 3;
       int k = (i + 2) % 3;
       directions[i] = Cross(cell[j], cell[k]);
       directions[i] *= 1.0/sqrt(Length2(directions[i]));
       if (directions[i] * cell[i] < 0.0)
         directions[i] *= -1.0;
     }
 
-  // Find the translations that wrap the real atoms into the box; then use those
-  // translations prior to decising upon the translations to use for ghost atoms.
-  // Also, apply the translations to the real atoms in update_images.
-  vector<Vec> scaledPositions;
-  realatoms->GetScaledPositions(scaledPositions, true);  // Get also ghosts
-  ASSERT(scaledPositions.size() == nAtoms + nGhosts);
-  orig_atoms_translations.resize(nAtoms + nGhosts);
-  for (int i = 0; i < nAtoms + nGhosts; ++i)
-  {
-    for (int j = 0; j < 3; ++j)
-      orig_atoms_translations[i][j] = - pbc[j] * (int) floor(scaledPositions[i][j]);
-  }
-  
   const Vec *r = realatoms->GetPositions();
   for (int i = -nbox[0]; i <= nbox[0]; i++)
     for (int j = -nbox[1]; j <= nbox[1]; j++)
       for (int k = -nbox[2]; k <= nbox[2]; k++)
         {
           if ((i == 0) && (j == 0) && (k == 0))
             continue;   // Central box.  Not images
           IVec tranl(i, j, k);
           translations.push_back(tranl);
           first_atom.push_back(original_atom.size());
           Vec shift = tranl[0] * cell[0] + tranl[1] * cell[1] + tranl[2] * cell[2];
           for (int n = 0; n < nAtoms + nGhosts; n++)
             {
-	      const IVec &otrans = orig_atoms_translations[n];
-              Vec rr = r[n] + shift + otrans[0] * cell[0] + otrans[1] * cell[1] + otrans[2] * cell[2];
+              Vec rr = r[n] + shift;
               Vec r2 = rr - toppoint;
               // Check the six limits, skip atom if any test fails
               // Check a lower limit, direction 0
               if ( (i < 0) && (rr * directions[0] < - range) )
                 continue;
               // Check upper limit, direction 0
               if ( (i > 0 ) && (r2 * directions[0] > range) )
@@ -231,41 +224,35 @@
   if (!initialized)
     {
       DEBUGPRINT;
       return;  // This happens when Begin is called from the initial SetAtoms call.
     }
   // Get the positions and atomic numbers of the real atoms and the ghosts.
   realatoms->GetPositions(allpositions, true);
-  ASSERT(allpositions.size() <= nSize);
-  // Translate the real atoms and the ghosts
-  const Vec *cell = realatoms->GetCell();
-  ASSERT(orig_atoms_translations.size() == nAtoms + nGhosts);
-  for (int i = 0; i < nAtoms + nGhosts; ++i)
-  {
-    const IVec otrans = orig_atoms_translations[i];
-    allpositions[i] += otrans[0] * cell[0] + otrans[1] * cell[1] + otrans[2] * cell[2];
-  }
+  assert(allpositions.size() <= nSize);
   allpositions.resize(nSize);
   allnumbers.resize(nSize);
   const asap_z_int *z = realatoms->GetAtomicNumbers();
   for (int i = 0; i < nAtoms + nGhosts; i++)
     allnumbers[i] = z[i];
   // Now update the images.  Both positions and atomic numbers may have changed.
   int target = nAtoms + nGhosts;
   int source = 0;
   int ngroups = translations.size();
+  const Vec *r = realatoms->GetPositions();
+  const Vec *cell = realatoms->GetCell();
 
   for (int i = 0; i < ngroups; i++)
     {
       const IVec &tr = translations[i];
       Vec shift = tr[0] * cell[0] + tr[1] * cell[1] + tr[2] * cell[2];
       for (int n = first_atom[i]; n < last_atom[i]; n++)
         {
-          allpositions[target] = allpositions[original_atom[source]] + shift;
+          allpositions[target] = r[original_atom[source]] + shift;
           allnumbers[target] = z[original_atom[source]];
           source++;
           target++;
         }
     }
-  ASSERT(target == nSize);
+  assert(target == nSize);
   DEBUGPRINT;
 }
```

### Comparing `asap3-3.13.1/Basics/ImageAtoms.h` & `asap3-3.9.6/Basics/ImageAtoms.h`

 * *Files 2% similar despite different names*

```diff
@@ -115,23 +115,21 @@
   /// Include ghosts if possible and requested.
   virtual void GetScaledPositions(vector<Vec> &scaledpos, bool ghosts=false);
 
   /// Get a copy of some positions, converted to scaled space.
   virtual void GetScaledPositions(vector<Vec> &scaledpos, const set<int> &which);
 
   /// Get the atomic numbers
-  virtual const asap_z_int *GetAtomicNumbers() 
-   {ASSERT(allnumbers.size() > 0); return &allnumbers[0];}
+  virtual const asap_z_int *GetAtomicNumbers() const
+   {assert(allnumbers.size() > 0); return &allnumbers[0];}
 
   /// Get the boundary conditions.
   ///
   /// These will be faked to free boundary conditions.
   virtual const bool *GetBoundaryConditions() const {return bc_are_free;}
-  virtual const bool *GET_BOUNDARY_CONDITIONS() const {return bc_are_free;}
-
 
   virtual bool AllFreeBoundaries() const {return true;}
 
   virtual bool AllPeriodicBoundaries() const {return false;}
 
 
   /// ALL THE FOLLOWING METHODS JUST FORWARD TO THE REAL ATOMS OBJECT.
@@ -150,14 +148,17 @@
   /// In a serial simulation, same as GetNumberOfAtoms, in a parallel simulation
   /// it is the sum over these over all processors.
   virtual int GetTotalNumberOfAtoms() const {return realatoms->GetTotalNumberOfAtoms();}
 
   /// Return three integers specifying the CPU layout.
   virtual IVec GetNumberOfCells() const {return realatoms->GetNumberOfCells();}
 
+  /// Get the cartesian momenta
+  virtual const Vec *GetMomenta() {return realatoms->GetMomenta();}
+
   /// Get the supercell
   virtual const Vec *GetCell() const {return realatoms->GetCell();}
 
   /// Get the supercell.   No sanity check!
   virtual const Vec *GET_CELL() const {return realatoms->GET_CELL();}
 
   /// Get the volume of the supercell
@@ -166,15 +167,15 @@
   /// Get the height of the supercell
   virtual const double *GetCellHeights() {return realatoms->GetCellHeights();}
   
   /// Get the inverse supercell
   virtual const Vec *GetInverseCell() {return realatoms->GetInverseCell();}
   
   /// Get a set of all elements present in the simulations.
-  virtual void GetListOfElements(set<int> &elements) {realatoms->GetListOfElements(elements);}
+  virtual void GetListOfElements(set<int> &elements) const {realatoms->GetListOfElements(elements);}
 
   /// Get the masses of the atoms
   virtual const double *GetMasses() {return realatoms->GetMasses();}
 
   /// Set a python array on the atoms.
   virtual void SetData(const char *name, PyObject *data) {realatoms->SetData(name, data);}
 
@@ -214,14 +215,19 @@
   virtual int GetNumbersCounter() const {return realatoms->GetNumbersCounter();}
   
   /// Counter showing changes to the positions.
   ///
   /// Also updated if CellCounter, NumbersCounter or AtomsCounter is updated.
   virtual int GetPositionsCounter() const {return realatoms->GetPositionsCounter();}
 
+  /// Counter showing changes to the momenta.
+  ///
+  /// Reading this counter will cause the momenta to be extracted from Python.
+  virtual int GetMomentaCounter() {return realatoms->GetMomentaCounter();}
+
   /// Print memory usage
   virtual long PrintMemory() const {return realatoms->PrintMemory();}
   
   // Return the map from image atoms to original atoms
   virtual const vector<int> &GetOriginalAtomsMap() const {return original_atom;}
 
   virtual int GetOriginalNumberOfAtoms() const {return nAtoms + nGhosts;}
@@ -240,15 +246,14 @@
   int nSize;
 
   double last_range;
   int cell_counter;
 
   vector<Vec> allpositions;
   vector<asap_z_int> allnumbers;
-  vector<IVec> orig_atoms_translations;  // The original atoms need to be folded into the box.
 
   static const bool bc_are_free[3];
 
   // A translation and two indices for each block of images that share the same
   // translation vector.
   vector<IVec> translations;
   vector<int> first_atom;
```

### Comparing `asap3-3.13.1/Basics/ImagePotential.cpp` & `asap3-3.9.6/Basics/ImagePotential.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 ImagePotential::ImagePotential(PyObject *self, Potential *p) : Potential(self)
 {
   DEBUGPRINT;
   CONSTRUCTOR;
   img_atoms = NULL;
   potential = p;
-  ASSERT(potential != NULL);
+  assert(potential != NULL);
   virials_collect_cnt = force_collect_cnt = 0;
 }
 
 ImagePotential::~ImagePotential()
 {
   DEBUGPRINT;
   DESTRUCTOR;
@@ -90,15 +90,15 @@
         DEBUGPRINT;
         const vector<Vec> &orig_forces = potential->GetForces(a);
         forces = orig_forces;
         CollectFromImages<Vec>(forces);
         force_collect_cnt = cnt;
       }
   }
-  catch (AsapErrorBase &)
+  catch (AsapErrorBase)
   {
       img_atoms->End();
       throw;
   }
   img_atoms->End();
   return forces;
 }
@@ -115,15 +115,15 @@
         DEBUGPRINT;
         const vector<SymTensor> &orig_virials = potential->GetVirials(a);
         virials = orig_virials;
         CollectFromImages<SymTensor>(virials);
         virials_collect_cnt = cnt;
     }
   }
-  catch (AsapErrorBase &)
+  catch (AsapErrorBase)
   {
       img_atoms->End();
       throw;
   }
   img_atoms->End();
   DEBUGPRINT;
   return virials;
```

### Comparing `asap3-3.13.1/Basics/ImagePotential.h` & `asap3-3.9.6/Basics/ImagePotential.h`

 * *Files 7% similar despite different names*

```diff
@@ -82,21 +82,14 @@
 
   /// Return the Python object containing neighbor list for the
   /// potential, if this type of potential supports it, and if it is
   /// defined now.  Otherwise, return NULL without setting a Python
   /// error.
   virtual PyObject *GetNeighborList() const {return potential->GetNeighborList();}
 
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms) {return potential->CheckAndUpdateNbList(pyatoms);}
-
   /// Return the cutoff radius used in the potential.
   virtual double GetCutoffRadius() const {return potential->GetCutoffRadius();}
 
   /// Return the lattice constant of the material, if well-defined.
 
   /// If a lattice constant of the material can be defined, return it
   /// in Angstrom, otherwise throw an exception.
```

### Comparing `asap3-3.13.1/Basics/Langevin.cpp` & `asap3-3.9.6/Basics/Langevin.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -107,43 +107,30 @@
 
 void Langevin::Run2(int nsteps, PyObject *observers, PyObject *self)
 {
   DEBUGPRINT;
 
   ParseObservers(observers);
   DEBUGPRINT;
+  const Vec *F = GetForces();
+  Vec *r = atoms->GetPositions();
+  Vec *p = atoms->GetMomenta();
   vector<Vec> rnd1;
   vector<Vec> rnd2;
   vector<Vec> rrnd;
   vector<Vec> prnd;
-  bool firstloop = true;
-  bool needcalculation = true;
-  Vec *r = NULL;
-  Vec *p = NULL;
-  const Vec *F = NULL;
+  rnd1.reserve(nAtoms + nAtoms/20);
+  rnd2.reserve(nAtoms + nAtoms/20);
+  rrnd.reserve(nAtoms + nAtoms/20);
+  prnd.reserve(nAtoms + nAtoms/20);
+
+
   for (int n = 0; n < nsteps; n++)  // nsteps-1 steps
     {
       CHECKNOASAPERROR; // Unnecessary paranoia.
-      if (needcalculation)
-      {
-	F = GetForces();  // After first iteration, this normally does nothing as
-		          // force is already calculated, but may fix rare trouble.
-	r = atoms->GetPositions();
-	p = atoms->GetMomenta();
-	if (firstloop)
-	  {
-	    // Cannot be done before the loop, as nAtoms becomes set by GetForces().
-	    rnd1.reserve(nAtoms + nAtoms/20);
-	    rnd2.reserve(nAtoms + nAtoms/20);
-	    rrnd.reserve(nAtoms + nAtoms/20);
-	    prnd.reserve(nAtoms + nAtoms/20);
-	    firstloop = false;
-	  }
-	needcalculation = false;
-      }
       // A buffer for the random numbers
       double *sdpos = atoms->GetDoubleData(sdpos_name);
       double *sdmom = atoms->GetDoubleData(sdmom_name);
       double *c1 = atoms->GetDoubleData(c1_name);
       double *c2 = atoms->GetDoubleData(c2_name);
       double *pmcor_v = NULL;
       double *cnst_v = NULL;
@@ -257,17 +244,15 @@
 #pragma omp parallel for
 #endif // _OPENMP
           for (int i = 0; i < nAtoms; i++)
             p[i] += c4 * F[i];
         }
 
       steps++;
-      needcalculation = CallObservers(self);
-      // The observers might change the positions array (e.g. wrapping into box)
-      // so we get a new pointer at the beginning of this loop if an observer was called.
+      CallObservers(self);
     }
   CleanupObservers();
   UpdateStepsInPython(self);
 }
 
 void Langevin::GetRandom(std::vector<Vec> &x1, std::vector<Vec> &x2, bool gaussian /*=true*/)
 {
```

### Comparing `asap3-3.13.1/Basics/Langevin.h` & `asap3-3.9.6/Basics/Langevin.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Matrix3x3.cpp` & `asap3-3.9.6/Basics/Matrix3x3.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Matrix3x3.h` & `asap3-3.9.6/Basics/Matrix3x3.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/MolecularDynamics.cpp` & `asap3-3.9.6/Basics/MolecularDynamics.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -90,48 +90,49 @@
     double timestep)
 {
   DEBUGPRINT;
   Py_INCREF(py_atoms);
   this->py_atoms = py_atoms;
   atoms = new DynamicAtoms(py_atoms);
   calculator = calc;
+  //std::cout << "MolecularDynamics using the calculator " << calc << std::endl;
   this->timestep = timestep;
-  getforcestring = PyUnicode_FromString("get_forces");
+  getforcestring = PyAsapString_FromString("get_forces");
   steps = 0;
   DEBUGPRINT;
 }
 
 MolecularDynamics::~MolecularDynamics()
 {
   Py_DECREF(py_atoms);
   delete atoms;
   DEBUGPRINT;
 }
 void MolecularDynamics::Run(int nsteps, PyObject *observers, PyObject *self)
 {
-  threadchecker UNUSED(th) = threadchecker(py_atoms);
+  threadchecker th = threadchecker(py_atoms);
   keep_pyreference keep_self = keep_pyreference(self);
   Run2(nsteps, observers, self);
 }
 
 const Vec *MolecularDynamics::GetForces()
 {
   // Get forces, either directly from the Asap Potential or through Python.
   if (calculator != NULL)
   {
     const vector<Vec> &forces = calculator->GetForces(py_atoms);
     nAtoms = forces.size();
-    ASSERT(nAtoms == atoms->GetNAtoms());
+    assert(nAtoms == atoms->GetNAtoms());
     return &forces[0];
   }
   else
   {
     const vector<Vec> &forces = GetForcesThroughPython();
     nAtoms = forces.size();
-    ASSERT(nAtoms == atoms->GetNAtoms());
+    assert(nAtoms == atoms->GetNAtoms());
     return &forces[0];
   }
 }
 
 const vector<Vec> &MolecularDynamics::GetForcesThroughPython()
 {
   PyArrayObject *py_forces = AsPyArray(PyObject_CallMethodObjArgs(py_atoms,
@@ -181,15 +182,15 @@
         {
           Py_DECREF(obs);
           Py_DECREF(py_line);
           CleanupObservers();
           throw AsapError("Each observer should be described by a 4-tuple.");
         }
       PyObject **line = PySequence_Fast_ITEMS(py_line);
-      int interval = (int) PyLong_AsLong(line[1]);
+      int interval = (int) PyAsapInt_AsLong(line[1]);
       if (interval < 0)
         {
           Py_DECREF(obs);
           Py_DECREF(py_line);
           CleanupObservers();
           throw AsapError("Observer has negative or non-integer interval.");
         }
@@ -225,35 +226,31 @@
       i != obs_kwargs.end(); ++i)
     {
       Py_DECREF(*i);
     }
   obs_kwargs.clear();
 }
 
-bool MolecularDynamics::CallObservers(PyObject *self)
+void MolecularDynamics::CallObservers(PyObject *self)
 {
   bool stepsupdated = false;
-  bool calledsomething = false;
   int n = obs_callable.size();
-  ASSERT(n == obs_kwargs.size());
+  assert(n == obs_kwargs.size());
   for (int i = 0; i < n; i++)
     if (steps % obs_interval[i] == 0)
       {
         if (!stepsupdated)
           {
             UpdateStepsInPython(self);
             stepsupdated = true;
           }
         PyObject *retval = PyObject_Call(obs_callable[i], obs_args[i], obs_kwargs[i]);
         if (retval == NULL)
           throw AsapPythonError();
-	calledsomething = true;
-	Py_DECREF(retval);
       }
-  return calledsomething;
 }
 
 void MolecularDynamics::UpdateStepsInPython(PyObject *self)
 {
   PyObject *n = Py_BuildValue("l", steps);
   int x = PyObject_SetAttrString(self, "nsteps", n);
   Py_DECREF(n);
```

### Comparing `asap3-3.13.1/Basics/MolecularDynamics.h` & `asap3-3.9.6/Basics/MolecularDynamics.h`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   virtual void Run(int nsteps, PyObject *observers, PyObject *self);
   virtual void Run2(int nsteps, PyObject *observers, PyObject *self) = 0;
 
 protected:
   const Vec *GetForces();
   const std::vector<Vec> &GetForcesThroughPython();
   void ParseObservers(PyObject *observers);
-  bool CallObservers(PyObject *self);  // Returns true if an observer was called.
+  void CallObservers(PyObject *self);
   void CleanupObservers();
   void UpdateStepsInPython(PyObject *self);
 
 protected:
   PyObject *py_atoms;
   DynamicAtoms *atoms;
   int nAtoms;
```

### Comparing `asap3-3.13.1/Basics/MonteCarloAtoms.cpp` & `asap3-3.9.6/Basics/MonteCarloAtoms.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 //#define ASAPDEBUG
 #include "Debug.h"
 
 
 bool MonteCarloAtoms::check_numbers(PyArrayObject *py_numbers, PyArrayObject *py_gh_num,
 				    bool step_count_atoms)
 {
-  ASSERT(py_gh_num == NULL);  // Must be a serial simulation.
+  assert(py_gh_num == NULL);  // Must be a serial simulation.
   PyArrayObject *mc_optim = AsPyArray(PyObject_GetAttrString(py_atoms, "mc_optim"));
   if (mc_optim == NULL)
     throw AsapError("Not a Monte Carlo enabled Atoms object!");
   if (PyArray_NDIM(mc_optim) != 1           // two-dimensional
       || PyArray_TYPE(mc_optim) != NPY_INT     // array of integers
       || !PyArray_ISCARRAY_RO(mc_optim))       // Contiguous etc.
     {
@@ -82,15 +82,15 @@
       return false;
     }
 }
 bool MonteCarloAtoms::check_positions(PyArrayObject *py_positions,
 				      PyArrayObject *py_gh_pos,
 				      bool step_count_atoms_or_cell)
 {
-  ASSERT(py_gh_pos == NULL);  // Must be a serial simulation.
+  assert(py_gh_pos == NULL);  // Must be a serial simulation.
   if (mc_optim_relevant)
     {
       if (modified_atoms.size() == 0)
 	{
 	  // Atoms are not modified! 
 	  mc_optim_relevant = false;
 	  return false;
```

### Comparing `asap3-3.13.1/Basics/MonteCarloAtoms.h` & `asap3-3.9.6/Basics/MonteCarloAtoms.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/NeighborCellLocator.cpp` & `asap3-3.9.6/Basics/NeighborCellLocator.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -80,28 +80,18 @@
   DEBUGPRINT;
 }
 
 NeighborCellLocator::~NeighborCellLocator()
 {
   DESTRUCTOR;
   DEBUGPRINT;
-  for (int i = 0; i < nbCells_onthefly.size(); ++i)
-    delete nbCells_onthefly[i];
-  nbCells_onthefly.clear();
-  DEBUGPRINT;
   AsapAtoms_DECREF(atoms);
   DEBUGPRINT;
 }
 
-void NeighborCellLocator::EnableNeighborsOfGhosts()
-{
-  invalid = true;
-  includeghostneighbors = true;
-}
-
 void NeighborCellLocator::MakeTranslationTable()
 {
   DEBUGPRINT;
   translationTable.resize(27);
   for (int i = 0; i < 3; i++)
     for (int j = 0; j < 3; j++)
       for (int k = 0; k < 3; k++)
@@ -118,44 +108,33 @@
   MEMORY;
   USETIMER("NeighborCellLocator::MakeList");
   if (verbose >= 1)
     cerr << " NeighborCellLocator-Update ";
   nAtoms = atoms->GetNumberOfAtoms();
   nAllAtoms = nAtoms + atoms->GetNumberOfGhostAtoms();
   if (includeghostneighbors)
-    nAtoms = nAllAtoms;
+    nAtoms = nAllAtoms;  // Only happens for SecondaryNeighborList
   /// Update positions and scaledpositions
   ScaleAndNormalizePositions();
-  ASSERT(scaledPositions.size() == nAllAtoms);
+  assert(scaledPositions.size() == nAllAtoms);
   MEMORY;
-
-  // If there are no atoms, we just make empty arrays and return
-  if (nAllAtoms == 0)
-  {
-    cellIndices.resize(0);
-    maxLength = 0.0;
-    invalid = false;
-    DEBUGPRINT;
-    return;   // Nothing to do.
-  }
   
-  DEBUGPRINT;
   const double *cellHeights = atoms->GetCellHeights();
   const bool *atomsperiodic = atoms->GetBoundaryConditions();
   for (int i = 0; i < 3; i++)
     periodic[i] = atomsperiodic[i];
   // Check the size.  As this locator does not use minimum image
   // convention, we can allow height down to rCut rather than the
   // usual 2*rCut.
   for (int i = 0; i < 3; i++)
     if (periodic[i] && cellHeights[i] < rCut)
       THROW( AsapError("NeighborCellLocator: The height of the cell (")
         << cellHeights[i] << ") must be larger than " << rCut );
 
-  const vector<Vec> &UNUSED(positions) = GetWrappedPositions();
+  const vector<Vec> &positions = GetWrappedPositions();
   const vector<Vec> &scaledpositions = GetScaledPositions();
 
   MEMORY;
   // Find the system size in scaled space coordinates.  Use this to
   // determine the number of cells.  If this processor only handles
   // part of space in a periodic direction, we must search for a range
   // of coordinates not present (it will be found on the outermost
@@ -328,15 +307,15 @@
       cells.resize(nTotalCells[3]);
       MEMORY;
       MakeNeighboringCellLists();
     }
   else
     {
       // Empty the old cells, but keep them to minimize reallocations
-      ASSERT(cells.size() == nTotalCells[3]);
+      assert(cells.size() == nTotalCells[3]);
       for (int i = 0; i < cells.size(); i++)
 	cells[i].clear();
     }
   MEMORY;
   cellIndices.resize(nAllAtoms);
   MEMORY;
 
@@ -344,23 +323,23 @@
   for (int a = 0; a < nAllAtoms; a++)
     {
       int index = 0;
       for (int i = 0; i < 3; i++)
 	{
 	  int k =
 	    int((scaledpositions[a][i] - minimum[i]) / size[i] * nCellsTrue[i]);
-	  ASSERT(k >= 0);
+	  assert(k >= 0);
 	  if (k > nCellsGapStart[i])
 	    {
-	      ASSERT (k > nCellsGapStart[i] + nCellsGapSize[i]);
+	      assert (k > nCellsGapStart[i] + nCellsGapSize[i]);
 	      k -= nCellsGapSize[i];
 	    }
 	  if (k == nCells[i])
 	    k--;
-          ASSERT(k < nCells[i]);
+          assert(k < nCells[i]);
 	  index += nTotalCells[i] * k;
 	}
       cells[index].push_back(a);
       cellIndices[a] = index;
     }
 
   // update reference positions for neighbor list:
@@ -476,24 +455,14 @@
       else if (periodic[2])
 	{
 	  data.first -= nTotalCells[3];
 	  data.second = 2 * magic[2];
 	  nbCells_back.push_back(data);
 	}
     }
-  DEBUGPRINT;
-  //std::cerr << "************** cells.size(): " << cells.size() << std::endl;
-  // Make the corner cases (literally!), and build the map
-  nbCells_all.clear();
-  for (int i = 0; i < nbCells_onthefly.size(); ++i)
-    delete nbCells_onthefly[i];
-  nbCells_onthefly.clear();
-  for (int i = 0; i < cells.size(); i++)
-    makeNbCells(i);
-  ASSERT(nbCells_all.size() == cells.size());
 }
 
 int NeighborCellLocator::GetNeighbors(int a1, int *neighbors, Vec *diffs,
 				      double *diffs2, int& size,
 				      double r) const
 {
   return CommonGetNeighbors(a1, neighbors, diffs, diffs2, size, r, false);
@@ -513,201 +482,97 @@
 
 
 void NeighborCellLocator::GetFullNeighbors(int a1, vector<int> &neighbors) const
 {
   CommonGetNeighbors(a1, neighbors, true);
 }
 
-
-int NeighborCellLocator::GetFullNeighborsQuery(Vec &position, int *neighbors, Vec *diffs, double *diffs2,
-                          int& nb_size, double r) const
-{
-  if (invalid)
-    throw AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.") << __LINE__;
-
-  const vector<Vec> &RESTRICT positions = GetWrappedPositions();
-  // Need to use GET_CELL instead of GetCell as the atoms are not open
-  // when called from the Python interface.
-  const Vec *RESTRICT superCell = atoms->GET_CELL();
-
-  // Normalize position
-  Vec wrapped_scaled_position;
-  Vec wrappedpos;
-  ScaleAndNormalizePosition(position, &wrapped_scaled_position, &wrappedpos);
-
-  // Find the cell of this atom
-  int index = 0;
-  for (int i = 0; i < 3; i++)
-  {
-    int k =
-      int((wrapped_scaled_position[i] - minimum[i]) / size[i] * nCellsTrue[i]);
-    if (k > nCellsGapStart[i])
-    {
-      ASSERT (k > nCellsGapStart[i] + nCellsGapSize[i]);
-      k -= nCellsGapSize[i];
-    }
-
-    // When boundaries are free, k may be outside our cell range
-    // We snap k back to the nearest cell and search from there
-    // In principle we could stop the search here 
-    // if k <= -2 or k > nCells[i]+1
-    if (k >= nCells[i])
-    {
-      k = nCells[i]-1;
-    }
-    else if (k < 0)
-    {
-      k = 0;
-    }
-    index += nTotalCells[i] * k;
-  }
-  int thiscell = index;
-
-  double rC2;
-  if (r > 0.0)
-    rC2 = r*r;
-  else
-    rC2 = rCut2;
-
-  int nNeighbors = 0;
-
-  // Ghost atoms have no neighbors - but they are neighbors to real atoms.
-  const nbcell_t *neighborCells = nbCells_all.at(thiscell);
-
-  // Loop over all neighboring cells, including this one
-  for (vector< pair<int, translationsidx_t> >::const_iterator i =
-      neighborCells->begin(); i < neighborCells->end(); ++i)
-  {
-    int othcell = i->first + thiscell;
-    IVec celltranslation = translationTable[i->second];
-    Vec pos1 = wrappedpos + celltranslation[0] * superCell[0] +
-      celltranslation[1] * superCell[1] + celltranslation[2] * superCell[2];
-    // Loop over all atoms in the cell.
-    vector<int>::const_iterator aend = cells[othcell].end();
-
-    for (vector<int>::const_iterator a2 = cells[othcell].begin();
-        a2 < aend; ++a2)
-    {
-      diffs[nNeighbors] = positions[*a2] - pos1;
-      diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-      neighbors[nNeighbors] = *a2;
-      nNeighbors++;
-    }
-  }
-  // Remove neighbors too far away
-  int j = 0;
-  for (int i = 0; i < nNeighbors; i++)
-  {
-    int a2 = neighbors[i];
-    if (i != j)
-    {
-      diffs[j] = diffs[i];
-      diffs2[j] = diffs2[i];
-      neighbors[j] = a2;
-    }
-    if (diffs2[i] < rC2)
-      j++;
-  }
-  nNeighbors = j;
-  nb_size -= nNeighbors;
-  ASSERT(nb_size >= 0);
-  return nNeighbors;
-}
-
-
-void NeighborCellLocator::makeNbCells(int thiscell)
+const NeighborCellLocator::nbcell_t
+&NeighborCellLocator::makeNbCells(int thiscell, nbcell_t &NbCells) const
 {
   IVec cellidx(thiscell % nTotalCells[1],
 	       (thiscell % nTotalCells[2]) / nTotalCells[1],
 	       thiscell / nTotalCells[2]);
-  ASSERT(thiscell == (cellidx[0] * nTotalCells[0] +
+  assert(thiscell == (cellidx[0] * nTotalCells[0] +
 		      cellidx[1] * nTotalCells[1] +
 		      cellidx[2] * nTotalCells[2]));
   int celltype = (cellidx[0] == 0) + 2 * (cellidx[0] == nCells[0]-1)
     + 4 * (cellidx[1] == 0) + 8 * (cellidx[1] == nCells[1]-1)
     + 16 * (cellidx[2] == 0) + 32 * (cellidx[2] == nCells[2]-1);
 
   if (celltype == 0)
-    nbCells_all[thiscell] = &nbCells_inside;
+    return nbCells_inside;
   else if (celltype == 1)
-    nbCells_all[thiscell] =  &nbCells_left;
+    return nbCells_left;
   else if (celltype == 2)
-    nbCells_all[thiscell] =  &nbCells_right;
+    return nbCells_right;
   else if (celltype == 4)
-    nbCells_all[thiscell] =  &nbCells_bottom;
+    return nbCells_bottom;
   else if (celltype == 8)
-    nbCells_all[thiscell] =  &nbCells_top;
+    return nbCells_top;
   else if (celltype == 16)
-    nbCells_all[thiscell] =  &nbCells_front;
+    return nbCells_front;
   else if (celltype == 32)
-    nbCells_all[thiscell] =  &nbCells_back;
-  else
+    return nbCells_back;
+  
+  // Edge or corner cell - make it on the fly.
+  NbCells.clear();
+
+  for (vector<IVec>::const_iterator i = neighborCellOffsets.begin();
+       i != neighborCellOffsets.end(); ++i)
     {
-      // Edge or corner cell - make it on the fly.
-      nbcell_t *NbCells = new nbcell_t;
-      nbCells_onthefly.push_back(NbCells);
-      NbCells->clear();
-      nbCells_all[thiscell] = NbCells;
-
-      for (vector<IVec>::const_iterator i = neighborCellOffsets.begin();
-	   i != neighborCellOffsets.end(); ++i)
-	{
-	  IVec othercell = cellidx + *i;
-	  translationsidx_t xlat = 0;
-	  IVec xlatvec(0,0,0);
-	  IVec magic(1,3,9);
-	  bool ok = true;
-	  for (int j = 0; j < 3; j++)
+      IVec othercell = cellidx + *i;
+      translationsidx_t xlat = 0;
+      IVec xlatvec(0,0,0);
+      IVec magic(1,3,9);
+      bool ok = true;
+      for (int j = 0; j < 3; j++)
+	{
+	  if (othercell[j] < 0)
 	    {
-	      if (othercell[j] < 0)
+	      if (!periodic[j])
 		{
-		  if (!periodic[j])
-		    {
-		      ok = false;
-		      break;
-		    }
-		  othercell[j] += nCells[j];
-		  //std::cerr << "*** Magic j=" << j << ": " << magic[j] << std::endl;
-		  xlat += magic[j] * 1;
-		  xlatvec[j] = 1;
+		  ok = false;
+		  break;
 		}
-	      else if (othercell[j] >= nCells[j])
+	      othercell[j] += nCells[j];
+	      xlat += magic[j] * 1;
+	      xlatvec[j] = 1;
+	    }
+	  else if (othercell[j] >= nCells[j])
+	    {
+	      if (!periodic[j])
 		{
-		  if (!periodic[j])
-		    {
-		      ok = false;
-		      break;
-		    }
-		  othercell[j] -= nCells[j];
-		  //std::cerr << "*** Magic j=" << j << ": " << magic[j] << std::endl;
-		  xlat += magic[j] * 2;
-		  xlatvec[j] = -1;
+		  ok = false;
+		  break;
 		}
-	      //std::cerr << xlat << "  ";
+	      othercell[j] -= nCells[j];
+	      xlat += magic[j] * 2;
+	      xlatvec[j] = -1;
 	    }
-	  if (ok) {
-	    //std::cerr << xlatvec << " ==?== " << xlat << ": " << translationTable[xlat] << std::endl;
-	    ASSERT(xlatvec == translationTable.at(xlat));
-	    pair<int, translationsidx_t> data;
-	    data.first = (othercell[0] * nTotalCells[0] +
-			  othercell[1] * nTotalCells[1] +
-			  othercell[2] * nTotalCells[2]) - thiscell;
-	    data.second = xlat;
-	    NbCells->push_back(data);
-	  }
 	}
+      if (ok) {
+	assert(xlatvec == translationTable[xlat]);
+	pair<int, translationsidx_t> data;
+	data.first = (othercell[0] * nTotalCells[0] +
+		      othercell[1] * nTotalCells[1] +
+		      othercell[2] * nTotalCells[2]) - thiscell;
+	data.second = xlat;
+	NbCells.push_back(data);
+      }
     }
+  return NbCells;
 }
 
 int NeighborCellLocator::CommonGetNeighbors(int a1, int *RESTRICT neighbors, Vec *RESTRICT diffs,
 					    double *RESTRICT diffs2, int& size,
 					    double r, bool wantfull) const
 {
   if (invalid)
-    throw AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.")  << __LINE__;
+    throw AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.");
 
   const vector<Vec> &RESTRICT positions = GetWrappedPositions();
   // Need to use GET_CELL instead of GetCell as the atoms are not open
   // when called from the Python interface.
   const Vec *RESTRICT superCell = atoms->GET_CELL();
 
   // Find the cell of this atom
@@ -719,19 +584,20 @@
     rC2 = rCut2;
 
   int nNeighbors = 0;
 
   // Ghost atoms have no neighbors - but they are neighbors to real atoms.
   if (a1 < nAtoms)
     {
-      const nbcell_t *neighborCells = nbCells_all.at(thiscell);
+      nbcell_t my_neighborCells;
+      const nbcell_t &neighborCells = makeNbCells(thiscell, my_neighborCells);
 
       // Loop over all neighboring cells, including this one
       for (vector< pair<int, translationsidx_t> >::const_iterator i =
-          neighborCells->begin(); i < neighborCells->end(); ++i)
+          neighborCells.begin(); i < neighborCells.end(); ++i)
         {
           int othcell = i->first + thiscell;
           IVec celltranslation = translationTable[i->second];
           Vec pos1 = positions[a1] + celltranslation[0] * superCell[0] +
               celltranslation[1] * superCell[1] + celltranslation[2] * superCell[2];
           // Loop over all atoms in the cell.
           vector<int>::const_iterator aend = cells[othcell].end();
@@ -753,28 +619,28 @@
       int a2 = neighbors[i];
       if (i != j)
         {
           diffs[j] = diffs[i];
           diffs2[j] = diffs2[i];
           neighbors[j] = a2;
         }
-      if ((diffs2[i] < rC2) && ((a2 > a1) || (wantfull && (a2 != a1))))
+      if ((diffs2[i] < rCut2) && ((a2 > a1) || (wantfull && (a2 != a1))))
         j++;
     }
   nNeighbors = j;
   size -= nNeighbors;
-  ASSERT(size >= 0);
+  assert(size >= 0);
   return nNeighbors;
 }
 
 void NeighborCellLocator::CommonGetNeighbors(int a1, vector<int> &neighbors,
 					     bool wantfull) const
 {
   if (invalid)
-    throw AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.") << __LINE__;
+    throw AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.");
   
   const vector<Vec> &positions_x = GetWrappedPositions();
   const Vec *RESTRICT superCell = atoms->GET_CELL();
 
   // Find the cell of this atom
   int thiscell = cellIndices[a1];
   neighbors.resize(maxLength);
@@ -785,20 +651,21 @@
   const Vec *RESTRICT positions = &positions_x[0];
   int *RESTRICT neighbors_p = &neighbors[0];
 
   const IVec *translationTable = &(this->translationTable)[0];
   // Ghost atoms have no neighbors - but they are neighbors to real atoms.
   if (a1 < nAtoms)
     {
-      const nbcell_t *neighborCells = nbCells_all.at(thiscell);
+      nbcell_t my_neighborCells;
+      const nbcell_t &neighborCells = makeNbCells(thiscell, my_neighborCells);
 
       // Loop over all neighboring cells, including this one
-      vector< pair<int, translationsidx_t> >::const_iterator end =  neighborCells->end();
+      vector< pair<int, translationsidx_t> >::const_iterator end =  neighborCells.end();
       for (vector< pair<int, translationsidx_t> >::const_iterator i =
-             neighborCells->begin(); i < end; ++i)
+             neighborCells.begin(); i < end; ++i)
         {
           int othcell = i->first + thiscell;
           IVec celltranslation = translationTable[i->second];
           Vec pos1 = positions[a1] + celltranslation[0] * superCell[0] +
             celltranslation[1] * superCell[1] + celltranslation[2] * superCell[2];
           // Loop over all atoms in the cell.
           vector<int>::const_iterator aend = cells[othcell].end();
@@ -823,36 +690,37 @@
         j++;
     }
   neighbors.resize(j);
   delete[] d2;
 }
 
 int NeighborCellLocator::GetListAndTranslations(int a1,
-       vector<neighboritem_t> &neighbors) const
+       vector< pair<int,translationsidx_t> > &neighbors) const
 {
   if (invalid)
-    THROW( AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.") << __LINE__);
+    THROW( AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.") );
   RETURNIFASAPERROR2(0);
   
   const vector<Vec> &positions = GetWrappedPositions();
   const Vec *superCell = atoms->GetCell();
 
   // Find the cell of this atom
   int thiscell = cellIndices[a1];
   double rC2 = rCut2;
 
   neighbors.clear();
   // Ghost atoms have no neighbors - but they are neighbors to real atoms.
   if (a1 < nAtoms)
     {
-      const nbcell_t *neighborCells = nbCells_all.at(thiscell);
+      nbcell_t my_neighborCells;
+      const nbcell_t &neighborCells = makeNbCells(thiscell, my_neighborCells);
 
       // Loop over all neighboring cells, including this one
       for (vector< pair<int, translationsidx_t> >::const_iterator i =
-             neighborCells->begin(); i < neighborCells->end(); ++i)
+             neighborCells.begin(); i < neighborCells.end(); ++i)
         {
           int othcell = i->first + thiscell;
           IVec celltranslation = translationTable[i->second];
           Vec pos1 = positions[a1] + celltranslation[0] * superCell[0] +
             celltranslation[1] * superCell[1] + celltranslation[2] * superCell[2];
           // Loop over all atoms in the cell.
           vector<int>::const_iterator aend = cells[othcell].end();
@@ -862,62 +730,61 @@
               double l2;
               if ((*a2 > a1) && ((l2 = Length2(positions[*a2] - pos1)) < rC2))
                 {
     #ifdef SLOWASSERT
                   if (l2 < 1e-6)
                     THROW( AsapError("XX Collision between atoms ") << a1 << " and " << *a2 );
     #endif
-                  //neighboritem_t data(*a2, i->second);
-		  neighboritem_t NEIGHBORITEM_PACK(data, *a2, i->second);
+                  pair<int, translationsidx_t> data(*a2, i->second);
                   neighbors.push_back(data);
                 }
             }
         }
     }
   return neighbors.size();
 }  
 
 int NeighborCellLocator::GetComplementaryListAndTranslations(int a1,
-       vector<neighboritem_t> &neighbors) const
+       vector< pair<int,translationsidx_t> > &neighbors) const
 {
   RETURNIFASAPERROR2(0);
   if (invalid)
-    THROW( AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.") << __LINE__ );
+    THROW( AsapError("NeighborCellLocator has been invalidated, possibly by another NeighborList using the same atoms.") );
   
   const vector<Vec> &positions = GetWrappedPositions();
   const Vec *superCell = atoms->GetCell();
 
   // Find the cell of this atom
   int thiscell = cellIndices[a1];
   double rC2 = rCut2;
 
   neighbors.clear();
 
   // Ghost atoms have no neighbors - but they are neighbors to real atoms.
   if (a1 < nAtoms)
     {
-      const nbcell_t *neighborCells = nbCells_all.at(thiscell);
+      nbcell_t my_neighborCells;
+      const nbcell_t &neighborCells = makeNbCells(thiscell, my_neighborCells);
 
       // Loop over all neighboring cells, including this one
       for (vector< pair<int, translationsidx_t> >::const_iterator i =
-             neighborCells->begin(); i < neighborCells->end(); ++i)
+             neighborCells.begin(); i < neighborCells.end(); ++i)
         {
           int othcell = i->first + thiscell;
           IVec celltranslation = translationTable[i->second];
           Vec pos1 = positions[a1] + celltranslation[0] * superCell[0] +
             celltranslation[1] * superCell[1] + celltranslation[2] * superCell[2];
           // Loop over all atoms in the cell.
           vector<int>::const_iterator aend = cells[othcell].end();
           for (vector<int>::const_iterator a2 = cells[othcell].begin();
                a2 < aend; ++a2)
             {
               if ((*a2 < a1) && (Length2(positions[*a2] - pos1) < rC2))
                 {
-                  //neighboritem_t data(*a2, i->second);
-		  neighboritem_t NEIGHBORITEM_PACK(data, *a2, i->second);
+                  pair<int, translationsidx_t> data(*a2, i->second);
                   neighbors.push_back(data);
                 }
             }
         }
     }
   return neighbors.size();
 }  
@@ -1015,34 +882,34 @@
 #if 0
 void NeighborCellLocator::RenormalizeReferencePositions(const vector<Vec>
 							&oldpos)
 {
   if (!invalid)
     {
       int n = atoms->GetNumberOfAtoms();
-      ASSERT(referencePositions.size() == n);
+      assert(referencePositions.size() == n);
       const Vec *pos = atoms->GetPositions();
       for (int i = 0; i < n; ++i)
 	referencePositions[i] += pos[i] - oldpos[i];
     }
 }
 #endif
 
 const vector<Vec> &NeighborCellLocator::GetScaledPositions() const
 {
   DEBUGPRINT;
-  ASSERT(scaledPositionsValid);
+  assert(scaledPositionsValid);
   return scaledPositions;
 }
 
 void NeighborCellLocator::ScaleAndNormalizePositions()
 {
   DEBUGPRINT;
   atoms->GetScaledPositions(scaledPositions, true);  // Get also ghosts
-  ASSERT(scaledPositions.size() == nAllAtoms);
+  assert(scaledPositions.size() == nAllAtoms);
   const bool *pbc = atoms->GetBoundaryConditions();
   // Special-case fully periodic and fully free boundaries
   if (pbc[0] && pbc[1] && pbc[2])
     {
       // Fully periodic boundaries
       int spsz = scaledPositions.size();
       if (wrappedPositions.capacity() < spsz)
@@ -1117,15 +984,15 @@
   DEBUGPRINT;
 }
 
 void NeighborCellLocator::ScaleAndNormalizePositions(const set<int> &modified,
 						     vector<Vec> &scaledpos)
 {
   DEBUGPRINT;
-  ASSERT(modified.size() == scaledpos.size());
+  assert(modified.size() == scaledpos.size());
   atoms->GetScaledPositions(scaledpos, modified);
   const bool *pbc = atoms->GetBoundaryConditions();
   // Special-case fully periodic and fully free boundaries, as they
   // are special-cased in the normal version.
   if (pbc[0] && pbc[1] && pbc[2])
     {
       const Vec *pos = atoms->GetPositions();
@@ -1185,64 +1052,14 @@
 	    + cell[1] * scaledPositions[i][1]
 	    + cell[2] * scaledPositions[i][2];
 	}
       scaledPositionsValid = wrappedPositionsValid = true;
     }
 }
 
-void NeighborCellLocator::ScaleAndNormalizePosition(Vec &position, Vec *outscaledpos, Vec *wrappedpos) const
-{
-  DEBUGPRINT;
-  const bool *pbc = atoms->GET_BOUNDARY_CONDITIONS();
-  const Vec *cell = atoms->GET_CELL();
-  const Vec *inv = atoms->GetInverseCell();
-  Vec scaledpos;
-
-  // Convert to scaled coordinates
-  for (int j = 0; j < 3; j++)
-  {
-    scaledpos[j] = position[0] * inv[0][j]
-                 + position[1] * inv[1][j]
-                 + position[2] * inv[2][j];
-  }
-
-  // Compute wrapped scaled positions
-  if (pbc[0] && pbc[1] && pbc[2])
-  {
-    scaledpos[0] -= floor(scaledpos[0]);
-    scaledpos[1] -= floor(scaledpos[1]);
-    scaledpos[2] -= floor(scaledpos[2]);
-  }
-  else if (!pbc[0] && !pbc[1] && !pbc[2])
-  {
-    // Fully free boundaries: no wrapping - do nothing
-    ;
-  }
-  else
-  {
-    // Mixed boundary conditions
-    int xpbc0 = (int) pbc[0];
-    int xpbc1 = (int) pbc[1];
-    int xpbc2 = (int) pbc[2];
-    Vec offsetpos;
-    offsetpos[0] = -floor(scaledpos[0]) * xpbc0;
-    scaledpos[0] += offsetpos[0];
-    offsetpos[1] = -floor(scaledpos[1]) * xpbc1;
-    scaledpos[1] += offsetpos[1];
-    offsetpos[2] = -floor(scaledpos[2]) * xpbc2;
-    scaledpos[2] += offsetpos[2];
-  }
-
-  // Compute wrapped position from the wrapped scaled position
-  *wrappedpos = cell[0] * scaledpos[0]
-    + cell[1] * scaledpos[1]
-    + cell[2] * scaledpos[2];
-  *outscaledpos = scaledpos;
-}
-
 void NeighborCellLocator::RenormalizePositions()
 {
   DEBUGPRINT;
   scaledPositionsValid = false;
   int nAtoms = this->nAtoms;       // Helps vectorization.
   int nAllAtoms = this->nAllAtoms;  
   const bool *pbc = atoms->GetBoundaryConditions();
@@ -1256,33 +1073,33 @@
 	  // the rescaling.
 	  Vec transformation[3];
 	  matrixMultiply3x3(transformation, old_inverse_cell, atoms->GetCell());
 	  memcpy(old_inverse_cell, atoms->GetInverseCell(), 3*sizeof(Vec));
 	  supercell_counter = atoms->GetCellCounter();
 	  //cerr << endl << __FUNCTION__ << ": " << referencePositions.size()
 	  //     << " " << offsetPositions.size() << endl;
-	  ASSERT(referencePositions.size() == nAtoms);
-	  ASSERT(offsetPositions.size() == nAllAtoms);
+	  assert(referencePositions.size() == nAtoms);
+	  assert(offsetPositions.size() == nAllAtoms);
 	  vector<Vec>::iterator rp = referencePositions.begin();
 	  vector<Vec>::iterator op = offsetPositions.begin();
 	  for(int i = 0; i < nAtoms; ++i, ++rp, ++op)
 	    {
 	      *op = transformation[0] * (*op)[0] + transformation[1] * (*op)[1]
 		+transformation[2] * (*op)[2];
 	      *rp = transformation[0] * (*rp)[0] + transformation[1] * (*rp)[1]
 		+transformation[2] * (*rp)[2];
 	    }
-	  ASSERT(rp == referencePositions.end());
+	  assert(rp == referencePositions.end());
 	  for(int i = nAtoms; i < nAllAtoms; ++i, ++op)
 	    *op = transformation[0] * (*op)[0] + transformation[1] * (*op)[1]
 	      +transformation[2] * (*op)[2];
-	  ASSERT(op == offsetPositions.end());
+	  assert(op == offsetPositions.end());
 	}
       // We now need to rewrap
-      ASSERT(wrappedPositions.size() == nAllAtoms);
+      assert(wrappedPositions.size() == nAllAtoms);
       const Vec *pos = atoms->GetPositions();
       vector<Vec>::const_iterator op = offsetPositions.begin();
       vector<Vec>::iterator end = wrappedPositions.end();
       for (vector<Vec>::iterator wp = wrappedPositions.begin(); wp != end;
 	   ++wp, ++pos, ++op)
 	*wp = *pos + *op;
       wrappedPositionsValid = true;
@@ -1313,16 +1130,16 @@
 	  wrappedPositionsValid = true;
 	}
       else
 	{
 	  // Mixed boundary conditions
 	  const Vec *cell = atoms->GetCell();
 	  atoms->GetScaledPositions(scaledPositions, true);
-	  ASSERT(scaledPositions.size() == scaledOffsetPositions.size());
-	  ASSERT(wrappedPositions.size() == scaledOffsetPositions.size());
+	  assert(scaledPositions.size() == scaledOffsetPositions.size());
+	  assert(wrappedPositions.size() == scaledOffsetPositions.size());
 	  vector<Vec>::const_iterator sop = scaledOffsetPositions.begin();
 	  vector<Vec>::iterator sp = scaledPositions.begin();
 	  vector<Vec>::iterator end = wrappedPositions.end();
 	  for (vector<Vec>::iterator wp = wrappedPositions.begin();
 	       wp != end; ++wp, ++sop, ++sp)
 	    {
 	      *sp += *sop;
@@ -1334,15 +1151,15 @@
     }
   DEBUGPRINT;
 }
 
 void NeighborCellLocator::RemakeLists_Simple(const set<int> &modified)
 {
   DEBUGPRINT;
-  ASSERT(modified.size() > 0);
+  assert(modified.size() > 0);
   // Transform positions to scaled space
   vector<Vec> scaledpos(modified.size());
   ScaleAndNormalizePositions(modified, scaledpos);
 
   const vector<Vec> &positions = GetWrappedPositions();
 
   // Assign to boxes.  Caveat: atom may be outsize the expected
@@ -1360,36 +1177,36 @@
 	    p = minimum[i];
 	  if (p > minimum[i] + size[i])
 	    p = minimum[i] + size[i];
 	  int k = int((p - minimum[i]) / size[i] * nCellsTrue[i]);
 	  if (k > nCellsGapStart[i])
 	    {
 #if 0
-	      ASSERT (k > nCellsGapStart[i] + nCellsGapSize[i]);
+	      assert (k > nCellsGapStart[i] + nCellsGapSize[i]);
 #endif
 	      k -= nCellsGapSize[i];
 	    }
 	  #if 0
-	  ASSERT(k >= 0);
+	  assert(k >= 0);
 #endif
 	  if (k == nCells[i])
 	    k--;
 #if 0
-	  ASSERT(k < nCells[i]);
+	  assert(k < nCells[i]);
 #endif
 	  index += nTotalCells[i] * k;
 	}
       if (index != cellIndices[*a])
 	{
 	  // Remove atom from old cell
 	  vector<int>::iterator i = cells[cellIndices[*a]].begin();
 	  vector<int>::iterator terminate = cells[cellIndices[*a]].end();
 	  while ((*i != *a) && (i != terminate))
 	    ++i;
-	  ASSERT(*i == *a);
+	  assert(*i == *a);
 	  cells[cellIndices[*a]].erase(i);
 	  // Add to new cell
 	  cells[index].push_back(*a);
 	  cellIndices[*a] = index;
 	}
       // We know that the atom is now in the right box
       referencePositions[*a] = positions[*a];
```

### Comparing `asap3-3.13.1/Basics/NeighborCellLocator.h` & `asap3-3.9.6/Basics/NeighborCellLocator.h`

 * *Files 5% similar despite different names*

```diff
@@ -36,48 +36,24 @@
 #include "Asap.h"
 #include "Vec.h"
 #include "NeighborLocator.h"
 #include "IVec.h"
 #include "Templates.h"
 #include <vector>
 using std::vector;
-#include <map>
 #include <utility>
 using std::pair;
 #include <math.h>
-#include <stdint.h>
-
-#define COMPACT_NBLIST
 
 namespace ASAPSPACE {
 
+//typedef unsigned char translationsidx_t;   // Could also be int
 typedef int translationsidx_t;   // Could also be unsigned char
+//typedef long translationsidx_t;   // Silly!
 
-// The datatpe neighboritem_t is mainly used in NeigbhorList.cpp
-// It is a combination of an index into the atoms and an index
-// into a list of translation vectors.
-#ifdef COMPACT_NBLIST
-// A neighborlist item is a single 32-bit unsigned integer,
-// the first 5 bits are the tranlation vector index, the last 27 are
-// the actual neighborlist index.
-typedef uint32_t neighboritem_t;
-#define NEIGHBOR_ITEM_MASK ((1 << 27) - 1)
-#define NEIGHBOR_XLAT_SHIFT 27
-#define NEIGHBOR_INDEX(x) ((x) & NEIGHBOR_ITEM_MASK)
-#define NEIGHBOR_XLAT(x) ((x) >> NEIGHBOR_XLAT_SHIFT)
-#define NEIGHBORITEM_PACK(x,a,b) x = a | (b << NEIGHBOR_XLAT_SHIFT)
-#else // COMPACT_NBLIST
-// A neighborlist item is a pair of an int (the actual neighborlist
-// index) and a translationsidx_t, the translation vector index.
-typedef pair<int,translationsidx_t> neighboritem_t;
-#define NEIGHBOR_INDEX(x) (x).first
-#define NEIGHBOR_XLAT(x) (x).second
-#define NEIGHBORITEM_PACK(x,a,b) x; (x).first = a; (x).second = b;
-#endif // COMPACT_NBLIST
-  
 PyAsap_NeighborLocatorObject *PyAsap_NewNeighborCellLocator(Atoms *a,
      double rCut, double driftfactor = 0.05);
 
 class NeighborCellLocator : public NeighborLocator
 {
 protected:
   /// Generate a neighbor list for atoms a with cutoff rCut.
@@ -87,20 +63,17 @@
   /// more than rCut*driftfactor.
   NeighborCellLocator(Atoms *a, double rCut, double driftfactor = 0.05);
   virtual ~NeighborCellLocator();
 
   friend PyAsap_NeighborLocatorObject *PyAsap_NewNeighborCellLocator(
        Atoms *a, double rCut, double driftfactor);
 
-  friend void PyAsap_Finalize<PyAsap_NeighborLocatorObject>(PyObject *self);
+  friend void PyAsap_Dealloc<PyAsap_NeighborLocatorObject>(PyObject *self);
 
 public:
-  /// Enable neighbors of ghost atoms by calling this just after the constructor
-  void EnableNeighborsOfGhosts();
-
   /// Check if the neighbor list can still be reused, update if not.
   bool CheckAndUpdateNeighborList();
 
   /// Check if the neighbor list can still be reused, update if not.
   ///
   /// This version is used when called from Python
   virtual bool CheckAndUpdateNeighborList(PyObject *atoms);
@@ -111,18 +84,18 @@
   /// it should be updated.
   virtual bool CheckNeighborList();
 
   /// Update neighbor list
   virtual void UpdateNeighborList();
 
   /// Get wrapped positions of all the atoms
-  const vector<Vec> &GetWrappedPositions() const {ASSERT(wrappedPositionsValid); 
+  const vector<Vec> &GetWrappedPositions() const {assert(wrappedPositionsValid); 
     return wrappedPositions;}
 
-  void GetWrappedPositions(vector<Vec> &wp) const {ASSERT(wrappedPositionsValid); 
+  void GetWrappedPositions(vector<Vec> &wp) const {assert(wrappedPositionsValid); 
     wp.insert(wp.begin(), wrappedPositions.begin(), wrappedPositions.end());}
   
   /// Get scaled positions of all the atoms
   const vector<Vec> &GetScaledPositions() const;
 
   /// Get reference positions (used by NeighborList)
   const Vec *GetReferencePositions() const {return &referencePositions[0];}
@@ -152,36 +125,36 @@
   /// This version of GetNeighbors only returns the numbers of the neighbors.
   /// It is intended for the Python interface.
   void GetNeighbors(int n, vector<int> &neighbors) const;
 
   int GetFullNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
 		       int& size, double r = -1.0) const;
 
-  /// Get information about the neighbors around a query position
-  ///
-  /// It is intended for the Python interface
-  int GetFullNeighborsQuery(Vec &position, int *neighbors, Vec *diffs, double *diffs2,
-		       int& nb_size, double r = -1.0) const;
-
   /// Get information about the neighbors of atom n (full neighbor list)
   ///
   /// This version of GetNeighbors only returns the numbers of the neighbors.
   /// It is intended for the Python interface.
   void GetFullNeighbors(int n, vector<int> &neighbors) const;
 
 
   /// Return the neighbors and the corresponding translations.
   ///
   /// The vectors are cleared before data is put into them.
   ///
   /// Return value: The number of neighbors.
-  int GetListAndTranslations(int n, vector<neighboritem_t> &neighbors) const;
+#if 0
+  int GetListAndTranslations(int n, vector<int> &neighbors,
+			     vector<translationsidx_t> &translations) const;
+#endif
+  int GetListAndTranslations(int n, vector< pair<int,translationsidx_t> >
+			     &neighbors) const;
   
   int GetComplementaryListAndTranslations(int n,
-					  vector<neighboritem_t> &neighbors) const;
+					  vector< pair<int,translationsidx_t> >
+					  &neighbors) const;
 
   /// Remake neighbor lists when a few atoms have been modified.
   ///
   /// This version, unlike NeighborList::RemakeList does
   /// not report back which other atoms have been affected.
   void RemakeLists_Simple(const set<int> &modified);
   
@@ -215,23 +188,14 @@
   ///
   /// The first argument is a set of atoms to be normalized, the
   /// corresponding scaled positions are placed in scaledpos.
 
   void ScaleAndNormalizePositions(const set<int> &modified,
 				  vector<Vec> &scaledpos);
 
-  /// Normalize a single position and calculate scaled space version
-  ///
-  /// The first argument is the position to be normalized, the
-  /// corresponding wrapped and scaled position is output in outscaledpos,
-  /// and the corresponding wrapped position in wrappedpos.
-  void ScaleAndNormalizePosition(Vec &position,
-                                 Vec *scaledpos,
-                                 Vec *wrappedpos) const;
-
   /// Normalizing new positions using the normalization already calculated.
   ///
   /// This is used when checking a neighborlist.
   void RenormalizePositions();
 
 #if 0
   /// Renormalize the old positions using old and new positions of the atoms.
@@ -264,17 +228,17 @@
 
   /// Make the lists of neighboring cells.
   void MakeNeighboringCellLists();
 
   /// Make translation table
   void MakeTranslationTable();
 
-  typedef vector< pair<int, translationsidx_t> > nbcell_t;
+  typedef vector<pair<int, translationsidx_t> > nbcell_t;
 
-  void makeNbCells(int thiscell);
+  const nbcell_t &makeNbCells(int thiscell, nbcell_t &NbCells) const;
 
   int CommonGetNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
 			 int& size, double r, bool wantfull) const;
 
   void CommonGetNeighbors(int a1, vector<int> &neighbors,
 			  bool wantfull) const;
 
@@ -315,28 +279,22 @@
   /// The number of the cell to which an atom belongs
   vector<int> cellIndices;
 
   /// For each cell, a list of the neighboring cells, and their offset
   /// across the periodic boundaries.
   vector<IVec> neighborCellOffsets;
 
-  /// List of neighboring cells, valid for ...
-  nbcell_t nbCells_inside;  // ...  a cell not touching the boundary.
-  nbcell_t nbCells_left;    // ...  a cell touching a single boundary.
+  /// List of neighboring cells, valid for a cell not touching the boundary.
+  nbcell_t nbCells_inside;
+  nbcell_t nbCells_left;
   nbcell_t nbCells_right;
   nbcell_t nbCells_top;
   nbcell_t nbCells_bottom;
   nbcell_t nbCells_front;
   nbcell_t nbCells_back;
-
-  /// Lists of neighboring cells for all cells.  Center and sides are
-  /// pointers to the objects above, edges and corners are unique.
-  std::map<int, nbcell_t*> nbCells_all; 
-  vector<nbcell_t*> nbCells_onthefly;  // On-the-fly elements in nbCells_all
-                                       // (for memory management).
   
   /// Table of possible translation vectors
   vector<IVec> translationTable;
 };
 
 } // end namespace
```

### Comparing `asap3-3.13.1/Basics/NeighborList.cpp` & `asap3-3.9.6/Basics/NeighborList.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 // see <http://www.gnu.org/licenses/>.
 
 
 #include "NeighborList.h"
 #include "Atoms.h"
 #include "Exception.h"
 #include "Timing.h"
-// #define ASAPDEBUG
+//#define ASAPDEBUG
 #include "Debug.h"
 #include <iostream>
 #include <stdio.h>
 using std::cerr;
 using std::endl;
 using std::flush;
 
@@ -53,15 +53,14 @@
       atoms = a;
       AsapAtoms_INCREF(atoms);
     }
   nAtoms = 0;  // Not valid yet
   invalid = true;
   firsttime = true;
   fulllists = false;
-  neighborsofghosts = false;
   reservedLength = 0;
   this->rCut = rCut;
   rCut2 = rCut * rCut;
   drift = driftfactor * rCut;
   drift2 = drift * drift;
   // A cell list is used to build the neighbor list.  Its cutoff must
   // include the drift of this list, but it does not need its own
@@ -69,15 +68,15 @@
   // additional migrations when it updates.
   if (rCut <= 0.0)
     throw AsapError("NeighborList: cutoff distance must be positive.");
   PyAsap_NeighborLocatorObject *nbl;
   nbl = PyAsap_NewNeighborCellLocator(atoms, rCut+2*drift, 0.0);
   cells_obj = (PyObject *) nbl;
   cells = dynamic_cast<NeighborCellLocator*>(nbl->cobj);
-  ASSERT(cells);
+  assert(cells);
   cells->GetTranslationTable(translationTable);
 }
 
 NeighborList::~NeighborList()
 {
   DESTRUCTOR;
   CHECKREF(cells_obj);
@@ -87,21 +86,14 @@
 
 void NeighborList::EnableFullNeighborLists()
 {
   invalid = true;
   fulllists = true;
 }
 
-void NeighborList::EnableNeighborsOfGhosts()
-{
-  invalid = true;
-  neighborsofghosts = true;
-  cells->EnableNeighborsOfGhosts();
-}
-
 void NeighborList::MakeList()
 {
   RETURNIFASAPERROR;
   USETIMER("NeighborList::MakeList");
   // Do we have any ghosts?
   //GhostAtoms *ghostAtoms = dynamic_cast<GhostAtoms *>(atoms);
 
@@ -140,28 +132,28 @@
       if (periodic[i] && superCellHeights[i] < 2 * rCut)
         THROW( AsapError("The height of the cell (")
         << superCellHeights[i] << ") must be larger than " << 2 * rCut );
 
     DEBUGPRINT;
     cells->UpdateNeighborList();
     DEBUGPRINT
-    ASSERT(nAtoms == atoms->GetNumberOfAtoms());
+    assert(nAtoms == atoms->GetNumberOfAtoms());
   }
   RETURNIFASAPERROR;
 
   int nAllAtoms = this->nAllAtoms; // Help vectorization
   
   // Make the list
   int myMaxLength = 0;
 #ifdef PRINTLISTSIZE
   int totlistsize = 0;
 #endif
   if (firsttime)
     {
-      vector<neighboritem_t> buf;
+      vector< pair<int, translationsidx_t> > buf;
       buf.reserve(cells->MaxNeighborListLength());
 #ifdef _OPENMP
 #pragma omp for nowait
 #endif // _OPENMP
       for (int i = 0; i < nAllAtoms; i++)
 	{
 	  int l = cells->GetListAndTranslations(i, buf);
@@ -260,14 +252,17 @@
     return true;
 
   int n_at = atoms->GetNumberOfAtoms();
   if (nAtoms != n_at || nAllAtoms != n_at + atoms->GetNumberOfGhostAtoms())
       return true;
 
   bool updateRequired = false;
+  DEBUGPRINT;
+  cells->RenormalizePositions(); // XXX Move out of omp single once parallelized.
+  DEBUGPRINT;
 
   const bool *newpbc = atoms->GetBoundaryConditions();
 
   if (invalid && verbose)
     cerr << "NeighborList::CheckAndUpdateNeighborList: NBList has been marked invalid." << endl;
 
   const Vec *ss = atoms->GetCell();
@@ -279,25 +274,20 @@
       invalid = true;
     }
 
   if (invalid)
     cells->Invalidate();
 
   updateRequired = invalid;
+  const Vec *positions = atoms->GetPositions();
+  const Vec *referencePositions = cells->GetReferencePositions();
 
   if (!updateRequired)
     {
       // Check how much the cell has changed.
-
-      DEBUGPRINT;
-      cells->RenormalizePositions(); // XXX Move out of omp single once parallelized.
-      DEBUGPRINT;
-      const Vec *positions = atoms->GetPositions();
-      const Vec *referencePositions = cells->GetReferencePositions();
-
       double max_strain_disp = GetMaxStrainDisplacement();
       double max2 = drift - max_strain_disp;
       if (max2 <= 0.0)
         updateRequired = true;
       else
         {
           max2 = max2 * max2;
@@ -368,37 +358,37 @@
   // when called from the Python interface.
   double rC2 = rCut2;
   if (r > 0.0)
     rC2 = r * r;
   Vec pos1 = positions[a1];
   int nNeighbors = 0;
 
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   iterat terminate = nbList[a1].end();
 
   if (pbc[0] || pbc[1] || pbc[2])
     {
       // Periodic along at least one direction
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1
-            - translationTable_scaled[NEIGHBOR_XLAT(*a2)];
+          diffs[nNeighbors] = positions[a2->first] - pos1
+            - translationTable_scaled[a2->second];
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
     }
   else
     {
       // Free boundary conditions
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1;
+          diffs[nNeighbors] = positions[a2->first] - pos1;
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
     }
   int j = 0;
   for (int i = 0; i < nNeighbors; i++)
     {
       if (i != j)
@@ -408,15 +398,15 @@
           neighbors[j] = neighbors[i];
         }
       if (diffs2[i] < rC2)
         j++;
     }
   nNeighbors = j;
   size -= nNeighbors;
-  ASSERT(size >= 0);
+  assert(size >= 0);
   return nNeighbors;
 }
 
 void NeighborList::GetNeighbors(int a1, vector<int> &neighbors) const
 {
   if (invalid)
     THROW( AsapError("NeighborList has been invalidated, possibly by another NeighborList using the same atoms.") );
@@ -428,34 +418,34 @@
   const vector<Vec> &positions = cells->GetWrappedPositions();
   Vec pos1 = positions[a1];
 
   const Vec *RESTRICT positions_p = &positions[0];  // Helps vectorization.
   int *RESTRICT neighbors_p = &neighbors[0];
     
   int n = 0;
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   iterat terminate = nbList[a1].end();
   if (pbc[0] || pbc[1] || pbc[2])
     {
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
-          Vec diff = positions_p[NEIGHBOR_INDEX(*a2)] - pos1
-            - translationTable_scaled[NEIGHBOR_XLAT(*a2)];
+          Vec diff = positions_p[a2->first] - pos1
+            - translationTable_scaled[a2->second];
           d2[n] = Length2(diff);
-          neighbors_p[n] = NEIGHBOR_INDEX(*a2);
+          neighbors_p[n] = a2->first;
           n++;
         }
     }
   else
     {
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
-          Vec diff = positions_p[NEIGHBOR_INDEX(*a2)] - pos1;
+          Vec diff = positions_p[a2->first] - pos1;
           d2[n] = Length2(diff);
-          neighbors_p[n] = NEIGHBOR_INDEX(*a2);
+          neighbors_p[n] = a2->first;
           n++;
         }
     }
   int j = 0;
   for (int i = 0; i < n; i++)
     {
       if (i != j)
@@ -489,54 +479,54 @@
   // when called from the Python interface.
   double rC2 = rCut2;
   if (r > 0.0)
     rC2 = r * r;
   Vec pos1 = positions[a1];
   int nNeighbors = 0;
 
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   if (pbc[0] || pbc[1] || pbc[2])
     {
       // Periodic along at least one direction
       iterat terminate = nbList[a1].end();
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1
-            - translationTable_scaled[NEIGHBOR_XLAT(*a2)];
+          diffs[nNeighbors] = positions[a2->first] - pos1
+            - translationTable_scaled[a2->second];
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
       terminate = complNbList[a1].end();
       for (iterat a2 = complNbList[a1].begin(); a2 < terminate; ++a2)
         {
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1
-            - translationTable_scaled[NEIGHBOR_XLAT(*a2)];
+          diffs[nNeighbors] = positions[a2->first] - pos1
+            - translationTable_scaled[a2->second];
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
     }
   else
     {
       // Free boundary conditions
       iterat terminate = nbList[a1].end();
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1;
+          diffs[nNeighbors] = positions[a2->first] - pos1;
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
       terminate = complNbList[a1].end();
       for (iterat a2 = complNbList[a1].begin(); a2 < terminate; ++a2)
         {
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1;
+          diffs[nNeighbors] = positions[a2->first] - pos1;
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
     }
   // Remove neighbors too far away
   int j = 0;
   for (int i = 0; i < nNeighbors; i++)
     {
@@ -548,62 +538,67 @@
         }
       if (diffs2[i] < rC2)
         j++;
     }
   nNeighbors = j;
 
   size -= nNeighbors;
-  ASSERT(size >= 0);
+  assert(size >= 0);
   return nNeighbors;
 }
 
 void NeighborList::GetFullNeighbors(int a1, vector<int> &neighbors) const
 {
   if (!fulllists)
     THROW( AsapError("Calling NeighborList::GetFullNeighbors but full lists are not enabled.") );
   RETURNIFASAPERROR;
   
   const vector<Vec> &positions = cells->GetWrappedPositions();
+  const Vec *superCell;
+  if (atoms->IsActive())
+    superCell = atoms->GetCell();
+  else
+    superCell = storedSuperCell;
   Vec pos1 = positions[a1];
 
   // Get the first half of the neighbor list
   GetNeighbors(a1, neighbors);
 
   // Get the second half
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   iterat terminate = complNbList[a1].end();
   for (iterat a2 = complNbList[a1].begin(); a2 < terminate; ++a2)
     {
-      Vec diff = positions[NEIGHBOR_INDEX(*a2)] - pos1
-	- translationTable_scaled[NEIGHBOR_XLAT(*a2)];
+      Vec diff = positions[a2->first] - pos1
+	- translationTable_scaled[a2->second];
       double d2 = Length2(diff);
       if (d2 < rCut2)
-	  neighbors.push_back(NEIGHBOR_INDEX(*a2));
+	  neighbors.push_back(a2->first);
     }
 }
 
 void NeighborList::RemakeLists(const set<int> &modified, set<int> &affected)
 {
   // Never called in OpenMP context - throwing exceptions is OK.
 #ifdef CHKFULLLIST
   CheckFullListConsistency("Beginning of RemakeLists", false);
 #endif // CHKFULLLIST
 #ifdef CHECKCONSISTENCY
   const vector<Vec> &pos = cells->GetWrappedPositions();
   const Vec *superCell = atoms->GetCell();
 #endif // CHECKCONSISTENCY
   
-  typedef vector<neighboritem_t>::iterator nbiterat;
+  typedef vector< pair<int,translationsidx_t> >::iterator nbiterat;
 
   if (invalid)
     throw AsapError("NeighborList has been invalidated, possibly by another neighbor list sharing the same atoms.");
   if (!fulllists)
     throw AsapError("NeighborList::RemakeLists() only supported if 'full neigbor lists' are enabled.");
   
-  ASSERT(modified.size() > 0);
+  assert(modified.size() > 0);
   affected.clear();
   affected.insert(modified.begin(), modified.end());
 
   // Update the NeighborCellLocator.  The positions of the
   // modified atoms are normalized here.
   cells->RemakeLists_Simple(modified);
 
@@ -611,68 +606,68 @@
   // remove the atoms from the neighbors' lists.  Atoms that are
   // already in the modified set are not affected.
   for (set<int>::const_iterator i = modified.begin(); i != modified.end(); ++i)
     {
       nbiterat terminate = nbList[*i].end();
       for (nbiterat j = nbList[*i].begin(); j != terminate; ++j)
 	{
-	  // NEIGHBOR_INDEX(*j) is a neighbor to modified atom *i
-	  affected.insert(NEIGHBOR_INDEX(*j));
-	  if (!modified.count(NEIGHBOR_INDEX(*j)))
+	  // j->first is a neighbor to modified atom *i
+	  affected.insert(j->first);
+	  if (!modified.count(j->first))
 	    {
 	      // Not in modified set.  Fix its complementary list:
-	      // Remove atom *i from compl. neighbor list of NEIGHBOR_INDEX(*j) 
-	      //int x = complNbList[NEIGHBOR_INDEX(*j)].erase(*i);
-	      nbiterat k = complNbList[NEIGHBOR_INDEX(*j)].begin();
-	      while ((NEIGHBOR_INDEX(*k) != *i) && (k != complNbList[NEIGHBOR_INDEX(*j)].end()))
+	      // Remove atom *i from compl. neighbor list of j->first 
+	      //int x = complNbList[j->first].erase(*i);
+	      nbiterat k = complNbList[j->first].begin();
+	      while ((k->first != *i) && (k != complNbList[j->first].end()))
 		++k;
-	      if (k != complNbList[NEIGHBOR_INDEX(*j)].end())
-		  complNbList[NEIGHBOR_INDEX(*j)].erase(k);
+	      if (k != complNbList[j->first].end())
+		  complNbList[j->first].erase(k);
 #ifdef CHECKCONSISTENCY
 	      else
 		{
 		  // Looks like an inconsistency, but we have to live
 		  // with them if the distance is above rCut.
-		  IVec celltranslation = translationTable[NEIGHBOR_XLAT(*j)];
+		  IVec celltranslation = translationTable[j->second];
 		  Vec pos1 = pos[*i] + celltranslation[0] * superCell[0]
 		    + celltranslation[1] * superCell[1]
 		    + celltranslation[2] * superCell[2];
-		  if (Length2(pos1 - pos[NEIGHBOR_INDEX(*j)]) < rCut2)
+		  if (Length2(pos1 - pos[j->first]) < rCut2)
 		    throw AsapError("Inconsistent neighbor list data: Did not find ")
 		      << *i << " on complementary nb list of atom "
-		      << NEIGHBOR_INDEX(*j);
+		      << j->first;
 		}
 #endif // CHECKCONSISTENCY
 	    }
 	}
       terminate = complNbList[*i].end();
       for (nbiterat j = complNbList[*i].begin(); j != terminate; ++j)
 	{
-	  affected.insert(NEIGHBOR_INDEX(*j));
-	  if (!modified.count(NEIGHBOR_INDEX(*j)))
+	  affected.insert(j->first);
+	  if (!modified.count(j->first))
 	    {
 	      // Not in modified set.  Fix its complementary list
-	      //int x = nbList[NEIGHBOR_INDEX(*j)].erase(*i);
-	      nbiterat k = nbList[NEIGHBOR_INDEX(*j)].begin();
-	      while ((NEIGHBOR_INDEX(*k) != *i) && (k != nbList[NEIGHBOR_INDEX(*j)].end()))
+	      //int x = nbList[j->first].erase(*i);
+	      nbiterat k = nbList[j->first].begin();
+	      while ((k->first != *i) && (k != nbList[j->first].end()))
 		++k;
-	      if (k != nbList[NEIGHBOR_INDEX(*j)].end())
-		  nbList[NEIGHBOR_INDEX(*j)].erase(k);
+	      if (k != nbList[j->first].end())
+		  nbList[j->first].erase(k);
 #ifdef CHECKCONSISTENCY
 	      else
 		{
 		  // Looks like an inconsistency, but we have to live
 		  // with them if the distance is above rCut.
-		  IVec celltranslation = translationTable[NEIGHBOR_XLAT(*j)];
+		  IVec celltranslation = translationTable[j->second];
 		  Vec pos1 = pos[*i] + celltranslation[0] * superCell[0]
 		    + celltranslation[1] * superCell[1]
 		    + celltranslation[2] * superCell[2];
-		  if (Length2(pos1 - pos[NEIGHBOR_INDEX(*j)]) < rCut2)
+		  if (Length2(pos1 - pos[j->first]) < rCut2)
 		    throw AsapError("Inconsistent neighbor list data: Did not find ")
-		      << *i << " on normal nb list of atom " << NEIGHBOR_INDEX(*j);
+		      << *i << " on normal nb list of atom " << j->first;
 		}
 #endif // CHECKCONSISTENCY
 	    }
 	}
     }
 
   // Get new neighbor lists for the modified atoms and for their new neighbors
@@ -680,20 +675,20 @@
   for (set<int>::const_iterator i = modified.begin(); i != modified.end(); ++i)
     {
       int l = cells->GetListAndTranslations(*i, nbList[*i]);
       l += cells->GetComplementaryListAndTranslations(*i, complNbList[*i]);
       if (l > maxLength)
 	maxLength = l;
       for (nbiterat j = nbList[*i].begin(); j != nbList[*i].end(); ++j)
-	if (!modified.count(NEIGHBOR_INDEX(*j)))
-	  newneighbors.insert(NEIGHBOR_INDEX(*j));
+	if (!modified.count(j->first))
+	  newneighbors.insert(j->first);
       for (nbiterat j = complNbList[*i].begin(); j != complNbList[*i].end();
 	   ++j)
-	if (!modified.count(NEIGHBOR_INDEX(*j)))
-	  newneighbors.insert(NEIGHBOR_INDEX(*j));
+	if (!modified.count(j->first))
+	  newneighbors.insert(j->first);
     }
   for (set<int>::const_iterator i = newneighbors.begin();
        i != newneighbors.end(); ++i)
     {
       int l = cells->GetListAndTranslations(*i, nbList[*i]);
       l += cells->GetComplementaryListAndTranslations(*i, complNbList[*i]);
       if (l > maxLength)
@@ -719,14 +714,15 @@
   CheckFullListConsistency("End of RemakeLists");
 #endif
 }
 
 int NeighborList::TestPartialUpdate(set<int> modified, PyObject *pyatoms)
 {
   set<int> dummy;
+  Atoms *atoms = GetAtoms();
   atoms->Begin(pyatoms);
   RemakeLists(modified, dummy);
   atoms->End();
   return dummy.size();
 }
 
 // Check consistency between nbList and complNbList.  Note that with
@@ -742,139 +738,139 @@
   if (invalid || !fulllists)
     return;
   const vector<Vec> &pos = cells->GetWrappedPositions();
   const Vec *superCell = atoms->GetCell();
   double rc2 = rCut + 4*drift;
   double rCut2 = rCut * rCut;
   rc2 *= rc2;
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   // Check that all info on nbList is found on complNbList
   for (int i = 0; i < nAtoms; i++)
     for (iterat j = nbList[i].begin(); j != nbList[i].end(); ++j)
       {
-	// NEIGHBOR_INDEX(*j) is on the nblist of i.  Is i on complnblist of NEIGHBOR_INDEX(*j)?
-	iterat k = complNbList[NEIGHBOR_INDEX(*j)].begin();
-	iterat k_end = complNbList[NEIGHBOR_INDEX(*j)].end();
-	while (NEIGHBOR_INDEX(*k) != i && k != k_end)
+	// j->first is on the nblist of i.  Is i on complnblist of j->first?
+	iterat k = complNbList[j->first].begin();
+	iterat k_end = complNbList[j->first].end();
+	while (k->first != i && k != k_end)
 	  ++k;
-	if (NEIGHBOR_INDEX(*k) != i)
+	if (k->first != i)
 	  {
 	    // Is the inconsistency safe?
-	    IVec celltranslation = translationTable[NEIGHBOR_XLAT(*j)];
+	    IVec celltranslation = translationTable[j->second];
 	    Vec pos1 = pos[i] + celltranslation[0] * superCell[0]
 	      + celltranslation[1] * superCell[1]
 	      + celltranslation[2] * superCell[2];
-	    if (Length2(pos1 - pos[NEIGHBOR_INDEX(*j)]) < rCut2)
-	      throw AsapError("nbList[") << i << "] contains " << NEIGHBOR_INDEX(*j)
-					 << ", but complNbList[" << NEIGHBOR_INDEX(*j)
+	    if (Length2(pos1 - pos[j->first]) < rCut2)
+	      throw AsapError("nbList[") << i << "] contains " << j->first
+					 << ", but complNbList[" << j->first
 					 << "] is missing " << i
 					 << ". (" << where << ")";
 	  }
 	if (chkdst) {
 	  // Are the atoms actually neighbors?
-	  IVec celltranslation = translationTable[NEIGHBOR_XLAT(*j)];
-	  Vec diff = pos[NEIGHBOR_INDEX(*j)] - pos[i] 
+	  IVec celltranslation = translationTable[j->second];
+	  Vec diff = pos[j->first] - pos[i] 
 	    - celltranslation[0] * superCell[0]
 	    - celltranslation[1] * superCell[1]
 	    - celltranslation[2] * superCell[2];
 	  if (Length2(diff) > rc2 + 1e-5)
-	    throw AsapError("nbList[") << i << "] contains " << NEIGHBOR_INDEX(*j)
+	    throw AsapError("nbList[") << i << "] contains " << j->first
 				       << ", but they are too far apart. ("
 				       << where << ") "
 				       << Length2(diff) << " > " << rc2
 				       << "\npos1 = " << pos[i]
-				       << "\npos2 = " << pos[NEIGHBOR_INDEX(*j)]
+				       << "\npos2 = " << pos[j->first]
 				       << "\ntranslation = " << celltranslation;
 	}
       }
   // Check that all info on complNbList is found on nbList
   for (int i = 0; i < nAtoms; i++)
     for (iterat j = complNbList[i].begin(); j != complNbList[i].end(); ++j)
       {
-	// NEIGHBOR_INDEX(*j) is on the complnblist of i.  Is i on nblist of NEIGHBOR_INDEX(*j)?
-	iterat k = nbList[NEIGHBOR_INDEX(*j)].begin();
-	iterat k_end = nbList[NEIGHBOR_INDEX(*j)].end();
-	while (NEIGHBOR_INDEX(*k) != i && k != k_end)
+	// j->first is on the complnblist of i.  Is i on nblist of j->first?
+	iterat k = nbList[j->first].begin();
+	iterat k_end = nbList[j->first].end();
+	while (k->first != i && k != k_end)
 	  ++k;
-	if (NEIGHBOR_INDEX(*k) != i)
+	if (k->first != i)
 	  {
 	    // Is the inconsistency safe?
-	    IVec celltranslation = translationTable[NEIGHBOR_XLAT(*j)];
-	    Vec diff = pos[NEIGHBOR_INDEX(*j)] - pos[i] 
+	    IVec celltranslation = translationTable[j->second];
+	    Vec diff = pos[j->first] - pos[i] 
 	      - celltranslation[0] * superCell[0]
 	      - celltranslation[1] * superCell[1]
 	      - celltranslation[2] * superCell[2];
 	    if (Length2(diff) < rCut2)
-	      throw AsapError("complNbList[") << i << "] contains " << NEIGHBOR_INDEX(*j)
-					      << ", but nbList[" << NEIGHBOR_INDEX(*j)
+	      throw AsapError("complNbList[") << i << "] contains " << j->first
+					      << ", but nbList[" << j->first
 					      << "] is missing " << i
 					      << ". (" << where << ")";
 	  }
       }
 }
 
 void NeighborList::printlist(int n) const
 {
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   cerr << "nbList[" << n << "]";
   for (iterat i = nbList[n].begin(); i != nbList[n].end(); ++i)
-    cerr << " " << NEIGHBOR_INDEX(*i);
+    cerr << " " << i->first;
   cerr << endl;
   if (fulllists)
     {
       cerr << "complNbList[" << n << "]";
       for (iterat i = complNbList[n].begin(); i != complNbList[n].end(); ++i)
-	cerr << " " << NEIGHBOR_INDEX(*i);
+	cerr << " " << i->first;
       cerr << endl;
     }
 } 
 
 void NeighborList::print_info(int n)
 {
   cerr << "NeighborList info on atom " << n << ":" << endl;
   cerr << "nbList:";
   for (int i = 0; i < nbList[n].size(); i++)
-    cerr << "  " << NEIGHBOR_INDEX(nbList[n][i]) << " " << NEIGHBOR_XLAT(nbList[n][i]);
+    cerr << "  " << nbList[n][i].first << " " << nbList[n][i].second;
   cerr << endl;
   if (fulllists)
     {
       cerr << "complNbList:";
       for (int i = 0; i < complNbList[n].size(); i++)
-	cerr << "  " << NEIGHBOR_INDEX(complNbList[n][i]) << " "
-	     << NEIGHBOR_XLAT(complNbList[n][i]);
+	cerr << "  " << complNbList[n][i].first << " "
+	     << complNbList[n][i].second;
       cerr << endl;
     }
   cells->print_info(n);
 }
 
 long NeighborList::PrintMemory() const
 {
   long n = 0;
   long ntot = 0;
-  typedef vector< vector<neighboritem_t> >::const_iterator iter;
+  typedef vector< vector< pair<int, translationsidx_t> > >::const_iterator iter;
   for (iter i = nbList.begin(); i != nbList.end(); i++)
     {
       n += i->size();
       ntot += i->capacity();
     }
   if (fulllists)
     for (iter i = complNbList.begin(); i != complNbList.end(); i++)
       {
 	n += i->size();
 	ntot += i->capacity();
       }
-  long mem = ntot * sizeof(neighboritem_t);
+  long mem = ntot * (sizeof(int) + sizeof(translationsidx_t));
   mem = (mem + 512*1024)/(1024*1024);
-  long overhead = (ntot - n) * sizeof(neighboritem_t);
+  long overhead = (ntot - n) * (sizeof(int) + sizeof(translationsidx_t));
   overhead = (overhead + 512*1024)/(1024*1024);
   char buffer[500];
   snprintf(buffer, 500,
-	   "*MEM* NeighborList %ld MB.  [ overhead %ld MB, %.2e items, full=%d, sizeof(neighboritem_t)=%ld ]",
+	   "*MEM* NeighborList %ld MB.  [ overhead %ld MB, %.2e items, full=%d, sizeof(xlat_idx)=%ld ]",
 	   mem, overhead, (double) n, (int) fulllists,
-	   (long) sizeof(neighboritem_t));
+	   (long) sizeof(translationsidx_t));
   cerr << buffer << endl;
   mem += cells->PrintMemory();
   return mem;
 }
 
 double NeighborList::GetMaxStrainDisplacement()
 {
```

### Comparing `asap3-3.13.1/Basics/NeighborList.h` & `asap3-3.9.6/Basics/NeighborList.h`

 * *Files 2% similar despite different names*

```diff
@@ -44,39 +44,36 @@
 using std::pair;
 #include <math.h>
 #include <string.h>
 
 namespace ASAPSPACE {
 
 PyAsap_NeighborLocatorObject *PyAsap_NewNeighborList(Atoms *atoms, double rCut,
-						     double driftfactor);
+						     double driftfactor, bool master=true);
 
 class NeighborList : public NeighborLocator
 {
 protected:
   /// Generate a neighbor list for atoms a with cutoff rCut.
 
   /// The neighbor list will contain all neighbors within the distance
   /// rCut.  The neighborlist can be reused until an atom has moved
   /// more than rCut*driftfactor. 
   NeighborList(Atoms *a, double rCut, double driftfactor);
   virtual ~NeighborList();
 
   friend ASAPSPACE::PyAsap_NeighborLocatorObject *PyAsap_NewNeighborList(Atoms *atoms,
-     double rCut, double driftfactor);
+     double rCut, double driftfactor, bool master);
 
-  friend void PyAsap_Finalize<PyAsap_NeighborLocatorObject>(PyObject *self);
+  friend void PyAsap_Dealloc<PyAsap_NeighborLocatorObject>(PyObject *self);
   
 public:
   /// Enable full neighbor lists by calling this just after the constructor
   void EnableFullNeighborLists();
 
-  /// Enable neighbors of ghost atoms by calling this just after the constructor
-  void EnableNeighborsOfGhosts();
-
   /// Check if full lists are enabled
   bool HasFullNeighborLists() const {return fulllists;}
 
   /// Get wrapped positions of all the atoms
   const vector<Vec> &GetWrappedPositions() const
   {return cells->GetWrappedPositions();}
 
@@ -216,31 +213,30 @@
   double rCut2;   ///< The square of the cutoff radius.
   double drift;   ///< The maximally allowed drift of an atom.
   double drift2;  ///< The square of the maximally allowed drift of an atom.
   int maxLength;  ///< The length of the longest neighbor list.
   int reservedLength;  ///< How large vectors should we reserve in the memory list. 
   bool firsttime; ///< True during the very first update.
   bool fulllists; ///< True if full neighbor lists are supported.
-  bool neighborsofghosts;  ///< True if neighbors of ghosts are provided.
   bool pbc[3];    ///< Boundary conditions at last update.
   Vec storedSuperCell[3]; ///< So full neighbor list can be accessed.
   Vec referenceSuperCell[3];  ///< For detecting shape changes.
   
   /// Cell locator used when constructing the neighbor list.
   NeighborCellLocator *cells;
   PyObject *cells_obj;
   
   /// Table of possible translation vectors
   vector<IVec> translationTable;
   vector<Vec> translationTable_scaled;  // Multiplied by basis vectors.
 
   /// The actual neigbor list (half list)
-  vector< vector<neighboritem_t> > nbList;
+  vector< vector< pair<int, translationsidx_t> > > nbList;
 
   /// The complementary neighbor list if full lists are enabled.
-  vector< vector<neighboritem_t> > complNbList;
+  vector< vector< pair<int, translationsidx_t> > > complNbList;
 };
 
 } // end namespace
 
 #endif //  NEIGHBORLIST2
```

### Comparing `asap3-3.13.1/Basics/NeighborList2013.cpp` & `asap3-3.9.6/Basics/NeighborList2013.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -41,40 +41,40 @@
 
   // Need to use GET_CELL instead of GetCell as the atoms are not open
   // when called from the Python interface.
   Vec pos1 = positions[a1];
   int nNeighbors = 0;
   asap_z_int a1Element = z[a1];
 
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   iterat terminate = nbList[a1].end();
   if (pbc[0] || pbc[1] || pbc[2])
     {
       // Periodic along at least one direction
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
           // Check to see if the potential neighboring atom should be
           // on the neighbor list of atom a1
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1
-            - translationTable_scaled[NEIGHBOR_XLAT(*a2)];
+          diffs[nNeighbors] = positions[a2->first] - pos1
+            - translationTable_scaled[a2->second];
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
     }
   else
     {
       // Free boundary conditions
       for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
         {
           // Check to see if the potential neighboring atom should be
           // on the neighbor list of atom a1
-          diffs[nNeighbors] = positions[NEIGHBOR_INDEX(*a2)] - pos1;
+          diffs[nNeighbors] = positions[a2->first] - pos1;
           diffs2[nNeighbors] = Length2(diffs[nNeighbors]);
-          neighbors[nNeighbors] = NEIGHBOR_INDEX(*a2);
+          neighbors[nNeighbors] = a2->first;
           nNeighbors++;
         }
     }
   int j = 0;
   const double *cut2 = rcut2_byz[a1Element];
   for (int i = 0; i < nNeighbors; i++)
     {
@@ -85,15 +85,15 @@
           neighbors[j] = neighbors[i];
         }
       if (diffs2[i] <  cut2[z[neighbors[i]]])
         j++;
     }
   nNeighbors = j;
   size -= nNeighbors;
-  ASSERT(size >= 0);
+  assert(size >= 0);
   return nNeighbors;
 }
 
 /// PYTHON VERSION!
 void NeighborList2013::GetNeighbors(int a1, vector<int> &neighbors) const
 {
   if (invalid)
@@ -102,25 +102,25 @@
   neighbors.clear();
   const vector<Vec> &positions = cells->GetWrappedPositions();
   const asap_z_int *z = atoms->GetAtomicNumbers();
 
   Vec pos1 = positions[a1];
   asap_z_int a1Element = z[a1];
 
-  typedef vector<neighboritem_t>::const_iterator iterat;
+  typedef vector< pair<int,translationsidx_t> >::const_iterator iterat;
   iterat terminate = nbList[a1].end();
   for (iterat a2 = nbList[a1].begin(); a2 < terminate; ++a2)
     {
-      Vec diff = positions[NEIGHBOR_INDEX(*a2)] - pos1
-	- translationTable_scaled[NEIGHBOR_XLAT(*a2)];
+      Vec diff = positions[a2->first] - pos1
+	- translationTable_scaled[a2->second];
       /* Assuming that the problem about accessing the element
        * type has been solved a1/2Element should be substituted
        * with the right command! */
       double d2 = Length2(diff);
-      asap_z_int a2Element = z[NEIGHBOR_INDEX(*a2)];
+      asap_z_int a2Element = z[a2->first];
       if (d2 < rcut2_byz[a1Element][a2Element])
-	    neighbors.push_back(NEIGHBOR_INDEX(*a2));
+	    neighbors.push_back(a2->first);
     }
 }
```

### Comparing `asap3-3.13.1/Basics/NeighborList2013.h` & `asap3-3.9.6/Basics/NeighborList2013.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/NeighborLocator.h` & `asap3-3.9.6/Basics/NeighborLocator.h`

 * *Files 2% similar despite different names*

```diff
@@ -161,19 +161,14 @@
 			       double r = -1.0) const
   {throw
       AsapError("Internal error: Calling half neighbor locator as a full one.");}
 
   virtual void GetFullNeighbors(int n, vector<int> &neighbors) const
   {throw
       AsapError("Internal error: Calling half neighbor locator as a full one.");}
-  virtual int GetFullNeighborsQuery(Vec &pos, int *neighbors, Vec *diffs,
-                              double *diffs2, int& size,
-                              double r = -1.0) const
-  {throw
-      AsapError("Internal error: Calling half neighbor locator as a full one.");}
 
   /// Print internal info about an atom
   virtual void print_info(int n) = 0;
 
   /// Print memory usage
   virtual long PrintMemory() const = 0;
```

### Comparing `asap3-3.13.1/Basics/NormalAtoms.cpp` & `asap3-3.9.6/Basics/NormalAtoms.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 {
   CONSTRUCTOR;
   DEBUGPRINT;
   nAtoms = 0;
   nGhosts = 0;
   active = false;
   firsttime = true;
-  hasGhosts = false;
-  count_atoms = count_cell = count_positions 
+  count_atoms = count_cell = count_positions = count_momenta
     = count_numbers = count_inverse_cell = 1;
   py_arrays = py_atoms = NULL;
-  getmasses_pyname = PyUnicode_FromString("get_masses");
-  ASSERT(getmasses_pyname != NULL);
+  momenta_ready = momenta_nonzero = false;
+  getmasses_pyname = PyAsapString_FromString("get_masses");
+  assert(getmasses_pyname != NULL);
   DEBUGPRINT;
 }
 
 NormalAtoms::~NormalAtoms()
 {
   DESTRUCTOR;
   DEBUGPRINT;
@@ -72,20 +72,20 @@
 }
 
 void NormalAtoms::Begin(PyObject *pyatoms, bool allow_reopen /* = false */)
 {
   DEBUGPRINT;
   // Grab a reference to the atoms while we access it, as we may
   // delete object in End() if it is called.
-  ASSERT(pyatoms != NULL);
+  assert(pyatoms != NULL);
   py_atoms = pyatoms;
   Py_INCREF(py_atoms); // DECREFed by End() - or DoBegin if trouble.
   if (active)
     {
-      ASSERT(active > 0);  // If negative something is REALLY wrong.
+      assert(active > 0);  // If negative something is REALLY wrong.
       // Atoms are already open - this may be unexpected!
       if (expect_reopen < active)
         {
           // Yes, unexpected reopen - may happen after an exception has
           // been caught.  Print a warning, then close atoms and continue
           // with lowest-level opening.
           cerr << endl
@@ -105,15 +105,15 @@
           if (allow_reopen)
             expect_reopen = active;
           Py_DECREF(py_atoms);
           return;  // Nothing more to do!
         }
     }
   // OK, atoms are not open, open them.
-  ASSERT(active == 0);
+  assert(active == 0);
   DoBegin(pyatoms);   // also sets active=1 if no exception occurs.
   if (allow_reopen)
     expect_reopen = active;
   else
     expect_reopen = 0;
 }
 
@@ -139,36 +139,20 @@
   // something goes wrong.
   try
     {
       py_arrays = PyObject_GetAttrString(pyatoms, "arrays");
       py_positions = AsPyArray(PyMapping_GetItemString(py_arrays, "positions"));
       py_numbers = AsPyArray(PyMapping_GetItemString(py_arrays, "numbers"));
       py_pbc = AsPyArray(PyObject_GetAttrString(pyatoms, "pbc"));
+      py_cell = AsPyArray(PyObject_GetAttrString(pyatoms, "cell"));
       if ((py_arrays == NULL) || (py_positions == NULL) || (py_numbers == NULL)
-	  || (py_pbc == NULL))
+	  || (py_pbc == NULL) || (py_cell == NULL))
 	throw AsapError("Failed to extract data from the atoms object.");
       DEBUGPRINT;
-      // Extracting the cell depends on the version of Asap.
-      PyObject *cellobj = PyObject_GetAttrString(pyatoms, "cell");
-      if (PyArray_Check(cellobj))
-      {
-	// Old behaviour: this is an array
-	py_cell = AsPyArray(cellobj);
-	cellobj = NULL;  // Reference has been stolen by py_cell.
-      }
-      else
-      {
-	// This is an object with an 'array' attribute containing the actual array
-	py_cell = AsPyArray(PyObject_GetAttrString(cellobj, "array"));
-	Py_DECREF(cellobj);
-	cellobj = NULL;
-      }
-      if (py_cell == NULL)
-	throw AsapError("Failed to extract cell from the atoms object.");
-      
+
       // Check that the positions object is sensible.
 #ifdef PARANOID
       if (PyArray_NDIM(py_positions) != 2           // two-dimensional
 	  || PyArray_DIM(py_positions, 1) != 3         // Second dim is 3
 	  || PyArray_TYPE(py_positions) != NPY_DOUBLE  // array of double
 	  || !PyArray_ISCARRAY_RO(py_positions))       // Contiguous etc.
 	{
@@ -258,15 +242,15 @@
       
       // Check and copy the positions
       step_count_positions =
 	check_positions(py_positions, py_gh_pos,
 			step_count_atoms || step_count_cell);
       DEBUGPRINT;
     }
-  catch(AsapError &)
+  catch(AsapError)
     {
       DEBUGPRINT;
       CHECKREF(py_atoms);
       Py_CLEAR(py_atoms);
       XCHECKREF(py_pbc);
       Py_XDECREF(py_pbc);
       XCHECKREF(py_cell);
@@ -317,14 +301,16 @@
   XCHECKREF(py_ghosts);
   Py_XDECREF(py_ghosts);
   XCHECKREF(py_gh_pos);
   Py_XDECREF(py_gh_pos);
   XCHECKREF(py_gh_num);
   Py_XDECREF(py_gh_num);
     
+  // We have not checked the momenta.
+  momenta_ready = false;
   // Mark that the atoms are now open
   active = 1;
 
   // ParallelAtoms must do something special if boundary conditions
   // have changed.
   if (changed_boundary_conditions && !firsttime)
     NewBoundaryConditions(pbc);
@@ -359,26 +345,20 @@
 #ifdef PARANOID
   if (PyArray_NDIM(py_cell) != 2           // two-dimensional
       || PyArray_DIM(py_cell, 0) != 3         // First dim is 3
       || PyArray_DIM(py_cell, 1) != 3         // Second dim is 3
       || PyArray_TYPE(py_cell) != NPY_DOUBLE  // array of double
       || !PyArray_ISCARRAY_RO(py_cell))       // Contiguous etc.
     throw AsapError("The unit cell has a wrong type or shape.");
-  ASSERT(PyArray_NBYTES(py_cell) == 3 * sizeof(Vec));
+  assert(PyArray_NBYTES(py_cell) == 3 * sizeof(Vec));
 #endif
   if (memcmp(cell, PyArray_DATA(py_cell), 3*sizeof(Vec)) != 0)
     {
       step_count_cell = true;
       memcpy(cell, PyArray_DATA(py_cell), 3*sizeof(Vec));
-      // Check if the unit cell contains vectors of zero length.
-      for(int i = 0; i < 3; i++)
-      {
-	if(Length2(cell[i]) == 0.0)
-	  throw AsapError("Invalid unit cell: One or more vectors has zero length.");
-      }
     }
   return step_count_cell;
 }
 
 // Helper function for NormalAtoms::check_numbers
 template<class T>
 static void copynum(vector<asap_z_int> &num, 
@@ -390,15 +370,15 @@
     *j++ = (asap_z_int) from[i];
   if (py_gh_num != NULL)
     {
       from = (T *) PyArray_DATA(py_gh_num);
       for (int i = 0; i < PyArray_DIM(py_gh_num,0); i++)
 	*j++ = (asap_z_int) from[i];
     }
-  ASSERT(j == num.end()); 
+  assert(j == num.end()); 
 }
 
 template<class T>
 static bool chknum(vector<asap_z_int> &num, 
     PyArrayObject *py_numbers, PyArrayObject *py_gh_num)
 {
   bool step_count_numbers = false;
@@ -412,15 +392,15 @@
     }
   if (py_gh_num)
     {
       from = (T *) PyArray_DATA(py_gh_num);
       for (int i = 0; i < PyArray_DIM(py_gh_num,0); i++)
 	*j++ = (asap_z_int) from[i];
     }
-  ASSERT(j == num.end());
+  assert(j == num.end());
   return step_count_numbers;
 }
 
 bool NormalAtoms::check_numbers(PyArrayObject *py_numbers, PyArrayObject *py_gh_num,
 			  bool step_count_atoms)
 {
   bool step_count_numbers = false;
@@ -480,23 +460,23 @@
       memcpy(&positions[0], PyArray_DATA(py_positions), nAtoms*sizeof(Vec));
       if (py_gh_pos && nGhosts > 0)
 	memcpy(&positions[nAtoms], PyArray_DATA(py_gh_pos),
 	       nGhosts*sizeof(Vec));
 #if 0
       for (int aa=0; aa < nAtoms; aa++)
 	{
-	  ASSERT(!isnan(positions[aa][0]));
-	  ASSERT(!isnan(positions[aa][1]));
-	  ASSERT(!isnan(positions[aa][2]));
+	  assert(!isnan(positions[aa][0]));
+	  assert(!isnan(positions[aa][1]));
+	  assert(!isnan(positions[aa][2]));
 	}
       for (int aa=nAtoms; aa < nAtoms+nGhosts; aa++)
 	{
-	  ASSERT(!isnan(positions[aa][0]));
-	  ASSERT(!isnan(positions[aa][1]));
-	  ASSERT(!isnan(positions[aa][2]));
+	  assert(!isnan(positions[aa][0]));
+	  assert(!isnan(positions[aa][1]));
+	  assert(!isnan(positions[aa][2]));
 	}
 #endif
     }
   return step_count_positions;
 }
 
 void NormalAtoms::End()
@@ -519,41 +499,41 @@
       DEBUGPRINT;
     }
 }
 
 void NormalAtoms::GetPositions(vector<Vec> &pos, bool ghosts /* = false */) const
 {
   DEBUGPRINT;
-  ASSERT(active);
+  assert(active);
   pos.clear();
   if (ghosts || nGhosts == 0)
     {
-      ASSERT(positions.size() == nAtoms + nGhosts);
+      assert(positions.size() == nAtoms + nGhosts);
       if (pos.capacity() < nAtoms + nGhosts)
         pos.reserve(nAtoms + nGhosts + (nAtoms + nGhosts)/25);  // 4% extra
       pos.insert(pos.begin(), positions.begin(), positions.end());
     }
   else
     {
       if (pos.capacity() < nAtoms)
         pos.reserve(nAtoms + nAtoms/25);  // 4% extra
       pos.insert(pos.begin(), positions.begin(), positions.begin() + nAtoms);
-      ASSERT(pos.size() == nAtoms);
+      assert(pos.size() == nAtoms);
     }
   DEBUGPRINT;
 }
  
 
 void NormalAtoms::GetScaledPositions(vector<Vec> &pos, bool ghosts /* = false */)
 {
   DEBUGPRINT;
   int n = nAtoms;
   if (ghosts)
     n += nGhosts;
-  ASSERT(positions.size() >= n);
+  assert(positions.size() >= n);
   const Vec *inv = GetInverseCell();
   if (pos.capacity() < n)
     pos.reserve(n + n/25);  // Reserve 4% extra.
   pos.resize(n);
   for (int i = 0; i < n; i++)
     for (int j = 0; j < 3; j++)
       pos[i][j] = positions[i][0] * inv[0][j]   
@@ -561,77 +541,130 @@
                 + positions[i][2] * inv[2][j];
   DEBUGPRINT;
 }
 
 void NormalAtoms::GetScaledPositions(vector<Vec> &scaledpos, const set<int> &which)
 {
   DEBUGPRINT;
-  ASSERT(scaledpos.size() == which.size());
+  assert(scaledpos.size() == which.size());
   const Vec *inv = GetInverseCell();
   vector<Vec>::iterator spi = scaledpos.begin();
   for (set<int>::const_iterator i = which.begin(); i != which.end(); ++i,++spi)
     for (int j = 0; j < 3; j++)
       (*spi)[j] = positions[*i][0] * inv[0][j]
                 + positions[*i][1] * inv[1][j]
                 + positions[*i][2] * inv[2][j];
   DEBUGPRINT;
 }
 
-const asap_z_int *NormalAtoms::GetAtomicNumbers()
-{
-  SASSERT(active);
-  if (numbers.size() <= 0)
-    NoAtomsErrorOrWarning();    // Defined in AtomsBasis.h but redefined for parallel simul where this is only a warning.
-  return &numbers[0];
-}
-
-void NormalAtoms::GetListOfElements(set<int> &elements)
+void NormalAtoms::GetListOfElements(set<int> &elements) const
 {
   DEBUGPRINT;
   const asap_z_int *atomicnumbers = GetAtomicNumbers();
 
   elements.clear();
   for (int i = 0; i < nAtoms; i++)
     {
       int z = atomicnumbers[i];
       if (elements.find(z) == elements.end())
         elements.insert(z);
     }
   DEBUGPRINT;
 }
+
+const Vec *NormalAtoms::GetMomenta()
+{
+  DEBUGPRINT;
+  (void) GetMomentaCounter();  // Make sure momenta are updated
+  if (momenta_ready)
+    return &momenta[0];
+  else
+    return NULL;
+}
+
+int NormalAtoms::GetMomentaCounter()
+{
+  DEBUGPRINT;
+  assert(active);
+  if (!momenta_ready)
+    {
+      PyArrayObject *py_momenta = AsPyArray(PyDict_GetItemString(py_arrays, "momenta"));
+      if (py_momenta != NULL)
+        {
+#ifdef PARANOID
+          // Check that the positions object is sensible.
+          if (PyArray_NDIM(py_momenta) != 2           // two-dimensional
+              || PyArray_DIM(py_momenta, 0) != nAtoms    // Fisrt dim is nAtoms
+              || PyArray_DIM(py_momenta, 1) != 3         // Second dim is 3
+              || PyArray_TYPE(py_momenta) != NPY_DOUBLE  // array of double
+              || !PyArray_ISCARRAY_RO(py_momenta))       // Contiguous etc.
+            throw AsapError("The momenta array has a wrong type or shape.");
+#endif
+          bool step_mom_ctr = false;
+          if (momenta.size() != nAtoms)
+            {
+              step_mom_ctr = true;
+              momenta.resize(nAtoms);
+            }
+          else
+            step_mom_ctr = (memcmp(&momenta[0], PyArray_DATA(py_momenta),
+                nAtoms*sizeof(Vec)) != 0);
+          if (step_mom_ctr)
+            {
+              count_momenta++;
+              memcpy(&momenta[0], PyArray_DATA(py_momenta), nAtoms*sizeof(Vec));
+            }
+          momenta_nonzero = true;
+          momenta_ready = true;
+        }
+      else
+        {
+          // No momenta, make them zero
+          PyErr_Clear();  // Clear the KeyError from PyDict_GetItemString
+          if ((momenta.size() != 0) && momenta_nonzero)
+            count_momenta++;  // OK, this is a change
+          momenta.resize(nAtoms);
+          memset(&momenta[0], 0, nAtoms*sizeof(Vec));
+          momenta_nonzero = false;
+          momenta_ready = true;
+        }
+    }
+  DEBUGPRINT;
+  return count_momenta;
+}
   
 const double *NormalAtoms::GetMasses()
 {
   if (py_masses == NULL)
     {
-      ASSERT(active);
+      assert(active);
       py_masses = AsPyArray(PyObject_CallMethodObjArgs(py_atoms, getmasses_pyname, NULL));
       if (py_masses == NULL)
         throw AsapPythonError();
 #ifdef PARANOID
       if (PyArray_NDIM(py_masses) != 1              // one-dimensional
           || PyArray_DIM(py_masses, 0) < nAtoms       // Correct size
           || PyArray_TYPE(py_masses) != NPY_DOUBLE  // array of double
           || !PyArray_ISCARRAY_RO(py_masses)
           )       // Contiguous etc.
         {
           DEBUGPRINT;
-          std::cerr << PyUnicode_AsUTF8(PyObject_Repr((PyObject *) py_masses)) << std::endl;
+          std::cerr << PyAsapString_AsString(PyObject_Repr((PyObject *) py_masses)) << std::endl;
           throw AsapError("The masses array has a wrong type or shape.");
         }
 #endif
     }
   return (const double *) PyArray_DATA(py_masses);
 }
 
 double NormalAtoms::GetVolume() const
 {
   DEBUGPRINT;
   double det;
-  ASSERT(active);
+  assert(active);
   det = -cell[0][2]*cell[1][1]*cell[2][0] +
     cell[0][1]*cell[1][2]*cell[2][0] +
     cell[0][2]*cell[1][0]*cell[2][1] -
     cell[0][0]*cell[1][2]*cell[2][1] -
     cell[0][1]*cell[1][0]*cell[2][2] +
     cell[0][0]*cell[1][1]*cell[2][2];
   DEBUGPRINT;
@@ -653,16 +686,15 @@
     invert_cell();
   return inverse;
 }
 
 void NormalAtoms::invert_cell()
 {
   DEBUGPRINT;
-  if (!active)
-    throw AsapError("NormalAtoms::invert_cell() called with inactive atoms (Neighborlist used on modified atoms?)");
+  assert(active);
   count_inverse_cell = count_cell;
   double determinant = Cross(cell[0], cell[1]) * cell[2];
   // Find heights
   for (int i = 0; i < 3; i++)
     {
       Vec inv = Cross(cell[(i + 1) % 3], cell[(i + 2) % 3]);
       heights[i] = fabs(determinant) / sqrt(Length2(inv));
@@ -698,47 +730,47 @@
   DEBUGPRINT;
   return flag;
 }
 
 // Set a python array on the atoms.
 void NormalAtoms::SetData(const char *name, PyObject *data)
 {
-  ASSERT(py_arrays != NULL);
+  assert(py_arrays != NULL);
   if (PyDict_SetItemString(py_arrays, name, data) == -1)
     throw AsapPythonError();
 }
 
 // Get a python array from the atoms
 PyObject *NormalAtoms::GetData(const char *name)
 {
-  ASSERT(py_arrays != NULL);
+  assert(py_arrays != NULL);
   PyObject *res = PyDict_GetItemString(py_arrays, name);
   if (res == NULL)
     throw AsapError("Failed to get array from atoms: ") << name;
   Py_INCREF(res);
   return res;
 }
 
 // Remove a python array from the atoms
 void NormalAtoms::DeleteData(const char *name)
 {
-  ASSERT(py_arrays != NULL);
+  assert(py_arrays != NULL);
   if (PyDict_DelItemString(py_arrays, name) == -1)
     throw AsapError("Failed to delete array from atoms: ") << name;
 }
     
 
 /// Get a Python array of integers, convert to C++ vector
 void NormalAtoms::GetIntegerData(const char *name, vector<asap_z_int> &data, 
                                  bool ghosts /* =false */) const
 {
   DEBUGPRINT;
-  ASSERT(active);
+  assert(active);
   data.clear();
-  ASSERT(py_arrays != NULL);
+  assert(py_arrays != NULL);
   PyArrayObject *d = AsPyArray(PyDict_GetItemString(py_arrays, name));
   if (d == NULL)
     throw AsapError("Failed to get array with name ") << name;
   if (PyArray_NDIM(d) != 1           // One-dimensional
 	  || PyArray_DIM(d, 0) != nAtoms // One per atom
 	  || !PyArray_ISINTEGER(d)       // array of integers
 	  || !PyArray_ISCARRAY_RO(d))    // Contiguous etc.
@@ -785,14 +817,15 @@
 	throw AsapError("Integer data array is an unsupported integer type: ") << name;
 }      
     
 long NormalAtoms::PrintMemory() const
 {
   long mem = 0;  // Count the big stuff.
   mem += positions.capacity() * sizeof(Vec);
+  mem += momenta.capacity() * sizeof(Vec);
   mem += numbers.capacity() * sizeof(int);
   mem = (mem + 512*1024)/(1024*1024);
   char buffer[500];
   snprintf(buffer, 500, "*MEM* Atoms/C++  %ld MB.", mem);
   cerr << buffer << endl;
   return mem;
 }
```

### Comparing `asap3-3.13.1/Basics/NormalAtoms.h` & `asap3-3.9.6/Basics/NormalAtoms.h`

 * *Files 4% similar despite different names*

```diff
@@ -89,33 +89,33 @@
   /// Finish accessing the Python atoms, freeing resources.
   virtual void End();
   
   /// Are the atoms active (opened by Begin()) ?
   virtual bool IsActive() const {return active;}
   
   /// Get the number of atoms
-  virtual int GetNumberOfAtoms() const {SASSERT(active) return nAtoms;}
+  virtual int GetNumberOfAtoms() const {ASSERT(active) return nAtoms;}
 
   /// Get the number of ghost atoms
-  virtual int GetNumberOfGhostAtoms() const {SASSERT(active) return nGhosts;}
+  virtual int GetNumberOfGhostAtoms() const {ASSERT(active) return nGhosts;}
   
   /// Get total number of atoms in parallel simulation.
   ///
   /// In a serial simulation, same as GetNumberOfAtoms, in a parallel simulation
   /// it is the sum over these over all processors.
   virtual int GetTotalNumberOfAtoms() const {return GetNumberOfAtoms();}
 
   /// Do we have ghost atoms? True if arrays are present, even if empty.
   virtual bool HasGhostAtoms() const {return hasGhosts;}
 
   /// Return three integers specifying the CPU layout.
   virtual IVec GetNumberOfCells() const {return IVec(1,1,1);}
 
   /// Get the cartesian positions.  Ghost positions, if any, are at the end.
-  virtual const Vec *GetPositions() const {SASSERT(active) return &positions[0];}
+  virtual const Vec *GetPositions() const {ASSERT(active) return &positions[0];}
 
   /// Get a copy of the cartesian positions.
   ///
   /// Include ghosts if possible and requested.
   virtual void GetPositions(vector<Vec> &pos, bool ghosts=false) const;
   
   /// Get a copy of the positions converted to scaled space.
@@ -123,46 +123,47 @@
   /// Include ghosts if possible and requested.
   virtual void GetScaledPositions(vector<Vec> &scaledpos, bool ghosts=false);
 
   /// Get a copy of some positions, converted to scaled space.
   virtual void GetScaledPositions(vector<Vec> &scaledpos, const set<int> &which);
 
   /// Get the atomic numbers
-  virtual const asap_z_int *GetAtomicNumbers();
+  virtual const asap_z_int *GetAtomicNumbers() const
+  {ASSERT(active) assert(numbers.size() > 0); return &numbers[0];}
   
+  /// Get the cartesian momenta
+  virtual const Vec *GetMomenta();
+
   /// Get the boundary conditions.
   virtual const bool *GetBoundaryConditions() const
-  {SASSERT(active) return pbc;}
-  /// Get boundary conditions. No sanity check!
-  virtual const bool *GET_BOUNDARY_CONDITIONS() const
-  {return pbc;}
+  {ASSERT(active) return pbc;}
 
   virtual bool AllFreeBoundaries() const
-  {SASSERT(active) return all_free_boundaries;}
+  {ASSERT(active) return all_free_boundaries;}
 
   virtual bool AllPeriodicBoundaries() const
-  {SASSERT(active) return all_periodic_boundaries;}
+  {ASSERT(active) return all_periodic_boundaries;}
 
   /// Get the supercell
-  virtual const Vec *GetCell() const {SASSERT(active) return cell;}
+  virtual const Vec *GetCell() const {ASSERT(active) return cell;}
 
   /// Get the supercell.   No sanity check!
   virtual const Vec *GET_CELL() const {return cell;}
 
   /// Get the volume of the supercell
   virtual double GetVolume() const;
   
   /// Get the height of the supercell
   virtual const double *GetCellHeights();
   
   /// Get the inverse supercell
   virtual const Vec *GetInverseCell();
   
   /// Get a set of all elements present in the simulations.
-  virtual void GetListOfElements(set<int> &elements);
+  virtual void GetListOfElements(set<int> &elements) const;
 
   /// Get the masses of the atoms
   virtual const double *GetMasses();
 
   /// Set a python array on the atoms.
   virtual void SetData(const char *name, PyObject *data);
 
@@ -170,14 +171,15 @@
   virtual PyObject *GetData(const char *name);
 
   /// Remove a python array from the atoms
   virtual void DeleteData(const char *name);
 
   /// Get a Python array of integers, convert to C++ vector
   virtual void GetIntegerData(const char *name, vector<asap_z_int> &data, bool ghosts=false) const;
+
   
   /// Update flag and counters across processors.
   ///
   /// Called by a Potential with a flag indicating if the neighborlist
   /// should be updated.  In a serial simulation, just return the flag.
   ///
   /// In a parallel simulation, communicate across processors so the
@@ -197,33 +199,38 @@
   /// date during the energy/force calculations.  If the data should
   /// be communicated at the beginning of the calculation, it should
   /// instead be placed in a ghost array.
   ///
   /// NB: In a serial simulation, do nothing except checking that no
   /// ghosts are present.
   virtual void CommunicateData(double *address, int n = 1)
-  {ASSERT(nGhosts == 0);}
+  {assert(nGhosts == 0);}
   
   /// Counter showing changes to the number of atoms or boundary conditions
-  virtual int GetAtomsCounter() const {SASSERT(active) return count_atoms;}
+  virtual int GetAtomsCounter() const {ASSERT(active) return count_atoms;}
 
   /// Counter showing changes to the unit cell
   ///
   /// Also updated if AtomsCounter has changed.
-  virtual int GetCellCounter() const {SASSERT(active) return count_cell;}
+  virtual int GetCellCounter() const {ASSERT(active) return count_cell;}
 
   /// Counter showing changes to the atomic numbers.
   ///
   /// Also updated if AtomsCounter has changed.
-  virtual int GetNumbersCounter() const {SASSERT(active) return count_numbers;}
+  virtual int GetNumbersCounter() const {ASSERT(active) return count_numbers;}
   
   /// Counter showing changes to the positions.
   ///
   /// Also updated if CellCounter, NumbersCounter or AtomsCounter is updated.
-  virtual int GetPositionsCounter() const {SASSERT(active) return count_positions;}
+  virtual int GetPositionsCounter() const {ASSERT(active) return count_positions;}
+
+  /// Counter showing changes to the momenta.
+  ///
+  /// Reading this counter will cause the momenta to be extracted from Python.
+  virtual int GetMomentaCounter();
 
   /// Print memory usage
   virtual long PrintMemory() const;
   
 protected:
   /// Start accessing the Python atoms.
   ///
@@ -255,33 +262,38 @@
   bool hasGhosts;         ///< We have ghost atoms.
   
   int active;             ///< 1 (or larger) if currently processing atoms.
   int expect_reopen;      ///< Allow new calls to Begin while active==expect_reopen.
   int nAtoms;             ///< The number of atoms.
   int nGhosts;            ///< The number of ghost atoms.
   vector<Vec> positions;  ///< A copy of the positions of the atoms.
+  vector<Vec> momenta;    ///< A copy of the momenta.
   vector<asap_z_int> numbers;    ///< A copy of the atomic numbers.
   
   Vec cell[3];            ///< The unit cell
   bool pbc[3];            ///< Boundary conditions
   bool all_free_boundaries;      ///< All pbc[] are false
   bool all_periodic_boundaries;  ///< All pbc[] are true
   Vec inverse[3];         ///< Inverse unit cell
   double heights[3];      ///< Heights of the unit cell
 
   PyObject *py_atoms;     ///< Stored reference to the atoms object.
   PyObject *py_arrays;    ///< Stored reference to arrays dictionary.
   PyArrayObject *py_masses;    ///< NumPy array containing the masses
   PyObject *getmasses_pyname;  ///< Python string "get_masses" (optimization).
 
+  bool momenta_ready;   ///< The momenta have been read and checked.
+  bool momenta_nonzero; ///< The momenta may be non-zero.
+
   // The counters.  Remember to update ParallelAtoms::UpdateBeforeCalculation
   // when adding new counters.
   int count_atoms;     ///< Counts rare, significant changes to atoms.
   int count_cell;      ///< Counts changes to the supercell.
   int count_positions; ///< Counts changes to the positions
   int count_numbers;   ///< Counts changes to the atomic numbers.
+  int count_momenta;   ///< Counts changes to the momenta.
   int count_inverse_cell; ///< When was the inverse cell last updated?
 };
 
 } // end namespace
 
 #endif // NORMALATOMS_H
```

### Comparing `asap3-3.13.1/Basics/RandomNumbers.cpp` & `asap3-3.9.6/Basics/RandomNumbers.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/RandomNumbers.h` & `asap3-3.9.6/Basics/RandomNumbers.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/SymTensor.h` & `asap3-3.9.6/Basics/SymTensor.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Timing.cpp` & `asap3-3.9.6/Basics/Timing.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Timing.h` & `asap3-3.9.6/Basics/Timing.h`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
   parenttimer = 0;
   activemaster = 0;
   count = 0;
 }
 
 void Timing_timer::Start(Timing_timer *parent)
 {
-  ASSERT(active == 0);
+  assert(active == 0);
   active = 1;
   count++;
   Timing_gettimes(&runningwall, &runningcpu);
   parenttimer = parent;
   if (parent) {
     parent->GoToChild(runningwall, runningcpu);
     activemaster = masters[parent->name];
@@ -220,52 +220,52 @@
   }
   else
     activemaster = 0;
 }
 
 void Timing_timer::Start(clock_t w, clock_t c)
 {
-  ASSERT(active == 0);
+  assert(active == 0);
   active = 1;
   count++;
   runningwall = w;
   runningcpu = c;
   parenttimer = 0;
   activemaster = 0;
 }
 
 void Timing_timer::Stop()
 {
-  ASSERT(active == 1);
+  assert(active == 1);
   active = 0;
   clock_t w, c;
   Timing_gettimes(&w, &c);
   walltime += w - runningwall;
   cputime += c - runningcpu;
   if (parenttimer)
     parenttimer->ReturnFromChild(w, c);
   if (activemaster)
     activemaster->Stop();
 }
 
 void Timing_timer::GoToChild(clock_t w, clock_t c)
 {
-  ASSERT(active == 1);
+  assert(active == 1);
   active = 2;
   walltime += w - runningwall;
   cputime += c - runningcpu;
   runningwall = w;
   runningcpu = c;
   if (activemaster)
     activemaster->GoToChild(w, c);
 }
 
 void Timing_timer::ReturnFromChild(clock_t w, clock_t c)
 {
-  ASSERT(active == 2);
+  assert(active == 2);
   active = 1;
   walltime_c += w - runningwall;
   cputime_c += c - runningcpu;
   runningwall = w;
   runningcpu = c;
   if (activemaster)
     activemaster->ReturnFromChild(w, c);
```

### Comparing `asap3-3.13.1/Basics/TimingResults.h` & `asap3-3.9.6/Basics/TimingResults.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/TinyMatrix.h` & `asap3-3.9.6/Basics/TinyMatrix.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Vec.cpp` & `asap3-3.9.6/Basics/Vec.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/Vec.h` & `asap3-3.9.6/Basics/Vec.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/VelocityVerlet.h` & `asap3-3.9.6/Basics/VelocityVerlet.h`

 * *Files 4% similar despite different names*

```diff
@@ -39,27 +39,26 @@
 class Potential;
 class DynamicAtoms;
 
 class VelocityVerlet : public MolecularDynamics
 {
 public:
   VelocityVerlet(PyObject *py_atoms, Potential *calc, double timestep);
-  virtual ~VelocityVerlet();
+  ~VelocityVerlet();
 
   virtual string GetName() const {return "VelocityVerlet";}
 
 protected:
   // Run the dynamics.  nsteps is the number of steps, observers is a Python
   // list of observers, each observer described by a tuple
   // (function, interval, args, kwargs) and function(*args, **kwargs) is
   // called for each interval time steps.
   //virtual void Run(int nsteps);
   virtual void Run2(int nsteps, PyObject *observers, PyObject *self);
 
 private:
   PyObject *fixatoms_name;
-  PyObject *atomic_masses_name;
 };
 
 } // end namespace
 
 #endif // _VELOCITYVERLET_H
```

### Comparing `asap3-3.13.1/Basics/mass.h` & `asap3-3.9.6/Basics/mass.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/stacktrace.c` & `asap3-3.9.6/Basics/stacktrace.c`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Basics/stacktrace.h` & `asap3-3.9.6/Basics/stacktrace.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Brenner/AtomPairInfoState.h` & `asap3-3.9.6/Brenner/AtomPairInfoState.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Brenner/BrennerPotential.cpp` & `asap3-3.9.6/Brenner/BrennerPotential.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 void BrennerPotential::SetAtoms(PyObject *a, Atoms* accessobj)
 {
   VERB(" SetAtoms");
   if (accessobj != NULL)
     throw AsapError("BrennerPotential::SetAtoms called with accessobj != NULL");
   if (atoms == NULL)
     atoms = new NormalAtoms();
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
 }
 
 double BrennerPotential::GetPotentialEnergy(PyObject *a)
 {
   VERB(" Energy[");
   Calculate(a);
   VERB("]");
@@ -134,15 +134,15 @@
   Calculate(a);
   VERB("]");
   return force;
 }
 
 void BrennerPotential::Calculate(PyObject *a)
 {
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(a);
   z = atoms->GetAtomicNumbers();
   positions = atoms->GetPositions();
   nAtoms = atoms->GetNumberOfAtoms();
   if (counter != atoms->GetPositionsCounter())
     {
       // The atoms have been modified.  Do a calculation.
@@ -161,26 +161,15 @@
       VERB("c");
       Epot = caguts();  // Do the actual calculation.
       counter = atoms->GetPositionsCounter();
     }
   atoms->End();
 }
 
-
-
-bool BrennerPotential::CheckAndUpdateNbList(PyObject *pyatoms)
-{
-  atoms->Begin(pyatoms);
-  bool updated = CheckAndUpdateNeighborList();
-  atoms->End();
-  return updated;
-}
-
-
-bool BrennerPotential::CheckAndUpdateNeighborList()
+void BrennerPotential::CheckAndUpdateNeighborList()
 {
   VERB("n");
   if (nblist == NULL)
     {
       // Make a new neighbor list.
       VERB("N");
 #ifdef SMARTCUTOFF
@@ -199,28 +188,27 @@
 	      rmax_nosq = r;
 	  }
 #endif
       double driftfactor = 0.1;
       PyAsap_NeighborLocatorObject *nbl =
 	PyAsap_NewNeighborList(atoms, rmax_nosq, driftfactor);
       nblist = dynamic_cast<NeighborList *>(nbl->cobj);
-      ASSERT(nblist != NULL);
+      assert(nblist != NULL);
       nblist_obj = (PyObject *) nbl;
       nblist->verbose = verbose;
       nblist->EnableFullNeighborLists();
       nblist->CheckAndUpdateNeighborList();
-      return true;
+      return;
     }
   bool update = (nblist->IsInvalid() || nblist->CheckNeighborList());
   if (update)
     {
       VERB("U");
       nblist->UpdateNeighborList();
     }
-  return update;
 }
 
 void BrennerPotential::CountAtoms()
 {
   VERB("+");
   for (int i = 0; i < 5; i++)
     noa[i] = 0;
```

### Comparing `asap3-3.13.1/Brenner/BrennerPotential.h` & `asap3-3.9.6/Brenner/BrennerPotential.h`

 * *Files 6% similar despite different names*

```diff
@@ -85,32 +85,25 @@
   /// Return the lattice constant of the material, if well-defined.
 
   /// If a lattice constant of the material can be defined, return it
   /// in Angstrom, otherwise throw an exception.
   virtual double GetLatticeConstant() const
   { throw AsapNotImplementedError("BrennerPotential::GetLatticeConstant not implemented.");}
 
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
-  
   /// Can this potential be used in parallel simulations?
   virtual bool Parallelizable() const {return false;}
 
   /// Print memory usage
   virtual long PrintMemory() const {return 0;}  // XXXX
 
 private:
   /// Calculate energies and forces.
   void Calculate(PyObject *a);
 
-  bool CheckAndUpdateNeighborList();
+  void CheckAndUpdateNeighborList();
 
   void CountAtoms();
 
   double caguts();
 
   double pibond();
```

### Comparing `asap3-3.13.1/Brenner/asapbrenner.h` & `asap3-3.9.6/Brenner/asapbrenner.h`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 #ifndef ASAPBRENNER_H
 #define ASAPBRENNER_H
 
 #include <Vec.h>
 #include "BrennerPotential.h"
 //#define ASAPDEBUG
 #include "Debug.h"
-#include <assert.h>
 
 typedef Vec bren_vector;
 typedef double Float;
 typedef double Double;
 
 // NTAB is defined as BRENNERNTAB in BrennerPotential.h to avoid name clashes.
 #define NTAB BRENNERNTAB
```

### Comparing `asap3-3.13.1/Brenner/bcuint.cpp` & `asap3-3.9.6/Brenner/bcuint.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -80,45 +80,63 @@
 		for (J=0; J<16; J++) {
 			CLM[I][L][M][J+1] = (Float) inter2d_in2_data[K-1][J];
 		}
 	}
 	{
 		int littlei;
 		for (littlei = 1; littlei < 3; littlei++)  {
+			if(xindex[0][0]!=1) {
+				int a = 10;
+			}
 			for (L=1; L <= MAX_BC_NEIGHBORS; L++)  {
+				if(xindex[0][0]!=1) {
+					int a = 10;
+				}
 				for (M=1; M <= MAX_BC_NEIGHBORS; M++) {
 					int II;
 					Double copy [16+1];
+					if(xindex[0][0]!=1) {
+						int a = 10;
+					}
 					for (II = 1; II < 17; II++) 
 						copy [II] = 0.0;
 					for (II = 1; II < 17; II++) {
 						/* i and j are the exponents of XX1, XX2 for the
 						term at position II in array CLM[L][M]. */
 						int i, j;
 						/* ti [z] is the coefficient of F1**z in the expansion of
 						(L+F1)**i. Analogously for tj. */
 						int ti[4], tj[4];
 						/* ie will be the term of the expansion of (L+F1)**i that we'll
 						be looking at.  Analogously je. */
-						int ie, je;
+						int ie, je, ke;
 						i = IN2[II][1];
 						j = IN2[II][2];
 						expand (L, ti, i);
 						expand (M, tj, j);
+						if(xindex[0][0]!=1) {
+		 					int a = 10;
+						}
 						for (ie = 0; ie < 4; ie++)
 							for (je = 0; je < 4; je++) {
 								copy [xindex [ie][je]] +=
 									CLM[littlei][L][M][II]*ti[ie]*tj[je];
 							}
 					}
+					if(xindex[0][0]!=1) {
+						int a = 10;
+			        }
                                         //DDL:
 					//BUG? Why count to 65? although copy is only 17 bytes 
 					//     AND data out of CLMS is accessed!!!
 					for (II = 1; II < 17; II++) {
 						CLMS [littlei][L][M][II] = copy [II];
+						if(xindex[0][0]!=1) {
+							int a = 10;
+						}
 					}
 				}
 			}
 		}
 	}
 }
 
@@ -129,16 +147,16 @@
 	/*bicubic spline*/
 
 	if (XX1 < 1) XX1 = 1;
 	if (XX2 < 1) XX2 = 1;
 	NH=(int)floor(XX1);
 	NC=(int)floor(XX2);
 
-	ASSERT (0 != NH);
-	ASSERT (0 != NC);
+	assert (0 != NH);
+	assert (0 != NC);
 	if(NH > MAX_BC_NEIGHBORS || NC > MAX_BC_NEIGHBORS)
 	{
 	  throw AsapError("BrennerPotential: A ")
 	    << (KJ >= 1 && KJ <= 4 ? ktype_name[KJ] : "invalid type")
 	    << " atom has too many neighbors for the bicubic spline. It has "
 	    << NH << " Hydrogen and " << NC
 	    << " Carbon neighbors; the maximum is "
```

### Comparing `asap3-3.13.1/Brenner/caguts.cpp` & `asap3-3.9.6/Brenner/caguts.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 Float BrennerPotential::caguts()
 {
   // The number of atoms
   const int num_atms = nAtoms;
   /* k is the position of the current neighbor in apis. */
   int k = 0;
+  int l;
   // Allocate buffers for neighbor list data
   int nmaxnb = nblist->MaxNeighborListLength();
   vector<int> iNeighbors(nmaxnb);
   vector<Vec> distances(nmaxnb);
   vector<double> sq_distances(nmaxnb);
   
   /* tote is the total energy, for the return value of caguts. */
@@ -183,15 +184,15 @@
         /* Now rp is the magnitude of the force from pairwise repulsion. */
         tote = tote + vv;
         
         /* rpp is the repulsive force between the pair. */
         thisPair->rpp = rp*thisPair->cor;
       } /* End loop over neighors. */
     } /* End loop over atoms. */
-    ASSERT (num_atms == i);
+    assert (num_atms == i);
     apis->ai_start [i] = k;
   } /* Forget i. */
   
   { /* FIXME Is there any reason not to merge this loop with the previous one?
      */
     int i;
     for (i = 0; i < num_atms; i++) {
@@ -200,15 +201,15 @@
       const int iNeighborCount =
 	nblist->GetFullNeighbors(i, &iNeighbors[0], &distances[0],
 				 &sq_distances[0], sizemax);
       /* Early escape if there is no neighbours to this atoms. This also avoids a memory access error */
       if (iNeighborCount == 0) continue;				 
       const struct AtomPairInfo *const apiNeighbors = pairs (i, apis);
       int jn;
-      ASSERT (iNeighborCount == numPairs(i, apis));
+      assert (iNeighborCount == numPairs(i, apis));
       for (jn = 0; jn < iNeighborCount; jn++) {
         const int j = iNeighbors [jn];
         if(apiNeighbors[jn].lcheck == 0) continue;
         if(i >= j) continue;
         //transForcex (i, j, info, apiNeighbors[jn].rpp.x);
         //transForcey (i, j, info, apiNeighbors[jn].rpp.y);
         //transForcez (i, j, info, apiNeighbors[jn].rpp.z);
```

### Comparing `asap3-3.13.1/Brenner/expand.cpp` & `asap3-3.9.6/Brenner/expand.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -26,12 +26,12 @@
   case 3:
     ti [0] = L * L * L;
     ti [1] = 3 * L * L;
     ti [2] = 3 * L;
     ti [3] = 1;
     break;
   default:
-    ASSERT (0 && "i should be between 0 and 3 inclusive");
+    assert (0 && "i should be between 0 and 3 inclusive");
   }
 }
 
 } // end namespace
```

### Comparing `asap3-3.13.1/Brenner/inter2d_iv.cpp` & `asap3-3.9.6/Brenner/inter2d_iv.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Brenner/mtable.cpp` & `asap3-3.9.6/Brenner/mtable.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Brenner/pibond.cpp` & `asap3-3.9.6/Brenner/pibond.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
              spline. */ 
           Float *exnij,
           /* dexni is a pointer to two Float's.  One is the partial of exnij
              with respect to N super C sub i, and the other is the partial of
              exnij with respect to N super H sub i. */
           Float *dexni)
 {
-  int k;
+  int k, jj;
   Float qi;
   /* nk will be the number of the neighbor by the time we're done. */
   int nk = 0; /* nl */
   //  XXX The following neighbor list access should be optimized away
   // Allocate buffers for neighbor list data
   int nmaxnb = nblist->MaxNeighborListLength();
   vector<int> iNeighbors(nmaxnb);
@@ -204,25 +204,25 @@
   /* stop_index is one past the index of the last neighbor. */
   int sizemax = nmaxnb;
   const int stop_index =
     nblist->GetFullNeighbors(index1, &iNeighbors[0], &distances[0],
 			     &sq_distances[0], sizemax);
   Float gangle, dgdthet;
   Float gangle1, dgdthet1;
-  ASSERT (getKtype (index1) == k_this);
-  ASSERT (sij == atom_pairj[j].rcor);
+  assert (getKtype (index1) == k_this);
+  assert (sij == atom_pairj[j].rcor);
   /* Apparently we don't get exact equality when we should on the next line. */
-  ASSERT (fabs (rsqij - sij * sij) < 0.00001);
+  assert (fabs (rsqij - sij * sij) < 0.00001);
   *xsij = 0.0; /* xsji */
   *ssumk = 0.0; /* ssuml */
   *conk = 0.0; /* conl */
   xni[0] = xhc[0][index1]; /* xnj */
   xni[1] = xhc[1][index1];
-  /* The next ASSERT says that other is either a hydrogen or carbon. */
-  ASSERT(kother-1 < 2);
+  /* The next assert says that other is either a hydrogen or carbon. */
+  assert(kother-1 < 2);
   xni[kother-1] -= atom_pairj[j].ww;
   /* qi is N super t sub i, in equation 11 on page 13, . */
   qi = xni[0] + xni[1] - 2.0; /* qj */
   *sdalik = 0.0; /* SDALJL */
   for(k = 0; k < stop_index; ++k) /* for(l) */
   {
     /* k is the index of a bond between formula-i and formula-k.  c_sign
@@ -256,15 +256,15 @@
     else if(costh < -1.0) costh = -1.0;
     cosk[nk] = costh;
     sink[nk] = sqrt(1.0-costh*costh); /* sinl */
     /* According to the online docs, acos never returns a value greater
      than pi.  What was the intent here?
      Sent email to Brenner 29 Jul 2000.  Tim Freeman.
      if(acos(costh) > M_PI) sink[nk] = -sink[nk]; */
-    ASSERT (acos(costh) <= M_PI);
+    assert (acos(costh) <= M_PI);
     if(k_this == 1) {
       /* Atom number index is a carbon. */
       int ig = igc[(int)floor(-costh*12.0)+13];
       /* gangle is G(cos(theta sub j i k)), mentioned in equation 7 on page
          10.  I hope the compiler discovers the shared subexpressions. */
       gangle = SPGC[ig][1] + SPGC[ig][2]*costh + SPGC[ig][3]*costh*costh
         + SPGC[ig][4]*costh*costh*costh
@@ -482,14 +482,17 @@
   int sizemax = nmaxnb;
   const int stop_index =
     nblist->GetFullNeighbors(i, &iNeighbors[0], &distances[0],
 			     &sq_distances[0], sizemax);
 
   const int *neighbor_start = &iNeighbors[0];
   const struct AtomPairInfo *iatom_pair = pairsconst (i, apis);
+  Float dbtori = 0.0;
+  Float dbtorj = 0.0;
+  Float dbtorc = 0.0;
   Float btor = 0.0;
   Float datori,datorj ,datorc;
   Float ator = TOR(xnt1,xnt2,conjug,&datori,&datorj,&datorc);  // XXX
   Float vatt_ator = vatt*ator;
 
   if(fabs(ator) <= 1.0e-08) {
      return;
@@ -549,15 +552,15 @@
       nblist->GetFullNeighbors(jn, &jneighbor_start[0], &distances[0],
 			       &sq_distances[0], sizemax);
     jatom_pair = pairsconst (jn, apis);
     nl = 0;
     for(l = 0; l < stop_index2; ++l) {
       int ln = jneighbor_start[l];
       Float sinl2, rcl, t1, t2, cw, bt, fcl, dfcl;
-      Float aa, aaa1, at2, rp1, rp2, rp3, rp4, rp5;
+      Float aa, aaa1, at2, rp1, rp2, rp3, rp4, rp5, rep;
       Float dt1dik, dt1djk, dt1djl, dt1dil, dt1dij;
       Float crlx, crly, crlz;
       bren_vector dt2dik, dt2dij;
       if(ln == i || jatom_pair[l].lcheck != 1) continue;
       ++nl;
       if(fabs(sinl[nl]) < 1.0e-01) continue;
       sinl2 = sinl[nl]*sinl[nl];
@@ -656,14 +659,15 @@
                Float vdrdi, Float vdrdc, Float *cfuni, Float sdalik,
                Float *xsjk, bren_vector *xk, Float *dcfuni, Float conk)
 {
   /* The code that increments nk here has to match up with the code that
    increments nk in calc1side, since we use nk to index into cfuni which is
    computed in calc1side. */
   int nk = 0;
+  int n; /* nl */
   int k; /* l */
   int m;
   Float dwr;
   //  XXX The following neighbor list access should be optimized away
   int nmaxnb = nblist->MaxNeighborListLength();
   vector<int> kNeighbors(nmaxnb);
   vector<Vec> distances(nmaxnb);
@@ -671,15 +675,15 @@
   /* stop_index is one past the index of the last neighbor. */
   int sizemax = nmaxnb;
   const int stop_index =
     nblist->GetFullNeighbors(index1, &kNeighbors[0], &distances[0],
 			     &sq_distances[0], sizemax);
   const struct AtomPairInfo *const kPairs = pairsconst (index1, apis);
   for(k = 0; k < stop_index; ++k) {
-    Float rp, rp1, rp2, ddr;
+    Float rp, rp1, rp2, rep, ddr;
     int kn = kNeighbors [k];
     int kk = getKtype (kn);
     if(i_side && k == indexj) continue;
     if(!i_side && kn == index2) continue;
     if(kPairs[k].lcheck != 1) continue;
     dwr = kPairs[k].dww/kPairs[k].rcor;
     ++nk; /*nk only increases when we get past the continue's above. */
@@ -782,15 +786,15 @@
        hydrogens_connected to 1.  Weird. Tim Freeman 6 Sep 2000. */
     hydrogens_connected[i] = 1;
     carbons_connected[i] = 1;
     for (jn = 0; jn < nCount; jn++) {
       if(1 == pairs[jn].lcheck) {
         const int j = iNeighbors [jn];
         const int atype = getKtype(j);
-        ASSERT(atype > 0 && atype <= 2);
+        assert(atype > 0 && atype <= 2);
         xhc[atype-1][i] += pairs[jn].ww;
       }
     }
   }
   /*
    * Sum over bonds between atoms I and J
    */
```

### Comparing `asap3-3.13.1/Brenner/radic.cpp` & `asap3-3.9.6/Brenner/radic.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,17 @@
       }
 }
 
 void BrennerPotential::init_in3()
 {
   DEBUGPRINT;
   int IC=0;
+  int I3D,ITD;
   int i,j, I, J, K, L, M, N;
+  FILE *inter3Dtors;
   for (I=1; I<5; I++) {
     for (J=1; J<5; J++) {
       for (K=1; K<5; K++) {
         IC=IC+1;
         /* It's weird that IN3 and dIN3 are the same as each other. */
         IN3[IC][1]=I-1;
         IN3[IC][2]=J-1;
```

### Comparing `asap3-3.13.1/Brenner/radicdata.cpp` & `asap3-3.9.6/Brenner/radicdata.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Brenner/sili_germ.cpp` & `asap3-3.9.6/Brenner/sili_germ.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   /*
    *     silicon: e = 4.6297255 eV/atom
    *              rnn = 2.3521697 A
    */
   bren_vector xt[250+1];
   Float xslj[250+1],xsij[250+1];
   Float s3, ss, rr, rsq2, rsq3, costh, aarg, aarg2, dgdthet;
-  Float rp, vv, vatt, dbdz, gangle;
+  Float rep, rp, vv, vatt, dbdz, gangle;
   Float dctdij, dctdli, dctdlj, dli, bli;
   Float tote = 0;
   int l;
   if(!si_ge_initialized)
     si_ge_init();   // Should never happen - remove?  JS.
   for(l = 0; l < num_atms; ++l) {
     const struct AtomPairInfo *const lpairs = pairsconst (l, apis);
@@ -84,15 +84,15 @@
 			       &sq_distances[0], sizemax);
 
     const int kl = getKtype(l);
     /* i is the index of a neighbor of l. */
     int i;
     for(i = 0; i < stop_index; ++i) {
       Float xsli, ssum;
-      int in, UNUSED(ki);
+      int in, ki;
       if (lpairs[i].lcheck != 2) continue;
       in = lNeighbors[i];
       /*  THIS IS THE IL TERM */
       /* There used to be a bug here -- we used i, which was an index into the
          neighbors list, as an index into the atom list to get the ktype of
          something.  They must have meant the ktype of the atom we're talking
          about, which has the index in in the atom list.  Tim Freeman 13 Sep
```

### Comparing `asap3-3.13.1/Brenner/spgch.cpp` & `asap3-3.9.6/Brenner/spgch.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/COPYING` & `asap3-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/COPYING.LESSER` & `asap3-3.9.6/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/AsapModule.cpp` & `asap3-3.9.6/Interface/AsapModule.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -41,20 +41,16 @@
 #ifdef WITH_OPENKIM
 #include "OpenKIMinterface.h"
 #endif
 #define ALLOCATE_TIMING
 #include "Timing.h"
 #include "TimingResults.h"
 #include "stacktrace.h"
-//#define ASAPDEBUG
 #include "Debug.h"
 #include "AsapModule.h"
-#ifdef ASAP_MKL
-#include <mkl.h>
-#endif // ASAP_MKL
 
 PyDoc_STRVAR(asapmodule__doc__, "C++ extension for Asap.\n");
 
 namespace ASAPSPACE {
 
 #ifdef _OPENMP
 AsapErrorBase *AsapGlobalException;
@@ -127,16 +123,20 @@
      PyAsap_support_openmp_doc},
     {"get_num_procs", PyAsap_get_num_procs, METH_NOARGS,
      PyAsap_get_num_procs_doc},
     {"set_num_threads", (PyCFunction)PyAsap_set_num_threads, METH_VARARGS|METH_KEYWORDS,
      PyAsap_set_num_threads_doc},
     {"heap_mallinfo", (PyCFunction)PyAsap_HeapMallinfo, METH_NOARGS,
      "Return heap size in kB."},
+#ifdef WITH_OPENKIM
+    {"OpenKIMinfo", (PyCFunction)PyAsap_NewOpenKIMinfo, METH_VARARGS|METH_KEYWORDS,
+     OpenKIMinfo_Docstring},
+#endif // WITH_OPENKIM
 #ifdef PARALLEL
-    {"DistributeAtoms", (PyCFunction)PyAsap_DistributeAtoms, METH_VARARGS|METH_KEYWORDS,
+    {"DistributeAtoms", PyAsap_DistributeAtoms, METH_O,
      "Distribute atoms in a parallel simulation."},
 #endif
     {NULL, NULL, 0, NULL}
   };
 
 
 #ifdef STACKTRACE
@@ -153,14 +153,15 @@
 }
 #endif // PARALLEL
 #endif // STACKTRACE
 
 } // end namespace
 
 // Module definition for Python 3
+#ifdef ASAP_PY3
 static int asap_traverse(PyObject *m, visitproc visit, void *arg)
 {
   //struct asap_module_state *state = GETMODULESTATE(m);  
   //Py_VISIT(xxxx);
   return 0;
 }
 
@@ -169,38 +170,54 @@
   //struct asap_module_state *state = GETMODULESTATE(m);  
   //Py_CLEAR(state->Asap_String_Stress);
   return 0;
 }
 
 static struct PyModuleDef asapmoduledef = {
   PyModuleDef_HEAD_INIT,
+#ifdef PARALLEL
   "_asap",
+#else
+  "_asap_p3",
+#endif
   asapmodule__doc__,
 #ifdef _OPENMP
   -1,      // Module uses global data - only one interpreter is possible.
 #else // _OPENMP
   0,       // Module does not have any module-global data i C++.
 #endif // _OPENMP
   AsapContents,
   NULL,
   asap_traverse,
   asap_clear,
   NULL
 };
 
+#endif // ASAP_PY3
 
 PyObject *AsapInitModule(void)
 {
   DEBUGPRINT;
 
   // Initialize the NumPy package.  Return NULL on failure.
   import_array1(NULL);
   DEBUGPRINT;
 
+#ifdef ASAP_PY3
   PyObject *m = PyModule_Create(&asapmoduledef);
+#else // ASAP_PY3
+  PyObject *m = Py_InitModule3(
+#ifdef PARALLEL
+			       "_asap",
+#else // PARALLEL
+			       "_asap_p2",
+#endif // PARALLEL
+			       AsapContents,
+			       asapmodule__doc__);
+#endif // ASAP_PY3
   if (m == NULL)
     return NULL;
 
   DEBUGPRINT;
 #ifdef _OPENMP
   AsapGlobalException = NULL;
 #endif
@@ -243,21 +260,11 @@
   Asap_setSignalHandlers(-1, 0);
 #endif //PARALLEL
 #endif //STACKTRACE
 
   // Create the verbose variable
   PyModule_AddIntConstant(m, "verbose", 0);
 
-#ifdef ASAP_MKL
-  assert(BUFLEN % (ASAP_MKL_ALIGN/sizeof(double)) == 0);  // Otherwise we break alignment
-  // Set the precision of MKL to low accuracy
-  // meaning that the last two bits of the mantissa may be
-  // incorrect, and that denormalized numbers are zero.
-  // The first cannot possibly influence a simulations,
-  // and denormalized numbers should never occur.
-  vmlSetMode(VML_LA | VML_FTZDAZ_ON | VML_ERRMODE_DEFAULT);
-#endif //ASAP_MKL
-  
   DEBUGPRINT;
   return m;
 }
```

### Comparing `asap3-3.13.1/Interface/AsapModule.h` & `asap3-3.9.6/Interface/AsapModule.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/AsapSerial.cpp` & `asap3-3.9.6/Interface/PTMInterface.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-// Copyright (C) 2008-2011 Jakob Schiotz and Center for Individual
-// Nanoparticle Functionality, Department of Physics, Technical
+// -*- C++ -*-
+// PTMInterface.h: Python interface to the Polyhedral Template Matching function.
+//
+// Copyright (C) 2016 Jakob Schiotz and Center for Atomic-scale
+// Materials Design, Department of Physics, Technical
 // University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
 //
 // This program is free software: you can redistribute it and/or
 // modify it under the terms of the GNU Lesser General Public License
 // version 3 as published by the Free Software Foundation.  Permission
@@ -17,16 +20,22 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-#undef PARALLEL
-#include "AsapModule.cpp"
+#ifndef _PTM_INTERFACE_H
+#define _PTM_INTERFACE_H
+
+#include "AsapPython.h"
+#include "Asap.h"
+
+namespace ASAPSPACE {
+
+void PyAsap_InitPTMmodule();
 
+PyObject* PyAsap_PTMall(PyObject* noself, PyObject* args, PyObject* kwargs);
 
-PyMODINIT_FUNC PyInit__asap(void)
-{
-    return AsapInitModule();
-}
+} // end namespace
 
+#endif // _PTM_INTERFACE_H
```

### Comparing `asap3-3.13.1/Interface/DynamicsInterface.cpp` & `asap3-3.9.6/Interface/DynamicsInterface.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,20 @@
 
 #define CHECK_DYN_INIT if (self->cobj == NULL) {	  \
     PyErr_SetString(PyAsap_ErrorObject,			  \
 		    "Dynamics object not initialized."); \
     return NULL;					  \
   }
 
+// Allow easy test for String in Python 2 and Unicode in Python 3
+#ifdef ASAP_PY3
+#define ASAP_PYSTRING PyUnicode_Type
+#else
+#define ASAP_PYSTRING PyString_Type
+#endif
   
 static int PyAsap_VelocityVerletInit(PyAsap_DynamicsObject *self, 
     PyObject *args, PyObject *kwargs)
 {
     static char *kwlist[] = {"atoms", "calc", "timestep", NULL};
   
     PyObject *atoms;
@@ -100,15 +106,14 @@
         return -1;
     }
     if (self->cobj == NULL)
         return -1;
     return 0;
 }
 
-
 static int PyAsap_LangevinInit(PyAsap_DynamicsObject *self,
     PyObject *args, PyObject *kwargs)
 {
   static char *kwlist[] = {"atoms", "calc", "timestep", "sdpos", "sdmom", "c1", "c2", "fixcm", "seed", NULL};
 
   PyObject *atoms;
   PyObject *calc;
@@ -116,16 +121,16 @@
   PyObject *sdpos;
   PyObject *sdmom;
   PyObject *c1;
   PyObject *c2;
   int fixcm;
   unsigned int seed;
   if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "OOdO!O!O!O!iI:Langevin", kwlist,
-          &atoms, &calc, &timestep, &PyUnicode_Type, &sdpos, &PyUnicode_Type, &sdmom,
-	  &PyUnicode_Type, &c1, &PyUnicode_Type, &c2, &fixcm, &seed))
+          &atoms, &calc, &timestep, &PyAsapString_Type, &sdpos, &PyAsapString_Type, &sdmom,
+	  &PyAsapString_Type, &c1, &PyAsapString_Type, &c2, &fixcm, &seed))
       return -1;
   CHECK_DYN_UNINIT;
   Potential *asap_calc = NULL;
   if (PyAsap_PotentialCheck(calc))
   {
       // We can use the potential directly.
       asap_calc = ((PyAsap_PotentialObject *)calc)->cobj;
@@ -209,16 +214,16 @@
     static char *kwlist[] = {"act0", "c3", "c4", "pmcor", "cnst", NULL};
     PyObject *act0;
     PyObject *c3;
     PyObject *c4;
     PyObject *pmcor;
     PyObject *cnst;
     if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O!O!O!O!O!:set_vector_constants", kwlist,
-        &PyUnicode_Type, &act0, &PyUnicode_Type, &c3, &PyUnicode_Type, &c4,
-        &PyUnicode_Type, &pmcor, &PyUnicode_Type, &cnst))
+        &PyAsapString_Type, &act0, &PyAsapString_Type, &c3, &PyAsapString_Type, &c4,
+        &PyAsapString_Type, &pmcor, &PyAsapString_Type, &cnst))
         return NULL;
     CHECK_DYN_INIT;
     Langevin *cobj = dynamic_cast<Langevin *>(self->cobj);
     if (cobj == NULL)
       {
         PyErr_SetString(PyExc_TypeError, "Apparently not a Langevin object.");
         return NULL;
@@ -280,20 +285,19 @@
         METH_VARARGS|METH_KEYWORDS, "Get two sets of random numbers"},
     {NULL}  // Sentinel
 };
 
 static void InitDynamicsType(PyTypeObject &type)
 {
   type.tp_new = PyType_GenericNew;
-  type.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HAVE_FINALIZE;
+  type.tp_dealloc = PyAsap_Dealloc<PyAsap_DynamicsObject>;
+  type.tp_flags = Py_TPFLAGS_DEFAULT;
   type.tp_repr = PyAsap_Representation<PyAsap_DynamicsObject>;
-  type.tp_finalize = PyAsap_Finalize<PyAsap_DynamicsObject>;
-  type.tp_dealloc = PyAsap_Dealloc;
 }
-
+			 
 int PyAsap_InitDynamicsInterface(PyObject *module)
 {
     // Init the Velocity Verlet dynamics
     InitDynamicsType(PyAsap_VelocityVerletType);
     PyAsap_VelocityVerletType.tp_init = (initproc) PyAsap_VelocityVerletInit;
     PyAsap_VelocityVerletType.tp_doc = VelocityVerlet_Docstring;
     PyAsap_VelocityVerletType.tp_methods = PyAsap_VelocityVerletMethods;
```

### Comparing `asap3-3.13.1/Interface/DynamicsInterface.h` & `asap3-3.9.6/Interface/DynamicsInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/EMTParameterProviderInterface.cpp` & `asap3-3.9.6/Interface/EMTParameterProviderInterface.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 // but the cobj pointer may point to C++ objects of different type,
 // depending on how the PyAsap_EMTParamProvObject was created.
 // Different factory functions provide PyAsap_EMTParamProvObject
 // objects with different contents.  Objects created the standard way
 // use a EMTPythonParameterProvider (XXX NOT IMPLEMENTED YET) which
 // should be subclassed in Python.
 
-// The PyAsap_EMTParamProvObject is defined in Potentials/EMTParameterProvider.h
+// The PyAsap_EMTParamProvObject is defined in Basics/EMTParameterProvider.h
 
 namespace ASAPSPACE {
 
 PyTypeObject PyAsap_EMTParamProvType = {
   PyVarObject_HEAD_INIT(NULL, 0)
   "_asap.EMTParameterProvider",
   sizeof(PyAsap_EMTParamProvObject),
@@ -162,23 +162,23 @@
    METH_NOARGS, "The maximal value of the neighbor list cutoff that may later be set."},
    {NULL}  // Sentinel
 };
 
 
 int PyAsap_InitEMTParameterProviderInterface(PyObject *module)
 {
-  PyAsap_EMTParamProvType.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HAVE_FINALIZE;
+  PyAsap_EMTParamProvType.tp_dealloc =
+    PyAsap_Dealloc<PyAsap_EMTParamProvObject>;
+  PyAsap_EMTParamProvType.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE;
   PyAsap_EMTParamProvType.tp_repr =
     PyAsap_Representation<PyAsap_EMTParamProvObject>;
   PyAsap_EMTParamProvType.tp_new = PyAsap_NewParameterProvider; 
   PyAsap_EMTParamProvType.tp_init = PyAsap_InitParameterProvider; 
   PyAsap_EMTParamProvType.tp_doc = EMTParamProv_Docstring;
   PyAsap_EMTParamProvType.tp_methods = PyAsap_ParamProvMethods;
-  PyAsap_EMTParamProvType.tp_finalize = PyAsap_Finalize<PyAsap_EMTParamProvObject>;
-  PyAsap_EMTParamProvType.tp_dealloc = PyAsap_Dealloc;
 
   if (PyType_Ready(&PyAsap_EMTParamProvType) < 0)
     return -1;
   PyModule_AddObject(module, "EMTParameters",
 		     (PyObject *) &PyAsap_EMTParamProvType);
   return 0;
 }
```

### Comparing `asap3-3.13.1/Interface/EMTParameterProviderInterface.h` & `asap3-3.9.6/Interface/EMTParameterProviderInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/ExceptionInterface.cpp` & `asap3-3.9.6/Interface/ExceptionInterface.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/ExceptionInterface.h` & `asap3-3.9.6/Interface/ExceptionInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/NeighborLocatorInterface.cpp` & `asap3-3.9.6/Interface/NeighborLocatorInterface.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -50,15 +50,16 @@
   sizeof(PyAsap_NeighborLocatorObject),
   // The rest are initialized by name for reliability.
 };
 
 static char NeighborLocator_Docstring[] = "NeighborLocator object.\n";
 
 PyAsap_NeighborLocatorObject *PyAsap_NewNeighborList(Atoms *atoms, double rCut,
-                                                     double driftfactor)
+                                                     double driftfactor,
+                                                     bool master /* =true */)
 {
   PyAsap_NeighborLocatorObject *self;
 
   self = PyObject_NEW(PyAsap_NeighborLocatorObject,
                       &PyAsap_NeighborLocatorType);
   if (self == NULL)
     throw AsapError("OOPS XXXX");
@@ -68,14 +69,19 @@
   self->cobj = new NeighborList(atoms, rCut, driftfactor);
   if (self->cobj == NULL)
     {
       CHECKREF(self);
       Py_DECREF(self);
       throw AsapError("Failed to create a new NeighborList object.");
     }
+  if (master)
+    {
+      // Set this neighbor list as the master list in parallel simulations.
+      atoms->SetPrimaryNbLocator((PyObject *) self);
+    }
   return self;
 }
 
 PyAsap_NeighborLocatorObject *PyAsap_NewNeighborList2013(Atoms *atoms, double rCut,
                                                        double driftfactor,
                                                        const TinyMatrix<double> &rcut2)
 {
@@ -171,18 +177,19 @@
       PyErr_SetString(PyExc_ValueError,
 		      "NeighborList: Cutoff must be greater than zero.");
       return NULL;
     }
   
   try {
     PyAsap_NeighborLocatorObject *self = PyAsap_NewNeighborList(NULL, rCut,
-								driftfactor);
+								driftfactor,
+								false);
     if (full) {
       NeighborList *nblist = dynamic_cast<NeighborList *>(self->cobj);
-      ASSERT(nblist != NULL);
+      assert(nblist != NULL);
       nblist->EnableFullNeighborLists();
       self->fulllist = true;
     }
     
     if (atoms != Py_None)
       self->cobj->CheckAndUpdateNeighborList(atoms);
     return (PyObject *) self;
@@ -365,107 +372,14 @@
   try {
     n = nblist->TestPartialUpdate(modif, atoms);
   }
   CATCHEXCEPTION;
   return Py_BuildValue("i", n);
 }
 
-static char PyAsap_NBL_GetNBQuery_Docstring[] =
-"Get information about the neighborhood around a query point.\n\n\
-Returns a 3-tuple for each query point: The indices of the neighbors,\n\
-the vectors pointing towards the neighbors and the squared distances\n\
-to the neighbors.\n\
-Periodic boundary conditions are taken into account.\n\n\
-Parameters:\n\
-    query_points: Nx3 array of query point positions.\n\
-    rcut (optional): The cutoff distance. If specified, must be smaller\n\
-      or equal to the value specified when creating the neighbor list.\n\
-";
-static PyObject *PyAsap_NBL_GetNBQuery(PyAsap_NeighborLocatorObject *self,
-				  PyObject *args, PyObject *kwargs)
-{
-  PyObject *py_arg_query_positions;
-  PyArrayObject *py_arr_query_positions;
-  PyObject *py_tup_return = NULL;
-  double rcut = -1.0;
-  static char *kwlist[] = {"query_points", "rCut", NULL};
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|d:get_neighbors",
-				   kwlist, &py_arg_query_positions, &rcut))
-    return NULL;
-  // Check sensibility
-  py_arr_query_positions = AsPyArray(py_arg_query_positions);
-  if (PyArray_NDIM(py_arr_query_positions) != 2)
-  {
-    PyErr_SetString(PyExc_ValueError, "NeighborLocator: Expected query points to be Nx3 numpy array.");
-    return NULL;
-  }
-  if (PyArray_SHAPE(py_arr_query_positions)[1] != 3)
-  {
-    PyErr_SetString(PyExc_ValueError, "NeighborLocator: Expected query points to be Nx3 numpy array.");
-    return NULL;
-  }
-  if (PyArray_SHAPE(py_arr_query_positions)[0] < 1)
-  {
-    PyErr_SetString(PyExc_ValueError, "NeighborLocator: Expected query points to be Nx3 numpy array.");
-    return NULL;
-  }
-  if (rcut > self->cobj->GetCutoffRadius())
-  {
-    PyErr_SetString(PyExc_ValueError, "NeighborLocator: too large cutoff.");
-    return NULL;
-  }
-  int num_query_points = PyArray_SHAPE(py_arr_query_positions)[0];
-  py_tup_return = PyTuple_New(num_query_points);
-  if (py_tup_return == NULL)
-  {
-    Py_XDECREF(py_tup_return);
-    return NULL;
-  }
-
-  int size = self->cobj->MaxNeighborListLength();
-  vector<int> neighbors(size);
-  vector<Vec> diff(size);
-  vector<double> diff2(size);
-  for (int i=0; i<num_query_points; i++)
-  {
-    int nnb;
-    int nb_size = size;
-    Vec pos;
-    neighbors.resize(size);
-    diff.resize(size);
-    diff2.resize(size);
-    pos[0] = *((npy_double *) PyArray_GETPTR2(py_arr_query_positions, i, 0));
-    pos[1] = *((npy_double *) PyArray_GETPTR2(py_arr_query_positions, i, 1));
-    pos[2] = *((npy_double *) PyArray_GETPTR2(py_arr_query_positions, i, 2));
-    nnb = self->cobj->GetFullNeighborsQuery(pos, &neighbors[0], &diff[0],
-                                         &diff2[0], nb_size, rcut);
-    neighbors.resize(nnb);
-    diff.resize(nnb);
-    diff2.resize(nnb);
-    PyObject *py_neighbors = PyAsap_ArrayFromVectorInt(neighbors);
-    PyObject *py_diff = PyAsap_ArrayFromVectorVec(diff);
-    PyObject *py_diff2 = PyAsap_ArrayFromVectorDouble(diff2);
-    if (py_neighbors == NULL || py_diff == NULL || py_diff2 == NULL)
-      {
-        // Conversion failed, strange!  Clean up and abort.
-        Py_XDECREF(py_neighbors);
-        Py_XDECREF(py_diff);
-        Py_XDECREF(py_diff2);
-        return NULL;
-      }
-    PyObject *py_res_one_query_point = Py_BuildValue("NNN", py_neighbors, py_diff, py_diff2);
-    if (py_res_one_query_point == NULL)
-    {
-      return NULL;
-    }
-    PyTuple_SET_ITEM(py_tup_return, i, py_res_one_query_point);
-  }
-  return py_tup_return;
-}
-
 static char PyAsap_NBL_GetNB_Docstring[] =
 "Get information about the neighbors of an atom.\n\n\
 Returns three arrays: The indices of the neighbors, the squared distances\n\
 to the neighbors, and the vectors pointing towards the neighbors.\n\
 Periodic boundary conditions are taken into account.\n\n\
 Parameters:\n\
   i: The atom queried.\n\
@@ -528,16 +442,14 @@
    METH_O, "Check the neighbor list, update if needed."},
   {"test_partial_update", (PyCFunction) PyAsap_NeighborLocatorPartialTest,
    METH_VARARGS, "Test partial update of neighbor list.  FOR DEBUGGING ONLY!"},
   {"get_wrapped_positions", (PyCFunction) PyAsap_NBL_GetWrapped,
    METH_NOARGS, "Get wrapped positions."},
   {"get_neighbors", (PyCFunction) PyAsap_NBL_GetNB,
    METH_VARARGS|METH_KEYWORDS, PyAsap_NBL_GetNB_Docstring},
-  {"get_neighbors_querypoint", (PyCFunction) PyAsap_NBL_GetNBQuery,
-   METH_VARARGS|METH_KEYWORDS, PyAsap_NBL_GetNBQuery_Docstring},
 #ifdef GETSCALED
   {"get_scaled_positions", (PyCFunction) PyAsap_NBL_GetScaled,
    METH_NOARGS, "Get neighborlist's idea of scaled positions."},
 #endif // GETSCALED
   {"print_info", (PyCFunction) PyAsap_NBL_PrintInfo,
    METH_VARARGS, "print debugging info about an atom."},
   {"print_memory", (PyCFunction)PyAsap_NblPrintMemory,
@@ -555,24 +467,24 @@
 	0,	                                       /* sq_inplace_concat */
 	0,	                                       /* sq_inplace_repeat */
 };
 
 int PyAsap_InitNeighborLocatorInterface(PyObject *module)
 {
   PyAsap_NeighborLocatorType.tp_new = NULL;  // Use factory functions
-  PyAsap_NeighborLocatorType.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_FINALIZE;
+  PyAsap_NeighborLocatorType.tp_dealloc =
+    PyAsap_Dealloc<PyAsap_NeighborLocatorObject>;
+  PyAsap_NeighborLocatorType.tp_flags = Py_TPFLAGS_DEFAULT;
   PyAsap_NeighborLocatorType.tp_methods = PyAsap_NeighborLocatorMethods;
   PyAsap_NeighborLocatorType.tp_as_sequence = &PyAsap_NeighborLocator_sequence;
   PyAsap_NeighborLocatorType.tp_repr =
     PyAsap_Representation<PyAsap_NeighborLocatorObject>;
   PyAsap_NeighborLocatorType.tp_doc = NeighborLocator_Docstring;
   PyAsap_NeighborLocatorType.tp_weaklistoffset = offsetof(PyAsap_NeighborLocatorObject,
       weakrefs);
-  PyAsap_NeighborLocatorType.tp_finalize = PyAsap_Finalize<PyAsap_NeighborLocatorObject>;
-  PyAsap_NeighborLocatorType.tp_dealloc = PyAsap_Dealloc;
   if (PyType_Ready(&PyAsap_NeighborLocatorType) < 0)
     return -1;
   return 0;
 }
 
 
 bool PyAsap_NeighborLocatorCheck(PyObject *obj)
```

### Comparing `asap3-3.13.1/Interface/NeighborLocatorInterface.h` & `asap3-3.9.6/Interface/NeighborLocatorInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/OpenMPInterface.cpp` & `asap3-3.9.6/Interface/OpenMPInterface.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/OpenMPInterface.h` & `asap3-3.9.6/Interface/OpenMPInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/PTMInterface.cpp` & `asap3-3.9.6/Interface/PTMInterface.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     int i = 0;
     for (i=0;i<num_types;i++)
     {
       PyObject* obj_type = PyTuple_GetItem(obj_types, i);
       if (obj_type == NULL)
         return -1;
 
-      if (!PyBytes_Check(obj_type))
+      if (!PyAsapString_Check(obj_type))
       {
-        PyErr_SetString(PyExc_TypeError, "type is not an ASCII string (bytes)");
+        PyErr_SetString(PyExc_TypeError, "type is not a string");
         return -1;
       }
 
       char* type = PyBytes_AsString(obj_type);
       if (type == NULL)
         return -1;
 
@@ -88,17 +88,16 @@
   PyObject* obj_types = NULL;
   int calculate_strains = false;
   int quick = false;
   int return_nblist = false;
   PyObject *obj_return_mappings = NULL;
   DEBUGPRINT;
   
-  static char* argnames[] = {"atoms", "cutoff", "target_structures",
-			     "calculate_strains", "quick",
-			     "return_nblist", "return_mappings", NULL};
+  static char* argnames[] = {"atoms", "cutoff", "structures", "calculate_strains",
+			     "quick", "return_nblist", "return_mappings", NULL};
   if (!PyArg_ParseTupleAndKeywords(args, kwargs, "Od|OiiiO:PTM_allatoms",
 				   argnames, &obj_atoms, &cutoff,
                                    &obj_types, &calculate_strains, &quick,
 				   &return_nblist, &obj_return_mappings))
     return NULL;
 
   DEBUGPRINT;
@@ -268,15 +267,15 @@
 	    maplen = 14;
 	  else if (*type_p == PTM_MATCH_ICO && (return_mappings & PTM_CHECK_ICO))
 	    maplen = 12;
 	  else if (*type_p == PTM_MATCH_SC && (return_mappings & PTM_CHECK_SC))
 	    maplen = 6;
 	  if (maplen)
 	    {
-	      PyObject *key = PyLong_FromLong(i);
+	      PyObject *key = PyAsapInt_FromLong(i);
 	      PyObject *value = PyArray_SimpleNew(1, &maplen, NPY_INT);
 	      if (key == NULL || value == NULL || PyDict_SetItem(dict_mappings, key, value) == -1)
 		{
 		  Py_DECREF(arr_type);
 		  Py_DECREF(arr_alloy);
 		  Py_DECREF(arr_scale);
 		  Py_DECREF(arr_rmsd);
```

### Comparing `asap3-3.13.1/Interface/PTMInterface.h` & `asap3-3.9.6/OpenKIMimport/OpenKIMinterface.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-// -*- C++ -*-
-// PTMInterface.h: Python interface to the Polyhedral Template Matching function.
+// OpenKIMinterface.cpp - Python interface to OpenKIM models.
 //
-// Copyright (C) 2016 Jakob Schiotz and Center for Atomic-scale
-// Materials Design, Department of Physics, Technical
+// This file is part of the optional Asap module to support OpenKIM
+// models.  Defines the Python interface to the modules in the
+// other files in OpenKIMimport.
+
+// Copyright (C) 2014 Jakob Schiotz and Center for Individual
+// Nanoparticle Functionality, Department of Physics, Technical
 // University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
+// Asap is released under the GNU Lesser Public License (LGPL) version 3.
+// However, the parts of Asap distributed within the OpenKIM project
+// (including this file) are also released under the Common Development
+// and Distribution License (CDDL) version 1.0.
 //
 // This program is free software: you can redistribute it and/or
 // modify it under the terms of the GNU Lesser General Public License
 // version 3 as published by the Free Software Foundation.  Permission
 // to use other versions of the GNU Lesser General Public License may
 // granted by Jakob Schiotz or the head of department of the
 // Department of Physics, Technical University of Denmark, as
@@ -20,22 +27,30 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-#ifndef _PTM_INTERFACE_H
-#define _PTM_INTERFACE_H
+
+#ifndef _OPENKIMINFO_INTERFACE_H
+#define _OPENKIMINFO_INTERFACE_H
 
 #include "AsapPython.h"
 #include "Asap.h"
 
 namespace ASAPSPACE {
 
-void PyAsap_InitPTMmodule();
+extern char OpenKIMinfo_Docstring[];
+extern char OpenKIMcalculator_Docstring[];
+
+PyObject *PyAsap_NewOpenKIMinfo(PyObject *noself, PyObject *args,
+                                PyObject *kwargs);
+
+PyObject *PyAsap_NewOpenKIMcalculator(PyObject *noself, PyObject *args,
+                                      PyObject *kwargs);
 
-PyObject* PyAsap_PTMall(PyObject* noself, PyObject* args, PyObject* kwargs);
+int PyAsap_InitOpenKIMInterface(PyObject *module);
 
 } // end namespace
 
-#endif // _PTM_INTERFACE_H
+#endif // _OPENKIMINFO_INTERFACE_
```

### Comparing `asap3-3.13.1/Interface/PotentialInterface.cpp` & `asap3-3.9.6/Interface/PotentialInterface.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 #include "Morse.h"
 #include "BrennerPotential.h"
 #include "EMTParameterProviderInterface.h"
 #include "ImagePotential.h"
 //#define ASAPDEBUG
 #include "Debug.h"
 #include "AsapModule.h"
-#include <stddef.h>  // for offsetof
 
 // PyAsap_PotentialObject is defined in Potential.h
 
 // Potential base class
 namespace ASAPSPACE {
 PyTypeObject PyAsap_PotentialType = {
   PyVarObject_HEAD_INIT(NULL, 0)
@@ -202,15 +201,15 @@
   static char *kwlist[] = {"prov", "verbose", NULL};
   
   PyObject *provider = NULL;
   int verbose = 0;
   if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O!i", kwlist,
 				   &PyAsap_EMTParamProvType, &provider, &verbose))
     return -1;
-  ASSERT(provider != NULL);
+  assert(provider != NULL);
   if (PyAsap_PotentialType.tp_init((PyObject *)self, args, kwargs) < 0)
     return -1;
   try
     {
       self->cobj = new EMT((PyObject *)self, provider, verbose);
       self->orig_cobj = self->cobj;
     }
@@ -236,15 +235,15 @@
 
   PyObject *parameters = NULL;
   int no_new = 0;
   int verbose = 0;
   if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O!ii", kwlist,
                                    &PyDict_Type, &parameters, &no_new, &verbose))
     return -1;
-  ASSERT(parameters != NULL);
+  assert(parameters != NULL);
   bool no_new_parameters = (bool) no_new;
   if (PyAsap_PotentialType.tp_init((PyObject *)self, args, kwargs) < 0)
     return -1;
   try
     {
       self->cobj = new EMT2013((PyObject *)self, parameters, no_new_parameters, verbose);
       self->orig_cobj = self->cobj;
@@ -271,15 +270,15 @@
   static char *kwlist[] = {"prov", "verbose", NULL};
   
   PyObject *provider = NULL;
   int verbose = 0;
   if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O!i", kwlist,
 				   &PyAsap_EMTParamProvType, &provider, &verbose))
     return -1;
-  ASSERT(provider != NULL);
+  assert(provider != NULL);
   if (PyAsap_PotentialType.tp_init((PyObject *)self, args, kwargs) < 0)
     return -1;
   self->cobj = new MonteCarloEMT((PyObject *)self, provider, verbose);
   self->orig_cobj = self->cobj;
   if (self->cobj == NULL)
     return -1;
   return 0;
@@ -691,32 +690,30 @@
   self->cobj = new BrennerPotential((PyObject *)self);
   self->orig_cobj = self->cobj;
   if (self->cobj == NULL)
     return -1;
   return 0;
 }
 
-static void PyAsap_PotentialFinalize(PyObject *self)
+static void PyAsap_PotentialDealloc(PyObject *self)
 {
   PyAsap_PotentialObject *myself = (PyAsap_PotentialObject *) self;
   if ((myself->cobj != NULL) && (myself->cobj != myself->orig_cobj))
     delete myself->cobj;       // Delete wrapper if separate object.
   if (myself->orig_cobj != NULL)
     delete myself->orig_cobj;  // Delete the actual Potential object.
+  Py_TYPE(self)->tp_free(self);
 }
 
 
 static PyObject *PyAsap_PotentialGetPotentialEnergy(PyAsap_PotentialObject *self,
-						    PyObject *args, PyObject *kwargs)
+					      PyObject *args)
 {
-  static char* argnames[] = {"atoms", "force_consistent", NULL};
   PyObject *atoms = NULL;
-  PyObject *forceconsistent = NULL; // Ignored, force is always consistent
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|O:get_potential_energy",
-				   argnames, &atoms, &forceconsistent))
+  if (!PyArg_ParseTuple(args, "O", &atoms))
     return NULL;
   CHECK_POT_INIT;
   double e;
   try {
     e = self->cobj->GetPotentialEnergy(atoms);
   }
   POTCATCHEXCEPTION;
@@ -738,14 +735,19 @@
 #else
       accessobj = (Atoms *) PyCapsule_GetPointer(py_accessobj, "asap3.accessobj");
 #endif
       if (accessobj == NULL)
 	return NULL;
     }
   try {
+#if 0
+      std::cerr << "Potential.SetAtoms: cobj: "
+          << self->cobj << " " << self->cobj->GetName()
+          << "     orig_cobj: "<< self->orig_cobj << " " << self->orig_cobj->GetName() << std::endl;
+#endif
       self->cobj->SetAtoms(atoms, accessobj);
   }
   POTCATCHEXCEPTION;
   self->setatoms_called = true;
   Py_RETURN_NONE;
 }
 
@@ -762,72 +764,54 @@
   }
   POTCATCHEXCEPTION;
 }
 
 static PyObject *PyAsap_PotentialGetForces(PyAsap_PotentialObject *self,
 				     PyObject *args)
 {
-  DEBUGPRINT;
   PyObject *atoms = NULL;
   if (!PyArg_ParseTuple(args, "O", &atoms))
     return NULL;
   CHECK_POT_INIT;
   try {
-    DEBUGPRINT;
     FP_EXCEPT_ON;
     const vector<Vec> &forces = self->cobj->GetForces(atoms);
     FP_EXCEPT_OFF;
-    DEBUGPRINT;
     return PyAsap_ArrayFromVectorVec(forces);
   }
   POTCATCHEXCEPTION;
 }
 
-static PyObject *PyAsap_PotentialGetVirial(PyAsap_PotentialObject *self,
+static PyObject *PyAsap_PotentialGetStress(PyAsap_PotentialObject *self,
 				     PyObject *args)
 {
   PyObject *atoms = NULL;
   if (!PyArg_ParseTuple(args, "O", &atoms))
     return NULL;
   CHECK_POT_INIT;
-  vector<double> virial(6);
+  vector<double> stress(6);
   try {
-      SymTensor s = self->cobj->GetVirial(atoms);
+      SymTensor s = self->cobj->GetStress(atoms);
       for (int i = 0; i < 6; i++)
-        virial[i] = s[i];  // Should instead write a PyAsap_ArrayFromSymTensor
+        stress[i] = s[i];  // Should instead write a PyAsap_ArrayFromSymTensor
   }
   POTCATCHEXCEPTION;
-  return PyAsap_ArrayFromVectorDouble(virial);
+  return PyAsap_ArrayFromVectorDouble(stress);
 }
 
-static PyObject *PyAsap_PotentialGetVirials(PyAsap_PotentialObject *self,
+static PyObject *PyAsap_PotentialGetStresses(PyAsap_PotentialObject *self,
 					     PyObject *args)
 {
   PyObject *atoms = NULL;
   if (!PyArg_ParseTuple(args, "O", &atoms))
     return NULL;
   CHECK_POT_INIT;
   try {
-    const vector<SymTensor> &virials = self->cobj->GetVirials(atoms);
-    return PyAsap_ArrayFromVectorSymTensor(virials);
-  }
-  POTCATCHEXCEPTION;
-}
-
-static PyObject *PyAsap_PotentialGetAtomicVolumes(PyAsap_PotentialObject *self,
-						  PyObject *noargs)
-{
-  CHECK_POT_INIT;
-  try {
-    vector<double> volumes;
-    self->cobj->GetAtomicVolumes(volumes);
-    if (volumes.size())
-      return PyAsap_ArrayFromVectorDouble(volumes);
-    else
-      Py_RETURN_NONE;
+    const vector<SymTensor> &stresses = self->cobj->GetStresses(atoms);
+    return PyAsap_ArrayFromVectorSymTensor(stresses);
   }
   POTCATCHEXCEPTION;
 }
 
 static PyObject *PyAsap_PotentialGetCutoff(PyAsap_PotentialObject *self,
                                            PyObject *noargs)
 {
@@ -855,15 +839,15 @@
   EMT *emt = dynamic_cast<EMT*>(self->orig_cobj);
   if (emt != NULL && strcmp(property, "sigma") == 0)
     {
       const vector<vector<double> > &s1 = emt->GetSigma1();
       const vector<vector<double> > &s2 = emt->GetSigma2();
       PyObject *py_s1 = PyList_New(s1.size());
       PyObject *py_s2 = PyList_New(s2.size());
-      ASSERT(s1.size() == s2.size());
+      assert(s1.size() == s2.size());
       for (int i = 0; i < s1.size(); i++)
 	{
 	  PyList_SET_ITEM(py_s1, i, PyAsap_ArrayFromVectorDouble(s1[i]));
 	  PyList_SET_ITEM(py_s2, i, PyAsap_ArrayFromVectorDouble(s2[i]));
 	}
       return Py_BuildValue("NN", py_s1, py_s2);
     }
@@ -875,59 +859,53 @@
                                           PyObject *args)
 {
   int subtractE0;
   if (!PyArg_ParseTuple(args, "i", &subtractE0))
     return NULL;
   CHECK_POT_INIT;
   EMT *emt = dynamic_cast<EMT*>(self->orig_cobj);
-  ASSERT(emt != NULL);  // Should not be possible
+  assert(emt != NULL);  // Should not be possible
   emt->SetSubtractE0(subtractE0);
   Py_RETURN_NONE;
 }
 
 
 static PyObject *PyAsap_CalcReq(PyAsap_PotentialObject *self,
 				PyObject *args)
 {
   PyObject *atoms = NULL;
   PyObject *proplist = NULL;
-  if (!PyArg_ParseTuple(args, "OO:_calculation_required", &atoms, &proplist))
+  if (!PyArg_ParseTuple(args, "OO:calculation_required", &atoms, &proplist))
     return NULL;
-  ASSERT(proplist != NULL);
+  assert(proplist != NULL);
   if (!PySequence_Check(proplist))
     {
       PyErr_SetString(PyExc_TypeError, "Argument to calculation_required must be a sequence");
       return NULL;
     }
   bool result = false;
   Py_ssize_t n = PySequence_Size(proplist); 
   for (Py_ssize_t i = 0; i < n; i++)
     {
       PyObject *pystr = PySequence_GetItem(proplist, i);
-      ASSERT(pystr != NULL);
-      if (!PyUnicode_Check(pystr))
+      assert(pystr != NULL);
+      if (!PyAsapString_Check(pystr))
 	{
 	  Py_DECREF(pystr);
 	  PyErr_SetString(PyExc_ValueError, "Non-string passed to calculation_required.");
 	  return NULL;
 	}
       try {
-	const char *cstring = PyUnicode_AsUTF8(pystr);
+	const char *cstring = PyAsapString_AsString(pystr);
         if (strcmp(cstring, "energy") == 0)
           result = result || self->cobj->CalcReq_Energy(atoms);
         else if (strcmp(cstring, "forces") == 0)
           result = result || self->cobj->CalcReq_Forces(atoms);
-        else if (strcmp(cstring, "virial") == 0)
-          result = result || self->cobj->CalcReq_Virial(atoms);
         else if (strcmp(cstring, "stress") == 0)
-          result = result || self->cobj->CalcReq_Virial(atoms);  // Also virial!
-        else if (strcmp(cstring, "virials") == 0)
-          result = result || self->cobj->CalcReq_Virials(atoms);
-        else if (strcmp(cstring, "stresses") == 0)
-          result = result || self->cobj->CalcReq_Virials(atoms);  // Also virials!
+          result = result || self->cobj->CalcReq_Stress(atoms);
         else
           result = true;  // All unsupported keywords must cause True to be returned
       }
       POTCATCHEXCEPTION;
       Py_DECREF(pystr);
     }
   if (result)
@@ -945,42 +923,14 @@
     PyErr_SetString(PyExc_RuntimeError,
 		    "No neighbor list (potential still unused?)");
   else
     Py_INCREF(nbl);
   return nbl;
 }
 
-static PyObject *PyAsap_PotentialCheckUpdateNbList(PyAsap_PotentialObject *self,
-						   PyObject *args, PyObject *kwargs)
-{
-  static char* argnames[] = {"atoms", NULL};
-  PyObject *atoms = NULL;
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:check_update_neighborlist",
-				   argnames, &atoms))
-    return NULL;
-  CHECK_POT_INIT;
-  bool updated = false;
-  try {
-    updated = self->cobj->CheckAndUpdateNbList(atoms);
-  }
-  POTCATCHEXCEPTION;
-  return PyBool_FromLong((long) updated);
-}
-
-
-static PyObject *PyAsap_PotentialGetName(PyAsap_PotentialObject *self,
-					   PyObject *noargs)
-{
-  CHECK_POT_INIT;
-  string sname = self->cobj->GetName();
-  const char *name = sname.c_str();
-  return Py_BuildValue("s", name);
-}
-
-
 namespace ASAPSPACE {
 
 char PyAsap_PotentialUseImageAtoms_Docstring[] =
     "Use image atoms (disable minimum image convention). INTERNAL USE ONLY!";
 
 PyObject *PyAsap_PotentialUseImageAtoms(PyAsap_PotentialObject *self,
                                         PyObject *noargs)
@@ -1034,37 +984,31 @@
   return Py_BuildValue("l", mem);
 }
 
 static PyMethodDef PyAsap_PotentialMethods[] = {
   {"set_atoms", (PyCFunction)PyAsap_PotentialSetAtoms,
    METH_VARARGS, "Set the atoms prior to the first calculation."},
   {"get_potential_energy", (PyCFunction)PyAsap_PotentialGetPotentialEnergy,
-   METH_VARARGS|METH_KEYWORDS, "Calculate the potential energy."},
+   METH_VARARGS, "Calculate the potential energy."},
   {"get_potential_energies", (PyCFunction)PyAsap_PotentialGetPotentialEnergies,
    METH_VARARGS, "Calculate the potential energies of all atoms."},
   {"get_forces", (PyCFunction)PyAsap_PotentialGetForces,
    METH_VARARGS, "Calculate the potential energies of all atoms."},
-  {"get_virial", (PyCFunction)PyAsap_PotentialGetVirial,
+  {"get_stress", (PyCFunction)PyAsap_PotentialGetStress,
    METH_VARARGS, "Calculate the potential energies of all atoms."},
-  {"get_virials", (PyCFunction)PyAsap_PotentialGetVirials,
+  {"get_stresses", (PyCFunction)PyAsap_PotentialGetStresses,
    METH_VARARGS, "Calculate the potential energies of all atoms."},
-  {"_get_atomic_volumes", (PyCFunction)PyAsap_PotentialGetAtomicVolumes,
-   METH_NOARGS, "Get volumes of the atoms (or None if unknown) for calculation of stress."},
   {"calculation_required", (PyCFunction)PyAsap_CalcReq,
    METH_VARARGS, "Check if a calculation is required."},
-  {"_get_neighborlist", (PyCFunction)PyAsap_PotentialGetNbList,
+  {"get_neighborlist", (PyCFunction)PyAsap_PotentialGetNbList,
    METH_NOARGS,  "Return the neighbor list (if any)."},
-  {"check_update_neighborlist", (PyCFunction)PyAsap_PotentialCheckUpdateNbList,
-   METH_VARARGS|METH_KEYWORDS, "Check and possibly update the neighbor list."},
   {"supports_parallel", (PyCFunction)PyAsap_Parallel,
    METH_NOARGS,  "Return True if the calculator supports parallel simulations."},
   {"get_cutoff", (PyCFunction)PyAsap_PotentialGetCutoff,
    METH_NOARGS, "Get the cutoff distance published by the calculator."},
-  {"_get_name", (PyCFunction)PyAsap_PotentialGetName,
-   METH_NOARGS, "Get the internal name of the C++ class (for internal use only)."},
   {"print_memory", (PyCFunction)PyAsap_PotPrintMemory,
    METH_NOARGS,  "Print an estimate of the memory usage."},
   {NULL}  // Sentinel
 };
 
 static PyMethodDef PyAsap_EMTMethods[] = {
   {"get_extra", (PyCFunction)PyAsap_PotentialGetExtra,
@@ -1103,22 +1047,20 @@
   type.tp_base = &PyAsap_PotentialType;
 }
 			 
 int PyAsap_InitPotentialInterface(PyObject *module)
 {
   // Init the potentials
   PyAsap_PotentialType.tp_new = PyType_GenericNew;
-  PyAsap_PotentialType.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HAVE_FINALIZE;
+  PyAsap_PotentialType.tp_dealloc = PyAsap_PotentialDealloc;
+  PyAsap_PotentialType.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE;
   PyAsap_PotentialType.tp_methods = PyAsap_PotentialMethods;
   PyAsap_PotentialType.tp_repr = PyAsap_Representation<PyAsap_PotentialObject>;
   PyAsap_PotentialType.tp_init = (initproc) PyAsap_PotentialInit;
   PyAsap_PotentialType.tp_doc = Potential_Docstring;
-  PyAsap_PotentialType.tp_weaklistoffset = offsetof(PyAsap_PotentialObject, weakrefs);
-  PyAsap_PotentialType.tp_finalize = PyAsap_PotentialFinalize;
-  PyAsap_PotentialType.tp_dealloc = PyAsap_Dealloc;
   if (PyType_Ready(&PyAsap_PotentialType) < 0)
     return -1;
 
   InitPotentialType(PyAsap_EMTType);
   PyAsap_EMTType.tp_init = (initproc) PyAsap_EMTInit;
   PyAsap_EMTType.tp_doc = EMT_Docstring;
   PyAsap_EMTType.tp_methods = PyAsap_EMTMethods;
```

### Comparing `asap3-3.13.1/Interface/PotentialInterface.h` & `asap3-3.9.6/Interface/PotentialInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/PythonConversions.cpp` & `asap3-3.9.6/Interface/PythonConversions.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/PythonConversions.h` & `asap3-3.9.6/Interface/PythonConversions.h`

 * *Files 9% similar despite different names*

```diff
@@ -41,64 +41,64 @@
 
 inline PyObject *PyAsap_ArrayFromVectorDouble(const vector<double> &data)
 {
   npy_intp size = data.size();
   PyObject *res = PyArray_SimpleNew(1, &size, NPY_DOUBLE);
   if (res == NULL)
     return NULL;
-  ASSERT(PyArray_NBYTES((PyArrayObject *) res) ==  size*sizeof(double));
+  assert(PyArray_NBYTES((PyArrayObject *) res) ==  size*sizeof(double));
   memcpy(PyArray_DATA((PyArrayObject *) res), &data[0], size*sizeof(double));
   return res;
 }
 
 inline PyObject *PyAsap_ArrayFromVectorInt(const vector<int> &data)
 {
   npy_intp size = data.size();
   PyObject *res = PyArray_SimpleNew(1, &size, NPY_INT);
   if (res == NULL)
     return NULL;
-  ASSERT(PyArray_NBYTES((PyArrayObject *) res) ==  size*sizeof(int));
+  assert(PyArray_NBYTES((PyArrayObject *) res) ==  size*sizeof(int));
   if (size > 0)
     memcpy(PyArray_DATA((PyArrayObject *) res), &data[0], size*sizeof(int));
   return res;
 }
 
 inline PyObject *PyAsap_ArrayFromVectorChar(const vector<char> &data)
 {
   npy_intp size = data.size();
   PyObject *res = PyArray_SimpleNew(1, &size, NPY_BYTE);
   if (res == NULL)
     return NULL;
-  ASSERT(PyArray_NBYTES((PyArrayObject *) res) ==  size*sizeof(char));
+  assert(PyArray_NBYTES((PyArrayObject *) res) ==  size*sizeof(char));
   memcpy(PyArray_DATA((PyArrayObject *) res), &data[0], size*sizeof(char));
   return res;
 }
 
 inline PyObject *PyAsap_ArrayFromVectorVec(const vector<Vec> &data)
 {
   npy_intp size[2];
   size[0] = data.size();
   size[1] = 3;
   PyObject *res = PyArray_SimpleNew(2, size, NPY_DOUBLE);
   if (res == NULL)
     return NULL;
-  ASSERT(PyArray_NBYTES((PyArrayObject *) res) ==  size[0]*sizeof(Vec));
+  assert(PyArray_NBYTES((PyArrayObject *) res) ==  size[0]*sizeof(Vec));
   memcpy(PyArray_DATA((PyArrayObject *) res), &data[0], size[0]*sizeof(Vec));
   return res;
 }
 
 inline PyObject *PyAsap_ArrayFromVectorSymTensor(const vector<SymTensor> &data)
 {
   npy_intp size[2];
   size[0] = data.size();
   size[1] = 6;
   PyObject *res = PyArray_SimpleNew(2, size, NPY_DOUBLE);
   if (res == NULL)
     return NULL;
-  ASSERT(PyArray_NBYTES((PyArrayObject *) res) ==  size[0]*sizeof(SymTensor));
+  assert(PyArray_NBYTES((PyArrayObject *) res) ==  size[0]*sizeof(SymTensor));
   memcpy(PyArray_DATA((PyArrayObject *) res), &data[0], size[0]*sizeof(SymTensor));
   return res;
 }
 
 int PyAsap_VectorIntFromArray(vector<int> &to, PyObject *from);
 
 int PyAsap_VectorDoubleFromArray(vector<double> &to, PyObject *from);
```

### Comparing `asap3-3.13.1/Interface/RDFInterface.cpp` & `asap3-3.9.6/Interface/RDFInterface.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -95,18 +95,18 @@
       CHKINT(PyTuple_SetItem(result, 2, rdfcountPy));
       // Now populate both Python lists
       for (int i = 0; i < nGroups; i++)
 	{
 	  PyObject *tmp;
 	  tmp = PyDict_New();
 	  CHK(tmp);
-	  PyList_SET_ITEM(rdfPy, i, tmp);
+	  CHKINT(PyList_SET_ITEM(rdfPy, i, tmp));
 	  tmp = PyDict_New();
 	  CHK(tmp);
-	  PyList_SET_ITEM(rdfcountPy, i, tmp);
+	  CHKINT(PyList_SET_ITEM(rdfcountPy, i, tmp));
 	}
       // Now we have two lists of empty dictionaries in each
       // language.  The Python RDF dictionary should now be
       // populated with pairs of elements mapping to NumPy
       // arrays containing the RDF.  The C++ maps should be
       // populated with the same pairs mapping to pointers into
       // these arrays.
@@ -132,27 +132,27 @@
 		    valPy = PyArray_ZEROS(1, &nBins, NPY_LONG, 0);
 		    CHK(valPy);
 
 		    CHKINT(PyDict_SetItem(mapPy, keyPy, valPy));
 		    Py_DECREF(keyPy); // mapPy now owns it.
 		    Py_DECREF(valPy);
 		  }
-		catch(AsapError &ex)
+		catch(AsapError ex)
 		  {
 		    Py_XDECREF(keyPy);
 		    Py_XDECREF(valPy);
 		    throw;
 		  }
 		// Fill the C++ map
 		pair<int, int> key(*e1, *e2);
 		rdf[i][key] = (long *) PyArray_DATA((PyArrayObject *) valPy);
 	      }
 	}
     }
-  catch(AsapError &ex)
+  catch(AsapError ex)
     {
       Py_DECREF(result);  // Discard all objects created so far
       std::cerr << "Error in RadialDistributionFunction (memory?) ("
 	   << __FILE__ << ":" << errln << ")" << std::endl;
       if (!PyErr_Occurred())
 	PyErr_Format(PyExc_MemoryError,
 		     "Out of memory in RadialDistributionFunction (%s:%d)",
@@ -186,15 +186,15 @@
   // objects except for rdfcount.  Insert that now.
   try
     {
       for (int i = 0; i < nGroups; i++)
 	{
 	  PyObject *mapPy = PyList_GetItem(rdfcountPy, i);
 	  CHK(mapPy);
-	  ASSERT(PyDict_Size(mapPy) == 0);
+	  assert(PyDict_Size(mapPy) == 0);
 	  map<int,long>::const_iterator enditer = rdfcount[i].end();
 	  for (map<int,long>::const_iterator mapiter = rdfcount[i].begin();
 	       mapiter != enditer; ++mapiter)
 	    {
 	      PyObject *key = Py_BuildValue("l", mapiter->first);
 	      CHK(key);
 	      PyObject *val = Py_BuildValue("l", mapiter->second);
@@ -202,15 +202,15 @@
 	      int x = PyDict_SetItem(mapPy, key, val);
 	      Py_DECREF(key);
 	      Py_DECREF(val);
 	      CHKINT(x);
 	    }
 	}
     } 
-  catch(AsapError &ex)
+  catch(AsapError ex)
     {
       Py_DECREF(result);  // Discard all objects created so far
       std::cerr << "Error in RadialDistributionFunction (memory?) ("
 	   << __FILE__ << ":" << errln << ")" << std::endl;
       if (!PyErr_Occurred())
 	PyErr_Format(PyExc_RuntimeError,
 		     "Unknown error in RadialDistributionFunction (%s:%d)",
```

### Comparing `asap3-3.13.1/Interface/RDFInterface.h` & `asap3-3.9.6/Interface/RDFInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Interface/Templates.h` & `asap3-3.9.6/Interface/Templates.h`

 * *Files 12% similar despite different names*

```diff
@@ -31,36 +31,24 @@
 
 namespace ASAPSPACE {
 
 template<class T>
 static PyObject *PyAsap_Representation(PyObject *self)
 {
   string repr = ((T*)self)->cobj->GetRepresentation();
-  return PyUnicode_FromString(repr.c_str());
+  return PyAsapString_FromString(repr.c_str());
 }
 
 template<class T>
-static void PyAsap_Finalize(PyObject *self)
-{
-  if ( ((T*)self)->cobj != NULL )
-  {
-    delete ((T*)self)->cobj;
-    ((T*)self)->cobj = NULL;
-  }
-}
-
 static void PyAsap_Dealloc(PyObject *self)
 {
-    if (PyType_HasFeature(Py_TYPE(self), Py_TPFLAGS_HAVE_FINALIZE))
-    {
-      if (PyObject_CallFinalizerFromDealloc(self))
-        return;
-    }
-    // Only clear out weakrefs if it is safe to do so.
-    if (PyType_SUPPORTS_WEAKREFS(Py_TYPE(self)) && Py_REFCNT(self) == 0)
+  if (((T*)self)->weakrefs != NULL)
         PyObject_ClearWeakRefs(self);
-    Py_TYPE(self)->tp_free(self);
+
+  if ( ((T*)self)->cobj != NULL )
+    delete ((T*)self)->cobj;
+  self->ob_type->tp_free(self);
 }
 
 } // end namespace
 
 #endif // _TEMPLATES_H
```

### Comparing `asap3-3.13.1/Interface/ToolsInterface.cpp` & `asap3-3.9.6/Interface/ToolsInterface.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,14 @@
 static int PyAsap_FullCNAInit(PyAsap_FullCNAObject *self, PyObject *args,
                               PyObject *kwargs)
 {
   static char *kwlist[] = {"atoms", "cutoff", NULL};
 
   PyObject *atoms;
   double cutoff;
-
-  self->weakrefs = NULL;
-
   if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "Od:FullCNA",
       kwlist, &atoms, &cutoff))
     return -1;
   if (cutoff <= 0.0)
     {
       PyErr_SetString(PyExc_ValueError,
           "FullCNA: Cutoff must be greater than zero.");
@@ -172,21 +169,20 @@
         METH_NOARGS,  "Return the raw CNA data."},
     {NULL}  // Sentinel
 };
 
 int PyAsap_InitToolsInterface(PyObject *module)
 {
   PyAsap_FullCNAType.tp_new = PyType_GenericNew;
-  PyAsap_FullCNAType.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_FINALIZE;
+  PyAsap_FullCNAType.tp_dealloc = PyAsap_Dealloc<PyAsap_FullCNAObject>;
+  PyAsap_FullCNAType.tp_flags = Py_TPFLAGS_DEFAULT;
   PyAsap_FullCNAType.tp_methods = PyAsap_FullCNAMethods;
   PyAsap_FullCNAType.tp_repr = PyAsap_Representation<PyAsap_FullCNAObject>;
   PyAsap_FullCNAType.tp_init = (initproc) PyAsap_FullCNAInit;
   PyAsap_FullCNAType.tp_doc = FullCNA_Docstring;
-  PyAsap_FullCNAType.tp_finalize = PyAsap_Finalize<PyAsap_FullCNAObject>;
-  PyAsap_FullCNAType.tp_dealloc = PyAsap_Dealloc;
   if (PyType_Ready(&PyAsap_FullCNAType) < 0)
     return -1;
   Py_INCREF(&PyAsap_FullCNAType);
   PyModule_AddObject(module, "FullCNA", (PyObject *) &PyAsap_FullCNAType);
   return 0;
 }
```

### Comparing `asap3-3.13.1/Interface/ToolsInterface.h` & `asap3-3.9.6/Interface/ToolsInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Makefile` & `asap3-3.9.6/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 #### (or makefile-hostname) and edit it.
 ####
 #### If you have an unsupported architecture, create a new makefike-KERNELNAME-ARCH
 #### file, and edit it.  Please send it to me at schiotz@fysik.dtu.dk
 
 
 
+# The version number is now defined in a single place
+VERSION := $(shell python Python/asap3/version.py)
+
 # ARCH is the machine architecture, used to select compiler flags etc
 # On some weird machines (Macs!) uname -m returns a name with a space in it.
 # It will be replaces with an underscore
 ARCH := $(shell uname -m | sed -e 's/ /_/g')
 HOSTNAME := $(shell uname -n | sed -e 's/ /_/g')
 KERNELNAME := $(shell uname -s | sed -e 's/ /_/g')
 
@@ -71,42 +74,50 @@
 
 ifeq ($(MAKECONFIGURATION), makefile-default)
 $(warning WARNING: No suitable configuration found.)
 endif
 $(info Getting configuration from $(MAKECONFIGURATION))
 include $(MAKECONFIGURATION)
 
-# Some versions of the Intel compilers are broken, and need to be
-# blacklisted.  Remember also to blacklist them in setup.py
-ifeq ($(COMPILER), intel)
-DUMPVERSION=$(shell $(CXX) -dumpversion)
-ifeq ($(DUMPVERSION), 15.0.1)
-$(error ERROR: Cannot compile with Intel compiler version $(DUMPVERSION) due to optimization error)
-endif
-ifeq ($(DUMPVERSION), 17.0.1)
-$(error ERROR: Cannot compile with Intel compiler version $(DUMPVERSION) due to optimization error)
-endif
-ifeq ($(DUMPVERSION), 17.0.2)
-$(error ERROR: Cannot compile with Intel compiler version $(DUMPVERSION) due to optimization error)
-endif
+ifeq ($(shell $(CXX) -dumpversion), 15.0.1)
+$(error ERROR: Cannot compile with Intel compiler version 15.0.1 due to optimization error)
 endif
 
+
 # The python executable.  May be overridden IN THE CONFIGURATION FILE for broken installations such
 # as the former DTU databar systems, or to select Python 3.
 ifndef PYTHON
 PYTHON=python
 endif
 
-
-# The version number of Asap
-VERSION := $(shell $(PYTHON) Python/asap3/version.py)
-
 # PYVER is the Python version
 PYVER := $(shell $(PYTHON) getconfig.py VERSION)
 
+# MYMAJOR is the major Python version number (i.e. 2 or 3)
+PYMAJOR := $(shell $(PYTHON) -c 'import sys; print(sys.version_info[0])')
+
+# LINKFORSHARED, PYTHONLIBS snd PYTHONCLIBDIR are variables used for
+# creating a custom Python interpreter for parallel Asap simulations.
+ifndef LINKFORSHARED
+LINKFORSHARED := $(shell $(PYTHON) getconfig.py LINKFORSHARED)
+endif
+ifndef PYTHONLIBS
+PYTHONLIBS := $(shell $(PYTHON) getconfig.py LIBS) \
+              $(shell $(PYTHON) getconfig.py LIBM)
+endif
+ifndef PYTHONCLIBDIR
+PYTHONCLIBDIR := $(shell $(PYTHON) getconfig.py LIBPL)
+endif
+ifndef PYTHONBLDLIBRARY
+PYTHONBLDLIBRARY := $(shell $(PYTHON) getconfig.py BLDLIBRARY)
+endif
+ifndef LDFLAGS
+LDFLAGS =  $(shell $(PYTHON) getconfig.py LDFLAGS)
+endif
+
 # INSTALLATION.  
 # "make install" will install .py files in the directory PYINSTALL,
 # and compiled files in BININSTALL.
 # DESTDIR is normally empty, used for relocation.
 # THIS MAY BE CHANGED IN THE CONFIGURATION FILES (i.e. on 64 bit linux)
 ifndef PYSITEPACKAGES
 PYSITEPACKAGES := $(shell $(PYTHON) getconfig.py SITEPACKAGES)
@@ -129,56 +140,56 @@
 ifndef PYTHON_INCLUDE
 PYTHON_INCLUDE := $(shell $(PYTHON) -c 'import distutils.sysconfig as ds; print("-I"+ds.get_python_inc())')
 endif
 ifndef NUMPY_INCLUDE
 NUMPY_INCLUDE:= $(shell $(PYTHON) -c 'import numpy; print("-I"+numpy.get_include())')
 endif
 
+# If ASAP_KIM_DIR is set, set ASAP_KIM_INC and ASAP_KIM_LIB
+# This is intended for an in-place installation of OpenKIM
+ifdef ASAP_KIM_DIR
+ifndef ASAP_KIM_INC
+ASAP_KIM_INC = $(ASAP_KIM_DIR)/src
+endif
+ifndef ASAP_KIM_LIB
+ASAP_KIM_LIB = $(ASAP_KIM_DIR)/src
+endif
+endif
+
 # If KIM_HOME is set, set ASAP_KIM_INC and ASAP_KIM_LIB
 # This is intended for a system-wide installation of OpenKIM
 ifdef KIM_HOME
 ifndef ASAP_KIM_INC
-ASAP_KIM_INC := -I$(KIM_HOME)/include/kim-api
+ASAP_KIM_INC = $(KIM_HOME)/include/kim-api-v1
 endif
 ifndef ASAP_KIM_LIB
-ASAP_KIM_LIB := -L$(KIM_HOME)/lib64 -L$(KIM_HOME)/lib -lkim-api
+ASAP_KIM_LIB = $(KIM_HOME)/lib
 endif
 endif
 
-# Try to determine if pkg-config knows about OpenKIM
-# Note that if KIM_HOME was set, that takes precedence.
-PKGCONFIG_KNOWS_KIM := $(shell pkg-config --exists libkim-api 1>/dev/null 2>&1 && echo yes || echo no)
-ifeq ($(PKGCONFIG_KNOWS_KIM),yes)
-    ASAP_KIM_INC := $(shell pkg-config --cflags libkim-api)
-    ASAP_KIM_LIB := $(shell pkg-config --libs libkim-api)
-endif
-
-
 # The object directories where object files are placed.
 ifndef OBJDIR
-OBJDIR = $(ARCH)$(POSTFIX)
+OBJDIR = $(ARCH)-p$(PYMAJOR)$(POSTFIX)
 endif
 ifndef BINDIR
 BINDIR = $(ARCH)
 endif
 
 
 # Source files
 
-CXXSRC_BASICS = AsapObject.cpp NormalAtoms.cpp Vec.cpp Exception.cpp  \
-	NeighborCellLocator.cpp NeighborList.cpp Matrix3x3.cpp \
-	MonteCarloAtoms.cpp Debug.cpp DynamicAtoms.cpp \
-	MolecularDynamics.cpp VelocityVerlet.cpp Timing.cpp \
-	NeighborList2013.cpp Langevin.cpp RandomNumbers.cpp \
-	ImageAtoms.cpp ImagePotential.cpp  \
-
-CXXSRC_POTENTIALS = Potential.cpp EMT.cpp MonteCarloEMT.cpp EMT2013.cpp \
+CXXSRC_BASICS = AsapObject.cpp NormalAtoms.cpp Vec.cpp Exception.cpp EMT.cpp \
 	EMTDefaultParameterProvider.cpp EMTRasmussenParameterProvider.cpp \
-	EMTPythonParameterProvider.cpp LennardJones.cpp Morse.cpp RGL.cpp \
-	RahmanStillingerLemberg.cpp MetalOxideInterface.cpp \
+	NeighborCellLocator.cpp NeighborList.cpp Matrix3x3.cpp \
+	LennardJones.cpp EMTPythonParameterProvider.cpp MonteCarloEMT.cpp \
+	MonteCarloAtoms.cpp Debug.cpp Morse.cpp \
+	DynamicAtoms.cpp MolecularDynamics.cpp VelocityVerlet.cpp Timing.cpp \
+	EMT2013.cpp NeighborList2013.cpp RGL.cpp Potential.cpp \
+	Langevin.cpp RahmanStillingerLemberg.cpp  RandomNumbers.cpp \
+	ImageAtoms.cpp ImagePotential.cpp MetalOxideInterface.cpp \
 	MetalOxideInterface2.cpp
 
 # Do not include autogenerated Basics/version.cpp on the list above, as that
 # would cause superfluous compilations.
 
 CXXSRC_INTERFACE = PotentialInterface.cpp \
 	ExceptionInterface.cpp PythonConversions.cpp \
@@ -187,36 +198,38 @@
 	OpenMPInterface.cpp PTMInterface.cpp
 
 CXXSRC_TOOLS = RawRadialDistribution.cpp CoordinationNumbers.cpp CNA.cpp \
 	GetNeighborList.cpp FullCNA.cpp SecondaryNeighborLocator.cpp
 
 CXXSRC_PTM = canonical.cpp graph_data.cpp convex_hull_incremental.cpp \
 	index_ptm.cpp alloy_types.cpp deformation_gradient.cpp \
-	normalize_vertices.cpp neighbour_ordering.cpp initialize_data.cpp
+	normalize_vertices.cpp polar_decomposition.cpp 	neighbour_ordering.cpp
 
-CXXSRC_PTM_QC = qcprot/quat.cpp qcprot/polar.cpp
+CXXSRC_PTM_QC = qcprot/qcprot.cpp qcprot/quat.cpp
 
 CXXSRC_PTM_V = voronoi/cell.cpp
 
 CSRC_EXTRA =
 
+CSRC_PARINTERFACE = mpi.c
+
 CXXSRC_PARALLEL = RegularGridDecomposition.cpp ParallelAtoms.cpp \
-	ParallelPotential.cpp AsapMPI.cpp
+	ParallelPotential.cpp
 
 SERIAL_INTERFACE = AsapSerial.cpp
 
 CXXSRC_PARINTERFACE = AsapParallel.cpp ParallelAtomsInterface.cpp \
-	ParallelPotentialInterface.cpp ParallelNeighborListInterface.cpp \
-	mpimodule.cpp
+	ParallelPotentialInterface.cpp ParallelNeighborListInterface.cpp
 
 CXXSRC_BRENNER = BrennerPotential.cpp caguts.cpp expand.cpp inter2d_iv.cpp \
 	mtable.cpp pibond.cpp radic.cpp radicdata.cpp sili_germ.cpp \
 	spgch.cpp bcuint.cpp
 
-CXXSRC_OPENKIM = OpenKIMinterface.cpp OpenKIMcalculator.cpp 
+CXXSRC_OPENKIM = OpenKIMinfo.cpp OpenKIMinterface.cpp OpenKIMcalculator.cpp \
+    DummyNeighborLocator.cpp
 
 TEMP_DOC_DIR = /tmp/Asap-documentation-$(USER)
 
 # Default values
 ifndef MPICC 
 MPICC=env LAMMPICC='$(CC)' OMPI_MPICC='$(CC)' mpicc
 endif
@@ -249,22 +262,18 @@
 endif
 ifndef LIBS
 LIBS = -lm 
 endif
 ifndef CXXSHARED
 CXXSHARED = $(CXX) -shared
 endif
-ifndef MPICXXSHARED
-MPICXXSHARED = $(MPICXX) -shared
-endif
 
 PAROBJDIR = $(OBJDIR)$(PARPOSTFIX)
 
 COMMONOBJS := $(CXXSRC_BASICS:%.cpp=Basics/$(OBJDIR)/%.o) \
-	$(CXXSRC_POTENTIALS:%.cpp=Potentials/$(OBJDIR)/%.o) \
 	$(CXXSRC_TOOLS:%.cpp=Tools/$(OBJDIR)/%.o) \
 	$(CXXSRC_INTERFACE:%.cpp=Interface/$(OBJDIR)/%.o) \
 	$(CXXSRC_BRENNER:%.cpp=Brenner/$(OBJDIR)/%.o) \
 	$(CXXSRC_PTM:%.cpp=PTM/$(OBJDIR)/%.o) \
 	$(CXXSRC_PTM_QC:qcprot/%.cpp=PTM/$(OBJDIR)/%.o) \
 	$(CXXSRC_PTM_V:voronoi/%.cpp=PTM/$(OBJDIR)/%.o) \
 	$(CSRC_EXTRA:%.c=Basics/$(OBJDIR)/%.o) 
@@ -273,15 +282,14 @@
 COMMONOBJS += $(CXXSRC_OPENKIM:%.cpp=OpenKIMimport/$(OBJDIR)/%.o) 
 endif
 
 SERIALOBJS := $(COMMONOBJS) \
 	$(SERIAL_INTERFACE:%.cpp=Interface/$(OBJDIR)/%.o)
 
 PARALLELOBJS := $(CXXSRC_BASICS:%.cpp=Basics/$(PAROBJDIR)/%.o) \
-	$(CXXSRC_POTENTIALS:%.cpp=Potentials/$(PAROBJDIR)/%.o) \
 	$(CXXSRC_TOOLS:%.cpp=Tools/$(PAROBJDIR)/%.o) \
 	$(CXXSRC_INTERFACE:%.cpp=Interface/$(PAROBJDIR)/%.o) \
 	$(CXXSRC_BRENNER:%.cpp=Brenner/$(PAROBJDIR)/%.o) \
 	$(CXXSRC_PTM:%.cpp=PTM/$(PAROBJDIR)/%.o) \
 	$(CXXSRC_PTM_QC:qcprot/%.cpp=PTM/$(PAROBJDIR)/%.o) \
 	$(CXXSRC_PTM_V:voronoi/%.cpp=PTM/$(PAROBJDIR)/%.o) \
 	$(CSRC_EXTRA:%.c=Basics/$(PAROBJDIR)/%.o) \
@@ -289,95 +297,111 @@
 	$(CXXSRC_PARINTERFACE:%.cpp=ParallelInterface/$(PAROBJDIR)/%.o) \
 	$(CSRC_PARINTERFACE:%.c=ParallelInterface/$(PAROBJDIR)/%.o) 
 
 ifdef ASAP_KIM_INC
 PARALLELOBJS += $(CXXSRC_OPENKIM:%.cpp=OpenKIMimport/$(PAROBJDIR)/%.o) 
 endif
 
-INCLUDES = -IBasics -IPotentials -ITools -IParallel -IInterface -IParallelInterface \
+INCLUDES = -IBasics -ITools -IParallel -IInterface -IParallelInterface \
 	 -IBrenner 
 ifdef ASAP_KIM_INC
-INCLUDES += -IOpenKIMimport $(ASAP_KIM_INC)
+INCLUDES += -IOpenKIMimport -I$(ASAP_KIM_INC)
 endif
 INCLUDES += $(PYTHON_INCLUDE) $(NUMPY_INCLUDE)
 
 ifdef ASAP_KIM_LIB
-LIBS += $(ASAP_KIM_LIB)
+LIBS += -L$(ASAP_KIM_LIB) -lkim-api-v1 
+EXTRA_LIBS += -L$(ASAP_KIM_LIB) -lkim-api-v1 
 CXXFLAGS += -DWITH_OPENKIM
 MPICXXFLAGS += -DWITH_OPENKIM
 DEPENDFLAGS += -DWITH_OPENKIM
 endif
 
 # Name of binaries
-ifndef BINSERIAL
-BINSERIAL = _asap_serial.so
-endif
-ifndef BINPARALLEL
-BINPARALLEL = _asap.so
-endif
+BINSERIAL = _asap_p$(PYMAJOR).so
+BINPARALLEL = asap-$(PYTHON)
 
 .DEFAULT: help
 
 help:
 	@echo
 	@echo "ASAP version $(VERSION) compilation:"
 	@echo
-	@echo "To compile the full version"
+	@echo "To compile the serial version:"
 	@echo "    make depend"
-	@echo "    make all"
+	@echo "    make serial"
 	@echo
-	@echo "To compile the serial-only version:"
+	@echo "To compile both the serial and the parallel version:"
 	@echo "    make depend"
-	@echo "    make serial"
+	@echo "    make parallel         (or make all)"
+	@echo
+	@echo "To install the serial version:"
+	@echo "    make install"
+	@echo
+	@echo "To install both the serial and the parallel version:"
+	@echo "    make install-parallel"
 	@echo
 	@echo "To make a tar file for distribution:"
 	@echo "    make tar"
 	@echo
+	@echo "To extract documentation from C++ source files, so it can be"
+	@echo "built into the Python modules as docstrings."
+	@echo "    make docs"
+	@echo "(the information will persist until updated with 'make docs' or"
+	@echo "deleted with 'make clean'.)"
+	@echo
 	@echo "To check the ASAP version number:"
 	@echo "    make version"
 	@echo
 	@echo "To check configuration variables:"
 	@echo "    make info"
 	@echo
 
-all: parallel
+all: serial parallel
 
-serial: $(BINDIR) Depend/$(OBJDIR)/depend.timestamp Basics/$(OBJDIR) Potentials/$(OBJDIR) Tools/$(OBJDIR) PTM/$(OBJDIR) Interface/$(OBJDIR) Brenner/$(OBJDIR) OpenKIMimport/$(OBJDIR) $(BINDIR)/$(BINSERIAL)
+serial: $(BINDIR) Depend/$(OBJDIR)/depend.timestamp Basics/$(OBJDIR) Tools/$(OBJDIR) PTM/$(OBJDIR) Interface/$(OBJDIR) Brenner/$(OBJDIR) OpenKIMimport/$(OBJDIR) $(BINDIR)/$(BINSERIAL)
 
-parallel: $(BINDIR) Depend/$(OBJDIR)/depend.timestamp Basics/$(PAROBJDIR) Potentials/$(PAROBJDIR) Tools/$(PAROBJDIR) PTM/$(PAROBJDIR) Interface/$(PAROBJDIR) Brenner/$(PAROBJDIR) OpenKIMimport/$(PAROBJDIR) Parallel/$(PAROBJDIR) ParallelInterface/$(PAROBJDIR)  $(BINDIR)/$(BINPARALLEL) 
+parallel: $(BINDIR) Depend/$(OBJDIR)/depend.timestamp Basics/$(PAROBJDIR) Tools/$(PAROBJDIR) PTM/$(PAROBJDIR) Interface/$(PAROBJDIR) Brenner/$(PAROBJDIR) OpenKIMimport/$(PAROBJDIR) Parallel/$(PAROBJDIR) ParallelInterface/$(PAROBJDIR)  $(BINDIR)/$(BINPARALLEL) 
 
-$(BINDIR)/$(BINSERIAL): $(SERIALOBJS) Python/asap3/version.py scripts/asap-qsub scripts/asap-sbatch
+$(BINDIR)/$(BINSERIAL): $(SERIALOBJS) Python/asap3/version.py scripts/asap-qsub
 	test -h $(BINDIR)/asap-qsub || (cd $(BINDIR) && ln -sf ../scripts/asap-qsub)
-	test -h $(BINDIR)/asap-sbatch || (cd $(BINDIR) && ln -sf ../scripts/asap-sbatch)
-	$(PYTHON) recordversion.py "$(VERSION)" "serial" "$(CXX)" "$(CXXFLAGS)" > Basics/$(OBJDIR)/version.cpp
+	python recordversion.py "$(VERSION)" "serial" "$(CXX)" "$(CXXFLAGS)" > Basics/$(OBJDIR)/version.cpp
 	$(CXX) -c $(CXXFLAGS) $(INCLUDES) Basics/$(OBJDIR)/version.cpp -o Basics/$(OBJDIR)/version.o 
 	rm -f $@
 	$(CXXSHARED) -g $(SERIALOBJS) Basics/$(OBJDIR)/version.o -o $@ $(LIBS)
 
-$(BINDIR)/$(BINPARALLEL): $(PARALLELOBJS) Python/asap3/version.py scripts/asap-qsub scripts/asap-sbatch
+$(BINDIR)/$(BINPARALLEL): $(PARALLELOBJS) Python/asap3/version.py scripts/asap-qsub asapmpiinfo-input.py
+	cp asapmpiinfo-input.py $(BINDIR)/asapmpiinfo3.py
+	echo "mpicc = '`which mpicc`'" >> $(BINDIR)/asapmpiinfo3.py
 	test -h $(BINDIR)/asap-qsub || (cd $(BINDIR) && ln -sf ../scripts/asap-qsub)
-	test -h $(BINDIR)/asap-sbatch || (cd $(BINDIR) && ln -sf ../scripts/asap-sbatch)
-	$(PYTHON) recordversion.py "$(VERSION)" "parallel" "$(MPICXX)" "$(MPICXXFLAGS)" > Basics/$(PAROBJDIR)/version_u.cpp
-	$(MPICXX) -c $(MPICXXFLAGS) $(INCLUDES) Basics/$(PAROBJDIR)/version_u.cpp -o Basics/$(PAROBJDIR)/version_u.o 
+	python recordversion.py "$(VERSION)" "parallel" "$(MPICXX)" "$(MPICXXFLAGS)" > Basics/$(PAROBJDIR)/version_p.cpp
+	$(MPICXX) -c $(MPICXXFLAGS) $(INCLUDES) Basics/$(PAROBJDIR)/version_p.cpp -o Basics/$(PAROBJDIR)/version_p.o 
 	rm -f $@
-	$(MPICXXSHARED) -g $(PARALLELOBJS) Basics/$(PAROBJDIR)/version_u.o -o $@ $(LIBS)
-
+	$(MPICXX) $(LINKFORSHARED) $(ASAPLINKFORSHARED) $(LDFLAGS) -o $@ -g \
+		$(PARALLELOBJS) Basics/$(PAROBJDIR)/version_p.o \
+		-L$(PYTHONCLIBDIR) $(PYTHONBLDLIBRARY) $(PYTHONLIBS) $(EXTRA_LIBS)
+
+# $(OBJDIR)/asap-python-serial: $(SERIALOBJS) Python/asap3/version.py
+# 	python recordversion.py '$(VERSION)' 'static' '$(CXX)' '$(CXXFLAGS)' > Basics/$(OBJDIR)/version_st.cpp
+# 	$(CXX) -c $(CXXFLAGS) $(INCLUDES) Basics/$(OBJDIR)/version_st.cpp -o Basics/$(OBJDIR)/version_st.o 
+# 	rm -f $@
+# 	$(CXX) $(LINKFORSHARED) $(ASAPLINKFORSHARED) -o $@ -g \
+# 		$(SERIALOBJS) Basics/$(OBJDIR)/version_st.o \
+# 		-L$(PYTHONCLIBDIR) -lpython$(PYVER) $(PYTHONLIBS) $(EXTRA_LIBS)
 
 clean:
-	rm -rf Basics/$(OBJDIR) Potentials/$(OBJDIR) Tools/$(OBJDIR) \
+	rm -rf Basics/$(OBJDIR) Tools/$(OBJDIR) \
 		Interface/$(OBJDIR) Parallel/$(PAROBJDIR) \
 		ParallelInterface/$(PAROBJDIR) Brenner/$(OBJDIR) \
-		OpenKIMimport/$(OBJDIR) PTM/$(OBJDIR) $(OBJDIR) $(BINDIR)
-	rm -rf Basics/$(PAROBJDIR) Potentials/$(PAROBJDIR) Tools/$(PAROBJDIR) \
+		OpenKIMimport/$(OBJDIR) PTM/$(OBJDIR) $(OBJDIR)
+	rm -rf Basics/$(PAROBJDIR) Tools/$(PAROBJDIR) \
 		Interface/$(PAROBJDIR) Brenner/$(PAROBJDIR) \
 		OpenKIMimport/$(PAROBJDIR) PTM/$(PAROBJDIR)
 
 cleanall:
-	@echo "**** Removing version.cpp files"
-	find . -name 'version.cpp' -print -delete
 	@echo "**** Removing .o files"
 	find . -name '*.o' -print -delete
 	@echo "**** Removing .a files"
 	find . -name '*.a' -print -delete
 	@echo "**** Removing .optrpt files (Intel optimization reports)"
 	find . -name '*.optrpt' -print -delete
 	@echo "**** Removing -pyc and .pyo files"
@@ -390,17 +414,17 @@
 	find . -name 'ptmmodule.so' -print -delete
 	@echo "**** Removing special build targets."
 	find . -name 'asapmpiinfo3.py' -print -delete
 	find . -name 'asap-qsub' -type l -print -delete
 	@echo "**** Removing empty directories"
 	find . -name '.git' -prune -o \( -type d -empty -print -exec rmdir {} + \)
 	@echo "**** Removing all dependencies"
-	-rm -rf Depend
+	rm -r Depend
 	@echo "**** Removing setup.py build folder"
-	-rm -rf build
+	rm -r build
 
 
 Depend/$(OBJDIR)/depend.timestamp: depend.CHANGES
 	@echo ''
 	@echo 'ERROR: The dependencies have changed. These are the last changes:'
 	@echo ''
 	@echo 'Date      Version    Description'
@@ -423,16 +447,14 @@
 depend-maybe:
 	$(MAKE) -q "Depend/$(OBJDIR)/depend.timestamp" || $(MAKE) depend
 
 depend-serial:
 	@echo "Creating dependencies for serial version (hidden for clarity)"
 	@($(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_BASICS:%=Basics/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Basics/$(OBJDIR)/\1@'; \
-	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_POTENTIALS:%=Potentials/%) $(INCLUDES) \
-		| sed -e 's@^\(.*\.o:\)@Potentials/$(OBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_TOOLS:%=Tools/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Tools/$(OBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_INTERFACE:%=Interface/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Interface/$(OBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_BRENNER:%=Brenner/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Brenner/$(OBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(SERIAL_INTERFACE:%=Interface/%) $(INCLUDES) \
@@ -453,22 +475,23 @@
 	@echo ""
 	@sleep 2
 	@echo "Creating dependencies for parallel version (hidden for clarity)"
 	@($(DEPENDMPICXX) $(DEPENDFLAG) $(CXXSRC_PARALLEL:%=Parallel/%) $(INCLUDES) $(MPIINCLUDES)\
 		| sed -e 's@^\(.*\.o:\)@Parallel/$(PAROBJDIR)/\1@'; \
 	 $(DEPENDMPICXX) $(DEPENDFLAG) $(INCLUDES) $(MPIINCLUDES) \
 		$(CXXSRC_PARINTERFACE:%=ParallelInterface/%) \
+		| sed -e 's@^\(.*\.o:\)@ParallelInterface/$(PAROBJDIR)/\1@'; \
+	 $(DEPENDMPICC) $(DEPENDFLAG) $(INCLUDES) $(MPIINCLUDES) \
+		$(CSRC_PARINTERFACE:%=ParallelInterface/%) \
 		| sed -e 's@^\(.*\.o:\)@ParallelInterface/$(PAROBJDIR)/\1@') \
 	 | $(DEPENDCLEAN) > Depend/$(OBJDIR)/make.parallel.depend
 ifneq ($(PAROBJDIR),$(OBJDIR))
 	@echo "Creating dependencies for parallel version (part 2)."
 	@($(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_BASICS:%=Basics/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Basics/$(PAROBJDIR)/\1@'; \
-	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_POTENTIALS:%=Potentials/%) $(INCLUDES) \
-		| sed -e 's@^\(.*\.o:\)@Potentials/$(PAROBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_TOOLS:%=Tools/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Tools/$(PAROBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_INTERFACE:%=Interface/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Interface/$(PAROBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(CXXSRC_BRENNER:%=Brenner/%) $(INCLUDES) \
 		| sed -e 's@^\(.*\.o:\)@Brenner/$(PAROBJDIR)/\1@'; \
 	 $(DEPENDCXX) $(DEPENDFLAG) $(SERIAL_INTERFACE:%=Interface/%) $(INCLUDES) \
@@ -495,17 +518,14 @@
 
 Basics/$(OBJDIR)/%.o: Basics/%.cpp
 	$(CXX) -c $(CXXFLAGS) $(INCLUDES) -o $@ $<
 
 Basics/$(OBJDIR)/%.o: Basics/%.c
 	$(CC) -c $(CFLAGS) $(INCLUDES) -o $@ $<
 
-Potentials/$(OBJDIR)/%.o: Potentials/%.cpp
-	$(CXX) -c $(CXXFLAGS) $(INCLUDES) -o $@ $<
-
 Tools/$(OBJDIR)/%.o: Tools/%.cpp
 	$(CXX) -c $(CXXFLAGS) $(INCLUDES) -o $@ $<
 
 Brenner/$(OBJDIR)/%.o: Brenner/%.cpp 
 	$(CXX) -c $(CXXFLAGS) $(INCLUDES) -o $@ $<
 
 PTM/$(OBJDIR)/%.o: PTM/%.cpp 
@@ -530,17 +550,14 @@
 # the parallel version, this is handled here.
 Basics/$(PAROBJDIR)/%.o: Basics/%.cpp
 	$(MPICXX) -c $(MPICXXFLAGS) $(INCLUDES) -o $@ $<
 
 Basics/$(PAROBJDIR)/%.o: Basics/%.c
 	$(MPICC) -c $(MPICFLAGS) $(INCLUDES) -o $@ $<
 
-Potentials/$(PAROBJDIR)/%.o: Potentials/%.cpp
-	$(MPICXX) -c $(MPICXXFLAGS) $(INCLUDES) -o $@ $<
-
 Tools/$(PAROBJDIR)/%.o: Tools/%.cpp
 	$(MPICXX) -c $(MPICXXFLAGS) $(INCLUDES) -o $@ $<
 
 Brenner/$(PAROBJDIR)/%.o: Brenner/%.cpp 
 	$(MPICXX) -c $(MPICXXFLAGS) $(BRENNERCFLAGS) $(INCLUDES) -o $@ $<
 
 PTM/$(PAROBJDIR)/%.o: PTM/%.cpp 
@@ -572,17 +589,14 @@
 
 ParallelInterface/$(PAROBJDIR)/%.o: ParallelInterface/%.c 
 	$(MPICC) -c $(MPICFLAGS) $(IFACEFLAGS) $(INCLUDES) $(MPIINCLUDES) -o $@ $<
 
 Basics/$(OBJDIR):
 	mkdir Basics/$(OBJDIR)
 
-Potentials/$(OBJDIR):
-	mkdir Potentials/$(OBJDIR)
-
 Tools/$(OBJDIR):
 	mkdir Tools/$(OBJDIR)
 
 PTM/$(OBJDIR):
 	mkdir PTM/$(OBJDIR)
 
 Interface/$(OBJDIR):
@@ -594,17 +608,14 @@
 OpenKIMimport/$(OBJDIR):
 	mkdir OpenKIMimport/$(OBJDIR)
 
 ifneq ($(PAROBJDIR),$(OBJDIR))
 Basics/$(PAROBJDIR):
 	mkdir Basics/$(PAROBJDIR)
 
-Potentials/$(PAROBJDIR):
-	mkdir Potentials/$(PAROBJDIR)
-
 Tools/$(PAROBJDIR):
 	mkdir Tools/$(PAROBJDIR)
 
 PTM/$(PAROBJDIR):
 	mkdir PTM/$(PAROBJDIR)
 
 Interface/$(PAROBJDIR):
@@ -619,41 +630,92 @@
 
 Parallel/$(PAROBJDIR):
 	mkdir Parallel/$(PAROBJDIR)
 
 ParallelInterface/$(PAROBJDIR):
 	mkdir ParallelInterface/$(PAROBJDIR)
 
+install:	install-serial
+	@echo 
+	@echo 
+	@echo 
+	@echo SERIAL INSTALLATION SUCCESSFUL
+	@echo
+	@echo "IMPORTANT:  For parallel installation use $(MAKE) install-parallel"
+	@echo 
+	@echo 
+
+install-serial: 	serial
+	@echo ""
+	@echo "Installing python files in $(PYINSTALL)"
+	@echo "           binary python files in $(BININSTALL)"
+	@echo "       and executables in $(EXECINSTALL)"
+	@echo
+	@sleep 3
+	test -d $(PYINSTALL) || mkdir -p $(PYINSTALL)
+	(cd Python/asap3 && find . -name '*.py' -print) | rsync -av --files-from=- Python/asap3 $(PYINSTALL)
+	$(PYTHON) -c 'from compileall import *; compile_dir("'$(PYINSTALL)'")'
+	test -d $(BININSTALL) || mkdir -p $(BININSTALL)
+	@$(MAKE) -q $(OBJDIR)/_asap.so || (echo "ERROR: Serial version not up to date!"; exit 1)
+	rm -f $(BININSTALL)/_asap.so
+	cp $(OBJDIR)/_asap.so $(BININSTALL)
+
+install-parallel: parallel install
+	@$(MAKE) -q $(OBJDIR)/asap-python || (echo "WARNING: Parallel version not up to date or could not be built!" ; exit 1)
+	rm -f $(EXECINSTALL)/asap-python
+	cp $(OBJDIR)/asapmpiinfo3.py $(BININSTALL)
+	test -d $(EXECINSTALL) || mkdir -p $(EXECINSTALL)
+	cp $(OBJDIR)/asap-python $(OBJDIR)/asap-qsub $(EXECINSTALL)
+	@echo 
+	@echo 
+	@echo 
+	@echo SERIAL+PARALLEL INSTALLATION SUCCESSFUL
+	@echo
+	@echo 
+	@echo 
+
 
 ########################################################
 ####
 ####  SPECIAL TARGETS:  Debugging, profiling etc
 ####
 ########################################################
 
+distribution:
+	$(PYTHON) check_distrib.py $(VERSION)
+
+filelist: setup-filelist.txt
+
+setup-filelist.txt: Makefile
+	rm -f setup-filelist.txt
+	touch setup-filelist.txt
+	for i in $(CXXSRC_BASICS) ; do echo Basics/$$i >> setup-filelist.txt; done
+	for i in $(CXXSRC_INTERFACE) ; do echo Interface/$$i >> setup-filelist.txt; done
+	for i in $(SERIAL_INTERFACE) ; do echo Interface/$$i >> setup-filelist.txt; done
+	for i in $(CXXSRC_BRENNER) ; do echo Brenner/$$i >> setup-filelist.txt; done
+	for i in $(CXXSRC_TOOLS) ; do echo Tools/$$i >> setup-filelist.txt; done
+
 
 tar:
 	rm -rf tmp
 	mkdir tmp
 	svn export . tmp/Asap-$(VERSION)
 	$(MAKE) -C tmp/Asap-$(VERSION) filelist
 	tar -c -v -z -C tmp -f Asap-$(VERSION).tar.gz Asap-$(VERSION)
 	rm -rf tmp
 	@echo
 	@echo "Tar file Asap-$(VERSION).tar.gz created."
 
 version:
-	@echo "ASAP version `$(PYTHON) Python/asap3/version.py`"
+	@echo "ASAP version `python Python/asap3/version.py`"
 
 info:
 	@echo "COMPILER = $(COMPILER)"
 	@echo "HAS_ICC = $(HAS_ICC)"
 	@echo "PYTHON = $(PYTHON)"
 	@echo "ARCH = $(ARCH)"
 	@echo "HOSTNAME = $(HOSTNAME)"
 	@echo "KERNELNAME = $(KERNELNAME)"
 	@echo "PYVER = $(PYVER)"
+	@echo "PYMAJOR = $(PYMAJOR)"
 	@echo "OBJDIR = $(OBJDIR)"
 	@echo "VERSION = $(VERSION)"
-	@echo "CXXFLAGS = $(CXXFLAGS)"
-	@echo "INCLUDES = $(INCLUDES)"
-	@echo "LIBS = $(LIBS)"
```

### Comparing `asap3-3.13.1/OpenKIMexport/KimAsapPython.h` & `asap3-3.9.6/OpenKIMexport/KimAsapPython.h`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 
 // Fake AsapPython.h file defining fake Python objects!
 
 #ifndef KIMASAPPYTHON_H
 #define KIMASAPPYTHON_H
 
-#include "KIM_ModelHeaders.hpp"
+#include "KIM_API_C.h"
+#include "KIM_API_status.h"
 
 #define PyObject_HEAD int ob_refcnt;
 
 typedef struct {
   PyObject_HEAD
 } PyObject;
 
@@ -55,15 +56,15 @@
 #define Py_XINCREF(op) do { if ((op) == NULL) ; else Py_INCREF(op); } while (0)
 #define Py_XDECREF(op) do { if ((op) == NULL) ; else Py_DECREF(op); } while (0)
 
 #define CHECKREF(x)
 
 #define Py_None NULL
 
-#define PyErr_SetString(a, b) LOG_ERROR(b)
+#define PyErr_SetString(a, b) KIM_API_report_error(__LINE__, __FILE__, (char *) b, KIM_STATUS_FAIL)
 
 // The following looks wrong on a 64-bit machine, but is actually OK
 // as all stuff depending on this type being 32-bit is gone in the KIM
 // wrapper case.
 typedef int npy_int32;
 
 #endif // not KIMASAPPYTHON_H
```

### Comparing `asap3-3.13.1/OpenKIMexport/KimAtoms.cpp` & `asap3-3.9.6/OpenKIMexport/KimAtoms.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -32,58 +32,56 @@
 // which is not available in OpenKIM.
 
 #include "KimAtoms.h"
 #include "Exception.h"
 #include "Debug.h"
 #include <math.h>
 
-KimAtoms::KimAtoms()
+KimAtoms::KimAtoms(intptr_t* pkim)
 {
   CONSTRUCTOR;
+  assert(pkim != NULL);
   refcount = 1;
+  this->pkim = pkim;
   counter = 2;
   count_inverse_cell = 1;
 }
 
 KimAtoms::~KimAtoms()
 {
   DESTRUCTOR;
 }
 
-void KimAtoms::ReInit(KIM::ModelComputeArguments const * const modelComputeArguments,
-		      int nAtoms,
-		      double const *pos,
-		      int const *z,
-		      int const *contributes)
+void KimAtoms::ReInit(int nAtoms, int nGhosts, double *pos, int *z)
 {
-  this->modelComputeArguments = modelComputeArguments;
   this->nAtoms = nAtoms;
-  positions.resize(nAtoms);
-  numbers.resize(nAtoms);
-  this->contributes = contributes;
-  for (int i = 0; i < nAtoms; i++)
+  this->nGhosts = nGhosts;
+  nAllAtoms = nAtoms + nGhosts;
+  positions.resize(nAllAtoms);
+  numbers.resize(nAllAtoms);
+  for (int i = 0; i < nAllAtoms; i++)
     {
       positions[i] = ((Vec *)pos)[i];
-      numbers[i] = (asap_z_int) z[i];
+      numbers[i] = z[i];
     }
   counter++;
   for (int i = 0; i < 3; i++)
     {
       for (int j = 0; j < 3; j++)
-        cell[i][j] = (i == j) * 50.0;   // Fake number as it is not really used.
+        cell[i][j] = (i == j) * 50.0;
     }
 }
 
 void KimAtoms::GetListOfElements(set<int> &elements) const
 {
   DEBUGPRINT;
   const asap_z_int *atomicnumbers = GetAtomicNumbers();
 
   elements.clear();
-  for (int i = 0; i < nAtoms; i++)
+  for (int i = 0; i < nAllAtoms; i++)
     {
       int z = atomicnumbers[i];
       if (elements.find(z) == elements.end())
         elements.insert(z);
     }
   DEBUGPRINT;
 }
@@ -118,25 +116,30 @@
 }
 
 void KimAtoms::GetPositions(vector<Vec> &pos, bool ghosts /* = false */) const
 {
   DEBUGPRINT;
   pos.clear();
   int n = nAtoms;
+  if (ghosts)
+    n = nAllAtoms;
+
   pos.reserve(n + n/25);  // 4% extra
   for (int i = 0; i < n; i++)
     pos[i] = positions[i];
 
   DEBUGPRINT;
 }
 
 void KimAtoms::GetScaledPositions(vector<Vec> &pos, bool ghosts /* = false */)
 {
   DEBUGPRINT;
   int n = nAtoms;
+  if (ghosts)
+    n += nGhosts;
   const Vec *inv = GetInverseCell();
   if (pos.capacity() < n)
     pos.reserve(n + n/25);  // Reserve 4% extra.
   pos.resize(n);
   for (int i = 0; i < n; i++)
     for (int j = 0; j < 3; j++)
       pos[i][j] = positions[i][0] * inv[0][j]
```

### Comparing `asap3-3.13.1/OpenKIMexport/KimAtoms.h` & `asap3-3.9.6/OpenKIMexport/KimAtoms.h`

 * *Files 16% similar despite different names*

```diff
@@ -58,52 +58,46 @@
   /// Delete the interface object.
   ///
   /// Protected: may only be called from AsapAtoms_DECREF() friend function.
   virtual ~KimAtoms();
 
 public:
   /// Create the interface object.
-  KimAtoms();
+  KimAtoms(intptr_t* pkim = NULL);
 
   /// Pass new KIM pointers to this object.
-  void ReInit(KIM::ModelComputeArguments const * const modelComputeArguments,
-	      int nAtoms,
-	      double const *pos,
-	      int const *z,
-	      int const *contributes);
+  void ReInit(int nAtoms, int nGhost, double *pos, int *z);
 
-  KIM::ModelComputeArguments const * const GetModelComputeArgumentsObject() {return modelComputeArguments;}
-
-  const int *GetParticleContributes() {return contributes;}
-  
   // Reference counting
   friend void AsapAtoms_INCREF(KimAtoms *atoms);
   friend void AsapAtoms_DECREF(KimAtoms *atoms);
 
   /// Begin and End do nothing
   virtual void Begin(void *pyatoms, bool expect_reopen=false) {};
   virtual void End() {};
 
   /// Atoms are always active
   inline bool IsActive() const {return true;}
 
   /// Get the number of atoms
   inline int GetNumberOfAtoms() const {return nAtoms;}
 
-  inline int GetNumberOfGhostAtoms() const {return 0;}  // All atoms in nAtoms !
+  inline int GetNumberOfGhostAtoms() const {return nGhosts;}
 
   /// Get total number of atoms in parallel simulation.
   ///
   /// In a serial simulation, same as GetNumberOfAtoms, in a parallel simulation
   /// it is the sum over these over all processors.
   virtual int GetTotalNumberOfAtoms() const {return GetNumberOfAtoms();}
 
-  // In reality, this function tells if the number of atoms might vary
-  // (e.g. in parallel simulations).
-  inline bool HasGhostAtoms() const {return true;}
+  // Note: HasGhostAtoms may have to be improved when parallel simulations
+  // are supported, see ticket #56, which is fixed for "normal" Asap use,
+  // but not necessarily for OpenKIM use (will depend on how parallelization
+  // is finally handled).
+  inline bool HasGhostAtoms() const {return nGhosts != 0;}
 
   /// Get the cartesian positions.  Ghost positions, if any, are at the end.
   inline const Vec *GetPositions() const {return &positions[0];}
 
   void GetPositions(vector<Vec> &pos, bool ghosts=false) const;
 
   void GetScaledPositions(vector<Vec> &scaledpos, bool ghosts=false);
@@ -164,19 +158,20 @@
 public:
   // Public data (naughty!)
   int refcount;           ///< Number of references to this object.
   NeighborLocator *kim_interface_nblist;
 
 private:
   // Data
-  const KIM::ModelComputeArguments *modelComputeArguments;
+  intptr_t* pkim;   // KIM API object.
   int nAtoms;  // The number of atoms
+  int nGhosts;
+  int nAllAtoms;
   vector<Vec> positions;  ///< A copy of the positions of the atoms.
   vector<asap_z_int> numbers;    ///< A copy of the atomic numbers.
-  const int *contributes;  ///< Does the atom contribute? (Not a copy, no casting).
   int counter, count_inverse_cell;
   Vec cell[3];            ///< The unit cell
   Vec inverse[3];         ///< The inverse unit cell
   double heights[3];      ///< Heights of the unit cell
   bool pbc[3];
   asapkim_nbtype nbtype;
 };
```

### Comparing `asap3-3.13.1/OpenKIMexport/KimNeighborLocator.cpp` & `asap3-3.9.6/OpenKIMexport/KimNeighborMIOPBCF.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 // -*- C++ -*-
 //
-// KimNeighborLocator.cpp: Common base class for KIM interface neighbor locators.
+// KimNeighborMIOPBCF.cpp: Kim Minimum-image periodic boundary conditions
+// full neighbor list.
 //
 // Copyright (C) 2012-2013 Jakob Schiotz and the Department of Physics,
 // Technical University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
 // Asap is released under the GNU Lesser Public License (LGPL) version 3.
 // However, the parts of Asap distributed within the OpenKIM project
@@ -24,93 +25,76 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-#include "KimNeighborLocator.h"
-#include "KIM_ModelHeaders.hpp"
-#include "Asap.h"
-#include "Debug.h"
+#include "KimNeighborMIOPBCF.h"
+#include "KimAsapPython.h"
+#include "KIM_API_C.h"
+#include "KIM_API_status.h"
+#include <math.h>
 
 namespace ASAPSPACE {
 
-PyAsap_NeighborLocatorObject *PyAsap_NewKimNeighborLocator(KimAtoms *atoms,
-							   double rCut)
+PyAsap_NeighborLocatorObject *PyAsap_NewKimNeighborMIOPBCF(intptr_t* pkim,
+                                                           KimAtoms *atoms,
+                                                           double rCut)
 {
   PyAsap_NeighborLocatorObject *self;
 
   self = (PyAsap_NeighborLocatorObject*) malloc(sizeof(PyAsap_NeighborLocatorObject));
   if (self == NULL)
     throw AsapError("malloc failed.");
 
   self->ob_refcnt = 1;
   self->weakrefs = NULL;
   self->fulllist = false;
-  self->cobj = new KimNeighborLocator(atoms, rCut);
+  self->cobj = new KimNeighborMIOPBCF(pkim, atoms, rCut);
   if (self->cobj == NULL)
     {
       CHECKREF(self);
       Py_DECREF(self);
       throw AsapError("Failed to create a new NeighborList object.");
     }
   return self;
 }
 
 } // end namespace
 
 
-
-KimNeighborLocator::KimNeighborLocator(KimAtoms *atoms, double rCut)
-{
-  CONSTRUCTOR;
-  this->atoms = atoms;
-  AsapAtoms_INCREF(atoms);
-  nAtoms = nGhosts = 0;
-  this->rcut = rCut;
-  rcut2 = rCut*rCut;
-}
-
-KimNeighborLocator::~KimNeighborLocator()
-{
-  DESTRUCTOR;
-  AsapAtoms_DECREF(atoms);
-}
-
-bool KimNeighborLocator::CheckNeighborList()
-{
-  bool result = (nAtoms != atoms->GetNumberOfAtoms());
-  UpdateNeighborList();
-  nAtoms = atoms->GetNumberOfAtoms();
-  nGhosts = atoms->GetNumberOfAtoms();
-  return result;
-}
-
-int KimNeighborLocator::GetFullNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
-					 int& size, double r /* = -1.0 */ ) const
+int KimNeighborMIOPBCF::GetFullNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
+                                        int& size, double r /* = -1.0 */ ) const
 {
-  int numberOfNeighbors;
-  const int *rawneighbors;
-  KIM::ModelComputeArguments const * const modelComputeArguments = atoms->GetModelComputeArgumentsObject();
-  assert(modelComputeArguments != NULL);
-  int error = modelComputeArguments->GetNeighborList(0, n, &numberOfNeighbors, &rawneighbors);
-  if (error)
-    throw AsapError("modelComputeArguments->GetNeighborLists failed ") << __FILE__ << ":" << __LINE__;
+  int currentAtom;
+  int number;
+  int *rawneighbors;
+  double *Rij;  // Not used in this KIM neighborlist mode.
+  int ier = KIM_API_get_neigh((void*)pkim, nbmode, check_iterator(n),
+      &currentAtom, &number, &rawneighbors, &Rij);
+  if (KIM_STATUS_OK != ier)
+    throw AsapError("KIM_API_get_neigh failed ") << __FILE__ << ":" << __LINE__;
+  assert(currentAtom == n);
   // Now construct the list of distance vectors
   const Vec *pos = atoms->GetPositions();
   const Vec *thispos = pos + n;
   int numnb = 0;
   double rcut2 = this->rcut2;
   if (r > 0)
     rcut2 = r*r;
-  for (int i = 0; i < numberOfNeighbors; i++)
+  for (int i = 0; i < number; i++)
     {
       const Vec *otherpos = pos + rawneighbors[i];
       diffs[numnb] = *otherpos - *thispos;
+      for (int j = 0; j < 3; j++)
+        {
+          if (fabs(diffs[numnb][j]) > 0.5*boxSideLengths[j])
+            diffs[numnb][j] -= (diffs[numnb][j]/fabs(diffs[numnb][j])) * boxSideLengths[j];
+        }
       diffs2[numnb] = diffs[numnb] * diffs[numnb];
       if (diffs2[numnb] <= rcut2)
         {
           neighbors[numnb] = rawneighbors[i];
           numnb++;
         }
     }
```

### Comparing `asap3-3.13.1/OpenKIMexport/KimNeighborLocator.h` & `asap3-3.9.6/OpenKIMexport/KimNeighborLocator.h`

 * *Files 12% similar despite different names*

```diff
@@ -36,32 +36,21 @@
 
 #include "NeighborLocator.h"
 
 #define INVALIDMETHOD {throw AsapError("Invalid KimNeighborLocator method called.");}
 
 namespace ASAPSPACE {
 
-PyAsap_NeighborLocatorObject *PyAsap_NewKimNeighborLocator(KimAtoms *atoms,
-							   double rCut);
-
-
 class KimNeighborLocator : public NeighborLocator
 {
 public:
-  KimNeighborLocator(KimAtoms *atoms, double rCut);
-  
-  friend PyAsap_NeighborLocatorObject *PyAsap_NewKimNeighborLocator(KimAtoms *atoms,
-								    double rCut);
+  KimNeighborLocator(intptr_t *pkim, KimAtoms *atoms);
 
-  friend void PyAsap_Finalize<PyAsap_NeighborLocatorObject>(PyObject *self);
-
-protected:
   virtual ~KimNeighborLocator();
 
-public:
   virtual string GetName() const INVALIDMETHOD;
 
   /// Check if the neighbor list can still be reused, update if not.
   ///
   /// KIM version: Call UpdateNeighborList and then return false.
   virtual bool CheckAndUpdateNeighborList() {return CheckNeighborList();}
 
@@ -78,15 +67,15 @@
   /// KIM version: Call UpdateNeigborList and then return false.
 
   virtual bool CheckNeighborList();
 
   /// Update neighbor list
   ///
   /// KIM version: Extract any necessary info from the API object.
-  virtual void UpdateNeighborList() {invalid = false;}  // Not much needed for this one.;
+  virtual void UpdateNeighborList() = 0;
 
   /// Get wrapped positions of all the atoms
   virtual const vector<Vec> &GetWrappedPositions() const INVALIDMETHOD
 
   virtual void GetWrappedPositions(vector<Vec> &wp) const INVALIDMETHOD;
 
   /// Get scaled positions of all the atoms
@@ -105,20 +94,16 @@
   ///
   /// Out values: neighbors[] contains the numbers of the atoms,
   /// diffs[] contains the \em relative positions of the atoms,
   /// diffs2[] contains the norms of the diffs vectors.
   ///
   /// Return value: The number of neighbors.
   virtual int GetNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
-                           int& size, double r = -1.0) const
-    {throw AsapError("Trying to use an OpenKIM full neighbor list as a half list");}
+                           int& size, double r = -1.0) const = 0;
 
-  virtual int GetFullNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
-                           int& size, double r = -1.0) const;
-  
   /// Get the neighbors of atom n (half neighbor list).
   ///
   /// This version of GetNeighbors only returns the numbers of the neighbors.
   /// It is intended for the Python interface.
   virtual void GetNeighbors(int n, vector<int> &neighbors) const INVALIDMETHOD;
 
   /// Return the guaranteed maximal length of a single atom's NB list.
@@ -142,21 +127,23 @@
 
   /// Print internal info about an atom
   virtual void print_info(int n) INVALIDMETHOD;
 
   /// Print memory usage
   virtual long PrintMemory() const INVALIDMETHOD;
 
+protected:
+  int check_iterator(int n) const;
+
 protected:  // Data
+  intptr_t *pkim;
   KimAtoms *atoms;
   bool nbmode;
   int nAtoms;
   int nGhosts;
-  double rcut;
-  double rcut2;  // Square of cutoff
 };
 
 } // end namespace
 
 #undef INVALIDMETHOD
 #endif // !KIMNEIGHBORLOCATOR_H
```

### Comparing `asap3-3.13.1/OpenKIMexport/KimTemplates.h` & `asap3-3.9.6/OpenKIMexport/KimTemplates.h`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 #include "AsapNamespace.h"
 #include <stdlib.h>
 
 namespace ASAPSPACE {
 
 template<class T>
-static void PyAsap_Finalize(PyObject *self)
+static void PyAsap_Dealloc(PyObject *self)
 {
   if ( ((T*)self)->cobj != NULL )
     delete ((T*)self)->cobj;
   free(self);
 }
 
 } // end namespace
```

### Comparing `asap3-3.13.1/OpenKIMexport/NeighborLocatorInterface.cpp` & `asap3-3.9.6/OpenKIMexport/NeighborLocatorInterface.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 
 #include "KimAsapPython.h"
 #include "NeighborCellLocator.h"
 
 namespace ASAPSPACE {
 
 PyAsap_NeighborLocatorObject *PyAsap_NewNeighborCellLocator(KimAtoms *atoms,
-    double rCut, double driftfactor)
+    double rCut, double driftfactor, bool slave)
 {
   PyAsap_NeighborLocatorObject *self;
 
   self = (PyAsap_NeighborLocatorObject*) malloc(sizeof(PyAsap_NeighborLocatorObject));
 
   if (self == NULL)
     throw AsapError("OOPS XXXX");
 
   self->weakrefs = NULL;
   self->fulllist = false;
-  self->cobj = new NeighborCellLocator(atoms, rCut, driftfactor);
+  self->cobj = new NeighborCellLocator(atoms, rCut, driftfactor, slave);
   if (self->cobj == NULL)
     {
       CHECKREF(self);
       Py_DECREF(self);
       throw AsapError("Failed to create a new NeighborCellLocator object.");
     }
   return self;
```

### Comparing `asap3-3.13.1/OpenKIMexport/asap_kim_api.cpp` & `asap3-3.9.6/OpenKIMexport/asap_kim_api.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -28,291 +28,289 @@
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
 
 #include "KimAsapPython.h"
 #include "asap_kim_api.h"
 #include "Potential.h"
-#include "KimNeighborLocator.h"
-#include "KIM_ModelDriverHeaders.hpp"
+#include "NeighborCellLocator.h"
+#include "KimNeighborMIOPBCH.h"
+#include "KimNeighborMIOPBCF.h"
+#include "KimNeighborNEIGHPUREH.h"
+#include "KimNeighborNEIGHPUREF.h"
+#include "KimNeighborNEIGHRVECH.h"
+#include "KimNeighborNEIGHRVECF.h"
+#include "KIM_API_C.h"
+#include "KIM_API_status.h"
 #include "SymTensor.h"
 #include "Debug.h"
 #include <stdlib.h>
 #include <string.h>
 
-AsapKimPotential::AsapKimPotential(KIM::ModelDriverCreate * const modelDriverCreate,
-				   bool supportvirial)
+AsapKimPotential::AsapKimPotential(intptr_t *pkim, const char* paramfile_names,
+                                   int nmstrlen, int numparamfiles,
+                                   bool supportvirial)
 {
   CONSTRUCTOR;
-  int error = 0;
-  int numparamfiles = 0;
+  int ier;
 
   potential = NULL;
   atoms = NULL;
-
-  // Register the units.  Conversion happens in the specific model.
-  
+  this->pkim = pkim;
   // Store the parameter file name(s) for later use by reinit.
-  modelDriverCreate->GetNumberOfParameterFiles(&numparamfiles);
-  paramfile_names.resize(numparamfiles);
-  for (int i = 0; i < numparamfiles; ++i)
-  {
-    std::string const * paramFileName;
-    error = modelDriverCreate->GetParameterFileName(i, &paramFileName);
-    if (error)
-      throw AsapError("AsapKimPotential: Unable to get parameter file name");
-    paramfile_names[i] = *paramFileName;
-  }
-
+  this->paramfile_names = new char[nmstrlen * numparamfiles];
+  memcpy(this->paramfile_names, paramfile_names, nmstrlen * numparamfiles);
+  this->nmstrlen = nmstrlen;
+  this->numparamfiles = numparamfiles;
   this->supportvirial = supportvirial;
-  error = modelDriverCreate->SetModelNumbering(KIM::NUMBERING::zeroBased);
-  assert(error == 0);   // Should not be able to fail.
-
-  // Store pointers -  XXXXX FIX THESE !!  
-  error = (
-    modelDriverCreate->SetRoutinePointer(
-      KIM::MODEL_ROUTINE_NAME::ComputeArgumentsCreate,
-      KIM::LANGUAGE_NAME::cpp,
-      true,
-      reinterpret_cast<KIM::Function *>(AsapKimPotential::ComputeArgumentsCreate))
-    || modelDriverCreate->SetRoutinePointer(
-      KIM::MODEL_ROUTINE_NAME::ComputeArgumentsDestroy,
-      KIM::LANGUAGE_NAME::cpp,
-      true,
-      reinterpret_cast<KIM::Function *>(AsapKimPotential::ComputeArgumentsDestroy))
-    || modelDriverCreate->SetRoutinePointer(
-      KIM::MODEL_ROUTINE_NAME::Compute,
-      KIM::LANGUAGE_NAME::cpp,
-      true,
-      reinterpret_cast<KIM::Function *>(AsapKimPotential::Compute_static))
-    || modelDriverCreate->SetRoutinePointer(
-      KIM::MODEL_ROUTINE_NAME::Destroy,
-      KIM::LANGUAGE_NAME::cpp,
-      true,
-      reinterpret_cast<KIM::Function *>(AsapKimPotential::Destroy))
-    //|| modelDriverCreate->SetRefreshPointer(
-    //  KIM::LANGUAGE_NAME::cpp,
-    //  (KIM::Function *)2)
-    );
-  assert(error == 0);  // Should not be able to fail.
+  // Check for the neighbor list type.
+  ier = KIM_API_get_NBC_method(pkim, &NBCstr);
+  if (KIM_STATUS_OK > ier)
+    {
+      KIM_API_report_error(__LINE__, __FILE__, "KIM_API_get_NBC_method", ier);
+      exit(1);
+    }
+  if (!strcmp("CLUSTER",NBCstr))
+    {
+      nblisttype = nbl_cluster;
+      need_contrib = false;
+    }
+  else if (!strcmp("MI_OPBC_H",NBCstr))
+    {
+      nblisttype = nbl_miopbc_h;
+      need_contrib = true;
+    }
+  else if (!strcmp("MI_OPBC_F",NBCstr))
+    {
+      nblisttype = nbl_miopbc_f;
+      need_contrib = false;
+    }
+  else if (!strcmp("NEIGH_PURE_H",NBCstr))
+    {
+      nblisttype = nbl_pure_h;
+      need_contrib = true;
+    }
+  else if (!strcmp("NEIGH_PURE_F",NBCstr))
+    {
+      nblisttype = nbl_pure_f;
+      need_contrib = false;
+    }
+  else if (!strcmp("NEIGH_RVEC_H",NBCstr))
+    {
+      nblisttype = nbl_rvec_h;
+      need_contrib = true;
+    }
+  else if (!strcmp("NEIGH_RVEC_F",NBCstr))
+    {
+      nblisttype = nbl_rvec_f;
+      need_contrib = false;
+    }
+  else
+    {
+      KIM_API_report_error(__LINE__, __FILE__, "Unknown NBC method", KIM_STATUS_FAIL);
+      exit(1);
+    }
 }
 
 AsapKimPotential::~AsapKimPotential()
 {
   DESTRUCTOR;
   if (potential != NULL)
     delete potential;
   if (atoms != NULL)
     AsapAtoms_DECREF(atoms);
+  delete paramfile_names;
 }
 
-void AsapKimPotential::SetPotential(Potential *pot)
-{
-  potential = pot;
-  potential_as_kimmixin = dynamic_cast<PotentialKimMixin*>(pot);
-  assert(potential_as_kimmixin != NULL);
-}
-
-PyAsap_NeighborLocatorObject *AsapKimPotential::CreateNeighborList(KimAtoms *atoms,
-                                                                   double cutoff,
-                                                                   double drift)
+int AsapKimPotential::compute_static(void* km)
 {
   int ier;
-  PyAsap_NeighborLocatorObject *nblist;
-  atoms->SetPBC(true, true, true);
-  nblist = PyAsap_NewKimNeighborLocator(atoms, cutoff);
-  return nblist;
-}
-
-// static member function
-int AsapKimPotential::ComputeArgumentsCreate(
-  KIM::ModelCompute const * const modelCompute,
-  KIM::ModelComputeArgumentsCreate * const modelComputeArgumentsCreate)
-{
-  AsapKimPotential *modelObject;
-  modelCompute->GetModelBufferPointer(reinterpret_cast<void **>(&modelObject));
-
-  return modelObject->potential_as_kimmixin->ComputeArgumentsCreate(
-      modelComputeArgumentsCreate);
-}
-
-// static member function
-int AsapKimPotential::ComputeArgumentsDestroy(
-  KIM::ModelCompute const * const modelCompute,
-  KIM::ModelComputeArgumentsDestroy * const modelComputeArgumentsDestroy)
-{
-  AsapKimPotential *modelObject;
-  modelCompute->GetModelBufferPointer(reinterpret_cast<void **>(&modelObject));
-
-  return modelObject->potential_as_kimmixin->ComputeArgumentsDestroy(
-      modelComputeArgumentsDestroy);
-}
-
-
-// static member function
-int AsapKimPotential::Destroy(KIM::ModelDestroy * const modelDestroy)
-{
-  AsapKimPotential *modelObject;
-  modelDestroy->GetModelBufferPointer(reinterpret_cast<void **>(&modelObject));
-
-  if (modelObject != NULL)
-  {
-    // delete object itself
-    delete modelObject;
-  }
-
-  // everything is good
-  return false;
+  assert(km != NULL);
+  intptr_t* pkim = *((intptr_t**) km);
+  assert(pkim != NULL);
+  AsapKimPotential *model = (AsapKimPotential *) KIM_API_get_model_buffer(pkim, &ier);
+  if (KIM_STATUS_OK > ier)
+    {
+      KIM_API_report_error(__LINE__, __FILE__, "KIM_API_get_model_buffer", ier);
+      return ier;
+    }
+  assert(model != NULL);
+  ier = model->compute(km);
+  return ier;
 }
 
-
-// static member function
-int AsapKimPotential::Compute_static(KIM::ModelCompute const * const modelCompute,
-				     KIM::ModelComputeArguments const * const modelComputeArguments)
+int AsapKimPotential::compute(void* km)
 {
-  AsapKimPotential * modelObject;
-  modelCompute->GetModelBufferPointer(reinterpret_cast<void **>(&modelObject));
-
-  return modelObject->Compute(modelCompute, modelComputeArguments);
-}
-
-#define MYLOG(x) modelCompute->LogEntry(KIM::LOG_VERBOSITY::error, x, __LINE__, __FILE__)
+  int ier;
 
-int AsapKimPotential::Compute(KIM::ModelCompute const * const modelCompute,
-			      KIM::ModelComputeArguments const * const modelComputeArguments)
-{
-  int error;
   assert(potential != NULL);
+  assert(pkim = *((intptr_t**) km));   // Sanity check
+  double *cutoff = NULL;
+  int *nAtoms = NULL;
+  int *nTotalAtoms = NULL;
+  int* particleSpecies = NULL;
+
+  // Flags indicating what we need to compute.
+  int comp_energy;
+  int comp_force;
+  int comp_particleEnergy;
+  int comp_virial = 0;
+  int comp_particleVirial = 0;
 
-  // Information from the atoms
-  int nAtoms = 0;
-  int *nAtoms_p = NULL;
-  
-  const double *coords = NULL;
-  const int *particleSpecies = NULL;
-  const int *particleContributing = NULL;
-
-  error =
-    modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::numberOfParticles,
-					      &nAtoms_p);
-  if (error)
-  {
-    MYLOG("Failed to get number of atoms.");
-    return error;
-  }
-  assert(nAtoms_p != NULL);
-  nAtoms = *nAtoms_p;
-  assert(nAtoms >= 0);
-  
-  error =
-    modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::coordinates,
-					      &coords)
-    || modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::particleSpeciesCodes,
-						 &particleSpecies)
-    || modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::particleContributing,
-						 &particleContributing);
-  if (error)
-  {
-    MYLOG("Failed to get coordinates, species or contribution pointer.");
-    return error;
-  }
-  assert(coords != NULL && particleSpecies != NULL && particleContributing != NULL);
-  
   // Quantities to be computed
+  double *coords = NULL;
   double *energy = NULL;
   double *forces = NULL;
   double *particleEnergy = NULL;
   double *virial = NULL;
   double *particleVirial = NULL;
 
-  error =
-    modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::partialEnergy,
-					      &energy)
-    || modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::partialParticleEnergy,
-						 &particleEnergy)
-    || modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::partialForces,
-						 &forces);
-  if (error)
-  {
-    MYLOG("Failed to get energy or force pointer.");
-    return error;
-  }
-  if (supportvirial)
-  {
-    error =(
-      modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::partialVirial,
-						&virial)
-      || modelComputeArguments->GetArgumentPointer(KIM::COMPUTE_ARGUMENT_NAME::partialParticleVirial,
-						 &particleVirial)
-      );
-    if (error)
+  /* check to see if we have been asked to compute the forces and particleEnergy */
+  /* If we support virials, also check if we should calculate them */
+  KIM_API_getm_compute(pkim, &ier, 5*3,
+                       "energy",         &comp_energy,         1,
+                       "forces",         &comp_force,          1,
+                       "particleEnergy", &comp_particleEnergy, 1,
+                       "virial",         &comp_virial,         supportvirial,
+                       "particleVirial", &comp_particleVirial, supportvirial
+  );
+  if (KIM_STATUS_OK > ier)
     {
-      MYLOG("Failed to get virial pointers.");
-      return error;
+      KIM_API_report_error(__LINE__, __FILE__, "KIM_API_getm_compute", ier);
+      return ier;
     }
-  }
 
-  // Create or update the KIM replacement of the ASAP Atoms access object.
+  KIM_API_getm_data(pkim, &ier, 10*3,
+                    "cutoff",                      &cutoff,          1,
+                    "numberOfParticles",           &nTotalAtoms,     1,
+                    "numberContributingParticles", &nAtoms,          need_contrib,
+                    "particleSpecies",             &particleSpecies, 1,
+                    "coordinates",                 &coords,          1,
+                    "energy",                      &energy,          comp_energy,
+                    "forces",                      &forces,          comp_force,
+                    "particleEnergy",              &particleEnergy,  comp_particleEnergy,
+                    "virial",                      &virial,          comp_virial,
+                    "particleVirial",              &particleVirial,  comp_particleVirial
+                    );
+  if (KIM_STATUS_OK > ier)
+    {
+      KIM_API_report_error(__LINE__, __FILE__, "KIM_API_getm_data", ier);
+      return ier;
+    }
+  if (!need_contrib)
+    nAtoms = nTotalAtoms;
+
   if (atoms == NULL)
     {
       // First call, create the Atoms interface object
-      atoms = new KimAtoms();
+      atoms = new KimAtoms(pkim);
       assert(atoms != NULL);
-      atoms->ReInit(modelComputeArguments, nAtoms, coords, particleSpecies, particleContributing);
-      try {
-	potential->SetAtoms(NULL, atoms);
-      }
-      catch (AsapError &e)
-      {
-	string msg = e.GetMessage();
-	MYLOG(msg.c_str());
-	return 1;
-      }
+      atoms->ReInit(*nAtoms, *nTotalAtoms - *nAtoms, coords, particleSpecies);
+      potential->SetAtoms(NULL, atoms);
     }
   else
     {
-      atoms->ReInit(modelComputeArguments, nAtoms, coords, particleSpecies, particleContributing);
+      atoms->ReInit(*nAtoms, *nTotalAtoms - *nAtoms, coords, particleSpecies);
     }
 
   // Now do the actual computation
   try
   {
-      if (particleEnergy != NULL)
+      if (comp_particleEnergy)
         {
           const vector<double> &energies_v = potential->GetPotentialEnergies(NULL);
-          assert(energies_v.size() == nAtoms);
-          for (int i = 0; i < nAtoms; i++)
+          assert(energies_v.size() == *nAtoms);
+          for (int i = 0; i < *nAtoms; i++)
             particleEnergy[i] = energies_v[i];
         }
-      if (energy != NULL)
+      if (comp_energy)
         *energy = potential->GetPotentialEnergy(NULL);
-      if (particleVirial != NULL)
+      if (comp_particleVirial)
         {
           const vector<SymTensor> &virials = potential->GetVirials(NULL);
-          assert(virials.size() == nAtoms);
+          assert(virials.size() == *nTotalAtoms);
           const double *virials_ptr = (double *) &virials[0];
-          for (int i = 0; i < 6*(nAtoms); i++)
+          for (int i = 0; i < 6*(*nTotalAtoms); i++)
             particleVirial[i] = virials_ptr[i];
         }
-      if (virial != NULL)
+      if (comp_virial)
         {
           SymTensor v = potential->GetVirial(NULL);
           for (int i = 0; i < 6; i++)
             virial[i] = v[i];
         }
-      if (forces != NULL)
+      if (comp_force)
         {
           const vector<Vec> &forces_v = potential->GetForces(NULL);
-          assert(forces_v.size() == nAtoms);
+          assert(forces_v.size() == *nTotalAtoms);
           const double *forces_v_ptr = (double *) &forces_v[0];
-          for (int i = 0; i < 3*(nAtoms); i++)
+          for (int i = 0; i < 3*(*nTotalAtoms); i++)
             forces[i] = forces_v_ptr[i];
         }
   }
   catch (AsapError &e)
   {
+      ier = KIM_STATUS_FAIL;
       string msg = e.GetMessage();
-      MYLOG(msg.c_str());
-      return 1;
+      // Will the following line store a pointer to something inside msg? Hopefully not!
+      KIM_API_report_error(__LINE__, __FILE__, (char *) msg.c_str(), ier);
+      return ier;
   }
-  return 0;
+  return KIM_STATUS_OK;
+}
+
+
+PyAsap_NeighborLocatorObject *AsapKimPotential::CreateNeighborList(KimAtoms *atoms,
+                                                                   double cutoff,
+                                                                   double drift)
+{
+  int ier;
+  PyAsap_NeighborLocatorObject *nblist;
+  if (nblisttype == nbl_cluster)
+    {
+      atoms->SetPBC(false, false, false);
+      nblist = PyAsap_NewNeighborCellLocator(atoms, cutoff, drift);
+      assert(nblist != NULL);
+    }
+  else if (nblisttype == nbl_miopbc_h)
+    {
+      atoms->SetPBC(true, true, true);
+      nblist = PyAsap_NewKimNeighborMIOPBCH(pkim, atoms, cutoff);
+    }
+  else if (nblisttype == nbl_miopbc_f)
+    {
+      atoms->SetPBC(true, true, true);
+      nblist = PyAsap_NewKimNeighborMIOPBCF(pkim, atoms, cutoff);
+    }
+  else if (nblisttype == nbl_pure_h)
+    {
+      atoms->SetPBC(true, true, true);
+      nblist = PyAsap_NewKimNeighborNEIGHPUREH(pkim, atoms, cutoff);
+    }
+  else if (nblisttype == nbl_pure_f)
+    {
+      atoms->SetPBC(true, true, true);
+      nblist = PyAsap_NewKimNeighborNEIGHPUREF(pkim, atoms, cutoff);
+    }
+  else if (nblisttype == nbl_rvec_h)
+    {
+      atoms->SetPBC(true, true, true);
+      nblist = PyAsap_NewKimNeighborNEIGHRVECH(pkim, atoms, cutoff);
+    }
+  else if (nblisttype == nbl_rvec_f)
+    {
+      atoms->SetPBC(true, true, true);
+      nblist = PyAsap_NewKimNeighborNEIGHRVECF(pkim, atoms, cutoff);
+    }
+  else
+    {
+      throw AsapError("Unknown NBC method: ") << NBCstr;
+    }
+  return nblist;
+}
+
+bool AsapKimPotential::UsesKimFullList()
+{
+  return ( (nblisttype == nbl_miopbc_f) ||
+           (nblisttype == nbl_pure_f) ||
+           (nblisttype == nbl_rvec_f) );
 }
```

### Comparing `asap3-3.13.1/OpenKIMexport/asap_kim_api.h` & `asap3-3.9.6/OpenKIMexport/KimNeighborMIOPBCF.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 // -*- C++ -*-
 //
-// asap_kim_api.h: Common interfaces classes for Asap potentials in OpenKIM.
+// KimNeighborMIOF.h: Kim Minimum-image periodic boundary conditions
+// full neighbor list.
 //
 // Copyright (C) 2012-2013 Jakob Schiotz and the Department of Physics,
 // Technical University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
 // Asap is released under the GNU Lesser Public License (LGPL) version 3.
 // However, the parts of Asap distributed within the OpenKIM project
@@ -24,92 +25,64 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
+#ifndef KIMNEIGHBORMIOPBCF_H
+#define KIMNEIGHBORMIOPBCF_H
 
-#ifndef ASAP_KIM_API_H
-#define ASAP_KIM_API_H
-
-#include "KimAtoms.h"
-#include "NeighborLocator.h"
+#include "KimNeighborMIOPBCH.h"
 
 namespace ASAPSPACE {
 
-class Potential;
+PyAsap_NeighborLocatorObject *PyAsap_NewKimNeighborMIOPBCF(intptr_t* pkim,
+                                                           KimAtoms *atoms,
+                                                           double rCut);
 
-class PotentialKimMixin
+class KimNeighborMIOPBCF : public KimNeighborMIOPBCH
 {
-public:
-  // PotentialKimMixin() {};
+protected:
+  KimNeighborMIOPBCF(intptr_t* pkim, KimAtoms *atoms, double rCut) :
+    KimNeighborMIOPBCH(pkim, atoms, rCut) {};
+
+  friend PyAsap_NeighborLocatorObject *PyAsap_NewKimNeighborMIOPBCF(intptr_t *pkim,
+                                                                    KimAtoms *atoms,
+                                                                    double rCut);
 
-  virtual int ComputeArgumentsCreate(
-    KIM::ModelComputeArgumentsCreate * const modelComputeArgumentsCreate) const = 0;
+  friend void PyAsap_Dealloc<PyAsap_NeighborLocatorObject>(PyObject *self);
 
-  // Per default, no ComputeArgumentsDestroy is needed.
-  virtual int ComputeArgumentsDestroy(
-    KIM::ModelComputeArgumentsDestroy * const modelComputeArgumentsDestroy) const {return 0;}
-};  
-
-// AsapKimPotential is the main object that KIM interfaces with.  It
-// delegates almost everything to the actual potential, which is both
-// an instance of an asap Potential and an instance of
-// PotentialKimMixin (multiple inheritance!).
-class AsapKimPotential
-{
 public:
-  AsapKimPotential(KIM::ModelDriverCreate * const modelDriverCreate,
-		   bool supportvirial);
-  virtual ~AsapKimPotential();
-
-  // Set the potential, it must be both a Potential and a PotentialKimMixin.
-  void SetPotential(Potential *pot);
-  
-  static int compute_static(void *km);
-  int compute(void *km);
-
-  PyAsap_NeighborLocatorObject *CreateNeighborList(KimAtoms *atoms,
-                                                   double cutoff,
-                                                   double drift);
-
-private:
-
-  int Compute(KIM::ModelCompute const * const modelCompute,
-              KIM::ModelComputeArguments const * const modelComputeArguments);
-  
-  // The following member functions are static, they are called as
-  // functions (not methods of an instance) to set up the API,
-  // information about the instance actually being set up is extracted
-  // from the first argument.
-  static int ComputeArgumentsCreate(
-    KIM::ModelCompute const * const modelCompute,
-    KIM::ModelComputeArgumentsCreate * const modelComputeArgumentsCreate);
-
-  static int ComputeArgumentsDestroy(
-    KIM::ModelCompute const * const modelCompute,
-    KIM::ModelComputeArgumentsDestroy * const modelComputeArgumentsDestroy);
-
-  static int Destroy(KIM::ModelDestroy * const modelDestroy);
+  // Destructor should be protected, but friend template functions do
+  // not work with GNU C++.
+  virtual ~KimNeighborMIOPBCF() {};
+
+  /// Get info about the neighbors of atom n.  The most important method :-)
+  ///
+  /// Input values: n is the number of the atom.  r (optional) is a
+  /// cutoff, must be less than rCut in the constructor (not
+  /// checked!).
+  ///
+  /// In-out values: size contains the maximum space in the arrays.
+  /// It is decremented by the number of neighbors placed in the
+  /// arrays.  It is an error to call GetNeighbors with too small a
+  /// value of size.
+  ///
+  /// Out values: neighbors[] contains the numbers of the atoms,
+  /// diffs[] contains the \em relative positions of the atoms,
+  /// diffs2[] contains the norms of the diffs vectors.
+  ///
+  /// Return value: The number of neighbors.
+  virtual int GetNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
+                           int& size, double r = -1.0) const
+    {throw AsapError("Trying to use an OpenKIM full neighbor list as a half list (KimNeighborMIOPBCF)");}
 
-  static int Compute_static(KIM::ModelCompute const * const modelCompute,
-			    KIM::ModelComputeArguments const * const modelComputeArguments);
+  virtual int GetFullNeighbors(int n, int *neighbors, Vec *diffs, double *diffs2,
+                               int& size, double r = -1.0) const;
 
-
-  
-public:
-  vector<string> paramfile_names;   // The original parameter file name list.  Possibly used by reinit.
-  bool supportvirial;      // This potential supports virials.
-
-private:
-  //Data
-  Potential *potential;    // The ASAP potential being used
-  PotentialKimMixin *potential_as_kimmixin;   // Same potential, different interface.
-  KimAtoms *atoms;
-  bool need_contrib;
-  const char *NBCstr;   // Neighbor list string, kept for error messages.
 };
 
 } // end namespace
 
-#endif // not ASAP_KIM_API_H
+#endif // !KIMNEIGHBORMIOPBCF_H
+
```

### Comparing `asap3-3.13.1/OpenKIMimport/OpenKIMcalculator.h` & `asap3-3.9.6/OpenKIMimport/OpenKIMcalculator.h`

 * *Files 14% similar despite different names*

```diff
@@ -36,40 +36,29 @@
 
 #include "AsapPython.h"
 #include "Asap.h"
 #include "Potential.h"
 #include <map>
 #include <vector>
 
-namespace KIM {
-  class Model;
-  class ComputeArguments;
-}
+class KIM_API_model;
 
 namespace ASAPSPACE {
 
+const char *PyAsap_get_kimerror(KIM_API_model *m, int x);
+
 class OpenKIMcalculator : public Potential
 {
 public:
-  class NeighborListData
-  {
-  public:
-    vector<NeighborLocator *>nblists;
-    vector<vector<int> > nb_buffers;
-  };
-
-public:
-  OpenKIMcalculator(PyObject *self, const char *name, int verbose=0);
+  OpenKIMcalculator(PyObject *self, int verbose=0);
   ~OpenKIMcalculator();
 
-  /// Indicate if a quantity should be supported (and allocated).
-  void PleaseSupport(string quantity, bool alloc);
-
-  /// Get all compute arguments/callbacks and their supported status.
-  std::map<string,string> GetComputeArguments();    // KIM2: New
+  void Initialize(const char *descr, const char *name);
+  /// Indicate if a quantity should be allocated in the KIM API.
+  void PleaseAllocate(string quantity, bool alloc);
 
   /// This potential can be used in parallel simulations
   virtual bool Parallelizable() const {return true;}
 
   /// Check if neighbor lists need an update.
   ///
   /// Return true if the neigbor list needs an update.  In parallel
@@ -78,14 +67,17 @@
   /// simulations, it also instructs the atoms to communicate their
   /// update status.
 
   virtual bool CheckNeighborList();
   /// Update the neighbor lists
   virtual void UpdateNeighborList();
 
+  /// Get information about supported elements.
+  void GetSupportedSymbols(std::vector<const char *> &symbols);
+
   void ClearTranslation() {z_to_typecode.clear();}
   void AddTranslation(int z, int typecode) {z_to_typecode[z] = typecode;}
 
   /// Get the particle type code (number) from the particle symbol
   int GetParticleTypeCode(const char *symbol);
 
   virtual void SetAtoms(PyObject *pyatoms, Atoms* accessobj = NULL);
@@ -103,123 +95,109 @@
   virtual bool CalcReq_Forces(PyObject *pyatoms);
 
   /// Is work required to calculate the stress?
   virtual bool CalcReq_Virials(PyObject *pyatoms);
 
   virtual std::string GetName() const {return "OpenKIMcalculator";}
 
-  void GetParameterNamesAndTypes(vector<string> &names, vector<int> &datatypes,
-				 vector<int> &sizes, vector<string> &descriptions);
-
-  void GetParameter(const int parameterindex, int *value);
-  void GetParameter(const int parameterindex, double *value);
-  void GetParameter(const int parameterindex, vector<int> &values);
-  void GetParameter(const int parameterindex, vector<double> &values);
-
-  void SetParameter(const int parameterindex, int value);
-  void SetParameter(const int parameterindex, double value);
-  void SetParameter(const int parameterindex, const vector<int> &values);
-  void SetParameter(const int parameterindex, const vector<double> &values);
+  const char *GetNBCmethod();
 
   /// Return the cutoff radius used in the potential.
-  virtual double GetCutoffRadius() const {return influenceDistance;}
-
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
+  virtual double GetCutoffRadius() const {return cutoff;}
 
   /// Return the lattice constant of the material, if well-defined.
 
   /// If a lattice constant of the material can be defined, return it
   /// in Angstrom, otherwise throw an exception.
   virtual double GetLatticeConstant() const
   {throw AsapError("OpenKIMcalculator::GetLatticeConstant not supported.");}
 
   /// Print memory usage
   virtual long PrintMemory() const
   {throw AsapError("OpenKIMcalculator::PrintMemory not supported.");}
 
-  //KIM_API_model *GetKimModel() {ASSERT(model_initialized); return model;}
+  // The OpenKIM neighbor list interface function passed to the model.
+  int get_neigh(int *mode, int* request,
+        int *particle, int *numnei, int **nei1particle,
+        double **rij);
+
+  KIM_API_model *GetKimModel() {assert(model_initialized); return model;}
 
 protected:
+  typedef enum {
+    nbl_cluster, nbl_pure_h, nbl_pure_f, nbl_miopbc_h, nbl_miopbc_f, nbl_rvec_h, nbl_rvec_f
+    } nblisttype_t;
+
   /// Allocate the neighbor list.
   virtual void CreateNeighborList();
 
-  void InitParameters();
-  void RefreshModel();
-
-  void VerifyKimCompatibility();
-
   /// (Re)allocate storage for forces, energies and intermediate results.
   virtual void Allocate();
 
   /// Calculate stuff
-  virtual void Calculate(PyObject *pyatoms);
+  virtual void Calculate(PyObject *pyatoms, bool calc_energy, bool calc_force);
   virtual void DoCalculate();
 
+  /// Set orthocell from atoms cell, and check orthogonality of the latter.
+  void SetOrthoCell();
+
 private:
-  KIM::Model *model;           ///< The KIM Model object
-  KIM::ComputeArguments *computeargs;   
+  KIM_API_model *model;
   bool model_initialized;
-  const char *kimname;         ///< Name of the OpenKIM model.
-  int numberOfNeighborLists;
-  vector<NeighborLocator *> nblists;     ///< The neighborlist object.
-  vector<PyObject *> nblist_objs;
-  int masternblist;      // Which one is the longest
-  vector<bool> independentlist;   ///< Marks the lists that are unique.
-  NeighborListData nblistdata;
+  NeighborLocator *nblist;     ///< The neighborlist object.
+  PyObject *nblist_obj;
   double driftfactor;             ///< Drift factor for the neighbor list.
-  double influenceDistance;  ///< The model's influence distance
-  vector<double> cutoffs;             //< The model's neighborlist cutoff, smaller or equal to the influence distance.
-  vector<int> paddingNeighborHints;
 
   int nAtoms;      ///< Number of particles without ghost atoms
   int nSize;       ///< Number of particles with ghost atoms
   int nAtomsAlloc, nSizeAlloc;  ///< Values of nAtoms and nSize at last allocation.
   bool ghostatoms;          ///< True if atoms have ghosts.
+  int nSpecies;
+  double cutoff;      // The cutoff, will be set by OpenKIM model.
   vector<int> species;
-  vector<int> particleContributing;
   vector<Vec> forces;
   vector<double> particleEnergy;
   vector<SymTensor> particleVirial;
   double energy;
   SymTensor virial;
 
+  nblisttype_t nblisttype;
+  bool nblist_half;
 #if 0
   int nb_accessmode;
 #endif
   vector<int> nb_buffer_n;
   vector<Vec> nb_buffer_rij;
   vector<double> nb_buffer_dist;
+  double orthocell[3];       // Cell size for MI_OPBC boundary conditions.
   int nblist_iterator;       // Next neighbor (used in iterator mode).
 
   std::map<asap_z_int,int> z_to_typecode;  // Translation of atomic number to KIM typecode.
 
   struct {
     bool energy;
     bool particleEnergy;
     bool forces;
     bool virial;
     bool particleVirial;
-  } support;
-  int support_n;  // Counts that they have all been set.
+  } pls_alloc;
+  int pls_alloc_n;  // Counts that they have all been set.
 
   /// A structure of counters to check if recalculations are necessary.
   struct {
     int nblist;
-    int compute;
+    int compute_energy;
+    int compute_force;
   } counters;
 
   /// A structure of bools, to remember if recalculations are necessary.
   struct {
     int nblist;
-    int compute;
+    int compute_energy;
+    int compute_force;
   } recalc;
 
 };
 
 } // namespace
```

### Comparing `asap3-3.13.1/OpenKIMimport/OpenKIMinterface.h` & `asap3-3.9.6/OpenKIMimport/OpenKIMinfo.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// OpenKIMinterface.cpp - Python interface to OpenKIM models.
+// OpenKIMInfo.h - a class to collect information about OpenKIM models.
 //
-// This file is part of the optional Asap module to support OpenKIM
-// models.  Defines the Python interface to the modules in the
-// other files in OpenKIMimport.
+// This class is part of the optional Asap module to support OpenKIM
+// models.  The class OpenKIMInfo collects information about a given
+// OpenKIM model, so it can be opened using the best neighbor list etc.
 
 // Copyright (C) 2014 Jakob Schiotz and Center for Individual
 // Nanoparticle Functionality, Department of Physics, Technical
 // University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
 // Asap is released under the GNU Lesser Public License (LGPL) version 3.
@@ -27,26 +27,66 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-
-#ifndef _OPENKIMINTERFACE_H
-#define _OPENKIMINTERFACE_H
+#ifndef _OPENKIMINFO_H
+#define _OPENKIMINFO_H
 
 #include "AsapPython.h"
-#include "Asap.h"
+#include "AsapNamespace.h"
+#include "AsapObject.h"
+#include <string>
+#include <vector>
+
+class KIM_API_model;
 
 namespace ASAPSPACE {
 
-extern char OpenKIMcalculator_Docstring[];
+class OpenKIMinfo;  // Defined later in this file.
+
+/// The Python object corresponding to a OpenKIMinfo object.
+typedef struct {
+  PyObject_HEAD
+  OpenKIMinfo *cobj;
+  PyObject *weakrefs;
+} PyAsap_OpenKIMinfoObject;
+
+PyAsap_OpenKIMinfoObject *PyAsap_NewOpenKIMinfoObject(const char *name);
+
+class OpenKIMinfo : public AsapObject
+{
+protected:
+  OpenKIMinfo(const char *name);
+
+  friend PyAsap_OpenKIMinfoObject *PyAsap_NewOpenKIMinfoObject(const char *name);
+
+public:
+  ~OpenKIMinfo();
+
+  virtual std::string GetName() const {return "OpenKIMinfo";}
+
+  /// Get information about supported elements.
+  void GetSupportedSymbols(std::vector<const char *> &symbols);
+
+  /// Get information about supported NBC methods.
+  const std::vector<const char *> &GetSupportedNBC();
+
+  /// Get information about supported neighbor access methods.
+  const std::vector<const char *> &GetSupportedAccess();
 
-PyObject *PyAsap_NewOpenKIMcalculator(PyObject *noself, PyObject *args,
-                                      PyObject *kwargs);
+  /// Check if a property exists.  Return index >= 0 if it exists, -1 if not.
+  int GetAPIindex(const char *name);
 
-int PyAsap_InitOpenKIMInterface(PyObject *module);
+private:
+  const char* name;
+  KIM_API_model *model;
+  char *particletypes;
+  std::vector<const char *> supported_nbc;
+  std::vector<const char *> supported_access;
+};
 
-} // end namespace
+} // End namespace
 
-#endif // _OPENKIMINTERFACE_H
+#endif // _OPENKIMINFO_H
```

### Comparing `asap3-3.13.1/PKG-INFO` & `asap3-3.9.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: asap3
-Version: 3.13.1
+Version: 3.9.6
 Summary: ASAP - classical potentials for MD with ASE.
 Home-page: https://wiki.fysik.dtu.dk/asap
-Maintainer: Jakob Schiotz et. al.
-Maintainer-email: schiotz@fysik.dtu.dk
+Author: Jakob Schiotz et. al.
+Author-email: schiotz@fysik.dtu.dk
 License: LGPLv3
+Description: ASAP (Atomic SimulAtion Program or As Soon As Possible) is a
+        package for large-scale molecular dynamics within the Atomic
+        Simulation Environment (ASE).  It implements a number of 'classical'
+        potentials, most importantly the Effective Medium Theory, and also the
+        mechanisms for domain-decomposition of the atoms.
 Platform: unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: COPYING
-License-File: COPYING.LESSER
-
-ASAP (Atomic SimulAtion Program or As Soon As Possible) is a
-package for large-scale molecular dynamics within the Atomic
-Simulation Environment (ASE).  It implements a number of 'classical'
-potentials, most importantly the Effective Medium Theory, and also the
-mechanisms for domain-decomposition of the atoms.
```

### Comparing `asap3-3.13.1/PTM/alloy_types.cpp` & `asap3-3.9.6/PTM/alloy_types.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-//#include <cstdint>
-#include "cpp11compat.h"
-#include "ptm_constants.h"
-
+#include "index_ptm.h"
 
 int32_t find_fcc_alloy_type(int8_t* mapping, int32_t* numbers)
 {
-	int len = PTM_NUM_POINTS_FCC;
-	int8_t temp[PTM_NUM_POINTS_FCC];
+	int len = 13;
+	int8_t temp[13];
 
 	int num_cu = 1, cu = numbers[0];
 	for (int i=1;i<len;i++)
 		if (numbers[i] == cu)
 			num_cu++;
 	if (num_cu == len)
 		return PTM_ALLOY_PURE;
@@ -68,16 +65,16 @@
 	}
 
 	return PTM_ALLOY_NONE;
 }
 
 int32_t find_bcc_alloy_type(int8_t* mapping, int32_t* numbers)
 {
-	int len = PTM_NUM_POINTS_BCC;
-	int8_t temp[PTM_NUM_POINTS_BCC];
+	int len = 15;
+	int8_t temp[15];
 
 	int num_cu = 1, cu = numbers[0];
 	for (int i=1;i<len;i++)
 		if (numbers[i] == cu)
 			num_cu++;
 	if (num_cu == len)
 		return PTM_ALLOY_PURE;
@@ -98,15 +95,16 @@
 			else if (temp[i] == au)
 			{
 				num_au_inner++;
 			}
 		}
 	}
 
-	for (int i=8;i<len-1;i++)
+
+	for (int i=8;i<14;i++)
 		if (temp[i] == cu)
 			num_cu_outer++;
 
 	if (num_au_inner == 8 && num_cu_outer == 6)
 		return PTM_ALLOY_B2;
 
 	return PTM_ALLOY_NONE;
```

### Comparing `asap3-3.13.1/PTM/canonical.cpp` & `asap3-3.9.6/PTM/canonical.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #include <string.h>
-#include "cpp11compat.h"
-//#include <cstdint>
-//#include <cstdbool>
-#include <algorithm>
-#include "ptm_constants.h"
+//#include <cassert>
+#include <cstdint>
+#include <cstdbool>
+#include "index_ptm.h"
 
+#define MIN(X, Y) (((X) < (Y)) ? (X) : (Y))
+#define MAX(X, Y) (((X) > (Y)) ? (X) : (Y))
 
-#define MAXE (3 * PTM_MAX_NBRS - 6)
+#define MAXV 14
+#define MAXE 36
 
-static bool build_facet_map(int num_facets, int8_t facets[][3], int8_t common[PTM_MAX_NBRS][PTM_MAX_NBRS])
+static bool build_facet_map(int num_facets, int8_t facets[][3], int8_t common[MAXV][MAXV])
 {
-	memset(common, -1, sizeof(int8_t) * PTM_MAX_NBRS * PTM_MAX_NBRS);
+	memset(common, -1, sizeof(int8_t) * MAXV * MAXV);
 
 	for (int i = 0;i<num_facets;i++)
 	{
 		int a = facets[i][0];
 		int b = facets[i][1];
 		int c = facets[i][2];
 
@@ -28,21 +30,21 @@
 		common[b][c] = a;
 		common[c][a] = b;
 	}
 
 	return true;
 }
 
-static bool weinberg(int num_nodes, int num_edges, int8_t common[PTM_MAX_NBRS][PTM_MAX_NBRS], int8_t* best_code, int8_t* canonical_labelling, int prev, int cur)
+static bool weinberg(int num_nodes, int num_edges, int8_t common[MAXV][MAXV], int8_t* best_code, int8_t* canonical_labelling, int prev, int cur)
 {
-	bool m[PTM_MAX_NBRS][PTM_MAX_NBRS];
-	memset(m, 0, sizeof(bool) * PTM_MAX_NBRS * PTM_MAX_NBRS);
+	bool m[MAXV][MAXV];
+	memset(m, 0, sizeof(bool) * MAXV * MAXV);
 
-	int8_t index[PTM_MAX_NBRS];
-	memset(index, -1, sizeof(int8_t) * PTM_MAX_NBRS);
+	int8_t index[MAXV];
+	memset(index, -1, sizeof(int8_t) * MAXV);
 	index[prev] = 0;
 	int n = 1;
 
 	bool winning = false;
 	int next = -1;
 	for (int it=1;it<2*num_edges;it++)
 	{
@@ -84,15 +86,15 @@
 	}
 
 	return false;
 }
 
 int canonical_form(int num_facets, int8_t facets[][3], int num_nodes, int8_t* degree, int8_t* canonical_labelling, uint64_t* p_hash)
 {
-	int8_t common[PTM_MAX_NBRS][PTM_MAX_NBRS] = {{0}};
+	int8_t common[MAXV][MAXV] = {{0}};
 	int num_edges = 3 * num_facets / 2;
 	if (!build_facet_map(num_facets, facets, common))
 		return -1;
 
 	int8_t best_code[2 * MAXE] = {0};
 	memset(best_code, 126, sizeof(int8_t) * 2 * num_edges);
 	best_code[0] = 0;
@@ -115,17 +117,17 @@
 			int b = facets[i][1];
 			int c = facets[i][2];
 
 			int da = degree[a];
 			int db = degree[b];
 			int dc = degree[c];
 
-			best_degree = std::max(best_degree, ((uint32_t)da << 16) | ((uint32_t)db << 8) | ((uint32_t)dc << 0));
-			best_degree = std::max(best_degree, ((uint32_t)da << 0) | ((uint32_t)db << 16) | ((uint32_t)dc << 8));
-			best_degree = std::max(best_degree, ((uint32_t)da << 8) | ((uint32_t)db << 0) | ((uint32_t)dc << 16));
+			best_degree = MAX(best_degree, ((uint32_t)da << 16) | ((uint32_t)db << 8) | ((uint32_t)dc << 0));
+			best_degree = MAX(best_degree, ((uint32_t)da << 0) | ((uint32_t)db << 16) | ((uint32_t)dc << 8));
+			best_degree = MAX(best_degree, ((uint32_t)da << 8) | ((uint32_t)db << 0) | ((uint32_t)dc << 16));
 		}
 
 		for (int i = 0;i<num_facets;i++)
 		{
 			int a = facets[i][0];
 			int b = facets[i][1];
 			int c = facets[i][2];
@@ -159,29 +161,7 @@
 		hash ^= e;
 	}
 
 	*p_hash = hash;
 	return PTM_NO_ERROR;
 }
 
-int graph_degree(int num_facets, int8_t facets[][3], int num_nodes, int8_t* degree)
-{
-	memset(degree, 0, sizeof(int8_t) * num_nodes);
-
-	for (int i = 0;i<num_facets;i++)
-	{
-		int a = facets[i][0];
-		int b = facets[i][1];
-		int c = facets[i][2];
-
-		degree[a]++;
-		degree[b]++;
-		degree[c]++;
-	}
-
-	int8_t max_degree = 0;
-	for (int i = 0;i<num_nodes;i++)
-		max_degree = std::max(max_degree, degree[i]);
-
-	return max_degree;
-}
-
```

### Comparing `asap3-3.13.1/PTM/convex_hull_incremental.cpp` & `asap3-3.9.6/PTM/convex_hull_incremental.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-#include "cpp11compat.h"
 #include <cmath>
 #include <cfloat>
 #include <string.h>
 #include <cassert>
-//#include <cstdint>
-//#include <cstdbool>
-#include <algorithm>
+#include <cstdint>
+#include <cstdbool>
 #include "convex_hull_incremental.hpp"
-#include "ptm_constants.h"
 
 
+#define MIN(X, Y) (((X) < (Y)) ? (X) : (Y))
+#define MAX(X, Y) (((X) > (Y)) ? (X) : (Y))
+
 #define VISIBLE 1
 #define INVISIBLE 2
 #define BOTH 3
 #define TOLERANCE 1E-8
 
 static double norm_squared(double* p)
 {
@@ -213,15 +213,15 @@
 		facet[1] = b;
 		facet[2] = c;
 	}
 }
 
 static int initialize_convex_hull(int num_points, const double (*points)[3], int8_t facets[][3], double plane_normal[][3], bool* processed, int* initial_vertices, double* barycentre)
 {
-	memset(processed, 0, PTM_MAX_POINTS * sizeof(bool));
+	memset(processed, 0, 15 * sizeof(bool));
 	memset(barycentre, 0, 3 * sizeof(double));
 	int ret = initial_simplex(num_points, points, initial_vertices);
 	if (ret != 0)
 		return ret;
 
 	for (int i = 0;i<4;i++)
 	{
@@ -241,19 +241,15 @@
 	add_facet(points, initial_vertices[0], initial_vertices[2], initial_vertices[3], facets[2], plane_normal[2], barycentre);
 	add_facet(points, initial_vertices[1], initial_vertices[2], initial_vertices[3], facets[3], plane_normal[3], barycentre);
 	return 0;
 }
 
 int get_convex_hull(int num_points, const double (*points)[3], int num_expected_facets, convexhull_t* ch, int8_t simplex[][3])
 {
-	assert(	num_points == PTM_NUM_POINTS_FCC
-		|| num_points == PTM_NUM_POINTS_HCP
-		|| num_points == PTM_NUM_POINTS_BCC
-		|| num_points == PTM_NUM_POINTS_ICO
-		|| num_points == PTM_NUM_POINTS_SC);
+	assert(num_points == 7 || num_points == 13 || num_points == 15);
 
 	int ret = 0;
 	int num_prev = ch->num_prev;
 	ch->num_prev = num_points;
 	if (!ch->ok || 0)
 	{
 		ret = initialize_convex_hull(num_points, points, ch->facets, ch->plane_normal, ch->processed, ch->initial_vertices, ch->barycentre);
@@ -268,16 +264,16 @@
 	{
 		if (ch->processed[i])
 			continue;
 		ch->processed[i] = true;
 
 		int num_to_add = 0;
 		int8_t to_add[MAXF][3];
-		int8_t edge_visible[PTM_MAX_POINTS][PTM_MAX_POINTS];
-		memset(edge_visible, 0, sizeof(int8_t) * PTM_MAX_POINTS * PTM_MAX_POINTS);
+		int8_t edge_visible[15][15];
+		memset(edge_visible, 0, sizeof(int8_t) * 15 * 15);
 		for (int j = 0;j<ch->num_facets;j++)
 		{
 			int a = ch->facets[j][0];
 			int b = ch->facets[j][1];
 			int c = ch->facets[j][2];
 
 			int u = 0, v = 0, w = 0;
```

### Comparing `asap3-3.13.1/PTM/deformation_gradient.hpp` & `asap3-3.9.6/PTM/deformation_gradient.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-#ifndef DEFORMATION_GRADIENT_HPP
-#define DEFORMATION_GRADIENT_HPP
+#include <cstdint>
+#include "deformation_gradient.hpp"
 
-//#include <cstdint>
-#include "cpp11compat.h"
-#include "ptm_constants.h"
-
-void calculate_deformation_gradient(int num_points, const double (*ideal_points)[3], int8_t* mapping, double (*normalized)[3], const double (*penrose)[3], double* F, double* res);
 
 //sc
 #define k_sc 0.5
-const double penrose_sc[PTM_NUM_POINTS_SC][3] = {	
+const double penrose_sc[7][3] = {	
 					{0, 0, 0},
 					{0, 0, -k_sc},
 					{0, 0, k_sc},
 					{0, -k_sc, 0},
 					{0, k_sc, 0},
 					{-k_sc, 0, 0},
 					{k_sc, 0, 0},
 				};
 
 //fcc
 #define k_fcc 0.17677669529663678216
-const double penrose_fcc[PTM_NUM_POINTS_FCC][3] = {
+const double penrose_fcc[13][3] = {
 					{0, 0, 0},
 					{0, k_fcc, k_fcc},
 					{0, -k_fcc, -k_fcc},
 					{0, k_fcc, -k_fcc},
 					{0, -k_fcc, k_fcc},
 					{k_fcc, 0, k_fcc},
 					{-k_fcc, 0, -k_fcc},
@@ -35,15 +30,15 @@
 					{-k_fcc, -k_fcc, 0},
 					{k_fcc, -k_fcc, 0},
 					{-k_fcc, k_fcc, -0},
 				};
 
 //hcp
 #define k_hcp 0.17677669529663678216
-const double penrose_hcp[PTM_NUM_POINTS_HCP][3] = {
+const double penrose_hcp[13][3] = {
 					{0, 0, 0},
 					{k_hcp, 0, k_hcp},
 					{-k_hcp/3, -4*k_hcp/3, -k_hcp/3},
 					{k_hcp, k_hcp, 0},
 					{-k_hcp/3, -k_hcp/3, -4*k_hcp/3},
 					{0, k_hcp, k_hcp},
 					{-4*k_hcp/3, -k_hcp/3, -k_hcp/3},
@@ -55,15 +50,15 @@
 					{0, -k_hcp, k_hcp},
 				};
 
 //ico
 #define k_ico 0.13143277802974323576
 #define phi 1.61803398874989490253
 //((1.0 + sqrt(5)) / 2)
-const double penrose_ico[PTM_NUM_POINTS_ICO][3] = {
+const double penrose_ico[13][3] = {
 					{0, 0, 0},
 					{0, k_ico, phi*k_ico},
 					{0, -k_ico, -phi*k_ico},
 					{0, k_ico, -phi*k_ico},
 					{0, -k_ico, phi*k_ico},
 					{-k_ico, -phi*k_ico, -0},
 					{k_ico, phi*k_ico, 0},
@@ -73,15 +68,15 @@
 					{phi*k_ico, 0, k_ico},
 					{phi*k_ico, 0, -k_ico},
 					{-phi*k_ico, 0, k_ico},
 				};
 
 //bcc
 #define k_bcc 0.11543038598460284017
-const double penrose_bcc[PTM_NUM_POINTS_BCC][3] = {
+const double penrose_bcc[15][3] = {
 					{0, 0, 0},
 					{-k_bcc, -k_bcc, -k_bcc},
 					{k_bcc, k_bcc, k_bcc},
 					{k_bcc, -k_bcc, -k_bcc},
 					{-k_bcc, k_bcc, k_bcc},
 					{-k_bcc, k_bcc, -k_bcc},
 					{k_bcc, -k_bcc, k_bcc},
@@ -90,9 +85,42 @@
 					{0, 0, -2*k_bcc},
 					{0, 0, 2*k_bcc},
 					{0, -2*k_bcc, 0},
 					{0, 2*k_bcc, 0},
 					{-2*k_bcc, 0, 0},
 					{2*k_bcc, 0, -0},
 				};
-#endif
+
+void calculate_deformation_gradient(int num_points, const double (*ideal_points)[3], int8_t* mapping, double (*normalized)[3], const double (*penrose)[3], double* F, double* res)
+{
+	for (int i = 0;i<3;i++)
+	{
+		for (int j = 0;j<3;j++)
+		{
+			double acc = 0.0;
+			for (int k = 0;k<num_points;k++)
+				acc += penrose[k][j] * normalized[mapping[k]][i];
+
+			F[i*3 + j] = acc;
+		}
+	}
+
+	res[0] = 0;
+	res[1] = 0;
+	res[2] = 0;
+
+	for (int k = 0;k<num_points;k++)
+	{
+		for (int i = 0;i<3;i++)
+		{
+			double acc = 0.0;
+			for (int j = 0;j<3;j++)
+			{
+				acc += F[i*3 + j] * ideal_points[k][j];
+			}
+
+			double delta = acc - normalized[mapping[k]][i];
+			res[i] += delta * delta;
+		}
+	}
+}
```

### Comparing `asap3-3.13.1/PTM/fundamental_mappings.hpp` & `asap3-3.9.6/PTM/fundamental_mappings.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #ifndef FUNDAMENTAL_MAPPINGS_HPP
 #define FUNDAMENTAL_MAPPINGS_HPP
 
-//#include <cstdint>
-#include "cpp11compat.h"
+#include <cstdint>
 
-const int8_t mapping_sc[24][PTM_MAX_POINTS] = {
-					{0, 1, 2, 3, 4, 5, 6},
+const int8_t mapping_sc[24][15] = {	{0, 1, 2, 3, 4, 5, 6},
 					{0, 2, 1, 4, 3, 5, 6},
 					{0, 2, 1, 3, 4, 6, 5},
 					{0, 1, 2, 4, 3, 6, 5},
 					{0, 3, 4, 5, 6, 1, 2},
 					{0, 5, 6, 2, 1, 4, 3},
 					{0, 6, 5, 1, 2, 4, 3},
 					{0, 4, 3, 5, 6, 2, 1},
@@ -26,16 +24,15 @@
 					{0, 2, 1, 5, 6, 3, 4},
 					{0, 5, 6, 4, 3, 1, 2},
 					{0, 3, 4, 1, 2, 6, 5},
 					{0, 2, 1, 6, 5, 4, 3},
 					{0, 6, 5, 4, 3, 2, 1},
 					{0, 4, 3, 2, 1, 6, 5}	};
 
-const int8_t mapping_fcc[24][PTM_MAX_POINTS] = {
-					{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12},
+const int8_t mapping_fcc[24][15] = {	{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12},
 					{0, 2, 1, 4, 3, 7, 8, 5, 6, 11, 12, 9, 10},
 					{0, 3, 4, 1, 2, 6, 5, 8, 7, 12, 11, 10, 9},
 					{0, 4, 3, 2, 1, 8, 7, 6, 5, 10, 9, 12, 11},
 					{0, 9, 10, 11, 12, 1, 2, 4, 3, 5, 6, 8, 7},
 					{0, 7, 8, 6, 5, 11, 12, 10, 9, 2, 1, 4, 3},
 					{0, 8, 7, 5, 6, 10, 9, 11, 12, 4, 3, 2, 1},
 					{0, 11, 12, 9, 10, 2, 1, 3, 4, 7, 8, 6, 5},
@@ -52,16 +49,15 @@
 					{0, 7, 8, 5, 6, 3, 4, 1, 2, 9, 10, 12, 11},
 					{0, 11, 12, 10, 9, 5, 6, 8, 7, 4, 3, 1, 2},
 					{0, 1, 2, 4, 3, 12, 11, 10, 9, 8, 7, 6, 5},
 					{0, 6, 5, 8, 7, 2, 1, 4, 3, 10, 9, 11, 12},
 					{0, 10, 9, 11, 12, 6, 5, 7, 8, 2, 1, 3, 4},
 					{0, 2, 1, 3, 4, 10, 9, 12, 11, 6, 5, 8, 7}	};
 
-const int8_t mapping_bcc[24][PTM_MAX_POINTS] = {
-					{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14},
+const int8_t mapping_bcc[24][15] = {	{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14},
 					{0, 4, 3, 2, 1, 7, 8, 5, 6, 10, 9, 12, 11, 13, 14},
 					{0, 6, 5, 7, 8, 2, 1, 3, 4, 10, 9, 11, 12, 14, 13},
 					{0, 8, 7, 5, 6, 3, 4, 2, 1, 9, 10, 12, 11, 14, 13},
 					{0, 1, 2, 7, 8, 3, 4, 5, 6, 11, 12, 13, 14, 9, 10},
 					{0, 4, 3, 7, 8, 5, 6, 2, 1, 13, 14, 10, 9, 12, 11},
 					{0, 8, 7, 3, 4, 2, 1, 5, 6, 14, 13, 9, 10, 12, 11},
 					{0, 4, 3, 5, 6, 2, 1, 7, 8, 12, 11, 13, 14, 10, 9},
@@ -78,16 +74,15 @@
 					{0, 7, 8, 4, 3, 6, 5, 1, 2, 10, 9, 13, 14, 11, 12},
 					{0, 5, 6, 4, 3, 1, 2, 8, 7, 13, 14, 12, 11, 9, 10},
 					{0, 3, 4, 1, 2, 6, 5, 8, 7, 11, 12, 9, 10, 14, 13},
 					{0, 2, 1, 6, 5, 4, 3, 8, 7, 10, 9, 14, 13, 12, 11},
 					{0, 2, 1, 8, 7, 6, 5, 4, 3, 14, 13, 12, 11, 10, 9},
 					{0, 2, 1, 4, 3, 8, 7, 6, 5, 12, 11, 10, 9, 14, 13}	};
 
-const int8_t mapping_ico[60][PTM_MAX_POINTS] = {
-					{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12},
+const int8_t mapping_ico[60][15] = {	{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12},
 					{0, 10, 9, 8, 7, 5, 6, 2, 1, 12, 11, 3, 4},
 					{0, 1, 2, 9, 10, 7, 8, 11, 12, 5, 6, 3, 4},
 					{0, 4, 3, 8, 7, 2, 1, 11, 12, 9, 10, 6, 5},
 					{0, 6, 5, 9, 10, 4, 3, 7, 8, 12, 11, 2, 1},
 					{0, 12, 11, 3, 4, 7, 8, 10, 9, 2, 1, 6, 5},
 					{0, 4, 3, 6, 5, 9, 10, 2, 1, 8, 7, 11, 12},
 					{0, 8, 7, 2, 1, 4, 3, 10, 9, 5, 6, 11, 12},
@@ -140,16 +135,15 @@
 					{0, 2, 1, 8, 7, 10, 9, 4, 3, 6, 5, 12, 11},
 					{0, 8, 7, 4, 3, 11, 12, 2, 1, 10, 9, 5, 6},
 					{0, 6, 5, 4, 3, 2, 1, 9, 10, 7, 8, 12, 11},
 					{0, 2, 1, 6, 5, 4, 3, 12, 11, 10, 9, 8, 7},
 					{0, 3, 4, 1, 2, 7, 8, 5, 6, 10, 9, 12, 11},
 					{0, 4, 3, 2, 1, 6, 5, 8, 7, 11, 12, 9, 10}	};
 
-const int8_t mapping_hcp[6][PTM_MAX_POINTS] = {
-					{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12},
+const int8_t mapping_hcp[6][15] = {	{0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12},
 					{0, 5, 6, 1, 2, 3, 4, 9, 10, 12, 11, 8, 7},
 					{0, 3, 4, 5, 6, 1, 2, 12, 11, 7, 8, 10, 9},
 					{0, 4, 3, 2, 1, 6, 5, 11, 12, 10, 9, 7, 8},
 					{0, 2, 1, 6, 5, 4, 3, 8, 7, 11, 12, 9, 10},
 					{0, 6, 5, 4, 3, 2, 1, 10, 9, 8, 7, 12, 11}	};
 
 #endif
```

### Comparing `asap3-3.13.1/PTM/graph_data.cpp` & `asap3-3.9.6/PTM/graph_data.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #include "graph_data.hpp"
 
 
-int8_t automorphisms[53][PTM_MAX_POINTS] = {
+int8_t automorphisms[53][15] = {
 	{  0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, 13, 14},
 	{  0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, -1, -1},
 	{  0,  4,  3, 10,  9,  5,  6, 12, 11,  8,  7,  1,  2, -1, -1},
 	{  0,  5,  6, 11, 12,  8,  7,  2,  1,  4,  3, 10,  9, -1, -1},
 	{  0,  8,  7,  1,  2,  4,  3,  9, 10,  5,  6, 11, 12, -1, -1},
 	{  0,  8,  7, 10,  9,  1,  2,  6,  5, 12, 11,  3,  4, -1, -1},
 	{  0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, -1, -1},
```

### Comparing `asap3-3.13.1/PTM/graph_data.hpp` & `asap3-3.9.6/PTM/graph_data.hpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 #ifndef GRAPH_DATA_HPP
 #define GRAPH_DATA_HPP
 
-//#include <cstdint>
-#include "cpp11compat.h"
-#include "ptm_constants.h"
-
+#include <cstdint>
 
 typedef struct
 {
 	int id;
 	uint64_t hash;
 	int automorphism_index;
 	int num_automorphisms;
-	int8_t canonical_labelling[PTM_MAX_POINTS];
-	int8_t facets[PTM_MAX_FACETS][3];
+	int8_t canonical_labelling[15];
+	int8_t facets[24][3];
 } graph_t;
 
 #define NUM_SC_GRAPHS 1
 #define NUM_ICO_GRAPHS 1
 #define NUM_FCC_GRAPHS 8
 #define NUM_HCP_GRAPHS 16
 #define NUM_BCC_GRAPHS 218
 
-extern int8_t automorphisms[][PTM_MAX_POINTS];
+extern int8_t automorphisms[][15];
 
 extern graph_t graphs_sc[NUM_SC_GRAPHS];
 extern graph_t graphs_fcc[NUM_FCC_GRAPHS];
 extern graph_t graphs_hcp[NUM_HCP_GRAPHS];
 extern graph_t graphs_ico[NUM_ICO_GRAPHS];
 extern graph_t graphs_bcc[NUM_BCC_GRAPHS];
```

### Comparing `asap3-3.13.1/PTM/index_ptm.h` & `asap3-3.9.6/PTM/index_ptm.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/PTM/neighbour_ordering.cpp` & `asap3-3.9.6/PTM/neighbour_ordering.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #include <cstdlib>
 #include <cmath>
 #include <cstring>
 #include <cassert>
 #include <algorithm>
-#include "ptm_constants.h"
 #include "voronoi/cell.hpp"
 using namespace voro;
+using namespace std;
 
+#define MAX_POINTS 19
 
 
 typedef struct
 {
 	double area;
 	double dist;
 	int index;
@@ -27,17 +28,17 @@
 	if (a.dist < b.dist)
 		return true;
 
 	return false;
 }
 
 //todo: change voronoi code to return errors rather than exiting
-static int calculate_voronoi_face_areas(int num_points, const double (*_points)[3], double* normsq, double max_norm, voronoicell_neighbor* v, std::vector<int>& nbr_indices, std::vector<double>& face_areas)
+static int calculate_voronoi_face_areas(int num_points, const double (*_points)[3], double* normsq, double max_norm, voronoicell_neighbor* v, vector<int>& nbr_indices, vector<double>& face_areas)
 {
-	const double k = 1000 * max_norm;	//todo: reduce this constant
+	const double k = 1000 * max_norm;
 	v->init(-k,k,-k,k,-k,k);
 
 	for (int i=1;i<num_points;i++)
 	{
 		double x = _points[i][0] - _points[0][0];
 		double y = _points[i][1] - _points[0][1];
 		double z = _points[i][2] - _points[0][2];
@@ -47,64 +48,65 @@
 	v->neighbors(nbr_indices);
 	v->face_areas(face_areas);
 	return 0;
 }
 
 int calculate_neighbour_ordering(void* _voronoi_handle, int num_points, const double (*_points)[3], int8_t* ordering)
 {
-	assert(num_points <= PTM_MAX_INPUT_POINTS);
+	assert(num_points <= MAX_POINTS);
 
 	voronoicell_neighbor* voronoi_handle = (voronoicell_neighbor*)_voronoi_handle;
 
 	double max_norm = 0;
-	double points[PTM_MAX_INPUT_POINTS][3];
-	double normsq[PTM_MAX_INPUT_POINTS];
+	double points[MAX_POINTS][3];
+	double normsq[MAX_POINTS];
 	for (int i = 0;i<num_points;i++)
 	{
 		double x = _points[i][0] - _points[0][0];
 		double y = _points[i][1] - _points[0][1];
 		double z = _points[i][2] - _points[0][2];
 		points[i][0] = x;
 		points[i][1] = y;
 		points[i][2] = z;
 
 		normsq[i] = x*x + y*y + z*z;
-		max_norm = std::max(max_norm, normsq[i]);
+		max_norm = max(max_norm, normsq[i]);
 #ifdef DEBUG
 		printf("point %d: %f\t%f\t%f\t%f\n", i, x, y, z, x*x + y*y + z*z);
 #endif
 	}
 
 	max_norm = sqrt(max_norm);
 
-	std::vector<int> nbr_indices(num_points + 6);
-	std::vector<double> face_areas(num_points + 6);
+	vector<int> nbr_indices(num_points+6);
+	vector<double> face_areas(num_points+6);
 	int ret = calculate_voronoi_face_areas(num_points, points, normsq, max_norm, voronoi_handle, nbr_indices, face_areas);
 	if (ret != 0)
 		return ret;
 
-	double areas[PTM_MAX_INPUT_POINTS];
+	double areas[MAX_POINTS];
 	memset(areas, 0, num_points * sizeof(double));
 	areas[0] = INFINITY;
 	for (size_t i=0;i<nbr_indices.size();i++)
 	{
 		int index = nbr_indices[i];
 		if (index > 0)
 			areas[index] = face_areas[i];
 	}
 
-	sorthelper_t data[PTM_MAX_INPUT_POINTS];
+	sorthelper_t data[MAX_POINTS];
 	for (int i=0;i<num_points;i++)
 	{
 		assert(areas[i] == areas[i]);
 		data[i].area = areas[i];
 		data[i].dist = normsq[i];
 		data[i].index = i;
 	}
 
+	//qsort(data, num_points, sizeof(sorthelper_t), sorthelper_compare);
 	std::sort(data, data + num_points, &sorthelper_compare);
 
 #ifdef DEBUG
 	for (int i=0;i<num_points;i++)
 		printf("%d %f\n", data[i].index, data[i].area);
 #endif
```

### Comparing `asap3-3.13.1/PTM/normalize_vertices.cpp` & `asap3-3.9.6/PTM/normalize_vertices.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/PTM/qcprot/polar.cpp` & `asap3-3.9.6/PTM/polar_decomposition.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 /*******************************************************************************
  *  -/_|:|_|_\- 
  *
- *  This code is a modification of D.L. Theobald's QCP rotation code.
+ *  This code is a modification of Theobald's QCP rotation code.
  *  It has been adapted to calculate the polar decomposition of a 3x3 matrix
- *  Adaption by P.M. Larsen
+ *  Adaption by PM Larsen
  *
  *  Original Author(s):	  Douglas L. Theobald
  *				  Department of Biochemistry
  *				  MS 009
  *				  Brandeis University
  *				  415 South St
  *				  Waltham, MA  02453
@@ -76,70 +76,79 @@
  *					invalid mem access
  *	2011/02/21	  Made CenterCoords use weights
  *	2011/05/02	  Finally changed CenterCoords declaration in qcprot.h
  *					Also changed some functions to static
  *	2011/07/08	  put in fabs() to fix taking sqrt of small neg numbers, fp error
  *	2012/07/26	  minor changes to comments and main.c, more info (v.1.4)
  *
- *      2016/05/29        QCP method adapted for polar decomposition of a 3x3 matrix,
- *			  for use in Polyhedral Template Matching.
+ *      2016/05/29        QCP method adapted for polar decomposition of a 3x3 matrix.  For use in Polyhedral Template Matching.
  *  
  ******************************************************************************/
 
-//#include <cstdbool>
+#include <cstdbool>
 #include <cmath>
-#include <algorithm>
-#include <cstring>
-#include "quat.hpp"
 
 
-static void matmul_3x3(double* A, double* x, double* b)
+static void matmul(double* A, double* x, double* b)
 {
 	b[0] = A[0] * x[0] + A[1] * x[3] + A[2] * x[6];
 	b[3] = A[3] * x[0] + A[4] * x[3] + A[5] * x[6];
 	b[6] = A[6] * x[0] + A[7] * x[3] + A[8] * x[6];
 
 	b[1] = A[0] * x[1] + A[1] * x[4] + A[2] * x[7];
 	b[4] = A[3] * x[1] + A[4] * x[4] + A[5] * x[7];
 	b[7] = A[6] * x[1] + A[7] * x[4] + A[8] * x[7];
 
 	b[2] = A[0] * x[2] + A[1] * x[5] + A[2] * x[8];
 	b[5] = A[3] * x[2] + A[4] * x[5] + A[5] * x[8];
 	b[8] = A[6] * x[2] + A[7] * x[5] + A[8] * x[8];
 }
 
-static double matrix_determinant_3x3(double* A)
+static void quaternion_to_rotation_matrix(double* q, double* u)
 {
-	return    A[0] * (A[4]*A[8] - A[5]*A[7])
-		- A[1] * (A[3]*A[8] - A[5]*A[6])
-		+ A[2] * (A[3]*A[7] - A[4]*A[6]);
+	double a = q[0];
+	double b = q[1];
+	double c = q[2];
+	double d = q[3];
+
+	u[0] = a*a + b*b - c*c - d*d;
+	u[1] = 2*b*c - 2*a*d;
+	u[2] = 2*b*d + 2*a*c;
+
+	u[3] = 2*b*c + 2*a*d;
+	u[4] = a*a - b*b + c*c - d*d;
+	u[5] = 2*c*d - 2*a*b;
+
+	u[6] = 2*b*d - 2*a*c;
+	u[7] = 2*c*d + 2*a*b;
+	u[8] = a*a - b*b - c*c + d*d;
 }
 
-static void flip_matrix(double* A)
-{
-	for (int i=0;i<9;i++)
-		A[i] = -A[i];
-}
-
-static bool optimal_quaternion(double* A, bool polar, double E0, double* p_nrmsdsq, double* qopt)
+int polar_decomposition_3x3(double* _A, bool right_sided, double* U, double* P)
 {
 	const double evecprec = 1e-6;
 	const double evalprec = 1e-11;
 
+	double A[9] = {_A[0], _A[1], _A[2], _A[3], _A[4], _A[5], _A[6], _A[7], _A[8]};
+	double det = A[0] * (A[4]*A[8] - A[5]*A[7]) - A[1] * (A[3]*A[8] - A[5]*A[6]) + A[2] * (A[3]*A[7] - A[4]*A[6]);
+	if (det < 0)
+	{
+		for (int i=0;i<9;i++)
+			A[i] = -A[i];
+	}
+
 	double	Sxx = A[0], Sxy = A[1], Sxz = A[2],
 		Syx = A[3], Syy = A[4], Syz = A[5],
 		Szx = A[6], Szy = A[7], Szz = A[8];
 
 	double	Sxx2 = Sxx * Sxx, Syy2 = Syy * Syy, Szz2 = Szz * Szz,
 		Sxy2 = Sxy * Sxy, Syz2 = Syz * Syz, Sxz2 = Sxz * Sxz,
 		Syx2 = Syx * Syx, Szy2 = Szy * Szy, Szx2 = Szx * Szx;
 
-	double fnorm_squared = Sxx2 + Syy2 + Szz2 + Sxy2 + Syz2 + Sxz2 + Syx2 + Szy2 + Szx2;
-
-	double SyzSzymSyySzz2 = 2.0 * (Syz * Szy - Syy * Szz);
+	double SyzSzymSyySzz2 = 2.0*(Syz*Szy - Syy*Szz);
 	double Sxx2Syy2Szz2Syz2Szy2 = Syy2 + Szz2 - Sxx2 + Syz2 + Szy2;
 	double SxzpSzx = Sxz + Szx;
 	double SyzpSzy = Syz + Szy;
 	double SxypSyx = Sxy + Syx;
 	double SyzmSzy = Syz - Szy;
 	double SxzmSzx = Sxz - Szx;
 	double SxymSyx = Sxy - Syx;
@@ -152,18 +161,23 @@
 		 + (Sxx2Syy2Szz2Syz2Szy2 + SyzSzymSyySzz2) * (Sxx2Syy2Szz2Syz2Szy2 - SyzSzymSyySzz2)
 		 + (-(SxzpSzx)*(SyzmSzy)+(SxymSyx)*(SxxmSyy-Szz)) * (-(SxzmSzx)*(SyzpSzy)+(SxymSyx)*(SxxmSyy+Szz))
 		 + (-(SxzpSzx)*(SyzpSzy)-(SxypSyx)*(SxxpSyy-Szz)) * (-(SxzmSzx)*(SyzmSzy)-(SxypSyx)*(SxxpSyy+Szz))
 		 + (+(SxypSyx)*(SyzpSzy)+(SxzpSzx)*(SxxmSyy+Szz)) * (-(SxymSyx)*(SyzmSzy)+(SxzpSzx)*(SxxpSyy+Szz))
 		 + (+(SxypSyx)*(SyzmSzy)+(SxzmSzx)*(SxxmSyy-Szz)) * (-(SxymSyx)*(SyzpSzy)+(SxzmSzx)*(SxxpSyy-Szz));
 
 	C[1] = 8.0 * (Sxx*Syz*Szy + Syy*Szx*Sxz + Szz*Sxy*Syx - Sxx*Syy*Szz - Syz*Szx*Sxy - Szy*Syx*Sxz);
-	C[2] = -2.0 * fnorm_squared;
+
+	C[2] = -2.0 * (Sxx2 + Syy2 + Szz2 + Sxy2 + Syx2 + Sxz2 + Szx2 + Syz2 + Szy2);
+
+	double fnorm_squared = 0.0;
+	for (int i=0;i<9;i++)
+		fnorm_squared += A[i]*A[i];
 
 	//Newton-Raphson
-	double mxEigenV = polar ? sqrt(3 * fnorm_squared) : E0;
+	double mxEigenV = sqrt(3 * fnorm_squared);
 	if (mxEigenV > evalprec)
 	{
 		for (int i=0;i<50;i++)
 		{
 			double oldg = mxEigenV;
 			double x2 = mxEigenV*mxEigenV;
 			double b = (x2 + C[2])*mxEigenV;
@@ -175,16 +189,14 @@
 		}
 	}
 	else
 	{
 		mxEigenV = 0.0;
 	}
 
-	(*p_nrmsdsq) = std::max(0.0, 2.0 * (E0 - mxEigenV));
-
 	double a11 = SxxpSyy + Szz - mxEigenV;
 	double a12 = SyzmSzy;
 	double a13 = -SxzmSzx;
 	double a14 = SxymSyx;
 
 	double a21 = SyzmSzy;
 	double a22 = SxxmSyy - Szz  -mxEigenV;
@@ -203,136 +215,94 @@
 
 	double a3344_4334 = a33 * a44 - a43 * a34;
 	double a3244_4234 = a32 * a44 - a42 * a34;
 	double a3243_4233 = a32 * a43 - a42 * a33;
 	double a3143_4133 = a31 * a43 - a41 * a33;
 	double a3144_4134 = a31 * a44 - a41 * a34;
 	double a3142_4132 = a31 * a42 - a41 * a32;
-	double a1324_1423 = a13 * a24 - a14 * a23;
-	double a1224_1422 = a12 * a24 - a14 * a22;
-	double a1223_1322 = a12 * a23 - a13 * a22;
-	double a1124_1421 = a11 * a24 - a14 * a21;
-	double a1123_1321 = a11 * a23 - a13 * a21;
-	double a1122_1221 = a11 * a22 - a12 * a21;
-
-	double q[4][4];
-	q[0][0] =  a12 * a3344_4334 - a13 * a3244_4234 + a14 * a3243_4233;
-	q[0][1] = -a11 * a3344_4334 + a13 * a3144_4134 - a14 * a3143_4133;
-	q[0][2] =  a11 * a3244_4234 - a12 * a3144_4134 + a14 * a3142_4132;
-	q[0][3] = -a11 * a3243_4233 + a12 * a3143_4133 - a13 * a3142_4132;
-
-	q[1][0] =  a22 * a3344_4334 - a23 * a3244_4234 + a24 * a3243_4233;
-	q[1][1] = -a21 * a3344_4334 + a23 * a3144_4134 - a24 * a3143_4133;
-	q[1][2] =  a21 * a3244_4234 - a22 * a3144_4134 + a24 * a3142_4132;
-	q[1][3] = -a21 * a3243_4233 + a22 * a3143_4133 - a23 * a3142_4132;
-
-	q[2][0] =  a32 * a1324_1423 - a33 * a1224_1422 + a34 * a1223_1322;
-	q[2][1] = -a31 * a1324_1423 + a33 * a1124_1421 - a34 * a1123_1321;
-	q[2][2] =  a31 * a1224_1422 - a32 * a1124_1421 + a34 * a1122_1221;
-	q[2][3] = -a31 * a1223_1322 + a32 * a1123_1321 - a33 * a1122_1221;
-
-	q[3][0] =  a42 * a1324_1423 - a43 * a1224_1422 + a44 * a1223_1322;
-	q[3][1] = -a41 * a1324_1423 + a43 * a1124_1421 - a44 * a1123_1321;
-	q[3][2] =  a41 * a1224_1422 - a42 * a1124_1421 + a44 * a1122_1221;
-	q[3][3] = -a41 * a1223_1322 + a42 * a1123_1321 - a43 * a1122_1221;
-
-	double qsqr[4];
-	for (int i=0;i<4;i++)
-		qsqr[i] = q[i][0]*q[i][0] + q[i][1]*q[i][1] + q[i][2]*q[i][2] + q[i][3]*q[i][3];
-
-	int bi = 0;
-	double max = 0;
-	for (int i=0;i<4;i++)
+
+	double q1 =  a22*a3344_4334-a23*a3244_4234+a24*a3243_4233;
+	double q2 = -a21*a3344_4334+a23*a3144_4134-a24*a3143_4133;
+	double q3 =  a21*a3244_4234-a22*a3144_4134+a24*a3142_4132;
+	double q4 = -a21*a3243_4233+a22*a3143_4133-a23*a3142_4132;
+
+	double qsqr = q1 * q1 + q2 * q2 + q3 * q3 + q4 * q4;
+	double q[4];
+
+	bool too_small = false;
+	//The following code tries to calculate another column in the adjoint matrix when the norm of the 
+	//current column is too small.
+	//Usually this block will never be activated.  To be absolutely safe this should be
+	//uncommented, but it is most likely unnecessary.
+	if (qsqr < evecprec)
 	{
-		if (qsqr[i] > max)
+		q1 =  a12*a3344_4334 - a13*a3244_4234 + a14*a3243_4233;
+		q2 = -a11*a3344_4334 + a13*a3144_4134 - a14*a3143_4133;
+		q3 =  a11*a3244_4234 - a12*a3144_4134 + a14*a3142_4132;
+		q4 = -a11*a3243_4233 + a12*a3143_4133 - a13*a3142_4132;
+		qsqr = q1*q1 + q2*q2 + q3*q3 + q4*q4;
+
+		if (qsqr < evecprec)
 		{
-			bi = i;
-			max = qsqr[i];
+			double a1324_1423 = a13 * a24 - a14 * a23, a1224_1422 = a12 * a24 - a14 * a22;
+			double a1223_1322 = a12 * a23 - a13 * a22, a1124_1421 = a11 * a24 - a14 * a21;
+			double a1123_1321 = a11 * a23 - a13 * a21, a1122_1221 = a11 * a22 - a12 * a21;
+
+			q1 =  a42 * a1324_1423 - a43 * a1224_1422 + a44 * a1223_1322;
+			q2 = -a41 * a1324_1423 + a43 * a1124_1421 - a44 * a1123_1321;
+			q3 =  a41 * a1224_1422 - a42 * a1124_1421 + a44 * a1122_1221;
+			q4 = -a41 * a1223_1322 + a42 * a1123_1321 - a43 * a1122_1221;
+			qsqr = q1*q1 + q2*q2 + q3*q3 + q4*q4;
+
+			if (qsqr < evecprec)
+			{
+				q1 =  a32 * a1324_1423 - a33 * a1224_1422 + a34 * a1223_1322;
+				q2 = -a31 * a1324_1423 + a33 * a1124_1421 - a34 * a1123_1321;
+				q3 =  a31 * a1224_1422 - a32 * a1124_1421 + a34 * a1122_1221;
+				q4 = -a31 * a1223_1322 + a32 * a1123_1321 - a33 * a1122_1221;
+				qsqr = q1*q1 + q2*q2 + q3*q3 + q4*q4;
+				
+				if (qsqr < evecprec)
+				{
+					//if qsqr is still too small, return the identity matrix.
+					q[0] = 1.0;
+					q[1] = 0.0;
+					q[2] = 0.0;
+					q[3] = 0.0;
+					U[0] = U[4] = U[8] = 1.0;
+					U[1] = U[2] = U[3] = U[5] = U[6] = U[7] = 0.0;
+					too_small = true;
+				}
+			}
 		}
 	}
 
-	bool too_small = false;
-	if (qsqr[bi] < evecprec)
-	{
-		//if qsqr is still too small, return the identity rotation.
-		q[bi][0] = 1;
-		q[bi][1] = 0;
-		q[bi][2] = 0;
-		q[bi][3] = 0;
-		too_small = true;
-	}
-	else
+	if (!too_small)
 	{
-		double normq = sqrt(qsqr[bi]);
-		q[bi][0] /= normq;
-		q[bi][1] /= normq;
-		q[bi][2] /= normq;
-		q[bi][3] /= normq;
+		double normq = sqrt(qsqr);
+		q1 /= normq;
+		q2 /= normq;
+		q3 /= normq;
+		q4 /= normq;
+		q[0] = -q1;
+		q[1] = q2;
+		q[2] = q3;
+		q[3] = q4;
+		quaternion_to_rotation_matrix(q, U);
 	}
 
-	memcpy(qopt, q[bi], 4 * sizeof(double));
-	return !too_small;
-}
-
-int polar_decomposition_3x3(double* _A, bool right_sided, double* U, double* P)
-{
-	double A[9];
-	memcpy(A, _A, 9 * sizeof(double));
-
-	double det = matrix_determinant_3x3(A);
-	if (det < 0)
-		flip_matrix(A);
-
-	double q[4];
-	double nrmsdsq = 0;
-	optimal_quaternion(A, true, -1, &nrmsdsq, q);
-	q[0] = -q[0];
-	quaternion_to_rotation_matrix(q, U);
-
 	if (det < 0)
-		flip_matrix(U);
+	{
+		for (int i=0;i<9;i++)
+			U[i] = -U[i];
+	}
 
-	double UT[9] = {U[0], U[3], U[6], U[1], U[4], U[7], U[2], U[5], U[8]};
+	double invU[9] = {U[0], U[3], U[6], U[1], U[4], U[7], U[2], U[5], U[8]};
 
 	if (right_sided)
-		matmul_3x3(UT, _A, P);
+		matmul(invU, _A, P);
 	else
-		matmul_3x3(_A, UT, P);
-
-	return 0;
-}
+		matmul(_A, invU, P);
 
-void InnerProduct(double *A, int num, const double (*coords1)[3], double (*coords2)[3], int8_t* permutation)
-{
-	A[0] = A[1] = A[2] = A[3] = A[4] = A[5] = A[6] = A[7] = A[8] = 0.0;
-
-	for (int i = 0; i < num; ++i)
-	{
-		double x1 = coords1[i][0];
-		double y1 = coords1[i][1];
-		double z1 = coords1[i][2];
-
-		double x2 = coords2[permutation[i]][0];
-		double y2 = coords2[permutation[i]][1];
-		double z2 = coords2[permutation[i]][2];
-
-		A[0] += x1 * x2;
-		A[1] += x1 * y2;
-		A[2] += x1 * z2;
-
-		A[3] += y1 * x2;
-		A[4] += y1 * y2;
-		A[5] += y1 * z2;
-
-		A[6] += z1 * x2;
-		A[7] += z1 * y2;
-		A[8] += z1 * z2;  
-	}
-}
-
-int FastCalcRMSDAndRotation(double *A, double E0, double *p_nrmsdsq, double *q, double* U)
-{
-	optimal_quaternion(A, false, E0, p_nrmsdsq, q);
-	quaternion_to_rotation_matrix(q, U);
-	return 0;
+	return !too_small;
 }
```

### Comparing `asap3-3.13.1/PTM/qcprot/quat.cpp` & `asap3-3.9.6/PTM/qcprot/quat.cpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/PTM/qcprot/quat.hpp` & `asap3-3.9.6/PTM/qcprot/quat.hpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/PTM/qcprot.h` & `asap3-3.9.6/PTM/qcprot.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/PTM/voronoi/cell.cpp` & `asap3-3.9.6/PTM/voronoi/cell.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -164,23 +164,21 @@
 void voronoicell_base::add_memory_vorder(vc_class &vc) {
 	int i=(current_vertex_order<<1),j,*p1,**p2;
 	if(i>max_vertex_order) voro_fatal_error("Vertex order memory allocation exceeded absolute maximum",VOROPP_MEMORY_ERROR);
 #if VOROPP_VERBOSE >=2
 	fprintf(stderr,"Vertex order memory scaled up to %d\n",i);
 #endif
 	p1=new int[i];
-	for(j=0;j<current_vertex_order;j++) p1[j]=mem[j];
-	while(j<i) p1[j++]=0;
+	for(j=0;j<current_vertex_order;j++) p1[j]=mem[j];while(j<i) p1[j++]=0;
 	delete [] mem;mem=p1;
 	p2=new int*[i];
 	for(j=0;j<current_vertex_order;j++) p2[j]=mep[j];
 	delete [] mep;mep=p2;
 	p1=new int[i];
-	for(j=0;j<current_vertex_order;j++) p1[j]=mec[j];
-	while(j<i) p1[j++]=0;
+	for(j=0;j<current_vertex_order;j++) p1[j]=mec[j];while(j<i) p1[j++]=0;
 	delete [] mec;mec=p1;
 	vc.n_add_memory_vorder(i);
 	current_vertex_order=i;
 }
 
 /** Doubles the size allocation of the main delete stack. If the allocation
  * exceeds the absolute maximum set in max_delete_size, then routine causes a
@@ -213,16 +211,15 @@
 }
 
 /** Initializes a Voronoi cell as a rectangular box with the given dimensions.
  * \param[in] (xmin,xmax) the minimum and maximum x coordinates.
  * \param[in] (ymin,ymax) the minimum and maximum y coordinates.
  * \param[in] (zmin,zmax) the minimum and maximum z coordinates. */
 void voronoicell_base::init_base(double xmin,double xmax,double ymin,double ymax,double zmin,double zmax) {
-	for(int i=0;i<current_vertex_order;i++) mec[i]=0;
-	up=0;
+	for(int i=0;i<current_vertex_order;i++) mec[i]=0;up=0;
 	mec[3]=p=8;xmin*=2;xmax*=2;ymin*=2;ymax*=2;zmin*=2;zmax*=2;
 	*pts=xmin;pts[1]=ymin;pts[2]=zmin;
 	pts[3]=xmax;pts[4]=ymin;pts[5]=zmin;
 	pts[6]=xmin;pts[7]=ymax;pts[8]=zmin;
 	pts[9]=xmax;pts[10]=ymax;pts[11]=zmin;
 	pts[12]=xmin;pts[13]=ymin;pts[14]=zmax;
 	pts[15]=xmax;pts[16]=ymin;pts[17]=zmax;
```

### Comparing `asap3-3.13.1/PTM/voronoi/cell.hpp` & `asap3-3.9.6/PTM/voronoi/cell.hpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/PTM/voronoi/config.hpp` & `asap3-3.9.6/PTM/voronoi/config.hpp`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Parallel/AsapMPI.cpp` & `asap3-3.9.6/Parallel/AsapMPI.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // -*- C++ -*-
-// AsapMPI.cpp: Interface to the MPI library.
+// AsapMPI.h: Interface to the MPI library.
 //
 // Copyright (C) 2001-2011 Jakob Schiotz and Center for Individual
 // Nanoparticle Functionality, Department of Physics, Technical
 // University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
 //
@@ -20,316 +20,303 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-#include "AsapPython.h"
-#include <mpi.h>
-//#include "Asap.h"
-#include "Timing.h"
-#include "AsapMPI.h"
-#include "Exception.h"
-
-
-// XXXXXX
-// IMPORTANT TO-DO:  Move code into module, so assert() can be turned back into ASSERT()
-// XXXXXX
-
 
-static void mpi_ensure_finalized(void)
-{
-  int already_finalized = 1;
-  int ierr = MPI_SUCCESS;
-
-  MPI_Finalized(&already_finalized);
-  if (!already_finalized)
-  {
-    ierr = MPI_Finalize();
-  }
-  if (ierr != MPI_SUCCESS)
-    PyErr_SetString(PyExc_RuntimeError, "MPI_Finalize error occurred");
-}
+#ifndef _ASAP_MPI_H
+#define _ASAP_MPI_H
 
+#include <mpi.h>
+#include <vector>
+using std::vector;
+#include <string>
+using std::string;
 
-// MPI initialization
-static void mpi_ensure_initialized(void)
-{
-  int already_initialized = 1;
-  int ierr = MPI_SUCCESS;
-
-  // Check whether MPI is already initialized
-  MPI_Initialized(&already_initialized);
-  if (!already_initialized)
-  {
-    // if not, let's initialize it
-    int provided = 0;
-    ierr = MPI_Init_thread(NULL, NULL,  MPI_THREAD_SERIALIZED, &provided);
-    if (ierr == MPI_SUCCESS && provided >=  MPI_THREAD_SERIALIZED)
-    {
-      // No problem: register finalization when at Python exit
-      Py_AtExit(*mpi_ensure_finalized);
-    }
-    else
-    {
-      // We have a problem: raise an exception
-      char err[MPI_MAX_ERROR_STRING];
-      int resultlen;
-      MPI_Error_string(ierr, err, &resultlen);
-      PyErr_SetString(PyExc_RuntimeError, err);
-    }
-  }
-}
-
+#include "Timing.h"
 
+namespace ASAPSPACE {
 
 /// The Communicator provides a simplified interface to the MPI protocol.
 
+/// Technical details: The MPI protocol needs to be accessed through
+/// the interface exported by Scientific Python's MPI module.
+/// Unfortunately, importing said MPI module's header file from a C++
+/// file fails, as it is a C header, causing mpi.h to be imported
+/// inside an 'extern "C" {}' statement, which will fail since mpi.h
+/// defines a C++ interface to MPI.  The solution is to encapsulate
+/// the actual MPI calls in a C file.
+class Communicator
+{
+public:
+  inline Communicator() {
+    MPI_Comm_dup(MPI_COMM_WORLD, &comm);
+    int ok = 0;
+    waiting = false;
+    recvwaiting = false;
+    MPI_Initialized(&ok);
+    assert(ok);
+    nProcessors = 0;
+    MPI_Comm_size(comm, &nProcessors);
+    MPI_Comm_rank(comm, &nProcessor);
+  }
 
-Communicator::Communicator()
-{
-  mpi_ensure_initialized();
-  
-  MPI_Comm_dup(MPI_COMM_WORLD, &comm);
-  int ok = 0;
-  waiting = false;
-  recvwaiting = false;
-  MPI_Initialized(&ok);
-  ASSERT(ok);
-  nProcessors = 0;
-  MPI_Comm_size(comm, &nProcessors);
-  MPI_Comm_rank(comm, &nProcessor);
-}
-
-Communicator::~Communicator()
-{
-  MPI_Comm_free(&comm);
-}
+  inline ~Communicator() {
+    MPI_Comm_free(&comm);
+  }
   
-/// Send the buffer to another processor,
-void Communicator::Send(const vector<char> &buffer, int dest)
-{
-  USETIMER("Communicator::Send");
+  /// Get the number of processors in the simulation.
+  inline int GetNumberOfProcessors() const {return nProcessors;}
+  /// Get the number of this processor (the "rank" in the MPI communicator).
+  inline int GetProcessorNumber() const {return nProcessor;}
+
+  /// Send the buffer to another processor,
+  inline void Send(const vector<char> &buffer, int dest) {
+    USETIMER("Communicator::Send");
 #ifdef USESYNCSEND
-  MPI_Ssend((void *) &buffer[0], buffer.size(), MPI_BYTE, dest,
-	    7, comm);  
+    MPI_Ssend((void *) &buffer[0], buffer.size(), MPI_BYTE, dest,
+	      7, comm);  
 #else
-  MPI_Send((void *) &buffer[0], buffer.size(), MPI_BYTE, dest,
-	   7, comm);  
+    MPI_Send((void *) &buffer[0], buffer.size(), MPI_BYTE, dest,
+	     7, comm);  
 #endif /* USESYNCSEND */    
-}
+    //asap_mpi_send(&(buffer[0]), buffer.size(), nProcessor);
+  }
 
-/// Send the buffer to another processor, but do not block sending process.
-void Communicator::NonBlockingSend(const vector<char> &buffer, int dest)
-{
-  USETIMER("Communicator::NonBlockingSend");
-  ASSERT(!waiting);
+  /// Send the buffer to another processor, but do not block sending process.
+  inline void NonBlockingSend(const vector<char> &buffer, int dest) {
+    USETIMER("Communicator::NonBlockingSend");
+    assert(!waiting);
 #ifdef USESYNCSEND
-  MPI_Issend((void *) &buffer[0], buffer.size(), MPI_BYTE, dest, 7,
-	     comm, &request);  
+    MPI_Issend((void *) &buffer[0], buffer.size(), MPI_BYTE, dest, 7,
+	       comm, &request);  
 #else /* USESYNCSEND */
-  MPI_Isend((void *) &buffer[0], buffer.size(), MPI_BYTE, dest, 7,
-	    comm, &request);  
+    MPI_Isend((void *) &buffer[0], buffer.size(), MPI_BYTE, dest, 7,
+	      comm, &request);  
 #endif /* USESYNCSEND  */
-  waiting = true;
-}
+    //asap_mpi_nonblocking_send(&buffer[0], buffer.size(), nProcessor, request);
+    waiting = true;
+  }
 
-/// \brief Receive a message, appending it to the buffer (which is
-/// resized accordingly).
-void Communicator::Receive(vector<char> &buffer, int src)
-{
-  USETIMER("Communicator::Receive");
-  MPI_Status status;
-  int cnt;
-  MPI_Probe(src, 7, comm, &status);
-  MPI_Get_count(&status, MPI_BYTE, &cnt);
-  int n = buffer.size();
-  if (cnt)
-    {
-      // Got real data, read it.
-      buffer.resize(n + cnt);
-      MPI_Recv(&buffer[n], cnt, MPI_BYTE, src, 7, comm,
-	       MPI_STATUS_IGNORE);
-    }
-  else
-    {
-      // Zero length message: Read it but discard it.  Apparently,
-      // MPI_Recv must be passed a valid address, the end of
-      // buffer[] is not OK.
-      char dummy[128];  
-      MPI_Recv(dummy, cnt, MPI_BYTE, src, 7, comm,
-	       MPI_STATUS_IGNORE);
-    }
-}
-
-/// Receive a message without blocking this process.
-
-/// Overwrites the buffer, which must be big enough to hold the
-/// message.  The corresponding WaitReceive call shrinks the buffer
-/// to the size of the actual message.
-void Communicator::NonBlockingReceive(vector<char> &buffer, int src)
-{
-  USETIMER("Communicator::NonBlockingReceive");
-  ASSERT(!recvwaiting);
-  MPI_Irecv(&buffer[0], buffer.size(), MPI_BYTE, src, 7, comm,
-	    &recvrequest);
-  recvbuffer = &buffer;
-  recvwaiting = true;
-}
-
-/// \name Reduction operations.
-/// They work as expected. :-)
-bool Communicator::LogicalOr(bool boolean)
-{
-  USETIMER("Communicator::LogicalOr");
-  int send = (int)boolean;
-  int receive;
-  MPI_Allreduce(&send, &receive, 1, MPI_INT, MPI_SUM, comm);
-  return (receive > 0);
-}
+  /// \brief Receive a message, appending it to the buffer (which is
+  /// resized accordingly).
+  inline void Receive(vector<char> &buffer, int src) {
+    USETIMER("Communicator::Receive");
+    MPI_Status status;
+    int cnt;
+    MPI_Probe(src, 7, comm, &status);
+    MPI_Get_count(&status, MPI_BYTE, &cnt);
+    //int cnt = asap_mpi_probe_and_count(nProcessor);
+    int n = buffer.size();
+    if (cnt)
+      {
+	// Got real data, read it.
+	buffer.resize(n + cnt);
+        MPI_Recv(&buffer[n], cnt, MPI_BYTE, src, 7, comm,
+		 MPI_STATUS_IGNORE);
+      }
+    else
+      {
+	// Zero length message: Read it but discard it.  Apparently,
+	// MPI_Recv must be passed a valid address, the end of
+	// buffer[] is not OK.
+	char dummy[128];  
+	MPI_Recv(dummy, cnt, MPI_BYTE, src, 7, comm,
+		 MPI_STATUS_IGNORE);
+      }
+  }
 
-int Communicator::Min(int x)
-{
-  USETIMER("Communicator::Min");
-  int min;
-  MPI_Allreduce(&x, &min, 1, MPI_INT, MPI_MIN, comm);
-  return min;
-}
+  /// Receive a message without blocking this process.
 
-double Communicator::Min(double x)
-{
-  USETIMER("Communicator::Min");
-  double min;
-  MPI_Allreduce(&x, &min, 1, MPI_DOUBLE, MPI_MIN, comm);
-  return min;
-}
+  /// Overwrites the buffer, which must be big enough to hold the
+  /// message.  The corresponding WaitReceive call shrinks the buffer
+  /// to the size of the actual message.
+  inline void NonBlockingReceive(vector<char> &buffer, int src) {
+    USETIMER("Communicator::NonBlockingReceive");
+    assert(!recvwaiting);
+    MPI_Irecv(&buffer[0], buffer.size(), MPI_BYTE, src, 7, comm,
+	      &recvrequest);
+    //asap_mpi_nonblocking_receive(&buffer[0], buffer.size(), nProcessor,
+    //				 recvrequest);
+    recvbuffer = &buffer;
+    recvwaiting = true;
+  }
 
-int Communicator::Max(int x)
-{
-  USETIMER("Communicator::Max");
-  int max;
-  MPI_Allreduce(&x, &max, 1, MPI_INT, MPI_MAX, comm);
-  return max;
-}
+#if 0  // Requires a patch to Scientific.MPI, and is not fastest.
+  
+  // Simultaneous send and receive.  The receive buffer is overwritten and
+  // resized.
+  void SendReceive(const vector<char> &sendbuf, int destination,
+                   vector<char> &recvbuf, int source);
+#endif
+
+  /// \name Reduction operations.
+  /// They work as expected. :-)
+
+  //@{
+  inline bool LogicalOr(bool boolean) {
+    USETIMER("Communicator::LogicalOr");
+    int send = (int)boolean;
+    int receive;
+    MPI_Allreduce(&send, &receive, 1, MPI_INT, MPI_SUM, comm);
+    //    asap_mpi_allreduce_sum_int(&send, &receive, 1);
+    return (receive > 0);
+  }
+    
+  inline int Min(int x) {
+    USETIMER("Communicator::Min");
+    int min;
+    MPI_Allreduce(&x, &min, 1, MPI_INT, MPI_MIN, comm);
+    //    asap_mpi_allreduce_min_double(&x, &min, 1);
+    return min;
+  }
 
-double Communicator::Max(double x)
-{
-  USETIMER("Communicator::Max");
-  double max;
-  MPI_Allreduce(&x, &max, 1, MPI_DOUBLE, MPI_MAX, comm);
-  return max;
-}
+  inline double Min(double x) {
+    USETIMER("Communicator::Min");
+    double min;
+    MPI_Allreduce(&x, &min, 1, MPI_DOUBLE, MPI_MIN, comm);
+    //    asap_mpi_allreduce_min_double(&x, &min, 1);
+    return min;
+  }
 
-void Communicator::Max(vector<int> &x, vector<int> &sum)
-{
-  USETIMER("Communicator::Max(vector<int>)");
-  sum.resize(x.size());
-  MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_INT, MPI_MAX, comm);
-}
+  inline int Max(int x) {
+    USETIMER("Communicator::Max");
+    int max;
+    MPI_Allreduce(&x, &max, 1, MPI_INT, MPI_MAX, comm);
+    //    asap_mpi_allreduce_max_double(&x, &max, 1);
+    return max;
+  }
+  
+  inline double Max(double x) {
+    USETIMER("Communicator::Max");
+    double max;
+    MPI_Allreduce(&x, &max, 1, MPI_DOUBLE, MPI_MAX, comm);
+    //    asap_mpi_allreduce_max_double(&x, &max, 1);
+    return max;
+  }
+  
+  inline void Max(vector<int> &x, vector<int> &sum) {
+    USETIMER("Communicator::Max(vector<int>)");
+    sum.resize(x.size());
+    MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_INT, MPI_MAX, comm);
+  }
+    
+  inline double Add(double x) {
+    USETIMER("Communicator::Add(double)");
+    double sum;
+    MPI_Allreduce(&x, &sum, 1, MPI_DOUBLE, MPI_SUM, comm);
+    //    asap_mpi_allreduce_sum_double(&x, &sum, 1);
+    return sum;
+  }
 
-double Communicator::Add(double x)
-{
-  USETIMER("Communicator::Add(double)");
-  double sum;
-  MPI_Allreduce(&x, &sum, 1, MPI_DOUBLE, MPI_SUM, comm);
-  return sum;
-}
+  inline int Add(int x) {
+    USETIMER("Communicator::Add(int)");
+    int sum;
+    MPI_Allreduce(&x, &sum, 1, MPI_INT, MPI_SUM, comm);
+    //    asap_mpi_allreduce_sum_int(&x, &sum, 1);
+    return sum;
+  }
+  
+  inline long Add(long x) {
+    USETIMER("Communicator::Add(long)");
+    long sum;
+    MPI_Allreduce(&x, &sum, 1, MPI_LONG, MPI_SUM, comm);
+    //    asap_mpi_allreduce_sum_long(&x, &sum, 1);
+    return sum;
+  }
+  
+  inline void Add(vector<int> &x, vector<int> &sum) {
+    USETIMER("Communicator::Add(vector<int>)");
+    sum.resize(x.size());
+    MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_INT, MPI_SUM, comm);
+    //    asap_mpi_allreduce_sum_int(&x[0], &sum[0], x.size());
+  }
+  
+  inline void Add(vector<long> &x, vector<long> &sum) {
+    USETIMER("Communicator::Add(vector<long>)");
+    sum.resize(x.size());
+    MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_LONG, MPI_SUM, comm);
+    //    asap_mpi_allreduce_sum_int(&x[0], &sum[0], x.size());
+  }
+  
+  inline void Add(vector<double> &x, vector<double> &sum) {
+    USETIMER("Communicator::Add(vector<double>)");
+    sum.resize(x.size());
+    MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_DOUBLE, MPI_SUM, comm);
+    //    asap_mpi_allreduce_sum_double(&x[0], &sum[0], x.size());
+  }
+  //@}
+  
+  /// Wait for a nonblocking send to complete.
 
-int Communicator::Add(int x)
-{
-  USETIMER("Communicator::Add(int)");
-  int sum;
-  MPI_Allreduce(&x, &sum, 1, MPI_INT, MPI_SUM, comm);
-  return sum;
-}
+  ///
+  /// When Wait() returns, the send buffer may be overwritten.
+  inline void Wait() {
+    USETIMER("Communicator::Wait");
+    assert(waiting);
+    MPI_Wait(&request, MPI_STATUS_IGNORE);
+    //    asap_mpi_wait(request);
+    waiting = false;
+  }
 
-long Communicator::Add(long x)
-{
-  USETIMER("Communicator::Add(long)");
-  long sum;
-  MPI_Allreduce(&x, &sum, 1, MPI_LONG, MPI_SUM, comm);
-  return sum;
-}
+  /// Wait for a nonblocking receive to complete.
 
-void Communicator::Add(vector<int> &x, vector<int> &sum)
-{
-  USETIMER("Communicator::Add(vector<int>)");
-  sum.resize(x.size());
-  MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_INT, MPI_SUM, comm);
-}
+  ///
+  /// At return, the receive buffer contains the incoming message.
+  inline void WaitReceive() {
+    USETIMER("Communicator::WaitReceive");
+    assert(recvwaiting);
+    int cnt;
+    MPI_Status status;
+    MPI_Wait(&recvrequest, &status);
+    MPI_Get_count(&status, MPI_BYTE, &cnt);
+    //int cnt = asap_mpi_wait_and_count(request);
+    recvbuffer->resize(cnt);
+    recvwaiting = false;
+  }
+  
+  /// All to all communication.
 
-void Communicator::Add(vector<long> &x, vector<long> &sum)
-{
-  USETIMER("Communicator::Add(vector<long>)");
-  sum.resize(x.size());
-  MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_LONG, MPI_SUM, comm);
-}
+  /// Send size integers to each process, receiving as many.  The size
+  /// of the sendbuffer must be size * nProcessors, the receive buffer
+  /// is resized to this same size.
+  inline void AllToAll(vector<int> &sendbuf, vector<int> &recvbuf, int size) {
+    USETIMER("Communicator::AllToAll");
+    assert(sendbuf.size() == size * nProcessors);
+    recvbuf.resize(size * nProcessors);
+    MPI_Alltoall(&sendbuf[0], size, MPI_INT, &recvbuf[0], size, MPI_INT,
+		 comm);
+    //    asap_mpi_all_to_all_int(&sendbuf[0], &recvbuf[0], size);
+  }
 
-void Communicator::Add(vector<double> &x, vector<double> &sum)
-{
-  USETIMER("Communicator::Add(vector<double>)");
-  sum.resize(x.size());
-  MPI_Allreduce(&x[0], &sum[0], x.size(), MPI_DOUBLE, MPI_SUM, comm);
-}
-  
-/// Wait for a nonblocking send to complete.
-
-///
-/// When Wait() returns, the send buffer may be overwritten.
-void Communicator::Wait()
-{
-  USETIMER("Communicator::Wait");
-  ASSERT(waiting);
-  MPI_Wait(&request, MPI_STATUS_IGNORE);
-  //    asap_mpi_wait(request);
-  waiting = false;
-}
-
-/// Wait for a nonblocking receive to complete.
-
-///
-/// At return, the receive buffer contains the incoming message.
-void Communicator::WaitReceive()
-{
-  USETIMER("Communicator::WaitReceive");
-  ASSERT(recvwaiting);
-  int cnt;
-  MPI_Status status;
-  MPI_Wait(&recvrequest, &status);
-  MPI_Get_count(&status, MPI_BYTE, &cnt);
-  //int cnt = asap_mpi_wait_and_count(request);
-  recvbuffer->resize(cnt);
-  recvwaiting = false;
-}
-
-/// All to all communication.
-
-/// Send size integers to each process, receiving as many.  The size
-/// of the sendbuffer must be size * nProcessors, the receive buffer
-/// is resized to this same size.
-void Communicator::AllToAll(vector<int> &sendbuf, vector<int> &recvbuf, int size)
-{
-  USETIMER("Communicator::AllToAll");
-  ASSERT(sendbuf.size() == size * nProcessors);
-  recvbuf.resize(size * nProcessors);
-  MPI_Alltoall(&sendbuf[0], size, MPI_INT, &recvbuf[0], size, MPI_INT,
-	       comm);
-  //    asap_mpi_all_to_all_int(&sendbuf[0], &recvbuf[0], size);
-}
-
-/// AllGather.
-
-/// Send size integers to all the processors, receive as
-/// many from each processor, size*nProcessor in total.  The size of
-/// the send buffer must be size, the receive buffer is resized to
-/// size*nProcessors.
-void Communicator::AllGather(vector<int> &sendbuf, vector<int> &recvbuf, int size)
-{
-  USETIMER("Communicator::AllGather");
-  ASSERT(sendbuf.size() == size);
-  recvbuf.resize(size * nProcessors);
-  MPI_Allgather(&sendbuf[0], size, MPI_INT, &recvbuf[0], size, MPI_INT,
-		comm);
-  //    asap_mpi_allgather_int(&sendbuf[0], &recvbuf[0], size);
-}
+  /// AllGather.
+
+  /// Send size integers to all the processors, receive as
+  /// many from each processor, size*nProcessor in total.  The size of
+  /// the send buffer must be size, the receive buffer is resized to
+  /// size*nProcessors.
+  inline void AllGather(vector<int> &sendbuf, vector<int> &recvbuf, int size) {
+    USETIMER("Communicator::AllGather");
+    assert(sendbuf.size() == size);
+    recvbuf.resize(size * nProcessors);
+    MPI_Allgather(&sendbuf[0], size, MPI_INT, &recvbuf[0], size, MPI_INT,
+		  comm);
+    //    asap_mpi_allgather_int(&sendbuf[0], &recvbuf[0], size);
+  }
+  
+private:
+  MPI_Comm comm;     ///< Communicator object
+  bool waiting;      ///< Waiting for nonblocking send
+  bool recvwaiting;  ///< Waiting for nonblocking receive
+  int nProcessor;    ///< The number of this processor
+  int nProcessors;   ///< The total number of processors in the simulation.
+  MPI_Request request;     ///< For nonblocking send.
+  MPI_Request recvrequest; ///< For nonblocking recv.
+  vector<char> *recvbuffer; ///< The buffer used in nonblocking recv.
+  // string filename;   // Not used?
+};
+
+} // end namespace
 
+#endif//  _ASAP_MPI_H
```

### Comparing `asap3-3.13.1/Parallel/DomainDecomposition.h` & `asap3-3.9.6/Parallel/DomainDecomposition.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Parallel/ParallelAtoms.cpp` & `asap3-3.9.6/Parallel/ParallelAtoms.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -30,78 +30,57 @@
 #include "Debug.h"
 #include <math.h>
 using std::cerr;
 using std::endl;
 using std::flush;
 
 static char mycobject[] = "_asap_parallelatoms_cobject";
-static char invalidghosts[] = "_asap_invalidghosts";
-
-// Exception thrown if ghosts are invalid.  Should always be caught internally.
-class AsapGhostInvalid : public AsapError
-{
-public:
-  AsapGhostInvalid(const char *m) : AsapError(m) {};
-};
 
 // #define REGARRAYINFO   // Print extra debugging info about reg. arrays.
 
-// Local function to get stride from PyArray, even if first dimension is zero
-// (PyArray_STRIDE returns 0 in that case for numpy version 1.23.X)
-static npy_intp get_stride_from_array(PyArrayObject *arr)
-{
-  npy_intp stride = PyArray_ITEMSIZE(arr);
-  for (int i = 1; i < PyArray_NDIM(arr); i++)
-    stride *= PyArray_DIM(arr, i);
-  ASSERT(PyArray_STRIDE(arr, 0) == 0 || PyArray_STRIDE(arr, 0) == stride);
-  return stride;
-}
-
 /////////////////////////////
 ////
 ////  CONSTRUCTOR
 ////
 /////////////////////////////
 
 
 ParallelAtoms::ParallelAtoms(PyObject *py_atoms, int verbose)
 {
   CONSTRUCTOR;
   this->verbose = verbose;
-  hasGhosts = true;
   try {
     DEBUGPRINT;
     migrationCounter = 0;
     decorated = false;
     ghost_count = 0;
-    haswarned_noatoms = false;
     mpi = new Communicator();  // Later, consider extracting from atoms.
-    ASSERT(mpi != NULL);
+    assert(mpi != NULL);
     extract_ncells(py_atoms);  // Read nCells from Python object
     domainDecomp = NULL;
     
     nProcessor = mpi->GetProcessorNumber();
     nProcessors = mpi->GetNumberOfProcessors();
     
     int nTotalCells = 1;
     for (int i = 0; i < 3; i++)
       nTotalCells *= nCells[i];
-    ASSERT(nTotalCells == nProcessors);
+    assert(nTotalCells == nProcessors);
     
     nTotalAtoms = 0;
     // We assume that a "char" is a byte!
-    ASSERT(sizeof(char) == 1);
+    assert(sizeof(char) == 1);
     
     // Now, we can create the domain decomposition.  We need to access
     // data from the atoms, the easiest is to open them.
     Begin(py_atoms);
     domainDecomp = new RegularGridDecomposition(GetCell(),
 						GetBoundaryConditions(),
-						nCells, mpi, verbose);
-    ASSERT(domainDecomp != NULL);
+						nCells, mpi);
+    assert(domainDecomp != NULL);
     End();
     DEBUGPRINT;
   }
   catch (...) {
     // If an error occurred in the constructor, the object is deallocated.
     // If refcount is non-zero, Atoms::~Atoms() will detect an error.
     DEBUGPRINT;
@@ -148,51 +127,38 @@
   Begin(pyatoms, allow_reopen, false);
 }
 
 void ParallelAtoms::Begin(PyObject *pyatoms, bool allow_reopen, bool postmigrate)
 {
   DEBUGPRINT;
   NormalAtoms::Begin(pyatoms, allow_reopen);
-  if (!haswarned_noatoms)
-  {
-    // The test suite needs to suppress this warning.
-    if (PyObject_HasAttrString(pyatoms, "suppress_warning_noatoms"))
-      haswarned_noatoms = true;  // Pretend the warning has already been issued
-  }
   if (nTotalAtoms == 0)
     nTotalAtoms = mpi->Add(nAtoms);
   if (!postmigrate && active == 1)
     {
       // Communicate the counters, so we see updates on other processors
-      const int ndata = 5;  // Five counters 
+      const int ndata = 6;  // Six counters 
       vector<int> mydata(ndata);
       vector<int> globaldata(ndata);
       mydata[0] = count_atoms;
       mydata[1] = count_cell;
       mydata[2] = count_positions;
       mydata[3] = count_numbers;
-      mydata[4] = count_inverse_cell;
+      mydata[4] = count_momenta;
+      mydata[5] = count_inverse_cell;
       mpi->Max(mydata, globaldata);
       count_atoms = globaldata[0];
       count_cell = globaldata[1];
       count_positions = globaldata[2];
       count_numbers = globaldata[3];
-      count_inverse_cell = globaldata[4];
+      count_momenta = globaldata[4];
+      count_inverse_cell = globaldata[5];
       if (decorated && ghost_count != count_positions)
 	{
-	  try {
-	    UpdateGhostData();
-	  } catch(AsapGhostInvalid &e) {
-	    // The ghosts have explicitly been marked invalid.
-	    double range = get_ghost_range();
-	    DecorateWithGhosts(range);
-	    UpdateGhostData();
-	    // This may also have invalidated nTotalAtoms
-	    nTotalAtoms = mpi->Add(nAtoms);
-	  }
+	  UpdateGhostData();
 	  ghost_count = count_positions;
 	}
     }
   DEBUGPRINT;
 }
 
 ////////////////////////////////
@@ -269,30 +235,30 @@
               while (j != sendlist->end() && *j != i)
                 ++j;
               if (j == sendlist->end())
 		throw AsapError("An atom is migrating to a non-neighboring processor (It must have a huge velocity - plasma physics is not supported!).");
 	    }
         }          
     }
-  ASSERT((sendlist->size() == recvlist->size()) &&
+  assert((sendlist->size() == recvlist->size()) &&
          (sendlist->size() < nProcessors));
   DEBUGPRINT;
 
   // Extract data from Python atoms
-  vector<std::string> array_names; // Sorted list of array names.
+  vector<const char *> array_names; // Sorted list of array names.
   vector<PyArrayObject *> arrays;  // Owned refs to arrays to migrate.
   get_array_names(py_arrays, array_names);
   get_arrays(py_arrays, array_names, arrays);
 
   DEBUGPRINT;
   // Send and receive:
-  int nBytes = 0;   // Number of bytes to be communicated per atom.
+  int nBytes = 0;
   for (vector<PyArrayObject *>::const_iterator arr = arrays.begin();
        arr < arrays.end(); ++arr)
-    nBytes += get_stride_from_array(*arr);
+    nBytes += PyArray_STRIDE(*arr, 0);
 
   receiveBuffer.resize(0);
   int nCommunicate = sendlist->size();
   DEBUGPRINT;
   for (int dp = 0; dp < nCommunicate; dp++)
     {
       int pSend = (*sendlist)[dp];
@@ -304,21 +270,21 @@
   DEBUGPRINT;
       for (int i = 0; i < nAtomsToSend; i++)
         {
           int a = cells[pSend][i];
 	  for (vector<PyArrayObject *>::const_iterator arr = arrays.begin();
 	       arr < arrays.end(); ++arr)
 	    {
-	      long stride = get_stride_from_array(*arr);
+	      int stride = PyArray_STRIDE(*arr, 0);
 	      memcpy(b, PyArray_BYTES(*arr) + a * stride, stride);
 	      b += stride;
 	    }
         }
       DEBUGPRINT;
-      ASSERT(b == &sendBuffer[0] + nAtomsToSend * nBytes);
+      assert(b == &sendBuffer[0] + nAtomsToSend * nBytes);
       if (verbose > 1)
         cerr << nProcessor << ": sending " << nAtomsToSend
 	     << " atoms of size " << nBytes << " bytes = "
              << sendBuffer.size() << " bytes to proc " << pSend << endl;
       DEBUGPRINT;
       mpi->NonBlockingSend(sendBuffer, pSend);
       DEBUGPRINT;
@@ -349,40 +315,40 @@
     {
       int a2 = migrated[i];
       int n = a2 - a1;
       if (n > 0)
 	{
 	  for (int j = 0; j < arrays.size(); j++)
 	    {
-	      long stride = get_stride_from_array(arrays[j]);
+	      int stride = PyArray_STRIDE(arrays[j], 0);
 	      memcpy(PyArray_BYTES(new_arrays[j]) + target * stride,
 		     PyArray_BYTES(arrays[j]) + a1 * stride,
 		     n * stride);
 	    }
 	  target += n;
 	}
       a1 = a2 + 1;
     }
-  ASSERT(target == nAtoms - nMigrated);
+  assert(target == nAtoms - nMigrated);
   DEBUGPRINT;
   
   // Append atoms from other processors:
   // SetNumberOfGhosts(0); XXXX
   char *b = &receiveBuffer[0];
   char *b0 = b;
   for (int a = nAtoms - nMigrated; a < nNewAtoms; a++)
     {
       for (int j = 0; j < new_arrays.size(); j++)
 	{
-	  long stride = get_stride_from_array(new_arrays[j]);
+	  int stride = PyArray_STRIDE(new_arrays[j], 0);
 	  memcpy(PyArray_BYTES(new_arrays[j]) + a * stride, b, stride);
 	  b += stride;
 	}
     }
-  ASSERT(b - b0 == receiveBuffer.size());
+  assert(b - b0 == receiveBuffer.size());
   nAtoms = nNewAtoms;
   DEBUGPRINT;
   release_arrays(arrays, array_names, 2);
   store_arrays(py_arrays, array_names, new_arrays);
   release_arrays(new_arrays, array_names, 2);
   CheckIdentities();
   set_ghost_range(-1.0);  // No ghosts yet.
@@ -417,15 +383,15 @@
 
 ////////////////////////////////
 ////
 ////  GetListOfElements
 ////
 ////////////////////////////////
 
-void ParallelAtoms::GetListOfElements(set<int> &elements)
+void ParallelAtoms::GetListOfElements(set<int> &elements) const
 {
   DEBUGPRINT;
   vector<char> buf;
   int *b;
   int thisproc = mpi->GetProcessorNumber();
   int nelem;
   
@@ -472,15 +438,15 @@
         mpi->Send(buf, proc);
     }
   else
     {
       elements.clear();
       mpi->Receive(buf, 0);
       nelem = buf.size() / sizeof(int);
-      ASSERT(nelem);
+      assert(nelem);
       b = (int *) &buf[0];
       for (int i = 0; i < nelem; i++)
         elements.insert(b[i]);
     }
   if (verbose > 1)
     {
       cerr << "Processor " << thisproc << ": List of elements: ";
@@ -506,15 +472,15 @@
   // This test does not work if long is a 32 bit integer.  This should
   // be a preprocessor test, but sizeof cannot be used in preprocessor
   // directives.
   if (sizeof(long) > 4)
     {
       DEBUGPRINT;
       USETIMER("ParallelAtoms::CheckIdentities");
-      // ASSERT(sizeof(long) > 4);
+      // assert(sizeof(long) > 4);
       const long *identities = GetIdentities();
       long totident = 0;
       long expected = ((long) nTotalAtoms) * (nTotalAtoms-1) / 2;
       for (int i = 0; i < nAtoms; i++)
 	totident += identities[i];
       vector<long> here(2);
       vector<long> sum;
@@ -560,15 +526,15 @@
 ////  GetIdentities
 ////
 ////////////////////////////////
 
 const long *ParallelAtoms::GetIdentities() const
 {
   DEBUGPRINT;
-  ASSERT(py_arrays != NULL && PyDict_Check(py_arrays));
+  assert(py_arrays != NULL && PyDict_Check(py_arrays));
   PyArrayObject *id = AsPyArray(PyDict_GetItemString(py_arrays, "ID")); // BORROWED ref!
   if (id == NULL)
     throw AsapError("Invalid ParallelAtoms object: No ID array.");
   if (PyArray_NDIM(id) != 1           // One-dimensional
       || PyArray_DIM(id, 0) != nAtoms    // One per atom
       || PyArray_TYPE(id) != NPY_LONG    // array of longs
       || !PyArray_ISCARRAY_RO(id))       // Contiguous etc.
@@ -592,150 +558,141 @@
   T *from = (T *) PyArray_DATA(py_numbers);
   for (int i = 0; i < nGh; i++)
     num[nAt + i] = (asap_z_int) from[i];
 }
 
 void ParallelAtoms::UpdateGhostData()
 {
-  // Potentially the ghosts could have been invalidated.  In that case
-  // throw a specific error that can be caught further up.
-  if (PyObject_HasAttrString(py_atoms, invalidghosts))
-    throw AsapGhostInvalid("Ghosts invalid");
-      
   DEBUGPRINT;
   if (verbose)
     cerr << " UG";
   vector<char> sendBuffer;
   vector<char> recvBuffer;
 
   USETIMER("ParallelAtoms::UpdateGhostData");
   // Check that we are not mixing data from two different ParallelAtoms objects.
-  ASSERT(py_atoms != NULL);
+  assert(py_atoms != NULL);
   PyObject *mypointer = PyObject_GetAttrString(py_atoms, mycobject);
   if (mypointer == NULL)
     throw AsapError("ParallelAtoms::UpdateGhostData: failed to get ") <<
       mycobject;
+#if PY_VERSION_HEX < 0x02070000
+  bool OK = PyCObject_Check(mypointer) && (PyCObject_AsVoidPtr(mypointer)
+					   == this);
+#else
   bool OK = (PyCapsule_CheckExact(mypointer) &&
 	     (PyCapsule_GetPointer(mypointer, "asap3.parallelatoms") == this));
+#endif
   Py_DECREF(mypointer);
   if (!OK)
     throw AsapError("ParallelAtoms::UpdateGhostData: Multiple objects are creating ghost atoms.");
 
   // Now we should populate the ghost data
   const vector<int> *sendlist = domainDecomp->GetSendList();
   const vector<int> *recvlist = domainDecomp->GetRecvList();
-  ASSERT(sendlist->size() == recvlist->size());
+  assert(sendlist->size() == recvlist->size());
   
   PyObject *py_ghosts = PyObject_GetAttrString(py_atoms, "ghosts");
   if (py_ghosts == NULL)
     throw AsapError("ParallelAtoms::UpdateGhostData: No ghosts found.");
   PyObject *py_arrays = PyObject_GetAttrString(py_atoms, "arrays");
   if (py_arrays == NULL)
     throw AsapError("ParallelAtoms::UpdateGhostData: No arrays found.");
   
-  vector<std::string> array_names;          // Sorted list of array names.
+  vector<const char *> array_names;          // Sorted list of array names.
   vector<PyArrayObject *> real_arrays;            // Data on real atoms.
   vector<PyArrayObject *> ghost_arrays;           // Ghost arrays to fill.
   get_array_names(py_ghosts, array_names);
   get_arrays(py_ghosts, array_names, ghost_arrays);
   get_arrays(py_arrays, array_names, real_arrays);
   int nBytes = 0;
   int pos_index = -1;
   int num_index = -1;
   // Count number of bytes and find the positions array.
   for (int i = 0; i < array_names.size(); i++)
     {
-      int n = get_stride_from_array(real_arrays[i]);
-      ASSERT(get_stride_from_array(ghost_arrays[i]) == n);
-      ASSERT(PyArray_DIM(real_arrays[i], 0) == nAtoms);
-      ASSERT(PyArray_DIM(ghost_arrays[i], 0) == nGhosts);
+      int n = PyArray_STRIDE(real_arrays[i], 0);
+      assert(PyArray_STRIDE(ghost_arrays[i], 0) == n);
+      assert(PyArray_DIM(real_arrays[i], 0) == nAtoms);
+      assert(PyArray_DIM(ghost_arrays[i], 0) == nGhosts);
       nBytes += n;
-      if (array_names[i].compare("positions") == 0)
+      if (strcmp(array_names[i], "positions") == 0)
 	{
 	  pos_index = i;
-	  ASSERT(n == sizeof(Vec));
+	  assert(n == sizeof(Vec));
 	}
-      if (array_names[i].compare("numbers") == 0)
+      if (strcmp(array_names[i], "numbers") == 0)
 	  num_index = i;
     }
-  ASSERT(pos_index >= 0);  // But no check for num_index: not compulsory.
+  assert(pos_index >= 0);  // But no check for num_index: not compulsory.
 
   num_ghosts_recv_from.resize(recvlist->size());
-  DEBUGPRINT;
-  long offset = 0;  // Offset into receiving arrays
+  int offset = 0;  // Offset into receiving arrays
   // Loop over processors
   for (int dp = 0; dp < sendlist->size(); dp++)
     {
       int send_p = (*sendlist)[dp];
       const vector< pair<int, int> > &indices = ghosts[send_p];
       sendBuffer.resize(indices.size() * nBytes);
       char *b = &sendBuffer[0];
       // Loop over arrays to send
       for (int arr = 0; arr < array_names.size(); arr++)
 	{
 	  // Loop over atoms to send
 	  typedef vector< pair<int, int> >::const_iterator VP;
 	  for (VP g = indices.begin(); g != indices.end(); ++g)
 	    {
-	      npy_intp stride = get_stride_from_array(real_arrays[arr]);
 	      char *from = PyArray_BYTES(real_arrays[arr]) +
-		((long)g->first) * stride;
-	      memcpy(b, from, stride);
-	      b += stride;
+		g->first * PyArray_STRIDE(real_arrays[arr], 0);
+	      memcpy(b, from, PyArray_STRIDE(real_arrays[arr], 0));
+	      b += PyArray_STRIDE(real_arrays[arr], 0);
 	    }
 	}
-      ASSERT(b - &sendBuffer[0] == sendBuffer.size());
+      assert(b - &sendBuffer[0] == sendBuffer.size());
 
       // Communicate
       mpi->NonBlockingSend(sendBuffer, send_p);
       int recv_p = (*recvlist)[dp];
       recvBuffer.clear();
       mpi->Receive(recvBuffer, recv_p);
       int n_recv = recvBuffer.size() / nBytes;
       num_ghosts_recv_from[dp] = n_recv;
       b = &recvBuffer[0];
       for (int arr = 0; arr < array_names.size(); arr++)
 	{
-	  npy_intp stride = get_stride_from_array(ghost_arrays[arr]);
-	  char *to = PyArray_BYTES(ghost_arrays[arr]) + offset * stride;
-	  memcpy(to, b, n_recv * stride);
-	  b += n_recv * stride;
+	  char *to = PyArray_BYTES(ghost_arrays[arr])
+	    + offset * PyArray_STRIDE(ghost_arrays[arr], 0);
+	  memcpy(to, b, n_recv * PyArray_STRIDE(ghost_arrays[arr], 0));
+	  b += n_recv * PyArray_STRIDE(ghost_arrays[arr], 0);
 	}
       offset += n_recv;
       mpi->Wait();
     }
-  DEBUGPRINT;
-  ASSERT(offset == nGhosts);
+  assert(offset == nGhosts);
   // Now, the ghost positions should be copied into the local positions array...
-  if (nGhosts > 0)
-  {
-    DEBUGPRINT;
-    assert(positions.size() > 0);
-    memcpy(&positions[nAtoms], PyArray_DATA(ghost_arrays[pos_index]),
-	   nGhosts*sizeof(Vec));
-    // ... and the atomic numbers.
-    DEBUGPRINT;
-    if (num_index >= 0)
-      {
-	PyArrayObject *py_numbers = ghost_arrays[num_index];
-	int tn = PyArray_TYPE(py_numbers);
-	if (PyArray_EquivTypenums(tn, ASAP_Z_ARRAYTYPE))
-	  copynum<asap_z_int>(numbers, py_numbers, nAtoms, nGhosts);
-	else if (PyArray_EquivTypenums(tn, NPY_INT32))
-	  copynum<npy_int32>(numbers, py_numbers, nAtoms, nGhosts);
-	else if (PyArray_EquivTypenums(tn, NPY_INT64))
-	  copynum<npy_int64>(numbers, py_numbers, nAtoms, nGhosts);
-	else if (PyArray_EquivTypenums(tn, NPY_INT8))
-	  copynum<npy_int8>(numbers, py_numbers, nAtoms, nGhosts);
-	else if (PyArray_EquivTypenums(tn, NPY_INT16))
-	  copynum<npy_int16>(numbers, py_numbers, nAtoms, nGhosts);
-	else
-	  throw AsapError("Atomic numbers are an unsupported integer type.");
-      }
-  }
+  memcpy(&positions[nAtoms], PyArray_DATA(ghost_arrays[pos_index]),
+	 nGhosts*sizeof(Vec));
+  // ... and the atomic numbers.
+  if (num_index >= 0)
+    {
+      PyArrayObject *py_numbers = ghost_arrays[num_index];
+      int tn = PyArray_TYPE(py_numbers);
+      if (PyArray_EquivTypenums(tn, ASAP_Z_ARRAYTYPE))
+	copynum<asap_z_int>(numbers, py_numbers, nAtoms, nGhosts);
+      else if (PyArray_EquivTypenums(tn, NPY_INT32))
+	copynum<npy_int32>(numbers, py_numbers, nAtoms, nGhosts);
+      else if (PyArray_EquivTypenums(tn, NPY_INT64))
+	copynum<npy_int64>(numbers, py_numbers, nAtoms, nGhosts);
+      else if (PyArray_EquivTypenums(tn, NPY_INT8))
+	copynum<npy_int8>(numbers, py_numbers, nAtoms, nGhosts);
+      else if (PyArray_EquivTypenums(tn, NPY_INT16))
+	copynum<npy_int16>(numbers, py_numbers, nAtoms, nGhosts);
+      else
+	throw AsapError("Atomic numbers are an unsupported integer type.");
+    }
   
   DEBUGPRINT;
   release_arrays(real_arrays, array_names, 2);
   release_arrays(ghost_arrays, array_names, 2);
   CHECKREF(py_arrays);
   Py_DECREF(py_arrays);
   CHECKREF(py_ghosts);
@@ -773,15 +730,15 @@
       p = (*recvlist)[dp];
       receiveBuffer.resize(0);
       mpi->Receive(receiveBuffer, p);
       memcpy(ghostAddress, &receiveBuffer[0], receiveBuffer.size());
       ghostAddress += receiveBuffer.size() / sizeof(double);
       mpi->Wait();
     }  
-  ASSERT(ghostAddress == address + n * (nAtoms + nGhosts));
+  assert(ghostAddress == address + n * (nAtoms + nGhosts));
   DEBUGPRINT;
 }
 
 
 ////////////////////////////////
 ////
 ////  UpdateBeforeCalculation
@@ -821,18 +778,14 @@
 
 void ParallelAtoms::DecorateWithGhosts(double range)
 {
   DEBUGPRINT;
   if (verbose)
     cerr << " DG";
   USETIMER("ParallelPotential::DecorateWithGhosts");
-  // If the ghosts are marked invalid, unmark them
-  if (PyObject_HasAttrString(py_atoms, invalidghosts))
-    PyObject_DelAttrString(py_atoms, invalidghosts);
-  
   // Delete old Ghosts:
   ghosts.resize(nProcessors);
   for (int p = 0; p < nProcessors; p++)
     ghosts[p].resize(0);
 
   domainDecomp->makeGhostExportLists(this, range, ghosts);
   int nGhosts;
@@ -865,15 +818,15 @@
 ////
 ////////////////////////////////
 
 // Get the number of cells from the Python object.
 void ParallelAtoms::extract_ncells(PyObject *pyatoms)
 {
   DEBUGPRINT;
-  ASSERT(pyatoms != NULL);
+  assert(pyatoms != NULL);
   PyArrayObject *py_cells = AsPyArray(PyObject_GetAttrString(pyatoms, "nCells"));
   if (py_cells == NULL)
     throw AsapError("No nCells. Not a ParallelAtoms object?");
   if (PyArray_NDIM(py_cells) != 1            // One-dimensional
       || PyArray_DIM(py_cells, 0) != 3          // shape = (3,)
       || PyArray_TYPE(py_cells) != NPY_LONG     // array of longs
       || !PyArray_ISCARRAY_RO(py_cells))
@@ -895,58 +848,52 @@
 ////////////////////////////////
 ////
 ////  get_array_names
 ////
 ////////////////////////////////
 								 
 // Get a sorted list of array names.
-void ParallelAtoms::get_array_names(PyObject *dict, vector<std::string> &names)
+void ParallelAtoms::get_array_names(PyObject *dict, vector<const char *> &names)
 {
   DEBUGPRINT;
-  ASSERT(dict != NULL && PyDict_Check(dict));
+  assert(dict != NULL && PyDict_Check(dict));
   PyObject *keys = PyDict_Keys(dict);
-  ASSERT(keys != NULL);
+  assert(keys != NULL);
   if (PyList_Sort(keys) != 0)
     throw AsapError("Failed to sort ParallelAtoms' arrays/ghosts");
   Py_ssize_t n = PyList_GET_SIZE(keys);
   names.resize((int) n);
   for (Py_ssize_t i = 0; i < n; i++)
     {
       PyObject *pyname = PyList_GET_ITEM(keys, i);
-      if (!PyUnicode_Check(pyname))
-	throw AsapError("Non-string key in ghost atom dictionary.");
-      // Make sure the Unicode object is ready and 8-bit data
-      if ((PyUnicode_READY(pyname) == -1)
-	  || (PyUnicode_KIND(pyname) != PyUnicode_1BYTE_KIND))
-	throw AsapError("Non-ascii key in ghost atom dictionary.");
-      // Now convert to a C++ string
-      names[(int)i].assign((char *)PyUnicode_1BYTE_DATA(pyname),
-			   (size_t)PyUnicode_GET_LENGTH(pyname));
+      const char *name = PyAsapString_AsString(pyname);
+      if (name == NULL)
+	throw AsapError("Invalid key is ParallelAtoms' arrays/ghosts.  Not a string?");
+      names[(int)i] = name;
     }
-  Py_DECREF(keys);
   DEBUGPRINT;
 }
 
 
 ////////////////////////////////
 ////
 ////  get_arrays
 ////
 ////////////////////////////////
 
 // Get a list of array objects.
-void ParallelAtoms::get_arrays(PyObject *dict, vector<std::string> &names,
+void ParallelAtoms::get_arrays(PyObject *dict, vector<const char *> &names,
 			       vector<PyArrayObject *> &arrays)
 {
-  ASSERT(dict != NULL && PyDict_Check(dict));
+  assert(dict != NULL && PyDict_Check(dict));
   int n = names.size();
   arrays.resize(n);
   for (int i = 0; i < n; i++)
     {
-      arrays[i] = AsPyArray(PyDict_GetItemString(dict, names[i].c_str()));
+      arrays[i] = AsPyArray(PyDict_GetItemString(dict, names[i]));
       if (arrays[i] == NULL || !PyArray_Check(arrays[i]))
 	throw AsapError("Invalid data in ParallelAtoms' arrays/ghosts[") <<
 	  names[i] << "].";
     }
   for (int i = 0; i < n; i++)
     {
       Py_INCREF(arrays[i]);
@@ -992,24 +939,24 @@
 ////
 ////  release_arrays
 ////
 ////////////////////////////////
 
 // Release references to arrays
 void ParallelAtoms::release_arrays(vector<PyArrayObject *> &arrays,
-				   vector<std::string> &names,
+				    vector<const char *> &names,
 				   int maxcount)
 {
   DEBUGPRINT;
-  vector<std::string>::const_iterator name = names.begin();
+  vector<const char*>::const_iterator name = names.begin();
   for (vector<PyArrayObject *>::iterator i = arrays.begin();
        i != arrays.end(); ++i, ++name)
     {
       if (Py_REFCNT(*i) > maxcount)
-	cerr << "ASAP warning: Extra reference detected for " << name->c_str() << endl;
+	cerr << "ASAP warning: Extra reference detected for " << *name << endl;
       CHECKREF(*i);
       Py_DECREF(*i);
     }
   arrays.clear();
   DEBUGPRINT;
 }
 
@@ -1017,23 +964,23 @@
 ////////////////////////////////
 ////
 ////  store_arrays
 ////
 ////////////////////////////////
 
 // Store arrays into a dictionary.
-void ParallelAtoms::store_arrays(PyObject *dict, vector<std::string> &names,
+void ParallelAtoms::store_arrays(PyObject *dict, vector<const char *> &names,
 				 vector<PyArrayObject *> &arrays)
 {
   DEBUGPRINT;
-  ASSERT(dict != NULL && PyDict_Check(dict));
+  assert(dict != NULL && PyDict_Check(dict));
   int n = names.size();
   for (int i = 0; i < n; i++)
     {
-      int x = PyDict_SetItemString(dict, names[i].c_str(), (PyObject *) arrays[i]);
+      int x = PyDict_SetItemString(dict, names[i], (PyObject *) arrays[i]);
       if (x != 0)
 	throw AsapPythonError();
     }
   DEBUGPRINT;
 }
 
 
@@ -1042,17 +989,17 @@
 ////  set_ghost_range
 ////
 ////////////////////////////////
 
 // Store the max range where the ghosts are valid.  Negative: no ghosts yet.
 void ParallelAtoms::set_ghost_range(double range)
 {
-  ASSERT(py_atoms != NULL);
+  assert(py_atoms != NULL);
   PyObject *x = PyFloat_FromDouble(range);
-  ASSERT(x != NULL);
+  assert(x != NULL);
   int y = PyObject_SetAttrString(py_atoms, "asap_ghost_range", x);
   Py_DECREF(x);
   if (y == -1)
     throw AsapError("Failed to set atoms.asap_ghost_range.");
 }
 
 
@@ -1060,15 +1007,15 @@
 ////
 ////  get_ghost_range
 ////
 ////////////////////////////////
 
 double ParallelAtoms::get_ghost_range()
 {
-  ASSERT(py_atoms != NULL);
+  assert(py_atoms != NULL);
   PyObject *py_x = PyObject_GetAttrString(py_atoms, "asap_ghost_range");
   if (py_x == NULL)
     throw AsapError("Failed to get atoms.asap_ghost_range.");
   if (!PyFloat_Check(py_x))
     {
       Py_DECREF(py_x);
       throw AsapError("Atoms.asap_ghost_range is not a number.");
@@ -1084,45 +1031,52 @@
 ////  set_number_of_ghosts
 ////
 ////////////////////////////////
 
 void ParallelAtoms::set_number_of_ghosts(int nGhosts)
 {
   this->nGhosts = nGhosts;
-  ASSERT(py_atoms != NULL);
+  assert(py_atoms != NULL);
   // First, place a pointer to this object in the Python object to
   // detect if two different ParallelAtoms objects try to use ghosts
   // at the same time.
+#if PY_VERSION_HEX < 0x02070000
+  PyObject *mypointer = PyCObject_FromVoidPtr(this, NULL);
+  if (mypointer == NULL)
+    throw AsapError("Creating PyCObject failed.");
+#else
   PyObject *mypointer = PyCapsule_New(this, "asap3.parallelatoms", NULL);
   if (mypointer == NULL)
     throw AsapError("Creating PyCapsule failed.");
+#endif
   if (PyObject_SetAttrString(py_atoms, mycobject, mypointer) == -1)
     throw AsapError("Failed to set attribute ") << mycobject;
   Py_DECREF(mypointer);
   
   // Now, resize ghost arrays.
   PyObject *py_ghosts = PyObject_GetAttrString(py_atoms, "ghosts");
   if (py_ghosts == NULL)
     throw AsapError("ParallelAtoms::set_number_of_ghosts:: No ghosts found.");
 
-  vector<std::string> array_names;          // Sorted list of array names.
+  vector<const char *> array_names;          // Sorted list of array names.
   vector<PyArrayObject *> arrays;                 // Ghost arrays to resize.
   get_array_names(py_ghosts, array_names);
   get_arrays(py_ghosts, array_names, arrays);
   vector<PyArrayObject *> new_arrays;             // New arrays for ghost data.
   make_new_arrays(new_arrays, arrays, nGhosts);
   release_arrays(arrays, array_names, 2);
   store_arrays(py_ghosts, array_names, new_arrays);
   release_arrays(new_arrays, array_names, 2);
   CHECKREF(py_ghosts);
   Py_DECREF(py_ghosts);
 
   // Finally, resize the vectors used for the position and the atomic numbers
   positions.resize(nAtoms + nGhosts);
-  numbers.resize(nAtoms + nGhosts);
+  if (numbers.size())
+    numbers.resize(nAtoms + nGhosts);
 }
 
 long ParallelAtoms::PrintMemory() const
 {
   long mem = NormalAtoms::PrintMemory();
   long ghmem = 0;  // Count the big stuff.
   for (vector< vector< pair<int, int> > >::const_iterator i = ghosts.begin();
@@ -1144,15 +1098,15 @@
   return mem + mymem;
 }
 
 void ParallelAtoms::CollectFromGhosts(vector<Vec> &data)
 {
   DEBUGPRINT;
   USETIMER("ParallelPotential::CollectFromGhosts");
-  ASSERT(data.size() == nAtoms + nGhosts);
+  assert(data.size() == nAtoms + nGhosts);
   Vec *address = &data[0];
   Vec *ghostAddress = address + nAtoms;
   // Inverse communication from normally.
   const vector <int> *recvlist = domainDecomp->GetSendList();
   const vector <int> *sendlist = domainDecomp->GetRecvList();
   for (int dp = 0; dp < recvlist->size(); dp++)
     {
@@ -1170,22 +1124,22 @@
       typedef vector< pair<int, int> >::const_iterator VP;
       for (VP g = indices.begin(); g != indices.end(); ++g)
         {
           data[g->first] += *(b++);
         }
       mpi->Wait();
     }
-  ASSERT(ghostAddress - &data[0] == nAtoms + nGhosts);
+  assert(ghostAddress - &data[0] == nAtoms + nGhosts);
 }
 
 void ParallelAtoms::CollectFromGhosts(vector<SymTensor> &data)
 {
   DEBUGPRINT;
   USETIMER("ParallelPotential::CollectFromGhosts");
-  ASSERT(data.size() == nAtoms + nGhosts);
+  assert(data.size() == nAtoms + nGhosts);
   SymTensor *address = &data[0];
   SymTensor *ghostAddress = address + nAtoms;
   // Inverse communication from normally.
   const vector <int> *recvlist = domainDecomp->GetSendList();
   const vector <int> *sendlist = domainDecomp->GetRecvList();
   for (int dp = 0; dp < recvlist->size(); dp++)
     {
@@ -1203,20 +1157,38 @@
       typedef vector< pair<int, int> >::const_iterator VP;
       for (VP g = indices.begin(); g != indices.end(); ++g)
         {
           data[g->first] += *(b++);
         }
       mpi->Wait();
     }
-  ASSERT(ghostAddress - &data[0] == nAtoms + nGhosts);
+  assert(ghostAddress - &data[0] == nAtoms + nGhosts);
 }
 
-  // Issue a warning if there are no atoms in the simulation, but only the first time.
-void ParallelAtoms::NoAtomsErrorOrWarning()
+void ParallelAtoms::SetPrimaryNbLocator(PyObject *nblocator)
 {
-  if (not haswarned_noatoms)
-  {
-    cerr << endl << "WARNING: No atoms on process number " << nProcessor << endl;
-    haswarned_noatoms = true;
-  }
+  PyObject *wref = PyWeakref_NewRef(nblocator, NULL);
+  if (wref == NULL)
+    throw AsapPythonError();
+  int x = PyObject_SetAttrString(py_atoms, "_asap_primary_nblist", wref);
+  Py_DECREF(wref);
+  if (x == -1)
+    throw AsapPythonError();
+}
+
+PyObject *ParallelAtoms::GetPrimaryNbLocator(PyObject *pyatoms)
+{
+  if (!PyObject_HasAttrString(pyatoms, "_asap_primary_nblist"))
+    return NULL;   // Not set.  This is not an error!
+  PyObject *wref = PyObject_GetAttrString(pyatoms, "_asap_primary_nblist");
+  if (wref == NULL)
+    throw AsapPythonError();
+  PyObject *locator = PyWeakref_GetObject(wref);
+  Py_DECREF(wref);
+  if (locator == NULL)
+    throw AsapPythonError();
+  if (locator == Py_None)
+    return NULL;  // Weak reference is dead.  This is not an error.
+  Py_INCREF(locator);  // Return a new reference
+  return locator;
 }
```

### Comparing `asap3-3.13.1/Parallel/ParallelAtoms.h` & `asap3-3.9.6/Parallel/ParallelAtoms.h`

 * *Files 6% similar despite different names*

```diff
@@ -93,15 +93,15 @@
   /// the flag passed as an argument is updated if just one processor
   /// thinks an update is necessary.  If the flag is true, a migration
   /// will also be triggered in a parallel simulation.  Finally,
   /// ghost atoms are created.
   virtual bool UpdateBeforeCalculation(bool flag, double range);
 
       /// Get a set of all elements present in the simulations.
-  virtual void GetListOfElements(set<int> &elements);
+  virtual void GetListOfElements(set<int> &elements) const;
 
   /// Distribute the atoms on the processors after creating them.
 
   /// Distribute should be called \em after the atoms have been
   /// created and any extra data in Python arrays (velocities etc) has
   /// been registered, but \em before the atoms are used for anything.
   void Distribute();
@@ -133,66 +133,76 @@
   ///
   /// This is used if a potential needs to communicate some kind of
   /// date during the energy/force calculations.  If the data should
   /// be communicated at the beginning of the calculation, it should
   /// instead be placed in a ghost array.
   virtual void CommunicateData(double *address, int n = 1);
 
-  /// Issue a if there are no atoms in the simulation.
-  virtual void NoAtomsErrorOrWarning();
-
+  /// Set the primary neighbor list in a PARALLEL simulation.
+  ///
+  /// The neighborlist locator is stored in the original Python
+  /// atoms object as a weak reference under the name _asap_primary_nblist
+  virtual void SetPrimaryNbLocator(PyObject *nblocator);
+
+  /// Get the primary neighbor list in a PARALLEL simulation.
+  ///
+  /// Ignored in serial simulations.  Returns a NEW reference
+  /// to the actual locator object (after dereferencing the weak
+  /// reference, or NULL if the weakref has expired or never been
+  /// set).
+  virtual PyObject *GetPrimaryNbLocator(PyObject *pyatoms);
 
 
   /// Print memory usage
   virtual long PrintMemory() const;
   
   /// Receive and sum up data from ghost atoms (inverse communication).
   ///
   /// Used to sum up the forces.
   void CollectFromGhosts(vector<Vec> &data);
   void CollectFromGhosts(vector<SymTensor> &data);
 
+private:
+  /// Check that all atoms are present exactly once.
+  void CheckIdentities();
+
   /// Update data (positions, atomic numbers, ...) on ghost atoms.
   ///
   /// This is called from UpdateBeforeCalculation right after
   /// calling DecorateWithGhosts; and from Begin if the atoms have
   /// been modified since last time it was called.
   void UpdateGhostData();
 
-private:
-  /// Check that all atoms are present exactly once.
-  void CheckIdentities();
-
   /// Create ghost atoms.  This is called from UpdateBeforeCalculation.
   void DecorateWithGhosts(double range);
 
   /// Take new boundary conditions into account.
   virtual void NewBoundaryConditions(const bool newperiodic[3]);
   
   /// Get the number of cells from the Python object.
   void extract_ncells(PyObject *pyatoms);
 
   /// Get a sorted list of array names.
-  void get_array_names(PyObject *dict, vector<std::string> &names);
+  void get_array_names(PyObject *dict, vector<const char *> &names);
 
   /// Get a list of array objects.
-  void get_arrays(PyObject *dict, vector<std::string> &names,
+  void get_arrays(PyObject *dict, vector<const char *> &names,
 		  vector<PyArrayObject *> &arrays);
 
   /// Make a set of new arrays corresponding to a set of old arrays
   void make_new_arrays(vector<PyArrayObject *> &newarrays,
 		       vector<PyArrayObject *> &oldarrays,
 		       int size);
 
   /// Release references to arrays
-  void release_arrays(vector<PyArrayObject *> &arrays, vector<std::string> &names,
+  void release_arrays(vector<PyArrayObject *> &arrays, vector<const char *> &names,
 		      int maxrefcount);
 
   /// Store arrays into a dictionary.
-  void store_arrays(PyObject *dict, vector<std::string> &names,
+  void store_arrays(PyObject *dict, vector<const char *> &names,
 		    vector<PyArrayObject *> &arrays);
   
   /// Store the max range where the ghosts are valid.  Negative: no ghosts yet.
   void set_ghost_range(double range);
 
   /// Read the max range where the ghosts are valid.  Negative: no ghosts yet.
   double get_ghost_range();
@@ -207,16 +217,15 @@
   int nProcessors;              ///< The number of processors
   Communicator *mpi;            ///< This object does the actual communication.
   DomainDecomposition *domainDecomp; ///< Decides where atoms belong.
   int nTotalAtoms;              ///< Sum of the number of atoms on all nodes.
   int migrationCounter;         ///< Counts each time atoms migrate.
   vector<char> sendBuffer;      ///< Buffor for outbound communication
   vector<char> receiveBuffer;   ///< Buffer for inbound communication
-  bool haswarned_noatoms;       ///< We only warn once against a cpu without atoms.
-  
+
   /// The ghost export list.
   ///
   /// This is a list of the ghost atoms on other processors which need
   /// to be updated from this one.
   ///
   /// ghosts is a list with one element for each processor.
   ///
```

### Comparing `asap3-3.13.1/Parallel/ParallelPotential.cpp` & `asap3-3.9.6/Parallel/ParallelPotential.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,24 @@
 #include "Debug.h"
 #include <set>
 using std::cerr;
 using std::endl;
 using std::flush;
 using std::set;
 
-ParallelPotential::ParallelPotential(PyObject *self, PyObject *p, int verbose) :
-  Potential(self, verbose), py_potential(NULL)
+ParallelPotential::ParallelPotential(PyObject *self, PyObject *p) : Potential(self), py_potential(NULL)
 {
   CONSTRUCTOR;
   DEBUGPRINT;
   par_atoms = NULL;
   if (!PyAsap_PotentialCheck(p))
     throw AsapError("Expected an Asap potential, got a ")
       << Py_TYPE(p)->tp_name;
   potential = ((PyAsap_PotentialObject *) p)->cobj;
-  ASSERT(potential != NULL);
+  assert(potential != NULL);
   if (!potential->Parallelizable())
     throw AsapError("This potential cannot be used in parallel simulations");
   py_potential = p;
   stress_collect_cnt = force_collect_cnt = 0;
   Py_INCREF(py_potential);
   DEBUGPRINT;
 }
@@ -62,23 +61,23 @@
     AsapAtoms_DECREF(par_atoms);
 }
 
 void ParallelPotential::SetAtoms(PyObject *pyatoms,
 				 Atoms* accessobj /* = NULL */)
 {
   DEBUGPRINT;
-  ASSERT(accessobj == NULL);
-  par_atoms = new ParallelAtoms(pyatoms, verbose);
+  assert(accessobj == NULL);
+  par_atoms = new ParallelAtoms(pyatoms);
   atoms = par_atoms;
   potential->SetAtoms_ThroughPython(pyatoms, par_atoms);
   mpi = par_atoms->GetCommunicator();
   // This MAY have changed the Potential object as an ImagePotential may
   // have been intercalated.
   potential = ((PyAsap_PotentialObject *) py_potential)->cobj;
-  ASSERT(mpi != NULL);
+  assert(mpi != NULL);
   DEBUGPRINT;
 }
 
 bool ParallelPotential::CalcReq_Energy(PyObject *a)
 {
   USETIMER("ParallelPotential::CalcReq_Energy");
   return mpi->LogicalOr(potential->CalcReq_Energy(a));
@@ -92,18 +91,18 @@
 
 bool ParallelPotential::CalcReq_Virials(PyObject *a)
 {
   USETIMER("ParallelPotential::CalcReq_Virials");
   return mpi->LogicalOr(potential->CalcReq_Virials(a));
 }
 
-bool ParallelPotential::CalcReq_Virial(PyObject *a)
+bool ParallelPotential::CalcReq_Stress(PyObject *a)
 {
-  USETIMER("ParallelPotential::CalcReq_Virial");
-  return mpi->LogicalOr(potential->CalcReq_Virial(a));
+  USETIMER("ParallelPotential::CalcReq_Stress");
+  return mpi->LogicalOr(potential->CalcReq_Stress(a));
 }
 
 double ParallelPotential::GetPotentialEnergy(PyObject *a)
 {
   USETIMER("ParallelPotential::GetPotentialEnergy");
   return mpi->Add(potential->GetPotentialEnergy(a));
 }
@@ -130,42 +129,42 @@
         const vector<Vec> &orig_forces = potential->GetForces(a);
         forces = orig_forces;
         par_atoms->CollectFromGhosts(forces);
         forces.resize(par_atoms->GetNumberOfAtoms());
         force_collect_cnt = cnt;
       }
   }
-  catch (AsapErrorBase &)
+  catch (AsapErrorBase)
   {
       atoms->End();
       throw;
   }
   par_atoms->End();
   DEBUGPRINT;
   return forces;
 }
 
 const vector<SymTensor> &ParallelPotential::GetVirials(PyObject *a)
 {
-  USETIMER("ParallelPotential::GetVirialss");
+  USETIMER("ParallelPotential::GetStresses");
   DEBUGPRINT;
   par_atoms->Begin(a, true);  // Allow reopen.
   try {
     int cnt = par_atoms->GetPositionsCounter();
     if (stress_collect_cnt != cnt)
       {
         DEBUGPRINT;
         const vector<SymTensor> &orig_stresses = potential->GetVirials(a);
         stresses = orig_stresses;
         par_atoms->CollectFromGhosts(stresses);
         stresses.resize(par_atoms->GetNumberOfAtoms());
         stress_collect_cnt = cnt;
       }
   }
-  catch (AsapErrorBase &)
+  catch (AsapErrorBase)
   {
       atoms->End();
       throw;
   }
   par_atoms->End();
   DEBUGPRINT;
   return stresses;
@@ -177,15 +176,35 @@
   DEBUGPRINT;
   SymTensor stress = potential->GetVirial(a);
   vector<double> s1(6);
   for (int i = 0; i < 6; i++)
     s1[i] = stress[i];
   vector<double> s2;
   mpi->Add(s1, s2);
-  ASSERT(s2.size() == 6);
+  assert(s2.size() == 6);
+  for (int i = 0; i < 6; i++)
+    stress[i] = s2[i];
+  DEBUGPRINT;
+  return stress;
+}
+
+SymTensor ParallelPotential::GetStress(PyObject *a)
+{
+  // Find contribution from own atoms to stress.  Potential::GetStress will
+  // call Potential::GetStresses, which then calls ParallelPotential::GetVirials
+  // which then calls potential->GetVirials.
+  DEBUGPRINT;
+  SymTensor stress = Potential::GetStress(a);
+  // Then sum them up
+  vector<double> s1(6);
+  for (int i = 0; i < 6; i++)
+    s1[i] = stress[i];
+  vector<double> s2;
+  mpi->Add(s1, s2);
+  assert(s2.size() == 6);
   for (int i = 0; i < 6; i++)
     stress[i] = s2[i];
   DEBUGPRINT;
   return stress;
 }
 
 void ParallelPotential::GetAtomicVolumes(vector<double> &volumes)
@@ -200,19 +219,14 @@
 // }
 
 PyObject *ParallelPotential::GetNeighborList() const
 {
   return potential->GetNeighborList();
 }
 
-bool ParallelPotential::CheckAndUpdateNbList(PyObject *pyatoms)
-{
-  return potential->CheckAndUpdateNbList(pyatoms);
-}
-
 double ParallelPotential::GetCutoffRadius() const
 {
   return potential->GetCutoffRadius();
 }
 
 double ParallelPotential::GetLatticeConstant() const
 {
@@ -220,14 +234,7 @@
 }
 
 long ParallelPotential::PrintMemory() const
 {
   return potential->PrintMemory();
 }
 
-void ParallelPotential::PyUpdateGhosts(PyObject *a)
-{
-  // Only for calling from Python in a few special cases
-  par_atoms->Begin(a);
-  par_atoms->UpdateGhostData();
-  par_atoms->End();
-}
```

### Comparing `asap3-3.13.1/Parallel/ParallelPotential.h` & `asap3-3.9.6/Parallel/ParallelPotential.h`

 * *Files 12% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 class Communicator;
 
 
 class ParallelPotential : public Potential
 {
 public:
   /// Create a parallel wrapper for the serial potential p
-  ParallelPotential(PyObject *self, PyObject *p, int verbose);
+  ParallelPotential(PyObject *self, PyObject *p);
 
   virtual ~ParallelPotential();
 
-  virtual string GetName() const {return "ParallelPotential(" + potential->GetName() + ")";}
+  virtual string GetName() const {return "ParallelPotential";}
 
   /// Print memory usage
   virtual long PrintMemory() const;
 
   /// Set the atoms belonging to this potential.
 
   /// This is called automatically by Atoms.SetCalculator() and should
@@ -64,56 +64,44 @@
   /// Calculate the forces on all atoms and return the result.
   virtual const vector<Vec> &GetForces(PyObject *a);
 
   /// Calculate the stress on all atoms.
   virtual const vector<SymTensor> &GetVirials(PyObject *a);
 
   /// Calculate the total stress of the system.
+  virtual SymTensor GetStress(PyObject *a);
   virtual SymTensor GetVirial(PyObject *a);
 
   /// Calculate the energy of all atoms.
   virtual const vector<double> &GetPotentialEnergies(PyObject *a);
 
   virtual bool CalcReq_Energy(PyObject *pyatoms);
   virtual bool CalcReq_Forces(PyObject *pyatoms);
-  virtual bool CalcReq_Virial(PyObject *pyatoms);
+  virtual bool CalcReq_Stress(PyObject *pyatoms);
   virtual bool CalcReq_Virials(PyObject *pyatoms);
 
   /// Return the neighbor list.
 
   /// Return the Python object containing neighbor list for the
   /// potential, if this type of potential supports it, and if it is
   /// defined now.  Otherwise, return NULL without setting a Python
   /// error.
   virtual PyObject *GetNeighborList() const;
 
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
-
-
   /// Return the cutoff radius used in the potential.
   virtual double GetCutoffRadius() const;
 
   /// Return the lattice constant of the material, if well-defined.
 
   /// If a lattice constant of the material can be defined, return it
   /// in Angstrom, otherwise throw an exception.
   virtual double GetLatticeConstant() const;
 
   virtual void GetAtomicVolumes(vector<double> &volumes);
 
-  /// Update data on ghost atoms
-  ///
-  /// This is only used for analysis functions in Python.
-  virtual void PyUpdateGhosts(PyObject *a);
-
 private:
   PyObject *py_potential;   ///< The wrapped potential (Python object)
   Potential *potential;     ///< The wrapped potential (C++ object)
   ParallelAtoms *par_atoms; ///< Parallel access to atoms.
   Communicator *mpi;        ///< The communicator object.
   vector<Vec> forces;       ///< Forces after gathering contributions from ghosts.
   vector<SymTensor> stresses; ///< Stresses after gathering contributions from ghosts.
```

### Comparing `asap3-3.13.1/Parallel/RegularGridDecomposition.cpp` & `asap3-3.9.6/Parallel/RegularGridDecomposition.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -51,25 +51,16 @@
       originalPeriodicity[i] = periodic[i];
       this->superCell[i] = superCell[i];
     }
   nTotalCells[0] = 1;
   for (int i = 0; i < 3; i++)
     nTotalCells[i + 1] = nTotalCells[i] * nCells[i];
   this->comm = comm;
-  ASSERT(nProcs == comm->GetNumberOfProcessors());
+  assert(nProcs == comm->GetNumberOfProcessors());
   thisProcessor = comm->GetProcessorNumber();
-  if (verbose > 2)
-  {
-    cerr << "Creating RegularGridDecomposition on process " << thisProcessor << " of " << nProcs << endl;
-    cerr << "  with a grid of " << nCells[0] << ", " << nCells[1] << ", " << nCells[2] << ", " << endl;
-    cerr << "  and a supercell of:" << endl;
-    cerr << "    " << superCell[0] << endl;
-    cerr << "    " << superCell[1] << endl;
-    cerr << "    " << superCell[2] << endl;
-  }
   InitializeNeighborsTable();
 #if 0
   if (thisProcessor == 0)
     {
       cerr << "RegularGridDecomposition neighbor table:" << endl;
       for (int i = 0; i < 27; i++)
         {
@@ -140,30 +131,30 @@
   const Vec *x = &positions[0];
   for (int a = 0; a < nAtoms; a++)
     {
       int proc = 0;
       for (int i = 0; i < 3; i++)
 	{
           int k = int(((*x)[i] - minimum[i]) / size[i] * nCells[i]);
-          ASSERT(k >= 0);
+          assert(k >= 0);
           if (k == nCells[i])
             k--;
-          ASSERT(k < nCells[i]);
+          assert(k < nCells[i]);
           proc += nTotalCells[i] * k;
 	}
-      ASSERT(proc >= 0);
-      ASSERT(proc < nProcs);
+      assert(proc >= 0);
+      assert(proc < nProcs);
       x++;
       if (proc != thisProcessor)
         {
           processor[proc].push_back(a);
           migrateAway.push_back(a);
         }
     }
-  if (verbose >= 3)
+  if (verbose >= 2)
     {
       cerr << "RegularGridDecomposition (Node " << thisProcessor 
            << "): Sending to other processors: [";
       for (int i = 0; i < nProcs; i++)
         cerr << " " << processor[i].size();
       cerr << " ]" << endl;
     }
@@ -210,15 +201,15 @@
 	    for (int j = 0; j < nAtoms; j++)
 	      positions[j][i] -= soffset[j][i];
 	}
       Py_DECREF(py_soffset);
       atoms->DeleteData(offsetname);
     }
 
-  if (verbose > 2)
+  if (verbose > 1)
     cerr << thisProcessor << ':' << minimum << " <> " << minimum + size
          << endl
          << nAtoms << " atoms on "
          << nCells[0] << " * " << nCells[1] << " * " << nCells[2] 
          << " processors" << endl;
 
   // Find out which atoms are ghost atoms on which processors:
@@ -237,15 +228,15 @@
               n += dn;
           }
       typedef vector< pair<int, int> >::const_iterator VP;
       for (VP nb = neighbors[n].begin(); nb != neighbors[n].end(); ++nb)
         ghostLists[nb->first].push_back(pair<int, int>(a, nb->second));
       ++p;
     }
-  ASSERT(p == positions.end());
+  assert(p == positions.end());
 }
 
     
 void RegularGridDecomposition::smallestBox(vector<Vec> &positions,
 					   const bool* originalPeriodicity,
                                            int nAtoms, Vec &minimum, Vec &size)
 {
@@ -289,24 +280,24 @@
               min = 1e99;
               max = -1e99;
             }
           min = comm->Min(min);
           max = comm->Max(max);
           minimum[i] = min;
           size[i] = max - min;
-          ASSERT(max > -1e99 && min < 1e99);
+          assert(max > -1e99 && min < 1e99);
           if (size[i] < 1e-7)
             {
               minimum[i] -= 0.5 * (1e-7 - size[i]);
               size[i] = 1e-7;
             }
         }
     }
     
-  if (verbose > 2)
+  if (verbose > 1)
     cerr << "Node " << thisProcessor << ':' << minimum << " "
          << minimum + size << "   "
          << nAtoms << " atoms on "
          << nCells[0] << " * " << nCells[1] << " * " << nCells[2] 
          << " processors" << endl;
 }
 
@@ -383,15 +374,15 @@
   recvlist.clear();
   // Find the position of this processor in the grid
   int n = thisProcessor;
   int selfi = n % nCells[0];
   n = n / nCells[0];
   int selfj = n % nCells[1];
   int selfk = n / nCells[1];
-  if (verbose > 2)
+  if (verbose)
     cerr << "I am processor " << thisProcessor << " at location "
 	 << selfi << "," << selfj << "," << selfk << endl;
   // Loop over neighboring positions, +/- 1 in each direction if the grid is
   // big enough
   int imin = nCells[0] > 2 ? -1 : 0;
   int imax = nCells[0] > 1 ? 1 : 0;
   int jmin = nCells[1] > 2 ? -1 : 0;
@@ -422,29 +413,29 @@
           if (node_r[i] < 0) node_r[i] += nCells[i];
           if (node_r[i] >= nCells[i]) node_r[i] -= nCells[i];
         }
         int sendto = nTotalCells[0] * node_s[0]
           + nTotalCells[1] * node_s[1] + nTotalCells[2] * node_s[2];
         int recvfrom = nTotalCells[0] * node_r[0]
           + nTotalCells[1] * node_r[1] + nTotalCells[2] * node_r[2];
-        ASSERT((sendto >= 0) && (recvfrom >= 0));
-        ASSERT((sendto < nProcs) && (recvfrom < nProcs));
+        assert((sendto >= 0) && (recvfrom >= 0));
+        assert((sendto < nProcs) && (recvfrom < nProcs));
         if ((is != 0) || (js != 0) || (ks != 0)) {
           sendlist.push_back(sendto);
           recvlist.push_back(recvfrom);
         } else {
-	  if (verbose > 2)
+	  if (verbose)
 	    cerr << "DEBUG: sendto=" << sendto << " is=" << is << " js="
 		 << js << " ks=" << ks << endl;
-          ASSERT(sendto == thisProcessor);
+          assert(sendto == thisProcessor);
         }
       }
     }
   }
-  if (verbose > 2) {
+  if (verbose) {
     cerr << "Send list:    ";
     for (vector<int>::iterator i = sendlist.begin(); i != sendlist.end(); ++i)
       cerr << *i << " ";
     cerr << endl;
     cerr << "Receive list: ";
     for (vector<int>::iterator i = recvlist.begin(); i != recvlist.end(); ++i)
       cerr << *i << " ";
```

### Comparing `asap3-3.13.1/Parallel/RegularGridDecomposition.h` & `asap3-3.9.6/Parallel/RegularGridDecomposition.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/ParallelInterface/AsapParallel.cpp` & `asap3-3.9.6/Tools/CoordinationNumbers.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-// Copyright (C) 2008-2011 Jakob Schiotz and Center for Individual
+// -*- C++ -*-
+//
+// Copyright (C) 2002-2011 Jakob Schiotz and Center for Individual
 // Nanoparticle Functionality, Department of Physics, Technical
 // University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
 //
 // This program is free software: you can redistribute it and/or
 // modify it under the terms of the GNU Lesser General Public License
@@ -17,24 +19,22 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-#define PARALLEL
-#include "mpimodule.h"
-#include "ParallelAtomsInterface.h"
-#include "ParallelPotentialInterface.h"
-#include "ParallelNeighborListInterface.h"
+#ifndef _COORDINATIONNUMBERS_H
+#define _COORDINATIONNUMBERS_H
+
+#include "AsapPython.h"
+#include <vector>
 
-// Now include the main code
-#include "AsapModule.cpp"
+namespace ASAPSPACE {
 
+class Atoms;
 
+void CoordinationNumbers(PyObject *py_atoms, double rCut, std::vector<int> &coord);
 
-PyMODINIT_FUNC PyInit__asap(void)
-{
-    return AsapInitModule();
-}
+} // end namespace
 
-  
+#endif // _COORDINATIONNUMBERS_H
```

### Comparing `asap3-3.13.1/ParallelInterface/ParallelAtomsInterface.cpp` & `asap3-3.9.6/ParallelInterface/ParallelAtomsInterface.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -27,29 +27,22 @@
 #include "Potential.h"
 #include "ParallelAtoms.h"
 #include "ParallelAtomsInterface.h"
 #include "ExceptionInterface.h"
 
 namespace ASAPSPACE {
 
-PyObject *PyAsap_DistributeAtoms(PyObject *noself, PyObject *args,
-				 PyObject *kwargs)
+PyObject *PyAsap_DistributeAtoms(PyObject *noself, PyObject *atoms)
 {
-  PyObject *atoms = NULL;
-  int verbose = 0;
-  static char *kwlist[] = {"atoms", "verbose", NULL};
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O|i:DistributeAtoms", kwlist, &atoms, &verbose))
-    return NULL;
-  
   ParallelAtoms *patoms;
   try {
-    patoms = new ParallelAtoms(atoms, verbose);
+    patoms = new ParallelAtoms(atoms);
   }
   CATCHEXCEPTION;
-  ASSERT(patoms != NULL);
+  assert(patoms != NULL);
   try {
     patoms->Begin(atoms);
     CHECKNOASAPERROR;
     patoms->Distribute();
     PROPAGATEASAPERROR;
     patoms->End();
   }
```

### Comparing `asap3-3.13.1/ParallelInterface/ParallelAtomsInterface.h` & `asap3-3.9.6/ParallelInterface/ParallelAtomsInterface.h`

 * *Files 2% similar despite different names*

```diff
@@ -29,13 +29,12 @@
 #ifndef _PARALLEL_ATOMS_INTERFACE_H
 #define _PARALLEL_ATOMS_INTERFACE_H
 
 #include "Asap.h"
 
 namespace ASAPSPACE {
 
-PyObject *PyAsap_DistributeAtoms(PyObject *noself,  PyObject *args,
-				 PyObject *kwargs);
+PyObject *PyAsap_DistributeAtoms(PyObject *noself, PyObject *atoms);
 
 } // end namespace
 
 #endif //_PARALLEL_ATOMS_INTERFACE_H
```

### Comparing `asap3-3.13.1/ParallelInterface/ParallelNeighborListInterface.cpp` & `asap3-3.9.6/ParallelInterface/ParallelNeighborListInterface.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,16 @@
   try {
     DEBUGPRINT;
     PyAsap_NeighborLocatorObject *self =
       PyAsap_NewSecondaryNeighborLocator(access, rCut, driftfactor);
     DEBUGPRINT;
     if (access != NULL)
       AsapAtoms_DECREF(access);
+    DEBUGPRINT;
     if (atoms != Py_None)
-    {
-      DEBUGPRINT;
       self->cobj->CheckAndUpdateNeighborList(atoms);
-    }
     DEBUGPRINT;
     return (PyObject *) self;
   }
   CATCHEXCEPTION;
 }
```

### Comparing `asap3-3.13.1/ParallelInterface/ParallelPotentialInterface.cpp` & `asap3-3.9.6/ParallelInterface/ParallelPotentialInterface.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -41,69 +41,37 @@
 static char ParPot_Docstring[] = "Parallel potential wrapper.\n";
 
 static int PyAsap_ParPotInit(PyAsap_PotentialObject *self, PyObject *args,
 			     PyObject *kwargs)
 {
   if (PyAsap_PotentialType.tp_init((PyObject *)self, args, kwargs) < 0)
     return -1;
-  static char *kwlist[] = {"potential", "verbose", NULL};
+  static char *kwlist[] = {"potential", NULL};
   PyObject *pypot;
-  int verb = 0;
-  if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O|i", kwlist, &pypot, &verb))
+  if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O", kwlist, &pypot))
     return -1;
   if (self->cobj != NULL)
     {
       PyErr_SetString(PyAsap_ErrorObject,				
 		      "ParallelPotential object already initialized.");	
       return -1;							
     }
-  self->cobj = new ParallelPotential((PyObject *)self, pypot, verb);
+  self->cobj = new ParallelPotential((PyObject *)self, pypot);
   if (self->cobj == NULL)
     return -1;
   return 0;
 }
 
-static char PyAsap_ParPotUpdateGhosts_Docstring[] = "Update data on ghost atoms.\n";
-
-static PyObject *PyAsap_ParPotUpdateGhosts(PyAsap_PotentialObject *self,
-					   PyObject *args)
-{
-  PyObject *atoms = NULL;
-  if (!PyArg_ParseTuple(args, "O", &atoms))
-    return NULL;
-  if (self->cobj == NULL)
-    {
-      PyErr_SetString(PyAsap_ErrorObject,
-		      "ParallelPotential object not initialized.");
-      return NULL;
-  }
-  try {
-    ParallelPotential *parpot = dynamic_cast<ParallelPotential *>(self->cobj);
-    ASSERT(parpot != NULL);
-    parpot->PyUpdateGhosts(atoms);
-  }
-  POTCATCHEXCEPTION;
-  Py_RETURN_NONE;
-}
-
-static PyMethodDef PyAsap_ParPotMethods[] = {
-  {"update_ghost_data", (PyCFunction) PyAsap_ParPotUpdateGhosts,
-   METH_VARARGS, PyAsap_ParPotUpdateGhosts_Docstring},
-  {NULL}  // Sentinel
-};
-
-
 namespace ASAPSPACE {
 
 int PyAsap_InitParallelPotentialInterface(PyObject *module)
 {
   InitPotentialType(PyAsap_ParPotType);
   PyAsap_ParPotType.tp_init = (initproc) PyAsap_ParPotInit;
   PyAsap_ParPotType.tp_doc = ParPot_Docstring;
-  PyAsap_ParPotType.tp_methods = PyAsap_ParPotMethods;
   if (PyType_Ready(&PyAsap_ParPotType) < 0)
     return -1;
   Py_INCREF(&PyAsap_ParPotType);
   PyModule_AddObject(module, "ParallelPotential",
 		     (PyObject *) &PyAsap_ParPotType);
   return 0;
 }
```

### Comparing `asap3-3.13.1/ParallelInterface/ParallelPotentialInterface.h` & `asap3-3.9.6/ParallelInterface/ParallelPotentialInterface.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/ParallelInterface/mpimodule.cpp` & `asap3-3.9.6/ParallelInterface/mpi.c`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
 
 #include "AsapPython.h"
-#include "Asap.h"
 #include <structmember.h>
 #include <mpi.h>
-#include <stddef.h>  // for offsetof
 #include "mpimodule.h"
-#include "Templates.h"
 
-#ifdef ASAPDEBUG
+#if ASAPDEBUG
 #include <stdio.h>
 #define DEBUGPRINT fprintf(stderr, "%s:%d  %s\n", __FILE__, __LINE__, __FUNCTION__)
 #else
 #define DEBUGPRINT
 #endif
 
 // #define LONGP(a) ((long*)((a)->data))
@@ -45,20 +42,14 @@
 // Check that array is well-behaved and contains data that can be sent.
 #define CHK_ARRAY(a) if ((a) == NULL                    		\
 			 || !PyArray_ISCARRAY(a) || !PyArray_ISNUMBER(a)) { \
     PyErr_SetString(PyExc_TypeError,					\
 		    "Not a proper NumPy array for MPI communication."); \
     return NULL; }
 
-#define CHK_ARRAY_RO(a) if ((a) == NULL                    		\
-			 || !PyArray_ISCARRAY_RO(a) || !PyArray_ISNUMBER(a)) { \
-    PyErr_SetString(PyExc_TypeError,					\
-		    "Not a proper NumPy array for MPI communication."); \
-    return NULL; }
-
 #define CHK_ARRAY_2(a) if ((a) == NULL || !PyArray_Check(a)             \
                          || !PyArray_ISCARRAY(a) || !PyArray_ISNUMBER(a)) { \
     PyErr_SetString(PyExc_TypeError,                                    \
                     "Not a proper NumPy array for MPI communication."); \
     return NULL; }
 
 // Check that two arrays have the same type, and the size of the
@@ -125,27 +116,27 @@
       Py_DECREF(self->buffer);
       self->status = 0;
       DEBUGPRINT;
       Py_RETURN_TRUE;
     }
   else
     {
-      DEBUGPRINT;
       Py_RETURN_FALSE;
     }
 }
 
-static void mpi_request_finalize(mpi_request *self)
+static void mpi_request_dealloc(mpi_request *self)
 {
   DEBUGPRINT;
   if (self->status)
     {
       DEBUGPRINT;
       mpi_request_wait(self, NULL);
     }
+  PyObject_Del(self);
   DEBUGPRINT;
 }
 
 static PyMemberDef mpi_request_members[] = {
     {"status", T_INT, offsetof(mpi_request, status), READONLY,
         "status of the request, non-zero if communication is pending."},
     {NULL}
@@ -161,18 +152,51 @@
     {NULL}
 };
 
 PyTypeObject mpi_request_type = {
   PyVarObject_HEAD_INIT(&PyType_Type, 0)
     "MPI_Request",             /*tp_name*/
     sizeof(mpi_request),             /*tp_basicsize*/
-  // The rest is initialized by name for reliability.
-};
+    0,                         /*tp_itemsize*/
+    (destructor)mpi_request_dealloc, /*tp_dealloc*/
+    0,                         /*tp_print*/
+    0,                         /*tp_getattr*/
+    0,                         /*tp_setattr*/
+    0,                         /*tp_compare*/
+    0,                         /*tp_repr*/
+    0,                         /*tp_as_number*/
+    0,                         /*tp_as_sequence*/
+    0,                         /*tp_as_mapping*/
+    0,                         /*tp_hash */
+    0,                         /*tp_call*/
+    0,                         /*tp_str*/
+    0,                         /*tp_getattro*/
+    0,                         /*tp_setattro*/
+    0,                         /*tp_as_buffer*/
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE, /*tp_flags*/
+    "MPI request object",           /* tp_doc */
+    0,                   /* tp_traverse */
+    0,                   /* tp_clear */
+    0,                   /* tp_richcompare */
+    0,                   /* tp_weaklistoffset */
+    0,                   /* tp_iter */
+    0,                   /* tp_iternext */
+    mpi_request_methods,             /* tp_methods */
+    mpi_request_members,
+    0,                         /* tp_getset */
+    0,                         /* tp_base */
+    0,                         /* tp_dict */
+    0,                         /* tp_descr_get */
+    0,                         /* tp_descr_set */
+    0,                         /* tp_dictoffset */
+    0,      /* tp_init */
+    0,                         /* tp_alloc */
+    0,                 /* tp_new */
 
-static char mpi_request_type_docstring[] = "MPI request object";
+};
 
 
 static mpi_request *PyAsap_NewMPIRequest()
 {
   mpi_request *self;
   DEBUGPRINT;
 
@@ -180,71 +204,72 @@
   if (self == NULL) return NULL;
   self->buffer = NULL;
   self->status = 1;  // Active
   DEBUGPRINT;
   return self;
 }
 
+static void mpi_dealloc(MPIObject *self)
+{
+  if (self->comm != MPI_COMM_WORLD)
+    {
+      MPI_Comm_free(&(self->comm));
+      CHECKREF(self->parent);
+      Py_XDECREF(self->parent);
+    }
+  Py_TYPE(self)->tp_free(self);
+}
 
 static PyObject * mpi_receive(MPIObject *self, PyObject *args, PyObject *kwargs)
 {
   PyArrayObject* a;
   int src = -1;
   int tag = 123;
   int block = 1;
   static char *kwlist[] = {"a", "src", "tag", "block", NULL};
 
-  DEBUGPRINT;
   if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O!i|ii:receive", kwlist,
 				   &PyArray_Type, &a, &src, &tag, &block))
     return NULL;
   CHK_ARRAY(a);
   if (src != -1)
     {
-      DEBUGPRINT;
       CHK_OTHER_PROC(src);
     }
   else
     src = MPI_ANY_SOURCE;
   int n = PyArray_DESCR(a)->elsize;
   int d;
   for (d = 0; d < PyArray_NDIM(a); d++)
     n *= PyArray_DIM(a, d);
-  DEBUGPRINT;
   if (block)
     {
       MPI_Status status;
-      DEBUGPRINT;
       MPI_Recv(PyArray_BYTES(a), n, MPI_BYTE, src, tag, self->comm,
 	       &status);
-      DEBUGPRINT;
       int real_source = status.MPI_SOURCE;
       return Py_BuildValue("i", real_source);
     }
   else
     {
-      DEBUGPRINT;
       mpi_request *req = PyAsap_NewMPIRequest();
       if (req == NULL) return NULL;
       req->buffer = a;
       Py_INCREF(req->buffer);
-      DEBUGPRINT;
       MPI_Irecv(PyArray_BYTES(a), n, MPI_BYTE, src, tag, self->comm, &(req->rq));
-      DEBUGPRINT;
       return (PyObject *) req;
     }
 }
 
 static PyObject * mpi_probe(MPIObject *self, PyObject *args, PyObject *kwargs)
 {
   int src = -1;
   int tag = -1;
   int block = 0;
   static char *kwlist[] = {"src", "tag", "block", NULL};
-  DEBUGPRINT;
   if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|iii:probe", kwlist,
 				   &src, &tag, &block))
     return NULL;
   
   if (src != -1)
     {
       CHK_OTHER_PROC(src);
@@ -267,59 +292,49 @@
     }
   if (flag)
     {
       src = status.MPI_SOURCE;
       tag = status.MPI_TAG;
       int count;
       MPI_Get_count(&status, MPI_BYTE, &count);
-      DEBUGPRINT;
       return Py_BuildValue("iii", src, tag, count);
     }
   else
-  {
-    DEBUGPRINT;
     Py_RETURN_NONE;
-  }
 }
 
 static PyObject * mpi_send(MPIObject *self, PyObject *args, PyObject *kwargs)
 {
   PyArrayObject* a;
   int dest;
   int tag = 123;
   int block = 1;
   static char *kwlist[] = {"a", "dest", "tag", "block", NULL};
-  DEBUGPRINT;
   if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O!i|ii:send", kwlist,
 				   &PyArray_Type, &a, &dest, &tag, &block))
     return NULL;
   CHK_ARRAY(a);
   CHK_OTHER_PROC(dest);
   int n = PyArray_DESCR(a)->elsize;
   int d;
   for (d = 0; d < PyArray_NDIM(a); d++)
     n *= PyArray_DIM(a,d);
   if (block)
     {
-      DEBUGPRINT;
       MPI_Send(PyArray_BYTES(a), n, MPI_BYTE, dest, tag, self->comm);
-      DEBUGPRINT;
       Py_RETURN_NONE;
     }
   else
     {
-      DEBUGPRINT;
       mpi_request *req = PyAsap_NewMPIRequest();
       if (req == NULL) return NULL;
       req->buffer = a;
       Py_INCREF(a);
-      DEBUGPRINT;
       MPI_Isend(PyArray_BYTES(a), n, MPI_BYTE, dest, tag, self->comm,
 		&(req->rq));
-      DEBUGPRINT;
       return (PyObject *) req;
     }
 }
 
 
 static PyObject * mpi_sendreceive(MPIObject *self, PyObject *args,
                                   PyObject *kwargs)
@@ -577,34 +592,34 @@
       double dout;
       if (root == -1)
         MPI_Allreduce(&din, &dout, 1, MPI_DOUBLE, operation, self->comm);
       else
         MPI_Reduce(&din, &dout, 1, MPI_DOUBLE, operation, root, self->comm);
       return PyFloat_FromDouble(dout);
     }
-  if (PyLong_Check(obj))
+  if (PyAsapInt_Check(obj))
     {
-      long din = PyLong_AsLong(obj);
+      long din = PyAsapInt_AsLong(obj);
       long dout;
       if (root == -1)
         MPI_Allreduce(&din, &dout, 1, MPI_LONG, operation, self->comm);
       else
         MPI_Reduce(&din, &dout, 1, MPI_LONG, operation, root, self->comm);
       return Py_BuildValue("l", dout);
     }
   else if (PyComplex_Check(obj) && allowcomplex)
     {
       double din[2];
       double dout[2];
       din[0] = PyComplex_RealAsDouble(obj);
       din[1] = PyComplex_ImagAsDouble(obj);
       if (root == -1)
-        MPI_Allreduce(&din, &dout, 2, MPI_DOUBLE, operation, self->comm);
+        MPI_Allreduce(&din, &dout, 2, MPI_DOUBLE, MPI_SUM, self->comm);
       else
-        MPI_Reduce(&din, &dout, 2, MPI_DOUBLE, operation, root, self->comm);
+        MPI_Reduce(&din, &dout, 2, MPI_DOUBLE, MPI_SUM, root, self->comm);
       return PyComplex_FromDoubles(dout[0], dout[1]);
     }
   else if (PyComplex_Check(obj))
     {
       PyErr_SetString(PyExc_ValueError,
 		      "Operation not allowed on complex numbers");
       return NULL;
@@ -768,33 +783,21 @@
 
 static PyObject * mpi_broadcast(MPIObject *self, PyObject *args)
 {
   PyArrayObject* buf;
   int root;
   if (!PyArg_ParseTuple(args, "O!i:broadcast", &PyArray_Type, &buf, &root))
     return NULL;
-  
-  // We may need to send from a non-contiguous array (but the receiving must be contiguous)
-  if (self->rank == root)
-  {
-    buf = PyArray_GETCONTIGUOUS(buf);
-    CHK_ARRAY_RO(buf);
-  }
-  else
-  {
-    Py_INCREF((PyObject *) buf);  // So we can decref later
-    CHK_ARRAY(buf);
-  }
+  CHK_ARRAY(buf);
   CHK_PROC(root);
   int n = PyArray_DESCR(buf)->elsize;
   int d;
   for (d = 0; d < PyArray_NDIM(buf); d++)
     n *= PyArray_DIM(buf,d);
   MPI_Bcast(PyArray_BYTES(buf), n, MPI_BYTE, root, self->comm);
-  Py_DECREF(buf);  // Release eventual copy of data
   Py_RETURN_NONE;
 }
 
 // Forward declaration of MPI_Communicator because it needs MPIType
 // that needs MPI_getattr that needs MPI_Methods that need
 // MPI_Communicator that need ...
 static PyObject * MPICommunicator(MPIObject *self, PyObject *args);
@@ -839,18 +842,17 @@
      "min(a, root=-1) minimum of arrays or scalars, result on all tasks unless root is given."},
     {"scatter",          (PyCFunction)mpi_scatter,      METH_VARARGS,
      "scatter(src, target, root) distributes array from root task."},
     {"gather",           (PyCFunction)mpi_gather,       METH_VARARGS,
      "gather(src, root, target=None) gathers data from all tasks on root task."},
     {"all_gather",       (PyCFunction)mpi_allgather,    METH_VARARGS,
      "all_gather(src, target) gathers data from all tasks on all tasks."},
-    {"broadcast",        (PyCFunction)mpi_broadcast,    METH_VARARGS,
-     "broadcast(buffer, root) Broadcast data in-place from root task."},
+    {"broadcast",        (PyCFunction)mpi_broadcast,    METH_VARARGS, 0},
     {"new_communicator", (PyCFunction)MPICommunicator,  METH_VARARGS,
-     "create a new communicator"},
+     "broadcast(buffer, root) Broadcast data in-place from root task."},
     {0, 0, 0, 0}
 };
 
 static PyMemberDef mpi_members[] = {
   {"size", T_INT, offsetof(MPIObject, size), 0, "Number of processors"},
   {"rank", T_INT, offsetof(MPIObject, rank), 0, "Number of this processor"},
   {0, 0, 0, 0, 0}  /* Sentinel */
@@ -864,19 +866,17 @@
   
   if (! PyArg_ParseTupleAndKeywords(args, kwds, "", kwlist))
     return NULL;
 
   self = (MPIObject *) type->tp_alloc(type, 0);
   if (self == NULL)
     return NULL;
-  self->cobj = new Communicator();
-  assert(self->cobj != NULL);
-  self->comm = self->cobj->get_mpi_comm();
-  MPI_Comm_size(self->comm, &(self->size));
-  MPI_Comm_rank(self->comm, &(self->rank));
+  MPI_Comm_size(MPI_COMM_WORLD, &(self->size));
+  MPI_Comm_rank(MPI_COMM_WORLD, &(self->rank));
+  self->comm = MPI_COMM_WORLD;
   self->parent = NULL;
   
   return (PyObject *) self;
 }
 
 // __init__
 static int InitMPIObject(MPIObject* self, PyObject *args, PyObject *kwds)
@@ -885,47 +885,71 @@
 
   if (! PyArg_ParseTupleAndKeywords(args, kwds, "", kwlist))
     return -1;
 
   return 0;
 }
 
-// __del__
-static void DelMPIObject(MPIObject* self)
-{
-  DEBUGPRINT;
-  if (self->cobj != NULL)  // Should always be true, but asserts not allowed here.
-    delete self->cobj;
-  self->cobj = NULL;
-  DEBUGPRINT;
-}
-
 PyTypeObject MPIType = {
   PyVarObject_HEAD_INIT(&PyType_Type, 0)
   "MPI",             /*tp_name*/
   sizeof(MPIObject),             /*tp_basicsize*/
-  // The rest is initialized by name for reliability.
-};
+  0,                         /*tp_itemsize*/
+  (destructor)mpi_dealloc, /*tp_dealloc*/
+  0,                         /*tp_print*/
+  //  mpi_get_attr,                         /*tp_getattr*/
+  0,                         /*tp_getattr*/
+  0,                         /*tp_setattr*/
+  0,                         /*tp_compare*/
+  0,                         /*tp_repr*/
+  0,                         /*tp_as_number*/
+  0,                         /*tp_as_sequence*/
+  0,                         /*tp_as_mapping*/
+  0,                         /*tp_hash */
+  0,                         /*tp_call*/
+  0,                         /*tp_str*/
+  0,                         /*tp_getattro*/
+  0,                         /*tp_setattro*/
+  0,                         /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE, /*tp_flags*/
+  "MPI object",           /* tp_doc */
+  0,                   /* tp_traverse */
+  0,                   /* tp_clear */
+  0,                   /* tp_richcompare */
+  0,                   /* tp_weaklistoffset */
+  0,                   /* tp_iter */
+  0,                   /* tp_iternext */
+  mpi_methods,             /* tp_methods */
+  mpi_members,
+    0,                         /* tp_getset */
+    0,                         /* tp_base */
+    0,                         /* tp_dict */
+    0,                         /* tp_descr_get */
+    0,                         /* tp_descr_set */
+    0,                         /* tp_dictoffset */
+    (initproc)InitMPIObject,      /* tp_init */
+    0,                         /* tp_alloc */
+    NewMPIObject,                 /* tp_new */
 
-static char MPIType_docstring[] = "MPI object";
+};
 
 static PyObject * MPICommunicator(MPIObject *self, PyObject *args)
 {
   PyArrayObject* ranks;
   if (!PyArg_ParseTuple(args, "O!", &PyArray_Type, &ranks))
     return NULL;
   MPI_Group group;
   MPI_Comm_group(self->comm, &group);
   int n = PyArray_DIMS(ranks)[0];
   MPI_Group newgroup;
   // Stupid hack; MPI_Group_incl wants a int argument;
   // numpy arrays are long (might be different from ints)
   // More clever ways are welcomed...
   int* ranks_int = GPAW_MALLOC(int, n);
-  long* ranks_long = (long *) PyArray_DATA(ranks);
+  long* ranks_long = PyArray_DATA(ranks);
   int i;
   for (i = 0; i < n ; i++ )
     ranks_int[i]=ranks_long[i];
   MPI_Group_incl(group, n, ranks_int, &newgroup);
   free(ranks_int);
   MPI_Comm comm;
   MPI_Comm_create(self->comm, newgroup, &comm);
@@ -947,39 +971,21 @@
       // don't want MPI_Finalize to be called before MPI_Comm_free):
       Py_INCREF(self);
       obj->parent = (PyObject*)self;
       return (PyObject*)obj;
     }
 }
 
-namespace ASAPSPACE {
-
 int PyAsap_InitMpiInterface(PyObject *module)
 {
-  MPIType.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HAVE_FINALIZE;
-  MPIType.tp_doc = MPIType_docstring;
-  MPIType.tp_methods = mpi_methods;
-  MPIType.tp_members = mpi_members;
-  MPIType.tp_init = (initproc)InitMPIObject;
-  MPIType.tp_new = NewMPIObject;
-  MPIType.tp_finalize = (destructor)DelMPIObject;
-  MPIType.tp_finalize = PyAsap_Dealloc;
   if (PyType_Ready(&MPIType) < 0)
     return -1;
-
-  mpi_request_type.tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HAVE_FINALIZE;
-  mpi_request_type.tp_doc = mpi_request_type_docstring;
-  mpi_request_type.tp_methods = mpi_request_methods;
-  mpi_request_type.tp_members = mpi_request_members;
-  mpi_request_type.tp_finalize = (destructor)mpi_request_finalize;
-  mpi_request_type.tp_finalize = PyAsap_Dealloc;
   if (PyType_Ready(&mpi_request_type) < 0)
     return -1;
 
   Py_INCREF(&MPIType);
   Py_INCREF(&mpi_request_type);
   PyModule_AddObject(module, "Communicator", (PyObject *)&MPIType);
 
   return 0;
 }
   
-} // namespace
```

### Comparing `asap3-3.13.1/ParallelInterface/mpimodule.h` & `asap3-3.9.6/ParallelInterface/mpimodule.h`

 * *Files 8% similar despite different names*

```diff
@@ -24,27 +24,26 @@
 // see <http://www.gnu.org/licenses/>.
 
 
 #ifndef _MPIMODULE_H
 #define _MPIMODULE_H
 #include <Python.h> /* Not AsapPython.h as that would break AsapParallel.cpp */
 #include <mpi.h>
-#include "AsapMPI.h"
-#include "Asap.h"
-
-namespace ASAPSPACE {
 
 typedef struct
 {
   PyObject_HEAD
   int size;
   int rank;
-  MPI_Comm comm;   // Remove real soon now.
-  Communicator *cobj;    
+  MPI_Comm comm;
   PyObject* parent;
 } MPIObject;
 
+#ifdef __cplusplus
+extern "C" {
+#endif
 int PyAsap_InitMpiInterface(PyObject *module);
-
-} // end namespace
+#ifdef __cplusplus
+}
+#endif
 
 #endif /* _MPIMODULE_H */
```

### Comparing `asap3-3.13.1/Potentials/EMT.cpp` & `asap3-3.9.6/Basics/EMT.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -23,18 +23,14 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-// Note: The macro ASAP_FOR_KIM is undefined when this file is
-// compiled as part of Asap, but is defined when it is part of the
-// OpenKIM model driver.
-
 #include "EMT.h"
 #include "Asap.h"
 #include "EMTParameterProvider.h"
 #include "Atoms.h"
 #include "Vec.h"
 #include "NeighborLocator.h"
 #ifndef ASAP_FOR_KIM
@@ -46,17 +42,14 @@
 #include "Debug.h"
 #include <math.h>
 #include <vector>
 #include <set>
 #include <cstdio>
 #include <iostream>
 #include <algorithm>
-#ifdef ASAP_MKL
-#include "mkl.h"
-#endif //ASAP_MKL
 using std::vector;
 using std::set;
 using std::cerr;
 using std::endl;
 using std::flush;
 using std::sort;
 
@@ -172,47 +165,33 @@
     mem += nblist->PrintMemory();
   return mem + atomsmem;
 }
 
 void EMT::SetAtoms(PyObject *pyatoms, Atoms* accessobj /* = NULL */)
 {
   DEBUGPRINT;
-  VERB("SetAtoms ");
   if (atoms != NULL)
     {
       // SetAtoms should only do anything the first time it is called.
       // Subsequent calls should just check for accessobj being NULL.
       if (accessobj != NULL && accessobj != atoms)
 	throw AsapError("EMT::SetAtoms called multiple times with accessobj != NULL");
-      // If SetAtoms is called multiple times, it should only check that no new element
-      // is introduced.
-      set<int> elements_set;
-      atoms->Begin(pyatoms);
-      atoms->GetListOfElements(elements_set);
-      atoms->End();
-      set<int> parameters_set;
-      for (int i = 0; i < parameters.size(); i++)
-      {
-	parameters_set.insert(parameters[i]->Z);
-      }
-      for (set<int>::iterator i = elements_set.begin(); i != elements_set.end(); i++)
-	if (parameters_set.find(*i) == parameters_set.end())
-	  throw AsapError("You cannot introduce a new element after initializing EMT calculator: Z=") << *i;
+      // SetAtoms should not do anything if called more than once!
       return;
     }
 
   // The first time SetAtoms is being called some initialization is done.
   if (accessobj != NULL)
     {
       atoms = accessobj;
       AsapAtoms_INCREF(atoms);
     }
   else
     atoms = new NormalAtoms();
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   nAtoms = atoms->GetNumberOfAtoms();
   nSize = nAtoms;
     
   InitParameters();
   initialized = true;
   if (nelements == 1)
@@ -317,23 +296,23 @@
   // Extract the elements from the list of atoms.
   // elements.clear();
   atoms->GetListOfElements(elements_set);
   for (set<int>::iterator i = elements_set.begin(); i != elements_set.end();
        ++i)
     elements.push_back(*i);
   nelements = elements.size();
-  ASSERT(nelements == elements_set.size());
+  assert(nelements == elements_set.size());
   sort(elements.begin(), elements.end());
 	
   // Get the EMT parameters
   parameters.clear();
   for (vector<int>::iterator i = elements.begin(); i != elements.end(); ++i)
     parameters.push_back(provider->GetParameters(*i));
 
-  //ASSERT(nelements == provider->GetNumberOfElements());
+  //assert(nelements == provider->GetNumberOfElements());
     
   // Calculate the quantities that can only be calculated, once the
   // elements in the simulations are known.
   provider->CalcGammaEtc();
   rFermi = provider->GetCutoffDistance();
   //rNbCut = 1.04500185048 * rFermi;
   rNbCut = provider->GetListCutoffDistance();
@@ -354,15 +333,15 @@
 }
 
 const vector<Vec> &EMT::GetForces(PyObject *pyatoms)
 {
   USETIMER("EMT::GetForces")
   DEBUGPRINT;
   VERB(" Force[");
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   recalc.nblist = CheckNeighborList();
   recalc.forces = (counters.forces != atoms->GetPositionsCounter());
   if (recalc.forces)
     {
       recalc.ids = (counters.ids != atoms->GetPositionsCounter());
       recalc.sigma1 = (counters.sigma1 != atoms->GetPositionsCounter());
@@ -373,15 +352,15 @@
       counters.beforeforces = atoms->GetPositionsCounter(); 
       counters.forces = atoms->GetPositionsCounter();
       VERB("]" << flush);
     }
   else
     {
       VERB("-]");
-      ASSERT(recalc.nblist == false);
+      assert(recalc.nblist == false);
     }
   DEBUGPRINT;
   atoms->End();
   MEMORY;
   DEBUGPRINT;
   return force;
 }
@@ -410,25 +389,20 @@
 {
   atoms->Begin(pyatoms);
   bool required = (counters.virials != atoms->GetPositionsCounter());
   atoms->End();
   return required;
 }
 
-bool EMT::CalcReq_Virial(PyObject *pyatoms)
-{
-  return CalcReq_Virials(pyatoms);
-}
-
 const vector<SymTensor> &EMT::GetVirials(PyObject *pyatoms)
 {
   USETIMER("EMT::GetVirials")
   DEBUGPRINT;
   VERB(" Virials[");
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
 
   recalc.nblist = CheckNeighborList();
   recalc.virials = (counters.virials != atoms->GetPositionsCounter());
   if (recalc.virials)
     {
       recalc.ids = (counters.ids != atoms->GetPositionsCounter());
@@ -439,15 +413,15 @@
       DEBUGPRINT;
       if (this->virials.size() == 0)
         AllocateStress();
       CalculateVirials();
     }
   else
     {
-      ASSERT(recalc.nblist == false);
+      assert(recalc.nblist == false);
     }
   VERB("]" << flush);
   DEBUGPRINT;
   counters.virials = atoms->GetPositionsCounter();
   counters.beforeforces = atoms->GetPositionsCounter(); 
   counters.forces = atoms->GetPositionsCounter();
   atoms->End();
@@ -475,17 +449,17 @@
       }
       PROPAGATEASAPERROR;
     }
 }
 
 void EMT::GetAtomicVolumes(vector<double> &v)
 {
-  v.resize(nAtoms);
+  v.resize(nSize);
   const double fourpithird = 4.1887902048;  // 4 * PI / 3
-  for (int i = 0; i < nAtoms; i++)
+  for (int i = 0; i < nSize; i++)
     {
       double s0 = parameters[id[i]]->seq;
       v[i] = fourpithird * s0 * s0 * s0;
     }
 }
 
 bool EMT::CalcReq_Energy(PyObject *pyatoms)
@@ -497,15 +471,15 @@
 }
 
 const vector<double> &EMT::GetPotentialEnergies(PyObject *pyatoms)
 {
   USETIMER("EMT::GetPotentialEnergies");
   DEBUGPRINT;
   VERB(" Energies[");
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   // Atoms may already be open if called from MonteCarloEMT object.
   if (!skip_begin)
     atoms->Begin(pyatoms);
   else
     skip_begin = false;
   recalc.nblist = CheckNeighborList();
   recalc.energies = (counters.energies != atoms->GetPositionsCounter());
@@ -519,27 +493,27 @@
       DEBUGPRINT;
       CalculateEnergies();
       counters.energies = atoms->GetPositionsCounter();
       counters.beforeforces = atoms->GetPositionsCounter(); 
     }
   else
     {
-      ASSERT(counters.beforeforces == atoms->GetPositionsCounter());
-      ASSERT(recalc.nblist == false);
+      assert(counters.beforeforces == atoms->GetPositionsCounter());
+      assert(recalc.nblist == false);
       
       if(subtractE0)
 	for (int i = 0; i < nAtoms; i++)
 	  Epot[i] = Ec[i] + Eas[i] - parameters[id[i]]->e0;
       else
 	for (int i = 0; i < nAtoms; i++)
 	  Epot[i] = Ec[i] + Eas[i];
 
       VERB("-");
     }
-  ASSERT(Epot.size() == nAtoms);
+  assert(Epot.size() == nAtoms);
   DEBUGPRINT;
   VERB("]" << flush);
   atoms->End();
   return Epot;
 }
 
 void EMT::CalculateEnergies()
@@ -569,32 +543,20 @@
   for (int i = 0; i < nAtoms; i++)
     etot += e[i];
   DEBUGPRINT;
   VERB("]" << flush);
   return etot;
 }
 
-
-bool EMT::CheckAndUpdateNbList(PyObject *pyatoms)
-{
-  atoms->Begin(pyatoms);
-  recalc.nblist = CheckNeighborList();
-  if (recalc.nblist)
-    UpdateNeighborList();
-  atoms->End();
-  return recalc.nblist;
-}
-
-
 bool EMT::CheckNeighborList()
 {
   RETURNIFASAPERROR2(false);
   USETIMER("EMT::CheckNeighborList");
   DEBUGPRINT;
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   bool update = (nblist == NULL) || nblist->IsInvalid();  // Update if invalid
   if (!update && (counters.nblist != atoms->GetPositionsCounter()))
     {
       VERB("n");
       update = nblist->CheckNeighborList();
     }
   // May communicate
@@ -737,26 +699,23 @@
       else
         {
           VERB("1");
         }
   }
 
   DEBUGPRINT;
+  // const Vec *pos = atoms->GetPositions();
   int maxnblen = nblist->MaxNeighborListLength();
   if (maxnblen > BUFLEN)
     {
       const Vec *cell = atoms->GetCell();
       THROW_RETURN( AsapError("Neighborlist overrun (did you squeeze your atoms?).\n")
 		    << "  Longest neighbor list is " << maxnblen << ".\n"
 		    << "  Cell is " << cell[0] << ", " << cell[1] << ", " << cell[2] );
     }
-#ifdef ASAP_FOR_KIM
-  const int *contributes = atoms->GetParticleContributes();
-  ASSERT(nAtoms == nSize);  // In OpenKIM, non-contributing atoms are not always at the end.
-#endif
   // Buffer data:
   TinyMatrix<int> nbatch(nelements,nelements);
   TinyMatrix<int[BUFLEN]> self(nelements,nelements);
   TinyMatrix<int[BUFLEN]> other(nelements,nelements);
   TinyMatrix<Vec[BUFLEN]> rnb(nelements,nelements);
   TinyMatrix<double[BUFLEN]> sqdist(nelements,nelements);
   vector<int> other_buf(BUFLEN);
@@ -790,17 +749,14 @@
 
   // Loop over atoms
 #ifdef _OPENMP
 #pragma omp for
 #endif // _OPENMP
   for (int atom = 0; atom < nAtoms; atom++)
     {
-#ifdef ASAP_FOR_KIM
-      if (!contributes[atom]) continue;   // Skip non-contributing atoms.
-#endif     
       int zself = id[atom];
       // Get neighbors and loop over them.  Simplest if only one element
       if (nelements == 1) 
         {
           int nbat = nbatch[0][0];  // only element
           int size = BUFLEN-nbat;
           int n;
@@ -808,30 +764,30 @@
             n = nblist->GetFullNeighbors(atom, other[0][0]+nbat,
                                          rnb[0][0]+nbat, sqdist[0][0]+nbat,
                                          size);
           else
             n = nblist->GetNeighbors(atom, other[0][0]+nbat,
                                      rnb[0][0]+nbat, sqdist[0][0]+nbat,
                                      size);
-          ASSERT(size >= 0);    // REMOVE LATER !!!
+          assert(size >= 0);    // REMOVE LATER !!!
           for (int i = nbat; i < nbat+n; i++)
             self[0][0][i] = atom;
           nbatch[0][0] += n;
         } 
       else 
         {
           int size = BUFLEN;
           int n;
           if (always_fullnblist)
             n = nblist->GetFullNeighbors(atom, &other_buf[0], &rnb_buf[0],
                                          &sqdist_buf[0], size);
           else
             n = nblist->GetNeighbors(atom, &other_buf[0], &rnb_buf[0],
                                      &sqdist_buf[0], size);
-          ASSERT(size >= 0);     // REMOVE LATER !!!
+          assert(size >= 0);     // REMOVE LATER !!!
 	  int *RESTRICT id = &(this->id)[0];
           for (int i = 0; i < n; i++) 
             {
               int zother = id[other_buf[i]];
               int nbat = nbatch[zself][zother]++;  // Count this atom
               self[zself][zother][nbat] = atom;
               other[zself][zother][nbat] = other_buf[i];
@@ -870,41 +826,28 @@
 }
 
 void EMT::sigma_batch(int *RESTRICT self, int *RESTRICT other,
                       double *RESTRICT sq_dist, int zs, int zo, int n,
                       bool calculatesigma2, bool partialupdate /* = false */)
 {
   USETIMER("EMT::sigma_batch");
-#ifdef ASAP_MKL
-  double *temporary = (double *) mkl_malloc(10 * BUFLEN * sizeof(double), ASAP_MKL_ALIGN);
-#else // ASAP_MKL
   double *temporary = new double[4*BUFLEN];
-#endif //ASAP_MKL
   double *RESTRICT dsigma1s = &temporary[0];
   double *RESTRICT dsigma2s = dsigma1s + BUFLEN;
   double *RESTRICT dsigma1o = dsigma2s + BUFLEN;
   double *RESTRICT dsigma2o = dsigma1o + BUFLEN;
-  //ASSERT(dsigma2o - temporary == (4 - 1) * BUFLEN);
-#ifdef ASAP_MKL
-  double *RESTRICT tmp_a = dsigma2o + BUFLEN;
-  double *RESTRICT tmp_b = tmp_a + BUFLEN;
-  double *RESTRICT tmp_c = tmp_b + BUFLEN;
-  double *RESTRICT tmp_d = tmp_c + BUFLEN;
-  double *RESTRICT tmp_e = tmp_d + BUFLEN;
-  double *RESTRICT tmp_f = tmp_e + BUFLEN;
-  //ASSERT(tmp_f - temporary == (10 - 1) * BUFLEN);
-#endif //ASAP_MKL  
+  assert(dsigma2o - temporary == (4 - 1) * BUFLEN);
   double cutslopecutdist;
   double other_eta2betaseq, self_eta2betaseq;
   double other_kappaoverbeta, self_kappaoverbeta;
   double other_kappaseq, self_kappaseq;
   double *s1s, *s1o, *s2s, *s2o;
   const emt_parameters *emtself, *emtother;
 
-  ASSERT(n <= BUFLEN);
+  assert(n <= BUFLEN);
   
   /* Get EMT parameters   REWRITE !!! XXXX */  
   emtself = parameters[zs];
   emtother = parameters[zo];
   double cutoffslope = this->cutoffslope;
   cutslopecutdist = cutoffslope * rFermi;
   other_eta2betaseq = emtother->eta2 * Beta * emtother->seq;
@@ -912,178 +855,82 @@
   other_kappaoverbeta = emtother->kappa / Beta;
   self_kappaoverbeta = emtself->kappa / Beta;
   other_kappaseq = emtother->kappa * emtother->seq;
   self_kappaseq = emtself->kappa * emtself->seq;
   double other_eta2 = emtother->eta2;
   double self_eta2 = emtself->eta2;
 
-  ASSERT(n <= BUFLEN);
+  assert(n <= BUFLEN);
   // We have four cases to handled, controlled by two booleans.
   // 1) Whether sigma2 needs to be calculated,  2) Whether we need a
   // different calculation for the two atoms interacting.  The latter is
   // the case if the atomic numbers are different, unless operating in
   // full neighborlist mode or doing a partial update for MonteCarloEMT,
   // in these cases calculations are not reused.
   bool calculateother = (zs != zo) && !always_fullnblist && !partialupdate;
   if (!calculateother && !calculatesigma2)
     {
-#ifdef ASAP_MKL
-      // dist[] = tmp_a[] = sqrt(sq_dist[])
-      vdSqrt(n, sq_dist, tmp_a);
-      for (int i = 0; i < n; i++)
-	{
-	  tmp_b[i] = cutoffslope * tmp_a[i] - cutslopecutdist;
-	  tmp_c[i] = -other_eta2 * tmp_a[i] + other_eta2betaseq;
-	}
-      // tmp_a[] = exp(tmp_b[]) = exp(cutoffslope * dist[] - cutslopecutdist)
-      vdExp(n, tmp_b, tmp_a);
-      // tmp_b[] = exp(tmp_c[]) = exp(-other_eta2 * dist[] + other_eta2betaseq)
-      vdExp(n, tmp_c, tmp_b);
-      for (int i = 0; i < n; i++)
-	{
-	  double wght = 1.0 / (1.0 + tmp_a[i]);
-	  dsigma1s[i] = wght * tmp_b[i];
-	}
-#else  // ASAP_MKL
       for (int i = 0; i < n; i++)
 	{
 	  /* dist = sqrt(sq_dist),  distances between atoms */
 	  double dist = sqrt(sq_dist[i]);
 	  /* Calculate weight factor (cutoff function) */
 	  double wght = 1.0 / (1.0 + exp(cutoffslope * dist
 					 - cutslopecutdist));
 	  /* Contribution to sigma1 */
 	  dsigma1s[i] = wght * exp(-other_eta2 * dist + other_eta2betaseq);
 	}
-#endif // ASAP_MKL
     }
   else if (calculateother && !calculatesigma2)
     {
-#ifdef ASAP_MKL
-      // dist[] = tmp_a[] = sqrt(sq_dist[])
-      vdSqrt(n, sq_dist, tmp_a);
-      for (int i = 0; i < n; i++)
-	{
-	  tmp_b[i] = cutoffslope * tmp_a[i] - cutslopecutdist;
-	  tmp_c[i] = -other_eta2 * tmp_a[i] + other_eta2betaseq;
-	  tmp_d[i] = -self_eta2 * tmp_a[i] + self_eta2betaseq;
-	}
-      // tmp_a[] = exp(tmp_b[]) = exp(cutoffslope * dist[] - cutslopecutdist)
-      vdExp(n, tmp_b, tmp_a);
-      // tmp_b[] = exp(tmp_c[]) = exp(-other_eta2 * dist[] + other_eta2betaseq)
-      vdExp(n, tmp_c, tmp_b);
-      // tmp_c[] = exp(tmp_d[]) = exp(-self_eta2 * dist[] + self_eta2betaseq)
-      vdExp(n, tmp_d, tmp_c);
-      for (int i = 0; i < n; i++)
-	{
-	  double wght = 1.0 / (1.0 + tmp_a[i]);
-	  dsigma1s[i] = wght * tmp_b[i];
-	  dsigma1o[i] = wght * tmp_c[i];
-	}
-#else // ASAP_MKL
       for (int i = 0; i < n; i++)
 	{
 	  /* dist = sqrt(sq_dist),  distances between atoms */
 	  double dist = sqrt(sq_dist[i]);
 	  /* Calculate weight factor (cutoff function) */
 	  double wght = 1.0 / (1.0 + exp(cutoffslope * dist
 					 - cutslopecutdist));
 	  /* Contributions to sigma1 */
 	  dsigma1s[i] = wght * exp(-other_eta2 * dist + other_eta2betaseq);
 	  dsigma1o[i] = wght * exp(-self_eta2 * dist + self_eta2betaseq);
 	}
-#endif //ASAP_MKL
     }
   else if (!calculateother && calculatesigma2)
     {
-#ifdef ASAP_MKL
-      // dist[] = tmp_a[] = sqrt(sq_dist[])
-      vdSqrt(n, sq_dist, tmp_a);
-      for (int i = 0; i < n; i++)
-	{
-	  tmp_b[i] = cutoffslope * tmp_a[i] - cutslopecutdist;
-	  tmp_c[i] = -other_eta2 * tmp_a[i] + other_eta2betaseq;
-	  tmp_d[i] = -other_kappaoverbeta * tmp_a[i] + other_kappaseq;
-	}
-      // tmp_a[] = exp(tmp_b[]) = exp(cutoffslope * dist[] - cutslopecutdist)
-      vdExp(n, tmp_b, tmp_a);
-      // tmp_b[] = exp(tmp_c[]) = exp(-other_eta2 * dist[] + other_eta2betaseq)
-      vdExp(n, tmp_c, tmp_b);
-      // tmp_c[] = exp(tmp_d[]) = exp(-other_kappaoverbeta * dist[] + other_kappaseq)
-      vdExp(n, tmp_d, tmp_c);
-      for (int i = 0; i < n; i++)
-	{
-	  double wght = 1.0 / (1.0 + tmp_a[i]);
-	  dsigma1s[i] = wght * tmp_b[i];
-	  dsigma2s[i] = wght * tmp_c[i];
-	}
-#else // ASAP_MKL
       for (int i = 0; i < n; i++)
 	{
 	  /* dist = sqrt(sq_dist),  distances between atoms */
 	  double dist = sqrt(sq_dist[i]);
 
 	  /* Calculate weight factor (cutoff function) */
 	  double wght = 1.0 / (1.0 + exp(cutoffslope * dist
 					 - cutslopecutdist));
 	  /* Contribution to sigma1 */
 	  dsigma1s[i] = wght * exp(-other_eta2 * dist + other_eta2betaseq);
 	  dsigma2s[i] = wght * exp(-other_kappaoverbeta * dist
 					+ other_kappaseq);
 
 	}
-#endif //ASAP_MKL
    }
   else // calculateother && calculatesigma2
     {
-#ifdef ASAP_MKL
-      // dist[] = tmp_a[] = sqrt(sq_dist[])
-      vdSqrt(n, sq_dist, tmp_a);
-      for (int i = 0; i < n; i++)
-	{
-	  tmp_b[i] = cutoffslope * tmp_a[i] - cutslopecutdist;
-	  tmp_c[i] = -other_eta2 * tmp_a[i] + other_eta2betaseq;
-	  tmp_d[i] = -self_eta2 * tmp_a[i] + self_eta2betaseq;
-	  tmp_e[i] = -other_kappaoverbeta * tmp_a[i] + other_kappaseq;
-	  tmp_f[i] = -self_kappaoverbeta * tmp_a[i] + self_kappaseq;
-	}
-      // tmp_a[] = exp(tmp_b[]) = exp(cutoffslope * dist[] - cutslopecutdist)
-      vdExp(n, tmp_b, tmp_a);
-      // tmp_b[] = exp(tmp_c[]) = exp(-other_eta2 * dist[] + other_eta2betaseq)
-      vdExp(n, tmp_c, tmp_b);
-      // tmp_c[] = exp(tmp_d[]) = exp(-self_eta2 * dist[] + self_eta2betaseq)
-      vdExp(n, tmp_d, tmp_c);
-      // tmp_d[] = exp(tmp_e[]) = exp(-other_kappaoverbeta * dist[] + other_kappaseq)
-      vdExp(n, tmp_e, tmp_d);
-      // tmp_e[] = exp(tmp_f[]) = exp(-self_kappaoverbeta * dist[] + self_kappaseq)
-      vdExp(n, tmp_f, tmp_e);
-      for (int i = 0; i < n; i++)
-	{
-	  double wght = 1.0 / (1.0 + tmp_a[i]);
-	  dsigma1s[i] = wght * tmp_b[i];
-	  dsigma1o[i] = wght * tmp_c[i];
-	  dsigma2s[i] = wght * tmp_d[i];
-	  dsigma2o[i] = wght * tmp_e[i];
-	}
-#else // ASAP_MKL
       for (int i = 0; i < n; i++)
 	{
 	  /* dist = sqrt(sq_dist),  distances between atoms */
 	  double dist = sqrt(sq_dist[i]);
 	  /* Calculate weight factor (cutoff function) */
 	  double wght = 1.0 / (1.0 + exp(cutoffslope * dist
 					 - cutslopecutdist));
 	  /* Contributions to sigma1 */
 	  dsigma1s[i] = wght * exp(-other_eta2 * dist + other_eta2betaseq);
 	  dsigma1o[i] = wght * exp(-self_eta2 * dist + self_eta2betaseq);
 	  dsigma2s[i] = wght * exp(-other_kappaoverbeta * dist
 				   + other_kappaseq);
 	  dsigma2o[i] = wght * exp(-self_kappaoverbeta * dist + self_kappaseq);
 	}
-#endif // ASAP_MKL
     }
 
   // Distribute the results to the atoms.
   if (!partialupdate && !always_fullnblist)
     {
       // This is the normal branch, both atoms need to be updated.
       if (calculatesigma2) 
@@ -1166,15 +1013,14 @@
     }
   else  // partialupdate OR always_fullnblist
     {
       // This branch may be taken by MonteCarloEMT during a partial update,
       // or by the normal EMT when not using Minimum Image Convention.  Since
       // full neighbor lists are used, only update the
       // 'self' atom, not the 'other' atom.
-      // In OpenKIM, this branch is always taken.
       if (calculatesigma2)
         {
           /* Distribute contributions to sigma1 and sigma2 */
           s1o = &sigma1[zo][0];
           s2o = &sigma2[zo][0];
     #ifdef _OPENMP
     #pragma omp critical
@@ -1200,19 +1046,15 @@
               {
                 int s = self[i];
                 s1o[s] += dsigma1s[i];
               }
           }
         }
     }
-#ifdef ASAP_MKL
-  mkl_free(temporary);
-#else
   delete[] temporary;
-#endif
 }
 
 
 // Calculate the energies if calc_Epot is true, otherwise just calculate the
 // derivatives needed for the forces. 
 void EMT::CalculateEnergiesAfterSigmas(bool calc_Epot)
 {
@@ -1224,15 +1066,15 @@
   double *RESTRICT sigma = &tmp_double[0];
   bool dosigmapart = (recalc.beforeforces || (calc_Epot && recalc.energies));
   bool doepotpart = (calc_Epot && recalc.energies);
   
   int zs, zo;
   double s;
   // Better performance if static ???
-  ASSERT(nelements < NMAXELEMENTS);
+  assert(nelements < NMAXELEMENTS);
   double inv12gamma1[NMAXELEMENTS];
   double neginvbetaeta2[NMAXELEMENTS];
   double neglambda[NMAXELEMENTS];
   double lambdaseq[NMAXELEMENTS];
   double negkappa[NMAXELEMENTS];
   double kappaseq[NMAXELEMENTS];
   double nege0lambdalambda[NMAXELEMENTS];
@@ -1264,15 +1106,15 @@
           int zs = id[i];
           for (int zo = 0; zo < nelements; zo++)
             s += (*chi)[zs][zo] * sigma1[zo][i];
           if (s < 1.0e-40)
             s = 1.0e-40;
           sigma[i] = s;
         }
-      ASSERT(nAtoms == radius.size() && nAtoms == Ec.size() &&
+      assert(nAtoms == radius.size() && nAtoms == Ec.size() &&
              nSize == dEds.size());
     }
 
   /* Calculate conbinations of EMT parameters */
   for (int i = 0; i < nelements; i++)
     {
      inv12gamma1[i] = 1.0 / (12.0 * parameters[i]->gamma1);
@@ -1337,16 +1179,16 @@
 #pragma omp master
 #endif // _OPENMP
           {
             VERB("e");
             DEBUGPRINT;
           }
           /* We also need Eas, but only for the real atoms */
-          ASSERT(sigma2isvalid);
-          ASSERT(counters.sigma2 == atoms->GetPositionsCounter());
+          assert(sigma2isvalid);
+          assert(counters.sigma2 == atoms->GetPositionsCounter());
           /* Calculate total sigma2 */
 #ifdef _OPENMP
 #pragma omp for
 #endif // _OPENMP
           for (int i = 0; i < nAtoms; i++)
             {
               s = 0.0;
@@ -1371,23 +1213,14 @@
 #ifdef _OPENMP
 #pragma omp for
 #endif // _OPENMP
           for (int i = 0; i < nAtoms; i++)
             Epot[i] = Ec[i] + Eas[i];
         }
     } // if (calc_Epot)
-  
-#ifdef ASAP_FOR_KIM
-  // In OpenKIM, nAtoms == nSize and the non-contributing atoms had
-  // their energies calculates.  Zap them.
-  const int *contributes = atoms->GetParticleContributes();
-  for (int i = 0; i < nAtoms; i++)
-    if (!contributes[i])
-      Epot[i] = Ec[i] = Eas[i] = dEds[i] = 0;
-#endif // ASAP_FOR_KIM
     
   DEBUGPRINT;    
 }
 
 void EMT::CalculateForcesAfterEnergies()
 {
   RETURNIFASAPERROR;
@@ -1416,29 +1249,25 @@
   TinyMatrixOfVector<vector<double> > sqdist(nelements,nelements, BUFLEN);
   TinyMatrixOfVector<vector<double> > dEdss(nelements,nelements, BUFLEN);
   TinyMatrixOfVector<vector<double> > dEdso(nelements,nelements, BUFLEN);
   vector<int> other_buf(BUFLEN);
   vector<Vec> rnb_buf(BUFLEN);
   vector<double> sqdist_buf(BUFLEN);
 
-#ifdef ASAP_FOR_KIM
-  const int *contributes = atoms->GetParticleContributes();
-#endif
-  
   // If there is only one element, CalculateForcesAfterEnergiesSingle should
   // be used.
-  ASSERT(nelements > 1);
+  assert(nelements > 1);
 
   int nSize = this->nSize;  // Helps optimization.
   Vec *RESTRICT force = &(this->force)[0];
   
   /* Set forces and virials to zero */
   if (virials.size())
     {
-      ASSERT(virials.size() == nSize);
+      assert(virials.size() == nSize);
 #ifdef _OPENMP
 #pragma omp for nowait
 #endif // _OPENMP
       for (int i = 0; i < nSize; i++)
         for (int j = 0; j < 6; j++)
           virials[i][j] = 0.0;
     }
@@ -1456,28 +1285,25 @@
       nbatch[i][j] = 0;
 
   // Loop over atoms
 #ifdef _OPENMP
 #pragma omp for
 #endif // _OPENMP
   for (int atom = 0; atom < nAtoms; atom++) {
-#ifdef ASAP_FOR_KIM
-    if (!contributes[atom]) continue;  // Skip non-contributing atom in OpenKIM, where nAtoms == nSize.
-#endif
     int zself = id[atom];
     // Get neighbors and loop over them.
     int size = BUFLEN;
     int n;
     if (always_fullnblist)
       n = nblist->GetFullNeighbors(atom, &other_buf[0], &rnb_buf[0],
                                    &sqdist_buf[0], size);
     else
       n = nblist->GetNeighbors(atom, &other_buf[0], &rnb_buf[0],
                                &sqdist_buf[0], size);
-    ASSERT(size >= 0);    // REMOVE LATER
+    assert(size >= 0);    // REMOVE LATER
     for (int i = 0; i < n; i++) {
       int zother = id[other_buf[i]];
       int nbat = nbatch[zself][zother]++;  // Count this atom
       self[zself][zother][nbat] = atom;
       other[zself][zother][nbat] = other_buf[i];
       rnb[zself][zother][nbat][0] = rnb_buf[i][0];
       rnb[zself][zother][nbat][1] = rnb_buf[i][1];
@@ -1535,32 +1361,28 @@
   vector<int> self(BUFLEN);
   vector<int> other(BUFLEN);
   vector<Vec> rnb(BUFLEN);
   vector<double> sqdist(BUFLEN);
   vector<double> dEdss(BUFLEN);
   vector<double> dEdso(BUFLEN);
 
-#ifdef ASAP_FOR_KIM
-  const int *contributes = atoms->GetParticleContributes();
-#endif
-  
   int nSize = this->nSize;   // These three lines help optimization.
   int nAtoms = this->nAtoms;
   Vec *RESTRICT force = &(this->force)[0];
   
   DEBUGPRINT;
   // If there is more than one element, CalculateForcesAfterEnergies should
   // be used.
-  ASSERT(nelements == 1);
+  assert(nelements == 1);
       
   /* Set forces and virials to zero */
-  ASSERT(this->force.size() >= nSize);
+  assert(this->force.size() >= nSize);
   if (virials.size())
     {
-      ASSERT(virials.size() == nSize);
+      assert(virials.size() == nSize);
 #ifdef _OPENMP
 #pragma omp for nowait
 #endif // _OPENMP
       for (int i = 0; i < nSize; i++)
         for (int j = 0; j < 6; j++)
           virials[i][j] = 0.0;
     }
@@ -1579,18 +1401,14 @@
   // Loop over atoms
   DEBUGPRINT;
 #ifdef _OPENMP
 #pragma omp for
 #endif // _OPENMP
   for (int atom = 0; atom < nAtoms; atom++) {
 
-#ifdef ASAP_FOR_KIM
-    if (!contributes[atom]) continue;  // Skip non-contributing atom in OpenKIM, where nAtoms == nSize.
-#endif
-
     // Get neighbors and loop over them.
     int size = BUFLEN-nbatch;
     int n;
     if (always_fullnblist)
       n = nblist->GetFullNeighbors(atom, &other[nbatch], &rnb[nbatch],
                                    &sqdist[nbatch], size);
     else
@@ -1627,37 +1445,24 @@
 // same reason, the temporary array is not a vector<>.
 void EMT::force_batch(const int *RESTRICT self, const int *RESTRICT other,
                       const Vec *RESTRICT rnb, const double *RESTRICT sq_dist,
                       const double *RESTRICT dEdss, const double *RESTRICT dEdso,
                       int zs, int zo, int n)
 {
   USETIMER("EMT::force_batch");
-#ifdef ASAP_MKL
-  double *temporary = (double *) mkl_malloc(8 * BUFLEN * sizeof(double), ASAP_MKL_ALIGN);
-  double *RESTRICT df = temporary;
-  double *RESTRICT tmp_a = df + BUFLEN;
-  double *RESTRICT tmp_b = tmp_a + BUFLEN;
-  double *RESTRICT tmp_c = tmp_b + BUFLEN;
-  double *RESTRICT tmp_d = tmp_c + BUFLEN;
-  double *RESTRICT tmp_e = tmp_d + BUFLEN;
-  double *RESTRICT tmp_f = tmp_e + BUFLEN;
-  double *RESTRICT tmp_g = tmp_f + BUFLEN;
-  //ASSERT(tmp_g - temporary == (8 - 1) * BUFLEN);
-#else // ASAP_MKL
   double *temporary = new double[BUFLEN];
   double *RESTRICT df = temporary;
-#endif // ASAP_MKL
   double cutslopecutdist, other_eta2betaseq, other_kappaoverbeta;
   double other_kappaseq, self_eta2betaseq, self_kappaoverbeta;
   double self_kappaseq, cnst_s, cnst_o;
   const emt_parameters *emtself, *emtother;
   //double pairA, exprcut, pairD;
   //double *tmp;
 
-  ASSERT(n <= BUFLEN);
+  assert(n <= BUFLEN);
   
   /* Get EMT parameters */
   emtself = parameters[zs];
   emtother = parameters[zo];
   cutslopecutdist = cutoffslope * rFermi;
   other_eta2betaseq = emtother->eta2 * Beta * emtother->seq;
   other_kappaoverbeta = emtother->kappa / Beta;
@@ -1670,49 +1475,17 @@
 
   cnst_s = -0.5 * emtself->V0 * (*chi)[zs][zo] / emtself->gamma2;
   cnst_o = -0.5 * emtother->V0 * (*chi)[zo][zs] / emtother->gamma2;
   double chi_zs_zo = (*chi)[zs][zo];
   double chi_zo_zs = (*chi)[zo][zs];
   // Three cases: 1) The two atoms have the same atomic number,
   // 2) they have different atomic number (less reuse of calculations)
-  // 3) we use full neighbor lists (no reuse).
+  // 3) we use full neighbor lists (no resuls).
   if ((zs == zo) && !always_fullnblist)
     { 
-#ifdef ASAP_MKL
-      /* Get the distances from their squares */
-      // dist[] = tmp_a[] = sqrt(sq_dist[])
-      vdSqrt(n, sq_dist, tmp_a);
-      // invdist[] = tmp_e[] = 1.0 / dist[]
-      vdInv(n, tmp_a, tmp_e);
-      for (int i = 0; i < n; i++)
-        {
-	  tmp_b[i] = cutoffslope * tmp_a[i] - cutslopecutdist;
-	  tmp_c[i] = -other_eta2 * tmp_a[i] + other_eta2betaseq;
-	  tmp_d[i] = -other_kappaoverbeta * tmp_a[i] + other_kappaseq;
-	}
-      // tmp_a[] = exp(tmp_b[]) = exp(cutoffslope * dist[] - cutslopecutdist)
-      vdExp(n, tmp_b, tmp_a);
-      // tmp_b[] = exp(tmp_c[]) = exp(-other_eta2 * dist[] + other_eta2betaseq)
-      vdExp(n, tmp_c, tmp_b);
-      // tmp_c[] = exp(tmp_d[]) = exp(-other_kappaoverbeta * dist[] + other_kappaseq)
-      vdExp(n, tmp_d, tmp_c);
-      for (int i = 0; i < n; i++)
-	{
-	  /* Calculate cutoff function (weight factor) */
-	  double wght = 1.0 / (1.0 + tmp_a[i]);
-	  /* Calculate derivative of the cutoff function. */
-	  double dwdr = -cutoffslope * wght * (1 - wght);
-	  double dsigma1dr = (dwdr - wght * other_eta2) * tmp_b[i];
-	  double dsigma2dr = (dwdr + wght * -other_kappaoverbeta) * tmp_c[i];
-	  df[i] = tmp_e[i] * (dsigma1dr * dEdss[i] * chi_zs_zo
-			      + cnst_s * dsigma2dr
-			      + dsigma1dr * dEdso[i] * chi_zo_zs
-			      + cnst_o * dsigma2dr * (other[i] < nAtoms));
-	}
-#else //ASAP_MKL
       for (int i = 0; i < n; i++)
 	{
 	  /* Get the distances from their squares */
 	  double dist = sqrt(sq_dist[i]);
 	  double inv_dist = 1.0 / dist;
 	  /* Calculate cutoff function (weight factor) */
 	  double wght = 1.0 / (1.0 + exp(cutoffslope * dist
@@ -1724,59 +1497,18 @@
 	  double dsigma2dr = (dwdr + wght * -other_kappaoverbeta) *
 	    exp(-other_kappaoverbeta * dist + other_kappaseq);
 	  df[i] = inv_dist * (dsigma1dr * dEdss[i] * chi_zs_zo
 			      + cnst_s * dsigma2dr // * (self[i] < nAtoms)   always true
 			      + dsigma1dr * dEdso[i] * chi_zo_zs
 			      + cnst_o * dsigma2dr * (other[i] < nAtoms));
 	}
-#endif //ASAP_MKL
     }
   else if (!always_fullnblist)
     {
       // zs != zo.
-#ifdef ASAP_MKL
-      /* Get the distances from their squares */
-      // dist[] = tmp_a[] = sqrt(sq_dist[])
-      vdSqrt(n, sq_dist, tmp_a);
-      // invdist[] = tmp_g[] = 1.0 / dist[]
-      vdInv(n, tmp_a, tmp_g);
-      for (int i = 0; i < n; i++)
-        {
-	  tmp_b[i] = cutoffslope * tmp_a[i] - cutslopecutdist;
-	  tmp_c[i] = -other_eta2 * tmp_a[i] + other_eta2betaseq;
-	  tmp_d[i] = -other_kappaoverbeta * tmp_a[i] + other_kappaseq;
-	  tmp_e[i] = -self_eta2 * tmp_a[i] + self_eta2betaseq;
-	  tmp_f[i] = -self_kappaoverbeta * tmp_a[i] + self_kappaseq;
-	}
-      // tmp_a[] = exp(tmp_b[]) = exp(cutoffslope * dist[] - cutslopecutdist)
-      vdExp(n, tmp_b, tmp_a);
-      // tmp_b[] = exp(tmp_c[]) = exp(-other_eta2 * dist[] + other_eta2betaseq)
-      vdExp(n, tmp_c, tmp_b);
-      // tmp_c[] = exp(tmp_d[]) = exp(-other_kappaoverbeta * dist[] + other_kappaseq)
-      vdExp(n, tmp_d, tmp_c);
-      // tmp_d[] = exp(tmp_e[]) = exp(-self_eta2 * dist[] + self_eta2betaseq)
-      vdExp(n, tmp_e, tmp_d);
-      // tmp_e[] = exp(tmp_f[]) = exp(-self_kappaoverbeta * dist[] + self_kappaseq)
-      vdExp(n, tmp_f, tmp_e);
-      for (int i = 0; i < n; i++)
-	{
-	  /* Calculate cutoff function (weight factor) */
-	  double wght = 1.0 / (1.0 + tmp_a[i]);
-	  /* Calculate derivative of the cutoff function. */
-	  double dwdr = -cutoffslope * wght * (1 - wght);
-	  double dsigma1dr_o = (dwdr - wght * other_eta2) * tmp_b[i];
-	  double dsigma2dr_o = (dwdr + wght * -other_kappaoverbeta) * tmp_c[i];
-	  double dsigma1dr_s = (dwdr - wght * self_eta2) * tmp_d[i];
-	  double dsigma2dr_s = (dwdr + wght * -self_kappaoverbeta) * tmp_e[i];
-	  df[i] = tmp_g[i] * (dsigma1dr_o * dEdss[i] * chi_zs_zo
-			      + cnst_s * dsigma2dr_o
-			      + dsigma1dr_s * dEdso[i] * chi_zo_zs
-			      + cnst_o * dsigma2dr_s * (other[i] < nAtoms));
-	}      
-#else // ASAP_MKL
       for (int i = 0; i < n; i++)
 	{
 	  /* Get the distances from their squares */
 	  double dist = sqrt(sq_dist[i]);
 	  double inv_dist = 1.0 / dist;
 	  /* Calculate cutoff function (weight factor) */
 	  double wght = 1.0 / (1.0 + exp(cutoffslope * dist -
@@ -1792,49 +1524,18 @@
 	  double dsigma2dr_s = (dwdr + wght * -self_kappaoverbeta) *
 	    exp(-self_kappaoverbeta * dist + self_kappaseq);
 	  df[i] = inv_dist * (dsigma1dr_o * dEdss[i] * chi_zs_zo
 			      + cnst_s * dsigma2dr_o // * (self[i] < nAtoms)  always true!
 			      + dsigma1dr_s * dEdso[i] * chi_zo_zs
 			      + cnst_o * dsigma2dr_s * (other[i] < nAtoms));
 	}
-#endif //ASAP_MKL
     }
   else
     {
       // Using full neighbor lists
-#ifdef ASAP_MKL
-      /* Get the distances from their squares */
-      // dist[] = tmp_a[] = sqrt(sq_dist[])
-      vdSqrt(n, sq_dist, tmp_a);
-      // invdist[] = tmp_e[] = 1.0 / dist[]
-      vdInv(n, tmp_a, tmp_e);
-      for (int i = 0; i < n; i++)
-        {
-	  tmp_b[i] = cutoffslope * tmp_a[i] - cutslopecutdist;
-	  tmp_c[i] = -other_eta2 * tmp_a[i] + other_eta2betaseq;
-	  tmp_d[i] = -other_kappaoverbeta * tmp_a[i] + other_kappaseq;
-	}
-      // tmp_a[] = exp(tmp_b[]) = exp(cutoffslope * dist[] - cutslopecutdist)
-      vdExp(n, tmp_b, tmp_a);
-      // tmp_b[] = exp(tmp_c[]) = exp(-other_eta2 * dist[] + other_eta2betaseq)
-      vdExp(n, tmp_c, tmp_b);
-      // tmp_c[] = exp(tmp_d[]) = exp(-other_kappaoverbeta * dist[] + other_kappaseq)
-      vdExp(n, tmp_d, tmp_c);
-      for (int i = 0; i < n; i++)
-        {
-          /* Calculate cutoff function (weight factor) */
-          double wght = 1.0 / (1.0 + tmp_a[i]);
-          /* Calculate derivative of the cutoff function. */
-          double dwdr = -cutoffslope * wght * (1 - wght);
-          double dsigma1dr_o = (dwdr - wght * other_eta2) * tmp_b[i];
-          double dsigma2dr_o = (dwdr + wght * -other_kappaoverbeta) * tmp_c[i];
-          df[i] = tmp_e[i] * (dsigma1dr_o * dEdss[i] * chi_zs_zo
-                              + cnst_s * dsigma2dr_o);
-	}
-#else // ASAP_MKL
       for (int i = 0; i < n; i++)
         {
           /* Get the distances from their squares */
           double dist = sqrt(sq_dist[i]);
           double inv_dist = 1.0 / dist;
           /* Calculate cutoff function (weight factor) */
           double wght = 1.0 / (1.0 + exp(cutoffslope * dist -
@@ -1844,24 +1545,17 @@
           double dsigma1dr_o = (dwdr - wght * other_eta2) *
             exp(-other_eta2 * dist + other_eta2betaseq);
           double dsigma2dr_o = (dwdr + wght * -other_kappaoverbeta) *
             exp(-other_kappaoverbeta * dist + other_kappaseq);
           df[i] = inv_dist * (dsigma1dr_o * dEdss[i] * chi_zs_zo
                               + cnst_s * dsigma2dr_o);
         }
-#endif // ASAP_MKL
     }
-
   distribute_force(self, other, df, rnb, n);
-
-#ifdef ASAP_MKL
-  mkl_free(temporary);
-#else
   delete[] temporary;
-#endif
 }
 
 void EMT::distribute_force(const int *RESTRICT self, const int *RESTRICT other,
     const double *RESTRICT df, const Vec *RESTRICT rnb, int n)
 {
   /* Distribute force contributions */
 #ifdef _OPENMP
@@ -1890,15 +1584,15 @@
               }
       }
   }
 }
 
 double EMT::GetLatticeConstant() const
 {
-    ASSERT(singleelement != 0);
+    assert(singleelement != 0);
     return Beta * singleelement->seq * sqrt(2.0);
 }
 
 void EMT::PrintParameters()
 {
   for (int i = 0; i < nelements; i++)
     {
```

### Comparing `asap3-3.13.1/Potentials/EMT.h` & `asap3-3.9.6/Basics/EMT.h`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,14 @@
   /// update status.
   virtual bool CheckNeighborList();
   /// Update the neighbor lists
   virtual void UpdateNeighborList();
 
   virtual bool CalcReq_Energy(PyObject *pyatoms);
   virtual bool CalcReq_Forces(PyObject *pyatoms);
-  virtual bool CalcReq_Virial(PyObject *pyatoms);
   virtual bool CalcReq_Virials(PyObject *pyatoms);
 
   virtual double GetCutoffRadius() const {return rNbCut;}
   virtual double GetLatticeConstant() const;
   virtual int GetNumberOfAtoms() const {return nAtoms;}
 
   /// Return a pointer to the EMT "density" sigma1.
@@ -109,21 +108,15 @@
   /// Return the neighbor list.
 
   /// Return a BORROWED reference to the Python object containing
   /// neighbor list for the
   /// potential, if this type of potential supports it, and if it is
   /// defined now.  Otherwise, return NULL without setting a Python
   /// error.
-  virtual PyObject *GetNeighborList() const {return nblist_obj;}
-
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
+  PyObject *GetNeighborList() const {return nblist_obj;}
 
   /// This potential can be used in parallel simulations
   virtual bool Parallelizable() const {return true;}
 
   /// Mark that the atoms have changed the boundary conditions.
   virtual void BoundaryConditionsChanged();
 
@@ -179,15 +172,16 @@
   virtual void force_batch(const int *self, const int *other, const Vec rnb[],
                            const double sq_dist[], const double dEdss[],
                            const double dEdso[], int zs, int zo, int n);
   void distribute_force(const int *self, const int *other,
       const double *df, const Vec *rnb, int n);
   
 protected:  // Data
-  bool ghostatoms;          ///< True if number of atoms is likely to vary (atoms have ghosts).
+  // Atoms *atoms;             ///< The atoms we are working on
+  bool ghostatoms;          ///< True if atoms have ghosts.
   int nAtoms;               ///< The number of (real) atoms.
   int nSize;  ///< Number of atoms including ghost atoms.
   NeighborLocator *nblist;     ///< The neighborlist object.
   PyObject *nblist_obj;
   double driftfactor;             ///< Drift factor for the neighbor list.
   EMTParameterProvider *provider; ///< The source of the EMT parameters
   PyObject *provider_obj;         ///< The Python object behind provider.
```

### Comparing `asap3-3.13.1/Potentials/EMT2013.cpp` & `asap3-3.9.6/Basics/EMT2013.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -98,24 +98,24 @@
       // Extract the elements from the parameter dictionary.
       GetListOfElements(elements_set);
     }
   for (set<int>::iterator i = elements_set.begin(); i != elements_set.end();
        ++i)
     elements.push_back(*i);
   nelements = elements.size();
-  ASSERT(nelements == elements_set.size());
+  assert(nelements == elements_set.size());
   sort(elements.begin(), elements.end());
 
   // Get the EMT parameters
   parameters.clear();
   for (vector<int>::iterator i = elements.begin(); i != elements.end(); ++i)
     parameters.push_back(ExtractParameters(*i));
 
   /* DELETE */
-  //ASSERT(nelements == provider->GetNumberOfElements());
+  //assert(nelements == provider->GetNumberOfElements());
   /* DELETE */
 
   /* Calculate the quantities that can only be calculated, once the
      elements in the simulations are known. */
 
   // Cutoff distances in the system and maximum cutoff distance are calculated
   CalculateCutoffDistances();
@@ -138,16 +138,16 @@
 
 void EMT2013::GetListOfElements(set<int> &elements)
 {
   PyObject *key;
   PyObject *value;
   Py_ssize_t pos = 0;
   while (PyDict_Next(param_obj, &pos, &key, &value)) {
-      long z = PyLong_AsLong(key);
-      ASSERT(z != -1);  // Either an error occurred or an element has Z=-1
+      long z = PyAsapInt_AsLong(key);
+      assert(z != -1);  // Either an error occurred or an element has Z=-1
       elements.insert((int) z);
   }
 }
 
 emt_parameters *EMT2013::ExtractParameters(int z)
 {
   // Initialization
@@ -270,27 +270,27 @@
 {
   USETIMER("EMT::sigma_batch");
   double *temporary = new double[4*BUFLEN];
   double *RESTRICT dsigma1s = temporary;
   double *RESTRICT dsigma2s = dsigma1s + BUFLEN;
   double *RESTRICT dsigma1o = dsigma2s + BUFLEN;
   double *RESTRICT dsigma2o = dsigma1o + BUFLEN;
-  ASSERT(dsigma2o - temporary == (4 - 1) * BUFLEN);
+  assert(dsigma2o - temporary == (4 - 1) * BUFLEN);
 
   // initialization of lsf parameters;
   /* TEMP */ double rcut, ds1sdrcut, ds2sdrcut, s1srcut, s2srcut,
                     ds1odrcut, ds2odrcut, s1orcut, s2orcut; /* TEMP */
 
   double other_eta2betaseq, self_eta2betaseq;
   double other_kappaoverbeta, self_kappaoverbeta;
   double other_kappaseq, self_kappaseq;
   double *s1s, *s1o, *s2s, *s2o;
   const emt_parameters *emtself, *emtother;
 
-  ASSERT(n <= BUFLEN);
+  assert(n <= BUFLEN);
 
   /* Get EMT parameters !!! REWRITE !!! XXXX */
   emtself = parameters[zs];
   emtother = parameters[zo];
   /* DELETE  cutslopecutdist = cutoffslope * rFermi;   DELETE */
   other_eta2betaseq = emtother->eta2 * beta * emtother->seq;
   self_eta2betaseq = emtself->eta2 * beta * emtself->seq;
@@ -325,15 +325,15 @@
   // 1) Whether sigma2 needs to be calculated,  2) Whether we need a
   // different calculation for the two atoms interacting.  The latter is
   // the case if the atomic numbers are different, unless operating in
   // full neighborlist mode or doing a partial update for MonteCarloEMT,
   // in these cases calculations are not reused.
 
   bool calculateother = (zs != zo) && !always_fullnblist && !partialupdate;
-  ASSERT(n <= BUFLEN);
+  assert(n <= BUFLEN);
   if (!calculateother && !calculatesigma2)
     {
       for (int i = 0; i < n; i++)
 	{
 	  /* dist = sqrt(sq_dist),  distances between atoms */
 	  double dist = sqrt(sq_dist[i]);
 	  /* Calculate Linear Subtraction Function (New cutoff function) */
@@ -512,15 +512,15 @@
   double *sigma = &tmp_double[0];
   bool dosigmapart = (recalc.beforeforces || (calc_Epot && recalc.energies));
   bool doepotpart = (calc_Epot && recalc.energies);
 
   int zs, zo;
   double s;
   // Better performance if static ???
-  ASSERT(nelements < NMAXELEMENTS);
+  assert(nelements < NMAXELEMENTS);
   double invgamma1[NMAXELEMENTS];
   double neginvbetaeta2[NMAXELEMENTS];
   double neglambda[NMAXELEMENTS];
   double lambdaseq[NMAXELEMENTS];
   double negkappa[NMAXELEMENTS];
   double kappaseq[NMAXELEMENTS];
   double nege0lambdalambda[NMAXELEMENTS];
@@ -561,15 +561,15 @@
           int zs = id[i];
           for (int zo = 0; zo < nelements; zo++)
             s += (*chi)[zs][zo] * sigma1[zo][i];
           if (s < 1.0e-9)
             s = 1.0e-9;
           sigma[i] = s;
         }
-      ASSERT(nAtoms == this->radius.size() && nAtoms == this->Ec.size() &&
+      assert(nAtoms == this->radius.size() && nAtoms == this->Ec.size() &&
              nSize == this->dEds.size());
     }
 
   /* Calculate combinations of EMT parameters */
   for (int i = 0; i < nelements; i++)
     {
       invgamma1[i] = 1.0 / (parameters[i]->gamma1);
@@ -625,16 +625,16 @@
 #pragma omp master
 #endif // _OPENMP
           {
             VERB("e");
             DEBUGPRINT;
           }
           /* We also need Eas, but only for the real atoms */
-          ASSERT(sigma2isvalid);
-          ASSERT(counters.sigma2 == atoms->GetPositionsCounter());
+          assert(sigma2isvalid);
+          assert(counters.sigma2 == atoms->GetPositionsCounter());
           /* Calculate total sigma2 */
 #ifdef _OPENMP
 #pragma omp for
 #endif // _OPENMP
           for (int i = 0; i < nAtoms; i++)
             {
               s = 0.0;
@@ -685,15 +685,15 @@
 
 
   // initialization of lsf parameters;
   /* TEMP */ double rcut, ds1sdrcut, ds2sdrcut, s1srcut, s2srcut,
     	  	  	  	ds1odrcut, ds2odrcut, s1orcut, s2orcut; /* TEMP */
 
 
-  ASSERT(n <= BUFLEN);
+  assert(n <= BUFLEN);
 
   /* Get EMT parameters */
   emtself = parameters[zs];
   emtother = parameters[zo];
   // cutslopecutdist = cutoffslope * rFermi;
   other_eta2betaseq = emtother->eta2 * beta * emtother->seq;
   other_kappaoverbeta = emtother->kappa / beta;
@@ -872,15 +872,15 @@
 PyObject *EMT2013::GetParameterDict() const
 {
   // Perform a deep copy of the parameter object
   Py_ssize_t n = 0;
   PyObject *key;
   PyObject *value;
   PyObject *result = PyDict_New();
-  ASSERT(result != NULL);
+  assert(result != NULL);
   while (PyDict_Next(param_obj, &n, &key, &value))
     {
       if (!PyDict_Check(value))
         throw AsapError("EMT2013::GetParameterDict found non-dictionary in parameter dictionary.");
       PyObject *cp_value = PyDict_Copy(value);
       if (PyDict_SetItem(result, key, cp_value) < 0)
         throw AsapError("EMT2013::GetParameterDict failed to copy parameter dictionary");
```

### Comparing `asap3-3.13.1/Potentials/EMT2013.h` & `asap3-3.9.6/Basics/EMT2013.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Potentials/EMTDefaultParameterProvider.cpp` & `asap3-3.9.6/Basics/EMTDefaultParameterProvider.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,21 @@
 const int EMTDefaultParameterProvider::shell1 = 4;
 const double EMTDefaultParameterProvider::bohr = 0.5291772; // Angstrom
 
 typedef vector<emt_parameters *>::iterator param_p_iter;
 
 EMTDefaultParameterProvider::EMTDefaultParameterProvider()
 {
-  chi = NULL;
+  chi = 0;
   listcutofffactor = 1.04500185048;
 }
 
 EMTDefaultParameterProvider::~EMTDefaultParameterProvider()
 {
-  if (chi != NULL) delete chi;
+  if (chi != 0) delete chi;
   for (param_p_iter ep = params.begin(); ep != params.end(); ++ep) 
   {
       emt_parameters *e = *ep;
       delete e;
   }
 }
 
@@ -173,15 +173,15 @@
   p->kappa = kappa / bohr;
   p->lambda = lambda / bohr;
   p->mass = mass;
   p->invmass = 1.0/mass;
   p->gamma1 = 0.0;        // These are calculated later!
   p->gamma2 = 0.0;
   p->Z = Z;
-  ASSERT(element == Z);
+  assert(element == Z);
   p->name = name;
   p->lengthscale = ls / sqrt(2.0) * bohr;
 
   return p;
 }
 
 void EMTDefaultParameterProvider::CalcGammaEtc()
@@ -252,16 +252,14 @@
     }
 }
 
 void EMTDefaultParameterProvider::calc_chi()
 {
   int n = params.size();
 
-  if (chi != NULL)
-    delete chi;
   chi = new TinyDoubleMatrix(n,n);
 
   for (int i = 0; i < n; ++i)
     for (int j = 0; j < n; ++j) {
       (*chi)[i][j] = params[j]->neq / params[i]->neq;
     }
 }
```

### Comparing `asap3-3.13.1/Potentials/EMTDefaultParameterProvider.h` & `asap3-3.9.6/Basics/EMTDefaultParameterProvider.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Potentials/EMTParameterProvider.h` & `asap3-3.9.6/Basics/EMTParameterProvider.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Potentials/EMTPythonParameterProvider.cpp` & `asap3-3.9.6/Basics/EMTPythonParameterProvider.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -62,35 +62,39 @@
       Py_DECREF(dict);  // We also abort GetNewParameters()
       throw AsapError("EMT parameter dictionary had no (or non-int) element ")
 	<< name;
     }
   return xval;
 }
 
-static const char *extract_str(PyObject *dict, const char *name)
+static char *extract_str(PyObject *dict, const char *name)
 {
   DEBUGPRINT;
   PyObject *x = PyDict_GetItemString(dict, name);
-  if (x == NULL || !PyUnicode_Check(x))
+  if (x == NULL || !PyAsapString_Check(x))
     {
       Py_DECREF(dict);  // We also abort GetNewParameters()
       throw
 	AsapError("EMT parameter dictionary had no (or non-string) element ")
 	<< name;
     }
   // "Intern" the string (the element name).  Interning the string
   // assures that the Python string object never goes away, but does
   // not introduce a memory leak as multiple identical strings are mapped
   // to the same string (no leak as long as the number of distinct element
   // names remains limited!).  The alternative, copying the string,
   // introduce a tiny leak as the pointer cannot be deallocated (usually
   // it refers to static memory).
+#ifdef ASAP_PY3
   PyUnicode_InternInPlace(&x);
-  const char *str = PyUnicode_AsUTF8(x);
-
+  char *str = PyUnicode_AsUTF8(x);
+#else
+  PyString_InternInPlace(&x);
+  char *str = PyString_AsString(x);
+#endif
   // Note that by failing to DECREF the string here we make the interned
   // string immortal, in contrast to what the docs say this does not
   // happen automatically when interning.
   // It might be better to make it immortal through the C API (undocumented!)
   // or to keep it alive in a dictionary for as long as this parameter provider
   // is alive.
   return str;
@@ -117,15 +121,15 @@
   p->lambda = extract(newparam, "lambda");
   p->mass = extract(newparam, "mass");
   p->Z = extract_int(newparam, "Z");
   p->name = extract_str(newparam, "name");
   p->invmass = 1.0 / p->mass;
   p->gamma1 = p->gamma2 = 0.0;
   p->lengthscale = 0.0;  // Remove
-  ASSERT(element == p->Z);
+  assert(element == p->Z);
 
   DEBUGPRINT;
   Py_DECREF(newparam);
   return p;
 }
```

### Comparing `asap3-3.13.1/Potentials/EMTPythonParameterProvider.h` & `asap3-3.9.6/Basics/EMTPythonParameterProvider.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Potentials/EMTRasmussenParameterProvider.cpp` & `asap3-3.9.6/Basics/EMTRasmussenParameterProvider.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
   p->kappa = kappa / bohr;
   p->lambda = lambda / bohr;
   p->mass = mass;
   p->invmass = 1.0/mass;
   p->gamma1 = 0.0;        // These are calculated later!
   p->gamma2 = 0.0;
   p->Z = Z;
-  ASSERT(element == Z);
+  assert(element == Z);
   p->name = name;
   p->lengthscale = ls / sqrt(2.0) * bohr;
 
   return p;
 }
 
 double EMTRasmussenParameterProvider::GetMaxListCutoffDistance()  // Max value, useful before initialization.
```

### Comparing `asap3-3.13.1/Potentials/EMTRasmussenParameterProvider.h` & `asap3-3.9.6/Basics/EMTRasmussenParameterProvider.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Potentials/LennardJones.cpp` & `asap3-3.9.6/Basics/LennardJones.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -60,17 +60,15 @@
 using std::cerr;
 using std::endl;
 using std::flush;
 using std::less;
 
 #define SPARSE_MATRIX_SIZE 92  // No Pu, please!  
 
-// Use same volume for all atoms in stress calculation.  If changed,
-// then update BuildinPotentials.py accordingly to enable or disable
-// .get_atomic_volumes().
+// Use same volume for all atoms in stress calculation.
 #define SHAREVOLUME   
 
 #if 0
 #define VERB(x) if (verbose == 1) cerr << x
 #else
 #define VERB(x)
 #endif
@@ -252,15 +250,15 @@
   if (accessobj != NULL)
     {
       atoms = accessobj;
       AsapAtoms_INCREF(atoms);
     }
   else
     atoms = new NormalAtoms();
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
 }
 
 //******************************************************************************
 //                             CalculateIDs
 //******************************************************************************
 /*
    calculates or defines the default rCut
@@ -281,119 +279,106 @@
 //                             Allocate
 //******************************************************************************
 void LennardJones::Allocate()
 {
   DEBUGPRINT;
   if (verbose)
     cerr << "Allocate(" << nAtoms << ") " << endl;
-  ASSERT(nAtoms != 0);
+  assert(nAtoms != 0);
   atomicEnergies.resize(nAtoms);
   forces.resize(nSize);
   virials.resize(nSize);
   DEBUGPRINT;
 }
 
-bool LennardJones::CheckAndUpdateNbList(PyObject *pyatoms)
-{
-  atoms->Begin(pyatoms);
-  bool updated = CheckNeighborLists();
-  atoms->End();
-  return updated;
-}
-
-
-
 //******************************************************************************
 //                             CheckNeighborLists
 //******************************************************************************
-bool LennardJones::CheckNeighborLists()
+void LennardJones::CheckNeighborLists()
 {
   DEBUGPRINT;
   if (counters.nblist == atoms->GetPositionsCounter() && neighborList != NULL
       && !neighborList->IsInvalid())
-    return false;
-  bool update = false;
+    return;
   if (neighborList)
     {
       DEBUGPRINT;
-      update = neighborList->CheckNeighborList();
+      bool update = neighborList->CheckNeighborList();
       update = atoms->UpdateBeforeCalculation(update,
 					  rCut * (1 + driftfactor));
       if (update)
 	neighborList->UpdateNeighborList();
       if ((nAtoms != atoms->GetNumberOfAtoms()) ||
           (nSize != nAtoms + atoms->GetNumberOfGhostAtoms()))
 	{
 	  DEBUGPRINT;
-	  ASSERT(update);
+	  assert(update);
 	  nAtoms = atoms->GetNumberOfAtoms();
 	  nSize = nAtoms + atoms->GetNumberOfGhostAtoms();
 	  Allocate();
 	}
     }
   else
     {
       DEBUGPRINT;
-      update = true;
       atoms->UpdateBeforeCalculation(true, rCut * (1 + driftfactor));
       PyAsap_NeighborLocatorObject *nbl = PyAsap_NewNeighborList(atoms, rCut,
 								 driftfactor);
       neighborList_obj = (PyObject *)nbl;
       neighborList = dynamic_cast<NeighborList*>(nbl->cobj);
       neighborList->verbose = verbose;
-      ASSERT(neighborList != NULL);
+      assert(neighborList != NULL);
       neighborList->CheckAndUpdateNeighborList();
       nAtoms = atoms->GetNumberOfAtoms();
       nSize = nAtoms + atoms->GetNumberOfGhostAtoms();
       Allocate();
     }
   counters.nblist = atoms->GetPositionsCounter();
   DEBUGPRINT;
-  return update;
 }
 
 //******************************************************************************
 //                             GetPotentialEnergy
 //******************************************************************************
 double LennardJones::GetPotentialEnergy(PyObject *pyatoms)
 {
   DEBUGPRINT;
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   CheckNeighborLists();
   DEBUGPRINT;
   double e = CalculateEnergyAndEnergies();
   atoms->End();
   return e;
 }
 
 const vector<double> &LennardJones::GetPotentialEnergies(PyObject *pyatoms)
 {
   DEBUGPRINT;
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   CheckNeighborLists();
   CalculateEnergyAndEnergies();
   atoms->End();
   DEBUGPRINT;
   return atomicEnergies;
 }
 
 //******************************************************************************
 //                               GetStresses 
 //******************************************************************************
 const vector<SymTensor> &LennardJones::GetVirials(PyObject *pyatoms)
 {
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   CheckNeighborLists();
   if (nAtoms != virials.size())
     virials.resize(nSize);
-  memset((void *) &virials[0], 0, nSize * sizeof(SymTensor));
-  GetVirials(&virials[0]);
+  memset(&virials[0], 0, nSize * sizeof(SymTensor));
+  GetVirials(atoms->GetMomenta(), &virials[0]);
   atoms->End();
   return virials;
 }
 
 //******************************************************************************
 //                               Stress 
 //******************************************************************************
@@ -418,15 +403,15 @@
                           m_{i}                                     r_ij^{14}     r_ij^{8}             
 */
 
 
 //******************************************************************************
 //                               GetStresses
 //******************************************************************************
-void LennardJones::GetVirials(SymTensor *stresses)
+void LennardJones::GetVirials(const Vec *momenta, SymTensor *stresses)
 {
   DEBUGPRINT;
 
   int maxNeighbors=neighborList->MaxNeighborListLength();//the max number of neighbors in neighborlist
   int numNeighbors; //the current number of neighbors in the iteration
 
   vector<Vec> diffs(maxNeighbors);
@@ -488,20 +473,20 @@
 }
 
 //******************************************************************************
 //                               GetCartesianForces 
 //******************************************************************************
 const vector<Vec> &LennardJones::GetForces(PyObject *pyatoms)
 {
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   CheckNeighborLists();
-  ASSERT(nSize >= nAtoms);
-  ASSERT(forces.size() == nSize);
-  memset((void *) &(forces[0]), 0, nSize * sizeof(Vec)); //zero the forces
+  assert(nSize >= nAtoms);
+  assert(forces.size() == nSize);
+  memset(&(forces[0]), 0, nSize * sizeof(Vec)); //zero the forces
   GetCartesianForces(forces);
   atoms->End();
   return forces;
 }
 
 //******************************************************************************
 //                           GetCartesianForces
@@ -588,15 +573,15 @@
 double LennardJones::CalculateEnergyAndEnergies() {
   if (counters.energies != atoms->GetPositionsCounter()) {
     memset(&atomicEnergies[0], 0, nAtoms * sizeof(double));
     CalculateEnergyAndEnergies(atomicEnergies);
     counters.energies = atoms->GetPositionsCounter();
   }
   double energy = 0.0;
-  ASSERT(atomicEnergies.size() == nAtoms);
+  assert(atomicEnergies.size() == nAtoms);
   for (int a = 0; a < nAtoms; a++) {
     energy +=  atomicEnergies[a];
   }
   return energy;
 }
```

### Comparing `asap3-3.13.1/Potentials/LennardJones.h` & `asap3-3.9.6/Basics/LennardJones.h`

 * *Files 4% similar despite different names*

```diff
@@ -119,32 +119,25 @@
   virtual long PrintMemory() const;
 
   void SetAtoms(PyObject *atoms, Atoms* accessobj = NULL); 
   double GetPotentialEnergy(PyObject *atoms);
   const vector<Vec> &GetForces(PyObject *atoms);
   const vector<SymTensor> &GetVirials(PyObject *atoms);
   const vector<double> &GetPotentialEnergies(PyObject *atoms);
-  bool CheckNeighborLists();
+  void CheckNeighborLists();
   double GetCutoffRadius() const {return rCut;}
   double GetLatticeConstant() const {return latticeConstant;}
   /// Return the neighbor list.
 
   /// Return the Python object containing neighbor list for the
   /// potential, if this type of potential supports it, and if it is
   /// defined now.  Otherwise, return NULL without setting a Python
   /// error.
   PyObject *GetNeighborList() const {return neighborList_obj;}
 
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
-  
   /// This potential can be used in parallel simulations
   virtual bool Parallelizable() const {return true;}
 
 private:
   /** \brief Allocates the memory needed by the data structures */
   void Allocate();
   /** \brief calculates the total energy and individual energies of the atoms */
@@ -155,15 +148,15 @@
   /** \brief helper function for GetCartesianForces*/
   /** \param start the start atom id
       \param end   the end atom id (exclusive)*/
   void GetCartesianForces(vector<Vec>& forces);
   /** \brief  private member function to calculate the stress for a range for atoms with id <code>start</code> to <code>end</code>*/
   /** \param start the start atom id
       \param end   the end atom id (exclusive)*/
-  void GetVirials(SymTensor *stresses);
+  void GetVirials(const Vec *momenta, SymTensor *stresses);
   void GetAtomicVolumes(vector<double> &volumes);
 
   /** \brief calculates a r-cut from the sigmas */
   double CalculateRCut(int numElements, const vector<double> &sigma); 
   /** \brief converts the parameters to the internal form */
   /** Fills the local epsilon and sigma matrices (stored as an array)
```

### Comparing `asap3-3.13.1/Potentials/MetalOxideInterface.h` & `asap3-3.9.6/Basics/MetalOxideInterface2.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // -*- C++ -*-
-// MetalOxideInterface.h: A potential for metal oxide interfaces
+// MetalOxideInterface2.h: A potential for metal oxide interfaces
 //
 // Copyright (C) 2014 Jacob Madsen, Jakob Schiotz and Center for
 // Individual Nanoparticle Functionality, Department of Physics,
 // Technical University of Denmark.  Email: jamad@fysik.dtu.dk
-//
+// 
 // This file is part of Asap version 3.
 //
 // This program is free software: you can redistribute it and/or
 // modify it under the terms of the GNU Lesser General Public License
 // version 3 as published by the Free Software Foundation.  Permission
 // to use other versions of the GNU Lesser General Public License may
 // granted by Jakob Schiotz or the head of department of the
@@ -20,16 +20,16 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-#ifndef MetalOxideInterface_H
-#define MetalOxideInterface_H
+#ifndef MetalOxideInterface2_H
+#define MetalOxideInterface2_H
 
 #include "AsapPython.h"
 #include "Asap.h"
 #include "Potential.h"
 #include "Vec.h"
 #include "SymTensor.h"
 #include <vector>
@@ -37,108 +37,106 @@
 //~ using std::vector;
 
 namespace ASAPSPACE {
 
 class Atoms;
 class NeighborList;
 
-class MetalOxideInterface : public Potential
+class MetalOxideInterface2 : public Potential
 {
 public:
 
-    MetalOxideInterface(PyObject *self,
-                double P, double Q, double A, double xi, double r0, double RGL_cut,
-                const std::vector<double> &q, double kappa,
-                const std::vector<double> &D, const std::vector<double> &alpha, const std::vector<double> &R0,
-                const std::vector<double> &a, const std::vector<double> &b, double &f0, double &oxide_cut,
-                const std::vector<double> &beta_, double gamma, double &interface_cut,
-                int verbose);
-    ~MetalOxideInterface();
-    
-    virtual string GetName() const {return "MetalOxideInterface";}
-    virtual long PrintMemory() const;
-    double GetCutoffRadius() const {return 0;}
-    double GetLatticeConstant() const {return 0;}
-
-    void SetAtoms(PyObject *atoms, Atoms* accessobj = NULL);
-    double GetPotentialEnergy(PyObject *atoms);
-    const std::vector<Vec> &GetForces(PyObject *atoms);
-    const std::vector<SymTensor> &GetVirials(PyObject *atoms);
-    const std::vector<double> &GetPotentialEnergies(PyObject *atoms);
-
-    bool CheckNeighborLists();
-
-    // Return the neighbor list
-    PyObject *GetNeighborList() const {return neighborList_obj;}
-
-    /// Check and possibly update a neighbor list associated with this potential.
-    ///
-    /// This is the only way a neighbor list borrowed from a potential should be updated.
-    /// Calling this function on a Potential not having a neighbor list is an error.
-    /// Returns true if the neighbor list was actually updated.
-    virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
+	MetalOxideInterface2(PyObject *self,
+			     double P, double Q, double A, double xi, double r0, double RGL_cut,
+			     const std::vector<double> &q, double kappa,
+			     const std::vector<double> &D, const std::vector<double> &alpha, const std::vector<double> &R0,
+			     const std::vector<double> &a, const std::vector<double> &b, double &f0, double &oxide_cut,
+			     const std::vector<double> &E, const std::vector<double> &rho0, const std::vector<double> &l0,
+			     const std::vector<double> &B, const std::vector<double> &C,
+			     double &interface_cut, int verbose);
+	~MetalOxideInterface2();
+	
+	virtual string GetName() const {return "MetalOxideInterface2";}
+	virtual long PrintMemory() const;
+	double GetCutoffRadius() const {return 0;}
+	double GetLatticeConstant() const {return 0;}
+
+	void SetAtoms(PyObject *atoms, Atoms* accessobj = NULL);
+	double GetPotentialEnergy(PyObject *atoms);
+	const std::vector<Vec> &GetForces(PyObject *atoms);
+	const std::vector<SymTensor> &GetVirials(PyObject *atoms);
+	const std::vector<double> &GetPotentialEnergies(PyObject *atoms);
+
+	void CheckNeighborLists();
+
+	// Return the neighbor list
+	PyObject *GetNeighborList() const {return neighborList_obj;}
 
-    // This potential can be used in parallel simulations
-    virtual bool Parallelizable() const {return true;}
+	// This potential can be used in parallel simulations
+	virtual bool Parallelizable() const {return true;}
 
 private:
-    // Allocate memory 
-    void Allocate();
+	// Allocate memory 
+	void Allocate();
 
-    // Get total energy
-    double CalculateEnergyAndEnergies();
-    
-    // Assign atom type
-    void AssignAtoms();
-    
-    // RGL potetial
-    void RGL(vector<double>& atomicEnergies);
-    void RGLForces(vector<Vec>& forces);
-        
-    // Oxide potetial
-    void Oxide(vector<double>& atomicEnergies);
-    void OxideForces(vector<Vec>& forces);
-    double Erfc(double x);
-    
-    // Interface potential
-    void InterfacePotential(vector<double>& atomicEnergies);
-    void InterfaceForces(vector<Vec>& forces);
-    
-    // Calculate energy shift
-    std::vector<double> OxideShift();
-
-    // Reference to the neighborlist
-    NeighborList *neighborList;
-    PyObject *neighborList_obj;
-    
-    // Number and type of atoms
-    int nAtoms, nSize, nMetals, nOxides;
-    std::vector<asap_z_int> metals, oxides, assignment, monolayer;
-    
-    // Potential parameters
-    double P, Q, A, xi, r0, qM, qO, kappa, f0, gamma;
-    std::vector<double> q, D, alpha, R0, a, b, beta;
-    
-    // Cut-off radius
-    double RGL_cut, oxide_cut, interface_cut, driftfactor;
+	// Get total energy
+	double CalculateEnergyAndEnergies();
+	
+	// Assign atom type
+	void AssignAtoms();
+	
+	// RGL potetial
+	void RGL(vector<double>& atomicEnergies);
+	void RGLForces(vector<Vec>& forces);
+		
+	// Oxide potetial
+	void Oxide(vector<double>& atomicEnergies);
+	void OxideForces(vector<Vec>& forces);
+	double Erfc(double x);
+	
+	// Interface potential
+	void InterfacePotential(vector<double>& atomicEnergies);
+	void InterfaceForces(vector<Vec>& forces);
+	
+	// Calculate energy shift
+	std::vector<double> OxideShift();
+    std::vector<double> InterfaceShift();
+
+	// Gets virials forces (not yet implemented)
+	void GetVirials(const Vec *momenta, SymTensor *stresses);
+	
+	// Reference to the neighborlist
+	NeighborList *neighborList;
+	PyObject *neighborList_obj;
+	
+	// Number and type of atoms
+	int nAtoms, nSize, nMetals, nOxides;
+	std::vector<asap_z_int> metals, oxides, assign, monolayer;
+	
+	// Potential parameters
+	double P, Q, A, xi, r0, qM, qO, kappa, f0;
+	std::vector<double> q, D, alpha, R0, a, b, E, rho0, l0, B, C;
+	
+	// Cut-off radius
+	double RGL_cut, oxide_cut, interface_cut, driftfactor;
   
-    // Atomic energies for atoms
-    std::vector<double> atomicEnergies, sigma_p, sigma_q;
-        
-    // GetStresses returns pointer in this
-    std::vector<SymTensor> virials;
-
-    // GetCartesianForces returns a pointer in this
-    std::vector<Vec> forces;
-
-    // Counters to check whether recalculations are necessary
-    struct {
-        int ids;
-        int nblist;
-        int energies;
-        int forces;
-        int stresses;
-    } counters;
+	// Atomic energies for atoms
+	std::vector<double> atomicEnergies, sigma_p, sigma_q;
+		
+	// GetStresses returns pointer in this
+	std::vector<SymTensor> virials;
+
+	// GetCartesianForces returns a pointer in this
+	std::vector<Vec> forces;
+
+	// Counters to check whether recalculations are necessary
+	struct {
+		int ids;
+		int nblist;
+		int energies;
+		int forces;
+		int stresses;
+	} counters;
 };
 }
 
-#endif //MetalOxideInterface
+#endif //MetalOxideInterface2
```

### Comparing `asap3-3.13.1/Potentials/MonteCarloEMT.cpp` & `asap3-3.9.6/Basics/MonteCarloEMT.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,19 @@
 {
   if (mc_atoms != NULL)
     AsapAtoms_DECREF(mc_atoms);
 }
 
 void MonteCarloEMT::SetAtoms(PyObject *pyatoms, Atoms* accessobj)
 {
-  ASSERT(accessobj == NULL);
+  assert(accessobj == NULL);
   if (atoms != NULL)
     throw AsapError("Cannot use the same MonteCarloEMT object for multiple Atoms objects.");
   mc_atoms = new MonteCarloAtoms();
-  ASSERT(mc_atoms != NULL);
+  assert(mc_atoms != NULL);
   EMT::SetAtoms(pyatoms, mc_atoms);
 }
 
 void MonteCarloEMT::CreateNeighborList()
 {
 #ifdef _OPENMP
 #pragma omp single
@@ -65,15 +65,15 @@
   {
     PyAsap_NeighborLocatorObject *nbl;
     nbl = PyAsap_NewNeighborList(atoms, rNbCut, driftfactor);
     nblist = nbl->cobj;
     nblist->verbose = verbose;
     nblist_obj = (PyObject *) nbl;
     NeighborList *realnblist = dynamic_cast<NeighborList*>(nblist);
-    ASSERT(realnblist != NULL);
+    assert(realnblist != NULL);
     realnblist->EnableFullNeighborLists();
     nbl->fulllist = true;
   }
   nblist->UpdateNeighborList();
 }
 
 const vector<double> &MonteCarloEMT::GetPotentialEnergies(PyObject *pyatoms)
@@ -89,18 +89,18 @@
       VERB(" MCEnergies[");
       DEBUGPRINT;
       if (counters.energies != atoms->GetPositionsCounter())
 	{
           DEBUGPRINT;
 	  const set<int> &modified_atoms = mc_atoms->GetModifiedAtoms();
 	  set<int> affected_atoms;
-	  ASSERT(modified_atoms.size() > 0);
+	  assert(modified_atoms.size() > 0);
 	  PartialCalculateIDs(modified_atoms);
 	  NeighborList *nbl = dynamic_cast<NeighborList*>(nblist);
-	  ASSERT(nbl != NULL);
+	  assert(nbl != NULL);
 	  nbl->RemakeLists(modified_atoms, affected_atoms);
 	  counters.nblist = atoms->GetPositionsCounter();
 	  VERB("(" << modified_atoms.size() << "/" << affected_atoms.size()
 	       << " atoms)");
 	  PartialCalculateSigmas(affected_atoms);
 	  PartialCalculateEnergiesAfterSigmas(affected_atoms);
 	  // CheckNeighborLists();
@@ -162,15 +162,15 @@
 void MonteCarloEMT::PartialCalculateSigmas(const set<int> &changedatoms)
 {
   USETIMER("MonteCarloEMT::PartialCalculateSigmas");
   int ctr = atoms->GetPositionsCounter();
   if ((counters.sigma1 == ctr) && (counters.sigma2 == ctr))
     return;
   counters.sigma1 = counters.sigma2 = ctr;
-  ASSERT(sigma2isvalid);
+  assert(sigma2isvalid);
   
   int maxnblen = nblist->MaxNeighborListLength();
   if (maxnblen > BUFLEN)
     throw AsapError("Neighborlist overrun (did you squeeze your atoms?).  Longest neighbor list is ") << maxnblen;
 
   // Buffer data:
   TinyMatrix<int> nbatch(nelements,nelements);
@@ -195,38 +195,38 @@
 
   // Loop over atoms
   for (set<int>::const_iterator atomptr = changedatoms.begin();
        atomptr != changedatoms.end(); ++atomptr) 
     {
       int atom = *atomptr;
       int zself = id[atom];
-      ASSERT(zself < nelements);
+      assert(zself < nelements);
       // Get neighbors and loop over them.  Simplest if only one element
       if (nelements == 1) 
         {
           int nbat = nbatch[0][0];  // only element
           int size = BUFLEN-nbat;
           int n = nblist->GetFullNeighbors(atom, other[0][0]+nbat,
 					   rnb[0][0]+nbat, sqdist[0][0]+nbat,
 					   size);
-          ASSERT(size >= 0);    // REMOVE LATER !!!
+          assert(size >= 0);    // REMOVE LATER !!!
           for (int i = nbat; i < nbat+n; i++)
             self[0][0][i] = atom;
           nbatch[0][0] += n;
         } 
       else 
         {
           int size = BUFLEN;
           int n = nblist->GetFullNeighbors(atom, other_buf, rnb_buf, sqdist_buf,
 					   size);
-          ASSERT(size >= 0);     // REMOVE LATER !!!
+          assert(size >= 0);     // REMOVE LATER !!!
           for (int i = 0; i < n; i++) 
             {
               int zother = id[other_buf[i]];
-	      ASSERT(zother < nelements);
+	      assert(zother < nelements);
               int nbat = nbatch[zself][zother]++;  // Count this atom
               self[zself][zother][nbat] = atom;
               other[zself][zother][nbat] = other_buf[i];
               rnb[zself][zother][nbat][0] = rnb_buf[i][0];
               rnb[zself][zother][nbat][1] = rnb_buf[i][1];
               rnb[zself][zother][nbat][2] = rnb_buf[i][2];
               sqdist[zself][zother][nbat] = sqdist_buf[i];
@@ -252,15 +252,15 @@
 
 void MonteCarloEMT::PartialCalculateEnergiesAfterSigmas(const set<int>
 							&changedatoms)
 {
   int i;
   int zo;
   // Better performance if static ???
-  ASSERT(nelements < NMAXELEMENTS);
+  assert(nelements < NMAXELEMENTS);
   double inv12gamma1[NMAXELEMENTS];
   double neglambda[NMAXELEMENTS];
   double lambdaseq[NMAXELEMENTS];
   double negkappa[NMAXELEMENTS];
   double kappaseq[NMAXELEMENTS];
   double nege0lambdalambda[NMAXELEMENTS];
   double e0lambdalambdaseq[NMAXELEMENTS];
@@ -292,15 +292,15 @@
                                        parameters[i]->seq);
       sixv0[i] = 6.0 * parameters[i]->V0;
       neghalfv0overgamma2[i] = -0.5 * parameters[i]->V0 /
         parameters[i]->gamma2;
       seq[i] = parameters[i]->seq;
     }
 
-  ASSERT(counters.beforeforces != atoms->GetPositionsCounter() ||
+  assert(counters.beforeforces != atoms->GetPositionsCounter() ||
 	 counters.energies != atoms->GetPositionsCounter());
     
   counters.beforeforces = counters.energies = atoms->GetPositionsCounter();
   VERB("E");
   /* Calculate total sigma1 */
   for (set<int>::const_iterator aptr = changedatoms.begin();
        aptr != changedatoms.end(); ++aptr)
@@ -319,16 +319,16 @@
       double ex2 = exp(negkappa[z] * radius[i] + kappaseq[z]);
       dEds[i] = (nege0lambdalambda[z] * radius[i] + e0lambdalambdaseq[z])
 	* ex1 + neg6v0kappa[z] * ex2;
       dEds[i] *= - invbetaeta2[z] / sigma;
       /* Cohesive energy */
       Ec[i] = (e0lambda[z] * radius[i] + eccnst[z]) * ex1;
       /* We also need Eas, but only for the real atoms */
-      ASSERT(sigma2isvalid);
-      ASSERT(counters.sigma2 == atoms->GetPositionsCounter());
+      assert(sigma2isvalid);
+      assert(counters.sigma2 == atoms->GetPositionsCounter());
       /* Calculate total sigma2 */
       sigma = 0.0;
       z = id[i];
       for (zo = 0; zo < nelements; zo++)
 	sigma += (*chi)[z][zo] * sigma2[zo][i];
       if (sigma < 1.0e-9)
 	sigma = 1.0e-9;
```

### Comparing `asap3-3.13.1/Potentials/MonteCarloEMT.h` & `asap3-3.9.6/Basics/MonteCarloEMT.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Potentials/Morse.cpp` & `asap3-3.9.6/Basics/Morse.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 
 // SunOS compiler: sqrt does not work with a literal number (cannot decide if
 // it is a double or a long double).
 #ifdef SUN_SQRT_LITERAL_HACK
 #define sqrt(x) sqrt((double) x)
 #endif
 
+// Standard mapping of the six independent parts of the stress tensor to
+// vector notation
+const static int stresscomp[3][3] = {{0, 5, 4}, {5, 1, 3}, {4, 3, 2}};
+
+
 
 //******************************************************************************
 //                                    Morse
 //******************************************************************************
 Morse::Morse(PyObject *self,
              const std::vector<int> &elements,
              const std::vector<double> &epsilon,
@@ -232,15 +237,15 @@
     }
   else
     {
       // This is at least the second time SetAtoms is called.
       if (accessobj != NULL)
 	throw AsapError("Morse::SetAtoms called multiple times with accessobj != NULL");
     }
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   
   // The Morse potential is often used for thin gasses or the like.
   // In those cases, the neighbor list's "drift factor" should be
   // increased for more efficient reuse of the list.  Experiments show
   // that a broad optimum occurs when there is on average around 0.1
   // atom per cell in the NeighborCellLocator object used by
   // NeighborList.  This may pt. only be done for serial simulations
@@ -253,15 +258,15 @@
       int n = atoms->GetNumberOfAtoms();
       double vol = atoms->GetVolume();
       double atomspercell = n / vol * pow(rCut,3);
       if (atomspercell < 0.05)
 	{
 	  // Low density, increase driftfactor
 	  driftfactor = (pow(0.1 / atomspercell, 1.0/3) - 1.0) / 2;
-	  ASSERT(driftfactor >= DRIFTFACTOR);
+	  assert(driftfactor >= DRIFTFACTOR);
 	}
       else
 	driftfactor = DRIFTFACTOR;  // High or medium density.
     }
   else
     driftfactor = DRIFTFACTOR;
   atoms->End();
@@ -292,72 +297,60 @@
 //                                 Allocate
 //******************************************************************************
 void Morse::Allocate()
 {
   DEBUGPRINT;
   if (verbose)
     cerr << "Allocate(" << nAtoms << ") " << endl;
-  ASSERT(nAtoms != 0);
+  assert(nAtoms != 0);
   atomicEnergies.resize(nAtoms);
   forces.resize(nSize);
   //stresses.resize(nAtoms);
   DEBUGPRINT;
 }
 
-bool Morse::CheckAndUpdateNbList(PyObject *pyatoms)
-{
-  atoms->Begin(pyatoms);
-  bool updated = CheckNeighborLists();
-  atoms->End();
-  return updated;
-}
-
-
 //******************************************************************************
 //                             CheckNeighborLists
 //******************************************************************************
-bool Morse::CheckNeighborLists()
+void Morse::CheckNeighborLists()
 {
   DEBUGPRINT;
   if (counters.nblist == atoms->GetPositionsCounter() && neighborList != NULL &&
       !neighborList->IsInvalid())
-    return false;
+    return;
 
-  bool update = false;
   if (neighborList) {
       DEBUGPRINT;
-      update = neighborList->CheckNeighborList();
+      bool update = neighborList->CheckNeighborList();
       update = atoms->UpdateBeforeCalculation(update, rCut * (1 + driftfactor));
       if (update)
         neighborList->UpdateNeighborList();
       if ((nAtoms != atoms->GetNumberOfAtoms()) ||
           (nSize != nAtoms + atoms->GetNumberOfGhostAtoms())) {
           DEBUGPRINT;
-          ASSERT(update);
+          assert(update);
           nAtoms = atoms->GetNumberOfAtoms();
           nSize = nAtoms + atoms->GetNumberOfGhostAtoms();
           Allocate();
       }
   } else {
       DEBUGPRINT;
-      update = true;
       atoms->UpdateBeforeCalculation(true, rCut * (1 + driftfactor));
       PyAsap_NeighborLocatorObject *nbl = PyAsap_NewNeighborList(atoms, rCut, driftfactor);
       neighborList_obj = (PyObject *)nbl;
       neighborList = nbl->cobj;
-      ASSERT(neighborList != NULL);
+      assert(neighborList != NULL);
       neighborList->verbose = verbose;
       neighborList->CheckAndUpdateNeighborList();
       nAtoms = atoms->GetNumberOfAtoms();
       nSize = nAtoms + atoms->GetNumberOfGhostAtoms();
       Allocate();
   }
   counters.nblist = atoms->GetPositionsCounter();
   DEBUGPRINT;
-  return update;
 }
 
 //******************************************************************************
 //                                GetStresses
 //******************************************************************************
 const vector<SymTensor> &Morse::GetVirials(PyObject *pyatoms)
 {
@@ -366,18 +359,18 @@
 
 
 //******************************************************************************
 //                                 GetForces 
 //******************************************************************************
 const vector<Vec> &Morse::GetForces(PyObject *pyatoms)
 {
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   CheckNeighborLists();
-  memset((void *) &(forces[0]), 0, nSize * sizeof(Vec)); //zero the forces
+  memset(&(forces[0]), 0, nSize * sizeof(Vec)); //zero the forces
   GetCartesianForces(forces);
   atoms->End();
   return forces;
 }
 
 
 //******************************************************************************
@@ -445,27 +438,27 @@
 
 //******************************************************************************
 //                             GetPotentialEnergy
 //******************************************************************************
 double Morse::GetPotentialEnergy(PyObject *pyatoms)
 {
   DEBUGPRINT;
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   CheckNeighborLists();
   DEBUGPRINT;
   double e = CalculateEnergyAndEnergies();
   atoms->End();
   return e;
 }
 
 const vector<double> &Morse::GetPotentialEnergies(PyObject *pyatoms)
 {
   DEBUGPRINT;
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   CheckNeighborLists();
   CalculateEnergyAndEnergies();
   atoms->End();
   DEBUGPRINT;
   return atomicEnergies;
 }
@@ -477,15 +470,15 @@
   if (counters.energies != atoms->GetPositionsCounter()) {
     memset(&atomicEnergies[0], 0, nAtoms * sizeof(double));
     CalculateEnergyAndEnergies(atomicEnergies);
     counters.energies = atoms->GetPositionsCounter();
   }
 
   double energy = 0.0;
-  ASSERT(atomicEnergies.size() == nAtoms);
+  assert(atomicEnergies.size() == nAtoms);
   for (int a = 0; a < nAtoms; a++) {
     energy +=  atomicEnergies[a];
   }
   return energy;
 }
 
 //******************************************************************************
```

### Comparing `asap3-3.13.1/Potentials/Morse.h` & `asap3-3.9.6/Basics/Morse.h`

 * *Files 4% similar despite different names*

```diff
@@ -97,33 +97,25 @@
   virtual long PrintMemory() const;
 
   void SetAtoms(PyObject *atoms, Atoms* accessobj = NULL); 
   double GetPotentialEnergy(PyObject *atoms);
   const vector<Vec> &GetForces(PyObject *atoms);
   const vector<SymTensor> &GetVirials(PyObject *atoms);
   const vector<double> &GetPotentialEnergies(PyObject *atoms);
-  bool CheckNeighborLists();
+  void CheckNeighborLists();
   double GetCutoffRadius() const {return rCut;}
   double GetLatticeConstant() const {return latticeConstant;}
   /// Return the neighbor list.
 
   /// Return the Python object containing neighbor list for the
   /// potential, if this type of potential supports it, and if it is
   /// defined now.  Otherwise, return NULL without setting a Python
   /// error.
   PyObject *GetNeighborList() const {return neighborList_obj;}
 
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
-
-
   /// This potential can be used in parallel simulations
   virtual bool Parallelizable() const {return true;}
 
   private:
   /** \brief sorts the values in items and adds them up*/
   double Add(vector<double> &items);
   /** \brief return abs(d1) < abs(d2) */
```

### Comparing `asap3-3.13.1/Potentials/Potential.h` & `asap3-3.9.6/Basics/Potential.h`

 * *Files 18% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 ///     special functionalily, such as ParallelPotential (implementing
 ///     parallel simulations) or QCPotential (implementing the
 ///     QuasiContinuum method).
 class Potential : public AsapObject
 {
 public:
   Potential(PyObject *self, int verbose=0) {
+    stresses_cnt = stresses_mom_cnt = -1;
     atoms=NULL;
     this->self = self;
     this->verbose = verbose;
   }
 
   virtual ~Potential() {}
   
@@ -112,50 +113,51 @@
   virtual const vector<SymTensor> &GetVirials(PyObject *a) = 0;
 
   /// Calculate the total "virial" of the system.
   ///
   /// The virial gives the stress of the sytem when divided by the system volume.
   virtual SymTensor GetVirial(PyObject *a);
 
+  /// Calculate the stress on all atoms.
+  virtual const vector<SymTensor> &GetStresses(PyObject *a);
+
+  /// Calculate the total stress of the system.
+  virtual SymTensor GetStress(PyObject *a);
+
   /// Calculate the energy of all atoms.
   virtual const vector<double> &GetPotentialEnergies(PyObject *a) = 0;
 
   // The following three functions are used to check if recalculations
   // are needed.  If a potential does not contain any logic to prevent
   // recalculations, these functions should return True.
 
   /// Is work required to calculate the energy?
   virtual bool CalcReq_Energy(PyObject *pyatoms) {return true;}
 
   /// Is work required to calculate the forces?
   virtual bool CalcReq_Forces(PyObject *pyatoms) {return true;}
 
   /// Is work required to calculate the stress?
-  virtual bool CalcReq_Virial(PyObject *pyatoms) {return CalcReq_Virials(pyatoms);}
   virtual bool CalcReq_Virials(PyObject *pyatoms) {return true;}
 
+  /// Is work required to calculate the stress?
+  virtual bool CalcReq_Stress(PyObject *pyatoms);
+
   // Check if Neighbor lists are up to date.
   //virtual void CheckNeighborLists() = 0;
 
   /// Return the neighbor list.
 
   /// Return a BORROWED reference to the Python object containing
   /// neighbor list for the
   /// potential, if this type of potential supports it, and if it is
-  /// defined now.  Otherwise, returns NULL without setting a Python
+  /// defined now.  Otherwise, return NULL without setting a Python
   /// error.
   virtual PyObject *GetNeighborList() const {return NULL;}
 
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms) = 0;
-
   /// Return the cutoff radius used in the potential.
   virtual double GetCutoffRadius() const = 0;
 
   /// Return the lattice constant of the material, if well-defined.
 
   /// If a lattice constant of the material can be defined, return it
   /// in Angstrom, otherwise throw an exception.
@@ -173,24 +175,27 @@
   virtual long PrintMemory() const = 0;
 
   /// Clean up after an exception.  Called by the interface code.
   void RecoverAfterException();
 
   /// Return the atomic volumes that should be used to calculate the stresses
   ///
+  /// The atoms should already be open, so no atoms parameter is passed.
   /// If an empty volumes vector is returned, GetStress will divide the unit
-  /// cell evenly amongst the atoms.  Can only be used after a call to GetVirials
-  /// with the same atoms; returns cached data, no atoms object is therefore passed
+  /// cell evenly amongst the atoms.
   virtual void GetAtomicVolumes(vector<double> &volumes) {volumes.clear();}
 
-  /// Return the atoms access object.  Used by a few tool functions.
-  virtual Atoms *GetAtoms() {return atoms;}
-
 protected:
   Atoms *atoms;
   PyObject *self;              ///< This objects Python counterpart
   int verbose;     // Verbosity level.
+  
+private:  // These *really* need to be private, not protected!
+  int stresses_cnt;
+  int stresses_mom_cnt;
+  vector<SymTensor> stresses;
+  SymTensor stress;
 };
 
 } // end namespace
 
 #endif // POTENTIAL_H
```

### Comparing `asap3-3.13.1/Potentials/RGL.cpp` & `asap3-3.9.6/Basics/RGL.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -104,15 +104,15 @@
   if (accessobj != NULL) {
     atoms = accessobj;
     AsapAtoms_INCREF(atoms);
   } else {
     atoms = new NormalAtoms();
   }
 
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   nAtoms = atoms->GetNumberOfAtoms();
   nSize = 0;  // Will be set when the NB list is created.  The value 0
               // should create enough trouble to detect if it is used before then.
   atoms->End();
 
   DEBUGPRINT;
@@ -195,20 +195,20 @@
     nSize = nAtoms + atoms->GetNumberOfGhostAtoms();
     ghostatoms = atoms->HasGhostAtoms();
     Allocate();
   }
   DEBUGPRINT;
 }
 
-bool RGL::CheckNeighborList()
+void RGL::CheckNeighborList()
 {
   USETIMER("RGL::CheckNeighborList");
   DEBUGPRINT;
   VERB(" CheckNBL[");
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
 
   // Update if invalid
   bool update = ((neighborlist == NULL) || neighborlist->IsInvalid());  
   if (!update) {
     DEBUGPRINT;
     VERB("u");
     update = neighborlist->CheckNeighborList();
@@ -220,26 +220,16 @@
     DEBUGPRINT;
     VERB("U");
     UpdateNeighborList();
   }
 
   DEBUGPRINT;
   VERB("]" << flush);
-  return update;
 }
 
-bool RGL::CheckAndUpdateNbList(PyObject *pyatoms)
-{
-  atoms->Begin(pyatoms);
-  bool updated = CheckNeighborList();
-  atoms->End();
-  return updated;
-}
-
-
 // Get functions
 double RGL::GetPotentialEnergy(PyObject *pyatoms) {
   USETIMER("RGL::GetPotentialEnergy");
   DEBUGPRINT;
   VERB(" Energy[");
 
   double etot = 0.0;
```

### Comparing `asap3-3.13.1/Potentials/RGL.h` & `asap3-3.9.6/Basics/RGL.h`

 * *Files 16% similar despite different names*

```diff
@@ -54,29 +54,21 @@
     bool CalcReq_Forces(PyObject *pyatoms);
     bool CalcReq_Virials(PyObject *pyatoms) {return CalcReq_Forces(pyatoms);}
 
     // Miscellaneous functions
     bool Parallelizable() const {return true;}
     long PrintMemory() const;
 
-    /// Check and possibly update a neighbor list associated with this potential.
-    ///
-    /// This is the only way a neighbor list borrowed from a potential should be updated.
-    /// Calling this function on a Potential not having a neighbor list is an error.
-    /// Returns true if the neighbor list was actually updated.
-    virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
-
-
   protected:
     void Allocate();
 
     // Neighborlist functions
     void CreateNeighborList();
     void UpdateNeighborList();
-    bool CheckNeighborList();
+    void CheckNeighborList();
 
     // Calculate functions
     void CalculateSigmasAndEnergies();
     void CalculateForcesAfterSigmas();
     void CalculateStressesAfterForces(bool virialonly);
 
     // Data structures and variables
```

### Comparing `asap3-3.13.1/Potentials/RahmanStillingerLemberg.h` & `asap3-3.9.6/Basics/RahmanStillingerLemberg.h`

 * *Files 3% similar despite different names*

```diff
@@ -129,32 +129,25 @@
   virtual long PrintMemory() const;
 
   void SetAtoms(PyObject *atoms, Atoms* accessobj = NULL); 
   double GetPotentialEnergy(PyObject *atoms);
   const vector<Vec> &GetForces(PyObject *atoms);
   const vector<SymTensor> &GetVirials(PyObject *atoms);
   const vector<double> &GetPotentialEnergies(PyObject *atoms);
-  bool CheckNeighborLists();
+  void CheckNeighborLists();
   double GetCutoffRadius() const {return rCut;}
   double GetLatticeConstant() const {return latticeConstant;}
   /// Return the neighbor list.
 
   /// Return the Python object containing neighbor list for the
   /// potential, if this type of potential supports it, and if it is
   /// defined now.  Otherwise, return NULL without setting a Python
   /// error.
   PyObject *GetNeighborList() const {return neighborList_obj;}
 
-  /// Check and possibly update a neighbor list associated with this potential.
-  ///
-  /// This is the only way a neighbor list borrowed from a potential should be updated.
-  /// Calling this function on a Potential not having a neighbor list is an error.
-  /// Returns true if the neighbor list was actually updated.
-  virtual bool CheckAndUpdateNbList(PyObject *pyatoms);
-  
   /// This potential can be used in parallel simulations
   virtual bool Parallelizable() const {return true;}
 
 private:
   /** \brief Allocates the memory needed by the data structures */
   void Allocate();
   /** \brief calculates the total energy and individual energies of the atoms */
@@ -162,14 +155,18 @@
   /** \brief helper function for CalculateEnergyAndEnergies*/
   void CalculateEnergyAndEnergies(vector<double>& atomicEnergies);
 
   /** \brief helper function for GetCartesianForces*/
   /** \param start the start atom id
       \param end   the end atom id (exclusive)*/
   void GetCartesianForces(vector<Vec>& forces);
+  /** \brief  private member function to calculate the stress for a range for atoms with id <code>start</code> to <code>end</code>*/
+  /** \param start the start atom id
+      \param end   the end atom id (exclusive)*/
+  void GetVirials(const Vec *momenta, SymTensor *stresses);
   
   /** \brief converts the parameters to the internal form */
   /** Fills the local epsilon and sigma matrices (stored as an array)
 
       Depending on the paramter *map* either sparse matrices are 
       created or a lookup array to map atom numbers to ids.
       <pre>
```

### Comparing `asap3-3.13.1/Python/asap3/EMT2011_py.py` & `asap3-3.9.6/Python/asap3/EMT2011_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,25 +127,25 @@
                 # Check to see if the elements i,j are defined.
                 if self.n0[i] and self.n0[j] != 0:
                     self.chi[i,j] = self.n0[i] / self.n0[j]
 
 
         ### Calculations of gamma1 and gamma2 ###
 
-        # Four (3 x NumElle)-arrays for lambda_1,2 (named L_1,2) and sigmaa_1,2 are calculated with the distance, 
+	# Four (3 x NumElle)-arrays for lambda_1,2 (named L_1,2) and sigmaa_1,2 are calculated with the distance, 
         # r_ij = (beta * Seq, sqrt(2) * beta * Seq, sqrt(3) * beta * Seq) for all supportet elements. 
         # where Z = Z'.
         
         # The NumberNearestNeighbours variable is set to the number of nearest neighbors included in the model.
-        NumberNearestNeighbours = 3
+	NumberNearestNeighbours = 3
         # arrays for lambda and sigmaa are initialized 
-        L_1_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
-        L_2_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
-        sigmaa_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
-        sigmab_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
+	L_1_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
+	L_2_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
+	sigmaa_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
+	sigmab_Z = numpy.zeros([NumberNearestNeighbours,NumElle])
         # The values for each are calculated for each neighbour distance
         for i in range(NumberNearestNeighbours):
             L_1_Z[i] = (self.dsigmaadrRCUT[range(NumElle),range(NumElle)] *
                        ((sqrt(1 + i) * beta * self.Seq) - self.r_cut[range(NumElle),range(NumElle)]) +
                         self.sigmaaRCUT[range(NumElle),range(NumElle)])
 
             L_2_Z[i] = (self.dsigmabdrRCUT[range(NumElle),range(NumElle)] *
@@ -185,15 +185,15 @@
         (other_j,r_ij,rsq) = self.nbList.get_neighbors(i)
 
         # The neighbor atoms which will actually give a contribution to the energy, based on the individual 
         # cutoff distances between atom i of type Z and atom j of type Z', are selected.
 
         # The neighbor atoms which fullfill the condition are chosen
         keep = numpy.sqrt(rsq) <= self.r_cut[self.Z[i],self.Z[other_j]]
-        
+	
         # The lists of data about the neighbor atoms are updated
         if len(keep) != 0:
             return (other_j[keep],r_ij[keep],rsq[keep])
         else:
             # nbList returned empty lists, but we cannot index a shape (0,3) array (r_ij)
             # with an empty list (bug in numpy?).
             return (other_j,r_ij,rsq)
```

### Comparing `asap3-3.13.1/Python/asap3/EMT2013Parameters.py` & `asap3-3.9.6/Python/asap3/EMT2013Parameters.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Internal/BuiltinPotentials.py` & `asap3-3.9.6/Python/asap3/Internal/BuiltinPotentials.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from __future__ import print_function
 # encoding: utf-8
 
 __docformat__ = "restructuredtext en"
 
 from asap3.Internal.Builtins import _asap
 from asap3.Internal.CheckArray import check_parameter_array, _ChkLJarray
-import asap3
 
 import numpy as np
 import ase
 import ase.calculators.emt
 import ase.data
 from ase.utils import basestring
 from copy import copy
@@ -64,141 +63,62 @@
     pbc = atoms.get_pbc()
     h = get_cell_heights(atoms)
     for i in range(3):
         if pbc[i] and h[i] < smallest:
             smallest = h[i]
     return smallest
 
-class AsapPotential:
-    """Mixin for all Asap potentials."""
-
-    _stresscomp = np.array([[0, 5, 4], [5, 1, 3], [4, 3, 2]])
-
-    def set_atoms_mixin(self, atoms):
-        """Set the atoms.  This mixin fixes compatibility with ASE 3.18.0 and earlier."""
-        if not hasattr(atoms, "get_global_number_of_atoms"):
-            atoms.get_global_number_of_atoms = atoms.get_number_of_atoms
-
-    def set_atoms(self, atoms, *args):
-        """Set the atoms.  This default version fixes compatibility with ASE 3.18.0 and earlier."""
-        self.set_atoms_mixin(atoms)
-        # Now call the potential.
-        super().set_atoms(atoms, *args)
-
-    def get_stress(self, atoms):
-        stress = self.get_virial(atoms)
-        if not getattr(atoms, "_ase_handles_dynamic_stress", False):
-            p = atoms.get_momenta()
-            masses = atoms.get_masses()
-            invmass = 1.0 / masses
-            for alpha in range(3):
-                for beta in range(alpha, 3):
-                    stress[self._stresscomp[alpha,beta]] -= (p[:,alpha] * p[:,beta] * invmass).sum()
-        stress /= atoms.get_volume()
-        return stress
-
-    def get_stresses(self, atoms):
-        stresses = self.get_virials(atoms)
-        if hasattr(self, 'get_atomic_volumes'):
-            invvol = 1.0 / self.get_atomic_volumes()
-        else:
-            invvol = atoms.get_global_number_of_atoms() / atoms.get_volume()
-        if not getattr(atoms, "_ase_handles_dynamic_stress", False):
-            p = atoms.get_momenta()
-            invmass = 1.0 / atoms.get_masses()
-            for alpha in range(3):
-                for beta in range(alpha, 3):
-                    stresses[:,self._stresscomp[alpha,beta]] -= p[:,alpha] * p[:,beta] * invmass
-        for i in range(6):
-            stresses[:,i] *= invvol            
-        return stresses
-
-    def get_property(self, prop, atoms, allow_calculation=True):
-        try:
-            if (not allow_calculation and
-                self.calculation_required(atoms, [prop])):
-                return None
-        except AttributeError:
-            pass
-
-        method = 'get_' + {'energy': 'potential_energy',
-                           'magmom': 'magnetic_moment',
-                           'magmoms': 'magnetic_moments',
-                           'dipole': 'dipole_moment'}.get(prop, prop)
-        try:
-            result = getattr(self, method)(atoms)
-        except AttributeError:
-            raise asap3.PropertyNotImplementedError
-        return result
-
-    def get_name(self):
-        return "asap3." + self._get_name()
-
-    def get_neighborlist(self):
-        """Return the neighbor locator"""
-        return self._get_neighborlist()
-    
-    name = property(get_name, doc="Name of the potential")
-    
-
-class EMT(AsapPotential, _asap.EMT):
+class EMT(_asap.EMT):
     """The Effective Medium Theory potential.
 
     Per default, the EMT potential uses standard parameters for the
     supported metals (Ni, Cu, Pd, Ag, Pt, Au).  If other parameters
     are desired, the relevant parameter provider can be provided as an
     optional argument.
     """
     def __init__(self, parameters=None, minimum_image=None, verbose=None):
         if parameters is None:
             parameters = EMTDefaultParameters()
         if verbose is None:
             verbose = _asap.verbose
         _asap.EMT.__init__(self, parameters, verbose)
-        self.verbose = verbose
         self.absolute_max_cutoff = parameters.get_max_cutoff_beforeinit()
         self._set_atoms_called = False
         self.use_minimum_image = minimum_image
         
     def set_atoms(self, atoms, *args):
-        self.set_atoms_mixin(atoms)
         if not self._set_atoms_called:
             if self.use_minimum_image is None:
                 self.use_minimum_image = smallest_pbc_direction(atoms) >= 2.1 * self.absolute_max_cutoff
             if not self.use_minimum_image:
                 #sys.stderr.write("Asap.EMT: Disabling minimum image convention.\n")
                 self._use_imageatoms()
         self._set_atoms_called = True
         _asap.EMT.set_atoms(self, atoms, *args)
 
-    def get_atomic_volumes(self):
-        return self._get_atomic_volumes()
-
-class MonteCarloEMT(AsapPotential, _asap.MonteCarloEMT):
+def MonteCarloEMT(parameters = None, verbose=None):
     """The Effective Medium Theory potential optimized for Monte Carlo.
 
     Per default, the EMT potential uses standard parameters for the
     supported metals (Ni, Cu, Pd, Ag, Pt, Au).  If other parameters
     are desired, the relevant parameter provider can be provided as an
     optional argument.
 
     This version is optimized for Monte Carlo simulations, at the
     price of somewhat slower ordinary energy and force calculations
     and a larger memory footprint.  In addition, this version cannot
     be parallelized.
     """
-    def __init__(self, parameters=None, verbose=None):
-        if parameters is None:
-            parameters = EMTDefaultParameters()
-        if verbose is None:
-            verbose = _asap.verbose
-        self.verbose = verbose
-        _asap.MonteCarloEMT.__init__(self, parameters, verbose)
+    if parameters is None:
+        parameters = EMTDefaultParameters()
+    if verbose is None:
+        verbose = _asap.verbose
+    return _asap.MonteCarloEMT(parameters, verbose)
 
-class EMT2013(AsapPotential, _asap.EMT2013):
+class EMT2013(_asap.EMT2013):
     """The Effective Medium Theory version 2011 potential.
     
     Parameters must be provided as a dictionary, the keys are
     elements (atomic numbers or strings), the values are dictionaries
     with parameters.  The names of the parameters are 'eta2', 'lambda',
     'kappa', 'E0', 'V0', 'S0' and 'n0'.
     
@@ -235,42 +155,37 @@
             params[z] = copy(parameters[k])
             params[z]['mass'] = ase.data.atomic_masses[z]
             s0 = params[z]['S0']
             if s0 > max_s0:
                 max_s0 = s0
         if verbose is None:
             verbose = _asap.verbose
-        self.verbose = verbose
         _asap.EMT2013.__init__(self, params, no_new_elements, verbose)
         beta = 1.809399790563555  # ((16*pi/3)^(1./3.))/sqrt(2)
         self.maxcut = 0.5 * (np.sqrt(1.5) + np.sqrt(2.)) * np.sqrt(2.) * beta * max_s0 * 1.05
         self._set_atoms_called = False
         self.use_minimum_image = minimum_image
         
     def set_atoms(self, atoms, *args):
-        self.set_atoms_mixin(atoms)
         if not self._set_atoms_called:
             if self.use_minimum_image is None:
                 self.use_minimum_image = smallest_pbc_direction(atoms) >= 2.5 * self.maxcut
             if not self.use_minimum_image:
                 #sys.stderr.write("Asap.EMT2013: Disabling minimum image convention.\n")
                 self._use_imageatoms()
         self._set_atoms_called = True
         _asap.EMT2013.set_atoms(self, atoms, *args)
 
-    def get_atomic_volumes(self):
-        return self._get_atomic_volumes()
-
-
 def EMT2011(parameters):
     """EMT2011 has been renamed EMT2013, please use the new version."""
     sys.stderr.write("\nASAP Warning: EMT2011 is deprecated, use EMT2013 instead.\n")
     return EMT2013(parameters)
 
-class RGL(AsapPotential, _asap.RGL):
+def RGL(elements, p=None, q=None, a=None, xi=None, r0=None,
+        cutoff=1.73, delta=0.15, debug=False, verbose=None):
     """
     Calculator based on the RGL/Gupta semi empirical tight-binding potential.
 
     Parameters
     ----------
     elements: List of the elements that will be supported.
 
@@ -289,136 +204,133 @@
     neighbor distances. Defauls is 0.15.
 
     The cutoff defaults are set to include the 3rd and not the 4th nearest
     neighors. The expected nearest neighbor distance is calculated based
     on the parameters.
     """
 
-    def __init__(self, elements, p=None, q=None, a=None, xi=None, r0=None,
-                 cutoff=1.73, delta=0.15, debug=False, verbose=None):
-        # Check if parameters is given as a dictionary
-        if isinstance(elements, dict):
-            parameters = elements.copy()
-
-            # Get elements
-            elements = []
-            elementmap = {}
-            for key in parameters.keys():
-                if isinstance(key, basestring):
-                    symbols = [key]
-                elif isinstance(key, tuple) and len(key) == 2:
-                    symbols = list(key)
-                else:
-                    raise KeyError('Key must either be a string or a tuple with ' +
-                                   'two elements.')
-                for s in symbols:
-                    if not s in elements:
-                        elementmap[s] = len(elements)
-                        elements.append(s)
-            n = len(elements)
-
-            # Get parameters
-            p = np.zeros((n, n)) 
-            q = np.zeros((n, n)) 
-            a = np.zeros((n, n)) 
-            xi = np.zeros((n, n)) 
-            r0 = np.zeros((n, n)) 
-
-            visit = np.zeros(n)
-            for key in parameters.keys():
-                if isinstance(key, basestring):
-                    i = j = elementmap[key]
-                elif isinstance(key, tuple) and len(key) == 2:
-                    i = elementmap[key[0]]
-                    j = elementmap[key[1]]
-                else:
-                    raise KeyError('Key must either be a string or a tuple with ' +
-                                   'two elements.')
-
-                visit[i] += 1
-                visit[j] += 1
-
-                p[i,j] = parameters[key][0]
-                q[i,j] = parameters[key][1]
-                a[i,j] = parameters[key][2]
-                xi[i,j] = parameters[key][3]
-                r0[i,j] = parameters[key][4]
-
-            if np.any(visit != n + 1):
-                raise ValueError('For some elements there are either too few or ' +
-                                 'too many parameters.')
-
-        # Interpret elements
-        if not isinstance(elements, (tuple, list, np.ndarray)):
-            elements = [elements]
+    # Check if parameters is given as a dictionary
+    if isinstance(elements, dict):
+        parameters = elements.copy()
+
+        # Get elements
+        elements = []
+        elementmap = {}
+        for key in parameters.keys():
+            if isinstance(key, basestring):
+                symbols = [key]
+            elif isinstance(key, tuple) and len(key) == 2:
+                symbols = list(key)
+            else:
+                raise KeyError('Key must either be a string or a tuple with ' +
+                               'two elements.')
+            for s in symbols:
+                if not s in elements:
+                    elementmap[s] = len(elements)
+                    elements.append(s)
         n = len(elements)
 
-        for i, symbol in enumerate(elements):
-            if isinstance(symbol, basestring):
-                elements[i] = ase.data.atomic_numbers[symbol]
-        elements = np.array(elements)
-
-
-        # Interpret parameters
-        p = check_parameter_array(n, "p", p)
-        q = check_parameter_array(n, "q", q)
-        a = check_parameter_array(n, "a", a)
-        xi = check_parameter_array(n, "xi", xi)
-        r0 = check_parameter_array(n, "r0", r0)
-
-        # Calculate cutoff
-        a1 = (np.log(np.sqrt(12) * a * p / (xi * q)) / (p - q) + 1) * r0
-
-        if not np.all((1.0 < a1) & (a1 < 10.0)):
-            raise ValueError('Unreasonable parameters - the nearest neighbor ' +
-                             'distance span [%.3f, %.3f]' % (a1.min(), a1.max()))
-
-        rcs = cutoff * a1.max()
-        rcd = delta * a1.max()
-        rce = rcs + rcd
-        #print "RGL cutoff: %.4f-%.4f" % (rcs, rcd)
-
-        # Calculate parameters for the cutoff function
-        qf = -xi * np.exp(-q * (rcs / r0 - 1)) / rcd**3
-        qd = q / r0 * rcd
-        q5 = (12.0*qf - 6.0*qf*qd + qf*qd*qd) / (2.0 * rcd**2)
-        q4 = (15.0*qf - 7.0*qf*qd + qf*qd*qd) / rcd
-        q3 = (20.0*qf - 8.0*qf*qd + qf*qd*qd) / 2.0
-
-        pf = -a * np.exp(-p * (rcs / r0 - 1)) / rcd**3
-        pd = p / r0 * rcd
-        p5 = (12.0*pf - 6.0*pf*pd + pf*pd*pd) / (2.0 * rcd**2)
-        p4 = (15.0*pf - 7.0*pf*pd + pf*pd*pd) / rcd
-        p3 = (20.0*pf - 8.0*pf*pd + pf*pd*pd) / 2.0
-
-        if debug:
-            print("RGL potential parameters")
-            print("p:", p)
-            print("q:", q)
-            print("a:", a)
-            print("xi:", xi)
-            print("r0:", r0)
-            print("rcs:", rcs)
-            print("rce:", rce)
-            print("q5:", q5)
-            print("q4:", q4)
-            print("q3:", q3)
-            print("p5:", p5)
-            print("p4:", p4)
-            print("p3:", p3)
+        # Get parameters
+        p = np.zeros((n, n)) 
+        q = np.zeros((n, n)) 
+        a = np.zeros((n, n)) 
+        xi = np.zeros((n, n)) 
+        r0 = np.zeros((n, n)) 
+
+        visit = np.zeros(n)
+        for key in parameters.keys():
+            if isinstance(key, basestring):
+                i = j = elementmap[key]
+            elif isinstance(key, tuple) and len(key) == 2:
+                i = elementmap[key[0]]
+                j = elementmap[key[1]]
+            else:
+                raise KeyError('Key must either be a string or a tuple with ' +
+                               'two elements.')
 
-        if verbose is None:
-            verbose = _asap.verbose
-        self.verbose = verbose
-        _asap.RGL.__init__(self, elements, p, q, a, xi * xi, r0, p3, p4, p5,
-                           q3, q4, q5, rcs, rce, verbose)
+            visit[i] += 1
+            visit[j] += 1
+
+            p[i,j] = parameters[key][0]
+            q[i,j] = parameters[key][1]
+            a[i,j] = parameters[key][2]
+            xi[i,j] = parameters[key][3]
+            r0[i,j] = parameters[key][4]
+
+        if np.any(visit != n + 1):
+            raise ValueError('For some elements there are either too few or ' +
+                             'too many parameters.')
+
+    # Interpret elements
+    if not isinstance(elements, (tuple, list, np.ndarray)):
+        elements = [elements]
+    n = len(elements)
+
+    for i, symbol in enumerate(elements):
+        if isinstance(symbol, basestring):
+            elements[i] = ase.data.atomic_numbers[symbol]
+    elements = np.array(elements)
+
+         
+    # Interpret parameters
+    p = check_parameter_array(n, "p", p)
+    q = check_parameter_array(n, "q", q)
+    a = check_parameter_array(n, "a", a)
+    xi = check_parameter_array(n, "xi", xi)
+    r0 = check_parameter_array(n, "r0", r0)
+
+    # Calculate cutoff
+    a1 = (np.log(np.sqrt(12) * a * p / (xi * q)) / (p - q) + 1) * r0
+
+    if not np.all((1.0 < a1) & (a1 < 10.0)):
+        raise ValueError('Unreasonable parameters - the nearest neighbor ' +
+                         'distance span [%.3f, %.3f]' % (a1.min(), a1.max()))
+
+    rcs = cutoff * a1.max()
+    rcd = delta * a1.max()
+    rce = rcs + rcd
+    #print "RGL cutoff: %.4f-%.4f" % (rcs, rcd)
+
+    # Calculate parameters for the cutoff function
+    qf = -xi * np.exp(-q * (rcs / r0 - 1)) / rcd**3
+    qd = q / r0 * rcd
+    q5 = (12.0*qf - 6.0*qf*qd + qf*qd*qd) / (2.0 * rcd**2)
+    q4 = (15.0*qf - 7.0*qf*qd + qf*qd*qd) / rcd
+    q3 = (20.0*qf - 8.0*qf*qd + qf*qd*qd) / 2.0
+
+    pf = -a * np.exp(-p * (rcs / r0 - 1)) / rcd**3
+    pd = p / r0 * rcd
+    p5 = (12.0*pf - 6.0*pf*pd + pf*pd*pd) / (2.0 * rcd**2)
+    p4 = (15.0*pf - 7.0*pf*pd + pf*pd*pd) / rcd
+    p3 = (20.0*pf - 8.0*pf*pd + pf*pd*pd) / 2.0
+
+    if debug:
+        print("RGL potential parameters")
+        print("p:", p)
+        print("q:", q)
+        print("a:", a)
+        print("xi:", xi)
+        print("r0:", r0)
+        print("rcs:", rcs)
+        print("rce:", rce)
+        print("q5:", q5)
+        print("q4:", q4)
+        print("q3:", q3)
+        print("p5:", p5)
+        print("p4:", p4)
+        print("p3:", p3)
+
+    if verbose is None:
+        verbose = _asap.verbose
+    return _asap.RGL(elements, p, q, a, xi * xi, r0, p3, p4, p5,
+                     q3, q4, q5, rcs, rce, verbose)
 
 Gupta = RGL
 
-class LennardJones(AsapPotential, _asap.LennardJones):
+def LennardJones(elements, epsilon, sigma, rCut=-1.0, modified=True, verbose=None):
     """Lennard-Jones potential.
 
     Parameters:
     
     elements:  Lists the elements that will be supported.
     
     epsilon and sigma: The LJ parameters.  2D arrays with each
@@ -429,66 +341,57 @@
     and sigma may be numbers.
 
     rCut:  The cutoff distance.  Default: XXX
 
     modified: Should the potential be shifted so no jump occurs at the
     cutoff.  Default: True.
     """
-    def __init__(self, elements, epsilon, sigma, rCut=-1.0, modified=True, verbose=None):
-        try:
-            numelements = len(elements)
-        except TypeError:
-            numelements = 1
-            elements = [elements]
-
-        epsilon = _ChkLJarray(epsilon, numelements, "epsilon")
-        sigma = _ChkLJarray(sigma, numelements, "sigma")
-        masses = [ase.data.atomic_masses[z] for z in elements]
-
-        if verbose is None:
-            verbose = _asap.verbose
-        self.verbose = verbose
-        _asap.LennardJones.__init__(self, numelements, elements, epsilon, sigma,
-                                    masses, rCut, modified, verbose)
+    try:
+        numelements = len(elements)
+    except TypeError:
+        numelements = 1
+        elements = [elements]
+
+    epsilon = _ChkLJarray(epsilon, numelements, "epsilon")
+    sigma = _ChkLJarray(sigma, numelements, "sigma")
+    masses = [ase.data.atomic_masses[z] for z in elements]
+
+    if verbose is None:
+        verbose = _asap.verbose
+    return _asap.LennardJones(numelements, elements, epsilon, sigma,
+                              masses, rCut, modified, verbose)
 
-    # Atomic volumes disabled in the C code.
-    #def get_atomic_volumes(self):
-    #    return self._get_atomic_volumes()
-
-
-class RahmanStillingerLemberg(AsapPotential, _asap.RahmanStillingerLemberg):
+def RahmanStillingerLemberg(D0, R0, y, a1, b1, c1, a2, b2, c2, a3, b3, c3, 
+                            elements, rCut=1.0, verbose=None):
     """Rahman Stillinger Lemberg potential (RSL2).
     """
-    def __init__(self, D0, R0, y, a1, b1, c1, a2, b2, c2, a3, b3, c3, 
-                 elements, rCut=1.0, verbose=None):
-        try:
-            numelements = len(elements)
-        except TypeError:
-            numelements = 1
-            elements = [elements]
-
-        D0 = _ChkLJarray(D0, numelements, "D0")
-        R0 = _ChkLJarray(R0, numelements, "R0")
-        y = _ChkLJarray(y, numelements, "y")
-        a1 = _ChkLJarray(a1, numelements, "a1")
-        b1 = _ChkLJarray(b1, numelements, "b1")
-        c1 = _ChkLJarray(c1, numelements, "c1")
-        a2 = _ChkLJarray(a2, numelements, "a2")
-        b2 = _ChkLJarray(b2, numelements, "b2")
-        c2 = _ChkLJarray(c2, numelements, "c2")
-        a3 = _ChkLJarray(a3, numelements, "a3")
-        b3 = _ChkLJarray(b3, numelements, "b3")
-        c3 = _ChkLJarray(c3, numelements, "c3")
-        masses = [ase.data.atomic_masses[z] for z in elements]
-        if verbose is None:
-            verbose = _asap.verbose
-        self.verbose = verbose
-        _asap.RahmanStillingerLemberg.__init__(self, numelements, 
-                    D0, R0, y, a1, b1, c1, a2, b2, c2, a3, b3, c3, 
-                    elements, masses, rCut, verbose)
+    try:
+        numelements = len(elements)
+    except TypeError:
+        numelements = 1
+        elements = [elements]
+
+    D0 = _ChkLJarray(D0, numelements, "D0")
+    R0 = _ChkLJarray(R0, numelements, "R0")
+    y = _ChkLJarray(y, numelements, "y")
+    a1 = _ChkLJarray(a1, numelements, "a1")
+    b1 = _ChkLJarray(b1, numelements, "b1")
+    c1 = _ChkLJarray(c1, numelements, "c1")
+    a2 = _ChkLJarray(a2, numelements, "a2")
+    b2 = _ChkLJarray(b2, numelements, "b2")
+    c2 = _ChkLJarray(c2, numelements, "c2")
+    a3 = _ChkLJarray(a3, numelements, "a3")
+    b3 = _ChkLJarray(b3, numelements, "b3")
+    c3 = _ChkLJarray(c3, numelements, "c3")
+    masses = [ase.data.atomic_masses[z] for z in elements]
+    if verbose is None:
+        verbose = _asap.verbose
+    return _asap.RahmanStillingerLemberg(numelements, 
+                                         D0, R0, y, a1, b1, c1, a2, b2, c2, a3, b3, c3, 
+                                         elements, masses, rCut, verbose)
 
 # def Ewald(q, elements, rCut=1.0):
 #     """Lennard-Jones potential.
 
 #     Parameters:
     
 #     elements:  Lists the elements that will be supported.
@@ -512,91 +415,88 @@
 #         elements = [elements]
 
 #       q = _ChkLJarray(q, numelements, "q")
 #     masses = [ase.data.atomic_masses[z] for z in elements]
     
 #     return _asap.Ewald(numelements, q, elements, masses, rCut)
 
-class MetalOxideInterface(AsapPotential, _asap.MetalOxideInterface):
+class MetalOxideInterface(_asap.MetalOxideInterface):
     def __init__(self,
                  P, Q, A, xi, r0, RGL_cut, 
                  q, kappa, 
                  D, alpha, R0, 
                  a, b, f0, oxide_cut,
                  beta, gamma, interface_cut, verbose=None):
         if verbose is None:
             verbose = _asap.verbose
-        self.verbose = verbose
         _asap.MetalOxideInterface.__init__(self, 
             P, Q, A, xi, r0, RGL_cut, 
             q, kappa, 
             D, alpha, R0, 
             a, b, f0, oxide_cut,
             beta, gamma, interface_cut, verbose)
         
         self.max_cutoff = max(RGL_cut, oxide_cut, interface_cut)
         self.atoms_intialized = False
         self._set_atoms_called = False
 
     def set_atoms(self, atoms, *args):
-        self.set_atoms_mixin(atoms)
+        
         if not self._set_atoms_called:
             if smallest_pbc_direction(atoms) < 2.05 * self.max_cutoff:
                 print('Using image atoms')
                 self._use_imageatoms()
             self._set_atoms_called = True
             
         if hasattr(atoms, 'ghosts'):
             atoms.ghosts['assignment'] = np.zeros((0,),dtype=np.int32)
         if hasattr(atoms, 'ghosts'):
             atoms.ghosts['monolayer'] = np.zeros((0,),dtype=np.int32)
         
         _asap.MetalOxideInterface.set_atoms(self, atoms, *args)
 
-class MetalOxideInterface2(AsapPotential, _asap.MetalOxideInterface2):
+class MetalOxideInterface2(_asap.MetalOxideInterface2):
     def __init__(self,
                 P, Q, A, xi, r0, RGL_cut, 
                 q, kappa, 
                 D, alpha, R0, 
                 a, b, f0, oxide_cut,
                 E, rho0, l0,
                 B, C,
                 interface_cut, verbose=None):
         if verbose is None:
             verbose =_asap.verbose
-        self.verbose = verbose
         _asap.MetalOxideInterface2.__init__(self, 
             P, Q, A, xi, r0, RGL_cut, 
             q, kappa, 
             D, alpha, R0, 
             a, b, f0, oxide_cut,
             E, rho0, l0,
             B, C,
             interface_cut, verbose)
         
         self.max_cutoff = max(RGL_cut, oxide_cut, interface_cut)
         self.atoms_intialized = False
         self._set_atoms_called = False
 
     def set_atoms(self, atoms, *args):
-        self.set_atoms_mixin(atoms)
         if not self._set_atoms_called:
             if smallest_pbc_direction(atoms) < 2.05 * self.max_cutoff:
                 print('Using image atoms')
                 self._use_imageatoms()
             self._set_atoms_called = True
             
         if hasattr(atoms, 'ghosts'):
             atoms.ghosts['assignment'] = np.zeros((0,),dtype=np.int32)
         if hasattr(atoms, 'ghosts'):
             atoms.ghosts['monolayer'] = np.zeros((0,),dtype=np.int32)
 
         _asap.MetalOxideInterface2.set_atoms(self, atoms, *args)
 
-class Morse(AsapPotential, _asap.Morse):
+def Morse(elements, epsilon, alpha, rmin, rCut=-1.0, modified=True, verbose=None):
     """Lennard-Jones potential.
 
     Parameters:
     
     elements:  Lists the elements that will be supported.
     
     epsilon, alpha and rmin: The Morse potential parameters.
@@ -607,29 +507,27 @@
     then epsilon and sigma may be numbers.
 
     rCut:  The cutoff distance.  Default: XXX
 
     modified: Should the potential be shifted so no jump occurs at the
     cutoff.  Default: True.
     """
-    def __init__(self, elements, epsilon, alpha, rmin, rCut=-1.0, modified=True, verbose=None):
-        try:
-            numelements = len(elements)
-        except TypeError:
-            numelements = 1
-            elements = [elements]
-        epsilon = _ChkLJarray(epsilon, numelements, "epsilon", "Morse")
-        alpha = _ChkLJarray(alpha, numelements, "alpha", "Morse")
-        rmin = _ChkLJarray(rmin, numelements, "rmin", "Morse")
-        if verbose is None:
-            verbose = _asap.verbose
-        self.verbose = verbose
+    try:
+        numelements = len(elements)
+    except TypeError:
+        numelements = 1
+        elements = [elements]
+    epsilon = _ChkLJarray(epsilon, numelements, "epsilon", "Morse")
+    alpha = _ChkLJarray(alpha, numelements, "alpha", "Morse")
+    rmin = _ChkLJarray(rmin, numelements, "rmin", "Morse")
+    if verbose is None:
+        verbose = _asap.verbose
 
-        _asap.Morse.__init__(self, elements, epsilon, alpha,
-                             rmin, rCut, modified, verbose)
+    return _asap.Morse(elements, epsilon, alpha,
+                       rmin, rCut, modified, verbose)
 
 
 # Disable ase.EMT to prevent catastrophic loss of performance.
 ase.calculators.emt.EMT.disabled = "Disabled by loading asap3."
 
 # Register if an OpenKIMcalculator is available
 OpenKIMsupported = hasattr(_asap, 'OpenKIMcalculator')
```

### Comparing `asap3-3.13.1/Python/asap3/Internal/CheckArray.py` & `asap3-3.9.6/Python/asap3/Internal/CheckArray.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Internal/Collector.py` & `asap3-3.9.6/Python/asap3/Internal/Collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,47 +6,41 @@
 import asap3
 import numpy as np
 
 class Collector:
     "Atoms-like filter collecting information on the master node."
     _is_asap_collector_object=True
 
-    def __init__(self, atoms, master=None, allow_forces=False, noconstraints=True):
+    def __init__(self, atoms, master=None, allow_forces=False):
         self.atoms = atoms
         self.comm = atoms.get_comm()
         self.allow_forces = allow_forces
         if master is None:
             master = (self.comm.rank == 0)
         self.master = master
-        if noconstraints:
-            self.constraints = []
-        else:
-            self.constraints = self.atoms.constraints
+        self.constraints = self.atoms.constraints
         self.reset_collector()
         
     def reset_collector(self):
         """Cache some stuff so Trajectory does not block."""
-        self._n = self.atoms.get_global_number_of_atoms()
+        self._n = self.atoms.get_number_of_atoms()
         try:
             del self.numbers
         except AttributeError:
             pass
         self.numbers = self.get_atomic_numbers()
 
     def __len__(self):
         if self.master:
             return self._n
         else:
             return 0
 
-    def get_global_number_of_atoms(self):
-        return self.atoms.get_global_number_of_atoms()
-
-    # Compatibility with ASE 3.18.0 and earlier
-    get_number_of_atoms = get_global_number_of_atoms
+    def get_number_of_atoms(self):
+        return self.atoms.get_number_of_atoms()
 
     def get_positions(self):
         return self.collect(self.atoms.get_positions)
 
     def get_forces(self):
         return self.collect(self.atoms.get_forces)
 
@@ -68,54 +62,45 @@
     def get_cell(self):
         return self.atoms.get_cell()
 
     def get_calculator(self):
         """Return a fake calculator that makes Trajectory work when it calls calculation_required."""
         return CollectorCalculator(self.atoms.get_calculator(), self.allow_forces)
 
-    @property
-    def calc(self):
-        """Calculator object."""
-        return self.get_calculator()
-    
     def get_stress(self):
         return self.atoms.get_stress()
 
     def get_pbc(self):
         return self.atoms.get_pbc()
     
     def get_info(self):
         return self.atoms.info
     
     def get_charges(self):
-        raise asap3.PropertyNotImplementedError
+        raise NotImplementedError
     
     def get_array(self, label):
         return self.collect(lambda a=self.atoms, l=label: a.get_array(l))
 
     def has(self, name):
         """Check for existance of array.
 
         name must be one of: 'tags', 'momenta', 'masses', 'magmoms',
         'charges'.
         """
         if name in ['positions', 'tags', 'momenta', 'numbers']:
             return self.atoms.has(name) 
         else:
             return False
-
-    def iterimages(self):
-        """An atom is also a list of images."""
-        yield self
-
+    
     def collect(self, method):
         "Collect data from all cpus onto the master."
         ids = self.atoms.get_ids()
         data = method()
-        n = self.atoms.get_global_number_of_atoms()
+        n = self.atoms.get_number_of_atoms()
         if self.master:
             shape = (n,) + data.shape[1:]
             result = np.zeros(shape, data.dtype)
             for cpu in range(self.comm.size):
                 if cpu != 0:
                     # Receive from cpu
                     nrecv = np.zeros(1, int)
@@ -160,45 +145,24 @@
     needs to test which quantities are available.  The calls are forwarded to
     the real potential acting on the real atoms.
     """
     def __init__(self, calc, allow_forces):
         try:
             self.name = calc.name
         except AttributeError:
-            try:
-                self.name = "asap3." + calc._get_name()
-            except AttributeError:
-                self.name = calc.__class__.__name__
+            self.name = calc.__class__.__name__.lower()
         self.allow_forces = allow_forces
         
     def calculation_required(self, atoms, props):
         if not self.allow_forces and 'forces' in props:
             return True
         assert isinstance(atoms, Collector)
         realcalc = atoms.atoms.get_calculator()
         x = realcalc.calculation_required(atoms.atoms, props)
         return x
     
-    # def get_potential_energy(self, atoms):
-    #     return atoms.atoms.get_potential_energy()
-    
-    # def get_forces(self, atoms):
-    #     return atoms.atoms.get_forces()
-
-    def get_property(self, prop, atoms, allow_calculation=True):
-        assert isinstance(atoms, Collector)
-        try:
-            if (not allow_calculation and
-                self.calculation_required(atoms, [prop])):
-                return None
-        except AttributeError:
-            pass
-
-        method = 'get_' + {'energy': 'potential_energy'}.get(prop, prop)
-        try:
-            result = getattr(atoms, method)()
-        except AttributeError:
-            raise asap3.PropertyNotImplementedError
-        return result
+    def get_potential_energy(self, atoms):
+        return atoms.atoms.get_potential_energy()
     
-                     
-            
+    def get_forces(self, atoms):
+        return atoms.atoms.get_forces()
+
```

### Comparing `asap3-3.13.1/Python/asap3/Internal/EMTParameters.py` & `asap3-3.9.6/Python/asap3/Internal/EMTParameters.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Internal/ListOfElements.py` & `asap3-3.9.6/Python/asap3/Internal/ListOfElements.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Internal/MonteCarloAtoms.py` & `asap3-3.9.6/Python/asap3/Internal/MonteCarloAtoms.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Internal/OpenKIMcalculator.py` & `asap3-3.9.6/Python/asap3/Internal/OpenKIMcalculator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,149 +1,280 @@
-"""A calculator based on the OpenKIM project.
-
-This module defines three object.
-
-OpenKIMcalculator is a calculator class that interfaces to any OpenKIM V2 model.
-
-OpenKIMparameters is a dictionary-like object that gives access to any
-mutable parameters of the OpenKIM model, the object is created by
-calling OpenKIMcalculator.get_parameters().
-
-OpenKIMavailable is a function returning a list of available OpenKIM models.
-"""
-from __future__ import print_function, division
+"""A calculator based on the OpenKIM project."""
+from __future__ import print_function
 
 from ase.calculators.calculator import Calculator
-from asap3 import _asap, AsapError
+from asap3 import _asap
 from asap3.Internal.ListOfElements import ListOfElements
-from asap3.Internal.BuiltinPotentials import get_cell_heights, smallest_pbc_direction, AsapPotential
+from asap3.Internal.BuiltinPotentials import get_cell_heights, smallest_pbc_direction
 from ase.data import atomic_numbers, chemical_symbols
 from ase.utils import basestring
 import numpy as np
 from copy import copy
-import subprocess
-import shutil
-import os
-from collections.abc import MutableMapping
-import numbers
 
-class OpenKIMcalculator(_asap.OpenKIMcalculator, AsapPotential):
+OpenKIMinfo = _asap.OpenKIMinfo
+
+kim_file_template = """#
+# Autogenerated KIM specification file.
+#
+# Generated by the Asap module OpenKIMcalculator.
+#
+
+KIM_API_Version := 1.6.0
+
+#  UNITS
+Unit_length      := A
+Unit_energy      := eV
+Unit_charge      := e
+Unit_temperature := K
+Unit_time        := ps
+
+SUPPORTED_ATOM/PARTICLES_TYPES:
+# Symbol/name               Type                    code
+%(symbols)s
+
+CONVENTIONS:
+# Name                      Type
+ZeroBasedLists              flag
+%(neighboraccess)s
+%(neighbormethods)s
+
+MODEL_INPUT:
+# Name                      Type         Unit                Shape              Requirements
+numberOfParticles           integer      none                []
+numberOfSpecies             integer      none                []
+particleSpecies             integer      none                [numberOfParticles]
+coordinates                 double       length              [numberOfParticles,3]
+get_neigh                   method       none                []
+neighObject                 pointer      none                []
+numberContributingParticles integer      none                []
+boxSideLengths              double       length              [3]
+
+MODEL_OUTPUT:
+# Name                      Type         Unit                Shape              Requirements
+destroy                     method       none                []
+compute                     method       none                []
+cutoff                      double       length              []
+%(energy)s
+%(forces)s
+%(particleEnergy)s
+%(virial)s
+%(particleVirial)s
+"""
+
+element_template = "%-2s                          spec                    %i\n"
+output_template = "%-27s double       %-19s [%s]"
+nb_template = "%-27s flag\n"
+
+class OpenKIMcalculator(_asap.OpenKIMcalculator):
     """A calculator interfacing to the OpenKIM models.
     
     Parameters:
     
     name: The long name of the KIM Model.
     
     Optional parameters:
     
     atoms:  If set, set_atoms is called immediately.  Default: no atoms set.
-                           
+    
+    allowed:  List of OpenKIM neighbor list keywords, only these will be considered when 
+              matching the model.  Default: ALl neighbor list modes are allowed.
+              
+    allow_mi_opbc:  If set to False, minimum-image orthogonal periodic boundary condition
+                    methods are not considered when mathcing the neighbor lists.  Useful
+                    if the cell is expected to become skewed during the simulation.
+
+    access:  Set to "iter" or "loca" to restrict the neigbor list access method to
+             iterator mode or locator mode, respectively.  Default: not restricted.
+             
     stress:  Set to False to refrain from calculate the global virial, even if the model
              supports it.  Default:  True (calculate global virial / stress).
              
     stresses: As above, but for atomic virials / stresses.
     
     verbose:  Set to True to print additional info during neigborlist matching.
     """
-    def __init__(self, name, atoms=None,
+    def __init__(self, name, atoms=None, allowed=None, allow_mi_opbc=True, access=None,
                  stress=True, stresses=True, verbose=False):
-        _asap.OpenKIMcalculator.__init__(self, name, verbose)
-        self.kimname = name
+        _asap.OpenKIMcalculator.__init__(self)
+        self.name = name
         self.atoms = None
+        self.allowed = allowed
+        self.allow_mi_opbc = allow_mi_opbc
+        self.access = access
         self.support_stress = stress
         self.support_stresses = stresses
         self.verbose = verbose
         if atoms is not None:
             self.set_atoms(atoms)
             
     def set_atoms(self, atoms, *args):
         """Set the atoms belonging to this calculator.
         
         The function set_atoms(atoms) is defined in C++, and just calls this
         Python function.  This ensures that this Python function is called
         regardless of whether set_atoms() is called from C++ or Python.
         """
+        self.kim_spec = self.get_kim_spec(atoms)
+        #print self.kim_spec
+        self._initialize(self.kim_spec, self.name)
+        # Inform the calculator about which quantities should be allocated and calculated.
+        for k,v in self.supported_calculations.items():
+            self.please_allocate(k, v)
         # Inform the calculator about the translation from atomic numbers to particle types.
+        supported_elements = [atomic_numbers[sym] for sym in self.get_supported_types()]
         self.z_to_typecode = {}
         elements = ListOfElements(atoms)
         for e in elements:
-            symbol = chemical_symbols[e]
-            try:
-                code = self.get_type_code(chemical_symbols[e])
-            except AsapError:
+            if e not in supported_elements:
                 raise RuntimeError("The OpenKIM model '%s' does not support element Z=%i (%s)."
-                                   % (self.kimname, e, chemical_symbols[e]))
+                                   % (self.name, e, chemical_symbols[e]))
+            code = self.get_type_code(chemical_symbols[e])
+            if code < 0:
+                raise ValueError("Negative KIM type codes not supported - what do they mean?")
             self.z_to_typecode[e] = code
             if self.verbose:
                 print("Translation: Z = %i -> id = %i" % (e, code))
         self.set_translation(self.z_to_typecode)
-
-        # Check the compute arguments required by the Model.
-        computearguments = self._get_compute_arguments()
-        requiredargs = ['numberOfParticles', 'particleSpeciesCodes', 'particleContributing',
-                        'coordinates', 'partialEnergy', 'partialForces', 'GetNeighborList']
-        for a in requiredargs:
-            if computearguments[a] == 'notSupported':
-                raise AsapError("The OpenKIM model '{}' does not support '{}'".format(self.kimname, a))
-            del computearguments[a]  # Processed
-        self.supported_calculations = {}
-        for k in ('partialEnergy', 'partialForces'):
-            self.supported_calculations[k] = True
-        
-        # partialParticleEnergy is optional, but we will calculate it if possible
-        arg = 'partialParticleEnergy'
-        self.supported_calculations[arg] = computearguments[arg] != 'notSupported'
-        del computearguments[arg]
-        # partialVirial and partialParticleVirial are allocated if they are required by the model, or if
-        # they are optional and stress is requested.
-        arg = 'partialVirial'
-        self.supported_calculations[arg] = (
-            computearguments[arg] == 'required' or
-            (self.support_stress and computearguments[arg] == 'optional'))
-        del computearguments[arg]
-        arg = 'partialParticleVirial'
-        self.supported_calculations[arg] = (
-            computearguments[arg] == 'required' or
-            (self.support_stress and computearguments[arg] == 'optional'))
-        del computearguments[arg]
-        # Make sure that the model does not require something extra.
-        for a, s in computearguments.items():
-            if s == 'required' or s == 'requiredByAPI':
-                raise RuntimeError("OpenKIM model '{}' requires parameter '{}' (status: '{}')".format(
-                    self.name, a, s))
-        
-        # Inform the calculator about which quantities should be allocated and calculated.
-        for k,v in self.supported_calculations.items():
-            self.please_support(k, v)
-
         # Find out which neighborlist type we got.  Check sanity and if ImageAtoms should be used.
+        nblistmethod = self.get_NBC_method()
         pbc = atoms.get_pbc()
+        cutoff = self.get_cutoff()
         if self.verbose:
-            print("Activating Image atoms (pbc = {})".format(str(pbc)))
-        self._use_imageatoms()
+            print("Neighbor list method: %s;  cutoff: %.3f A;  pbc: %s" % (nblistmethod, cutoff, pbc))
+        if nblistmethod == 'CLUSTER':
+            if not np.array_equal(pbc, (False, False, False)):
+                raise RuntimeError("OpenKIM chose CLUSTER, but PBC are "+str(pbc))
+        elif nblistmethod == 'NEIGH_RVEC_H' or nblistmethod == 'NEIGH_RVEC_F':
+            if smallest_pbc_direction(atoms) < 3 * cutoff:
+                if self.verbose:
+                    print("Disabling minimum image convention for", nblistmethod)
+                self._use_imageatoms()
+        elif nblistmethod == "NEIGH_PURE_H" or nblistmethod == "NEIGH_PURE_F":
+            if self.verbose:
+                print("Activating Image atoms for", nblistmethod)
+            self._use_imageatoms()
+        elif nblistmethod == "MI_OPBC_H" or nblistmethod == "MI_OPBC_F":
+            if not np.array_equal(pbc, (True, True, True)):
+                raise RuntimeError("OpenKIM chose %s, but PBC are %s" (nblistmethod, str(pbc)))
+            if smallest_pbc_direction(atoms) < 2 * cutoff:
+                raise RuntimeError("OpenKIM chose %s, but system is too small." % (nblistmethod,))
         _asap.OpenKIMcalculator.set_atoms(self, atoms, *args)
-
-    def get_supported_elements(self, user=True):
-        """Get a list of supported elements (as chemical symbols).
-
-        If the optional argument user=True (the default) then elements with
-        names 'user01' to 'user20' may also be returned as supported.
+        
+    def get_kim_spec(self, atoms):
+        """Return the KIM specification string.
+        
+        Side effects:
+        self.supported_calculations (dictionary) will indicate which quantities
+        can be calculated by the Model.
+        self.z_to_typecode (dictionary) gives the translation from the 
+        atomic numbers to the type codes of the model.
         """
-        supported = []
-        candidates = chemical_symbols[1:]  # chemical_symbols[0] is 'X' and should be skipped.
-        if user:
-            candidates += ['user{:02d}'.format(x) for x in range(1,21)]
-        for element in candidates:
-            try:
-                self.get_type_code(element)
-            except AsapError:
-                pass
-            else:
-                supported.append(element)
-        return supported
+        kim_variables = {'symbols': '', 'neighbormethods': ''}
+        elements = ListOfElements(atoms)
+        info = OpenKIMinfo(self.name)
+        supported_elements = [atomic_numbers[sym] for sym in info.get_supported_types()]
+        self.z_to_typecode = {}
+        for e in elements:
+            if e not in supported_elements:
+                raise RuntimeError("The OpenKIM model '%s' does not support element Z=%i (%s)."
+                                   % (self.name, e, chemical_symbols[e]))
+            kim_variables['symbols'] += element_template % (chemical_symbols[e], e)
+        test_methods = ('energy', 'particleEnergy', 'forces', 'virial', 'particleVirial')
+        self.supported_calculations = {}
+        for method in test_methods:
+            self.supported_calculations[method] = info.get_API_index(method) > 0
+        if not self.support_stress:
+            self.supported_calculations['virial'] = False
+        if not self.support_stresses:
+            self.supported_calculations['particleVirial'] = False
+        if self.supported_calculations['energy']:
+            kim_variables['energy'] = output_template % ('energy', 'energy', '')
+        else:
+            kim_variables['energy'] = ''
+        if self.supported_calculations['particleEnergy']:
+            kim_variables['particleEnergy'] = output_template % ('particleEnergy', 'energy', 'numberOfParticles')
+        else:
+            kim_variables['particleEnergy'] = ''
+        if self.supported_calculations['forces']:
+            kim_variables['forces'] = output_template % ('forces', 'force', 'numberOfParticles,3')
+        else:
+            kim_variables['forces'] = ''
+        if self.support_stress and self.supported_calculations['virial']:
+            kim_variables['virial'] = output_template % ('virial', 'energy', '6')
+        else:
+            kim_variables['virial'] = ''
+        if self.support_stress and self.supported_calculations['particleVirial']:
+            kim_variables['particleVirial'] = output_template % ('particleVirial', 'energy', 'numberOfParticles,6')
+        else:
+            kim_variables['particleVirial'] = ''
+        nb_methods = self.find_neighbor_methods(atoms)
+        for nbm in nb_methods:
+            kim_variables['neighbormethods'] += nb_template % (nbm,)
+        if self.access == None:
+            kim_variables['neighboraccess'] = "Neigh_IterAccess            flag\nNeigh_LocaAccess            flag"
+        elif self.access.lower() == 'iter':
+            if self.verbose:
+                print("Using Neigh_IterAccess only")
+            kim_variables['neighboraccess'] = "Neigh_IterAccess            flag"
+        elif self.access.lower() == 'loca':
+            if self.verbose:
+                print("Using Neigh_LocaAccess only")
+            kim_variables['neighboraccess'] = "Neigh_LocaAccess            flag"
+        else:
+            raise ValueError("Illegal value for neighborlist access method: " + str(self.access))
+        return kim_file_template % kim_variables          
+        
+    def find_neighbor_methods(self, atoms):
+        """Find which neighbor methods are relevant for this atom type
+        
+        Parameters:
+        atoms: 
+        The atoms object - its cell and PBC are examined.
+        
+        allowed (optional, default=None): 
+        The list of neighborlist methods being considered, in prioritized order.  
+        The default (None) means all methods, in the order NEIGH_RVEC_H, 
+        NEIGH_PURE_H, NEIGH_RVEC_F, NEIGH_PURE_F, MI_OPBC_H, MI_OPBC_F, 
+        CLUSTER.
+        
+        allow_mi_opbc (optional, default=True):
+        If set to False, the methods MI_OPBC_H/F will not be considered.  Normally,
+        they are considered if there are full periodic boundary conditions and the
+        unit cell is orthorhombic.  However, the unit cell may change during a
+        simulation, in those cases preventing these boundary conditions may be
+        a good idea.
+        """
+        if not self.allowed:
+            allowed = ["NEIGH_RVEC_H", "NEIGH_PURE_H", "NEIGH_RVEC_F", 
+                       "NEIGH_PURE_F", "MI_OPBC_H", "MI_OPBC_F",
+                       "CLUSTER"]
+        elif isinstance(self.allowed, basestring):
+            allowed = [self.allowed,]
+        else:
+            allowed = copy(self.allowed)  # Will be modified
+        remove = []
+        uc = atoms.get_cell()
+        diagonal = True
+        for i in range(3):
+            for j in range(3):
+                if i != j and np.abs(uc[i,j]) > 1e-15:
+                    diagonal = False  
+        if not (self.allow_mi_opbc and atoms.get_pbc().all() and diagonal):
+            # Minimum Image Orthogonal Periodic Boundary Conditions
+            # are not allowed
+            remove.extend(["MI_OPBC_H", "MI_OPBC_F"])
+        if  atoms.get_pbc().any():
+            # Cluster method is not allowed
+            remove.append("CLUSTER")
+        for rem in remove:
+            if rem in allowed:
+                allowed.remove(rem)
+        if self.verbose:
+            print("Allowed PBC:", allowed)
+        return allowed
     
     def get_parameters(self, kind='free', integers=[]):
         """Get the parameters of the model as a dictionary.
         
         The optional parameter 'kind' specifies which kind of parameters you get.
         It can take three values:
         'free' (the default).  You only get the "free" parameters, i.e. those that
@@ -219,163 +350,15 @@
             if isinstance(value, float):
                 self._set_parameter_scalar(realkey, value)
             elif isinstance(value, np.ndarray):
                 self._set_parameter_array(realkey, value)
             else:
                 raise TypeError("Unsupported value type - must be float or numpy array.")
         self._reinit()
-
-    def get_name(self):
-        return "asap3.OpenKIMcalculator(" + self.kimname + ")"
-
-    def _get_parameters(self):
-        return OpenKIMparameters(self)
     
-    name = property(get_name, doc="Name of the potential")
-
-    parameters = property(_get_parameters, doc="Published parameters of the OpenKIM model")
-
-class OpenKIMparameters(MutableMapping):
-    def __init__(self, model):
-        self.model = model
-        self.parameters = {}
-        self.descriptions = {}
-        for i, (name, typecode, size, description) in enumerate(model._get_parameter_names_types()):
-            self.parameters[name] = (i, typecode, size)
-            self.descriptions[name] = description
-
-    def __len__(self):
-        return len(self.parameters)
-
-    def __getitem__(self, key):
-        return self.model._get_parameter(*self.parameters[key])
-
-    def __setitem__(self, key, value):
-        index = self.parameters[key][0]
-        if isinstance(value, numbers.Number):
-            # A scalar
-            self.model._set_parameter(index, value)
-        else:
-            # An array - flatten it.
-            self.model._set_parameter(index, np.ravel(value)) 
-
-    def __delitem__(self, key):
-        raise RuntimeError("Cannot delete a parameter from an OpenKIM model.")
-    
-    def __iter__(self):
-        for p in self.parameters:
-            yield p
-        
-    def get_parameter(self, key, shape=None):
-        p = self[key]
-        if shape is None:
-            return p
-        elif isinstance(shape, tuple):
-            return p.reshape(shape)
-        shape = shape.lower()
-        if shape == "square":
-            size = int(np.round(np.sqrt(len(p))))
-            if size*size == len(p):
-                return p.reshape((size,size))
-            else:
-                raise ValueError("Cannot return parameter as a square matrix, its length is {}".format(len(p)))
-        if shape == "upper triangular":
-            shape = "ut"
-        elif shape == "lower triangular":
-            shape = "lt"
-        if shape == "ut" or shape == "lt":
-            size =  int(np.floor(np.sqrt(2*len(p))))
-            if size * (size + 1) // 2 == len(p):
-                result = np.zeros((size, size), dtype=p.dtype)
-                if shape == "ut":
-                    idx = np.triu_indices(size)
-                else:
-                    idx = np.tril_indices(size)
-                result[idx] = p
-                return result
-            else:
-                raise ValueError("Cannot return parameter as a triangular matrix ({}), its length is {}".format(shape, len(p)))
-        else:
-            raise ValueError("Unknown shape "+shape)
-        
-    def set_parameter(self, key, value, shape=None):
-        if shape is None:
-            self[key] = value
-            return
-        if len(value.shape) != 2 or value.shape[0] != value.shape[1]:
-            raise ValueError("All supported shapes assume a square matrix")
-        shape = shape.lower()
-        if shape == "square":
-            self[key] = value  # Flattened in __setitem__
-        elif shape == "ut" or shape == "upper triangular":
-            idx = np.triu_indices(len(value))
-            self[key] = value[idx]
-        elif shape == "lt" or shape == "lower triangular":
-            idx = np.tril_indices(len(value))
-            self[key] = value[idx]
-
-
-def _get_openkim_model_string(verbose):
-    exename = "kim-api-collections-info"
-    args = ' portable_models'
-    sistername = 'kim-api-collections-management'
-
-    # First try if the program is on the path.
-    try:
-        modelstring = subprocess.check_output(exename+args, shell=True, stderr=subprocess.STDOUT).decode('utf-8')
-        return modelstring
-    except subprocess.CalledProcessError:
-        pass
-
-    # Then look for it using pkg-config
-    exepath = None
-    try:
-        prefix = subprocess.check_output("pkg-config libkim-api --variable=libexecdir", shell=True).decode('utf-8').strip()
-    except subprocess.CalledProcessError:
-        pass
-    else:
-        exepath = os.path.join(prefix, 'kim-api', exename)
-        if verbose:
-            print("Found using pkg-config:", exepath)
-
-    # Finally, try to look for where kim-api-collections-management and then check ../libexec
-    if not exepath and hasattr(shutil, 'which'):
-        management = shutil.which(sistername)
-        if management:
-            prefix = os.path.dirname(os.path.dirname(management))
-            exepath = os.path.join(prefix, 'libexec', 'kim-api', exename)
-            if verbose:
-                print("Found relative to", sistername, ":", exepath)
-    if not exepath:
-        raise RuntimeError("Cannot locate "+exename+" to generate list of KIM models.")
-
-    if not os.access(exepath, os.R_OK):
-        raise RuntimeError("Executable should be at "+exepath+" but is absent or not usable.")
-
-    try:
-        modelstring = subprocess.check_output(exepath+args, shell=True).decode('utf-8')
-        return modelstring
-    except subprocess.CalledProcessError:
-        raise RuntimeError("Running "+exepath+" failed.")
-
-
-def OpenKIMavailable(verbose=0):
-    """Get the list of installed OpenKIM models.
-
-    The list is obtained by locating and running the command line tool
-    kim-api-collections-info
-    """
-    modelstring = _get_openkim_model_string(verbose)
-    models = []
-    for line in modelstring.split('\n'):
-        if line:
-            models.append(line.split()[1])
-    return models
-
-
 if __name__ == '__main__':
     from ase.lattice.cubic import FaceCenteredCubic
     atoms = FaceCenteredCubic(size=(10,10,10), symbol='Cu')
     print("Creating calculator")
     pot = OpenKIMcalculator('EMT_Asap_Standard_AlAgAuCuNiPdPt__MO_118428466217_000')
     print("Setting atoms")
     atoms.set_calculator(pot)
```

### Comparing `asap3-3.13.1/Python/asap3/Internal/Subject.py` & `asap3-3.9.6/Python/asap3/Internal/Subject.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Internal/Threads.py` & `asap3-3.9.6/Python/asap3/Internal/Threads.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Internal/UtilityFunctions.py` & `asap3-3.9.6/Python/asap3/Internal/UtilityFunctions.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from __future__ import print_function
 
 __docformat__ = "restructuredtext en"
 
 
 from asap3.Internal.Builtins import _asap, get_version, get_short_version
 from asap3 import __file__ as _asapfile
-import numpy as np
 import ase
 import sys
 import os
 
 def print_version(level = 0):
     """Print the version number of the loaded version of Asap.
 
@@ -23,24 +22,17 @@
     """
     try:
         compiledfile = _asap.__file__
     except AttributeError:
         compiledfile = "<built-in>"
     print(get_version())
     if level >= 1:
-        pv = sys.version.split('\n')
-        print("  Python module: ", _asapfile)
-        print("  C++ module:    ", compiledfile)
-        print("  ase module:    ", ase.__file__)
-        print()
-        print("  Python version:", pv[0])
-        for pvline in pv[1:]:
-            print("                 ", pvline)
-        print("  numpy version: ", np.version.version)
-        print("  ase version:   ", ase.__version__)
+        print("  Python module:", _asapfile)
+        print("  C++ module:   ", compiledfile)
+        print("  ase module:   ", ase.__file__)
 
 def DebugOutput(filename, stdout=1, nomaster=False, sync=True):
     """Debugging output on each node goes to a different file.
 
     Redirect stderr to a different file on each node.  The filename should
     contain %d, which is replaced by the node number.  The file is opened
     with minimal buffering, and stderr (standard error) is redirected to
@@ -82,15 +74,15 @@
             vmpeak = int(words[1])
         elif words[0] == "VmData:":
             vmdata = int(words[1])
         elif words[0] == "VmRSS:":
             vmrss = int(words[1])
     print("Memory [proc %d '%s']: %d MB total (%d MB peak, %d MB data, %d MB rss)" % (
         asap3.mpi.world.rank, txt, (vmsize+512) / 1024,
-        (vmpeak+512) / 1024, (vmdata+512) / 1024, (vmrss+512)/1024)) #, file=sys.stderr)        
+        (vmpeak+512) / 1024, (vmdata+512) / 1024, (vmrss+512)/1024), file=sys.stderr)        
     procfile.close()
     if a is not None:
         memory_usage(a)
 
 def memory_usage(obj, total=True):
     """Print the memory usage of some kinds of objects.
```

### Comparing `asap3-3.13.1/Python/asap3/Internal/checkversion.py` & `asap3-3.9.6/Python/asap3/Internal/checkversion.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Base.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Base.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Basin.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Basin.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Metropolis.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Metropolis.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Base.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Base.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Data/fcc.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Data/fcc.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Data/symmetry.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Data/symmetry.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Moves/Surface.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Moves/Surface.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/MonteCarlo/Start.py` & `asap3-3.9.6/Python/asap3/MonteCarlo/Start.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/AsapFileToTrajectory.py` & `asap3-3.9.6/Python/asap3/Tools/AsapFileToTrajectory.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/AtomicEnergies.py` & `asap3-3.9.6/Python/asap3/Tools/AtomicEnergies.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/EMT_two_atom_test.py` & `asap3-3.9.6/Python/asap3/Tools/EMT_two_atom_test.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ElasticConstants.py` & `asap3-3.9.6/Python/asap3/Tools/ElasticConstants.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/MaterialProperties.py` & `asap3-3.9.6/Python/asap3/Tools/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/OptimizationDatabase.py` & `asap3-3.9.6/Python/asap3/Tools/OptimizationDatabase.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/EMT.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/EMT.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/GetParameters.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/GetParameters.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Optimization.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Optimization.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Performance.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Performance.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Quantities.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Quantities.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ase.io.trajectory import Trajectory
 from ase.data import reference_states, atomic_numbers, chemical_symbols
 from ase.units import kJ, GPa
 from ase.optimize import BFGS, QuasiNewton
 from ase.constraints import StrainFilter
 from ase.lattice.cubic import BodyCenteredCubic, FaceCenteredCubic
 from ase.lattice.hexagonal import HexagonalClosedPacked
-from ase.build import fcc100, fcc110, fcc111, hcp0001
+from ase.lattice.surface import fcc100, fcc110, fcc111, hcp0001
 from ase.lattice.compounds import B2, L1_2, L1_0
 from ase.lattice.spacegroup import crystal
 from ase.cluster.octahedron import Octahedron
 from ase.utils import basestring
 
 class QuantityCalc:
     properties = {'fcc_size': (1, 1, 1), # Size of the FCC and HCP unit cell
@@ -248,15 +248,14 @@
             print("Structure: %s" % (structure,))
             print("Elements: %s\n" % (elements,))
 
         e_full = self.get_value('energy', structure, elements,
                                  self.calc_lattice_constants)
 
         atoms = Atoms([elements[0]], [(0.0, 0.0, 0.0)])
-        atoms.center(vacuum=1.0)
         atoms.set_calculator(self.get_calc())
         e_reduced = atoms.get_potential_energy()
 
         e = e_reduced - e_full
 
         self.values[('cohesive_energy', structure, elements)] = e
 
@@ -659,23 +658,23 @@
             print(40 * "-" + "\n")
 
 
     def calc_stacking_fault(self, structure, elements):
         if structure != 'fcc':
             raise ValueError("Cannot calculate stacking fault energy of structure "+structure)
         a = self.latticeconstants[(structure, elements)]
-        atoms = fcc111(elements[0], (1,2,5), orthogonal=True, a=a, vacuum=a/(2 * np.sqrt(3.0)))
+        atoms = fcc111(elements[0], (1,2,5), orthogonal=True, a=a)
         atoms.set_pbc(True)
         atoms = atoms.repeat(self.properties['sf_repeat'])
         atoms.set_calculator(self.get_calc())
         dyn = QuasiNewton(atoms, logfile=None, trajectory=None)
         dyn.run(fmax=0.02)
         e_sf = atoms.get_potential_energy()
         n_sf = len(atoms)
-        atoms = fcc111(elements[0], (1,2,6), orthogonal=True, a=a, vacuum=a/(2 * np.sqrt(3.0)))
+        atoms = fcc111(elements[0], (1,2,6), orthogonal=True, a=a)
         atoms.set_pbc(True)
         atoms = atoms.repeat(self.properties['sf_repeat'])
         atoms.set_calculator(self.get_calc())
         dyn = QuasiNewton(atoms, logfile=None, trajectory=None)
         dyn.run(fmax=0.02)
         e_bulk = atoms.get_potential_energy()
         n_bulk = len(atoms)
@@ -779,15 +778,15 @@
                 n = l / 3 + 1
                 c = 3 - l % 3
             atoms = L1_2(symbol=elements, size=(8, 4, n),
                          #directions=[[1,-1,0],[1,0,-1],[1,1,1]], latticeconstant=a)
                          directions=[[1,-1,0],[1,1,-2],[1,1,1]], latticeconstant=a)
             atoms.set_pbc([True, True, False])
             # Wrap positions
-            scpos = atoms.get_scaled_positions(wrap=True)
+            scpos = atoms.get_scaled_positions()
             scpos[scpos > (1.0 - 1e-12)] = 0.0
             atoms.set_scaled_positions(scpos)
             # Remove layers
             if c > 0:
                 atoms = atoms[atoms.get_positions()[:,2] > (c - 0.5) * a / np.sqrt(3.0)]
             # Set vacuum
             atoms.center(axis=2, vacuum=10.0)
```

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/RGL.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/RGL.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Sampling.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Sampling.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/ScipyFmin.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/ScipyFmin.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/Search.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/Search.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/ParameterOptimization/SearchParallel.py` & `asap3-3.9.6/Python/asap3/Tools/ParameterOptimization/SearchParallel.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/SurfaceEnergies.py` & `asap3-3.9.6/Python/asap3/Tools/SurfaceEnergies.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/Timing.py` & `asap3-3.9.6/Python/asap3/Tools/Timing.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/Tools/niflheim.py` & `asap3-3.9.6/Python/asap3/Tools/niflheim.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/__init__.py` & `asap3-3.9.6/Python/asap3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,41 +96,33 @@
         MakeParallelAtoms
     from asap3.Internal.Collector import Collector
     from ase.parallel import paropen
 
 # OpenKIM may or may not be built into Asap
 from asap3.Internal.BuiltinPotentials import OpenKIMsupported
 if OpenKIMsupported:
-    from asap3.Internal.OpenKIMcalculator import OpenKIMcalculator, OpenKIMavailable
+    from asap3.Internal.OpenKIMcalculator import OpenKIMcalculator, OpenKIMinfo
 
 import ase
 from ase import Atoms
 from ase.visualize import view
 import ase.units as units
 # from ase.md.velocitydistribution import MaxwellBoltzmannDistribution, Stationary
 
-try:
-    from ase.calculators.calculator import PropertyNotImplementedError
-except ImportError:
-    # ASE version 3.12 or earlier.
-    class PropertyNotImplementedError(NotImplementedError):
-        pass
-
 NeighborList = _asap.NeighborList
 NeighborCellLocator = _asap.NeighborCellLocator
 FullNeighborList = _asap.FullNeighborList
 heap_mallinfo = _asap.heap_mallinfo
 
 # Check Asap installation for consistency
 check_version()
 
 # Check that a modern ASE is used in parallel simulations
 #
 # Due to a change in ASEs build system, older ASEs will not detect
 # that ASAP is running in parallel, and ase.parallel will not work.
 if parallelpossible:
-    import asap3.mpi
     import ase.parallel
+    import asap3.mpi
     if asap3.mpi.world.size != ase.parallel.world.size:
-        print(asap3.mpi.world.size, ase.parallel.world.size)
-        raise ImportError("Asap requires ASE version 3.22.0 or updated developer installation.")
+        raise ImportError("Asap requires ASE version 3.12 or updated developer installation.")
```

### Comparing `asap3-3.13.1/Python/asap3/analysis/averagepositions.py` & `asap3-3.9.6/Python/asap3/analysis/averagepositions.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/analysis/clusterposition.py` & `asap3-3.9.6/Python/asap3/analysis/clusterposition.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/analysis/localstructure.py` & `asap3-3.9.6/Python/asap3/analysis/localstructure.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 method MUST be overridden and augmented to call one of the get_xxx_cna
 methods, and use the returned information somehow.
 
 """
 
 import numpy as np
 from asap3 import _asap
-from asap3.mpi import world
 import ase.data
 from asap3.Internal.ListOfElements import ListOfElements
 from asap3.Internal.Subject import Subject
 
 def GuessLatticeConstant(atoms):
     """Gets an estimate of the lattice constant for a system.
 
@@ -49,45 +48,32 @@
     Note that this function is only intended for guessing a cutoff
     radius for e.g. CNA analysis, do not rely on this lattice constant
     being very meaningful.
 
     If any element does not have a lattice constant, a KeyError is raised.
     """
     refstate = ase.data.reference_states
-    loe = ListOfElements(atoms)
-    if len(loe) == 1:
-        if len(atoms):
-            z = atoms.get_atomic_numbers()
-            assert(z.min() == z.max())
-            # Cast to int is a numpy bug workaround: np.int32 objects are not ints
-            if refstate[int(z[0])]['symmetry'] == 'hcp':
-                latconst = refstate[int(z[0])]['a'] * np.sqrt(2)
-            else:
-                latconst = refstate[int(z[0])]['a']
+    z = atoms.get_atomic_numbers()
+    if z.min() == z.max():
+        # Cast to int is a numpy bug workaround: np.int32 objects are not ints
+        if refstate[int(z[0])]['symmetry'] == 'hcp':
+            return refstate[int(z[0])]['a'] * np.sqrt(2)
         else:
-            latconst = 0.0
-    else:
-        if len(atoms):
-            a = 0.0
-            n = 0
-            z = atoms.get_atomic_numbers()
-            for e in loe:
-                n1 = np.equal(z, e).sum() # Number of atoms with this element
-                if refstate[int(e)]['symmetry'] == 'hcp':
-                    a += n1 * refstate[int(e)]['a'] * np.sqrt(2)
-                else:
-                    a += n1 * refstate[int(e)]['a']
-                n += n1
-            latconst = a / n
+            return refstate[int(z[0])]['a']
+    a = 0.0
+    n = 0
+    for e in ListOfElements(atoms):
+        n1 = np.equal(z, e).sum() # Number of atoms with this element
+        if refstate[int(e)]['symmetry'] == 'hcp':
+            a += n1 * refstate[int(e)]['a'] * np.sqrt(2)
         else:
-            latconst = 0.0
-    if world.size > 1:
-        latconst = world.sum(latconst * len(atoms)) / atoms.get_global_number_of_atoms()
-    return latconst
-            
+            a += n1 * refstate[int(e)]['a']
+        n += n1
+    return a / n    
+
 def CNA(atoms, rCut=None):
     """Restricted Common Neighbor Analysis on a list of atoms.
 
     Returns an array of integers (int8) reflecting the local crystal structure.
     FCC is class 0, HCP is class 1 and everything else is class 2.
 
     It requires a value of rCut between the first and second shell.
```

### Comparing `asap3-3.13.1/Python/asap3/analysis/particle.py` & `asap3-3.9.6/Python/asap3/analysis/particle.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/analysis/ptm.py` & `asap3-3.9.6/Python/asap3/analysis/ptm.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from __future__ import print_function
 import asap3
 from asap3.Internal.Subject import Subject
 import numpy as np
-import sys
 
 def PTM(atoms, cutoff=10.0, rmsd_max=None, **kwargs):
     """Run Complex Hull Analysis on an Atoms object.
 
     Parameters:
     atoms: The atoms object
 
@@ -88,27 +87,15 @@
          
     'info': A tuple of two integers, the number of atoms analyzed by PTM
         and the number of atoms skipped due to insufficient neighbors.
 
     'nblist': (only if return_nblist is True) A neighbor list object.
 
     """
-    for argument in ('target_structures', 'return_mappings'):
-        if argument in kwargs:
-            # The C++ code only accepts tuples of bytes (str in Python 2),
-            # we need more flexibility.
-            structs = kwargs[argument]
-            if structs is None:
-                continue
-            if isinstance(structs, tuple):
-                structs = list(structs)  # Make mutable
-            for i, s in enumerate(structs):
-                if isinstance(s, str):
-                    structs[i] = s.encode()  # Convert to bytes
-            kwargs[argument] = tuple(structs)
+
     data = asap3._asap.PTM_allatoms(atoms, cutoff, **kwargs)
     if rmsd_max:
         data['structure'][data['rmsd'] > rmsd_max] = 0
     return data
 
 class PTMobserver(Subject):
     """Polyhedral Template Matching observer object.
@@ -171,15 +158,15 @@
         self.quantity = quantity
         if analyze_first:
             self.analyze()  # There will not be any observers yet.
         
     def analyze(self):
         "Runs the PTM analysis."
         self.data = PTM(self.atoms, cutoff=self.cutoff, rmsd_max=self.rmsd_max, 
-                        target_structures=self.target_structures,
+                        structures=self.target_structures,
                         calculate_strains=self.strains,
                         quick=self.quick)
         if self.quantity:
             self.atoms.set_tags(self.data[self.quantity])
         self.call_observers()
         
     update = analyze
@@ -229,34 +216,22 @@
     #   by the PTM code, so all indices must be one less than the number above.
     hcp_inplane = np.array((7, 8, 9, 10, 12, 11)) - 1
     hcp_above = np.array((5, 3, 1)) - 1
     hcp_below = np.array((6, 4, 2)) - 1
     def analyze(self):
         "Runs the PTM analysis."
         self.data = PTM(self.atoms, cutoff=self.cutoff, rmsd_max=self.rmsd_max, 
-                        target_structures=self.target_structures,
+                        structures=self.target_structures,
                         calculate_strains=self.strains,
                         quick=self.quick, return_mappings=('hcp',))
         new_s = self.data['structure']
         s = np.array(new_s)  # A copy so we can change the original.
         mappings = self.data['mappings']
         hcpatoms = (s == 2).nonzero()[0]
-        if getattr(self.atoms, "parallel", False):
-            # Parallel simulation - we need to communicate the structures
-            nghosts = len(self.atoms.ghosts['positions'])
-            label = '_ptm_disloc_analysis_internal'
-            self.atoms.arrays[label] = s
-            self.atoms.ghosts[label] = np.zeros(nghosts, dtype=s.dtype)
-            del s # Suppress a warning from asap - no extra references are allowed
-            self.atoms.get_calculator().update_ghost_data(self.atoms)
-            s = self.atoms.arrays[label]  # Restore s - same as before.
-            ghost_structs = self.atoms.ghosts[label]
-            del self.atoms.ghosts[label]
-            del self.atoms.arrays[label]
-            s = np.concatenate((s, ghost_structs))
+        assert(len(mappings) == len(hcpatoms))
         for i in hcpatoms:
             mapping = mappings[i]
             nhcp = 0
             nfcc = 0
             nbsum = np.zeros(3)
             # Atom types of the neighbors
             inplane = s[mapping[self.hcp_inplane]] == 2
@@ -267,15 +242,15 @@
             belowsum = below.sum()
             fccsum = (s[mapping] == 1).sum()
             # Heuristic for finding typical structures of HCP atoms
             if inplanesum == 6 and abovesum == 0 and belowsum == 0:
                 # A single basal plane of HCP atoms: Twin boundary
                 new_s[i] = 6
             elif inplanesum == 6 and ((abovesum == 3 and belowsum == 0) or
-                                      (abovesum == 0 and belowsum == 3)):
+                                      (abovesum == 0 and belowsum == 6)):
                 # Looks like two parallel planes of HCP atoms: Stacking fault.
                 new_s[i] = 7
             elif (3 <= inplanesum <= 5
                   and inplanesum + abovesum + belowsum + fccsum >= 11
                   and (bool(abovesum) ^ bool(belowsum))):
                 # A partial basal plane, with a possibly partial plane either
                 # above or below, but not both. At most one non-HCP/FCC atom.
@@ -285,11 +260,10 @@
                 # there are only two boundaries between HCP and non-HCP atoms
                 rolled = np.roll(inplane, 1)
                 if np.logical_xor(inplane, rolled).sum() == 2:
                     new_s[i] = 8
         # Kill the mappings dictionary to save memory
         del mappings, self.data['mappings']
         self.atoms.set_tags(new_s)
-        self.atoms.set_array("rmsd", self.data['rmsd'])
         self.call_observers()
         
     update = analyze
```

### Comparing `asap3-3.13.1/Python/asap3/analysis/rdf.py` & `asap3-3.9.6/Python/asap3/analysis/rdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,22 +38,17 @@
         be calculated and averaged before any observer of this object
         is notified and/or the RDF is saved to a file.
 
         autoclear (optional, default=False): Should the RDF be cleared
         after the RDF has been processed by observers and/or written
         to a file?  The default is to continue to accumulate data.
         """
-
-        if not hasattr(atoms, "get_global_number_of_atoms"):
-            # ASE 3.18.0 (and older) compatibility)
-            atoms.get_global_number_of_atoms = atoms.get_number_of_atoms
-
         Subject.__init__(self)
         self.atoms = atoms
-        self.natoms = atoms.get_global_number_of_atoms()
+        self.natoms = atoms.get_number_of_atoms()
         self.globalrdf = None
         self.rMax = rMax * 1.0  # Guard against integer divisions.
         self.nBins = nBins
         self.dr = self.rMax / nBins
         self.interval = interval
         self.average = average
         self.autoclear = autoclear
@@ -106,15 +101,15 @@
                     self.save()
                 self.n2 = 0
 
     def do_rdf(self):
         """Do the actual RDF calculation.  Do not call directly."""
         if self.verbose:
             print("Calculating RDF", file=sys.stderr)
-        assert self.natoms == self.atoms.get_global_number_of_atoms()
+        assert self.natoms == self.atoms.get_number_of_atoms()
         
         # Check if we need to replace the atoms with a copy.
         atoms = self.atoms
         if world.size > 1:
             try:
                 calc = atoms.get_calculator()
             except AttributeError:
```

### Comparing `asap3-3.13.1/Python/asap3/fixepydoc.py` & `asap3-3.9.6/Python/asap3/fixepydoc.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/io/ReadOldFiles.py` & `asap3-3.9.6/Python/asap3/io/ReadOldFiles.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/io/cpu_setup.py` & `asap3-3.9.6/Python/asap3/io/cpu_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,9 +50,9 @@
     [len0, len1, len2] = [float(e) for e in dim]
 
     cubes = [(len0 / a, len1 / b, len2 / c) for (a, b, c) in factorizations]
     ratios = [(x*y*z) / (2*x*y + 2*y*z + 2*z*x) for (x, y, z) in cubes]
 
     best_fac = max([(e, bf) for e, bf in zip(ratios, factorizations)])[1]
     cpus = [e[1] for e in sorted(zip(order, best_fac))]
-    return np.array(cpus).astype(int)
+    return np.array(cpus)
```

### Comparing `asap3-3.13.1/Python/asap3/io/trajectory.py` & `asap3-3.9.6/Python/asap3/io/trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 
             if self.master:
                 num_cores = ase.parallel.world.size
                 print("num cpus:", num_cores)
                 print("cell:", np.diag(atoms.cell).tolist())
                 cpus = cpu_setup.calculate_optimal_cpu_setup(num_cores, np.diag(atoms.cell).tolist())
                 print("cpu setup:", cpus)
-            else:
-                cpus = np.zeros(3, int)
 
             cpus = ase.parallel.broadcast(cpus, 0)
             return asap3.MakeParallelAtoms(atoms, cpus)
         else:
             return asap3.MakeParallelAtoms(atoms, cpus)
 
 
@@ -163,15 +161,15 @@
         if master is not None:
             if atoms.get_comm().rank != 0:
                 raise NotImplementedError("It is required that the cpu with rank 0 is the master")
         else:
             if atoms and hasattr(atoms, 'get_comm'):
                 rank = atoms.get_comm().rank
             else:
-                rank = ase.parallel.world.rank
+                rank = ase.parallel.rank
             master = (rank == 0)
         if atoms is not None and getattr(atoms, "parallel", False):
             atoms = asap3.Collector(atoms, master, self.allow_forces)        
         trajectory.TrajectoryWriter.__init__(self, filename, mode=mode, atoms=atoms, 
                                        properties=properties, extra=extra, master=master)
        
     def write(self, atoms=None, **kwargs):
```

### Comparing `asap3-3.13.1/Python/asap3/md/langevin.py` & `asap3-3.9.6/Python/asap3/md/langevin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,109 @@
 """Langevin dynamics class."""
 
 import numpy as np
 from numpy.random import standard_normal, randint
 import asap3
 import ase
-import ase.units
 from asap3.md.md import ParallelMolDynMixin
 from ase.md.md import MolecularDynamics
 from ase.md.langevin import Langevin as Langevin_ASE
 import asap3.constraints
 import sys
 
-class ASE_Langevin_v3_or_4(Langevin_ASE, ParallelMolDynMixin, object):
-    def __init__(self, atoms, timestep, temperature=None, friction=None, fixcm=True,
-                     *, temperature_K=None, **kwargs):
+class ASE_Langevin_v2(Langevin_ASE, ParallelMolDynMixin, object):
+    def __init__(self, atoms, timestep, temperature, friction, fixcm=True,
+                 trajectory=None, logfile=None, loginterval=1):
+        assert(getattr(Langevin_ASE, "_lgv_version", 1) == 2)
         ParallelMolDynMixin.__init__(self, "Langevin", atoms)
-        if Langevin_ASE._lgv_version == 3:
-            if temperature_K is not None:
-                assert temperature is None
-                temperature = ase.units.kB * temperature_K
-            Langevin_ASE.__init__(self, atoms, timestep, temperature=temperature,
-                                  friction=friction, fixcm=fixcm,
-                                  communicator=None, **kwargs)
-        else:
-            assert Langevin_ASE._lgv_version in (4, 5)
-            Langevin_ASE.__init__(self, atoms, timestep, temperature=temperature,
-                                  friction=friction, temperature_K=temperature_K,
-                                  fixcm=fixcm, communicator=None, **kwargs)
+        Langevin_ASE.__init__(self, atoms, timestep, temperature, friction, fixcm,
+                              trajectory, logfile, loginterval, communicator=None)
+        
+    sdpos = property(lambda s: s.get("sdpos"), lambda s, x: s.set("sdpos", x))
+    sdmom = property(lambda s: s.get("sdmom"), lambda s, x: s.set("sdmom", x))
+    c1 = property(lambda s: s.get("c1"), lambda s, x: s.set("c1", x))
+    c2 = property(lambda s: s.get("c2"), lambda s, x: s.set("c2", x))
+    act0 = property(lambda s: s.get("act0"), lambda s, x: s.set("act0", x))
+    c3 = property(lambda s: s.get("c3"), lambda s, x: s.set("c3", x))
+    c4 = property(lambda s: s.get("c4"), lambda s, x: s.set("c4", x))
+    pmcor = property(lambda s: s.get("pmcor"), lambda s, x: s.set("pmcor", x))
+    cnst = property(lambda s: s.get("cnst"), lambda s, x: s.set("cnst", x))
+    masses = property(lambda s: s.get("masses"), lambda s, x: s.set("masses", x))
 
-    def run(self, steps):
-        self.before_run()
-        super().run(steps)
-        self.after_run()
+class ASE_Langevin_v3(Langevin_ASE, ParallelMolDynMixin, object):
+    def __init__(self, atoms, timestep, temperature, friction, fixcm=True,
+                 trajectory=None, logfile=None, loginterval=1):
+        assert(getattr(Langevin_ASE, "_lgv_version", 1) == 3)
+        ParallelMolDynMixin.__init__(self, "Langevin", atoms)
+        Langevin_ASE.__init__(self, atoms, timestep, temperature, friction, fixcm,
+                              trajectory, logfile, loginterval, communicator=None)
 
-    def _get_com_velocity(self, velocity=None):
+    def _get_com_velocity(self):
         """Return the center of mass velocity."""
-        if velocity is None:
-            velocity = self.v  # Compatibility with older ASE
         if getattr(self.atoms, "parallel", False):
             data = np.zeros(4)
-            data[:3] = np.dot(self.masses.flatten(), velocity)
+            data[:3] = np.dot(self.masses.flatten(), self.v)
             data[3] = self.masses.sum()
             self.atoms.comm.sum(data)
             return data[:3] / data[3]
         else:
-            return np.dot(self.masses.flatten(), velocity) / self.masses.sum()
+            return np.dot(self.masses.flatten(), self.v) / self.masses.sum()
 
     temp = property(lambda s: s.get("temp"), lambda s, x: s.set("temp", x))
     fr = property(lambda s: s.get("fr"), lambda s, x: s.set("fr", x))
     masses = property(lambda s: s.get("masses"), lambda s, x: s.set("masses", x))
     c1 = property(lambda s: s.get("c1"), lambda s, x: s.set("c1", x))
     c2 = property(lambda s: s.get("c2"), lambda s, x: s.set("c2", x))
     c3 = property(lambda s: s.get("c3"), lambda s, x: s.set("c3", x))
     c4 = property(lambda s: s.get("c4"), lambda s, x: s.set("c4", x))
     c5 = property(lambda s: s.get("c5"), lambda s, x: s.set("c5", x))
     v = property(lambda s: s.get("v"), lambda s, x: s.set("v", x))
-    # Depending on the ASE version, either xi and eta will exist, or rnd_vel and rnd_pos
     xi = property(lambda s: s.get("xi"), lambda s, x: s.set("xi", x))
     eta = property(lambda s: s.get("eta"), lambda s, x: s.set("eta", x))
-    rnd_pos = property(lambda s: s.get("rnd_pos"), lambda s, x: s.set("rnd_pos", x))
-    rnd_vel = property(lambda s: s.get("rnd_vel"), lambda s, x: s.set("rnd_vel", x))
 
 class Langevin_Fast(MolecularDynamics, ParallelMolDynMixin, object):
-    def __init__(self, atoms, timestep, temperature=None, friction=None, fixcm=True,
-                     *, temperature_K=None, 
-                     trajectory=None, logfile=None, loginterval=1, seed=None):
-        if Langevin_ASE._lgv_version == 3:
-            # Simplified logic
-            if temperature_K is not None:
-                temperature = temperature_K * ase.units.kB
-        else:
-            assert Langevin_ASE._lgv_version >= 4
-            temperature = ase.units.kB * self._process_temperature(temperature, temperature_K, 'eV')
+    def __init__(self, atoms, timestep, temperature, friction, fixcm=True,
+                 trajectory=None, logfile=None, loginterval=1):
+        assert(getattr(Langevin_ASE, "_lgv_version", 1) >= 2)
         ParallelMolDynMixin.__init__(self, "Langevin", atoms)
         self._uselocaldata = False # Need to store on atoms for serial simul too.
-        self.calculator = atoms.get_calculator()
+        self.calculator = atoms.get_calculator()            
+        self.asap_md = asap3._asap.Langevin(atoms, self.calculator, timestep,
+                                            self.prefix+"sdpos", self.prefix+"sdmom",
+                                            self.prefix+"c1", self.prefix+"c2",
+                                            fixcm, randint(1 << 30))
         if not atoms.has('momenta'):
             atoms.set_momenta(np.zeros((len(atoms), 3), float))
-        self.atoms_have_constraints = len(atoms.constraints)
-        if self.atoms_have_constraints:
-            if len(atoms.constraints) != 1:
-                raise RuntimeError("ASAP Langevin dynamics only support a single constraint.")
+        if atoms.constraints:
+            assert len(atoms.constraints) == 1
             constraint = atoms.constraints[0]
-            if not isinstance(constraint, asap3.constraints.FixAtoms):
-                raise RuntimeError("ASAP Langevin dynamics only support the ASAP FixAtoms constraint.")
+            assert isinstance(constraint, asap3.constraints.FixAtoms)
+            constraint.prepare_for_asap(atoms)            
             # Make all constants arrays by making friction an array
-            friction = friction * np.ones(len(atoms))
-            fixcm = False   # Unneccesary (and incompatible) when FixAtoms constraint used.
-        if seed is None:
-            seed = randint(1 << 30)
-        assert isinstance(seed, int), "seed must be an int"
-        self.asap_md = asap3._asap.Langevin(atoms, self.calculator, timestep,
-                                            self.prefix+"sdpos", self.prefix+"sdmom",
-                                            self.prefix+"c1", self.prefix+"c2",
-                                            fixcm, seed)
+            friction = friction * np.zeros(len(atoms))
         MolecularDynamics.__init__(self, atoms, timestep, trajectory,
                                    logfile, loginterval)
         self.temp = temperature
         self.frict = friction
         self.fixcm = fixcm  # will the center of mass be held fixed?
         self.communicator = None
         self.updatevars()
 
-    def set_temperature(self, temperature=None, *, temperature_K=None):
-        self.temp =  ase.units.kB * self._process_temperature(temperature, temperature_K, 'eV')
+    def set_temperature(self, temperature):
+        self.temp = temperature
         self.updatevars()
 
     def set_friction(self, friction):
         self.frict = friction
         self.updatevars()
 
     def set_timestep(self, timestep):
         self.dt = timestep
         self.updatevars()
-
+        
     def updatevars(self):
         dt = self.dt
         # If the friction is an array some other constants must be arrays too.
         self._localfrict = hasattr(self.frict, 'shape')
         lt = self.frict * dt
         masses = self.masses
         sdpos = dt * np.sqrt(self.temp / masses.reshape(-1) *
@@ -151,67 +137,67 @@
         self.c2 = c2
         self.act0 = act0
         self.c3 = c3
         self.c4 = c4
         self.pmcor = pmcor
         self.cnst = cnst
         # Also works in parallel Asap:
-        self.natoms = self.atoms.get_global_number_of_atoms() #GLOBAL number of atoms
+        self.natoms = self.atoms.get_number_of_atoms() #GLOBAL number of atoms
         if len(self.atoms.constraints) == 1:
             # Process the FixAtoms constraint
             constr = self.atoms.constraints[0].index
             self.sdpos[constr] = 0.0
             self.sdmom[constr] = 0.0
             self.c1[constr] = 0.0
             self.c2[constr] = 0.0
             self.c3[constr] = 0.0
             self.c4[constr] = 0.0
             self.act0[constr] = 0.0
         if self._localfrict:
-            self.asap_md.set_vector_constants(self.prefix+"act0", self.prefix+"c3",
-                                              self.prefix+"c4", self.prefix+"pmcor",
+            self.asap_md.set_vector_constants(self.prefix+"act0", self.prefix+"c3", 
+                                              self.prefix+"c4", self.prefix+"pmcor", 
                                               self.prefix+"cnst")
         else:
             self.asap_md.set_scalar_constants(self.act0, self.c3, self.c4,
                                               self.pmcor, self.cnst)
-
+            
     def run(self, steps):
         assert(self.calculator is self.atoms.get_calculator())
-        if self.atoms.constraints or self.atoms_have_constraints:
-            # Constraints may have been added, removed or changed
-            self.updatevars()
-        self.before_run()
         self.asap_md.run(steps, self.observers, self)
-        self.after_run()
-        self.atoms_have_constraints = len(self.atoms.constraints)
-
+        
     def get_random(self, gaussian):
         return self.asap_md.get_random(gaussian)
-
+    
     # Properties are not inherited, need to repeat them
     sdpos = property(lambda s: s.get("sdpos"), lambda s, x: s.set("sdpos", x))
     sdmom = property(lambda s: s.get("sdmom"), lambda s, x: s.set("sdmom", x))
     c1 = property(lambda s: s.get("c1"), lambda s, x: s.set("c1", x))
     c2 = property(lambda s: s.get("c2"), lambda s, x: s.set("c2", x))
     act0 = property(lambda s: s.get("act0"), lambda s, x: s.set("act0", x))
     c3 = property(lambda s: s.get("c3"), lambda s, x: s.set("c3", x))
     c4 = property(lambda s: s.get("c4"), lambda s, x: s.set("c4", x))
     pmcor = property(lambda s: s.get("pmcor"), lambda s, x: s.set("pmcor", x))
     cnst = property(lambda s: s.get("cnst"), lambda s, x: s.set("cnst", x))
     masses = property(lambda s: s.get("masses"), lambda s, x: s.set("masses", x))
-    frict = property(lambda s: s.get("frict"), lambda s, x: s.set("frict", x))
+
 
 def Langevin(atoms, *args, **kwargs):
-    if (isinstance(atoms, ase.Atoms)
+    if (isinstance(atoms, ase.Atoms) 
         and asap3.constraints.check_asap_constraints(atoms)
-        and not kwargs.pop('forceASE', False)
        ):
-        # Nothing prevents Asap optimization
+        # ASE Langevin is version 2 and nothing prevents Asap optimization
         sys.stderr.write("Using Asap-optimized C++-Langevin algorithm\n")
         return Langevin_Fast(atoms, *args, **kwargs)
-    elif Langevin_ASE._lgv_version in (3, 4, 5):
+    elif Langevin_ASE._lgv_version == 2:
+        # ASE Langevin is version 2
+        sys.stderr.write("Using ASE-based Langevin algorithm version 2\n")
+        return ASE_Langevin_v2(atoms, *args, **kwargs)
+    elif Langevin_ASE._lgv_version == 3:
         # ASE Langevin is version 3
-        sys.stderr.write("Using ASE-based Langevin algorithm\n")
-        return ASE_Langevin_v3_or_4(atoms, *args, **kwargs)
+        sys.stderr.write("Using ASE-based Langevin algorithm version 3\n")
+        return ASE_Langevin_v3(atoms, *args, **kwargs)
     else:
         raise RuntimeError(
             "The Langevin dynamics in ASE has unsupported version {0}.".format(Langevin_ASE._lgv_version))
+    
+
+
```

### Comparing `asap3-3.13.1/Python/asap3/md/verlet.py` & `asap3-3.9.6/Python/asap3/md/verlet_fast.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,45 @@
 '''
 Created on Mar 16, 2011
 
 @author: schiotz
 '''
 
 from ase.md.md import MolecularDynamics
-from ase.md.verlet import VelocityVerlet as _VelocityVerlet
-from asap3.md.md import ParallelMolDynMixinNoData
+from ase.md.verlet import VelocityVerlet as VelocityVerlet_ASE
 import ase
 import asap3
 import numpy as np
 import sys
 
-class VelocityVerlet_Asap(MolecularDynamics, ParallelMolDynMixinNoData):
-    def __init__(self, atoms, timestep, trajectory=None, logfile=None,
+class VelocityVerlet_Asap(MolecularDynamics):
+    def __init__(self, atoms, dt, trajectory=None, logfile=None,
                  loginterval=1):
-        MolecularDynamics.__init__(self, atoms, timestep, trajectory, logfile,
+        MolecularDynamics.__init__(self, atoms, dt, trajectory, logfile,
                                    loginterval)
         if not atoms.has('momenta'):
             atoms.set_momenta(np.zeros((len(atoms), 3), float))
         self.calculator = atoms.get_calculator()
-        self.asap_md = asap3._asap.VelocityVerlet(atoms, self.calculator, timestep)
-            
-    def run(self, steps):
-        assert(self.calculator is self.atoms.get_calculator())
-        self.before_run()
-        # Extra stuff needs to be done for FixAtoms constraint.
-        if self.atoms.constraints:
-            if len(self.atoms.constraints) != 1:
-                raise RuntimeError("AASAP Verlet can only do parallel dynamics with a single constraint.")
-            constraint = self.atoms.constraints[0]
-            if not  isinstance(constraint, asap3.constraints.FixAtoms):
-                raise RuntimeError("ASAP Verlet only supports constrained dynamics with the ASAP FixAtoms constraint.")
+        self.asap_md = asap3._asap.VelocityVerlet(atoms, self.calculator, dt)
+        # Identify FixAtoms constraint
+        if atoms.constraints:
+            assert len(atoms.constraints) == 1
+            constraint = atoms.constraints[0]
+            assert isinstance(constraint, asap3.constraints.FixAtoms)
+            constraint.prepare_for_asap(atoms)
             mask = constraint.index
-            if not mask.dtype == bool:
-                mask2 = np.zeros(len(self.atoms), bool)
-                mask2[mask] = True
-                mask = mask2
-            assert mask.shape == (len(self.atoms),) and mask.dtype == bool
+            assert mask.shape == (len(atoms),) and mask.dtype == bool
             mult = np.logical_not(mask).astype(float)
             self.atoms.arrays["FixAtoms_mult_double"] = mult
-            del mask, mult
-        self.asap_md.run(steps, self.observers, self)
-        self.after_run()
-        if self.atoms.constraints:
-            del self.atoms.arrays["FixAtoms_mult_double"]
-
-class VelocityVerlet_ASE(_VelocityVerlet, ParallelMolDynMixinNoData):
+            
     def run(self, steps):
-        self.before_run()
-        super().run(steps)
-        self.after_run()
+        assert(self.calculator is self.atoms.get_calculator())
+        self.asap_md.run(steps, self.observers, self)
         
-def VelocityVerlet(atoms, timestep, trajectory=None, logfile=None, loginterval=1):
+def VelocityVerlet(atoms, dt, trajectory=None, logfile=None, loginterval=1):
     if isinstance(atoms, ase.Atoms) and asap3.constraints.check_asap_constraints(atoms):
         sys.stderr.write("Using Asap-optimized Verlet algorithm\n")
-        return VelocityVerlet_Asap(atoms, timestep, trajectory, logfile, loginterval)
+        return VelocityVerlet_Asap(atoms, dt, trajectory, logfile, loginterval)
     else:
         sys.stderr.write("Using ASE Verlet algorithm\n")
-        return VelocityVerlet_ASE(atoms, timestep, trajectory, logfile, loginterval)
+        return VelocityVerlet_ASE(atoms, dt, trajectory, logfile, loginterval)
```

### Comparing `asap3-3.13.1/Python/asap3/mpi.py` & `asap3-3.9.6/Python/asap3/mpi.py`

 * *Files 20% similar despite different names*

```diff
@@ -76,15 +76,20 @@
                 return None
             else:
                 # Oops, this will be the original _asap.Communicator class.
                 return comm
 
         def broadcast_string(self, string, root):
             if rank == root:
-                assert isinstance(string, bytes)
+                if sys.version_info[0] == 2:
+                    # Python 2 
+                    assert isinstance(string, str)
+                else:
+                    # Python 3
+                    assert isinstance(string, bytes)
                 n = npy.array(len(string), int)
             else:
                 n = npy.zeros(1, int)
             self.broadcast(n, root)
             if rank == root:
                 string = npy.fromstring(string, npy.int8)
             else:
@@ -95,14 +100,29 @@
     world = _Communicator()
 else:
     world = SerialCommunicator()
 
 size = world.size
 rank = world.rank
 parallel = (size > 1)
+    
+def broadcast_string(string=None, root=MASTER, comm=world):
+    if rank == root:
+        assert isinstance(string, str)
+        n = npy.array(len(string), int)
+    else:
+        assert string is None
+        n = npy.zeros(1, int)
+    comm.broadcast(n, root)
+    if rank == root:
+        string = npy.fromstring(string, npy.int8)
+    else:
+        string = npy.zeros(n, npy.int8)
+    comm.broadcast(string, root)
+    return string.tostring()
 
 
 def all_gather_array(comm, a): #???
     # Gather array into flat array
     shape = (comm.size,) + npy.shape(a)
     all = npy.zeros(shape)
     comm.all_gather(a, all)
```

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/AdsCalc.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/AdsCalc.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/Logger.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/Logger.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/atommontecarlodata.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/atommontecarlodata.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/cluster.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/cluster.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/clusteratom.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/clusteratom.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/data/au.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/data/au.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/data/fcc.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/data/fcc.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/data/symmetry.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/data/symmetry.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/langmuirExpression.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/langmuirExpression.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/mc_result.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/mc_result.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/montecarlo/atom.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/montecarlo/atom.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/montecarlo/surface.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/montecarlo/surface.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/nanoparticle_mc/resizecluster.py` & `asap3-3.9.6/Python/asap3/nanoparticle_mc/resizecluster.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/optimize/fire.py` & `asap3-3.9.6/Python/asap3/optimize/fire.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 
     def read(self):
         if world.size > 1:
             raise NotImplementedError("Restarting is not implemented for FIRE in parallel mode (ASAP).")
         v, self.dt = self.load()
         self.atoms.set_array(self.vtag, v)
        
-    def step(self,f=None):
+    def step(self,f):
         atoms = self.atoms
-        if f is None:
-            f = atoms.get_forces()
         if not atoms.has(self.vtag):
             v = np.zeros((len(atoms), 3))
         else:
             v = atoms.get_array(self.vtag)
             vf = np.vdot(f, v)
             if world.size > 1:
                 vf = world.sum(vf)
@@ -47,20 +45,16 @@
 
         v += self.dt * f
         dr = self.dt * v
         drdr = np.vdot(dr, dr)
         if world.size > 1:
             drdr = world.sum(drdr)
         normdr = np.sqrt(drdr)
-        try:
-            maxstep = self.maxstep
-        except AttributeError:
-            maxstep = self.maxmove
-        if normdr > maxstep:
-            dr = maxstep * dr / normdr
+        if normdr > self.maxmove:
+            dr = self.maxmove * dr / normdr
         r = atoms.get_positions()
         atoms.set_positions(r + dr)
         atoms.set_array(self.vtag, v)
         self.dump((v, self.dt))
         
     def dump(self, data):
         # Can only restart in serial mode
```

### Comparing `asap3-3.13.1/Python/asap3/optimize/mdmin.py` & `asap3-3.9.6/Python/asap3/optimize/mdmin.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,17 @@
     def initialize(self):
         self.dt = 0.1
 
     def read(self):
         v, self.dt = self.load()
         atoms.set_velocities(v)
         
-    def step(self, f=None):
+    def step(self, f):
         atoms = self.atoms
-        if f is None:
-            f = atoms.get_forces()
-            
+
         v = atoms.get_velocities()
         if v is None:
             v = npy.zeros((len(atoms), 3))
         else:
             v += 0.5 * self.dt * f
             # Correct velocities:
             vf = npy.vdot(v, f)
```

### Comparing `asap3-3.13.1/Python/asap3/optimize/optimize.py` & `asap3-3.9.6/Python/asap3/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/setup/VelocityDistribution.py` & `asap3-3.9.6/Python/asap3/setup/VelocityDistribution.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/setup/dislocation.py` & `asap3-3.9.6/Python/asap3/setup/dislocation.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 The main function is `Dislocation`, it returns the displacement field
 (see `Asap.Setup.DisplacementField`) of a dislocation.  The displacement
 field is constructed as the sum of the fields of the edge and screw
 components, except if one of the components is zero, in which case it
 is omitted.  The displacement field can be applied to a lattice.
 """
-
 from __future__ import print_function
+
+__docformat__ = "restructuredtext en"
+
+
 from numpy import *
 import numbers
 from asap3.setup.displacementfield import DisplacementField
 
-__docformat__ = "restructuredtext en"
-
 def magn(v):
     """The magnitude of a vector."""
     return sqrt(dot(v, v))
 
-def Dislocation(origin, line, Burgers, PoissonRatio=None,
-                glideplane=None, debug=None):
+def Dislocation(origin, line, Burgers, PoissonRatio=None, debug=None):
     """Set up a dislocation with mixed screw and edge character.
 
     In the following description, a 3-vector may be a tuple, list or
     numeric array with three elements.
     
     This function will set up a straight dislocation through a
     specified point with a given Burgers vector.  The first argument
@@ -35,55 +35,46 @@
     and the second argument ('line', a 3-vector) gives the dislocation
     line (only the direction of the vector matters). The third
     parameter ('Burgers', a 3-vector) specifies the Burgers vector of
     the dislocation.  Finally, the fourth argument is an optional
     parameter which specifies Poisson's ratio of the material.  The
     default value is 1/3.
     
-    Returns a `setup.displacementfield.DisplacementField` object.
+    Returns a `Setup.DisplacementField.DisplacementField` object.
     Displacement fields may be added together (and multiplied by
-    scalars).  The dislplacement field can be applied to any 
-    Atoms object using field.`apply_to(atoms)`.  The Atoms are 
-    modified using the get_positions() and Set_positions() methods.
+    scalars).  The dislplacement field can be applied to any list of
+    atoms using field.`apply_to(listofatoms)`.  The list of atoms is
+    modified using its GetCartesianPositions() and
+    SetCartesianPositions() methods.
 
     Example:
 
-        from asap3 import *
-        from ase.lattice.cubic import FaceCenteredCubic
-        from asap3.detup.dislocation import Dislocation
-
-        splitting = 5
-        size = (30, 25, 7)
-        Gold = "Au"
-
-        slab = FaceCenteredCubic(directions=((1,1,-2), (-1,1,0), (1,1,1)),
-                                 size=size, symbol=Gold, pbc=False)
-        basis = slab.get_cell()
-        # Center of system, slight offset to not hit an atom.
-        center = 0.5 * array([basis[0,0], basis[1,1], basis[2,2]]) + array([0.1, 0.1, 0.1])
-        offset = 0.5 * splitting * slab.miller_to_direction((-1,0,1))
-
-        d1 = Dislocation(center - offset, slab.miller_to_direction((-1,-1,0)),
-                         slab.miller_to_direction((-2,-1,1))/6.0)
-        d2 = Dislocation(center + offset, slab.miller_to_direction((1,1,0)),
-                         slab.miller_to_direction((1,2,1))/6.0)
-        atoms = Atoms(slab)
-        (d1+d2).apply_to(atoms)
+         from Setup.Lattice.FCC111Ortho import FCC111Ortho
+         from Structures.ChemicalElements import *
+         from Numeric import *
+         from Asap.Setup.Dislocation import Dislocation
+         lat = FCC111Ortho((12,12,12), Copper, 6.78)
+         center = matrixmultiply(lat.GetCoordinateBasis(), (0.5, 0.5, 0.5)) 
+         line = lat.MillerToDirection((0,0.2,1))
+         Burgers = lat.MillerToDirection((0.5,0.5,0))
+         disloc = Dislocation(center, line, Burgers)
+         disloc.apply_to(lat)
+         plot = lat.GetPlot()         
+
     """
 
     line = array(line) / magn(line)
     Burgers = array(Burgers)
     screw_b = dot(Burgers, line)
     edge_b = Burgers - screw_b * line
-    small = 1e-6
-    
-    if abs(screw_b) < small:
+
+    if screw_b == 0.0:
         result = EdgeDislocation(origin, line, edge_b, PoissonRatio,
                                  debug=debug)
-    elif magn(edge_b) < small:
+    elif magn(edge_b) == 0.0:
         result = ScrewDislocation(origin, line, screw_b, debug=debug)
     else:
         result = (EdgeDislocation(origin, line, edge_b, PoissonRatio,
                                   debug=debug) +
                   ScrewDislocation(origin, line, screw_b, cut=edge_b,
                                    debug=debug))
     return result
@@ -102,19 +93,32 @@
     vector matters).  The third ('b', a scalar) gives the Burgers
     vector (positive means parallel to the dislocation line, negative
     means antiparallel).  The third optional argument (cut, a 3-tuple)
     gives a direction that lies in the cutting plane when starting in
     the origin.  If not given, (1.0, 0.0, 0.0) is used unless parallel
     to the dislocation line, in which case (0.0, 1.0, 0.0) is used.
 
-    Returns a `setup.displacementfield.DisplacementField` object.
-    Displacement fields may be added together (and multiplied by
-    scalars).  The dislplacement field can be applied to any 
-    Atoms object using field.`apply_to(atoms)`.  The Atoms are 
-    modified using the get_positions() and Set_positions() methods.
+    Returns a Setup.DisplacementField.DisplacementField object.
+    Dislplacement fields may be added together (and multiplied by
+    scalars).  The dislplacement field can be applied to any list of
+    atoms using 'field.apply_to(listofatoms)'.  The list of atoms is
+    modified using its 'GetCartesianPositions()' and
+    'SetCartesianPositions()' methods.
+
+    Example:
+
+      >>> from Setup.Lattice.FCC111Ortho import FCC111Ortho
+      >>> from Structures.ChemicalElements import *
+      >>> from Asap.Setup.Dislocation import ScrewDislocation
+      >>> from Numeric import *
+      >>> lat = FCC111Ortho((12,12,12), Copper, 3.6)
+      >>> center = matrixmultiply(lat.GetCoordinateBasis(), (0.5, 0.5, 0.5))
+      >>> disloc = ScrewDislocation(center, lat.MillerToDirection((1,1,1)), 3.6*sqrt(3.0))
+      >>> disloc.apply_to(lat)
+      >>> plot = lat.GetPlot()
     """
 
     # Make sure the burgers vector is a float, not a vector.
     if not isinstance(b, numbers.Real):
         raise TypeError("The 'Burgers vector' argument must be a number (specifying its length).")
     
     # Normalize line and cut, and assure that they are NumPy arrays
@@ -167,21 +171,36 @@
     vector matters). The third parameter
     ('Burgers', a 3-tuple) specifies the Burgers vector of the dislocation.
     The Burgers vector must be perpendicular to the line vector. Finally, the
     fourth argument is an optional parameter which specifies Poisson's ratio
     (unlike in the case of a screw dislocation, this number is needed in order
     to calculate the displacement field). The default value of Poisson's ratio
     is 1/3. 
-
-    Returns a `setup.displacementfield.DisplacementField` object.
-    Displacement fields may be added together (and multiplied by
-    scalars).  The dislplacement field can be applied to any 
-    Atoms object using field.`apply_to(atoms)`.  The Atoms are 
-    modified using the get_positions() and set_positions() methods.
     
+    Returns a Setup.DisplacementField.DisplacementField object.
+    Dislplacement fields may be added together (and multiplied by
+    scalars).  The dislplacement field can be applied to any list of
+    atoms using 'field.apply_to(listofatoms)'.  The list of atoms is
+    modified using its 'GetCartesianPositions()' and
+    'SetCartesianPositions()' methods.
+
+    Example:
+
+         from Setup.Lattice.FCC111Ortho import FCC111Ortho
+         from Structures.ChemicalElements import *
+         from Numeric import *
+         from Asap.Setup.Dislocation import EdgeDislocation
+         lat = FCC111Ortho((12,12,12), Copper, 6.78)
+         center = matrixmultiply(lat.GetCoordinateBasis(), (0.5, 0.5, 0.5)) 
+         line = lat.MillerToDirection((0,0,1))
+         Burgers = lat.MillerToDirection((0.5,0.5,0))
+         disloc = Edge(center, line, Burgers)
+         disloc.apply_to(lat)
+         plot = lat.GetPlot()         
+
     """
 
     # Normalize line and Burgers, and check their orthogonality
     b = magn(Burgers)
     normBurgers = array(Burgers) / b
     normline = array(line) / magn(line)
     assert perp(normline, normBurgers)
```

### Comparing `asap3-3.13.1/Python/asap3/setup/displacementfield.py` & `asap3-3.9.6/Python/asap3/setup/displacementfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,15 @@
 
     Function objects are callable objects (i.e. they behave like
     functions), but they can be added and multiplied with scalars
     and with themselves.
     """
     
     def __init__(self,expr):
-        self._expr = expr
-
-    def __call__(self, *args, **kwargs):
-        return self._expr(*args, **kwargs)
+        self.__call__=expr
 
     def __add__(self,other):
         if callable(other):
             return self.__class__(lambda x,other=other,oldfunc=self : oldfunc(x)+other(x))
         else:
             return self.__class__(lambda x,const=other,oldfunc=self : oldfunc(x)+const)
 
@@ -74,42 +71,43 @@
             return self.__class__(lambda x,other=other,oldfunc=self : other(x)/oldfunc(x))
         else:
             return self.__class__(lambda x,const=other,oldfunc=self : const/oldfunc(x))
 
 class DisplacementField(VectorFunction):
     """A displacement field.
 
-    Displacement fields are returned e.g. by the ``setup.dislocation``
-    modules, they are vector fields (see ``VectorFunction``) and can be
-    applied to a lattice using the ``apply_to()`` method.  The
+    Displacement fields are returned e.g. by the `Setup.Dislocation`
+    modules, they are vector fields (see `VectorFunction`) and can be
+    applied to a lattice using the `apply_to()` method.  The
     DisplacementField instance can also be used as a function taking
     an N x 3 array of positions and returning an N x 3 array of
     displacements.
 
     To create a displacement field, define a function taking an N x 3
     array of positions and returning an N x 3 array of displacements,
     then create the DisplacementField with the function as the sole
     argument.  A 'lambda' construct will often be useful.  For an
-    example, see the source code of `setup.dislocation.ScrewDislocation`.
+    example, see the source code of `Setup.Dislocation.Screw`.
     
     """
 
     def apply_to(self, list, fixedbox=0, usepositions=None):
-        """Apply the displacement field to an Atoms object.
+        """Apply the displacement field to a list of atoms.
 
-        The atoms are modified to reflect the displacement field.
+        The list of atoms object is modified to reflect the displacement
+        field.
 
         Two optional arguments are possible.
 
         fixedpox (default: 0): Adjust the displacement field to keep
         the corners of the computational box fixed by adding a smooth
         displacement field to the specified field.
 
         usepositions (default: None): If given, it must be an array
-        containing the positions of all atoms, to be used
+        containing the Cartesian positions of all atoms, to be used
         instead of the positions extracted from the list of atoms.  It
         can be useful if several displacement fields are to be applied
         to the same system, by giving the original positions as this
         argument the fields can be applied sequentially while
         obtaining an effect similar to adding the fields and then
         applying the sum.  This is mainly useful if the displacement
         field contains discontinuities, where a previously applied
```

### Comparing `asap3-3.13.1/Python/asap3/setup/nanocrystalline/helpers.py` & `asap3-3.9.6/Python/asap3/setup/make_sample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,17 @@
 from __future__ import print_function
 from __future__ import absolute_import
-from __future__ import division
 from asap3 import NeighborCellLocator
-from asap3.setup.multidislocation import random_dislocations
-from asap3.setup.dislocation import Dislocation
-from asap3.memory import get_max_memory
 from ase.atoms import Atoms
-from ase.lattice.cubic import FaceCenteredCubic, BodyCenteredCubic
-import ase.data
+from ase.lattice.cubic import FaceCenteredCubic
 import numpy as np
 import scipy.spatial
-from multiprocessing import Pool, cpu_count
 from . import plane_utils
 from . import quat_utils
 import math
-import sys
-import os
-
-###
-###  Below are helper functions for make_nanocrystalline
-###
 
 
 def remove_close(atoms, min_dist):
     "Remove atoms that are too close"
     print("Removing atoms that are too close (d_cut = %.3f Angstrom)" % (min_dist,))
     remove = set()
     nblist = NeighborCellLocator(min_dist, atoms)
@@ -47,62 +35,32 @@
     for i in a:
         for j in a:
             for k in a:
                 if i == j == k == 0: continue
                 ctr += [size * [i, j, k] + c for c in centres]
     ctr = np.array(ctr)
 
-    voronoi = scipy.spatial.Voronoi(ctr, furthest_site=False,
-                                    incremental=False, qhull_options=None)
+    voronoi = scipy.spatial.Voronoi(ctr, furthest_site=False, incremental=False, qhull_options=None)
     regions = [voronoi.regions[voronoi.point_region[i]] for i in range(len(centres))]
 
     grain_cells = []
     for i, reg in enumerate(regions):
 
         cell_vertices = np.array([voronoi.vertices[v] for v in reg])
         hull = scipy.spatial.ConvexHull(cell_vertices)
 
-        bounding_planes = [plane_utils.plane_equation(centres[i], h, cell_vertices)
-                           for h in hull.simplices]
+        bounding_planes = [plane_utils.plane_equation(centres[i], h, cell_vertices) for h in hull.simplices]
         grain_cells += [(cell_vertices, bounding_planes)]
 
     return grain_cells
 
-_field_to_apply = None
-
-def apply_fields(r):
-    global _field_to_apply
-    res = np.zeros_like(r)
-    for f in _field_to_apply:
-        res += f(r)
-    return res
-
-_positions_args = None
-def create_layer_positions(i):
-    global _positions_args
-    y0, y1, z0, z1, unit = _positions_args
-    positions = [np.dot((i, j, k), unit.cell) + atom_pos
-                 for j in range(y0, y1+1)
-                 for k in range(z0, z1+1)
-                 for atom_pos in unit.get_positions()]
-    return np.array(positions)
 
-def create_atoms(centres, rotations, unit, size, min_dist, dislocations=None,
-                 multiproc=False):
+def create_atoms(centres, rotations, unit, size, min_dist):
     "Create the nanocrystalline sample"
-    global _field_to_apply, _positions_args
 
-    if multiproc:
-        if multiproc is True:
-            multiproc_cpus = None  # Use default
-        else:
-            if not isinstance(multiproc, int) or multiproc <= 0:
-                raise TypeError("multiproc argument must be a positive integer.")
-            multiproc_cpus = multiproc  # Use specified number
-            
     grain_cells = calculate_grain_bounding_planes(centres, size)
 
     ntotal = 0
     result = None
     for grain_num, (centre, rotation) in enumerate(zip(centres, rotations)):
         assert centre.shape == (3,)
         assert rotation.shape == (3,3)
@@ -130,88 +88,69 @@
         y0 = int(math.floor(ymin / cubic_cell[1]))
         z0 = int(math.floor(zmin / cubic_cell[2]))
 
         x1 = int(math.ceil(xmax / cubic_cell[0]))
         y1 = int(math.ceil(ymax / cubic_cell[1]))
         z1 = int(math.ceil(zmax / cubic_cell[2]))
 
-        # If there are dislocations, make space for their worst-case
-        # cumulative dislplacement
-        if dislocations:
-            field = dislocations[grain_num]
-            n_disl = len(field)
-            correction = int(n_disl // np.sqrt(2))
-            x0 -= correction
-            y0 -= correction
-            z0 -= correction
-            x1 += correction
-            y1 += correction
-            z1 += correction
-            
         #create cube of atoms    #todo: outer product
-        if multiproc:
-            _positions_args = (y0, y1, z0, z1, unit)
-            pool = Pool(multiproc_cpus)
-            positions = pool.map(create_layer_positions, range(x0, x1+1))
-            positions = np.concatenate(positions)
-            pool.close()
-        else:
-            positions = [np.dot((i, j, k), unit.cell) + atom_pos
-                         for i in range(x0, x1+1)
-                         for j in range(y0, y1+1)
-                         for k in range(z0, z1+1)
-                         for atom_pos in unit.get_positions()]
-            positions = np.array(positions)
-        print("Temporary length of position array:", len(positions))
-        sys.stdout.flush()
-        # Apply dislocation field, if any
-        if dislocations:
-            centre_of_mass = positions.sum(axis=0)/len(positions)
-            if multiproc:
-                if multiproc_cpus:
-                    ncores = multiproc_cpus
-                else:
-                    ncores = cpu_count()
-                print("Using {} cores.".format(ncores))
-                _field_to_apply = field  # Cannot pass a lambda to Pool.map
-                arg = np.array_split(positions - centre_of_mass, ncores)
-                pool = Pool(multiproc_cpus)
-                res = pool.map(apply_fields, arg)
-                totalfield = np.concatenate(res)
-                pool.close()
-                assert totalfield.shape == positions.shape
-            else:
-                totalfield = np.zeros_like(positions)
-                for i, f in enumerate(field):
-                    totalfield += f(positions - centre_of_mass)
-            positions = positions + totalfield
-            print(n_disl, "dislocations introduced.")
-            sys.stdout.flush()
-        # Apply rotation
-        positions = np.dot(positions, U.transpose())
-        
+        positions = [np.dot(U, (np.dot((i, j, k), unit.cell) + atom_pos)) for i in range(x0, x1+1) for j in range(y0, y1+1) for k in range(z0, z1+1) for atom_pos in unit.get_positions()]
+        positions = np.array(positions)
+        print(len(positions))
+
         #remove excess atoms
-        print("Removing excess atoms.")
         in_cell = np.ones(len(positions)).astype(np.int8)
         for (p, n) in bounding_planes:
             in_cell = np.logical_and(in_cell, np.dot(n, (positions - p).T) > 0)
 
         positions = positions[in_cell]
 
-        print("Creating Atoms object, and merging...")
         atoms = Atoms(positions = positions, cell=size, numbers = 29 * np.ones(len(positions)))
         atoms.set_tags(grain_num * np.ones(len(atoms), int))
         if result is None:
             result = atoms
             atoms.set_cell(size, scale_atoms=False)
             atoms.set_pbc(True)
         else:
             result.extend(atoms)
-        print("grain %d contains %d atoms (max mem. %.1f GB)."
-              % (grain_num, len(positions), get_max_memory()/1024))
-        sys.stdout.flush()
+        print("grain: %d contains %d atoms" % (grain_num, len(positions)))
 
     print("Total atoms:", len(result))
     result = remove_close(result, min_dist)
     print("Remaining atoms:", len(result))
     return result
 
+def make_nanocrystal(size, centres, rotations, min_dist=2.0, unit=None, symbol=None, latticeconstant=None):
+    """Create a nanocrystalline sample.
+
+    Parameters:
+      size:      Size of the system, in Angstrom (either a number or three numbers).
+      centres:   Positions of grains in scaled coordinates.
+      rotations: Rotation matrices for the grains.
+
+      min_dist (optional):
+                 If two atoms are closer than this distance, one of them is removed
+                 (default: 2.0).
+
+    In addition, either the 'unit' or the 'symbol' parameter must be specified.
+      unit (optional):
+                 A unit cell for building the crystals (Atoms object).
+                 MUST be orthorhombic!
+      symbol (optional):
+                 If unit is None, then an FCC crystal of this element is used.
+      latticeconstant (optional):
+                 If symbol is specified, this overrides the default lattice constant.
+    """
+
+    assert type(size) == float or type(size) == list
+    if type(size) == float:
+        size = np.array([size, size, size])
+    elif type(size) == list:
+        size = np.array(size)
+    assert size.shape == (3,)
+    assert len(centres) == len(rotations)
+    centres *= size
+    if unit is None:
+        unit = FaceCenteredCubic(symbol=symbol, size=(1,1,1), pbc=True, latticeconstant=latticeconstant)
+
+    return create_atoms(centres, rotations, unit, size, min_dist)
+
```

### Comparing `asap3-3.13.1/Python/asap3/setup/nanocrystalline/plane_utils.py` & `asap3-3.9.6/Python/asap3/setup/plane_utils.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/setup/nanocrystalline/quat_utils.py` & `asap3-3.9.6/Python/asap3/setup/quat_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     s1 = math.sin(x1)
     c1 = math.cos(x1)
     s2 = math.sin(x2)
     c2 = math.cos(x2)
     return np.array([s1*r1, c1*r1, s2*r2, c2*r2])
 
 def random_rotation_matrix():
+    q = random_quaternion()
+    return quaternion_to_rotation_matrix(q)
+
+def random_rotation_matrix():
     """Returns a random rotation matrix."""
     return quaternion_to_rotation_matrix(random_quaternion())
 
 def rotation_matrix_to_quaternion(u):
 
     r11 = u[0][0]
     r12 = u[0][1]
```

### Comparing `asap3-3.13.1/Python/asap3/testtools.py` & `asap3-3.9.6/Python/asap3/testtools.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Python/asap3/timing.py` & `asap3-3.9.6/Python/asap3/timing.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/BrennerNanotube.py` & `asap3-3.9.6/Test/BrennerNanotube.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/BrennerPullNanotube.py` & `asap3-3.9.6/Test/BrennerPullNanotube.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from ase.structure import nanotube
 from ase.optimize import BFGS, MDMin
 from asap3 import BrennerPotential
 from asap3.testtools import ReportTest
 import numpy as np
 
 atoms = nanotube(5, 5, length=10)
-atoms.center(axis=(0,1), vacuum=0.0)
 atoms.set_calculator(BrennerPotential())
 uc = atoms.get_cell()
 l0 = uc[2,2]
 
 e = -1e100
 for eps in np.linspace(0, 0.5, 201):
     uc[2,2] = l0 * (1 + eps)
```

### Comparing `asap3-3.13.1/Test/BrennerStress.py` & `asap3-3.9.6/Test/BrennerStress.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 """
 from __future__ import print_function
 
 from asap3 import *
 from ase import data, Atoms
 from ase.lattice.cubic import Diamond
 from ase.lattice.hexagonal import Graphite
+#from asap3.md.verlet import VelocityVerlet
+#from asap3.md.langevin import Langevin
 from asap3.testtools import ReportTest
 import numpy as np
 
 defaultstrains = 0.01 * np.array((-1, -0.75, -0.5, -0.25, 0.0,
                                          0.25, 0.5, 0.75, 1.0))
                                        
 book = {}
@@ -127,20 +129,20 @@
         For bulk modulus, it will be ((0,0), (1,1), (2,2)) etc.
     """
     energies = []
     basis = atoms.get_cell()
     vol = np.linalg.det(basis)
     for epsilon in strains:
         if shear:
-            adjustment = np.zeros((3,3), float)
+            adjustment = np.zeros((3,3), np.float)
             for idx in indices:
                 adjustment[idx[0]] += idx[2] * epsilon * basis[idx[1]]
             atoms.set_cell(adjustment + basis, scale_atoms=True)
         else:
-            scaling = np.ones((3,3), float)
+            scaling = np.ones((3,3), np.float)
             for idx in indices:
                 scaling[idx[0]] += idx[1]*epsilon
             atoms.set_cell(scaling * basis, scale_atoms=True)
         energy = atoms.get_potential_energy()
         #print ""
         #print epsilon, energy/len(atoms)
         energies.append((epsilon, energy/vol))
@@ -261,13 +263,13 @@
         latconst = data.reference_states[z]['a']
         initial = Diamond(directions=[[1,0,0],[0,1,0],[0,0,1]],
                           symbol=symbol, size=(6,6,6))
         ReportTest("Number of atoms", len(initial), 6*6*6*8, 0)
     atoms = Atoms(initial)
     #view(atoms)
     atoms.set_calculator(BrennerPotential())
-    atoms.set_momenta(np.zeros((len(atoms),3), float))
+    atoms.set_momenta(np.zeros((len(atoms),3), np.float))
     findlatticeconst(atoms, latconst)
     del book[element]['symbol']
     elasticconstants(atoms, element, **book[element])
 
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/BundleTrajectory.py` & `asap3-3.9.6/Test/Trajectories_ase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from __future__ import print_function
 from asap3 import *
 from asap3.md.verlet import VelocityVerlet
 from ase.lattice.cubic import FaceCenteredCubic
-from asap3.io.trajectory import *
-#from ase.io.bundletrajectory import BundleTrajectory
+from ase.io.trajectory import *
 from ase.io import write
 from numpy import *
 import sys, os, time
 from asap3.testtools import ReportTest
 
 #DebugOutput("output.%d")
 print_version(1)
-delete = True
-#precision = 1.5e-4  # We store positions in single precision.
+delete = False
 precision = 1e-8
 
 def maketraj(atoms, t, nstep):
     e = [atoms.get_potential_energy()]
     dyn = VelocityVerlet(atoms, 5*units.fs)
     for i in range(nstep):
         dyn.run(10)
@@ -38,66 +36,43 @@
         if recalc:
             atoms.set_calculator(EMT())
         ReportTest("Checking frame %d" % (i,), atoms.get_potential_energy(),
                    e[i], precision)
         i += 1
 
 initial = FaceCenteredCubic(size=(10,10,10), symbol="Cu", pbc=(1,0,0))
-initial.set_momenta(zeros((len(initial),3)))
-initial.set_tags(arange(len(initial)))
+
 
 atoms = initial.copy()
 atoms.set_calculator(EMT())
 print("Writing trajectory")
-traj = BundleTrajectory("traj1.bundle", "w", atoms, singleprecision=False)
+traj = Trajectory("traj1.traj", "w", atoms)
+atoms.get_potential_energy()
 traj.write()
 energies = maketraj(atoms, traj, 10)
 traj.close()
 
 print("Reading trajectory (recalculating energies)")
-traj = BundleTrajectory("traj1.bundle")
+traj = Trajectory("traj1.traj")
 checktraj(traj, energies)
 
 print("Reading trajectory (stored energies)")
-traj = BundleTrajectory("traj1.bundle")
+traj = Trajectory("traj1.traj")
 checktraj(traj, energies, recalc=False)
 
-print("Repeating simulation")
-atoms = traj[5]
-atoms.set_calculator(EMT())
-energies2 = maketraj(atoms, None, 5)
-for i in range(5):
-    ReportTest("Rerun[%d]" % (i,), energies2[i], energies[i+5], precision)
-traj.close()
-
-print("Appending to trajectory")
-atoms = BundleTrajectory("traj1.bundle")[-1]
-atoms.set_calculator(EMT())
-traj = BundleTrajectory("traj1.bundle", "a", atoms)
-energies2 = maketraj(atoms, traj, 5)
-traj.close()
-
-print("Reading longer trajectory")
-traj = BundleTrajectory("traj1.bundle")
-checktraj(traj, energies + energies2[1:])
-
-print("Writing trajectory with write")
-write("traj2.bundle", atoms, format='bundletrajectory')
-
 print("Writing a trajectory without precalculated energies.")
 atoms = initial.copy()
 atoms.set_calculator(EMT())
-traj = BundleTrajectory("traj3.bundle", "w", atoms, singleprecision=False)
+traj = Trajectory("traj3.traj", "w", atoms, properties=['energy'])
+atoms.get_potential_energy()
 traj.write()
 maketraj_no_e(atoms, traj, 10)
 traj.close()
-traj = BundleTrajectory("traj3.bundle")
+traj = Trajectory("traj3.traj")
 checktraj(traj, energies, recalc=False)
 
 if delete:
     print("Deleting trajectory")
-    BundleTrajectory.delete_bundle("traj1.bundle")
-    BundleTrajectory.delete_bundle("traj2.bundle")
-    BundleTrajectory.delete_bundle("traj3.bundle")
-
+    os.unlink("traj1.traj")
+    os.unlink("traj3.traj")
     
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/CNAleak.py` & `asap3-3.9.6/Test/CNAleak.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/CalculationRequired.py` & `asap3-3.9.6/Test/CalculationRequired.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/ChangeAtoms.py` & `asap3-3.9.6/Test/ChangeAtoms.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/ChangeAtoms2.py` & `asap3-3.9.6/Test/ChangeAtoms2.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/ChangeCalculator.py` & `asap3-3.9.6/Test/ChangeCalculator.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/ChangePeriodicity.py` & `asap3-3.9.6/Test/ChangePeriodicity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,29 @@
 from __future__ import print_function
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from numpy import *
 from asap3.testtools import ReportTest
 
 print_version(1)
+#set_verbose(1)
 
 atoms = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]], size=(6,6,6),
                           symbol="Cu", pbc=(1,1,0))
 atoms.set_calculator(EMT())
 ecorrect = atoms.get_potential_energy()
 
 atoms2 = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]], size=(6,6,6),
                           symbol="Cu", pbc=(0,0,0))
-atoms2.set_calculator(EMT())
-atoms2.get_potential_energy()
 atoms2.set_pbc((1,1,0))
+atoms2.set_calculator(EMT())
 e1= atoms2.get_potential_energy()
-ReportTest("PBC (0,0,0) -> (1,1,0) correct", e1, ecorrect, 0.001)
-
-atoms3 = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]], size=(6,6,6),
-                          symbol="Cu", pbc=(1,1,1))
-atoms3.set_calculator(EMT())
-atoms3.get_potential_energy()
-atoms3.set_pbc((1,1,0))
-e3= atoms3.get_potential_energy()
-ReportTest("PBC (0,0,0) -> (1,1,0) correct", e3, ecorrect, 0.001)
-
-
-
+ReportTest("e1 correct", e1, ecorrect, 0.001)
 
 atoms.set_pbc((0,1,0))
-atoms.get_potential_energy()
 atoms.set_pbc((1,1,0))
 e2 = atoms.get_potential_energy()
 ReportTest("e2 correct", e2, ecorrect, 0.001)
 
 print("Setting pbc")
 atoms.set_pbc((0,1,0))
 print("Calculating energy")
```

### Comparing `asap3-3.13.1/Test/ChangeUnitCell.py` & `asap3-3.9.6/Test/ChangeUnitCell.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/ChangeUnitCell2.py` & `asap3-3.9.6/Test/ChangeUnitCell2.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/ConstraintInTraj.py` & `asap3-3.9.6/Test/ConstraintInTraj.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from __future__ import print_function
 from asap3 import *
 from asap3.constraints import FixAtoms
 from ase.lattice.cubic import FaceCenteredCubic
 from ase.io import read, write
 from asap3.io import Trajectory
 import os
-import numpy as np
-
-usemask = True
 
 fn = "testconstraint"
 atoms = FaceCenteredCubic(symbol='Cu', size=(3,3,3))
-if usemask:
-    c = FixAtoms(mask=np.arange(len(atoms))<3)
-else:
-    c = FixAtoms(indices=(2,3))
+c = FixAtoms(indices=(2,3))
 atoms.set_constraint(c)
-print(c)
 
 traj = Trajectory(fn+'.trj', "w", atoms)
 traj.write()
 traj.close()
 del traj
 
 traj = BundleTrajectory(fn+'.bundle', "w", atoms)
```

### Comparing `asap3-3.13.1/Test/Constraints.py` & `asap3-3.9.6/Test/Constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the FixAtoms constraint and the Subset filter."""
+from __future__ import print_function
 
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.md.velocitydistribution import MaxwellBoltzmannDistribution
 from asap3.md.verlet import VelocityVerlet
 from ase.constraints import Filter
 from asap3.constraints import FixAtoms
@@ -10,15 +11,15 @@
 from asap3.testtools import ReportTest
 import numpy as np
 
 init = FaceCenteredCubic(size=(10,10,10), symbol='Cu', pbc=False)
 z = init.get_positions()[:,2]
 fixedatoms = np.less(z, 0.501*z.max())
 print(len(init), sum(fixedatoms))
-MaxwellBoltzmannDistribution(init, temperature_K=2000)
+MaxwellBoltzmannDistribution(init, 2000*units.kB)
 
 print()
 print("Running simulation with Filter")
 atoms1 = Atoms(init)
 atoms1.set_calculator(EMT())
 atoms1a = Filter(atoms1, mask=np.logical_not(fixedatoms))
 
@@ -60,24 +61,24 @@
 
 print()
 print("Running Langevin simulation with Asap's FixAtoms")
 atoms4 = Atoms(init)
 atoms4.set_calculator(EMT())
 atoms4.set_constraint(FixAtoms(mask=fixedatoms))
 
-dyn = Langevin(atoms4, 0.5*units.fs, temperature_K=1000, friction=0.01)
+dyn = Langevin(atoms4, 0.5*units.fs, 1000*units.kB, 0.01)
 dyn.run(50)
 
 print()
 print("Running Langevin simulation with ASE's FixAtoms")
 atoms5 = Atoms(init)
 atoms5.set_calculator(EMT())
 atoms5.set_constraint(ASE_FixAtoms(mask=fixedatoms))
 
-dyn = Langevin(atoms5, 0.5*units.fs, temperature_K=1000, friction=0.01)
+dyn = Langevin(atoms5, 0.5*units.fs, 1000*units.kB, 0.01)
 dyn.run(50)
 
 print()
 sanity = [[atoms1, "Verlet + Filter"],
           [atoms2, "Verlet + Asap's FixAtoms"],
           [atoms3, "Verlet + ASE's FixAtoms"],
           [atoms4, "Langevin + Asap's FixAtoms"],
```

### Comparing `asap3-3.13.1/Test/EMT2013elements.py` & `asap3-3.9.6/Test/EMT2013elements.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/EMTleak.py` & `asap3-3.9.6/Test/EMTleak.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/ExplicitMasses.py` & `asap3-3.9.6/Test/NoInterference.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,62 @@
+from __future__ import print_function
+# Test that various observers and analysis tools do not interfere with
+# the energy calculator e.g. by messing up the neighbor list.
+
+from asap3 import *
 from asap3.md.verlet import VelocityVerlet
 from asap3.md.langevin import Langevin
-from asap3.md.velocitydistribution import MaxwellBoltzmannDistribution
-from asap3 import EMT
+from ase.lattice.cubic import *
+from asap3.analysis import RestrictedCNA, RadialDistributionFunction
+from numpy import *
 from asap3.testtools import ReportTest
-from ase.build import bulk
-from ase import units
-import numpy as np
-
-# Global parameters:
-T=300
-timestep=5
-
-def testmd(atoms, dynclass, name, dynkwargs={}):
-    MaxwellBoltzmannDistribution(atoms, temperature_K=T*2, force_temp=True)
-    atoms.set_calculator(EMT())
-    dyn = dynclass(atoms, timestep=timestep*units.fs, **dynkwargs)
-    tt =  atoms.get_temperature()
-    print("Initial temperature:", tt)
-    ReportTest("Initial temperature ({})".format(name), tt, 2*T, 1e-9)
-    p = atoms.get_momenta()
-    print("Initial square momenta:", (p*p).sum())
-    dyn.run(500)
-    tt =  atoms.get_temperature()
-    print("Final temperature:", tt)
-    ReportTest("Final temperature ({})".format(name), tt, T, 20.0)
-    p = atoms.get_momenta()
-    print("Final square momenta:", (p*p).sum())
-    print()
-
-mass_Cu = 63.546
-size = 7
-
-atoms = bulk('Cu', cubic=True).repeat((size,size,size))
-assert len(atoms) == 4*size**3
-testmd(atoms, VelocityVerlet, "Verlet - normal")
-
-atoms = bulk('Cu', cubic=True).repeat((size,size,size))
-atoms.set_masses(0.5*mass_Cu*np.ones(len(atoms)))
-testmd(atoms, VelocityVerlet, "Verlet - low mass")
-
-lgvkw = {'temperature_K': T, 'friction':0.05}
-atoms = bulk('Cu', cubic=True).repeat((size,size,size))
-testmd(atoms, Langevin, "Langevin - normal", lgvkw)
-
-atoms = bulk('Cu', cubic=True).repeat((size,size,size))
-atoms.set_masses(0.5*mass_Cu*np.ones(len(atoms)))
-testmd(atoms, Langevin, "Langevin - low mass", lgvkw)
 
-ReportTest.Summary()
+def Compare(name, atoms, observer, ref, interval=4):
+    dyn = VelocityVerlet(atoms, 5*units.fs)
+    dyn.attach(observer, interval=interval)
+    r = []
+    for i in range(50):
+        dyn.run(5)
+        epot = atoms.get_potential_energy() / len(atoms)
+        ekin = atoms.get_kinetic_energy() / len(atoms)
+        r.append([epot, ekin, epot+ekin])
+    r = array(r)
+    diff = r - ref
+    maxdiff = diff.max()
+    print("Maximal difference is", maxdiff)
+    ReportTest(name, maxdiff, 0.0, 1e-6)
+    
+print_version(1)
+
+print("Making initial system")
+iniatoms = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]],
+                             size=(10,5,5), symbol="Cu", pbc=(1,1,0))
+iniatoms.set_calculator(EMT())
+inidyn = Langevin(iniatoms, 5*units.fs, 450*units.kB, 0.05)
+inidyn.run(100)
+print("Temperature is now", iniatoms.get_kinetic_energy() / (1.5*units.kB*len(iniatoms)), "K")
+
+print("Making reference simulation")
+refatoms = Atoms(iniatoms)
+refatoms.set_calculator(EMT())
+dyn = VelocityVerlet(refatoms, 5*units.fs)
+ref = []
+for i in range(50):
+    dyn.run(5)
+    epot = refatoms.get_potential_energy() / len(refatoms)
+    ekin = refatoms.get_kinetic_energy() / len(refatoms)
+    ref.append([epot, ekin, epot+ekin])
+
+ref = array(ref)
+
+print("Testing RestrictedCNA")
+atoms = Atoms(iniatoms)
+atoms.set_calculator(EMT())
+cna = RestrictedCNA(atoms)
+Compare("RestrictedCNA", atoms, cna.analyze, ref)
+
+print("Testing RadialDistributionFunction")
+atoms = Atoms(iniatoms)
+atoms.set_calculator(EMT())
+rdf = RadialDistributionFunction(atoms, 4.0, 25)
+Compare("RadialDistributionFunction", atoms, rdf.update, ref)
+
```

### Comparing `asap3-3.13.1/Test/FIRE.py` & `asap3-3.9.6/Test/FIRE.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 atoms = bulk('Cu')
 atoms = atoms.repeat((7, 7, 100))
 
 print("Testing FIRE relaxation")
 atoms.set_calculator(EMT())
 e0 = atoms.get_potential_energy()
-natoms = atoms.get_global_number_of_atoms()
+natoms = atoms.get_number_of_atoms()
 ReportTest("Number of atoms", natoms, 4900, 0)
 print("Potential energy before perturbation:", e0, e0/natoms)
 
 dx = 0.1 * np.sin(42 * np.arange(3 * len(atoms)))
 dx.shape = (-1, 3)
 atoms.set_positions(dx + atoms.get_positions())
 e1 = atoms.get_potential_energy()
```

### Comparing `asap3-3.13.1/Test/FieldPlotter.py` & `asap3-3.9.6/Test/FieldPlotter.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Hydrocarbons.py` & `asap3-3.9.6/Test/Hydrocarbons.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/LJ_Stress.py` & `asap3-3.9.6/Test/LJ_Stress.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/LargeShear.py` & `asap3-3.9.6/Test/LargeShear.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Lattice.py` & `asap3-3.9.6/Test/Lattice.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/LennardJones.py` & `asap3-3.9.6/Test/LennardJones.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 #!/usr/bin/python
 # Copyright (C) 2007  CAMP
 # Please see the accompanying LICENSE file for further information.
 
 # Tests the LennardJones potential.
 
+#import ASE.ChemicalElements.mass
+from __future__ import print_function
 from ase import Atoms, data
 
 from asap3 import *
 from ase.lattice.cubic import *
-from ase.lattice.compounds import *
 from asap3.testtools import ReportTest
 from asap3.md.verlet import VelocityVerlet
 
 from StressModule import *
 from time import time, localtime, strftime
 import numpy as np
 
 print_version(1)
 #AsapThreads()
 
 Silent=True
 
-if getattr(Atoms, '_ase_handles_dynamic_stress', False):
-    stresshack = {'include_ideal_gas': True}
-else:
-    stresshack = {}
-
 # Calculates Emin radius:
 # 4*epsilon*((sigma/rij)^12-(sigma/rij)^6)
 # f(r)  = 4*e*((s/r)^(12)-(s/r)^(6))
 # f'(r) = 4*e*(6*s^6/r^7-12*s^12/r^13)
 #         4*e*(6*s^6/r^7-12*s^12/r^13)=0
 #         r = s*2^(1/6)
 def EminRadius(sigma):
@@ -41,15 +37,14 @@
   #print ''
   elements = [29]
   epsilon  = [0.15]
   sigma    = [2.7]
 
   atoms=Atoms(positions=[(0.0, 0.0, 0.0),(10.0, 10.0, 10.0)],
               symbols="2Cu")
-  atoms.center(vacuum=1.0)
 
   atoms.set_calculator(LennardJones(elements, epsilon, sigma, -1.0, False))
 
  
   result = atoms.get_potential_energy()
   #print "Energy is ", result;
   ReportTest("Expected energy for two atoms with r>rcut", result, 0, 1e-12, silent=Silent)
@@ -61,15 +56,14 @@
   epsilon  = [0.15]
   sigma    = [2.7]
 
   EminR = EminRadius(sigma[0])
 
   atoms=Atoms(positions=[(0.0, 0.0, 0.0),(0.0, 0.0, EminR)],
                     symbols="Cu2")
-  atoms.center(vacuum=1.0)
 
   atoms.set_calculator(LennardJones(elements, epsilon, sigma, -1.0, False))
 
 
   result = atoms.get_potential_energy()
   ReportTest("  Expected energy for two atoms with r->Emin=-epsilon", result, -epsilon[0], 1e-14, silent=Silent)
 
@@ -78,15 +72,14 @@
   print("\nRunning LJ twoAtomForce")
   elements = [29]
   epsilon  = [0.15]
   sigma    = [2.7]
 
   atoms=Atoms(positions=[(0.0, 0.0, 0.0),(0.0, 0.0, 2.0)],
               symbols="Cu2")
-  atoms.center(vacuum=1.0)
 
   atoms.set_calculator(LennardJones(elements, epsilon, sigma, -1.0, False))
 
 
   result = atoms.get_potential_energy()
 
   r = atoms.get_positions()
@@ -106,15 +99,15 @@
 
   etot1 = (atoms.get_potential_energy() + atoms.get_kinetic_energy())
   dyn.run(1000)
   etot2 = (atoms.get_potential_energy() + atoms.get_kinetic_energy())
   ReportTest(("  Energy conservation (%s)" % ("Cu",)), etot1, etot2, 1.0, silent=Silent)
 
   epot = atoms.get_potential_energies()
-  stress = atoms.get_stresses(**stresshack)
+  stress = atoms.get_stresses()
 
   e = []
   s = []
   j = 0
   for i in range(0, len(atoms), 100):
       e.append(epot[i])
       s.append(stress[i,j])
@@ -148,17 +141,17 @@
       elements = [29, 79, 39]
       epsilon  = [0.15, 0.00, 0.00,
                   0.10, 0.25, 0.00,
                   0.31, 0.60, 0.15]
       sigma    = [2.7 , 0.00, 0.00,
                   1.90, 2.7 , 0.00,
                   2.20, 1.50, 2.7 ]
-      atoms = L1_2(directions=[[1,0,0],[0,1,0],[0,0,1]], size=(size,size,size),
-                     symbol=("Cu", "Au"), pbc=(1,0,1), debug=0,
-                     latticeconstant=3.95)
+      atoms = L1_2([[1,0,0],[0,1,0],[0,0,1]], size=(size,size,size),
+                              element=("Cu", "Au"), periodic=(1,0,1), debug=0,
+                              latticeconstant=3.95)
       atoms.set_calculator(LennardJones(elements, epsilon, sigma, rCut, v0))
     else:
       elements = [29]
       epsilon  = [0.15]
       sigma    = [2.7]
       atoms = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]],
                                 size=(size,size,size),
@@ -178,33 +171,33 @@
     for i in range(nsteps//10):
         dyn.run(10)
         #print atoms.get_potential_energy()/len(atoms), atoms.get_kinetic_energy()/len(atoms), (atoms.get_potential_energy() + atoms.get_kinetic_energy())/len(atoms)
     etot2 = (atoms.get_potential_energy() + atoms.get_kinetic_energy())
     ReportTest(("  Energy conservation (%s)" % ("Cu",)), etot1, etot2, 2, silent=Silent)
     print("Before: ", etot1, " now: ", etot2, " diff= ", (etot1-etot2))
     epot = atoms.get_potential_energies()
-    stress = atoms.get_stresses(**stresshack)
+    stress = atoms.get_stresses()
     print("  Reporting energies and stresses")
     
     e = []
     s = []
     j = 0
     for i in range(0, len(atoms), 100):
         e.append(epot[i])
         s.append(stress[i,j])
         j = (j + 1) % 6
     print("  e"+"Cu"+" =", repr(e))
     print("  s"+"Cu"+" =", repr(s))
     end = time();
     print("  ++++ Test runtime of the LJ dynamicsTest was %d seconds ++++\n\n" %(end-start))
     if 1:
-        sumstress = np.zeros(6, float)
+        sumstress = np.zeros(6, np.float)
         for s in stress:
             sumstress += s
-        totalstress = atoms.get_stress(**stresshack)
+        totalstress = atoms.get_stress()
         for i in range(6):
             ReportTest("Sum of stresses (%d)" % (i,), sumstress[i]/len(atoms),
                        totalstress[i], abs(0.01*totalstress[i]))
     
 
 #TODO: create a better test
 #some stress tests fail because the model doesn't quite fit:
@@ -258,29 +251,29 @@
     atoms = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]],
                               size=(size,size,size),
                               symbol="Cu", pbc=(1,0,1), debug=0,
                               latticeconstant=latconst)
 
     atoms.set_calculator(LennardJones(elements, epsilon, sigma, rCut, v0))
 
-    atoms.set_momenta(np.zeros((len(atoms),3), float))
+    atoms.set_momenta(np.zeros((len(atoms),3), np.float))
     #findlatticeconst(atoms, latconst)  ## Lattice const already OK
     elasticconstants(atoms, symb, fitfact=20.0, fitfact2=20.0, **book[symb])
     end = time();
     print("&&&& Test runtime of the LJ stressTest was %d seconds &&&&" %(end-start))
 
 
 start = time();
 twoAtomClose()
 twoAtomTest()
 twoAtomForce()
 #dynamicsTest(10, 10, 200, False, -1, True, False) #3 kinds of atoms, no map
 #dynamicsTest(10, 10, 200, False, -1, True, True)  #3 kinds of atoms, map
 dynamicsTest(10, 10, 200, False, -1, False) #1 kind of atom
-#dynamicsTest(20, 10, 200, True, -1, True)
+#dynamicsTest(20, 10, 200, True, -1, False)
 #dynamicsTest(10, 10, 10000, True, -1, False, False)
 #dynamicsTest(10, 10, 10000, True, -1, False, True)
 #dynamicsTest(10, 40000, 200, False, -1, False))
 stressTest(False)
 stressTest(False, True)
 #stressTest(True)
```

### Comparing `asap3-3.13.1/Test/LocalStructure.py` & `asap3-3.9.6/Test/LocalStructure.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/MonteCarloOptim_Alloy.py` & `asap3-3.9.6/Test/MonteCarloOptim_Alloy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def checkenergies(a, a2):
     err = 0
     if 0:
         print("    Checking Cartesian positions")
         err = abs((a.get_positions() - a2.get_positions()).ravel())
         idx = argmax(err)
-        at, co = idx//3, idx%3
+        at, co = idx/3, idx%3
         print("      err =", err[idx], "at", idx, ":", at, co)
         ReportTest("      Worst Cartesian position (%d,%d)" % (at, co),
                    a.get_positions()[at,co],
                    a2.get_positions()[at,co], 1e-10)
     print("    Checking energies")
     e1 = a.get_potential_energies()
     e2 = a2.get_potential_energies()
@@ -72,15 +72,15 @@
     print ("Number of %s atoms (Z=%d): %d"
            % (e[0], e[1], sum(equal(atoms.get_atomic_numbers(), e[1]))))
 
 print() 
 print("Testing perturbations of single atoms")
 
 magnarr = array((0.0, 0.01, 0.1, 1.0, 3.0, 10.0))
-numarr = array((1, 3, 10, len(atoms)//2, -3))
+numarr = array((1, 3, 10, len(atoms)/2, -3))
 pick1 = argsort(random.random((len(magnarr),)))
 for magn in take(magnarr, pick1):
     pick2 = argsort(random.random((len(numarr),)))
     for number in take(numarr, pick2):
         # Pick number random atoms.
         if number < 0:
             # Find N neighboring atoms and perturb them
```

### Comparing `asap3-3.13.1/Test/MonteCarloOptim_Energy.py` & `asap3-3.9.6/Test/MonteCarloOptim_Energy.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/MonteCarloOptim_NbList.py` & `asap3-3.9.6/Test/MonteCarloOptim_NbList.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     #nb2 = FullNeighborList(a, cut)
     a2 = Atoms(a)
     #nb2 = NeighborList(cut, a2, 0, full=True)
     nb2 = FullNeighborList(cut, a2, 0)
     print("    Checking Cartesian positions")
     err = abs((a.get_positions() - a2.get_positions()).ravel())
     idx = argmax(err)
-    at, co = idx//3, idx%3
+    at, co = idx/3, idx%3
     print("      err =", err[idx], "at", idx, ":", at, co)
     ReportTest("      Worst Cartesian position (%d,%d)" % (at, co),
                a.get_positions()[at,co],
                a2.get_positions()[at,co], 1e-10)
     #print "    Checking internal positions"
     #err = abs((a.GetInternalPositions() - a2.GetInternalPositions()).flat)
     #idx = argmax(err)
@@ -116,15 +116,15 @@
 
 print() 
 print("Testing perturbations of single atoms")
 
 magnarr = array((0.0, 0.01, 0.1, 1.0, 3.0, 10.0))
 pick1 = argsort(random.random((len(magnarr),)))
 for magn in take(magnarr, pick1):
-    numarr = array((1, 3, 10, len(atoms)//2, -3))
+    numarr = array((1, 3, 10, len(atoms)/2, -3))
     pick2 = argsort(random.random((len(numarr),)))
     for number in take(numarr, pick2):
         # Pick number random atoms.
         if number < 0:
             # Find N neighboring atoms and perturb them
             number = -number
             n = 0
```

### Comparing `asap3-3.13.1/Test/Morse.py` & `asap3-3.9.6/Test/Morse.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 def TestPotentialCutoff():
     print("Running TestPotentialCutoff...")
 
     for e1 in elements:
         for e2 in elements:
             calc = Morse(elements, epsilon, alpha, rmin)
             atoms = Atoms([e1, e2], [[0.0, 0.0, 0.0], [rcut + 1.0, 0.0, 0.0]])
-            atoms.center(vacuum=1.0)
             atoms.set_calculator(calc)
 
             energy = atoms.get_potential_energy()
 
             s1, s2 = chemical_symbols[e1], chemical_symbols[e2]
             ReportTest("Energy for %s-%s with r > rcut" % (s1, s2),
                        energy, 0.0, 1e-12, silent=True)
@@ -37,15 +36,14 @@
 def TestPotentialMinimum():
     print("Running TestPotentialMinimum...")
 
     for i, e1 in enumerate(elements):
         for j, e2 in enumerate(elements):
             calc = Morse(elements, epsilon, alpha, rmin)
             atoms = Atoms([e1, e2], [[0.0, 0.0, 0.0], [rmin[i, j], 0.0, 0.0]])
-            atoms.center(vacuum=1.0)
             atoms.set_calculator(calc)
 
             energy = atoms.get_potential_energy()
 
             s1, s2 = chemical_symbols[e1], chemical_symbols[e2]
             ReportTest("Energy for %s-%s with r = rmin" % (s1, s2),
                        energy, -epsilon[i, j], 1e-2, silent=True)
@@ -60,15 +58,15 @@
         i = np.random.randint(len(atoms)-1)
         if atoms[i].number != atomic_numbers['Ru']:
             atoms[i].number = atomic_numbers['Ru']
             n += 1
     atoms.set_calculator(calc)
 
     # Set initial momentum
-    MaxwellBoltzmannDistribution(atoms, temperature_K=300)
+    MaxwellBoltzmannDistribution(atoms, 300*units.kB)
 
     # Run dynamics
     dyn = VelocityVerlet(atoms, 1.0 * units.fs, logfile='test-energy.dat', loginterval=10)
     dyn.run(10)
     etot = (atoms.get_potential_energy() + atoms.get_kinetic_energy())/len(atoms)
     print("%-9s %-9s %-9s" % ("Epot", "Ekin", "Sum"))
     for i in range(25):
```

### Comparing `asap3-3.13.1/Test/NbCellLocator.py` & `asap3-3.9.6/Test/NbCellLocator.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/NeighborList.py` & `asap3-3.9.6/Test/NeighborList.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/NoMI_LeftHanded.py` & `asap3-3.9.6/Test/NoMI_LeftHanded.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/OpenKIM_AllModels.py` & `asap3-3.9.6/Test/OpenKIM_AllModels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,181 +1,154 @@
 from __future__ import print_function
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.testtools import ReportTest
 import numpy as np
+from OpenKIM_modelname import openkimmodels
 from numpy.random import RandomState
-from ase.data import reference_states, atomic_numbers, chemical_symbols
-from ase.build import bulk
+from ase.data import reference_states, atomic_numbers
+from ase.lattice import bulk
 import sys
 
-brokenmodels = [
-    'ex_model_Ar_P_Morse_MultiCutoff',                           # Does not set Destroy pointer.
-    'EAM_IMD_BrommerGaehler_2006B_AlNiCo__MO_128037485276_003',  # Force and energy inconsistent
-    'EAM_NN_Johnson_1988_Cu__MO_887933271505_002',               # Force and energy inconsistent
-    'EAM_Magnetic2GQuintic',                                     # Crash with Intel compiler.
-    'EAM_MagneticCubic',                                         # Crash with Intel compiler.
-    'amp_parametrized_model',                                    # Experimental
-    # The following break in openkim-20210128
-    #'SNAP_',                                                     # Fails to initialize.  [1]
-    'Tersoff_LAMMPS_',  # [2]
-    ]
-
-# [1]  Unable to convert energy unit.
-
-# [2] Error returned by KIM's ConvertUnit() when trying to get charge units.
-
-
-# Some models require a specific primary and secondary element,
-# e.g. if it is aiming at impurity calculations, and using the wrong
-# element as host brings it outside its comfort zone.
-explicit_elements = {
-    'EAM_Dynamo_HepburnAckland_2008_FeC__MO_143977152728_005': ('Fe', 'C'),   # C impurity in Fe
-    'EAM_Dynamo_SmirnovaKuskinStarikov_2013_UMoXe__MO_679329885632_005': ('U', 'Mo'),
-    'SW_WangStroudMarkworth_1989_CdTe__MO_786496821446_000': ('Cd', 'Te'),
-    'SW_ZhouWardMartin_2013_CdTeZnSeHgS__MO_503261197030_002': ('Zn', 'Se'),
-    }
-
-# These models are painfully slow on a 7x7x7 system.
-smallmodel = {
-    'DUNN_WenTadmor_2019v1_C__MO_584345505904_000',
-    'DUNN_WenTadmor_2019v2_C__MO_956135237832_000',
-    'DUNN_WenTadmor_2019v3_C__MO_714772088128_000',
-}
-
+brokenmodels = ['Dipole_Umeno_YSZ__MO_394669891912_001',  # Crash with Intel compiler, some consistency problems
+                'IMD_EAM_Schopf_',   # Crash.  Also fails vc_forces_numer_deriv
+                'Pair_Morse_Shifted_GirifalcoWeizer_HighCutoff_St__MO_497591319122_001',  # No such element.  St ????
+                'Pair_Morse_Shifted_GirifalcoWeizer_LowCutoff_St__MO_801083489225_001',   # No such element.  St ????
+                'Pair_Morse_Shifted_GirifalcoWeizer_MedCutoff_St__MO_964297938209_001',   # No such element.  St ????
+                'kcc_meam_LiSi__MO_596436139350_001',  # Crash if simulator supports particleEnergies.
+                'EMT_Asap_MetalGlass_CuMgZr__MO_655725647552_001',   # Crash - known to be broken.
+                'EMT_Asap_Standard_Jacobsen_Stoltze_Norskov_AlAgAuCuNiPdPt__MO_118428466217_001', # do.
+                'model_ArCHHeXe_BOP_AIREBO__MO_154399806462_001',  # Exception.  Too many particles.  FORTRAN
+                'MEAM_2NN_Fe_to_Ga__MO_145522277939_001',  # Crash if simulator supports particleEnergies.
+                'MEAM_2NN_GaInN__MO_117938381510_001',     # Crash if simulator supports particleEnergies.
+                'Glue_Ercolessi_Adams_Al__MO_324507536345_001',  # Segmentation fault.  FORTRAN
+               ]
     
 tolerance = 1e-4
 #set_verbose(1)
 
-if OpenKIMsupported:
-    openkimmodels = OpenKIMavailable()
-else:
+if not OpenKIMsupported:
     openkimmodels = []
     print("OpenKIM support is not compiled into Asap.")
     
 #rnd = RandomState(42)  # We want deterministic random numbers
 rnd = RandomState()
 
 known_states = ['bcc', 'fcc', 'hcp', 'diamond', 'sc']
 
-delta = 0.001
+delta = 0.01
+
+openkimmodels = openkimmodels + ['EMT']
 
 if len(sys.argv) > 1:
     openkimmodels = sys.argv[1:]
     brokenmodels = []
 
 skipped = []
 crashed = []
-
-#rnd.shuffle(openkimmodels)
-
 for model in openkimmodels:
     broken = False
     for brk in brokenmodels:
         if model.startswith(brk):
             broken = True
     if broken:
         print("\nSkipping broken KIM model:", model)
-        skipped.append((model, "Blacklisted"))
+        skipped.append(model)
         continue
     print("\nKIM model:", model)
     if model == 'EMT':
-        calculator = EMT()
         elements = ('Cu', 'Au', 'Ag')
+        nblists = [None]
+        access = [None]
     else:
-        calculator = OpenKIMcalculator(model)
-        elements = calculator.get_supported_elements(user=False)
+        info = OpenKIMinfo(model)
+        elements = info.get_supported_types()
+        nblists = info.get_supported_nblist()
+        access = info.get_supported_access()
     print("Supported elements:", elements)
-    overrule_elements = model in explicit_elements
-    if overrule_elements:
-        elements = explicit_elements[model]
-    if len(elements) == 0:
-        print("No standard elements supported - SKIPPING MODEL!")
-        continue
-    elif len(elements) == 1:
+    print("Supported neighborlist methods:", nblists)
+    print("Supported access methods:", access)
+    if len(access) > 1:
+        access = ['loca', 'iter']
+    else:
+        access = [None]
+    if len(elements) == 1:
         main = elements[0]
         other = None
         state = reference_states[atomic_numbers[main]]
     else:
-        if not overrule_elements:
-            elements = list(elements)
-            rnd.shuffle(elements)
+        elements = list(elements)
+        rnd.shuffle(elements)
         for i in range(len(elements)):
             main = elements[i]
             other = elements[i-1]
             state = reference_states[atomic_numbers[main]]
-            if state and state['symmetry'] in known_states:
+            if state['symmetry'] in known_states:
                 break
     if state['symmetry'] not in known_states:
-        print("Cannot simulate {}, reference state '{}' not supported".format(main, state['symmetry']))
+        print("Cannot simulate %s, reference state '%s' not supported" % (main, state['symmetry']))
         print("SKIPPING MODEL!")
         continue
-
-    for case in range(2):
-        if case == 0:
-            if model in smallmodel:
-                init_atoms = bulk(main, orthorhombic=True).repeat((4,4,4))
-            else:
-                init_atoms = bulk(main, orthorhombic=True).repeat((7,7,7))
-        elif case == 1:
-            init_atoms = bulk(main).repeat((1,2,7))
-            # We cannot reuse the OpenKIMcalculator
-            if model != "EMT":
-                calculator = OpenKIMcalculator(model)
-        else:
-            raise RuntimeError("Unknown case "+str(case))
-        r = init_atoms.get_positions()
-        r += rnd.normal(0.0, 0.1, r.shape)
-        init_atoms.set_positions(r)
-        z = init_atoms.get_atomic_numbers()
-        if other:
-            some_atoms = rnd.randint(0, 20, len(init_atoms)) == 0
-            z[some_atoms] = atomic_numbers[other]
-            init_atoms.set_atomic_numbers(z)
-            z_other = atomic_numbers[other]
-        else:
-            z_other = 0
-        print ("Generated a %s system with %i %s-atoms and %i %s-atoms"
-                   % (state['symmetry'], 
-                          np.equal(z, atomic_numbers[main]).sum(),
-                          main,
-                          np.equal(z, z_other).sum(),
-                          other))
-        print("Lattice constant a =", state['a']) 
-        old_energy = old_forces = None
-        rndat = rnd.randint(len(init_atoms))
-
-
-
-        #print "Testing %s with %s" % (model, nbl)
-        atoms = Atoms(init_atoms)
-        try:
-            atoms.set_calculator(calculator)
-            e = atoms.get_potential_energy()
-            f = atoms.get_forces()
-        except (RuntimeError, ValueError, AsapError) as exc:
-            txt = "{} (case {}) raised exception {}: {}".format(model, case, str(type(exc)), str(exc))
-            print(txt)
-            crashed.append(txt)
-            continue
-
-        atoms[rndat].position[0] += delta
-        de = atoms.get_potential_energy() - e
-        f = 0.5 * f + 0.5 * atoms.get_forces()
-        exp_de = -delta * f[rndat,0]
-        #print "Old energy: %.9f.   Change: %.9f    Expected: %.9f   Abs: %.9e   Relative: %.9f" % (e, de, exp_de, de-exp_de, (de-exp_de)/exp_de)
-        ReportTest("{} (case {}) force consistent".format(model, case), de, exp_de, tolerance)
-
     
-print("Skipped models:")
-if skipped:
-    for m in skipped:
-        print("   {}: \t{}".format(*m))
-else:
-    print("    None")
+    init_atoms = bulk(main, orthorhombic=True).repeat((7,7,7))
+    r = init_atoms.get_positions()
+    r += rnd.normal(0.0, 0.1, r.shape)
+    init_atoms.set_positions(r)
+    z = init_atoms.get_atomic_numbers()
+    if other:
+        some_atoms = rnd.randint(0, 20, len(init_atoms)) == 0
+        z[some_atoms] = atomic_numbers[other]
+        init_atoms.set_atomic_numbers(z)
+        z_other = atomic_numbers[other]
+    else:
+        z_other = 0
+    print ("Generated a %s system with %i %s-atoms and %i %s-atoms"
+           % (state['symmetry'], 
+              np.equal(z, atomic_numbers[main]).sum(),
+              main,
+              np.equal(z, z_other).sum(),
+              other))
+    print("Lattice constant a =", state['a']) 
+    old_energy = old_forces = None
+    rndat = rnd.randint(len(init_atoms))
+    for nbl in nblists:
+        for ac in access:
+            #print "Testing %s with %s" % (model, nbl)
+            atoms = Atoms(init_atoms)
+            if nbl == 'CLUSTER':
+                atoms.set_pbc(False)
+            try:
+                if model == 'EMT':
+                    atoms.set_calculator(EMT())
+                else:
+                    atoms.set_calculator(OpenKIMcalculator(model, allowed=nbl, access=ac))
+                e = atoms.get_potential_energy()
+                f = atoms.get_forces()
+            except (RuntimeError, ValueError, AsapError) as exc:
+                txt = ("%s with %s(%s) raised exception %s: %s" %
+                       (model, nbl, str(ac), str(type(exc)), str(exc)))
+                print(txt)
+                crashed.append(txt)
+                continue
+            if nbl != 'CLUSTER':
+                if old_energy == None:
+                    old_energy = e
+                    old_forces = f
+                else:
+                    ReportTest("%s with %s(%s); energy unchanged" % (model, nbl, str(ac)),
+                               e, old_energy, 1e-6)
+                    ReportTest("%s with %s(%s); force unchanged" % (model, nbl, str(ac)),
+                               f[rndat,0], old_forces[rndat,0], 1e-6)                    
+            atoms[rndat].position[0] += delta
+            de = atoms.get_potential_energy() - e
+            f = 0.5 * f + 0.5 * atoms.get_forces()
+            exp_de = -delta * f[rndat,0]
+            #print "Old energy: %.9f.   Change: %.9f    Expected: %.9f   Abs: %.9e   Relative: %.9f" % (e, de, exp_de, de-exp_de, (de-exp_de)/exp_de)
+            ReportTest("%s with %s(%s) force consistent" % (model, nbl, str(ac)), de, exp_de, tolerance)
+        
+print("Skipped models (registerd as crashing):")
+for m in skipped:
+    print("   ", m)
 print("Crashing models:")
-if crashed:
-    for m in crashed:
-        print("   ", m)
-else:
-    print("    None")
+for m in crashed:
+    print("   ", m)
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/OpenKIM_EMT.py` & `asap3-3.9.6/Test/OpenKIM_EMT.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,52 @@
 from __future__ import print_function
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.testtools import ReportTest
-from ase.build import bulk
 import numpy as np
-import itertools
-
-openkimmodel = 'EMT_Asap_Standard_JacobsenStoltzeNorskov_1996_%s__%s'
-
-shortkimid = {
-    'Ag': 'MO_303974873468_001',
-    'Al': 'MO_623376124862_001',
-    'Au': 'MO_017524376569_001',
-    'Cu': 'MO_396616545191_001',
-    'Ni': 'MO_108408461881_001',
-    'Pd': 'MO_066802556726_001',
-    'Pt': 'MO_637493005914_001',
-    }
+from OpenKIM_modelname import openkimmodel
 
 #set_verbose(1)
 step = 500
 
-if getattr(Atoms, '_ase_handles_dynamic_stress', False):
-    stresshack = {'include_ideal_gas': True}
-else:
-    stresshack = {}
-
 if OpenKIMsupported:
-    pbc_list = itertools.cycle(((1,1,1), (0,0,0), (0,0,1)))
-    size_list = itertools.cycle(((10, 10, 10), (20, 5, 2), (2, 2, 2), (1, 1, 1)))
-    elements = ('Al', 'Ag', 'Au', 'Cu', 'Ni', 'Pd', 'Pt')
+    pbc_candidates = ["NEIGH_RVEC_H", 
+                      "NEIGH_PURE_H",
+                      "NEIGH_RVEC_F", 
+                      "NEIGH_PURE_F",
+                      "MI_OPBC_H", 
+                      "MI_OPBC_F",
+                      "CLUSTER"
+                      ]
 else:
-    elements = ()
+    pbc_candidates = []
     print("OpenKIM support is not compiled into Asap.")
 
-for element in elements:
-    for i in (0, 1):
-        pbc = next(pbc_list)
-        size = next(size_list)
-        txt = ("%s=%i%i%i-%i-%i-%i " % ((element,) + pbc + size))
+for nbltype in pbc_candidates:
+    if nbltype.startswith("MI_OPBC"):
+        boundaries = ((1,1,1),)
+    elif nbltype == "CLUSTER":
+        boundaries = ((0,0,0),)
+    else:
+        boundaries = ((1,1,1), (0,0,0), (0,0,1))
+        
+    for pbc in boundaries:
+        txt = nbltype + (" PBC=%1i%1i%1i " % pbc)
         # Test that EMT reimported through OpenKIM gives the right results.
-        atoms_kim = bulk(element).repeat(size)
+        atoms_kim = FaceCenteredCubic(size=(10,10,10), symbol='Cu')
         #atoms_kim = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]],
         #                    size=(30, 30, 30),
         #                    symbol="Cu")
         natoms = len(atoms_kim)
         atoms_kim.set_pbc(pbc)
         r = atoms_kim.get_positions()
         r.flat[:] += 0.1 * np.sin(np.arange(3*natoms))
         atoms_kim.set_positions(r)
         atoms_emt = atoms_kim.copy()
-        try:
-            kim = OpenKIMcalculator(openkimmodel % (element, shortkimid[element]))
-        except AsapError as oops:
-           if oops.args[0].startswith('Failed to initialize OpenKIM model'):
-               print("OpenKIM model {} not installed - skipping test.".format(
-                   openkimmodel % (element, shortkimid[element])))
-               continue
-           else:
-               raise   # Something else went wrong.
+        kim = OpenKIMcalculator(openkimmodel, allowed=nbltype)
         emt = EMT()
         emt.set_subtractE0(False)
         atoms_kim.set_calculator(kim)
         atoms_emt.set_calculator(emt)
         ek = atoms_kim.get_potential_energy()
         ee = atoms_emt.get_potential_energy()
         ReportTest(txt+"Total energy", ek, ee, 1e-8)
@@ -72,19 +56,20 @@
             ReportTest(txt+"Energy of atom %i" % (i,), ek[i], ee[i], 1e-8)
         fk = atoms_kim.get_forces()
         fe = atoms_emt.get_forces()
         n = 0
         for i in range(0, natoms, step):
             n = (n + 1) % 3
             ReportTest(txt+"Force(%i) of atom %i" % (n, i), fk[i, n], fe[i, n], 1e-8)
-        sk = atoms_kim.get_stress(**stresshack)
-        se = atoms_emt.get_stress(**stresshack)
+        sk = atoms_kim.get_stress()
+        se = atoms_emt.get_stress()
         for i in range(6):
             ReportTest(txt+"Stress(%i)" % (i,), sk[i], se[i], 1e-8)
-        sk = atoms_kim.get_stresses(**stresshack)
-        se = atoms_emt.get_stresses(**stresshack)
+        sk = atoms_kim.get_stresses()
+        se = atoms_emt.get_stresses()
         for i in range(0, natoms, step):
             n = (n + 1) % 6
             # Volume per atom is not defined the same way: greater tolerance needed
             ReportTest(txt+"Stress(%i) of atom %i" % (n, i), sk[i, n], se[i, n], 1e-3)
+
     
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/OpenKIM_modelname.py` & `asap3-3.9.6/Test/OpenKIM_modelname.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import print_function
 import os
 
-openkimmodel = "EMT_Asap_Standard_JacobsenStoltzeNorskov_1996_AlAgAuCuNiPdPt__MO_115316750986_001"
+openkimmodel = "EMT_Asap_Standard_Jacobsen_Stoltze_Norskov_AlAgAuCuNiPdPt__MO_118428466217_002"
 
 if 'ASAP_KIM_DIR' in os.environ:
     _d = os.path.join(os.environ['ASAP_KIM_DIR'], 'src/models')
 elif 'ASAP_KIM_LIB' in os.environ:
-    _d  = os.path.join(os.environ['ASAP_KIM_LIB'], 'kim-api/models')
+    _d  = os.path.join(os.environ['ASAP_KIM_LIB'], 'kim-api-v1/models')
 elif 'KIM_HOME' in os.environ:
-    _d  = os.path.join(os.environ['KIM_HOME'], 'lib/kim-api/models')
+    _d  = os.path.join(os.environ['KIM_HOME'], 'lib/kim-api-v1/models')
 else:
     _d = None
 
-if _d is not None and os.path.exists(_d):
+if _d is not None:
     openkimmodels = [x for x in os.listdir(_d) if os.path.isdir(os.path.join(_d,x))]
     openkimmodels.sort()
 else:
     openkimmodels = []
     
 if __name__ == "__main__":
     print(openkimmodels)
```

### Comparing `asap3-3.13.1/Test/PBCwrap.py` & `asap3-3.9.6/Test/PBCwrap.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 """Check that energy is correct even after wrapping through periodic boundary conditions.
 """
 from __future__ import print_function
 
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3 import *
 from asap3.testtools import *
-from numpy.random.mtrand import RandomState
-import pickle
-
-random = RandomState()
-with open("PBCwrap-rng.pickle", "wb") as pfile:
-    pickle.dump(random, pfile)
+import random
 
 ref_atoms = FaceCenteredCubic(size=(7,7,7), symbol="Cu", pbc=(True, False, True))
 ref_atoms.set_calculator(EMT())
 
 ref_energy = ref_atoms.get_potential_energy()
 ref_energies = ref_atoms.get_potential_energies()
 ref_forces = ref_atoms.get_forces()
```

### Comparing `asap3-3.13.1/Test/Potentials.py` & `asap3-3.9.6/Test/Potentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,42 +2,31 @@
 # Testing various potentials.
 
 from asap3 import *
 from asap3.md.verlet import VelocityVerlet
 from asap3.EMT2013Parameters import sihb_PtY_parameters
 from ase.lattice.cubic import *
 from ase.lattice.compounds import *
-try:
-    from ase.data import atomic_masses_legacy
-except ImportError:
-    atomic_masses_legacy = None
 from numpy import *
 from asap3.testtools import ReportTest
 try:
     import potResults
 except ImportError:
     resultfail = True
 else:
     resultfail = False
 import os
 
-if getattr(Atoms, '_ase_handles_dynamic_stress', False):
-    stresshack = {'include_ideal_gas': True}
-else:
-    stresshack = {}
-
 timeunit = 1.018047e-14             # Seconds
 femtosecond = 1e-15 / timeunit      # Femtosecond in atomic units
 
 print_version(1)
 
 
 def dotest(atoms, nsteps, ampl, name):
-    if atomic_masses_legacy is not None:
-        atoms.set_masses(atomic_masses_legacy[atoms.numbers])
     print("Potential energy", atoms.get_potential_energy() / len(atoms))
     r = atoms.get_positions()
     r.flat[:] += ampl * sin(arange(3*len(atoms)))
     atoms.set_positions(r)
     print("Potential energy", atoms.get_potential_energy() / len(atoms))
 
     print("Running Verlet dynamics (%s)" % (name,))
@@ -45,15 +34,15 @@
     etot1 = (atoms.get_potential_energy() + atoms.get_kinetic_energy())
     dyn.run(nsteps)
     etot2 = (atoms.get_potential_energy() + atoms.get_kinetic_energy())
     ReportTest(("Energy conservation (%s)" % (name,)), etot1, etot2, 1.0)
     print(etot1, etot2)
 
     epot = atoms.get_potential_energies()
-    stress = atoms.get_stresses(**stresshack)
+    stress = atoms.get_stresses()
     if firsttime:
         print("Reporting energies and stresses")
         e = []
         s = []
         j = 0
         for i in range(0, len(atoms), 100):
             e.append(epot[i])
```

### Comparing `asap3-3.13.1/Test/RDF.py` & `asap3-3.9.6/Test/RDF.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/RDF2.py` & `asap3-3.9.6/Test/RDF2.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/RawRDF.py` & `asap3-3.9.6/Test/RawRDF.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/RawRDF2.py` & `asap3-3.9.6/Test/RawRDF2.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/SizeConsist_EMT.py` & `asap3-3.9.6/Test/SizeConsist_EMT.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/SizeConsist_EMT2013.py` & `asap3-3.9.6/Test/SizeConsist_EMT2013.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/SizeConsist_LeftHand.py` & `asap3-3.9.6/Test/SizeConsist_LeftHand.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/SizeConsist_OpenKIM.py` & `asap3-3.9.6/Test/SizeConsist_OpenKIM.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 from asap3 import *
 from numpy import *
 from asap3.testtools import ReportTest
 from ase.lattice.cubic import *
 from OpenKIM_modelname import openkimmodel
 
 element = 'Au'
+if OpenKIMsupported:
+    sizes = arange(10,0,-1)
+    pbc_candidates = ["NEIGH_RVEC_H", 
+                      "NEIGH_PURE_H",
+                      "NEIGH_RVEC_F", 
+                      "NEIGH_PURE_F",
+                      ]
+else:
+    sizes = []
+    pbc_candidates = []
 
 energy = None
 force = None
 
-if OpenKIMsupported:
-    sizes = arange(10,0,-1)
+for nbl in pbc_candidates:
     for s in sizes:
         atoms = FaceCenteredCubic(symbol=element, size=(s,s,s), pbc=True)
         r = atoms.get_positions()
         for i in range(0, len(r), 4):
             r[i][0] += 0.1
         atoms.set_positions(r)
-        try:
-            atoms.set_calculator(OpenKIMcalculator(openkimmodel))
-        except AsapError as oops:
-            if oops.args[0].startswith('Failed to initialize OpenKIM model'):
-                print("OpenKIM model {} not installed - skipping test.".format(openkimmodel))
-                break
-            else:
-                raise
+        atoms.set_calculator(OpenKIMcalculator(openkimmodel, allowed=nbl))
         e = atoms.get_potential_energy() / len(atoms)   
         print("%5i atoms: E = %.5f eV/atom" % (len(atoms), e))
         if energy is None:
             energy = e
         else:
             ReportTest("Energy for size %i (%i atoms)" % (s, len(atoms)),
                        e, energy, 1e-8)
```

### Comparing `asap3-3.13.1/Test/SpecialEMT.pickle` & `asap3-3.9.6/Test/SpecialEMT.pickle`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/SpecialEMT.py` & `asap3-3.9.6/Test/SpecialEMT.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 from ase.lattice.compounds import *
 
 print_version(1)
 datafile = "SpecialEMT.pickle"
 CuMgdat = "../doc/EMT-MgCu-glass.dat"
 CuZrdat = "../doc/EMT-CuZr-glass.dat"
 
-picklehack = {'encoding': 'latin1'}
+if sys.version_info[0] >= 3:
+    picklehack = {'encoding': 'latin1'}
+else:
+    picklehack = {}
     
 if len(sys.argv) > 1:
     if len(sys.argv) == 2 and sys.argv[1] == "init":
         init = True
     else:
         print(__doc__, file=sys.stderr)
         sys.exit(1)
```

### Comparing `asap3-3.13.1/Test/StdParamProv.py` & `asap3-3.9.6/Test/StdParamProv.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Stress.py` & `asap3-3.9.6/Test/Stress.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 """
 from __future__ import print_function
 
 from StressModule import *
 from ase import data, Atoms
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.md.verlet import VelocityVerlet
+from asap3.md.langevin import Langevin
 
 defaultstrains = 0.01 * np.array((-1, -0.75, -0.5, -0.25, 0.0,
                                          0.25, 0.5, 0.75, 1.0))
                                        
 book = {}
 book['Cu'] = {"bookbulk": (134.3, 133.99),
               "bookc11": (168.3, 171.65),
@@ -81,12 +82,12 @@
     ReportTest("Number of atoms", len(initial), 4000, 0)
     atoms = Atoms(initial)
     if symb.find("Rasmussen") >= 0:
         print("Using the special EMT parameters by T. Rasmussen")
         atoms.set_calculator(EMT(EMTRasmussenParameters()))
     else:
         atoms.set_calculator(EMT())
-    atoms.set_momenta(np.zeros((len(atoms),3), float))
+    atoms.set_momenta(np.zeros((len(atoms),3), np.float))
     findlatticeconst(atoms, latconst)
     elasticconstants(atoms, symb, **book[symb])
 
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/StressCrash.py` & `asap3-3.9.6/Test/StressCrash.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,68 +2,63 @@
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.testtools import ReportTest
 from asap3.md.velocitydistribution import *
 
 #set_verbose(1)
 
-if getattr(Atoms, '_ase_handles_dynamic_stress', False):
-    stresshack = {'include_ideal_gas': True}
-else:
-    stresshack = {}
-
 atoms = FaceCenteredCubic(directions=((1,0,0), (0,1,0), (0,0,1)),
                           size=(15,15,15), symbol="Cu", pbc=True)
 atoms.set_calculator(EMT())
 
 atoms.get_forces()
 atoms.get_forces()
-MaxwellBoltzmannDistribution(atoms, temperature_K=300)
+MaxwellBoltzmannDistribution(atoms, 300 * units.kB)
 atoms.get_forces()
 atoms.get_forces()
 
 atoms = FaceCenteredCubic(directions=((1,0,0), (0,1,0), (0,0,1)),
                           size=(15,15,15), symbol="Cu", pbc=True)
 atoms.set_calculator(EMT())
-s = atoms.get_stress(**stresshack)
+s = atoms.get_stress()
 print()
 print("Stress:", s)
-s = atoms.get_stress(**stresshack)
+s = atoms.get_stress()
 print()
 print("Stress:", s)
-MaxwellBoltzmannDistribution(atoms, temperature_K=300)
-s = atoms.get_stress(**stresshack)
+MaxwellBoltzmannDistribution(atoms, 300 * units.kB)
+s = atoms.get_stress()
 print()
 print("Stress:", s)
-s = atoms.get_stress(**stresshack)
+s = atoms.get_stress()
 print()
 print("Stress:", s)
-MaxwellBoltzmannDistribution(atoms, temperature_K=300)
-s = atoms.get_stress(**stresshack)
+MaxwellBoltzmannDistribution(atoms, 300 * units.kB)
+s = atoms.get_stress()
 print()
 print("Stress:", s)
-s = atoms.get_stress(**stresshack)
+s = atoms.get_stress()
 print()
 print("Stress:", s)
 
 atoms = FaceCenteredCubic(directions=((1,0,0), (0,1,0), (0,0,1)),
                           size=(15,15,15), symbol="Cu", pbc=True)
 atoms.set_calculator(EMT())
-s = atoms.get_stress(**stresshack)
+s = atoms.get_stress()
 atoms.get_forces()
 atoms.get_forces()
-MaxwellBoltzmannDistribution(atoms, temperature_K=300)
+MaxwellBoltzmannDistribution(atoms, 300 * units.kB)
 atoms.get_forces()
 atoms.get_forces()
 
 atoms = FaceCenteredCubic(directions=((1,0,0), (0,1,0), (0,0,1)),
                           size=(15,15,15), symbol="Cu", pbc=True)
 atoms.set_calculator(EMT())
 atoms.get_stresses()
 atoms.get_stresses()
-MaxwellBoltzmannDistribution(atoms, temperature_K=300)
+MaxwellBoltzmannDistribution(atoms, 300 * units.kB)
 atoms.get_stresses()
 atoms.get_stresses()
 
 print()
 print()
 print("No crash: Test passes succesfully!")
```

### Comparing `asap3-3.13.1/Test/StressModule.py` & `asap3-3.9.6/Test/StressModule.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 from __future__ import print_function
 
 import numpy as np
 import sys
 from asap3 import *
 from asap3.testtools import ReportTest
 
-
-if getattr(Atoms, '_ase_handles_dynamic_stress', False):
-    stresshack = {'include_ideal_gas': True}
-else:
-    stresshack = {}
-
+# When not imported as a module, the following are imported later:
+#from Setup.Lattice.FCC111Ortho import *
+#from Structures.ChemicalElements import Copper, Silver
+#import Structures.ChemicalElements.AtomicWeight
+#import Structures.ChemicalElements.CrystalStructure
+#from Structures.IonDynamics import VelocityVerlet, Langevin
 
 defaultstrains = 0.01 * np.array((-1, -0.75, -0.5, -0.25, 0.0,
                                          0.25, 0.5, 0.75, 1.0))
 
 def polynomialLeastSquaresFit(parameters, data, max_iterations=None,
                               stopping_limit = 0.0001):
     """Least-square fit to a polynomial.
@@ -75,25 +75,25 @@
     """
     energies = []
     stresses = []
     basis = atoms.get_cell()
     vol = np.linalg.det(basis)
     for epsilon in strains:
         if shear:
-            adjustment = np.zeros((3,3), float)
+            adjustment = np.zeros((3,3), np.float)
             for idx in indices:
                 adjustment[idx[0]] += idx[2] * epsilon * basis[idx[1]]
             atoms.set_cell(adjustment + basis, scale_atoms=True)
         else:
-            scaling = np.ones((3,3), float)
+            scaling = np.ones((3,3), np.float)
             for idx in indices:
                 scaling[idx[0]] += idx[1]*epsilon
             atoms.set_cell(scaling * basis, scale_atoms=True)
         energy = atoms.get_potential_energy()
-        stress = atoms.get_stress(**stresshack)
+        stress = atoms.get_stress()
         #print ""
         #print epsilon, energy/len(atoms)
         #print stress
         energies.append((epsilon, energy/vol))
         stresses.append((epsilon,) + tuple(stress))
     atoms.set_cell(basis, scale_atoms=True)
     energies = np.array(energies)
```

### Comparing `asap3-3.13.1/Test/Subset.py` & `asap3-3.9.6/Test/Subset.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/TestAll.py` & `asap3-3.9.6/Test/TestAll.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 A simple test script.
 
 Runs and times all scripts named ``*.py``.  The tests that execute
 the fastest will be run first.
 """
+from __future__ import print_function
 
-#SBATCH --partition=xeon8
-#SBATCH -N 1
-#SBATCH -n 1
-#SBATCH --time=0:30:00
-#SBATCH --mem=2G
-#SBATCH --output=Test-%J.out
+#PBS -m ae
+#PBS -q medium
+
+## Tell asap-qsub that there is per default no threading.
+#ASAP N
 
 import glob
 import time
 import pickle
 import sys
 import gc
 try:
     import StringIO
 except ImportError:
     # Python 3?
     import io as StringIO
 from optparse import OptionParser
-import os
 import asap3
+import os
 from ase.parallel import paropen
 
 from asap3.mpi import world
 master = world.rank == 0
 
 
 if master:
@@ -36,43 +36,29 @@
     print("*** Running ASAP Test Suite ***")
     print("")
     asap3.print_version(1)
     
 brokentests = [
                'PrintMemory.py',  # Not really broken, but prints to stderr
                'EMTleak.py',      # Prints to stderr
+               'Exception.py',    # Does not work with testsuite.
                # REALLY BROKEN TESTS
                'BrennerNanotube.py',  # Leaks memory (bug in numpy)
                'BrennerStress.py',    # Must be completed.
                'OpenKIM_AllModels.py',  # Tests the models, not Asap.  Some fail.
                'RDF2.py',
                'Hydrocarbons.py',
                'FieldPlotter.py',    # Fails on machines without gs or netpbm
                'bundleTrajPreserveZ.py',  # Fails on buildbot due to old ASE.
-               'ConstraintInTraj.py',
-               'NotImplemented.py',  # Fails with newer ASE.
                ]
 
-slowtests = [
-    'TinyLangevin.py',
-    'BrennerPullNanotube.py',
-    'Langevin.py',
-    'CNAleak.py',
-    'NbCellLocator.py',
-    'NPT.py',
-    'Berendsen.py',
-    'parallelLennardJones.py', 
-    'parallelLangevin.py',
-    'parallelLongVerlet.py',
-    'splitBundleTrajectories.py',
-    'parallelFixatomTemperature.py',
-    'parallelNPT.py',
-    'parallelConstraints.py',
-    'parallelOpenKIM_EMT.py',
-    ]
+slowtests = ['HooverNPT.py', 'HooverNPTtraj.py', 'Langevin.py',
+             'LongLangevin.py', 'TinyLangevin.py',
+             'parallelLennardJones.py',
+             'parallelLangevin.py', 'parallelLongVerlet.py']
 
 stdout = sys.stdout
 stderr = sys.stderr
 if not master:
     stdout = sys.stdout = open(("TestAll-proc%d.out" % (world.rank)), "w")
 
 parser = OptionParser(usage='%prog [options] [tests]',
@@ -103,18 +89,14 @@
                   action='store_true',
                   help='Run with threading enabled (4 threads forced).')
 
 parser.add_option('-v', '--view-output',
                   action='store_true',
                   help="View output of all tests instead of redirecting them.")
 
-parser.add_option('-L', '--leaktest',
-                  action='store_true',
-                  help="Enable leak testing.")
-
 options, tests = parser.parse_args()
 
 # Clear the arguments, so we do not trouble the tests.
 del sys.argv[1:]
 
 if options.parallel:
     path = 'parallel/'
@@ -165,15 +147,15 @@
     tests = [(t, test) for t, test in tests if t == 0.0]
 
 L = max([len(test) for told, test in tests])
 print('-----------------------------------------------------------------')
 print(' test', ' ' * (L - 4), 'result      time (old)')
 print('-----------------------------------------------------------------')
 
-leaktest = options.leaktest
+leaktest = True
 garbage = []
 failed = []
 # Do tests:
 for told, test in tests:
     
     if not options.view_output:
         sys.stdout = StringIO.StringIO()
@@ -268,11 +250,10 @@
 
 # Report the error to build bot.
 failedname = "TestAll-failed.txt"
 if len(failed):
     failedfile = paropen(failedname, "w")
     failedfile.write(str(len(failed))+'\n')
     failedfile.close()
-    sys.exit(1)
 else:
-    if os.path.exists(failedname) and master:
+    if os.path.exists(failedname):
         os.remove(failedname)
```

### Comparing `asap3-3.13.1/Test/Timing/BigTiming.py` & `asap3-3.9.6/Test/Timing/Timing_OpenKIM.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 #! /usr/bin/env python
 
-#PBS -N BigTiming
+#PBS -N Timing
 #PBS -l nodes=1:ppn=4:opteron285
 #PBS -q small
 
 from __future__ import print_function
 from numpy import *
 from asap3 import *
 from asap3.md.verlet import VelocityVerlet
 from asap3.md.langevin import Langevin
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.timing import report_timing
-from asap3.memory import get_max_memory
-import sys, pickle, time, subprocess, os, re
+import sys, pickle, time, commands, os, re
 import numpy as np
 from asap3.testtools import ReportTest
 
 # cpu time:  time.clock().   Wall clock time: time.time()
 
 #Verbose(1)
 
-print_version(1)
-
 usethread = (len(sys.argv) > 1 and
              (sys.argv[1] == "-t" or sys.argv[1] == "-T"))
 if usethread:
     if sys.argv[1] == "-t":
         AsapThreads()
     else:
         AsapThreads(4)
 
-host = subprocess.check_output("hostname").decode('utf-8').strip()
-
+host = commands.getoutput("hostname")
 timesteps = 25
 if usethread:
-    dbfilename = "timing-thread-big.dat"
-    logfilename = "timing-thread-big.log"
+    dbfilename = "timing-thread.dat"
+    logfilename = "timing-thread.log"
 else:
-    dbfilename = "timing-big.dat"
-    logfilename = "timing-big.log"
-selfcheckfilename = "timing-selfcheck-big.dat"
+    dbfilename = "timing.dat"
+    logfilename = "timing.log"
+selfcheckfilename = "timing-selfcheck.dat"
 asapversion = get_version()
 when = time.strftime("%a %d %b %Y %H:%M", time.localtime(time.time()))
 
 randomstate = "randomstate.pickle"
 if os.path.isfile(randomstate):
     np.random.set_state(pickle.load(open(randomstate, "rb")))
 else:
@@ -66,33 +62,36 @@
 else:
     fullhost = host
 print("Current time is "+when)
 print("")
 
 print("Preparing system")
 initial = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]],
-                            size=(70, 70, 70),
+                            size=(30, 30, 30),
                             symbol="Cu")
-ReportTest("Number of atoms", len(initial), 1372000, 0)
+ReportTest("Number of atoms", len(initial), 108000, 0)
 r = initial.get_positions()
 r.flat[:] += 0.14 * sin(arange(3*len(initial)))
 initial.set_positions(r)
 
 print("Running self-test.")
 atoms = Atoms(initial)
-atoms.set_calculator(EMT())
+#atoms.set_calculator(EMT())
+atoms.set_calculator(OpenKIMcalculator('EMT_Asap_Standard_AlAgAuCuNiPdPt__MO_118428466217_000'))
 e = atoms.get_potential_energies()
 f = atoms.get_forces()
 if os.access(selfcheckfilename, os.F_OK):
     olde, oldf = pickle.load(open(selfcheckfilename, "rb"))
     de = max(fabs(e - olde))
     df = max(fabs(f.flat[:] - oldf.flat[:]))
     print("Maximal deviation:  Energy", de, "  Force", df)
     ReportTest("Max force error", df, 0.0, 1e-11)
     ReportTest("Max energy error", de, 0.0, 1e-11)
+    print(e[:20])
+    print(olde[:20])
     del olde, oldf
 else:
     print("WARNING: No self-check database found, creating it.")
     pickle.dump((e, f), open(selfcheckfilename, "wb"))
 del e,f,atoms
 
 ReportTest.Summary(exit=1)
@@ -106,15 +105,14 @@
 startcpu, startwall = time.clock(), time.time()
 dynamics.run(timesteps)
 
 vcpu, vwall = time.clock() - startcpu, time.time() - startwall
 vfraction = vcpu/vwall
 sys.stderr.write("\n")
 print("Verlet dynamics done.")
-atoms.get_calculator().print_memory()
 del dynamics, atoms
 
 print("Preparing to run Langevin dynamics.")
 atoms = Atoms(initial)
 atoms.set_calculator(EMT())
 dynamics = Langevin(atoms, 5*units.fs, 400*units.kB, 0.001)
 
@@ -122,15 +120,14 @@
 startcpu, startwall = time.clock(), time.time()
 dynamics.run(timesteps)
 
 lcpu, lwall = time.clock() - startcpu, time.time() - startwall
 lfraction = lcpu/lwall
 sys.stderr.write("\n")
 print("Langevin dynamics done.")
-atoms.get_calculator().print_memory()
 del dynamics, atoms
 
 print("")
 print("")
 print("TIMING RESULTS:")
 print("Verlet:   CPU time %.2fs  Wall clock time %.2fs (%.0f%%)" % (vcpu, vwall, vfraction * 100))
 print("Langevin: CPU time %.2fs  Wall clock time %.2fs (%.0f%%)" % (lcpu, lwall, lfraction * 100))
@@ -195,22 +192,18 @@
     if founddb:
         os.rename(dbfilename, bakfilename)
     os.rename(newfilename, dbfilename)
 
 now=time.strftime("%Y/%m/%d %H:%M")
 version = asapversion.split()[2]
 compiler = asapversion.split("'")[1]
-logline = ( "%-20s %s tot=%-6.2f  %6.2f %6.2f %-2.0f  %6.2f %6.2f %-2.0f  mem=%.0f MB  ver %s %s"
+logline = ( "%-20s %s tot=%-6.2f  %6.2f %6.2f %-2.0f  %6.2f %6.2f %-2.0f  ver %s %s"
             % (fullhost[:20], now, vcpu+lcpu, vcpu, vwall, vfraction*100,
-               lcpu, lwall, lfraction*100, get_max_memory(),
-               version, compiler))
+               lcpu, lwall, lfraction*100, version, compiler))
 print("\nLog line:")
 print(logline)
 
 logfile = open(logfilename, "a")
 logfile.write(logline+"\n")
 logfile.close()
 
 report_timing()
-
-print("Max memory:", get_max_memory())
-
```

### Comparing `asap3-3.13.1/Test/Timing/MonteCarloTiming.py` & `asap3-3.9.6/Test/Timing/MonteCarloTiming.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def MakeSystem(size, element, perturbation):
     lc = data.reference_states[data.atomic_numbers[element]]['a'] / 2.0**(1.0/3.0)
     
     atoms = MonteCarloAtoms(SimpleCubic(directions=((1,0,0),(0,1,0),(0,0,1)),
                                         size=size, symbol=element,
                                         latticeconstant=lc,
                                         pbc=True))
-    rs = atoms.get_scaled_positions(wrap=True)
+    rs = atoms.get_scaled_positions()
     atoms.set_scaled_positions(0.5 * (rs + rs*rs))
     r = atoms.get_positions()
     dr = perturbation * random.standard_normal(r.shape)
     atoms.set_positions(r + dr)
     return atoms
 
 
@@ -63,15 +63,15 @@
             de = 500.0*kT
         if (de > 0.0 and random.random() > exp(-de/kT)):
             atom.set_position(oldpos)
             nrej = nrej + 1
         else:
             e = newe
     tcpu, twall = time.clock() - startcpu, time.time() - startwall
-    atoms.wrap()
+    atoms.set_scaled_positions(atoms.get_scaled_positions())
     #p2 = RasMol(atoms.Repeat((2,2,2)))
     pc = 100.0 * tcpu / twall
     timing = 1e6 * tcpu / nsteps[i]
 
     print()
     print("Acceptance ratio:", 100.0 * (nsteps[i]-nrej) / nsteps[i])
     print("Energy change:", atoms.get_potential_energy() - eorig, "eV")
```

### Comparing `asap3-3.13.1/Test/Timing/Morse.py` & `asap3-3.9.6/Test/Timing/Morse.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/OfficialTiming.py` & `asap3-3.9.6/Test/Timing/OfficialTiming.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/OpenKIM_MemLeak.py` & `asap3-3.9.6/Test/Timing/OpenKIM_MemLeak.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/OpenKIM_ParTiming.py` & `asap3-3.9.6/Test/Timing/OpenKIM_ParTiming.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/OpenKIM_Profiling.py` & `asap3-3.9.6/Test/Timing/OpenKIM_Profiling.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/ParallelTiming.py` & `asap3-3.9.6/Test/Timing/ParallelTiming.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,23 @@
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.testtools import ReportTest
 from asap3.md.velocitydistribution import MaxwellBoltzmannDistribution
 from asap3 import mpi
 from asap3.md.npt import NPT
 from ase import units
-from io import StringIO
+from StringIO import StringIO
 import sys
-from subprocess import getoutput
+import commands
 import time
 
-possibleLayouts = [(1,1,2), (1,2,2), (2,2,2), (2,2,3), (2,2,4), (2,3,3), 
-                   (2, 3, 4), (2, 4, 4), (2, 4, 5), (3,3,3), (3,3,4), (3,4,4), (4,4,4), 
-                   (4,4,5), (4,5,5), (4,6,6), (6,6,6)]
-systemSizes = [((6,6,7), 1500), ((13,14,14), 150), ((29,29,30), 15), 
-               ((63,63,63), 8)]
+possibleLayouts = [(1,1,2), (1,2,2), (2,2,2), (2,2,3), (2,2,4), (2,3,3),
+                   (3,3,3), (3,3,4), (3,4,4), (4,4,4), (4,4,5), (4,5,5),
+                   (4,6,6), (6,6,6)]
+systemSizes = [((6,6,7), 1500), ((13,14,14), 150), ((29,29,30), 15), ((63,63,63), 8)]
 ##systemSizes = [((6,6,7), 100), ((13,14,14), 10)]
 
 if len(sys.argv) > 1:
     postfix = "-" + sys.argv[1]
 else:
     postfix = ""
 logfilename = "paralleltiming%s.log" % (postfix,)
@@ -112,15 +111,15 @@
     dyn.run(50)
     if ismaster:
         print("Done.  Temperature =", temperature(atoms), \
               "K.  Number of atoms: ", len(atoms))
     return atoms
 
 
-host = getoutput("hostname")
+host = commands.getoutput("hostname")
 when = time.strftime("%a %d %b %Y %H:%M", time.localtime(time.time()))
 asapversion = get_version()
 
 random.seed([42+mpi.world.rank, 12345*mpi.world.rank])
 
 layouts = {}
 for l in possibleLayouts:
@@ -198,24 +197,24 @@
     atoms = MakeParallelAtoms(atoms, cpuLayout)
 
     # Run the parallel timings (big systems)
     MaxwellBoltzmannDistribution(atoms, 300 * units.kB)
     name = "Verlet%d-big" % (atomspercpu,)
     atoms.set_calculator(EMT())
     dyn = VelocityVerlet(atoms, 5*units.fs)
-    ParallelTiming(name, dyn.run, 4*steps, atoms.get_global_number_of_atoms(),
+    ParallelTiming(name, dyn.run, 4*steps, atoms.get_number_of_atoms(),
                    verlet, bigtable)
     name = "Langevin%d-big" % (atomspercpu,)
     dyn = Langevin(atoms, 5*units.fs, 300*units.kB, 0.001)
-    ParallelTiming(name, dyn.run, 4*steps, atoms.get_global_number_of_atoms(),
+    ParallelTiming(name, dyn.run, 4*steps, atoms.get_number_of_atoms(),
                    langevin, bigtable)
     #name = "NPT%d-big" % (atomspercpu,)
     #dyn = NPT(atoms, 5*units.fs, 300*units.kB, 0, 25*units.fs,
     #          (75*units.fs)**2 * 140*units.GPa)
-    #ParallelTiming(name, dyn.run, 4*steps, atoms.get_global_number_of_atoms(),
+    #ParallelTiming(name, dyn.run, 4*steps, atoms.get_number_of_atoms(),
     #               npt, bigtable)
 
     # Make parallel systems without repeating
     if ismaster:
         atoms = Atoms(positions=positions,
                       cell = basis,
                       pbc = (1,1,1))
@@ -232,24 +231,24 @@
         continue
 
     # Run the parallel timings (fast systems)
     MaxwellBoltzmannDistribution(atoms, 300 * units.kB)
     name = "Verlet%d-fast" % (atomspercpu,)
     atoms.set_calculator(EMT())
     dyn = VelocityVerlet(atoms, 5*units.fs)
-    ParallelTiming(name, dyn.run, 4*steps, atoms.get_global_number_of_atoms(),
+    ParallelTiming(name, dyn.run, 4*steps, atoms.get_number_of_atoms(),
                    verlet, fasttable)
     name = "Langevin%d-fast" % (atomspercpu,)
     dyn = Langevin(atoms, 5*units.fs, 300*units.kB, 0.001)
-    ParallelTiming(name, dyn.run, 4*steps, atoms.get_global_number_of_atoms(),
+    ParallelTiming(name, dyn.run, 4*steps, atoms.get_number_of_atoms(),
                    langevin, fasttable)
     #name = "NPT%d-fast" % (atomspercpu,)
     #dyn = HooverNPT(atoms, 5*units.fs, 300*units.kB, 0, 25*units.fs,
     #                (75*units.fs)**2 * 140*units.GPa)
-    #ParallelTiming(name, dyn.run, 4*steps, atoms.get_global_number_of_atoms(),
+    #ParallelTiming(name, dyn.run, 4*steps, atoms.get_number_of_atoms(),
     #               npt, fasttable)
 
 if ismaster:
     bigtable.write("\n")
     fasttable.write("\n")
     
 logger.close()
```

### Comparing `asap3-3.13.1/Test/Timing/ThreadForceTiming.py` & `asap3-3.9.6/Test/Timing/ThreadForceTiming.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/Timing.py` & `asap3-3.9.6/Test/Timing/Timing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 #! /usr/bin/env python
 
-#SBATCH --partition=xeon8
-#SBATCH -N 1
-#SBATCH -n 4
-#SBATCH --time=1:00:00
-#SBATCH --mem=2G
-#SBATCH --output=Timing-%J.out
+#PBS -N Timing
+#PBS -l nodes=1:ppn=4:opteron285
+#PBS -q small
 
+from __future__ import print_function
 from numpy import *
 from asap3 import *
 from asap3.md.verlet import VelocityVerlet
 from asap3.md.langevin import Langevin
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.timing import report_timing
 import sys, pickle, time, subprocess, os, re
 import numpy as np
 from asap3.testtools import ReportTest
 
-# cpu time:  time.perf_counter().   Wall clock time: time.time()
+# cpu time:  time.clock().   Wall clock time: time.time()
 
 #Verbose(1)
 
 print_version(1)
 
 usethread = (len(sys.argv) > 1 and
              (sys.argv[1] == "-t" or sys.argv[1] == "-T"))
 if usethread:
     if sys.argv[1] == "-t":
         AsapThreads()
     else:
         AsapThreads(4)
 
-host = subprocess.check_output("hostname").decode('utf-8').strip()
-
+host = str(subprocess.check_output("hostname"))
 timesteps = 25
 if usethread:
     dbfilename = "timing-thread.dat"
     logfilename = "timing-thread.log"
 else:
     dbfilename = "timing.dat"
     logfilename = "timing.log"
@@ -100,33 +97,33 @@
 
 print("Preparing to run Verlet dynamics.")
 atoms = Atoms(initial)
 atoms.set_calculator(EMT())
 dynamics = VelocityVerlet(atoms, 5*units.fs)
 
 print("Running Verlet dynamics.")
-startcpu, startwall = time.perf_counter(), time.time()
+startcpu, startwall = time.clock(), time.time()
 dynamics.run(timesteps)
 
-vcpu, vwall = time.perf_counter() - startcpu, time.time() - startwall
+vcpu, vwall = time.clock() - startcpu, time.time() - startwall
 vfraction = vcpu/vwall
 sys.stderr.write("\n")
 print("Verlet dynamics done.")
 del dynamics, atoms
 
 print("Preparing to run Langevin dynamics.")
 atoms = Atoms(initial)
 atoms.set_calculator(EMT())
-dynamics = Langevin(atoms, 5*units.fs, temperature_K=400, friction=0.001)
+dynamics = Langevin(atoms, 5*units.fs, 400*units.kB, 0.001)
 
 print("Running Langevin dynamics.")
-startcpu, startwall = time.perf_counter(), time.time()
+startcpu, startwall = time.clock(), time.time()
 dynamics.run(timesteps)
 
-lcpu, lwall = time.perf_counter() - startcpu, time.time() - startwall
+lcpu, lwall = time.clock() - startcpu, time.time() - startwall
 lfraction = lcpu/lwall
 sys.stderr.write("\n")
 print("Langevin dynamics done.")
 del dynamics, atoms
 
 print("")
 print("")
```

### Comparing `asap3-3.13.1/Test/Timing/TimingEMT2013.py` & `asap3-3.9.6/Test/Timing/TimingEMT2013.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/TimingLangevin.py` & `asap3-3.9.6/Test/Timing/TimingLangevin.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/Timing/TimingVerlet.py` & `asap3-3.9.6/Test/Timing/TimingVerlet.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/TinyLangevin.py` & `asap3-3.9.6/Test/TinyLangevin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 #! /usr/bin/env python
-#SBATCH --mail-type=FAIL
-#SBATCH --mail-user=schiotz@fysik.dtu.dk
-#SBATCH --partition=xeon16
-#SBATCH -N 1
-#SBATCH -n 1
-#SBATCH --time=00:30:00
-#SBATCH --job-name=tinylangevin
-
+#PBS -N TinyLangevin
+#PBS -q long
+#PBS -l nodes=1:opteron4
 
 """testLangevin.py - test the Langevin dynamics.
 
 Usage: python testLangevin.py
 
 Tests Langevin dynamics using the EMT Copper potential.
 """
@@ -26,15 +21,15 @@
 from ase import units
 from asap3.io import Trajectory
 
 nequil = 10000
 nequilprint = 25
 nsteps = 500000
 nprint = 250
-tolerance = 0.04
+tolerance = 0.01
 nminor = 25
 timestep = 5 * units.fs
 
 # Use Langevin from ASE if --ase argument is given
 if len(sys.argv) > 1 and sys.argv[1] == "--ase":
     print("--ase specified: Using unmodified ASE Langevin dynamics.")
     from ase.md.langevin import Langevin
@@ -60,43 +55,43 @@
     return params[0] * exp(-params[1] * x) + params[2]
 
 output =open("Langevin.dat", "w")
 
 results = []
 
 for temp, frict, fixcm in ((0.025, 0.001, True), (0.025, 0.0001, False),):
-    dyn = Langevin(atoms, timestep, temperature_K=temp/units.kB, friction=frict, fixcm=fixcm)
+    dyn = Langevin(atoms, timestep, temp, frict, fixcm=fixcm)
     traj = Trajectory("Langevin-{0}-{1}-{2}.traj".format(temp, frict, fixcm),
                       "w", atoms)
     print("")
     print("Testing Langevin dynamics with T = %f eV and lambda = %f" % (temp, frict))
     ekin = atoms.get_kinetic_energy()/len(atoms)
     print(ekin)
     output.write("%.8f\n" % ekin)
     temperatures = [(0, 2.0 / 3.0 * ekin)]
     a = 0.1
     b = frict
     c = temp
     print("Equilibrating ...")
     tstart = time.time()
-    for i in range(1,nequil+1):
+    for i in xrange(1,nequil+1):
         dyn.run(nminor)
         ekin = atoms.get_kinetic_energy() / len(atoms)
         if i % nequilprint == 0:
 
             print("%.6f  T = %.6f (goal: %f)" % \
                   (ekin, 2.0/3.0 * ekin, temp))
         output.write("%.8f\n" % ekin)
     tequil = time.time() - tstart
     print("This took %s minutes." % (tequil / 60))
     output.write("&\n")
     temperatures = []
     print("Taking data")
     tstart = time.time()
-    for i in range(1,nsteps+1):
+    for i in xrange(1,nsteps+1):
         dyn.run(nminor)
         ekin = atoms.get_kinetic_energy() / len(atoms)
         temperatures.append(2.0/3.0 * ekin)
         if i % nprint == 0:
             tnow = time.time() - tstart
             tleft = (nsteps-i) * tnow / i
             print("%.6f    (time left: %.1f minutes)" % (ekin, tleft/60))
@@ -107,17 +102,18 @@
     mean = sum(temperatures) / len(temperatures)
     print("Mean temperature:", mean, "eV")
     print("")
     print("This test is statistical, and may in rare cases fail due to a")
     print("statistical fluctuation.")
     print("")
     expected = temp
+    if fixcm:
+        expected *= 7.0 / 8.0
     results.append((mean, (mean - expected)/expected))
     ReportTest("Mean temperature:", mean, expected, tolerance*temp)
 
 print("RESULTS:")
 for r in results:
     print("%.8f  %.8f" % r)
     
 output.close()
 
-ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/Trajectories.py` & `asap3-3.9.6/Test/Trajectories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import print_function
 from asap3 import *
 from asap3.md.verlet import VelocityVerlet
 from ase.lattice.cubic import FaceCenteredCubic
-#from asap3.io.trajectory import *
-from ase.io.trajectory import *
+from asap3.io.trajectory import *
 from ase.io import write
 from numpy import *
 import sys, os, time
 from asap3.testtools import ReportTest
 
 #DebugOutput("output.%d")
 print_version(1)
@@ -41,16 +40,14 @@
         i += 1
 
 initial = FaceCenteredCubic(size=(10,10,10), symbol="Cu", pbc=(1,0,0))
 
 
 atoms = initial.copy()
 atoms.set_calculator(EMT())
-atoms.get_potential_energy()
-atoms.get_forces()
 print("Writing trajectory")
 traj = Trajectory("traj1.traj", "w", atoms)
 traj.write()
 energies = maketraj(atoms, traj, 10)
 traj.close()
 
 print("Reading trajectory (recalculating energies)")
@@ -86,16 +83,16 @@
 print("Writing a trajectory without precalculated energies.")
 atoms = initial.copy()
 atoms.set_calculator(EMT())
 traj = Trajectory("traj3.traj", "w", atoms)
 traj.write()
 maketraj_no_e(atoms, traj, 10)
 traj.close()
-#traj = Trajectory("traj3.traj")
-#checktraj(traj, energies, recalc=False)
+traj = Trajectory("traj3.traj")
+checktraj(traj, energies, recalc=False)
 
 if delete:
     print("Deleting trajectory")
     os.unlink("traj1.traj")
     os.unlink("traj2.traj")
     os.unlink("traj3.traj")
```

### Comparing `asap3-3.13.1/Test/Verlet.py` & `asap3-3.9.6/Test/Verlet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 from __future__ import print_function
 from asap3 import *
 from numpy import *
 from pickle import load, dump
 from asap3.testtools import ReportTest
-import ase.data
 import sys
 
 timeunit = 1.018047e-14             # Seconds
 femtosecond = 1e-15 / timeunit      # Marginally different from units.fs
 
 print_version(1)
 
-picklehack = {'encoding': 'latin1'}
-if getattr(Atoms, '_ase_handles_dynamic_stress', False):
-    stresshack = {'include_ideal_gas': True}
+if sys.version_info[0] >= 3:
+    picklehack = {'encoding': 'latin1'}
 else:
-    stresshack = {}
+    picklehack = {}
 
-if hasattr(ase.data, 'atomic_masses_legacy'):
-    # Newer ASE
-    picklefile = "Verlet.pickle"
-else:
-    picklefile = "Verlet_legacymass.pickle"
-
-data = load(open(picklefile, "rb"), **picklehack)
+data = load(open("testVerlet.pickle", "rb"), **picklehack)
 init_pos = array(data["initial"])
 init_pos.shape = (-1,3)
 init_box = array(data["box"])
 init_box.shape = (3,3)
 atoms = Atoms(positions=init_pos, cell=init_box)
 atoms.set_atomic_numbers(47*ones((len(atoms),)))
 atoms.set_calculator(EMT())
@@ -47,13 +39,13 @@
         ReportTest("Energy conservation:", epot + ekin, etot, 0.001)
         
 final_pos = array(data["final"])
 diff = max(abs(atoms.get_positions().flat - final_pos))
 print("Maximal deviation of positions:", diff)
 ReportTest("Maximal deviation of positions", diff, 0, 1e-9)
 
-diff = max(abs(atoms.get_stresses(**stresshack).flat - array(data["stress"])))
+diff = max(abs(atoms.get_stresses().flat - array(data["stress"])))
 
 print("Maximal deviation of stresses:", diff)
 ReportTest("Maximal deviation of stresses", diff, 0, 1e-9)
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/Verlet_OpenKIM.py` & `asap3-3.9.6/Test/Verlet_OpenKIM.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,29 @@
 from __future__ import print_function
 from asap3 import *
+from pickle import *
 from numpy import *
-from pickle import load, dump
 from asap3.testtools import ReportTest
 from OpenKIM_modelname import openkimmodel
-import ase.data
 
 timeunit = 1.018047e-14             # Seconds
 femtosecond = 1e-15 / timeunit      # Marginally different from units.fs
 
 print_version(1)
 
-picklehack = {'encoding': 'latin1'}
-
-if hasattr(ase.data, 'atomic_masses_legacy'):
-    # Newer ASE
-    picklefile = "Verlet.pickle"
-else:
-    picklefile = "Verlet_legacymass.pickle"
-
 if OpenKIMsupported:
-    try:
-        calc = OpenKIMcalculator(openkimmodel)
-    except AsapError as oops:
-        if oops.args[0].startswith('Failed to initialize OpenKIM model'):
-            print("OpenKIM model {} not installed - skipping test.".format(openkimmodel))
-            calc = None
-        else:
-            raise
-
-    
-if OpenKIMsupported and calc is not None:
-    data = load(open(picklefile, "rb"), **picklehack)
+    data = load(open("testVerlet.pickle", "rb"))
     init_pos = array(data["initial"])
     init_pos.shape = (-1,3)
     init_box = array(data["box"])
     init_box.shape = (3,3)
     atoms = Atoms(positions=init_pos, cell=init_box)
     atoms.set_atomic_numbers(47*ones((len(atoms),)))
-    atoms.set_calculator(calc)
+    atoms.set_calculator(OpenKIMcalculator(openkimmodel))
+    
     dyn = VelocityVerlet(atoms, 2 * femtosecond)
     dyn.attach(MDLogger(dyn, atoms, '-', peratom=True), interval=5)
     
     etot = None
     
     for i in range(10):
         dyn.run(20)
```

### Comparing `asap3-3.13.1/Test/ase_emt.py` & `asap3-3.9.6/Test/ase_emt.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 
 elements = ("Ni", "Cu", "Pd", "Ag", "Pt")
 
 for e1 in elements:
     for e2 in elements:
         atoms = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]], size=(1,1,2),
                                   symbol=e1, pbc=(1,0,1), debug=0)
-        atoms.set_calculator(EMT_ASE(asap_cutoff=True))
+        atoms.set_calculator(EMT_ASE(fixed_cutoff=False))
         e_e1_ase = atoms.get_potential_energy()
         atoms.set_calculator(EMT_ASAP())
         e_e1_asap = atoms.get_potential_energy()
         natoms = len(atoms)
 
         print("{0} energy (ASE) \t{1:.5f}".format(e1, e_e1_ase/natoms))
         print("{0} energy (ASAP)\t{1:.5f}".format(e1, e_e1_asap/natoms))
 
         atoms = FaceCenteredCubic(directions=[[1,0,0],[0,1,0],[0,0,1]], size=(1,1,2),
                                   symbol=e2, pbc=(1,0,1), debug=0)
-        atoms.set_calculator(EMT_ASE(asap_cutoff=True))
+        atoms.set_calculator(EMT_ASE(fixed_cutoff=False))
         e_e2_ase = atoms.get_potential_energy()
         atoms.set_calculator(EMT_ASAP())
         e_e2_asap = atoms.get_potential_energy()
 
         print("{0} energy (ASE) \t{1:.5f}".format(e2, e_e2_ase/natoms))
         print("{0} energy (ASAP)\t{1:.5f}".format(e2, e_e2_asap/natoms))
 
         atoms = L1_2(directions=[[1,0,0],[0,1,0],[0,0,1]], size=(1,1,2),
                      symbol=(e1, e2), latticeconstant=3.95, pbc=(1,0,1), 
                      debug=0)
         
-        atoms.set_calculator(EMT_ASE(asap_cutoff=True))
+        atoms.set_calculator(EMT_ASE(fixed_cutoff=False))
         e_alloy_ase = atoms.get_potential_energy() - (2*e_e1_ase + 6*e_e2_ase)/8
         atoms.set_calculator(EMT_ASAP())
         e_alloy_asap = atoms.get_potential_energy() - (2*e_e1_asap + 6*e_e2_asap)/8
 
         print("Alloy energy (ASE) \t{0:.5f}".format(e_alloy_ase/natoms))
         print("Alloy energy (ASAP)\t{0:.5f}".format(e_alloy_asap/natoms))
         ReportTest("{0}{1}_3 alloy energy".format(e1, e2), e_alloy_ase, e_alloy_asap, 1e-4)
```

### Comparing `asap3-3.13.1/Test/parallel/Force1D.py` & `asap3-3.9.6/Test/parallel/Force1D.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/parallel/bundleTrajPreserveZ.py` & `asap3-3.9.6/Test/parallel/bundleTrajPreserveZ.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     atoms = initial.copy()
   
 check_z(atoms)
 
 if dosim:
     print("Simulation: create the bundle")
     # Give a momentum distribution likely to cause migration
-    MaxwellBoltzmannDistribution(atoms, temperature_K=5000)
+    MaxwellBoltzmannDistribution(atoms, 5000*units.kB)
     p = atoms.get_momenta()
     pz = p[10,2]
     p[:,2] += pz
 
     atoms.set_calculator(EMT())
     if isparallel:
         traj = BundleTrajectory("preservez.bundle", "w", atoms, split=True)
```

### Comparing `asap3-3.13.1/Test/parallel/emptyNode.py` & `asap3-3.9.6/Test/parallel/parallelLocalStructure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,85 @@
-"""
-Tests that Asap works in parallel simulations even if a process has no atoms.
-
-Name: emptyNode.py
-
-Description: Part of the Asap test suite.  Tests parallelization robustness.
-
-Usage: mpirun -np 4 asap-python emptyNode.py
-
-Expected result: The output should end with 'ALL TESTS SUCCEEDED'.
-"""
+"""Test local crystal structure analysis (CNA and Coordination number)."""
 from __future__ import print_function
 
-from ase.build import bulk
-from ase.lattice.cubic import FaceCenteredCubic
+from asap3 import *
+from asap3.analysis import FullCNA, RestrictedCNA, CoordinationNumbers
 from asap3.testtools import ReportTest
-from asap3 import MakeParallelAtoms, EMT
 from asap3.mpi import world
+from ase.lattice import bulk
 import numpy as np
-from ase.visualize import view
 
+debug = 0
+if debug == 1:
+    DebugOutput("parallel%d.log", nomaster=True)
+elif debug == 2:
+    time.sleep(world.rank)
+    print("PID:", os.getpid())
+    time.sleep(20)
+
+ismaster = world.rank == 0
+isparallel = world.size != 1
 if world.size == 1:
     cpulayout = None
 elif world.size == 2:
     cpulayout = [2,1,1]
 elif world.size == 3:
     cpulayout = [1,3,1]
 elif world.size == 4:
-    cpulayout = [2,2,1]
-
-def makesystem(delta):
-    atoms = FaceCenteredCubic("Cu", size=(15,15,15), pbc=False)
-    x = atoms.cell[0,0] / 2
-    y = atoms.cell[1,1] / 2
-    pos = atoms.get_positions()
-    keep = np.logical_or(pos[:,0] > x + delta, pos[:,1] > y + delta)
-    return atoms[keep]
+    cpulayout = [2,1,2]
 
-def distribute(atoms):
-    if world.rank != 0:
+for usepot in (True, False):
+    if ismaster:
+        atoms = bulk('Cu')
+        atoms = atoms.repeat((10, 10, 10))
+        if isparallel:
+            atoms = atoms.repeat(cpulayout)
+        del atoms[100]   #Create point defect
+    else:
         atoms = None
-    return MakeParallelAtoms(atoms, cpulayout)
-
-
-def testsystem(origatoms, label):
-    origatoms.set_calculator(None)
-    atoms = distribute(origatoms)
-    atoms.suppress_warning_noatoms = True   # Kill a warning on stderr
-    print("Number of atoms on process {}: {}".format(world.rank, len(atoms)))
-    atoms.set_calculator(EMT())
-    energy_par = atoms.get_potential_energy()
-
-    origatoms.set_calculator(EMT())
-    energy_ser = origatoms.get_potential_energy()
-
-    ReportTest(label+": Energy match", energy_par, energy_ser, 1e-6)
-
-a = makesystem(10.0)
-testsystem(a, "Large missing part on master")
-
-a.rotate(90, 'z', center='COU')
-testsystem(a, "Large missing part on slave")
-
-a = makesystem(1.0)
-testsystem(a, "Small missing part on master")
-
-a.rotate(90, 'z', center='COU')
-testsystem(a, "Small missing part on slave")
+    if isparallel:
+        atoms = MakeParallelAtoms(atoms, cpulayout)
+    natoms = atoms.get_number_of_atoms()
+    if usepot:
+        atoms.set_calculator(EMT())
+        atoms.get_potential_energy()
+    
+    print("Testing CNA")
+    RestrictedCNA(atoms)
+    t = atoms.get_tags()
+    counts = np.zeros(3, int)
+    for i in range(3):
+        counts[i] = (t == i).sum()
+    world.sum(counts)
+    
+    ReportTest("CNA: fcc atoms", counts[0], natoms-12, 0)
+    ReportTest("CNA: hcp atoms", counts[1], 0, 0)
+    ReportTest("CNA: other atoms", counts[2], 12, 0)
+    
+    print()
+    print("Testing coordination number")
+    t = CoordinationNumbers(atoms)
+    counts = np.zeros(20, int)
+    wanted = np.zeros(20, int)
+    wanted[11] = 12
+    wanted[12] = natoms - 12
+    for i in range(len(counts)):
+        counts[i] = (t == i).sum()
+    if isparallel:
+        world.sum(counts)
+    for i in range(len(counts)):
+        ReportTest("Coordination number {0}".format(i), counts[i], wanted[i], 0)
+        
+    print()
+    print("Testing Full CNA")
+    cnacalc = FullCNA(atoms)
+    cna = cnacalc.get_normal_cna()
+    print(cna[0])
+    ReportTest("Length of CNA vector", len(cna), len(atoms), 0)
+    for i in range(len(atoms)):
+        ReportTest("Number of CNA vectors (atom {0})".format(i), 
+                   sum(cna[i].values()), t[i], 0, silent=True)
+        if (t[i] == 12):
+            ReportTest("Number of 421 bonds (atom {0})".format(i),
+                       cna[i][(4,2,1)], 12, 0, silent=True)
+      
+ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/parallel/longMelting.py` & `asap3-3.9.6/Test/parallel/longMelting.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 def main(element, T_up, T_low, T_expect, bulkmodulus, makepot):
     def set_temp_fric(dyn, atoms):
         z = atoms.get_positions()[:,2]
         zmax = atoms.get_cell()[2,2]
         zmin = 0
         T = T_low + (T_up - T_low) * (z - zmin) / (zmax - zmin)
-        dyn.set_temperature(temperature_K=T)
+        dyn.set_temperature(T * units.kB)
 
     rnd = world.sum(random.randint(0,2**32)) # Insures the same number on all nodes.
     prefix = "melt-%s-%s" % (element, hex(rnd)[2:])
     if master:
         print("Using output directory", prefix)
         os.mkdir(prefix)
     else:
@@ -111,56 +111,52 @@
             time.sleep(1)
     if master:
         atoms = FaceCenteredCubic(symbol=element, size=size, pbc=(True, True, False))
         atoms.center(vacuum=10.0, axis=2)
     else:
         atoms = None
     atoms = MakeParallelAtoms(atoms, cpulayout1)
-    print(world.rank, '-', len(atoms), atoms.get_global_number_of_atoms())
+    print(world.rank, '-', len(atoms), atoms.get_number_of_atoms())
     atoms.set_calculator(makepot())
     #view(atoms)
     
-    dyn = Langevin(atoms, 5*units.fs, temperature_K=0.0, friction=friction)
+    dyn = Langevin(atoms, 5*units.fs, 0.0, friction)
     logger = MDLogger(dyn, atoms, prefix+'/Melt-phase1.log', stress=True, peratom=True)
     dyn.attach(logger, interval=100)
     set_temp_fric(dyn, atoms)
-    unstress = Inhomogeneous_NPTBerendsen(atoms, 50*units.fs, temperature_K=0,
-                                          pressure_au=0, taut=500*units.fs,
-                                          taup=500*units.fs,
-                                          compressibility_au=1/bulkmodulus)
+    unstress = Inhomogeneous_NPTBerendsen(atoms, 50*units.fs, 0, taup=500*units.fs,
+                                          compressibility=1/bulkmodulus)
     dyn.attach(unstress.scale_positions_and_cell, interval=10)
     #traj = PickleTrajectory("melting-phase1.traj", "w", atoms)
     fn1 = prefix + "/Melt-phase1.bundle" 
     if master:
         print("Opening file", fn1)
     traj = BundleTrajectory(fn1, "w", atoms, split=True)
     dyn.attach(traj, interval=500)
     
     therm = Thermometer(atoms, prefix+"/TempProfile-phase1.dat")
     dyn.attach(therm.update, interval=500)
     
-    for i in range(steps1 // 100):
+    for i in range(steps1 / 100):
         dyn.run(100)
         set_temp_fric(dyn, atoms)
     if master:
         print("Closing file", fn1)
     traj.close()
     del traj, atoms
     
     # Reread the bundle
     atoms = BundleTrajectory(fn1).get_atoms(-1, cpulayout2)
     atoms.set_calculator(makepot())
     dyn = VelocityVerlet(atoms, 5*units.fs)
     logger = MDLogger(dyn, atoms, prefix+'/PtMelt-phase2.log', stress=True, peratom=True)
-    dyn.attach(logger, interval=1000)  
-    unstress = Inhomogeneous_NPTBerendsen(atoms, 50*units.fs,
-                                          temperature_K=0,
-                                          pressure_au=0,
-                                          taup=5000*units.fs, taut=1000*units.fs,
-                                          compressibility_au=1/bulkmodulus)
+    dyn.attach(logger, interval=1000)
+    unstress = Inhomogeneous_NPTBerendsen(atoms, 50*units.fs, 0,
+                                          taup=5000*units.fs,
+                                          compressibility=1/bulkmodulus)
     dyn.attach(unstress.scale_positions_and_cell, interval=10)
     fn2 = prefix + "/Melt-phase2.bundle" 
     if master:
         print("Opening file", fn2)
     traj = BundleTrajectory(fn2, "w", atoms)
     dyn.attach(traj, interval=steps2/100)
     
@@ -186,10 +182,10 @@
     ReportTest.Summary()    
 
 if __name__ == '__main__':
     main(element = 'Pt',
          T_up = 2000.0,  #K
          T_low = 1000.0, #K
          T_expect = 1357, #K
-         bulkmodulus = 230.0 * units.GPa,  # Bulk modulus of Pt
+         bulkmodulus = 230.0e9 / 1.0e5,  # Bulk modulus of Pt in bar
          makepot = EMT
          )
```

### Comparing `asap3-3.13.1/Test/parallel/makeparallel.py` & `asap3-3.9.6/Test/parallel/makeparallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 if world.size == 1 or world.rank == 1:
     atoms = FaceCenteredCubic(symbol="Cu", size=(20,20,30))
 else:
     atoms = None
 
 if world.size > 1:
     atoms = MakeParallelAtoms(atoms, layout, distribute=False)
-    natoms = atoms.get_global_number_of_atoms()
+    natoms = atoms.get_number_of_atoms()
 else:
     natoms = len(atoms)
     
 report()
 
 print()
 print()
```

### Comparing `asap3-3.13.1/Test/parallel/migration.py` & `asap3-3.9.6/Test/parallel/migration.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,25 +28,24 @@
 else:
     atoms0 = None
     
 atoms0 = MakeParallelAtoms(atoms0, cpulayout)
 atoms0.set_calculator(pot())
 
 print("*********** FIRST FORCE CALCULATION ************", file=sys.stderr)
-print("len(atoms) =", len(atoms0), "   no. atoms =", atoms0.get_global_number_of_atoms(), file=sys.stderr)
+print("len(atoms) =", len(atoms0), "   no. atoms =", atoms0.get_number_of_atoms(), file=sys.stderr)
 f0 = atoms0.get_forces()
 perturbation = 0.01 * np.random.standard_normal(atoms0.get_positions().shape)
 r = atoms0.get_positions() + perturbation
 atoms0.set_positions(r)
 print("*********** SECOND FORCE CALCULATION ************", file=sys.stderr)
 
 f1 = atoms0.get_forces()
 
 print("*********** COPYING ATOMS **************", file=sys.stderr)
-#atoms0.set_calculator(None)  # Cannot copy parallel calculators
 atoms2 = ParallelAtoms(cpulayout, atoms0.comm, atoms0, distribute=False)
 atoms2.set_calculator(pot())
 print("*********** THIRD FORCE CALCULATION ************", file=sys.stderr)
 f2 = atoms2.get_forces()
 
 #maxdev = abs(f2 - f1).max()
 #print maxdev
```

### Comparing `asap3-3.13.1/Test/parallel/moveatoms.py` & `asap3-3.9.6/Test/parallel/moveatoms.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 #set_verbose(1)
 
 if isparallel:
     atoms = MakeParallelAtoms(atoms, cpulayout, distribute=False)
     atoms.ghosts["ID"] = zeros(0,int)
     print("Distributing")
     atoms.distribute()
-    nTotalAtoms = atoms.get_global_number_of_atoms()
+    nTotalAtoms = atoms.get_number_of_atoms()
 else:
     nTotalAtoms = len(atoms)
     atoms.arrays["ID"] = arange(nTotalAtoms)
 
 print("Setting potential")
 atoms.set_calculator(EMT())
```

### Comparing `asap3-3.13.1/Test/parallel/moveatomsLJ.py` & `asap3-3.9.6/Test/parallel/moveatomsLJ.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 #set_verbose(1)
 
 if isparallel:
     atoms = MakeParallelAtoms(atoms, cpulayout, distribute=False)
     atoms.ghosts["ID"] = zeros(0,int)
     print("Distributing")
     atoms.distribute()
-    nTotalAtoms = atoms.get_global_number_of_atoms()
+    nTotalAtoms = atoms.get_number_of_atoms()
 else:
     nTotalAtoms = len(atoms)
     atoms.arrays["ID"] = arange(nTotalAtoms)
 
 print("Setting potential")
 atoms.set_calculator(LennardJones([29], [0.15], [2.7], 2.7*1.9, True))
```

### Comparing `asap3-3.13.1/Test/parallel/parallelBundleTrajectories.py` & `asap3-3.9.6/Test/parallel/parallelBundleTrajectories.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     atoms = MakeParallelAtoms(initial, cpulayout)
 else:
     atoms = initial.copy()
     
 atoms.set_calculator(EMT())
 atoms.set_momenta(zeros((len(atoms), 3)))
 print("Writing trajectory")
-traj = BundleTrajectory("traj1.bundle", "w", atoms, singleprecision=False)
+traj = BundleTrajectory("traj1.bundle", "w", atoms)
 traj.write()
 energies = maketraj(atoms, traj, 10)
 traj.close()
 
 if ismaster:
     print("Reading trajectory (serial)")
     traj = BundleTrajectory("traj1.bundle")
```

### Comparing `asap3-3.13.1/Test/parallel/parallelChangeConstraints.py` & `asap3-3.9.6/Test/parallel/parallelConstraints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Test the FixAtoms constraint and the Subset filter."""
 from __future__ import print_function
 
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.md.velocitydistribution import MaxwellBoltzmannDistribution
 from asap3.md.verlet import VelocityVerlet
-from asap3.md.nvtberendsen import NVTBerendsen
 from asap3.constraints import Filter, FixAtoms
 from ase.constraints import FixAtoms as ASE_FixAtoms
 from asap3.testtools import ReportTest
 from asap3.mpi import world
 import numpy as np
 
 debug = 0
@@ -30,71 +29,72 @@
 elif world.size == 2:
     cpulayout = [2,1,1]
 elif world.size == 3:
     cpulayout = [1,3,1]
 elif world.size == 4:
     cpulayout = [2,1,2]
 
-def sanity(name, atoms):
-    initial = atoms.arrays['r_init']
-    final = atoms.get_positions()
-    fixed = atoms.get_tags().astype(bool)
-    
-    print(f"Sanity check, {name}:")
-    ok = (final == initial) + np.logical_not(fixed)[:,np.newaxis]
+if ismaster:
+    init = FaceCenteredCubic(size=(10,10,10), symbol='Cu', pbc=False)
+    z = init.get_positions()[:,2]
+    fixedatoms = np.less(z, 0.501*z.max())
+    print(len(init), sum(fixedatoms))
+    MaxwellBoltzmannDistribution(init, 6000*units.kB)
+    init.set_tags(fixedatoms)
+else:
+    init = None
+
+print()
+print("Running simulation with Filter")
+atoms1 = MakeParallelAtoms(init, cpulayout)
+atoms1.arrays['r_init'] = atoms1.get_positions()
+atoms1.set_calculator(EMT())
+atoms1a = Filter(atoms1, mask=np.logical_not(atoms1.get_tags()))
+
+dyn = VelocityVerlet(atoms1a, 3*units.fs)
+dyn.run(100)
+
+print()
+print("Running simulation with Asap's FixAtoms")
+atoms2 = MakeParallelAtoms(init, cpulayout)
+atoms2.arrays['r_init'] = atoms2.get_positions()
+atoms2.set_calculator(EMT())
+atoms2.set_constraint(FixAtoms(mask=atoms2.get_tags()))
+
+dyn = VelocityVerlet(atoms2, 3*units.fs)
+dyn.run(100)
+
+print()
+print("Running Langevin simulation with Asap's FixAtoms")
+atoms4 = MakeParallelAtoms(init, cpulayout)
+atoms4.arrays['r_init'] = atoms4.get_positions()
+atoms4.set_calculator(EMT())
+atoms4.set_constraint(FixAtoms(mask=atoms4.get_tags()))
+
+dyn = Langevin(atoms4, 3*units.fs, 3000*units.kB, 0.01)
+dyn.run(100)
+
+
+print()
+sanity = [[atoms1, "Verlet + Filter"],
+          [atoms2, "Verlet + Asap's FixAtoms"],
+          [atoms4, "Langevin + Asap's FixAtoms"],
+          ]
+for a, label in sanity:
+    print(world.rank, "Sanity check, %s:", (label,))
+    r_init = a.arrays['r_init']
+    ok = (a.get_positions() == r_init) + np.logical_not(a.get_tags())[:,np.newaxis]
     if ok.all():
-        print("  Stationary atoms have not moved: OK")
+        print(world.rank, "  Stationary atoms have not moved: OK")
     else:
-        raise RuntimeError(f"Stationary atoms have moved ({name})")
-    ok = (final != initial) + fixed[:,np.newaxis]
+        raise RuntimeError("Stationary atoms have moved (%s)" % (label,))
+    ok = (a.get_positions() != r_init) + a.get_tags()[:,np.newaxis]
     if ok.all():
-        print("  Mobile atoms have moved: OK")
+        print(world.rank, "  Mobile atoms have moved: OK")
     else:
-        raise RuntimeError(f"Mobile atoms have not moved ({name})")
-
-for dynamics in ("Verlet", "NVTBerendsen", "Langevin",):
+        raise RuntimeError("Mobile atoms have not moved (%s)" % (label,))
     
-    if ismaster:
-        size = 5 * np.array(cpulayout)
-        init = FaceCenteredCubic(size=size, symbol='Cu', pbc=False)
-        z = init.get_positions()[:,2]
-        fixedatoms = np.less(z, 0.501*z.max())
-        print(len(init), sum(fixedatoms))
-        MaxwellBoltzmannDistribution(init, temperature_K=6000)
-        init.set_tags(fixedatoms)
-    else:
-        init = None
-
-
-    print()
-    print("Running simulation with Asap's FixAtoms")
-    atoms2 = MakeParallelAtoms(init, cpulayout)
-    atoms2.arrays['r_init'] = atoms2.get_positions()
-    atoms2.set_calculator(EMT())
-    atoms2.set_constraint(FixAtoms(mask=atoms2.get_tags().astype(bool)))
-
-    if dynamics == "Verlet":
-        dyn = VelocityVerlet(atoms2, 3*units.fs)
-    elif dynamics == "NVTBerendsen":
-        dyn = NVTBerendsen(atoms2, 3*units.fs, temperature_K=2000, taut=200*units.fs)
-    elif dynamics == "Langevin":
-        dyn = Langevin(atoms2, 3*units.fs, temperature_K=2000, friction=1e-3)
-    else:
-        assert False
-    dyn.run(1000)
-
-    sanity(dynamics+"+FixAtoms", atoms2)
-
-    x = atoms2.get_positions()[:,0]
-    fixedatoms2 = np.less(x, 0.501 * x.max())
-    atoms2.set_tags(fixedatoms2)
-    atoms2.arrays['r_init'] = atoms2.get_positions()
-    atoms2.set_constraint(FixAtoms(mask=fixedatoms2))
-
-    dyn.run(1000)
-
-    sanity(dynamics+"+new-FixAtoms", atoms2)
 
 print("ALL TESTS SUCCEEDED!")
```

### Comparing `asap3-3.13.1/Test/parallel/parallelFIRE.py` & `asap3-3.9.6/Test/parallel/parallelFIRE.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     atoms = None
 if isparallel:
     atoms = MakeParallelAtoms(atoms, cpulayout)    
 
 print("Testing FIRE relaxation")
 atoms.set_calculator(EMT())
 e0 = atoms.get_potential_energy()
-natoms = atoms.get_global_number_of_atoms()
+natoms = atoms.get_number_of_atoms()
 ReportTest("Number of atoms", natoms, 10000, 0)
 print("Potential energy before perturbation:", e0, e0/natoms)
 
 atoms.set_positions(atoms.get_array("perturbation") + atoms.get_positions())
 e1 = atoms.get_potential_energy()
 print("Potential energy after perturbation:", e1, e1/natoms)
```

### Comparing `asap3-3.13.1/Test/parallel/parallelLangevin.py` & `asap3-3.9.6/Test/parallel/parallelLangevin.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 import sys, time
 from numpy import *
 import asap3
 from asap3.testtools import ReportTest
 from asap3.md.langevin import Langevin
 from asap3.md.verlet import VelocityVerlet
 from ase.lattice.cubic import FaceCenteredCubic
-from ase import units
 from asap3 import *
 from asap3.mpi import world
 
 nequil = 1000
 nequilprint = 25
-nsteps = 10000
+nsteps = 20000
 nprint = 250
 tolerance = 0.01
 nminor = 25
 timestep = 0.5
 
 #set_verbose(1)
 
@@ -52,15 +51,15 @@
     atoms.set_momenta(p - pavg)
 else:
     atoms = None
 
 if isparallel:
     atoms = MakeParallelAtoms(atoms, cpulayout)
 atoms.set_calculator(asap3.EMT())
-natoms = atoms.get_global_number_of_atoms()
+natoms = atoms.get_number_of_atoms()
     
 ReportTest("Number of atoms", natoms, 7*7*7*4, 0)
 
 print("Initializing ...")
 predyn = VelocityVerlet(atoms, 0.5)
 try:
     predyn.run(2500)
@@ -81,15 +80,15 @@
 
 def targetfunc(params, x):
     return params[0] * exp(-params[1] * x) + params[2]
 
 output = open("Langevin.dat", "w")
 
 for temp, frict in ((0.01, 0.001),):
-    dyn = Langevin(atoms, timestep, temperature_K=temp/units.kB, friction=frict)
+    dyn = Langevin(atoms, timestep, temp, frict)
     print("")
     print("Testing Langevin dynamics with T = %f eV and lambda = %f" % (temp, frict))
     ekin = atoms.get_kinetic_energy()/natoms
     print(ekin)
     output.write("%.8f\n" % ekin)
     temperatures = [(0, 2.0 / 3.0 * ekin)]
     a = 0.1
```

### Comparing `asap3-3.13.1/Test/parallel/parallelLennardJones.py` & `asap3-3.9.6/Test/parallel/parallelLennardJones.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     initial = None
     stdout = open("/dev/null", "w")
 
 for cpulayout in layout:
     if cpulayout:
         print("Test with layout "+str(cpulayout), file=stdout)
         atoms = MakeParallelAtoms(initial, cpulayout)
-        natoms = atoms.get_global_number_of_atoms()
+        natoms = atoms.get_number_of_atoms()
     else:
         print("Serial test", file=stdout)
         atoms = Atoms(initial)
         natoms = len(atoms)
     print("Number of atoms:", natoms)
     temp = atoms.get_kinetic_energy() / (1.5*units.kB*natoms)
     print("Temp:", temp, "K", file=stdout)
```

### Comparing `asap3-3.13.1/Test/parallel/parallelLocalStructure.py` & `asap3-3.9.6/Test/parallel/parallelNeighborLocator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test local crystal structure analysis (CNA and Coordination number)."""
 from __future__ import print_function
 
 from asap3 import *
-from asap3.analysis import FullCNA, RestrictedCNA, CoordinationNumbers
+from asap3.analysis.localstructure import RestrictedCNA, CoordinationNumbers
 from asap3.testtools import ReportTest
 from asap3.mpi import world
-from ase.lattice import bulk
+from ase.build import bulk
 import numpy as np
 
 debug = 0
 if debug == 1:
     DebugOutput("parallel%d.log", nomaster=True)
 elif debug == 2:
     time.sleep(world.rank)
@@ -23,63 +23,71 @@
 elif world.size == 2:
     cpulayout = [2,1,1]
 elif world.size == 3:
     cpulayout = [1,3,1]
 elif world.size == 4:
     cpulayout = [2,1,2]
 
+nbl_cutoff = 4.5
+
+def makesystem():
+    atoms = bulk('Cu')
+    atoms = atoms.repeat((15, 15, 15))
+    if cpulayout:
+        atoms = atoms.repeat(cpulayout)
+    atoms.set_pbc((True, False, True))
+    #atoms.set_pbc((False, True, True))
+    del atoms[87]   #Create point defect
+    return atoms
+
 for usepot in (True, False):
+    # Make serial nb list.
+    seratoms = makesystem()
+    sernblist = FullNeighborList(nbl_cutoff, seratoms)
+
+    # Make parallel nb list
     if ismaster:
-        atoms = bulk('Cu')
-        atoms = atoms.repeat((10, 10, 10))
-        if isparallel:
-            atoms = atoms.repeat(cpulayout)
-        del atoms[100]   #Create point defect
+        atoms = makesystem()
     else:
         atoms = None
     if isparallel:
         atoms = MakeParallelAtoms(atoms, cpulayout)
-    natoms = atoms.get_global_number_of_atoms()
+    natoms = atoms.get_number_of_atoms()
     if usepot:
         atoms.set_calculator(EMT())
-        atoms.get_potential_energy()
-    
-    print("Testing CNA")
-    RestrictedCNA(atoms)
-    t = atoms.get_tags()
-    counts = np.zeros(3, int)
-    for i in range(3):
-        counts[i] = (t == i).sum()
-    world.sum(counts)
-    
-    ReportTest("CNA: fcc atoms", counts[0], natoms-12, 0)
-    ReportTest("CNA: hcp atoms", counts[1], 0, 0)
-    ReportTest("CNA: other atoms", counts[2], 12, 0)
+        old_energy = atoms.get_potential_energy()
+        print(atoms.get_calculator().get_cutoff())
+        print(len(atoms), atoms.get_number_of_atoms())
+        #assert atoms.get_calculator().get_cutoff() >= nbl_cutoff
     
-    print()
-    print("Testing coordination number")
-    t = CoordinationNumbers(atoms)
-    counts = np.zeros(20, int)
-    wanted = np.zeros(20, int)
-    wanted[11] = 12
-    wanted[12] = natoms - 12
-    for i in range(len(counts)):
-        counts[i] = (t == i).sum()
+    print("Testing parallel neighbor locator (usepot = {0})".format(usepot))
+    nblist = FullNeighborList(nbl_cutoff, atoms)
+    print("Length of neighbor locator", len(nblist), len(atoms))
+    print(nblist[-1])
     if isparallel:
-        world.sum(counts)
-    for i in range(len(counts)):
-        ReportTest("Coordination number {0}".format(i), counts[i], wanted[i], 0)
-        
-    print()
-    print("Testing Full CNA")
-    cnacalc = FullCNA(atoms)
-    cna = cnacalc.get_normal_cna()
-    print(cna[0])
-    ReportTest("Length of CNA vector", len(cna), len(atoms), 0)
+        ids = atoms.get_ids()
+    else:
+        ids = range(len(atoms))
+    maxlen = -1
+    minlen = 1e100
     for i in range(len(atoms)):
-        ReportTest("Number of CNA vectors (atom {0})".format(i), 
-                   sum(cna[i].values()), t[i], 0, silent=True)
-        if (t[i] == 12):
-            ReportTest("Number of 421 bonds (atom {0})".format(i),
-                       cna[i][(4,2,1)], 12, 0, silent=True)
-      
-ReportTest.Summary()
+        l = len(nblist[i])
+        l_exp = len(sernblist[ids[i]])
+        ReportTest("NBlist length (i={0}, id={1})".format(i, ids[i]), 
+                   l, l_exp, 0, silent=True)
+        if l > maxlen:
+            maxlen = l
+        if l < minlen:
+            minlen = l
+        if l == l_exp:
+            snbl = set((n for n in sernblist[ids[i]]))
+            for nb in nblist[i]:
+                if nb < len(atoms):
+                    assert ids[nb] in snbl
+
+    print("Neighbor list length:", minlen, '-', maxlen)
+    if usepot:
+        atoms[1].position += np.array((1e-5,0,0))
+        ReportTest("Energy", atoms.get_potential_energy(), old_energy, 1e-4)
+ 
+
+#ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/parallel/parallelLongVerlet.py` & `asap3-3.9.6/Test/parallel/parallelLongVerlet.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from asap3 import *
 from ase.lattice.cubic import FaceCenteredCubic
 from pickle import *
 from numpy import *
 import sys, os, time
 from asap3.testtools import *
 from asap3.mpi import world
-from asap3.md.velocitydistribution import MaxwellBoltzmannDistribution
 
 debug = 0
 if debug == 1:
     DebugOutput("longverlet%d.log", nomaster=True)
 elif debug == 2:
     time.sleep(world.rank)
     print("PID:", os.getpid())
@@ -39,17 +38,17 @@
 isparallel = world.size != 1
 if ismaster:
     print_version(1)
     
 if world.size == 1:
     cpulayouts = [None]
 elif world.size == 2:
-    cpulayouts = [[2,1,1],]
+    cpulayouts = [[2,1,1], [1,2,1]]
 elif world.size == 3:
-    cpulayouts = [[3,1,1],]
+    cpulayouts = [[3,1,1], [1,1,3]]
 elif world.size == 4:
     cpulayouts = [[4,1,1], [2,1,2]]
 elif world.size == 8:
     cpulayouts = [[8,1,1], [4,2,1], [2,2,2]]
 elif world.size == 16:
     cpulayouts = [[8,1,2], [4,2,2]]
 else:
@@ -57,41 +56,40 @@
 
 e_start_dict = {}
 for cpulayout in cpulayouts:
     for boundary in ((1,1,1), (0,0,0), (0,1,1), (1,0,0)):
         print ("CPU Layout: %s.  Periodic boundary conditions: %s."
                % (str(cpulayout), str(boundary)))
         if ismaster:
-            size = array((20, 10, 10)) * cpulayout
-            atoms = FaceCenteredCubic(size=size, symbol="Cu",
+            atoms = FaceCenteredCubic(size=(160,20,20), symbol="Cu",
                                       pbc=boundary, latticeconstant=3.61*1.04)
         else:
             atoms = None
         if isparallel:
             atoms = MakeParallelAtoms(atoms, cpulayout)
-        natoms = atoms.get_global_number_of_atoms()
+        natoms = atoms.get_number_of_atoms()
         atoms.set_calculator(EMT())
-        MaxwellBoltzmannDistribution(atoms, temperature_K=3000)
+        MaxwellBoltzmannDistribution(atoms, 3000*units.kB)
         if ismaster:
             print("Initializing")
         e_st_pot = atoms.get_potential_energy()/natoms
         try:
             e_start_pot = e_start_dict[boundary]
         except KeyError:
             e_start_pot = e_start_dict[boundary] = e_st_pot
         else:
              ReportTest("Initial energy ", e_st_pot, e_start_pot, 1e-4,
                         silent=True)
-        dyn = VelocityVerlet(atoms, logfile="-", timestep=3*units.fs, loginterval=1)
+        dyn = VelocityVerlet(atoms, logfile="-", dt=3*units.fs, loginterval=1)
         dyn.run(50)
         e_start = (atoms.get_potential_energy() 
                    + atoms.get_kinetic_energy())/natoms
         if ismaster:
             print("Running")
-        dyn = VelocityVerlet(atoms, timestep=5*units.fs)
+        dyn = VelocityVerlet(atoms, dt=5*units.fs)
         logger = MDLogger(dyn, atoms, '-', peratom=True)
         logger()
         dyn.attach(logger, interval=25)
         if writetraj:
             if cpulayout is None:
                 tname = "longVerlet-serial-%d-%d-%d.traj" % tuple(boundary)
             else:
@@ -102,11 +100,11 @@
             dyn.attach(traj, interval=1000)
         
         for i in range(100):
             dyn.run(100)
             if i % 5 == 4:
                 print(i+1, "%")
             e = (atoms.get_potential_energy() + atoms.get_kinetic_energy())/natoms
-            ReportTest("Step "+str(i), e, e_start, 3e-4, silent=True)
+            ReportTest("Step "+str(i), e, e_start, 1e-4, silent=True)
 
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/parallel/parallelNPT.py` & `asap3-3.9.6/Test/parallel/parallelNPT.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,21 @@
 from asap3.md.langevin import Langevin
 from asap3.io.trajectory import Trajectory
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.testtools import ReportTest
 from asap3.mpi import world
 from ase import units
 import sys
-import numpy as np
 
 T_goal = 300 # K
 p_goal = 1 # GPa
 bulk = 137 # Gpa
 cp = 24.43 # J / (K * mol)
 step1 = 25
 
-#set_verbose(1)
-
-np.random.seed([4314523, world.size, world.rank])
-
 if len(sys.argv) == 1 or sys.argv[0].endswith("TestAll.py"):
     out1 = "testNPT-1.out"
     out2 = "testNPT-2.out"
     ttime = 25
     ptime = 75
 elif len(sys.argv) == 3:
     ttime = float(sys.argv[1])
@@ -53,60 +48,57 @@
 else:
     if ismaster:
         atoms = FaceCenteredCubic(size=(30,15,15), symbol="Cu", pbc=True)
     else:
         atoms = None
     atoms = MakeParallelAtoms(atoms, cpulayout)
     atoms.set_calculator(EMT())
-    print("Number of atoms:", atoms.get_global_number_of_atoms())
+    print("Number of atoms:", atoms.get_number_of_atoms())
 
     print("Heating to %d K using Langevin" % T_goal)
-    lgv = Langevin(atoms, 5 * units.fs, temperature_K=2*T_goal,
-                       friction=0.05)
+    lgv = Langevin(atoms, 5 * units.fs, temperature=2*T_goal*units.kB, friction=0.05)
 
-    while atoms.get_kinetic_energy() < 1.5 * atoms.get_global_number_of_atoms() * T_goal * units.kB:
+    while atoms.get_kinetic_energy() < 1.5 * atoms.get_number_of_atoms() * T_goal * units.kB:
         lgv.run(5)
-        T = atoms.get_kinetic_energy() / (1.5 * atoms.get_global_number_of_atoms() * units.kB)
+        T = atoms.get_kinetic_energy() / (1.5 * atoms.get_number_of_atoms() * units.kB)
         print("Temperature is now %.2f K" % (T,))
     print("Desired temperature reached!")
 
-    lgv.set_temperature(temperature_K=T_goal)
+    lgv.set_temperature(T_goal*units.kB)
 
     for i in range(2):
         lgv.run(20)
         s = atoms.get_stress()
         p = -(s[0] + s[1] + s[2])/3.0 / units.GPa
-        T = atoms.get_kinetic_energy() / (1.5 * atoms.get_global_number_of_atoms() * units.kB)
+        T = atoms.get_kinetic_energy() / (1.5 * atoms.get_number_of_atoms() * units.kB)
         print("Pressure is %f GPa, desired pressure is %f GPa (T = %.2f K)" % (p, p_goal, T))
         dv = (p - p_goal) / bulk
         print("Adjusting volume by", dv)
         cell = atoms.get_cell()
         atoms.set_cell(cell * (1.0 + dv/3.0))
 
-    T = atoms.get_kinetic_energy() / (1.5 * atoms.get_global_number_of_atoms() * units.kB)
+    T = atoms.get_kinetic_energy() / (1.5 * atoms.get_number_of_atoms() * units.kB)
     print("Temperature is now %.2f K" % (T,))
 
     stressstate = array([-2, -1, 0, 0, 0, 0])*p_goal*units.GPa
-    dyn = NPT(atoms, 5 * units.fs, temperature_K=T_goal,
-                  externalstress=stressstate,
-                  ttime=ttime*units.fs,
-                  pfactor=(ptime*units.fs)**2 * bulk * units.GPa)
+    dyn = NPT(atoms, 5 * units.fs, T_goal*units.kB, stressstate,
+              ttime*units.fs, (ptime*units.fs)**2 * bulk * units.GPa)
     traj = Trajectory("NPT-atoms.traj", "w", atoms)
     #dyntraj = ParallelHooverNPTTrajectory("NPT-dyn-traj.nc", dyn, interval = 50)
     dyn.attach(traj, interval=50)
     #dyn.Attach(dyntraj)
 
     out = open(out1, "w")
 
     temp = []
     pres = []
     vol = []
     for i in range(step1):
         dyn.run(5)
-        T = atoms.get_kinetic_energy() / (1.5 * atoms.get_global_number_of_atoms() * units.kB)
+        T = atoms.get_kinetic_energy() / (1.5 * atoms.get_number_of_atoms() * units.kB)
         s = atoms.get_stress() / units.GPa
         p = -(s[0] + s[1] + s[2])/3.0
         out.write("%5.2f %5.2f %7.5f      %7.5f %7.5f %7.5f %7.5f %7.5f %7.5f\n" %
                   ((dyn.get_time(), T, p)+tuple(s)))
         out.flush()
         cell = atoms.get_cell()
         v = cell[0,0] * cell[1,1] * cell[2,2]
```

### Comparing `asap3-3.13.1/Test/parallel/parallelOpenKIM_EMT.py` & `asap3-3.9.6/Test/parallel/parallelOpenKIM_NeighRvec_H.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 from __future__ import print_function
 #import production
 
 from asap3 import *
 from asap3.md.verlet import VelocityVerlet
+from pickle import *
 from numpy import *
-from pickle import load
 import sys, os, time
 from asap3.testtools import *
 from asap3.mpi import world
 
-openkimmodel = "EMT_Asap_Standard_JacobsenStoltzeNorskov_1996_Cu__MO_396616545191_001"
-
-picklehack = {'encoding': 'latin1'}
+openkimmodel = "EMT_Asap_Standard_Jacobsen_Stoltze_Norskov_AlAgAuCuNiPdPt__MO_118428466217_002"
 
 if OpenKIMsupported:
-    try:
-        calc = OpenKIMcalculator(openkimmodel)
-    except AsapError as oops:
-        if oops.args[0].startswith('Failed to initialize OpenKIM model'):
-            print("OpenKIM model {} not installed - skipping test.".format(openkimmodel))
-            calc = None
-        else:
-            raise
-    
-if OpenKIMsupported and calc is not None:
+
     debug = 0
     if debug == 1:
-        DebugOutput("parallelopenkim%d.log", nomaster=True)
+        DebugOutput("makeverlet%d.log", nomaster=True)
     elif debug == 2:
         time.sleep(world.rank)
         print("PID:", os.getpid())
         time.sleep(20)
 
     print_version(1)
     #set_verbose(1)
@@ -78,18 +67,18 @@
     if isparallel:
         print("RUNNING PARALLEL VERSION OF TEST SCRIPT")
     else:
         print("RUNNING SERIAL VERSION OF TEST SCRIPT")
 
     if ismaster:
         # First, load a small system
-        if os.path.exists("Verlet_legacymass.pickle"):
-            data = load(open("Verlet_legacymass.pickle", "rb"), **picklehack)
+        if os.path.exists("testVerlet.pickle"):
+            data = load(open("testVerlet.pickle", "rb"))
         else:
-            data = load(open("../Verlet_legacymass.pickle", "rb"), **picklehack)
+            data = load(open("../testVerlet.pickle", "rb"))
         init_pos = array(data["initial"])
         init_pos.shape = (-1,3)
         init_box = array(data["box"])
         init_box.shape = (3,3)
         a = Atoms(positions=init_pos, cell=init_box, pbc=(1,1,1))
         a.set_atomic_numbers(29*ones(len(a)))
         #atoms = a.repeat((2,2,3))
@@ -102,22 +91,23 @@
         out = sys.stderr
     else:
         atoms = None
         out = open("/dev/null", "w")
 
     if isparallel:
         atoms = MakeParallelAtoms(atoms, cpulayout)
-        nTotalAtoms = atoms.get_global_number_of_atoms()
+        nTotalAtoms = atoms.get_number_of_atoms()
     else:
         nTotalAtoms = len(atoms)
 
     #report()
 
     print("Setting potential")
-    atoms.set_calculator(calc)
+    atoms.set_calculator(OpenKIMcalculator(openkimmodel, allowed='NEIGH_RVEC_H'))
+
     dyn = VelocityVerlet(atoms, 2 * femtosecond)
     # if isparallel:
     #     traj = ParallelNetCDFTrajectory("ptraj.nc", atoms, interval=20)
     # else:
     #     traj = NetCDFTrajectory("ptraj.nc", atoms, interval=20)
     # dyn.Attach(traj)
     # traj.Update()
```

### Comparing `asap3-3.13.1/Test/parallel/parallelPBC.py` & `asap3-3.9.6/Test/parallel/parallelPBC.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,13 +46,13 @@
     if ismaster:
         atoms = makesystem()
         atoms.set_pbc(pbc)
     else:
         atoms = None
     if isparallel:
         atoms = MakeParallelAtoms(atoms, cpulayout)
-    natoms = atoms.get_global_number_of_atoms()
+    natoms = atoms.get_number_of_atoms()
     atoms.set_calculator(EMT())
     energy = atoms.get_potential_energy()
     ReportTest("PBC={0}".format(str(pbc)), energy, old_energy, 1e-6)
 
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/parallel/parallelPBC2.py` & `asap3-3.9.6/Test/parallel/parallelPBC2.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,13 +51,13 @@
     if ismaster:
         atoms = makesystem()
         atoms.set_pbc(pbc)
     else:
         atoms = None
     if isparallel:
         atoms = MakeParallelAtoms(atoms, cpulayout)
-    natoms = atoms.get_global_number_of_atoms()
+    natoms = atoms.get_number_of_atoms()
     atoms.set_calculator(EMT())
     energy = atoms.get_potential_energy()
     ReportTest("PBC={0}".format(str(pbc)), energy, old_energy, 1e-6)
 
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/parallel/parallelPotentials.pickle` & `asap3-3.9.6/Test/parallel/parallelPotentials.pickle`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/parallel/parallelPotentials.py` & `asap3-3.9.6/Test/parallel/parallelPotentials.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/parallel/parallelRDF.py` & `asap3-3.9.6/Test/parallel/parallelRDF.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                               size=(10,10,10), latticeconstant=latconst)
         if isparallel:
             atoms = atoms.repeat(cpulayout)
     else:
         atoms = None
     if isparallel:
         atoms = MakeParallelAtoms(atoms, cpulayout)
-    natoms = atoms.get_global_number_of_atoms()
+    natoms = atoms.get_number_of_atoms()
 
     if withemt:
         atoms.set_calculator(EMT())
         print(atoms.get_potential_energy())
 
     rdf = RadialDistributionFunction(atoms, maxrdf, nbins, verbose=True)
     z = atoms.get_atomic_numbers()[0]
```

### Comparing `asap3-3.13.1/Test/parallel/parallelStress.py` & `asap3-3.9.6/Test/parallel/parallelStress.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 import sys
 sys.path.append("..")
 from StressModule import *
 from ase import data, Atoms
 from ase.lattice.cubic import FaceCenteredCubic
 from ase.md.verlet import VelocityVerlet
+from ase.md.langevin import Langevin
 from asap3.mpi import world
 
 debug = 0
 if debug == 1:
     DebugOutput("parallelStress-%d.log", nomaster=True)
 elif debug == 2:
     time.sleep(world.rank)
@@ -110,12 +111,12 @@
     else:
         atoms = MakeParallelAtoms(None, cpulayout)
     if symb.find("Rasmussen") >= 0:
         print("Using the special EMT parameters by T. Rasmussen")
         atoms.set_calculator(EMT(EMTRasmussenParameters()))
     else:
         atoms.set_calculator(EMT())
-    atoms.set_momenta(np.zeros((len(atoms),3), float))
+    atoms.set_momenta(np.zeros((len(atoms),3), np.float))
     findlatticeconst(atoms, latconst)
     elasticconstants(atoms, symb, **book[symb])
 
 ReportTest.Summary()
```

### Comparing `asap3-3.13.1/Test/parallel/parallelTrajectories.py` & `asap3-3.9.6/Test/parallel/parallelTrajectories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import print_function
 from asap3 import *
 from ase.md.verlet import VelocityVerlet
 from ase.lattice.cubic import FaceCenteredCubic
 from asap3.io.trajectory import *
 from numpy import *
 import sys, os, time
 from asap3.testtools import ReportTest
```

### Comparing `asap3-3.13.1/Test/parallel/parallelVerlet.py` & `asap3-3.9.6/Test/parallel/parallelVerlet.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,18 +64,18 @@
 if isparallel:
     print("RUNNING PARALLEL VERSION OF TEST SCRIPT")
 else:
     print("RUNNING SERIAL VERSION OF TEST SCRIPT")
 
 if ismaster:
     # First, load a small system
-    if os.path.exists("Verlet_legacymass.pickle"):
-        picfile = "Verlet_legacymass.pickle"
+    if os.path.exists("testVerlet.pickle"):
+        picfile = "testVerlet.pickle"
     else:
-        picfile = "../Verlet_legacymass.pickle"
+        picfile = "../testVerlet.pickle"
     try:
         data = load(open(picfile, "rb"))
     except UnicodeDecodeError:
         data = load(open(picfile, "rb"), encoding='latin1')
     init_pos = array(data["initial"])
     init_pos.shape = (-1,3)
     init_box = array(data["box"])
@@ -92,15 +92,15 @@
     out = sys.stderr
 else:
     atoms = None
     out = open("/dev/null", "w")
 
 if isparallel:
     atoms = MakeParallelAtoms(atoms, cpulayout)
-    nTotalAtoms = atoms.get_global_number_of_atoms()
+    nTotalAtoms = atoms.get_number_of_atoms()
 else:
     nTotalAtoms = len(atoms)
 
 #report()
 
 print("Setting potential")
 atoms.set_calculator(EMT())
```

### Comparing `asap3-3.13.1/Test/parallel/simplempi.py` & `asap3-3.9.6/Test/parallel/simplempi.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,30 +29,26 @@
 world.wait(rq)
 
 ReportTest("Data received by %s from %s" % (world.rank, fr), indata[0], 2*fr, 0)
 
 
 outdata = world.rank * np.arange(10000000)
 indata = np.zeros(10000000, int)
-print("Data types:", outdata.shape, outdata.dtype, indata.shape, indata.dtype)
 
 to = world.rank + 1
 if to >= world.size:
     to = 0
 fr = world.rank - 1
 if fr < 0:
     fr += world.size
 
 print("%d: to=%d from=%d" % (world.rank, to, fr))
 
 rq = world.send(outdata, to, block=False)
-print("%d: Nonblocking send returned" % (world.rank,))
-print("%d: %s" % (world.rank, repr(rq)))
 world.receive(indata, fr)
-print("%d: Receive returned" % (world.rank,)) 
 #world.wait(rq)
 print("Request completed:", rq.test())
 rq.wait()
 
 assert (indata == fr * np.arange(10000000)).all()
 
 s = world.sum(2.5 * world.rank)
```

### Comparing `asap3-3.13.1/Test/potResults.py` & `asap3-3.9.6/Test/potResults.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Test/test_reproducible.py` & `asap3-3.9.6/Test/test_reproducible.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 from __future__ import print_function
 
 from numpy import *
 from asap3 import *
 import pickle, os, sys, time
 
 # PrintVersion(1)
-picklehack = {'encoding': 'latin1'}
-
-if getattr(Atoms, '_ase_handles_dynamic_stress', False):
-    stresshack = {'include_ideal_gas': True}
+if sys.version_info[0] >= 3:
+    picklehack = {'encoding': 'latin1'}
 else:
-    stresshack = {}
-    
+    picklehack = {}
+
 def main():
     datafile = "test_reproducible2.dat"
     is_data = os.access(datafile, os.R_OK)
     initialize = 0
     if len(sys.argv) == 2 and sys.argv[1] == "init":
         initialize = 1
         if os.access(datafile, os.R_OK):
@@ -59,15 +57,15 @@
     r += dr
     lattice.set_positions(r)
 
     atoms1 = Atoms(lattice)
     atoms1.set_calculator(EMT())
 
     print("Total energy:", atoms1.get_potential_energy())
-    print("Stress:", atoms1.get_stress(**stresshack))
+    print("Stress:", atoms1.get_stress())
     #CNA(atoms1)
     #plot = atoms1.GetPlot()
     #time.sleep(10)
 
     z = lattice.get_atomic_numbers()
     z[0] = z[1] = 47
     lattice.set_atomic_numbers(z)
```

### Comparing `asap3-3.13.1/Tools/CNA.cpp` & `asap3-3.9.6/Tools/CNA.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -25,52 +25,44 @@
 #include "CNA.h"
 #include "Atoms.h"
 #include "NeighborList.h"
 #include "Vec.h"
 #include "Timing.h"
 #include "Exception.h"
 #include "GetNeighborList.h"
-#include "Debug.h"
 #include <vector>
 using std::vector;
 
 namespace ASAPSPACE {
 
 void CNA(PyObject *py_atoms, double rCut, vector<char> &cna)
 {
-  DEBUGPRINT;
   USETIMER("CNA");
   // Create a full neighbor list object
   PyObject *py_nblist = GetSecondaryNeighborList(py_atoms, rCut);
-  DEBUGPRINT;
   if (py_nblist == NULL)
     throw AsapPythonError();
   NeighborLocator *nl = ((PyAsap_NeighborLocatorObject*) py_nblist)->cobj;
-  ASSERT(nl != NULL);
-  ASSERT(!nl->IsInvalid());
+  assert(nl != NULL);
   Atoms *atoms = nl->GetAtoms();
 
-  DEBUGPRINT;
   atoms->Begin(py_atoms);
   int nAtoms = atoms->GetNumberOfAtoms();
   int nTotal = nAtoms + atoms->GetNumberOfGhostAtoms();
-  ASSERT(!nl->IsInvalid());
 
   vector<int> numFCC(nTotal);
   vector<int> numHCP(nTotal);
   for (unsigned int a2 = 0; a2 < nTotal; a2++)
     {
       vector<int> nbs2;
-      DEBUGPRINT;
       nl->GetFullNeighbors(a2, nbs2);
-      DEBUGPRINT;
       for (unsigned int n2 = 0; n2 < nbs2.size(); n2++)
 	{
 	  int a1 = nbs2[n2];
-	  ASSERT(a1 < nTotal);
+	  assert(a1 < nTotal);
 	  if (a1 < a2)
 	    {
 	      vector<int> common;
 	      vector<int> nbs1;
 	      nl->GetFullNeighbors(a1, nbs1);
 	      for (unsigned int n1 = 0; n1 < nbs1.size(); n1++)
 		{
@@ -110,15 +102,14 @@
 			}
 		    }
 		}
 	    }
 	}
     }
   // 0: fcc (421), 1: hcp (422), 2: other
-  DEBUGPRINT;
   cna.resize(nAtoms);
   for (int a = 0; a < nAtoms; a++)
     {
       vector<int> nbs;
       nl->GetFullNeighbors(a, nbs);
       if (nbs.size() == 12)
 	{
@@ -130,11 +121,10 @@
 	    cna[a] = 2;
 	}
       else
 	cna[a] = 2;
     }
   atoms->End();
   Py_DECREF(py_nblist);
-  DEBUGPRINT;
 }
 
 } // end namespace
```

### Comparing `asap3-3.13.1/Tools/CNA.h` & `asap3-3.9.6/Tools/CNA.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Tools/CoordinationNumbers.cpp` & `asap3-3.9.6/Tools/CoordinationNumbers.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 #include "CoordinationNumbers.h"
 #include "Atoms.h"
 #include "NeighborLocator.h"
 #include "GetNeighborList.h"
 #include "Vec.h"
 #include "Timing.h"
 #include "Exception.h"
-//#define ASAPDEBUG
-#include "Debug.h"
 #include <vector>
 using std::vector;
 
 namespace ASAPSPACE {
 
 void CoordinationNumbers(PyObject *py_atoms, double rCut, vector<int> &coord)
 {
-  DEBUGPRINT;
   USETIMER("CoordinationNumbers");
   // Create a full neighbor list object
   PyObject *py_nblist = NULL;
   Atoms *atoms = NULL;
   // Get a neighbor list, and an open atoms object.
   GetNbList_FromAtoms(py_atoms, rCut, &py_nblist, &atoms);
   NeighborLocator *nl = ((PyAsap_NeighborLocatorObject*) py_nblist)->cobj;
-  ASSERT(nl != NULL);
+  assert(nl != NULL);
 
   int nAtoms = atoms->GetNumberOfAtoms();
+  int nTotal = nAtoms + atoms->GetNumberOfGhostAtoms();
+  
+
   coord.clear();
   coord.resize(nAtoms);
   int maxlistlen = nl->MaxNeighborListLength();
   vector<int> nb_buffer(maxlistlen);
   vector<Vec> diffs(maxlistlen);
   vector<double> diffs2(maxlistlen);
   for (int a1 = 0; a1 < nAtoms; a1++)
@@ -67,11 +67,10 @@
           if (a2 < nAtoms)
             coord[a2]++;
         }
     }
   atoms->End();
   AsapAtoms_DECREF(atoms);
   Py_DECREF(py_nblist);
-  DEBUGPRINT;
 }
 
 } // end namespace
```

### Comparing `asap3-3.13.1/Tools/CoordinationNumbers.h` & `asap3-3.9.6/Interface/AsapSerial.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-// -*- C++ -*-
-//
-// Copyright (C) 2002-2011 Jakob Schiotz and Center for Individual
+// Copyright (C) 2008-2011 Jakob Schiotz and Center for Individual
 // Nanoparticle Functionality, Department of Physics, Technical
 // University of Denmark.  Email: schiotz@fysik.dtu.dk
 //
 // This file is part of Asap version 3.
 //
 // This program is free software: you can redistribute it and/or
 // modify it under the terms of the GNU Lesser General Public License
@@ -19,22 +17,37 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 // GNU General Public License for more details.
 //
 // You should have received a copy of the GNU General Public License
 // and the GNU Lesser Public License along with this program.  If not,
 // see <http://www.gnu.org/licenses/>.
 
-#ifndef _COORDINATIONNUMBERS_H
-#define _COORDINATIONNUMBERS_H
-
-#include "AsapPython.h"
-#include <vector>
+#undef PARALLEL
+#include "AsapModule.cpp"
 
-namespace ASAPSPACE {
 
-class Atoms;
+#if PY_MAJOR_VERSION >= 3
+PyMODINIT_FUNC PyInit__asap_p3(void)
+{
+    return AsapInitModule();
+}
+#else
+PyMODINIT_FUNC init_asap_p2(void)
+{
+    AsapInitModule();
+}
+#endif
 
-void CoordinationNumbers(PyObject *py_atoms, double rCut, std::vector<int> &coord);
 
-} // end namespace
 
-#endif // _COORDINATIONNUMBERS_H
+#if 0
+// For testing only
+int main(int argc, char **argv)
+{
+  int status;
+  
+  Py_Initialize();
+  initasapserial3();
+  status = Py_Main(argc, argv);
+  return status;
+}
+#endif
```

### Comparing `asap3-3.13.1/Tools/FullCNA.cpp` & `asap3-3.9.6/Tools/FullCNA.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -100,15 +100,15 @@
   usingCutoffMap = true;
 }
 
 void FullCNA::MakeCNA()
 {
   DEBUGPRINT;
   // Don't call this function again
-  ASSERT(atoms == NULL && py_nblist == NULL);
+  assert(atoms == NULL && py_nblist == NULL);
   ready = true;
 
   py_nblist = GetSecondaryNeighborList(py_atoms, cnaCutoff);
   if (py_nblist == NULL)
     throw AsapPythonError();
   NeighborLocator *nblistBonds = ((PyAsap_NeighborLocatorObject *) py_nblist)->cobj;
   atoms = nblistBonds->GetAtoms();
@@ -213,15 +213,15 @@
         }
     }
 
   // erase adjacent bonds from bondsToProcess
   for( bondIter = adjacentBonds.begin(); bondIter != adjacentBonds.end(); bondIter++ )
     {
       std::vector<intPair>::iterator bond = find(bondsToProcess.begin(),bondsToProcess.end(),*bondIter);
-      ASSERT(bond != bondsToProcess.end());
+      assert(bond != bondsToProcess.end());
       bondsToProcess.erase(bond);
       //bondsToProcess.remove(*bondIter);
     }
 
   atomsProcessed.push_back(atom);
   for( bondIter = adjacentBonds.begin(); bondIter != adjacentBonds.end(); bondIter++ )
     {
@@ -275,15 +275,15 @@
         {
           if(nbrs1[nbrIdx1] == nbrs2[nbrIdx2])
             {
               commonNeighbors.push_back(nbrs1[nbrIdx1]);
               count += 1;
             }
         }
-      ASSERT(count <= 1);
+      assert(count <= 1);
     }
 
   // the first index is the number of common neighbors
   int numCommonNbrs = commonNeighbors.size();
   index[0] = numCommonNbrs;
 
   vector<intPair> bondsToProcess;
@@ -340,15 +340,15 @@
       // is it bigger than the maximum?
       if(thisClusterSize > maxClusterSize)
         maxClusterSize = thisCluster.size();
 
       nBondsLeft = bondsToProcess.size();
     }
   // sanity check
-  ASSERT(totalBondsInClusters == numCNBonds);
+  assert(totalBondsInClusters == numCNBonds);
 
   // the third index is the size of the largest cluster
   index[2] = maxClusterSize;
 
   // Now code the numbers into a single integer
   int codeindex = (index[0] * CNA_CODE_MULT + index[1]) * CNA_CODE_MULT
       + index[2];
@@ -374,15 +374,15 @@
   npy_int32 *ptr = (npy_int32 *) PyArray_DATA((PyArrayObject *) result);
   for (int i = 0; i < dims[0]; ++i)
     {
       *(ptr++) = cnaIndices[i].first.first;
       *(ptr++) = cnaIndices[i].first.second;
       *(ptr++) = cnaIndices[i].second;
     }
-  ASSERT(3 * dims[0] == ptr - (npy_int32 *) PyArray_DATA((PyArrayObject *) result));
+  assert(3 * dims[0] == ptr - (npy_int32 *) PyArray_DATA((PyArrayObject *) result));
   DEBUGPRINT;
   return result;
 }
 
 // Return a Python list with CNA data for each atom.  Each element is
 // a dictionary with the CNA tuples as keys and bond numbers as values.
 PyObject *FullCNA::GetPerAtomCNA()
```

### Comparing `asap3-3.13.1/Tools/FullCNA.h` & `asap3-3.9.6/Tools/FullCNA.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Tools/GetNeighborList.cpp` & `asap3-3.9.6/Tools/GetNeighborList.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -34,47 +34,42 @@
 // Return a neighborlist object and an Atoms access object (either new
 // or reused from the potential).  Begin() will have been called on the atoms.
 
 void GetNbList_FromAtoms(PyObject *pyatoms, double rCut,
 			      PyObject **pynblist, Atoms **atoms)
 {
   PyObject *py_pot = NULL;
+  Potential *pot = NULL;
   NeighborLocator *nblist = NULL;
   *pynblist = NULL;  // Not found yet.
   py_pot = PyObject_CallMethod(pyatoms, "get_calculator", "");
   if (py_pot == NULL)
     PyErr_Clear();
   else
     {
       // Got a potential.
       DEBUGPRINT;
-      // Get the neighbor list, bypassing a Python-defined wrapper function
-      *pynblist = PyObject_CallMethod(py_pot, "_get_neighborlist", "");
+      *pynblist = PyObject_CallMethod(py_pot, "get_neighborlist", "");
       if (*pynblist == NULL)
         PyErr_Clear();
       else
         {
           if (PyAsap_NeighborLocatorCheck(*pynblist))
             {
               // Got an ASAP neighborlocator object.
               DEBUGPRINT;
                nblist = ((PyAsap_NeighborLocatorObject *)*pynblist)->cobj;
                if (nblist->GetCutoffRadius() >= rCut)
                  {
                    // Use this neighbor list
                    DEBUGPRINT;
-		   PyObject *method = PyUnicode_FromString("check_update_neighborlist");
-		   PyObject *obj = PyObject_CallMethodObjArgs(py_pot, method, pyatoms, NULL);
-		   Py_DECREF(method);
-		   if (obj == NULL)
-		     throw AsapPythonError();
-		   Py_DECREF(obj);
-                   *atoms = ((PyAsap_PotentialObject *) py_pot)->cobj->GetAtoms();
+                   *atoms = nblist->GetAtoms();
                    AsapAtoms_INCREF(*atoms);
                    (*atoms)->Begin(pyatoms);
+                   nblist->CheckAndUpdateNeighborList();
                  }
                else
                  {
                    // Discard neighbor list
                    DEBUGPRINT;
                    nblist = NULL;
                    Py_CLEAR(*pynblist);
@@ -88,41 +83,41 @@
             }
         }
     }
   Py_XDECREF(py_pot);
   if (nblist == NULL)
     {
       DEBUGPRINT;
-      ASSERT(*pynblist == NULL);
+      assert(*pynblist == NULL);
       // Create interface object and neighborlist object
       *pynblist = GetSecondaryNeighborList(pyatoms, rCut);
       if (*pynblist == NULL)
         throw AsapPythonError();
       nblist = ((PyAsap_NeighborLocatorObject *)*pynblist)->cobj;
       *atoms = nblist->GetAtoms();
-      ASSERT(*atoms != NULL);
+      assert(*atoms != NULL);
       AsapAtoms_INCREF(*atoms);
       (*atoms)->Begin(pyatoms);
     }
-  ASSERT(*atoms != NULL);
-  ASSERT(*pynblist != NULL);
+  assert(*atoms != NULL);
+  assert(*pynblist != NULL);
 }
 
 PyObject *GetSecondaryNeighborList(PyObject *pyatoms, double rCut)
 {
   // Create the neighor list by calling PyAsap_NewFullNeighborList, taking
   // python objects as arguments, rather than the usual C++ creation function
   // (in this case PyAsap_NewSecondaryNeighborLocator) taking C++ arguments.
   // This is because the Python function is wrapped in the outher Module
   // layer, so it works correctly also in parallel simulations (includes
   // ghost atoms correctly).
   PyObject *args = Py_BuildValue("(dOd)", rCut, pyatoms, 0.0);
-  ASSERT(args != NULL);  // How could this fail?
+  assert(args != NULL);  // How could this fail?
   PyObject *kwargs = PyDict_New();
-  ASSERT(kwargs != NULL);
+  assert(kwargs != NULL);
   PyObject *nblist = PyAsap_NewNeighborCellLocator_Py(NULL, args, kwargs);
   Py_DECREF(args);
   Py_DECREF(kwargs);
   return nblist;
 }
```

### Comparing `asap3-3.13.1/Tools/GetNeighborList.h` & `asap3-3.9.6/Tools/GetNeighborList.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Tools/RawRadialDistribution.cpp` & `asap3-3.9.6/Tools/RawRadialDistribution.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -48,42 +48,42 @@
 #if 0
   // Check that the group array is meaningful  XXX THIS LOOKS WRONG! Loop over atoms!
   for (int i = 0; i < nGroups; i++)
     if (group[i] < 0 || group[i] >= nGroups)
       throw AsapError("Invalid group for atom ") << i << ": " << group[i];
 #endif
   
-  ASSERT(result.size() == nGroups);
-  ASSERT(counts.size() == nGroups);
+  assert(result.size() == nGroups);
+  assert(counts.size() == nGroups);
 
 #if 0
   // Check that the output data is zero.
   typedef map< pair<int,int>, long* >::const_iterator iter1;
   typedef map<int,long>::const_iterator iter2;
   for (int i = 0; i < nGroups; i++)
     {
       for (iter1 j = result[i].begin(); j != result[i].end(); ++j)
 	{
 	  cerr << "Checking group " << i << " " << j->first.first << ", "
 	       << j->first.second << endl;
 	  for (int k = 0; k < nBins; k++)
-	    ASSERT(j->second[k] == 0);
+	    assert(j->second[k] == 0);
 	}
       for (iter2 j = counts[i].begin(); j != counts[i].end(); ++j)
-	ASSERT(j->second == 0);
+	assert(j->second == 0);
     }    
 #endif
   
   // Create a neighbor list that can access the atoms.
   PyObject *py_nblist = GetSecondaryNeighborList(pyatoms, rCut);
   if (py_nblist == NULL)
     throw AsapPythonError();
   NeighborLocator *nblist = ((PyAsap_NeighborLocatorObject*)py_nblist)->cobj;
   Atoms *atoms = nblist->GetAtoms();
-  ASSERT(atoms != NULL);
+  assert(atoms != NULL);
   atoms->Begin(pyatoms);
   
   // Get some info about the atoms
   const asap_z_int *z = atoms->GetAtomicNumbers();
   int nAtoms = atoms->GetNumberOfAtoms();
 
 #if 0
@@ -106,25 +106,25 @@
   for (int atom = 0; atom < nAtoms; atom++)
     {
       counts[group[atom]][z[atom]] += 1;        // Count the atom
       forward.first = reverse.second = z[atom];
       int maxnb2 = maxnb;  // Will be changed by the next line
       int nnb = nblist->GetNeighbors(atom, &other[0], &rnb[0], &sqdist[0],
 				     maxnb2, rCut);
-      ASSERT(nnb < maxnb);
+      assert(nnb < maxnb);
       // Loop over neighbors
       for (int i = 0; i < nnb; i++)
 	{
 	  int nb = other[i];
 	  double r = sqrt(sqdist[i]);
 	  int bin = int(r/deltaR);
 	  if (bin >= nBins)
 	    {
 	      // If r == rCut, bin==nBins.  Discard this case.
-	      ASSERT(bin == nBins);  
+	      assert(bin == nBins);  
 	      break;
 	    }
 	  forward.second = reverse.first = z[nb];
 	  result[group[atom]][forward][bin] += 1;
 	  // Check if the neighbor is a ghost
 	  if (nb < nAtoms)
 	    {
```

### Comparing `asap3-3.13.1/Tools/RawRadialDistribution.h` & `asap3-3.9.6/Tools/RawRadialDistribution.h`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/Tools/SecondaryNeighborLocator.cpp` & `asap3-3.9.6/Tools/SecondaryNeighborLocator.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -34,93 +34,66 @@
 // neighbor locator then uses the primary locator to keep the ghost atoms
 // updated.  It is thus an error if the secondary neighbor locator has
 // longer range than the primary.  If no primary locator is present, the
 // secondary will handle ghost atoms itself, until a primary locator appears
 // when/if the user later adds a potential.
 
 #include "SecondaryNeighborLocator.h"
-#include "Potential.h"
 //#define ASAPDEBUG
 #include "Debug.h"
 
 bool SecondaryNeighborLocator::CheckAndUpdateNeighborList(PyObject *atoms_obj)
 {
-  DEBUGPRINT;
-  // If there are ghost atoms (a parallel simulation), then we may need to
-  // use the master neighbor list to update the ghosts.
-  if (atoms->HasGhostAtoms())
-  {
-    // Check if there is a calculator and it is an Asap Potential.  If so,
-    // use it to update the master neighbor list.  And use its access object.
-    py_master = PyObject_GetAttrString(atoms_obj, "calc");
-    if (py_master == NULL)
-      PyErr_Clear();
-    else if (!PyAsap_PotentialCheck(py_master))
-      Py_CLEAR(py_master);  // Calculator is no good.
-  }
-  else
-  {
-    py_master = NULL;  // No ghosts, no need to involve a master neighbor list.
-  }
-  bool update = false;
+  // Check if there is a master neighbor list.  If so, use its access object.
+  py_master = atoms->GetPrimaryNbLocator(atoms_obj);
   if (py_master != NULL)
-  {
-    // Get the access object from the Potential
-    DEBUGPRINT;
-    Potential *master = ((PyAsap_PotentialObject *) py_master)->cobj;
-    Atoms *newatoms = master->GetAtoms();
-    ASSERT(newatoms != NULL);
-    if (newatoms != atoms)
-    {
-      // Replace access object with this one.
-      DEBUGPRINT;
-      AsapAtoms_INCREF(newatoms);
-      AsapAtoms_DECREF(atoms);
-      atoms = newatoms;
-    }
-
-    // Update the master neighbor list
-    DEBUGPRINT;
-    if (master->GetCutoffRadius() < this->GetCutoffRadiusWithDrift())
-      throw AsapError("Attempting to create a secondary neighbor list with larger cutoff than the master list: ")
-	<<  this->GetCutoffRadiusWithDrift() << " versus " << master->GetCutoffRadius();
-    update = master->CheckAndUpdateNbList(atoms_obj);
-    
-    // If the master list did not need an update, we may still need it.
-    atoms->Begin(atoms_obj);
-    if (!update)
     {
-      DEBUGPRINT;
-      update = NeighborCellLocator::CheckNeighborList();
+      NeighborLocator *master = ((PyAsap_NeighborLocatorObject *) py_master)->cobj;
+      Atoms *newatoms = master->GetAtoms();
+      assert(newatoms != NULL);
+      if (newatoms != atoms)
+        {
+          // Replace access object with this one.
+          AsapAtoms_INCREF(newatoms);
+          AsapAtoms_DECREF(atoms);
+          atoms = newatoms;
+        }
     }
-    DEBUGPRINT;
-    if (invalid || update)
-      UpdateNeighborList();
-    atoms->End();
-    DEBUGPRINT;
-  }
-  else
-  {
-    // No master.  We must handle ghost atoms and migration here.
-    DEBUGPRINT;
-    atoms->Begin(atoms_obj);
-    bool update = NeighborCellLocator::CheckNeighborList();
-    update = atoms->UpdateBeforeCalculation(update, rCut);
-    DEBUGPRINT;
-    if (invalid || update)
-      UpdateNeighborList();
-    atoms->End();
-    DEBUGPRINT;
-  }
-
-  ASSERT(!IsInvalid());
+  bool updated = NeighborCellLocator::CheckAndUpdateNeighborList(atoms_obj);
   Py_XDECREF(py_master);
   py_master = NULL;
-  return update;
-};
-  
+  return updated;
+}
+
 bool SecondaryNeighborLocator::CheckNeighborList()
 {
   DEBUGPRINT;
-  throw AsapError("SecondaryNeighborLocator::CheckNeighborList() called directly.");
+  if (py_master)
+    {
+      DEBUGPRINT;
+      NeighborLocator *master = ((PyAsap_NeighborLocatorObject *) py_master)->cobj;
+      assert(master != NULL);
+      if (master->GetCutoffRadius() < this->GetCutoffRadiusWithDrift())
+        throw AsapError("Attempting to create a secondary neighbor list with larger cutoff than the master list: ")
+          <<  this->GetCutoffRadiusWithDrift() << " versus " << master->GetCutoffRadius();
+      DEBUGPRINT;
+      bool masterupdate = master->CheckNeighborList();
+      // May communicate
+      DEBUGPRINT;
+      masterupdate = atoms->UpdateBeforeCalculation(masterupdate,
+                                                    master->GetCutoffRadiusWithDrift());
+      DEBUGPRINT;
+      if (masterupdate)
+        master->UpdateNeighborList();
+      DEBUGPRINT;
+      return NeighborCellLocator::CheckNeighborList();
+    }
+  else
+    {
+      // No master.  We must handle ghost atoms and migration here.
+      DEBUGPRINT;
+      bool update = NeighborCellLocator::CheckNeighborList();
+      update = atoms->UpdateBeforeCalculation(update, rCut);
+      DEBUGPRINT;
+      return update;
+    }
 }
-
```

### Comparing `asap3-3.13.1/Tools/SecondaryNeighborLocator.h` & `asap3-3.9.6/Tools/SecondaryNeighborLocator.h`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     NeighborCellLocator(a, rCut, driftfactor)
   {includeghostneighbors = true; py_master = NULL;}
   virtual ~SecondaryNeighborLocator() {};
 
   friend PyAsap_NeighborLocatorObject *PyAsap_NewSecondaryNeighborLocator(
        Atoms *a, double rCut, double driftfactor);
 
-  friend void PyAsap_Finalize<PyAsap_NeighborLocatorObject>(PyObject *self);
+  friend void PyAsap_Dealloc<PyAsap_NeighborLocatorObject>(PyObject *self);
 
 public:
   /// Check the neighbor list.
   ///
   /// Check if the neighbor list can still be reused, return true if
   /// it should be updated.  Before checking, check AND UPDATE the master
   /// neighbor list, if present.
```

### Comparing `asap3-3.13.1/depend.CHANGES` & `asap3-3.9.6/depend.CHANGES`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,7 @@
 03Nov14   3.7.9      Moved numerous headerfiles around for OpenKIMcalculator.
 09Nov14   3.8.0      Remove ParallelAtoms.h accidentally included from ImagePotential.cpp
 18Dec14   3.8.5      Add the MetalOxideInterface potential.
 02Jun15   3.8.9      Parameter support for the OpenKIM models.
 30Jul15   3.8.10     Added SecondaryNeighborList.
 22Mar16	  3.8.16     Added polyhedral template matching.
 11Oct16	  3.9.4	     Countless changes, including new build system for PTM.
-22Feb18	  3.10.9     New header files in PTM module.
-01May18   3.10.10    Remove C++11 requirement.
-21Aug18	  3.11.0     Remove OpenKIMinfo.h when updating to OpenKIM version 2.X
-24Aug18	  3.11.1     Move potentials into their own folder.
-17Mar20	  3.12.0     Refactor MPI communicator code.
-19Mar21    3.12.3     MPI module imports Templates.h
-05Apr21    3.12.4     CoordinationNumbers.cpp includes Debug.h
-16Apr21	  3.12.6     SecondaryNeigborLocator.cpp includes Potential.h
```

### Comparing `asap3-3.13.1/getconfig.py` & `asap3-3.9.6/getconfig.py`

 * *Files identical despite different names*

### Comparing `asap3-3.13.1/makefile-Darwin-x86_64` & `asap3-3.9.6/makefile-Darwin-x86_64`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # Mac OS X with the GNU compilers
-
-PYTHON=python3
-#BINPARALLEL = asap-python
-
-# This should match what was used to build OpenKIM !
 CC=gcc
 CXX=g++
 #OPENMPFLAGS=-fopenmp
-#CFLAGS = -O3 -pipe -g -Wall -Wno-sign-compare -Wno-unused-function -Wno-write-strings -Wno-terminate
 CFLAGS = -O3 -pipe -g -Wall -Wno-sign-compare -Wno-unused-function -Wno-write-strings
 CXXFLAGS = $(CFLAGS)
 PARPOSTFIX = -par
 MPICFLAGS = $(CFLAGS) $(OPENMPFLAGS)
 MPICXXFLAGS = $(MPICFLAGS)
 
 # Extra flags to silence compiler warnings in Interface and ParallelInterface
 IFACEFLAGS = -Wno-strict-aliasing
 BRENNERCFLAGS =  -Wno-strict-aliasing -Wno-unused
 #LIBS = -lm -lgomp
 LIBS = -lm
 CSRC_EXTRA = 
 MPIINCLUDES=
 CXXSHARED = $(CXX) -bundle -undefined dynamic_lookup
-MPICXXSHARED = $(MPICXX) -bundle -undefined dynamic_lookup
 CXXFLAGSGPROF = -O3 -g -fPIC -pg
 CXXFLAGSDEBUG = -O3 -tpp7 -xW -g
 DEPENDFLAG = -MM
 DEPENDCLEAN = sed -e 's@/usr/[^ ]*@@g' | sed -e '/^ *\\ *$$/d'
 CPP_LIB="/usr/lib/libstdc++.so.6"
 EXTRA_LIBS = $(OPENMPFLAGS)
-
-
+# When using homebrew's Python the LINKFORSHARED variable gets set to nonsense. 
+LINKFORSHARED =
```

### Comparing `asap3-3.13.1/makefile-Linux-x86_64-gnu` & `asap3-3.9.6/makefile-Linux-x86_64-gnu`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 # Uncomment to enable OpenMP support
 #OPENMPFLAGS = -openmp
 
 # C and C++ compiler and compilation flags.  You enable OpenMP support here.
 # OpenMP is currently only supported in the parallel version.
 CC=gcc
 CXX=g++
-CFLAGS = -O3 -g -march=native -m64 -pipe -fPIC -ffast-math -Wall -Wno-sign-compare -Wno-unused-function -Wno-terminate
-CXXFLAGS = $(CFLAGS)
-
-ASAP_SET_RPATH=-Wl,-rpath=
+CFLAGS = -O3 -g -march=native -m64 -pipe -fPIC -ffast-math -Wall -Wno-sign-compare -Wno-unused-function
+CXXFLAGS = -std=c++11 $(CFLAGS)
 
 # Compilation flags for parallel simulations
 MPICFLAGS = $(CFLAGS) $(OPENMPFLAGS)
 MPICXXFLAGS = $(MPICFLAGS)
 
 # Extra libraries and flags needed when linking the executable for parallel simulations
 EXTRA_LIBS =  $(OPENMPFLAGS)
```

### Comparing `asap3-3.13.1/makefile-Linux-x86_64-intel` & `asap3-3.9.6/makefile-Linux-x86_64-intel`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #### Python executable.  Uncomment and set to python3 to compile for Python 3
 #PYTHON=python
 
 
 #### Compilers and compilation flags
 
 # Uncomment to enable OpenMP support
-#OPENMPFLAGS = -openmp
+OPENMPFLAGS = -openmp
 
 # C and C++ compiler and compilation flags.  You enable OpenMP support here.
 # OpenMP is currently only supported in the parallel version.
 CC=icc
 CXX=icpc
 CFLAGS = -O3 -g -xHost -fPIC
-CXXFLAGS = $(CFLAGS)
+CXXFLAGS = -std=c++11 $(CFLAGS)
 LIBS = -lsvml -lm 
 
 # Compilation flags for parallel simulations
-MPICFLAGS = -O3 -g -xHost $(OPENMPFLAGS)
-MPICXXFLAGS = $(MPICFLAGS)
+MPICFLAGS = -O3 -g -xHost -fast $(OPENMPFLAGS)
+MPICXXFLAGS = -std=c++11 $(MPICFLAGS)
 EXTRA_LIBS =  $(OPENMPFLAGS)
 
 # Enable PARPOSTFIX if the compilation flags for parallel and serial code is different.
 PARPOSTFIX = -par
 
 # Extra flags to silence compiler warnings in Interface and ParallelInterface
 #IFACEFLAGS = -Wno-write-strings -Wno-strict-aliasing
```

### Comparing `asap3-3.13.1/makefile-local-gcc-svml` & `asap3-3.9.6/makefile-niflheim6`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,48 @@
 ########################################################################################
-#### Generic configuration file for Linux with x86_64 processor and the GNU compiler
+#### Configuration file for DTU Physics' cluster Niflheim.
 ####
-#### Please do not edit this file to configure - instead make a copy called
-#### makefile-default or makefile-HOSTNAME and edit that file.
+#### This uses the Intel compilers
 ####
 
+
 #### Override object directories to separate similar architectures.
 OBJDIR = $(FYS_PLATFORM)$(POSTFIX)
 BINDIR = $(OBJDIR)
 $(info FYS_PLATFORM detected - building for CAMd/CINF/Niflheim with OBJDIR=$(OBJDIR).)
 
 
-
 #### Python executable.  Uncomment and set to python3 to compile for Python 3
 #PYTHON=python
 
 
 #### Compilers and compilation flags
 
 # Uncomment to enable OpenMP support
 #OPENMPFLAGS = -openmp
+OPENMPFLAGS = 
 
 # C and C++ compiler and compilation flags.  You enable OpenMP support here.
 # OpenMP is currently only supported in the parallel version.
-CC=gcc
-CXX=g++
-CFLAGS = -O3 -g -march=native -fPIC -ffast-math -Wall -Wno-sign-compare -Wno-unused-function -ftree-vectorize -funsafe-math-optimizations -mveclibabi=svml 
-CXXFLAGS = $(CFLAGS)
+CC=icc
+CXX=icpc
+CFLAGS = -O3 -g -xHost -fPIC -qopt-report=5 -qopt-report-phase=vec
+CXXFLAGS = -std=c++11 $(CFLAGS)
 LIBS = -lsvml -lm 
 
 # Compilation flags for parallel simulations
-MPICFLAGS = $(CFLAGS) $(OPENMPFLAGS)
-MPICXXFLAGS = $(MPICFLAGS)
-
-# Extra libraries and flags needed when linking the executable for parallel simulations
+MPICFLAGS = -O3 -g -xHost $(OPENMPFLAGS)
+MPICXXFLAGS = -std=c++11 $(MPICFLAGS)
 EXTRA_LIBS =  $(OPENMPFLAGS)
 
 # Enable PARPOSTFIX if the compilation flags for parallel and serial code is different,
 # e.g. if to OpenMP is enabled in one case.
-ifdef OPENMPFLAGS
 PARPOSTFIX = -par
-endif
 
 # Extra flags to silence compiler warnings in Interface and ParallelInterface
 IFACEFLAGS = -Wno-write-strings -Wno-strict-aliasing
 
 # Extra flags to silence compiler warning for the Brenner potential
 BRENNERCFLAGS =  -Wno-strict-aliasing -Wno-unused
 
 
-#### Compilation flags and command that may need to be changed on special architectures.
-#### The values in the comments are a good starting point.
-
-# Compilation command for linking shared object
-#CXXSHARED = $(CXX) -shared
-
-# Libraries for linkage.  LIBS is for both serial and parallel version, EXTRA_LIBS is for parallel only.
-#LIBS = -lm
-
-# Dependency generation
-#DEPENDFLAG = -MM
-#DEPENDCLEAN = sed -e 's@/usr/[^ ]*@@g' | sed -e '/^ *\\ *$$/d'
 
-EXTRA_LIBS =  -lreadline -lsvml
```

### Comparing `asap3-3.13.1/recordversion.py` & `asap3-3.9.6/recordversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Writes the version.c file containing version information.
 
 Usage:  call from makefile like this:
   python recordversion.py '$(VERSION)' 'edition' '$(CXX)' '$(CXXFLAGS)' > version.cpp
 where edition specifies serial or parallel editions.
 """
+from __future__ import print_function
 
 from time import *
 from sys import argv
 import os
 
 contents = '''
 // version.cpp
@@ -32,23 +33,22 @@
 {
   return "%s";
 }
 
 } // end namespace
 '''
 
-if __name__ == '__main__':
-    assert(len(argv) == 5)
-    version = argv[1]
-    edition = argv[2]
-    if argv[4] != "":
-        compiler = argv[3] + " " + argv[4]
-    else:
-        compiler = argv[3]
-    #when = strftime("%Y-%m-%d %H:%M", localtime(time()))
-    try:
-        host = os.uname()[1]
-    except:
-        host = 'unknown'
+assert(len(argv) == 5)
+version = argv[1]
+edition = argv[2]
+if argv[4] != "":
+    compiler = argv[3] + " " + argv[4]
+else:
+    compiler = argv[3]
+#when = strftime("%Y-%m-%d %H:%M", localtime(time()))
+try:
+    host = os.uname()[1]
+except:
+    host = 'unknown'
 
 
-    print(contents % (version, edition, host, compiler, version))
+print(contents % (version, edition, host, compiler, version))
```

### Comparing `asap3-3.13.1/scripts/asap-qsub` & `asap3-3.9.6/scripts/asap-qsub`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/python
 # Emacs: This is -*- python -*-
 
 """asap-qsub: Submit an Asap job to Niflheim.
 
 Usage:
     asap-qsub [options] job.py [job-command-line]
 
@@ -11,15 +11,14 @@
 
 In addition to the usual qsub options, an option of the form --ASAP=X
 may be passed, where X is one of the letters S, P or T specifying a
 serial, parallel or multithreaded application (overriding the usual
 detection).
 """
 
-from __future__ import print_function
 import sys
 import os
 import string
 import copy
 import subprocess
 import time
```

