# Comparing `tmp/ocsmesh-1.3.2.tar.gz` & `tmp/ocsmesh-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsmesh-1.3.2.tar", last modified: Tue Jun 13 16:24:26 2023, max compression
+gzip compressed data, was "ocsmesh-1.3.3.tar", last modified: Tue Jun 20 14:25:19 2023, max compression
```

## Comparing `ocsmesh-1.3.2.tar` & `ocsmesh-1.3.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.460197 ocsmesh-1.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.464197 ocsmesh-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/functional_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/functional_test_2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.464197 ocsmesh-1.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/noaa_33879_DS1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.468197 ocsmesh-1.3.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.size_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.468197 ocsmesh-1.3.2/ocsmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/mesh_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/remesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/remesh_by_shape_factor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23104 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/subset_n_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/linefeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/shapely.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/hfun/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/ocsmesh/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/ocsmesh/mesh/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/parsers/grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/parsers/sms2dm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/ocsmesh/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/ops/combine_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/ops/combine_hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    64799 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    68014 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.464197 ocsmesh-1.3.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/geom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30865 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/cli/build_geom.sh
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/cli/build_hfun.sh
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/cli/remesh_by_dem.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.085631 ocsmesh-1.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.089631 ocsmesh-1.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/functional_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/functional_test_2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.089631 ocsmesh-1.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/noaa_33879_DS1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.size_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/ocsmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/ocsmesh/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/mesh_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/remesh_by_shape_factor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23645 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/subset_n_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/linefeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/shapely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/hfun/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/mesh/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/parsers/grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/parsers/sms2dm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/ops/combine_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/ops/combine_hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64799 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68014 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/ocsmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.085631 ocsmesh-1.3.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30865 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/cli/build_geom.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/cli/build_hfun.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/cli/remesh_by_dem.sh
```

### Comparing `ocsmesh-1.3.2/.github/workflows/documentation.yml` & `ocsmesh-1.3.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/.github/workflows/functional_test.yml` & `ocsmesh-1.3.3/.github/workflows/functional_test.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/.github/workflows/functional_test_2.yml` & `ocsmesh-1.3.3/.github/workflows/functional_test_2.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/.github/workflows/pylint.yml` & `ocsmesh-1.3.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/.github/workflows/release.yml` & `ocsmesh-1.3.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/.gitignore` & `ocsmesh-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/.pylintrc` & `ocsmesh-1.3.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/LICENSE` & `ocsmesh-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/PKG-INFO` & `ocsmesh-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.2
+Version: 1.3.3
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
@@ -181,15 +181,15 @@
 python ./setup.py install_jigsaw # To install latest Jigsaw from GitHub
 python ./setup.py install # Installs the OCSMesh library to the current Python environment
 # OR
 python ./setup.py develop # Run this if you are a developer.
 ```
 
 #### Requirements
-* 3.7 <= Python < 3.10
+* 3.9 <= Python
 * CMake 
 * C/C++ compilers
 
 ## How to Cite
 Title : OCSMesh: a data-driven automated unstructured mesh generation software for coastal ocean modeling
 
 Personal Author(s) : Mani, Soroosh;Calzada, Jaime R.;Moghimi, Saeed;Zhang, Y. Joseph;Myers, Edward;Pe’eri, Shachak;
```

### Comparing `ocsmesh-1.3.2/README.md` & `ocsmesh-1.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 python ./setup.py install_jigsaw # To install latest Jigsaw from GitHub
 python ./setup.py install # Installs the OCSMesh library to the current Python environment
 # OR
 python ./setup.py develop # Run this if you are a developer.
 ```
 
 #### Requirements
-* 3.7 <= Python < 3.10
+* 3.9 <= Python
 * CMake 
 * C/C++ compilers
 
 ## How to Cite
 Title : OCSMesh: a data-driven automated unstructured mesh generation software for coastal ocean modeling
 
 Personal Author(s) : Mani, Soroosh;Calzada, Jaime R.;Moghimi, Saeed;Zhang, Y. Joseph;Myers, Edward;Pe’eri, Shachak;
```

### Comparing `ocsmesh-1.3.2/docs/Makefile` & `ocsmesh-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/docs/make.bat` & `ocsmesh-1.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/docs/noaa_33879_DS1.pdf` & `ocsmesh-1.3.3/docs/noaa_33879_DS1.pdf`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/docs/source/conf.py` & `ocsmesh-1.3.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/__init__.py` & `ocsmesh-1.3.3/ocsmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/__main__.py` & `ocsmesh-1.3.3/ocsmesh/__main__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/cli/cli.py` & `ocsmesh-1.3.3/ocsmesh/cli/cli.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/cli/mesh_upgrader.py` & `ocsmesh-1.3.3/ocsmesh/cli/mesh_upgrader.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/cli/remesh.py` & `ocsmesh-1.3.3/ocsmesh/cli/remesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/cli/remesh_by_shape_factor.py` & `ocsmesh-1.3.3/ocsmesh/cli/remesh_by_shape_factor.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/cli/subset_n_combine.py` & `ocsmesh-1.3.3/ocsmesh/cli/subset_n_combine.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,29 @@
 #        hfun=jig_hfun,
             init=jig_init
             )
 
         jig_mesh.value = np.zeros((jig_mesh.vert2.shape[0], 1))
         self._transform_mesh(jig_mesh, crs)
 
+        # NOTE: Remove out of domain elements (some corner cases!)
+        elems = jig_mesh.tria3['index']
+        coord = jig_mesh.vert2['coord']
+
+        gdf_elems = gpd.GeoDataFrame(
+            geometry=[Polygon(tri) for tri in coord[elems]],
+            crs=jig_mesh.crs
+        )
+        idx = gdf_elems.representative_point().sindex.query(
+            seam.get_multipolygon(), predicate='intersects'
+        )
+        flag = np.zeros(len(gdf_elems), dtype=bool)
+        flag[idx] = True
+        jig_mesh.tria3 = jig_mesh.tria3[flag]
+
         return jig_mesh
 
 
     def _transform_mesh(self, mesh, out_crs):
 
         transformer = Transformer.from_crs(
             mesh.crs, out_crs, always_xy=True)
```

### Comparing `ocsmesh-1.3.2/ocsmesh/cmd.py` & `ocsmesh-1.3.3/ocsmesh/cmd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/db.py` & `ocsmesh-1.3.3/ocsmesh/db.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/driver.py` & `ocsmesh-1.3.3/ocsmesh/driver.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/features/channel.py` & `ocsmesh-1.3.3/ocsmesh/features/channel.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/features/constraint.py` & `ocsmesh-1.3.3/ocsmesh/features/constraint.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/features/contour.py` & `ocsmesh-1.3.3/ocsmesh/features/contour.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/features/linefeature.py` & `ocsmesh-1.3.3/ocsmesh/features/linefeature.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/features/patch.py` & `ocsmesh-1.3.3/ocsmesh/features/patch.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/figures.py` & `ocsmesh-1.3.3/ocsmesh/figures.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/geom/base.py` & `ocsmesh-1.3.3/ocsmesh/geom/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/geom/collector.py` & `ocsmesh-1.3.3/ocsmesh/geom/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/geom/geom.py` & `ocsmesh-1.3.3/ocsmesh/geom/geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/geom/mesh.py` & `ocsmesh-1.3.3/ocsmesh/geom/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/geom/raster.py` & `ocsmesh-1.3.3/ocsmesh/geom/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/geom/shapely.py` & `ocsmesh-1.3.3/ocsmesh/geom/shapely.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/hfun/base.py` & `ocsmesh-1.3.3/ocsmesh/hfun/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/hfun/collector.py` & `ocsmesh-1.3.3/ocsmesh/hfun/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/hfun/hfun.py` & `ocsmesh-1.3.3/ocsmesh/hfun/hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/hfun/mesh.py` & `ocsmesh-1.3.3/ocsmesh/hfun/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/hfun/raster.py` & `ocsmesh-1.3.3/ocsmesh/hfun/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/interp.py` & `ocsmesh-1.3.3/ocsmesh/interp.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/mesh/base.py` & `ocsmesh-1.3.3/ocsmesh/mesh/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/mesh/mesh.py` & `ocsmesh-1.3.3/ocsmesh/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/mesh/parsers/grd.py` & `ocsmesh-1.3.3/ocsmesh/mesh/parsers/grd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/mesh/parsers/sms2dm.py` & `ocsmesh-1.3.3/ocsmesh/mesh/parsers/sms2dm.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/ops/combine_geom.py` & `ocsmesh-1.3.3/ocsmesh/ops/combine_geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/ops/combine_hfun.py` & `ocsmesh-1.3.3/ocsmesh/ops/combine_hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/raster.py` & `ocsmesh-1.3.3/ocsmesh/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh/utils.py` & `ocsmesh-1.3.3/ocsmesh/utils.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/ocsmesh.egg-info/PKG-INFO` & `ocsmesh-1.3.3/ocsmesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.2
+Version: 1.3.3
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
@@ -181,15 +181,15 @@
 python ./setup.py install_jigsaw # To install latest Jigsaw from GitHub
 python ./setup.py install # Installs the OCSMesh library to the current Python environment
 # OR
 python ./setup.py develop # Run this if you are a developer.
 ```
 
 #### Requirements
-* 3.7 <= Python < 3.10
+* 3.9 <= Python
 * CMake 
 * C/C++ compilers
 
 ## How to Cite
 Title : OCSMesh: a data-driven automated unstructured mesh generation software for coastal ocean modeling
 
 Personal Author(s) : Mani, Soroosh;Calzada, Jaime R.;Moghimi, Saeed;Zhang, Y. Joseph;Myers, Edward;Pe’eri, Shachak;
```

### Comparing `ocsmesh-1.3.2/ocsmesh.egg-info/SOURCES.txt` & `ocsmesh-1.3.3/ocsmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/pyproject.toml` & `ocsmesh-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/setup.py` & `ocsmesh-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/tests/api/common.py` & `ocsmesh-1.3.3/tests/api/common.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/tests/api/driver.py` & `ocsmesh-1.3.3/tests/api/driver.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/tests/api/features.py` & `ocsmesh-1.3.3/tests/api/features.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/tests/api/geom.py` & `ocsmesh-1.3.3/tests/api/geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/tests/api/hfun.py` & `ocsmesh-1.3.3/tests/api/hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/tests/api/mesh.py` & `ocsmesh-1.3.3/tests/api/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.2/tests/api/utils.py` & `ocsmesh-1.3.3/tests/api/utils.py`

 * *Files identical despite different names*

