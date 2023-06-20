# Comparing `tmp/SPLayout-0.4.6.tar.gz` & `tmp/SPLayout-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SPLayout-0.4.6.tar", last modified: Thu May  4 12:35:07 2023, max compression
+gzip compressed data, was "SPLayout-0.4.7.tar", last modified: Tue Jun 20 10:35:14 2023, max compression
```

## Comparing `SPLayout-0.4.6.tar` & `SPLayout-0.4.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/
--rw-rw-rw-   0        0        0     2146 2023-05-04 12:35:07.000000 SPLayout-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-02-23 14:51:36.000000 SPLayout-0.4.6/README.md
--rw-rw-rw-   0        0        0     1473 2023-02-23 14:51:44.000000 SPLayout-0.4.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/SPLayout.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2023-05-04 12:35:07.000000 SPLayout-0.4.6/SPLayout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 12:35:06.000000 SPLayout-0.4.6/SPLayout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 12:35:07.000000 SPLayout-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-02-23 14:06:17.000000 SPLayout-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/
--rw-rw-rw-   0        0        0     1987 2023-05-04 12:32:29.000000 SPLayout-0.4.6/splayout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/adjointmethod/
--rw-rw-rw-   0        0        0      293 2023-02-24 04:21:26.000000 SPLayout-0.4.6/splayout/adjointmethod/__init__.py
--rw-rw-rw-   0        0        0    10984 2023-02-23 12:33:21.000000 SPLayout-0.4.6/splayout/adjointmethod/adjointshapeopt.py
--rw-rw-rw-   0        0        0    10645 2023-05-04 11:28:32.000000 SPLayout-0.4.6/splayout/adjointmethod/adjointtopologyopt.py
--rw-rw-rw-   0        0        0    10586 2023-02-23 12:35:47.000000 SPLayout-0.4.6/splayout/adjointmethod/shaperegion2d.py
--rw-rw-rw-   0        0        0    10652 2023-02-23 12:35:57.000000 SPLayout-0.4.6/splayout/adjointmethod/shaperegion3d.py
--rw-rw-rw-   0        0        0    11374 2023-02-23 12:36:38.000000 SPLayout-0.4.6/splayout/adjointmethod/topologyregion2d.py
--rw-rw-rw-   0        0        0    11304 2023-05-04 05:46:43.000000 SPLayout-0.4.6/splayout/adjointmethod/topologyregion3d.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/algorithms/
--rw-rw-rw-   0        0        0      312 2023-05-04 05:08:40.000000 SPLayout-0.4.6/splayout/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5781 2022-01-04 05:22:28.000000 SPLayout-0.4.6/splayout/algorithms/binarybatalgorithm.py
--rw-rw-rw-   0        0        0     6360 2022-01-04 06:04:34.000000 SPLayout-0.4.6/splayout/algorithms/binarygeneticalgorithm.py
--rw-rw-rw-   0        0        0     5831 2023-05-04 05:07:54.000000 SPLayout-0.4.6/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-rw-rw-   0        0        0     4305 2023-02-23 12:22:49.000000 SPLayout-0.4.6/splayout/algorithms/directbinarysearchalgorithm.py
--rw-rw-rw-   0        0        0     7326 2023-05-04 05:08:40.000000 SPLayout-0.4.6/splayout/algorithms/particleswarmalgorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/components/
--rw-rw-rw-   0        0        0     3728 2023-02-23 12:38:12.000000 SPLayout-0.4.6/splayout/components/AEMDgrating.py
--rw-rw-rw-   0        0        0      714 2023-02-23 13:44:58.000000 SPLayout-0.4.6/splayout/components/__init__.py
--rw-rw-rw-   0        0        0     4403 2023-02-23 12:38:42.000000 SPLayout-0.4.6/splayout/components/bend.py
--rw-rw-rw-   0        0        0     9026 2023-02-23 12:39:10.000000 SPLayout-0.4.6/splayout/components/doubleconnector.py
--rw-rw-rw-   0        0        0     6092 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/filledpattern.py
--rw-rw-rw-   0        0        0    49359 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/microring.py
--rw-rw-rw-   0        0        0    21403 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/pixelsregion.py
--rw-rw-rw-   0        0        0     7433 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/polygon.py
--rw-rw-rw-   0        0        0    14219 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/quarbend.py
--rw-rw-rw-   0        0        0    18098 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/sbend.py
--rw-rw-rw-   0        0        0    13136 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/selfdefinecomponent.py
--rw-rw-rw-   0        0        0    28052 2023-02-23 12:43:30.000000 SPLayout-0.4.6/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-rw-rw-   0        0        0     7270 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/slowlyvaryingtaper.py
--rw-rw-rw-   0        0        0     6668 2023-02-23 14:27:24.000000 SPLayout-0.4.6/splayout/components/taper.py
--rw-rw-rw-   0        0        0     1269 2023-02-23 12:41:22.000000 SPLayout-0.4.6/splayout/components/text.py
--rw-rw-rw-   0        0        0     8908 2023-02-23 12:42:22.000000 SPLayout-0.4.6/splayout/components/waveguide.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/lumericalcommun/
--rw-rw-rw-   0        0        0       72 2023-02-23 12:26:37.000000 SPLayout-0.4.6/splayout/lumericalcommun/__init__.py
--rw-rw-rw-   0        0        0    77831 2023-04-15 14:25:50.000000 SPLayout-0.4.6/splayout/lumericalcommun/fdtdapi.py
--rw-rw-rw-   0        0        0    44213 2023-02-23 12:42:48.000000 SPLayout-0.4.6/splayout/lumericalcommun/modeapi.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:35:07.000000 SPLayout-0.4.6/splayout/utils/
--rw-rw-rw-   0        0        0       20 2023-02-23 12:27:14.000000 SPLayout-0.4.6/splayout/utils/__init__.py
--rw-rw-rw-   0        0        0    14788 2023-05-04 04:58:18.000000 SPLayout-0.4.6/splayout/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.186224 SPLayout-0.4.7/
+-rw-rw-rw-   0        0        0    35803 2023-06-20 10:20:16.000000 SPLayout-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0     1719 2023-06-20 10:35:14.186224 SPLayout-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1473 2023-06-20 10:20:16.000000 SPLayout-0.4.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.157477 SPLayout-0.4.7/SPLayout.egg-info/
+-rw-rw-rw-   0        0        0     1719 2023-06-20 10:35:14.000000 SPLayout-0.4.7/SPLayout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1489 2023-06-20 10:35:14.000000 SPLayout-0.4.7/SPLayout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:35:14.000000 SPLayout-0.4.7/SPLayout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-20 10:35:14.000000 SPLayout-0.4.7/SPLayout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 10:35:14.000000 SPLayout-0.4.7/SPLayout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:35:14.186224 SPLayout-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-06-20 10:20:16.000000 SPLayout-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.157477 SPLayout-0.4.7/splayout/
+-rw-rw-rw-   0        0        0     1987 2023-06-20 10:30:23.000000 SPLayout-0.4.7/splayout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.163556 SPLayout-0.4.7/splayout/adjointmethod/
+-rw-rw-rw-   0        0        0      293 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/adjointmethod/__init__.py
+-rw-rw-rw-   0        0        0    10984 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/adjointmethod/adjointshapeopt.py
+-rw-rw-rw-   0        0        0    10645 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/adjointmethod/adjointtopologyopt.py
+-rw-rw-rw-   0        0        0    10586 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/adjointmethod/shaperegion2d.py
+-rw-rw-rw-   0        0        0    10652 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/adjointmethod/shaperegion3d.py
+-rw-rw-rw-   0        0        0    11374 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/adjointmethod/topologyregion2d.py
+-rw-rw-rw-   0        0        0    11304 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/adjointmethod/topologyregion3d.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.168116 SPLayout-0.4.7/splayout/algorithms/
+-rw-rw-rw-   0        0        0      312 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5781 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/algorithms/binarybatalgorithm.py
+-rw-rw-rw-   0        0        0     6360 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/algorithms/binarygeneticalgorithm.py
+-rw-rw-rw-   0        0        0     5831 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-rw-rw-   0        0        0     4305 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-rw-rw-   0        0        0     7326 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/algorithms/particleswarmalgorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.181167 SPLayout-0.4.7/splayout/components/
+-rw-rw-rw-   0        0        0     3728 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/AEMDgrating.py
+-rw-rw-rw-   0        0        0      714 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/__init__.py
+-rw-rw-rw-   0        0        0     4403 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/bend.py
+-rw-rw-rw-   0        0        0     9026 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/doubleconnector.py
+-rw-rw-rw-   0        0        0     6092 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/filledpattern.py
+-rw-rw-rw-   0        0        0    49359 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/microring.py
+-rw-rw-rw-   0        0        0    21403 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/pixelsregion.py
+-rw-rw-rw-   0        0        0     7433 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/polygon.py
+-rw-rw-rw-   0        0        0    14219 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/quarbend.py
+-rw-rw-rw-   0        0        0    18098 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/sbend.py
+-rw-rw-rw-   0        0        0    13136 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/selfdefinecomponent.py
+-rw-rw-rw-   0        0        0    28052 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-rw-rw-   0        0        0     7270 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/slowlyvaryingtaper.py
+-rw-rw-rw-   0        0        0     6668 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/taper.py
+-rw-rw-rw-   0        0        0     1269 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/text.py
+-rw-rw-rw-   0        0        0     8908 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/components/waveguide.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.184067 SPLayout-0.4.7/splayout/lumericalcommun/
+-rw-rw-rw-   0        0        0       72 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/lumericalcommun/__init__.py
+-rw-rw-rw-   0        0        0    77889 2023-06-20 10:22:43.000000 SPLayout-0.4.7/splayout/lumericalcommun/fdtdapi.py
+-rw-rw-rw-   0        0        0    44213 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/lumericalcommun/modeapi.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:35:14.185123 SPLayout-0.4.7/splayout/utils/
+-rw-rw-rw-   0        0        0       20 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/utils/__init__.py
+-rw-rw-rw-   0        0        0    14788 2023-06-20 10:20:16.000000 SPLayout-0.4.7/splayout/utils/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SPLayout-0.4.6/PKG-INFO` & `SPLayout-0.4.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.4.6
+Version: 0.4.7
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
-License: UNKNOWN
-Description: SPLayout
-        ========
-        
-        |GitHub repository| |GitHub license|
-        
-        SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a package for silicon photonics structures design. It provides commonly used silicon photonics structure classes for fast integration and pixelized blocks for inverse design and optimization. Some inverse design algorithms are also integrated in it like DBS (Direct Binary Search) and BBA (Binary Bat Algorithm).
-        
-        The GDSII streaming is based on gdspy(https://github.com/heitzmann/gdspy) and FDTD simulation is executed on Ansys Lumerical.
-        
-        
-        Dependency
-        ----------
-        
-        -  Python 3.6+
-        -  gdspy
-        -  scipy
-        -  numpy
-        -  (Ansys Lumerical for FDTDSimulation and MODESimulation)
-        
-        Installation
-        ------------
-        
-        use pip:
-        
-        ::
-        
-            pip install splayout
-        
-        or download from the source and build/install with:
-        
-        ::
-        
-            python setup.py install
-        
-        Documentation
-        -------------
-        
-        The documentation can be found
-        `here <https://splayout.readthedocs.io/en/latest/>`__.
-        
-        
-        `History (Click Here) <https://github.com/Hideousmon/SPLayout/tree/main/history.md>`__
-        -------------------------------------------------------------------------------------------
-        
-        
-        .. |GitHub repository| image:: https://img.shields.io/badge/github-SPLayout-blue
-           :target: https://github.com/Hideousmon/SPLayout
-        .. |GitHub license| image:: https://img.shields.io/badge/lisence-GNU--3.0-green
-           :target: https://github.com/Hideousmon/SPLayout/blob/main/LICENSE
-        
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+SPLayout
+========
+
+|GitHub repository| |GitHub license|
+
+SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a package for silicon photonics structures design. It provides commonly used silicon photonics structure classes for fast integration and pixelized blocks for inverse design and optimization. Some inverse design algorithms are also integrated in it like DBS (Direct Binary Search) and BBA (Binary Bat Algorithm).
+
+The GDSII streaming is based on gdspy(https://github.com/heitzmann/gdspy) and FDTD simulation is executed on Ansys Lumerical.
+
+
+Dependency
+----------
+
+-  Python 3.6+
+-  gdspy
+-  scipy
+-  numpy
+-  (Ansys Lumerical for FDTDSimulation and MODESimulation)
+
+Installation
+------------
+
+use pip:
+
+::
+
+    pip install splayout
+
+or download from the source and build/install with:
+
+::
+
+    python setup.py install
+
+Documentation
+-------------
+
+The documentation can be found
+`here <https://splayout.readthedocs.io/en/latest/>`__.
+
+
+`History (Click Here) <https://github.com/Hideousmon/SPLayout/tree/main/history.md>`__
+-------------------------------------------------------------------------------------------
+
+
+.. |GitHub repository| image:: https://img.shields.io/badge/github-SPLayout-blue
+   :target: https://github.com/Hideousmon/SPLayout
+.. |GitHub license| image:: https://img.shields.io/badge/lisence-GNU--3.0-green
+   :target: https://github.com/Hideousmon/SPLayout/blob/main/LICENSE
+
```

### Comparing `SPLayout-0.4.6/README.rst` & `SPLayout-0.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/SPLayout.egg-info/PKG-INFO` & `SPLayout-0.4.7/SPLayout.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.4.6
+Version: 0.4.7
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
-License: UNKNOWN
-Description: SPLayout
-        ========
-        
-        |GitHub repository| |GitHub license|
-        
-        SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a package for silicon photonics structures design. It provides commonly used silicon photonics structure classes for fast integration and pixelized blocks for inverse design and optimization. Some inverse design algorithms are also integrated in it like DBS (Direct Binary Search) and BBA (Binary Bat Algorithm).
-        
-        The GDSII streaming is based on gdspy(https://github.com/heitzmann/gdspy) and FDTD simulation is executed on Ansys Lumerical.
-        
-        
-        Dependency
-        ----------
-        
-        -  Python 3.6+
-        -  gdspy
-        -  scipy
-        -  numpy
-        -  (Ansys Lumerical for FDTDSimulation and MODESimulation)
-        
-        Installation
-        ------------
-        
-        use pip:
-        
-        ::
-        
-            pip install splayout
-        
-        or download from the source and build/install with:
-        
-        ::
-        
-            python setup.py install
-        
-        Documentation
-        -------------
-        
-        The documentation can be found
-        `here <https://splayout.readthedocs.io/en/latest/>`__.
-        
-        
-        `History (Click Here) <https://github.com/Hideousmon/SPLayout/tree/main/history.md>`__
-        -------------------------------------------------------------------------------------------
-        
-        
-        .. |GitHub repository| image:: https://img.shields.io/badge/github-SPLayout-blue
-           :target: https://github.com/Hideousmon/SPLayout
-        .. |GitHub license| image:: https://img.shields.io/badge/lisence-GNU--3.0-green
-           :target: https://github.com/Hideousmon/SPLayout/blob/main/LICENSE
-        
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+SPLayout
+========
+
+|GitHub repository| |GitHub license|
+
+SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a package for silicon photonics structures design. It provides commonly used silicon photonics structure classes for fast integration and pixelized blocks for inverse design and optimization. Some inverse design algorithms are also integrated in it like DBS (Direct Binary Search) and BBA (Binary Bat Algorithm).
+
+The GDSII streaming is based on gdspy(https://github.com/heitzmann/gdspy) and FDTD simulation is executed on Ansys Lumerical.
+
+
+Dependency
+----------
+
+-  Python 3.6+
+-  gdspy
+-  scipy
+-  numpy
+-  (Ansys Lumerical for FDTDSimulation and MODESimulation)
+
+Installation
+------------
+
+use pip:
+
+::
+
+    pip install splayout
+
+or download from the source and build/install with:
+
+::
+
+    python setup.py install
+
+Documentation
+-------------
+
+The documentation can be found
+`here <https://splayout.readthedocs.io/en/latest/>`__.
+
+
+`History (Click Here) <https://github.com/Hideousmon/SPLayout/tree/main/history.md>`__
+-------------------------------------------------------------------------------------------
+
+
+.. |GitHub repository| image:: https://img.shields.io/badge/github-SPLayout-blue
+   :target: https://github.com/Hideousmon/SPLayout
+.. |GitHub license| image:: https://img.shields.io/badge/lisence-GNU--3.0-green
+   :target: https://github.com/Hideousmon/SPLayout/blob/main/LICENSE
+
```

### Comparing `SPLayout-0.4.6/SPLayout.egg-info/SOURCES.txt` & `SPLayout-0.4.7/SPLayout.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-README.md
+LICENSE
 README.rst
 setup.py
 SPLayout.egg-info/PKG-INFO
 SPLayout.egg-info/SOURCES.txt
 SPLayout.egg-info/dependency_links.txt
 SPLayout.egg-info/requires.txt
 SPLayout.egg-info/top_level.txt
```

### Comparing `SPLayout-0.4.6/setup.py` & `SPLayout-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/__init__.py` & `SPLayout-0.4.7/splayout/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
```

### Comparing `SPLayout-0.4.6/splayout/adjointmethod/adjointshapeopt.py` & `SPLayout-0.4.7/splayout/adjointmethod/adjointshapeopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/adjointmethod/adjointtopologyopt.py` & `SPLayout-0.4.7/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/adjointmethod/shaperegion2d.py` & `SPLayout-0.4.7/splayout/adjointmethod/shaperegion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/adjointmethod/shaperegion3d.py` & `SPLayout-0.4.7/splayout/adjointmethod/shaperegion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/adjointmethod/topologyregion2d.py` & `SPLayout-0.4.7/splayout/adjointmethod/topologyregion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/adjointmethod/topologyregion3d.py` & `SPLayout-0.4.7/splayout/adjointmethod/topologyregion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/algorithms/binarybatalgorithm.py` & `SPLayout-0.4.7/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/algorithms/binarygeneticalgorithm.py` & `SPLayout-0.4.7/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/algorithms/binaryparticleswarmalgorithm.py` & `SPLayout-0.4.7/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/algorithms/directbinarysearchalgorithm.py` & `SPLayout-0.4.7/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/algorithms/particleswarmalgorithm.py` & `SPLayout-0.4.7/splayout/algorithms/particleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/AEMDgrating.py` & `SPLayout-0.4.7/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/__init__.py` & `SPLayout-0.4.7/splayout/components/__init__.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/bend.py` & `SPLayout-0.4.7/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/doubleconnector.py` & `SPLayout-0.4.7/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/filledpattern.py` & `SPLayout-0.4.7/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/microring.py` & `SPLayout-0.4.7/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/pixelsregion.py` & `SPLayout-0.4.7/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/polygon.py` & `SPLayout-0.4.7/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/quarbend.py` & `SPLayout-0.4.7/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/sbend.py` & `SPLayout-0.4.7/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/selfdefinecomponent.py` & `SPLayout-0.4.7/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/simpleasymmetricdirectionalcoupler.py` & `SPLayout-0.4.7/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/slowlyvaryingtaper.py` & `SPLayout-0.4.7/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/taper.py` & `SPLayout-0.4.7/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/text.py` & `SPLayout-0.4.7/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/components/waveguide.py` & `SPLayout-0.4.7/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/lumericalcommun/fdtdapi.py` & `SPLayout-0.4.7/splayout/lumericalcommun/fdtdapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,17 @@
         -----
         This function will automatically add a power monitor at the same position with same shape.
         If use update_mode the monitor should be put after adding fdtd region and mesh region.
         If z_min and z_max are specified, the height property will be invalid.
         """
         position = tuple_to_point(position)
         power_monitor_name = expansion_name + "_expansion"
-        self.add_power_monitor(position, width=width, height=height, monitor_name=power_monitor_name, points=points,
-                               normal_direction=normal_direction)
+        self.add_power_monitor(position, width=width, height=height,
+                               z_min=z_min, z_max=z_max, monitor_name=power_monitor_name,
+                               points=points, normal_direction=normal_direction)
         self.fdtd.eval("addmodeexpansion;")
         self.fdtd.eval("set(\"name\",\"" + expansion_name + "\");")
         if (normal_direction == HORIZONTAL):
             self.fdtd.eval("set(\"monitor type\",1);")
             self.fdtd.eval("set(\"x\"," +  "%.6f"%(position.x) + "e-6);")
             self.fdtd.eval("set(\"y\"," +  "%.6f"%(position.y) + "e-6);")
             self.fdtd.eval("set(\"y span\"," +  "%.6f"%(width) + "e-6);")
```

### Comparing `SPLayout-0.4.6/splayout/lumericalcommun/modeapi.py` & `SPLayout-0.4.7/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.6/splayout/utils/utils.py` & `SPLayout-0.4.7/splayout/utils/utils.py`

 * *Files identical despite different names*

