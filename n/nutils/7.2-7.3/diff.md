# Comparing `tmp/nutils-7.2.tar.gz` & `tmp/nutils-7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutils-7.2.tar", last modified: Fri Nov  4 10:41:16 2022, max compression
+gzip compressed data, was "nutils-7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nutils-7.2.tar` & `nutils-7.3.tar`

### file list

```diff
@@ -1,47 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:41:16.833729 nutils-7.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-11-04 10:41:16.833729 nutils-7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-11-04 10:41:15.000000 nutils-7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:41:16.833729 nutils-7.2/nutils/
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-11-04 10:41:15.000000 nutils-7.2/nutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11164 2022-11-04 10:41:15.000000 nutils-7.2/nutils/_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    15035 2022-11-04 10:41:15.000000 nutils-7.2/nutils/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    15210 2022-11-04 10:41:15.000000 nutils-7.2/nutils/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-11-04 10:41:15.000000 nutils-7.2/nutils/debug_flags.py
--rw-r--r--   0 runner    (1001) docker     (121)    46150 2022-11-04 10:41:15.000000 nutils-7.2/nutils/element.py
--rw-r--r--   0 runner    (1001) docker     (121)    20862 2022-11-04 10:41:15.000000 nutils-7.2/nutils/elementseq.py
--rw-r--r--   0 runner    (1001) docker     (121)   174749 2022-11-04 10:41:15.000000 nutils-7.2/nutils/evaluable.py
--rw-r--r--   0 runner    (1001) docker     (121)     6838 2022-11-04 10:41:15.000000 nutils-7.2/nutils/export.py
--rw-r--r--   0 runner    (1001) docker     (121)    84274 2022-11-04 10:41:15.000000 nutils-7.2/nutils/expression_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    40199 2022-11-04 10:41:15.000000 nutils-7.2/nutils/expression_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)   139029 2022-11-04 10:41:15.000000 nutils-7.2/nutils/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:41:16.833729 nutils-7.2/nutils/matrix/
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-11-04 10:41:15.000000 nutils-7.2/nutils/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-04 10:41:15.000000 nutils-7.2/nutils/matrix/_auto.py
--rw-r--r--   0 runner    (1001) docker     (121)    13356 2022-11-04 10:41:15.000000 nutils-7.2/nutils/matrix/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14021 2022-11-04 10:41:15.000000 nutils-7.2/nutils/matrix/_mkl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-11-04 10:41:15.000000 nutils-7.2/nutils/matrix/_numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4267 2022-11-04 10:41:15.000000 nutils-7.2/nutils/matrix/_scipy.py
--rw-r--r--   0 runner    (1001) docker     (121)    31749 2022-11-04 10:41:15.000000 nutils-7.2/nutils/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    23008 2022-11-04 10:41:15.000000 nutils-7.2/nutils/numeric.py
--rw-r--r--   0 runner    (1001) docker     (121)     5767 2022-11-04 10:41:15.000000 nutils-7.2/nutils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    19541 2022-11-04 10:41:15.000000 nutils-7.2/nutils/points.py
--rw-r--r--   0 runner    (1001) docker     (121)    22402 2022-11-04 10:41:15.000000 nutils-7.2/nutils/pointsseq.py
--rw-r--r--   0 runner    (1001) docker     (121)    43599 2022-11-04 10:41:15.000000 nutils-7.2/nutils/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)    44018 2022-11-04 10:41:15.000000 nutils-7.2/nutils/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)    13225 2022-11-04 10:41:15.000000 nutils-7.2/nutils/sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)    11497 2022-11-04 10:41:15.000000 nutils-7.2/nutils/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)   147824 2022-11-04 10:41:15.000000 nutils-7.2/nutils/topology.py
--rw-r--r--   0 runner    (1001) docker     (121)    24673 2022-11-04 10:41:15.000000 nutils-7.2/nutils/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    38427 2022-11-04 10:41:15.000000 nutils-7.2/nutils/transformseq.py
--rw-r--r--   0 runner    (1001) docker     (121)    49559 2022-11-04 10:41:15.000000 nutils-7.2/nutils/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     6934 2022-11-04 10:41:15.000000 nutils-7.2/nutils/unit.py
--rw-r--r--   0 runner    (1001) docker     (121)    16461 2022-11-04 10:41:15.000000 nutils-7.2/nutils/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-11-04 10:41:15.000000 nutils-7.2/nutils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:41:16.833729 nutils-7.2/nutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-11-04 10:41:16.000000 nutils-7.2/nutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-11-04 10:41:16.000000 nutils-7.2/nutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 10:41:16.000000 nutils-7.2/nutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-04 10:41:16.000000 nutils-7.2/nutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-04 10:41:16.000000 nutils-7.2/nutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 10:41:16.833729 nutils-7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-11-04 10:41:15.000000 nutils-7.2/setup.py
+-rw-r--r--   0        0        0       13 2023-06-20 07:52:04.243517 nutils-7.3/.codecov.yml
+-rw-r--r--   0        0        0       58 2023-06-20 07:52:04.243517 nutils-7.3/.coveragerc
+-rw-r--r--   0        0        0      539 2023-06-20 07:52:04.243517 nutils-7.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     9669 2023-06-20 07:52:04.243517 nutils-7.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0       65 2023-06-20 07:52:04.243517 nutils-7.3/.gitignore
+-rw-r--r--   0        0        0    39725 2023-06-20 07:52:04.243517 nutils-7.3/CHANGELOG.rst
+-rw-r--r--   0        0        0     1062 2023-06-20 07:52:04.243517 nutils-7.3/LICENSE
+-rw-r--r--   0        0        0     5629 2023-06-20 07:52:04.243517 nutils-7.3/README.md
+-rw-r--r--   0        0        0     1437 2023-06-20 07:52:04.243517 nutils-7.3/devtools/__init__.py
+-rw-r--r--   0        0        0     1303 2023-06-20 07:52:04.243517 nutils-7.3/devtools/_git.py
+-rw-r--r--   0        0        0      732 2023-06-20 07:52:04.243517 nutils-7.3/devtools/_log_default.py
+-rw-r--r--   0        0        0      649 2023-06-20 07:52:04.243517 nutils-7.3/devtools/_log_gha.py
+-rw-r--r--   0        0        0     3985 2023-06-20 07:52:04.243517 nutils-7.3/devtools/container/__init__.py
+-rw-r--r--   0        0        0     6103 2023-06-20 07:52:04.243517 nutils-7.3/devtools/container/build.py
+-rw-r--r--   0        0        0     1698 2023-06-20 07:52:04.243517 nutils-7.3/devtools/container/build_base.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:52:04.243517 nutils-7.3/devtools/gha/__init__.py
+-rw-r--r--   0        0        0     1242 2023-06-20 07:52:04.243517 nutils-7.3/devtools/gha/configure_mkl.py
+-rw-r--r--   0        0        0     1697 2023-06-20 07:52:04.243517 nutils-7.3/devtools/gha/coverage_report_xml.py
+-rw-r--r--   0        0        0      776 2023-06-20 07:52:04.243517 nutils-7.3/devtools/gha/get_base_and_image_tags.py
+-rw-r--r--   0        0        0      105 2023-06-20 07:52:04.243517 nutils-7.3/docs/_static/mods.css
+-rw-r--r--   0        0        0      585 2023-06-20 07:52:04.243517 nutils-7.3/docs/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0    11343 2023-06-20 07:52:04.243517 nutils-7.3/docs/conf.py
+-rw-r--r--   0        0        0   360414 2023-06-20 07:52:04.247517 nutils-7.3/docs/favicon.ico
+-rw-r--r--   0        0        0      510 2023-06-20 07:52:04.247517 nutils-7.3/docs/index.rst
+-rw-r--r--   0        0        0     5591 2023-06-20 07:52:04.247517 nutils-7.3/docs/sphinx_mods.py
+-rw-r--r--   0        0        0      456 2023-06-20 07:52:04.247517 nutils-7.3/examples/__init__.py
+-rw-r--r--   0        0        0     6802 2023-06-20 07:52:04.247517 nutils-7.3/examples/adaptivity.py
+-rw-r--r--   0        0        0     4408 2023-06-20 07:52:04.247517 nutils-7.3/examples/burgers.py
+-rw-r--r--   0        0        0    12895 2023-06-20 07:52:04.247517 nutils-7.3/examples/cahnhilliard.py
+-rw-r--r--   0        0        0    10903 2023-06-20 07:52:04.247517 nutils-7.3/examples/coil.py
+-rw-r--r--   0        0        0    12856 2023-06-20 07:52:04.247517 nutils-7.3/examples/cylinderflow.py
+-rw-r--r--   0        0        0    15064 2023-06-20 07:52:04.247517 nutils-7.3/examples/drivencavity.py
+-rw-r--r--   0        0        0     7185 2023-06-20 07:52:04.247517 nutils-7.3/examples/elasticity.py
+-rw-r--r--   0        0        0     5882 2023-06-20 07:52:04.247517 nutils-7.3/examples/finitestrain.py
+-rw-r--r--   0        0        0     7492 2023-06-20 07:52:04.247517 nutils-7.3/examples/laplace.py
+-rw-r--r--   0        0        0     9758 2023-06-20 07:52:04.247517 nutils-7.3/examples/platewithhole.py
+-rw-r--r--   0        0        0     2088 2023-06-20 07:52:04.247517 nutils-7.3/examples/poisson.py
+-rw-r--r--   0        0        0      871 2023-06-20 07:52:04.247517 nutils-7.3/nutils/__init__.py
+-rw-r--r--   0        0        0    11164 2023-06-20 07:52:04.247517 nutils-7.3/nutils/_graph.py
+-rw-r--r--   0        0        0    15035 2023-06-20 07:52:04.247517 nutils-7.3/nutils/cache.py
+-rw-r--r--   0        0        0    15210 2023-06-20 07:52:04.247517 nutils-7.3/nutils/cli.py
+-rw-r--r--   0        0        0      468 2023-06-20 07:52:04.247517 nutils-7.3/nutils/debug_flags.py
+-rw-r--r--   0        0        0    46150 2023-06-20 07:52:04.247517 nutils-7.3/nutils/element.py
+-rw-r--r--   0        0        0    20862 2023-06-20 07:52:04.247517 nutils-7.3/nutils/elementseq.py
+-rw-r--r--   0        0        0   174749 2023-06-20 07:52:04.251517 nutils-7.3/nutils/evaluable.py
+-rw-r--r--   0        0        0     6946 2023-06-20 07:52:04.251517 nutils-7.3/nutils/export.py
+-rw-r--r--   0        0        0    84274 2023-06-20 07:52:04.251517 nutils-7.3/nutils/expression_v1.py
+-rw-r--r--   0        0        0    40199 2023-06-20 07:52:04.251517 nutils-7.3/nutils/expression_v2.py
+-rw-r--r--   0        0        0   139029 2023-06-20 07:52:04.251517 nutils-7.3/nutils/function.py
+-rw-r--r--   0        0        0     2475 2023-06-20 07:52:04.251517 nutils-7.3/nutils/matrix/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-20 07:52:04.251517 nutils-7.3/nutils/matrix/_auto.py
+-rw-r--r--   0        0        0    13356 2023-06-20 07:52:04.251517 nutils-7.3/nutils/matrix/_base.py
+-rw-r--r--   0        0        0    14021 2023-06-20 07:52:04.251517 nutils-7.3/nutils/matrix/_mkl.py
+-rw-r--r--   0        0        0     2292 2023-06-20 07:52:04.251517 nutils-7.3/nutils/matrix/_numpy.py
+-rw-r--r--   0        0        0     4267 2023-06-20 07:52:04.251517 nutils-7.3/nutils/matrix/_scipy.py
+-rw-r--r--   0        0        0    31749 2023-06-20 07:52:04.251517 nutils-7.3/nutils/mesh.py
+-rw-r--r--   0        0        0    23027 2023-06-20 07:52:04.251517 nutils-7.3/nutils/numeric.py
+-rw-r--r--   0        0        0     5767 2023-06-20 07:52:04.251517 nutils-7.3/nutils/parallel.py
+-rw-r--r--   0        0        0    19627 2023-06-20 07:52:04.251517 nutils-7.3/nutils/points.py
+-rw-r--r--   0        0        0    22402 2023-06-20 07:52:04.251517 nutils-7.3/nutils/pointsseq.py
+-rw-r--r--   0        0        0    47965 2023-06-20 07:52:04.251517 nutils-7.3/nutils/sample.py
+-rw-r--r--   0        0        0    44018 2023-06-20 07:52:04.251517 nutils-7.3/nutils/solver.py
+-rw-r--r--   0        0        0    13225 2023-06-20 07:52:04.251517 nutils-7.3/nutils/sparse.py
+-rw-r--r--   0        0        0    11497 2023-06-20 07:52:04.251517 nutils-7.3/nutils/testing.py
+-rw-r--r--   0        0        0   148854 2023-06-20 07:52:04.255518 nutils-7.3/nutils/topology.py
+-rw-r--r--   0        0        0    24673 2023-06-20 07:52:04.255518 nutils-7.3/nutils/transform.py
+-rw-r--r--   0        0        0    38427 2023-06-20 07:52:04.255518 nutils-7.3/nutils/transformseq.py
+-rw-r--r--   0        0        0    49559 2023-06-20 07:52:04.255518 nutils-7.3/nutils/types.py
+-rw-r--r--   0        0        0     6934 2023-06-20 07:52:04.255518 nutils-7.3/nutils/unit.py
+-rw-r--r--   0        0        0    18250 2023-06-20 07:52:04.255518 nutils-7.3/nutils/util.py
+-rw-r--r--   0        0        0     1020 2023-06-20 07:52:04.255518 nutils-7.3/nutils/warnings.py
+-rw-r--r--   0        0        0      720 2023-06-20 07:52:04.255518 nutils-7.3/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-06-20 07:52:04.255518 nutils-7.3/readthedocs.yml
+-rw-r--r--   0        0        0        0 2023-06-20 07:52:04.255518 nutils-7.3/tests/__init__.py
+-rw-r--r--   0        0        0    16414 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_basis.py
+-rw-r--r--   0        0        0    14034 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_cache.py
+-rw-r--r--   0        0        0     5572 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_cli.py
+-rw-r--r--   0        0        0     2977 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_docs.py
+-rw-r--r--   0        0        0     4916 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_element.py
+-rw-r--r--   0        0        0     9541 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_elementseq.py
+-rw-r--r--   0        0        0    65386 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_evaluable.py
+-rw-r--r--   0        0        0     9353 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_export.py
+-rw-r--r--   0        0        0    52174 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_expression_v1.py
+-rw-r--r--   0        0        0    24532 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_expression_v2.py
+-rw-r--r--   0        0        0    18454 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_finitecell.py
+-rw-r--r--   0        0        0    67732 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_function.py
+-rw-r--r--   0        0        0    13425 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_graph.py
+-rw-r--r--   0        0        0     3214 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_ischeme.py
+-rw-r--r--   0        0        0    11189 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_matrix.py
+-rw-r--r--   0        0        0     7242 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_mesh.py
+-rw-r--r--   0        0        0     1388 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_mesh/mesh2d.geo
+-rw-r--r--   0        0        0     6702 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_mesh/mesh2d_p1_v2.msh
+-rw-r--r--   0        0        0     5618 2023-06-20 07:52:04.255518 nutils-7.3/tests/test_mesh/mesh2d_p1_v4.msh
+-rw-r--r--   0        0        0    17648 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh2d_p2_v2.msh
+-rw-r--r--   0        0        0    16228 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh2d_p2_v4.msh
+-rw-r--r--   0        0        0    35340 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh2d_p3_v2.msh
+-rw-r--r--   0        0        0    33181 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh2d_p3_v4.msh
+-rw-r--r--   0        0        0    59708 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh2d_p4_v2.msh
+-rw-r--r--   0        0        0    56807 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh2d_p4_v4.msh
+-rw-r--r--   0        0        0     3221 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh3d.geo
+-rw-r--r--   0        0        0    78920 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh3d_p1_v2.msh
+-rw-r--r--   0        0        0    59146 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh3d_p1_v4.msh
+-rw-r--r--   0        0        0   254705 2023-06-20 07:52:04.259518 nutils-7.3/tests/test_mesh/mesh3d_p2_v2.msh
+-rw-r--r--   0        0        0   225898 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_mesh/mesh3d_p2_v4.msh
+-rw-r--r--   0        0        0      742 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_mesh/mesh3dmani.geo
+-rw-r--r--   0        0        0     5893 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_mesh/mesh3dmani_p1_v2.msh
+-rw-r--r--   0        0        0     5587 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_mesh/mesh3dmani_p1_v4.msh
+-rw-r--r--   0        0        0    17016 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_mesh/mesh3dmani_p2_v2.msh
+-rw-r--r--   0        0        0    16281 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_mesh/mesh3dmani_p2_v4.msh
+-rw-r--r--   0        0        0     2665 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_normals.py
+-rw-r--r--   0        0        0    11273 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_numeric.py
+-rw-r--r--   0        0        0     2204 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_parallel.py
+-rw-r--r--   0        0        0     7066 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_points.py
+-rw-r--r--   0        0        0    11292 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_pointsseq.py
+-rw-r--r--   0        0        0     2268 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_quadrature.py
+-rw-r--r--   0        0        0    25943 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_sample.py
+-rw-r--r--   0        0        0    13474 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_solver.py
+-rw-r--r--   0        0        0    13697 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_sparse.py
+-rw-r--r--   0        0        0     1705 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_testing.py
+-rw-r--r--   0        0        0    61518 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_topology.py
+-rw-r--r--   0        0        0     6397 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_transform.py
+-rw-r--r--   0        0        0    21581 2023-06-20 07:52:04.263518 nutils-7.3/tests/test_transformseq.py
+-rw-r--r--   0        0        0    38683 2023-06-20 07:52:04.267518 nutils-7.3/tests/test_types.py
+-rw-r--r--   0        0        0     2317 2023-06-20 07:52:04.267518 nutils-7.3/tests/test_unit.py
+-rw-r--r--   0        0        0     8101 2023-06-20 07:52:04.267518 nutils-7.3/tests/test_util.py
+-rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 nutils-7.3/PKG-INFO
```

### Comparing `nutils-7.2/README.md` & `nutils-7.3/README.md`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/__init__.py` & `nutils-7.3/nutils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+'Numerical Utilities for Finite Element Analysis'
+
 import sys
 import numpy
 from distutils.version import LooseVersion
 
 assert sys.version_info >= (3, 5)
 assert LooseVersion(numpy.version.version) >= LooseVersion('1.16'), 'nutils requires numpy 1.16 or higher, got {}'.format(numpy.version.version)
 
-version = '7.2'
+__version__ = version = '7.3'
 version_name = 'hiyamugi'
 long_version = ('{} "{}"' if version_name else '{}').format(version, version_name)
 
 __all__ = [
     'cache',
     'cli',
     'element',
```

### Comparing `nutils-7.2/nutils/_graph.py` & `nutils-7.3/nutils/_graph.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/cache.py` & `nutils-7.3/nutils/cache.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/cli.py` & `nutils-7.3/nutils/cli.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/element.py` & `nutils-7.3/nutils/element.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/elementseq.py` & `nutils-7.3/nutils/elementseq.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/evaluable.py` & `nutils-7.3/nutils/evaluable.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/export.py` & `nutils-7.3/nutils/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,18 +153,22 @@
     t_cells[:, 1:] = cells
 
     name_vtk = name + '.vtk'
     with log.userfile(name_vtk, 'wb') as vtk:
         vtk.write(b'# vtk DataFile Version 3.0\nvtk output\nBINARY\nDATASET UNSTRUCTURED_GRID\n')
         vtk.write('POINTS {} {}\n'.format(npoints, vtkdtype[points.dtype]).encode('ascii'))
         points.tofile(vtk)
+        vtk.write(b"\n")
         vtk.write('CELLS {} {}\n'.format(ncells, t_cells.size).encode('ascii'))
         t_cells.tofile(vtk)
+        vtk.write(b"\n")
         vtk.write('CELL_TYPES {}\n'.format(ncells).encode('ascii'))
         vtkcelltype[nverts].repeat(ncells).tofile(vtk)
+        vtk.write(b"\n")
         for n, items in gathered:
             vtk.write('{}_DATA {}\n'.format('POINT' if n == npoints else 'CELL', n).encode('ascii'))
             for dname, array in items:
                 vtk.write(vtkndim[array.ndim].format(dname, vtkdtype[array.dtype]).encode('ascii'))
                 array.tofile(vtk)
+                vtk.write(b"\n")
 
 # vim:sw=2:sts=2:et
```

### Comparing `nutils-7.2/nutils/expression_v1.py` & `nutils-7.3/nutils/expression_v1.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/expression_v2.py` & `nutils-7.3/nutils/expression_v2.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/function.py` & `nutils-7.3/nutils/function.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/matrix/__init__.py` & `nutils-7.3/nutils/matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/matrix/_base.py` & `nutils-7.3/nutils/matrix/_base.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/matrix/_mkl.py` & `nutils-7.3/nutils/matrix/_mkl.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/matrix/_numpy.py` & `nutils-7.3/nutils/matrix/_numpy.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/matrix/_scipy.py` & `nutils-7.3/nutils/matrix/_scipy.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/mesh.py` & `nutils-7.3/nutils/mesh.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/numeric.py` & `nutils-7.3/nutils/numeric.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
             except numpy.linalg.LinAlgError:
                 Ainv[index] = numpy.nan
     return Ainv
 
 
 isarray = lambda a: isinstance(a, numpy.ndarray)
 isboolarray = lambda a: isarray(a) and a.dtype == bool
-isbool = lambda a: isboolarray(a) and a.ndim == 0 or type(a) == bool
+isbool = lambda a: isboolarray(a) and a.ndim == 0 or isinstance(a, (bool, numpy.bool_))
 isint = lambda a: isinstance(a, numbers.Integral)
 isnumber = lambda a: isinstance(a, numbers.Number)
 isintarray = lambda a: isarray(a) and numpy.issubdtype(a.dtype, numpy.integer)
 asobjvector = lambda v: numpy.array((None,)+tuple(v), dtype=object)[1:]  # 'None' prevents interpretation of objects as axes
 
 
 def blockdiag(args):
```

### Comparing `nutils-7.2/nutils/parallel.py` & `nutils-7.3/nutils/parallel.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/points.py` & `nutils-7.3/nutils/points.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     def hull(self):
         '''Triangulation of the exterior hull.
 
         A two-dimensional integer array with ``ndims`` columns, of which every row
         defines a simplex by mapping vertices into the list of points.
         '''
 
+        assert self.ndims > 0, 'hull is not defined for a zero-dimensional point set'
         edge_vertices = numpy.arange(self.ndims+1).repeat(self.ndims).reshape(self.ndims, self.ndims+1).T  # ndims+1 x ndims
         edge_simplices = numpy.sort(self.tri, axis=1)[:, edge_vertices]  # nelems x ndims+1 x ndims
         elems, edges = divmod(numpy.lexsort(edge_simplices.reshape(-1, self.ndims).T), self.ndims+1)
         sorted_edge_simplices = edge_simplices[elems, edges]  # (nelems x ndims+1) x ndims; matching edges are now adjacent
         notequal = numpy.not_equal(sorted_edge_simplices[1:], sorted_edge_simplices[:-1]).any(axis=1)
         return types.frozenarray(sorted_edge_simplices[numpy.hstack([True, notequal]) & numpy.hstack([notequal, True])], copy=False)
```

### Comparing `nutils-7.2/nutils/pointsseq.py` & `nutils-7.3/nutils/pointsseq.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/sample.py` & `nutils-7.3/nutils/sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 connectivity through its :attr:`Sample.tri` and :attr:`Sample.hull`
 properties, representing a (n-dimensional) triangulation of the interior and
 boundary, respectively. Availability of these properties depends on the
 selected sample points, and is typically used in combination with the "bezier"
 set.
 '''
 
-from . import types, points, util, function, evaluable, parallel, numeric, matrix, sparse, warnings
+from . import types, points, util, function, evaluable, parallel, matrix, sparse, warnings
 from .pointsseq import PointsSequence
 from .transformseq import Transforms
 from .transform import EvaluableTransformChain
 from typing import Iterable, Mapping, Optional, Sequence, Tuple, Union
 import numpy
 import numbers
 import collections.abc
@@ -602,14 +602,98 @@
     def integral(self, func: function.IntoArray) -> function.Array:
         return self._sample1.integral(func) + self._sample2.integral(func)
 
     def __call__(self, func: function.IntoArray) -> function.Array:
         return function.concatenate([self._sample1(func), self._sample2(func)])
 
 
+def _simplex_strip(strip):
+    # Helper function that creates simplices for an extruded simplex, with
+    # vertices arranged in a [2,n] shape (prepended with an arbitrary number of
+    # axes). The Strategy is to create the first simplex from the first vertex
+    # in layer 1 and all vertices from layer 2, the second from all but the
+    # first of layer 2 and the first two of layer 1, and so on until the last
+    # simplex consists of all vertices of layer 1 and the last of layer 2.
+
+    assert strip.dtype == int
+    *shape, m, n = strip.shape
+    assert m == 2
+    flat = strip.reshape((*shape, 2*n)) # ravel last two axes, reallocates if necessary
+    flat = numpy.ascontiguousarray(flat) # required for use as buffer
+    *strides, s = flat.strides
+    return numpy.ndarray(buffer=flat, dtype=int, shape=(*shape, n, n+1), strides=(*strides, s, s))
+
+
+def _mul_tri(tri1, tri2):
+    # Helper function that computes the tri1 x tri2 product. The indices should
+    # be pre-multiplied with the appropriate strides.
+
+    if tri2 is None: # multiplication with 'empty' right hand side
+        return tri1
+
+    if tri1.shape[1] > tri2.shape[1]: # swap to reduce cases below
+        tri1, tri2 = tri2, tri1
+
+    ndims1 = tri1.shape[1] - 1
+    ndims2 = tri2.shape[1] - 1
+
+    tri_outer = tri1[:,None,:,None] + tri2[None,:,None,:]
+
+    if ndims1 == 0: # Left multiplication by a 0D sample
+        # Multiply the left 0D tri by the right tri and maintain the latter's
+        # triangulation.
+        tri = tri_outer.reshape(-1, ndims2+1)
+    elif ndims1 == 1: # Left multiplication by a 1D sample
+        # Multiply the left 1D tri by the right tri and triangulate using a
+        # simplex strip.
+        tri = _simplex_strip(tri_outer).reshape(-1, ndims2+2)
+    else:
+        raise NotImplementedError(f'tri not supported for {ndims1}D x {ndims2}D multiplication')
+
+    assert tri.shape[1] == ndims1 + ndims2 + 1
+    return tri
+
+
+def _mul_hull(tri1, tri2, hull1, hull2):
+    # Helper function that computes the hull1 x hull2 product. The indices
+    # should be pre-multiplied with the appropriate strides. If either tri1 or
+    # tri2 represents a 0D triangulation (i.e. a point) then the corresponding
+    # hull value will be ignored.
+
+    if tri2 is None: # multiplication with 'empty' right hand side
+        return hull1
+
+    if tri1.shape[1] > tri2.shape[1]: # swap to reduce cases below
+        tri1, tri2 = tri2, tri1
+        hull1, hull2 = hull2, hull1
+
+    ndims1 = tri1.shape[1] - 1
+    ndims2 = tri2.shape[1] - 1
+
+    if ndims1 == 0: # Left multiplication by a 0D sample
+        # Multiply the left 0D tri by the right hull and maintain the latter's
+        # triangulation.
+        hull_outer = tri1[:,None,:,None] + hull2[None,:,None,:] # ...,1,ndims2
+        hull = hull_outer.reshape(-1, ndims2)
+    elif ndims1 == 1: # Left multiplication by a 1D sample
+        # 1. Multiply the left 1D tri by the right hull and triangulate using a
+        # simplex strip.
+        hull_outer = tri1[:,None,:,None] + hull2[None,:,None,:] # ...,2,ndims2
+        hull = _simplex_strip(hull_outer).reshape(-1, ndims2+1)
+        # 2. Multiply the left 0D hull by the right tri and maintain the
+        # latter's triangulation.
+        hull_outer = hull1[:,None,:,None] + tri2[None,:,None,:] # ...,1,ndims2+1
+        hull = numpy.concatenate([hull_outer.reshape(-1, ndims2+1), hull])
+    else:
+        raise NotImplementedError(f'hull not supported for {ndims1}D x {ndims2}D multiplication')
+
+    assert hull.shape[1] == ndims1 + ndims2
+    return hull
+
+
 class _Mul(_TensorialSample):
 
     def __init__(self, sample1: Sample, sample2: Sample) -> None:
         assert set(sample1.spaces).isdisjoint(set(sample2.spaces))
         self._sample1 = sample1
         self._sample2 = sample2
         super().__init__(sample1.spaces + sample2.spaces, sample1.ndims + sample2.ndims, sample1.nelems * sample2.nelems, sample1.npoints * sample2.npoints)
@@ -633,57 +717,92 @@
         return evaluable.einsum('A,B->AB', weights1, weights2)
 
     def update_lower_args(self, __ielem: evaluable.Array, points_shape: _PointsShape, transform_chains: _TransformChainsMap, coordinates: _CoordinatesMap) -> Tuple[_PointsShape, _TransformChainsMap, _CoordinatesMap]:
         ielem1, ielem2 = evaluable.divmod(__ielem, self._sample2.nelems)
         points_shape, transform_chains, coordinates = self._sample1.update_lower_args(ielem1, points_shape, transform_chains, coordinates)
         return self._sample2.update_lower_args(ielem2, points_shape, transform_chains, coordinates)
 
+    @property
+    def _reversed_factors(self):
+        # Helper method that generates the factors of arbitrarily nested
+        # multiplications in reverse order.
+
+        for s in self._sample2, self._sample1:
+            if isinstance(s, _Mul):
+                yield from s._reversed_factors
+            else:
+                yield s
+
+    def _get_element_tri_hull(self, ielem: int, with_hull: bool) -> numpy.ndarray:
+        # Helper method that returns the element_tri and element_hull for a
+        # given element index, used by get_element_tri and get_element_hull.
+        #
+        # To save work in case only the element_tri is required, a None value
+        # is returned for the latter if the with_hull flag is set to False. The
+        # converse (returning only the hull) is not possible as construction of
+        # the hull implies construction of the tri.
+
+        if not 0 <= ielem < self.nelems:
+            raise IndexError('element number is out of bounds')
+
+        # We loop from the final factor back to the first because of the order
+        # in which both the element index and the element vertices are raveled.
+
+        tri = hull = None
+        stride = 1
+        for sample in self._reversed_factors:
+            ielem, i = divmod(ielem, sample.nelems) # i is the unraveled element index in sample
+            nverts = len(sample.getindex(i))
+            sample_tri = sample.get_element_tri(i) * stride
+            if with_hull:
+                sample_hull = sample.ndims and sample.get_element_hull(i) * stride
+                hull = _mul_hull(sample_tri, tri, sample_hull, hull)
+            tri = _mul_tri(sample_tri, tri)
+            stride *= nverts # update stride to include the element's vertex count
+        assert ielem == 0
+        return tri, hull
+
     def get_element_tri(self, ielem: int) -> numpy.ndarray:
-        if self._sample1.ndims == 1:
-            ielem1, ielem2 = divmod(ielem, self._sample2.nelems)
-            npoints2 = len(self._sample2.getindex(ielem2))
-            tri12 = self._sample1.get_element_tri(ielem1)[:, None, :, None] * npoints2 + self._sample2.get_element_tri(ielem2)[None, :, None, :]  # ntri1 x ntri2 x 2 x ndims
-            return numeric.overlapping(tri12.reshape(-1, 2*self.ndims), n=self.ndims+1).reshape(-1, self.ndims+1)
-        elif self._sample1.npoints == 1:
-            return self._sample2.get_element_tri(ielem)
-        elif self._sample2.npoints == 1:
-            return self._sample1.get_element_tri(ielem)
-        else:
-            return super().get_element_tri(ielem)
+        return self._get_element_tri_hull(ielem, with_hull=False)[0]
 
     def get_element_hull(self, ielem: int) -> numpy.ndarray:
-        if self._sample1.ndims == 1:
-            ielem1, ielem2 = divmod(ielem, self._sample2.nelems)
-            npoints2 = len(self._sample2.getindex(ielem2))
-            hull1 = self._sample1.get_element_hull(ielem1)[:, None, :, None] * npoints2 + self._sample2.get_element_tri(ielem2)[None, :, None, :]  # 2 x ntri2 x 1 x ndims
-            hull2 = self._sample1.get_element_tri(ielem1)[:, None, :, None] * npoints2 + self._sample2.get_element_hull(ielem2)[None, :, None, :]  # ntri1 x nhull2 x 2 x ndims-1
-            return numpy.concatenate([hull1.reshape(-1, self.ndims), numeric.overlapping(hull2.reshape(-1, 2*(self.ndims-1)), n=self.ndims).reshape(-1, self.ndims)])
-        elif self._sample1.npoints == 1:
-            return self._sample2.get_element_hull(ielem)
-        elif self._sample2.npoints == 1:
-            return self._sample1.get_element_hull(ielem)
-        else:
-            return super().get_element_hull(ielem)
+        return self._get_element_tri_hull(ielem, with_hull=True)[1]
+
+    def _tri_hull(self, with_hull) -> numpy.ndarray:
+        # Helper method that returns the tri and hull of the sample, used by
+        # the tri and hull. These properties replace the default implementation
+        # via get_element_tri and get_element_hull by a faster algorithm that
+        # applies the product structure directly on the level of the sample.
+        #
+        # To save work in case only tri is required, a None value is returned
+        # for hull if the with_hull flag is set to False. The converse
+        # (returning only hull) is not possible as construction of hull implies
+        # construction of tri.
+        #
+        # We loop from the final factor back to the first because of the order
+        # in which the sample points are raveled.
+
+        tri = hull = None
+        stride = 1
+        for sample in self._reversed_factors:
+            sample_tri = sample.tri * stride
+            if with_hull:
+                sample_hull = sample.ndims and sample.hull * stride
+                hull = _mul_hull(sample_tri, tri, sample_hull, hull)
+            tri = _mul_tri(sample_tri, tri)
+            stride *= sample.npoints # update stride to include the sample's point count
+        return tri, hull
 
     @property
     def tri(self) -> numpy.ndarray:
-        if self._sample1.ndims == 1:
-            tri12 = self._sample1.tri[:, None, :, None] * self._sample2.npoints + self._sample2.tri[None, :, None, :]  # ntri1 x ntri2 x 2 x ndims
-            return numeric.overlapping(tri12.reshape(-1, 2*self.ndims), n=self.ndims+1).reshape(-1, self.ndims+1)
-        else:
-            return super().tri
+        return self._tri_hull(with_hull=False)[0]
 
     @property
     def hull(self) -> numpy.ndarray:
-        if self._sample1.ndims == 1:
-            hull1 = self._sample1.hull[:, None, :, None] * self._sample2.npoints + self._sample2.tri[None, :, None, :]  # 2 x ntri2 x 1 x ndims
-            hull2 = self._sample1.tri[:, None, :, None] * self._sample2.npoints + self._sample2.hull[None, :, None, :]  # ntri1 x nhull2 x 2 x ndims-1
-            return numpy.concatenate([hull1.reshape(-1, self.ndims), numeric.overlapping(hull2.reshape(-1, 2*(self.ndims-1)), n=self.ndims).reshape(-1, self.ndims)])
-        else:
-            return super().hull
+        return self._tri_hull(with_hull=True)[1]
 
     def integral(self, func: function.IntoArray) -> function.Array:
         return self._sample1.integral(self._sample2.integral(func))
 
     def __call__(self, func: function.IntoArray) -> function.Array:
         return function.ravel(self._sample1(self._sample2(func)), axis=0)
 
@@ -742,16 +861,18 @@
                 coordinates[space] = evaluable.prependaxes(evaluable._take(coords, self._getslice(ilocalsi, ielem), axis=0), points_shape)
         return (*points_shape, size), transform_chains, coordinates
 
     def get_evaluable_indices(self, ielem):
         return self._getslice(self._indices, ielem)
 
     def get_evaluable_weights(self, ielem):
-        weights = self._samples[0].get_evaluable_weights(evaluable.Take(self._ielems[0], ielem))
-        return self._getslice(weights, ielem)
+        ielem0 = evaluable.Take(self._ielems[0], ielem)
+        slice0 = self._getslice(self._ilocals[0], ielem)
+        weights = self._samples[0].get_evaluable_weights(ielem0)
+        return evaluable._take(weights, slice0, axis=0)
 
 
 class _TakeElements(_TensorialSample):
 
     __cache__ = '_offsets'
 
     def __init__(self, parent: Sample, indices: types.arraydata) -> None:
```

### Comparing `nutils-7.2/nutils/solver.py` & `nutils-7.3/nutils/solver.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/sparse.py` & `nutils-7.3/nutils/sparse.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/testing.py` & `nutils-7.3/nutils/testing.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/topology.py` & `nutils-7.3/nutils/topology.py`

 * *Files 0% similar despite different names*

```diff
@@ -1487,27 +1487,25 @@
             raise ValueError('locate requires either tol or eps to be strictly positive')
         coords = numpy.asarray(coords, dtype=float)
         if geom.ndim == 0:
             geom = geom[_]
             coords = coords[..., _]
         if not geom.shape == coords.shape[1:] == (self.ndims,):
             raise ValueError('invalid geometry or point shape for {}D topology'.format(self.ndims))
+        if skip_missing and weights is not None:
+            raise ValueError('weights and skip_missing are mutually exclusive')
         centroids = self.sample('_centroid', None).eval(geom)
         assert len(centroids) == len(self)
         ielems = parallel.shempty(len(coords), dtype=int)
         points = parallel.shempty((len(coords), len(geom)), dtype=float)
         _ielem = evaluable.Argument('_locate_ielem', shape=(), dtype=int)
         _point = evaluable.Argument('_locate_point', shape=(self.ndims,))
         egeom = geom.lower((), {self.space: (self.transforms.get_evaluable(_ielem), self.opposites.get_evaluable(_ielem))}, {self.space: _point})
         xJ = evaluable.Tuple((egeom, evaluable.derivative(egeom, _point))).simplified
         arguments = dict(arguments or ())
-        if skip_missing:
-            if weights is not None:
-                raise ValueError('weights and skip_missing are mutually exclusive')
-            missing = parallel.shzeros(len(coords), dtype=bool)
         with parallel.ctxrange('locating', len(coords)) as ipoints:
             for ipoint in ipoints:
                 xt = coords[ipoint]  # target
                 dist = numpy.linalg.norm(centroids - xt, axis=1)
                 for ielem in numpy.argsort(dist) if maxdist is None \
                         else sorted((dist < maxdist).nonzero()[0], key=dist.__getitem__):
                     ref = self.references[ielem]
@@ -1533,22 +1531,29 @@
                         p += dp  # NOTE: modifies arguments['_locate_point'] in place
                     else:
                         if ref.inside(p, max(eps, ep)):
                             ielems[ipoint] = ielem
                             points[ipoint] = p
                             break
                 else:
-                    if skip_missing:
-                        missing[ipoint] = True
-                    else:
-                        raise LocateError('failed to locate point: {}'.format(xt))
-        if skip_missing:
-            ielems = ielems[~missing]
-            points = points[~missing]
-        return self._sample(ielems, points, weights)
+                    ielems[ipoint] = -1 # mark point as missing
+                    if not skip_missing:
+                        # rather than raising LocateError here, which
+                        # parallel.fork will reraise as a general Exception if
+                        # ipoint was assigned to a child process, we fast
+                        # forward through the remaining points to abandon the
+                        # loop and subsequently raise from the main process.
+                        for ipoint in ipoints:
+                            pass
+        if -1 not in ielems: # all points are found
+            return self._sample(ielems, points, weights)
+        elif skip_missing: # not all points are found and that's ok, we just leave those out
+            return self._sample(ielems[ielems != -1], points[ielems != -1])
+        else: # not all points are found and that's an error
+            raise LocateError(f'failed to locate point: {coords[ielems==-1][0]}')
 
     def _sample(self, ielems, coords, weights=None):
         index = numpy.argsort(ielems, kind='stable')
         sorted_ielems = ielems[index]
         offsets = [0, *(sorted_ielems[:-1] != sorted_ielems[1:]).nonzero()[0]+1, len(index)]
 
         unique_ielems = sorted_ielems[offsets[:-1]]
@@ -1640,37 +1645,24 @@
         assert numeric.isint(degree) and degree >= 0
 
         if degree == 0:
             raise ValueError('Cannot build a C^0-continuous basis of degree 0.  Use basis \'discont\' instead.')
 
         coeffs = [ref.get_poly_coeffs(name, degree=degree) for ref in self.references]
         offsets = numpy.cumsum([0] + [len(c) for c in coeffs])
-        dofmap = numpy.repeat(-1, offsets[-1])
-        for ielem, ioppelems in enumerate(self.connectivity):
-            for iedge, jelem in enumerate(ioppelems):  # loop over element neighbors and merge dofs
-                if jelem < ielem:
-                    continue  # either there is no neighbor along iedge or situation will be inspected from the other side
-                jedge = util.index(self.connectivity[jelem], ielem)
-                idofs = offsets[ielem] + self.references[ielem].get_edge_dofs(degree, iedge)
-                jdofs = offsets[jelem] + self.references[jelem].get_edge_dofs(degree, jedge)
-                for idof, jdof in zip(idofs, jdofs):
-                    while dofmap[idof] != -1:
-                        idof = dofmap[idof]
-                    while dofmap[jdof] != -1:
-                        jdof = dofmap[jdof]
-                    if idof != jdof:
-                        dofmap[max(idof, jdof)] = min(idof, jdof)  # create left-looking pointer
-        # assign dof numbers left-to-right
-        ndofs = 0
-        for i, n in enumerate(dofmap):
-            if n == -1:
-                dofmap[i] = ndofs
-                ndofs += 1
-            else:
-                dofmap[i] = dofmap[n]
+        # To merge matching dofs we loop over the connectivity table to find
+        # neighbouring elements (limited to jelem > ielem to consider every
+        # neighbour pair exactly once as well as ignore exterior boundaries)
+        # and mark the degrees of freedom on both sides to be equal.
+        dofmap, ndofs = util.merge_index_map(offsets[-1], (merge_set
+            for ielem, ioppelems in enumerate(self.connectivity)
+                for iedge, jelem in enumerate(ioppelems) if jelem >= ielem
+                    for merge_set in zip(
+                        offsets[ielem] + self.references[ielem].get_edge_dofs(degree, iedge),
+                        offsets[jelem] + self.references[jelem].get_edge_dofs(degree, util.index(self.connectivity[jelem], ielem)))))
 
         elem_slices = map(slice, offsets[:-1], offsets[1:])
         dofs = tuple(types.frozenarray(dofmap[s]) for s in elem_slices)
         return function.PlainBasis(coeffs, dofs, ndofs, self.f_index, self.f_coords)
 
     def basis_lagrange(self, degree):
         'lagrange shape functions'
@@ -2573,24 +2565,45 @@
     @log.withcontext
     def basis(self, name, *args, **kwargs):
         if isinstance(self.basetopo, HierarchicalTopology):
             warnings.warn('basis may be linearly dependent; a linearly indepent basis is obtained by trimming first, then creating hierarchical refinements')
         basis = self.basetopo.basis(name, *args, **kwargs)
         return function.PrunedBasis(basis, self._indices, self.f_index, self.f_coords)
 
-    def locate(self, geom, coords, *, eps=0, **kwargs):
-        sample = self.basetopo.locate(geom, coords, eps=eps, **kwargs)
-        for isampleelem, (transforms, points) in enumerate(zip(sample.transforms[0], sample.points)):
+    def locate(self, geom, coords, *, eps=0, skip_missing=False, **kwargs):
+        sample = self.basetopo.locate(geom, coords, eps=eps, skip_missing=skip_missing, **kwargs)
+        missing = []
+        for isampleelem, (transforms, points_) in enumerate(zip(sample.transforms[0], sample.points)):
             ielem = self.basetopo.transforms.index(transforms)
             ref = self.refs[ielem]
             if ref != self.basetopo.references[ielem]:
-                for i, coord in enumerate(points.coords):
+                for i, coord in enumerate(points_.coords):
                     if not ref.inside(coord, eps):
-                        raise LocateError('failed to locate point: {}'.format(coords[sample.getindex(isampleelem)[i]]))
-        return sample
+                        if not skip_missing:
+                            raise LocateError('failed to locate point: {}'.format(coords[sample.getindex(isampleelem)[i]]))
+                        missing.append((isampleelem, i))
+        if not missing:
+            return sample
+        selection = numpy.ones(len(sample.points), dtype=bool)
+        newpoints = []
+        for isampleelem, points_ in enumerate(sample.points):
+            mymissing = [] # collect missing points for current element
+            for isampleelem_, i in missing[:points_.npoints]:
+                if isampleelem_ != isampleelem:
+                    break
+                mymissing.append(i)
+            if not mymissing: # no points are missing -> keep existing points object
+                newpoints.append(points_)
+            elif len(mymissing) < points_.npoints: # some points are missing -> create new CoordsPoints object
+                newpoints.append(points.CoordsPoints(points_.coords[~numeric.asboolean(mymissing, points_.npoints)]))
+            else: # all points are missing -> remove element from return sample
+                selection[isampleelem] = False
+            del missing[:len(mymissing)]
+        assert not missing
+        return Sample.new(sample.space, [trans[selection] for trans in sample.transforms], PointsSequence.from_iter(newpoints, sample.ndims))
 
 
 class RefinedTopology(TransformChainsTopology):
     'refinement'
 
     __slots__ = 'basetopo',
     __cache__ = 'boundary', 'connectivity'
@@ -2691,15 +2704,18 @@
     def slice_unchecked(self, __s: slice, __idim: int) -> 'HierarchicalTopology':
         return self._rebase(self.basetopo.slice_unchecked(__s, __idim))
 
     def get_groups(self, *groups: str) -> 'HierarchicalTopology':
         return self._rebase(self.basetopo.get_groups(*groups))
 
     def refined_by(self, refine):
-        refine = tuple(refine)
+        if isinstance(refine, Topology):
+            refine = refine.transforms
+        else:
+            refine = tuple(refine)
         if not all(map(numeric.isint, refine)):
             refine = tuple(self.transforms.index_with_tail(item)[0] for item in refine)
         refine = numpy.unique(numpy.array(refine, dtype=int))
         splits = numpy.searchsorted(refine, self._offsets, side='left')
         indices_per_level = list(map(list, self._indices_per_level))+[[]]
         fine = self.basetopo
         for ilevel, (start, stop) in enumerate(zip(splits[:-1], splits[1:])):
@@ -3130,23 +3146,17 @@
                     # append boundary dofs to list (in increasing order, automatic by outer loop and dof increment)
                     commonboundarydofs.setdefault(boundary.id, []).append(boundarydofs)
             dofcount += numpy.prod(patchdofcount)
 
         if patchcontinuous:
             # build merge mapping: merge common boundary dofs (from low to high)
             pairs = itertools.chain(*(zip(*dofs) for dofs in commonboundarydofs.values() if len(dofs) > 1))
-            merge = numpy.arange(dofcount)
-            for dofs in sorted(pairs):
-                merge[list(dofs)] = merge[list(dofs)].min()
-            assert all(numpy.all(merge[a] == merge[b]) for a, *B in commonboundarydofs.values() for b in B), 'something went wrong is merging interface dofs; this should not have happened'
-            # build renumber mapping: renumber remaining dofs consecutively, starting at 0
-            remainder, renumber = numpy.unique(merge, return_inverse=True)
+            renumber, dofcount = util.merge_index_map(dofcount, pairs)
             # apply mappings
             dofmap = tuple(types.frozenarray(renumber[v], copy=False) for v in dofmap)
-            dofcount = len(remainder)
 
         return function.PlainBasis(coeffs, dofmap, dofcount, self.f_index, self.f_coords)
 
     def basis_patch(self):
         'degree zero patchwise discontinuous basis'
 
         transforms = transformseq.PlainTransforms(tuple((patch.topo.root,) for patch in self.patches), self.ndims, self.ndims)
```

### Comparing `nutils-7.2/nutils/transform.py` & `nutils-7.3/nutils/transform.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/transformseq.py` & `nutils-7.3/nutils/transformseq.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/types.py` & `nutils-7.3/nutils/types.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/unit.py` & `nutils-7.3/nutils/unit.py`

 * *Files identical despite different names*

### Comparing `nutils-7.2/nutils/util.py` & `nutils-7.3/nutils/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 from . import numeric
 import sys
 import os
 import numpy
 import collections.abc
 import inspect
+import itertools
 import functools
 import operator
 import numbers
 import pathlib
 import ctypes
 import io
 import contextlib
+from typing import Iterable, Sequence, Tuple
 
 supports_outdirfd = os.open in os.supports_dir_fd and os.listdir in os.supports_fd
 
 sum = functools.partial(functools.reduce, operator.add)
 product = functools.partial(functools.reduce, operator.mul)
 
 
@@ -520,8 +522,57 @@
             try:
                 val = self.__dict__[func.__name__]
             except KeyError:
                 self.__dict__[func.__name__] = val = func(self)
             return val
         return property(wrapped)
 
+
+def merge_index_map(nin: int, merge_sets: Iterable[Sequence[int]]) -> Tuple[numpy.ndarray, int]:
+    '''Returns an index map relating ``nin`` unmerged elements to ``nout`` merged elements.
+
+    The index map, an array of length ``nin``, satisfies the following conditions:
+
+    *   For every merge set in ``merge_sets``: for every pair of indices ``i``
+        and ``j`` in a merge set, ``index_map[i] == index_map[j]`` is true.
+
+        In code, the following is true::
+
+            all(index_map[i] == index_map[j] for i, *js in merge_sets for j in js)
+
+    *   Selecting the first occurences of indices in ``index_map`` gives the
+        sequence ``range(nout)``.
+
+    Args
+    ----
+    nin : :class:`int`
+        The number of elements before merging.
+    merge_sets : iterable of sequences of at least one :class:`int`
+        An iterable of merge sets, where each merge set lists the indices of
+        input elements that should be merged. Every merge set should have at
+        least one index.
+
+    Returns
+    -------
+    index_map : :class:`numpy.ndarray`
+        Index map with satisfying the above conditions.
+    nout : :class:`int`
+        The number of output indices.
+    '''
+
+    index_map = numpy.arange(nin)
+    def resolve(index):
+        parent = index_map[index]
+        while index != parent:
+            index = parent
+            parent = index_map[index]
+        return index
+    for merge_set in merge_sets:
+        resolved = list(map(resolve, merge_set))
+        index_map[resolved] = min(resolved)
+    new_indices = itertools.count()
+    for iin, ptr in enumerate(index_map):
+        index_map[iin] = next(new_indices) if iin == ptr else index_map[ptr]
+    return index_map, next(new_indices)
+
+
 # vim:sw=2:sts=2:et
```

### Comparing `nutils-7.2/nutils/warnings.py` & `nutils-7.3/nutils/warnings.py`

 * *Files identical despite different names*

