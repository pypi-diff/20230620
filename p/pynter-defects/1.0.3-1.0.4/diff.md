# Comparing `tmp/pynter-defects-1.0.3.tar.gz` & `tmp/pynter-defects-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynter-defects-1.0.3.tar", last modified: Tue Jun 20 12:17:07 2023, max compression
+gzip compressed data, was "pynter-defects-1.0.4.tar", last modified: Tue Jun 20 12:27:21 2023, max compression
```

## Comparing `pynter-defects-1.0.3.tar` & `pynter-defects-1.0.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.862180 pynter-defects-1.0.3/
--rw-rw-r--   0 villa     (1123) villa     (1123)      181 2023-06-20 12:17:07.826181 pynter-defects-1.0.3/PKG-INFO
--rwxrwxr-x   0 villa     (1123) villa     (1123)      731 2023-06-16 16:30:53.000000 pynter-defects-1.0.3/README.md
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:06.538209 pynter-defects-1.0.3/pynter/
--rw-rw-r--   0 villa     (1123) villa     (1123)     3699 2023-06-20 11:44:15.000000 pynter-defects-1.0.3/pynter/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:06.654206 pynter-defects-1.0.3/pynter/automations/
--rw-rw-r--   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.3/pynter/automations/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6625 2023-05-30 14:13:48.000000 pynter-defects-1.0.3/pynter/automations/core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    20887 2023-05-30 14:17:51.000000 pynter-defects-1.0.3/pynter/automations/vasp.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:06.902201 pynter-defects-1.0.3/pynter/cli/
--rw-rw-r--   0 villa     (1123) villa     (1123)     3416 2023-06-07 14:47:05.000000 pynter-defects-1.0.3/pynter/cli/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3410 2023-05-31 09:10:02.000000 pynter-defects-1.0.3/pynter/cli/automations.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6964 2023-06-16 17:17:43.000000 pynter-defects-1.0.3/pynter/cli/config.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    17275 2023-06-07 14:47:05.000000 pynter-defects-1.0.3/pynter/cli/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     5338 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/cli/hpc.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6375 2023-06-07 14:47:05.000000 pynter-defects-1.0.3/pynter/cli/inputs.py
--rwxrwxr--   0 villa     (1123) villa     (1123)     2039 2023-06-16 17:20:40.000000 pynter-defects-1.0.3/pynter/cli/main.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1732 2023-06-07 14:47:05.000000 pynter-defects-1.0.3/pynter/cli/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     4045 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/cli/phase_diagram.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     7896 2023-05-31 09:33:54.000000 pynter-defects-1.0.3/pynter/cli/plotter.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3782 2023-06-02 14:17:35.000000 pynter-defects-1.0.3/pynter/cli/slurm.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1452 2023-06-05 09:25:02.000000 pynter-defects-1.0.3/pynter/cli/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:06.966199 pynter-defects-1.0.3/pynter/data/
--rw-rw-r--   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.3/pynter/data/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.010199 pynter-defects-1.0.3/pynter/data/database/
--rw-rw-r--   0 villa     (1123) villa     (1123)        3 2020-11-13 14:36:46.000000 pynter-defects-1.0.3/pynter/data/database/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     2162 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/data/database/creator.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     5696 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/data/database/query.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    29512 2023-06-07 14:47:05.000000 pynter-defects-1.0.3/pynter/data/datasets.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    11750 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/data/jobs.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.250193 pynter-defects-1.0.3/pynter/defects/
--rw-rw-r--   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.3/pynter/defects/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    45917 2023-06-02 12:11:11.000000 pynter-defects-1.0.3/pynter/defects/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    10821 2023-05-03 16:47:07.000000 pynter-defects-1.0.3/pynter/defects/corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    35277 2023-05-23 12:43:01.000000 pynter-defects-1.0.3/pynter/defects/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6471 2023-05-23 12:43:01.000000 pynter-defects-1.0.3/pynter/defects/elasticity.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    11914 2023-05-31 16:46:23.000000 pynter-defects-1.0.3/pynter/defects/entries.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    15353 2023-05-23 12:43:01.000000 pynter-defects-1.0.3/pynter/defects/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.386191 pynter-defects-1.0.3/pynter/defects/pmg/
--rwxrwxr-x   0 villa     (1123) villa     (1123)    24611 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/defects/pmg/pmg_defects_core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    39163 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/defects/pmg/pmg_defects_corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    60074 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/defects/pmg/pmg_defects_utils.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    39933 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/defects/pmg/pmg_dos.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    12053 2023-05-23 12:43:01.000000 pynter-defects-1.0.3/pynter/defects/structure.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    19876 2023-05-23 12:43:02.000000 pynter-defects-1.0.3/pynter/defects/thermodynamics.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      994 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/defects/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.430189 pynter-defects-1.0.3/pynter/phase_diagram/
--rw-rw-r--   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.3/pynter/phase_diagram/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    32436 2023-05-23 12:43:02.000000 pynter-defects-1.0.3/pynter/phase_diagram/chempots.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     7430 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/phase_diagram/plotter.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    10388 2023-06-15 16:23:42.000000 pynter-defects-1.0.3/pynter/phase_diagram/thermodynamics.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.470189 pynter-defects-1.0.3/pynter/slurm/
--rw-rw-r--   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.3/pynter/slurm/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     9004 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/slurm/interface.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    10376 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/slurm/job_script.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1486 2023-05-23 12:43:02.000000 pynter-defects-1.0.3/pynter/slurm/job_status.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.610186 pynter-defects-1.0.3/pynter/testing/
--rw-rw-r--   0 villa     (1123) villa     (1123)     2363 2023-06-15 16:23:42.000000 pynter-defects-1.0.3/pynter/testing/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     5798 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/testing/core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     2574 2023-06-15 16:23:43.000000 pynter-defects-1.0.3/pynter/testing/data.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1285 2023-06-15 16:23:43.000000 pynter-defects-1.0.3/pynter/testing/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1493 2023-06-15 16:23:43.000000 pynter-defects-1.0.3/pynter/testing/phase_diagram.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      988 2023-06-15 16:23:43.000000 pynter-defects-1.0.3/pynter/testing/slurm.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      916 2023-06-15 16:23:43.000000 pynter-defects-1.0.3/pynter/testing/structure.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     4923 2023-06-15 16:23:43.000000 pynter-defects-1.0.3/pynter/testing/vasp.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.662185 pynter-defects-1.0.3/pynter/tools/
--rw-rw-r--   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.3/pynter/tools/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1038 2020-10-12 14:14:35.000000 pynter-defects-1.0.3/pynter/tools/format.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     7021 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/tools/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      251 2022-01-18 18:41:18.000000 pynter-defects-1.0.3/pynter/tools/plotter.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     9866 2023-05-23 12:43:02.000000 pynter-defects-1.0.3/pynter/tools/structure.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     8433 2023-05-31 15:51:51.000000 pynter-defects-1.0.3/pynter/tools/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.734183 pynter-defects-1.0.3/pynter/vasp/
--rw-rw-r--   0 villa     (1123) villa     (1123)        0 2023-06-20 11:37:46.000000 pynter-defects-1.0.3/pynter/vasp/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     9323 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/vasp/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    10172 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/vasp/default_inputs.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    36606 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/vasp/jobs.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6192 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/vasp/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.758182 pynter-defects-1.0.3/pynter/vasp/pmg/
--rw-rw-r--   0 villa     (1123) villa     (1123)   183623 2023-04-18 08:58:38.000000 pynter-defects-1.0.3/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    51327 2023-06-19 16:27:10.000000 pynter-defects-1.0.3/pynter/vasp/schemes.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-20 12:17:07.822181 pynter-defects-1.0.3/pynter_defects.egg-info/
--rw-rw-r--   0 villa     (1123) villa     (1123)      181 2023-06-20 12:17:04.000000 pynter-defects-1.0.3/pynter_defects.egg-info/PKG-INFO
--rw-rw-r--   0 villa     (1123) villa     (1123)     2016 2023-06-20 12:17:05.000000 pynter-defects-1.0.3/pynter_defects.egg-info/SOURCES.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)        1 2023-06-20 12:17:04.000000 pynter-defects-1.0.3/pynter_defects.egg-info/dependency_links.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       48 2023-06-20 12:17:04.000000 pynter-defects-1.0.3/pynter_defects.egg-info/entry_points.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       89 2023-06-20 12:17:04.000000 pynter-defects-1.0.3/pynter_defects.egg-info/requires.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       18 2023-06-20 12:17:04.000000 pynter-defects-1.0.3/pynter_defects.egg-info/top_level.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       38 2023-06-20 12:17:07.866180 pynter-defects-1.0.3/setup.cfg
--rw-rw-r--   0 villa     (1123) villa     (1123)      763 2023-06-20 11:14:09.000000 pynter-defects-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.694124 pynter-defects-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-20 12:27:21.694124 pynter-defects-1.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.686124 pynter-defects-1.0.4/pynter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.686124 pynter-defects-1.0.4/pynter/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/automations/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/automations/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.686124 pynter-defects-1.0.4/pynter/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/inputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/data/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/data/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/data/database/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/data/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29512 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/data/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45917 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/defects/pmg/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24611 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/pmg/pmg_defects_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/pmg/pmg_defects_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60074 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/pmg/pmg_defects_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39933 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/pmg/pmg_dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/phase_diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/phase_diagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32436 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/phase_diagram/chempots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/phase_diagram/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/phase_diagram/thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/slurm/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/slurm/job_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/slurm/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/testing/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.690124 pynter-defects-1.0.4/pynter/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/tools/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/tools/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/tools/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/tools/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.694124 pynter-defects-1.0.4/pynter/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/vasp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/vasp/default_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/vasp/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.694124 pynter-defects-1.0.4/pynter/vasp/pmg/
+-rw-r--r--   0 runner    (1001) docker     (123)   183623 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/pynter/vasp/schemes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:27:21.694124 pynter-defects-1.0.4/pynter_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-20 12:27:21.000000 pynter-defects-1.0.4/pynter_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-20 12:27:21.000000 pynter-defects-1.0.4/pynter_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:27:21.000000 pynter-defects-1.0.4/pynter_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 12:27:21.000000 pynter-defects-1.0.4/pynter_defects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 12:27:21.000000 pynter-defects-1.0.4/pynter_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 12:27:21.000000 pynter-defects-1.0.4/pynter_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:27:21.694124 pynter-defects-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-20 12:27:13.000000 pynter-defects-1.0.4/setup.py
```

### Comparing `pynter-defects-1.0.3/README.md` & `pynter-defects-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/__init__.py` & `pynter-defects-1.0.4/pynter/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/automations/core.py` & `pynter-defects-1.0.4/pynter/automations/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/automations/vasp.py` & `pynter-defects-1.0.4/pynter/automations/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/analysis.py` & `pynter-defects-1.0.4/pynter/cli/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/automations.py` & `pynter-defects-1.0.4/pynter/cli/automations.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/config.py` & `pynter-defects-1.0.4/pynter/cli/config.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/defects.py` & `pynter-defects-1.0.4/pynter/cli/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/hpc.py` & `pynter-defects-1.0.4/pynter/cli/hpc.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/inputs.py` & `pynter-defects-1.0.4/pynter/cli/inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/main.py` & `pynter-defects-1.0.4/pynter/cli/main.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/materials_project.py` & `pynter-defects-1.0.4/pynter/cli/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/phase_diagram.py` & `pynter-defects-1.0.4/pynter/cli/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/plotter.py` & `pynter-defects-1.0.4/pynter/cli/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/slurm.py` & `pynter-defects-1.0.4/pynter/cli/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/cli/utils.py` & `pynter-defects-1.0.4/pynter/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/data/database/creator.py` & `pynter-defects-1.0.4/pynter/data/database/creator.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/data/database/query.py` & `pynter-defects-1.0.4/pynter/data/database/query.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/data/datasets.py` & `pynter-defects-1.0.4/pynter/data/datasets.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/data/jobs.py` & `pynter-defects-1.0.4/pynter/data/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/analysis.py` & `pynter-defects-1.0.4/pynter/defects/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/corrections.py` & `pynter-defects-1.0.4/pynter/defects/corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/defects.py` & `pynter-defects-1.0.4/pynter/defects/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/elasticity.py` & `pynter-defects-1.0.4/pynter/defects/elasticity.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/entries.py` & `pynter-defects-1.0.4/pynter/defects/entries.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/plotter.py` & `pynter-defects-1.0.4/pynter/defects/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/pmg/pmg_defects_core.py` & `pynter-defects-1.0.4/pynter/defects/pmg/pmg_defects_core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/pmg/pmg_defects_corrections.py` & `pynter-defects-1.0.4/pynter/defects/pmg/pmg_defects_corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/pmg/pmg_defects_utils.py` & `pynter-defects-1.0.4/pynter/defects/pmg/pmg_defects_utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/pmg/pmg_dos.py` & `pynter-defects-1.0.4/pynter/defects/pmg/pmg_dos.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/structure.py` & `pynter-defects-1.0.4/pynter/defects/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/thermodynamics.py` & `pynter-defects-1.0.4/pynter/defects/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/defects/utils.py` & `pynter-defects-1.0.4/pynter/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/phase_diagram/chempots.py` & `pynter-defects-1.0.4/pynter/phase_diagram/chempots.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/phase_diagram/plotter.py` & `pynter-defects-1.0.4/pynter/phase_diagram/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/phase_diagram/thermodynamics.py` & `pynter-defects-1.0.4/pynter/phase_diagram/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/slurm/interface.py` & `pynter-defects-1.0.4/pynter/slurm/interface.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/slurm/job_script.py` & `pynter-defects-1.0.4/pynter/slurm/job_script.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/slurm/job_status.py` & `pynter-defects-1.0.4/pynter/slurm/job_status.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/__init__.py` & `pynter-defects-1.0.4/pynter/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/core.py` & `pynter-defects-1.0.4/pynter/testing/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/data.py` & `pynter-defects-1.0.4/pynter/testing/data.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/defects.py` & `pynter-defects-1.0.4/pynter/testing/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/phase_diagram.py` & `pynter-defects-1.0.4/pynter/testing/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/slurm.py` & `pynter-defects-1.0.4/pynter/testing/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/structure.py` & `pynter-defects-1.0.4/pynter/testing/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/testing/vasp.py` & `pynter-defects-1.0.4/pynter/testing/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/tools/format.py` & `pynter-defects-1.0.4/pynter/tools/format.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/tools/materials_project.py` & `pynter-defects-1.0.4/pynter/tools/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/tools/structure.py` & `pynter-defects-1.0.4/pynter/tools/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/tools/utils.py` & `pynter-defects-1.0.4/pynter/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/vasp/analysis.py` & `pynter-defects-1.0.4/pynter/vasp/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/vasp/default_inputs.py` & `pynter-defects-1.0.4/pynter/vasp/default_inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/vasp/jobs.py` & `pynter-defects-1.0.4/pynter/vasp/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/vasp/plotter.py` & `pynter-defects-1.0.4/pynter/vasp/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/vasp/pmg/pmg_electronic_structure_plotter.py` & `pynter-defects-1.0.4/pynter/vasp/pmg/pmg_electronic_structure_plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter/vasp/schemes.py` & `pynter-defects-1.0.4/pynter/vasp/schemes.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/pynter_defects.egg-info/SOURCES.txt` & `pynter-defects-1.0.4/pynter_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.3/setup.py` & `pynter-defects-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @author: villa
 """
 from setuptools import setup, find_namespace_packages
 
 
 setup(
     name='pynter-defects',
-    version='1.0.3',
+    version='1.0.4',
     author='Lorenzo Villa',
     description='Tools for atomistic calculations, provides features for point-defect calculations with VASP',
     packages=find_namespace_packages(exclude=["pynter.*.tests", "pynter.*.*.tests"]),
     install_requires=[
         'ase',
         'pymatgen>=2023.3.23',
         'pymatgen-analysis-defects>=2023.3.25',
```

