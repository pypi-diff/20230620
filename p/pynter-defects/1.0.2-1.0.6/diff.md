# Comparing `tmp/pynter-defects-1.0.2.tar.gz` & `tmp/pynter-defects-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynter-defects-1.0.2.tar", last modified: Mon Jun 19 09:32:07 2023, max compression
+gzip compressed data, was "pynter-defects-1.0.6.tar", last modified: Tue Jun 20 13:26:31 2023, max compression
```

## Comparing `pynter-defects-1.0.2.tar` & `pynter-defects-1.0.6.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.276624 pynter-defects-1.0.2/
--rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-19 09:32:07.276624 pynter-defects-1.0.2/PKG-INFO
--rwxrwxr-x   0 villa     (1123) villa     (1123)      731 2023-06-16 16:30:53.000000 pynter-defects-1.0.2/README.md
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.288646 pynter-defects-1.0.2/pynter/
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1793 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.316645 pynter-defects-1.0.2/pynter/automations/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/automations/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     6625 2023-05-30 14:13:48.000000 pynter-defects-1.0.2/pynter/automations/core.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    20887 2023-05-30 14:17:51.000000 pynter-defects-1.0.2/pynter/automations/vasp.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.496641 pynter-defects-1.0.2/pynter/cli/
--rw-rw-r--   0 villa     (1123) villa     (1123)     3416 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3410 2023-05-31 09:10:02.000000 pynter-defects-1.0.2/pynter/cli/automations.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6964 2023-06-16 17:17:43.000000 pynter-defects-1.0.2/pynter/cli/config.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    17275 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     5371 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/hpc.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6375 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/inputs.py
--rwxrwxr--   0 villa     (1123) villa     (1123)     2039 2023-06-16 17:20:40.000000 pynter-defects-1.0.2/pynter/cli/main.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1732 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     4062 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/cli/phase_diagram.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     7896 2023-05-31 09:33:54.000000 pynter-defects-1.0.2/pynter/cli/plotter.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     3782 2023-06-02 14:17:35.000000 pynter-defects-1.0.2/pynter/cli/slurm.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1452 2023-06-05 09:25:02.000000 pynter-defects-1.0.2/pynter/cli/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.524641 pynter-defects-1.0.2/pynter/data/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/data/__init__.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.580639 pynter-defects-1.0.2/pynter/data/database/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        3 2020-11-13 14:36:46.000000 pynter-defects-1.0.2/pynter/data/database/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     2179 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/data/database/creator.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     5713 2022-01-18 18:41:16.000000 pynter-defects-1.0.2/pynter/data/database/query.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    29512 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/data/datasets.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    11765 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/data/jobs.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.724636 pynter-defects-1.0.2/pynter/defects/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/defects/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    45917 2023-06-02 12:11:11.000000 pynter-defects-1.0.2/pynter/defects/analysis.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    10821 2023-05-03 16:47:07.000000 pynter-defects-1.0.2/pynter/defects/corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    35277 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6471 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/elasticity.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    11914 2023-05-31 16:46:23.000000 pynter-defects-1.0.2/pynter/defects/entries.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    15353 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.804635 pynter-defects-1.0.2/pynter/defects/pmg/
--rwxrwxr-x   0 villa     (1123) villa     (1123)    24611 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    39163 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_corrections.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    60074 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_utils.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    39933 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/pmg/pmg_dos.py
--rw-rw-r--   0 villa     (1123) villa     (1123)    12053 2023-05-23 12:43:01.000000 pynter-defects-1.0.2/pynter/defects/structure.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    19876 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/defects/thermodynamics.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)      994 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/defects/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.864633 pynter-defects-1.0.2/pynter/phase_diagram/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/phase_diagram/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    32436 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/phase_diagram/chempots.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     7430 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/phase_diagram/plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10388 2023-06-15 16:23:42.000000 pynter-defects-1.0.2/pynter/phase_diagram/thermodynamics.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:06.920632 pynter-defects-1.0.2/pynter/slurm/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/slurm/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9065 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/slurm/interface.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10416 2023-06-12 14:42:45.000000 pynter-defects-1.0.2/pynter/slurm/job_script.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1486 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/slurm/job_status.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.004630 pynter-defects-1.0.2/pynter/testing/
--rw-rw-r--   0 villa     (1123) villa     (1123)     2363 2023-06-15 16:23:42.000000 pynter-defects-1.0.2/pynter/testing/__init__.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     6067 2023-06-15 16:23:42.000000 pynter-defects-1.0.2/pynter/testing/core.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     2574 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/data.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1285 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/defects.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     1493 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/phase_diagram.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      988 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/slurm.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      916 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/structure.py
--rw-rw-r--   0 villa     (1123) villa     (1123)     4923 2023-06-15 16:23:43.000000 pynter-defects-1.0.2/pynter/testing/vasp.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.084628 pynter-defects-1.0.2/pynter/tools/
--rwxrwxr-x   0 villa     (1123) villa     (1123)        0 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/tools/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     1038 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/tools/format.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     7422 2023-06-02 12:18:36.000000 pynter-defects-1.0.2/pynter/tools/materials_project.py
--rw-rw-r--   0 villa     (1123) villa     (1123)      251 2022-01-18 18:41:18.000000 pynter-defects-1.0.2/pynter/tools/plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9866 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/tools/structure.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     8433 2023-05-31 15:51:51.000000 pynter-defects-1.0.2/pynter/tools/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.224625 pynter-defects-1.0.2/pynter/vasp/
--rwxrwxr-x   0 villa     (1123) villa     (1123)      872 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/vasp/__init__.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     9438 2022-01-18 18:41:18.000000 pynter-defects-1.0.2/pynter/vasp/analysis.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    10352 2023-05-23 12:43:02.000000 pynter-defects-1.0.2/pynter/vasp/default_inputs.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    36627 2023-06-07 14:47:05.000000 pynter-defects-1.0.2/pynter/vasp/jobs.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     6192 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/vasp/plotter.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.228625 pynter-defects-1.0.2/pynter/vasp/pmg/
--rw-rw-r--   0 villa     (1123) villa     (1123)   183623 2023-04-18 08:58:38.000000 pynter-defects-1.0.2/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)    51500 2023-06-05 12:14:41.000000 pynter-defects-1.0.2/pynter/vasp/schemes.py
--rwxrwxr-x   0 villa     (1123) villa     (1123)     3845 2020-10-12 14:14:35.000000 pynter-defects-1.0.2/pynter/vasp/utils.py
-drwxrwxr-x   0 villa     (1123) villa     (1123)        0 2023-06-19 09:32:07.272624 pynter-defects-1.0.2/pynter_defects.egg-info/
--rw-rw-r--   0 villa     (1123) villa     (1123)      122 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/PKG-INFO
--rw-rw-r--   0 villa     (1123) villa     (1123)     2037 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/SOURCES.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)        1 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/dependency_links.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       48 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/entry_points.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       89 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/requires.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       18 2023-06-19 09:32:05.000000 pynter-defects-1.0.2/pynter_defects.egg-info/top_level.txt
--rw-rw-r--   0 villa     (1123) villa     (1123)       38 2023-06-19 09:32:07.276624 pynter-defects-1.0.2/setup.cfg
--rw-rw-r--   0 villa     (1123) villa     (1123)      703 2023-06-19 09:17:15.000000 pynter-defects-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.348495 pynter-defects-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 13:26:31.348495 pynter-defects-1.0.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.328495 pynter-defects-1.0.6/pynter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.328495 pynter-defects-1.0.6/pynter/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/automations/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/automations/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.332495 pynter-defects-1.0.6/pynter/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/inputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/config_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.332495 pynter-defects-1.0.6/pynter/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.332495 pynter-defects-1.0.6/pynter/data/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/database/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29512 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.336495 pynter-defects-1.0.6/pynter/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45917 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.336495 pynter-defects-1.0.6/pynter/defects/pmg/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24611 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60074 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39933 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.336495 pynter-defects-1.0.6/pynter/phase_diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32436 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/chempots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.340495 pynter-defects-1.0.6/pynter/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/job_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.340495 pynter-defects-1.0.6/pynter/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/default_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter/vasp/pmg/
+-rw-r--r--   0 runner    (1001) docker     (123)   183623 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/vasp_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:26:31.348495 pynter-defects-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/setup.py
```

### Comparing `pynter-defects-1.0.2/README.md` & `pynter-defects-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/automations/core.py` & `pynter-defects-1.0.6/pynter/automations/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/automations/vasp.py` & `pynter-defects-1.0.6/pynter/automations/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/analysis.py` & `pynter-defects-1.0.6/pynter/cli/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/automations.py` & `pynter-defects-1.0.6/pynter/cli/automations.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/config.py` & `pynter-defects-1.0.6/pynter/cli/config.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/defects.py` & `pynter-defects-1.0.6/pynter/cli/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/hpc.py` & `pynter-defects-1.0.6/pynter/cli/hpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from datetime import datetime
 import subprocess
 import schedule
 from shutil import which
 
 from monty.dev import requires
 
-from pynter.__init__ import load_config, run_local
+from pynter import SETTINGS, run_local
 from pynter.slurm.job_script import ScriptHandler
 from pynter.data.jobs import get_job_from_directory
 
 def setup_hpc(subparsers):
     
     parser_hpc = subparsers.add_parser('HPC',help='Interface with High Performance Computer')
     
@@ -31,18 +31,17 @@
     parser_job = subparsers_hpc.add_parser('job',help='Sync and run job on HPC')
     setup_job(parser_job)
     
     return
 
 
 def setup_sync(parser):
-    config = load_config()
-    hostname = config['HPC']['hostname']
-    workdir = config['HPC']['workdir']
-    localdir = config['HPC']['localdir']
+    hostname = SETTINGS['HPC']['hostname']
+    workdir = SETTINGS['HPC']['workdir']
+    localdir = SETTINGS['HPC']['localdir']
     
     parser.add_argument('-dry','--dry-run',action='store_true',help='Dry run with rsync (default: %(default)s)',default=False,dest='dry_run')
     parser.add_argument('-exc','--exclude',action='append',help='Files to exclude from sync (default: %(default)s)',
                         default=['core.*','WAVECAR'],metavar='',type=str,dest='exclude')
     parser.add_argument('-host','--hostname',help='ssh alias of the HPC (default: %(default)s)',default=hostname,metavar='',type=str,dest='hostname')
     parser.add_argument('-ldir','--localdir',help='Local directory (default: %(default)s)',default=localdir,metavar='',type=str,dest='localdir')
     parser.add_argument('-wdir','--workdir',help='Remote directory (default: %(default)s)',default=workdir,metavar='',type=str,dest='workdir')
```

### Comparing `pynter-defects-1.0.2/pynter/cli/inputs.py` & `pynter-defects-1.0.6/pynter/cli/inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/main.py` & `pynter-defects-1.0.6/pynter/cli/main.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/materials_project.py` & `pynter-defects-1.0.6/pynter/cli/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/phase_diagram.py` & `pynter-defects-1.0.6/pynter/cli/phase_diagram.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import os
 
 from pymatgen.core.composition import Composition
 from pymatgen.entries.compatibility import MaterialsProjectCompatibility
 from pymatgen.analysis.phase_diagram import PhaseDiagram
 
-from pynter.__init__ import load_config
+from pynter import SETTINGS
 from pynter.phase_diagram.chempots import PDHandler, Reservoirs
 from pynter.tools.utils import save_object_as_json
 
 
 def setup_phase_diagram(subparsers):
     
     parser_sub = subparsers.add_parser('phase-diagram',help='Generate phase diagrams with pymatgen from the Materials Project database')
@@ -71,15 +71,15 @@
 
 
 def get_chempots(pd,composition):
     return PDHandler(pd).get_all_boundaries_chempots(composition)
     
 def get_phase_diagram(elements):  
     from pymatgen.ext.matproj import MPRester
-    with MPRester(load_config()['API_KEY']) as mpr:
+    with MPRester(SETTINGS['API_KEY']) as mpr:
         compat = MaterialsProjectCompatibility()  # sets energy corrections and +U/pseudopotential choice
         unprocessed_entries = mpr.get_entries_in_chemsys(elements,inc_structure=True)
     processed_entries = compat.process_entries(unprocessed_entries)  # filter and add energy corrections    
     return PhaseDiagram(processed_entries)
 
 def plot_pd(pd):
     return PDHandler(pd).get_plot()
```

### Comparing `pynter-defects-1.0.2/pynter/cli/plotter.py` & `pynter-defects-1.0.6/pynter/cli/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/slurm.py` & `pynter-defects-1.0.6/pynter/cli/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/cli/utils.py` & `pynter-defects-1.0.6/pynter/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/data/database/creator.py` & `pynter-defects-1.0.6/pynter/data/database/creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 Created on Mon Nov  9 11:12:09 2020
 
 @author: villa
 """
 
 import warnings
 from matgendb.creator import VaspToDbTaskDrone
-from pynter.__init__ import load_config
+from pynter import SETTINGS
 
-dbconfig = load_config()['dbconfig']
+dbconfig = SETTINGS['dbconfig']
 
 # for VaspJob we use pymatgen-db interface
 class VaspJobDrone(VaspToDbTaskDrone):
     """
     Subclass of VaspToDbTaskDrone in pymatgen-db (matgendb) package.
     To set up the database for VaspJob we use the pymatgen-db package which already provides a useful
     interface to the other pymatgen objects that are already used (like Structure or ComputedEntry).
```

### Comparing `pynter-defects-1.0.2/pynter/data/database/query.py` & `pynter-defects-1.0.6/pynter/data/database/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 @author: villa
 """
 
 
 from matgendb.query_engine import QueryEngine
 from pymatgen.io.vasp.inputs import VaspInput, Incar,Kpoints,Poscar,Potcar
 from pynter.vasp.jobs import VaspJob
-from pynter.__init__ import load_config
+from pynter import SETTINGS
 
 
-dbconfig = load_config()['dbconfig']
+dbconfig = SETTINGS['dbconfig']
 
 class VaspJobQuery(QueryEngine):
     """
     Subclass of QueryEngine in pymatgen-db (matgendb) package.
     To set up the database for VaspJob we use the pymatgen-db package which already provides a useful
     interface to the other pymatgen objects that are already used (like Structure or ComputedEntry).
     This class helps to interface a VaspJob object with the database.
```

### Comparing `pynter-defects-1.0.2/pynter/data/datasets.py` & `pynter-defects-1.0.6/pynter/data/datasets.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/data/jobs.py` & `pynter-defects-1.0.6/pynter/data/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 from abc import abstractmethod
 import os
 import os.path as op
 import shutil
+
 from pynter.slurm.job_script import ScriptHandler
 from pynter.slurm.interface import HPCInterface
 from pynter.tools.utils import grep_list
-from pynter.__init__ import load_config, run_local
+
 
 class Job:
     
     def __init__(self,path=None,inputs=None,job_settings=None,outputs=None,job_script_filename=None,name=None):
         """
         Class to control and organize inputs and outputs of a generic job.
 
@@ -29,15 +30,15 @@
         name : (str)
             Name of the job. If none the name is searched in the job script.
 
         """
                 
         self.path = path if path else os.getcwd()
         self.inputs = inputs
-        self.job_settings = job_settings.copy()
+        self.job_settings = job_settings.copy() if job_settings else job_settings
         self.outputs = outputs
         self.job_script_filename = job_script_filename if job_script_filename else ScriptHandler().filename
         
         self._localdir = HPCInterface().localdir
         self._workdir = HPCInterface().workdir
         self.path_relative = op.abspath(self.path).replace(self._localdir,'')
```

### Comparing `pynter-defects-1.0.2/pynter/defects/analysis.py` & `pynter-defects-1.0.6/pynter/defects/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/corrections.py` & `pynter-defects-1.0.6/pynter/defects/corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/defects.py` & `pynter-defects-1.0.6/pynter/defects/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/elasticity.py` & `pynter-defects-1.0.6/pynter/defects/elasticity.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/entries.py` & `pynter-defects-1.0.6/pynter/defects/entries.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/plotter.py` & `pynter-defects-1.0.6/pynter/defects/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_core.py` & `pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_corrections.py` & `pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/pmg/pmg_defects_utils.py` & `pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/pmg/pmg_dos.py` & `pynter-defects-1.0.6/pynter/defects/pmg/pmg_dos.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/structure.py` & `pynter-defects-1.0.6/pynter/defects/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/thermodynamics.py` & `pynter-defects-1.0.6/pynter/defects/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/defects/utils.py` & `pynter-defects-1.0.6/pynter/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/phase_diagram/chempots.py` & `pynter-defects-1.0.6/pynter/phase_diagram/chempots.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/phase_diagram/plotter.py` & `pynter-defects-1.0.6/pynter/phase_diagram/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/phase_diagram/thermodynamics.py` & `pynter-defects-1.0.6/pynter/phase_diagram/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/slurm/interface.py` & `pynter-defects-1.0.6/pynter/slurm/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
-import subprocess
-import os
 import os.path as op
-from glob import glob
 from shutil import which
+
 from monty.dev import requires
-from pynter.__init__ import load_config, run_local
 
+from pynter import run_local, SETTINGS
+    
 
 class HPCInterface:
     
     @requires(which("sshpass"),
               "sshpass needs to be installed, you can install it with 'sudo apt-get install sshpass'.")
     @requires(which("rsync"),
           "rsync needs to be installed, you can install it with 'sudo apt-get install rsync'.")
@@ -21,15 +20,15 @@
 
         Parameters
         ----------
         config : (dict), optional
             Configuration dictionary. If None is loaded from .pynter/config.yml.
         """
         if not config:
-            config = load_config()['HPC']
+            config = SETTINGS['HPC']
         
         for key,value in config.items():
             setattr(self, key, value)      
 
 
     def cancel_jobs(self,*args,printout=True,dry_run=False,**kwargs):
         """
```

### Comparing `pynter-defects-1.0.2/pynter/slurm/job_script.py` & `pynter-defects-1.0.6/pynter/slurm/job_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import re
 import os
 import os.path as op
-from pynter.__init__ import load_config
+
+from pynter import SETTINGS
 from pynter.tools.utils import grep_list
 
 class ScriptHandler:
     
     def __init__(self, **kwargs):
         """
         Parameters
@@ -30,16 +31,15 @@
             add_stop_array : (Bool), Add lines for stopping array jobs when calculation is converged. \n                
                 If True is effective only if key 'array_size' is not None
             add_automation : (str) , Automation script to add to the file.                
             add_lines_header : (List) , Lines to add in the header part of the file.
             add_lines_body : (List) , Lines to add in the body part of the file.
         """
         
-        config = load_config()
-        default_settings = config['job_settings']
+        default_settings = SETTINGS['job_settings']
         
         for key,value in default_settings.items():
             setattr(self,key,value)
         
         for key, value in kwargs.items():
             if key in default_settings:
                 setattr(self,key,value)
```

### Comparing `pynter-defects-1.0.2/pynter/slurm/job_status.py` & `pynter-defects-1.0.6/pynter/slurm/job_status.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/testing/__init__.py` & `pynter-defects-1.0.6/pynter/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/testing/core.py` & `pynter-defects-1.0.6/pynter/testing/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,24 +70,14 @@
         for l1, l2 in zip(lines1, lines2):
             if l1.strip() != l2.strip():
                 failed.append(f"{l1} != {l2}")
         return len(failed) == 0
     
     
     @property
-    def cfgfile(self):
-        homedir = os.getenv("HOME")
-        return op.join(homedir,'.pynter','config.yml')
-    
-    @property
-    def cfgfile_vasp(self):
-        homedir = os.getenv("HOME")
-        return op.join(homedir,'.pynter','vasp.yml')
-    
-    @property
     def incar_settings(self):
         incar_settings = {'ALGO': 'Normal',
          'AMIX': 0.2,
          'EDIFF': 1e-06,
          'EDIFFG': -0.05,
          'ENCUT': 550,
          'IBRION': 2,
```

### Comparing `pynter-defects-1.0.2/pynter/testing/data.py` & `pynter-defects-1.0.6/pynter/testing/data.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/testing/defects.py` & `pynter-defects-1.0.6/pynter/testing/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/testing/phase_diagram.py` & `pynter-defects-1.0.6/pynter/testing/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/testing/slurm.py` & `pynter-defects-1.0.6/pynter/testing/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/testing/structure.py` & `pynter-defects-1.0.6/pynter/testing/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/testing/vasp.py` & `pynter-defects-1.0.6/pynter/testing/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/tools/format.py` & `pynter-defects-1.0.6/pynter/tools/format.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/tools/materials_project.py` & `pynter-defects-1.0.6/pynter/tools/materials_project.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,169 +1,173 @@
 #!/usr/bin/env python
 
 from pymatgen.ext.matproj import MPRester
 
-from pynter.__init__ import load_config, get_cfgfile
+from pynter import  get_cfgfile
+from pynter import SETTINGS
 
 try:
-    API_KEY = load_config()['API_KEY']
+    API_KEY = SETTINGS['API_KEY']
 except:
     cfgfile = get_cfgfile()
     raise KeyError('"API_KEY" needs to be present in the %s file' %cfgfile)
 
 
-with MPRester(API_KEY) as mpr:
-
-    class MPDatabase:
+class MPDatabase:
+    
+    def __init__(self,mp_id=None):
+        """
+        Class to retrieve data from Materials Project database
+
+        Parameters
+        ----------
+        mp_id : (str), optional
+            Materials-ID. The default is None.
+        """
+        
+        self.mp_id = mp_id if mp_id else None
+        self.api_key = API_KEY
+    
+    @property
+    def mp_rester(self):
+        return MPRester(API_KEY)
         
-        def __init__(self,mp_id=None):
-            """
-            Class to retrieve data from Materials Project database
-
-            Parameters
-            ----------
-            mp_id : (str), optional
-                Materials-ID. The default is None.
-            """
-            
-            self.mp_id = mp_id if mp_id else None
-            self.api_key = API_KEY
         
-        @property
-        def mp_rester(self):
-            return mpr
-            
-            
-        def get_data(self,data_type='vasp'):    
-            """
-            Flexible method to get any data using the Materials Project REST
-            interface. Generally used by other methods for more specific queries.
-    
-            Format of REST return is *always* a list of dict (regardless of the
-            number of pieces of data returned. The general format is as follows:
-    
-            [{"material_id": material_id, "property_name" : value}, ...]
-    
-            This is generally a call to
-            https://www.materialsproject.org/rest/v2/materials/vasp/<prop>.
-            See https://github.com/materialsproject/mapidoc for details.
-    
-            Parameters
-            ----------
-                data_type (str): Type of data to return. Currently can either be
-                    "vasp" or "exp".
-            Returns:
-                List of dictionaries with available MP data
-            """
+    def get_data(self,data_type='vasp'):    
+        """
+        Flexible method to get any data using the Materials Project REST
+        interface. Generally used by other methods for more specific queries.
+
+        Format of REST return is *always* a list of dict (regardless of the
+        number of pieces of data returned. The general format is as follows:
+
+        [{"material_id": material_id, "property_name" : value}, ...]
+
+        This is generally a call to
+        https://www.materialsproject.org/rest/v2/materials/vasp/<prop>.
+        See https://github.com/materialsproject/mapidoc for details.
+
+        Parameters
+        ----------
+            data_type (str): Type of data to return. Currently can either be
+                "vasp" or "exp".
+        Returns:
+            List of dictionaries with available MP data
+        """
+        with MPRester(API_KEY) as mpr:
             data = mpr.get_data(self.mp_id,data_type=data_type) 
-            
-            return data
+        
+        return data
 
 
-        def get_entries(self,chemsys_formula_id_criteria,compatible_only=True,inc_structure='initial',
-                        property_data=None,conventional_unit_cell=False,sort_by_e_above_hull=True):
-            """
-            Get a list of ComputedEntries or ComputedStructureEntries corresponding
-            to a chemical system, formula, or materials_id or full criteria.
-    
-            Parameters
-            ----------
-                chemsys_formula_id_criteria (str/dict): A chemical system
-                    (e.g., Li-Fe-O), or formula (e.g., Fe2O3) or materials_id
-                    (e.g., mp-1234) or full Mongo-style dict criteria.
-                compatible_only (bool): Whether to return only "compatible"
-                    entries. Compatible entries are entries that have been
-                    processed using the MaterialsProject2020Compatibility class,
-                    which performs adjustments to allow mixing of GGA and GGA+U
-                    calculations for more accurate phase diagrams and reaction
-                    energies.
-                inc_structure (str): If None, entries returned are
-                    ComputedEntries. If inc_structure="initial",
-                    ComputedStructureEntries with initial structures are returned.
-                    Otherwise, ComputedStructureEntries with final structures
-                    are returned.
-                property_data (list): Specify additional properties to include in
-                    entry.data. If None, no data. Should be a subset of
-                    supported_properties.
-                conventional_unit_cell (bool): Whether to get the standard
-                    conventional unit cell
-                sort_by_e_above_hull (bool): Whether to sort the list of entries by
-                    e_above_hull (will query e_above_hull as a property_data if True).
-    
-            Returns:
-                List of ComputedEntry or ComputedStructureEntry objects.
-            """
-            return mpr.get_entries(chemsys_formula_id_criteria,compatible_only,inc_structure,
+    def get_entries(self,chemsys_formula_id_criteria,compatible_only=True,inc_structure='initial',
+                    property_data=None,conventional_unit_cell=False,sort_by_e_above_hull=True):
+        """
+        Get a list of ComputedEntries or ComputedStructureEntries corresponding
+        to a chemical system, formula, or materials_id or full criteria.
+
+        Parameters
+        ----------
+            chemsys_formula_id_criteria (str/dict): A chemical system
+                (e.g., Li-Fe-O), or formula (e.g., Fe2O3) or materials_id
+                (e.g., mp-1234) or full Mongo-style dict criteria.
+            compatible_only (bool): Whether to return only "compatible"
+                entries. Compatible entries are entries that have been
+                processed using the MaterialsProject2020Compatibility class,
+                which performs adjustments to allow mixing of GGA and GGA+U
+                calculations for more accurate phase diagrams and reaction
+                energies.
+            inc_structure (str): If None, entries returned are
+                ComputedEntries. If inc_structure="initial",
+                ComputedStructureEntries with initial structures are returned.
+                Otherwise, ComputedStructureEntries with final structures
+                are returned.
+            property_data (list): Specify additional properties to include in
+                entry.data. If None, no data. Should be a subset of
+                supported_properties.
+            conventional_unit_cell (bool): Whether to get the standard
+                conventional unit cell
+            sort_by_e_above_hull (bool): Whether to sort the list of entries by
+                e_above_hull (will query e_above_hull as a property_data if True).
+
+        Returns:
+            List of ComputedEntry or ComputedStructureEntry objects.
+        """
+        with MPRester(API_KEY) as mpr:
+            entries = mpr.get_entries(chemsys_formula_id_criteria,compatible_only,inc_structure,
                                    property_data,conventional_unit_cell,sort_by_e_above_hull)
-        
-        
-        def get_entries_from_compositions(self,compositions,lowest_e_above_hull=False,compatible_only=True,
-                                          inc_structure='initial',property_data=None,
-                                          conventional_unit_cell=False):
-            """
-            Get a dictionary with compositions (strings) as keys and a list of ComputedEntries 
-            or ComputedStructureEntries as values.
-    
-            Parameters
-            ----------
-                compositions (list): List of strings with compositions.
-                stable_only (bool): Get phase with lowest E above hull.
-                compatible_only (bool): 
-                    Whether to return only "compatible"
-                    entries. Compatible entries are entries that have been
-                    processed using the MaterialsProject2020Compatibility class,
-                    which performs adjustments to allow mixing of GGA and GGA+U
-                    calculations for more accurate phase diagrams and reaction
-                    energies.
-                inc_structure (str):
-                    If None, entries returned are
-                    ComputedEntries. If inc_structure="initial",
-                    ComputedStructureEntries with initial structures are returned.
-                    Otherwise, ComputedStructureEntries with final structures
-                    are returned.
-                property_data (list):
-                    Specify additional properties to include in
-                    entry.data. If None, no data. Should be a subset of
-                    supported_properties.
-                conventional_unit_cell (bool):
-                    Whether to get the standard conventional unit cell
-                sort_by_e_above_hull (bool): Whether to sort the list of entries by
-                    e_above_hull (will query e_above_hull as a property_data if True).
-    
-            Returns:
-                List of ComputedEntry or ComputedStructureEntry objects.
-            """
-            entries_dict = {}
-            for comp in compositions:
-                entries = self.get_entries(comp,compatible_only,inc_structure,property_data,
-                                                      conventional_unit_cell,sort_by_e_above_hull=True)
-                if lowest_e_above_hull:
-                    entries_dict[comp] = entries[0] # sorted by e_above_hull
-                else:
-                    entries_dict[comp] = entries
-            return entries_dict
-        
-
-        def get_structure(self,final=False,conventional_unit_cell=False):
-            """
-            Get a Structure corresponding to a material_id.
-    
-            Parameters
-            ----------
-                material_id (str): Materials Project material_id (a string,
-                    e.g., mp-1234).
-                final (bool): Whether to get the final structure, or the initial
-                    (pre-relaxation) structure. Defaults to True.
-                conventional_unit_cell (bool): Whether to get the standard
-                    conventional unit cell
-    
-            Returns:
-                Structure object.
-            """
-            return mpr.get_structure_by_material_id(self.mp_id,final=final,conventional_unit_cell=conventional_unit_cell).get_sorted_structure()  
+        return entries
+    
+    
+    def get_entries_from_compositions(self,compositions,lowest_e_above_hull=False,compatible_only=True,
+                                      inc_structure='initial',property_data=None,
+                                      conventional_unit_cell=False):
+        """
+        Get a dictionary with compositions (strings) as keys and a list of ComputedEntries 
+        or ComputedStructureEntries as values.
+
+        Parameters
+        ----------
+            compositions (list): List of strings with compositions.
+            stable_only (bool): Get phase with lowest E above hull.
+            compatible_only (bool): 
+                Whether to return only "compatible"
+                entries. Compatible entries are entries that have been
+                processed using the MaterialsProject2020Compatibility class,
+                which performs adjustments to allow mixing of GGA and GGA+U
+                calculations for more accurate phase diagrams and reaction
+                energies.
+            inc_structure (str):
+                If None, entries returned are
+                ComputedEntries. If inc_structure="initial",
+                ComputedStructureEntries with initial structures are returned.
+                Otherwise, ComputedStructureEntries with final structures
+                are returned.
+            property_data (list):
+                Specify additional properties to include in
+                entry.data. If None, no data. Should be a subset of
+                supported_properties.
+            conventional_unit_cell (bool):
+                Whether to get the standard conventional unit cell
+            sort_by_e_above_hull (bool): Whether to sort the list of entries by
+                e_above_hull (will query e_above_hull as a property_data if True).
+
+        Returns:
+            List of ComputedEntry or ComputedStructureEntry objects.
+        """
+        entries_dict = {}
+        for comp in compositions:
+            entries = self.get_entries(comp,compatible_only,inc_structure,property_data,
+                                                  conventional_unit_cell,sort_by_e_above_hull=True)
+            if lowest_e_above_hull:
+                entries_dict[comp] = entries[0] # sorted by e_above_hull
+            else:
+                entries_dict[comp] = entries
+        return entries_dict
+    
+
+    def get_structure(self,final=False,conventional_unit_cell=False):
+        """
+        Get a Structure corresponding to a material_id.
+
+        Parameters
+        ----------
+            material_id (str): Materials Project material_id (a string,
+                e.g., mp-1234).
+            final (bool): Whether to get the final structure, or the initial
+                (pre-relaxation) structure. Defaults to True.
+            conventional_unit_cell (bool): Whether to get the standard
+                conventional unit cell
+
+        Returns:
+            Structure object.
+        """
+        with MPRester(API_KEY) as mpr:
+            structure = mpr.get_structure_by_material_id(self.mp_id,final=final,conventional_unit_cell=conventional_unit_cell).get_sorted_structure()
+        return structure
```

### Comparing `pynter-defects-1.0.2/pynter/tools/structure.py` & `pynter-defects-1.0.6/pynter/tools/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/tools/utils.py` & `pynter-defects-1.0.6/pynter/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/vasp/analysis.py` & `pynter-defects-1.0.6/pynter/vasp/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
-import os
+
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
+
 from pymatgen.core.periodic_table import Element
-from pymatgen.electronic_structure.plotter import BSDOSPlotter
 from pymatgen.analysis.eos import EOS
-from pynter.vasp.plotter import plot_spd_dos
+
 
 matplotlib.rcParams.update({'font.size': 15})
 
 
 class DatasetAnalysis:
     
     def __init__(self,jobs):
```

### Comparing `pynter-defects-1.0.2/pynter/vasp/default_inputs.py` & `pynter-defects-1.0.6/pynter/vasp/default_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,38 +3,36 @@
 """
 Created on Fri Feb 21 10:59:10 2020
 
 @author: villa
 """
 
 from pymatgen.io.vasp.inputs import Kpoints, Poscar, Potcar, VaspInput, Incar
-from pynter.vasp.__init__ import load_vasp_default, get_vasp_cfgfile
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.symmetry.bandstructure import HighSymmKpath
 
+from pynter import SETTINGS
 
-cfgfile = get_vasp_cfgfile()
 
 class DefaultInputs:
     """
     Class to generate VASP input files with default parameters. Use with extreme care.    
     """
     
-    def __init__(self,structure=None,sort_structure=True,cfgfile=cfgfile):
+    def __init__(self,structure=None,sort_structure=True):
         """
         Parameters
         ----------
         structure : Pymatgen Structure object. The default is None. If no Structure is given only default INCAR can be generated.
         sort_structure (bool) : Sort structure to avoid POSCAR/POTCAR inconsistencies. The default is True.
-        cfgfile : File with default VASP parameters. The default is "~/.pynter.vasp.yml".
         """
-        if sort_structure:
+        if structure and sort_structure:
             structure.sort()
         self._structure = structure if structure else None 
-        defaults = load_vasp_default(cfgfile=cfgfile)
+        defaults = SETTINGS['vasp']
         
         self.default_potcar_symbols =  defaults['default_potcar_symbols']
         if self.structure:
             self.potcar_symbols = [self.default_potcar_symbols[el.symbol] for el in self.structure.composition.elements]
         self.incar_default_flags = defaults['incar_default']
         
     @property
```

### Comparing `pynter-defects-1.0.2/pynter/vasp/jobs.py` & `pynter-defects-1.0.6/pynter/vasp/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 
 @author: villa
 """
 
 
 import os
 import os.path as op
+import warnings
+import numpy as np
+import json
+from glob import glob
+
+from monty.json import MontyDecoder, MontyEncoder
+
 from pymatgen.io.vasp.inputs import VaspInput, Poscar, Incar, Kpoints, Potcar
 from pymatgen.io.vasp.outputs import Vasprun, Oszicar
 from pymatgen.core.structure import Structure
 from pymatgen.analysis.transition_state import NEBAnalysis
-from pynter.slurm.job_script import ScriptHandler
-import numpy as np
-import json
-from monty.json import MontyDecoder, MontyEncoder
-from glob import glob
+
 from pynter.tools.utils import grep
 from pynter.data.jobs import Job
 from pynter.slurm.interface import HPCInterface
-from pynter.vasp.__init__ import load_vasp_default
-import warnings
+from pynter.slurm.job_script import ScriptHandler
+from pynter import SETTINGS
+
+
 from pymatgen.io.vasp.inputs import UnknownPotcarWarning
 
 warnings.filterwarnings("ignore", category=UnknownPotcarWarning)
 
 
 class VaspJob(Job):
  
@@ -479,15 +484,15 @@
         data : (list), optional
             List of attributes of Vasprun to parse in ComputedStructureEntry.
             the attributes parsed by default are 'final_energy','structures','eigenvalue_band_properties',
             'parameters','actual_kpoints','ionic_steps'. The default is None.
         """                
         self._is_converged = self._get_convergence()
         
-        self._default_data_computed_entry = load_vasp_default()['computed_entry_default'] # default imports from Vasprun
+        self._default_data_computed_entry = SETTINGS['vasp']['computed_entry_default'] # default imports from Vasprun
 
         kwargs = self._parse_kwargs(**kwargs)  
         if self.vasprun:
             data = self._default_data_computed_entry 
             if kwargs['data']:
                 for attr in kwargs['data']:
                     data.append(attr)
```

### Comparing `pynter-defects-1.0.2/pynter/vasp/plotter.py` & `pynter-defects-1.0.6/pynter/vasp/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/vasp/pmg/pmg_electronic_structure_plotter.py` & `pynter-defects-1.0.6/pynter/vasp/pmg/pmg_electronic_structure_plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.2/pynter/vasp/schemes.py` & `pynter-defects-1.0.6/pynter/vasp/schemes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 Created on Wed Feb 19 14:52:51 2020
 
 @author: villa
 """
 import os
 import os.path as op
 import numpy as np
+
 from pymatgen.core.periodic_table import Element
-from pymatgen.symmetry.bandstructure import HighSymmKpath
 from pymatgen.io.vasp.inputs import VaspInput, Incar, Poscar, Kpoints
+
 from pynter.vasp.default_inputs import DefaultInputs
 from pynter.vasp.jobs import VaspJob, VaspNEBJob
-from pynter.defects.structure import create_vacancy_structures, create_substitution_structures
-from pynter.defects.defects import create_vacancies, create_substitutions, create_interstitials
+from pynter.defects.defects import create_vacancies, create_substitutions
 
 
 class InputSets:
     
     def __init__(self,path=None,vaspinput=None,structure=None,incar_settings=None,kpoints=None,potcar=None,
                  job_settings=None,name=None,add_parent_folder=False):
         """
```

### Comparing `pynter-defects-1.0.2/pynter_defects.egg-info/SOURCES.txt` & `pynter-defects-1.0.6/pynter_defects.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 pynter/__init__.py
+pynter/config_default.yml
 pynter/automations/__init__.py
 pynter/automations/core.py
 pynter/automations/vasp.py
 pynter/cli/analysis.py
 pynter/cli/automations.py
 pynter/cli/config.py
 pynter/cli/defects.py
@@ -60,15 +61,15 @@
 pynter/tools/utils.py
 pynter/vasp/__init__.py
 pynter/vasp/analysis.py
 pynter/vasp/default_inputs.py
 pynter/vasp/jobs.py
 pynter/vasp/plotter.py
 pynter/vasp/schemes.py
-pynter/vasp/utils.py
+pynter/vasp/vasp_default.yml
 pynter/vasp/pmg/pmg_electronic_structure_plotter.py
 pynter_defects.egg-info/PKG-INFO
 pynter_defects.egg-info/SOURCES.txt
 pynter_defects.egg-info/dependency_links.txt
 pynter_defects.egg-info/entry_points.txt
 pynter_defects.egg-info/requires.txt
 pynter_defects.egg-info/top_level.txt
```

