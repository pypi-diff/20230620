# Comparing `tmp/pyslim-1.0.2.tar.gz` & `tmp/pyslim-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslim-1.0.2.tar", last modified: Tue Jun 20 21:03:18 2023, max compression
+gzip compressed data, was "pyslim-1.0b1.tar", last modified: Sat Jun  4 04:59:28 2022, max compression
```

## Comparing `pyslim-1.0.2.tar` & `pyslim-1.0b1.tar`

### file list

```diff
@@ -1,209 +1,192 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.213519 pyslim-1.0.2/
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2020-10-22 02:53:30.000000 pyslim-1.0.2/.codecov.yml
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.105516 pyslim-1.0.2/.github/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.113516 pyslim-1.0.2/.github/workflows/
--rw-r--r--   0 peter     (1000) peter     (1000)     3352 2023-06-20 19:36:32.000000 pyslim-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0 peter     (1000) peter     (1000)     3498 2023-06-20 19:36:32.000000 pyslim-1.0.2/.github/workflows/tests.yml
--rw-r--r--   0 peter     (1000) peter     (1000)      104 2023-06-14 21:14:29.000000 pyslim-1.0.2/.gitignore
--rw-r--r--   0 peter     (1000) peter     (1000)     9692 2023-06-20 21:02:02.000000 pyslim-1.0.2/CHANGELOG.rst
--rw-r--r--   0 peter     (1000) peter     (1000)     1078 2020-08-27 16:00:40.000000 pyslim-1.0.2/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)     1242 2023-06-20 21:03:18.213519 pyslim-1.0.2/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)    11288 2019-04-25 04:01:10.000000 pyslim-1.0.2/README.html
--rw-r--r--   0 peter     (1000) peter     (1000)      783 2023-06-14 21:14:29.000000 pyslim-1.0.2/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.121516 pyslim-1.0.2/docs/
--rw-r--r--   0 peter     (1000) peter     (1000)      104 2023-06-20 21:00:33.000000 pyslim-1.0.2/docs/.gitignore
--rw-r--r--   0 peter     (1000) peter     (1000)      732 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     1398 2023-06-20 19:36:32.000000 pyslim-1.0.2/docs/_config.yml
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.125517 pyslim-1.0.2/docs/_static/
--rw-r--r--   0 peter     (1000) peter     (1000)     2162 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_static/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)   127863 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/_static/annotate_genome.png
--rw-r--r--   0 peter     (1000) peter     (1000)   187800 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/_static/annotated_p_vs_s.png
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1047 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_static/export-layers-svg.sh
--rw-r--r--   0 peter     (1000) peter     (1000)   169670 2022-08-11 19:54:04.000000 pyslim-1.0.2/docs/_static/pedigree0.png
--rw-r--r--   0 peter     (1000) peter     (1000)    55231 2022-08-11 19:46:11.000000 pyslim-1.0.2/docs/_static/pedigree0.svg
--rw-r--r--   0 peter     (1000) peter     (1000)   285215 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_static/pedigree01.png
--rw-r--r--   0 peter     (1000) peter     (1000)   111698 2022-08-11 19:54:04.000000 pyslim-1.0.2/docs/_static/pedigree1.png
--rw-r--r--   0 peter     (1000) peter     (1000)    41364 2022-08-11 19:46:11.000000 pyslim-1.0.2/docs/_static/pedigree1.svg
--rw-r--r--   0 peter     (1000) peter     (1000)   199641 2022-08-11 19:54:05.000000 pyslim-1.0.2/docs/_static/pedigree2.png
--rw-r--r--   0 peter     (1000) peter     (1000)    56799 2022-08-11 19:46:11.000000 pyslim-1.0.2/docs/_static/pedigree2.svg
--rw-r--r--   0 peter     (1000) peter     (1000)   134067 2022-08-11 19:54:06.000000 pyslim-1.0.2/docs/_static/pedigree_mutate.png
--rw-r--r--   0 peter     (1000) peter     (1000)    50171 2022-08-11 19:46:11.000000 pyslim-1.0.2/docs/_static/pedigree_mutate.svg
--rw-r--r--   0 peter     (1000) peter     (1000)   143371 2022-08-11 19:54:05.000000 pyslim-1.0.2/docs/_static/pedigree_recapitate.png
--rw-r--r--   0 peter     (1000) peter     (1000)    50004 2022-08-11 19:46:11.000000 pyslim-1.0.2/docs/_static/pedigree_recapitate.svg
--rw-r--r--   0 peter     (1000) peter     (1000)   181909 2021-02-20 21:37:04.000000 pyslim-1.0.2/docs/_static/pedigree_remember.png
--rw-r--r--   0 peter     (1000) peter     (1000)   120875 2022-08-11 19:54:06.000000 pyslim-1.0.2/docs/_static/pedigree_simplify.png
--rw-r--r--   0 peter     (1000) peter     (1000)    41603 2022-08-11 19:46:11.000000 pyslim-1.0.2/docs/_static/pedigree_simplify.svg
--rw-r--r--   0 peter     (1000) peter     (1000)   107060 2022-08-11 19:46:11.000000 pyslim-1.0.2/docs/_static/pedigrees.ink.svg
--rw-r--r--   0 peter     (1000) peter     (1000)       52 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_static/pedigrees.ink.svg.md5
--rw-r--r--   0 peter     (1000) peter     (1000)     1643 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_static/phylo.pdf
--rw-r--r--   0 peter     (1000) peter     (1000)    46500 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_static/phylo.png
--rw-r--r--   0 peter     (1000) peter     (1000)       93 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_static/phylo.tsv
--rw-r--r--   0 peter     (1000) peter     (1000)       78 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/_static/recomb_rates.tsv
--rw-r--r--   0 peter     (1000) peter     (1000)      476 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/_toc.yml
--rw-r--r--   0 peter     (1000) peter     (1000)    14315 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/annotate_genome.pdf
--rw-r--r--   0 peter     (1000) peter     (1000)   136457 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/annotated_p_vs_s.pdf
--rwxr-xr-x   0 peter     (1000) peter     (1000)      536 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/build.sh
--rw-r--r--   0 peter     (1000) peter     (1000)     6001 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/conf.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1834 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/development.md
--rw-r--r--   0 peter     (1000) peter     (1000)      626 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/example_sim.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      956 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/generation_time.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1137 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/installation.md
--rw-r--r--   0 peter     (1000) peter     (1000)     5904 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/introduction.md
--rw-r--r--   0 peter     (1000) peter     (1000)     7907 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/metadata.md
--rw-r--r--   0 peter     (1000) peter     (1000)      952 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/migrants.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      861 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/neutral_restart.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1313 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/phylo_bgs.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     9947 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/previous_versions.md
--rw-r--r--   0 peter     (1000) peter     (1000)     2837 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/python_api.md
--rw-r--r--   0 peter     (1000) peter     (1000)      347 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/rapid_adaptation.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      696 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/reload_annotated.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      453 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/selection.slim
--rw-r--r--   0 peter     (1000) peter     (1000)    27478 2023-06-20 19:36:32.000000 pyslim-1.0.2/docs/time_units.md
--rw-r--r--   0 peter     (1000) peter     (1000)    47491 2023-06-20 21:00:33.000000 pyslim-1.0.2/docs/tutorial.md
--rw-r--r--   0 peter     (1000) peter     (1000)     1189 2021-12-09 00:53:14.000000 pyslim-1.0.2/docs/util.py
--rw-r--r--   0 peter     (1000) peter     (1000)    21698 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/vignette_coalescent_diversity.md
--rw-r--r--   0 peter     (1000) peter     (1000)     8725 2023-06-20 13:56:37.000000 pyslim-1.0.2/docs/vignette_continuing.md
--rw-r--r--   0 peter     (1000) peter     (1000)    12757 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/vignette_parallel_phylo.md
--rw-r--r--   0 peter     (1000) peter     (1000)    16658 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/vignette_space.md
--rw-r--r--   0 peter     (1000) peter     (1000)     1803 2023-06-14 21:14:29.000000 pyslim-1.0.2/docs/vignette_space.slim
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.129516 pyslim-1.0.2/pyslim/
--rw-r--r--   0 peter     (1000) peter     (1000)      369 2023-06-14 21:14:29.000000 pyslim-1.0.2/pyslim/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      158 2023-06-20 21:01:35.000000 pyslim-1.0.2/pyslim/_version.py
--rw-r--r--   0 peter     (1000) peter     (1000)    37238 2023-06-20 03:33:36.000000 pyslim-1.0.2/pyslim/methods.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2321 2023-06-14 21:14:29.000000 pyslim-1.0.2/pyslim/provenance.py
--rw-r--r--   0 peter     (1000) peter     (1000)    42038 2023-06-14 21:14:29.000000 pyslim-1.0.2/pyslim/slim_metadata.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4347 2023-06-14 21:14:29.000000 pyslim-1.0.2/pyslim/slim_tree_sequence.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7500 2023-06-14 21:14:29.000000 pyslim-1.0.2/pyslim/spatial.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1273 2023-06-14 21:14:29.000000 pyslim-1.0.2/pyslim/util.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.129516 pyslim-1.0.2/pyslim.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1242 2023-06-20 21:03:18.000000 pyslim-1.0.2/pyslim.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     7785 2023-06-20 21:03:18.000000 pyslim-1.0.2/pyslim.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-06-20 21:03:18.000000 pyslim-1.0.2/pyslim.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2018-06-27 17:05:45.000000 pyslim-1.0.2/pyslim.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)       34 2023-06-20 21:03:18.000000 pyslim-1.0.2/pyslim.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        7 2023-06-20 21:03:18.000000 pyslim-1.0.2/pyslim.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.129516 pyslim-1.0.2/requirements/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.129516 pyslim-1.0.2/requirements/CI-conda/
--rw-r--r--   0 peter     (1000) peter     (1000)      267 2023-06-14 21:14:29.000000 pyslim-1.0.2/requirements/CI-conda/ci-environment.yml
--rw-r--r--   0 peter     (1000) peter     (1000)       29 2023-06-14 21:14:29.000000 pyslim-1.0.2/requirements/CI-conda/requirements.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.129516 pyslim-1.0.2/requirements/CI-docs/
--rw-r--r--   0 peter     (1000) peter     (1000)      193 2023-06-20 19:36:32.000000 pyslim-1.0.2/requirements/CI-docs/requirements.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.129516 pyslim-1.0.2/requirements/CI-pip/
--rw-r--r--   0 peter     (1000) peter     (1000)       81 2023-06-20 19:36:32.000000 pyslim-1.0.2/requirements/CI-pip/requirements.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       42 2023-06-14 21:14:29.000000 pyslim-1.0.2/requirements/conda-minimal.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-06-20 21:03:18.213519 pyslim-1.0.2/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)     1302 2023-06-14 21:14:29.000000 pyslim-1.0.2/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.137517 pyslim-1.0.2/tests/
--rw-r--r--   0 peter     (1000) peter     (1000)      741 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)     8906 2023-06-19 22:27:16.000000 pyslim-1.0.2/tests/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.141517 pyslim-1.0.2/tests/benchmark/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1324 2020-10-30 17:45:26.000000 pyslim-1.0.2/tests/benchmark/annotation.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1299 2020-10-30 17:45:26.000000 pyslim-1.0.2/tests/benchmark/metadata.sh
--rw-r--r--   0 peter     (1000) peter     (1000)      577 2020-10-22 02:53:30.000000 pyslim-1.0.2/tests/benchmark/metadata.slim
--rw-r--r--   0 peter     (1000) peter     (1000)    12360 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/conftest.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.161517 pyslim-1.0.2/tests/extra_recipes/
--rw-r--r--   0 peter     (1000) peter     (1000)       12 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/extra_recipes/.gitignore
--rw-r--r--   0 peter     (1000) peter     (1000)     4017 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)      602 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.1 - A minimal tree-seq model.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      845 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation I.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1265 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation II.py
--rw-r--r--   0 peter     (1000) peter     (1000)      573 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.2 - Overlaying neutral mutations.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1019 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.3 - Simulation conditional upon fixation of a sweep, preserving ancestry I.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1043 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.3 - Simulation conditional upon fixation of a sweep, preserving ancestry II.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      859 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) I.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1533 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) II.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1133 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) I.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1062 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) II.py
--rw-r--r--   0 peter     (1000) peter     (1000)      612 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit I.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      564 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit II.py
--rw-r--r--   0 peter     (1000) peter     (1000)      295 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history I.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1005 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history II.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      219 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history III.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1577 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history I.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1072 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history II.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      541 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models I.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      974 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models II.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1265 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models III.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)      268 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/extra_recipes/check_trees.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5416 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/recipe_specs.py
--rw-r--r--   0 peter     (1000) peter     (1000)    42649 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_annotation.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9166 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_metadata.py
--rw-r--r--   0 peter     (1000) peter     (1000)    17761 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_provenance.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 21:03:18.213519 pyslim-1.0.2/tests/test_recipes/
--rw-r--r--   0 peter     (1000) peter     (1000)      913 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/make_v3_test_additions.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2387 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/make_v3_tests.sh
--rw-r--r--   0 peter     (1000) peter     (1000)     1886 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)    16348 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.0.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    20204 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.2.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    20276 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.3.1.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    22236 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.4.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    33116 2021-02-22 14:50:45.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.5.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    33604 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.5_and_v3.6.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    33388 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.6.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    33796 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.7.trees
--rw-r--r--   0 peter     (1000) peter     (1000)     1887 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_early_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1887 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_early_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1886 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_early_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1887 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_first_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1887 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_first_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1886 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_first_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1886 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_late_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1886 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_late_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1885 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_late_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1985 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_WF_migration.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      612 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_init_mutated_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      826 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_init_mutated_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      490 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_long_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      702 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_long_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      667 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_long_nucleotides.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1699 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_mutation_spectrum.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2097 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)    10972 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.0.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    14620 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.2.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    14588 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.3.1.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    13212 2021-02-20 21:37:04.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.4.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    21252 2021-02-22 14:50:45.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.5.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    21516 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.6.trees
--rw-r--r--   0 peter     (1000) peter     (1000)    21740 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.7.trees
--rw-r--r--   0 peter     (1000) peter     (1000)     2098 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_early_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2098 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_early_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2097 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_early_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2098 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_first_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2098 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_first_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2097 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_first_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2100 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_late_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2100 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_late_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2099 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_late_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      778 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_nonstacked.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2236 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nonWF_selfing.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1984 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nucleotides_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2170 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nucleotides_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2165 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_nucleotides_plus_others.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2084 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_WF_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2087 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_WF_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2134 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_WF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2267 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_nonWF_early.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2270 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_nonWF_first.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2265 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_nonWF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2340 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_remember_and_retain.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2234 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_retain_everyone_WF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2278 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_retain_everyone_nonWF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2445 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_retain_sometimes_WF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2489 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_retain_sometimes_nonWF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2467 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_retain_unary_WF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     2511 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_retain_unary_nonWF_late.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1948 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_roots.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      814 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/recipe_with_metadata.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      960 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1349 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_and_remove_subpop_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      961 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_and_run_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      948 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_and_run_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1340 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_msprime.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1719 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_multispecies_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     1722 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_multispecies_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      999 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      951 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_nucleotides_WF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)      933 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_recipes/restart_nucleotides_nonWF.slim
--rw-r--r--   0 peter     (1000) peter     (1000)     7682 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_spatial.py
--rw-r--r--   0 peter     (1000) peter     (1000)    43483 2023-06-20 03:33:36.000000 pyslim-1.0.2/tests/test_tree_sequence.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2942 2023-06-14 21:14:29.000000 pyslim-1.0.2/tests/test_util.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.563259 pyslim-1.0b1/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.519258 pyslim-1.0b1/.circleci/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2127 2022-06-03 16:21:38.000000 pyslim-1.0b1/.circleci/config.yml
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2020-10-22 02:53:30.000000 pyslim-1.0b1/.codecov.yml
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.511258 pyslim-1.0b1/.github/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.519258 pyslim-1.0b1/.github/workflows/
+-rw-r--r--   0 peter     (1000) peter     (1000)     3950 2022-06-03 16:21:38.000000 pyslim-1.0b1/.github/workflows/tests.yml
+-rw-r--r--   0 peter     (1000) peter     (1000)       91 2021-12-17 15:19:12.000000 pyslim-1.0b1/.gitignore
+-rw-r--r--   0 peter     (1000) peter     (1000)     8083 2022-06-03 21:00:34.000000 pyslim-1.0b1/CHANGELOG.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     1078 2020-08-27 16:00:40.000000 pyslim-1.0b1/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)     1262 2022-06-04 04:59:28.559259 pyslim-1.0b1/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)    11288 2019-04-25 04:01:10.000000 pyslim-1.0b1/README.html
+-rw-r--r--   0 peter     (1000) peter     (1000)      783 2022-06-03 16:21:38.000000 pyslim-1.0b1/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.527258 pyslim-1.0b1/docs/
+-rw-r--r--   0 peter     (1000) peter     (1000)       88 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/.gitignore
+-rw-r--r--   0 peter     (1000) peter     (1000)      579 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1328 2021-12-20 23:43:11.000000 pyslim-1.0b1/docs/_config.yml
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.543259 pyslim-1.0b1/docs/_static/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2162 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)   127863 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/annotate_genome.png
+-rw-r--r--   0 peter     (1000) peter     (1000)   187800 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/annotated_p_vs_s.png
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1047 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/export-layers-svg.sh
+-rw-r--r--   0 peter     (1000) peter     (1000)   169670 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree0.png
+-rw-r--r--   0 peter     (1000) peter     (1000)    55231 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree0.svg
+-rw-r--r--   0 peter     (1000) peter     (1000)   285215 2021-12-16 05:56:16.000000 pyslim-1.0b1/docs/_static/pedigree01.png
+-rw-r--r--   0 peter     (1000) peter     (1000)   111698 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree1.png
+-rw-r--r--   0 peter     (1000) peter     (1000)    41364 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree1.svg
+-rw-r--r--   0 peter     (1000) peter     (1000)   199641 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree2.png
+-rw-r--r--   0 peter     (1000) peter     (1000)    56799 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree2.svg
+-rw-r--r--   0 peter     (1000) peter     (1000)   134067 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree_mutate.png
+-rw-r--r--   0 peter     (1000) peter     (1000)    50171 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree_mutate.svg
+-rw-r--r--   0 peter     (1000) peter     (1000)   143371 2021-12-15 09:42:17.000000 pyslim-1.0b1/docs/_static/pedigree_recapitate.png
+-rw-r--r--   0 peter     (1000) peter     (1000)    50004 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree_recapitate.svg
+-rw-r--r--   0 peter     (1000) peter     (1000)   181909 2021-02-20 21:37:04.000000 pyslim-1.0b1/docs/_static/pedigree_remember.png
+-rw-r--r--   0 peter     (1000) peter     (1000)   120875 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/pedigree_simplify.png
+-rw-r--r--   0 peter     (1000) peter     (1000)    41603 2021-07-16 17:16:26.000000 pyslim-1.0b1/docs/_static/pedigree_simplify.svg
+-rw-r--r--   0 peter     (1000) peter     (1000)   107060 2021-07-16 17:15:57.000000 pyslim-1.0b1/docs/_static/pedigrees.ink.svg
+-rw-r--r--   0 peter     (1000) peter     (1000)     1643 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/phylo.pdf
+-rw-r--r--   0 peter     (1000) peter     (1000)    46500 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/phylo.png
+-rw-r--r--   0 peter     (1000) peter     (1000)       93 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/phylo.tsv
+-rw-r--r--   0 peter     (1000) peter     (1000)       78 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/_static/recomb_rates.tsv
+-rw-r--r--   0 peter     (1000) peter     (1000)      455 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/_toc.yml
+-rw-r--r--   0 peter     (1000) peter     (1000)    14315 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/annotate_genome.pdf
+-rw-r--r--   0 peter     (1000) peter     (1000)   136457 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/annotated_p_vs_s.pdf
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      536 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/build.sh
+-rw-r--r--   0 peter     (1000) peter     (1000)     6001 2021-12-21 17:07:26.000000 pyslim-1.0b1/docs/conf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1834 2021-12-21 17:07:26.000000 pyslim-1.0b1/docs/development.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      626 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/example_sim.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      925 2021-12-21 17:07:26.000000 pyslim-1.0b1/docs/installation.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     5938 2021-12-21 17:07:26.000000 pyslim-1.0b1/docs/introduction.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    20046 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/metadata.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      952 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/migrants.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      861 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/neutral_restart.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1313 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/phylo_bgs.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     7361 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/previous_versions.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     3047 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/python_api.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      347 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/rapid_adaptation.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      696 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/reload_annotated.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      453 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/selection.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)    45515 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/tutorial.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     1189 2021-12-09 00:53:14.000000 pyslim-1.0b1/docs/util.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    21775 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/vignette_coalescent_diversity.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     8664 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/vignette_continuing.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    12757 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/vignette_parallel_phylo.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/vignette_space.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     1803 2022-06-03 16:21:38.000000 pyslim-1.0b1/docs/vignette_space.slim
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.547259 pyslim-1.0b1/pyslim/
+-rw-r--r--   0 peter     (1000) peter     (1000)      369 2021-12-09 00:53:14.000000 pyslim-1.0b1/pyslim/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      158 2022-06-03 21:00:34.000000 pyslim-1.0b1/pyslim/_version.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    34544 2022-06-03 16:21:38.000000 pyslim-1.0b1/pyslim/methods.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2321 2022-06-03 16:21:38.000000 pyslim-1.0b1/pyslim/provenance.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    41300 2022-06-03 16:21:38.000000 pyslim-1.0b1/pyslim/slim_metadata.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4114 2022-06-03 16:21:38.000000 pyslim-1.0b1/pyslim/slim_tree_sequence.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7448 2022-06-03 16:21:38.000000 pyslim-1.0b1/pyslim/spatial.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      997 2022-06-03 16:21:38.000000 pyslim-1.0b1/pyslim/util.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.547259 pyslim-1.0b1/pyslim.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1262 2022-06-04 04:59:28.000000 pyslim-1.0b1/pyslim.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     6973 2022-06-04 04:59:28.000000 pyslim-1.0b1/pyslim.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2022-06-04 04:59:28.000000 pyslim-1.0b1/pyslim.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2018-06-27 17:05:45.000000 pyslim-1.0b1/pyslim.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)       42 2022-06-04 04:59:28.000000 pyslim-1.0b1/pyslim.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        7 2022-06-04 04:59:28.000000 pyslim-1.0b1/pyslim.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.547259 pyslim-1.0b1/requirements/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.547259 pyslim-1.0b1/requirements/CI-conda/
+-rw-r--r--   0 peter     (1000) peter     (1000)       29 2022-06-03 16:21:38.000000 pyslim-1.0b1/requirements/CI-conda/requirements.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.547259 pyslim-1.0b1/requirements/CI-docs/
+-rw-r--r--   0 peter     (1000) peter     (1000)      191 2022-06-03 16:21:38.000000 pyslim-1.0b1/requirements/CI-docs/requirements.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.547259 pyslim-1.0b1/requirements/CI-pip/
+-rw-r--r--   0 peter     (1000) peter     (1000)       82 2022-06-03 16:21:38.000000 pyslim-1.0b1/requirements/CI-pip/requirements.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       42 2021-12-16 21:16:07.000000 pyslim-1.0b1/requirements/conda-minimal.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2022-06-04 04:59:28.563259 pyslim-1.0b1/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)     1322 2022-06-03 05:04:47.000000 pyslim-1.0b1/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.547259 pyslim-1.0b1/tests/
+-rw-r--r--   0 peter     (1000) peter     (1000)      741 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     8932 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.551259 pyslim-1.0b1/tests/benchmark/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1324 2020-10-30 17:45:26.000000 pyslim-1.0b1/tests/benchmark/annotation.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1299 2020-10-30 17:45:26.000000 pyslim-1.0b1/tests/benchmark/metadata.sh
+-rw-r--r--   0 peter     (1000) peter     (1000)      577 2020-10-22 02:53:30.000000 pyslim-1.0b1/tests/benchmark/metadata.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     8965 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/conftest.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.555259 pyslim-1.0b1/tests/extra_recipes/
+-rw-r--r--   0 peter     (1000) peter     (1000)       12 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/extra_recipes/.gitignore
+-rw-r--r--   0 peter     (1000) peter     (1000)     3635 2021-12-20 23:43:11.000000 pyslim-1.0b1/tests/extra_recipes/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)      602 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.1 - A minimal tree-seq model.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      845 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation I.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1267 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation II.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      573 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.2 - Overlaying neutral mutations.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1019 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.3 - Simulation conditional upon fixation of a sweep, preserving ancestry I.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1043 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.3 - Simulation conditional upon fixation of a sweep, preserving ancestry II.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      859 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) I.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1533 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) II.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1133 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) I.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1062 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) II.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      612 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit I.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      564 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit II.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      295 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history I.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1005 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history II.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      219 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history III.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1577 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history I.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1072 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history II.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      541 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models I.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      974 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models II.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1265 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models III.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      268 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/extra_recipes/check_trees.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5892 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/recipe_specs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    33622 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_annotation.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9166 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_metadata.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17761 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_provenance.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-06-04 04:59:28.559259 pyslim-1.0b1/tests/test_recipes/
+-rw-r--r--   0 peter     (1000) peter     (1000)      913 2022-05-14 06:40:19.000000 pyslim-1.0b1/tests/test_recipes/make_v3_test_additions.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2387 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/make_v3_tests.sh
+-rw-r--r--   0 peter     (1000) peter     (1000)     1492 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)    16348 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.0.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    20204 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.2.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    20276 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.3.1.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    22236 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.4.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    33116 2021-02-22 14:50:45.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.5.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    33604 2022-05-14 06:40:19.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.5_and_v3.6.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    33388 2021-12-15 05:24:35.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.6.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    33796 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.7.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)     1493 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF_early_early.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1491 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF_early_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1492 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF_late_early.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1490 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF_late_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1591 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_WF_migration.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      612 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_init_mutated_WF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      826 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_init_mutated_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      490 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_long_WF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      702 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_long_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      667 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_long_nucleotides.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1699 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_mutation_spectrum.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1703 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)    10972 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.0.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    14620 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.2.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    14588 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.3.1.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    13212 2021-02-20 21:37:04.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.4.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    21252 2021-02-22 14:50:45.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.5.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    21516 2021-12-15 05:24:35.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.6.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)    21740 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.7.trees
+-rw-r--r--   0 peter     (1000) peter     (1000)     1704 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF_early_early.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1703 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF_early_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1706 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF_late_early.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1705 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF_late_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      860 2021-12-09 00:53:14.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF_nonstacked.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1842 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nonWF_selfing.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1590 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nucleotides_WF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1777 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nucleotides_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1771 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_nucleotides_plus_others.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1690 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_WF_early.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1814 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_WF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1873 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_nonWF_early.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1871 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_nonWF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1946 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_remember_and_retain.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1840 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_retain_everyone_WF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1884 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_retain_everyone_nonWF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     2051 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_retain_sometimes_WF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     2095 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_retain_sometimes_nonWF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     2073 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_retain_unary_WF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     2117 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_retain_unary_nonWF_late.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1554 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/recipe_roots.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      814 2021-12-16 05:56:16.000000 pyslim-1.0b1/tests/test_recipes/recipe_with_metadata.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      960 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_WF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1349 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_and_remove_subpop_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      961 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_and_run_WF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      948 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_and_run_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     1340 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_msprime.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      999 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      894 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_nucleotides_WF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)      933 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_recipes/restart_nucleotides_nonWF.slim
+-rw-r--r--   0 peter     (1000) peter     (1000)     7699 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_spatial.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    39533 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_tree_sequence.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2637 2022-06-03 16:21:38.000000 pyslim-1.0b1/tests/test_util.py
```

### Comparing `pyslim-1.0.2/.github/workflows/docs.yml` & `pyslim-1.0b1/.github/workflows/tests.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-name: Docs
+name: Tests
 
 on:
   pull_request:
   push:
     branches: [main]
 
 jobs:
 
   test:
     name: Python
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python: [ 3.9 ]
+        python: [ 3.8, 3.9 ]
         os:  [ macos-latest, ubuntu-latest ]
     defaults:
       run:
         shell: bash
     steps:
       - name: Cancel Previous Runs
         uses: styfle/cancel-workflow-action@0.6.0
@@ -29,15 +29,15 @@
           submodules: true
 
       - name: Cache conda and dependancies
         id: cache
         uses: actions/cache@v2
         env:
           # Increase this to reset the cache if the key hasn't changed.
-          CACHE_NUM: 5
+          CACHE_NUM: 3
         with:
           path: |
             c:\Miniconda\envs\anaconda-client-env
             /usr/share/miniconda/envs/anaconda-client-env
             ~/osx-conda
             ~/.profile
           key: ${{ runner.os }}-${{ matrix.python}}-conda-v${{ env.CACHE_NUM }}-${{ hashFiles('requirements/CI-pip/requirements.txt') }}-${{ hashFiles('requirements/CI-conda/requirements.txt') }}-${{ hashFiles('requirements/CI-docs/requirements.txt') }}
@@ -58,17 +58,18 @@
         run: |
           cp ~/.bash_profile ~/.profile
 
       - name: Install conda deps
         if: steps.cache.outputs.cache-hit != 'true'
         shell: bash -l {0} #We need a login shell to get conda
         run: |
-          if [ "$RUNNER_OS" != "Windows" ]; then
-            conda install --yes slim
-          fi
+          # TODO: uncomment when SLiM v4 is released
+          # if [ "$RUNNER_OS" != "Windows" ]; then
+          #   conda install --yes slim
+          # fi
           conda install --yes --file=requirements/CI-conda/requirements.txt
 
       - name: Install pip deps
         if: steps.cache.outputs.cache-hit != 'true'
         shell: bash -l {0}
         run: |
           pip install -r requirements/CI-pip/requirements.txt
@@ -81,28 +82,36 @@
 
       - name: Fix OSX Cache Restore
         if: steps.cache.outputs.cache-hit == 'true' && matrix.os == 'macos-latest'
         run: |
           mkdir -p /usr/local/miniconda/envs
           sudo cp -r ~/osx-conda /usr/local/miniconda/envs/anaconda-client-env
 
-      # # Retaining commented block for next devel cycle
-      # - name: Build SLiM
-      #   run: |
-      #     git clone https://github.com/messerlab/SLiM.git
-      #     cd SLiM
-      #     mkdir -p Release
-      #     cd Release
-      #     cmake -D CMAKE_BUILD_TYPE=Release ..
-      #     make -j 2
+      # Installing SLiM from conda now.
+      # TODO: comment this out again when SLiM v4 is released
+      - name: Build SLiM
+        run: |
+          git clone https://github.com/messerlab/SLiM.git
+          cd SLiM
+          git checkout -b multispecies origin/multispecies
+          mkdir -p Release
+          cd Release
+          cmake -D CMAKE_BUILD_TYPE=Release ..
+          make -j 2
 
-      - name: Build docs
+      - name: Run tests
         run: |
           source ~/.profile
           conda activate anaconda-client-env
           export PATH=$PWD/SLiM/Release:$PATH
-          slim -v
-          pip list
-          cd docs && make
+          pytest -xv -n2 tests
 
+      - name: Build docs
+        run: |
+          source ~/.profile
+          conda activate anaconda-client-env
+          export PATH=$PATH:$PWD/SLiM/Release
+          touch docs/_static/{pedigree0.svg,pedigree1.svg,pedigree2.svg,pedigree_recapitate.svg,pedigree_simplify.svg,pedigree_mutate.svg}
+          touch docs/_static/{pedigree01.png,pedigree0.png,pedigree1.png,pedigree2.png,pedigree_recapitate.png,pedigree_simplify.png,pedigree_mutate.png}
+          cd docs && make
```

### Comparing `pyslim-1.0.2/CHANGELOG.rst` & `pyslim-1.0b1/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,65 @@
 ***************************
-[1.0.2] - 2023-06-20
+[UPCOMING.X.X] - XXXX-XX-XX
 ***************************
 
-**Bugfixes**:
-
-- From 1.0.1 back to 0.700, there was a bug in `recapitate` when using the
-    `ancestral_Ne` parameter that introduced a bottleneck to diploid size Ne=1
-    for each SLiM subpopulation for 1 or 2 generations *unless* either (a) it
-    was a WF simulation, with calls to addSubPop() in first() or early() and
-    treeSeqOutput() in late(), or (b) it was a nonWF simulation, with calls to
-    addSubPop() in first() and treeSeqOutput() in early() or late(). The fix
-    correctly starts the msprime population with effective size `ancestral_Ne`
-    at the time of the roots, which might be at the value of
-    `ts.metadata['SLiM']['tick']`, this value minus 1, or this value minus 2.
-    Furthermore, `recapitate` now throws an error if any roots of any trees
-    are not at the same time as the others. (:user:`petrelharp`, :pr:`308`)
-
-
-
-***************************
-[1.0.1] - 2022-09-23
-***************************
-
-- Documentation of how to empirically measure generation time
-    and check that it is correct
-    (:user:`silastittes`, :user:`petrelharp`, :pr:`301`, :pr:`293`).
-
-- Minor modifications to `convert_alleles` and `generate_nucleotides`
-    so that they run in a reasonable amount of time
-    (:user:`petrelharp`, :pr:`299`).
-
-- Addition of method to find the next SLiM mutation ID,
-    `pyslim.next_slim_id` (:user:`mufernando`, :pr:`290`).
-
-
 ***************************
-[1.0] - 2022-08-12
+[1.0 beta] - 2022-06-03
 ***************************
 
 **Breaking changes**:
 
-- Removed `SlimTreeSequence` class entirely (it was previously deprecated).
-    All its methods are either available in `tskit.TreeSequence`
-    or are now called by `pyslim.fn(ts, ...)` instead of `ts.fn(...)`.
+- Removed `SlimTreeSequence` class entirely.
 
 - TODO: Deprecated `util.unique_labels_by_group`.
 
+- TODO: what about `slim_ts.mutation_at` and `slim_ts.nucleotide_at` (used in a Recipe)
+
 - Moved some methods of `SlimTreeSequence` to pyslim:
     * instead of `slim_ts.slim_time(t)` do `pyslim.slim_time(ts, t)`
     * instead of `slim_ts.individuals_alive_at(t)` do `pyslim.individuals_alive_at(ts, t)`
     * instead of `slim_ts.individuals_parents(t)` do `pyslim.individuals_parents(ts, t)`
     * instead of `slim_ts.individuals_ages(t)` do `pyslim.individuals_ages(ts, t)`
 
-- The methods `slim_ts.mutation_at( )` and `slim_ts.nucleotide_at( )`
-    are now methods of pyslim, whose first argument is the tree sequence.
 
 - In SLiM v4 "generation" has been renamed to "tick", and so corresponding things
   in pyslim have been renamed: top-level metadata now has `ts.metadata["SLiM"]["tick"]`
   instead of `ts.metadata["SLiM"]["generation"]`
 
 - Renamed `pyslim.annotate_defaults()` to `pyslim.annotate()`, with slight
   changes in behavior: since msprime.sim_ancestry() now simulates individuals
   by default, annotation does not set up individuals: if you have a tree
   sequence without individuals (e.g., produced by msprime.simulate()) then you
   need to set up those individuals yourself.
 
 - To update a tree sequence produced by an old version of SLiM to the current one,
-  use `pyslim.update( )`. (However, note that reading it in to SLiM and
+  use `pyslim.update_tables( )`. (However, note that reading it in to SLiM and
   writing it out again might be even easier.)
 
 - The method `pyslim.set_tree_sequence_metadata` now has arguments `tick` and `cycle`
   instead of `generation`.
 
 - Removed `pyslim.make_slim_provenance_dict`.
 
 **Other notable changes**:
 
 - Top-level metadata now has a `tick` attribute that is (for now) a synonym
     for `generation`; the latter will be deprecated at some point in the future.
 
+- TODO: Individual properties `time` and `population` now moved to tskit
+
 - Methods for getting time, population, and location information about individuals
   are now in tskit:
     * `SlimTreeSequence.individual_times` is now `TreeSequence.individuals_time()`
-    * `SlimTreeSequence.individual_populations` is now `TreeSequence.individuals_population()`
+    * `SlimTreeSequence.individual_populations` is now `TreeSequence.individualx_population()`
     * `SlimTreeSequence.individual_locations` is now `TreeSequence.individuals_location()`
   However, this will be invisible to the user. In each case note the the
   location of the "s" has moved (to "individual*s* time" instead of "individual
   time*s*"), but the original version remains an undocumented alias.
 
-**New features**:
-
-- Methods like `pyslim.individuals_alive_at( )` now deal with the new `stage="first"`.
-
 
 ********************
 [0.700] - 2021-12-20
 ********************
 
 **Breaking changes**:
```

### Comparing `pyslim-1.0.2/LICENSE` & `pyslim-1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/PKG-INFO` & `pyslim-1.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyslim
-Version: 1.0.2
+Version: 1.0b1
 Summary: Manipulate tree sequences produced by SLiM.
 Home-page: https://github.com/tskit-dev/pyslim
 Author: Peter Ralph
 Author-email: petrel.harp@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/tskit-dev/pyslim/issues
 Project-URL: Source, https://github.com/tskit-dev/pyslim
 Keywords: tree sequences,tskit
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyslim
 
 `pyslim` is a python module that provides a few extra tools for dealing with tree sequences
@@ -26,7 +27,9 @@
 ## Installation
 
 To install `pyslim`, do
 ```
 pip install pyslim
 ```
 or read the documentation for how to [install from source](https://tskit.dev/pyslim/stable/development.html#sec-development).
+
+
```

### Comparing `pyslim-1.0.2/README.html` & `pyslim-1.0b1/README.html`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/README.md` & `pyslim-1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_config.yml` & `pyslim-1.0b1/docs/_config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 author: Tskit Developers
 copyright: "2021"
 only_build_toc_files: true
 # logo: logo.png
 
 execute:
   execute_notebooks: cache
-  timeout: 300
 
 repository:
   url: https://github.com/tskit-dev/pyslim
   branch: main
   path_to_book: docs
 
 html:
@@ -40,11 +39,10 @@
       todo_include_todos: true
       intersphinx_mapping:
         python: ["https://docs.python.org/3/", null]
         tskit: ["https://tskit.dev/tskit/docs/stable", null]
         msprime: ["https://tskit.dev/msprime/docs/stable", null]
         tutorials: ["https://tskit.dev/tutorials/", null]
         stdpopsim: ["https://popsim-consortium.github.io/stdpopsim-docs/stable", null]
-        numpy: ["https://numpy.org/doc/stable/", null]
       myst_enable_extensions:
       - colon_fence
       - deflist
```

### Comparing `pyslim-1.0.2/docs/_static/Makefile` & `pyslim-1.0b1/docs/_static/Makefile`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/annotate_genome.png` & `pyslim-1.0b1/docs/_static/annotate_genome.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/annotated_p_vs_s.png` & `pyslim-1.0b1/docs/_static/annotated_p_vs_s.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/export-layers-svg.sh` & `pyslim-1.0b1/docs/_static/export-layers-svg.sh`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree0.png` & `pyslim-1.0b1/docs/_static/pedigree0.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree0.svg` & `pyslim-1.0b1/docs/_static/pedigree0.svg`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree01.png` & `pyslim-1.0b1/docs/_static/pedigree01.png`

 * *Files 1% similar despite different names*

#### sng

```diff
@@ -12,29 +12,29 @@
 gAMA {0.45455}
 bKGD {red: 255;  green: 255;  blue: 255;}
 pHYs {xpixels: 11811; ypixels: 11811; per: meter;}  # (300 dpi)
 private caNv {
     hex 00000278 00000441 00000000 00000000 ;
 }
 tIME {
-    # 11 Aug 2022 19:45:13 GMT
-    year:   2022
-    month:  8
-    day:    11
-    hour:   19
-    minute: 45
-    second: 13
+    # 15 Dec 2021 09:42:16 GMT
+    year:   2021
+    month:  12
+    day:    15
+    hour:   9
+    minute: 42
+    second: 16
 }
 tEXt {
     keyword: "date:create";
-    text: "2022-08-11T19:45:12+00:00";
+    text: "2021-12-09T00:53:14+00:00";
 }
 tEXt {
     keyword: "date:modify";
-    text: "2022-08-11T19:45:12+00:00";
+    text: "2021-12-09T00:53:14+00:00";
 }
 tEXt {
     keyword: "Software";
     text: "www.inkscape.org";
 }
 IMAGE {
     pixels hex
```

### Comparing `pyslim-1.0.2/docs/_static/pedigree1.png` & `pyslim-1.0b1/docs/_static/pedigree1.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree1.svg` & `pyslim-1.0b1/docs/_static/pedigree1.svg`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree2.png` & `pyslim-1.0b1/docs/_static/pedigree2.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree2.svg` & `pyslim-1.0b1/docs/_static/pedigree2.svg`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree_mutate.png` & `pyslim-1.0b1/docs/_static/pedigree_mutate.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree_mutate.svg` & `pyslim-1.0b1/docs/_static/pedigree_mutate.svg`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree_recapitate.png` & `pyslim-1.0b1/docs/_static/pedigree_recapitate.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree_recapitate.svg` & `pyslim-1.0b1/docs/_static/pedigree_recapitate.svg`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree_remember.png` & `pyslim-1.0b1/docs/_static/pedigree_remember.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree_simplify.png` & `pyslim-1.0b1/docs/_static/pedigree_simplify.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigree_simplify.svg` & `pyslim-1.0b1/docs/_static/pedigree_simplify.svg`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/pedigrees.ink.svg` & `pyslim-1.0b1/docs/_static/pedigrees.ink.svg`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/phylo.pdf` & `pyslim-1.0b1/docs/_static/phylo.pdf`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/_static/phylo.png` & `pyslim-1.0b1/docs/_static/phylo.png`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/annotate_genome.pdf` & `pyslim-1.0b1/docs/annotate_genome.pdf`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/annotated_p_vs_s.pdf` & `pyslim-1.0b1/docs/annotated_p_vs_s.pdf`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/build.sh` & `pyslim-1.0b1/docs/build.sh`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/conf.py` & `pyslim-1.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/development.md` & `pyslim-1.0b1/docs/development.md`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/example_sim.slim` & `pyslim-1.0b1/docs/example_sim.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/generation_time.slim` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.3 - Simulation conditional upon fixation of a sweep, preserving ancestry II.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,34 @@
+// Keywords: tree-sequence recording, tree sequence recording, conditional sweep
+
 initialize() {
-	initializeSLiMModelType("nonWF");
-	initializeSex("A");
 	initializeTreeSeq();
-	initializeMutationRate(2e-8);
-	initializeMutationType("m1", 0.5, "f", 0.0);
-	initializeGenomicElementType("g1", m1, 1.0);
-	initializeGenomicElement(g1, 0, 1e8-1);
+	initializeMutationRate(1e-8);
+	initializeMutationType("m2", 0.5, "g", -0.01, 1.0);  // deleterious
+	initializeMutationType("m3", 1.0, "f", 0.05);        // introduced
+	initializeGenomicElementType("g1", m2, 1.0);
+	initializeGenomicElement(g1, 0, 99999);
 	initializeRecombinationRate(1e-8);
-	defineConstant("K", 1000);
-	defineGlobal("GENTIME", rep(NAN, 100));
-}
-
-reproduction(p1, "F") {
-	for (k in seqLen(rpois(1, individual.age))) {
-		mate = subpop.sampleIndividuals(1, sex="M");
-		offspring = subpop.addCrossed(individual, mate);
-	}
 }
-
 1 early() {
-	sim.addSubpop("p1", K);
+	defineConstant("simID", getSeed());
+	sim.addSubpop("p1", 500);
 }
-
-early() {
-	p1.fitnessScaling = K / p1.individualCount;
-}
-
-1: late() {
-	// this should happen *after* mortality (so, in late())
-	GENTIME[community.tick - 1] = mean(p1.individuals.meanParentAge);
-}
-
-100 late() {
-	sim.treeSeqOutput(
-		"generation_time.trees",
-		metadata=Dictionary("generation_times", GENTIME)
-		);
-	catn("Done! Mean generation time " + mean(GENTIME[50:99]));
+1000 late() {
+	target = sample(p1.genomes, 1);
+	target.addNewDrawnMutation(m3, 10000);
+	sim.treeSeqOutput("/tmp/slim_" + simID + ".trees");
+}
+1000:100000 late() {
+	if (sim.countOfMutationsOfType(m3) == 0) {
+		if (sum(sim.substitutions.mutationType == m3) == 1) {
+			cat(simID + ": FIXED\n");
+			sim.treeSeqOutput("slim_" + simID + "_FIXED.trees");
+			sim.simulationFinished();
+		} else {
+			cat(simID + ": LOST - RESTARTING\n");
+			
+			sim.readFromPopulationFile("/tmp/slim_" + simID + ".trees");
+			setSeed(rdunif(1, 0, asInteger(2^62) - 1));
+		}
+	}
 }
```

### Comparing `pyslim-1.0.2/docs/installation.md` & `pyslim-1.0b1/docs/installation.md`

 * *Files 21% similar despite different names*

```diff
@@ -11,28 +11,21 @@
   name: python3
 ---
 
 (sec_installation)=
 
 # Installation
 
-Pyslim can be installed using the standard [pip](https://pypi.org/project/pyslim/) distribution method:
+Pyslim can be installed using the standard [pip](https://pypi.org/project/pip/) distribution method:
 
 ```bash
 python3 -m pip install pyslim
 ```
 
-To install a [different version](https://pypi.org/project/pyslim/#history), e.g., 
-the 1.0 beta release whose version string is "1.0b1", just append this, like:
-
-```bash
-python3 -m pip install pyslim==1.0b1
-```
-
-Alternatively, you can install from source as described in [](sec_development).
+Alternatively, you can install from source as described in {ref}`sec_development`.
 
 
 ## Troubleshooting
 
 If you find a bug in ``pyslim`` or want to suggest an improvement, please
 [open an issue](https://github.com/tskit-dev/pyslim/issues) on our github page.
 If you have a question about using tree sequences,
```

### Comparing `pyslim-1.0.2/docs/introduction.md` & `pyslim-1.0b1/docs/introduction.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ---
 
 (sec_introduction)=
 
 # Introduction
 
 This is the documentation for pyslim, a Python API
-for reading and modifying [tskit](tskit:sec_introduction) tree sequence files
+for reading and modifying {ref}`tskit <tskit:sec_introduction>` tree sequence files
 produced by [SLiM](https://messerlab.org/slim/), 
 or modifying files produced by other programs (e.g.,
-[msprime](msprime:sec_intro),
+{ref}`msprime <msprime:sec_intro>`,
 [fwdpy11](https://fwdpy11.readthedocs.io/en/stable/pages/tsoverview.html),
 and [tsinfer](https://tsinfer.readthedocs.io/)) for use in SLiM. 
 
 SLiM can read and write *tree sequences*, which store genetic genealogies
 for entire populations. These can be used to efficiently encode both the state of the
 population at various points during a simulation *as well as* the complete genomic
 ancestry. Furthermore, SLiM can "load" a saved tree sequence
@@ -32,21 +32,21 @@
 tree sequence file.
 
 
 ## Overview
 
 A tree sequence is a way of storing both the full genetic history and the genotypes
 of a bunch of genomes.
-See [the tskit documentation](tskit:sec_introduction)
+See {ref}`the tskit documentation <tskit:sec_introduction>`
 for more description of the tree sequence and underlying data structure,
 and definitions of the important terms.
 Each (haploid) genome is associated with a *node*,
 and the "focal" nodes are called *sample nodes* or simply *samples*.
 Many operations on tree sequences act on the sample nodes by default (see the
-[tskit data model](tskit:sec_nodes_or_individuals)
+{ref}`tskit data model <tskit:sec_nodes_or_individuals>`
 for more on this topic), and the tree sequence always describes the genealogy of the
 entire genome of all the samples, at at least over the simulated time period.
 (Other nodes in the tree sequence represent ancestral genomes
 about which we might have only partial information).
 SLiM simulates diploid organisms, so each *individual* usually has two nodes;
 many operations you might want to do involve first finding the individuals you want,
 and then looking at their nodes.
@@ -100,15 +100,15 @@
 and the individuals containing them, are always present in the tree sequence.
 
 In contrast to the individuals containing sample nodes, you can see that all the other
 circles, representing historical (i.e., dead) individuals, have vanished, although
 sometimes their nodes remain. By default, only individuals with sample nodes are recorded
 in the tree sequence; that means the other, remaining, nodes lose any information about
 which individuals they were in (the tutorial explains ways to
-[retain this information](sec_retaining_individuals).
+{ref}`retain this information <sec_retaining_individuals>`).
 
 As well as the historical individuals, many historical *nodes*  have been removed too,
 along with with their genealogical relationships (i.e. the lines, which in
 tree-sequence-speak are known as "edges"). The deleted nodes are simply those that are
 not needed to reconstruct the relationships between the sample nodes. For example, we
 remove nodes leading to a dead end (e.g. in individuals who had no offspring). Similarly,
 as time goes on, recombination events in conjunction with genetic drift can gradually
@@ -123,9 +123,9 @@
 
 ## What else can I find out from the tree sequence?
 
 Enough information is stored in the tree sequence
 to completely reconstruct the state of the SLiM simulation
 (except for user-defined data, like a `tag`).
 Most of this is stored as *metadata*, which pyslim makes accessible:
-see [](sec_metadata).
+see {ref}`sec_metadata`.
```

### Comparing `pyslim-1.0.2/docs/migrants.slim` & `pyslim-1.0b1/docs/migrants.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/neutral_restart.slim` & `pyslim-1.0b1/docs/neutral_restart.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/phylo_bgs.slim` & `pyslim-1.0b1/docs/phylo_bgs.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/reload_annotated.slim` & `pyslim-1.0b1/docs/reload_annotated.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/time_units.md` & `pyslim-1.0b1/docs/metadata.md`

 * *Files 27% similar despite different names*

```diff
@@ -9,442 +9,339 @@
   display_name: Python 3
   language: python
   name: python3
 ---
 
 ```{code-cell}
 :tags: [remove-cell]
-import warnings
 import pyslim, tskit, msprime
 from IPython.display import SVG
 import numpy as np
-import matplotlib.pyplot as plt
+import random
+random.seed(23)
 
 ts = tskit.load("example_sim.trees")
+tables = ts.tables
 ```
 
 ```{eval-rst}
 .. currentmodule:: pyslim
 ```
 
-# Time units
 
-There are a number of subtle ways that time units can trip up the user;
-below are explanations of how to deal with most of these topics.
-At issue is the fact that tree sequences produced by SLiM
-have times in units of "ticks", rather than generations. 
-If we query such a tree sequence for its time units we see 
-its return value
-```{code-cell}
-ts.time_units
-```
-
-In general this mean it can be conceptually tricky to make sure that time units
-are consistent across different stages of simulation.
-
-(Note: it *is* possible to set the time units to whatever you want,
-using the ``timeUnit`` parameter to ``initializeTreeSeq( )``,
-but this only affects this label in metadata (i.e., the output of
-``ts.time_units``, and does not actually change how times are recorded
-in the tree sequence.)
-
-
-## Mutation rates with msprime
-
-Only you really know how much time in the real world
-corresponds to one spin around SLiM's life cycle.
-one spin around SLiM's life cycle corresponds to.
-So, SLiM does not specify what its time units actually are,
-and refers to them as "ticks".
-Previous versions of SLiM called these "generations",
-but this is only correct for simulations in which all organisms die every tick.
-Converting these times into real-world times is usually not too hard:
-maybe in your simulation one tick = one year,
-or maybe you need to multiply by a (mean) generation time known from empirical data.
-
-However, it becomes important to know what the time units are
-when interfacing with msprime.
-For instance, suppose you've done a WF simulation for an organism whose mean generation time
-in the real world is 30 years, and you want to overlay neutral mutations using msprime.
-The mutation rate passed to msprime is in units of mutations per unit-of-time-in-the-tree-sequence,
-so since you did a WF simulation, the units of time in the tree sequence are in generations,
-and you should give it mutation rate in mutations per generation.
-The rate in units of mutations per year would be 30 times smaller,
-and so would give you 30 times fewer neutral mutations than you want.
-Conversely, if you did a nonWF simulation where one tick = one year,
-then you'd want the mutation rate in units of mutations per year.
-
-## Coalescence, recombination, and migration rates in recapitation
-
-If you recapitate with msprime, then the same issue occurs for coalescence rates.
-This is less obvious, because "coalescence rate" is not an argument to msprime;
-rather, the coalescence rate in a given population
-is {math}`1/2N`, where {math}`N` is the (effective) size of that population.
-(The 2 in the denominator is actually the 'ploidy' argument to msprime, which defaults to 2.)
-This is the correct rate, *in units of coalescences per generation*.
-Since it's "per generation", this means that if you want to recapitate a tree sequence
-generated by SLiM in which one tick is not one generation,
-then **you need to adjust the effective population sizes accordingly**.
-For instance, suppose as above that we did a nonWF simulation
-in which one tick = one year, for a species with generation time 30 years,
-and we want to recapitate with an effective size of 10,000 diploids.
-An effective size of 10,000 diploids means one coalescence per pair of lineages
-every 20,000 generations;
-since one unit of time in the tree sequence equals 1/30th of a generation,
-this is one coalescence per pair of lineages every 600,000 time units,
-which we can get msprime to do by asking for an effective population size of 300,000.
-In other words, if a generation in our tree sequence is {math}`T` units of time,
-then we need to divide the coalescence rate by {math}`T,`
-which we do by multiplying effective population sizes by {math}`T`.
-
-(A better way of thinking about this could be to say that since the mean time to coalescence
-is twice the effective population size,
-actually effective population size is in units of *time*, rather than individuals.)
-
-To recapitate we need to also pick recombination and (possibly) migration rates.
-Since these are rates, they are also in units of something "per time",
-and so just as for mutation rates, we need to ensure they are in the correct units.
-Recombination rates in particular come in units of "per generation"
-(since a Morgan is in units of recombinations per generation),
-and so a rate of {math}`r` Morgans would need to be divided by {math}`T`
-before it's passed to msprime for recapitation.
-Since msprime (by default) runs a continuous-time simulation,
-there is no harm in adjusting time units in msprime this way,
-but it is confusing.
-
-
-### `TimeUnitsMismatchWarning`
-
-Above we saw that if we want msprime to simulate coalescence in a population of size 10,000
-to recapitate our tree sequence whose times are given in units of 1/30th of a generation, 
-then we need to ask it for a population of (effective) size 300,000.
-In other words, the "population sizes" of msprime are *only* in units of individuals
-(as one would expect a population size to be)
-*if* times are being measured in units of generations.
-For this reason, although it's not strictly true,
-sometimes we say that "msprime times are in units of generations".
-Also, msprime will produce a warning if it is handed a tree sequence
-whose time units are not "generations":
-
-```{code-cell}
-:tags: ["remove-output"]
-rts = pyslim.recapitate(ts,
-            recombination_rate=1e-8,
-            ancestral_Ne=200, random_seed=5)
-```
-```{code-cell}
-:tags: ["remove-input"]
-import textwrap
-with warnings.catch_warnings(record=True) as w:
-    rts = pyslim.recapitate(ts,
-                recombination_rate=1e-8,
-                ancestral_Ne=200, random_seed=5)
-    print("\n".join(textwrap.wrap(f"TimeUnitsMismatchWarning: {str(w[0].message)}", width=90)))
-```
-
-Think of this warning as a friendly reminder to pay attention to your time units.
-To make this warning disappear, the easiest option is to do as the warning suggests
-and just ask python to ignore it:
-
-```{code-cell}
-import warnings
-warnings.simplefilter('ignore', msprime.TimeUnitsMismatchWarning)
-rts = pyslim.recapitate(ts,
-            recombination_rate=1e-8,
-            ancestral_Ne=200, random_seed=5)
-```
-
-To re-label the time units on your tree sequence
-as being in "generations" (but! only do this if it's true!),
-you must convert to a TableCollection and back (since the tables are mutable
-but the tree sequence is not):
-
-```{code-cell}
-print(f"Time units before: {ts.time_units}")
-t = ts.dump_tables()
-t.time_units = 'generations'
-ts = t.tree_sequence()
-print(f"Time units after: {ts.time_units}")
-```
-
-## Example: calculating generation times in a SLiM simulation
-
-In a nonWF simulation, the generation time is not something that you get to explicitly set:
-rather, like population size it is an emergent property of the rules of the simulation.
-So, it's important to be able to calculate what the (average) generation time actually is
-in a given simulation (keeping in mind that the answer may vary across time and space).
-This is not really a pyslim operation at all,
-but since it's important to the considerations above,
-here's an easy way to do this.
-The definition of generation time appropriate for comparison to a coalescent simulation
-is "average amount of time between birth of parent and birth of child".
-(Note that this is the birth of the *average* child in some sense,
-not the average time to each parent's first child!)
-Therefore,
-an easy and convenient way to measure this is to
-record for each individual their parents' ages at the times of their births,
-and then take the average across all individuals alive at a given time.
-(This is only one possible choice,
-and other choices are usually but not always equivalent,
-but a discussion of the options and distinctions
-would make this tutorial lengthy and confusing.
-
-Here is a script that computes this.
-In the simulation, females' fecundity increases with their age,
-and so we expect "generation time" to be larger than the mean age of individuals
-alive at a given time.
-In the script, we store the average of the mean parent ages across all 
-extant individuals every tick using SLiM Individuals' `meanParentAge` property, 
-and store the vector in top-level metadata when we write out the tree sequence.
-
-```{literalinclude} generation_time.slim
-```
-```{code-cell}
-%%bash
-slim -s 23 generation_time.slim | tail -n1
-```
-
-(About the warning: we turned on mutations for a good reason; see below.)
-Now we can look at our empirical calculation of generation time.
-Note that the first generation individuals have a mean parent age of 0.0,
-so we expect generation time to go up at first.
+(sec_metadata)=
 
-```{code-cell}
-gts = tskit.load("generation_time.trees")
-gentimes = gts.metadata["SLiM"]["user_metadata"]["generation_times"]
-
-fig, ax = plt.subplots(figsize=(12, 6), dpi=300)
-ax.set_xlabel("tick")
-ax.set_ylabel("generation time")
-ax.plot(np.arange(1, len(gentimes)+1), gentimes);
-```
-
-In the script above we added mutations during the SLiM simulation to do a simple check 
-to verify the `meanParentAge` property correctly estimates mean generation time. 
-If it does, then the mean sequence divergence calculated from the mutations introduced by SLiM
-should (approximately) match the mean length of branches in the tree sequence separating two samples
-multiplied by the expected number of mutations per unit time.
-(We get the mean branch length using the {meth}`ts.diversity <tskit.TreeSequence.diversity>` method with ``mode="branch"``;
-see the [tskit documentation](tskit:sec_stats) for details.)
-This involves the generation time because "mutations per unit time" is equal to
-"mutations per generation" (here, the mutation rate per bp, {math}`10^{-8}`)
-divided by "time per generation" (i.e., mean generation time).
+# Metadata
 
+(sec_metdata_overview)=
 
-```{code-cell}
-slim_diversity = gts.diversity(mode = 'site')
-ts_diversity = gts.diversity(mode='branch') * 1e-8 / np.mean(gentimes)
-
-print(f"slim diversity: {slim_diversity}\n"
-      f"scaled tree sequence diversity: {ts_diversity}\n"
-      f"error: {100 * np.abs(slim_diversity - ts_diversity)/slim_diversity:0.3f}%"
-)
-```
+## Overview
 
-Now, to recapitate this simulation
-in a population with effective size 1000,
-and using the recombination rate from the SLiM script of {math}`10^{-8}`
-crossovers per generation
-and {math}`2 \times 10^{-8}` mutations per generation,
-we need to scale {math}`N_e` and both rates by the generation time.
-Furthermore, since we already have mutations up until 100 time units ago,
-we need to put mutations on only previous to that time.
+SLiM puts SLiM-specific information into the *metadata* for the tree sequence,
+as well as for each populations, individuals, nodes and mutations.
+Here is a quick reference to what information is available:
+see the SLiM manual for the more technical writeup.
+A good way to get a generic metadata example is with {func}`.default_slim_metadata`.
+
+**Top-level:**
+If `ts` is your tree sequence, then `ts.metadata` is a dict,
+and `ts.metadata["SLiM"]` contains information about the simulation:
+
+- `file_version`: the version of the SLiM tree sequence file format
+- `tick`: the value of `community.tick` within SLiM when the file was written out
+- `cycle`: the value of `sim.cycle` within SLiM when the file was written out
+- `model_type`: either `"WF"` or `"nonWF"`
+- `nucleotide_based`: whether this is a nucleotide-based simulation
+- `separate_sexes`: whether the simulation has separate sexes or not
+- `spatial_dimensionality`: for instance, `""` or `"x"` or `"xy"` (etcetera)
+- `spatial_periodicity`: whether space wraps around in some directions (same format as dimensionality)
+- `stage`: the *stage* of the life cycle at which the file was written out (either `"first"`, `"early"`, or `"late"`)
+
+**Populations:**
+Information about each SLiM-produced population is written to metatadata.
+The format uses JSON and is extensible, so other keys may be present
+and some keys may be missing (for instance, there are no spatial bounds
+in a nonspatial simulation). The metadata may be `None` for populations
+that SLiM did not use. The keys that SLiM uses are:
+
+- `slim_id`: the ID of this population in SLiM
+- `name`: the name of the population (by default, `p0`, `p1`, etcetera)
+- `description`: a string describing the population
+- `selfing_fraction`, `female_cloning_fraction`, `male_cloning_fraction`, and `sex_ratio`: only present when applicable (e.g., in WF simulations)
+- `bounds_x0`, `bounds_x1`, `bounds_y0`, `bounds_y1`, `bounds_z0`, and `bounds_z1`: the spatial bounds, when applicable
+- `migration_records`: A *list* of entries decribing migration between populations in a WF model.
+
+**Individuals:**
+Each individual produced by SLiM contains the following metadata:
+
+- `pedigree_id`: the "pedigree ID", unique within the SLiM simulation
+- `pedigree_p1`, `pedigree_p2`: the pedigree IDs of the individuals' two
+  parents (they may be equal in the case of selfing, or `-1` to indicate no
+  parent, in the case of the initial generation or for cloning)
+- `age`: the `.age` property within SLiM at the time the file was written out
+- `subpopulation`: the subpopulation within SLiM the individual was in at the time the file was written out
+- `sex`: the sex of the individual (either {data}`.INDIVIDUAL_TYPE_FEMALE`, {data}`.INDIVIDUAL_TYPE_MALE`, or {data}`.INDIVIDUAL_TYPE_HERMAPHRODITE`)
+- `flags`: additional information; currently only recording whether the individual was a "migrant" or not (see the SLiM manual)
+
+**Nodes:**
+Each "node" produced by SLiM (i.e., "genome" within SLiM) has:
+
+- 'slim_id': the unique ID associated with the genome by SLiM
+- 'is_null': whether the genome is a "null" genome (in which case it isn't
+  really there, so shouldn't have any mutations or relationships in the tree
+  sequence!)
+- 'genome_type': the 'type' of this genome (0 for autosome, 1 for X, 2 for Y)
+
+**Mutations:**
+Each mutation's metadata is a dictionary with a single key, `"mutation_list"`,
+whose entry is a *list* of metadata dictionaries corresponding to the mutations that are "stacked",
+i.e., all present, in all genomes inheriting from this (tskit) mutation.
+So, `ts.mutation(12).metadata["mutation_list"]` is a list, each of whose entries contains:
+
+- `mutation_type`: the numeric ID of the `MutationType` within SLiM
+- `selection_coeff`: the selection coefficient
+- `subpopulation`: the numeric ID of the subpopulation the mutation occurred in
+- `slim_time`: the value of `community.tick` when the mutation occurred
+- `nucleotide`: either `-1` if there is no associated nucleotide, or the numeric code for the nucleotide (see {data}`.NUCLEOTIDES`)
+
+
+(sec_metadata_tools)=
+
+## Metadata tools
+
+The dictionaries describing the schema for these metadata entries
+are available in {data}`.slim_metadata_schemas`.
+Furthermore, this method may be useful in working with metadata:
 
-```{code-cell}
-gentimes = gts.metadata["SLiM"]["user_metadata"]["generation_times"]
-gt = np.mean(gentimes[-50:])
-recomb_rate = 1e-8 # per generation
-Ne = 1000 # generations
-mut_rate = 2e-8 # per generation
-with warnings.catch_warnings(record=True) as w:
-    rts = pyslim.recapitate(gts,
-                recombination_rate=recomb_rate / gt,
-                ancestral_Ne=Ne * gt,
-                random_seed=5)
-    mts = msprime.sim_mutations(
-               rts,
-               rate=mut_rate / gt,
-               model=msprime.SLiMMutationModel(type=0),
-               keep=True,
-               start_time=100,
-    )
-
-print(f"Mean genetic diversity is now {mts.diversity():.2e},\n"
-      f"  and the expected value under a WF model is "
-      f"4 * N * mu = {4 * Ne * mut_rate:.2e}")
+```{eval-rst}
+.. autofunction:: default_slim_metadata
 ```
 
-We get a lower value of genetic diversity than expected under a WF model,
-but that's expected because both fluctuating population sizes
-and age-associated variability in fecundity will decrease the effective population size.
-
 
 (sec_metadata_converting_times)=
 
-## Converting from SLiM time to tskit time and back
+## Converting from SLiM time to tskit time
 
 :::{note}
 This is a nitpicky, document-the-details section.
 Hopefully, you don't have to deal with the specifics of converting between tskit and SLiM time,
 but this page is here for you if you do.
 :::
 
 SLiM is a forwards simulator, while the tree sequence format thinks about things
 *retrospectively*, and so works with times in units of *time ago*.
 Mostly, you don't have to convert between the two,
 unless you want to match up information in a tree sequence
 with information written out by SLiM itself.
 In other words, SLiM's time counter measures the number of time steps
-("ticks") since the start of the simulation,
+("tick") since the start of the simulation,
 and times in the tree sequence record how long before the end of the simulation.
-However, there are quite a few details, and off-by-one errors are easy to make,
-so we'll spell it out here.
-Hopefully, you can just use pyslim's methods
-{func}`.slim_time`, {func}`.individuals_alive_at`,
-and {func}`.individual_ages_at`
-without needing to actually do any conversions yourself.
+However, there are Some Details, and off-by-one errors are easy to make,
+so we'll spell it out in detail.
 
-SLiM's time counter is called the "tick".
+SLiM's time counter is called the "tick"
+(although a "year" or "life cycle" would be a more appropriate name for a nonWF model).
 The SLiM tick starts at 1, and records which round of the life cycle the simulation is in.
 However, the order of the life cycle differs between WF and nonWF models:
-in a WF model, it is *first* {math}`\to` *early* {math}`\to` *birth* {math}`\to` *late*",
-while in a nonWF model, it is *first* {math}`\to` *birth* {math}`\to` *early* {math}`\to` *late*.
-Often, the first set of individuals are created in the *early()* phase of tick 1,
+in a WF model, it is "*early* {math}`\to` *birth* {math}`\to` *late*",
+while in a nonWF model, it is "*birth* {math}`\to` *early* {math}`\to` *late*".
+Usually, the first set of individuals are created in the *early()* phase of tick 1,
 and so in a WF model reproduce immediately, in the same tick they were "born".
 Parents and offspring cannot have the same birth time in the tree sequence,
 and so some clever bookkeeping was required.
 You'll want to refer to the tables below to see what's going on.
 "Time" in a tree sequence is actually *time ago*,
 or *time before the tree sequence was recorded*.
 To obtain this number, and ensure that offspring cannot have the same birth time-ago
 in the tree sequence as their parents,
 SLiM also keeps track of "how many birth phases of the life cycle have happened so far"
 (the column "# births" in the tables).
 As the simulation goes along,
 tskit time ago is recorded as minus one times the number of birth phases so far.
-(We multiply by -1 because as we move forward in time,
-we accumulate a negative number of "time-ago" units.)
 When the tree sequence is output, the current cumulative number of birth phases
 is added to this,
 so "tskit time ago" is, equivalently, "how many birth phases happened since this time".
 In a nonWF model, the two counters ("tick" and "number of birth phases")
-are always in sync; but in a WF model they are not (during *first* and *early*).
+are always in sync; but in a WF they are not (during *early*).
 The extra wrinkle this introduces is that the correspondence between "tskit time ago"
-and "SLiM time" depends on *which phase the tree sequence was recorded in*.
+and "SLiM time" depends on *which phase the tree sequence was recorded in*,
+but only for WF models.
+
+To help keep all this straight, here are schematics for WF and nonWF models.
+(To see the nonWF model, click on the tab.)
+
+```{tabbed} WF model
+
+For a WF model, the SLiM tick (first column) can be obtained by subtracting the
+tskit time ago from the SLiM tick at time of output only during the same stage that output occured in.
+
+|    tick            |       stage         |  # births          |                                |  tskit time ago, early output |   tskit time ago, late output |
+|--------------------|---------------------|--------------------|--------------------------------|-------------------------------|-------------------------------|
+|       1            |       early         |       0            | {math}`\leftarrow` add subpops |        n-1                    |         n                     |
+|       1            |       birth         |       1            |                                |        n-2                    |         n-1                   |
+|       1            |       late          |       1            |                                |        n-2                    |         n-1                   |
+|       2            |       early         |       1            |                                |        n-2                    |         n-1                   |
+|       2            |       birth         |       2            |                                |        n-3                    |         n-2                   |
+|       2            |       late          |       2            |                                |        n-3                    |         n-2                   |
+|       3            |       early         |       2            |                                |        n-3                    |         n-2                   |
+|       3            |       birth         |       3            |                                |        n-4                    |         n-3                   |
+|       3            |       late          |       3            |                                |        n-4                    |         n-3                   |
+| {math}`\downarrow` | {math}`\cdots`      | {math}`\downarrow` |                                | {math}`\uparrow`              | {math}`\uparrow`              |
+|       n-2          |       early         |       n-3          |                                |        2                      |         2                     |
+|       n-2          |       birth         |       n-2          |                                |        1                      |         2                     |
+|       n-2          |       late          |       n-2          |                                |        1                      |         2                     |
+|       n-1          |       early         |       n-2          |                                |        1                      |         2                     |
+|       n-1          |       birth         |       n-1          |                                |        0                      |         1                     |
+|       n-1          |       late          |       n-1          |                                |        0                      |         1                     |
+|       n            |       early         |       n-1          |  treeSeqOutput {math}`\to`     |        0                      |         1                     |
+|       n            |       birth         |       n            |                                |                               |         0                     |
+|       n            |       late          |       n            |                                | treeSeqOutput {math}`\to`     |         0                     |
+
+```
+
+```{tabbed} nonWF model
 
-When the tree sequence is written out, SLiM records the value of its current tick
-and the current stage,
-which can be found in the metadata: ``ts.metadata['SLiM']['tick']``,
-and ``ts.metadata['SLiM']['stage']``.
-The "SLiM time" referred to by a ``time`` in the tree sequence
+Note that for nonWF models the SLiM time (first column) can always be obtained by subtracting the
+tskit time ago from the SLiM time at time of output.
+
+|    tick            |       stage         |  # births          |                                |  tskit time ago, early output |   tskit time ago, late output |
+|--------------------|---------------------|--------------------|--------------------------------|-------------------------------|-------------------------------|
+|       1            |       birth         |       1            |                                |        n-1                    |         n-1                   |
+|       1            |       early         |       1            | {math}`\leftarrow` add subpops |        n-1                    |         n-1                   |
+|       1            |       late          |       1            |                                |        n-1                    |         n-1                   |
+|       2            |       birth         |       2            |                                |        n-2                    |         n-2                   |
+|       2            |       early         |       2            |                                |        n-2                    |         n-2                   |
+|       2            |       late          |       2            |                                |        n-2                    |         n-2                   |
+|       3            |       birth         |       3            |                                |        n-3                    |         n-3                   |
+|       3            |       early         |       3            |                                |        n-3                    |         n-3                   |
+|       3            |       late          |       3            |                                |        n-3                    |         n-3                   |
+| {math}`\downarrow` | {math}`\cdots`      | {math}`\downarrow` |                                | {math}`\uparrow`              | {math}`\uparrow`              |
+|       n-2          |       birth         |       n-2          |                                |        2                      |         2                     |
+|       n-2          |       early         |       n-2          |                                |        2                      |         2                     |
+|       n-2          |       late          |       n-2          |                                |        2                      |         2                     |
+|       n-1          |       birth         |       n-1          |                                |        1                      |         1                     |
+|       n-1          |       early         |       n-1          |                                |        1                      |         1                     |
+|       n-1          |       late          |       n-1          |                                |        1                      |         1                     |
+|       n            |       birth         |       n            |                                |        0                      |         0                     |
+|       n            |       early         |       n            |  treeSeqOutput {math}`\to`     |        0                      |         0                     |
+|       n            |       late          |       n            |                                | treeSeqOutput {math}`\to`     |         0                     |
+
+```
+When the tree sequence is written out, SLiM records the value of its current tick,
+which can be found in the metadata: ``ts.metadata['SLiM']['tick']``.
+In most cases, the "SLiM time" referred to by a ``time`` in the tree sequence
 (i.e., the value that would be reported by ``community.tick``
 within SLiM at the point in time thus referenced)
-can be obtained by subtracting ``time`` from ``ts.metadata['SLiM']['tick']``
-and possibly adding or subtracting one depending on the current stage.
-The fiddly details are worked out by the {func}`.slim_time` method,
-which takes a ``stage`` argument.
+can be obtained by subtracting ``time`` from ``ts.metadata['SLiM']['tick']``.
+**However,** in WF models, birth happens between the "early()" and "late()" stages,
+so if the tree sequence was written out using ``sim.treeSeqOutput()`` during "early()" in a WF model,
+the tree sequence's times measure time before the last set of individuals are born,
+i.e., before SLiM time step ``ts.metadata['SLiM']['tick'] - 1``.
+The stage that the tree sequence was saved is recorded in the metadata of the tree sequence,
+as ``ts.metadata['SLiM']['stage']``.
+Using this, we can convert from the times of a tree sequence ``ts``
+to SLiM time as follows:
+
+```{code-cell}
+def slim_time(ts, time, stage):
+  slim_time = ts.metadata["SLiM"]["tick"] - time
+  if ts.metadata['SLiM']['model_type'] == "WF":
+    if (ts.metadata['SLiM']['stage'] == "early"
+        and stage == "late"):
+        slim_time -= 1
+    if (ts.metadata['SLiM']['stage'] == "late"
+        and stage == "early"):
+        slim_time += 1
+  return slim_time
+```
 
-Some of the other methods in pyslim -- those that depend on {func}`.individuals_alive_at`
+This is what is computed by the {meth}`.SlimTreeSequence.slim_time` method
+(which also has a ``stage`` argument).
+
+Some of the other methods in pyslim -- those that depend on {meth}`pyslim.individuals_alive_at`
 -- need you to tell them during which stage the tree sequence was saved with ``sim.treeSeqOutput``,
 and need this to be the same as the stage that any individuals were saved with ``sim.treeSeqRememberIndividuals``.
-(This can add another factor of plus or minus one to the calculations.)
-This argument, ``remembered_stage``, defaults to *late()*;
+This argument, ``remembered_stage``, defaults to "late()";
 we recommend that you also default to always Remembering individuals, and saving out the tree sequence,
-during *late()* as well, unless you have good reason not to.
+during "late()" as well, unless you have good reason not to.
+(This means you *must specify* the stage of the block in your SLiM script,
+since the stage defaults to "early()"!)
 
-### Detailed description of conversion
 
+## Modifying SLiM metadata
 
-To help keep all this straight, here are schematics for WF and nonWF models.
-(To see the nonWF model schematic, click on the "nonWF" tab.)
+For more on working with metadata,
+see {ref}`tskit's metadata documentation <tskit:sec_metadata>`.
 
-````{tab-set}
-```{tab-item} WF model
 
-For a WF model, the SLiM tick (first column) can be obtained by subtracting the
-tskit time ago from the SLiM tick at time of output only during the same stage that output occured in.
-Suppose that we want to know what tick counter in SLiM corresponds to a given tskit time ago.
-The answer to this depends on what stage, unfortunately.
-Let {math}`k` be the value of the tick counter, {math}`n` be the total number of ticks,
-i.e., the value of ``ts.metadata["SLiM"]["tick"]``,
-{math}`t` be the tskit time,
-{math}`x=1` if the stage is *first()* or *early()* and 0 otherwise,
-and {math}`y=1` if the tree sequence was output in *late()*.
-Then, as can be verified from the table below, {math}`k + t = n + x + y - 1`.
-The right-hand columns show {math}`t`, i.e.,
-what the **tskit time ago** is at the corresponding point in the SLiM simulation.
-
-|    tick            |       stage         |  # births          |                                |  ``first`` output         |  ``early`` output         |   ``late`` output |
-|--------------------|---------------------|--------------------|--------------------------------|---------------------------|---------------------------|-------------------|
-|       1            |       first         |       0            | {math}`\leftarrow` add subpops |        n-1                |        n-1                |         n         |
-|       1            |       early         |       0            |                                |        n-1                |        n-1                |         n         |
-|       1            |       birth         |       1            |                                |        n-2                |        n-2                |         n-1       |
-|       1            |       late          |       1            |                                |        n-2                |        n-2                |         n-1       |
-|       2            |       first         |       1            |                                |        n-2                |        n-2                |         n-1       |
-|       2            |       early         |       1            |                                |        n-2                |        n-2                |         n-1       |
-|       2            |       birth         |       2            |                                |        n-3                |        n-3                |         n-2       |
-|       2            |       late          |       2            |                                |        n-3                |        n-3                |         n-2       |
-|       3            |       first         |       2            |                                |        n-3                |        n-3                |         n-2       |
-|       3            |       early         |       2            |                                |        n-3                |        n-3                |         n-2       |
-|       3            |       birth         |       3            |                                |        n-4                |        n-4                |         n-3       |
-|       3            |       late          |       3            |                                |        n-4                |        n-4                |         n-3       |
-| {math}`\downarrow` | {math}`\cdots`      | {math}`\downarrow` |                                | {math}`\uparrow`          | {math}`\uparrow`          | {math}`\uparrow`  |
-|       n-2          |       first         |       n-3          |                                |        2                  |        2                  |         2         |
-|       n-2          |       early         |       n-3          |                                |        2                  |        2                  |         2         |
-|       n-2          |       birth         |       n-2          |                                |        1                  |        1                  |         2         |
-|       n-2          |       late          |       n-2          |                                |        1                  |        1                  |         2         |
-|       n-1          |       first         |       n-2          |                                |        1                  |        1                  |         2         |
-|       n-1          |       early         |       n-2          |                                |        1                  |        1                  |         2         |
-|       n-1          |       birth         |       n-1          |                                |        0                  |        0                  |         1         |
-|       n-1          |       late          |       n-1          |                                |        0                  |        0                  |         1         |
-|       n            |       first         |       n-1          |  treeSeqOutput {math}`\to`     |        0                  |        0                  |         1         |
-|       n            |       early         |       n-1          |                                | treeSeqOutput {math}`\to` |        0                  |         1         |
-|       n            |       birth         |       n            |                                |                           |                           |         0         |
-|       n            |       late          |       n            |                                |                           | treeSeqOutput {math}`\to` |         0         |
+### Top-level metadata
 
-```
+The entries of the top-level metadata dict are *read-only*.
+So, you might think that
+`tables.metadata["SLiM"]["model_type"] = "nonWF"`
+would switch the model type,
+but this in fact (silently) does nothing. To modify the top-level metadata,
+we must (a) work with tables (as tree sequences are immutable, and (b)
+extract the metadata dict, modify the dict, and copy it back in.
+Instead, you should do
+```{code-cell}
+md = tables.metadata
+md["SLiM"]["model_type"] = "nonWF"
+tables.metadata = md
+```
+Modifying the top-level metadata
+could be used to set spatial bounds on an annotated msprime simulation, for instance.
+(This is recorded in the population metadata.)
+
+
+### Modifying SLiM metadata in tables
+
+
+To modify the metadata that ``pyslim`` has introduced into
+the tree sequence produced by a coalescent simulation,
+or the metadata in a SLiM-produced tree sequence,
+we need to edit the TableCollection that forms the editable data behind the tree sequence.
+For instance, to set the ages of the individuals in the tree sequence to random numbers between 1 and 4,
+we will extract a copy of the underlying tables, clear it,
+and then iterate over the individuals in the tree sequence,
+as we go re-inserting them into the tables
+after replacing their metadata with a modified version:
 
-```{tab-item} nonWF model
+```{code-cell}
+tables = ts.dump_tables()
+tables.individuals.clear()
+for ind in ts.individuals():
+    md = ind.metadata
+    md["age"] = random.choice([1,2,3,4])
+    _ = tables.individuals.append(
+        ind.replace(metadata=md)
+    )
 
-Note that for nonWF models the SLiM time (first column) can always be obtained by subtracting the
-tskit time ago from the SLiM time at time of output.
-Suppose that we want to know what tick counter in SLiM corresponds to a given tskit time ago.
-The answer to this depends on what stage, unfortunately.
-Let {math}`k` be the value of the tick counter, {math}`n` be the total number of ticks,
-i.e., the value of ``ts.metadata["SLiM"]["tick"]``,
-let {math}`t` be the tskit time,
-{math}`x=1` if the stage is "first" and 0 otherwise,
-and {math}`y=1` if the tree sequence was output in *early()* or *late()*.
-Then, as can be verified from the table below, {math}`k + t = n + x + y - 1`.
-The right-hand columns show {math}`t`, i.e.,
-what the **tskit time ago** is at the corresponding point in the SLiM simulation.
-
-|    tick            |       stage         |  # births          |                                |  first output              |  early output              |   late output    |
-|--------------------|---------------------|--------------------|--------------------------------|----------------------------|----------------------------|------------------|
-|       1            |       first         |       0            | {math}`\leftarrow` add subpops |        n-1                 |        n                   |         n        |
-|       1            |       birth         |       1            |                                |        n-2                 |        n-1                 |         n-1      |
-|       1            |       early         |       1            | {math}`\leftarrow` add subpops |        n-2                 |        n-1                 |         n-1      |
-|       1            |       late          |       1            |                                |        n-2                 |        n-1                 |         n-1      |
-|       2            |       first         |       1            |                                |        n-2                 |        n-1                 |         n-1      |
-|       2            |       birth         |       2            |                                |        n-3                 |        n-2                 |         n-2      |
-|       2            |       early         |       2            |                                |        n-3                 |        n-2                 |         n-2      |
-|       2            |       late          |       2            |                                |        n-3                 |        n-2                 |         n-2      |
-|       3            |       first         |       2            |                                |        n-3                 |        n-2                 |         n-2      |
-|       3            |       birth         |       3            |                                |        n-4                 |        n-3                 |         n-3      |
-|       3            |       early         |       3            |                                |        n-4                 |        n-3                 |         n-3      |
-|       3            |       late          |       3            |                                |        n-4                 |        n-3                 |         n-3      |
-| {math}`\downarrow` | {math}`\cdots`      | {math}`\downarrow` |                                | {math}`\uparrow`           | {math}`\uparrow`           | {math}`\uparrow` |
-|       n-2          |       first         |       n-3          |                                |        2                   |        3                   |         3        |
-|       n-2          |       birth         |       n-2          |                                |        1                   |        2                   |         2        |
-|       n-2          |       early         |       n-2          |                                |        1                   |        2                   |         2        |
-|       n-2          |       late          |       n-2          |                                |        1                   |        2                   |         2        |
-|       n-1          |       first         |       n-2          |                                |        1                   |        2                   |         2        |
-|       n-1          |       birth         |       n-1          |                                |        0                   |        1                   |         1        |
-|       n-1          |       early         |       n-1          |                                |        0                   |        1                   |         1        |
-|       n-1          |       late          |       n-1          |                                |        0                   |        1                   |         1        |
-|       n            |       first         |       n-1          |  treeSeqOutput {math}`\to`     |        0                   |        1                   |         1        |
-|       n            |       birth         |       n            |                                |                            |        0                   |         0        |
-|       n            |       early         |       n            |                                |  treeSeqOutput {math}`\to` |        0                   |         0        |
-|       n            |       late          |       n            |                                |                            | treeSeqOutput {math}`\to`  |         0        |
+mod_ts = tables.tree_sequence()
 
-```
-````
+# check that it worked:
+print("First ten ages:", [mod_ts.individual(i).metadata["age"] for i in range(10)])
+for ind in mod_ts.individuals():
+    assert ind.metadata['age'] in [1, 2, 3, 4]
+
+# save out the tree sequence
+mod_ts.dump("modified_ts.trees")
+```
+
+## Technical details
+
+### Metadata entries
+
+SLiM records additional information in the metadata columns of Individual, Node, and Mutation tables,
+in a binary format using the python ``struct`` module.
+See {ref}`tskit's metadata documentation <tskit:sec_metadata>`
+for details on how this works.
+Nothing besides this binary information can be stored in the metadata of these tables if the tree sequence is to be used by SLiM,
+and so when ``pyslim`` annotates an existing tree sequence, anything in those columns is overwritten.
+Population metadata is stored as JSON, however, which is more flexible.
+For more detailed documentation on the contents and format of the metadata, see the SLiM manual.
+
+Of particular note is that *nodes* and *populations* may have empty metadata.
+SLiM will not use the metadata of nodes that are not associated with alive individuals,
+so this can safely be omitted (and makes recapitation easier).
+And, populations not used by SLiM will have empty metadata.
+All remaining metadata are required (besides edges and sites, whose metadata is not used at all).
```

### Comparing `pyslim-1.0.2/docs/tutorial.md` & `pyslim-1.0b1/docs/tutorial.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 # Tutorial
 
 This tutorial covers the most common uses of tree sequences in SLiM/pyslim.
 
 ## Recapitation, simplification, and mutation
 
-Perhaps the most common pyslim operations involve [](sec_tutorial_recapitation),
-[](sec_tutorial_simplification),  and/or [](sec_tutorial_adding_neutral_mutations).
+Perhaps the most common pyslim operations involve {ref}`sec_tutorial_recapitation`,
+{ref}`sec_tutorial_simplification`,  and/or {ref}`sec_tutorial_adding_neutral_mutations`.
 Below we illustrate all three in the context of running a "hybrid" simulation, combining
 both forwards and backwards (coalescent) methods. This hybrid approach is a popular
 application of pyslim because coalescent algorithms, although more limited in the degree
 of biological realism they can attain, can be much faster than the forwards algorithms
 implemented in SLiM.
 
 A typical use-case is to take an existing SLiM simulation and endow
@@ -58,26 +58,26 @@
 
 2. {meth}`simplify() <tskit.TreeSequence.simplify>` : For efficiency, subset the tree
    sequence to only the information relevant for those 1,000 individuals
    we wish to sample.
 
 3. {func}`msprime.sim_mutations` : Add neutral mutations to the tree sequence.
 
+
 These steps are described below. First, to get something to work with,
 you can run this simple SLiM script of a single population of sexual organisms,
 fluctuating around 1000 individuals, for 1000 generations:
 
 ```{literalinclude} example_sim.slim
 ```
 
 You can run this in the shell,
 setting the random seed so you get exactly the same results
 as in the code below:
 ```{code-cell}
-:tags: ["hide-output"]
 %%bash
 slim -s 23 example_sim.slim
 ```
 
 
 (sec_tutorial_recapitation)=
 
@@ -87,15 +87,15 @@
 ```{figure} _static/pedigree_recapitate.png
 ---
 scale: 42%
 align: right
 name: pedigree_recapitate
 ---
 Recapitation adds the green nodes by coalescent simulation.
-(See [the introduction](sec_left_in_tree_sequence)
+(See {ref}`the introduction <sec_left_in_tree_sequence>`
 for a diagram of the previous state.)
 ```
 
 Although we can initialize a SLiM simulation with the results of a coalescent simulation,
 if during the simulation we don't actually use the genotypes for anything, it
 can be much more efficient to do this afterwards, hence only doing a coalescent
 simulation for the portions of the first-generation ancestors that have
@@ -135,15 +135,15 @@
 
 The {func}`.recapitate` method
 is just a thin wrapper around {func}`msprime.sim_ancestry`,
 and you need to set up demography explicitly - for instance, in the example above
 we've simulated from an ancestral population of ``Ne=200`` diploids.
 If you have more than one population,
 you must set migration rates or else coalescence will never happen
-(see [](sec_recapitate_with_migration) for an example,
+(see {ref}`sec_recapitate_with_migration` for an example,
 and {func}`.recapitate` for more).
 
 
 #### Recapitation with a nonuniform recombination map
 
 Above, we recapitated using a uniform genetic map.
 But, msprime - like SLiM - can simulate with recombination drawn from an arbitrary genetic map.
@@ -264,15 +264,15 @@
 
 Probably, your simulations have produced many more fictitious genomes
 than you will be lucky enough to have in real life,
 so at some point you may want to reduce your dataset to a realistic sample size.
 We can get rid of unneeded samples and any extra information from them by using
 an operation called *simplification* (this is the same basic approach that SLiM
 implements under the hood when outputting a tree sequence, as described in
-[the introduction](sec_left_in_tree_sequence)).
+{ref}`the introduction <sec_left_in_tree_sequence>`).
 
 Depicted in the figure at the right is the result of applying an explicit call to
 {meth}`tskit.TreeSequence.simplify` to our example tree sequence.
 In the call we asked to keep only 4
 genomes (contained in 2 of the individuals in the current generation). This has
 substantially simplified the tree sequence, because only information relevant to the
 genealogies of the 4 sample nodes has been kept. (Precisely, simplification retains only
@@ -325,15 +325,15 @@
 
 print(f"Before, there were {rts.num_samples} sample nodes (and {rts.num_individuals} individuals)\n"
       f"in the tree sequence, and now there are {sts.num_samples} sample nodes\n"
       f"(and {sts.num_individuals} individuals).")
 ```
 
 **Note** that you must pass simplify a list of *node IDs*, not individual IDs.
-Here, we used the {func}`.individuals_alive_at` method to obtain the list
+Here, we used the {meth}`.individuals_alive_at` method to obtain the list
 of individuals alive today.
 Also note that there are *still* more than 100 individuals remaining - 15 non-sample individuals
 have not been simplified away,
 because they have nodes that are required to describe the genealogies of the samples.
 (Since this is a non-Wright-Fisher simulation,
 parents and children can be both alive at the same time in the final generation.)
 
@@ -359,19 +359,18 @@
 Continuing with the cartoons from above, these are added to each branch of the tree sequence
 at the rate per unit time that you request.
 We'll add these using the {class}`msprime.SLiMMutationModel`, so that the file can be read back into SLiM,
 but any of the other mutation models in msprime could be used.
 This works as follows:
 
 ```{code-cell}
-next_id = pyslim.next_slim_mutation_id(sts)
 ts = msprime.sim_mutations(
            sts,
            rate=1e-8,
-           model=msprime.SLiMMutationModel(type=0, next_id=next_id),
+           model=msprime.SLiMMutationModel(type=0),
            keep=True,
 )
 
 print(f"The tree sequence now has {ts.num_mutations} mutations,\n"
       f"and mean pairwise nucleotide diversity is {ts.diversity():0.3e}.")
 ```
 
@@ -387,53 +386,14 @@
     and it makes the most sense if we add a type that was unused in the simulation.
     In this example we don't have any existing mutation types, so we can safely use ``type=0``.
 
 3. We also add ``keep = True``, to keep any existing mutations.
     In this example there aren't any, so this isn't strictly necessary,
     but this is a good default.
 
-4. If there are existing SLiM mutations on the tree sequence we need to
-    make sure any newly added mutations have distinct SLiM IDs,
-    so we use :meth:`.next_slim_mutation_id` to figure out
-    what the next available ID is, and pass it in.
-
-
-(sec_output)=
-
-### Writing out genotypes to VCF
-
-Downstream applications often need input in VCF format,
-which we can get with a call to {meth}`tskit.TreeSequence.write_vcf`.
-However, if we do that with this tree sequence, we'll get a malformed VCF,
-with empty strings in the REF column and a strange comma-separated list of integers
-in the ALT column. The reason for this is because we added mutations
-using the `SLiMMutationModel`, and has to do with how SLiM stores enough information
-in the tree sequence to be able to load it back in.
-So, to write out valid VCF with nucleotides for alleles,
-we need to (1) if the SLiM simulation was not a nucleotide model, add nucleotides
-to the SLiM mutations with {func}`generate_nucleotides`,
-and (2) move those nucleotides over into the "ancestral state"
-and "derived state" slots of the tree sequence with {func}`convert_alleles`.
-If all your mutations in SLiM were nucleotide mutations, you only need to do (2).
-And, beware that (2) is an irreversible step: if you write the tree sequence
-produced by {func}`convert_alleles` to a file, you can't load that file into SLiM any more.
-So, to do this we'll do:
-
-```{code-cell}
-nts = pyslim.generate_nucleotides(ts)
-nts = pyslim.convert_alleles(nts)
-sample_indivs = np.unique([ts.node(n).individual for n in nts.samples()])
-with open("example_sim.vcf", "w") as vcffile:
-    nts.write_vcf(vcffile, individuals=sample_indivs[:5])
-```
-
-Here we've just extracted genotypes for the first five individuals;
-see below for what's going on in that code and what you probably
-actually want to do;
-see also {meth}`tskit.TreeSequence.write_vcf` for more options.
 
 
 (sec_extracting_individuals)=
 
 ## Extracting SLiM individuals
 
 Another important thing to be able to do is to extract
@@ -441,15 +401,15 @@
 for analysis or for outputting their genotypes, for instance.
 This section demonstrates some basic manipulations of individuals.
 
 ### Extracting a sample of individuals
 
 The first, most common method to extract individuals is simply to get all
 those that were alive at a particular time,
-using {func}`.individuals_alive_at`. For instance, to get
+using {meth}`.individuals_alive_at`. For instance, to get
 the list of individual IDs of all those alive at the end of the
 simulation (i.e., zero time units ago), we could do:
 
 ```{code-cell}
 orig_ts = tskit.load("example_sim.trees")
 alive = pyslim.individuals_alive_at(orig_ts, 0)
 
@@ -510,15 +470,15 @@
     print ("Error:")
     print (e)
 ```
 
 This is just telling us that some of the individuals we're trying
 to write to the VCF have nodes that are not samples.
 The reference to "missing" is a red herring:
-see [the tskit documentation](tskit:sec_data_model_missing_data)
+see {ref}`the tskit documentation <tskit:sec_data_model_missing_data>`
 for what it's talking about.
 So, instead of writing out genotypes of everyone alive,
 we need to get the list of alive individuals *whose nodes are samples*,
 using {meth}`is_sample() <tskit.Node.is_sample>`:
 
 ```{code-cell}
 indivlist = []
@@ -542,15 +502,14 @@
 but with two populations exchanging migrants:
 
 ```{literalinclude} migrants.slim
 ```
 
 Let's run it:
 ```{code-cell}
-:tags: ["hide-output"]
 %%bash
 slim -s 32 migrants.slim
 ```
 
 To count up how many individuals are in each population,
 we could do:
 
@@ -635,30 +594,30 @@
 ```
 
 
 ## Individual metadata
 
 Each ``Mutation``, ``Population``, ``Node``, and ``Individual``, as well as the tree
 sequence as a whole, carries additional information stored by SLiM in its ``metadata``
-property. A fuller description of metadata in general is given in [](sec_metadata),
+property. A fuller description of metadata in general is given in {ref}`sec_metadata`,
 but as a quick introduction, here is the information available
 about an individual in the previous example:
 
 ```{code-cell}
 :tags: ["remove-output"]
 ind = ts.individual(0)
 ```
 ```{code-cell}
 :tags: ["remove-input"]
 util.pp(ind)
 ```
 
 Some information is generic to individuals in tree sequences of any format:
 ``id`` (the ID internal to the tree sequence),
-``flags`` (described [below](sec_individual_flags)),
+``flags`` (described {ref}`below <sec_individual_flags>`),
 ``location`` (the [x,y,z] coordinates of the individual),
 ``nodes`` (an array of the node IDs that represent the genomes of this individual),
 and ``time`` (the time, in units of "time ago" that the individual was born).
 
 Other information, contained in the ``metadata`` field, is specific to tree sequences
 produced by SLiM. This is described in more detail in the SLiM manual, but briefly:
 
@@ -667,15 +626,15 @@
   were recorded, or at the time
   the simulation stopped if they were still alive  (NB: SLiM uses the word
   "subpopulation" for what is simply called a "population" in tree-sequence parlance)
 - ``sex`` is their sex (as an integer, one of {data}`.INDIVIDUAL_TYPE_FEMALE`,
   {data}`.INDIVIDUAL_TYPE_MALE`, or {data}`.INDIVIDUAL_TYPE_HERMAPHRODITE`).
 - ``flags`` holds additional information about the individual recorded by SLiM
   (currently, only whether the individual has migrated or not:
-  see [](sec_constants_and_flags)).
+  see {ref}`sec_constants_and_flags`).
 
 
 We can use this metadata in many ways, for example, to create an age distribution by sex:
 
 ```{code-cell}
 import numpy as np
 max_age = max([ind.metadata["age"] for ind in ts.individuals()])
@@ -698,22 +657,22 @@
 all individuals would have sex equal to {data}`.INDIVIDUAL_TYPE_HERMAPHRODITE`
 (which is -1).
 
 Several fields associated with individuals are also available as numpy arrays,
 across all individuals at once:
 {attr}`tskit.TreeSequence.individuals_location`,
 {attr}`tskit.TreeSequence.individuals_population`,
-{attr}`tskit.TreeSequence.individuals_time` (also see
-{func}`.individual_ages` and {func}`.individual_ages_at`).
+{attr}`tskit.TreeSequence.individual_times` (also see
+{meth}`.individual_ages` and {meth}`.individual_ages_at`).
 Using these can sometimes be easier than
 iterating over individuals as above. For example,
 suppose that we want to randomly sample 10 individuals alive and older than 2 time steps
 from each of the populations at the end of the simulation,
 and simplify the tree sequence to retain only those individuals.
-This can be done using the numpy arrays returned by {func}`.individual_ages`
+This can be done using the numpy arrays {attr}`pyslim.individual_ages`
 and `.individuals_population` as follows:
 
 ```{code-cell}
 alive = pyslim.individuals_alive_at(ts, 0)
 adults = alive[pyslim.individual_ages(ts)[alive] > 2]
 pops = [
    [i for i in adults if ts.individual(i).metadata['subpopulation'] == k]
@@ -773,16 +732,16 @@
 
 By default, a call to ``treeSeqRememberIndividuals()`` will permanently remember one or
 more individuals, by marking their nodes as actual samples: the simulated equivalent of
 ancient DNA dug out of permafrost, or stored
 in an old collecting tube. This means any tree sequence subsequently recorded will always
 contain this individual, its nodes (now marked as samples), and its full ancestry. As
 with any other sample nodes, any permanently remembered individuals can be removed from
-the tree sequence by [](sec_tutorial_simplification). The result of remembering an
-individual in the [introductory example](sec_left_in_tree_sequence) is pictured on the right.
+the tree sequence by {ref}`sec_tutorial_simplification`. The result of remembering an
+individual in the {ref}`introductory example <sec_left_in_tree_sequence>` is pictured on the right.
 
 
 (sec_retaining_individuals)=
 
 ### Retaining individuals
 
 Alternatively, you may want to avoid treating historical individuals and their genomes as
@@ -790,26 +749,26 @@
 reconstructing the genetic ancestry of the sample nodes. This can save some computational
 burden, as not only will nodes and individuals be removed once they are no longer
 ancestral, but also the full ancestry of the retained individuals does not need to be
 kept. You can retain individuals in this way by using
 ``treeSeqRememberIndividuals(..., permanent=F)``.
 
 Since a retained individual's nodes are not marked as samples, they are subject to the
-[normal removal process](sec_left_in_tree_sequence), and it is possible to end up
+{ref}`normal removal process <sec_left_in_tree_sequence>`, and it is possible to end up
 with an individual containing only one genome, as shown in the diagram. However, as soon
 as *both* nodes of a retained individual have been lost, the individual itself is deleted
 too.
 
 Note that by default, nodes are only kept if they mark a coalescent point (MRCA or branch
 point) in one or more of the trees in a tree sequence. This can be changed by
 initialising tree sequence recording in SLiM using
 ``treeSeqInitialize(retainCoalescentOnly=F)``. SLiM will then
 preserve all retained individuals while they remain in the genealogy, even if their nodes
 are not coalescent points in a tree (so-called "unary nodes"). Similarly, if you later
-decide to reduce the number of samples via [](sec_tutorial_simplification),
+decide to reduce the number of samples via {ref}`sec_tutorial_simplification`,
 retained individuals will be kept only if they are still MRCAs in the ancestry of the
 selected samples. To preserve them even if their nodes are not coalescent points, you
 can specify ``ts.simplify(selected_samples, keep_unary_in_individuals=True)``.
 
 :::{todo}
 Add SLiM code which includes retaining and remembering, and perhaps some python code
 to show them.
@@ -862,17 +821,17 @@
 
 for k in indiv_types:
   print(f"Number of individuals that are {k}: {indiv_types[k]}")
 ```
 
 :::{note}
 In previous versions of SLiM/pyslim, the first generation of individuals were
-kept in the tree sequence, to allow [](sec_tutorial_recapitation). With the
+kept in the tree sequence, to allow {ref}`sec_tutorial_recapitation`. With the
 addition of the ``keep_input_roots=True`` option to the
-[](sec_tutorial_simplification) process, this is no longer necessary,
+{ref}`sec_tutorial_simplification` process, this is no longer necessary,
 so these are no longer present, unless you specifically Remember them.
 :::
 
 
 ## Generating intial diversity with msprime
 
 Suppose now that we'd like to *start* a SLiM simulation
@@ -919,19 +878,19 @@
 :tags: ["remove-input"]
 util.pp(ind)
 ```
 Looking at the ``metadata`` above, we see the default values are ``age=0``
 hermaphrodites (``sex=-1``), for instance.
 
 Now let's add SLiM mutations.
-These will be neutral, as {func}`msprime.sim_mutations`
+These will be neutral, as {func}`msprime.sim_mutation`
 doesn't have the ability to dynamically modify the selection coefficients
 stored in the mutation metadata.
 To modify the mutations to be under selection,
-see [](sec_vignette_coalescent_diversity).
+see {ref}`sec_vignette_coalescent_diversity`.
 ```{code-cell}
 ts = msprime.sim_mutations(
                 ts, rate=1e-8,
                 model=msprime.SLiMMutationModel(type=0),
                 random_seed=9
 )
 ```
@@ -954,33 +913,31 @@
 Here's a minimal SLiM script that reads in the tree sequence file
 and runs it for a bit longer.
 
 ```{literalinclude} neutral_restart.slim
 ```
 
 ```{code-cell}
-:tags: ["hide-output"]
 %%bash
 slim -s 123 neutral_restart.slim
 ```
 
-A more in-depth example is provided at [](sec_vignette_coalescent_diversity).
+A more in-depth example is provided at {ref}`sec_vignette_coalescent_diversity`.
 See the SLiM manual for more about this operation.
 
 
 ## Extracting information about selected mutations
 
 Here is a simple SLiM simulation with two types of mutation:
 `m1` are deleterious, and `m2` are beneficial.
 Let's see how to extract information about these mutations.
 
 ```{literalinclude} selection.slim
 ```
 ```{code-cell}
-:tags: ["hide-output"]
 %%bash
 slim -s 23 selection.slim
 ```
 
 First, let's see how many mutations there are:
 
 ```{code-cell}
@@ -1185,15 +1142,15 @@
 
 ## Possibly important technical notes
 
 Also known as "gotchas".
 
 1. If you use msprime to simulate a tree sequence, and then use that to initialize a SLiM simulation,
     you have to specify the same sequence length in both: as in the examples above,
-    the ``sequence_length`` argument to {func}`msprime.sim_ancestry` should be equal to the SLiM sequence length
+    the ``sequence_length`` argument to {meth}`msprime.sim_ancestry` should be equal to the SLiM sequence length
     *plus 1.0* (e.g., if the base positions in SLiM are 0 to 99, then there are 100 bases in all,
     so the sequence length should be 100).
 
 2. Make sure to distinguish *individuals* and *nodes*!
    ``tskit`` "nodes" correspond to SLiM "genomes".
    Individuals in SLiM are diploid, so normally, each has two nodes (but retained
    individuals may have nodes removed by simplification: see below).
```

### Comparing `pyslim-1.0.2/docs/util.py` & `pyslim-1.0b1/docs/util.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/vignette_coalescent_diversity.md` & `pyslim-1.0b1/docs/vignette_coalescent_diversity.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,16 @@
 import pyslim, tskit, msprime
 from IPython.display import SVG
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 
 import util
-```
 
-```{eval-rst}
-.. currentmodule:: pyslim
+np.random.seed(1234)
 ```
 
 (sec_vignette_coalescent_diversity)=
 
 # Vignette: Starting with diversity generated by coalescent simulation
 
 This vignette shows how to simulate history with msprime,
@@ -114,21 +112,21 @@
 At this point, we have genealogical information: individuals,
 nodes (chromosomes), and relationships between them,
 but no genetic diversity; no mutations.
 First, we'll add SLiM metadata to all of these things,
 a procedure we call "annotating".
 
 ```{code-cell}
-ots = pyslim.annotate(ots, model_type="WF", tick=1, stage="late")
+ots = pyslim.annotate(ots, model_type="WF", tick=1)
 ```
 
 This method adds default metadata to everything that needs it:
 in this case, all individuals, all nodes that are part of alive individuals,
 and all populations referenced by nodes.
-These default values are returned by {func}`.slim_default_metadata`
+These default values are returned by {meth}`.slim_default_metadata`
 (e.g., all individuals are hermaphrodite, all chromosomes are autosomal);
 see {func}`.annotate` for more information.
 
 ## Add SLiM mutations
 
 Next, we're going to use the {class}`msprime.SLiMMutationModel` to add mutations
 to the tree sequence. These will carry SLiM metadata, but this metadata
@@ -188,25 +186,24 @@
 as a comma-separated list of integers in the derived state of the mutation.
 So, in case some SLiM mutations appear in more than one mutation
 in the tree sequence, we will build a map from SLiM ID to selection coefficient:
 ``mut_map[k]`` will give the selection coefficient of the SLiM mutation with
 SLiM mutation ID ``k``.
 
 ```{code-cell}
-rng = np.random.default_rng(seed=1234)
 tables = ots.tables
 tables.mutations.clear()
 mut_map = {}
 for m in ots.mutations():
   md_list = m.metadata["mutation_list"]
   slim_ids = m.derived_state.split(",")
   assert len(slim_ids) == len(md_list)
   for sid, md in zip(slim_ids, md_list):
      if sid not in mut_map:
-        mut_map[sid] = rng.exponential(scale=0.04)
+        mut_map[sid] = np.random.exponential(scale=0.04)
      md["selection_coeff"] = mut_map[sid]
   _ = tables.mutations.append(
           m.replace(metadata={"mutation_list": md_list})
   )
 
 # check we didn't mess anything up
 assert tables.mutations.num_rows == ots.num_mutations
@@ -311,15 +308,17 @@
 A simple thing to look at next is: how did the selected mutations
 change in frequency? We can do this thanks to our having
 Remembered the first generation.
 First, we'll compute all allele frequencies
 among both the first generation and the final generation:
 
 ```{code-cell}
-times = list(set(ts.individuals_time))
+# TODO: will work on next tskit release
+# times = list(set(ts.individual_times))
+times = [ts.node(ind.nodes[0]).time for ind in ts.individuals()]
 times.sort()
 print("The times ago at which individuals in the tree sequence were born:", times)
 # The times ago at which individuals in the tree sequence were born: [0.0, 100.0]
 nodes_by_time = [ts.samples(time=t) for t in times]
 
 num_nodes = np.array([len(x) for x in nodes_by_time])
 p = ts.sample_count_stat(nodes_by_time, lambda x: x/num_nodes, 2, windows='sites',
@@ -399,15 +398,15 @@
 And, importantly, we've added ``keep=True`` so that existing mutations
 are not discarded.
 
 ```{code-cell}
 neutral_mut_map = msprime.RateMap(
            position=breaks,
            rate=[2.97e-8, 2.997e-8, 2.97e-8])
-next_id = pyslim.next_slim_mutation_id(ts)
+next_id = max([max(map(int, m.derived_state.split(","))) for m in ts.mutations()])
 neutral_mut_model = msprime.SLiMMutationModel(
                                 type=1,
                                 next_id=next_id)
 mts = msprime.sim_mutations(
                 ts,
                 rate=neutral_mut_map,
                 model=neutral_mut_model,
```

### Comparing `pyslim-1.0.2/docs/vignette_continuing.md` & `pyslim-1.0b1/docs/vignette_continuing.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,17 @@
 mut_types = set([md['mutation_type']
                 for mut in ts.mutations()
                 for md in mut.metadata['mutation_list']])
 print(f"Keeping {rts.num_mutations} existing mutations of type(s) {mut_types}.")
 assert 0 not in mut_types
 
 # add type m0 mutations
-next_id = pyslim.next_slim_mutation_id(rts)
 rts = msprime.sim_mutations(
             rts, rate=1e-8, random_seed=7, keep=True,
-            model=msprime.SLiMMutationModel(type=0, next_id=next_id)
+            model=msprime.SLiMMutationModel(type=0)
 )
 
 p = rts.sample_count_stat(
                 [rts.samples()], lambda x: x/20000, 1, windows='sites',
                 span_normalise=False, polarised=True, strict=False)
 print(f"After mutation, there are {rts.num_sites} segregating sites, of which {np.sum(p > 0.25)}")
 print(f"are at frequency above 25%, and {np.sum(p > 0.05)} are above 5%.")
```

### Comparing `pyslim-1.0.2/docs/vignette_parallel_phylo.md` & `pyslim-1.0b1/docs/vignette_parallel_phylo.md`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/docs/vignette_space.md` & `pyslim-1.0b1/docs/vignette_space.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,17 @@
 which requires 37,095 distinct trees along the genome.
 Individuals are diploid, which explains why the number of individuals
 is equal to half the number of samples.
 Let's have a look at how old those individuals are,
 by tabulating when they were born:
 
 ```{code-cell}
-individual_times = slim_ts.individuals_time
+# TODO: will work on next tskit release
+# individual_times = slim_ts.individual_times
+individual_times = np.array([slim_ts.node(ind.nodes[0]).time for ind in slim_ts.individuals()])
 for t in np.unique(individual_times):
     print(f"There are {np.sum(individual_times == t)} individuals from time {t}.")
 ```
 
 These "times" record the birth times of each individual.
 These are *tskit* times, which are in units of "time ago",
 so for instance, there are 343 individuals born one time unit before the end of the simulation
@@ -147,15 +149,15 @@
          keep=True,
 )
 ts.dump("spatial_sim.recap.trees")
 
 print(f"The tree sequence now has {ts.num_trees} trees,\n"
        " and {ts.num_mutations} mutations.")
 ```
-See [](sec_tutorial_adding_neutral_mutations) for discussion of the options to
+See {ref}`sec_tutorial_adding_neutral_mutations` for discussion of the options to
 {func}`msprime.sim_mutations`.
 
 
 We will have no further use for ``slim_ts`` or for ``recap_ts``;
 we've just given them separate names for tidyness.
 And, since the original SLiM mutation had no mutations, we didn't need to specify ``keep=True``
 in {func}`sim_mutations <msprime.sim_mutations>`, but if we *had* put down selected mutations with SLiM
@@ -176,15 +178,17 @@
 2. Five individuals sampled randomly from everyone alive 1000 time steps ago.
 
 ```{code-cell}
 
 np.random.seed(23)
 
 alive = pyslim.individuals_alive_at(ts, 0)
-locs = ts.individuals_location[alive, :]
+# TODO: will work in the next tskit release
+# locs = ts.individual_locations[alive, :]
+locs = np.array([ts.individual(ind).location for ind in alive])
 
 W = 35
 w = 5
 groups = {
   'topleft' : alive[np.logical_and(locs[:, 0] < w, locs[:, 1] < w)],
   'topright' : alive[np.logical_and(locs[:, 0] < w, locs[:, 1] > W - w)],
   'bottomleft' : alive[np.logical_and(locs[:, 0] > W - w, locs[:, 1] < w)],
@@ -219,23 +223,25 @@
 
 ## Plotting locations
 
 We should check this: plot where these individuals lie
 relative to everyone else.
 The individuals locations are available as a property of individuals,
 but to make things easier, it's also present in a `num_individuals x 3`
-numpy array as ``ts.individuals_location``.
+numpy array as ``ts.individual_locations``.
 (There are three columns because SLiM allows for
 `(x, y, z)` coordinates, but we'll just use the first two.)
 Since ``groups["topleft"]`` is an array of individual IDs,
 we can pull out the locations of the "topleft" individuals
 by indexing the rows of the individual location array:
 ```{code-cell}
 print("Locations:")
-all_locs = ts.individuals_location
+# TODO: will work in next tskit release
+# all_locs = ts.individual_locations
+all_locs = np.array([ind.location for ind in ts.individuals()])
 print(all_locs)
 print("shape:")
 all_locs.shape
 print("topleft locations shape:")
 all_locs[groups["topleft"], :].shape
 ```
 
@@ -249,15 +255,17 @@
 import matplotlib.pyplot as plt
 
 group_order = ['topleft', 'topright', 'bottomleft', 'bottomright', 'center', 'ancient']
 ind_colors = np.repeat(0, ts.num_individuals)
 for j, k in enumerate(group_order):
   ind_colors[groups[k]] = 1 + j
 
-old_locs = ts.individuals_location[old_ones, :]
+# TODO: will work in next tskit release
+# old_locs = ts.individual_locations[old_ones, :]
+old_locs = np.array([ind.location for ind in ts.individuals()])[old_ones, :]
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12, 6), dpi=300)
 ax1.set_title("today")
 ax1.scatter(locs[:,0], locs[:,1], s=20, c=ind_colors[alive])
 ax2.set_title("long ago")
 ax2.scatter(old_locs[:, 0], old_locs[:, 1], s=20, c=ind_colors[old_ones]);
 ```
@@ -350,15 +358,17 @@
 
 Here we've only computed divergences in the *upper triangle* of the pairwise divergence matrix,
 with heterozygosities on the diagonal.
 We'll also need pairwise geographic distances:
 
 ```{code-cell}
 geog_dist = np.repeat(0.0, len(pairs))
-locs = ts.individuals_location
+# TODO: will work in next tskit release
+# locs = ts.individual_locations
+locs = np.array([ind.location for ind in ts.individuals()])
 for k, (i, j) in enumerate(pairs):
   geog_dist[k] = np.sqrt(np.sum(
                     (locs[ind_ids[i], :]
                      - locs[ind_ids[j], :])**2
                  ))
 ```
 
@@ -427,19 +437,19 @@
 
 
 ## More information
 
 1. The distinction between "nodes" (i.e., genomes) and "individuals" can be confusing,
    as well as the idea of "samples".
    Please see the
-   [tskit documentation](tskit:sec_data_model)
+   {ref}`tskit documentation <tskit:sec_data_model>`
    for more explanation about these concepts.
 
 2. The general interface for computing statistics (explaining, for instance, the "indexes"
-   argument above) is described in [tskit documentation](tskit:sec_stats) also.
+   argument above) is described in {ref}`tskit documentation <tskit:sec_stats>` also.
 
 
 ## What about simplification?
 
 The tree sequence we worked with here contains more information than we need,
 including the first generation individuals.
 If we wanted to remove this, we could have used the
```

### Comparing `pyslim-1.0.2/docs/vignette_space.slim` & `pyslim-1.0b1/docs/vignette_space.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/pyslim/methods.py` & `pyslim-1.0b1/pyslim/methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import numpy as np
 
 from .slim_tree_sequence import *
 from .slim_metadata import *
 from .provenance import *
 from .util import *
 
-
 def recapitate(ts,
                ancestral_Ne=None,
                **kwargs
     ):
     '''
     Returns a "recapitated" tree sequence, by using msprime to run a
     coalescent simulation from the "top" of this tree sequence, i.e.,
@@ -35,50 +34,24 @@
     argument: see :func:`msprime.sim_ancestry`.
     
     In general, all defaults are whatever the defaults of
     {meth}`msprime.sim_ancestry` are; this includes recombination rate, so
     that if neither ``recombination_rate`` or a ``recombination_map`` are
     provided, there will be *no* recombination.
 
-    :param tskit.TreeSequence ts: The tree sequence to transform.
+    :param TreeSequence ts: The tree sequence to transform.
     :param float ancestral_Ne: If specified, then will simulate from a single
         ancestral population of this size. It is an error to specify this
         as well as ``demography``.
     :param dict kwargs: Any other arguments to :func:`msprime.sim_ancestry`.
     '''
     is_current_version(ts, _warn=True)
     if ancestral_Ne is not None:
         if "demography" in kwargs:
             raise ValueError("You cannot specify both `demography` and `ancestral_Ne`.")
-        recap_time = ts.metadata['SLiM']['tick']
-        # In various circumstances depending on the stage in which the simulation was
-        # started and when the tree sequence was written out, the time of the roots
-        # might be one or even two less than the "tick" value. We have access
-        # to the stage the tree sequence was written out, but not the time it
-        # was *started*. So, we'll just check if we need to subtract one or two.
-        # Consistency checking this requires looping over all the trees, unfortunately,
-        # but it avoids some common errors.
-        root_times = list(set([ts.node(n).time for t in ts.trees() for n in t.roots]))
-        for adj in (1, 2):
-            if np.allclose(root_times, recap_time - adj):
-                recap_time -= adj
-        if len(root_times) > 1 or not np.allclose(root_times, recap_time):
-            message = (
-                "Not all roots of the provided tree sequence are at the time expected "
-                "by recapitate(). This could happen if you've simplified in "
-                "python before recapitating (fix: don't simplify first). "
-                "If could also happen in other situations, e.g., "
-                "you added new individuals without parents in SLiM "
-                "during the course of the simulation with sim.addSubPop(), "
-                "in which case you will probably need to recapitate with "
-                "msprime.sim_ancestry(initial_state=ts, ...). "
-                f"(Expected root time: {recap_time}; "
-                f"Observed root times: {root_times})"
-            )
-            raise ValueError(message)
         demography = msprime.Demography.from_tree_sequence(ts)
         # must set pop sizes to >0 even though we merge immediately
         for pop in demography.populations:
             pop.initial_size=1.0
         ancestral_name = "ancestral"
         derived_names = [pop.name for pop in demography.populations]
         while ancestral_name in derived_names:
@@ -129,29 +102,27 @@
         with open('nucs.vcf', 'w') as f:
             nts.write_vcf(f)
 
     This method will produce an error if the tree sequence does not have a
     valid reference sequence or if any mutations do not have nucleotides: to first
     generate these, see :func:`.generate_nucleotides`.
 
-    :param tskit.TreeSequence ts: The tree sequence to transform.
+    :param TreeSequence ts: The tree sequence to transform.
     """
     tables = ts.dump_tables()
     has_refseq = (
             ts.has_reference_sequence()
             and len(ts.reference_sequence.data) > 0
     )
-    if not has_refseq:
-        raise ValueError("Tree sequence must have a valid reference sequence.")
     # unfortunately, nucleotide mutations may be stacked (e.g., substitutions
     # will appear this way) and they don't appear in any particular order;
     # so we must guess which is the most recent, by choosing the one that
     # has the largest SLiM time, doesn't appear in the parent list, or has
     # the lagest SLiM ID.
-    nuc_inds = tables.mutations.metadata_vector(['mutation_list', 0, 'nucleotide'], dtype='int')
+    slim_muts = np.repeat(0, ts.num_mutations)
     num_stacked = np.array([len(m.metadata['mutation_list']) for m in ts.mutations()])
     for k in np.where(num_stacked > 1)[0]:
         mut = ts.mutation(k)
         if mut.parent == tskit.NULL:
             pids = []
         else:
             pids = ts.mutation(mut.parent).derived_state.split(",")
@@ -163,36 +134,41 @@
                 j
             ) for j, (i, md) in
             enumerate(
                 zip(mut.derived_state.split(","), mut.metadata['mutation_list'])
             )
         ]
         x.sort()
-        j = x[-1][3]
-        nuc_inds[k] = mut.metadata['mutation_list'][j]['nucleotide']
+        slim_muts[k] = x[-1][3]
+    # gah that was terrible, ok back to it
+    nuc_inds = np.array(
+            [m.metadata['mutation_list'][0]['nucleotide']
+                for k, m in zip(slim_muts, ts.mutations())],
+            dtype='int',
+    )
     if np.any(nuc_inds == -1):
         raise ValueError("All mutations must be nucleotide mutations.")
+    if not has_refseq:
+        raise ValueError("Tree sequence must have a valid reference sequence.")
+    aa = [ts.reference_sequence.data[k] for k in tables.sites.position.astype('int')]
     da = np.array(NUCLEOTIDES)[nuc_inds]
+    tables.sites.packset_ancestral_state(aa)
     tables.mutations.packset_derived_state(da)
-    k = tables.sites.position.astype('int')
-    aa = np.frombuffer(ts.reference_sequence.data.encode('utf-8'), dtype='S1')[k]
-    tables.sites.packset_ancestral_state(aa.tobytes().decode('utf-8'))
 
     return tables.tree_sequence()
 
 
 def generate_nucleotides(ts, reference_sequence=None, keep=True, seed=None):
     """
     Returns a modified tree sequence in which mutations have been randomly assigned nucleotides
     and (optionally) a reference sequence has been randomly generated.
 
     If ``reference_sequence`` is a string of nucleotides (A, C, G, and T) of
     length equal to the sequence length, this is used for the reference
-    sequence. If no reference sequence is given, the reference_sequence property
-    of ts is used if present; if not then a sequence of independent and
+    sequence. Otherwise (the default), a reference sequence of independent and
     uniformly random nucleotides is generated.
 
     SLiM stores the nucleotide as an integer in the mutation metadata, with -1 meaning "not
     a nucleotide mutation". This method assigns nucleotides by stepping through
     each mutation and picking a random nucleotide uniformly out of the three
     possible nucleotides that differ from the parental state (i.e., the derived
     state of the parental mutation, or the ancestral state if the mutation has
@@ -201,47 +177,39 @@
 
     Technical note: in the case of stacked mutations, the SLiM mutation that
     determines the nucleotide state of the (tskit) mutation is the one with the largest
     slim_time attribute. This method tries to assign nucleotides so that each mutation
     differs from the previous state, but this is not always possible in certain
     unlikely cases.
 
-    :param tskit.TreeSequence ts: The tree sequence to transform.
-    :param bool reference_sequence: A reference sequence, or None to use an existing reference,
-        or to randomly generate one.
+    :param TreeSequence ts: The tree sequence to transform.
+    :param bool reference_sequence: A reference sequence, or None to randomly generate one.
     :param bool keep: Whether to leave existing nucleotides in mutations that already have one.
     :param int seed: The random seed for generating new alleles.
     """
     rng = np.random.default_rng(seed=seed)
     if reference_sequence is None:
-        if not ts.has_reference_sequence():
-            reference_sequence = rng.choice(
-                    np.array([65, 67, 71, 84], dtype=np.int8),
-                    int(ts.sequence_length),
-                    replace=True,
-            ).tobytes().decode('ascii')
-    else:
-        if len(reference_sequence) != ts.sequence_length:
-            raise ValueError("Reference sequence must have length equal to sequence_length.")
-        if len([x for x in reference_sequence if x not in NUCLEOTIDES]) > 0:
-            raise ValueError("Reference sequence must be a string of A, C, G, and T only.")
+        reference_sequence = rng.choice(
+                np.array([65, 67, 71, 84], dtype=np.int8),
+                int(ts.sequence_length),
+                replace=True,
+        ).tobytes().decode('ascii')
+
+    if len(reference_sequence) != ts.sequence_length:
+        raise ValueError("Reference sequence must have length equal to sequence_length.")
+    if len([x for x in reference_sequence if x not in NUCLEOTIDES]) > 0:
+        raise ValueError("Reference sequence must be a string of A, C, G, and T only.")
 
     tables = ts.dump_tables()
-    if reference_sequence is not None:
-        tables.reference_sequence.data = reference_sequence
+    tables.reference_sequence.data = reference_sequence
     tables.mutations.clear()
     sets = [[k for k in range(4) if k != i] for i in range(4)]
     states = np.full((ts.num_mutations,), -1)
-    k = tables.sites.position.astype('int')
-    aa_list = np.searchsorted(
-            NUCLEOTIDES,
-            np.frombuffer(tables.reference_sequence.data.encode('utf-8'), dtype='S1')[k],
-    )
     for site in ts.sites():
-        aa = aa_list[site.id]
+        aa = NUCLEOTIDES.index(reference_sequence[int(site.position)])
         muts = {}
         for mut in site.mutations:
             if mut.parent == tskit.NULL:
                 pa = aa
                 pds = []
             else:
                 pa = states[mut.parent]
@@ -271,135 +239,177 @@
 
 
 def individual_ages(ts):
     """
     Returns the ages of all individuals in the tree sequence, extracted
     from metadata. The result is a array of length equal to the number of
     individuals, with k-th entry equal to ``ts.individual(k).metadata["age"]``.
-
-    :return: An array of ages of individuals.
     """
     if ts.metadata['SLiM']['model_type'] != "WF":
         ages = ts.tables.individuals.metadata_vector("age")
     else:
         ages = np.zeros(ts.num_individuals, dtype='int')
     return ages
 
 
+def individual_locations(ts):
+    """
+    Returns the ages of all individuals in the tree sequence, extracted
+    from metadata. The result is a array of length equal to the number of
+    individuals, with k-th entry equal to ``ts.individual(k).metadata["age"]``.
+    """
+    x = ts.tables.individuals.location
+    x.shape = (ts.num_individuals, 3)
+    return x
+
+
+def individual_times(ts):
+    """
+    TODO: implement in tskit
+    """
+    nodes = ts.tables.nodes
+    if not np.all(unique_labels_by_group(nodes.individual,
+                                         nodes.time)):
+        raise ValueError("Individual has nodes from more than one time.")
+    individual_times = np.zeros(ts.num_individuals)
+    has_indiv = (nodes.individual >= 0)
+    which_indiv = nodes.individual[has_indiv]
+    # if we did not do the sanity check above then an individual with nodes
+    # with more than one time would get the time of their last node in the list
+    individual_times[which_indiv] = nodes.time[has_indiv]
+    return individual_times
+
+
+def individual_populations(ts):
+    """
+    TODO: implement in tskit
+    """
+    nodes = ts.tables.nodes
+    if not np.all(unique_labels_by_group(nodes.individual,
+                                         nodes.population)):
+        raise ValueError("Individual has nodes from more than one population.")
+    individual_populations = np.repeat(np.int32(-1), ts.num_individuals)
+    has_indiv = (nodes.individual >= 0)
+    which_indiv = nodes.individual[has_indiv]
+    # if we did not do the sanity check above then an individual with nodes in
+    # more than one pop would get the pop of their last node in the list
+    individual_populations[which_indiv] = nodes.population[has_indiv]
+    return individual_populations
+
+
 def individuals_alive_at(ts, time, stage='late', remembered_stage=None,
                          population=None, samples_only=False):
     """
     Returns an array giving the IDs of all individuals that are known to be
     alive at the given time ago.  This is determined using their birth time
     ago (given by their `time` attribute) and, for nonWF models,
     their `age` attribute (which is equal to their age at the last time
-    they were Remembered). See also {func}`.individual_ages_at`.
+    they were Remembered). See also :meth:`.individual_ages_at`.
 
     In WF models, birth occurs after "early()", so that individuals are only
     alive during "late()" for the time step when they have age zero,
     while in nonWF models, birth occurs before "early()", so they are alive
     for both stages.
     
     In both WF and nonWF models, mortality occurs between
     "early()" and "late()", so that individuals are last alive during the
     "early()" stage of the time step of their final age, and if individuals
-    are alive during "late()" they will also be alive during "first()" and
-    "early()" of the next time step. This means it is important to know during
-    which stage individuals were Remembered - for instance, if the call to
+    are alive during "late()" they will also be alive during "early()" of the
+    next time step. This means it is important to know during which stage
+    individuals were Remembered - for instance, if the call to
     sim.treeSeqRememberIndividuals() was made during "early()" of a given time step,
     then those individuals might not have survived until "late()" of that
     time step. Since SLiM does not record the stage at which individuals
     were Remembered, you can specify this by setting ``remembered_stages``:
     it should be the stage during which *all* calls to
     ``sim.treeSeqRememberIndividuals()``,  as well as to ``sim.treeSeqOutput()``,
     were made.
 
-    Note also that in nonWF models, birth occurs between "first()" and
-    "early()", so the possible parents in a given time step are those that are
-    alive in "early()" and have age greater than zero, or, equivalently, are
-    alive in "late()" during the previous time step.
+    Note also that in nonWF models, birth occurs before "early()", so the
+    possible parents in a given time step are those that are alive in
+    "early()" and have age greater than zero, or, equivalently, are alive in
+    "late()" during the previous time step.
     In WF models, birth occurs after "early()", so possible parents in a
     given time step are those that are alive during "early()" of that time
     step or are alive during "late()" of the previous time step.
 
-    Since individuals may be created not during the usual 'birth' stage
-    by `addSubPop( )`, and the stage at which they are created is not stored,
-    results may be unreliable for the first-generation individuals.
-
-    :param tskit.TreeSequence ts: A tree sequence.
-    :param float time: The number of ticks (i.e., time steps) ago.
+    :param TreeSequence ts: A tree sequence.
+    :param float time: The number of time steps ago.
     :param str stage: The stage in the SLiM life cycle that we are inquiring
-        about (either "first", "early" or "late"; defaults to "late").
+        about (either "early" or "late"; defaults to "late").
     :param str remembered_stage: The stage in the SLiM life cycle
         during which individuals were Remembered (defaults to the stage the
         tree sequence was recorded at, stored in metadata).
     :param int population: If given, return only individuals in the
         population(s) with these population ID(s).
     :param bool samples_only: Whether to return only individuals who have at
         least one node marked as samples.
     """
     is_current_version(ts, _warn=True)
-    if stage not in ("late", "early", "first"):
+    if stage not in ("late", "early"):
         raise ValueError(f"Unknown stage '{stage}': "
-                          "should be either 'first', 'early' or 'late'.")
+                          "should be either 'early' or 'late'.")
 
     if remembered_stage is None:
         remembered_stage = ts.metadata['SLiM']['stage']
 
-    if remembered_stage not in ("late", "early", "first"):
+    if remembered_stage not in ("late", "early"):
         raise ValueError(f"Unknown remembered_stage '{remembered_stage}': "
-                          "should be either 'first', 'early' or 'late'.")
+                          "should be either 'early' or 'late'.")
     if remembered_stage != ts.metadata['SLiM']['stage']:
         warnings.warn(f"Provided remembered_stage '{remembered_stage}' does not"
                       " match the stage at which the tree sequence was saved"
                       f" ('{ts.metadata['SLiM']['stage']}'). This is not necessarily"
                       " an error, but mismatched stages will lead to inconsistencies:"
                       " make sure you know what you're doing.")
 
-    # An individual's tskit time is the tskit counter at the time of their birth.
-    # The tskit counter clicks once at the start of each reproduction bout.
-    # In a WF model, individuals are alive for all stages with the same value
-    # of the tskit counter. In a nonWF model, an individual of age `a` will be
-    # alive for `a + 1` 'early' events, and `a` 'late' and 'first' events,
-    # starting with the one having the same value of the tskit counter.
-    # Also note that if remembered_stage is 'late', then they are recorded
-    # before their age counter clicks, so they will actually have age one greater.
-    # Since `time` is in "number of time steps ago",
-    # we are inquiring about SLiM tick `n - time`, where `n` is
-    # the value of `ts.metadata["SLiM"]["tick"]`. To convert this along with
-    # our stage information into a tskit time `t`,
-    # let x = 1 if the stage is 'first' or (is 'early' and WF)
-    # and y = 1 if remembered stage is 'late' or (is 'early' and nonWF);
-    # then t = time + x + y - 1 .
-    is_wf = (ts.metadata['SLiM']['model_type'] == "WF")
-    x = (stage == "first" or (stage == "early" and is_wf))
-    y = (remembered_stage == "late" or (remembered_stage == "early" and not is_wf))
-    t = time + x + y - 1
-    birth_times = ts.individuals_time
+    # birth_time is the time ago that they were first alive in 'late'
+    # in a nonWF model they are alive for the same time step's 'early'
+    # but in a WF model the first 'early' they were alive for is one more recent
+    birth_times = individual_times(ts)
+    # birth_times - birth_offset is the first time ago they were alive
+    # during stage 'stage'
+    if stage == "early" and ts.metadata['SLiM']['model_type'] == "WF":
+        birth_offset = 1
+    else:
+        birth_offset = 0
+    # ages is the number of complete life cycles they are known to have lived through,
+    # and so individuals have lived through at least 'age + 1' of both stages.
+    # In nonWF models, they live for one more 'early' than 'late',
+    # but this is only reflected in their age if Remembered in 'early'.
     ages = individual_ages(ts)
-    if is_wf:
-        alive_bool = (birth_times == t)
+    # ages + age_offset + 1 is the number of 'stage' stages they are known
+    # to have lived through
+    if (ts.metadata['SLiM']['model_type'] == "WF"
+            or stage == remembered_stage):
+        age_offset = 0
     else:
-        age_offset = (stage == "early") + (remembered_stage == "late")
-        alive_bool = np.logical_and(
-                birth_times >= t,
-                birth_times - ages < t + age_offset
-        )
+        if (remembered_stage == "early"
+                and stage == "late"):
+            age_offset = -1
+        else:
+            age_offset = 1
+    # if adjusted age=0 then they are be alive at exactly one time step
+    alive_bool = np.logical_and(
+            birth_times >= time + birth_offset,
+            birth_times - ages <= time + birth_offset + age_offset)
+
     if population is not None:
         alive_bool &= np.isin(
-                ts.individuals_population,
+                individual_populations(ts),
                 population
         )
     if samples_only:
         nodes = ts.tables.nodes
         alive_bool &= (
                 0 < np.bincount(1 + nodes.individual,
                                 nodes.flags & tskit.NODE_IS_SAMPLE,
                                 minlength=1 + ts.num_individuals)[1:]
         )
+
     return np.where(alive_bool)[0]
 
 
 def individual_ages_at(ts, time, stage="late", remembered_stage="late"):
     """
     Returns the `ages` of each individual at the corresponding time ago,
     which will be ``nan`` if the individual is either not born yet or dead.
@@ -411,76 +421,72 @@
 
     Since age increments at the end of each time step,
     the age is the number of time steps ends the individual has lived
     through, so if they were born in time step `time`, then their age
     will be zero.
 
     In a WF model, this method does not provide any more information than
-    does {func}`.individuals_alive_at`, but for consistency, non-nan ages
-    will be 0 in "late" and 1 in "first" and "early".
-    See {func}`.individuals_alive_at` for further discussion.
+    does :meth:`.individuals_alive_at`, but for consistency, non-nan ages
+    will be 0 in "late" and 1 in "early".
+    See :meth:`.individuals_alive_at` for further discussion.
 
-    :param tskit.TreeSequence ts: A tree sequence.
+    :param TreeSequence ts: A tree sequence.
     :param float time: The reference time ago.
     :param str stage: The stage in the SLiM life cycle used to determine who
         is alive (either "early" or "late"; defaults to "late").
     :param str remembered_stage: The stage in the SLiM life cycle during which
         individuals were Remembered.
     """
     ages = np.repeat(np.nan, ts.num_individuals)
     alive = individuals_alive_at(
             ts,
             time,
             stage=stage,
             remembered_stage=remembered_stage
     )
-    # to convert individuals_time to number of ticks ago we subtract (y - 1), so
-    is_wf = (ts.metadata['SLiM']['model_type'] == "WF")
-    y = (remembered_stage == "late" or (remembered_stage == "early" and not is_wf))
-    t = time + y - 1
-    ages[alive] = ts.individuals_time[alive] - t
+    ages[alive] = individual_times(ts)[alive] - time
     return ages
 
 
 def slim_time(ts, time, stage="late"):
     """
     Converts the given "tskit times" (i.e., in units of time before the end
     of the simulation) to SLiM times (those recorded by SLiM, usually in units
     of ticks since the start of the simulation). Although the latter are
     always integers, these will not be if the provided times are not integers.
 
     When the tree sequence is written out, SLiM records the current
     current tick in the metadata:
-    ``ts.metadata['SLiM']['tick']``. In most cases, the "SLiM time"
+    ``ts.metadata['SLiM']['tick']``. In most cases, the “SLiM time”
     referred to by a time ago in the tree sequence (i.e., the value that would
     be reported by community.tick within SLiM at the point in time thus
     referenced) can be obtained by subtracting that time ago from
     ``ts.metadata['SLiM']['tick']``. However, in WF models, birth
     happens between the “early()” and “late()” stages, so if the tree
     sequence was written out using sim.treeSeqOutput() during “early()” in
     a WF model, the tree sequence’s times measure time before the last set
     of individuals are born, i.e., before SLiM time step
-    ``ts.metadata['SLiM']['tick'] - 1``. The same thing applies to
-    the "first" stage for both WF and nonWF models.
+    ``ts.metadata['SLiM']['tick'] - 1``.
 
     In some situations (e.g., mutations added during early() in WF models)
     this may not return what you expect. See :ref:`sec_metadata_converting_times`
     for more discussion.
 
-    :param tskit.TreeSequence ts: A SLiM-compatible TreeSequence.
-    :param numpy.ndarray time: An array of times to be converted.
-    :param str stage: The stage of the SLiM life cycle that the SLiM time
+    :param TreeSequence ts: A SLiM-compatible TreeSequence.
+    :param array time: An array of times to be converted.
+    :param string stage: The stage of the SLiM life cycle that the SLiM time
         should be computed for.
     """
     is_current_version(ts, _warn=True)
-    is_wf = (ts.metadata['SLiM']['model_type'] == "WF")
-    remembered_stage = ts.metadata['SLiM']['stage']
-    x = (stage == "first" or (stage == "early" and is_wf))
-    y = (remembered_stage == "late" or (remembered_stage == "early" and not is_wf))
-    slim_time = ts.metadata['SLiM']['tick'] - time + x + y - 1
+    slim_time = ts.metadata['SLiM']['tick'] - time
+    if ts.metadata['SLiM']['model_type'] == "WF":
+        if (ts.metadata['SLiM']['stage'] == "early" and stage == "late"):
+            slim_time -= 1
+        if (ts.metadata['SLiM']['stage'] == "late" and stage == "early"):
+            slim_time += 1
     return slim_time
 
 
 def _do_individual_parents_stuff(ts, return_parents=False):
     # Helper for has_individual_parents and individual_parents,
     # which share a lot of machinery.
     tables = ts.tables
@@ -497,15 +503,15 @@
     # edges describing relationships between individuals
     indiv_edges = np.logical_and(
             np.logical_and(edge_parent_indiv != tskit.NULL,
                                  edge_child_indiv != tskit.NULL),
             unique_parent_edges)
     # individual edges where the parent was alive during "late"
     # of the time step before the child is born
-    ind_times = ts.individuals_time
+    ind_times = individual_times(ts)
     ind_ages = individual_ages(ts)
     child_births = ind_times[edge_child_indiv[indiv_edges]]
     parent_births = ind_times[edge_parent_indiv[indiv_edges]]
     alive_edges = indiv_edges.copy()
     if ts.metadata['SLiM']['model_type'] == "WF":
         alive_edges[indiv_edges] = (child_births + 1 == parent_births)
     else:
@@ -532,20 +538,20 @@
 
 
 def individual_parents(ts):
     '''
     Finds all parent-child relationships in the tree sequence (as far as we
     can tell). The output will be a two-column array with row [i,j]
     indicating that individual i is a parent of individual j.  See
-    {func}`.has_individual_parents` for exactly which parents are returned.
+    :meth:`.has_individual_parents` for exactly which parents are returned.
 
-    See {func}`.individuals_alive_at` for further discussion about how
+    See :meth:`.individuals_alive_at` for further discussion about how
     this is determined based on when the individuals were Remembered.
 
-    :param tskit.TreeSequence ts: A :class:`tskit.TreeSequence`.
+    :param TreeSequence ts: A :class:`TreeSequence`.
     :return: An array of individual IDs, with row [i, j] if individual i is
         a parent of individual j.
     '''
     return _do_individual_parents_stuff(ts, return_parents=True)
 
 
 def has_individual_parents(ts):
@@ -559,31 +565,31 @@
     - those parental individuals were alive when the individual was born,
     - the parental individuals account for two whole genomes.
 
     This returns a boolean array indicating for each individual whether all
     these are true. Note in particular that individuals with only *one*
     recorded parent are *not* counted as "having parents".
 
-    See {func}`.individuals_alive_at` for further discussion about how
+    See :meth:`.individuals_alive_at` for further discussion about how
     this is determined based on when the individuals were Remembered.
 
-    :param tskit.TreeSequence ts: A :class:`tskit.TreeSequence`.
+    :param TreeSequence ts: A :class:`TreeSequence`.
     :return: A boolean array of length equal to ``targets``.
     '''
     return _do_individual_parents_stuff(ts, return_parents=False)
 
 
 def annotate(ts, **kwargs):
     '''
     Takes a tree sequence (as produced by msprime, for instance), and adds in the
     information necessary for SLiM to use it as an initial state, filling in
-    mostly default values. Returns a :class:`tskit.TreeSequence`.
+    mostly default values. Returns a :class:`TreeSequence`.
 
-    :param tskit.TreeSequence ts: A :class:`tskit.TreeSequence`.
-    :param str model_type: SLiM model type: either "WF" or "nonWF".
+    :param TreeSequence ts: A :class:`TreeSequence`.
+    :param string model_type: SLiM model type: either "WF" or "nonWF".
     :param int tick: What tick number in SLiM correponds to
         ``time=0`` in the tree sequence.
     :param int cycle: What cycle number in SLiM correponds to
         ``time=0`` in the tree sequence (default: equal to ``tick``).
     :param int stage: What stage in SLiM's cycle has the tree sequence
         been written out in (defaults to "early"; must be "early" or "late").
     :param str reference_sequence: A reference sequence of length
@@ -595,17 +601,17 @@
     annotate_tables(tables, **kwargs)
     return tables.tree_sequence()
 
 
 def annotate_tables(tables, model_type, tick, cycle=None, stage="early", reference_sequence=None,
         annotate_mutations=True):
     '''
-    Does the work of :func:`annotate`, but modifies the tables in place: so,
+    Does the work of :func:`annotate_defaults()`, but modifies the tables in place: so,
     takes tables as produced by ``msprime``, and makes them look like the
-    tables as output by SLiM. See :func:`annotate` for details.
+    tables as output by SLiM. See :func:`annotate_defaults` for details.
     '''
     if stage not in ("early", "late"):
         raise ValueError(f"stage must be 'early' or 'late' (provided {stage})")
     if (type(tick) is not int) or (tick < 1):
         raise ValueError("tick must be an integer and at least 1.")
     # set_nodes must come before set_populations
     if model_type == "WF":
@@ -632,40 +638,14 @@
     _annotate_nodes_individuals(tables, age=default_ages)
     _annotate_populations(tables)
     if annotate_mutations:
         _annotate_sites_mutations(tables)
     if reference_sequence is not None:
         tables.reference_sequence.data = reference_sequence
 
-def next_slim_mutation_id(ts):
-    '''
-    Returns the next SLiM mutation ID for this tree sequence. This is useful 
-    because if you want to add more mutations to your SLiM tree sequence using 
-    :func:`msprime.sim_mutations`, you may need to specify the parameter 
-    `next_id` in your :class:`msprime.SLiMMutationModel` to be larger than any 
-    existing mutation IDs. Setting `next_id` equal to the output of this 
-    function will allow the mutated tree sequence to be read in by SLiM.
-    To do this, recall that the "derived state" of SLiM's mutations are
-    comma-separated strings of mutation IDs; this function just parses all derived
-    states and returns one larger than the largest integer found. It will return an error
-    if it encounters derived states that are not comma-separated strings of integers.
-    '''
-    max_id = 0
-    for mut in ts.mutations():
-        ds = mut.derived_state
-        if len(ds) > 0:
-            for d in ds.split(","):
-                try:
-                    max_id = max(max_id, int(d))
-                except ValueError:
-                    raise ValueError(f"The derived state of a mutation ({ds}) in the tree "
-                                     "sequence is not a comma-separated list of values "
-                                     "coercible to int. This is not a valid SLiM tree sequence.")
-    return max_id + 1
-
 
 def _annotate_nodes_individuals(tables, age):
     '''
     Adds to a TableCollection the information relevant to individuals required
     for SLiM to load in a tree sequence, that is found in Node and Individual
     tables.  This will replace the metadata in those tables. For this to work,
     assumes all sample nodes are in individuals.
@@ -752,14 +732,15 @@
         tables.nodes.population[
             np.logical_and(
                 tables.nodes.individual >= 0,
                 alive_ind[tables.nodes.individual]
             )
         ]
     )
+    num_pops = max(np.max(tables.nodes.population), np.max(do_pops)) + 1
     for j, p in enumerate(tables.populations):
         if j in do_pops:
             if "slim_id" not in p.metadata:
                 md = default_slim_metadata("population")
                 md["slim_id"] = j
                 md["name"] = f"pop_{j}"
                 tables.populations[j] = p.replace(metadata=md)
@@ -772,19 +753,14 @@
     of the Mutation table,  It will also
     - give SLiM IDs to each mutation
     - replace ancestral states with ""
     This will replace any information already in the metadata or derived state
     columns of the Mutation table. We set slim_time in metadata so that
     - tick = floor(tskit time) + slim_time
     '''
-    if len(tables.mutations.metadata) > 0:
-        warnings.warn(
-                "The provided tree sequence already has some mutations with "
-                "metadata; this metadata will be overwritten."
-        )
     num_mutations = tables.mutations.num_rows
     default_mut = default_slim_metadata("mutation_list_entry")
     dsb, dso = tskit.pack_bytes([str(j).encode() for j in range(num_mutations)])
     slim_time = tables.metadata["SLiM"]["tick"] - np.floor(tables.mutations.time).astype("int")
     mms = tables.mutations.metadata_schema
     mutation_metadata = [
             mms.encode_row(
```

### Comparing `pyslim-1.0.2/pyslim/provenance.py` & `pyslim-1.0b1/pyslim/provenance.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/pyslim/slim_metadata.py` & `pyslim-1.0b1/pyslim/slim_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,41 +2,20 @@
 import json
 import warnings
 
 from ._version import *
 from .provenance import *
 
 GENOME_TYPE_AUTOSOME = 0
-"""
-A value used in node metadata ("genome_type") to indicate the node is an autosome.
-"""
 GENOME_TYPE_X = 1
-"""
-A value used in node metadata ("genome_type") to indicate the node is an X chromosome.
-"""
 GENOME_TYPE_Y = 2
-"""
-A value used in node metadata ("genome_type") to indicate the node is a Y chromosome.
-"""
 INDIVIDUAL_TYPE_HERMAPHRODITE = -1
-"""
-A value used in individual metadata ("sex") to indicate the individual is a hermaphrodite.
-"""
 INDIVIDUAL_TYPE_FEMALE = 0
-"""
-A value used in individual metadata ("sex") to indicate the individual is a male.
-"""
 INDIVIDUAL_TYPE_MALE = 1
-"""
-A value used in individual metadata ("sex") to indicate the individual is a female.
-"""
 INDIVIDUAL_FLAG_MIGRATED = 0x01
-"""
-An individual flag indicating the individual is a migrant.
-"""
 
 # These are copied from slim_globals.h and modified to be python not json (eg false->False)
 _raw_slim_metadata_schemas = {
     "tree_sequence" :
     {
         "$schema": "http://json-schema.org/schema#",
         "codec": "json",
@@ -431,30 +410,27 @@
         "type": [
                 "object",
                 "null"
         ]
     }
 }
 
-slim_metadata_schemas = {k: tskit.MetadataSchema(_raw_slim_metadata_schemas[k]) for k in _raw_slim_metadata_schemas}
-"""
-A dictionary containing the metadata schemas used by SLiM for each of the tables,
-and for top-level metadata.
-"""
+slim_metadata_schemas = {k: tskit.MetadataSchema(_raw_slim_metadata_schemas[k])
+        for k in _raw_slim_metadata_schemas}
 
 
 def default_slim_metadata(name):
-    """
+    '''
     Returns default metadata of type ``name``, where ``name`` is one of
     "tree_sequence", "edge", "site", "mutation", "mutation_list_entry",
     "node", "individual", or "population".
 
     :param str name: The type of metadata requested.
     :rtype dict:
-    """
+    '''
     if name == "tree_sequence":
         out = {
              "SLiM" : {
                  "model_type" : "nonWF",
                  "cycle" : 1,
                  "tick" : 1,
                  "file_version" : slim_file_version,
```

### Comparing `pyslim-1.0.2/pyslim/slim_tree_sequence.py` & `pyslim-1.0b1/pyslim/slim_tree_sequence.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,38 +7,23 @@
 from ._version import *
 from .slim_metadata import *
 from .provenance import *
 from .util import *
 from .slim_metadata import _old_metadata_schema
 
 INDIVIDUAL_ALIVE = 2**16
-"""
-Used in ``individual.flags`` to denote the individual is alive
-when the tree sequence was written out.
-"""
 INDIVIDUAL_REMEMBERED = 2**17
-"""
-Used in ``individual.flags`` to denote the individual was
-marked as "remembered".
-"""
 INDIVIDUAL_RETAINED = 2**18
-"""
-Used in ``individual.flags`` to denote the individual was
-marked as "retained".
-"""
 # deprecated but keep it around for backwards compatibility
 # (also, it means effectively the same thing as RETAINED)
 INDIVIDUAL_FIRST_GEN = INDIVIDUAL_RETAINED
 
+# A nucleotide k in mutation metadata actually means
+# something that in reference_sequence is NUCLEOTIDES[k]
 NUCLEOTIDES = ['A', 'C', 'G', 'T']
-"""
-Mutation metadata records the nucleotide as an integer,
-translated to ACGT by indexing this array,
-so a nucleotide value of ``k`` actually means NUCLEOTIDES[k].
-"""
 
 
 def load(*args, **kwargs):
     raise RuntimeError("This method has been removed: use tskit.load( ) instead.")
 
 
 def mutation_at(ts, node, position, time=None):
@@ -61,20 +46,20 @@
     if position < 0 or position >= ts.sequence_length:
         raise ValueError("Position {} not valid.".format(position))
     if node < 0 or node >= ts.num_nodes:
         raise ValueError("Node {} not valid.".format(node))
     if time is None:
         time = ts.node(node).time
     tree = ts.at(position)
+    # TODO: use `position` argument to ts.site( )
+    site_pos = ts.tables.sites.position
     out = tskit.NULL
-    try:
-        site = ts.site(position=position)
-    except ValueError:
-        pass
-    else:
+    if position in site_pos:
+        site_index = np.where(site_pos == position)[0][0]
+        site = ts.site(site_index)
         mut_nodes = []
         # look for only mutations that occurred before `time`
         # not strictly necessary if time was None
         for mut in site.mutations:
             if mut.time >= time:
                 mut_nodes.append(mut.node)
         n = node
```

### Comparing `pyslim-1.0.2/pyslim/spatial.py` & `pyslim-1.0b1/pyslim/spatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     '''
     Takes the locations of individuals and tests if each is within [x0, x1) and
     [y0, y1). Returns a list the same length as the number of individuals with
     True if the corresponding individual is within the bounds and False
     otherwise.  This is a helper function for `population_size`, and may change
     or be removed in the future.
 
-    :param numpy.ndarray locations: An n x 3 array with rows individuals, the first
+    :param array locations: An n x 3 array with rows individuals, the first
         column the x coordinates, and the second column the y coordinates.
     :param float x0: The lower x coordinate boundary.
     :param float x1: The upper x coordinate boundary.
     :param float y0: The lower y coordinate boundary.
     :param float y1: The upper y coordinate boundary.
     '''
     return np.logical_and(
@@ -53,16 +53,16 @@
     birth times [3, 1, 5, 4] and death times [0, 1, 2, 4]. The first individual
     is alive for three time steps in [t0, t1): 1, 2, and 3; the second
     individual for one time step: 1; the third individual for two time steps: 2
     and 3, and the fourth individual for zero (since the time interval is open
     on the right and it was born at t1). So the average population size is (3 +
     1 + 2 + 0)/(4-1) = 2.
 
-    :param numpy.ndarray birth_times: Birth times of individuals.
-    :param numpy.ndarray death_times: Death times of individuals. Should be the same
+    :param array birth_times: Birth times of individuals.
+    :param array death_times: Death times of individuals. Should be the same
         length as `birth_times`. Death times are less than or equal to birth times.
     :param float t0: Lower time endpoint.
     :param float t1: Upper time endpoint. t1 is greater than t0.
 
     '''
     # length of the segment of time in [t0, t1) that the individual
     # was alive for, i.e., of the intersection with [birth, death].
@@ -87,18 +87,18 @@
     averaged across all times in the half-open interval ``[time_bins[k], time_bins[k + 1])``.
 
     For integer endpoints of the time bins, this average is equivalent to
     recording the number of indivduals that are alive at each time in the time
     interval and have location in the relevant location bin, then taking the
     mean of these recorded population sizes.
 
-    :param tskit.TreeSequence ts: The tree sequence to calculate population size from.
-    :param numpy.ndarray x_bins: The x-coordinates of the boundaries of the location bins.
-    :param numpy.ndarray y_bins: The y-coordinates of the boundaries of the location bins.
-    :param numpy.ndarray time_bins: The endpoints of the time bins.
+    :param TreeSequence ts: The tree sequence to calculate population size from.
+    :param array x_bins: The x-coordinates of the boundaries of the location bins.
+    :param array y_bins: The y-coordinates of the boundaries of the location bins.
+    :param array time_bins: The endpoints of the time bins.
     :param str stage: The stage in the SLiM life cycle that the endpoints of
         the time bins refer to (either "early" or "late"; defaults to "late").
     :param str remembered_stage: The stage in the SLiM life cycle during which
         individuals were Remembered (defaults to the stage the tree sequence was
         recorded at, stored in metadata).
     '''
 
@@ -121,15 +121,15 @@
                       " make sure you know what you're doing.")
 
     # see individuals_alive_at for explanation
     if stage == "early" and ts.metadata['SLiM']['model_type'] == "WF":
         birth_offset = 1
     else:
         birth_offset = 0
-    birth_times = ts.individuals_time - birth_offset
+    birth_times = individual_times(ts) - birth_offset
     if (ts.metadata['SLiM']['model_type'] == "WF"
             or stage == remembered_stage):
         age_offset = 0
     else:
         if (remembered_stage == "early"
                 and stage == "late"):
             age_offset = -1
@@ -143,15 +143,15 @@
     y_breaks = y_bins
 
     nxbins = len(x_breaks) - 1
     nybins = len(y_breaks) - 1
     ntbins = len(time_breaks) - 1
     popsize = np.empty((nxbins, nybins, ntbins))
 
-    locations = ts.individuals_location
+    locations = individual_locations(ts)
 
     for i in np.arange(nxbins):
         for j in np.arange(nybins):
             x0, x1 = x_breaks[i], x_breaks[i + 1]
             y0, y1 = y_breaks[j], y_breaks[j + 1]
             in_bin = _in_location_bin(locations, x0, x1, y0, y1)
             for k in np.arange(ntbins):
```

### Comparing `pyslim-1.0.2/pyslim.egg-info/PKG-INFO` & `pyslim-1.0b1/pyslim.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyslim
-Version: 1.0.2
+Version: 1.0b1
 Summary: Manipulate tree sequences produced by SLiM.
 Home-page: https://github.com/tskit-dev/pyslim
 Author: Peter Ralph
 Author-email: petrel.harp@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/tskit-dev/pyslim/issues
 Project-URL: Source, https://github.com/tskit-dev/pyslim
 Keywords: tree sequences,tskit
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyslim
 
 `pyslim` is a python module that provides a few extra tools for dealing with tree sequences
@@ -26,7 +27,9 @@
 ## Installation
 
 To install `pyslim`, do
 ```
 pip install pyslim
 ```
 or read the documentation for how to [install from source](https://tskit.dev/pyslim/stable/development.html#sec-development).
+
+
```

### Comparing `pyslim-1.0.2/pyslim.egg-info/SOURCES.txt` & `pyslim-1.0b1/pyslim.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 .codecov.yml
 .gitignore
 CHANGELOG.rst
 LICENSE
 README.html
 README.md
 setup.py
-.github/workflows/docs.yml
+.circleci/config.yml
 .github/workflows/tests.yml
 docs/.gitignore
 docs/Makefile
 docs/_config.yml
 docs/_toc.yml
 docs/annotate_genome.pdf
 docs/annotated_p_vs_s.pdf
 docs/build.sh
 docs/conf.py
 docs/development.md
 docs/example_sim.slim
-docs/generation_time.slim
 docs/installation.md
 docs/introduction.md
 docs/metadata.md
 docs/migrants.slim
 docs/neutral_restart.slim
 docs/phylo_bgs.slim
 docs/previous_versions.md
 docs/python_api.md
 docs/rapid_adaptation.slim
 docs/reload_annotated.slim
 docs/selection.slim
-docs/time_units.md
 docs/tutorial.md
 docs/util.py
 docs/vignette_coalescent_diversity.md
 docs/vignette_continuing.md
 docs/vignette_parallel_phylo.md
 docs/vignette_space.md
 docs/vignette_space.slim
@@ -52,15 +50,14 @@
 docs/_static/pedigree_mutate.svg
 docs/_static/pedigree_recapitate.png
 docs/_static/pedigree_recapitate.svg
 docs/_static/pedigree_remember.png
 docs/_static/pedigree_simplify.png
 docs/_static/pedigree_simplify.svg
 docs/_static/pedigrees.ink.svg
-docs/_static/pedigrees.ink.svg.md5
 docs/_static/phylo.pdf
 docs/_static/phylo.png
 docs/_static/phylo.tsv
 docs/_static/recomb_rates.tsv
 pyslim/__init__.py
 pyslim/_version.py
 pyslim/methods.py
@@ -72,15 +69,14 @@
 pyslim.egg-info/PKG-INFO
 pyslim.egg-info/SOURCES.txt
 pyslim.egg-info/dependency_links.txt
 pyslim.egg-info/not-zip-safe
 pyslim.egg-info/requires.txt
 pyslim.egg-info/top_level.txt
 requirements/conda-minimal.txt
-requirements/CI-conda/ci-environment.yml
 requirements/CI-conda/requirements.txt
 requirements/CI-docs/requirements.txt
 requirements/CI-pip/requirements.txt
 tests/README.md
 tests/__init__.py
 tests/conftest.py
 tests/recipe_specs.py
@@ -124,21 +120,16 @@
 tests/test_recipes/recipe_WF.v3.3.1.trees
 tests/test_recipes/recipe_WF.v3.4.trees
 tests/test_recipes/recipe_WF.v3.5.trees
 tests/test_recipes/recipe_WF.v3.5_and_v3.6.trees
 tests/test_recipes/recipe_WF.v3.6.trees
 tests/test_recipes/recipe_WF.v3.7.trees
 tests/test_recipes/recipe_WF_early_early.slim
-tests/test_recipes/recipe_WF_early_first.slim
 tests/test_recipes/recipe_WF_early_late.slim
-tests/test_recipes/recipe_WF_first_early.slim
-tests/test_recipes/recipe_WF_first_first.slim
-tests/test_recipes/recipe_WF_first_late.slim
 tests/test_recipes/recipe_WF_late_early.slim
-tests/test_recipes/recipe_WF_late_first.slim
 tests/test_recipes/recipe_WF_late_late.slim
 tests/test_recipes/recipe_WF_migration.slim
 tests/test_recipes/recipe_init_mutated_WF.slim
 tests/test_recipes/recipe_init_mutated_nonWF.slim
 tests/test_recipes/recipe_long_WF.slim
 tests/test_recipes/recipe_long_nonWF.slim
 tests/test_recipes/recipe_long_nucleotides.slim
@@ -148,32 +139,25 @@
 tests/test_recipes/recipe_nonWF.v3.2.trees
 tests/test_recipes/recipe_nonWF.v3.3.1.trees
 tests/test_recipes/recipe_nonWF.v3.4.trees
 tests/test_recipes/recipe_nonWF.v3.5.trees
 tests/test_recipes/recipe_nonWF.v3.6.trees
 tests/test_recipes/recipe_nonWF.v3.7.trees
 tests/test_recipes/recipe_nonWF_early_early.slim
-tests/test_recipes/recipe_nonWF_early_first.slim
 tests/test_recipes/recipe_nonWF_early_late.slim
-tests/test_recipes/recipe_nonWF_first_early.slim
-tests/test_recipes/recipe_nonWF_first_first.slim
-tests/test_recipes/recipe_nonWF_first_late.slim
 tests/test_recipes/recipe_nonWF_late_early.slim
-tests/test_recipes/recipe_nonWF_late_first.slim
 tests/test_recipes/recipe_nonWF_late_late.slim
 tests/test_recipes/recipe_nonWF_nonstacked.slim
 tests/test_recipes/recipe_nonWF_selfing.slim
 tests/test_recipes/recipe_nucleotides_WF.slim
 tests/test_recipes/recipe_nucleotides_nonWF.slim
 tests/test_recipes/recipe_nucleotides_plus_others.slim
 tests/test_recipes/recipe_record_everyone_WF_early.slim
-tests/test_recipes/recipe_record_everyone_WF_first.slim
 tests/test_recipes/recipe_record_everyone_WF_late.slim
 tests/test_recipes/recipe_record_everyone_nonWF_early.slim
-tests/test_recipes/recipe_record_everyone_nonWF_first.slim
 tests/test_recipes/recipe_record_everyone_nonWF_late.slim
 tests/test_recipes/recipe_remember_and_retain.slim
 tests/test_recipes/recipe_retain_everyone_WF_late.slim
 tests/test_recipes/recipe_retain_everyone_nonWF_late.slim
 tests/test_recipes/recipe_retain_sometimes_WF_late.slim
 tests/test_recipes/recipe_retain_sometimes_nonWF_late.slim
 tests/test_recipes/recipe_retain_unary_WF_late.slim
@@ -181,12 +165,10 @@
 tests/test_recipes/recipe_roots.slim
 tests/test_recipes/recipe_with_metadata.slim
 tests/test_recipes/restart_WF.slim
 tests/test_recipes/restart_and_remove_subpop_nonWF.slim
 tests/test_recipes/restart_and_run_WF.slim
 tests/test_recipes/restart_and_run_nonWF.slim
 tests/test_recipes/restart_msprime.slim
-tests/test_recipes/restart_multispecies_WF.slim
-tests/test_recipes/restart_multispecies_nonWF.slim
 tests/test_recipes/restart_nonWF.slim
 tests/test_recipes/restart_nucleotides_WF.slim
 tests/test_recipes/restart_nucleotides_nonWF.slim
```

### Comparing `pyslim-1.0.2/setup.py` & `pyslim-1.0b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,19 @@
       license='MIT',
       packages=['pyslim'],
       include_package_data=True,
       zip_safe=False,
       install_requires=[
           'msprime>=1.0.1',
           'tskit',
-          'numpy'
-      ],
+          'kastore',
+          'numpy'],
       extras_require={
           'dev': [],
       },
 
       setup_requires=[],
       project_urls={
           'Bug Reports': 'https://github.com/tskit-dev/pyslim/issues',
           'Source': 'https://github.com/tskit-dev/pyslim',
       },
-)
+      )
```

### Comparing `pyslim-1.0.2/tests/README.md` & `pyslim-1.0b1/tests/README.md`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/__init__.py` & `pyslim-1.0b1/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Common code for the pyslim test cases.
 """
 import os
 import json
 import random
+import base64
 import warnings
 
 import pyslim
 import tskit
 import msprime
 import pytest
+import attr
 import numpy as np
 
 
 class PyslimTestCase:
     '''
     Base class for test cases in pyslim.
     '''
```

### Comparing `pyslim-1.0.2/tests/benchmark/annotation.sh` & `pyslim-1.0b1/tests/benchmark/annotation.sh`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/benchmark/metadata.sh` & `pyslim-1.0b1/tests/benchmark/metadata.sh`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/benchmark/metadata.slim` & `pyslim-1.0b1/tests/benchmark/metadata.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/conftest.py` & `pyslim-1.0b1/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -75,169 +75,82 @@
             self.Outfile(
                 path=os.path.join(out_dir, "out_mutations.json"),
                 slim_name="MUTATIONS_FILE",
                 post_process=self.read_dictionary,
                 key="mutation_info",
             ),
         ]
-
     def __getitem__(self, index):
         return self._outfiles[index]
 
     def __len__(self, index):
         return len(self._outfiles)
     
     def results(self):
         res = {"path": {}}
         for o in self._outfiles:
             res["path"][o.key] = o.path
             if os.path.isfile(o.path):
                 assert o.key not in res
                 res[o.key] = o.post_process(o.path) 
         return res
-
-
-class MultiOutfiles(Outfiles):
     
-    def __init__(self, out_dir, species):
-        # Note: the 'key' below cannot match a 'key' in recipe_specs
-        self._outfiles = []
-        for sp in species:
-            self._outfiles.extend([
-                self.Outfile(
-                    path=os.path.join(out_dir, f"{sp}_out.trees"),
-                    slim_name=f"TREES_FILE_{sp}",  # The var containing the path name for SLiM output
-                    post_process=tskit.load,  # function applied on path to create returned obj
-                    key=f"ts_{sp}",  # The key to use for the post-processed item in the returned dict
-                ),
-                self.Outfile(
-                    path=os.path.join(out_dir, f"{sp}_out.pedigree"),
-                    slim_name=f"PEDIGREE_FILE_{sp}",
-                    post_process=self.parse_pedigree_info,
-                    key=f"info_{sp}",
-                ),
-                self.Outfile(
-                    path=os.path.join(out_dir, f"{sp}_out_mutations.json"),
-                    slim_name=f"MUTATIONS_FILE_{sp}",
-                    post_process=self.read_dictionary,
-                    key=f"mutation_info_{sp}",
-                ),
-            ])
-
 
-def run_slim(recipe, out_dir, recipe_dir="test_recipes", species=None, **kwargs):
+def run_slim(recipe, out_dir, recipe_dir="test_recipes", **kwargs):
     """
     Run the recipe, present in the recipe_dir, outputting to files in out_dir
     kwargs are passed as variables to SLiM (in addition to the outfiles)
     """
     script_dir = os.path.dirname(os.path.realpath(__file__))
     full_recipe = os.path.abspath(os.path.join(script_dir, recipe_dir, recipe))
     if not os.path.isfile(full_recipe):
         raise RuntimeError(f"{full_recipe} cannot be found")
     assert os.path.isdir(out_dir)  # should have been generated by the calling function
-    if species is None:
-        outfiles = Outfiles(out_dir)
-    else:
-        outfiles = MultiOutfiles(out_dir, species)
+    outfiles = Outfiles(out_dir)
     slim_vars = []
     for o in outfiles:
         if o.slim_name != "":
-            # for happy windows filepaths
-            tmp_str = o.path.replace('\\', '\\\\')
-            slim_vars += ["-d", f"{o.slim_name}=\"{tmp_str}\""]
+            slim_vars += ["-d", f"{o.slim_name}=\"{o.path}\""]
     for k in kwargs:
         x = kwargs[k]
         if x is not None:
             if isinstance(x, str) and x[:10] != 'Dictionary':
-                # for happy windows filepaths
-                x = x.replace('\\', '\\\\')
                 x = f"'{x}'"
             if isinstance(x, bool):
                 x = 'T' if x else 'F'
             slim_vars += ["-d", f"{k}={x}"]
     cmd = ["slim", "-s", "23"] + slim_vars + [full_recipe]
     print(f"Running {' '.join(cmd)}, outputting errors etc. to '{out_dir}/SLiM_run_output.log'")
     with open(os.path.join(out_dir, "SLiM_run_output.log"), "w") as out:
         retval = subprocess.call(cmd, stderr=subprocess.STDOUT, stdout=out)
-    if retval != 0:
-        errmsg = f"Could not run {' '.join(cmd)}"
-        errline = False
-        with open(os.path.join(out_dir, "SLiM_run_output.log"), "r") as err:
-            for line in err:
-                if line[:5] == "ERROR" or line[:5] == "Error":
-                    errline = True
-                    errmsg += "\n"
-                if errline and len(line.strip()) > 0:
-                    errmsg += line
-        raise RuntimeError(errmsg)
+        if retval != 0:
+            raise RuntimeError(f"Could not run {' '.join(cmd)}")
     return outfiles.results()
 
 
-def _obj_to_eidos(x):
-    if isinstance(x, str):
-        out = '"' + x + '"'
-    elif isinstance(x, dict):
-        out = _dict_to_eidos(x)
-    elif x is None:
-        out = 'NULL'
-    else:
-        out = x
-    return out
-
-
-def _dict_to_eidos(d):
-    txt = "Dictionary(" + ", ".join([f"\"{a}\", {_obj_to_eidos(b)}" for a, b in d.items()]) + ")"
-    return txt
-
-
 class HelperFunctions:
     @classmethod
     def run_slim_restart(cls, in_ts, recipe, out_dir, subpop_map=None, **kwargs):
         # Saves out the tree sequence to a trees file and run the SLiM recipe
         # on it, saving to files in out_dir.
         infile = os.path.join(out_dir, "in.trees")
         in_ts.dump(infile)
-        # for happy windows filepaths       
-        infile_str = infile.replace('\\', '\\\\')
         kwargs['TREES_IN'] = infile
         if 'STAGE' not in kwargs:
             kwargs['STAGE'] = in_ts.metadata['SLiM']['stage']
         if subpop_map is not None:
             # subpopMap argument has entries like { "p1" : 2 },
             # meaning that when loaded in, subpop p1 will be the second row
             # in the population table
-            spm = _dict_to_eidos(subpop_map)
+            spm = "Dictionary(" + ", ".join([f"\"{a}\", {b}" for a, b in subpop_map.items()]) + ")"
             kwargs['SUBPOP_MAP'] = spm
         results = run_slim(recipe, out_dir, **kwargs)
         return results["ts"]
 
     @classmethod
-    def run_multispecies_slim_restart(cls, in_ts, recipe, out_dir, subpop_map=None, **kwargs):
-        # in_ts should now be a dictionary with keys corresponding to species names
-        infiles = {}
-        for sp in in_ts:
-            infiles[sp] = os.path.join(out_dir, f"{sp}_in.trees")
-            in_ts[sp].dump(infiles[sp])
-        infiles_str_dict = {}
-        for k, v in infiles.items():
-            # for happy windows filepaths
-            infiles_str_dict[k] = v.replace('\\', '\\\\')        
-        kwargs['TREES_IN'] = _dict_to_eidos(infiles_str_dict)
-        if 'STAGE' not in kwargs:
-            kwargs['STAGE'] = in_ts[sp].metadata['SLiM']['stage']
-        if subpop_map is not None:
-            # subpopMap argument has entries like { "p1" : 2 },
-            # meaning that when loaded in, subpop p1 will be the second row
-            # in the population table
-            kwargs['SUBPOP_MAP'] = _dict_to_eidos(subpop_map)
-        results = run_slim(recipe, out_dir, species=list(in_ts.keys()), **kwargs)
-        out = { sp: results[f"ts_{sp}"] for sp in in_ts }
-        return out
-
-    @classmethod
     def run_msprime_restart(cls, in_ts, out_dir, sex=None, WF=False):
         out_ts = cls.run_slim_restart(
             in_ts,
             "restart_msprime.slim",  # This is standard script defined in test_recipes
             out_dir,
             WF=WF,
             SEX=sex,
```

### Comparing `pyslim-1.0.2/tests/extra_recipes/Makefile` & `pyslim-1.0b1/tests/extra_recipes/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 export SHELL=/bin/bash
 .PRECIOUS : recipe_17.4.trees
 
-check : recipe_17.1_overlaid.log recipe_17.3.log recipe_17.4.png recipe_17.5.png recipe_17.7.log recipe_17.8_III.log recipe_17.9.log recipe_17.10.log recipe_nucleotides_II.log recipe_nucleotides_III.log
+check : recipe_17.1_overlaid.log recipe_17.3.log recipe_17.4.png recipe_17.5.png recipe_17.7.log recipe_17.8_III.log recipe_17.9.log recipe_nucleotides_II.log recipe_nucleotides_III.log
 	echo "-------------"
 	echo "17.1 + 17.2"
 	cat recipe_17.1_overlaid.log
 	echo "-------------"
 	echo "17.3"
 	cat recipe_17.3.log
 	echo "-------------"
@@ -21,17 +21,14 @@
 	echo "17.8"
 	head  recipe_17.8_III.log
 	echo "(snipped $$(wc -l recipe_17.8_III.log) lines)"
 	echo "-------------"
 	echo "17.9"
 	cat recipe_17.9.log 
 	echo "-------------"
-	echo "17.10"
-	cat recipe_17.10.log 
-	echo "-------------"
 	echo "18.13 II"
 	cat recipe_nucleotides_II.log
 	echo "-------------"
 	echo "18.13 III"
 	head recipe_nucleotides_III.log
 	echo "(snipped $$(wc -l recipe_nucleotides_III.log) lines)"
 	echo "-------------"
@@ -88,20 +85,14 @@
 
 recipe_17.9.trees : Recipe\ 17.9\ -\ Starting\ a\ sexual\ nonWF\ model\ with\ a\ coalescent\ history\ I.py
 	python3 "$<"
 
 recipe_17.9.log : Recipe\ 17.9\ -\ Starting\ a\ sexual\ nonWF\ model\ with\ a\ coalescent\ history\ II.txt recipe_17.9.trees
 	slim -s 2345 "$<" &> $@
 
-recipe_17.10.log : Recipe\ 17.10\ -\ Adding\ a\ neutral\ burn-in\ after\ simulation\ with\ recapitation\ II.py recipe_17.10_decap.trees
-	python3 "$<" &> $@
-
-recipe_17.10_decap.trees : Recipe\ 17.10\ -\ Adding\ a\ neutral\ burn-in\ after\ simulation\ with\ recapitation\ I.txt
-	slim -s 2344 "$<" &> $@.log
-
 recipe_nucleotides.trees : Recipe\ 18.13\ -\ Tree-sequence\ recording\ and\ nucleotide-based\ models\ I.txt
 	slim -s 2345 "$<" &> $@.log
 
 recipe_nucleotides_II.log : Recipe\ 18.13\ -\ Tree-sequence\ recording\ and\ nucleotide-based\ models\ II.py recipe_nucleotides.trees
 	python3 "$<" &> $@
 
 recipe_nucleotides_III.log : Recipe\ 18.13\ -\ Tree-sequence\ recording\ and\ nucleotide-based\ models\ III.py recipe_nucleotides.trees
```

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.1 - A minimal tree-seq model.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.1 - A minimal tree-seq model.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation I.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation I.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation II.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.10 - Adding a neutral burn-in after simulation with recapitation II.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Keywords: Python, tree-sequence recording, tree sequence recording
 
-import tskit, pyslim
+import msprime, pyslim
 import numpy as np
 import matplotlib.pyplot as plt
 
 # Load the .trees file
 ts = tskit.load("recipe_17.10_decap.trees")    # no simplify!
 
 # Calculate tree heights, giving uncoalesced sites the maximum time
```

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.2 - Overlaying neutral mutations.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.2 - Overlaying neutral mutations.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.3 - Simulation conditional upon fixation of a sweep, preserving ancestry I.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.3 - Simulation conditional upon fixation of a sweep, preserving ancestry I.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) I.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) I.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) II.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.4 - Detecting the dip in diversity (analyzing tree heights in Python) II.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) I.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) I.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) II.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.5 - Mapping admixture (analyzing ancestry in Python) II.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit I.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit I.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit II.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.7 - Analyzing selection coefficients in Python with tskit II.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history II.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.8 - Starting a hermaphroditic WF model with a coalescent history II.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history I.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history I.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history II.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 17.9 - Starting a sexual nonWF model with a coalescent history II.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models I.txt` & `pyslim-1.0b1/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models I.txt`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models II.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models II.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models III.py` & `pyslim-1.0b1/tests/extra_recipes/Recipe 18.13 - Tree-sequence recording and nucleotide-based models III.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_annotation.py` & `pyslim-1.0b1/tests/test_annotation.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,105 +112,14 @@
         assert in_ts.num_provenances + 1 == out_ts.num_provenances
         in_tables = in_ts.dump_tables()
         in_tables.sort()
         out_tables = out_ts.dump_tables()
         out_tables.sort()
         self.assertTableCollectionsEqual(in_tables, out_tables, skip_provenance=-1)
 
-    def verify_remapping(self, ts, rts, subpop_map):
-        # below we assume the restart has not done additional simulation
-        do_remap = (subpop_map is not None)
-        if not do_remap:
-            subpop_map = { f"p{k}" : k for k in range(ts.num_populations) }
-        fwd_map = {-1 : -1}
-        rev_map = {-1 : -1}
-        for pk in subpop_map:
-            # keys are requried to be of the form "pK"
-            rts_k = int(pk[1:])
-            assert rts_k < rts.num_populations
-            ts_k = subpop_map[pk]
-            assert ts_k < ts.num_populations
-            assert ts_k not in fwd_map
-            fwd_map[ts_k] = rts_k
-            assert rts_k not in rev_map
-            rev_map[rts_k] = ts_k
-
-        # all pops in ts should be present UNLESS they have no metadata
-        for pop in ts.populations():
-            assert pop.id in fwd_map or pop.metadata is None
-
-        # any extra pops in rts should have empty metadata
-        for pop in rts.populations():
-            if pop.id not in rev_map:
-                assert pop.metadata is None
-
-        for ts_k, rts_k in fwd_map.items():
-            if ts_k != -1:
-                ts_pop = ts.population(ts_k)
-                rts_pop = rts.population(rts_k)
-                ts_md = ts_pop.metadata
-                rts_md = rts_pop.metadata
-                if ts_md is None:
-                    assert rts_md is None
-                else:
-                    if do_remap and (
-                            ts_md['name'] == f"p{ts_pop.id}"
-                            or ts_md['name'] == f"pop_{ts_pop.id}"
-                    ):
-                        ts_md['name'] = f"p{rts_pop.id}"
-                    assert ts_md['name'] == rts_md['name']
-                    if "slim_id" not in ts_md:
-                        assert ts_md == rts_md
-                    else:
-                        assert ts_md["slim_id"] == ts_pop.id
-                        assert rts_md["slim_id"] == rts_pop.id
-                        k = "migration_records"
-                        if k in ts_md:
-                            assert k in rts_md or len(ts_md[k]) == 0
-                        else:
-                            assert k not in rts_md or len(rts_md[k]) == 0
-                        if k in ts_md and k in rts_md:
-                            assert len(ts_md[k]) == len(rts_md[k])
-                            for x, y in zip(ts_md[k], rts_md[k]):
-                                assert x['migration_rate'] == y['migration_rate']
-                                assert fwd_map[x['source_subpop']] == y['source_subpop']
-
-        # check other tables have been remapped
-        # (uses the fact that no additional simulation has been done)
-        assert ts.num_nodes == rts.num_nodes
-        for n, rn in zip(ts.nodes(), rts.nodes()):
-            n.population = fwd_map[n.population]
-            # there can be rounding error due to time shift
-            assert np.isclose(n.time, rn.time, atol=1e-16)
-            n.time = rn.time
-            assert n == rn
-
-        assert ts.num_migrations == rts.num_migrations
-        for m, rm in zip(ts.migrations(), rts.migrations()):
-            m.source = fwd_map[m.source]
-            m.dest = fwd_map[m.dest]
-            assert m == rm
-
-        assert ts.num_mutations == rts.num_mutations
-        for m, rm in zip(ts.mutations(), rts.mutations()):
-            md = m.metadata
-            rmd = rm.metadata
-            assert len(md['mutation_list']) == len(rmd['mutation_list'])
-            for x, y in zip(md['mutation_list'], rmd['mutation_list']):
-                x['subpopulation'] = fwd_map[x['subpopulation']]
-                assert x == y
-
-        assert ts.num_individuals == rts.num_individuals
-        for i, ri in zip(ts.individuals(), rts.individuals()):
-            md = i.metadata
-            rmd = ri.metadata
-            md['subpopulation'] = fwd_map[md['subpopulation']]
-            assert md == rmd
-
-
     def test_annotate_errors(self, helper_functions):
         for ts in helper_functions.get_msprime_examples():
             with pytest.raises(ValueError):
                 _ = pyslim.annotate(ts, model_type="WF", tick=0)
             with pytest.raises(ValueError):
                 _ = pyslim.annotate(ts, model_type="WF", tick=4.4)
             with pytest.raises(ValueError):
@@ -229,32 +138,14 @@
                 discrete_genome=False,
                 random_seed=9,
         )
         with pytest.raises(ValueError) as except_info:
             _ = pyslim.annotate(ts, model_type="WF", tick=1)
         assert "not at integer" in str(except_info)
 
-    def test_warns_overwriting_mutations(self, helper_functions):
-        ts = msprime.sim_ancestry(
-                4,
-                population_size=10,
-                sequence_length=10,
-                recombination_rate=0.01,
-                random_seed=100,
-        )
-        ts = msprime.sim_mutations(
-                ts,
-                rate=1,
-                random_seed=12,
-                model=msprime.SLiMMutationModel(type=1)
-        )
-        assert ts.num_mutations > 0
-        with pytest.warns(Warning, match="already has.*metadata"):
-            slim_ts = pyslim.annotate(ts, model_type="WF", tick=1) 
-
     def test_just_simulate(self, helper_functions, tmp_path):
         ts = msprime.sim_ancestry(
                 4,
                 population_size=10,
                 sequence_length=10,
                 recombination_rate=0.01,
                 random_seed=100,
@@ -432,15 +323,15 @@
                     [ms.validate_and_encode_row(r) for r in metadata]
             )
             new_ts = tables.tree_sequence()
             for j, x in enumerate(new_ts.mutations()):
                 md = x.metadata
                 assert np.isclose(md['mutation_list'][0]["selection_coeff"], selcoefs[j])
 
-    def test_dont_annotate_mutations(self):
+    def test_dont_annotate_mutations(self, helper_functions):
         # Test the option to not overwrite mutation annotations
         ts = msprime.sim_ancestry(10, random_seed=5)
         ts = msprime.sim_mutations(ts, rate=5, random_seed=3)
         assert ts.num_mutations > 0
         tables = ts.dump_tables()
         pre_mutations = tables.mutations.copy()
         pyslim.annotate_tables(
@@ -450,102 +341,76 @@
                 annotate_mutations=False
         )
         # this is necessary because b'' actually is decoded to
         # an empty mutation_list by the schema
         pre_mutations.metadata_schema = tables.mutations.metadata_schema
         assert tables.mutations.equals(pre_mutations)
 
-    def test_annotate_empty(self):
-        t = tskit.TableCollection(sequence_length=10)
-        at = pyslim.annotate_tables(t, model_type='nonWF', tick=1)
-        assert t.metadata_schema == pyslim.slim_metadata_schemas['tree_sequence']
-        for x in ("population", "individual", "node", "site", "mutation"):
-            assert getattr(t, x + "s").metadata_schema == pyslim.slim_metadata_schemas[x]
-
     def test_no_populations_errors(self, helper_functions, tmp_path):
         # test SLiM errors when individuals are in non-SLiM populations
         ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=456)
+        ts = pyslim.annotate(ts, model_type='nonWF', tick=1, stage="late")
         t = ts.dump_tables()
-        p = t.populations.add_row(metadata={'name': '', 'description': ''})
-        i = t.individuals.add_row()
-        t.nodes.add_row(time=0.0, flags=tskit.NODE_IS_SAMPLE, individual=i)
-        t.nodes.add_row(time=0.0, flags=tskit.NODE_IS_SAMPLE, individual=i)
-        pyslim.annotate_tables(t, model_type='nonWF', tick=1, stage="late")
-        pop = t.populations[-1]
-        t.populations[-1] = pop.replace(metadata = {'name' : 'not_slim', 'description' : ''})
-        ind = t.individuals[-1]
-        md = ind.metadata
-        md['subpopulation'] = (t.populations.num_rows - 1)
-        t.individuals[-1] = ind.replace(metadata=md)
+        t.populations.clear()
+        t.populations.add_row(metadata={})
         ts = t.tree_sequence()
-        with pytest.raises(RuntimeError, match='individual has a subpopulation id .1.'):
+        for p in ts.populations():
+            assert "slim_id" not in p.metadata
+        with pytest.raises(RuntimeError):
             _ = helper_functions.run_slim_restart(
                     ts,
-                    "restart_nonWF.slim",
+                    "restart_WF.slim",
                     tmp_path,
-                    WF=False,
+                    WF=True,
             )
 
     def test_empty_populations_errors(self, helper_functions, tmp_path):
         # test SLiM errors on having empty populations in a WF model
         ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=455)
         ts = pyslim.annotate(ts, model_type='WF', tick=1, stage="late")
-        # first make sure does not error without the empty pops
-        rts = helper_functions.run_slim_restart(
-                ts,
-                "restart_WF.slim",
-                tmp_path,
-                WF=True,
-        )
-        assert rts.num_populations == 1
-        # now add empty subpops
         t = ts.dump_tables()
         for k in range(5):
             md = pyslim.default_slim_metadata('population')
             md['slim_id'] = k + 1
             md['name'] = f"new_pop_num_{k}"
             t.populations.add_row(metadata=md)
         ts = t.tree_sequence()
         for p in ts.populations():
             assert "slim_id" in p.metadata
-        with pytest.raises(RuntimeError, match='subpopulation.*empty'):
+        with pytest.raises(RuntimeError):
             _ = helper_functions.run_slim_restart(
                     ts,
                     "restart_WF.slim",
                     tmp_path,
                     WF=True,
             )
 
     def test_empty_populations(self, helper_functions, tmp_path):
         # test SLiM doesn't error on having empty populations in a nonWF model
         # however, it may rewrite the metadata
-        ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=456)
+        ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=455)
         ts = pyslim.annotate(ts, model_type='nonWF', tick=1)
         t = ts.dump_tables()
         for k in range(5):
             md = pyslim.default_slim_metadata('population')
             md['slim_id'] = k + 1
             md['name'] = f"new_pop_num_{k}"
             md['description'] = f"the {k}-th added pop"
             t.populations.add_row(metadata=md)
         ts = t.tree_sequence()
-        for subpop_map in (
-                None,
-                {"p0": 0, "p1": 1, "p2": 2, "p3": 3, "p4": 4, "p5": 5},
-                {"p0": 0, "p2": 1, "p1": 2, "p9": 3, "p4": 4, "p6": 5},
-                {"p10": 0, "p2": 1, "p1": 2, "p9": 3, "p4": 4, "p6": 5},
-            ):
-            sts = helper_functions.run_slim_restart(
-                    ts,
-                    "restart_nonWF.slim",
-                    tmp_path,
-                    WF=False,
-                    subpop_map=subpop_map,
-            )
-            self.verify_remapping(ts, sts, subpop_map)
+        sts = helper_functions.run_slim_restart(
+                ts,
+                "restart_nonWF.slim",
+                tmp_path,
+                WF=False,
+        )
+        assert ts.num_populations == sts.num_populations
+        for p, q in zip(ts.populations(), sts.populations()):
+            assert p.metadata['name'] == q.metadata['name']
+            assert p.metadata['slim_id'] == q.metadata['slim_id']
 
     def test_many_populations(self, helper_functions, tmp_path):
         # test we can add more than one population and that names are preserved
         ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=455)
         t = ts.dump_tables()
         for k in range(1, 6):
             md = pyslim.default_slim_metadata('population')
@@ -566,58 +431,14 @@
                 tmp_path,
                 WF=True,
         )
         for k in range(1, 6):
             md = sts.population(k).metadata
             assert md['name'] == f"new_pop_num_{k}"
 
-    def test_many_species_errors(self, helper_functions, tmp_path):
-        # should error when there are population conflicts between species
-        fox_ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=455)
-        fox_ts = pyslim.annotate(fox_ts, model_type='WF', tick=1)
-        mouse_ts = msprime.sim_ancestry(5, population_size=20, sequence_length=1000, random_seed=234)
-        mouse_ts = pyslim.annotate(mouse_ts, model_type='WF', tick=1)
-        with pytest.raises(RuntimeError, match='p0 has been used already'):
-            _ = helper_functions.run_multispecies_slim_restart(
-                    {'fox': fox_ts, 'mouse': mouse_ts},
-                    'restart_multispecies_WF.slim',
-                    tmp_path,
-                    WF=True,
-            )
-        with pytest.raises(RuntimeError, match='p1 has been used already'):
-            _ = helper_functions.run_multispecies_slim_restart(
-                    {'fox': fox_ts, 'mouse': mouse_ts},
-                    'restart_multispecies_WF.slim',
-                    tmp_path,
-                    WF=True,
-                    subpop_map={'fox': {'p1': 0}, 'mouse': {'p1': 0}},
-            )
-
-    def test_many_species(self, helper_functions, tmp_path):
-        # verify we can load more than one species
-        for wf in (True, False):
-            fox_ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=455)
-            mouse_ts = msprime.sim_ancestry(5, population_size=20, sequence_length=1000, random_seed=234)
-            fox_ts = pyslim.annotate(fox_ts, model_type="WF" if wf else "nonWF", tick=1)
-            mouse_ts = pyslim.annotate(mouse_ts, model_type="WF" if wf else "nonWF", tick=1)
-            for subpop_map in (
-                        {'fox' : None, 'mouse' : {'p1' : 0}},
-                        {'fox' : {'p1' : 0}, 'mouse' : None},
-                        {'fox' : {'p3' : 0}, 'mouse' : {'p0' : 0}},
-                    ):
-                tsd = helper_functions.run_multispecies_slim_restart(
-                        {'fox': fox_ts, 'mouse': mouse_ts},
-                        'restart_multispecies_WF.slim' if wf else 'restart_multispecies_nonWF.slim',
-                        tmp_path,
-                        WF=wf,
-                        subpop_map = subpop_map,
-                )
-                self.verify_remapping(fox_ts, tsd['fox'], subpop_map['fox'])
-                self.verify_remapping(mouse_ts, tsd['mouse'], subpop_map['mouse'])
-
     def test_keeps_extra_populations(self, helper_functions, tmp_path):
         # test that non-SLiM metadata is not removed
         d = msprime.Demography()
         d.add_population(initial_size=10, name="A", extra_metadata={"pi": 3.1415})
         md = pyslim.default_slim_metadata('population')
         del md['name']
         del md['description']
@@ -644,102 +465,112 @@
         assert p.metadata['pi'] == 3.1415
         p = sts.population(1)
         assert p.metadata['name'] == "B"
         p = sts.population(2)
         assert p.metadata['name'] == "C"
         assert p.metadata['abc'] == 123
 
+    def verify_remapping(self, ts, rts, subpop_map):
+        # below we assume the restart has not done additional simulation
+        do_remap = (subpop_map is not None)
+        if not do_remap:
+            subpop_map = { f"p{k}" : k for k in range(ts.num_populations) }
+        fwd_map = {-1 : -1}
+        rev_map = {-1 : -1}
+        for pk in subpop_map:
+            rts_k = int(pk[1:])
+            assert rts_k < rts.num_populations
+            ts_k = subpop_map[pk]
+            assert ts_k < ts.num_populations
+            fwd_map[ts_k] = rts_k
+            rev_map[rts_k] = ts_k
+
+        # all pops in ts should be present
+        for pop in ts.populations():
+            assert pop.id in fwd_map
+
+        # any extra pops in rts should have empty metadata
+        for pop in rts.populations():
+            if pop.id not in rev_map:
+                assert pop.metadata is None
+
+        for ts_k, rts_k in fwd_map.items():
+            if ts_k != -1:
+                ts_pop = ts.population(ts_k)
+                rts_pop = rts.population(rts_k)
+                ts_md = ts_pop.metadata
+                rts_md = rts_pop.metadata
+                if ts_md is None:
+                    assert rts_md is None
+                else:
+                    if do_remap and (
+                            ts_md['name'] == f"p{ts_pop.id}"
+                            or ts_md['name'] == f"pop_{ts_pop.id}"
+                    ):
+                        ts_md['name'] = f"p{rts_pop.id}"
+                    assert ts_md['name'] == rts_md['name']
+                    if "slim_id" not in ts_md:
+                        assert ts_md == rts_md
+                    else:
+                        assert ts_md["slim_id"] == ts_pop.id
+                        assert rts_md["slim_id"] == rts_pop.id
+                        k = "migration_records"
+                        assert (k in ts_md) == (k in rts_md)
+                        if k in ts_md:
+                            assert len(ts_md[k]) == len(rts_md[k])
+                            for x, y in zip(ts_md[k], rts_md[k]):
+                                assert x['migration_rate'] == y['migration_rate']
+                                assert fwd_map[x['source_subpop']] == y['source_subpop']
+
+        # check other tables have been remapped
+        # (uses the fact that no additional simulation has been done)
+        assert ts.num_nodes == rts.num_nodes
+        for n, rn in zip(ts.nodes(), rts.nodes()):
+            n.population = fwd_map[n.population]
+            assert n == rn
+
+        assert ts.num_migrations == rts.num_migrations
+        for m, rm in zip(ts.migrations(), rts.migrations()):
+            m.source = fwd_map[m.source]
+            m.dest = fwd_map[m.dest]
+            assert m == rm
+
+        assert ts.num_mutations == rts.num_mutations
+        for m, rm in zip(ts.mutations(), rts.mutations()):
+            md = m.metadata
+            rmd = rm.metadata
+            assert len(md['mutation_list']) == len(rmd['mutation_list'])
+            for x, y in zip(md['mutation_list'], rmd['mutation_list']):
+                x['subpopulation'] = fwd_map[x['subpopulation']]
+                assert x == y
+
+        assert ts.num_individuals == rts.num_individuals
+        for i, ri in zip(ts.individuals(), rts.individuals()):
+            md = i.metadata
+            rmd = ri.metadata
+            md['subpopulation'] = fwd_map[md['subpopulation']]
+            assert md == rmd
+
+
     def test_remapping_errors(self, helper_functions, tmp_path):
-        d = msprime.Demography()
-        d.add_population(initial_size=10, name="p0")
-        d.add_population(initial_size=10, name="p1")
-        d.add_population(initial_size=10, name="A")
-        d.add_population_split(time=1.0, derived=["p0", "p1"], ancestral="A")
-        ts = msprime.sim_ancestry(
-                {"p0": 5, "p1": 5},
-                demography=d,
-                sequence_length=100,
-                random_seed=455,
-        )
+        ts = msprime.sim_ancestry(5, population_size=10, sequence_length=100, random_seed=455)
         ts = pyslim.annotate(ts, model_type='nonWF', tick=1, stage="late")
-        # test must refer to all subpopulations
-        with pytest.raises(RuntimeError, match='subpopulation id 2 is used.*but is not remapped'):
-            _ = helper_functions.run_slim_restart(
-                    ts,
-                    "restart_nonWF.slim",
-                    tmp_path,
-                    WF=False,
-                    subpop_map = {
-                        "p0" : 0,
-                        "p1" : 1,
-                    }
-            )
         # test can't map the same subpop to two different pops
-        with pytest.raises(RuntimeError, match='subpopMap value .0. is not unique'):
-            _ = helper_functions.run_slim_restart(
-                    ts,
-                    "restart_nonWF.slim",
-                    tmp_path,
-                    WF=False,
-                    subpop_map = {
-                        "p0" : 0,
-                        "p1" : 0,
-                        "p2" : 1,
-                        "p3" : 2,
-                    }
-            )
-        # test errors if it refers to non-existing subpop
         with pytest.raises(RuntimeError):
             _ = helper_functions.run_slim_restart(
                     ts,
-                    "restart_nonWF.slim",
+                    "restart_WF.slim",
                     tmp_path,
-                    WF=False,
+                    WF=True,
                     subpop_map = {
                         "p0" : 0,
-                        "p1" : 1,
-                        "p2" : 2,
-                        "p3" : 3,
+                        "p1" : 0,
                     }
             )
 
-    def test_remapping_empty_pops(self, helper_functions, tmp_path):
-        # test that subpop_map doesn't need to explicitly refer to empty pops
-        d = msprime.Demography()
-        d.add_population(initial_size=10, name="p0")
-        d.add_population(initial_size=10, name="p1")
-        d.add_population(initial_size=10, name="p2") # unused
-        d.add_population(initial_size=10, name="A")
-        d.add_population_split(time=1.0, derived=["p0", "p1"], ancestral="A")
-        ts = msprime.sim_ancestry(
-                {"p0": 5, "p1": 5},
-                demography=d,
-                sequence_length=100,
-                random_seed=456,
-        )
-        ts = pyslim.annotate(ts, model_type='nonWF', tick=1, stage="late")
-        t = ts.dump_tables()
-        r = t.populations[2].replace(metadata=None)
-        # make both pop 2 and 4 empty
-        t.populations[2] = r
-        t.populations.append(r)
-        ts = t.tree_sequence()
-        for subpop_map in (
-                {"p0" : 0, "p1" : 1, "p2" : 2, "p3" : 3, "p4" : 4},
-                    {"p0" : 0, "p1" : 1, "p3": 3},
-                ):
-            rts = helper_functions.run_slim_restart(
-                    ts,
-                    "restart_nonWF.slim",
-                    tmp_path,
-                    WF=False,
-                    subpop_map = subpop_map
-            )
-            self.verify_remapping(ts, rts, subpop_map)
-
     def test_remapping(self, helper_functions, tmp_path):
         d = msprime.Demography()
         # pop 0
         d.add_population(initial_size=10, name="A", extra_metadata={"pi": 3.1415})
         # pop 1
         md = pyslim.default_slim_metadata('population')
         del md['name']
@@ -762,16 +593,14 @@
         md['migration_records'] = [
             {
                 "migration_rate" : 0.9,
                 "source_subpop" : 1,
             }
         ]
         d.add_population(initial_size=10, name="D", extra_metadata=md)
-        # pop 4
-        d.add_population(initial_size=10, name="XYZ", extra_metadata={"abc": 5123})
         d.add_population_split(time=1.0, derived=["pop_1", "D"], ancestral="A")
         ts = msprime.sim_ancestry(
                 samples={"pop_1": 5, "D": 5},
                 demography=d,
                 sequence_length=100,
                 random_seed=455
         )
@@ -781,59 +610,32 @@
                 rate=1e-2,
                 random_seed=9,
                 model=msprime.SLiMMutationModel(type=1),
         )
         assert ts.num_mutations > 0
         for subpop_map in (
                 None,
-                {"p0" : 0, "p1" : 1, "p2" : 2, "p3" : 3, "p4" : 4},
-                {"p0" : 1, "p1" : 0, "p2" : 2, "p3" : 3, "p4" : 4},
-                {"p5" : 0, "p0" : 1, "p7" : 2, "p2" : 3, "p9" : 4},
+                {"p0" : 0, "p1" : 1, "p2" : 2, "p3" : 3},
+                {"p0" : 1, "p1" : 0, "p2" : 2, "p3" : 3},
+                {"p5" : 0, "p0" : 1, "p7" : 2, "p2" : 3},
         ):
             rts = helper_functions.run_slim_restart(
                     ts,
                     "restart_WF.slim",
                     tmp_path,
                     WF=True,
                     subpop_map = subpop_map,
             )
             self.verify_remapping(ts, rts, subpop_map)
 
-    @pytest.mark.skip(reason="migration table not supported by simplify")
-    def test_remaps_migration_table(self, helper_functions, tmp_path):
-        d = msprime.Demography()
-        d.add_population(initial_size=10, name="p0")
-        d.add_population(initial_size=10, name="p1")
-        d.add_population(initial_size=10, name="A")
-        d.add_population_split(time=1.0, derived=["p0", "p1"], ancestral="A")
-        d.set_migration_rate(0, 1, 0.1)
-        d.set_migration_rate(1, 0, 0.1)
-        ts = msprime.sim_ancestry(
-                {"p0": 5, "p1": 5},
-                demography=d,
-                sequence_length=100,
-                random_seed=455,
-                record_migrations=True
-        )
-        ts = pyslim.annotate(ts, model_type='WF', tick=1, stage="late")
-        assert ts.num_migrations > 0
-        rts = helper_functions.run_slim_restart(
-                ts,
-                "restart_WF.slim",
-                tmp_path,
-                WF=True,
-                subpop_map = {"p5" : 0, "p2" : 1, "p0" : 2 },
-        )
-        self.verify_remapping(ts, rts, subpop_map)
-
     @pytest.mark.parametrize(
         'restart_name, recipe', restarted_recipe_eq("remove_subpop"), indirect=["recipe"])
     def test_keep_slim_names(self, restart_name, recipe, helper_functions, tmp_path):
-        # test that SLiM retains names of SLiM populations
-        # even when those populations are removed
+        # test that SLiM retains names of SLim populations
+        # even when those are removed
         in_ts = recipe["ts"]
         # this recipe moves everyone to subpop 0
         out_ts = helper_functions.run_slim_restart(in_ts, restart_name, tmp_path)
         for n in out_ts.samples(time=0):
             assert out_ts.node(n).population == 0
         for j in range(1, in_ts.num_populations):
             in_md = in_ts.population(j).metadata
```

### Comparing `pyslim-1.0.2/tests/test_metadata.py` & `pyslim-1.0b1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_provenance.py` & `pyslim-1.0b1/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/make_v3_test_additions.py` & `pyslim-1.0b1/tests/test_recipes/make_v3_test_additions.py`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/make_v3_tests.sh` & `pyslim-1.0b1/tests/test_recipes/make_v3_tests.sh`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_WF_early.slim`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T);
+    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
+    defineConstant("K", 10);
 }
 
-1 early() { 
+1 early() {
     sim.addSubpop("p1", 10);
+    for (ind in p1.individuals)
+        ind.setSpatialPosition(p1.pointUniform());
 }
 
-10 late() {
+early() {
+    sim.treeSeqRememberIndividuals(p1.individuals);
+}
+
+10 early() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.0.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.0.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.2.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.2.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.3.1.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.3.1.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.4.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.4.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.5.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.5.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.5_and_v3.6.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.5_and_v3.6.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.6.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.6.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF.v3.7.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.v3.7.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_early_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_WF_early_early.slim`

 * *Files 15% similar despite different names*

```diff
@@ -19,49 +19,37 @@
 10 early() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_early_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nucleotides_nonWF.slim`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-initialize()
-{
+initialize() {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T);
+	defineConstant("L", 1e2);
+    initializeSLiMModelType("nonWF");
+	initializeSLiMOptions(keepPedigrees=T, nucleotideBased=T);
     initializeTreeSeq();
-    initializeMutationRate(1e-2);
-    initializeMutationType("m1", 0.5, "f", -0.1);
-    initializeGenomicElementType("g1", m1, 1.0);
-    initializeGenomicElement(g1, 0, 99);
-    initializeRecombinationRate(1e-2);
+	initializeAncestralNucleotides(randomNucleotides(L));
+	initializeMutationTypeNuc("m1", 0.5, "f", 0.0);
+	initializeGenomicElementType("g1", m1, 1.0, mmJukesCantor(4e-2));
+	initializeGenomicElement(g1, 0, L-1);
+	initializeRecombinationRate(1e-2);
+    defineConstant("K", 10);
 }
 
-1 early() { 
-    sim.addSubpop("p1", 10);
+reproduction() {
+    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
 }
 
-10 first() {
+1 early() {
+	sim.addSubpop("p1", 10);
+}
+
+early() {
+    p1.fitnessScaling = K / p1.individualCount;
+}
+
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
+
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_early_late.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_WF.slim`

 * *Files 16% similar despite different names*

```diff
@@ -19,49 +19,37 @@
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_first_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_WF_late.slim`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T);
+    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
+    defineConstant("K", 10);
 }
 
-1 first() { 
+1 early() {
     sim.addSubpop("p1", 10);
+    for (ind in p1.individuals) {
+        ind.setSpatialPosition(p1.pointUniform());
+    }
+    // it will help to record the first-gen ones that die as well
+    sim.treeSeqRememberIndividuals(p1.individuals);
+}
+
+late() {
+    sim.treeSeqRememberIndividuals(p1.individuals);
 }
 
-10 early() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_first_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nucleotides_WF.slim`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,57 @@
-initialize()
-{
+// Based on Example 18.1
+
+initialize() {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T);
+	defineConstant("L", 1e2);
+	initializeSLiMOptions(keepPedigrees=T, nucleotideBased=T);
     initializeTreeSeq();
-    initializeMutationRate(1e-2);
-    initializeMutationType("m1", 0.5, "f", -0.1);
-    initializeGenomicElementType("g1", m1, 1.0);
-    initializeGenomicElement(g1, 0, 99);
-    initializeRecombinationRate(1e-2);
+	initializeAncestralNucleotides(randomNucleotides(L));
+	initializeMutationTypeNuc("m1", 0.5, "f", 0.0);
+	initializeGenomicElementType("g1", m1, 1.0, mmJukesCantor(4e-2));
+	initializeGenomicElement(g1, 0, L-1);
+	initializeRecombinationRate(1e-2);
 }
 
-1 first() { 
-    sim.addSubpop("p1", 10);
+1 early() {
+	sim.addSubpop("p1", 10);
 }
 
-10 first() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_first_late.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_remember_and_retain.slim`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T);
+    initializeSLiMModelType("nonWF");
+    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
+    defineConstant("K", 10);
 }
 
-1 first() { 
+reproduction() {
+    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
+}
+
+1 early() {
     sim.addSubpop("p1", 10);
+    for (ind in p1.individuals)
+        ind.setSpatialPosition(p1.pointUniform());
+}
+
+early() {
+    p1.fitnessScaling = K / p1.individualCount;
+}
+
+late() {
+    // alternate remembering and retaining
+    sim.treeSeqRememberIndividuals(p1.individuals, permanent=(sim.cycle % 2 == 0));
 }
 
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_late_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_roots.slim`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,55 @@
-initialize()
-{
+initialize() {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
+    defineConstant("chromosome_length", 249250);
     initializeSLiMOptions(keepPedigrees=T);
     initializeTreeSeq();
-    initializeMutationRate(1e-2);
-    initializeMutationType("m1", 0.5, "f", -0.1);
+    initializeMutationRate(0);
+    initializeMutationType("m1", 0.5, "f", 0);
     initializeGenomicElementType("g1", m1, 1.0);
-    initializeGenomicElement(g1, 0, 99);
-    initializeRecombinationRate(1e-2);
+    initializeGenomicElement(g1, 0, chromosome_length-1);
+    initializeRecombinationRate(1e-8);
 }
 
-1 late() { 
-    sim.addSubpop("p1", 10);
+1 early() {
+    sim.addSubpop('p1', 1000);
 }
 
-10 early() {
+100 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_late_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_retain_everyone_WF_late.slim`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T);
+    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
+    defineConstant("K", 10);
 }
 
-1 late() { 
+1 early() {
     sim.addSubpop("p1", 10);
+    for (ind in p1.individuals) {
+        ind.setSpatialPosition(p1.pointUniform());
+    }
+    // it will help to record the first-gen ones that die as well
+    sim.treeSeqRememberIndividuals(p1.individuals, permanent=F);
+}
+
+late() {
+    sim.treeSeqRememberIndividuals(p1.individuals, permanent=F);
 }
 
-10 first() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_late_late.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_retain_everyone_nonWF_late.slim`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T);
+    initializeSLiMModelType("nonWF");
+    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
+    defineConstant("K", 10);
 }
 
-1 late() { 
+reproduction() {
+    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
+}
+
+1 early() {
     sim.addSubpop("p1", 10);
+    for (ind in p1.individuals)
+        ind.setSpatialPosition(p1.pointUniform());
+}
+
+early() {
+    p1.fitnessScaling = K / p1.individualCount;
+}
+
+late() {
+    sim.treeSeqRememberIndividuals(p1.individuals, permanent=F);
 }
 
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_WF_migration.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_WF_migration.slim`

 * *Files 12% similar despite different names*

```diff
@@ -22,49 +22,37 @@
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_init_mutated_WF.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_init_mutated_WF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_init_mutated_nonWF.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_init_mutated_nonWF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_long_nonWF.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_long_nonWF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_long_nucleotides.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_long_nucleotides.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_mutation_spectrum.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_mutation_spectrum.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_nonWF_late.slim`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
     initializeSLiMModelType("nonWF");
-    initializeSLiMOptions(keepPedigrees=T);
+    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
     defineConstant("K", 10);
@@ -16,62 +16,56 @@
 
 reproduction() {
     subpop.addCrossed(individual, subpop.sampleIndividuals(1));
 }
 
 1 early() {
     sim.addSubpop("p1", 10);
+    for (ind in p1.individuals)
+        ind.setSpatialPosition(p1.pointUniform());
 }
 
 early() {
     p1.fitnessScaling = K / p1.individualCount;
 }
 
+late() {
+    sim.treeSeqRememberIndividuals(p1.individuals);
+}
+
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.0.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.0.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.2.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.2.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.3.1.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.3.1.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.4.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.4.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.5.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.5.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.6.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.6.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF.v3.7.trees` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.v3.7.trees`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_early_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_retain_sometimes_WF_late.slim`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,70 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMModelType("nonWF");
-    initializeSLiMOptions(keepPedigrees=T);
+    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
     defineConstant("K", 10);
 }
 
-reproduction() {
-    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
-}
-
 1 early() {
     sim.addSubpop("p1", 10);
+    for (ind in p1.individuals) {
+        ind.setSpatialPosition(p1.pointUniform());
+    }
+    // it will help to record the first-gen ones that die as well
+    sim.treeSeqRememberIndividuals(p1.individuals, permanent=F);
 }
 
-early() {
-    p1.fitnessScaling = K / p1.individualCount;
+late() {
+    if (runif(1) < 0.7) {
+      inds = sample(p1.individuals, min(p1.individualCount, 3));
+      sim.treeSeqRememberIndividuals(inds, permanent=F);
+      inds = sample(p1.individuals, min(p1.individualCount, 3));
+      sim.treeSeqRememberIndividuals(inds, permanent=T);
+    }
 }
 
-10 early() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_early_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_WF_late_late.slim`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,55 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMModelType("nonWF");
     initializeSLiMOptions(keepPedigrees=T);
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
-    defineConstant("K", 10);
 }
 
-reproduction() {
-    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
-}
-
-1 early() {
+1 late() { 
     sim.addSubpop("p1", 10);
 }
 
-early() {
-    p1.fitnessScaling = K / p1.individualCount;
-}
-
-10 first() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 late() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_early_late.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_WF_late_early.slim`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,55 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMModelType("nonWF");
     initializeSLiMOptions(keepPedigrees=T);
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
-    defineConstant("K", 10);
 }
 
-reproduction() {
-    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
-}
-
-1 early() {
+1 late() { 
     sim.addSubpop("p1", 10);
 }
 
-early() {
-    p1.fitnessScaling = K / p1.individualCount;
-}
-
-10 late() {
+10 early() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_first_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF_late_late.slim`

 * *Files 25% similar despite different names*

```diff
@@ -14,64 +14,52 @@
     defineConstant("K", 10);
 }
 
 reproduction() {
     subpop.addCrossed(individual, subpop.sampleIndividuals(1));
 }
 
-1 first() {
+1 late() {
     sim.addSubpop("p1", 10);
 }
 
-early() {
+2: early() {
     p1.fitnessScaling = K / p1.individualCount;
 }
 
-10 early() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_first_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF.slim`

 * *Files 27% similar despite different names*

```diff
@@ -14,64 +14,52 @@
     defineConstant("K", 10);
 }
 
 reproduction() {
     subpop.addCrossed(individual, subpop.sampleIndividuals(1));
 }
 
-1 first() {
+1 early() {
     sim.addSubpop("p1", 10);
 }
 
 early() {
     p1.fitnessScaling = K / p1.individualCount;
 }
 
-10 first() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_first_late.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF_early_late.slim`

 * *Files 26% similar despite different names*

```diff
@@ -14,64 +14,52 @@
     defineConstant("K", 10);
 }
 
 reproduction() {
     subpop.addCrossed(individual, subpop.sampleIndividuals(1));
 }
 
-1 first() {
+1 early() {
     sim.addSubpop("p1", 10);
 }
 
 early() {
     p1.fitnessScaling = K / p1.individualCount;
 }
 
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_late_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF_early_early.slim`

 * *Files 18% similar despite different names*

```diff
@@ -14,64 +14,52 @@
     defineConstant("K", 10);
 }
 
 reproduction() {
     subpop.addCrossed(individual, subpop.sampleIndividuals(1));
 }
 
-1 late() {
+1 early() {
     sim.addSubpop("p1", 10);
 }
 
-2: early() {
+early() {
     p1.fitnessScaling = K / p1.individualCount;
 }
 
 10 early() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_late_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF_late_early.slim`

 * *Files 23% similar despite different names*

```diff
@@ -22,56 +22,44 @@
     sim.addSubpop("p1", 10);
 }
 
 2: early() {
     p1.fitnessScaling = K / p1.individualCount;
 }
 
-10 first() {
+10 early() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_nonstacked.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF_nonstacked.slim`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 initialize()
 {
     setSeed(24);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
+    if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
     initializeSLiMModelType("nonWF");
     initializeSLiMOptions(keepPedigrees=T);
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     m1.mutationStackPolicy = "l";
     initializeGenomicElementType("g1", m1, 1.0);
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_nonWF_selfing.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nucleotides_plus_others.slim`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,63 @@
-initialize()
-{
+// Based on Example 18.1
+
+initialize() {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMModelType("nonWF");
-    initializeSLiMOptions(keepPedigrees=T);
+	defineConstant("L", 1e2);
+	initializeSLiMOptions(keepPedigrees=T, nucleotideBased=T);
     initializeTreeSeq();
-    initializeMutationRate(1e-2);
-    initializeMutationType("m1", 0.5, "f", -0.1);
-    initializeGenomicElementType("g1", m1, 1.0);
-    initializeGenomicElement(g1, 0, 99);
-    initializeRecombinationRate(1e-2);
-    defineConstant("K", 10);
-}
-
-reproduction() {
-    if (runif(1) < 0.25) {
-        mate = subpop.sampleIndividuals(1);
-    } else {
-        mate = individual;
-    }
-    for (_ in seqLen(rpois(1, 2))) {
-      subpop.addCrossed(individual, mate);
-    }
+	initializeAncestralNucleotides(randomNucleotides(L));
+	initializeMutationTypeNuc("m1", 0.5, "f", 0.0);
+	initializeMutationType("m2", 0.5, "n", 0.0, 0.1);
+	initializeGenomicElementType("g1", m1, 1.0, mmJukesCantor(4e-2));
+	initializeGenomicElement(g1, 0, L-1);
+	initializeRecombinationRate(1e-2);
 }
 
 1 early() {
-    sim.addSubpop("p1", 10);
+	sim.addSubpop("p1", 10);
 }
 
-early() {
-    p1.fitnessScaling = K / p1.individualCount;
+1: late() {
+    // add *non-nucleotide* mutations also
+    sample(p1.genomes, 10).addNewDrawnMutation(m2, rdunif(10, 0, L-1));
 }
 
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_WF_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_nonWF_selfing.slim`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
+    initializeSLiMModelType("nonWF");
+    initializeSLiMOptions(keepPedigrees=T);
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
     defineConstant("K", 10);
 }
 
+reproduction() {
+    if (runif(1) < 0.25) {
+        mate = subpop.sampleIndividuals(1);
+    } else {
+        mate = individual;
+    }
+    for (_ in seqLen(rpois(1, 2))) {
+      subpop.addCrossed(individual, mate);
+    }
+}
+
 1 early() {
     sim.addSubpop("p1", 10);
-    for (ind in p1.individuals)
-        ind.setSpatialPosition(p1.pointUniform());
 }
 
 early() {
-    sim.treeSeqRememberIndividuals(p1.individuals);
+    p1.fitnessScaling = K / p1.individualCount;
 }
 
-10 early() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_WF_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_record_everyone_nonWF_early.slim`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
+    initializeSLiMModelType("nonWF");
     initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
     defineConstant("K", 10);
 }
 
-1 first() {
+reproduction() {
+    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
+}
+
+1 early() {
     sim.addSubpop("p1", 10);
     for (ind in p1.individuals)
         ind.setSpatialPosition(p1.pointUniform());
 }
 
-1: first() {
+early() {
+    p1.fitnessScaling = K / p1.individualCount;
+}
+
+early() {
     sim.treeSeqRememberIndividuals(p1.individuals);
 }
 
-10 first() {
+10 early() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_nonWF_early.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_retain_unary_WF_late.slim`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,70 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMModelType("nonWF");
     initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
-    initializeTreeSeq();
+    initializeTreeSeq(retainCoalescentOnly=F);
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
     defineConstant("K", 10);
 }
 
-reproduction() {
-    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
-}
-
 1 early() {
     sim.addSubpop("p1", 10);
-    for (ind in p1.individuals)
+    for (ind in p1.individuals) {
         ind.setSpatialPosition(p1.pointUniform());
+    }
+    // it will help to record the first-gen ones that die as well
+    sim.treeSeqRememberIndividuals(p1.individuals, permanent=F);
 }
 
-early() {
-    p1.fitnessScaling = K / p1.individualCount;
-}
-
-early() {
-    sim.treeSeqRememberIndividuals(p1.individuals);
+late() {
+    if (runif(1) < 0.7) {
+      inds = sample(p1.individuals, min(p1.individualCount, 3));
+      sim.treeSeqRememberIndividuals(inds, permanent=F);
+      inds = sample(p1.individuals, min(p1.individualCount, 3));
+      sim.treeSeqRememberIndividuals(inds, permanent=T);
+    }
 }
 
-10 early() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_nonWF_first.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_retain_unary_nonWF_late.slim`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
     initializeSLiMModelType("nonWF");
     initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
-    initializeTreeSeq();
+    initializeTreeSeq(retainCoalescentOnly=F);
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
     defineConstant("K", 10);
 }
@@ -24,60 +24,53 @@
         ind.setSpatialPosition(p1.pointUniform());
 }
 
 early() {
     p1.fitnessScaling = K / p1.individualCount;
 }
 
-2: first() {
-    sim.treeSeqRememberIndividuals(p1.individuals);
+late() {
+    if (runif(1) < 0.7) {
+      inds = sample(p1.individuals, min(p1.individualCount, 3));
+      sim.treeSeqRememberIndividuals(inds, permanent=F);
+      inds = sample(p1.individuals, min(p1.individualCount, 3));
+      sim.treeSeqRememberIndividuals(inds, permanent=T);
+    }
 }
 
-10 first() {
+10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_record_everyone_nonWF_late.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_WF_early_late.slim`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,55 @@
 initialize()
 {
     setSeed(23);
     if (!exists("TREES_FILE")) defineGlobal("TREES_FILE", "out.trees"); 
     if (!exists("PEDIGREE_FILE")) defineGlobal("PEDIGREE_FILE", "out.pedigree"); 
-    initializeSLiMModelType("nonWF");
-    initializeSLiMOptions(keepPedigrees=T, dimensionality="xy");
+    initializeSLiMOptions(keepPedigrees=T);
     initializeTreeSeq();
     initializeMutationRate(1e-2);
     initializeMutationType("m1", 0.5, "f", -0.1);
     initializeGenomicElementType("g1", m1, 1.0);
     initializeGenomicElement(g1, 0, 99);
     initializeRecombinationRate(1e-2);
-    defineConstant("K", 10);
 }
 
-reproduction() {
-    subpop.addCrossed(individual, subpop.sampleIndividuals(1));
-}
-
-1 early() {
+1 early() { 
     sim.addSubpop("p1", 10);
-    for (ind in p1.individuals)
-        ind.setSpatialPosition(p1.pointUniform());
-}
-
-early() {
-    p1.fitnessScaling = K / p1.individualCount;
-}
-
-late() {
-    sim.treeSeqRememberIndividuals(p1.individuals);
 }
 
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 late() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_retain_sometimes_nonWF_late.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_retain_sometimes_nonWF_late.slim`

 * *Files 25% similar despite different names*

```diff
@@ -40,49 +40,37 @@
 10 late() {
     sim.treeSeqOutput(TREES_FILE);
     catn("Done.");
     sim.simulationFinished();
 }
 
 // PEDIGREE OUTPUT
-1 first() {
+1 early() {
     writeFile(PEDIGREE_FILE,
        paste(c("generation", "stage", "individual", "age", "parent1", "parent2"),
              sep="\t"));
 }
 
-1: first() {
-    for (pop in sim.subpopulations) {
-        for (ind in pop.individuals) {
-            age = community.modelType == "nonWF" ? ind.age else -1;
-            writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
-                   sep='\t'),
-             append=T);
-        }
-    }
-}
-
 1: early() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'early', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
 
 1: late() {
     for (pop in sim.subpopulations) {
         for (ind in pop.individuals) {
             age = community.modelType == "nonWF" ? ind.age else -1;
             writeFile(PEDIGREE_FILE,
-             paste(c(sim.cycle, community.cycleStage, ind.pedigreeID, age, ind.pedigreeParentIDs),
+             paste(c(sim.cycle, 'late', ind.pedigreeID, age, ind.pedigreeParentIDs),
                    sep='\t'),
              append=T);
         }
     }
 }
```

### Comparing `pyslim-1.0.2/tests/test_recipes/recipe_with_metadata.slim` & `pyslim-1.0b1/tests/test_recipes/recipe_with_metadata.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_WF.slim` & `pyslim-1.0b1/tests/test_recipes/restart_WF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_and_remove_subpop_nonWF.slim` & `pyslim-1.0b1/tests/test_recipes/restart_and_remove_subpop_nonWF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_and_run_WF.slim` & `pyslim-1.0b1/tests/test_recipes/restart_and_run_WF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_and_run_nonWF.slim` & `pyslim-1.0b1/tests/test_recipes/restart_and_run_nonWF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_msprime.slim` & `pyslim-1.0b1/tests/test_recipes/restart_msprime.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_nonWF.slim` & `pyslim-1.0b1/tests/test_recipes/restart_nonWF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_nucleotides_WF.slim` & `pyslim-1.0b1/tests/test_recipes/restart_nucleotides_WF.slim`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     // as well as any bespoke TREES_FILE for output, you need to define:
     //  TREES_IN = path to trees to initialise
 	defineConstant("L", 1e2);
 	initializeSLiMOptions(keepPedigrees=T, nucleotideBased=T);
     initializeTreeSeq();
 	initializeAncestralNucleotides(paste0(rep("A", L)));
 	initializeMutationTypeNuc("m1", 0.5, "f", 0.0);
-    initializeMutationTypeNuc("m2", 0.5, "n", 0.0, 0.1);
 	initializeGenomicElementType("g1", m1, 1.0, mmJukesCantor(4e-2));
 	initializeGenomicElement(g1, 0, L-1);
 	initializeRecombinationRate(1e-2);
 	if (!exists("SUBPOP_MAP")) defineConstant("SUBPOP_MAP", NULL);
 }
 
 1 late() {
```

### Comparing `pyslim-1.0.2/tests/test_recipes/restart_nucleotides_nonWF.slim` & `pyslim-1.0b1/tests/test_recipes/restart_nucleotides_nonWF.slim`

 * *Files identical despite different names*

### Comparing `pyslim-1.0.2/tests/test_spatial.py` & `pyslim-1.0b1/tests/test_spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test cases for tree sequences.
 """
+import pickle
 import random
 import os
 
 import numpy as np
 import pytest
 import tskit
 import msprime
@@ -36,16 +37,16 @@
         # Initialize array to store popoluationsize
         nxbins = len(x_breaks) - 1
         nybins = len(y_breaks) - 1
         ntbins = len(time_breaks) - 1
         popsize = np.empty((nxbins, nybins, ntbins))
 
         # Location, times, and ages of individuals
-        locations = ts.individuals_location
-        times = ts.individuals_times
+        locations = pyslim.individual_locations(ts)
+        times = pyslim.individual_times(ts)
 
         # Iterate through location bins and time bins
         for i in np.arange(nxbins):
             for j in np.arange(nybins):
                 # Endpoints of bins
                 x0, x1 = x_breaks[i], x_breaks[i + 1]
                 y0, y1 = y_breaks[j], y_breaks[j + 1]
@@ -58,22 +59,21 @@
                             ind = ts.individual(ind_id)
                             if (ind.location[0] < x1 and ind.location[0] >= x0 and ind.location[1] < y1 and ind.location[1] >= y0):
                                 alive += 1/(t1-t0)
                     popsize[i, j, k] = alive     
         return(popsize)
 
     def make_bins(self, ts):
-        locs = ts.individuals_location
-        max_time = max(ts.individuals_time)
+        locs = pyslim.individual_locations(ts)
         for nx in np.arange(1, 20, 10):
             for ny in np.arange(1, 20, 10):
                 for nt in np.arange(1, 60, 30):
                     yield [np.linspace(0, round(max(locs[:,0])), nx + 1), 
                            np.linspace(0, round(max(locs[:,1])), ny + 1),
-                           np.round(np.linspace(0, max(nt, max_time), nt + 1))]  
+                           np.round(np.linspace(0, max(nt, max(pyslim.individual_times(ts))), nt + 1))]  
 
     def verify(self, ts, remembered_stage):
         for bins in self.make_bins(ts):
             for stage in ('early', 'late'):
                 x_bins, y_bins, time_bins = bins
                 # as computed by pyslim
                 popsize0 = pyslim.population_size(ts, x_bins, y_bins, time_bins, stage=stage, remembered_stage=remembered_stage)
```

### Comparing `pyslim-1.0.2/tests/test_tree_sequence.py` & `pyslim-1.0b1/tests/test_tree_sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test cases for tree sequences.
 """
+import pickle
 import random
 import numpy as np
 import os
 
 import pytest
 import tskit
 import msprime
@@ -27,65 +28,14 @@
         # the mutations in "init_mutated" examples have mutations that are *added*
         # in *early*, and so their times match in that stage.
         else:
             for mut in ts.mutations():
                 mut_time = max([x['slim_time'] for x in mut.metadata['mutation_list']])
                 assert mut_time == pyslim.slim_time(ts, mut.time, stage="early")
 
-class TestNextMutationID(tests.PyslimTestCase):
-    '''
-    Tests for the function that returns the largest SLiM mutation ID.
-    '''
-    def test_next_id(self, recipe):
-        ts = recipe["ts"]
-        mt_ids_str = ','.join(tskit.unpack_strings(ts.tables.mutations.derived_state, ts.tables.mutations.derived_state_offset))
-        mt_ids = [int(i or 0) for i in mt_ids_str.split(',')]
-        max_mt_id = max(mt_ids)
-        assert max_mt_id + 1 == pyslim.next_slim_mutation_id(ts)
-
-    @pytest.mark.parametrize('recipe', recipe_eq("adds_mutations"), indirect=True)
-    def test_reload_slim(self, recipe, helper_functions, tmp_path):
-        ts = recipe["ts"]
-        rts = self.do_recapitate(
-                    ts,
-                    recombination_rate=1e-8,
-                    ancestral_Ne=100,
-                    random_seed=875,
-        )
-        next_id = pyslim.next_slim_mutation_id(rts)
-        mts = msprime.sim_mutations(
-                rts,
-                rate=1e-4,
-                keep=True,
-                model=msprime.SLiMMutationModel(type=1, next_id=next_id),
-        )
-        assert mts.num_mutations > rts.num_mutations
-        rrts = helper_functions.run_slim_restart(
-                mts,
-                "restart_nucleotides_WF.slim",
-                tmp_path,
-                WF=False,
-        )
-        # nothing should change
-        assert pyslim.next_slim_mutation_id(mts) == pyslim.next_slim_mutation_id(rrts)
-        assert rrts.num_mutations == mts.num_mutations
-
-        def test_invalid_derived_state(self):
-            ts = msprime.sim_ancestry(
-                    4,
-                    sequence_length=10,
-                    population_size=10,
-                    random_seed=10,
-            )
-            mts = msprime.sim_mutations(ts,
-                    model="jc69",
-                    rate=0.5,
-                    random_seed=23)
-            with pytest.raises(ValueError, match="need to be coercible to int"):
-                pyslim.next_slim_mutation_id(mts)
 
 class TestRecapitate(tests.PyslimTestCase):
     '''
     Tests for recapitation.
     '''
 
     def check_recap_consistency(self, ts, recap):
@@ -138,26 +88,16 @@
                         ts,
                         recombination_rate=0.0,
                         demography=msprime.Demography.from_tree_sequence(ts),
                         ancestral_Ne=10,
                         random_seed=123,
             )
 
-    def test_root_mismatch_error(self):
-        ts = msprime.sim_ancestry(4, sequence_length=10, random_seed=12)
-        recap_time = 100
-        ts = pyslim.annotate(ts, model_type="nonWF", tick=recap_time)
-        assert ts.node(ts.first().roots[0]).time < recap_time
-        with pytest.raises(ValueError, match="at the time expected by recapitate"):
-            rts = self.do_recapitate(ts, ancestral_Ne=10)
-
     def test_unique_names(self):
-        ts = msprime.sim_ancestry(4, sequence_length=10, random_seed=12, end_time=1.0)
-        # adjust seed if not
-        assert min([t.num_roots for t in ts.trees()]) > 1
+        ts = msprime.sim_ancestry(4, sequence_length=10, random_seed=12)
         ts = pyslim.annotate(ts, model_type="nonWF", tick=1)
         t = ts.dump_tables()
         md = t.populations[0].metadata
         md.update({"name": "ancestral"})
         t.populations[0] = t.populations[0].replace(metadata=md)
         md.update({"name": "ancestral_ancestral", "slim_id": 1})
         t.populations.add_row(metadata=md)
@@ -233,29 +173,44 @@
     @pytest.mark.parametrize('recipe', recipe_eq(exclude="long"), indirect=True)
     def test_first_gen_nodes(self, recipe):
         # check that all the roots of the trees are present
         # (note this will fail if some populations were started at different
         # times than others)
         ts = recipe["ts"]
         root_time = ts.metadata['SLiM']['tick']
-        is_wf = (ts.metadata['SLiM']['model_type'] == 'WF')
-        remembered_stage = ts.metadata['SLiM']['stage']
-        if (not is_wf) or (remembered_stage != 'late'):
+        if (ts.metadata['SLiM']['stage'] == 'early'
+                or ts.metadata['SLiM']['model_type'] == 'nonWF'):
             root_time -= 1
-        if (not is_wf) and ("begun_first" in recipe):
-            root_time += 1
-        if (not is_wf) and ("remembered_first" in recipe):
-            root_time -= 1
-        if is_wf and ("begun_late" in recipe):
+        if (ts.metadata['SLiM']['model_type'] == 'WF' and "begun_late" in recipe):
             root_time -= 1
         for t in ts.trees():
             for u in t.roots:
                 assert ts.node(u).time == root_time
 
 
+class TestMutationMetadata(tests.PyslimTestCase):
+    '''
+    Tests for extra stuff related to Mutations.
+    '''
+
+    @pytest.mark.parametrize('recipe', recipe_eq(exclude=("init_mutated", "long")), indirect=True)
+    def test_slim_time(self, recipe):
+        ts = recipe["ts"]
+        # check that slim_times make sense, i.e., that
+        # slim_generation == (time + slim_time + (model_type == "WF" and stage="early"))
+        offset = (
+            (ts.metadata["SLiM"]["model_type"] == "WF")
+            and
+            (ts.metadata["SLiM"]["stage"] == "early")
+        )
+        for mut in ts.mutations():
+            mut_slim_time = max([u["slim_time"] for u in mut.metadata["mutation_list"]])
+            assert ts.metadata['SLiM']['tick'] == mut_slim_time + mut.time + offset
+
+
 class TestIndividualAges(tests.PyslimTestCase):
     # tests for individuals_alive_at and individual_ages_at
 
     @pytest.mark.parametrize('recipe', [next(recipe_eq("everyone"))], indirect=True)
     def test_errors(self, recipe):
         ts = recipe["ts"]
         for stage in ['abcd', 10, []]:
@@ -275,15 +230,15 @@
         else:
             with pytest.warns(UserWarning):
                 pyslim.individuals_alive_at(ts, 0, remembered_stage="early")
 
     @pytest.mark.parametrize('recipe', recipe_eq("multipop", exclude="remembered_early"), indirect=True)
     def test_population(self, recipe):
         ts = recipe["ts"]
-        individual_populations = ts.individuals_population
+        individual_populations = pyslim.individual_populations(ts)
         all_inds = pyslim.individuals_alive_at(ts, 0)
         assert len(all_inds) > 0
         for p in range(ts.num_populations):
             sub_inds = pyslim.individuals_alive_at(ts, 0, population=p)
             assert set(sub_inds) == set(all_inds[individual_populations == p])
             sub_inds = pyslim.individuals_alive_at(ts, 0, population=[p])
             assert set(sub_inds) == set(all_inds[individual_populations == p])
@@ -318,41 +273,31 @@
             if n.flags & tskit.NODE_IS_SAMPLE:
                 assert slim_id in sdict
 
     @pytest.mark.parametrize('recipe', recipe_eq("pedigree"), indirect=True)
     def test_ages(self, recipe):
         ts = recipe["ts"]
         info = recipe["info"]
-        remembered_stage = 'late'
-        if 'remembered_first' in recipe:
-            remembered_stage = 'first' 
-        elif 'remembered_early' in recipe:
-            remembered_stage = 'early' 
+        remembered_stage = 'early' if 'remembered_early' in recipe else 'late'
         assert remembered_stage == ts.metadata['SLiM']['stage']
         max_time_ago = ts.metadata['SLiM']['tick']
-        if remembered_stage in ('first', 'early'):
+        if remembered_stage == 'early':
             max_time_ago -= 1
         for time in range(0, max_time_ago):
-            slim_tick = ts.metadata['SLiM']['tick'] - time
-            check_stages = ('first', 'early', 'late')
-            if time == 0:
-                if remembered_stage == 'first':
-                    # if we remember in first we don't know who's still there
-                    # in later stages of that time step
-                    check_stages = ('first', )
-                elif remembered_stage == 'early':
-                    check_stages = ('first', 'early')
-            if time == max_time_ago:
-                if remembered_stage == 'early':
-                    # if we set up the population in early there aren't individuals in first
-                    # of the very first time step
-                    check_stages = ('early', 'late')
-                elif remembered_stage == 'late':
-                    # similarly for late
-                    check_stages = ('late', )
+            # if written out during 'early' in a WF model,
+            # tskit time 0 will be the SLiM time step *before* slim_generation
+            slim_time = ts.metadata['SLiM']['tick'] - time
+            if remembered_stage == 'early' and ts.metadata["SLiM"]["model_type"] == "WF":
+                slim_time -= 1
+            if remembered_stage == 'early' and time == 0:
+                # if we remember in early we don't know who's still there
+                # in late of the last time step
+                check_stages = ('early',)
+            else:
+                check_stages = ('early', 'late')
             for stage in check_stages:
                 alive = pyslim.individuals_alive_at(
                             ts,
                             time,
                             stage=stage,
                             remembered_stage=remembered_stage
                 )
@@ -360,41 +305,38 @@
                             ts,
                             time,
                             stage=stage,
                             remembered_stage=remembered_stage
                 )
                 for ind in ts.individuals():
                     ind_time = ts.node(ind.nodes[0]).time
-                    # bad things can happen for the very first individuals
-                    # depending on when the subpops are created
-                    if (('everyone' in recipe or ind_time == 0) and
-                            (remembered_stage == "early" or ind_time < max_time_ago)):
+                    if 'everyone' in recipe or ind_time == 0:
                         slim_id = ind.metadata["pedigree_id"]
                         assert slim_id in info
-                        slim_alive = (slim_tick, stage) in info[slim_id]['age']
+                        slim_alive = (slim_time, stage) in info[slim_id]['age']
                         pyslim_alive = ind.id in alive
                         assert slim_alive == pyslim_alive
                         if slim_alive:
-                            slim_age = info[slim_id]['age'][(slim_tick, stage)]
+                            slim_age = info[slim_id]['age'][(slim_time, stage)]
                             if ts.metadata["SLiM"]["model_type"] == "WF":
                                 # SLiM records -1 but we return 0 in late and 1 in early
-                                slim_age = 0 + (stage in ('first', 'early'))
+                                slim_age = 0 + (stage == 'early')
                             assert ages[ind.id] == slim_age
                         else:
                             assert np.isnan(ages[ind.id])
 
 
 class TestHasIndividualParents(tests.PyslimTestCase):
 
     def verify_has_parents(self, ts):
         right_answer = np.repeat(True, ts.num_individuals)
         node_indivs = ts.tables.nodes.individual
         parent_ids = [set() for _ in ts.individuals()]
         node_parent_ids = [set() for _ in ts.nodes()]
-        individual_times = ts.individuals_time
+        individual_times = pyslim.individual_times(ts)
         individual_ages = pyslim.individual_ages(ts)
         for t in ts.trees():
             for i in ts.individuals():
                 if len(i.nodes) != 2:
                     right_answer[i.id] = False
                 for n in i.nodes:
                     pn = t.parent(n)
@@ -435,54 +377,55 @@
         has_parents = pyslim.has_individual_parents(ts)
         right_parents = np.sort(np.array(right_parents), axis=0)
         parents = np.sort(pyslim.individual_parents(ts), axis=0)
         assert np.array_equal(right_answer, has_parents)
         assert np.array_equal(right_parents, parents)
 
     def get_first_gen(self, ts):
-        # root_time = ts.metadata["SLiM"]["tick"]
-        # if ts.metadata['SLiM']['model_type'] != 'WF' or ts.metadata['SLiM']['stage'] != 'late':
-        #     root_time -= 1
+        root_time = ts.metadata["SLiM"]["tick"]
+        if ts.metadata['SLiM']['model_type'] != 'WF' or ts.metadata['SLiM']['stage'] != 'late':
+            root_time -= 1
         nodes = ts.tables.nodes
-        root_time = np.max(nodes.time)
         first_gen = set(nodes.individual[nodes.time == root_time])
         first_gen.discard(tskit.NULL)
         return np.array(list(first_gen), dtype='int')
 
+    @pytest.mark.skip("Waiting on next tskit release.")
     @pytest.mark.parametrize('recipe', recipe_eq("everyone"), indirect=True)
     def test_everyone(self, recipe):
         # since everyone is recorded, only the initial individuals should
         # not have parents
         ts = recipe["ts"]
         right_answer = np.repeat(True, ts.num_individuals)
         first_gen = self.get_first_gen(ts)
-        assert len(first_gen) > 0
         right_answer[first_gen] = False
         has_parents = pyslim.has_individual_parents(ts)
         assert np.array_equal(right_answer, has_parents)
         self.verify_has_parents(ts)
 
+    @pytest.mark.skip("Waiting on next tskit release.")
     @pytest.mark.parametrize('recipe', recipe_eq("everyone"), indirect=True)
     def test_post_recap(self, recipe):
         # the same should be true after recapitation
         ts = recipe["ts"]
         right_answer = np.repeat(True, ts.num_individuals)
         first_gen = self.get_first_gen(ts)
         right_answer[first_gen] = False
         assert(ts.num_populations <= 2)
         ts = self.do_recapitate(ts, recombination_rate=0.01, ancestral_Ne=10, random_seed=11)
         has_parents = pyslim.has_individual_parents(ts)
         assert np.array_equal(right_answer, has_parents)
         self.verify_has_parents(ts)
 
+    @pytest.mark.skip("Waiting on next tskit release.")
     @pytest.mark.parametrize('recipe', recipe_eq("everyone"), indirect=True)
     def test_post_simplify(self, recipe):
         ts = recipe["ts"]
         rng = np.random.default_rng(seed=3)
-        individual_times = ts.individuals_time
+        individual_times = pyslim.individual_times(ts)
         keep_indivs = rng.choice(
                 np.where(individual_times < ts.metadata['SLiM']['tick'] - 1)[0],
                 size=30,
                 replace=False
         )
         keep_nodes = []
         for i in keep_indivs:
@@ -760,33 +703,14 @@
         ntc.sites.clear()
         tc.mutations.clear()
         ntc.mutations.clear()
         tc.provenances.clear()
         ntc.provenances.clear()
         assert tc == ntc
 
-    def scramble_mutations(self, ts):
-        # scramble order of mutations so that the most recent is not always first,
-        # since we don't have a reliable way to get that out of SLiM
-        rng = np.random.default_rng(123)
-        t = ts.dump_tables()
-        t.mutations.clear()
-        for m in ts.mutations():
-            a = np.array(m.derived_state.split(","))
-            ii = rng.permutation(len(a))
-            ml = [m.metadata['mutation_list'][i] for i in ii]
-            t.mutations.append(
-                    m.replace(
-                        derived_state=",".join(a[ii]),
-                        metadata={'mutation_list': ml}
-                    )
-            )
-        t.compute_mutation_parents()
-        return t.tree_sequence()
-
     def test_convert_alleles_errors(self):
         ts = msprime.sim_ancestry(4, sequence_length=10, population_size=10)
         with pytest.raises(ValueError, match="must have a valid reference sequence"):
             _ = pyslim.convert_alleles(ts)
         ts = pyslim.annotate(ts, model_type="nonWF", tick=1)
         with pytest.raises(ValueError, match="must have a valid reference sequence"):
             _ = pyslim.convert_alleles(ts)
@@ -816,32 +740,14 @@
             if j % 2 == 0:
                 t.mutations.append(mut)
         t.compute_mutation_parents()
         ts = t.tree_sequence()
         cts = pyslim.convert_alleles(ts)
         self.verify_converted_nucleotides(ts, cts)
 
-    @pytest.mark.parametrize(
-            'recipe', recipe_eq("nucleotides", exclude="non-nucleotides"), indirect=True
-    )
-    def test_convert_alleles_scrambled(self, recipe):
-        ts = self.scramble_mutations(recipe["ts"])
-        cts = pyslim.convert_alleles(ts)
-        self.verify_converted_nucleotides(ts, cts)
-
-    @pytest.mark.parametrize(
-            'recipe', recipe_eq("nucleotides", exclude="non-nucleotides"), indirect=True
-    )
-    def test_keeps_reference_sequence(self, recipe):
-        ts = recipe["ts"]
-        assert ts.has_reference_sequence()
-        nts = pyslim.generate_nucleotides(ts, seed=123)
-        assert nts.has_reference_sequence()
-        assert ts.reference_sequence == nts.reference_sequence
-
     def test_generate_nucleotides_errors(self):
         ts = msprime.sim_ancestry(4, sequence_length=10, population_size=10, random_seed=777)
         with pytest.raises(ValueError, match="must have length equal"):
             _ = pyslim.generate_nucleotides(ts, reference_sequence="AAA")
         with pytest.raises(ValueError, match="must have length equal"):
             _ = pyslim.generate_nucleotides(ts, reference_sequence=[1, 2, 3])
         with pytest.raises(ValueError, match="must be a string of"):
```

### Comparing `pyslim-1.0.2/tests/test_util.py` & `pyslim-1.0b1/tests/test_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 """
 Test cases for utility functions.
 """
-import pytest
-import warnings
+import tests
 import numpy as np
 
 import pyslim
 
 class TestUniqueLabelsByGroup():
 
     def verify_unique_labels_by_group(self, group, label, minlength):
-        with pytest.warns(FutureWarning):
-            x = pyslim.util.unique_labels_by_group(group, label, minlength)
+        x = pyslim.util.unique_labels_by_group(group, label, minlength)
         assert len(x) >= minlength
         for g in range(len(x)):
             u = set(label[group == g])
             if (len(u) == 1) != x[g]:
                 print(g, u, x[g], label[group == g], label.dtype)
             assert (len(u) <= 1) == x[g]
 
     def test_all_same(self):
         n = 10
         group = np.repeat(1, 10)
         label = np.arange(10)
         self.verify_unique_labels_by_group(group, label, 1)
-        with pytest.warns(FutureWarning):
-            x = pyslim.util.unique_labels_by_group(group, label, 1)
+        x = pyslim.util.unique_labels_by_group(group, label, 1)
         assert len(x) == 2
         assert x[0] == True
         assert x[1] == False
         label = np.repeat(5, 10)
         self.verify_unique_labels_by_group(group, label, 1)
-        with pytest.warns(FutureWarning):
-            x = pyslim.util.unique_labels_by_group(group, label, 1)
+        x = pyslim.util.unique_labels_by_group(group, label, 1)
         assert len(x) == 2
         assert x[0] == True
         assert x[1] == True
 
     def test_all_unique(self):
         ng = 10
         group = np.arange(ng)
         label = np.arange(ng)
         self.verify_unique_labels_by_group(group, label, ng)
-        with pytest.warns(FutureWarning):
-            x = pyslim.util.unique_labels_by_group(group, label, ng)
+        x = pyslim.util.unique_labels_by_group(group, label, ng)
         assert np.all(x)
         group = np.append(group, [-1, -1, -1])
         label = np.append(label, [0, 1, 2])
         self.verify_unique_labels_by_group(group, label, ng)
-        with pytest.warns(FutureWarning):
-            x = pyslim.util.unique_labels_by_group(group, label, ng)
+        x = pyslim.util.unique_labels_by_group(group, label, ng)
         assert np.all(x)
 
     def test_unique_labels_by_group(self):
         np.random.seed(23)
         for ng in 3 * np.arange(2, 15):
             for n in (10, 100):
                 for nl in (2, ng):
@@ -65,14 +59,13 @@
                         # int32 labels
                         self.verify_unique_labels_by_group(group, label.astype("int32"), ng)
                         # and float labels
                         label = minl + np.random.choice(np.random.uniform(0, 1, nl), size=n)
                         self.verify_unique_labels_by_group(group, label, ng)
 
     def test_unused_labels(self):
-        with pytest.warns(FutureWarning):
-            x = pyslim.unique_labels_by_group(
-                group=np.array([1, 1, 4], dtype='int'),
-                label=np.array([2, 2, 2], dtype='int')
-            )
+        x = pyslim.unique_labels_by_group(
+            group=np.array([1, 1, 4], dtype='int'),
+            label=np.array([2, 2, 2], dtype='int')
+        )
         assert np.all(x)
```

