# Comparing `tmp/pygwb-0.2.tar.gz` & `tmp/pygwb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygwb-0.2.tar", last modified: Sat Feb 25 02:48:04 2023, max compression
+gzip compressed data, was "pygwb-1.0.0.tar", last modified: Fri Mar 31 01:58:16 2023, max compression
```

## Comparing `pygwb-0.2.tar` & `pygwb-1.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-02-25 02:48:04.786654 pygwb-0.2/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)       81 2022-04-20 22:31:55.000000 pygwb-0.2/.coveragerc
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      350 2022-10-10 02:44:00.000000 pygwb-0.2/.gitignore
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3762 2023-01-27 02:26:35.000000 pygwb-0.2/.gitlab-ci.yml
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      933 2022-04-20 22:31:55.000000 pygwb-0.2/.pre-commit-config.yaml
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10301 2022-03-16 19:09:33.000000 pygwb-0.2/CONTRIBUTING.md
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1069 2022-03-16 19:09:33.000000 pygwb-0.2/LICENSE
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)       86 2022-10-10 06:22:25.000000 pygwb-0.2/MANIFEST.in
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2639 2023-02-25 02:48:04.787654 pygwb-0.2/PKG-INFO
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1901 2023-02-07 22:31:38.000000 pygwb-0.2/README.md
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     7259 2022-03-16 19:09:33.000000 pygwb-0.2/checkpoint.pkl
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-02-25 02:48:04.739653 pygwb-0.2/docs/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      606 2022-03-16 19:09:33.000000 pygwb-0.2/docs/Makefile
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-02-25 02:48:04.765653 pygwb-0.2/pygwb/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      107 2022-10-10 02:11:55.000000 pygwb-0.2/pygwb/__init__.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      155 2023-02-25 02:48:03.000000 pygwb-0.2/pygwb/_version.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    63485 2023-02-25 02:16:03.000000 pygwb-0.2/pygwb/baseline.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      296 2023-02-25 00:33:10.000000 pygwb-0.2/pygwb/constants.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     6823 2023-02-25 02:20:10.000000 pygwb-0.2/pygwb/delta_sigma_cut.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    15812 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb/detector.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3756 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb/html.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    14640 2023-02-01 19:24:44.000000 pygwb-0.2/pygwb/network.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10219 2022-08-15 17:05:36.000000 pygwb-0.2/pygwb/notch.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10081 2022-08-15 17:05:36.000000 pygwb-0.2/pygwb/omega_spectra.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     6837 2022-03-16 19:09:33.000000 pygwb-0.2/pygwb/orfs.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    18284 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb/parameters.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    23209 2022-08-15 17:05:36.000000 pygwb-0.2/pygwb/pe.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    12497 2023-02-25 02:19:19.000000 pygwb-0.2/pygwb/postprocessing.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    17291 2023-02-25 00:26:42.000000 pygwb-0.2/pygwb/preprocessing.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    23067 2023-02-06 00:08:53.000000 pygwb-0.2/pygwb/simulator.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    19508 2023-02-09 22:52:21.000000 pygwb-0.2/pygwb/spectral.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    45536 2023-01-27 22:25:50.000000 pygwb-0.2/pygwb/statistical_checks.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     6622 2023-02-09 22:50:50.000000 pygwb-0.2/pygwb/util.py
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     8134 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb/workflow.py
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-02-25 02:48:04.772654 pygwb-0.2/pygwb.egg-info/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2639 2023-02-25 02:48:03.000000 pygwb-0.2/pygwb.egg-info/PKG-INFO
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      974 2023-02-25 02:48:04.000000 pygwb-0.2/pygwb.egg-info/SOURCES.txt
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        1 2023-02-25 02:48:03.000000 pygwb-0.2/pygwb.egg-info/dependency_links.txt
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      141 2023-02-25 02:48:03.000000 pygwb-0.2/pygwb.egg-info/requires.txt
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        6 2023-02-25 02:48:03.000000 pygwb-0.2/pygwb.egg-info/top_level.txt
-drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-02-25 02:48:04.785654 pygwb-0.2/pygwb_pipe/
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      544 2022-09-30 15:53:13.000000 pygwb-0.2/pygwb_pipe/README.md
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2343 2023-02-25 01:02:42.000000 pygwb-0.2/pygwb_pipe/parameters.ini
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2287 2022-07-08 17:09:27.000000 pygwb-0.2/pygwb_pipe/parameters_mock.ini
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     9249 2023-01-30 22:17:29.000000 pygwb-0.2/pygwb_pipe/pygwb_combine
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     8036 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb_pipe/pygwb_create_isotropic_workflow
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     6562 2023-01-27 22:25:50.000000 pygwb-0.2/pygwb_pipe/pygwb_dag
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1172 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb_pipe/pygwb_html
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     9131 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb_pipe/pygwb_pe
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     7257 2023-02-25 02:18:29.000000 pygwb-0.2/pygwb_pipe/pygwb_pipe
--rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1388 2023-01-27 22:25:50.000000 pygwb-0.2/pygwb_pipe/pygwb_stats
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1368 2023-02-21 22:11:58.000000 pygwb-0.2/pygwb_pipe/workflow_config.ini
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      212 2022-10-10 04:12:40.000000 pygwb-0.2/pyproject.toml
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      465 2023-02-25 02:48:04.788654 pygwb-0.2/setup.cfg
--rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1910 2023-02-21 22:13:58.000000 pygwb-0.2/setup.py
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.492250 pygwb-1.0.0/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)       81 2022-04-20 22:31:55.000000 pygwb-1.0.0/.coveragerc
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      350 2022-10-10 02:44:00.000000 pygwb-1.0.0/.gitignore
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3887 2023-03-04 00:43:41.000000 pygwb-1.0.0/.gitlab-ci.yml
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      933 2022-04-20 22:31:55.000000 pygwb-1.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10301 2022-03-16 19:09:33.000000 pygwb-1.0.0/CONTRIBUTING.md
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1069 2022-03-16 19:09:33.000000 pygwb-1.0.0/LICENSE
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)       86 2022-10-10 06:22:25.000000 pygwb-1.0.0/MANIFEST.in
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3964 2023-03-31 01:58:16.493250 pygwb-1.0.0/PKG-INFO
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3224 2023-03-31 01:54:46.000000 pygwb-1.0.0/README.md
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     7259 2022-03-16 19:09:33.000000 pygwb-1.0.0/checkpoint.pkl
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.455250 pygwb-1.0.0/docs/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      606 2022-03-16 19:09:33.000000 pygwb-1.0.0/docs/Makefile
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.477250 pygwb-1.0.0/pygwb/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      107 2022-10-10 02:11:55.000000 pygwb-1.0.0/pygwb/__init__.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      160 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb/_version.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    64009 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/baseline.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      296 2023-02-28 18:40:50.000000 pygwb-1.0.0/pygwb/constants.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     7009 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/delta_sigma_cut.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    16072 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/detector.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3637 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/html.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    14627 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/network.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10219 2022-08-15 17:05:36.000000 pygwb-1.0.0/pygwb/notch.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    10081 2022-08-15 17:05:36.000000 pygwb-1.0.0/pygwb/omega_spectra.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     6837 2022-03-16 19:09:33.000000 pygwb-1.0.0/pygwb/orfs.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    18154 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/parameters.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    23187 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/pe.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    13678 2023-03-29 18:34:28.000000 pygwb-1.0.0/pygwb/postprocessing.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    17279 2023-03-09 21:39:38.000000 pygwb-1.0.0/pygwb/preprocessing.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    22915 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/simulator.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    19581 2023-03-29 18:34:29.000000 pygwb-1.0.0/pygwb/spectral.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)    45345 2023-02-28 18:42:00.000000 pygwb-1.0.0/pygwb/statistical_checks.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     9934 2023-03-29 18:34:29.000000 pygwb-1.0.0/pygwb/util.py
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     8134 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb/workflow.py
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.481250 pygwb-1.0.0/pygwb.egg-info/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     3964 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/PKG-INFO
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      974 2023-03-31 01:58:16.000000 pygwb-1.0.0/pygwb.egg-info/SOURCES.txt
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        1 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/dependency_links.txt
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      127 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/requires.txt
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)        6 2023-03-31 01:58:15.000000 pygwb-1.0.0/pygwb.egg-info/top_level.txt
+drwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)        0 2023-03-31 01:58:16.492250 pygwb-1.0.0/pygwb_pipe/
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      544 2022-09-30 15:53:13.000000 pygwb-1.0.0/pygwb_pipe/README.md
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2343 2023-02-25 01:02:42.000000 pygwb-1.0.0/pygwb_pipe/parameters.ini
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     2287 2022-07-08 17:09:27.000000 pygwb-1.0.0/pygwb_pipe/parameters_mock.ini
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     9249 2023-01-30 22:17:29.000000 pygwb-1.0.0/pygwb_pipe/pygwb_combine
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     8036 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb_pipe/pygwb_create_isotropic_workflow
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     6600 2023-03-29 18:34:29.000000 pygwb-1.0.0/pygwb_pipe/pygwb_dag
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1172 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb_pipe/pygwb_html
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     9814 2023-03-04 00:43:41.000000 pygwb-1.0.0/pygwb_pipe/pygwb_pe
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     7257 2023-02-25 02:18:29.000000 pygwb-1.0.0/pygwb_pipe/pygwb_pipe
+-rwxrwxr-x   0 arianna.renzini (45773) arianna.renzini (45773)     1388 2023-01-27 22:25:50.000000 pygwb-1.0.0/pygwb_pipe/pygwb_stats
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1368 2023-02-21 22:11:58.000000 pygwb-1.0.0/pygwb_pipe/workflow_config.ini
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      212 2022-10-10 04:12:40.000000 pygwb-1.0.0/pyproject.toml
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)      465 2023-03-31 01:58:16.494250 pygwb-1.0.0/setup.cfg
+-rw-rw-r--   0 arianna.renzini (45773) arianna.renzini (45773)     1885 2023-02-28 18:42:00.000000 pygwb-1.0.0/setup.py
```

### Comparing `pygwb-0.2/.gitlab-ci.yml` & `pygwb-1.0.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     - python -c "import pygwb.pe"
     - python -c "import pygwb.postprocessing"
     - python -c "import pygwb.preprocessing"
     - python -c "import pygwb.simulator"
     - python -c "import pygwb.spectral"
     - python -c "import pygwb.statistical_checks"
     - python -c "import pygwb.util"
+    - for script in $(pip show -f pygwb | grep "bin\/" | xargs -I {} basename {}); do
+          ${script} --help;
+      done
 
 basic-3.8:
   <<: *basic-python
   image: python:3.8
 
 basic-3.9:
   <<: *basic-python
```

### Comparing `pygwb-0.2/.pre-commit-config.yaml` & `pygwb-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/CONTRIBUTING.md` & `pygwb-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/LICENSE` & `pygwb-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/checkpoint.pkl` & `pygwb-1.0.0/checkpoint.pkl`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/docs/Makefile` & `pygwb-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb/baseline.py` & `pygwb-1.0.0/pygwb/baseline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import json
 import pickle
 import warnings
 
 import h5py
 import numpy as np
 from loguru import logger
@@ -14,15 +13,15 @@
 from .notch import StochNotchList
 from .orfs import calc_orf
 from .postprocessing import (
     calc_Y_sigma_from_Yf_sigmaf,
     calculate_point_estimate_sigma_spectra,
     postprocess_Y_sigma,
 )
-from .spectral import coarse_grain_spectrogram, cross_spectral_density
+from .spectral import cross_spectral_density
 
 
 class Baseline(object):
     """
     Baseline object for stochastic analyses.
     """
 
@@ -128,15 +127,15 @@
         else:
             raise ValueError(
                 "Overlap reduction function to be used has not yet been set. To set it, set the orf_polarization property."
             )
 
     @property
     def orf_polarization(self):
-        """"""
+        """Overlap reduction function polarization"""
         if self._orf_polarization_set:
             return self._orf_polarization
         else:
             raise ValueError(
                 "Overlap reduction function polarization han not yet been set."
             )
 
@@ -255,14 +254,22 @@
             self._duration_set = True
         else:
             warnings.warn("Neither baseline nor interferometer duration is set.")
             self._duration = dur
             self._duration_set = True
 
     @property
+    def csd_segment_offset(self):
+        if self._duration_set:
+            stride = self.duration * (1 - self.overlap_factor)
+            return int(np.ceil(self.duration / stride)) * int(self.N_average_segments_welch_psd/2)
+        else:
+            raise ValueError("Trying to calculate CSD segment offset before setting duration. Need to set duration before attempting this.")
+
+    @property
     def frequencies(self):
         """Frequency array associated to this baseline."""
         if self._frequencies_set:
             return self._frequencies
         else:
             raise ValueError("frequencies have not yet been set.")
 
@@ -682,25 +689,27 @@
         frequency_resolution: float
             The frequency resolution at which the cross and power spectral densities are calculated.
         """
         try:
             self.interferometer_1.set_psd_spectrogram(
                 frequency_resolution,
                 overlap_factor=self.overlap_factor,
-                window_fftgram_dict=self.window_fftgram_dict,
+                window_fftgram_dict_welch_psd={"window_fftgram": "hann"},
+                overlap_factor_welch_psd=0.5,
             )
         except AttributeError:
             raise AssertionError(
                 "Interferometer {self.interferometer_1.name} has no timeseries data! Need to set timeseries data in the interferometer first."
             )
         try:
             self.interferometer_2.set_psd_spectrogram(
                 frequency_resolution,
                 overlap_factor=self.overlap_factor,
-                window_fftgram_dict=self.window_fftgram_dict,
+                window_fftgram_dict_welch_psd={"window_fftgram": "hann"},
+                overlap_factor_welch_psd=0.5,
             )
         except AttributeError:
             raise AssertionError(
                 "Interferometer {self.interferometer_2.name} has no timeseries data! Need to set timeseries data in the interferometer first."
             )
         self.csd = cross_spectral_density(
             self.interferometer_1.timeseries,
@@ -731,19 +740,17 @@
         # TODO: make this less fragile.
         # For now, recalculate ORF in case frequencies have changed.
         # self._tensor_orf_calculated = False
         # self.frequencies = self.csd.frequencies.value
 
     def set_average_cross_spectral_density(self):
         """If csd has been calculated, sets the average csd for the baseline"""
-        stride = self.duration * (1 - self.overlap_factor)
-        csd_segment_offset = int(np.ceil(self.duration / stride))
         try:
             self.average_csd = self.csd[
-                csd_segment_offset : -(csd_segment_offset + 1) + 1
+                self.csd_segment_offset : -(self.csd_segment_offset + 1) + 1
             ]
         except AttributeError:
             print(
                 "CSD has not been calculated yet! Need to set_cross_and_power_spectral_density first."
             )
         # TODO: make this less fragile.
         # For now, recalculate ORF in case frequencies have changed.
@@ -833,18 +840,17 @@
             freqs=self.frequencies,
             csd=self.average_csd,
             avg_psd_1=self.interferometer_1.average_psd,
             avg_psd_2=self.interferometer_2.average_psd,
             orf=self.overlap_reduction_function,
             sample_rate=self.sampling_frequency,
             segment_duration=self.duration,
-            window_fftgram_dict={"window_fftgram": "hann"},
             fref=fref,
             alpha=alpha,
-        )
+        ) #missing: pwelch estimation parameters
 
         sigma_name = f"{self.name} sigma spectrogram alpha={alpha}"
         self.point_estimate_spectrogram = OmegaSpectrogram(
             Y_fs,
             times=self.average_csd.times,
             frequencies=self.average_csd.frequencies,
             name=self.name + f" with alpha={alpha}",
@@ -899,14 +905,19 @@
         apply_dsc: bool, optional
             Apply delta sigma cut flag; if True, removes the badGPStimes from the spectra calculations.
             Default is True.
         apply_notches: bool, optional
             Apply spectral notches flag; if True, remove the notches specified in the notch_list from the spectra calculations.
             Default is True.
         """
+        if self.overlap_factor>0.0:
+            do_overlap = True
+        else:
+            do_overlap = False
+
         if apply_dsc == True:
             if not hasattr(self, "badGPStimes"):
                 warnings.warn(
                     "Delta sigma cut has not been calculated yet, hence no delta sigma cut will be applied... If this is a mistake, please run `calculate_delta_sigma_cut` first, then re-calculate point estimate/sigma spectra."
                 )
             if badtimes is None:
                 if hasattr(self, "badGPStimes"):
@@ -964,15 +975,17 @@
             self.point_estimate_spectrogram.value,
             self.sigma_spectrogram.value ** 2,
             self.duration,
             deltaF,
             self.sampling_frequency,
             frequency_mask=self.frequency_mask,
             badtimes_mask=bad_times_indexes,
-        )
+            do_overlap=do_overlap,
+            N_avg_segs=self.N_average_segments_welch_psd,
+        )#missing: pwelch estimation parameters
 
         self.point_estimate_spectrum = OmegaSpectrum(
             point_estimate,
             frequencies=self.frequencies,
             name=self.name + " point estimate spectrum",
             epoch=epoch,
             alpha=alpha,
@@ -1087,15 +1100,14 @@
         delta_sigma_cut,
         alphas,
         fref,
         flow=20,
         fhigh=1726,
         notch_list_path="",
         polarization="tensor",
-        window_fftgram_dict: dict = {"window_fftgram": "hann"},
         return_naive_and_averaged_sigmas: bool = False,
     ):
         """
         Calculate the delta sigma cut using the naive and average psds, if set in the baseline.
 
         Parameters
         ==========
@@ -1120,27 +1132,25 @@
             Dictionary with window characteristics. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
         """
         if not self._orf_polarization_set:
             self.orf_polarization = polarization
 
         deltaF = self.frequencies[1] - self.frequencies[0]
         self.crop_frequencies_average_psd_csd(flow=flow, fhigh=fhigh)
-        stride = self.duration * (1 - self.overlap_factor)
-        csd_segment_offset = int(np.ceil(self.duration / stride))
 
         naive_psd_1 = self.interferometer_1.psd_spectrogram[
-            csd_segment_offset:-csd_segment_offset
+            self.csd_segment_offset:-self.csd_segment_offset
         ]
         naive_psd_2 = self.interferometer_2.psd_spectrogram[
-            csd_segment_offset:-csd_segment_offset
+            self.csd_segment_offset:-self.csd_segment_offset
         ]
 
         naive_psd_1_cropped = naive_psd_1.crop_frequencies(flow, fhigh + deltaF)
         naive_psd_2_cropped = naive_psd_2.crop_frequencies(flow, fhigh + deltaF)
-
+        
         if notch_list_path:
             self.notch_list_path = notch_list_path
         if self.notch_list_path:
             logger.debug(
                 "loading notches for delta sigma cut from " + self.notch_list_path
             )
             self.set_frequency_mask(self.notch_list_path)
@@ -1155,17 +1165,18 @@
             psd1_slide=self.interferometer_1.average_psd,
             psd2_slide=self.interferometer_2.average_psd,
             alphas=alphas,
             sample_rate=self.sampling_frequency,
             orf=self.overlap_reduction_function,
             fref=fref,
             frequency_mask=self.frequency_mask,
-            window_fftgram_dict=window_fftgram_dict,
+            N_average_segments_welch_psd = self.N_average_segments_welch_psd,
             return_naive_and_averaged_sigmas=return_naive_and_averaged_sigmas,
-        )
+        )#missing: pwelch estimation parameters
+
         self.badGPStimes = badGPStimes
         self.delta_sigmas = delta_sigmas
 
     def save_point_estimate_spectra(
         self,
         save_data_type,
         filename,
```

### Comparing `pygwb-0.2/pygwb/delta_sigma_cut.py` & `pygwb-1.0.0/pygwb/delta_sigma_cut.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 from loguru import logger
 
-from pygwb.notch import StochNotch, StochNotchList
 from pygwb.postprocessing import calculate_point_estimate_sigma_spectra
 from pygwb.util import calc_bias
 
 
 def dsc_cut(
     naive_sigma: np.ndarray,
     slide_sigma: np.ndarray,
@@ -58,14 +57,16 @@
     psd2_slide: np.ndarray,
     alphas: np.ndarray,
     sample_rate: int,
     orf: np.array,
     fref: int,
     frequency_mask: np.array = True,
     window_fftgram_dict: dict = {"window_fftgram": "hann"},
+    overlap_factor: float=0.5,
+    N_average_segments_welch_psd = 2,
     return_naive_and_averaged_sigmas: bool = False,
 ):
 
     """
     Function that runs the delta sigma cut
 
     Parameters
@@ -112,30 +113,32 @@
     """
 
     logger.info("Running delta sigma cut")
     nalphas = len(alphas)
     times = np.array(psd1_naive.times)
     ntimes = len(times)
     df = psd1_naive.df.value
-    dt = 1 / sample_rate  # psd1_naive.df.value ** (-1)
+    dt = 1 / sample_rate  
     # Naive estimate
     bf_ns = calc_bias(
         segmentDuration=segment_duration,
         deltaF=df,
         deltaT=dt,
         N_avg_segs=1,
         window_fftgram_dict=window_fftgram_dict,
+        overlap_factor=overlap_factor
     )
     # Sliding estimate
     bf_ss = calc_bias(
         segmentDuration=segment_duration,
         deltaF=df,
         deltaT=dt,
-        N_avg_segs=2,
+        N_avg_segs=N_average_segments_welch_psd,
         window_fftgram_dict=window_fftgram_dict,
+        overlap_factor=overlap_factor
     )
     freqs = np.array(psd1_naive.frequencies)
     overall_cut = np.zeros((ntimes, 1), dtype="bool")
     cuts = np.zeros((nalphas, ntimes), dtype="bool")
     naive_sigmas = np.zeros((nalphas, ntimes))
     slide_sigmas = np.zeros((nalphas, ntimes))
     dsigmas = np.zeros((nalphas, ntimes))
@@ -152,27 +155,29 @@
             naive_sigma_with_Hf = calculate_point_estimate_sigma_spectra(
                 freqs=freqs,
                 avg_psd_1=psd1_naive_time,
                 avg_psd_2=psd2_naive_time,
                 orf=orf,
                 sample_rate=sample_rate,
                 window_fftgram_dict=window_fftgram_dict,
+                overlap_factor=overlap_factor,
                 segment_duration=segment_duration,
                 csd=None,
                 fref=fref,
                 alpha=alpha,
             )
 
             slide_sigma_with_Hf = calculate_point_estimate_sigma_spectra(
                 freqs=freqs,
                 avg_psd_1=psd1_slide_time,
                 avg_psd_2=psd2_slide_time,
                 orf=orf,
                 sample_rate=sample_rate,
                 window_fftgram_dict=window_fftgram_dict,
+                overlap_factor=overlap_factor,
                 segment_duration=segment_duration,
                 csd=None,
                 fref=fref,
                 alpha=alpha,
             )
 
             naive_sensitivity_integrand_with_Hf = 1.0 / naive_sigma_with_Hf
```

### Comparing `pygwb-0.2/pygwb/detector.py` & `pygwb-1.0.0/pygwb/detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import os
 
 import bilby.gw.detector
-import numpy as np
-from bilby.gw.detector.psd import PowerSpectralDensity
+from bilby.gw.detector import PowerSpectralDensity
 from gwpy.segments import SegmentList
 
 from .preprocessing import (
     preprocessing_data_channel_name,
     preprocessing_data_gwpy_timeseries,
     preprocessing_data_timeseries_array,
     self_gate_data,
@@ -101,15 +100,19 @@
             with open(filename, "r") as parameter_file:
                 lines = parameter_file.readlines()
                 for line in lines:
                     if line[0] == "#" or line[0] == "\n":
                         continue
                     split_line = line.split("=")
                     key = split_line[0].strip()
-                    value = eval("=".join(split_line[1:]))
+                    value = eval(
+                        "=".join(split_line[1:]),
+                        dict(__builtins__=dict()),
+                        dict(PowerSpectralDensity=PowerSpectralDensity),
+                    )
                     parameters[key] = value
             if "shape" not in parameters.keys():
                 logging.debug("Assuming L shape for name")
             elif parameters["shape"].lower() in ["l", "ligo"]:
                 parameters.pop("shape")
             elif parameters["shape"].lower() in ["triangular", "triangle"]:
                 raise ValueError("Triangular detectros are not implemented yet.")
@@ -288,41 +291,42 @@
         self._check_timeseries_sample_rate(new_sample_rate)
         self.sampling_frequency = new_sample_rate
 
     def set_psd_spectrogram(
         self,
         frequency_resolution,
         overlap_factor=0.5,
-        overlap_factor_welch_psd=0,
-        window_fftgram_dict={"window_fftgram": "hann"},
+        window_fftgram_dict_welch_psd={"window_fftgram": "hann"},
+        overlap_factor_welch_psd=0.5,
     ):
         """
         Set psd_spectrogram attribute from a given spectrum-related information.
 
         Parameters
         ==========
         frequency_resolution: float
             Frequency resolution of the final PSDs; This sets the time duration
             over which FFTs are calculated in the pwelch method
         overlap_factor: float, optional
             Amount of overlap between adjacent segments (range between 0 and 1)
             This factor should be same as the one used for cross_spectral_density
             (default 0, no overlap)
-        window_fftgram_dict: dictionary, optional
-            Dictionary containing name and parameters describing which window to use when producing fftgrams for psds and csds. Default is \"hann\".
+        window_fftgram_dict_welch_psd: dictionary, optional
+            Dictionary containing name and parameters describing which window to use when producing fftgrams for welch psd estimation. Default is \"hann\".
 
         """
 
         # psd_array = spectral.psd(self.timeseries, frequencies)
         self.psd_spectrogram = power_spectral_density(
             self.timeseries,
             self.duration,
             frequency_resolution,
             overlap_factor=overlap_factor,
-            window_fftgram_dict=window_fftgram_dict,
+            window_fftgram_dict_welch_psd=window_fftgram_dict_welch_psd,
+            overlap_factor_welch_psd=overlap_factor_welch_psd,
         )
         self.psd_spectrogram.channel = self.timeseries.channel
         self._check_spectrogram_channel_name(self.timeseries.channel.name)
         self._check_spectrogram_frequency_resolution(frequency_resolution)
 
     def set_average_psd(self, N_average_segments_welch_psd=2):
         """
```

### Comparing `pygwb-0.2/pygwb/html.py` & `pygwb-1.0.0/pygwb/html.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) California Institute of Technology 2023
 #
 # This file is part of pygwb.
 
 import argparse
 import glob
-import json
 import logging
 import os
-import sys
-import time
 
 import gwsumm
 import gwsumm.plot
 import gwsumm.tabs
-import matplotlib.pyplot as plt
-import numpy
 from gwpy.time import from_gps
-from gwpy.timeseries import TimeSeries
 
 """Create pygwb html
 """
 
 def pygwb_html(outdir='./', config=None):
 
     # =====================
```

### Comparing `pygwb-0.2/pygwb/network.py` & `pygwb-1.0.0/pygwb/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import warnings
 
-import bilby
 import gwpy
 import numpy as np
 from loguru import logger
 
 from .baseline import Baseline
 from .notch import StochNotchList
 from .omega_spectra import OmegaSpectrum
```

### Comparing `pygwb-0.2/pygwb/notch.py` & `pygwb-1.0.0/pygwb/notch.py`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb/omega_spectra.py` & `pygwb-1.0.0/pygwb/omega_spectra.py`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb/orfs.py` & `pygwb-1.0.0/pygwb/orfs.py`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb/parameters.py` & `pygwb-1.0.0/pygwb/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import argparse
+import configparser
 import enum
-import json
 import re
-import sys
 import warnings
 from dataclasses import asdict, dataclass, field
-from pathlib import Path
 from typing import List
 
 import json5
 
-if sys.version_info >= (3, 0):
-    import configparser
-else:
-    import ConfigParser as configparser
-
 
 @dataclass
 class Parameters:
     """
     Parameters class: a dataclass which contains all parameters required for initialising a pygwb Interferometer, a pygwb Baseline, and run pygwb_pipe.
 
     Attributes
```

### Comparing `pygwb-0.2/pygwb/pe.py` & `pygwb-1.0.0/pygwb/pe.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,18 +515,16 @@
             self._parameters = parameters
         else:
             raise ValueError(f"unexpected type for parameters {type(parameters)}")
 
     def model_function(self, bline):
         model = np.zeros(bline.frequencies.shape)
         for pol in self.polarizations:
-            orf_pol = eval(f"bline.{pol}_overlap_reduction_function")
-            orf_parent = eval(
-                f"bline.{self.polarizations[0]}_overlap_reduction_function"
-            )
+            orf_pol = getattr(bline, f"{pol}_overlap_reduction_function")
+            orf_parent = getattr(bline, f"{self.polarizations[0]}_overlap_reduction_function")
             model += (
                 orf_pol
                 / orf_parent
                 * self.parameters[f"omega_ref_{pol}"]
                 * (bline.frequencies / self.fref) ** (self.parameters[f"alpha_{pol}"])
             )
         return model
```

### Comparing `pygwb-0.2/pygwb/postprocessing.py` & `pygwb-1.0.0/pygwb/postprocessing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import pickle
-
-import h5py
 import numpy as np
 import scipy.ndimage as ndi
 from loguru import logger
-from tqdm import tqdm
 
 from pygwb.constants import H0
 from pygwb.omega_spectra import OmegaSpectrum
 
 from .util import _check_omegaspectra, calc_bias, window_factors
 
 
@@ -16,15 +12,18 @@
     Y_fs,
     var_fs,
     segment_duration,
     deltaF,
     new_sample_rate,
     frequency_mask=True,
     badtimes_mask=None,
+    do_overlap=True,
     window_fftgram_dict={"window_fftgram": "hann"},
+    overlap_factor=0.5,
+    N_avg_segs=2,
 ):
     """Run postprocessing of point estimate and sigma spectrograms, combining even and
     odd segments in the case of overlapping data. For more details see - https://dcc.ligo.org/public/0027/T040089/000/T040089-00.pdf
 
     Parameters:
     -----------
     Y_fs : array-like
@@ -34,16 +33,23 @@
     segment_duration : float
         Duration of each time segment
     deltaF : float
         Frequency resolution
     new_sample_rate : float
         sample rate of timeseries after resampling
     frequency_mask: array-like, optional
-        Boolean mask to apply to frequencies for the calculation
-    window_fftgram_dict : dictionary containing window information
+        Boolean mask to apply to frequencies for the calculation. Defaults to True which includes all frequencies in the analysis.
+    badtimes_mask: array-like, optional
+        Boolean mask to apply to GPStimes in the calculation. Defaults to None such that all times are included.
+    do_overlap: bool, optional
+        Indicates whether to proceed with the odd/even postprocessing calculation which assumes a 50\% overlap between consecutive segments. Default is True.
+    window_fftgram_dict: dictionary, optional
+        Dictionary with window characteristics used in PSD estimation. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
+    overlap_factor: float, optional
+        Overlap factor used in PSD estimation. Default is 0.5.
 
     Returns:
     --------
     Y_f_new : array-like
         1D point estimate spectrum
     sigma_f_few : array-like
         1D sigma spectrum
@@ -57,25 +63,27 @@
     Y_fs_sliced = []
     var_fs_sliced = []
 
     for sli in ndi.find_objects(labels):
         Y = Y_fs[sli]
         var = var_fs[sli]
 
-        if len(Y) == 1:
+        if len(Y) == 1 or not do_overlap:
             Y_fs_sliced.append(Y[0])
             var_fs_sliced.append(var[0])
         else:
             Y_red, var_red = odd_even_segment_postprocessing(
                 Y,
                 var,
                 segment_duration,
                 new_sample_rate,
                 frequency_mask=frequency_mask,
                 window_fftgram_dict=window_fftgram_dict,
+                overlap_factor=overlap_factor,
+                N_avg_segs=N_avg_segs,
             )
             Y_fs_sliced.append(Y_red)
             var_fs_sliced.append(var_red)
 
     Y_fs_sliced = np.array(Y_fs_sliced)
     var_fs_sliced = np.array(var_fs_sliced)
 
@@ -83,30 +91,33 @@
         Y_fs_sliced, np.sqrt(var_fs_sliced)
     )
 
     bias = calc_bias(
         segment_duration,
         deltaF,
         1 / new_sample_rate,
-        N_avg_segs=2,
+        N_avg_segs=N_avg_segs,
         window_fftgram_dict=window_fftgram_dict,
+        overlap_factor=overlap_factor,
     )
     logger.debug(f"Bias factor: {bias}")
     sigma_f_new *= bias
 
     return Y_f_new, sigma_f_new
 
 
 def odd_even_segment_postprocessing(
     Y_fs,
     var_fs,
     segment_duration,
     new_sample_rate,
     frequency_mask=True,
     window_fftgram_dict={"window_fftgram": "hann"},
+    overlap_factor=0.5,
+    N_avg_segs=2,
 ):
     """Perform averaging which combines even and odd segments for overlapping data. 
 
     Parameters:
     -----------
     Y_fs : array-like
         2D array of point estimates with Ntimes x Nfreqs with overlapping segments
@@ -114,25 +125,27 @@
         2D array of variances or 2D with dimensions Ntimes x Nfreqs with overlapping time segments
     segment_duration : float
         Duration of each time segment
     new_sample_rate : float
         sample rate of timeseries after resampling
     frequency_mask: array-like, optional
         Boolean mask to apply to frequencies for the calculation
-    window_fftgram_dict : dictionary containing window information
+    window_fftgram_dict: dictionary, optional
+        Dictionary with window characteristics used in PSD estimation. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
+    overlap_factor: float, optional
 
     Returns:
     --------
     Y_f_new : array-like
         1D point estimate spectrum
     var_f_few : array-like
         1D sigma spectrum
     """
     _, w1w2squaredbar, _, w1w2squaredovlbar = window_factors(
-        int(segment_duration * new_sample_rate), window_fftgram_dict
+        int(segment_duration * new_sample_rate), window_fftgram_dict, overlap_factor=overlap_factor
     )
     k = w1w2squaredovlbar / w1w2squaredbar
 
     size = np.size(Y_fs, axis=0)
     # even/odd indices
     evens = np.arange(0, size, 2)
     odds = np.arange(1, size, 2)
@@ -259,14 +272,15 @@
     csd,
     avg_psd_1,
     avg_psd_2,
     orf,
     sample_rate,
     segment_duration,
     window_fftgram_dict={"window_fftgram": "hann"},
+    overlap_factor=0.5,
     fref=25.0,
     alpha=0.0,
 ):
     """
     Calculate the Omega point estimate and associated sigma integrand,
     given a set of cross-spectral and power-spectral density spectrograms.
     This is particularly useful for statistical checks.
@@ -286,15 +300,17 @@
     orf: array_like
         Overlap reduction function.
     sample_rate: float
         Sampling rate of the data.
     segment_duration: float
         Duration of each segment in seconds.
     window_fftgram_dict: dictionary, optional
-        Dictionary with window characteristics. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
+        Dictionary with window characteristics used in PSD estimation. Default is `(window_fftgram_dict={"window_fftgram": "hann"}`
+    overlap_factor: float, optional
+        Overlap factor used in PSD estimation. Default is 0.5.
     fref: float, optional
         Reference frequency to use in the weighting calculation.
         Final result refers to this frequency.
     alpha: float, optional
         Spectral index to use in the weighting.
     """
     S_alpha = 3 * H0.si.value ** 2 / (10 * np.pi ** 2) / freqs ** 3
@@ -304,15 +320,15 @@
         / (2 * segment_duration * (freqs[1] - freqs[0]))
         * avg_psd_1
         * avg_psd_2
         / (orf ** 2 * S_alpha ** 2)
     )
 
     w1w2bar, w1w2squaredbar, _, _ = window_factors(
-        int(sample_rate * segment_duration), window_fftgram_dict=window_fftgram_dict
+        int(sample_rate * segment_duration), window_fftgram_dict=window_fftgram_dict, overlap_factor=overlap_factor
     )
     var_fs = var_fs * w1w2squaredbar / w1w2bar ** 2
     if csd is not None:
         Y_fs = (csd) / (orf * S_alpha)
         return Y_fs, var_fs
     else:
         return var_fs
```

### Comparing `pygwb-0.2/pygwb/preprocessing.py` & `pygwb-1.0.0/pygwb/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import os
 import warnings
 
 import lal
 import numpy as np
 import scipy
-from gwpy import signal, timeseries
+from gwpy import timeseries
 
 
 def set_start_time(
     job_start_GPS: int,
     job_end_GPS: int,
     buffer_secs: int,
     segment_duration: int,
@@ -215,15 +215,15 @@
     Returns
     =======
     filtered: gwpy_timeseries
         Timeseries containing the filtered and high passed data
     """
     if (new_sample_rate * number_cropped_seconds) < 18:
         warnings.warn(
-            f"Number of cropped seconds requested {number_cropped_seconds}s is low compared to the sampling rate {new_sampling_rate}: cropped-seconds x sampling-rate = {number_cropped_seconds*new_sampling_rate}."
+            f"Number of cropped seconds requested {number_cropped_seconds}s is low compared to the sampling rate {new_sample_rate}: cropped-seconds x sampling-rate = {number_cropped_seconds*new_sample_rate}."
         )
     data_to_resample = copy.deepcopy(time_series_data.value)
     original_times = copy.deepcopy(time_series_data.times)
     nan_mask = np.isnan(time_series_data.value)  # .flatten()
 
     if np.sum(nan_mask) != 0:
         data_nansafe = data_to_resample[~nan_mask]
```

### Comparing `pygwb-0.2/pygwb/simulator.py` & `pygwb-1.0.0/pygwb/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,18 @@
-import argparse
-import os
-import sys
-
 import bilby
 import gwpy
-import h5py
 import numpy as np
 from bilby.core.utils import create_frequency_series
 from gwpy.timeseries import TimeSeries
 from loguru import logger
 from tqdm import tqdm
 
 from pygwb.baseline import Baseline, get_baselines
 from pygwb.util import interpolate_frequency_series
 
-if sys.version_info >= (3, 0):
-    import configparser
-else:
-    import ConfigParser as configparser
-
 
 class Simulator(object):
     def __init__(
         self,
         interferometers,
         N_segments,
         duration,
```

### Comparing `pygwb-0.2/pygwb/spectral.py` & `pygwb-1.0.0/pygwb/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,15 +477,16 @@
 
 
 def power_spectral_density(
     time_series_data:  TimeSeries,
     segment_duration:  TimeSeries,
     frequency_resolution: float,
     overlap_factor: float = 0.5,
-    window_fftgram_dict: dict = {"window_fftgram": "hann"},
+    window_fftgram_dict_welch_psd: dict = {"window_fftgram": "hann"},
+    overlap_factor_welch_psd: float = 0.5,
 ):
     """
     Compute the PSDs of every segment (defined by the segment duration)
     in the time series using pwelch method.
 
     Parameters
     ----------
@@ -515,17 +516,17 @@
     # Length of data blocks to be used in pwelch
     fftlength = int(1.0 / frequency_resolution)
 
     # No zero-pad is used in the PSD estimation
     fft_gram_data = fftgram(
         time_series_data,
         fftlength,
-        overlap_factor=overlap_factor,
+        overlap_factor=overlap_factor_welch_psd,
         zeropad=False,
-        window_fftgram_dict=window_fftgram_dict,
+        window_fftgram_dict=window_fftgram_dict_welch_psd,
     )
 
     # Use pwelch method (averaging) to get PSDs for each segment duration 
     # of data
     psd_spectrogram = pwelch_psd(
         2 * np.conj(fft_gram_data) * fft_gram_data,
         segment_duration,
```

### Comparing `pygwb-0.2/pygwb/statistical_checks.py` & `pygwb-1.0.0/pygwb/statistical_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import pickle
 from os import listdir
 from os.path import isfile, join
 from pathlib import Path
 
-import gwpy
-import h5py
 import matplotlib
 import matplotlib.pyplot as plt
 
 matplotlib.rcParams['figure.figsize'] = (8,6)
 matplotlib.rcParams['axes.grid'] = True
 matplotlib.rcParams['grid.linestyle'] = ':'
 matplotlib.rcParams['grid.color'] = 'grey'
@@ -21,24 +18,20 @@
 rc('text', usetex=True)
 
 import seaborn as sns
 
 sea = sns.color_palette("tab10")
 
 import numpy as np
-from scipy import integrate, special, stats
+from scipy import integrate, stats
 from scipy.optimize import curve_fit
 
 from pygwb.baseline import Baseline
 from pygwb.parameters import Parameters
-from pygwb.postprocessing import (
-    calc_Y_sigma_from_Yf_sigmaf,
-    calculate_point_estimate_sigma_spectra,
-)
-from pygwb.util import StatKS, calc_bias, interpolate_frequency_series
+from pygwb.util import StatKS, calc_bias
 
 
 class StatisticalChecks(object):
     def __init__(
         self,
         sliding_times_all,
         sliding_omega_all,
```

### Comparing `pygwb-0.2/pygwb/workflow.py` & `pygwb-1.0.0/pygwb/workflow.py`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb.egg-info/SOURCES.txt` & `pygwb-1.0.0/pygwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/README.md` & `pygwb-1.0.0/pygwb_pipe/README.md`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/parameters.ini` & `pygwb-1.0.0/pygwb_pipe/parameters.ini`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/parameters_mock.ini` & `pygwb-1.0.0/pygwb_pipe/parameters_mock.ini`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/pygwb_combine` & `pygwb-1.0.0/pygwb_pipe/pygwb_combine`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/pygwb_create_isotropic_workflow` & `pygwb-1.0.0/pygwb_pipe/pygwb_create_isotropic_workflow`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/pygwb_dag` & `pygwb-1.0.0/pygwb_pipe/pygwb_dag`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         dag_args.pickle_out = "True"
     if not dag_args.wipe_ifo:
         dag_args.wipe_ifo = "True"  
     if not dag_args.calc_pt_est:
         dag_args.calc_pt_est = "True"        
         
     # Filepaths
-    outputdir = dag_args.parentdir / "output"
-    logdir = outputdir / "condorLogs"
+    outputdir = (dag_args.parentdir / "output")
+    logdir = (outputdir / "condorLogs")
     
     # Make directories
     logdir.mkdir(parents=True, exist_ok=True)
     outputdir.mkdir(parents=True, exist_ok=True)
     
     dag = outputdir / dag_args.dag_name
     
@@ -137,17 +137,17 @@
     length_actual = length_list[t_index]
 
     with open(dag,"w") as dagfile:
 
         for index,t0 in enumerate(t0_actual): 
             dagfile.write(f"JOB {index} {os.path.abspath(dag_args.subfile)}\n")
 
-            args = (f"--t0 {t0} --tf {tf_actual[index]} --output_path {outputdir} --apply_dsc {dag_args.apply_dsc} --param_file {os.path.abspath(dag_args.param_file)}" 
+            args = (f"--t0 {t0} --tf {tf_actual[index]} --output_path {os.path.abspath(outputdir)} --apply_dsc {dag_args.apply_dsc} --param_file {os.path.abspath(dag_args.param_file)}" 
                     f" --pickle_out {dag_args.pickle_out} --wipe_ifo {dag_args.wipe_ifo} --calc_pt_est {dag_args.calc_pt_est}")
             dagfile.write(
-                    f'VARS {index} job="{t0}-{tf_actual[index]}" executable="{executable}" ARGS="{args}" logdir="{logdir}"\n'
+                    f'VARS {index} job="{t0}-{tf_actual[index]}" executable="{executable}" ARGS="{args}" logdir="{os.path.abspath(logdir)}"\n'
             )
             dagfile.write('\n')
         
 if __name__ == "__main__":
     main()
```

### Comparing `pygwb-0.2/pygwb_pipe/pygwb_html` & `pygwb-1.0.0/pygwb_pipe/pygwb_html`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/pygwb_pe` & `pygwb-1.0.0/pygwb_pipe/pygwb_pe`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 #!/bin/env python
 
 import argparse
 import json
-import sys
 
 import numpy as np
 import bilby
+import h5py
 
 from fractions import Fraction
 
 import pygwb.pe as pe
 from pygwb.baseline import Baseline
 from pygwb.detector import Interferometer
 
+def load_hdf5(fname_path):
+    hf = h5py.File(fname_path, "r")
+    point_estimate_spectrum = np.array(hf.get("point_estimate_spectrum"))
+    sigma_spectrum = np.array(hf.get("sigma_spectrum"))
+    if "freqs" not in hf.keys():
+        freqs = None
+    else:
+        freqs = np.array(hf.get("freqs"))
+        
+    return (freqs, point_estimate_spectrum, sigma_spectrum)
 
 def main():
     pe_parser = argparse.ArgumentParser(add_help=True)
     pe_parser.add_argument(
         "--path_to_file", help="Path to data file (or pickled baseline) to use for analysis.", action="store", type=str, required=True
     )
     pe_parser.add_argument(
@@ -37,21 +47,21 @@
     pe_parser.add_argument(
         "--injection_parameters", help="The injected parameters.", required= False, default="None", type=str, action="store"
     )
     pe_parser.add_argument(
         "--quantiles", help="The quantiles used for plotting in plot corner, default is [0.05, 0.95].", type=str, action="store", required=False, default="None"
     )
     pe_parser.add_argument(
-        "--f0", help="If no frequencies are saved in the loaded npz file, you can give f0, fhigh and df to the script. This is f0", type=float, action="store", default=None
+        "--f0", help="If no frequencies are saved in the loaded npz file, you can give f0, fhigh and df to the script. This is f0, the begin frequency.", type=float, action="store", default=None
     )
     pe_parser.add_argument(
-        "--fhigh", help="If no frequencies are saved in the loaded npz file, you can give f0, fhigh and df to the script. This is fhigh", type=float, action="store", default=None
+        "--fhigh", help="If no frequencies are saved in the loaded npz file, you can give f0, fhigh and df to the script. This is fhigh, the end frequency.", type=float, action="store", default=None
     )
     pe_parser.add_argument(
-        "--df", help="If no frequencies are saved in the loaded npz file, you can give f0, fhigh and df to the script. This is df", type=float, action="store", default=None
+        "--df", help="If no frequencies are saved in the loaded npz file, you can give f0, fhigh and df to the script. This is df, the frequency spacing.", type=float, action="store", default=None
     )
     pe_parser.add_argument(
         "--calibration_epsilon", help="Calibration uncertainty. 0 by default.", type=float, action="store", default=None, required=False,
     )
     
     script_args = pe_parser.parse_known_args()[0]
     
@@ -69,15 +79,15 @@
                              "Smooth-Broken-Power-Law": ["omega_ref", "fbreak", "alpha_1", "alpha_2", "delta"],
                              "Schumann": ["kappa_H1", "kappa_L1", "beta_L1", "beta_H1"],
                              "Parity-Violation": ["omega_ref", "alpha", "Pi"],
                              "Parity-Violation-2": ["omega_ref", "alpha", "beta"]}
     
     if script_args.model not in dictionary_models.keys():
         raise ValueError(
-            "The model you provided is not supported."
+            "The model {script_args.model} you provided is not supported."
         )
     else:
         class_model = dictionary_models[script_args.model]
         
     if script_args.model_prior_file == 'None': 
         dict_loaded = {"omega_ref":bilby.core.prior.LogUniform(1e-11,1e-8,"$\\Omega_{ref}$"),"alpha":bilby.core.prior.Uniform(-4, 4,'$\\alpha$')}
     else:
@@ -98,17 +108,22 @@
             )
       
     if not all(key in all_parameters_dict.keys() for key in dictionary_parameters[script_args.model]):
         raise ValueError(
             f"Not all required parameters of the model are present in one of the parameters dictionaries. \n These are the required parameters: {dictionary_parameters[script_args.model]}."
         )
     
-    if script_args.path_to_file.endswith(("npz")):
-        
-        frequencies, point_estimate_spectrum, sigma_spectrum = load_npz(script_args.path_to_file)
+
+    if script_args.path_to_file.endswith(("npz")) or script_args.path_to_file.endswith((".h5")):
+    
+        if script_args.path_to_file.endswith(("npz")):
+            frequencies, point_estimate_spectrum, sigma_spectrum = load_npz(script_args.path_to_file)
+        else:
+            frequencies, point_estimate_spectrum, sigma_spectrum = load_hdf5(script_args.path_to_file)
+
         
         if frequencies is None:
             frequencies = np.arange(script_args.f0, script_args.fhigh + script_args.df, script_args.df)
         
         point_estimates = [point_estimate_spectrum]
         sigmas = [sigma_spectrum]
         
@@ -135,15 +150,15 @@
     
     elif script_args.path_to_file.endswith((".p", ".pickle")):
         
         base_12 = Baseline.load_from_pickle(script_args.path_to_file)
     
     else:
         raise TypeError(
-            "The provided file format is currently not supported, try a npz file or a pickled baseline instead."
+            "The provided file format is currently not supported, try an npz, hdf5 file or a pickled baseline instead."
         )
     
     
     kwargs = {"baselines":[base_12], "model_name":script_args.model} #, "fref":script_args.fref}
     kwargs.update(extra_kwargs)
     model = class_model(**kwargs)
     priors = dict_loaded
@@ -169,15 +184,15 @@
     outdir=script_args.output_dir,label= 'hlv', injection_parameters = injection_parameters) #walks=10, maxmcmc = 10000, npoints= 1000
 
     if script_args.quantiles == "None":
         quantiles = [0.05, 0.95]
     else:
         quantiles = json.loads(script_args.quantiles)
         
-    print(quantiles)
+    #print(quantiles)
 
     hlv.plot_corner(show_titles=True, title_fmt='.3g', use_math_text=True, quantiles=quantiles, range=range_list)
     
 
 if __name__ == "__main__":
     main()
```

### Comparing `pygwb-0.2/pygwb_pipe/pygwb_pipe` & `pygwb-1.0.0/pygwb_pipe/pygwb_pipe`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/pygwb_stats` & `pygwb-1.0.0/pygwb_pipe/pygwb_stats`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/pygwb_pipe/workflow_config.ini` & `pygwb-1.0.0/pygwb_pipe/workflow_config.ini`

 * *Files identical despite different names*

### Comparing `pygwb-0.2/setup.py` & `pygwb-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,24 @@
     license="MIT",
     packages=["pygwb"],
     package_dir={"pygwb": "pygwb"},
     scripts=['pygwb_pipe/pygwb_pipe','pygwb_pipe/pygwb_combine', 'pygwb_pipe/pygwb_stats', 'pygwb_pipe/pygwb_dag', 'pygwb_pipe/pygwb_pe', 'pygwb_pipe/pygwb_create_isotropic_workflow', 'pygwb_pipe/pygwb_html'],
     install_requires=[
         "numpy",
         "matplotlib",
-        "scipy==1.8.0",
+        "scipy>=1.8.0",
         "bilby>=1.4",
-        "gwpy==3.0.1",
+        "gwpy>=3.0.1",
         "astropy>=5.2",
         "gwdetchar",
         "gwsumm",
         "pycondor",
-        "lalsuite==7.3",
+        "lalsuite>=7.3",
         "loguru",
         "json5",
-        "jinja2==3.0.3",
         "seaborn",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
```

