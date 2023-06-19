# Comparing `tmp/pygwb-1.0.0.tar.gz` & `tmp/pygwb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygwb-1.0.0.tar", last modified: Fri Mar 31 01:58:16 2023, max compression
+gzip compressed data, was "pygwb-1.3.0.tar", last modified: Mon Jun 19 23:48:24 2023, max compression
```

## Comparing `pygwb-1.0.0.tar` & `pygwb-1.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.492250 pygwb-1.0.0/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)       81 2022-04-20 22:31:55.000000 pygwb-1.0.0/.coveragerc
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      350 2022-10-10 02:44:00.000000 pygwb-1.0.0/.gitignore
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3887 2023-03-04 00:43:41.000000 pygwb-1.0.0/.gitlab-ci.yml
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      933 2022-04-20 22:31:55.000000 pygwb-1.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10301 2022-03-16 19:09:33.000000 pygwb-1.0.0/CONTRIBUTING.md
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1069 2022-03-16 19:09:33.000000 pygwb-1.0.0/LICENSE
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)       86 2022-10-10 06:22:25.000000 pygwb-1.0.0/MANIFEST.in
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3964 2023-03-31 01:58:16.493250 pygwb-1.0.0/PKG-INFO
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3224 2023-03-31 01:54:46.000000 pygwb-1.0.0/README.md
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     7259 2022-03-16 19:09:33.000000 pygwb-1.0.0/checkpoint.pkl
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.455250 pygwb-1.0.0/docs/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      606 2022-03-16 19:09:33.000000 pygwb-1.0.0/docs/Makefile
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.477250 pygwb-1.0.0/pygwb/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      107 2022-10-10 02:11:55.000000 pygwb-1.0.0/pygwb/__init__.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      160 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb/_version.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    64009 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/baseline.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      296 2023-02-28 18:40:50.000000 pygwb-1.0.0/pygwb/constants.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     7009 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/delta_sigma_cut.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    16072 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/detector.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3637 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/html.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    14627 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/network.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10219 2022-08-15 17:05:36.000000 pygwb-1.0.0/pygwb/notch.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10081 2022-08-15 17:05:36.000000 pygwb-1.0.0/pygwb/omega_spectra.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     6837 2022-03-16 19:09:33.000000 pygwb-1.0.0/pygwb/orfs.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    18154 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/parameters.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    23187 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/pe.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    13678 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/postprocessing.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    17279 2023-03-09 21:39:38.000000 pygwb-1.0.0/pygwb/preprocessing.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    22915 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/simulator.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    19581 2023-03-29 18:34:29.000000 pygwb-1.0.0/pygwb/spectral.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    45345 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/statistical_checks.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     9934 2023-03-29 18:34:29.000000 pygwb-1.0.0/pygwb/util.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     8134 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb/workflow.py
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.481250 pygwb-1.0.0/pygwb.egg-info/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3964 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/PKG-INFO
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      974 2023-03-31 01:58:16.000000 pygwb-1.0.0/pygwb.egg-info/SOURCES.txt
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        1 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/dependency_links.txt
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      127 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/requires.txt
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        6 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/top_level.txt
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.492250 pygwb-1.0.0/pygwb_pipe/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      544 2022-09-30 15:53:13.000000 pygwb-1.0.0/pygwb_pipe/README.md
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2343 2023-02-25 01:02:42.000000 pygwb-1.0.0/pygwb_pipe/parameters.ini
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2287 2022-07-08 17:09:27.000000 pygwb-1.0.0/pygwb_pipe/parameters_mock.ini
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     9249 2023-01-30 22:17:29.000000 pygwb-1.0.0/pygwb_pipe/pygwb_combine
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     8036 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb_pipe/pygwb_create_isotropic_workflow
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     6600 2023-03-29 18:34:29.000000 pygwb-1.0.0/pygwb_pipe/pygwb_dag
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1172 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb_pipe/pygwb_html
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     9814 2023-03-04 00:43:41.000000 pygwb-1.0.0/pygwb_pipe/pygwb_pe
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     7257 2023-02-25 02:18:29.000000 pygwb-1.0.0/pygwb_pipe/pygwb_pipe
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1388 2023-01-27 22:25:50.000000 pygwb-1.0.0/pygwb_pipe/pygwb_stats
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1368 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb_pipe/workflow_config.ini
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      212 2022-10-10 04:12:40.000000 pygwb-1.0.0/pyproject.toml
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      465 2023-03-31 01:58:16.494250 pygwb-1.0.0/setup.cfg
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1885 2023-02-28 18:42:00.000000 pygwb-1.0.0/setup.py
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-06-19 23:48:23.998197 pygwb-1.3.0/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      113 2023-04-22 00:14:33.000000 pygwb-1.3.0/.coveragerc
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      350 2022-10-10 02:44:00.000000 pygwb-1.3.0/.gitignore
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3895 2023-05-08 18:37:02.000000 pygwb-1.3.0/.gitlab-ci.yml
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      933 2022-04-20 22:31:55.000000 pygwb-1.3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10301 2022-03-16 19:09:33.000000 pygwb-1.3.0/CONTRIBUTING.md
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1072 2023-04-22 00:14:33.000000 pygwb-1.3.0/LICENSE
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)       86 2022-10-10 06:22:25.000000 pygwb-1.3.0/MANIFEST.in
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3964 2023-06-19 23:48:23.998197 pygwb-1.3.0/PKG-INFO
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3224 2023-03-31 01:54:46.000000 pygwb-1.3.0/README.md
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     7259 2022-03-16 19:09:33.000000 pygwb-1.3.0/checkpoint.pkl
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-06-19 23:48:23.957196 pygwb-1.3.0/docs/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      606 2022-03-16 19:09:33.000000 pygwb-1.3.0/docs/Makefile
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-06-19 23:48:23.981196 pygwb-1.3.0/pygwb/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      107 2022-10-10 02:11:55.000000 pygwb-1.3.0/pygwb/__init__.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      160 2023-06-19 23:48:22.000000 pygwb-1.3.0/pygwb/_version.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    76353 2023-06-19 00:38:41.000000 pygwb-1.3.0/pygwb/baseline.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      656 2023-04-22 00:14:33.000000 pygwb-1.3.0/pygwb/coherence.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      296 2023-02-28 18:40:50.000000 pygwb-1.3.0/pygwb/constants.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     6997 2023-05-24 18:43:16.000000 pygwb-1.3.0/pygwb/delta_sigma_cut.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    17702 2023-06-13 19:08:53.000000 pygwb-1.3.0/pygwb/detector.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3944 2023-06-13 23:36:19.000000 pygwb-1.3.0/pygwb/html.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    15638 2023-05-11 00:08:45.000000 pygwb-1.3.0/pygwb/network.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10219 2022-08-15 17:05:36.000000 pygwb-1.3.0/pygwb/notch.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10081 2022-08-15 17:05:36.000000 pygwb-1.3.0/pygwb/omega_spectra.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     6837 2022-03-16 19:09:33.000000 pygwb-1.3.0/pygwb/orfs.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    22080 2023-06-13 19:08:53.000000 pygwb-1.3.0/pygwb/parameters.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    23187 2023-02-28 18:42:00.000000 pygwb-1.3.0/pygwb/pe.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    13577 2023-06-19 00:39:38.000000 pygwb-1.3.0/pygwb/postprocessing.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    18111 2023-06-13 19:08:53.000000 pygwb-1.3.0/pygwb/preprocessing.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    22915 2023-02-28 18:42:00.000000 pygwb-1.3.0/pygwb/simulator.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    20353 2023-06-16 16:38:25.000000 pygwb-1.3.0/pygwb/spectral.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    66857 2023-06-16 18:17:57.000000 pygwb-1.3.0/pygwb/statistical_checks.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10143 2023-05-11 00:08:45.000000 pygwb-1.3.0/pygwb/util.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    21390 2023-05-28 23:22:51.000000 pygwb-1.3.0/pygwb/workflow.py
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-06-19 23:48:23.987197 pygwb-1.3.0/pygwb.egg-info/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3964 2023-06-19 23:48:22.000000 pygwb-1.3.0/pygwb.egg-info/PKG-INFO
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      962 2023-06-19 23:48:23.000000 pygwb-1.3.0/pygwb.egg-info/SOURCES.txt
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        1 2023-06-19 23:48:22.000000 pygwb-1.3.0/pygwb.egg-info/dependency_links.txt
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      127 2023-06-19 23:48:22.000000 pygwb-1.3.0/pygwb.egg-info/requires.txt
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        6 2023-06-19 23:48:22.000000 pygwb-1.3.0/pygwb.egg-info/top_level.txt
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-06-19 23:48:23.997197 pygwb-1.3.0/pygwb_pipe/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      544 2022-09-30 15:53:13.000000 pygwb-1.3.0/pygwb_pipe/README.md
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2422 2023-06-14 22:38:49.000000 pygwb-1.3.0/pygwb_pipe/parameters.ini
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)    14727 2023-06-13 15:29:17.000000 pygwb-1.3.0/pygwb_pipe/pygwb_combine
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     7264 2023-05-25 21:10:04.000000 pygwb-1.3.0/pygwb_pipe/pygwb_create_isotropic_workflow
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     6600 2023-03-29 18:34:29.000000 pygwb-1.3.0/pygwb_pipe/pygwb_dag
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1369 2023-04-22 00:14:33.000000 pygwb-1.3.0/pygwb_pipe/pygwb_html
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)    10285 2023-04-25 21:43:00.000000 pygwb-1.3.0/pygwb_pipe/pygwb_pe
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     9014 2023-06-13 19:08:53.000000 pygwb-1.3.0/pygwb_pipe/pygwb_pipe
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1769 2023-06-13 22:37:10.000000 pygwb-1.3.0/pygwb_pipe/pygwb_stats
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1368 2023-02-21 22:11:58.000000 pygwb-1.3.0/pygwb_pipe/workflow_config.ini
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      212 2022-10-10 04:12:40.000000 pygwb-1.3.0/pyproject.toml
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      466 2023-06-19 23:48:23.999197 pygwb-1.3.0/setup.cfg
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1885 2023-05-23 18:14:19.000000 pygwb-1.3.0/setup.py
```

### Comparing `pygwb-1.0.0/.gitlab-ci.yml` & `pygwb-1.3.0/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 documentation:
   stage: documentation
   image: python:3.8
   before_script:
     - apt-get -yqq update
     - apt-get -yqq install pandoc
     - pip install --upgrade pip setuptools
-    - pip install ipykernel ipython jupyter
+    - pip install ipykernel ipython==8.12.0 jupyter
     - pip install sphinx numpydoc nbsphinx sphinx_rtd_theme sphinx-tabs autodoc ipython-genutils
     - pip install .
 
   script:
     - cd docs
     - cp ../tutorials/*.ipynb ./
     - cp ../tutorials/*.dat ./
```

### Comparing `pygwb-1.0.0/.pre-commit-config.yaml` & `pygwb-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/CONTRIBUTING.md` & `pygwb-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/LICENSE` & `pygwb-1.3.0/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Andrew Matas
+Copyright (c) 2023 Arianna Renzini
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pygwb-1.0.0/PKG-INFO` & `pygwb-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwb
-Version: 1.0.0
+Version: 1.3.0
 Summary: Lighweight python stochastic GWB analysis pipeline
 Home-page: https://git.ligo.org/pygwb/pygwb
 Author: Arianna Renzini, Sylvia Biscoveanu, Shivaraj Khandasamy, Kamiel Janssens, Max Lalleman, Katarina Martinovic, Andrew Matas, Patrick Meyers, Alba Romero, Colm Talbot, Leo Tsukada, Kevin Turbang
 Author-email: arianna.renzini@ligo.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pygwb-1.0.0/README.md` & `pygwb-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/checkpoint.pkl` & `pygwb-1.3.0/checkpoint.pkl`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/docs/Makefile` & `pygwb-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb/baseline.py` & `pygwb-1.3.0/pygwb/baseline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import pickle
 import warnings
 
 import h5py
 import numpy as np
+from gwpy.frequencyseries import FrequencySeries
 from loguru import logger
 
-from pygwb.delta_sigma_cut import run_dsc
-from pygwb.omega_spectra import OmegaSpectrogram, OmegaSpectrum
-
+from .coherence import calculate_coherence
 from .constants import h0
+from .delta_sigma_cut import run_dsc
 from .notch import StochNotchList
+from .omega_spectra import OmegaSpectrogram, OmegaSpectrum
 from .orfs import calc_orf
 from .postprocessing import (
     calc_Y_sigma_from_Yf_sigmaf,
     calculate_point_estimate_sigma_spectra,
     postprocess_Y_sigma,
 )
 from .spectral import cross_spectral_density
@@ -30,18 +31,21 @@
         name,
         interferometer_1,
         interferometer_2,
         duration=None,
         frequencies=None,
         calibration_epsilon=0,
         notch_list_path="",
+        coarse_grain_psd=False,
+        coarse_grain_csd=True,
+        overlap_factor_welch=0.5,
         overlap_factor=0.5,
-        zeropad_csd=True,
         window_fftgram_dict={"window_fftgram": "hann"},
-        N_average_segments_welch_psd=2,
+        window_fftgram_dict_welch={"window_fftgram": "hann"},
+        N_average_segments_psd=2,
         sampling_frequency=None,
     ):
         """
         Instantiate a Baseline.
 
         Parameters
         ----------
@@ -55,49 +59,85 @@
         frequencies: array_like, optional
             The frequency array for the Baseline and
             interferometers
         calibration_epsilon: float, optional
             Calibration uncertainty for this baseline
         notch_list_path: str, optional
             File path of the baseline notch list
+        coarse_grain_psd: bool
+            Whether to apply coarse graining to obtain PSD spectra. Default is False.
+        coarse_grain_csd: bool
+            Whether to apply coarse graining to obtain CSD spectra. Default is True.
+        overlap_factor_welch: float, optional
+            Overlap factor to use when if using Welch's method to estimate spectra (NOT coarsegraining). For \"hann\" window use 0.5 overlap_factor and for \"boxcar"\ window use 0 overlap_factor. Default is 0.5 (50% overlap), which is optimal when using Welch's method with a \"hann\" window.
+ 
         overlap_factor: float, optional
             Factor by which to overlap the segments in the psd and csd estimation.
             Default is 1/2, if set to 0 no overlap is performed.
-        zeropad_csd: bool, optional
-            If True, applies zeropadding in the csd estimation. True by default.
         window_fftgram_dict: dictionary, optional
-            Dictionary containing name and parameters describing which window to use when producing fftgrams for psds and csds. Default is \"hann\".
-        N_average_segments_welch_psd: int, optional
+            Dictionary containing name and parameters describing which window to use when producing fftgrams for csds (and psds if these are coarse-grained). Default is \"hann\".
+        window_fftgram_dict_welch: dictionary, optional
+            Dictionary containing name and parameters describing which window to use when producing fftgrams with Welch's method. Default is \"hann\".
+        N_average_segments_psd: int, optional
             Number of segments used for PSD averaging (from both sides of the segment of interest)
             N_avg_segs should be even and >= 2.
         """
         self.name = name
         self.interferometer_1 = interferometer_1
         self.interferometer_2 = interferometer_2
         self.calibration_epsilon = calibration_epsilon
         self.notch_list_path = notch_list_path
+        self.coarse_grain_psd = coarse_grain_psd
+        self.coarse_grain_csd = coarse_grain_csd
+        self.overlap_factor_welch = overlap_factor_welch
         self.overlap_factor = overlap_factor
-        self.zeropad_csd = zeropad_csd
         self.window_fftgram_dict = window_fftgram_dict
-        self.N_average_segments_welch_psd = N_average_segments_welch_psd
+        self.window_fftgram_dict_welch = window_fftgram_dict_welch
+        self.N_average_segments_psd = N_average_segments_psd
         self._tensor_orf_calculated = False
         self._vector_orf_calculated = False
         self._scalar_orf_calculated = False
         self._gamma_v_calculated = False
         self._orf_polarization_set = False
-        self.duration = duration
+        self._point_estimate_spectrogram_set = False
+        self._point_estimate_spectrum_set = False
+        self._point_estimate_set = False
+        self._sigma_spectrogram_set = False
+        self._sigma_spectrum_set = False
+        self._sigma_set = False
+        self._coherence_spectrum_set = False
         self.sampling_frequency = sampling_frequency
         self.duration = duration
         self.frequencies = frequencies
         self.minimum_frequency = max(
             interferometer_1.minimum_frequency, interferometer_2.minimum_frequency
         )
         self.maximum_frequency = min(
             interferometer_1.maximum_frequency, interferometer_2.maximum_frequency
         )
+        # if CSD is estimated by coarse-graining, it must be zeropaded. 
+        self.zeropad_csd = self.coarse_grain_csd
+        # if PSD is estimated by coarse-graining, no overlap is used between PSD estimates. This is required for the bias factor calculation.
+        if self.coarse_grain_psd:
+            self.overlap_factor_psd = 0.0
+            self.window_fftgram_dict_psd = self.window_fftgram_dict
+            self.window_fftgram_dict_for_bias_factors = {"window_fftgram": "boxcar"}
+        else:
+            self.overlap_factor_psd = self.overlap_factor_welch
+            self.window_fftgram_dict_psd = self.window_fftgram_dict_welch
+            self.window_fftgram_dict_for_bias_factors = self.window_fftgram_dict_psd
+        if self.coarse_grain_csd:
+            self.window_fftgram_dict_csd = self.window_fftgram_dict
+        else:
+            self.window_fftgram_dict_csd = self.window_fftgram_dict_welch
+        # throw a warning if overlap factors are unsupported
+        if self.overlap_factor>0.5:
+            warnings.warn("Overlap factor not fully supported. Overlap factor should be overlap_factor <= 0.5.")
+        if self.overlap_factor_welch>0.5:
+            warnings.warn("Overlap factor for spectral estimation using Welch's method not fully supported. Overlap factor should be overlap_factor_welch <= 0.5.")
 
     def __eq__(self, other):
         if not type(self) == type(other):
             return False
         else:
             return all(
                 [
@@ -121,25 +161,25 @@
         elif self._orf_polarization == "vector":
             return self.vector_overlap_reduction_function
         elif self._orf_polarization == "scalar":
             return self.scalar_overlap_reduction_function
         elif self._orf_polarization == "right_left":
             return self.gamma_v
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Overlap reduction function to be used has not yet been set. To set it, set the orf_polarization property."
             )
 
     @property
     def orf_polarization(self):
         """Overlap reduction function polarization"""
         if self._orf_polarization_set:
             return self._orf_polarization
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Overlap reduction function polarization han not yet been set."
             )
 
     @orf_polarization.setter
     def orf_polarization(self, pol):
         self._orf_polarization = pol
         self._orf_polarization_set = True
@@ -206,15 +246,15 @@
 
     @property
     def duration(self):
         """Duration in seconds of a unit segment of data stored in the baseline detectors."""
         if self._duration_set:
             return self._duration
         else:
-            raise ValueError("Duration not yet set.")
+            raise AttributeError("Duration not yet set.")
 
     @duration.setter
     def duration(self, dur):
         """Sets the duration for the Baseline and interferometers
 
         If `duration` is passed, check that it matches the `duration`
         in the interferometers, if present.
@@ -257,25 +297,25 @@
             self._duration = dur
             self._duration_set = True
 
     @property
     def csd_segment_offset(self):
         if self._duration_set:
             stride = self.duration * (1 - self.overlap_factor)
-            return int(np.ceil(self.duration / stride)) * int(self.N_average_segments_welch_psd/2)
+            return int(np.ceil(self.duration / stride)) * int(self.N_average_segments_psd/2)
         else:
             raise ValueError("Trying to calculate CSD segment offset before setting duration. Need to set duration before attempting this.")
 
     @property
     def frequencies(self):
         """Frequency array associated to this baseline."""
         if self._frequencies_set:
             return self._frequencies
         else:
-            raise ValueError("frequencies have not yet been set.")
+            raise AttributeError("frequencies have not yet been set.")
 
     @frequencies.setter
     def frequencies(self, freqs):
         self._frequencies = freqs
         self._frequencies_set = True
         self.frequency_mask = None
         # delete the orfs, set the calculated flag to zero
@@ -291,98 +331,127 @@
 
     @property
     def point_estimate_spectrogram(self):
         """Point estimate spectrogram (in Omega units) calculated using data in this baseline."""
         if self._point_estimate_spectrogram_set:
             return self._point_estimate_spectrogram
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Omega point estimate spectrogram not yet set. To set it, use `set_point_estimate_sigma_spectrogram` method."
             )
 
     @point_estimate_spectrogram.setter
     def point_estimate_spectrogram(self, pt_est):
         self._point_estimate_spectrogram = pt_est
         self._point_estimate_spectrogram_set = True
 
     @property
     def sigma_spectrogram(self):
         """Sigma spectrogram (in Omega units) calculated using data in this baseline."""
         if self._sigma_spectrogram_set:
             return self._sigma_spectrogram
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Omega sigma spectrogram not yet set. To set it, use `set_point_estimate_sigma_spectrogram` method."
             )
 
     @sigma_spectrogram.setter
     def sigma_spectrogram(self, sig):
         self._sigma_spectrogram = sig
         self._sigma_spectrogram_set = True
 
     @property
     def point_estimate_spectrum(self):
         """Point estimate spectrum (in Omega units) calculated using data in this baseline."""
         if self._point_estimate_spectrum_set:
             return self._point_estimate_spectrum
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Omega point estimate spectrum not yet set. To set it, use `set_point_estimate_sigma_spectrum` method."
             )
 
     @point_estimate_spectrum.setter
     def point_estimate_spectrum(self, pt_est):
         self._point_estimate_spectrum = pt_est
         self._point_estimate_spectrum_set = True
 
     @property
     def sigma_spectrum(self):
         """Sigma spectrum (in Omega units) calculated using data in this baseline."""
         if self._sigma_spectrum_set:
             return self._sigma_spectrum
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Omega sigma spectrum not yet set. To set it, use `set_point_estimate_sigma_spectrum` method."
             )
 
     @sigma_spectrum.setter
     def sigma_spectrum(self, sig):
         self._sigma_spectrum = sig
         self._sigma_spectrum_set = True
 
     @property
     def point_estimate(self):
         """Point estimate (in Omega units) calculated using data in this baseline."""
         if self._point_estimate_set:
             return self._point_estimate
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Omega point estimate not yet set. To set it, use `set_point_estimate_sigma` method."
             )
 
     @point_estimate.setter
     def point_estimate(self, pt_est):
         self._point_estimate = pt_est
         self._point_estimate_set = True
 
     @property
     def sigma(self):
         """Sigma (in Omega units) calculated using data in this baseline."""
         if self._sigma_set:
             return self._sigma
         else:
-            raise ValueError(
+            raise AttributeError(
                 "Omega sigma not yet set. To set it, use `set_point_estimate_sigma` method."
             )
 
     @sigma.setter
     def sigma(self, sig):
         self._sigma = sig
         self._sigma_set = True
 
+    @property
+    def coherence_spectrum(self):
+        """Coherence spectrum calculated using data in this baseline."""
+        if self._coherence_spectrum_set:
+            return self._coherence_spectrum
+        else:
+            raise AttributeError(
+                "Coherence spectrum not yet set. To set it, use `set_coherence_spectrum` method."
+            )
+
+    @coherence_spectrum.setter
+    def coherence_spectrum(self, coh):
+        self._coherence_spectrum = coh
+        self._coherence_spectrum_set = True
+
+    @property
+    def coherence_dict(self):
+        """Coherence dictionary based on data in this baseline."""
+        if self._coherence_spectrum_set:
+            return self._coherence_dict
+        else:
+            raise AttributeError(
+                "Coherence spectrum not yet set. To set it, use `set_coherence_spectrum` method."
+            )
+
+    @coherence_dict.setter
+    def coherence_dict(self, cohdict):
+        self._coherence_dict = cohdict
+
     def _check_durations_match_baseline_ifos(self, duration):
         if self.interferometer_1.duration and self.interferometer_2.duration:
             self._check_ifo_durations_match()
             if not duration == self.interferometer_1.duration:
                 raise AssertionError(
                     "Interferometer durations do not match given Baseline duration!"
                 )
@@ -404,15 +473,15 @@
     @property
     def sampling_frequency(self):
         """Sampling frequency of the data stored in this baseline. This must match the
         sampling frequency stored in this baseline's interferometers."""
         if hasattr(self, "_sampling_frequency"):
             return self._sampling_frequency
         else:
-            raise ValueError("sampling frequency not set.")
+            raise AttributeError("sampling frequency not set.")
 
     @sampling_frequency.setter
     def sampling_frequency(self, sampling_frequency):
         """Sets the sampling_frequency for the Baseline and interferometers
 
         If `sampling_frequency` is passed, check that it matches the `sampling_frequency`
         in the interferometers, if present.
@@ -466,29 +535,29 @@
 
     @property
     def badGPStimes(self):
         """GPS times flagged by delta sigma cut."""
         if hasattr(self, "_badGPStimes"):
             return self._badGPStimes
         else:
-            raise ValueError(
+            raise AttributeError(
                 "bad GPS times are not set - need to run delta_sigma_cut first."
             )
 
     @badGPStimes.setter
     def badGPStimes(self, badGPStimes):
         self._badGPStimes = badGPStimes
 
     @property
     def delta_sigmas(self):
         """Values of delta sigmas for data segments in the baseline."""
         if hasattr(self, "_delta_sigmas"):
             return self._delta_sigmas
         else:
-            raise ValueError(
+            raise AttributeError(
                 "delta_sigmas are not set - need to run delta_sigma_cut first."
             )
 
     @delta_sigmas.setter
     def delta_sigmas(self, delta_sigmas):
         self._delta_sigmas = delta_sigmas
 
@@ -640,18 +709,21 @@
             name=name,
             interferometer_1=interferometer_1,
             interferometer_2=interferometer_2,
             duration=parameters.segment_duration,
             calibration_epsilon=parameters.calibration_epsilon,
             frequencies=frequencies,
             notch_list_path=parameters.notch_list_path,
+            coarse_grain_psd=parameters.coarse_grain_psd,
+            coarse_grain_csd=parameters.coarse_grain_csd,
+            overlap_factor_welch=parameters.overlap_factor_welch,
             overlap_factor=parameters.overlap_factor,
-            zeropad_csd=parameters.zeropad_csd,
             window_fftgram_dict=parameters.window_fft_dict,
-            N_average_segments_welch_psd=parameters.N_average_segments_welch_psd,
+            window_fftgram_dict_welch=parameters.window_fft_dict_welch,
+            N_average_segments_psd=parameters.N_average_segments_psd,
             sampling_frequency=parameters.new_sample_rate,
         )
 
     @classmethod
     def load_from_pickle(cls, filename):
         """
         Load baseline object from pickle file.
@@ -688,54 +760,58 @@
         ==========
         frequency_resolution: float
             The frequency resolution at which the cross and power spectral densities are calculated.
         """
         try:
             self.interferometer_1.set_psd_spectrogram(
                 frequency_resolution,
+                coarse_grain=self.coarse_grain_psd,
                 overlap_factor=self.overlap_factor,
-                window_fftgram_dict_welch_psd={"window_fftgram": "hann"},
-                overlap_factor_welch_psd=0.5,
+                window_fftgram_dict=self.window_fftgram_dict_psd,
+                overlap_factor_welch=self.overlap_factor_welch,
             )
         except AttributeError:
             raise AssertionError(
                 "Interferometer {self.interferometer_1.name} has no timeseries data! Need to set timeseries data in the interferometer first."
             )
         try:
             self.interferometer_2.set_psd_spectrogram(
                 frequency_resolution,
+                coarse_grain=self.coarse_grain_psd,
                 overlap_factor=self.overlap_factor,
-                window_fftgram_dict_welch_psd={"window_fftgram": "hann"},
-                overlap_factor_welch_psd=0.5,
+                window_fftgram_dict=self.window_fftgram_dict_psd,
+                overlap_factor_welch=self.overlap_factor_welch,
             )
         except AttributeError:
             raise AssertionError(
                 "Interferometer {self.interferometer_2.name} has no timeseries data! Need to set timeseries data in the interferometer first."
             )
         self.csd = cross_spectral_density(
             self.interferometer_1.timeseries,
             self.interferometer_2.timeseries,
             self.duration,
             frequency_resolution,
+            coarse_grain=self.coarse_grain_csd,
             overlap_factor=self.overlap_factor,
             zeropad=self.zeropad_csd,
-            window_fftgram_dict=self.window_fftgram_dict,
+            window_fftgram_dict=self.window_fftgram_dict_csd,
+            overlap_factor_welch=self.overlap_factor_welch,
         )
 
         # TODO: make this less fragile.
         # For now, reset frequencies,
         # recalculate ORF in case frequencies have changed.
         self._tensor_orf_calculated = False
         self.frequencies = self.csd.frequencies.value
 
     def set_average_power_spectral_densities(self):
         """If psds have been calculated, sets the average psd in each ifo"""
         try:
-            self.interferometer_1.set_average_psd(self.N_average_segments_welch_psd)
-            self.interferometer_2.set_average_psd(self.N_average_segments_welch_psd)
+            self.interferometer_1.set_average_psd(self.N_average_segments_psd)
+            self.interferometer_2.set_average_psd(self.N_average_segments_psd)
         except AttributeError:
             print(
                 "PSDs have not been calculated yet! Need to set_cross_and_power_spectral_density first."
             )
 
         # TODO: make this less fragile.
         # For now, recalculate ORF in case frequencies have changed.
@@ -781,30 +857,32 @@
             )
         if hasattr(self.interferometer_2, "average_psd"):
             self.interferometer_2.average_psd = (
                 self.interferometer_2.average_psd.crop_frequencies(flow, fhigh + deltaF)
             )
         if hasattr(self, "average_csd"):
             self.average_csd = self.average_csd.crop_frequencies(flow, fhigh + deltaF)
-        if hasattr(self, "point_estimate_spectrogram"):
+        if self._point_estimate_spectrogram_set:
             self.point_estimate_spectrogram = (
                 self.point_estimate_spectrogram.crop_frequencies(flow, fhigh + deltaF)
             )
-        if hasattr(self, "sigma_spectrogram"):
+        if self._sigma_spectrogram_set:
             self.sigma_spectrogram = self.sigma_spectrogram.crop_frequencies(
                 flow, fhigh + deltaF
             )
-        if hasattr(self, "point_estimate_spectrum"):
+        if self._point_estimate_spectrum_set:
             self.point_estimate_spectrum = self.point_estimate_spectrum.crop(
                 flow, fhigh + deltaF
             )
-        if hasattr(self, "sigma_spectrum"):
+        if self._sigma_spectrum_set:
             self.sigma_spectrum = self.sigma_spectrum.crop(flow, fhigh + deltaF)
-        if hasattr(self, "point_estimate"):
+        if self._point_estimate_set:
             self.set_point_estimate_sigma()
+        if self._coherence_spectrum_set:
+            self.coherence_spectrum = self.coherence_spectrum.crop(flow, fhigh + deltaF)
 
     def set_point_estimate_sigma_spectrogram(
         self, alpha=0.0, fref=25, flow=20, fhigh=1726, polarization="tensor"
     ):
         """
         Set point estimate and sigma spectrogram. Resulting spectrogram
         *does not include frequency weighting for alpha*.
@@ -831,26 +909,27 @@
         # self.set_average_power_spectral_densities()
 
         self.crop_frequencies_average_psd_csd(flow, fhigh)
 
         if not self._orf_polarization_set:
             self.orf_polarization = polarization
 
-        # don't get rid of information unless we need to.
         Y_fs, var_fs = calculate_point_estimate_sigma_spectra(
             freqs=self.frequencies,
             csd=self.average_csd,
             avg_psd_1=self.interferometer_1.average_psd,
             avg_psd_2=self.interferometer_2.average_psd,
             orf=self.overlap_reduction_function,
             sample_rate=self.sampling_frequency,
             segment_duration=self.duration,
             fref=fref,
             alpha=alpha,
-        ) #missing: pwelch estimation parameters
+            overlap_factor=self.overlap_factor,
+            window_fftgram_dict=self.window_fftgram_dict_csd
+        ) 
 
         sigma_name = f"{self.name} sigma spectrogram alpha={alpha}"
         self.point_estimate_spectrogram = OmegaSpectrogram(
             Y_fs,
             times=self.average_csd.times,
             frequencies=self.average_csd.frequencies,
             name=self.name + f" with alpha={alpha}",
@@ -905,34 +984,21 @@
         apply_dsc: bool, optional
             Apply delta sigma cut flag; if True, removes the badGPStimes from the spectra calculations.
             Default is True.
         apply_notches: bool, optional
             Apply spectral notches flag; if True, remove the notches specified in the notch_list from the spectra calculations.
             Default is True.
         """
-        if self.overlap_factor>0.0:
-            do_overlap = True
-        else:
-            do_overlap = False
-
         if apply_dsc == True:
             if not hasattr(self, "badGPStimes"):
                 warnings.warn(
                     "Delta sigma cut has not been calculated yet, hence no delta sigma cut will be applied... If this is a mistake, please run `calculate_delta_sigma_cut` first, then re-calculate point estimate/sigma spectra."
                 )
-            if badtimes is None:
-                if hasattr(self, "badGPStimes"):
-                    badtimes = self.badGPStimes
-            else:
-                badtimes = np.append(badtimes, self.badGPStimes)
-                self.badGPStimes = badtimes
-        else:
-            badtimes = np.array([])
 
-        if hasattr(self, "point_estimate_spectrogram"):
+        if self._point_estimate_spectrogram_set:
             # reweight based on alpha that has been supplied
             self.point_estimate_spectrogram.reweight(new_alpha=alpha, new_fref=fref)
             self.sigma_spectrogram.reweight(new_alpha=alpha, new_fref=fref)
         else:
             logger.info(
                 "Point estimate and sigma spectrograms are not set yet. setting now..."
             )
@@ -942,50 +1008,54 @@
                 flow=flow,
                 fhigh=fhigh,
                 polarization=polarization,
             )
         deltaF = self.frequencies[1] - self.frequencies[0]
 
         # should be True for each bad time
-        bad_times_indexes = np.array(
-            [np.any(t == badtimes) for t in self.point_estimate_spectrogram.times.value]
-        )
+        bad_times_indexes = self._get_bad_times_indexes(times=self.point_estimate_spectrogram.times.value, badtimes=badtimes, apply_dsc=apply_dsc)
 
         logger.info(f"{np.sum(bad_times_indexes)} bad segments removed.")
 
         # start time, for metadata
         epoch = self.point_estimate_spectrogram.times[0]
 
         if self.sampling_frequency is None:
-            raise ValueError(
+            raise AttributeError(
                 "the sampling frequency is not set! Cannot proceed with spectrum calculation."
             )
 
         if apply_dsc:
             if len(self.delta_sigmas["times"]) == len(self.badGPStimes):
-                raise ValueError(
+                warnings.warn(
                     "The delta sigma cut has flagged all times in this dataset. No point estimate/sigma values can be calculated."
                 )
-
+                self.point_estimate_spectrum =  np.zeros(len(self.frequencies))
+                self.sigma_spectrum = np.inf * np.ones(len(self.frequencies))
+                return 
+            
         # setting the frequency mask for the before/after calculation
         self.set_frequency_mask(
             notch_list_path=notch_list_path, apply_notches=apply_notches
         )
 
         point_estimate, sigma = postprocess_Y_sigma(
             self.point_estimate_spectrogram.value,
             self.sigma_spectrogram.value ** 2,
             self.duration,
             deltaF,
             self.sampling_frequency,
             frequency_mask=self.frequency_mask,
+            window_fftgram_dict=self.window_fftgram_dict,
+            window_fftgram_dict_welch=self.window_fftgram_dict_for_bias_factors,
             badtimes_mask=bad_times_indexes,
-            do_overlap=do_overlap,
-            N_avg_segs=self.N_average_segments_welch_psd,
-        )#missing: pwelch estimation parameters
+            overlap_factor=self.overlap_factor,
+            overlap_factor_welch=self.overlap_factor_psd,
+            N_avg_segs=self.N_average_segments_psd,
+        )
 
         self.point_estimate_spectrum = OmegaSpectrum(
             point_estimate,
             frequencies=self.frequencies,
             name=self.name + " point estimate spectrum",
             epoch=epoch,
             alpha=alpha,
@@ -1018,15 +1088,15 @@
         """
         Set point estimate sigma based on a set of parameters. This is estimate of omega_gw in each frequency bin.
 
         Parameters
         ==========
         badtimes: np.array, optional
             Array of times to exclude from point estimate/sigma calculation.
-            If no times are passed, none will be excluded.
+            Default is None.
         alpha: float, optional
             Spectral index to use in the re-weighting. Default is 0.
         fref: float, optional
             Reference frequency to use in the re-weighting. Default is 25.
         flow: float, optional
             Low frequency. Default is 20 Hz.
         fhigh: float, optional
@@ -1041,15 +1111,15 @@
             Apply delta sigma cut flag; if True, removes the badGPStimes from the spectra calculations.
             Default is True.
         apply_notches: bool, optional
             Apply spectral notches flag; if True, remove the notches specified in the notch_list from the spectra calculations.
             Default is True.
         """
 
-        if hasattr(self, "point_estimate_spectrum"):
+        if self._point_estimate_spectrum_set:
             self.point_estimate_spectrum.reweight(new_alpha=alpha, new_fref=fref)
             self.sigma_spectrum.reweight(new_alpha=alpha, new_fref=fref)
             self.point_estimate_spectrogram.reweight(new_alpha=alpha, new_fref=fref)
             self.sigma_spectrogram.reweight(new_alpha=alpha, new_fref=fref)
         else:
             logger.info(
                 "Point estimate and sigma spectra have not been set before. Setting it now..."
@@ -1068,14 +1138,19 @@
                 notch_list_path=notch_list_path,
             )
 
         self.set_frequency_mask(
             notch_list_path=notch_list_path, apply_notches=apply_notches
         )
 
+        if self.sigma_spectrum[0] == np.infty:
+                self.sigma = np.inf
+                self.point_estimate = 0
+                return 
+
         Y, sigma = calc_Y_sigma_from_Yf_sigmaf(
             self.point_estimate_spectrum,
             self.sigma_spectrum,
             frequency_mask=self.frequency_mask,
             alpha=alpha,
             fref=fref,
         )
@@ -1153,33 +1228,123 @@
             logger.debug(
                 "loading notches for delta sigma cut from " + self.notch_list_path
             )
             self.set_frequency_mask(self.notch_list_path)
         else:
             self.set_frequency_mask()
 
+
         badGPStimes, delta_sigmas = run_dsc(
             dsc=delta_sigma_cut,
             segment_duration=self.duration,
             psd1_naive=naive_psd_1_cropped,
             psd2_naive=naive_psd_2_cropped,
             psd1_slide=self.interferometer_1.average_psd,
             psd2_slide=self.interferometer_2.average_psd,
             alphas=alphas,
             sample_rate=self.sampling_frequency,
             orf=self.overlap_reduction_function,
             fref=fref,
             frequency_mask=self.frequency_mask,
-            N_average_segments_welch_psd = self.N_average_segments_welch_psd,
+            window_fftgram_dict=self.window_fftgram_dict_for_bias_factors,
+            overlap_factor=self.overlap_factor_psd, 
+            N_average_segments_psd = self.N_average_segments_psd,
             return_naive_and_averaged_sigmas=return_naive_and_averaged_sigmas,
-        )#missing: pwelch estimation parameters
+        )
 
         self.badGPStimes = badGPStimes
         self.delta_sigmas = delta_sigmas
 
+    def set_coherence_spectrum(self, flow=20, fhigh=1726, badtimes=None, apply_dsc=True):
+        """
+        Set the coherence spectrum between detectors, averaged over all data in the baseline.
+
+        Parameters
+        ==========
+        flow: float, optional
+            Low frequency. Default is 20 Hz.
+        fhigh: float, optional
+            High frequency. Default is 1726 Hz.
+        badtimes: np.array, optional
+            Array of times to exclude from the coherence calculation.
+            Default is None.
+        apply_dsc: bool, optional
+            Apply delta sigma cut flag; if True, removes the badGPStimes from the spectra calculations.
+            Default is True.
+
+        Note: The coherence calculation uses averaged naive PSD estimates as the coherence is calculated using CSD and PSD estimates of each individual segment, calculated \"on shell\".
+        """
+
+        bad_times_indexes = self._get_bad_times_indexes(times=self.interferometer_1.psd_spectrogram.times.value, apply_dsc=apply_dsc)
+
+        deltaF = self.frequencies[1] - self.frequencies[0]
+        n_segs = len(self.interferometer_1.psd_spectrogram[~bad_times_indexes])
+
+        psd_1_average = np.mean(self.interferometer_1.psd_spectrogram[~bad_times_indexes].crop_frequencies(flow, fhigh + deltaF), axis=0)
+        psd_2_average = np.mean(self.interferometer_2.psd_spectrogram[~bad_times_indexes].crop_frequencies(flow, fhigh + deltaF), axis=0)
+        csd_average = np.mean(self.csd[~bad_times_indexes].crop_frequencies(flow, fhigh + deltaF), axis=0)
+
+        coherence = calculate_coherence(
+            psd_1_average,
+            psd_2_average,
+            csd_average,
+        )
+
+        epoch = self.csd.times[0]
+
+        self.coherence_spectrum = FrequencySeries(
+            coherence,
+            frequencies=self.frequencies,
+            name=self.name + " coherence spectrum",
+            epoch=epoch,
+        )
+
+        self.coherence_dict = {}
+        self.coherence_dict['psd_1_average'] = psd_1_average
+        self.coherence_dict['psd_2_average'] = psd_2_average
+        self.coherence_dict['csd_average']= csd_average
+        self.coherence_dict['n_segs']= n_segs
+        self.coherence_dict['coherence']= coherence
+        self.coherence_dict['frequencies']= self.frequencies
+        self.coherence_dict['epoch']= epoch
+
+
+
+    def _get_bad_times_indexes(self, times, badtimes=None, apply_dsc=False):
+        """
+        Get indexes for segments with bad GPS times, to be removed from analysis.
+
+        Parameters
+        ==========
+        badtimes: np.array, optional
+            Array of times to exclude from further calculation.
+            Default is None.
+        apply_dsc: bool
+            If True, calculates the indexes of the segments with a bad GPS time, according to the delta sigma cut. If False, returns None.
+        """
+
+        if apply_dsc == True:
+            if not hasattr(self, "badGPStimes"):
+                warnings.warn(
+                    "Delta sigma cut has not been calculated yet, hence no delta sigma cut will be applied... If this is a mistake, please run `calculate_delta_sigma_cut` first, then re-calculate point estimate/sigma spectra."
+                )
+            if badtimes is not None:
+                if hasattr(self, "badGPStimes"):
+                    badtimes = np.append(badtimes, self.badGPStimes)
+                self.badGPStimes = badtimes
+            else:
+                badtimes = self.badGPStimes
+        else:
+            badtimes = np.array([])
+
+        bad_times_indexes = np.array(
+            [np.any(t == badtimes) for t in times]
+        )
+        return bad_times_indexes
+
     def save_point_estimate_spectra(
         self,
         save_data_type,
         filename,
     ):
         """
         Save the overall point estimate Y, its error bar sigma,
@@ -1204,15 +1369,15 @@
             save = self._npz_save
             ext = ".npz"
 
         elif save_data_type == "json":
             save = self._json_save
             ext = ".json"
 
-        elif save_data_type == "hdf5":
+        elif save_data_type == "hdf5" or save_data_type == "h5":
             save = self._hdf5_save
             ext = ".h5"
 
         else:
             raise ValueError(
                 "The provided data type is not supported, try using 'pickle', 'npz', 'json' or 'hdf5' instead."
             )
@@ -1225,14 +1390,18 @@
             self.sigma_spectrum,
             self.point_estimate,
             self.sigma,
             self.point_estimate_spectrogram,
             self.sigma_spectrogram,
             self.badGPStimes,
             self.delta_sigmas,
+            self.interferometer_1.gates,
+            self.interferometer_1.gate_pad,
+            self.interferometer_2.gates,
+            self.interferometer_2.gate_pad,
         )
 
     def save_psds_csds(
         self,
         save_data_type,
         filename,
     ):
@@ -1258,33 +1427,52 @@
             save_csd = self._npz_save_csd
             ext = ".npz"
 
         elif save_data_type == "json":
             save_csd = self._json_save_csd
             ext = ".json"
 
-        elif save_data_type == "hdf5":
+        elif save_data_type == "hdf5" or save_data_type == "h5":
             save_csd = self._hdf5_save_csd
             ext = ".h5"
 
         else:
             raise ValueError(
                 "The provided data type is not supported, try using 'pickle', 'npz', 'json' or 'hdf5' instead."
             )
 
+        try:
+            coherence = self.coherence_spectrum
+            psd_1_coh = self.coherence_dict['psd_1_average']
+            psd_2_coh = self.coherence_dict['psd_2_average']
+            csd_coh = self.coherence_dict['csd_average']
+            n_segs_coh = self.coherence_dict['n_segs']
+
+        except AttributeError:
+            coherence = None
+            psd_1_coh = None
+            psd_2_coh = None
+            csd_coh = None
+            n_segs_coh = None
+
         save_csd(
             f"{filename}{ext}",
-            self.frequencies,
+            self.csd.frequencies.value,
             self.average_csd.frequencies.value,
             self.csd,
             self.average_csd,
             self.interferometer_1.psd_spectrogram,
             self.interferometer_2.psd_spectrogram,
             self.interferometer_1.average_psd,
             self.interferometer_2.average_psd,
+            coherence,
+            psd_1_coh,
+            psd_2_coh,
+            csd_coh,
+            n_segs_coh,
         )
 
     def _npz_save(
         self,
         filename,
         frequencies,
         frequency_mask,
@@ -1292,14 +1480,18 @@
         sigma_spectrum,
         point_estimate,
         sigma,
         point_estimate_spectrogram,
         sigma_spectrogram,
         badGPStimes,
         delta_sigmas,
+        ifo_1_gates,
+        ifo_1_gate_pad,
+        ifo_2_gates,
+        ifo_2_gate_pad,
     ):
         try:
             naive_sigma_values = delta_sigmas["naive_sigmas"]
             slide_sigma_values = delta_sigmas["slide_sigmas"]
         except KeyError:
             naive_sigma_values = None
             slide_sigma_values = None
@@ -1316,14 +1508,18 @@
             sigma_spectrogram=sigma_spectrogram,
             badGPStimes=badGPStimes,
             delta_sigma_alphas=delta_sigmas["alphas"],
             delta_sigma_times=delta_sigmas["times"],
             delta_sigma_values=delta_sigmas["values"],
             naive_sigma_values=naive_sigma_values,
             slide_sigma_values=slide_sigma_values,
+            ifo_1_gates=ifo_1_gates,
+            ifo_1_gate_pad=ifo_1_gate_pad,
+            ifo_2_gates=ifo_2_gates,
+            ifo_2_gate_pad=ifo_2_gate_pad,
         )
 
     def _pickle_save(
         self,
         filename,
         frequencies,
         frequency_mask,
@@ -1331,26 +1527,34 @@
         sigma_spectrum,
         point_estimate,
         sigma,
         point_estimate_spectrogram,
         sigma_spectrogram,
         badGPStimes,
         delta_sigmas,
+        ifo_1_gates,
+        ifo_1_gate_pad,
+        ifo_2_gates,
+        ifo_2_gate_pad,
     ):
         save_dictionary = {
             "frequencies": frequencies,
             "frequency_mask": frequency_mask,
             "point_estimate_spectrum": point_estimate_spectrum,
             "sigma_spectrum": sigma_spectrum,
             "point_estimate": point_estimate,
             "sigma": sigma,
             "point_estimate_spectrogram": point_estimate_spectrogram,
             "sigma_spectrogram": sigma_spectrogram,
             "badGPStimes": badGPStimes,
             "delta_sigmas": list(delta_sigmas.items()),
+            "ifo_1_gates": ifo_1_gates,
+            "ifo_1_gate_pad": ifo_1_gate_pad,
+            "ifo_2_gates": ifo_2_gates,
+            "ifo_2_gate_pad": ifo_2_gate_pad,
         }
 
         with open(filename, "wb") as f:
             pickle.dump(save_dictionary, f)
 
     def _json_save(
         self,
@@ -1361,14 +1565,18 @@
         sigma_spectrum,
         point_estimate,
         sigma,
         point_estimate_spectrogram,
         sigma_spectrogram,
         badGPStimes,
         delta_sigmas,
+        ifo_1_gates,
+        ifo_1_gate_pad,
+        ifo_2_gates,
+        ifo_2_gate_pad,
     ):
         list_freqs = frequencies.tolist()
         list_freqs_mask = frequency_mask.tolist()
         list_point_estimate_spectrum_r = np.real(point_estimate_spectrum.value).tolist()
         list_point_estimate_spectrum_i = np.imag(point_estimate_spectrum.value).tolist()
         list_sigma_spectrum = sigma_spectrum.value.tolist()
 
@@ -1380,15 +1588,15 @@
         ).tolist()
         point_estimate_segment_times = point_estimate_spectrogram.times.value.tolist()
 
         list_sigma_segment = sigma_spectrogram.value.tolist()
         sigma_segment_times = sigma_spectrogram.times.value.tolist()
 
         badGPStimes_list = badGPStimes.tolist()
-
+        
         save_dictionary = {
             "frequencies": list_freqs,
             "frequency_mask": list_freqs_mask,
             "point_estimate_spectrum_real": list_point_estimate_spectrum_r,
             "point_estimate_spectrum_imag": list_point_estimate_spectrum_i,
             "sigma_spectrum": list_sigma_spectrum,
             "point_estimate": point_estimate,
@@ -1397,14 +1605,18 @@
             "point_estimate_spectrogram_imag": list_point_estimate_segment_i,
             "point_estimate_spectrogram_times": point_estimate_segment_times,
             "sigma_spectrogram": list_sigma_segment,
             "sigma_spectrogram_times": sigma_segment_times,
             "badGPStimes": badGPStimes_list,
             "delta_sigma_alphas": delta_sigmas["alphas"],
             "delta_sigma_values": delta_sigmas["values"].tolist(),
+            "ifo_1_gates": ifo_1_gates,
+            "ifo_1_gate_pad": ifo_1_gate_pad,
+            "ifo_2_gates": ifo_2_gates,
+            "ifo_2_gate_pad": ifo_2_gate_pad,
         }
         try:
             save_dictionary["naive_sigma_values"] = delta_sigmas[
                 "naive_sigmas"
             ].tolist()
             save_dictionary["slide_sigma_values"] = delta_sigmas[
                 "slide_sigmas"
@@ -1424,14 +1636,18 @@
         sigma_spectrum,
         point_estimate,
         sigma,
         point_estimate_spectrogram,
         sigma_spectrogram,
         badGPStimes,
         delta_sigmas,
+        ifo_1_gates,
+        ifo_1_gate_pad,
+        ifo_2_gates,
+        ifo_2_gate_pad,
         compress=False,
     ):
         hf = h5py.File(filename, "w")
 
         if compress:
             compression = "gzip"
             logger.info("Data will be compressed without loss of data")
@@ -1484,27 +1700,40 @@
                 "slide_sigma_values",
                 data=delta_sigmas["slide_sigmas"],
                 compression=compression,
             )
         except KeyError:
             pass
 
+        gates_group = hf.create_group("Gated_Times")
+        gates_group.create_dataset(
+            "ifo_1_gates", data=ifo_1_gates, compression=compression
+        )
+        gates_group.create_dataset(
+            "ifo_2_gates", data=ifo_2_gates, compression=compression
+        )
+
         hf.close()
 
     def _npz_save_csd(
         self,
         filename,
         freqs,
         avg_freqs,
         csd,
         avg_csd,
         psd_1,
         psd_2,
         avg_psd_1,
         avg_psd_2,
+        coherence,
+        psd_1_coh,
+        psd_2_coh,
+        csd_coh,
+        n_segs_coh,
     ):
         np.savez(
             filename,
             freqs=freqs,
             avg_freqs=avg_freqs,
             csd=csd,
             avg_csd=avg_csd,
@@ -1512,38 +1741,53 @@
             psd_2=psd_2,
             avg_psd_1=avg_psd_1,
             avg_psd_2=avg_psd_2,
             csd_times=csd.times.value,
             avg_csd_times=avg_csd.times.value,
             psd_times=psd_1.times.value,
             avg_psd_times=avg_psd_1.times.value,
+            coherence=coherence,
+            psd_1_coh=psd_1_coh,
+            psd_2_coh=psd_2_coh,
+            csd_coh=csd_coh,
+            n_segs_coh=n_segs_coh,
         )
 
     def _pickle_save_csd(
         self,
         filename,
         freqs,
         avg_freqs,
         csd,
         avg_csd,
         psd_1,
         psd_2,
         avg_psd_1,
         avg_psd_2,
+        coherence,
+        psd_1_coh,
+        psd_2_coh,
+        csd_coh,
+        n_segs_coh,
     ):
 
         save_dictionary = {
             "freqs": freqs,
             "avg_freqs": avg_freqs,
             "csd": csd,
             "avg_csd": avg_csd,
             "psd_1": psd_1,
             "psd_2": psd_2,
             "avg_psd_1": avg_psd_1,
             "avg_psd_2": avg_psd_2,
+            "coherence": coherence,
+            "psd_1_coh": psd_1_coh,
+            "psd_2_coh": psd_2_coh,
+            "csd_coh": csd_coh,
+            "n_segs_coh": n_segs_coh,
         }
 
         # with open(filename, "wb") as f:
         #   pickle.dump(saveObject, f)
 
         with open(filename, "wb") as f:
             pickle.dump(save_dictionary, f)
@@ -1555,14 +1799,19 @@
         avg_freqs,
         csd,
         avg_csd,
         psd_1,
         psd_2,
         avg_psd_1,
         avg_psd_2,
+        coherence,
+        psd_1_coh,
+        psd_2_coh,
+        csd_coh,
+        n_segs_coh,
     ):
         """
         It seems that saving spectrograms in json does not work, hence everything is converted into a list and saved that way in the json file.
         A second issue is that json does not seem to recognise complex values, hence the csd is split up into a real and imaginary part.
         When loading in this json file, one needs to 'reconstruct' the csd as a spectrogram using these two lists and the times and frequencies.
         """
         list_freqs = freqs.tolist()
@@ -1591,14 +1840,35 @@
         psd_times = psd_1.times.value.tolist()
         list_psd_2 = psd_2.value.tolist()
         psd_2_times = psd_2.times.value.tolist()
         list_avg_psd_1 = avg_psd_1.value.tolist()
         avg_psd_times = avg_psd_1.times.value.tolist()
         list_avg_psd_2 = avg_psd_2.value.tolist()
         avg_psd_2_times = avg_psd_2.times.value.tolist()
+        if coherence:
+            list_coherence = coherence.value.tolist()
+            list_psd_1_coh = psd_1_coh.value.tolist()
+            list_psd_2_coh = psd_2_coh.value.tolist()
+            list_csd_coh = csd_coh.value.tolist()
+            real_csd_coh = np.zeros(np.shape(list_csd_coh))
+            imag_csd_coh = np.zeros(np.shape(list_csd_coh))
+            for ix, elem in enumerate(list_csd_coh):
+                    real_csd_coh[ix] = elem.real
+                    imag_csd_coh[ix] = elem.imag
+            real_csd_coh_list = real_csd_coh.tolist()
+            imag_csd_coh_list = imag_csd_coh.tolist()
+            list_n_segs_coh = n_segs_coh
+        else:
+            list_coherence = None
+            list_psd_1_coh = None
+            list_psd_2_coh = None
+            list_csd_coh = None
+            real_csd_coh_list = None
+            imag_csd_coh_list = None
+            list_n_segs_coh = None
 
         save_dictionary = {
             "frequencies": list_freqs,
             "avg_frequencies": list_avg_freqs,
             "csd_real": real_csd_list,
             "csd_imag": imag_csd_list,
             "csd_times": csd_times,
@@ -1609,14 +1879,20 @@
             "psd_1_times": psd_times,
             "psd_2": list_psd_2,
             "psd_2_times": psd_2_times,
             "avg_psd_1": list_avg_psd_1,
             "avg_psd_1_times": avg_psd_times,
             "avg_psd_2": list_avg_psd_2,
             "avg_psd_2_times": avg_psd_2_times,
+            "coherence": list_coherence,
+            "psd_1_coh": list_psd_1_coh,
+            "psd_2_coh": list_psd_2_coh,
+            "csd_coh_real": real_csd_coh_list,
+            "csd_coh_imag": real_csd_coh_list,
+            "n_segs_coh": list_n_segs_coh,
         }
 
         with open(filename, "w") as outfile:
             json.dump(save_dictionary, outfile)
 
     def _hdf5_save_csd(
         self,
@@ -1625,14 +1901,19 @@
         avg_freqs,
         csd,
         avg_csd,
         psd_1,
         psd_2,
         avg_psd_1,
         avg_psd_2,
+        coherence,
+        psd_1_coh,
+        psd_2_coh,
+        csd_coh,
+        n_segs_coh,
         compress=False,
     ):
         hf = h5py.File(filename, "w")
 
         csd_times = csd.times.value
         psd_1_times = psd_1.times.value
         psd_2_times = psd_2.times.value
@@ -1686,14 +1967,21 @@
         avg_psd_2_group.create_dataset(
             "avg_psd_2", data=avg_psd_2, compression=compression
         )
         avg_psd_2_group.create_dataset(
             "avg_psd_2_times", data=avg_psd_2_times, compression=compression
         )
 
+        if coherence:
+            hf.create_dataset("coherence", data=coherence, compression=compression)
+            hf.create_dataset("psd_1_coherence", data=psd_1_coh, compression=compression)
+            hf.create_dataset("psd_2_coherence", data=psd_2_coh, compression=compression)
+            hf.create_dataset("csd_coherence", data=csd_coh, compression=compression)
+            hf.create_dataset("n_segs_coherence", data=n_segs_coh, compression=compression)
+
         hf.close()
 
 
 def get_baselines(interferometers, frequencies=None):
     """
     Get set of Baseline objects given a list of interferometers.
     Parameters
```

### Comparing `pygwb-1.0.0/pygwb/delta_sigma_cut.py` & `pygwb-1.3.0/pygwb/delta_sigma_cut.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     alphas: np.ndarray,
     sample_rate: int,
     orf: np.array,
     fref: int,
     frequency_mask: np.array = True,
     window_fftgram_dict: dict = {"window_fftgram": "hann"},
     overlap_factor: float=0.5,
-    N_average_segments_welch_psd = 2,
+    N_average_segments_psd = 2,
     return_naive_and_averaged_sigmas: bool = False,
 ):
 
     """
     Function that runs the delta sigma cut
 
     Parameters
@@ -128,15 +128,15 @@
         overlap_factor=overlap_factor
     )
     # Sliding estimate
     bf_ss = calc_bias(
         segmentDuration=segment_duration,
         deltaF=df,
         deltaT=dt,
-        N_avg_segs=N_average_segments_welch_psd,
+        N_avg_segs=N_average_segments_psd,
         window_fftgram_dict=window_fftgram_dict,
         overlap_factor=overlap_factor
     )
     freqs = np.array(psd1_naive.frequencies)
     overall_cut = np.zeros((ntimes, 1), dtype="bool")
     cuts = np.zeros((nalphas, ntimes), dtype="bool")
     naive_sigmas = np.zeros((nalphas, ntimes))
```

### Comparing `pygwb-1.0.0/pygwb/detector.py` & `pygwb-1.3.0/pygwb/detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -148,14 +148,15 @@
         channel = str(ifo.name + ":" + parameters.channel)
 
         ifo.set_timeseries_from_channel_name(
             channel,
             t0=parameters.t0,
             tf=parameters.tf,
             data_type=parameters.data_type,
+            frametype=parameters.frametype,
             local_data_path=parameters.local_data_path,
             new_sample_rate=parameters.new_sample_rate,
             cutoff_frequency=parameters.cutoff_frequency,
             segment_duration=parameters.segment_duration,
             number_cropped_seconds=parameters.number_cropped_seconds,
             window_downsampling=parameters.window_downsampling,
             ftype=parameters.ftype,
@@ -177,14 +178,15 @@
         **kwargs : keyword arguments passed to preprocess module.
 
         """
 
         t0 = kwargs.pop("t0")
         tf = kwargs.pop("tf")
         data_type = kwargs.pop("data_type")
+        frametype = kwargs.pop("frametype")
         local_data_path = kwargs.pop("local_data_path")
         new_sample_rate = kwargs.pop("new_sample_rate")
         input_sample_rate = kwargs.pop("input_sample_rate")
         cutoff_frequency = kwargs.pop("cutoff_frequency")
         segment_duration = kwargs.pop("segment_duration")
         number_cropped_seconds = kwargs.pop("number_cropped_seconds")
         window_downsampling = kwargs.pop("window_downsampling")
@@ -194,14 +196,15 @@
         self.duration = segment_duration
         self.timeseries = preprocessing_data_channel_name(
             IFO=self.name,
             channel=channel,
             t0=t0,
             tf=tf,
             data_type=data_type,
+            frametype=frametype,
             local_data_path=local_data_path,
             new_sample_rate=new_sample_rate,
             cutoff_frequency=cutoff_frequency,
             segment_duration=segment_duration,
             number_cropped_seconds=number_cropped_seconds,
             window_downsampling=window_downsampling,
             ftype=ftype,
@@ -290,62 +293,72 @@
         self.timeseries.channel = kwargs.pop("channel")
         self._check_timeseries_sample_rate(new_sample_rate)
         self.sampling_frequency = new_sample_rate
 
     def set_psd_spectrogram(
         self,
         frequency_resolution,
+        coarse_grain=False,
         overlap_factor=0.5,
-        window_fftgram_dict_welch_psd={"window_fftgram": "hann"},
-        overlap_factor_welch_psd=0.5,
+        window_fftgram_dict={"window_fftgram": "hann"},
+        overlap_factor_welch=0.5,
     ):
         """
         Set psd_spectrogram attribute from a given spectrum-related information.
 
         Parameters
         ==========
         frequency_resolution: float
             Frequency resolution of the final PSDs; This sets the time duration
             over which FFTs are calculated in the pwelch method
+        coarse_grain: bool
+            Coarse-graining flag; if True, PSD will be estimated via coarse-graining
+            as opposed to Welch-averaging. Default is False.
         overlap_factor: float, optional
             Amount of overlap between adjacent segments (range between 0 and 1)
             This factor should be same as the one used for cross_spectral_density
             (default 0, no overlap)
-        window_fftgram_dict_welch_psd: dictionary, optional
-            Dictionary containing name and parameters describing which window to use when producing fftgrams for welch psd estimation. Default is \"hann\".
+        window_fftgram_dict: dictionary, optional
+            Dictionary containing name and parameters describing which window to use when producing fftgrams for psd estimation. Default is \"hann\".
+        overlap_factor_welch: float, optional
+            Overlap factor to use when if using Welch's method to estimate the PSD (NOT coarsegraining). For \"hann\" window use 0.5 overlap_factor and for \"boxcar"\ window use 0 overlap_factor. Default is 0.5 (50% overlap), which is optimal when using Welch's method with a \"hann\" window.
 
         """
 
-        # psd_array = spectral.psd(self.timeseries, frequencies)
+        # PSD estimation needs zeropadding when using coarse-graining
+        zeropad_psd = coarse_grain
+
         self.psd_spectrogram = power_spectral_density(
             self.timeseries,
             self.duration,
             frequency_resolution,
+            coarse_grain=coarse_grain,
+            zeropad=zeropad_psd,
             overlap_factor=overlap_factor,
-            window_fftgram_dict_welch_psd=window_fftgram_dict_welch_psd,
-            overlap_factor_welch_psd=overlap_factor_welch_psd,
+            window_fftgram_dict=window_fftgram_dict,
+            overlap_factor_welch=overlap_factor_welch,
         )
         self.psd_spectrogram.channel = self.timeseries.channel
         self._check_spectrogram_channel_name(self.timeseries.channel.name)
         self._check_spectrogram_frequency_resolution(frequency_resolution)
 
-    def set_average_psd(self, N_average_segments_welch_psd=2):
+    def set_average_psd(self, N_average_segments=2):
         """
         Set average_psd attribute from the existing raw psd
 
         Parameters
         ==========
-        N_average_segments_welch_psd : int
+        N_average_segments: int
             Number of segments used for PSD averaging (from both sides of the segment of interest)
             N_avg_segs should be even and >= 2
 
         """
         try:
             self.average_psd = before_after_average(
-                self.psd_spectrogram, self.duration, N_average_segments_welch_psd
+                self.psd_spectrogram, self.duration, N_average_segments
             )
         except AttributeError:
             print(
                 "PSDs have not been calculated yet! Need to set_psd_spectrogram first."
             )
 
     def gate_data_apply(self, **kwargs):
@@ -383,14 +396,41 @@
             gate_threshold=gate_threshold,
             cluster_window=cluster_window,
             whiten=gate_whiten,
         )
         self.gates = self.gates | new_gates
         self.gate_pad = gate_tpad
 
+    def apply_gates_from_file(self, loaded_object, index, **kwargs):
+        """
+        Load gates from a pygwb output file and apply them to the Interferometer object. 
+        The gated times are stored as a property of the object.
+        
+        Parameters
+        ==========
+        loaded_object : 
+            Object that represents the data in the output file, e.g. a loaded npzobject.
+        index ; int
+            Integer representing the correct ifo object in the baseline
+        gate_tpad : float
+            half-width time duration (seconds) in which the Planck window
+            is tapered
+        """
+        gates = loaded_object[f"ifo_{index}_gates"]
+        gate_tpad = kwargs.pop("gate_tpad")
+
+        self.timeseries, new_gates = self_gate_data(
+            self.timeseries,
+            tpad=gate_tpad,
+            gates=gates,
+        )
+
+        self.gates = self.gates | new_gates
+        self.gate_pad = gate_tpad
+
     def _check_ifo_name(self, name):
         if not self.name == name:
             raise AssertionError(
                 "The ifo name in Interferomaeter class does not match given name!"
             )
 
     def _check_timeseries_channel_name(self, channel_name):
```

### Comparing `pygwb-1.0.0/pygwb/html.py` & `pygwb-1.3.0/pygwb/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import gwsumm.plot
 import gwsumm.tabs
 from gwpy.time import from_gps
 
 """Create pygwb html
 """
 
-def pygwb_html(outdir='./', config=None):
+def pygwb_html(outdir='./', config=None, segment_results=False):
 
     # =====================
     # get data
     
     ifo = 'Network'
     # =====================
     # now make the html page
@@ -37,46 +37,46 @@
     home_index = os.path.join(output_dir,'index.html')
 
     plot_sub_dir = os.path.join(output_dir, 'output/combined_results')
     home_plots = glob.glob(plot_sub_dir+'/*.png')
     home_plots = sorted(home_plots)
     home_plots = ['/'.join(plot_loc.split('/')[-3:]) for plot_loc in home_plots]
     
-    plot_tab = gwsumm.tabs.PlotTab('Stochmon combined results',path=output_dir,index=home_index)
+    plot_tab = gwsumm.tabs.PlotTab('pygwb combined results',path=output_dir,index=home_index)
     plot_tab.set_layout((2,2))
     for plot_name in home_plots:
         plot = gwsumm.plot.core.SummaryPlot(href='./'+os.path.join(output_dir,plot_name))
 
         plot_tab.add_plot(plot)
     base_tabs.append(plot_tab)
     tabs.append(plot_tab)
 
     seg_tabs = []
-    segment_folders = glob.glob(output_dir+'/output/*-*')
-    for i, seg_folder in enumerate(segment_folders):
-        page_name = seg_folder.split('/')[-1].split('-')[0]
-        page_name = from_gps(int(page_name)).strftime('%Y-%m-%d %H:%M:%S')
-        if i==0:
-            tab0 = gwsumm.tabs.PlotTab(page_name,
-                                       path=output_dir,parent='Segment results')
-            tab = tab0
-        else:
-            tab = gwsumm.tabs.PlotTab(page_name,
-                                      path=output_dir,parent=tab0.parent)
-
-        seg_plots = glob.glob(seg_folder+'/*.png')
-        seg_plots = sorted(seg_plots)
-        seg_plots = ['/'.join(plot_loc.split('/')[-3:]) for plot_loc in seg_plots]
-        for plot_name in seg_plots:
-            plot = gwsumm.plot.core.SummaryPlot(href='./'+os.path.join(output_dir,plot_name))
-            tab.add_plot(plot)
-        tab.set_layout((2))
-        seg_tabs.append(tab)
-        tabs.append(tab)
-
+    if segment_results:
+        segment_folders = glob.glob(output_dir+'/output/*-*')
+        for i, seg_folder in enumerate(segment_folders):
+            page_name = seg_folder.split('/')[-1].split('-')[0]
+            page_name = from_gps(int(page_name)).strftime('%Y-%m-%d %H:%M:%S')
+            if i==0:
+                tab0 = gwsumm.tabs.PlotTab(page_name,
+                                           path=output_dir,parent='Segment results')
+                tab = tab0
+            else:
+                tab = gwsumm.tabs.PlotTab(page_name,
+                                          path=output_dir,parent=tab0.parent)
+
+            seg_plots = glob.glob(seg_folder+'/*.png')
+            seg_plots = sorted(seg_plots)
+            seg_plots = ['/'.join(plot_loc.split('/')[-3:]) for plot_loc in seg_plots]
+            for plot_name in seg_plots:
+                plot = gwsumm.plot.core.SummaryPlot(href='./'+os.path.join(output_dir,plot_name))
+                tab.add_plot(plot)
+            tab.set_layout((2))
+            seg_tabs.append(tab)
+            tabs.append(tab)
     
     about_tab = gwsumm.tabs.AboutTab('About',path=output_dir)
     about_href = about_tab.href
     
     # Write out tabs
     logging.info('Writing html of tabs...')
     for tab in base_tabs:
@@ -99,16 +99,18 @@
                         help='increase verbose output')
     parser.add_argument('-V', '--version', action='version',
                         version=__version__)
     parser.add_argument('-o', '--output-dir', type=os.path.abspath,
                         help='Directory for all output')
     parser.add_argument('-p', '--plot-dir', type=os.path.abspath,
                         help='Directory of plots to show')
+    parser.add_argument('--plot-segment-results', action='store_true',
+                        help='Create result pages for every segment')
     args = parser.parse_args(args=args)
 
     # call the above function
-    pygwb_html(outdir=args.output_dir)
+    pygwb_html(outdir=args.output_dir, segment_results=args.plot_segment_results)
 
 # allow be be run on the command line
 if __name__ == "__main__":
     main(args=None)
```

### Comparing `pygwb-1.0.0/pygwb/network.py` & `pygwb-1.3.0/pygwb/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,22 @@
     def __init__(
         self,
         name,
         interferometers,
         duration=None,
         frequencies=None,
         calibration_epsilon=0,
-        notch_list_path=None,
+        notch_list_path="",
+        coarse_grain_psd=False,
+        coarse_grain_csd=True,
+        overlap_factor_welch=0.5,
         overlap_factor=0.5,
-        zeropad_csd=True,
         window_fftgram_dict={"window_fftgram": "hann"},
-        N_average_segments_welch_psd=2,
+        window_fftgram_dict_welch={"window_fftgram": "hann"},
+        N_average_segments_psd=2,
     ):
         """
         Instantiate a Network object.
 
         Parameters
         ----------
         name: str
@@ -49,21 +52,28 @@
         frequencies: array_like, optional
             the frequency array for the Baseline and
             interferometers
         calibration_epsilon: float, optional
             calibration uncertainty for this baseline -- currently only supports a single notch list for all baselines
         notch_list_path: str, optional
             file path of the baseline notch list -- currently only supports a single notch list for all baselines
+        coarse_grain_psd: bool
+            Whether to apply coarse graining to obtain PSD spectra. Default is False.
+        coarse_grain_csd: bool
+            Whether to apply coarse graining to obtain CSD spectra. Default is True.
+        overlap_factor_welch: float, optional
+            Overlap factor to use when if using Welch's method to estimate spectra (NOT coarsegraining). For \"hann\" window use 0.5 overlap_factor and for \"boxcar"\ window use 0 overlap_factor. Default is 0.5 (50% overlap), which is optimal when using Welch's method with a \"hann\" window.
         overlap_factor: float, optional
-            factor by which to overlap the segments in the psd and csd estimation. Default is 1/2, if set to 0 no overlap is performed.
-        zeropad_csd: bool, optional
-            if True, applies zeropadding in the csd estimation. True by default.
+            Factor by which to overlap the segments in the psd and csd estimation.
+            Default is 1/2, if set to 0 no overlap is performed.
         window_fftgram_dict: dictionary, optional
-            Dictionary containing name and parameters describing which window to use when producing fftgrams for psds and csds. Default is \"hann\".
-        N_average_segments_welch_psd: int, optional
+            Dictionary containing name and parameters describing which window to use when producing fftgrams for csds (and psds if these are coarse-grained). Default is \"hann\".
+        window_fftgram_dict_welch: dictionary, optional
+            Dictionary containing name and parameters describing which window to use when producing fftgrams with Welch's method. Default is \"hann\".
+        N_average_segments_psd: int, optional
             Number of segments used for PSD averaging (from both sides of the segment of interest)
             N_avg_segs should be even and >= 2
         """
         self.name = name
         self.interferometers = interferometers
         self.Nifo = len(interferometers)
         self.set_duration(duration)
@@ -83,18 +93,21 @@
                     base_name,
                     self.interferometers[i],
                     self.interferometers[j],
                     duration=duration,
                     frequencies=frequencies,
                     calibration_epsilon=calibration_epsilon,
                     notch_list_path=notch_list_path,
+                    coarse_grain_psd=coarse_grain_psd,
+                    coarse_grain_csd=coarse_grain_csd,
+                    overlap_factor_welch=overlap_factor_welch,
                     overlap_factor=overlap_factor,
-                    zeropad_csd=zeropad_csd,
                     window_fftgram_dict=window_fftgram_dict,
-                    N_average_segments_welch_psd=N_average_segments_welch_psd,
+                    window_fftgram_dict_welch=window_fftgram_dict_welch,
+                    N_average_segments_psd=N_average_segments_psd,
                 )
             )
 
         self.baselines = baselines
 
     @classmethod
     def from_baselines(cls, name, baselines):
@@ -230,15 +243,15 @@
                 )
 
         data_simulator = Simulator(
             self.interferometers,
             N_segments,
             duration=self.duration,
             intensity_GW=GWB_intensity,
-            injection_dict=CBC_dict, 
+            injection_dict=CBC_dict,
             start_time=start_time,
             sampling_frequency=sampling_frequency,
             no_noise=no_noise,
         )
         data = data_simulator.get_data_for_interferometers()
 
         if inject_into_data_flag:
```

### Comparing `pygwb-1.0.0/pygwb/notch.py` & `pygwb-1.3.0/pygwb/notch.py`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb/omega_spectra.py` & `pygwb-1.3.0/pygwb/omega_spectra.py`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb/orfs.py` & `pygwb-1.3.0/pygwb/orfs.py`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb/parameters.py` & `pygwb-1.3.0/pygwb/parameters.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,18 +16,22 @@
 
     Attributes
     ----------
     t0 : float
         Initial time.
     tf: float
         Final time.
+    interferometer_list: list
+        List of interferometers to run the analysis with. Default is [\"H1\", \"L1\"]
     data_type: str
         Type of data to access/download; options are private, public, local. Default is public.
     channel: str
         Channel name; needs to match an existing channel. Default is \"GWOSC-16KHZ_R1_STRAIN\"
+    frametype: str
+        Frame type; Optional, desired channel needs to be found in listed frametype. Only used when data_type=private. Default is empty.
     new_sample_rate: int
         Sample rate to use when downsampling the data (Hz). Default is 4096 Hz.
     input_sample_rate: int
         Sample rate of the read data (Hz). Default is 16384 Hz.
     cutoff_frequency: int
         Lower frequency cutoff; applied in filtering in preprocessing (Hz). Default is 11 Hz.
     segment_duration: int
@@ -46,40 +50,46 @@
         Spectral index to filter the data for. Default is 0.
     fref: int
         Reference frequency to filter the data at (Hz). Default is 25 Hz.
     flow: int
         Lower frequency to include in the analysis (Hz). Default is 20 Hz.
     fhigh: int
         Higher frequency to include in the analysis (Hz). Default is 1726 Hz.
-    coarse_grain: bool
-        Whether to apply coarse graining to the spectra. Default is 0.
-    interferometer_list: list
-        List of interferometers to run the analysis with. Default is [\"H1\", \"L1\"]
     local_data_path: str
         Path(s) to local data, if the local data option is chosen. Default is empty.
     notch_list_path: str
         Path to the notch list file. Default is empty.
-    N_average_segments_welch_psd: int
+    coarse_grain_psd: bool
+        Whether to apply coarse graining to obtain PSD spectra. Default is False.
+    coarse_grain_csd: bool
+        Whether to apply coarse graining to obtain CSD spectra. Default is True.
+    overlap_factor_welch: float
+        Overlap factor to use when if using Welch's method to estimate spectra (NOT coarsegraining). For \"hann\" window use 0.5 overlap_factor and for \"boxcar\" window use 0 overlap_factor. Default is 0.5 (50% overlap), which is optimal when using Welch's method with a \"hann\" window.
+        Whether to apply coarse graining to obtain CSD spectra. Default is True.
+    N_average_segments_psd: int
         Number of segments to average over when calculating the psd with Welch method. Default is 2.
     window_fft_dict: dict
         Dictionary containing name and parameters describing which window to use when producing fftgrams for psds and csds. Default is \"hann\".
+    window_fft_dict_welch: dict 
+        Dictionary containing name and parameters relative to which window to use when producing fftgrams for pwelch calculation. Default is "hann".
     calibration_epsilon: float
         Calibation coefficient. Default is 0.
     overlap_factor: float
         Factor by which to overlap consecutive segments for analysis. Default is 0.5 (50%% overlap)
-    zeropad_csd: bool
-        Whether to zeropad the csd or not. Default is True.
     delta_sigma_cut: float
         Cutoff value for the delta sigma cut. Default is 0.2.
     alphas_delta_sigma_cut: list
         List of spectral indexes to use in delta sigma cut calculation. Default is [-5, 0, 3].
     save_data_type: str
         Suffix for the output data file. Options are hdf5, npz, json, pickle. Default is json.
     time_shift: int
         Seconds to timeshift the data by in preprocessing. Default is 0.
+    path_gate_data: str
+        Path to the map with pygwb output containing information about gates. If loading a single file, it has to be an .npzfile 
+        with the same structure as a pygwb output file. Default is an empty string.
     gate_data: bool
         Whether to apply self-gating to the data in preprocessing. Default is False.
     gate_tzero: float
         Gate tzero. Default is 1.0.
     gate_tpad: float
         Gate tpad. Default is 0.5.
     gate_threshold: float
@@ -94,49 +104,53 @@
         option to return naive and sliding sigmas from delta sigma cut
     window_fftgram_dict: dictionary, optional
         Dictionary with window characteristics. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
     """
 
     t0: float = 0
     tf: float = 100
+    interferometer_list: List = field(default_factory=lambda: ["H1", "L1"])
     data_type: str = "public"
     channel: str = "GWOSC-16KHZ_R1_STRAIN"
+    frametype: str = ""
     new_sample_rate: int = 4096
     input_sample_rate: int = 16384
     cutoff_frequency: float = 11
     segment_duration: int = 192
     number_cropped_seconds: int = 2
     window_downsampling: str = "hamming"
     ftype: str = "fir"
     frequency_resolution: float = 0.03125
     polarization: str = "tensor"
     alpha: float = 0
     fref: float = 25
     flow: float = 20
     fhigh: float = 1726
-    coarse_grain: bool = False
-    interferometer_list: List = field(default_factory=lambda: ["H1", "L1"])
     local_data_path: str = ""
     notch_list_path: str = ""
-    N_average_segments_welch_psd: int = 2
+    coarse_grain_psd: bool = False
+    coarse_grain_csd: bool = True
+    overlap_factor_welch: float = 0.5
+    N_average_segments_psd: int = 2
     window_fft_dict: dict = field(default_factory=lambda: {"window_fftgram": "hann"})
+    window_fft_dict_welch: dict = field(default_factory=lambda: {"window_fftgram": "hann"})
     calibration_epsilon: float = 0
     overlap_factor: float = 0.5
-    zeropad_csd: bool = True
     delta_sigma_cut: float = 0.2
     alphas_delta_sigma_cut: List = field(default_factory=lambda: [-5, 0, 3])
     save_data_type: str = "npz"
     time_shift: int = 0
+    path_gate_data: str = ""
     gate_data: bool = False
     gate_tzero: float = 1.0
     gate_tpad: float = 0.5
     gate_threshold: float = 50.0
     cluster_window: float = 0.5
     gate_whiten: bool = True
-    tag: str = "C00"
+    tag: str = ""
     return_naive_and_averaged_sigmas: bool = False
 
 
     def update_from_dictionary(self, kwargs):
         """Update parameters from a dictionary
 
         Parameters
@@ -144,15 +158,15 @@
         kwargs: dictionary
             Dictionary of parameters to update.
         """
         ann = getattr(self, "__annotations__", {})
         for name, dtype in ann.items():
             if name in kwargs:
                 try:
-                    if not bool(re.search("\{*\}", kwargs[name])): 
+                    if not bool(re.search("^.+:.+,.+:.+$", kwargs[name])): 
                         kwargs[name] = dtype(kwargs[name]) if kwargs[name] != 'False' else False
                 except TypeError:
                     pass
                 setattr(self, name, kwargs[name])
         for name in kwargs:
             if name not in ann.keys():
                 warnings.warn(
@@ -184,14 +198,15 @@
                 dictionary["alphas_delta_sigma_cut"]
             )
         if dictionary["interferometer_list"]:
             dictionary["interferometer_list"] = json5.loads(
                 dictionary["interferometer_list"]
             )
         dictionary["window_fft_dict"] = dict(config.items("window_fft_specs"))
+        dictionary["window_fft_dict_welch"] = dict(config.items("window_fft_welch_specs"))
         for item in dictionary.copy():
             if not dictionary[item]:
                 dictionary.pop(item)
         self.update_from_dictionary(dictionary)
 
     def update_from_arguments(self, args: List[str]) -> None:
         """Update parameters from a set of arguments
@@ -206,36 +221,56 @@
         -----
         Not all possible options are available through argument updating. The two exceptions are the dictionary
         attributes which can not be parsed easily by argparse. These are
         * window_fft_dict: this is composed by the single argument
             -- window_fftgram
         This is the only option currently supported. To use windows that require extra parameters, pass these as part of an
         .ini file, in the relevant section [window_fft_specs].
+        * window_fft_dict_welch: this is composed by the single argument
+            -- window_fftgram_welch
         """
         if not args:
             return
         ann = getattr(self, "__annotations__", {})
         parser = argparse.ArgumentParser()
         for name, dtype in ann.items():
             if dtype == List:
                 parser.add_argument(f"--{name}", type=str, nargs='+', required=False)
             else:
-                parser.add_argument(f"--{name}", type=dtype, required=False)
+                parser.add_argument(f"--{name}", type=str, required=False)
 
         parser.add_argument("--window_fftgram", type=str, required=False)
+        parser.add_argument("--window_fftgram_welch", type=str, required=False)
         parsed, _ = parser.parse_known_args(args)
         dictionary = vars(parsed)
         for item in dictionary.copy():
             if dictionary[item] is None:
                 dictionary.pop(item)
         if "window_fftgram" in dictionary:
             window_fft_dict = {}
-            window_fft_dict["window_fftgram"] = dictionary["window_fftgram"]
-            dictionary.pop("window_fftgram")
+            wfgram_name, *wfgram = dictionary.pop("window_fftgram").split(',')
+            window_fft_dict["window_fftgram"] = wfgram_name
+            if wfgram_name.lower()=='tukey':
+                window_fft_dict["alpha"] = wfgram[0]
+            elif wfgram_name.lower()=='hann':
+                pass
+            else: 
+                raise ValueError(f"Window {wfgram_name} not supported from command line! Please try submitting through a full parameter ini file.")
             dictionary["window_fft_dict"] = window_fft_dict
+        if "window_fftgram_welch" in dictionary:
+            window_fft_dict_welch = {}
+            wfgram_name_welch, *wfgram_welch = dictionary.pop("window_fftgram_welch").split(',')
+            window_fft_dict_welch["window_fftgram"] = wfgram_name_welch
+            if wfgram_name_welch.lower()=='tukey':
+                window_fft_dict_welch["alpha"] = wfgram[0]
+            elif wfgram_name_welch.lower()=='hann':
+                pass
+            else: 
+                raise ValueError(f"Window {wfgram_name_welch} not supported from command line! Please try submitting through a full parameter ini file.")
+            dictionary["window_fft_dict_welch"] = window_fft_dict_welch
         self.update_from_dictionary(dictionary)
 
     def save_paramfile(self, output_path):
         """Save parameters to a parameters ini file.
 
         Parameters
         ----------
@@ -244,19 +279,20 @@
         """
         param = configparser.ConfigParser()
         param.optionxform = str
         param_dict = asdict(self)
         # for key, value in param_dict.items():
         #    param_dict[key] = str(value)
         data_specs_dict = {}
-        data_specs_dict["interferometer_list"] = param_dict["interferometer_list"]
         data_specs_dict["t0"] = param_dict["t0"]
         data_specs_dict["tf"] = param_dict["tf"]
+        data_specs_dict["interferometer_list"] = param_dict["interferometer_list"]
         data_specs_dict["data_type"] = param_dict["data_type"]
         data_specs_dict["channel"] = param_dict["channel"]
+        data_specs_dict["frametype"] = param_dict["frametype"]
         data_specs_dict["time_shift"] = param_dict["time_shift"]
         param["data_specs"] = data_specs_dict
 
         preprocessing_dict = {}
         preprocessing_dict["new_sample_rate"] = param_dict["new_sample_rate"]
         preprocessing_dict["cutoff_frequency"] = param_dict["cutoff_frequency"]
         preprocessing_dict["segment_duration"] = param_dict["segment_duration"]
@@ -264,34 +300,37 @@
             "number_cropped_seconds"
         ]
         preprocessing_dict["window_downsampling"] = param_dict["window_downsampling"]
         preprocessing_dict["ftype"] = param_dict["ftype"]
         param["preprocessing"] = preprocessing_dict
         
         gating_dict = {}
+        gating_dict["path_gate_data"] = param_dict["path_gate_data"]
         gating_dict["gate_data"] = param_dict["gate_data"]
         gating_dict["gate_whiten"] = param_dict["gate_whiten"]
         gating_dict["gate_tzero"] = param_dict["gate_tzero"]
         gating_dict["gate_tpad"] = param_dict["gate_tpad"]
         gating_dict["gate_threshold"] = param_dict["gate_threshold"]
         gating_dict["cluster_window"] = param_dict["cluster_window"]
         param["gating"] = gating_dict
 
         param["window_fft_specs"] = self.window_fft_dict
+        param["window_fft_welch_specs"] = self.window_fft_dict_welch
 
         density_estimation_dict = {}
         density_estimation_dict["frequency_resolution"] = param_dict[
             "frequency_resolution"
         ]
-        density_estimation_dict["N_average_segments_welch_psd"] = param_dict[
-            "N_average_segments_welch_psd"
+        density_estimation_dict["N_average_segments_psd"] = param_dict[
+            "N_average_segments_psd"
         ]
-        density_estimation_dict["coarse_grain"] = param_dict["coarse_grain"]
+        density_estimation_dict["coarse_grain_psd"] = param_dict["coarse_grain_psd"]
+        density_estimation_dict["coarse_grain_csd"] = param_dict["coarse_grain_csd"]
+        density_estimation_dict["overlap_factor_welch"] = param_dict["overlap_factor_welch"]
         density_estimation_dict["overlap_factor"] = param_dict["overlap_factor"]
-        density_estimation_dict["zeropad_csd"] = param_dict["zeropad_csd"]
         param["density_estimation"] = density_estimation_dict
 
         postprocessing_dict = {}
         postprocessing_dict["polarization"] = param_dict["polarization"]
         postprocessing_dict["alpha"] = param_dict["alpha"]
         postprocessing_dict["fref"] = param_dict["fref"]
         postprocessing_dict["flow"] = param_dict["flow"]
@@ -318,40 +357,49 @@
         output_dict["save_data_type"] = param_dict["save_data_type"]
         param["output"] = output_dict
 
         with open(output_path, "w") as configfile:
             param.write(configfile)
 
     def parse_ifo_parameters(self):
+        ifo_parameters = ['channel', 'frametype', 'input_sample_rate', 'local_data_path', 'time_shift']
         ifo_list = self.interferometer_list
         param_dict = {}
         for ifo in ifo_list:
             param_dict[ifo] = Parameters()
         current_param_dict = self.__dict__
         for attr in current_param_dict.keys():
-            if bool(re.search("\{*\}", str(current_param_dict[attr]))) and type(current_param_dict[attr]) is not dict:
-                attr_str = str(current_param_dict[attr]).replace("{","").replace("}","")
-                attr_split = attr_str.split()
-                attr_dict = {key: value for key, value in (pair.split(':') for pair in attr_split)} 
-                for ifo in ifo_list:
-                    param_dict[ifo].update_from_dictionary({attr: attr_dict[ifo]})
+            if attr in ifo_parameters:
+                attr_str = str(current_param_dict[attr])
+                attr_split = attr_str.split(',')
+                if len(attr_split)>1:
+                    attr_dict = {key: value for key, value in (pair.split(':') for pair in attr_split)} 
+                    for ifo in ifo_list:
+                        param_dict[ifo].update_from_dictionary({attr: attr_dict[ifo]})
+                else:
+                    for ifo in ifo_list:
+                        param_dict[ifo].update_from_dictionary({attr: current_param_dict[attr]})
             else:
                 for ifo in ifo_list:
                     param_dict[ifo].update_from_dictionary({attr: current_param_dict[attr]})
 
         return param_dict
 
 
 class ParametersHelp(enum.Enum):
     """Description of the arguments in the Parameters class. This is an enumeration class and is not meant for user interaction."""
 
     t0 = "Initial time."
     tf = "Final time."
+    interferometer_list = (
+        'List of interferometers to run the analysis with. Default is ["H1", "L1"]'
+    )
     data_type = "Type of data to access/download; options are private, public, local. Default is public."
     channel = 'Channel name; needs to match an existing channel. Default is "GWOSC-16KHZ_R1_STRAIN" '
+    frametype = 'Frame type; Optional, desired channel needs to be found in listed frametype. Only used when data_type=private. Default is empty. '
     new_sample_rate = (
         "Sample rate to use when downsampling the data (Hz). Default is 4096 Hz."
     )
     input_sample_rate = "Sample rate of the read data (Hz). Default is 16384 Hz."
     cutoff_frequency = "Lower frequency cutoff; applied in filtering in preprocessing (Hz). Default is 11 Hz."
     segment_duration = "Duration of the individual segments to analyse (seconds). Default is 192 seconds."
     number_cropped_seconds = "Number of seconds to crop at the start and end of the analysed data (seconds). Default is 2 seconds."
@@ -361,29 +409,32 @@
         "Frequency resolution of the final output spectrum (Hz). Default is 1\/32 Hz."
     )
     polarization = "Polarisation type for the overlap reduction function calculation; options are scalar, vector, tensor. Default is tensor."
     alpha = "Spectral index to filter the data for. Default is 0."
     fref = "Reference frequency to filter the data at (Hz). Default is 25 Hz."
     flow = "Lower frequency to include in the analysis (Hz). Default is 20 Hz."
     fhigh = "Higher frequency to include in the analysis (Hz). Default is 1726 Hz."
-    coarse_grain = "Whether to apply coarse graining to the spectra. Default is 0."
-    interferometer_list = (
-        'List of interferometers to run the analysis with. Default is ["H1", "L1"]'
-    )
     local_data_path = "Path(s) to local data, if the local data option is chosen. Default is empty."
     notch_list_path = "Path to the notch list file. Default is empty."
-    N_average_segments_welch_psd = "Number of segments to average over when calculating the psd with Welch method. Default is 2."
+    coarse_grain_psd = "Whether to apply coarse graining to obtain PSD spectra. Default is False."
+    coarse_grain_csd = "Whether to apply coarse graining to obtain CSD spectra. Default is True."
+    overlap_factor_welch = "Overlap factor to use when if using Welch's method to estimate spectra (NOT coarsegraining). For \"hann\" window use 0.5 overlap_factor and for \"boxcar\" window use 0 overlap_factor. Default is 0.5 (50%% overlap), which is optimal when using Welch's method with a \"hann\" window."
+    N_average_segments_psd = "Number of segments to average over when calculating the psd with Welch's method. Default is 2."
     window_fft_dict = 'Dictionary containing name and parameters relative to which window to use when producing fftgrams for psds and csds. Default is "hann".'
+    window_fft_dict_welch = 'Dictionary containing name and parameters relative to which window to use when producing fftgrams for pwelch calculation. Default is "hann".'
     calibration_epsilon = "Calibation coefficient. Default is 0."
     overlap_factor = "Factor by which to overlap consecutive segments for analysis. Default is 0.5 (50%% overlap)"
-    zeropad_csd = "Whether to zeropad the csd or not. Default is True."
     delta_sigma_cut = "Cutoff value for the delta sigma cut. Default is 0.2."
     alphas_delta_sigma_cut = "List of spectral indexes to use in delta sigma cut calculation. Default is [-5, 0, 3]."
     save_data_type = "Suffix for the output data file. Options are hdf5, npz, json, pickle. Default is json."
     time_shift = "Seconds to timeshift the data by in preprocessing. Default is 0."
+    path_gate_data = (
+        "Path to the pygwb output containing information about gates. If loading a single file, it has to be an .npzfile "
+        "with the same structure as a pygwb output file. Default is an empty string."
+    )
     gate_data = (
         "Whether to apply self-gating to the data in preprocessing. Default is False."
     )
     gate_tzero = "Gate tzero. Default is 1.0."
     gate_tpad = "Gate tpad. Default is 0.5."
     gate_threshold = "Gate threshold. Default is 50."
     cluster_window = "Cluster window. Default is 0.5."
```

### Comparing `pygwb-1.0.0/pygwb/pe.py` & `pygwb-1.3.0/pygwb/pe.py`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb/postprocessing.py` & `pygwb-1.3.0/pygwb/postprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     Y_fs,
     var_fs,
     segment_duration,
     deltaF,
     new_sample_rate,
     frequency_mask=True,
     badtimes_mask=None,
-    do_overlap=True,
     window_fftgram_dict={"window_fftgram": "hann"},
+    window_fftgram_dict_welch={"window_fftgram": "hann"},
     overlap_factor=0.5,
+    overlap_factor_welch=0.5,
     N_avg_segs=2,
 ):
     """Run postprocessing of point estimate and sigma spectrograms, combining even and
     odd segments in the case of overlapping data. For more details see - https://dcc.ligo.org/public/0027/T040089/000/T040089-00.pdf
 
     Parameters:
     -----------
@@ -36,16 +37,14 @@
         Frequency resolution
     new_sample_rate : float
         sample rate of timeseries after resampling
     frequency_mask: array-like, optional
         Boolean mask to apply to frequencies for the calculation. Defaults to True which includes all frequencies in the analysis.
     badtimes_mask: array-like, optional
         Boolean mask to apply to GPStimes in the calculation. Defaults to None such that all times are included.
-    do_overlap: bool, optional
-        Indicates whether to proceed with the odd/even postprocessing calculation which assumes a 50\% overlap between consecutive segments. Default is True.
     window_fftgram_dict: dictionary, optional
         Dictionary with window characteristics used in PSD estimation. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
     overlap_factor: float, optional
         Overlap factor used in PSD estimation. Default is 0.5.
 
     Returns:
     --------
@@ -63,15 +62,15 @@
     Y_fs_sliced = []
     var_fs_sliced = []
 
     for sli in ndi.find_objects(labels):
         Y = Y_fs[sli]
         var = var_fs[sli]
 
-        if len(Y) == 1 or not do_overlap:
+        if len(Y) == 1:
             Y_fs_sliced.append(Y[0])
             var_fs_sliced.append(var[0])
         else:
             Y_red, var_red = odd_even_segment_postprocessing(
                 Y,
                 var,
                 segment_duration,
@@ -92,16 +91,16 @@
     )
 
     bias = calc_bias(
         segment_duration,
         deltaF,
         1 / new_sample_rate,
         N_avg_segs=N_avg_segs,
-        window_fftgram_dict=window_fftgram_dict,
-        overlap_factor=overlap_factor,
+        window_fftgram_dict=window_fftgram_dict_welch,
+        overlap_factor=overlap_factor_welch,
     )
     logger.debug(f"Bias factor: {bias}")
     sigma_f_new *= bias
 
     return Y_f_new, sigma_f_new
 
 
@@ -300,25 +299,26 @@
     orf: array_like
         Overlap reduction function.
     sample_rate: float
         Sampling rate of the data.
     segment_duration: float
         Duration of each segment in seconds.
     window_fftgram_dict: dictionary, optional
-        Dictionary with window characteristics used in PSD estimation. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
+        Dictionary with window characteristics used in analysis segment estimation. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
     overlap_factor: float, optional
-        Overlap factor used in PSD estimation. Default is 0.5.
+        Overlap factor used in analysis segment estimation. Default is 0.5.
     fref: float, optional
         Reference frequency to use in the weighting calculation.
         Final result refers to this frequency.
     alpha: float, optional
         Spectral index to use in the weighting.
     """
     S_alpha = 3 * H0.si.value ** 2 / (10 * np.pi ** 2) / freqs ** 3
     S_alpha *= (freqs / fref) ** float(alpha)
+
     var_fs = (
         1
         / (2 * segment_duration * (freqs[1] - freqs[0]))
         * avg_psd_1
         * avg_psd_2
         / (orf ** 2 * S_alpha ** 2)
     )
```

### Comparing `pygwb-1.0.0/pygwb/preprocessing.py` & `pygwb-1.3.0/pygwb/preprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import os
 import warnings
 
 import lal
 import numpy as np
 import scipy
 from gwpy import timeseries
+from gwpy.segments import Segment, SegmentList
+from gwsumm.data.timeseries import get_timeseries
 
 
 def set_start_time(
     job_start_GPS: int,
     job_end_GPS: int,
     buffer_secs: int,
     segment_duration: int,
@@ -65,14 +67,15 @@
 def read_data(
     IFO: str,
     data_type: str,
     channel: str,
     t0: int,
     tf: int,
     local_data_path: str = "",
+    frametype: str = "",
     tag: str = "C00",
     input_sample_rate: int = 16384,
 ):
     """
     Function doing the reading of the data to be used in the
     stochastic pipeline
 
@@ -93,14 +96,17 @@
 
     t0: int
         GPS time of the start of the data taking
 
     tf: int
         GPS time of the end of the data taking
 
+    frametype: string
+        Frame type that contains the channel, only used if data_type=private (e.g.: "L1_HOFT_C00")
+
     local_data_path: str, optional
         path where local gwf is stored
 
     tag: str, optional
         tag identifying type of data, e.g.: 'C00', 'C01'
 
     input_sample_rate: int
@@ -109,19 +115,26 @@
     Returns
     =======
     data: TimeSeries object
         Time series containing the requested data
     """
     if data_type == "public":
         data = timeseries.TimeSeries.fetch_open_data(
-            IFO, t0, tf, sample_rate=input_sample_rate, tag=tag
+            IFO, t0, tf, sample_rate=input_sample_rate
         )
         data.channel = channel
     elif data_type == "private":
-        data = timeseries.TimeSeries.get(channel, start=t0, end=tf, verbose=True)
+        if frametype=="":
+            frametype=None
+        data = get_timeseries(channel, segments=[[t0, tf]], frametype=frametype)
+        if len(data) > 1:
+            raise ValueError("Something went wrong while getting the data!"
+                             "There was more than one data stretch returned.")
+        else:
+            data = data[0]
         data.channel = channel
     elif data_type == "local":
         if os.path.isdir(local_data_path):
             local_data = []
             for f in os.listdir(local_data_path):
                 local_data.append(os.path.join(local_data_path, f))
         else:
@@ -255,14 +268,15 @@
 def self_gate_data(
     time_series_data: timeseries.TimeSeries,
     tzero: float = 1.0,
     tpad: float = 0.5,
     gate_threshold: float = 50.0,
     cluster_window: float = 0.5,
     whiten: bool = True,
+    gates: SegmentList = None
 ):
     """
     Function to self-gate
     data to be used in the stochastic pipeline
 
     Parameters
     ==========
@@ -300,35 +314,37 @@
 
     Notes
     -----
     This method is based on `gwpy.timeseries.gate`. See
     https://gwpy.github.io/docs/latest/api/gwpy.timeseries.TimeSeries/?highlight=timeseries#gwpy.timeseries.TimeSeries.gate
     for additional details.
     """
-
-    from gwpy.segments import Segment, SegmentList
     from scipy.signal import find_peaks
 
     # Find points to gate based on a threshold
     sample = time_series_data.sample_rate.to("Hz").value
-    data = time_series_data.whiten() if whiten else time_series_data
-    window_samples = cluster_window * sample
-    gates = find_peaks(abs(data.value), height=gate_threshold, distance=window_samples)[
-        0
-    ]
-    # represent gates as time segments
-    deadtime = SegmentList(
-        [
-            Segment(
-                time_series_data.t0.value + (k / sample) - tzero,
-                time_series_data.t0.value + (k / sample) + tzero,
-            )
-            for k in gates
+    if gates is None:
+        data = time_series_data.whiten() if whiten else time_series_data
+        window_samples = cluster_window * sample
+        gates = find_peaks(abs(data.value), height=gate_threshold, distance=window_samples)[
+            0
         ]
-    ).coalesce()
+    # represent gates as time segments
+        deadtime = SegmentList(
+            [
+                Segment(
+                    time_series_data.t0.value + (k / sample) - tzero,
+                    time_series_data.t0.value + (k / sample) + tzero,
+                )
+                for k in gates
+            ]
+        ).coalesce()
+    else:
+        deadtime = SegmentList([Segment(k[0], k[1]) for k in gates]).coalesce()
+
     # return the self-gated timeseries
     gated = time_series_data.mask(deadtime=deadtime, const=0, tpad=tpad)
     return gated, deadtime
 
 
 def shift_timeseries(time_series_data: timeseries.TimeSeries, time_shift: int = 0):
 
@@ -433,14 +449,15 @@
     cutoff_frequency: float,
     segment_duration: int,
     number_cropped_seconds: int = 2,
     window_downsampling: str = "hamming",
     ftype: str = "fir",
     time_shift: int = 0,
     local_data_path: str = "",
+    frametype: str = "",
     tag: str = "C00",
     input_sample_rate: int = 16384,
 ):
     """
     Function doing the pre-processing of the data to be used in the
     stochastic pipeline
 
@@ -458,14 +475,17 @@
     data_type: string
         String indicating the type of data to be read,
         either 'public' or 'private'
 
     channel: string
         Name of the channel (e.g.: "L1:GWOSC-4KHZ_R1_STRAIN")
 
+    frametype: string
+       Frame type that contains the channel, only used if data_type=private (e.g.: "L1_HOFT_C00") 
+
     new_sample_rate:int
         Sampling rate of the downsampled-timeseries
 
     cutoff_frequency: float
         Frequency (in Hz) from which to start applying the
         high pass filter
 
@@ -503,14 +523,15 @@
         segment_duration=segment_duration,
     )
 
     time_series_data = read_data(
         IFO=IFO,
         data_type=data_type,
         channel=channel,
+        frametype=frametype,
         t0=data_start_time - number_cropped_seconds,
         tf=tf,
         local_data_path=local_data_path,
         tag=tag,
         input_sample_rate=input_sample_rate,
     )
```

### Comparing `pygwb-1.0.0/pygwb/simulator.py` & `pygwb-1.3.0/pygwb/simulator.py`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb/spectral.py` & `pygwb-1.3.0/pygwb/spectral.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,212 +1,216 @@
+import copy
+import warnings
+
 import numpy as np
 from gwpy.frequencyseries import FrequencySeries
 from gwpy.spectrogram import Spectrogram
 from gwpy.timeseries import TimeSeries
 from scipy.signal import get_window, spectrogram
 
 from pygwb.util import get_window_tuple, parse_window_dict
 
 
 def fftgram(
     time_series_data: TimeSeries,
     fftlength: int,
-    overlap_factor: float=0.5,
-    zeropad: bool=False,
-    window_fftgram_dict: dict={"window_fftgram": "hann"},
+    overlap_factor: float = 0.5,
+    zeropad: bool = False,
+    window_fftgram_dict: dict = {"window_fftgram": "hann"},
 ):
     """Create an fftgram from a timeseries
 
     Parameters
     ----------
     time_series_data: gwpy timeseries
         Timeseries from which to compute the fftgram.
     fftlength: int
         Length of each segment (in seconds) for computing FFT.
     overlap_factor: float, optional
-        Factor of overlap between adjacent FFT segments (values range from 0 
+        Factor of overlap between adjacent FFT segments (values range from 0
         to 1). Users should provide proper combination of overlap_factor and
-        window_fftgram_dict. For \"hann\" window use 0.5 overlap_factor and 
+        window_fftgram_dict. For \"hann\" window use 0.5 overlap_factor and
         for \"boxcar"\ window use 0 overlap_factor. Default 0.5 (50% overlap).
-    zeropadd: bool, optional
-        Before doing FFT whether to zero pad the data equal to the length of 
+    zeropad: bool, optional
+        Before doing FFT whether to zero pad the data equal to the length of
         FFT or not. Default is False.
     window_fftgram_dict: dictionary, optional
-        Dictionary containing name and parameters describing which window to 
+        Dictionary containing name and parameters describing which window to
         use for producing FFTs. Default is \"hann\".
 
     Returns
     -------
     data_fftgram: gwpy spectrogram (complex)
         fftgram containing several FFTs in a matrix format
     """
-    
+
     sample_rate = int(1 / time_series_data.dt.value)
 
     # get the window function
     window_tuple = get_window_tuple(parse_window_dict(window_fftgram_dict))
-    window_fftgram = get_window(window_tuple, fftlength * sample_rate, 
-                                fftbins=False)
+    window_fftgram = get_window(window_tuple, fftlength * sample_rate, fftbins=False)
 
     # calculate the spectrogram using scipy.signal.spectrogram
     if zeropad:
-        f, t, Sxx = spectrogram(
-            time_series_data.data,
-            fs=sample_rate,
-            window=window_fftgram,
-            nperseg=fftlength * sample_rate,
-            noverlap=overlap_factor * fftlength * sample_rate,
-            nfft=2 * fftlength * sample_rate,
-            mode="complex",
-            detrend=False,
-        )
+        nfft = 2 * fftlength * sample_rate
     else:
-        f, t, Sxx = spectrogram(
-            time_series_data.data,
-            fs=sample_rate,
-            window=window_fftgram,
-            nperseg=fftlength * sample_rate,
-            noverlap=overlap_factor * fftlength * sample_rate,
-            nfft=fftlength * sample_rate,
-            mode="complex",
-            detrend=False,
-        )
+        nfft = fftlength * sample_rate
+
+    f, t, Sxx = spectrogram(
+        time_series_data.data,
+        fs=sample_rate,
+        window=window_fftgram,
+        nperseg=fftlength * sample_rate,
+        noverlap=overlap_factor * fftlength * sample_rate,
+        nfft=nfft,
+        mode="complex",
+        detrend=False,
+    )
 
     # convert the above spectrogram into gwpy spectrogram object
     ffts = []
     for ii in range(len(t)):
-        ffts.append(FrequencySeries(Sxx.T[ii], f0= f[0], df = f[1]-f[0]))
+        ffts.append(FrequencySeries(Sxx.T[ii], f0=f[0], df=f[1] - f[0]))
 
-    data_fftgram = Spectrogram.from_spectra(*ffts, epoch=time_series_data.t0, 
-                                            dt=t[1]-t[0])
+    data_fftgram = Spectrogram.from_spectra(
+        *ffts, epoch=time_series_data.t0, dt=t[1] - t[0]
+    )
 
     return data_fftgram
 
 
 def pwelch_psd(
-    psdgram: Spectrogram, 
-    segment_duration: int, 
-    overlap_factor: float = 0.5):
-
+    psdgram: Spectrogram, segment_duration: int, overlap_factor: float = 0.5
+):
     """
     Estimate PSD using pwelch method.
 
     Parameters
     ==========
     psdgram: gwpy spectrogram (PSD)
        PSD gram data to be averaged
     segment_duration: int
-        Data duration over which PSDs need to be averaged. Should be greater 
-        than or equal to the duration used for FFT. 
+        Data duration over which PSDs need to be averaged. Should be greater
+        than or equal to the duration used for FFT.
     overlap_factor: float, optional
-        Amount of overlap between adjacent average PSDs, can vary between 0 
-        and 1. This factor should be same as the one used for CSD estimation. 
-        Default is 0.5.
+        Amount of overlap between adjacent average PSDs, can vary between 0
+        and 1. Default is 0.5.
 
     Returns
     =======
     avg_psdgram: gwpy psd spectrogram
         averaged over segments within the segment_duration
     """
-    
+
     averaging_factor = round(segment_duration * psdgram.dy.value)
 
-    if averaging_factor < 1:    
-        raise ValueError('''Segment_duration should be greater than the FFT
-                        duration used for PSD calculation''')
-    elif averaging_factor == 1: # nothing to average in this case
+    if averaging_factor < 1:
+        raise ValueError(
+            """Segment_duration should be greater than the FFT
+                        duration used for PSD calculation"""
+        )
+    elif averaging_factor == 1:  # nothing to average in this case
         avg_psdgram = np.real(psdgram)
     else:
         # total duration of the original time series
-        job_duration = (psdgram.xindex.value[-1] +
-                        1/psdgram.dy.value - psdgram.xindex.value[0])
+        job_duration = (
+            psdgram.xindex.value[-1] + 1 / psdgram.dy.value - psdgram.xindex.value[0]
+        )
         # possible number of (overlapping) segments
-        stride = segment_duration*(1-overlap_factor)
-        n_segments = int((job_duration - overlap_factor* segment_duration)/
-                         stride)
-        
-        avg_psds = []        
+        stride = segment_duration * (1 - overlap_factor)
+        n_segments = int((job_duration - overlap_factor * segment_duration) / stride)
+        avg_psds = []
         segments_start_times = np.zeros(n_segments)
         start_time = psdgram.xindex.value[0]
+        if n_segments==0:
+            avg_psds = np.mean(psdgram[True], axis=0)
         for ii in range(n_segments):
-            seg_indices = ((psdgram.xindex.value >= start_time) & 
-                            (psdgram.xindex.value <= 
-                             (start_time + segment_duration - 
-                              1 / psdgram.dy.value)))
+            seg_indices = (psdgram.xindex.value >= start_time) & (
+                psdgram.xindex.value
+                <= (start_time + segment_duration - 1 / psdgram.dy.value)
+            )
             avg_psds.append(psdgram[seg_indices].mean(axis=0))
             segments_start_times[ii] = start_time
             # move to next (overlapping) segment
             start_time = start_time + stride
 
-        avg_psdgram = Spectrogram.from_spectra(*avg_psds, 
-                             epoch=segments_start_times[0], 
-                             dt=stride)
-
-    return np.real(avg_psdgram)
+        avg_psdgram = Spectrogram.from_spectra(
+            *avg_psds, epoch=psdgram.xindex.value[0], dt=stride
+        )
 
+    return avg_psdgram
 
-def before_after_average(
-    psdgram: Spectrogram, 
-    segment_duration: int, 
-    N_avg_segs: int):
 
+def before_after_average(psdgram: Spectrogram, segment_duration: int, N_avg_segs: int):
     """
-    Average the requested number of PSDs from segments adjacent to the segment 
+    Average the requested number of PSDs from segments adjacent to the segment
     of interest (for which CDS is calculated)
 
     Parameters
     ----------
     psdgram: gwpy spectrogram (PSD)
         PSD spectrogram.
     segment_duration: int
         Duration of data used for each PSD calculation.
     N_avg_segs: int
-        Number of segments to be used for PSD averaging (from both sides of 
+        Number of segments to be used for PSD averaging (from both sides of
         the segment of interest). N_avg_segs should be even and >= 2
 
     Returns
     -------
-    avg_psdgram: gwpy spectrogram 
+    avg_psdgram: gwpy spectrogram
         averaged psd gram
     """
 
     if N_avg_segs < 2:
-        raise ValueError('N_avg_segs should be >=2')
+        raise ValueError("N_avg_segs should be >=2")
 
     if (N_avg_segs % 2) != 0:
-        raise ValueError('N_avg_segs should be even')
+        raise ValueError("N_avg_segs should be even")
 
-    if ((psdgram.xindex.value[-1] - psdgram.xindex.value[0]) < 
-        (N_avg_segs * segment_duration)):
-        max_N_avg_segs = round((psdgram.xindex.value[-1] - 
-                                psdgram.xindex.value[0])/segment_duration)
-        raise ValueError(f''' Input (PSD) spectrogram does not have enough 
+    if (psdgram.xindex.value[-1] - psdgram.xindex.value[0]) < (
+        N_avg_segs * segment_duration
+    ):
+        max_N_avg_segs = round(
+            (psdgram.xindex.value[-1] - psdgram.xindex.value[0]) / segment_duration
+        )
+        raise ValueError(
+            f""" Input (PSD) spectrogram does not have enough 
                            segments to be used with given N_avg_segs. Here 
                            N_avg_segs should be less than or equal to
-                           {max_N_avg_segs}.''')
+                           {max_N_avg_segs}."""
+        )
 
     # segments for which average PSDs need to be calculcated
-    seg_times = [value for value in psdgram.xindex.value 
-                 if  (((value - psdgram.xindex.value[0]) >= 
-                       (N_avg_segs / 2 * segment_duration)) &
-                      ((psdgram.xindex.value[-1] - value) >= 
-                       (N_avg_segs / 2 * segment_duration)))]
+    seg_times = [
+        value
+        for value in psdgram.xindex.value
+        if (
+            ((value - psdgram.xindex.value[0]) >= (N_avg_segs / 2 * segment_duration))
+            & (
+                (psdgram.xindex.value[-1] - value)
+                >= (N_avg_segs / 2 * segment_duration)
+            )
+        )
+    ]
 
-    avg_psds = [] 
+    avg_psds = []
     for ii in seg_times:
         seg_diffs = abs(psdgram.xindex.value - ii) / segment_duration
-        seg_indices = ((seg_diffs <= (N_avg_segs / 2)) & 
-                       ((seg_diffs % 1) == 0) & 
-                       ((psdgram.xindex.value - ii) !=0))
+        seg_indices = (
+            (seg_diffs <= (N_avg_segs / 2))
+            & ((seg_diffs % 1) == 0)
+            & ((psdgram.xindex.value - ii) != 0)
+        )
         # Below we only average non-overlapping segments (this is a choice)
         avg_psds.append(psdgram[seg_indices].mean(axis=0))
-        
-    avg_psdgram = Spectrogram.from_spectra(*avg_psds, 
-                             epoch=seg_times[0], 
-                             dt=psdgram.dx.value)    
+
+    avg_psdgram = Spectrogram.from_spectra(
+        *avg_psds, epoch=seg_times[0], dt=psdgram.dx.value
+    )
     return avg_psdgram
 
 
 def coarse_grain(data, coarsening_factor):
     """
     Coarse grain a frequency series by an integer factor.
 
@@ -362,187 +366,212 @@
     )
 
     value = spectrogram.value
 
     if delta_t is not None:
         factor = delta_t / spectrogram.dt.value
         func = methods[time_method]
-        value = np.apply_along_axis(func, axis=0, arr=value, 
-                                    coarsening_factor=factor)
+        value = np.apply_along_axis(func, axis=0, arr=value, coarsening_factor=factor)
         coarse_times = func(spectrogram.times.value, coarsening_factor=factor)
         coarse_times += spectrogram.times.value[0] - coarse_times[0]
     else:
         coarse_times = spectrogram.times
 
     if delta_f is not None:
         factor = delta_f / spectrogram.df.value
         func = methods[frequency_method]
-        value = np.apply_along_axis(func, axis=1, arr=value, 
-                                    coarsening_factor=factor)
+        value = np.apply_along_axis(func, axis=1, arr=value, coarsening_factor=factor)
         coarse_frequencies = func(
             spectrogram.frequencies.value, coarsening_factor=factor
         )
     else:
         coarse_frequencies = spectrogram.frequencies
-        
+
     # create gwpy spectrogram object
     specgrams = []
-    # to avoid precision issues
-    deltaF = (coarse_frequencies[10] - coarse_frequencies[0])/10 
+    # To avoid precision issues rounding the frequency values at ~1% level; ideally we expect the ratio coarse_frequencies[0]/spectrogram.dy.value/factor to be an integer
+    f0 = np.round(coarse_frequencies[0]/spectrogram.dy.value/factor, 2) * spectrogram.dy.value * factor
+    deltaF = f0
     for ii in value:
-        specgrams.append(FrequencySeries(ii, f0=coarse_frequencies[0], 
-                    df = deltaF))
-        
-    output = Spectrogram.from_spectra(*specgrams, epoch=coarse_times[0].value, 
-                            dt=coarse_times[1].value-coarse_times[0].value)
-    
+        specgrams.append(FrequencySeries(ii, f0=f0, df=deltaF))
+
+    output = Spectrogram.from_spectra(
+        *specgrams,
+        epoch=coarse_times[0].value,
+        dt=coarse_times[1].value - coarse_times[0].value,
+    )
+
     return output
 
 
 def cross_spectral_density(
-    time_series_data1:  TimeSeries,
-    time_series_data2:  TimeSeries,
+    time_series_data1: TimeSeries,
+    time_series_data2: TimeSeries,
     segment_duration: int,
     frequency_resolution: float,
+    coarse_grain: bool = True,
     overlap_factor: float = 0.5,
+    overlap_factor_welch: float = 0.5,
     zeropad: bool = False,
-    window_fftgram_dict: dict={"window_fftgram": "hann"},
+    window_fftgram_dict: dict = {"window_fftgram": "hann"},
+    is_psd: bool = False,
 ):
     """
-    Compute the cross spectral density from two time series inputs
+    Compute the cross spectral density from two time series inputs.
 
     Parameters
     ----------
     time_series_data1: gwpy timeseries
         Timeseries data of detector1.
     time_series_data2: gwpy timeseries
         Timeseries data of detector2.
     segment duration: int
         data duration over which CSDs need to be calculated.
     frequency_resolution: float
         Frequency resolution of the final CSDs. This is achieved by averaing in
         frequency domain.
     overlap_factor: float, optional
         Amount of overlap between adjacent segments (range between 0 and 1)
-        This factor should be same as the one used for power_spectral_density.
-        Users should provide proper combination of overlap_factor and
-        window_fftgram_dict. For \"hann\" window use 0.5 overlap_factor and for \"boxcar"\ 
-        window use 0 overlap_factor. Default id 0.5 (50% overlap).
-    zeropadd: bool, optional
-        Before doing FFT whether to zero pad the data equal to the length of 
+    overlap_factor_welch: float
+        Overlap factor to use when using Welch's method (NOT coarsegraining). Users should provide proper combination of overlap_factor and window_fftgram_dict. For \"hann\" window use 0.5 overlap_factor and for \"boxcar"\ window use 0 overlap_factor. Default is 0.5 (50% overlap), which is optimal when using Welch's method with a \"hann\" window.
+    zeropad: bool, optional
+        Before doing FFT whether to zero pad the data equal to the length of
         FFT or not. Default is False.
     window_fftgram_dict: dictionary, optional
-        Dictionary containing name and parameters describing which window to 
+        Dictionary containing name and parameters describing which window to
         use for producing FFTs. Default is \"hann\".
 
     Returns
     -------
     csd_spectrogram: gwpy spectrogram
        Cross spectral density of the two timeseries
     """
 
-    # Check if the lengths of two time-series are equal
-    if len(time_series_data1.data) != len(time_series_data2.data):
-        raise ValueError('Lengths of two input time series are not equal')
-        
-    # Check if the sample rates of two input time-series are equal
-    if time_series_data1.dt.value != time_series_data2.dt.value:
-        raise ValueError('Sample rates of two input time series are not equal')
-    
+    if (segment_duration * frequency_resolution) % 1 != 0:
+        warnings.warn(
+            "Multiplying the parameters segment_duration and frequency_resolution gives a non-integer. "
+            "This could lead to possible issues while computing CSDs and PSDs. \n It will also lead to data loss when computing the PSD. "
+            "To avoid this, make sure this multiplication is an integer."
+        )
+
+    if coarse_grain:
+        fftlength = segment_duration
+        overlap_factor_fftgram = overlap_factor
+    else:
+        # Length of data blocks to be used in pwelch
+        fftlength = int(1.0 / frequency_resolution)
+        overlap_factor_fftgram = overlap_factor_welch
+
     fft_gram_1 = fftgram(
         time_series_data1,
-        segment_duration,
-        overlap_factor=overlap_factor,
-        zeropad=zeropad,
-        window_fftgram_dict=window_fftgram_dict,
-    )
-    fft_gram_2 = fftgram(
-        time_series_data2,
-        segment_duration,
-        overlap_factor=overlap_factor,
+        fftlength,
+        overlap_factor=overlap_factor_fftgram,
         zeropad=zeropad,
         window_fftgram_dict=window_fftgram_dict,
     )
 
-    csd_spectrogram = coarse_grain_spectrogram(
-        2 * np.conj(fft_gram_1) * fft_gram_2, delta_f=frequency_resolution
-    )
+    if is_psd:
+        fft_gram_2 = copy.deepcopy(fft_gram_1)
+
+    else:
+        # Check if the lengths of two time-series are equal
+        if len(time_series_data1.data) != len(time_series_data2.data):
+            raise ValueError("Lengths of two input time series are not equal")
+
+        # Check if the sample rates of two input time-series are equal
+        if time_series_data1.dt.value != time_series_data2.dt.value:
+            raise ValueError("Sample rates of two input time series are not equal")
+
+        fft_gram_2 = fftgram(
+            time_series_data2,
+            fftlength,
+            overlap_factor=overlap_factor_fftgram,
+            zeropad=zeropad,
+            window_fftgram_dict=window_fftgram_dict,
+        )
 
-    # Correct the scaling of DC and nyquist frequency components in agreement 
+    if not coarse_grain:
+        csd_spectrogram = pwelch_psd(
+            2 * np.conj(fft_gram_1) * fft_gram_2,
+            segment_duration,
+            overlap_factor=overlap_factor,
+        )
+    else:
+        csd_spectrogram = coarse_grain_spectrogram(
+            2 * np.conj(fft_gram_1) * fft_gram_2, delta_f=frequency_resolution
+        )
+
+    # Correct the scaling of DC and nyquist frequency components in agreement
     # with scipy.signal.welch (and pwelch in matlab)
     for ii in range(len(csd_spectrogram)):
-        csd_spectrogram[ii].value[0] = csd_spectrogram[ii].value[0]/2
-        csd_spectrogram[ii].value[-1] = csd_spectrogram[ii].value[-1]/2
-       
-    return csd_spectrogram
+        csd_spectrogram[ii].value[0] = csd_spectrogram[ii].value[0] / 2
+        csd_spectrogram[ii].value[-1] = csd_spectrogram[ii].value[-1] / 2
+
+    if is_psd:
+        return np.real(csd_spectrogram)
+    else:
+        return csd_spectrogram
 
 
 def power_spectral_density(
-    time_series_data:  TimeSeries,
-    segment_duration:  TimeSeries,
+    time_series_data: TimeSeries,
+    segment_duration: int,
     frequency_resolution: float,
+    coarse_grain: bool = False,
+    zeropad: bool = False,
     overlap_factor: float = 0.5,
-    window_fftgram_dict_welch_psd: dict = {"window_fftgram": "hann"},
-    overlap_factor_welch_psd: float = 0.5,
+    window_fftgram_dict: dict = {"window_fftgram": "hann"},
+    overlap_factor_welch: float = 0.5,
 ):
     """
     Compute the PSDs of every segment (defined by the segment duration)
     in the time series using pwelch method.
 
     Parameters
     ----------
     time_series_data: gwpy timeseries
         Timeseries from which to compute PSDs.
     segment duration: int
         Data duration over which each PSDs need to be calculated.
     frequency_resolution: float
         Frequency resolution of the final PSDs. This sets the time duration
         over which FFTs are calculated in the pwelch method.
+    coarse_grain: bool
+        Coarse-graining flag; if True, PSD will be estimated via coarse-graining
+        as opposed to Welch-averaging. Default is False.
+    zeropad: bool, optional
+        Before doing FFT whether to zero pad the data equal to the length of
+        FFT or not. Default is False.
     overlap_factor: float, optional
         Amount of overlap between adjacent segments (range between 0 and 1).
         This factor should be same as the one used for cross_spectral_density.
-        Users should provide proper combination of overlap_factor and
-        window_fftgram_dict. For \"hann\" window use 0.5 overlap_factor and 
-        for \"boxcar"\ window use 0 overlap_factor. Default is 0.5 (50% overlap)
     window_fftgram_dict: dictionary, optional
-        Dictionary containing name and parameters describing which window to 
+        Dictionary containing name and parameters describing which window to
         use for producing FFTs. Default is \"hann\".
-     
+    overlap_factor_welch: float
+        Overlap factor to use when using Welch's method (NOT coarsegraining). Users should provide proper combination of overlap_factor and window_fftgram_dict. For \"hann\" window use 0.5 overlap_factor and for \"boxcar"\ window use 0 overlap_factor. Default is 0.5 (50% overlap), which is optimal when using Welch's method with a \"hann\" window.
+
     Returns
     -------
     psd_spectrogram: gwpy PSD spectrogram
         PSD spectrogram with each PSD duration equal to segment duration
     """
-    
-    # Length of data blocks to be used in pwelch
-    fftlength = int(1.0 / frequency_resolution)
-
-    # No zero-pad is used in the PSD estimation
-    fft_gram_data = fftgram(
-        time_series_data,
-        fftlength,
-        overlap_factor=overlap_factor_welch_psd,
-        zeropad=False,
-        window_fftgram_dict=window_fftgram_dict_welch_psd,
-    )
 
-    # Use pwelch method (averaging) to get PSDs for each segment duration 
-    # of data
-    psd_spectrogram = pwelch_psd(
-        2 * np.conj(fft_gram_data) * fft_gram_data,
-        segment_duration,
+    psd_spectrogram = cross_spectral_density(
+        time_series_data1=time_series_data,
+        time_series_data2=None,
+        segment_duration=segment_duration,
+        frequency_resolution=frequency_resolution,
+        coarse_grain=coarse_grain,
         overlap_factor=overlap_factor,
+        overlap_factor_welch=overlap_factor_welch,
+        zeropad=zeropad,
+        window_fftgram_dict=window_fftgram_dict,
+        is_psd=True,
     )
-
-    # Correct the scaling of DC and nyquist frequency components in agreement  
-    # with scipy.signal.welch (and pwelch in matlab)
-    for ii in range(len(psd_spectrogram)):
-        psd_spectrogram[ii].value[0] = psd_spectrogram[ii].value[0]/2
-        psd_spectrogram[ii].value[-1] = psd_spectrogram[ii].value[-1]/2
-       
     return psd_spectrogram
 
 
 def running_mean(data, coarsening_factor=1, axis=-1):
     """
     Compute the running mean of an array, this uses the default axis of numpy
     cumsum.
@@ -561,10 +590,10 @@
     array-like: the averaged array of size M - coarsening factor
     """
     coarsening_factor = int(coarsening_factor)
     if axis != -1:
         data = np.swapaxes(axis, -1)
     cumsum = np.cumsum(np.insert(data, 0, 0))
     return (
-        np.swapaxes(cumsum[coarsening_factor:] - cumsum[:-coarsening_factor], 
-                    axis, -1)/ coarsening_factor
+        np.swapaxes(cumsum[coarsening_factor:] - cumsum[:-coarsening_factor], axis, -1)
+        / coarsening_factor
     )
```

### Comparing `pygwb-1.0.0/pygwb/statistical_checks.py` & `pygwb-1.3.0/pygwb/statistical_checks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,111 @@
+import json
+import warnings
 from os import listdir
 from os.path import isfile, join
 from pathlib import Path
 
 import matplotlib
 import matplotlib.pyplot as plt
+import matplotlib.transforms as mt
+from astropy.time import Time
+from loguru import logger
 
 matplotlib.rcParams['figure.figsize'] = (8,6)
 matplotlib.rcParams['axes.grid'] = True
 matplotlib.rcParams['grid.linestyle'] = ':'
 matplotlib.rcParams['grid.color'] = 'grey'
 matplotlib.rcParams['lines.linewidth'] = 2
 matplotlib.rcParams['legend.handlelength'] = 3
 
 from matplotlib import rc
 
 rc('font', **{'family': 'serif', 'serif': ['Computer Modern']})
-rc('text', usetex=True)
+# FIXME - changed to get workflow running
+rc('text', usetex=False)
 
 import seaborn as sns
 
 sea = sns.color_palette("tab10")
 
 import numpy as np
 from scipy import integrate, stats
 from scipy.optimize import curve_fit
 
 from pygwb.baseline import Baseline
+from pygwb.notch import StochNotchList
 from pygwb.parameters import Parameters
 from pygwb.util import StatKS, calc_bias
 
 
 class StatisticalChecks(object):
     def __init__(
         self,
         sliding_times_all,
         sliding_omega_all,
         sliding_sigmas_all,
         naive_sigmas_all,
+        coherence_spectrum,
+        coherence_n_segs,
         point_estimate_spectrum,
         sigma_spectrum,
-        freqs,
+        frequencies,
         badGPSTimes,
         delta_sigmas,
         plot_dir,
         baseline_name,
         param_file,
-        legend_fontsize = 16
+        frequency_mask = None,
+        gates_ifo1 = None,
+        gates_ifo2 = None,
+        file_tag = None,
+        legend_fontsize = 16,
+        convention = 'pygwb'
     ):
         """
         The statistical checks class performs various tests by plotting different quantities and saving this plots. This allows the user to check for consistency with expected results. Concretely, the following tests and plots can be generated: running point estimate, running sigma, (cumulative) point estimate integrand, real and imaginary part of point estimate integrand, FFT of the point estimate integrand, (cumulative) sensitivity, evolution of omega and sigma as a function of time, omega and sigma distribution, KS test, and a linear trend analysis of omega in time. Furthermore, part of these plots compares the values of these quantities before and after the delta sigma cut. Each of these plots can be made by calling the relevant class method (e.g. `plot_running_point_estimate()`).
 
         Parameters
         ==========
         sliding_times_all: array
             Array of GPS times before the bad GPS times from the delta sigma cut are applied.
         sliding_omega_all: array
             Array of sliding omegas before the bad GPS times from the delta sigma cut are applied.
         sliding_sigmas_all: array
             Array of sliding sigmas before the bad GPS times from the delta sigma cut are applied.
         naive_sigmas_all: array
             Array of naive sigmas before the bad GPS times from the delta sigma cut are applied.
+        coherence_spectrum: array
+            Array containing a coherence spectrum. Each entry in this array corresponds to the 2-detector coherence spectrum evaluated at the corresponding frequency in the frequencies array.
+        coherence_n_segs: int
+            Number of segments used for coherence calculation.
         point_estimate_spectrum: array
-            Array containing the point estimate spectrum. Each entry in this array corresponds to the point estimate spectrum evaluated at the corresponding frequency in the freqs array.
+            Array containing the point estimate spectrum. Each entry in this array corresponds to the point estimate spectrum evaluated at the corresponding frequency in the frequencies array.
         sigma_spectrum: array
-            Array containing the sigma spectrum. Each entry in this array corresponds to the sigma spectrum evaluated at the corresponding frequency in the freqs array.
-        freqs: array
+            Array containing the sigma spectrum. Each entry in this array corresponds to the sigma spectrum evaluated at the corresponding frequency in the frequencies array.
+        frequencies: array
             Array containing the frequencies.
         badGPStimes: array
             Array of bad GPS times, i.e. times that do not pass the delta sigma cut.
         delta_sigmas: array
             Array containing the value of delta sigma for all times in sliding_times_all.
         plot_dir: str
             String with the path to which the output of the statistical checks (various plots) will be saved.
         baseline_name: str
             Name of the baseline under consideration.
         param_file: str
             String with path to the file containing the parameters that were used for the analysis run.
+        frequency_mask: array
+            Boolean mask applied to the specrtra in broad-band analyses. 
+        gates_ifo1/gates_ifo2: list
+            List of gates applied to interferometer 1/2.
+        file_tag: str
+            Tag to be used in file naming convention.
+        legend_fontsize: int
+            Font size for plot legends. Default is 16. All other fonts are scaled to this font.
 
         Returns
         =======
         Initializes an instance of the statistical checks class.
         """
         self.params = Parameters()
         self.params.update_from_file(param_file)
@@ -90,14 +116,30 @@
         self.sliding_sigmas_all = sliding_sigmas_all
         self.naive_sigmas_all = naive_sigmas_all
         self.badGPStimes = badGPSTimes
         self.delta_sigmas_all = delta_sigmas
         self.sliding_deviate_all = (
             self.sliding_omega_all - np.nanmean(self.sliding_omega_all)
         ) / self.sliding_sigmas_all
+        self.gates_ifo1 = gates_ifo1
+        self.gates_ifo2 = gates_ifo2
+
+        self.frequencies = frequencies
+        if frequency_mask is not None:
+            self.frequency_mask = frequency_mask
+        else:
+            self.frequency_mask = True
+
+        self.coherence_spectrum = coherence_spectrum
+        fftlength = int(1.0 / (self.frequencies[1] - self.frequencies[0]))
+        self.n_segs = coherence_n_segs*(1.-self.params.overlap_factor) * int(np.floor(self.params.segment_duration/(fftlength*(1.-self.params.overlap_factor_welch)))-1)
+        if self.params.coarse_grain_csd:
+            # Note: this breaks down when self.params.segment_duration/fftlength < 3
+            self.n_segs = coherence_n_segs*(1.-self.params.overlap_factor) * int(np.floor(self.params.segment_duration/(fftlength)))
+        self.n_segs_statement = r"The number of segments is" + f" {self.n_segs}."
 
         self.sigma_spectrum = sigma_spectrum
         self.point_estimate_spectrum = point_estimate_spectrum
 
         self.plot_dir = Path(plot_dir)
 
         self.baseline_name = baseline_name
@@ -105,37 +147,60 @@
         self.deltaF = self.params.frequency_resolution
         self.new_sample_rate = self.params.new_sample_rate
         self.deltaT = 1.0 / self.new_sample_rate
         self.fref = self.params.fref
         self.flow = self.params.flow
         self.fhigh = self.params.fhigh
 
-        self.freqs = freqs
-
         self.alpha = self.params.alpha
         (
             self.sliding_times_cut,
             self.days_cut,
             self.sliding_omega_cut,
             self.sliding_sigma_cut,
             self.naive_sigma_cut,
             self.delta_sigmas_cut,
             self.sliding_deviate_cut,
             self.sliding_deviate_KS,
         ) = self.get_data_after_dsc()
+        self.dsc_percent = (len(self.sliding_times_all) - len(self.sliding_times_cut))/len(self.sliding_times_all) * 100
+        self.dsc_statement = r"The $\Delta\sigma$ cut removed" + f"{float(f'{self.dsc_percent:.2g}'):g}% of the data."
+
+        tot_tot_segs = ((sliding_times_all - sliding_times_all[0])[-1])/(self.params.segment_duration*(1-self.params.overlap_factor))
+        self.percent_obs_segs = len(self.naive_sigmas_all)/tot_tot_segs * 100
 
         (
             self.running_pt_estimate,
             self.running_sigmas,
         ) = self.compute_running_quantities()
 
+        t0 = Time(self.sliding_times_all[0], format='gps')
+        t0 = Time(t0, format='iso', scale='utc', precision=0, out_subfmt='date_hm')
+        tf = Time(self.sliding_times_all[-1], format='gps')
+        tf = Time(tf, format='iso', scale='utc', precision=0, out_subfmt='date_hm')
+        self.time_tag = f"{t0}"+" $-$ "+f"{tf}"
+
+        if file_tag:
+            self.file_tag = file_tag
+        else:
+            self.file_tag = f"{self.sliding_times_all[0]}-{self.params.tf}"
+
         self.legend_fontsize = legend_fontsize
         self.axes_labelsize = legend_fontsize + 2
+        self.title_fontsize = legend_fontsize + 4
         self.annotate_fontsize = legend_fontsize - 4
 
+        ## convention: stochmon
+        if convention == 'stochmon':
+            self.days_all = self.days_all*24 + t0.ymdhms.hour + t0.ymdhms.minute/60
+            self.days_cut = self.days_cut*24 + t0.ymdhms.hour + t0.ymdhms.minute/60
+            self.xaxis = f"Hours since {t0}"
+        else:
+            self.xaxis = f"Days since {t0}"
+
     def get_data_after_dsc(self):
         """
         Function that returns the GPS times, the sliding omegas, the sliding sigmas, the naive sigmas, the delta sigmas and the sliding deviates after the bad GPS times from the delta sigma cut were applied. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `sliding_times_all`).
 
         Returns
         =======
         sliding_times_cut: array
@@ -150,25 +215,27 @@
             Array of naive sigmas after the bad GPS times were applied.
         delta_sigma_cut: array
             Array of the delta sigma values after the bad GPS times were applied.
         sliding_deviate_cut: array
             Array of the deviates after the bad GPS times were applied.
         """
         bad_gps_times = self.badGPStimes
-        bad_gps_mask = [(t not in bad_gps_times) for t in self.sliding_times_all]
+        bad_gps_mask = np.array([(t not in bad_gps_times) for t in self.sliding_times_all])
 
+        bad_gps_mask[~np.isfinite(self.sliding_omega_all)] = False
         sliding_times_cut = self.sliding_times_all.copy()
         days_cut = self.days_all.copy()
         sliding_omega_cut = self.sliding_omega_all.copy()
         sliding_sigma_cut = self.sliding_sigmas_all.copy()
         naive_sigma_cut = self.naive_sigmas_all.copy()
         delta_sigma_cut = self.delta_sigmas_all.copy()
         sliding_deviate_cut = self.sliding_deviate_all.copy()
 
         sliding_times_cut = sliding_times_cut[bad_gps_mask]
+
         days_cut = days_cut[bad_gps_mask]
         sliding_omega_cut = sliding_omega_cut[bad_gps_mask]
         sliding_sigma_cut = sliding_sigma_cut[bad_gps_mask]
         naive_sigma_cut = naive_sigma_cut[bad_gps_mask]
         delta_sigma_cut = delta_sigma_cut[bad_gps_mask]
         sliding_deviate_cut = (
             sliding_omega_cut - np.nanmean(self.sliding_omega_all)
@@ -202,20 +269,20 @@
         """
         running_pt_estimate = self.sliding_omega_cut.copy()
         running_sigmas = self.sliding_sigma_cut.copy()
 
         ii = 0
         while ii < self.sliding_times_cut.shape[0] - 1:
             ii += 1
-            numerator = running_pt_estimate[ii - 1] / (
+            numerator = np.nansum([running_pt_estimate[ii - 1] / (
                 running_sigmas[ii - 1] ** 2
-            ) + self.sliding_omega_cut[ii] / (self.sliding_sigma_cut[ii] ** 2)
-            denominator = 1.0 / (running_sigmas[ii - 1] ** 2) + 1 / (
+            ) , self.sliding_omega_cut[ii] / (self.sliding_sigma_cut[ii] ** 2)])
+            denominator = np.nansum([1.0 / (running_sigmas[ii - 1] ** 2) , 1 / (
                 self.sliding_sigma_cut[ii] ** 2
-            )
+            )])
             running_pt_estimate[ii] = numerator / denominator
             running_sigmas[ii] = np.sqrt(1.0 / denominator)
 
         return running_pt_estimate, running_sigmas
 
     def compute_ifft_integrand(self):
         """
@@ -227,24 +294,23 @@
             Array containing the time lag values (in seconds).
         omega_t: array
             Array containing the
 
         """
 
         numFreqs = self.point_estimate_spectrum.shape[0]
-        freqs = self.flow + self.deltaF * np.arange(0, numFreqs)
         fhigh = self.flow + self.deltaF * numFreqs
 
         fNyq = 1 / (2 * self.deltaT)
 
         numFreqs_pre = np.floor(self.flow / self.deltaF) - 1
         f_pre = self.deltaF * np.arange(1, numFreqs_pre + 1)
         numFreqs_post = np.floor((fNyq - fhigh) / self.deltaF)
         f_post = fhigh + self.deltaF * np.arange(0, numFreqs_post)
-        fp = np.concatenate((f_pre, freqs, f_post))
+        fp = np.concatenate((f_pre, self.frequencies, f_post))
         fn = -np.flipud(fp)
         f_tot = np.concatenate((fn, np.array([0]), fp))
 
         integrand_pre = np.zeros(int(numFreqs_pre))
         integrand_post = np.zeros(int(numFreqs_post))
         integrand_p = np.concatenate(
             (integrand_pre, 0.5 * self.point_estimate_spectrum, integrand_post)
@@ -271,14 +337,16 @@
         ==========
         ymin: float
             Minimum value on the y-axis.
         ymax: float
             Maximum value on the y-axis.
 
         """
+        if self.days_cut.size==0:
+            return
         fig = plt.figure(figsize=(10, 8))
         plt.plot(
             self.days_cut,
             self.running_pt_estimate,
             ".",
             color="black",
             markersize=2,
@@ -298,265 +366,549 @@
             color=sea[0],
             markersize=2,
         )
         plt.grid(True)
         plt.xlim(self.days_cut[0], self.days_cut[-1])
         if ymin and ymax:
             plt.ylim(ymin, ymax)
-        plt.xlabel("Days since start of run", size=self.axes_labelsize)
+        plt.xlabel(self.xaxis, size=self.axes_labelsize)
         plt.ylabel(r"Point estimate $\pm 1.65 \sigma$", size=self.axes_labelsize)
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.annotate(
+            f"baseline time: {float(f'{self.percent_obs_segs:.2g}'):g}%",
+            xy=(0.5, 0.9),
+            xycoords="axes fraction",
+            size = self.annotate_fontsize,
+            bbox=dict(boxstyle="round", facecolor="white", alpha=1),
+        )
+        plt.title(f'Running point estimate in {self.time_tag}', fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-running_point_estimate.png", bbox_inches='tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-running_point_estimate.png", bbox_inches='tight'
         )
+        plt.close()
 
     def plot_running_sigma(self):
         """
         Generates and saves a plot of the running sigma. The plotted values are the ones after the delta sigma cut. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `days_cut`).
 
         """
+        if self.days_cut.size==0:
+            return
         fig = plt.figure(figsize=(10, 8))
-        plt.semilogy(
-            self.days_cut, self.running_sigmas, color=sea[0], label=self.baseline_name
+        plt.plot(
+            self.days_cut, self.running_sigmas, '.', markersize=2, color=sea[0], label=self.baseline_name
         )
         plt.grid(True)
+        plt.yscale("log")
         plt.xlim(self.days_cut[0], self.days_cut[-1])
-        plt.xlabel("Days since start of run", size=self.axes_labelsize)
+        plt.xlabel(self.xaxis, size=self.axes_labelsize)
         plt.ylabel(r"$\sigma$", size=self.axes_labelsize)
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(r'Running $\sigma$ ' + f'in {self.time_tag}', fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-running_sigma.png", bbox_inches = 'tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-running_sigma.png", bbox_inches = 'tight'
         )
+        plt.close()
 
     def plot_IFFT_point_estimate_integrand(self):
         """
         Generates and saves a plot of the IFFT of the point estimate integrand. The IFFT of the point estimate integrand is computed using the method "compute_ifft_integrand". This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `point_estimate_integrand`).
         """
         t_array, omega_array = self.compute_ifft_integrand()
+        if len(t_array) != len(omega_array):
+            warnings.warn("Times and Omega arrays don't match in the IFFT. No plot could be generated. Investigation is highly recommended.")
+            return
 
         fig = plt.figure(figsize=(10, 8))
         plt.plot(t_array, omega_array, color=sea[0], label=self.baseline_name)
         plt.grid(True)
         plt.xlim(t_array[0], t_array[-1])
         plt.xlabel("Lag (s)", size=self.axes_labelsize)
-        plt.ylabel("IFFT of Integrand of Pt Estimate", size=self.axes_labelsize)
+        plt.ylabel(r"$\Omega$ integrand IFFT", size=self.axes_labelsize)
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(r"$\Omega$ integrand IFFT" + f" in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-IFFT_point_estimate_integrand.png", bbox_inches='tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-IFFT_point_estimate_integrand.png", bbox_inches='tight'
         )
+        plt.close()
 
     def plot_SNR_spectrum(self):
         """
         Generates and saves a plot of the point estimate integrand. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `point_estimate_integrand`).
 
         """
-        plt.figure(figsize=(10, 8))
-        plt.semilogy(
-            self.freqs,
+        if np.isnan(self.point_estimate_spectrum).all() or not np.real(self.point_estimate_spectrum).any():
+            return
+        fig, axs = plt.subplots(figsize=(10, 8))
+        axs.semilogy(
+            self.frequencies,
             abs(self.point_estimate_spectrum / self.sigma_spectrum),
             color=sea[0],
         )
-        plt.xlabel("Frequency (Hz)", size=self.axes_labelsize)
-        plt.ylabel(r"$|{\rm SNR}(f)|$", size=self.axes_labelsize)
+        trans = mt.blended_transform_factory(axs.transData, axs.transAxes) 
+        axs.vlines(self.frequencies[~self.frequency_mask], ymin=0, ymax=1, linewidth=1, linestyle=':', color='black', alpha=0.5, transform=trans)
+        axs.set_xlabel("Frequency (Hz)", size=self.axes_labelsize)
+        axs.set_ylabel(r"$|{\rm SNR}(f)|$", size=self.axes_labelsize)
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
-        plt.xscale("log")
+        axs.set_xscale("log")
+        plt.title(f"|SNR| in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-abs_point_estimate_integrand.png",
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-abs_point_estimate_integrand.png",
             bbox_inches="tight",
         )
+        plt.close()
 
     def plot_cumulative_SNR_spectrum(self):
         """
         Generates and saves a plot of the cumulative point estimate integrand. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `point_estimate_integrand`).
         """
+        pt_est_cumul = self.point_estimate_spectrum.copy()
+        pt_est_cumul[~self.frequency_mask] = 0
         cum_pt_estimate = integrate.cumtrapz(
-            np.abs(self.point_estimate_spectrum / self.sigma_spectrum), self.freqs
+            np.abs(pt_est_cumul/ self.sigma_spectrum), self.frequencies
         )
         cum_pt_estimate = cum_pt_estimate / cum_pt_estimate[-1]
-        plt.figure(figsize=(10, 8))
-        plt.plot(self.freqs[:-1], cum_pt_estimate, color=sea[0])
-        plt.xlabel("Frequency (Hz)", size=self.axes_labelsize)
-        plt.ylabel(r"Cumulative $|{\rm SNR}(f)|$", size=self.axes_labelsize)
-        plt.xscale("log")
+        fig, axs = plt.subplots(figsize=(10, 8))
+        axs.plot(self.frequencies[:-1], cum_pt_estimate, color=sea[0])
+        axs.set_xlabel("Frequency (Hz)", size=self.axes_labelsize)
+        axs.set_ylabel(r"Cumulative $|{\rm SNR}(f)|$", size=self.axes_labelsize)
+        axs.set_xscale("log")
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(f"Cumulative SNR in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-cumulative_SNR_spectrum.png",
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-cumulative_SNR_spectrum.png",
             bbox_inches="tight",
         )
+        plt.close()
 
     def plot_real_SNR_spectrum(self):
         """
         Generates and saves a plot of the real part of the SNR spectrum. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `point_estimate_spectrum` and `sigma_spectrum`).
         """
-        plt.figure(figsize=(10, 8))
-        plt.plot(
-            self.freqs,
+        fig, axs =  plt.subplots(figsize=(10, 8))
+        axs.plot(
+            self.frequencies,
             np.real(self.point_estimate_spectrum / self.sigma_spectrum),
             color=sea[0],
         )
-        plt.xlabel("Frequency (Hz)", size=self.axes_labelsize)
-        plt.ylabel(r"Re$({\rm SNR}(f))$", size=self.axes_labelsize)
-        plt.xscale("log")
+        trans = mt.blended_transform_factory(axs.transData, axs.transAxes) 
+        axs.vlines(self.frequencies[~self.frequency_mask], ymin=0, ymax=1, linewidth=1, linestyle=':', color='black', alpha=0.5, transform=trans)
+        axs.set_xlabel("Frequency (Hz)", size=self.axes_labelsize)
+        axs.set_ylabel(r"Re$({\rm SNR}(f))$", size=self.axes_labelsize)
+        axs.set_xscale("log")
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(f"Real SNR in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-real_SNR_spectrum.png",
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-real_SNR_spectrum.png",
             bbox_inches="tight",
         )
+        plt.close()
 
     def plot_imag_SNR_spectrum(self):
         """
         Generates and saves a plot of the imaginary part of the SNR spectrum. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `point_estimate_spectrum` and `sigma_spectrum`).
         """
-        plt.figure(figsize=(10, 8))
-        plt.plot(
-            self.freqs,
+        fig, axs = plt.subplots(figsize=(10, 8))
+        axs.plot(
+            self.frequencies,
             np.imag(self.point_estimate_spectrum / self.sigma_spectrum),
             color=sea[0],
         )
-        plt.xlabel("Frequency (Hz)", size=self.axes_labelsize)
-        plt.ylabel(r"Im$({\rm SNR}(f))$", size=self.axes_labelsize)
-        plt.xscale("log")
+        trans = mt.blended_transform_factory(axs.transData, axs.transAxes) 
+        axs.vlines(self.frequencies[~self.frequency_mask], ymin=0, ymax=1, linewidth=1, linestyle=':', color='black', alpha=0.5, transform=trans)
+        axs.set_xlabel("Frequency (Hz)", size=self.axes_labelsize)
+        axs.set_ylabel(r"Im$({\rm SNR}(f))$", size=self.axes_labelsize)
+        axs.set_xscale("log")
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(f"Imaginary SNR in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-imag_SNR_spectrum.png",
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-imag_SNR_spectrum.png",
             bbox_inches="tight",
         )
+        plt.close()
 
     def plot_sigma_spectrum(self):
         """
         Generates and saves a plot of the sigma spectrum. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `sigma_spectrum`).
         """
+        if np.isinf(self.sigma_spectrum).all() or not np.real(self.point_estimate_spectrum).any():
+            return
+
+        fig, axs = plt.subplots(figsize=(10, 8))
+        axs.plot(self.frequencies, self.sigma_spectrum, color=sea[0])
+        trans = mt.blended_transform_factory(axs.transData, axs.transAxes) 
+        axs.vlines(self.frequencies[~self.frequency_mask], ymin=0, ymax=1, linewidth=1, linestyle=':', color='black', alpha=0.5, transform=trans)
+        axs.set_xlabel("Frequency (Hz)", size=self.axes_labelsize)
+        axs.set_ylabel(r"$\sigma(f)$", size=self.axes_labelsize)
+        axs.set_xscale("log")
+        axs.set_yscale("log")
+        plt.xticks(fontsize=self.legend_fontsize)
+        plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(r"Total $\sigma$ spectrum" + f" in {self.time_tag}", fontsize=self.title_fontsize)
+        plt.savefig(
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-sigma_spectrum.png",
+            bbox_inches="tight",
+        )
+        plt.close()
+
+    def plot_coherence_spectrum(self, flow=None, fhigh=None):
+        """
+        Generates and saves a plot of the coherence spectrum, if present. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `coherence_spectrum`).
+        """
+        if self.coherence_spectrum is None or self.coherence_spectrum.size==1:
+            return
+
+        flow = flow or self.flow
+        fhigh = fhigh or self.fhigh
+
         plt.figure(figsize=(10, 8))
-        plt.plot(self.freqs, self.sigma_spectrum, color=sea[0])
+        plt.plot(self.frequencies, self.coherence_spectrum, color=sea[0])
+        plt.axhline(y=1./self.n_segs,dashes=(4,3),color='black')
+        plt.xlim(flow, fhigh)
         plt.xlabel("Frequency (Hz)", size=self.axes_labelsize)
-        plt.ylabel(r"$\sigma(f)$", size=self.axes_labelsize)
+        plt.ylabel(r"coherence spectrum", size=self.axes_labelsize)
         plt.xscale("log")
         plt.yscale("log")
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.annotate(
+            f"{self.params.channel}",
+            xy=(0.01, 0.03),
+            xycoords="axes fraction",
+            size = self.annotate_fontsize,
+            bbox=dict(boxstyle="round", facecolor="white", alpha=1),
+        )
+        plt.title(r"Coherence ($\Delta f$ = " + f"{float(f'{self.deltaF:.4g}'):g}Hz) in {self.time_tag}", fontsize=self.title_fontsize)
+        plt.savefig(
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-coherence_spectrum.png",
+            bbox_inches="tight",
+        )
+        plt.close()
+
+        plt.figure(figsize=(10, 8))
+        plt.plot(self.frequencies, self.coherence_spectrum, color=sea[0])
+        plt.axhline(y=1./self.n_segs,dashes=(4,3),color='black')
+        plt.xlim(flow, 200)
+        plt.xlabel("Frequency (Hz)", size=self.axes_labelsize)
+        plt.ylabel(r"coherence spectrum", size=self.axes_labelsize)
+        plt.yscale("log")
+        plt.xticks(fontsize=self.legend_fontsize)
+        plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(r"Coherence ($\Delta f$ = " + f"{float(f'{self.deltaF:.4g}'):g}Hz) in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-sigma_spectrum.png",
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-coherence_spectrum_zoom.png",
             bbox_inches="tight",
         )
+        plt.close()
+
+
+    def plot_hist_coherence(self,total_bins = None):
+        r"""
+        Generates and saves a histogram of the coherence distribution. The plot shows the data after the delta-sigma cut (bad GPS times) was applied. This function does not require any input parameters, as it accesses the data through the attributes of the class.
+        Furthermore, it also saves a text file which contains the frequencies at which outliers of the coherence distribution were identified, i.e. spectral artefacts.
+        """
+        if self.coherence_spectrum is None or self.coherence_spectrum.size==1:
+            return
+
+        coherence = self.coherence_spectrum
+        coherence_clipped = np.ones(len(coherence))
+        clip_val = 50* 1/self.n_segs
+        for i in range(len(coherence_clipped)):
+            if coherence[i] >= clip_val:
+                coherence_clipped[i] = clip_val
+            else:
+                coherence_clipped[i] = coherence[i]
+        frequencies = self.frequencies
+        if total_bins is None:
+            total_bins = 250
+        bins =  np.linspace(0, max(coherence), total_bins)
+        bins_clipped =  np.linspace(0, max(coherence_clipped), total_bins)
+        n_frequencies = len(frequencies)
+        delta_coherence = bins[1]-bins[0]
+        delta_coherence_clipped = bins_clipped[1]-bins_clipped[0]
+        resolution = frequencies[1] - frequencies[0]
+        fftlength = int(1.0 / resolution)
+        
+        coherence_notched = coherence*self.frequency_mask
+        coherence_notched_clipped = coherence_clipped*self.frequency_mask
+
+        coherence_highres = np.arange(0,1,1e-6)
+        predicted_highres = (self.n_segs-1) * (1- coherence_highres)**(self.n_segs-2)
+        threshold = coherence_highres[np.where(predicted_highres <= 1/(n_frequencies*delta_coherence_clipped))[0][0]]
+
+        probability = n_frequencies*delta_coherence_clipped * predicted_highres
+
+        fig, axs = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))
+   
+        axs.hist(
+            coherence,
+            bins,
+            color=sea[3],
+            ec="k",
+            lw = 0.1,
+            zorder=1,
+            density = True,
+            label = 'Before notching',
+        )
+        axs.hist(
+            coherence_notched,
+            bins,
+            color=sea[0],
+            ec="k",
+            lw = 0.1,
+            zorder=2,
+            density = True,
+            label = 'After notching',
+        )
+        axs.plot(
+            coherence_highres, 
+            predicted_highres,
+            color=sea[1],
+            zorder=3,
+            alpha = 0.8,
+            label="Predicted",
+        )
+        axs.axvline(
+            np.abs(threshold),
+            zorder=4,
+            color=sea[8],
+            linestyle='dashed',
+            label="Threshold",
+        )
+
+        axs.set_xlabel(r"Coherence", size=self.axes_labelsize)
+        axs.set_ylabel(r"Probability distribution", size=self.axes_labelsize)
+        axs.legend(fontsize=self.legend_fontsize)
+        axs.set_yscale("log")
+        axs.set_xlim(0, max(coherence))
+        axs.set_ylim(0.5/(n_frequencies*delta_coherence),10*predicted_highres[0])
+        axs.tick_params(axis="x", labelsize=self.legend_fontsize)
+        axs.tick_params(axis="y", labelsize=self.legend_fontsize)
+        plt.title(r"Coherence hist ($\Delta f$ = " + f"{resolution:.3f}Hz) in" f" {self.time_tag}", fontsize=self.title_fontsize)
+        plt.savefig(
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-histogram_coherence.png", bbox_inches = 'tight'
+        )
+        plt.close()
 
+        fig, axs = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))      
+
+        axs.hist(
+            coherence_clipped,
+            bins_clipped,
+            color=sea[3],
+            ec="k",
+            lw = 0.1,
+            zorder=1,
+            density = True,
+            label = 'Before notching',
+        )
+        axs.hist(
+            coherence_notched_clipped,
+            bins_clipped,
+            color=sea[0],
+            ec="k",
+            lw = 0.1,
+            zorder=2,
+            density = True,
+            label = 'After notching',
+        )
+        axs.plot(
+            coherence_highres, 
+            predicted_highres,
+            color=sea[1],
+            zorder=3,
+            alpha = 0.8,
+            label="Predicted",
+        )
+        axs.axvline(
+            np.abs(threshold),
+            zorder=4,
+            color=sea[8],
+            linestyle='dashed',
+            label="Threshold",
+        )
+
+        axs.set_xlabel(r"Coherence", size=self.axes_labelsize)
+        axs.set_ylabel(r"Probability distribution", size=self.axes_labelsize)
+        axs.legend(fontsize=self.legend_fontsize)
+        axs.set_yscale("log")
+        axs.set_xlim(0,max(coherence_clipped))
+        axs.set_ylim(0.5/(n_frequencies*delta_coherence_clipped),10*predicted_highres[0])
+        axs.tick_params(axis="x", labelsize=self.legend_fontsize)
+        axs.tick_params(axis="y", labelsize=self.legend_fontsize)
+
+        plt.title(r"Coherence hist (zoomed) ($\Delta f$ = " + f"{resolution:.3f}Hz) in" f" {self.time_tag}", fontsize=self.title_fontsize)
+        plt.savefig(
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-histogram_coherence_zoom.png", bbox_inches = 'tight'
+        )
+        plt.close()
+
+        outlier_coherence = [(frequencies[i], coherence[i],probability[np.where(coherence_highres>=coherence[i])[0][0]]) for i in range(len(coherence)) if (coherence[i] > np.abs(threshold) and self.frequency_mask[i] == True)]
+        outlier_coherence_notched = [(frequencies[i], coherence[i],probability[np.where(coherence_highres>=coherence[i])[0][0]]) for i in range(len(coherence)) if (coherence[i] > np.abs(threshold) and self.frequency_mask[i] == False)]
+        n_outlier = len(outlier_coherence)
+        file_name = f"{self.plot_dir / self.baseline_name}-{self.file_tag}-list_coherence_outlier.txt"
+        with open(file_name, 'w') as f:
+            f.write('Frequencies  \tCoherence \tProbability\n')
+            for tup in outlier_coherence:
+                f.write(f'{tup[0]}\t{tup[1]}\t{tup[2]}\n')
+            f.write('\n The outliers below are already included in the applied version of the notch-list\n')
+            for tup in outlier_coherence_notched:
+                f.write(f'{tup[0]}\t{tup[1]}\t{tup[2]}\n')
+                
     def plot_cumulative_sensitivity(self):
         """
         Generates and saves a plot of the cumulative sensitivity. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `sigma_spectrum`).
 
         """
+        if np.isinf(self.sigma_spectrum).all() or not np.real(self.point_estimate_spectrum).any():
+            return
 
-        cumul_sens = integrate.cumtrapz((1 / self.sigma_spectrum ** 2), self.freqs)
+        sigma_cumul = self.sigma_spectrum.copy()
+        sigma_cumul[~self.frequency_mask] = np.inf
+        cumul_sens = integrate.cumtrapz((1 / sigma_cumul ** 2), self.frequencies)
         cumul_sens = cumul_sens / cumul_sens[-1]
         plt.figure(figsize=(10, 8))
-        plt.plot(self.freqs[:-1], cumul_sens, color=sea[0])
+        plt.plot(self.frequencies[:-1], cumul_sens, color=sea[0])
         plt.xlabel("Frequency (Hz)", size=self.axes_labelsize)
         plt.ylabel("Cumulative sensitivity", size=self.axes_labelsize)
         plt.xscale("log")
         plt.xticks(fontsize=self.legend_fontsize)
         plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(r"$1/\sigma^2$ " + f"in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-cumulative_sigma_spectrum.png",
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-cumulative_sigma_spectrum.png",
             bbox_inches="tight",
         )
+        plt.close()
 
     def plot_omega_sigma_in_time(self):
         r"""
         Generates and saves a panel plot with a scatter plot of :math:`\sigma` vs :math:`\Delta{\rm SNR}_i`, as well as the evolution of :math:`\Omega`, :math:`\sigma`, and :math:`(\Omega-\langle\Omega\rangle)/\sigma` as a function of the days since the start of the run. All plots show the data before and after the delta-sigma cut (bad GPS times) was applied. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `sliding_sigmas_all`).
         """
-        fig, axs = plt.subplots(nrows=3, ncols=1, figsize=(10, 18))
+        fig, axs = plt.subplots(nrows=3, ncols=1, figsize=(10, 15), constrained_layout=True)
+        fig.suptitle(r"$\Omega$, $\sigma$, and" + f" SNR variations in {self.time_tag} with/out " + r"$\Delta\sigma$ cut", fontsize=self.title_fontsize)
 
-        axs[0].plot(self.days_all, self.sliding_omega_all, color=sea[3], label="All data")
+        axs[0].plot(self.days_all, self.sliding_omega_all, color=sea[3], linewidth=1, alpha=0.5, label="All data")
         axs[0].plot(
             self.days_cut,
             self.sliding_omega_cut,
-            color=sea[0],
+            color=sea[0], linewidth=1, alpha=0.5,
             label=r"Data after $|\Delta\sigma|/\sigma$ outlier cut",
         )
-        axs[0].set_xlabel("Days since start of run", size=self.axes_labelsize)
+        axs[0].plot(self.days_all, self.sliding_omega_all, '.', color=sea[3])
+        axs[0].plot(
+            self.days_cut,
+            self.sliding_omega_cut, '.',
+            color=sea[0],
+        )
+        axs[0].set_xlabel(self.xaxis, size=self.axes_labelsize)
         axs[0].set_ylabel(r"$\Omega$", size=self.axes_labelsize)
         axs[0].legend(loc="upper left", fontsize=self.legend_fontsize)
         axs[0].set_xlim(0, self.days_all[-1])
         axs[0].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[0].tick_params(axis="y", labelsize=self.legend_fontsize)
         axs[0].yaxis.offsetText.set_fontsize(self.legend_fontsize)
 
-        axs[1].plot(self.days_all, self.sliding_sigmas_all, color=sea[3], label="All data")
+        axs[1].plot(self.days_all, self.sliding_sigmas_all, color=sea[3], linewidth=1, alpha=0.5, label="All data")
         axs[1].plot(
             self.days_cut,
             self.sliding_sigma_cut,
             color=sea[0],
+            linewidth=1,
+            alpha=0.5,
             label=r"Data after $|\Delta\sigma|/\sigma$ outlier cut",
         )
-        axs[1].set_xlabel("Days since start of run", size=self.axes_labelsize)
+        axs[1].plot(self.days_all, self.sliding_sigmas_all,'.', color=sea[3])
+        axs[1].plot(
+            self.days_cut,
+            self.sliding_sigma_cut,'.',
+            color=sea[0]
+        )
+        axs[1].set_xlabel(self.xaxis, size=self.axes_labelsize)
         axs[1].set_ylabel(r"$\sigma$", size=self.axes_labelsize)
         axs[1].legend(loc="upper left", fontsize=self.legend_fontsize)
         axs[1].set_xlim(0, self.days_all[-1])
+        axs[1].set_yscale('log')
         axs[1].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[1].tick_params(axis="y", labelsize=self.legend_fontsize)
         axs[1].yaxis.offsetText.set_fontsize(self.legend_fontsize)
 
-        axs[2].plot(self.days_all, self.sliding_deviate_all, color=sea[3], label="All data")
+        axs[2].plot(self.days_all, self.sliding_deviate_all, color=sea[3], linewidth=1, alpha=0.5, label="All data")
         axs[2].plot(
             self.days_cut,
             self.sliding_deviate_cut,
-            color=sea[0],
+            color=sea[0], linewidth=1, alpha=0.5,
             label=r"Data after $|\Delta\sigma|/\sigma$ outlier cut",
         )
-        axs[2].set_xlabel("Days since start of run", size=self.axes_labelsize)
+        axs[2].plot(self.days_all, self.sliding_deviate_all, '.', color=sea[3])
+        axs[2].plot(
+            self.days_cut,
+            self.sliding_deviate_cut, '.',
+            color=sea[0],
+        )
+        axs[2].set_xlabel(self.xaxis, size=self.axes_labelsize)
         axs[2].set_ylabel(r"$\Delta{\rm SNR}_i$", size=self.axes_labelsize)
         axs[2].legend(loc="upper left", fontsize=self.legend_fontsize)
         axs[2].set_xlim(0, self.days_all[-1])
+        axs[2].set_yscale("symlog")
         axs[2].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[2].tick_params(axis="y", labelsize=self.legend_fontsize)
 
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-omega_sigma_time.png", bbox_inches='tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-omega_sigma_time.png", bbox_inches='tight'
         )
+        plt.close()
 
     def plot_hist_sigma_dsc(self):
         r"""
         Generates and saves a panel plot with a histogram of :math:`|\Delta\sigma|/\sigma`, as well as a histogram of :math:`\sigma`. Both plots show the data before and after the delta-sigma cut (bad GPS times) was applied. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `delta_sigmas_all`).
 
         """
-        fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 14))
+        fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 14), constrained_layout=True)
+        fig.suptitle(r"$\Delta\sigma$ and $\sigma$ distributions in" f" {self.time_tag} with/out " + r"$\Delta\sigma$ cut", fontsize=self.title_fontsize)
 
         axs[0].hist(
             self.delta_sigmas_all,
             bins=80,
             color=sea[3],
             ec="k",
             lw=0.5,
             label="All data",
             range=(0.0001, 1),
         )
         axs[0].hist(
             self.delta_sigmas_cut,
             bins=80,
             color=sea[0],
+            alpha = 0.6,
             ec="k",
             lw=0.5,
             label=r"Data after $|\Delta\sigma|/\sigma$ outlier cut",
             range=(0.0001, 1),
         )
         axs[0].set_xlabel(r"$|\Delta\sigma|/\sigma$", size=self.axes_labelsize)
-        axs[0].set_ylabel(r"\# per bin", size=self.axes_labelsize)
+        axs[0].set_ylabel(r"count", size=self.axes_labelsize)
         axs[0].legend(fontsize=self.legend_fontsize)
         axs[0].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[0].tick_params(axis="y", labelsize=self.legend_fontsize)
         axs[0].yaxis.offsetText.set_fontsize(self.legend_fontsize)
 
-        minx1 = min(self.sliding_sigma_cut)
-        maxx1 = max(self.sliding_sigma_cut)
+        if self.sliding_sigma_cut.size==0:
+            minx1 = min(self.sliding_sigmas_all)
+            maxx1 = max(self.sliding_sigmas_all)
+        else:
+            minx1 = min(self.sliding_sigma_cut)
+            maxx1 = max(self.sliding_sigma_cut)
         nx = 50
 
         axs[1].hist(
             self.sliding_sigmas_all,
             bins=nx,
             color=sea[3],
             ec="k",
@@ -564,30 +916,32 @@
             label="All data",
             range=(minx1, maxx1),
         )
         axs[1].hist(
             self.sliding_sigma_cut,
             bins=nx,
             color=sea[0],
+            alpha = 0.6,
             ec="k",
             lw=0.5,
             label=r"Data after $|\Delta\sigma|/\sigma$ outlier cut",
             range=(minx1, maxx1),
         )
         axs[1].set_xlabel(r"$\sigma$", size=self.axes_labelsize)
-        axs[1].set_ylabel(r"\# per bin", size=self.axes_labelsize)
+        axs[1].set_ylabel(r"count", size=self.axes_labelsize)
         axs[1].legend(fontsize=self.legend_fontsize)
         axs[1].set_yscale("log")
         axs[1].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[1].tick_params(axis="y", labelsize=self.legend_fontsize)
         axs[1].xaxis.offsetText.set_fontsize(self.legend_fontsize)
 
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-histogram_sigma_dsc.png", bbox_inches='tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-histogram_sigma_dsc.png", bbox_inches='tight'
         )
+        plt.close()
 
     def plot_scatter_sigma_dsc(self):
         """
         Generates and saves a scatter plot of :math:`|\Delta\sigma]/\sigma` vs :math:`\sigma`. The plot shows the data before and after the delta-sigma cut (bad GPS times) was applied. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `delta_sigmas_all`).
         """
         fig, axs = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))
 
@@ -612,34 +966,71 @@
         axs.set_ylabel(r"$\sigma$", size=self.axes_labelsize)
         axs.set_yscale("log")
         axs.set_xscale("log")
         axs.legend(fontsize=self.legend_fontsize)
         axs.tick_params(axis="x", labelsize=self.legend_fontsize)
         axs.tick_params(axis="y", labelsize=self.legend_fontsize)
 
+        axs.annotate(
+            r"Data cut by $\Delta\sigma$ cut"+f": {float(f'{self.dsc_percent:.2g}'):g}%",
+            xy=(0.05, 0.8),
+            xycoords="axes fraction",
+            size = self.annotate_fontsize,
+            bbox=dict(boxstyle="round", facecolor="white", alpha=1),
+        )
+        plt.title(r"$\Delta\sigma$ distribution in" f" {self.time_tag} with/out " + r"$\Delta\sigma$ cut", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-scatter_sigma_dsc.png", bbox_inches = 'tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-scatter_sigma_dsc.png", bbox_inches = 'tight'
         )
+        plt.close()
 
     def plot_scatter_omega_sigma_dsc(self):
         r"""
         Generates and saves a panel plot with scatter plots of :math:`|\Delta\sigma|/\sigma` vs :math:`\Delta{\rm SNR}_i`, as well as :math:`\sigma` vs :math:`(\Omega-\langle\Omega\rangle)/\sigma`. All plots show the data before and after the delta-sigma cut (bad GPS times) was applied. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `delta_sigmas_all`).
         """
-        fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 14))
-
-        maxx0 = max(self.delta_sigmas_cut)
-        maxx0 += maxx0 / 10.0
+        fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 13), constrained_layout=True)
+        fig.suptitle(r"$\Delta$SNR spread" + f" in {self.time_tag} with/out " + r"$\Delta\sigma$ cut", fontsize=self.title_fontsize)
 
-        minx0 = min(self.delta_sigmas_cut)
-        minx0 -= minx0 / 10.0
-
-        maxy0 = np.nanmax(self.sliding_deviate_cut)
-        maxy0 += maxy0 / 10.0
-        miny0 = np.nanmin(self.sliding_deviate_cut)
-        miny0 -= miny0 / 10.0
+        if self.delta_sigmas_cut.size==0:
+            maxx0 = max(self.delta_sigmas_all)
+            maxx0 += maxx0 / 10.0
+            minx0 = min(self.delta_sigmas_all)
+            minx0 -= minx0 / 10.0
+            maxy0 = np.nanmax(self.sliding_deviate_all)
+            maxy0 += maxy0 / 10.0
+            miny0 = np.nanmin(self.sliding_deviate_all)
+            miny0 -= miny0 / 10.0
+
+            maxx1 = max(self.sliding_sigmas_all)
+            maxx1 += maxx1 / 10.0
+            minx1 = min(self.sliding_sigmas_all)
+            minx1 -= minx1 / 10.0
+            maxy1 = max(self.sliding_deviate_all)
+            maxy1 += maxy1 / 10.0
+            miny1 = min(self.sliding_deviate_all)
+            miny1 -= miny1 / 10.0
+
+        else:
+            maxx0 = max(self.delta_sigmas_cut)
+            maxx0 += maxx0 / 10.0
+            minx0 = min(self.delta_sigmas_cut)
+            minx0 -= minx0 / 10.0
+            maxy0 = np.nanmax(self.sliding_deviate_cut)
+            maxy0 += maxy0 / 10.0
+            miny0 = np.nanmin(self.sliding_deviate_cut)
+            miny0 -= miny0 / 10.0
+
+            maxx1 = max(self.sliding_sigma_cut)
+            maxx1 += maxx1 / 10.0
+            minx1 = min(self.sliding_sigma_cut)
+            minx1 -= minx1 / 10.0
+            maxy1 = max(self.sliding_deviate_cut)
+            maxy1 += maxy1 / 10.0
+            miny1 = min(self.sliding_deviate_cut)
+            miny1 -= miny1 / 10.0
 
         axs[0].scatter(
             self.delta_sigmas_all,
             self.sliding_deviate_all,
             marker=".",
             color=sea[3],
             label="All data",
@@ -657,25 +1048,14 @@
         axs[0].set_ylabel(r"$\Delta{\rm SNR}_i$", size=self.axes_labelsize)
         axs[0].set_xlim(minx0, maxx0)
         axs[0].set_ylim(miny0, maxy0)
         axs[0].legend(fontsize=self.legend_fontsize)
         axs[0].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[0].tick_params(axis="y", labelsize=self.legend_fontsize)
 
-        maxx1 = max(self.sliding_sigma_cut)
-        maxx1 += maxx1 / 10.0
-
-        minx1 = min(self.sliding_sigma_cut)
-        minx1 -= minx1 / 10.0
-
-        maxy1 = max(self.sliding_deviate_cut)
-        maxy1 += maxy1 / 10.0
-
-        miny1 = min(self.sliding_deviate_cut)
-        miny1 -= miny1 / 10.0
 
         axs[1].scatter(
             self.sliding_sigmas_all,
             self.sliding_deviate_all,
             marker=".",
             color=sea[3],
             label="All data",
@@ -695,59 +1075,70 @@
         axs[1].set_xlim(minx1, maxx1)
         axs[1].set_ylim(miny1, maxy1)
         axs[1].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[1].tick_params(axis="y", labelsize=self.legend_fontsize)
         axs[1].xaxis.offsetText.set_fontsize(self.legend_fontsize)
 
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-scatter_omega_sigma_dsc.png", bbox_inches = 'tight')
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-scatter_omega_sigma_dsc.png", bbox_inches = 'tight')
+        plt.close()
 
     def plot_hist_omega_pre_post_dsc(self):
         r"""
         Generates and saves a histogram of the :math:`\Delta{\rm SNR}_i` distribution. The plot shows the data before and after the delta-sigma cut (bad GPS times) was applied. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `sliding_deviate_all`).
         """
         fig, axs = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))
 
+        # nan-safing the histograms for good measure...
+        bins=np.histogram(np.hstack((self.sliding_deviate_all[~np.isnan(self.sliding_deviate_all)], self.sliding_deviate_cut[~np.isnan(self.sliding_deviate_cut)])), bins=202)[1]
+        
         axs.hist(
             self.sliding_deviate_all,
-            bins=101,
+            bins,
             color=sea[3],
             ec="k",
             lw=0.5,
             label="All data",
         )
         axs.hist(
             self.sliding_deviate_cut,
-            bins=101,
+            bins,
             color=sea[0],
+            alpha = 0.6,
             ec="k",
             lw=0.5,
             label=r"Data after $|\Delta\sigma|/\sigma$ outlier cut",
         )
+        
         axs.set_xlabel(r"$\Delta{\rm SNR}_i$", size=self.axes_labelsize)
-        axs.set_ylabel(r"\# per bin", size=self.axes_labelsize)
+        axs.set_ylabel(r"count", size=self.axes_labelsize)
         axs.legend(fontsize=self.legend_fontsize)
         axs.set_yscale("log")
         axs.tick_params(axis="x", labelsize=self.legend_fontsize)
         axs.tick_params(axis="y", labelsize=self.legend_fontsize)
 
+        plt.title(r"$\Delta$SNR distribution in" f" {self.time_tag} with/out " + r"$\Delta\sigma$ cut", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-histogram_omega_dsc.png", bbox_inches = 'tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-histogram_omega_dsc.png", bbox_inches = 'tight'
         )
+        plt.close()
 
     def plot_KS_test(self, bias_factor=None):
         """
         Generates and saves a panel plot with results of the Kolmogorov-Smirnov test for Gaussianity. The cumulative distribution of the data (after the delta-sigma (bad GPS times) cut) is compared to the one of Gaussian data, where the bias factor for the sigmas is taken into account. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `sliding_deviate_cut`).
 
         Parameters
         ==========
         bias_factor: float
             Bias factor to consider in the KS calculation.
 
         """
+        if self.delta_sigmas_cut.size==0:
+            return
+
         if bias_factor is None:
             bias_factor = calc_bias(self.segment_duration, self.deltaF, self.deltaT)
         dof_scale_factor = 1.0 / (1.0 + 3.0 / 35.0)
         lx = len(self.sliding_deviate_cut)
 
         sorted_deviates = np.sort(self.sliding_deviate_KS / bias_factor)
 
@@ -762,15 +1153,17 @@
 
         dks_x = max(abs(cdf - normal_cdf))
         lx_eff = lx * dof_scale_factor
 
         lam = (np.sqrt(lx_eff) + 0.12 + 0.11 / np.sqrt(lx_eff)) * dks_x
         pval_KS = StatKS(lam)
 
-        fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 8))
+        fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 8), constrained_layout=True)
+        fig.suptitle(f"Kolmogorov-Smirnov test in {self.time_tag}", fontsize=self.title_fontsize)
+
         axs[0].plot(bins_count[1:], cdf, "k", label="Data")
         axs[0].plot(
             bins_count[1:],
             normal_cdf,
             color=sea[3],
             label=r"Erf with $\sigma$=" + str(round(bias_factor, 2)),
         )
@@ -796,60 +1189,86 @@
             xy=(0.025, 0.9),
             xycoords="axes fraction",
             size = self.annotate_fontsize
         )
         axs[1].tick_params(axis="x", labelsize=self.legend_fontsize)
         axs[1].tick_params(axis="y", labelsize=self.legend_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-KS_test.png", bbox_inches = 'tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-KS_test.png", bbox_inches = 'tight'
         )
+        plt.close()
 
-    def plot_hist_sigma_squared(self):
+    def plot_hist_sigma_squared(self, max_val = 5, total_bins=100, label_number = 6):
         """
         Generates and saves a histogram of :math:`\sigma^2/\langle\sigma^2\rangle`. The plot shows data after the delta-sigma (bad GPS times) cut. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. self.sliding_sigma_cut).
 
         Parameters
         ==========
 
         Returns
         =======
 
         """
+        if self.delta_sigmas_cut.size==0:
+            return
+        
+        values = 1 / np.nanmean(self.sliding_sigma_cut ** 2) * self.sliding_sigma_cut ** 2
+        
+        values_clipped = np.ones(len(values))
+        
+        for i in range(len(values_clipped)):
+            if values[i] >= max_val:
+                values_clipped[i] = max_val
+            else:
+                values_clipped[i] = values[i]
+                
+        bins = np.linspace(0, max(values_clipped), total_bins)
+        
         fig, axs = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))
-        axs.hist(
-            1 / np.nanmean(self.sliding_sigma_cut ** 2) * self.sliding_sigma_cut ** 2,
-            bins=1500,
+        _, bins, patches = plt.hist(
+            values_clipped,
+            bins=bins,
             color=sea[0],
             ec="k",
             lw=0.5,
             label=r"Data after $|\Delta\sigma|/\sigma$ outlier cut",
         )
+        
         axs.set_xlabel(r"$\sigma^2/\langle\sigma^2\rangle$", size=self.axes_labelsize)
-        axs.set_ylabel(r"\# per bin", size=self.axes_labelsize)
+        axs.set_ylabel(r"count", size=self.axes_labelsize)
         axs.set_yscale("log")
-        axs.set_xlim(0, 5)
+        axs.set_xlim(0, max_val)
         axs.legend(fontsize=self.legend_fontsize)
         axs.tick_params(axis="x", labelsize=self.legend_fontsize)
         axs.tick_params(axis="y", labelsize=self.legend_fontsize)
-
+        
+        xticks_tmp = np.linspace(0, max_val, label_number)
+        labels = [str(i) for i in xticks_tmp]
+        labels[-1]+="+"
+        plt.xticks(xticks_tmp, labels)
+        
+        plt.title(f"Relative variance in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-histogram_sigma_squared.png", bbox_inches = 'tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-histogram_sigma_squared.png", bbox_inches = 'tight'
         )
+        plt.close()
 
     def plot_omega_time_fit(self):
         """
         Generates and saves a plot of :math:`\Omega` as a function of time and fits the data to perform a linear trend analysis. The plot shows data after the delta-sigma (bad GPS times) cut. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. self.sliding_omega_cut).
 
         Parameters
         ==========
 
         Returns
         =======
 
         """
+        if self.days_cut.size==0:
+            return
         fig, axs = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))
 
         t_obs = self.days_cut[-1]
         scale = np.sqrt(np.var(self.sliding_omega_cut))
 
         def func(x, a, b):
             return a * (x - t_obs / 2) * t_obs + b
@@ -865,15 +1284,15 @@
             sigma=sliding_sigma_cut_nansafe,
         )
         c1, c2 = popt[0], popt[1]
         axs.plot(self.days_cut, func(self.days_cut, c1, c2), color=sea[3])
         axs.plot(self.days_cut, self.sliding_omega_cut, '.', color=sea[0], markersize=1)
         axs.plot(self.days_cut, 3 * self.sliding_sigma_cut, color=sea[0], linewidth=1.5)
         axs.plot(self.days_cut, -3 * self.sliding_sigma_cut, color=sea[0], linewidth=1.5)
-        axs.set_xlabel("Days since start of run", size=self.axes_labelsize)
+        axs.set_xlabel(self.xaxis, size=self.axes_labelsize)
         axs.set_ylabel(r"$\Omega_i$", size=self.axes_labelsize)
         axs.set_xlim(self.days_cut[0], self.days_cut[-1])
         axs.annotate(
             r"Linear trend analysis: $\Omega(t) = C_1 (t-T_{\rm obs}/2) T_{\rm obs} + C_2 C_1 = $"
             + str(f"{c1:.3e}")
             + "\nC$_2$ = "
             + str(f"{c2:.3e}"),
@@ -881,22 +1300,27 @@
             xycoords="axes fraction",
             size = self.annotate_fontsize,
             bbox=dict(boxstyle="round", facecolor="white", alpha=1),
         )
         axs.tick_params(axis="x", labelsize=self.legend_fontsize)
         axs.tick_params(axis="y", labelsize=self.legend_fontsize)
         axs.xaxis.offsetText.set_fontsize(self.legend_fontsize)
+        plt.title(r"Time evolution of $\Omega$ " + f"in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-omega_time_fit.png", bbox_inches = 'tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-omega_time_fit.png", bbox_inches = 'tight'
         )
+        plt.close()
 
     def plot_sigma_time_fit(self):
         """
         Generates and saves a plot of :math:`\sigma` as a function of time and fits the data to perform a linear trend analysis. The plot shows data after the delta-sigma (bad GPS times) cut. This function does not require any input parameters, as it accesses the data through the attributes of the class (e.g. `sliding_sigma_cut`).
         """
+        if self.days_cut.size==0:
+            return
+
         fig, axs = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))
 
         t_obs = self.days_cut[-1]
         scale = np.sqrt(np.var(self.sliding_sigma_cut))
 
         def func(x, a, b):
             return a * (x - t_obs / 2) * t_obs + b
@@ -909,15 +1333,15 @@
             func,
             self.days_cut[nanmask],
             sliding_sigma_cut_nansafe,
         )
         c1, c2 = popt[0], popt[1]
         axs.plot(self.days_cut, func(self.days_cut, c1, c2), color=sea[3])
         axs.plot(self.days_cut, self.sliding_sigma_cut, ".", color=sea[0], markersize=1)
-        axs.set_xlabel("Days since start of run", size=self.axes_labelsize)
+        axs.set_xlabel(self.xaxis, size=self.axes_labelsize)
         axs.set_ylabel(r"$\sigma_i$", size=self.axes_labelsize)
         axs.set_xlim(self.days_cut[0], self.days_cut[-1])
         axs.set_ylim(mean_sigma - 1.2 * mean_sigma, mean_sigma + 2.2 * mean_sigma)
         axs.annotate(
             r"Linear trend analysis: $\sigma(t) = C_1 (t-T_{\rm obs}/2) T_{\rm obs} + C_2 C_1 = $"
             + str(f"{c1:.3e}")
             + "\nC$_2$ = "
@@ -925,17 +1349,70 @@
             xy=(0.05, 0.05),
             xycoords="axes fraction",
             size = self.annotate_fontsize,
             bbox=dict(boxstyle="round", facecolor="white", alpha=1),
         )
         axs.tick_params(axis="x", labelsize=self.legend_fontsize)
         axs.tick_params(axis="y", labelsize=self.legend_fontsize)
+        plt.title(r"Time evolution of $\sigma$ " + f"in {self.time_tag}", fontsize=self.title_fontsize)
+        plt.savefig(
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-sigma_time_fit.png", bbox_inches = 'tight'
+        )
+        plt.close()
+
+    def plot_gates_in_time(self):
+        if self.gates_ifo1 is None and self.gates_ifo2 is None:
+            self.gates_ifo1_statement=None
+            self.gates_ifo2_statement=None
+            return
+        
+        fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(10, 8))
+        if self.gates_ifo1 is None:
+            self.gates_ifo1_statement=None
+        else:
+            self.total_gated_time_ifo1 = np.sum(self.gates_ifo1[:,1]-self.gates_ifo1[:,0])
+            self.total_gated_percent_ifo1 = self.total_gated_time_ifo1/(int(self.sliding_times_all[-1])- int(self.sliding_times_all[0]))*100
+            gate_times_in_days_ifo1 = (np.array(self.gates_ifo1[:,0]) - self.sliding_times_all[0]) / 86400.0
+            self.gates_ifo1_statement= f"Data gated out: {self.total_gated_time_ifo1} s\n" f"Percentage: {float(f'{self.total_gated_percent_ifo1:.2g}'):g}%"
+            gatefig1 = ax.plot(gate_times_in_days_ifo1, self.gates_ifo1[:,1]-self.gates_ifo1[:,0], 's', color=sea[3], label="IFO1:\n" f"{self.gates_ifo1_statement}")
+            first_legend = ax.legend(handles=gatefig1, loc=(0.05,0.75), fontsize = self.axes_labelsize)
+            ax.add_artist(first_legend)
+        if self.gates_ifo2 is None:
+            self.gates_ifo2_statement=None
+        else:
+            self.total_gated_time_ifo2 = np.sum(self.gates_ifo2[:,1]-self.gates_ifo2[:,0])
+            self.total_gated_percent_ifo2 = self.total_gated_time_ifo2/(int(self.sliding_times_all[-1])- int(self.sliding_times_all[0]))*100
+            gate_times_in_days_ifo2 = (np.array(self.gates_ifo2[:,0]) - self.sliding_times_all[0]) / 86400.0
+            self.gates_ifo2_statement= f"Data gated out: {self.total_gated_time_ifo2} s\n" f"Percentage: {float(f'{self.total_gated_percent_ifo2:.2g}'):g}%"
+            gatefig2 = ax.plot(gate_times_in_days_ifo2, self.gates_ifo2[:,1]-self.gates_ifo2[:,0], 's', color=sea[0], label="IFO2:\n" f"{self.gates_ifo2_statement}")
+            ax.legend(handles=gatefig2, loc=(0.05, 0.1), fontsize = self.axes_labelsize)
+        ax.set_xlabel(self.xaxis, size=self.axes_labelsize)
+        ax.set_ylabel("Gate length (s)", size=self.axes_labelsize)
+        plt.xticks(fontsize=self.legend_fontsize)
+        plt.yticks(fontsize=self.legend_fontsize)
+        plt.title(f"Gates applied to {self.baseline_name} in {self.time_tag}", fontsize=self.title_fontsize)
         plt.savefig(
-            f"{self.plot_dir / self.baseline_name}-{self.sliding_times_all[0]}-{self.sliding_times_all[-1]}-sigma_time_fit.png", bbox_inches = 'tight'
+            f"{self.plot_dir / self.baseline_name}-{self.file_tag}-gates_time.png",
+            bbox_inches="tight",
         )
+        plt.close()
+            
+
+
+    def save_all_statements(self):
+        """
+        Saves all useful statements gathered throughout the checks to a json file.
+        """
+        statements = {}
+        statements['dsc'] = self.dsc_statement
+        statements['gates_ifo1'] = self.gates_ifo1_statement
+        statements['gates_ifo2'] = self.gates_ifo2_statement
+        statements['n_segs'] = self.n_segs_statement
+        with open("stats_statements.json", "w") as outfile:
+                json.dump(statements, outfile)
 
     def generate_all_plots(self):
         """
         Generates and saves all the statistical analysis plots.
         """
         self.plot_running_point_estimate()
         self.plot_running_sigma()
@@ -951,136 +1428,106 @@
         self.plot_scatter_sigma_dsc()
         self.plot_scatter_omega_sigma_dsc()
         self.plot_hist_omega_pre_post_dsc()
         self.plot_KS_test()
         self.plot_hist_sigma_squared()
         self.plot_omega_time_fit()
         self.plot_sigma_time_fit()
+        self.plot_gates_in_time()
+        if self.coherence_spectrum is not None:
+            self.plot_coherence_spectrum()
+            self.plot_hist_coherence()
+        self.save_all_statements()
 
 
 def sortingFunction(item):
     return float(item[5:].partition("-")[0])
 
 
 def run_statistical_checks_from_file(
-    combine_file_path, dsc_file_path, plot_dir, param_file, legend_fontsize=16
+    combine_file_path, dsc_file_path, plot_dir, param_file, legend_fontsize=16, coherence_file_path = None, file_tag = None, convention='pygwb'
 ):
     """
     Assumes files are in npz for now. Will generalize later.
     """
     params = Parameters()
     params.update_from_file(param_file)
 
     spectra_file = np.load(combine_file_path)
     dsc_file = np.load(dsc_file_path)
 
     badGPStimes = dsc_file["badGPStimes"]
     delta_sigmas = dsc_file["delta_sigmas"]
     sliding_times = dsc_file["times"]
     naive_sigma_all = dsc_file["naive_sigmas"]
+    gates_ifo1 = dsc_file["gates_ifo1"]
+    gates_ifo2 = dsc_file["gates_ifo2"]
+    if gates_ifo1.size==0:
+        gates_ifo1=None
+    if gates_ifo2.size==0:
+        gates_ifo2=None
 
     sliding_omega_all, sliding_sigmas_all = (
         spectra_file["point_estimates_seg_UW"],
         spectra_file["sigmas_seg_UW"],
     )
 
-    freqs = np.arange(
+    frequencies = np.arange(
         0,
         params.new_sample_rate / 2.0 + params.frequency_resolution,
         params.frequency_resolution,
     )
-    cut = (params.fhigh >= freqs) & (freqs >= params.flow)
+    frequency_cut = (params.fhigh >= frequencies) & (frequencies >= params.flow)
+    try:
+        frequency_mask = spectra_file["frequency_mask"]
+    except KeyError:
+        try:
+            notch_list_path = params.notch_list_path
+            logger.debug("loading notches from " + notch_list_path)
+            notch_list = StochNotchList.load_from_file(notch_list_path)
+            frequency_mask = notch_list.get_notch_mask(frequencies[frequency_cut])
+
+        except:
+            frequency_mask = None
 
     spectrum_file = np.load(combine_file_path, mmap_mode="r")
 
     point_estimate_spectrum = spectrum_file["point_estimate_spectrum"]
     sigma_spectrum = spectrum_file["sigma_spectrum"]
 
     baseline_name = params.interferometer_list[0] + params.interferometer_list[1]
 
     # select alpha for statistical checks
     delta_sigmas_sel = delta_sigmas.T[1]
     naive_sigmas_sel = naive_sigma_all.T[1]
 
+    if coherence_file_path is not None:
+        coh_data = np.load(coherence_file_path, allow_pickle=True)
+        coherence_spectrum = coh_data['coherence']
+        coherence_n_segs = coh_data['n_segs_coh']
+    else:
+        coherence_spectrum = None
+        coherence_n_segs = None
+
     return StatisticalChecks(
         sliding_times,
         sliding_omega_all,
         sliding_sigmas_all,
         naive_sigmas_sel,
+        coherence_spectrum,
+        coherence_n_segs,
         point_estimate_spectrum,
         sigma_spectrum,
-        freqs[cut],
+        frequencies[frequency_cut],
         badGPStimes,
         delta_sigmas_sel,
         plot_dir,
         baseline_name,
         param_file,
-        legend_fontsize=legend_fontsize
-    )
-
-
-def run_statistical_checks_baseline_pickle(
-    baseline_directory, combine_file_path, plot_dir, param_file
-):
-    params = Parameters()
-    params.update_from_file(param_file)
-    baseline_directory = Path(baseline_directory)
-
-    baseline_list = [
-        f
-        for f in listdir(baseline_directory)
-        if isfile(join(baseline_directory, f))
-        if f.startswith("H1")
-    ]
-    baseline_list.sort(key=sortingFunction)
-
-    baseline_list = np.array(baseline_list)
-
-    file_0 = join(baseline_directory, baseline_list[0])
-    baseline_0 = Baseline.load_from_pickle(file_0)
-
-    freqs = baseline_0.frequencies
-    baseline_name = baseline_0.name
-
-    bad_GPS_times = np.array([])
-    delta_sigmas = []
-    naive_sigmas = []
-    sliding_times = []
-
-    for baseline in baseline_list:
-        print(f"loading baseline file {baseline}...")
-        filename = join(baseline_directory, baseline)
-        base = Baseline.load_from_pickle(filename)
-
-        bad_GPS_times = np.append(bad_GPS_times, base.badGPStimes)
-
-        delta_sigmas.append(base.delta_sigmas["values"][1])
-        naive_sigmas.append(base.delta_sigmas["naive_sigmas"][1])
-        sliding_times.append(base.delta_sigmas["times"])
-
-    delta_sigmas = np.concatenate(delta_sigmas)
-    naive_sigmas = np.concatenate(naive_sigmas)
-    sliding_times = np.concatenate(sliding_times)
-
-    spectrum_file = np.load(combine_file_path, mmap_mode="r")
-
-    sliding_omega_all, sliding_sigmas_all = (
-        spectrum_file["point_estimates_seg_UW"],
-        spectrum_file["sigmas_seg_UW"],
+        frequency_mask,
+        gates_ifo1,
+        gates_ifo2,
+        file_tag=file_tag,
+        legend_fontsize=legend_fontsize,
+        convention=convention
     )
-    point_estimate_spectrum = spectrum_file["point_estimate_spectrum"]
-    sigma_spectrum = spectrum_file["sigma_spectrum"]
 
-    return StatisticalChecks(
-        sliding_times,
-        sliding_omega_all,
-        sliding_sigmas_all,
-        naive_sigmas,
-        point_estimate_spectrum,
-        sigma_spectrum,
-        freqs,
-        bad_GPS_times,
-        delta_sigmas,
-        plot_dir,
-        baseline_name,
-        param_file,
-    )
```

### Comparing `pygwb-1.0.0/pygwb/util.py` & `pygwb-1.3.0/pygwb/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,19 +43,22 @@
     w1w2squaredovlbar: float
     """
     window_tuple = get_window_tuple(window_fftgram_dict)
     w = get_window(window_tuple, N, fftbins=False)
     w1w2bar = np.mean(w ** 2)
     w1w2squaredbar = np.mean(w ** 4)
 
-    w1 = w[N - int(N * overlap_factor) : N] 
-    w2 = w[0 : int(N * overlap_factor)] 
-
-    w1w2squaredovlbar = 1 / (N * overlap_factor) * np.sum(w1 ** 2 * w2 ** 2)
-    w1w2ovlbar = 1 / (N * overlap_factor) * np.sum(w1 * w2)
+    S = N - int(overlap_factor*N)
+    
+    if overlap_factor==0.0 or overlap_factor==0:
+        w1w2squaredovlbar = 0.0
+        w1w2ovlbar = 0.0
+    else:
+        w1w2squaredovlbar = 1 / (N*overlap_factor) * np.sum(w[0:N-S]**2*w[S:N]**2)
+        w1w2ovlbar = 1 / (N*overlap_factor) * np.sum(w[0:N-S]*w[S:N])
 
     return w1w2bar, w1w2squaredbar, w1w2ovlbar, w1w2squaredovlbar
 
 
 def get_window_tuple(window_fftgram_dict={"window_fftgram": "hann"}):
     """
     Unpack the `window_fft_dict` dictionary into a `tuple` that may be read by scipy.get_window.
@@ -170,15 +173,15 @@
     
     # K is the number of segments that will be averaged in the corresponding Welch estimate
     K = 1 + int((nSamples - N)/S)
 
     # Form the weighted sum of the window correlations for shifts j = 1 to K-1
     rho_sum = 0
     for j in range(1, K):
-        rho_sum = rho_sum + (K - j)/K*calc_rho(N, j, window_tuple=window_tuple, overlap_factor=overlap_factor)
+        rho_sum += (K - j)/K*calc_rho(N, j, window_tuple=window_tuple, overlap_factor=overlap_factor)
     
     Neff = K/(1 + 2 * rho_sum)
 
     return Neff
 
 
 def calc_bias(
@@ -216,18 +219,23 @@
     # Number of samples in the window used for Welch's estimate
     N = int(1 / (deltaT * deltaF))
 
     # Effective number of segments that are averaged for this windowing scheme
     window_tuple = get_window_tuple(window_fftgram_dict)
     Neff = effective_welch_averages(nSamples, N, window_tuple, overlap_factor=overlap_factor)
 
-    # Correction for number of PSDs that will be averaged 
-    Neff = N_avg_segs * Neff
-    
-    bias = Neff / (Neff - 1)
+    # if Neff is the same as the true number of segments, no bias.
+    if Neff == (nSamples/N):
+        bias = 1.0
+
+    else:
+        # Correction for number of PSDs that will be averaged 
+        Neff = N_avg_segs * Neff
+        bias = Neff / (Neff - 1)
+
     return bias
 
 
 def omega_to_power(omega_GWB, frequencies):
     """
     Compute the GW power spectrum starting from the omega_GWB
     spectrum.
```

### Comparing `pygwb-1.0.0/pygwb/workflow.py` & `pygwb-1.3.0/pygwb_pipe/pygwb_create_isotropic_workflow`

 * *Files 20% similar despite different names*

```diff
@@ -1,230 +1,196 @@
+#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) California Institute of Technology 2023
 #
 # This file is part of pygwb.
 
-"""Core workflow functions"""
-
+import argparse
+import configparser
+import distutils
+import glob
+import logging
 import os
-import shutil
-from collections.abc import Iterable
-from getpass import getuser
-
-from pycondor import Dagman as pyDagman
-from pycondor import Job as pyJob
-
-ACCOUNTING_GROUP_USER = os.getenv(
-    '_CONDOR_ACCOUNTING_USER',
-    getuser(),
-)
-
-def makedir(dir_path):
-    if not os.path.exists(dir_path):
-        os.makedirs(dir_path)
-
-def config_override(config, overrides):
-    if not overrides:
-        return config 
-    for ov in overrides:
-        split_ov = ov.split(':')
-        try:
-            ov_sec, ov_key, ov_val = \
-                split_ov[0], split_ov[1], ':'.join(split_ov[2:])
-        except:
-            raise ValueError(f"Overrides must be in the form 'section:key:value', you used '{ov}'")
-        if ov_sec not in config.sections():
-            config[ov_sec] = {}    
-        config[ov_sec][ov_key] = ov_val
-    return config
-
-def config_write(config, output_loc):
-    with open(output_loc, 'w') as configfile:
-        config.write(configfile)
-
-
-class Job(pyJob):
-    """
-    Wrapper class of pycondor.Job
-    """
-
-    def __init__(self, name, executable, output_arg=None, 
-                 output_file=None, accounting_group=None, 
-                 extra_lines=[], arguments=None,retry=None,
-                 request_disk='2048MB', request_memory='512MB',
-                 **kwargs):
-
-        exec_path = shutil.which(executable)
-        if exec_path is None:
-            raise TypeError('execuatble must be installed in environment'+
-                       ' or given as an absolute path')
-
-        if accounting_group is not None:
-            condorcmds = [
-                f"accounting_group = {accounting_group}",
-                f"accounting_group_user = {ACCOUNTING_GROUP_USER}",
-                ]
-            condorcmds.extend(extra_lines)
+
+import numpy as np
+import pandas as pd
+import pycondor
+from pycondor import Dagman
+
+from pygwb.html import pygwb_html
+from pygwb.workflow import Dagman, IsotropicWorkflow, Job, makedir
+
+__process_name__ = 'pygwb_create_workflow'
+__version__ = '1.2.2'
+
+
+def make_workflow(args=None):
+
+    pygwb_wf = IsotropicWorkflow('pygwb_dagman', 
+                                 config_file=args.configfile,
+                                 basedir=args.basedir,
+                                 config_overrides=args.config_overrides)
+
+    seglist_pruned = pygwb_wf.setup_segments()
+
+    # check if we want segment-level results
+    if pygwb_wf.config.has_option('general', 'plot_segment_results'):
+        segment_results = bool(distutils.util.strtobool(pygwb_wf.config['general']['plot_segment_results']))
+    else:
+        segment_results = False
+
+    all_jobs = []
+    pipe_jobs = []
+
+    cumu_dir = os.path.join(pygwb_wf.dagman.result_dir, 'combined_results/')
+    makedir(cumu_dir)
+
+    first_start = int(seglist_pruned[0][0])
+    last_start = 0
+
+    all_coh_files = []
+    all_data_files = []
+    all_param_files = []
+    for seg in seglist_pruned:
+        start = int(seg[0])
+        end = int(seg[1])
+        dur = int(end-start)
+        seg_dir = os.path.join(pygwb_wf.dagman.result_dir, f'{start}-{dur}/')
+        makedir(seg_dir)
+
+        last_start = start
+
+        pipe_job, pipe_output = pygwb_wf.create_pygwb_pipe_job(parents=[], 
+            output_path=seg_dir, 
+            t0=start, tf=end
+            )
+        all_jobs.append(pipe_job)
+        pipe_jobs.append(pipe_job)
+        param_file, coh_file, data_file = pipe_output
+        all_param_files.append(param_file)
+        all_coh_files.append(coh_file)
+        all_data_files.append(data_file)
+
+        if segment_results:
+            # extra vars
+            combine_job, combine_output = pygwb_wf.create_pygwb_combine_job(
+                t0=start, tf=end,
+                parents=[pipe_job], output_path=seg_dir,
+                data_path=data_file, coherence_path=coh_file, param_file=param_file,
+                alpha=pygwb_wf.alpha, fref=pygwb_wf.fref)
+            all_jobs.append(combine_job)
+
+            # extra vars
+            csd_file, coh_file, dsc_file = combine_output
+            stats_job = pygwb_wf.create_pygwb_stats_job(
+                t0=start, tf=end,
+                parents=[combine_job], output_path=seg_dir,
+                csd_file=csd_file,
+                dsc_file=dsc_file,
+                coh_file=coh_file,
+                param_file=param_file)
+            all_jobs.append(stats_job)
+
+    # make cumulative results
+    # FIX ME - how the param file is passed
+    cumu_combine_job, cumu_combine_output = pygwb_wf.create_pygwb_combine_job(
+        t0=pygwb_wf.t0, tf=pygwb_wf.tf,
+        parents=pipe_jobs, output_path=cumu_dir,
+        data_path=all_data_files, coherence_path=all_coh_files, param_file=all_param_files[-1],
+        alpha=pygwb_wf.alpha, fref=pygwb_wf.fref)
+    all_jobs.append(cumu_combine_job)
+
+    csd_file, coh_file, dsc_file = cumu_combine_output
+    cumu_stats_job = pygwb_wf.create_pygwb_stats_job(
+        t0=pygwb_wf.t0, tf=pygwb_wf.tf,
+        parents=[cumu_combine_job], output_path=cumu_dir,
+        csd_file=csd_file,
+        dsc_file=dsc_file,
+        coh_file=coh_file,
+        param_file=all_param_files[-1]) # Also FIX ME (param_file)
+    all_jobs.append(cumu_stats_job)
+
+    pygwb_html(pygwb_wf.dagman.base_dir, config=pygwb_wf.config_path, segment_results=segment_results)
+
+    # write out segment list and job file
+    seg_dir = os.path.join(pygwb_wf.dagman.result_dir, 'segment_lists/')
+    makedir(seg_dir)
+    start_list = np.array(seglist_pruned).T[0]
+    end_list = np.array(seglist_pruned).T[1]
+    dur_list = end_list - start_list
+    ones_list = np.ones(len(dur_list), dtype=int)
+    df = pd.DataFrame(data={'one': ones_list,
+                            'start': start_list,
+                            'end': end_list,
+                            'dur': dur_list})
+    jobfile_loc = os.path.join(seg_dir, "jobfile.dat") 
+    df.to_csv(jobfile_loc, sep = " ", header=False, index=False)
+
+    # make html page
+    html_job = pygwb_wf.create_pygwb_html_job( 
+        t0=pygwb_wf.t0, tf=pygwb_wf.tf, parents=all_jobs, segment_results=segment_results,
+        output_path=pygwb_wf.dagman.base_dir, plot_path=pygwb_wf.dagman.result_dir)
+
+    # parse the cache file and filter workflow
+    if pygwb_wf.cache_file_path:
+        logging.info('Parsing cache file...')
+        cache = pygwb_wf.dagman.load_cache(pygwb_wf.cache_file_path)
+        if len(cache):
+            logging.info('Filtering out pre-computed jobs from workflow...')
+            pygwb_wf.dagman.filter_and_remove_from_cache(cache)
         else:
-            raise TypeError('accounting group must be supplied')
+            logging.info('No files were found in cache file, skipping...')
 
-        output_args = []
-            
-        if output_file is not None:
-            if isinstance(output_arg, str):
-                output_args.append(output_arg)
-                if isinstance(output_file, str):
-                    self.output_file = [output_file]
-                    output_args.append(output_file)
-                elif isinstance(output_file, Iterable):
-                    self.output_file = output_file
-                    for arg in output_file:
-                        output_args.append(arg) 
-                else:
-                    raise TypeError('output_files must be a string or an iterable')
-            else:
-                raise TypeError('output_arg must be a string')
-                
-        arguments = ' '.join(list([arguments])+list(output_args))
-
-        if retry == None:
-            retry = 3
-            
-        super(Job,self).__init__(name, exec_path, arguments=arguments,
-                                 extra_lines=condorcmds, retry=retry, 
-                                 request_disk=request_disk, 
-                                 request_memory=request_memory, 
-                                 **kwargs)
-
-class Dagman(pyDagman):
-    """
-    Wrapper class of pycondor.Dagman
-    """
-    def __init__(self, name, basedir=None, **kwargs):
-        self.base_dir = os.path.abspath(basedir)
-        self.submit_dir = os.path.join(self.base_dir, 'condor')
-        self.error_dir = os.path.join(self.base_dir, 'condor')
-        self.log_dir = os.path.join(self.base_dir, 'condor')
-        self.output_dir = os.path.join(self.base_dir, 'condor')
-        self.result_dir = os.path.join(self.base_dir, 'output')
-        super(Dagman,self).__init__(name, submit=self.submit_dir, **kwargs)
-
-    def make_dir(self):
-       makedir(self.base_dir)
-       makedir(self.submit_dir)
-       makedir(self.error_dir)
-       makedir(self.log_dir)
-       makedir(self.output_dir)
-       makedir(self.result_dir)
-
-def collect_job_arguments(config, job_type):
-    config_sec = config[job_type]
-    args_list = list()
-    for key in config_sec.keys():
-        args_list.append('--' + str(key))
-        val = str(config_sec[key])
-        if val[0] == '$':
-            val_source = val.replace('${', '').replace('}', '')
-            val_source = val_source.split(':')
-            val = config[val_source[0]][val_source[1]]
-        args_list.append(val)
-    return args_list
-
-def create_pygwb_pipe_job(dagman, config, t0=None, tf=None, parents=[], output_path=None):
-#pygwb_pipe --param_file parameters.ini --output_path output/ --t0 ${START} --tf ${END}
-    dur = int(tf-t0)
-    name = f'pygwb_pipe_{int(t0)}_{dur}'
-    args = collect_job_arguments(config, 'pygwb_pipe')
-    args = args + [
-        '--output_path', output_path,
-        '--t0', str(t0),
-        '--tf', str(tf)
-        ]
-    job = Job(name=name,
-              executable=config['executables']['pygwb_pipe'],
-              accounting_group = config['general']['accounting_group'],
-              submit=dagman.submit_dir,
-              error=dagman.error_dir,
-              output=dagman.output_dir,
-              log=dagman.log_dir,
-              arguments=' '.join(args),
-              request_disk='128MB',
-              request_memory='2048MB',
-              dag=dagman)
-    for parent in parents:
-        job.add_parent(parent)
-    return job
-
-def create_pygwb_combine_job(dagman, config, t0=None, tf=None, parents=[], output_path=None,
-    data_path=None, param_file=None,
-    alpha=0., fref=30, h0=0.7):
-#pygwb_combine --data_path output/ --param_file output/parameters_final.ini --alpha 0 --fref 30 --h0 0.7 --out_path ./output/
-    dur = int(tf-t0)
-    name = f'pygwb_combine_{int(t0)}_{dur}'
-    args = collect_job_arguments(config, 'pygwb_combine')
-    args = args + [
-        '--param_file', param_file,
-        '--out_path', output_path,
-        '--data_path', data_path,
-        ]
-    job = Job(name=name,
-              executable=config['executables']['pygwb_combine'],
-              accounting_group = config['general']['accounting_group'],
-              submit=dagman.submit_dir,
-              error=dagman.error_dir,
-              output=dagman.output_dir,
-              log=dagman.log_dir,
-              arguments=' '.join(args),
-              request_disk='128MB',
-              request_memory='1024MB',
-              dag=dagman)
-    for parent in parents:
-        job.add_parent(parent)
-    return job
-
-def create_pygwb_stats_job(dagman, config, t0=None, tf=None, parents=[], output_path=None,
-    csd_file=None, dsc_file=None, param_file=None):
-    dur = int(tf-t0)
-    name = f'pygwb_stats_{int(t0)}_{dur}'
-    args = collect_job_arguments(config, 'pygwb_stats')
-    args = args + [
-        '-pf', param_file,
-        '-pd', output_path,
-        '-c', csd_file,
-        '-dsc', dsc_file
-        ]
-    job = Job(name=name,
-              executable=config['executables']['pygwb_stats'],
-              accounting_group = config['general']['accounting_group'],
-              submit=dagman.submit_dir,
-              error=dagman.error_dir,
-              output=dagman.output_dir,
-              log=dagman.log_dir,
-              arguments=' '.join(args),
-              request_disk='128MB',
-              request_memory='512MB',
-              dag=dagman)
-    for parent in parents:
-        job.add_parent(parent)
-    return job
-
-def create_pygwb_html_job(dagman, config, t0=None, tf=None, parents=[], output_path=None, plot_path=None):
-    name = f'pygwb_html'
-    args = collect_job_arguments(config, 'pygwb_html')
-    args = args + [
-        '-p', plot_path,
-        '-o', output_path,
-        ]
-    job = Job(name=name,
-              executable=config['executables']['pygwb_html'],
-              accounting_group = config['general']['accounting_group'],
-              submit=dagman.submit_dir,
-              error=dagman.error_dir,
-              output=dagman.output_dir,
-              log=dagman.log_dir,
-              arguments=' '.join(args),
-              request_disk='128MB',
-              request_memory='1024MB',
-              dag=dagman)
-    for parent in parents:
-        job.add_parent(parent)
-    return job
+    new_cache_path = os.path.join(pygwb_wf.dagman.base_dir, 'pygwb_cache.txt')
+    logging.info(f'Writing out new cache file at {new_cache_path}')
+    pygwb_wf.dagman.save_output_loc(output_loc=new_cache_path)
+
+    pygwb_wf.dagman.build(fancyname=False)
+
+    if args.submit:
+        logging.info('Submitting to condor...')
+        pygwb_wf.dagman.submit_dag()
+    elif args.run_locally:
+        pygwb_wf.dagman.run_jobs_serially()
+    else:
+        logging.info('PyGWB Isotropic Workflow can be submitted to condor by running the following:'
+                      f'\n\n\t  condor_submit_dag {pygwb_wf.dagman.submit_file}\n')
+
+    logging.info('Done')
+
+
+def main(args=None):
+    logging.basicConfig(format='%(asctime)s:%(levelname)s : %(message)s',
+                    level=logging.WARNING)
+    logger = logging.getLogger()
+
+    parser = argparse.ArgumentParser(description=__doc__,
+                                     prog=__process_name__)
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='increase verbose output')
+    parser.add_argument('--debug', action='store_true',
+                        help='increase verbose output to debug')
+    parser.add_argument('-V', '--version', action='version',
+                        version=__version__)
+    parser.add_argument('--basedir', type=os.path.abspath, required=True,
+            help='Build directory for condor logging')
+    parser.add_argument('--configfile', type=str, required=True,
+            help='config file with workflow parameters')
+    parser.add_argument('--config-overrides', type=str, nargs='+', default=[],
+            help='config overrides listed in the form SECTION:KEY:VALUE')
+    parser.add_argument('--submit', action='store_true',
+            help='Submit workflow automatically')
+    parser.add_argument('--run_locally', action='store_true',
+            help='Run job on local universe')
+    args = parser.parse_args(args=args)
+
+    if args.verbose:
+        logger.setLevel(logging.INFO)
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+
+    # call the above function
+    make_workflow(args=args)
+
+# allow be be run on the command line
+if __name__ == "__main__":
+    main(args=None)
```

### Comparing `pygwb-1.0.0/pygwb.egg-info/PKG-INFO` & `pygwb-1.3.0/pygwb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwb
-Version: 1.0.0
+Version: 1.3.0
 Summary: Lighweight python stochastic GWB analysis pipeline
 Home-page: https://git.ligo.org/pygwb/pygwb
 Author: Arianna Renzini, Sylvia Biscoveanu, Shivaraj Khandasamy, Kamiel Janssens, Max Lalleman, Katarina Martinovic, Andrew Matas, Patrick Meyers, Alba Romero, Colm Talbot, Leo Tsukada, Kevin Turbang
 Author-email: arianna.renzini@ligo.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pygwb-1.0.0/pygwb.egg-info/SOURCES.txt` & `pygwb-1.3.0/pygwb.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 docs/Makefile
 pygwb/__init__.py
 pygwb/_version.py
 pygwb/baseline.py
+pygwb/coherence.py
 pygwb/constants.py
 pygwb/delta_sigma_cut.py
 pygwb/detector.py
 pygwb/html.py
 pygwb/network.py
 pygwb/notch.py
 pygwb/omega_spectra.py
@@ -34,15 +35,14 @@
 pygwb.egg-info/PKG-INFO
 pygwb.egg-info/SOURCES.txt
 pygwb.egg-info/dependency_links.txt
 pygwb.egg-info/requires.txt
 pygwb.egg-info/top_level.txt
 pygwb_pipe/README.md
 pygwb_pipe/parameters.ini
-pygwb_pipe/parameters_mock.ini
 pygwb_pipe/pygwb_combine
 pygwb_pipe/pygwb_create_isotropic_workflow
 pygwb_pipe/pygwb_dag
 pygwb_pipe/pygwb_html
 pygwb_pipe/pygwb_pe
 pygwb_pipe/pygwb_pipe
 pygwb_pipe/pygwb_stats
```

### Comparing `pygwb-1.0.0/pygwb_pipe/README.md` & `pygwb-1.3.0/pygwb_pipe/README.md`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb_pipe/parameters.ini` & `pygwb-1.3.0/pygwb_pipe/parameters.ini`

 * *Files 4% similar despite different names*

```diff
@@ -40,22 +40,25 @@
 ; amplitude threshold, if the data exceeds this value a gating window will be placed
 gate_threshold: 50
 ; time duration (seconds) over which gating points will be clustered
 cluster_window: 0.5
 [window_fft_specs]
 ; Window used for fft (used CSD and PSD estimation)
 window_fftgram: hann
+[window_fft_welch_specs]
+window_fftgram: hann
 [density_estimation]
 ; Final frequency resolution of CSD and PSD 
 frequency_resolution: 0.03125
 ; Coarse graining : 0 - pwelch PSD estimate - 1 - corase-grain PSD estimate
-N_average_segments_welch_psd: 2
-coarse_grain: 0
+N_average_segments_psd: 2
+coarse_grain_psd: False
+coarse_grain_csd: True
+overlap_factor_welch: 0.5
 overlap_factor: 0.5
-zeropad_csd: True
 [postprocessing]
 polarization: tensor 
 ; Power law index
 alpha: 0
 ; Reference frequency in Hz
 fref: 25
 ; Lower frequency boudn used for analysis in Hz
```

### Comparing `pygwb-1.0.0/pygwb_pipe/pygwb_dag` & `pygwb-1.3.0/pygwb_pipe/pygwb_dag`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/pygwb_pipe/pygwb_html` & `pygwb-1.3.0/pygwb_pipe/pygwb_html`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #!/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) California Institute of Technology 2023
 #
 # This file is part of pygwb.
 
-import logging, argparse, os
+import argparse
+import logging
+import os
+
 from pygwb.html import pygwb_html
 
 __process_name__ = 'pygwb_html'
 __version__ = '0.0.1'
 
 def main(args=None):
     logging.basicConfig()
@@ -21,15 +24,17 @@
                         help='increase verbose output')
     parser.add_argument('-V', '--version', action='version',
                         version=__version__)
     parser.add_argument('-o', '--output-dir', type=os.path.abspath,
                         help='Directory for all output')
     parser.add_argument('-p', '--plot-dir', type=os.path.abspath,
                         help='Directory of plots to show')
+    parser.add_argument('--plot-segment-results', action='store_true',
+                        help='Create result pages for every segment')
     args = parser.parse_args(args=args)
 
     # call the above function
-    pygwb_html(outdir=args.output_dir)
+    pygwb_html(outdir=args.output_dir, segment_results=args.plot_segment_results)
 
 # allow be be run on the command line
 if __name__ == "__main__":
     main(args=None)
```

### Comparing `pygwb-1.0.0/pygwb_pipe/pygwb_pe` & `pygwb-1.3.0/pygwb_pipe/pygwb_pe`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,60 @@
 #!/bin/env python
 
 import argparse
 import json
+from fractions import Fraction
 
-import numpy as np
 import bilby
 import h5py
-
-from fractions import Fraction
+import numpy as np
 
 import pygwb.pe as pe
 from pygwb.baseline import Baseline
 from pygwb.detector import Interferometer
 
+def load_npz(fname_path):
+    data = np.load(fname_path)
+    ptEst_ff = np.real(data["point_estimate_spectrum"])
+    sigma_ff = data["sigma_spectrum"]
+    goodInds = np.logical_and(np.invert(np.isnan(ptEst_ff)), ptEst_ff!=0, sigma_ff!=0)
+    if "frequencies" not in data.keys():
+        freqs = None
+    else:
+        freqs = data["frequencies"]
+        freqs = freqs[goodInds]
+    Y_f = ptEst_ff[goodInds]
+    sigma_f = sigma_ff[goodInds]
+    return (freqs,Y_f,sigma_f)
+
 def load_hdf5(fname_path):
     hf = h5py.File(fname_path, "r")
     point_estimate_spectrum = np.array(hf.get("point_estimate_spectrum"))
     sigma_spectrum = np.array(hf.get("sigma_spectrum"))
     if "freqs" not in hf.keys():
         freqs = None
     else:
         freqs = np.array(hf.get("freqs"))
         
     return (freqs, point_estimate_spectrum, sigma_spectrum)
 
+def load_npz(fname_path):
+    data = np.load(fname_path)
+    ptEst_ff = np.real(data["point_estimate_spectrum"])
+    sigma_ff = data["sigma_spectrum"]
+    goodInds = np.logical_and(np.invert(np.isnan(ptEst_ff)), ptEst_ff!=0, sigma_ff!=0)
+    if "frequencies" not in data.keys():
+        freqs = None
+    else:
+        freqs = data["frequencies"]
+        freqs = freqs[goodInds]
+    Y_f = ptEst_ff[goodInds]
+    sigma_f = sigma_ff[goodInds]
+    return (freqs,Y_f,sigma_f)
+
 def main():
     pe_parser = argparse.ArgumentParser(add_help=True)
     pe_parser.add_argument(
         "--path_to_file", help="Path to data file (or pickled baseline) to use for analysis.", action="store", type=str, required=True
     )
     pe_parser.add_argument(
         "--ifos", help="List of names of two interferometers for which you want to run PE, default is H1 and L1. Not needed when running from a pickled baseline.", action="store", type=str, required=False, default = "None"
@@ -191,21 +218,7 @@
     #print(quantiles)
 
     hlv.plot_corner(show_titles=True, title_fmt='.3g', use_math_text=True, quantiles=quantiles, range=range_list)
     
 
 if __name__ == "__main__":
     main()
-
-def load_npz(fname_path):
-    data = np.load(fname_path)
-    ptEst_ff = np.real(data["point_estimate_spectrum"])
-    sigma_ff = data["sigma_spectrum"]
-    goodInds = np.logical_and(np.invert(np.isnan(ptEst_ff)), ptEst_ff!=0, sigma_ff!=0)
-    if "frequencies" not in data.keys():
-        freqs = None
-    else:
-        freqs = data["frequencies"]
-        freqs = freqs[goodInds]
-    Y_f = ptEst_ff[goodInds]
-    sigma_f = sigma_ff[goodInds]
-    return (freqs,Y_f,sigma_f)
```

### Comparing `pygwb-1.0.0/pygwb_pipe/pygwb_pipe` & `pygwb-1.3.0/pygwb_pipe/pygwb_pipe`

 * *Files 21% similar despite different names*

```diff
@@ -22,38 +22,44 @@
     ann = getattr(Parameters, "__annotations__", {})
     parser = argparse.ArgumentParser(parents=[parent])
     for name, dtype in ann.items():
         name_help = ParametersHelp[name].help
         if dtype == List:
             parser.add_argument(f"--{name}", help=name_help, type=str, nargs='+', required=False)
         else:
-            parser.add_argument(f"--{name}", help=name_help, type=dtype, required=False)
+            parser.add_argument(f"--{name}", help=name_help, type=str, required=False)
     return parser
 
 def main():
     params = Parameters()
     pipe_parser = argparse.ArgumentParser(add_help=False)
     pipe_parser.add_argument(
         "--param_file", help="Parameter file to use for analysis.", action="store", type=str, required=False
     )
     pipe_parser.add_argument(
         "--output_path", help="Location to save output to.", action="store", type=str, required=False
     )
     pipe_parser.add_argument(
+        "--calc_coh", help="Calculate coherence spectrum from data.", action="store", type=str, required=False
+    )
+    pipe_parser.add_argument(
         "--calc_pt_est", help="Calculate omega point estimate and sigma from data.", action="store", type=str, required=False
     )
     pipe_parser.add_argument(
         "--apply_dsc", help="Apply delta sigma cut when calculating final output.", action="store", type=str, required=False
     )
     pipe_parser.add_argument(
         "--pickle_out", help="Pickle output Baseline of the analysis.", action="store", type=str, required=False
     )
     pipe_parser.add_argument(
         "--wipe_ifo", help="Wipe interferometer data to reduce size of pickled Baseline.", action="store", type=str, required=False
     )
+    pipe_parser.add_argument(
+        "--file_tag", help="File naming tag. By default, reads in first and last time in dataset.", action="store", type=str, required=False
+    )
 
     help_args = help_arguments(pipe_parser)
     help_args.parse_known_args()  # for help
 
     script_args, parameters_args = pipe_parser.parse_known_args()
 
     if script_args.param_file:
@@ -64,20 +70,18 @@
     if script_args.output_path:
         output_path = Path(script_args.output_path)
         if not output_path.exists():
             output_path.mkdir(parents=True)
     else: 
         output_path = Path('')
 
-    if script_args.param_file:
-        outfile_path = f"{output_path}/{Path(script_args.param_file).stem}_final{Path(script_args.param_file).suffix}"
+    if script_args.calc_coh:
+        pipe_calculate_coherence = bool(distutils.util.strtobool(script_args.calc_coh))
     else:
-        outfile_path = Path(f"{output_path}/parameters_final.ini")
-    params.save_paramfile(str(outfile_path))
-    logger.info(f"Saved final param file at {outfile_path}.")
+        pipe_calculate_coherence = False
 
     if script_args.calc_pt_est:
         pipe_calculate_point_estimate = bool(distutils.util.strtobool(script_args.calc_pt_est))
     else:
         pipe_calculate_point_estimate = True
     
     if script_args.apply_dsc:
@@ -91,32 +95,60 @@
         pipe_pickle_baseline = True
 
     if script_args.wipe_ifo:
         wipe_ifo = bool(distutils.util.strtobool(script_args.wipe_ifo))
     else:
         wipe_ifo = True
 
+    if not script_args.file_tag:
+        script_args.file_tag = f"{int(params.t0)}-{int(params.tf)}"
+
+    if script_args.param_file:
+        outfile_path = f"{output_path}/{Path(script_args.param_file).stem}_{script_args.file_tag}_final{Path(script_args.param_file).suffix}"
+    else:
+        outfile_path = Path(f"{output_path}/parameters_{script_args.file_tag}_final.ini")
+    params.save_paramfile(str(outfile_path))
+    logger.info(f"Saved final param file at {outfile_path}.")
+
     param_dict = params.parse_ifo_parameters()
     ifo_list = params.interferometer_list
     ifo_1 = Interferometer.from_parameters(ifo_list[0], param_dict[ifo_list[0]])
     ifo_2 = Interferometer.from_parameters(ifo_list[1], param_dict[ifo_list[1]])
     logger.info(f"Loaded up interferometers with selected parameters.")
 
     if params.gate_data:
-        logger.info(f"Applying gates.")
-        for ifo, ifo_obj in zip(ifo_list, [ifo_1, ifo_1]):
-            gate_params = { 
-                    "gate_tzero":param_dict[ifo].gate_tzero,
-                    "gate_tpad":param_dict[ifo].gate_tpad,
-                    "gate_threshold":param_dict[ifo].gate_threshold,
-                    "cluster_window":param_dict[ifo].cluster_window,
-                    "gate_whiten":param_dict[ifo].gate_whiten,
-                    }
-            ifo_obj.gate_data_apply(**gate_params)
-            logger.info(f"Gates for IFO {ifo}:{ifo_obj.gates}")
+        if params.path_gate_data:
+            logger.info("Loading gates from file.")
+            params.path_gate_data = Path(params.path_gate_data)
+            if not params.path_gate_data.is_file():
+                list_of_gatefiles = sorted(params.path_gate_data.glob("point_estimate*.npz"))
+                npzobject_list = [path for path in list_of_gatefiles if path.match(f"*{int(params.t0)}-{int(params.tf)}*")]
+                npzobject = np.load(params.path_gate_data / npzobject_list[0])
+            else:
+                npzobject = np.load(params.path_gate_data)
+            for index, ifo_obj in enumerate([ifo_1, ifo_2]):
+                ifo_obj.apply_gates_from_file(
+                    npzobject,
+                    index + 1,
+                    gate_tpad=param_dict[ifo_list[index]].gate_tpad,
+                )
+                logger.info(f"Gates loaded and applied for IFO {ifo_list[index]}:{ifo_obj.gates}")
+
+        else:
+            logger.info(f"Applying autogating procedure.")
+            for ifo, ifo_obj in zip(ifo_list, [ifo_1, ifo_2]):
+                gate_params = { 
+                        "gate_tzero":param_dict[ifo].gate_tzero,
+                        "gate_tpad":param_dict[ifo].gate_tpad,
+                        "gate_threshold":param_dict[ifo].gate_threshold,
+                        "cluster_window":param_dict[ifo].cluster_window,
+                        "gate_whiten":param_dict[ifo].gate_whiten,
+                        }
+                ifo_obj.gate_data_apply(**gate_params)
+                logger.info(f"Gates for IFO {ifo}:{ifo_obj.gates}")
 
     base_12 = Baseline.from_parameters(ifo_1, ifo_2, params)
     logger.info(
         f"Baseline with interferometers {ifo_1.name}, {ifo_2.name} initialised."
     )
 
     logger.info(f"Setting PSDs and CSDs of the baseline...")
@@ -142,55 +174,60 @@
         return_naive_and_averaged_sigmas = True
     )
 
     logger.info(
         f"times flagged by the delta sigma cut as badGPStimes:{base_12.badGPStimes}"
     )
 
+    if pipe_calculate_coherence:
+        logger.info(f"calculating the coherence...")
+
+        base_12.set_coherence_spectrum(apply_dsc=pipe_apply_dsc)
+
     if pipe_calculate_point_estimate:
         logger.info(f"calculating the point estimate and sigma...")
 
         base_12.set_point_estimate_sigma(
             alpha=params.alpha,
             fref=params.fref,
             flow=params.flow,
             fhigh=params.fhigh,
             apply_dsc=pipe_apply_dsc
         )
 
         logger.success(
-            f"Ran stochastic search over times {int(params.t0)}-{int(params.tf)}"
+            f"Ran stochastic search over times {script_args.file_tag}"
         )
         logger.success(f"\tPOINT ESTIMATE: {base_12.point_estimate:e}")
         logger.success(f"\tSIGMA: {base_12.sigma:e}")
 
-        data_file_name = f"{output_path}/point_estimate_sigma_{int(params.t0)}-{int(params.tf)}"
+        data_file_name = f"{output_path}/point_estimate_sigma_{script_args.file_tag}"
 
         logger.info(
             "Saving point_estimate and sigma spectrograms, spectra, and final values to file."
         )
         logger.info("Saving average psds and csd to file.")
         base_12.save_point_estimate_spectra(
             params.save_data_type,
             data_file_name,
         )
-        csd_file_name = f"{output_path}/csds_psds_{int(params.t0)}-{int(params.tf)}"
+        csd_file_name = f"{output_path}/psds_csds_{script_args.file_tag}"
         base_12.save_psds_csds(
             params.save_data_type,
             csd_file_name,
         )
         if pipe_pickle_baseline:
             logger.info("Pickling the baseline.")
-            pickle_name = f"{output_path}/{base_12.name}_{int(params.t0)}-{int(params.tf)}.pickle"
+            pickle_name = f"{output_path}/{base_12.name}_{script_args.file_tag}.pickle"
             base_12.save_to_pickle(pickle_name, wipe=wipe_ifo)
 
     else:
         logger.info("Saving average psds and csd to file.")
 
-        data_file_name = f"psds_csds_{int(params.t0)}-{int(params.tf)}"
+        data_file_name = f"{output_path}/psds_csds_{script_args.file_tag}"
 
         base_12.npz_save_psds_csds(
             data_file_name,
             base_12.frequencies,
             base_12.csd,
             base_12.interferometer_1.average_psd,
             base_12.interferometer_2.average_psd,
```

### Comparing `pygwb-1.0.0/pygwb_pipe/workflow_config.ini` & `pygwb-1.3.0/pygwb_pipe/workflow_config.ini`

 * *Files identical despite different names*

### Comparing `pygwb-1.0.0/setup.py` & `pygwb-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     package_dir={"pygwb": "pygwb"},
     scripts=['pygwb_pipe/pygwb_pipe','pygwb_pipe/pygwb_combine', 'pygwb_pipe/pygwb_stats', 'pygwb_pipe/pygwb_dag', 'pygwb_pipe/pygwb_pe', 'pygwb_pipe/pygwb_create_isotropic_workflow', 'pygwb_pipe/pygwb_html'],
     install_requires=[
         "numpy",
         "matplotlib",
         "scipy>=1.8.0",
         "bilby>=1.4",
-        "gwpy>=3.0.1",
-        "astropy>=5.2",
+        "gwpy>=3.0.4",
+        "astropy==5.2",
         "gwdetchar",
         "gwsumm",
         "pycondor",
         "lalsuite>=7.3",
         "loguru",
         "json5",
         "seaborn",
```

