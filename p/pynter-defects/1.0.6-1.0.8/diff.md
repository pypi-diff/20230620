# Comparing `tmp/pynter-defects-1.0.6.tar.gz` & `tmp/pynter-defects-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynter-defects-1.0.6.tar", last modified: Tue Jun 20 13:26:31 2023, max compression
+gzip compressed data, was "pynter-defects-1.0.8.tar", last modified: Tue Jun 20 15:23:26 2023, max compression
```

## Comparing `pynter-defects-1.0.6.tar` & `pynter-defects-1.0.8.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.348495 pynter-defects-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 13:26:31.348495 pynter-defects-1.0.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.328495 pynter-defects-1.0.6/pynter/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.328495 pynter-defects-1.0.6/pynter/automations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/automations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/automations/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/automations/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.332495 pynter-defects-1.0.6/pynter/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/defects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/inputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/phase_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/config_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.332495 pynter-defects-1.0.6/pynter/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.332495 pynter-defects-1.0.6/pynter/data/database/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/database/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/database/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    29512 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/data/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.336495 pynter-defects-1.0.6/pynter/defects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45917 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/defects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.336495 pynter-defects-1.0.6/pynter/defects/pmg/
--rwxr-xr-x   0 runner    (1001) docker     (123)    24611 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    60074 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39933 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/pmg/pmg_dos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.336495 pynter-defects-1.0.6/pynter/phase_diagram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32436 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/chempots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/phase_diagram/thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.340495 pynter-defects-1.0.6/pynter/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/job_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/slurm/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.340495 pynter-defects-1.0.6/pynter/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/defects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/phase_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/testing/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/default_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter/vasp/pmg/
--rw-r--r--   0 runner    (1001) docker     (123)   183623 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/pynter/vasp/vasp_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:26:31.344495 pynter-defects-1.0.6/pynter_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:26:31.000000 pynter-defects-1.0.6/pynter_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:26:31.348495 pynter-defects-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-20 13:26:14.000000 pynter-defects-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/automations/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/automations/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/inputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/config_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/data/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/database/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29513 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45918 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/defects/pmg/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24611 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60074 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39933 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19877 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/phase_diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/chempots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/job_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/pynter/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/default_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/pynter/vasp/pmg/
+-rw-r--r--   0 runner    (1001) docker     (123)   183623 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 15:23:17.000000 pynter-defects-1.0.8/pynter/vasp/vasp_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/pynter_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-20 15:23:17.000000 pynter-defects-1.0.8/setup.py
```

### Comparing `pynter-defects-1.0.6/PKG-INFO` & `pynter-defects-1.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynter-defects
-Version: 1.0.6
+Version: 1.0.8
 Summary: Tools for atomistic calculations, provides features for point-defect calculations with VASP
 Author: Lorenzo Villa
 Description-Content-Type: text/markdown
 
 # pynter
 Tools for atomistic calculations. Uses pymatgen package (https://pymatgen.org). The main features are designed to systematically run, analyse and plot DFT point defect calculations with VASP.
```

### Comparing `pynter-defects-1.0.6/README.md` & `pynter-defects-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/__init__.py` & `pynter-defects-1.0.8/pynter/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/automations/core.py` & `pynter-defects-1.0.8/pynter/automations/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/automations/vasp.py` & `pynter-defects-1.0.8/pynter/automations/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/analysis.py` & `pynter-defects-1.0.8/pynter/cli/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/automations.py` & `pynter-defects-1.0.8/pynter/cli/automations.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/config.py` & `pynter-defects-1.0.8/pynter/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
         
         filename = filename_config
         
         print('Begin setup\n')
         print('HPC setup:')
         hostname = input('Hostname: ')
         localdir = input('Local calculation directory: ')
-        localdir = os.path.abspath(localdir)
+        localdir = os.path.abspath(localdir) if localdir else None
         workdir = input('Remote calculation directory: ')
-        workdir = os.path.normpath(workdir)
+        workdir = os.path.normpath(workdir) if workdir else None
         
         print('\nDefault settings for job script setup: ')
         project_id = input('Project ID: ')
         email = input('email address (Default None): ')
         path_exe = input('Path of default executable: ')
         job_script_filename = input('Job script filename (default job.sh): ')
```

### Comparing `pynter-defects-1.0.6/pynter/cli/defects.py` & `pynter-defects-1.0.8/pynter/cli/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/hpc.py` & `pynter-defects-1.0.8/pynter/cli/hpc.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/inputs.py` & `pynter-defects-1.0.8/pynter/cli/inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/main.py` & `pynter-defects-1.0.8/pynter/cli/main.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/materials_project.py` & `pynter-defects-1.0.8/pynter/cli/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/phase_diagram.py` & `pynter-defects-1.0.8/pynter/cli/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/plotter.py` & `pynter-defects-1.0.8/pynter/cli/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/slurm.py` & `pynter-defects-1.0.8/pynter/cli/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/cli/utils.py` & `pynter-defects-1.0.8/pynter/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/config_default.yml` & `pynter-defects-1.0.8/pynter/config_default.yml`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/data/database/creator.py` & `pynter-defects-1.0.8/pynter/data/database/creator.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/data/database/query.py` & `pynter-defects-1.0.8/pynter/data/database/query.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/data/datasets.py` & `pynter-defects-1.0.8/pynter/data/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         Dataset object.
 
         """
         if op.isfile(path_or_string):
             with open(path_or_string) as file:
                 d = json.load(file)
         else:
-            d = json.load(path_or_string)
+            d = json.loads(path_or_string)
         return Dataset.from_dict(d)
         
     
     
     @staticmethod
     def from_directory(path=None,job_script_filenames='job.sh',sort='name',load_outputs=True,jobs_kwargs=None): 
         """
```

### Comparing `pynter-defects-1.0.6/pynter/data/jobs.py` & `pynter-defects-1.0.8/pynter/data/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/analysis.py` & `pynter-defects-1.0.8/pynter/defects/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         DefectsAnalysis object.
 
         """
         if op.isfile(path_or_string):
             with open(path_or_string) as file:
                 d = json.load(file)
         else:
-            d = json.load(path_or_string)
+            d = json.loads(path_or_string)
         return DefectsAnalysis.from_dict(d)
 
 
     @property
     def elements(self):
         """
         List of all the elements involved in exchange of atoms with a reservoir
```

### Comparing `pynter-defects-1.0.6/pynter/defects/corrections.py` & `pynter-defects-1.0.8/pynter/defects/corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/defects.py` & `pynter-defects-1.0.8/pynter/defects/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/elasticity.py` & `pynter-defects-1.0.8/pynter/defects/elasticity.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/entries.py` & `pynter-defects-1.0.8/pynter/defects/entries.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/plotter.py` & `pynter-defects-1.0.8/pynter/defects/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_core.py` & `pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_corrections.py` & `pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/pmg/pmg_defects_utils.py` & `pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/pmg/pmg_dos.py` & `pynter-defects-1.0.8/pynter/defects/pmg/pmg_dos.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/structure.py` & `pynter-defects-1.0.8/pynter/defects/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/defects/thermodynamics.py` & `pynter-defects-1.0.8/pynter/defects/thermodynamics.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,15 @@
         ThermoData object.
 
         """
         if op.isfile(path_or_string):
             with open(path_or_string) as file:
                 d = json.load(file)
         else:
-            d = json.load(path_or_string)
+            d = json.loads(path_or_string)
         return ThermoData.from_dict(d)
     
     
     def get_specific_pressures(self,p_values):
         """
         Get ThermoData object only for specific pressure values. The closest pressure value
         present in list is chosen for each provided value.
```

### Comparing `pynter-defects-1.0.6/pynter/defects/utils.py` & `pynter-defects-1.0.8/pynter/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/phase_diagram/chempots.py` & `pynter-defects-1.0.8/pynter/phase_diagram/chempots.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         Reservoir object.
 
         """
         if op.isfile(path_or_string):
             with open(path_or_string) as file:
                 d = json.load(file)
         else:
-            d = json.load(path_or_string)
+            d = json.loads(path_or_string)
         return Reservoirs.from_dict(d)
 
 
     def filter_reservoirs(self,inplace=False,elements=None):
         """
         Get new Reservoir object filtering the chempots dictionary.
```

### Comparing `pynter-defects-1.0.6/pynter/phase_diagram/plotter.py` & `pynter-defects-1.0.8/pynter/phase_diagram/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/phase_diagram/thermodynamics.py` & `pynter-defects-1.0.8/pynter/phase_diagram/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/slurm/interface.py` & `pynter-defects-1.0.8/pynter/slurm/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 from monty.dev import requires
 
 from pynter import run_local, SETTINGS
     
 
 class HPCInterface:
     
-    @requires(which("sshpass"),
-              "sshpass needs to be installed, you can install it with 'sudo apt-get install sshpass'.")
-    @requires(which("rsync"),
-          "rsync needs to be installed, you can install it with 'sudo apt-get install rsync'.")
     
     def __init__(self,config=None):
         """
         Class to interface commands with HPC
 
         Parameters
         ----------
@@ -48,15 +44,17 @@
         cmd = 'scancel '
         for arg in args:
             cmd += arg + ' '
                 
         stdout,stderr = self.command(cmd,printout,dry_run,**kwargs)
         return stdout,stderr
 
-            
+
+    @requires(which("sshpass"),
+              "sshpass needs to be installed, you can install it with 'sudo apt-get install sshpass'.")     
     def command(self,cmd,printout=True,dry_run=False,**kwargs):   
         """
         Run command on HPC
 
         Parameters
         ----------
         cmd : (str)
@@ -137,15 +135,17 @@
         stderr : (str)
             Error.
         """
         
         stdout,stderr = self.command(cmd,printout,dry_run,**kwargs)
         return stdout, stderr
     
-
+    
+    @requires(which("rsync"),
+          "rsync needs to be installed, you can install it with 'sudo apt-get install rsync'.")
     def rsync_from_hpc(self,remotedir=None,localdir=None,exclude=None,printout=True,dry_run=False,**kwargs):
         """
         Sync folders from HPC to local machine. The command "rsync" is used. With this function all
         the folders contained in the remote dir are synched to the local dir.
 
         Parameters
         ----------
@@ -184,14 +184,16 @@
                 cmd += f'--exclude={s} ' 
         cmd += f"-e ssh {self.hostname}:{remotedir} {localdir} "
 
         stdout,stderr = run_local(cmd,printout=printout,dry_run=False,**kwargs)
         return stdout,stderr
 
 
+    @requires(which("rsync"),
+          "rsync needs to be installed, you can install it with 'sudo apt-get install rsync'.")
     def rsync_to_hpc(self,localdir=None,remotedir=None,exclude=None,printout=True,dry_run=False,**kwargs):
         """
         Sync folders from local machine to HPC. The command "rsync" is used. With this function all
         the folders contained in the local dir are synched to the remote dir.
 
         Parameters
         ----------
@@ -229,15 +231,17 @@
                 cmd += f'--exclude={s} '
         cmd += f"-e ssh  {localdir} {self.hostname}:{remotedir} "
         
         stdout,stderr = run_local(cmd,printout=printout,dry_run=False,**kwargs)
 
         return stdout,stderr
     
-          
+    
+    @requires(which("sshpass"),
+              "sshpass needs to be installed, you can install it with 'sudo apt-get install sshpass'.")      
     def sbatch(self,path='',job_script_filename='job.sh',printout=True,dry_run=False,**kwargs):
         """
         Execute "sbatch" command on HPC to run job.
 
         Parameters
         ----------
         path : (str), optional
```

### Comparing `pynter-defects-1.0.6/pynter/slurm/job_script.py` & `pynter-defects-1.0.8/pynter/slurm/job_script.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/slurm/job_status.py` & `pynter-defects-1.0.8/pynter/slurm/job_status.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/__init__.py` & `pynter-defects-1.0.8/pynter/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/core.py` & `pynter-defects-1.0.8/pynter/testing/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/data.py` & `pynter-defects-1.0.8/pynter/testing/data.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/defects.py` & `pynter-defects-1.0.8/pynter/testing/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/phase_diagram.py` & `pynter-defects-1.0.8/pynter/testing/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/slurm.py` & `pynter-defects-1.0.8/pynter/testing/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/structure.py` & `pynter-defects-1.0.8/pynter/testing/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/testing/vasp.py` & `pynter-defects-1.0.8/pynter/testing/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/tools/format.py` & `pynter-defects-1.0.8/pynter/tools/format.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/tools/materials_project.py` & `pynter-defects-1.0.8/pynter/tools/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/tools/structure.py` & `pynter-defects-1.0.8/pynter/tools/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/tools/utils.py` & `pynter-defects-1.0.8/pynter/tools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,14 +129,32 @@
     return names
     
 def explore_pynter_packages():
     path = pynter.__path__[0]
     return explore_packages(path)            
 
 
+def get_content_from_url(file_url):
+    """
+    Get content from URL.
+
+    Parameters
+    ----------
+    file_url: URL to retrieve content from.
+
+    Returns
+    -------
+    String with content.
+    """
+    import urllib.request
+    with urllib.request.urlopen(file_url) as url:
+       content = url.read().decode('utf-8')
+    return content
+    
+
 def get_object_feature(obj,feature):
     """
     Get value of attribute or method of a generic Object.
     If feature is a single method only the string with the method's name is required.
     If the target feature is stored in a dictionary (or dict of dictionaries), a list of this format needs to be provided:
         ["method_name",key1,key2,...] - This will identify the value of Object.method[key1][key2][...] .
```

### Comparing `pynter-defects-1.0.6/pynter/vasp/analysis.py` & `pynter-defects-1.0.8/pynter/vasp/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/vasp/default_inputs.py` & `pynter-defects-1.0.8/pynter/vasp/default_inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/vasp/jobs.py` & `pynter-defects-1.0.8/pynter/vasp/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/vasp/plotter.py` & `pynter-defects-1.0.8/pynter/vasp/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/vasp/pmg/pmg_electronic_structure_plotter.py` & `pynter-defects-1.0.8/pynter/vasp/pmg/pmg_electronic_structure_plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/vasp/schemes.py` & `pynter-defects-1.0.8/pynter/vasp/schemes.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter/vasp/vasp_default.yml` & `pynter-defects-1.0.8/pynter/vasp/vasp_default.yml`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/pynter_defects.egg-info/PKG-INFO` & `pynter-defects-1.0.8/pynter_defects.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynter-defects
-Version: 1.0.6
+Version: 1.0.8
 Summary: Tools for atomistic calculations, provides features for point-defect calculations with VASP
 Author: Lorenzo Villa
 Description-Content-Type: text/markdown
 
 # pynter
 Tools for atomistic calculations. Uses pymatgen package (https://pymatgen.org). The main features are designed to systematically run, analyse and plot DFT point defect calculations with VASP.
```

### Comparing `pynter-defects-1.0.6/pynter_defects.egg-info/SOURCES.txt` & `pynter-defects-1.0.8/pynter_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.6/setup.py` & `pynter-defects-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md") as file:
     long_description = file.read()
 
 setup(
     name='pynter-defects',
-    version='1.0.6',
+    version='1.0.8',
     author='Lorenzo Villa',
     description='Tools for atomistic calculations, provides features for point-defect calculations with VASP',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(exclude=["pynter.*.tests", "pynter.*.*.tests"]),
     install_requires=[
         'ase',
```

