# Comparing `tmp/exaparser-2023.6.16.post0.tar.gz` & `tmp/exaparser-2023.6.20.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exaparser-2023.6.16.post0.tar", last modified: Fri Jun 16 01:20:02 2023, max compression
+gzip compressed data, was "exaparser-2023.6.20.post0.tar", last modified: Tue Jun 20 02:23:56 2023, max compression
```

## Comparing `exaparser-2023.6.16.post0.tar` & `exaparser-2023.6.20.post0.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.586689 exaparser-2023.6.16.post0/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.534686 exaparser-2023.6.16.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.558687 exaparser-2023.6.16.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-16 01:20:02.586689 exaparser-2023.6.16.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.546686 exaparser-2023.6.16.post0/exaparser/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 01:20:02.000000 exaparser-2023.6.16.post0/exaparser/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.546686 exaparser-2023.6.16.post0/exaparser/data/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/data/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.550687 exaparser-2023.6.16.post0/exaparser/data/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/data/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/data/handlers/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/data/handlers/exabyte.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/data/handlers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.550687 exaparser-2023.6.16.post0/exaparser/job/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.550687 exaparser-2023.6.16.post0/exaparser/job/compute/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/job/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/job/compute/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.550687 exaparser-2023.6.16.post0/exaparser/job/compute/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/job/compute/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/job/compute/managers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/job/compute/managers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.562687 exaparser-2023.6.16.post0/exaparser/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/templates/espresso.json
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/templates/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/templates/vasp.json
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.554687 exaparser-2023.6.16.post0/exaparser/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/subworkflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.554687 exaparser-2023.6.16.post0/exaparser/workflow/units/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.554687 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.554687 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/modeling/espresso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/modeling/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.558687 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/scripting/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/units/subworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/exaparser/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.558687 exaparser-2023.6.16.post0/exaparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-16 01:20:02.000000 exaparser-2023.6.16.post0/exaparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-16 01:20:02.000000 exaparser-2023.6.16.post0/exaparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:20:02.000000 exaparser-2023.6.16.post0/exaparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 01:20:02.000000 exaparser-2023.6.16.post0/exaparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 01:20:02.000000 exaparser-2023.6.16.post0/exaparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 01:20:02.000000 exaparser-2023.6.16.post0/exaparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-16 01:20:02.586689 exaparser-2023.6.16.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.562687 exaparser-2023.6.16.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.538686 exaparser-2023.6.16.post0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.562687 exaparser-2023.6.16.post0/tests/fixtures/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/shell-job.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.562687 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/job.rms
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.538686 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.566687 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.570688 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   160469 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.570688 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.570688 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.574688 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.574688 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.574688 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)   377892 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   160388 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.574688 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/pseudo/
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/pw-scf.in
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.578688 exaparser-2023.6.16.post0/tests/fixtures/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/shell-job.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.582688 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/CHG
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/CHGCAR
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/CONTCAR
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/DOSCAR
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/EIGENVAL
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/IBZKPT
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/INCAR
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/KPOINTS
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/OSZICAR
--rw-r--r--   0 runner    (1001) docker     (123)    53180 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/PCDAT
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/POSCAR
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/POTCAR
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/WAVECAR
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/XDATCAR
--rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/job.rms
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    37663 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.586689 exaparser-2023.6.16.post0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/integration/test_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:02.586689 exaparser-2023.6.16.post0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:19:23.000000 exaparser-2023.6.16.post0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.133239 exaparser-2023.6.20.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.113239 exaparser-2023.6.20.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-20 02:23:56.133239 exaparser-2023.6.20.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.117239 exaparser-2023.6.20.post0/exaparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-20 02:23:56.000000 exaparser-2023.6.20.post0/exaparser/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.117239 exaparser-2023.6.20.post0/exaparser/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/data/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.117239 exaparser-2023.6.20.post0/exaparser/data/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/data/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/data/handlers/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/data/handlers/exabyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/data/handlers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/job/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/job/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/job/compute/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/job/compute/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/job/compute/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/job/compute/managers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/job/compute/managers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/templates/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/templates/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/templates/vasp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/subworkflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/workflow/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/modeling/espresso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/modeling/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/scripting/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/units/subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/exaparser/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.121239 exaparser-2023.6.20.post0/exaparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-20 02:23:56.000000 exaparser-2023.6.20.post0/exaparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-20 02:23:56.000000 exaparser-2023.6.20.post0/exaparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:23:56.000000 exaparser-2023.6.20.post0/exaparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 02:23:56.000000 exaparser-2023.6.20.post0/exaparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-20 02:23:56.000000 exaparser-2023.6.20.post0/exaparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 02:23:56.000000 exaparser-2023.6.20.post0/exaparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-20 02:23:56.133239 exaparser-2023.6.20.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.125239 exaparser-2023.6.20.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.117239 exaparser-2023.6.20.post0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.125239 exaparser-2023.6.20.post0/tests/fixtures/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/shell-job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.125239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/job.rms
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.117239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.125239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.125239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   160469 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.125239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.129239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.129239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.129239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.129239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   377892 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   160388 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.129239 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/pw-scf.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.129239 exaparser-2023.6.20.post0/tests/fixtures/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/shell-job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.133239 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/CHG
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/CHGCAR
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/CONTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/DOSCAR
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/EIGENVAL
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/IBZKPT
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/INCAR
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/OSZICAR
+-rw-r--r--   0 runner    (1001) docker     (123)    53180 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/PCDAT
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/WAVECAR
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/XDATCAR
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/job.rms
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    37663 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.133239 exaparser-2023.6.20.post0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/integration/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:56.133239 exaparser-2023.6.20.post0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:23:18.000000 exaparser-2023.6.20.post0/tests/utils.py
```

### Comparing `exaparser-2023.6.16.post0/.github/workflows/cicd.yml` & `exaparser-2023.6.20.post0/.github/workflows/cicd.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,38 @@
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
   cancel-in-progress: true
 
 jobs:
 
+  run-linter:
+    runs-on: ubuntu-20.04
+    strategy:
+      matrix:
+        python-version: [3.8.6]
+
+    steps:
+      - name: Checkout this repository
+        uses: actions/checkout@v3
+        with:
+          lfs: true
+
+      - name: Checkout actions repository
+        uses: actions/checkout@v3
+        with:
+          repository: Exabyte-io/actions
+          token: ${{ secrets.BOT_GITHUB_TOKEN }}
+          path: actions
+
+      - name: Run ruff linter
+        uses: ./actions/py/lint
+        with:
+          python-version: ${{ matrix.python-version }}
+
   run-tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.7, 3.8]
 
     steps:
@@ -32,15 +56,15 @@
         with:
           python-version: ${{ matrix.python-version }}
           unit-test-directory: tests/unit
           integration-test-directory: tests/integration
 
 
   publish:
-    needs: run-tests
+    needs: [run-linter, run-tests]
     runs-on: ubuntu-latest
     if: github.ref_name == 'dev'
 
     steps:
       - name: Checkout this repository
         uses: actions/checkout@v2
         with:
```

### Comparing `exaparser-2023.6.16.post0/.gitignore` & `exaparser-2023.6.20.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/LICENSE` & `exaparser-2023.6.20.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/PKG-INFO` & `exaparser-2023.6.20.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exaparser
-Version: 2023.6.16.post0
+Version: 2023.6.20.post0
 Summary: Exabyte Parser
 Home-page: https://github.com/Exabyte-io/exaparser
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
```

### Comparing `exaparser-2023.6.16.post0/README.md` & `exaparser-2023.6.20.post0/README.md`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/config` & `exaparser-2023.6.20.post0/config`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/exaparser/cli.py` & `exaparser-2023.6.20.post0/exaparser/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from .config import ExaParserConfig
 from .data.factory import get_data_handler
 from .job import Job
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
-    parser.add_argument('-n', '--name', required=True, help='job name')
-    parser.add_argument('-c', '--config', help='full path to config file')
-    parser.add_argument('-w', '--work-dir', dest="work_dir", required=True, help='full path to working directory')
+    parser.add_argument("-n", "--name", required=True, help="job name")
+    parser.add_argument("-c", "--config", help="full path to config file")
+    parser.add_argument("-w", "--work-dir", dest="work_dir", required=True, help="full path to working directory")
     return parser.parse_args()
 
 
 def main():
     args = parse_arguments()
     if args.config:
         ExaParserConfig.read(args.config)
```

### Comparing `exaparser-2023.6.16.post0/exaparser/config.py` & `exaparser-2023.6.20.post0/exaparser/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 def find_config_file() -> Path:
     """
     Look in an ordered list of standard locations for the exaparser config file, and return the first one we find.
     If no config file is found, throw an Exception()
     """
     possible_filepaths = [
-        Path(__file__) / '../../config',
-        Path(os.path.expanduser('~')) / '.exabyte/exaparser/config',
-        Path('/etc/exabyte/exaparser/config'),
+        Path(__file__) / "../../config",
+        Path(os.path.expanduser("~")) / ".exabyte/exaparser/config",
+        Path("/etc/exabyte/exaparser/config"),
     ]
     for path in possible_filepaths:
         path = path.resolve()
         if path.is_file():
             return path
-    raise Exception('Could not find exaparser config file in any of the known locations.')
+    raise Exception("Could not find exaparser config file in any of the known locations.")
 
 
 ExaParserConfig = configparser.ConfigParser(allow_no_value=True)
 ExaParserConfig.read(find_config_file())
```

### Comparing `exaparser-2023.6.16.post0/exaparser/data/factory.py` & `exaparser-2023.6.20.post0/exaparser/data/factory.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/exaparser/data/handlers/disk.py` & `exaparser-2023.6.20.post0/exaparser/data/handlers/disk.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/exaparser/data/handlers/exabyte.py` & `exaparser-2023.6.20.post0/exaparser/data/handlers/exabyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         """
         return [
             ExaParserConfig.get("exabyte_api_data_handler", "hostname"),
             ExaParserConfig.getint("exabyte_api_data_handler", "port"),
             ExaParserConfig.get("exabyte_api_data_handler", "account_id"),
             ExaParserConfig.get("exabyte_api_data_handler", "auth_token"),
             ExaParserConfig.get("exabyte_api_data_handler", "version"),
-            ExaParserConfig.getboolean("exabyte_api_data_handler", "secure")
+            ExaParserConfig.getboolean("exabyte_api_data_handler", "secure"),
         ]
 
     @property
     def owner(self):
         """
         Returns the owner configuration extracted from the project.
 
@@ -68,15 +68,15 @@
         Returns:
              dict
         """
         if not self._project:
             self._project = self.project_endpoints.list(
                 {
                     "slug": ExaParserConfig["global"]["project_slug"],
-                    "owner.slug": ExaParserConfig["global"]["owner_slug"]
+                    "owner.slug": ExaParserConfig["global"]["owner_slug"],
                 }
             )[0]
         return self._project
 
     def create_structures(self, job):
         """
         Creates initial/final structures in web application.
@@ -91,21 +91,23 @@
             config["initial"]["owner"] = self.owner
             config["initial"]["tags"] = ["external"]
             structures.append(config)
 
         if not len(structures):
             return []
         headers = self.material_endpoints.headers
-        data = json.dumps({
-            "jobId": job["_id"],
-            "structures": structures,
-            "unitId": job["workflow"]["subworkflows"][0]["units"][0]["flowchartId"],
-        })
+        data = json.dumps(
+            {
+                "jobId": job["_id"],
+                "structures": structures,
+                "unitId": job["workflow"]["subworkflows"][0]["units"][0]["flowchartId"],
+            }
+        )
 
-        return self.material_endpoints.request('POST', "structures/", headers=headers, data=data)
+        return self.material_endpoints.request("POST", "structures/", headers=headers, data=data)
 
     def create_job(self):
         """
         Creates job in web application.
 
         Note: job must be set as external (isExternal=True) to be able to access the files.
 
@@ -182,15 +184,15 @@
             job_id (str): job ID.
         """
         for config in self.job.stdout_files:
             output_chunks_count = 0
             file_descriptor = open(config["stdoutFile"])
             while True:
                 chunk = file_descriptor.read(OUTPUT_CHUNK_SIZE)
-                if chunk != '':
+                if chunk != "":
                     data = {
                         "chunk": chunk,
                         "repetition": 0,
                         "order": output_chunks_count,
                         "unitFlowchartId": config["unitFlowchartId"],
                     }
                     self.job_endpoints.insert_output_files(id_=job_id, data=json.dumps(data))
```

### Comparing `exaparser-2023.6.16.post0/exaparser/enums.py` & `exaparser-2023.6.20.post0/exaparser/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 00000000: 4553 5052 4553 534f 5f45 5845 4355 5441  ESPRESSO_EXECUTA
 00000010: 424c 455f 4e41 4d45 5f52 4547 4558 203d  BLE_NAME_REGEX =
-00000020: 2072 275c 732b 5072 6f67 7261 6d20 282e   r'\s+Program (.
+00000020: 2072 225c 732b 5072 6f67 7261 6d20 282e   r"\s+Program (.
 00000030: 2a29 2076 2e2a 2073 7461 7274 7320 6f6e  *) v.* starts on
-00000040: 202e 2a27 0a45 5350 5245 5353 4f5f 494e   .*'.ESPRESSO_IN
+00000040: 202e 2a22 0a45 5350 5245 5353 4f5f 494e   .*".ESPRESSO_IN
 00000050: 5055 545f 4649 4c45 5f52 4547 4558 203d  PUT_FILE_REGEX =
-00000060: 2072 2726 434f 4e54 524f 4c7c 2653 5953   r'&CONTROL|&SYS
+00000060: 2072 2226 434f 4e54 524f 4c7c 2653 5953   r"&CONTROL|&SYS
 00000070: 5445 4d7c 2645 4c45 4354 524f 4e53 7c26  TEM|&ELECTRONS|&
 00000080: 494f 4e53 7c26 4345 4c4c 7c26 4241 4e44  IONS|&CELL|&BAND
 00000090: 537c 2649 4e50 5554 7c26 5052 4f4a 5746  S|&INPUT|&PROJWF
-000000a0: 437c 2644 4f53 7c27 0a0a 4553 5052 4553  C|&DOS|'..ESPRES
+000000a0: 437c 2644 4f53 7c22 0a0a 4553 5052 4553  C|&DOS|"..ESPRES
 000000b0: 534f 5f45 5845 4355 5441 424c 455f 4e41  SO_EXECUTABLE_NA
 000000c0: 4d45 5f4d 4150 203d 207b 0a20 2020 2022  ME_MAP = {.    "
 000000d0: 5057 5343 4622 3a20 2270 772e 7822 2c0a  PWSCF": "pw.x",.
 000000e0: 2020 2020 2242 414e 4453 223a 2022 6261      "BANDS": "ba
 000000f0: 6e64 732e 7822 2c0a 2020 2020 224d 4154  nds.x",.    "MAT
 00000100: 4459 4e22 3a20 226d 6174 6479 6e2e 7822  DYN": "matdyn.x"
 00000110: 2c0a 2020 2020 2244 594e 4d41 5422 3a20  ,.    "DYNMAT":
```

### Comparing `exaparser-2023.6.16.post0/exaparser/job/__init__.py` & `exaparser-2023.6.20.post0/exaparser/job/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,18 +49,20 @@
 
         Returns:
              list[dict]
         """
         stdout_files = []
         for unit in self.workflow.execution_units:
             if os.path.exists(unit.stdout_file):
-                stdout_files.append({
-                    "stdoutFile": unit.stdout_file,
-                    "unitFlowchartId": unit.flowchartId,
-                })
+                stdout_files.append(
+                    {
+                        "stdoutFile": unit.stdout_file,
+                        "unitFlowchartId": unit.flowchartId,
+                    }
+                )
         return stdout_files
 
     @property
     def status(self):
         """
         Returns job status.
         Status is set to "error" if there is a unit in "error" status.
@@ -102,19 +104,15 @@
         """
         Returns the job in JSON format.
 
         Returns:
              dict
         """
         return {
-            "_project": {
-                "slug": ExaParserConfig["global"]["project_slug"]
-            },
+            "_project": {"slug": ExaParserConfig["global"]["project_slug"]},
             "compute": self.compute.to_json(),
-            "owner": {
-                "slug": ExaParserConfig["global"]["owner_slug"]
-            },
+            "owner": {"slug": ExaParserConfig["global"]["owner_slug"]},
             "name": self.name,
             "status": self.status,
             "workDir": self.work_dir,
-            "workflow": self.workflow.to_json()
+            "workflow": self.workflow.to_json(),
         }
```

### Comparing `exaparser-2023.6.16.post0/exaparser/job/compute/__init__.py` & `exaparser-2023.6.20.post0/exaparser/job/compute/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,13 +50,8 @@
 
         Returns:
              int
         """
         return "01:00:00"
 
     def to_json(self):
-        return {
-            "ppn": self.ppn,
-            "nodes": self.nodes,
-            "queue": self.queue,
-            "timeLimit": self.walltime
-        }
+        return {"ppn": self.ppn, "nodes": self.nodes, "queue": self.queue, "timeLimit": self.walltime}
```

### Comparing `exaparser-2023.6.16.post0/exaparser/templates/espresso.json` & `exaparser-2023.6.20.post0/exaparser/templates/espresso.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/exaparser/templates/shell.json` & `exaparser-2023.6.20.post0/exaparser/templates/shell.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/exaparser/templates/vasp.json` & `exaparser-2023.6.20.post0/exaparser/templates/vasp.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/exaparser/utils.py` & `exaparser-2023.6.20.post0/exaparser/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,12 +87,12 @@
 
     Args:
         file_ (dict): a dictionary with path and presignedURL keys.
     """
     path = file_["path"]
     session = requests.Session()
     if os.path.getsize(path) == 0:
-        with open(path, 'w+') as f:
-            f.write('\n')
+        with open(path, "w+") as f:
+            f.write("\n")
     headers = {"Content-Length": str(os.path.getsize(path))}
     with open(path) as f:
         session.request("PUT", file_["URL"], data=f, headers=headers).raise_for_status()
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/subworkflow.py` & `exaparser-2023.6.20.post0/exaparser/workflow/subworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,9 +82,9 @@
         """
         return {
             "_id": self.id,
             "name": self.name,
             "model": self.model,
             "properties": [],
             "application": self.application,
-            "units": [u.to_json() for u in self.units]
+            "units": [u.to_json() for u in self.units],
         }
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/__init__.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
              dict
         """
         return {
             "flowchartId": self.flowchartId,
             "name": self.name,
             "head": self.head,
             "type": self.type,
-            "next": self.next_flowchartId
+            "next": self.next_flowchartId,
         }
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/execution/__init__.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/execution/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def __init__(self, config, work_dir):
         super(BaseExecutionUnit, self).__init__(config, work_dir)
         self.work_dir = os.path.join(self.work_dir, self.config.get("workDir", ""))
 
     @property
     def stdout_file(self):
-        return os.path.join(self.work_dir, self.config.get("stdoutFile", '.'.join((self.name, 'out'))))
+        return os.path.join(self.work_dir, self.config.get("stdoutFile", ".".join((self.name, "out"))))
 
     @property
     def application(self):
         """
         Returns the application used in the unit.
         Override upon inheritance.
 
@@ -62,19 +62,21 @@
 
         Returns:
              list[dict]
         """
         input_ = []
         for config in self.config.get("input", []):
             path_ = os.path.join(self.work_dir, config["name"])
-            input_.append({
-                "name": config["name"],
-                "isManuallyChanged": True,
-                "rendered": read(path_) if os.path.exists(path_) else ""
-            })
+            input_.append(
+                {
+                    "name": config["name"],
+                    "isManuallyChanged": True,
+                    "rendered": read(path_) if os.path.exists(path_) else "",
+                }
+            )
         return input_
 
     @property
     def postProcessors(self):
         """
         Returns a list of postProcessors used in the unit.
         Override upon inheritance as necessary.
@@ -99,27 +101,29 @@
         """
         Returns the unit in JSON format.
 
         Returns:
              dict
         """
         config = super(BaseExecutionUnit, self).to_json()
-        config.update({
-            "application": self.application,
-            "executable": self.executable,
-            "input": self.input,
-            "monitors": self.monitors,
-            "name": self.name,
-            "postProcessors": self.postProcessors,
-            "preProcessors": self.preProcessors,
-            "results": self.results,
-            "type": "execution",
-            "status": self.status,
-            "statusTrack": self.status_track,
-        })
+        config.update(
+            {
+                "application": self.application,
+                "executable": self.executable,
+                "input": self.input,
+                "monitors": self.monitors,
+                "name": self.name,
+                "postProcessors": self.postProcessors,
+                "preProcessors": self.preProcessors,
+                "results": self.results,
+                "type": "execution",
+                "status": self.status,
+                "statusTrack": self.status_track,
+            }
+        )
         return config
 
     @property
     def status(self):
         """
         Returns unit status.
 
@@ -134,20 +138,15 @@
     def status_track(self):
         """
         Returns unit status track.
 
         Returns:
              list[dict]
         """
-        return [
-            {
-                "trackedAt": int(os.path.getmtime(self.work_dir)),
-                "status": self.status
-            }
-        ]
+        return [{"trackedAt": int(os.path.getmtime(self.work_dir)), "status": self.status}]
 
     @property
     def results(self):
         """
         Returns a list of property names extracted from the unit.
 
         Returns:
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/execution/modeling/__init__.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/execution/modeling/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         Returns:
              dict
         """
         try:
             express = ExPrESS(self.parser_name, **dict(work_dir=self.work_dir, stdout_file=self.stdout_file))
             return express.property(property_, *args, **kwargs)
-        except:
+        except Exception:
             pass
 
     @property
     def initial_structures(self):
         """
         Safely returns a list of initial structures used in this unit.
 
@@ -46,15 +46,15 @@
         structures = []
         try:
             express = ExPrESS(self.parser_name, **dict(work_dir=self.work_dir, stdout_file=self.stdout_file))
             for structure_string in express.parser.initial_structure_strings():
                 initial_structure = express.property("material", structure_string=structure_string)
                 initial_structure["name"] = "initial_structure"
                 structures.append(initial_structure)
-        except:
+        except Exception:
             pass
         return structures
 
     @property
     def final_structures(self):
         """
         Safely returns a list of final structures generated in this unit.
@@ -66,15 +66,15 @@
         try:
             express = ExPrESS(self.parser_name, **dict(work_dir=self.work_dir, stdout_file=self.stdout_file))
             for structure_string in express.parser.final_structure_strings():
                 final_structure = express.property("material", structure_string=structure_string)
                 final_structure["name"] = "final_structure"
                 final_structure["repetition"] = 0
                 structures.append(final_structure)
-        except:
+        except Exception:
             pass
         return structures
 
     @property
     def structures(self):
         """
         Returns a list of structure pairs (initial/final) extracted from the unit.
@@ -82,18 +82,15 @@
         Returns:
              list[dict]
         """
         structures = []
         final_structures = self.final_structures
         initial_structures = self.initial_structures
         for index, structure in enumerate(initial_structures):
-            structures.append({
-                "initial": structure,
-                "final": final_structures[index]
-            })
+            structures.append({"initial": structure, "final": final_structures[index]})
         return structures
 
     @property
     def properties(self):
         """
         Returns a list of properties in EDC format extracted from the unit.
 
@@ -103,17 +100,11 @@
         properties = []
         for name in [r["name"] for r in self.results]:
             if name == "final_structure":
                 continue
             property_ = self.safely_extract_property(name)
             if property_:
                 property_.update({"repetition": 0})
-                properties.append({
-                    "data": property_,
-                    "source": {
-                        "type": "exabyte",
-                        "info": {
-                            "unitId": self.flowchartId
-                        }
-                    }
-                })
+                properties.append(
+                    {"data": property_, "source": {"type": "exabyte", "info": {"unitId": self.flowchartId}}}
+                )
         return properties
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/execution/modeling/espresso.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/execution/modeling/espresso.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import re
 import xml.etree.ElementTree as ET
 
 from express.parsers.apps.espresso.settings import XML_DATA_FILE as ESPRESSO_XML_FILE
 
-from exaparser.enums import *
+from exaparser.enums import (
+    ESPRESSO_SUPPORTED_VERSIONS,
+    ESPRESSO_DEFAULT_VERSION,
+    ESPRESSO_EXECUTABLE_NAME_MAP,
+    ESPRESSO_EXECUTABLE_NAME_REGEX,
+)
 from exaparser.utils import find_file
 from . import ModelingExecutionUnit
 
 
 class EspressoExecutionUnit(ModelingExecutionUnit):
     """
     Espresso execution unit parser class.
@@ -36,37 +41,31 @@
         """
         Returns the application version used in the unit.
 
         Returns:
              str
         """
         root = ET.parse(self.xml_path).getroot()
-        version = root.find('HEADER').find("CREATOR").attrib.get("VERSION").strip()
+        version = root.find("HEADER").find("CREATOR").attrib.get("VERSION").strip()
         return version if version in ESPRESSO_SUPPORTED_VERSIONS else ESPRESSO_DEFAULT_VERSION
 
     @property
     def application(self):
         """
         Returns the application used in the unit.
 
         Returns:
              dict
         """
-        return {
-            "name": "espresso",
-            "version": self.version,
-            "summary": "Quantum Espresso"
-        }
+        return {"name": "espresso", "version": self.version, "summary": "Quantum Espresso"}
 
     @property
     def executable(self):
         """
         Returns the executable used in the unit.
 
         Returns:
              dict
         """
         with open(self.stdout_file) as f:
             executable = ESPRESSO_EXECUTABLE_NAME_MAP[re.findall(ESPRESSO_EXECUTABLE_NAME_REGEX, f.read())[0]]
-            return {
-                "name": executable
-            }
+            return {"name": executable}
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/execution/modeling/vasp.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/execution/modeling/vasp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import xml.etree.ElementTree as ET
 
 from express.parsers.apps.vasp.settings import XML_DATA_FILE as VASP_XML_FILE
 
-from exaparser.enums import *
+from exaparser.enums import VASP_SUPPORTED_VERSIONS, VASP_DEFAULT_VERSION
 from exaparser.utils import find_file
 from . import ModelingExecutionUnit
 
 
 class VaspExecutionUnit(ModelingExecutionUnit):
     """
     Vasp execution unit parser class.
@@ -34,36 +34,30 @@
     def application(self):
         """
         Returns the application used in the unit.
 
         Returns:
              dict
         """
-        return {
-            "name": "vasp",
-            "version": self.version,
-            "summary": "Vienna Ab-initio Simulation Package"
-        }
+        return {"name": "vasp", "version": self.version, "summary": "Vienna Ab-initio Simulation Package"}
 
     @property
     def version(self):
         """
         Returns the application version used in the unit.
 
         Returns:
              str
         """
         root = ET.parse(self.xml_path).getroot()
-        version = root.find('generator').find('.//i[@name="version"]').text.strip()
+        version = root.find("generator").find('.//i[@name="version"]').text.strip()
         return version if version in VASP_SUPPORTED_VERSIONS else VASP_DEFAULT_VERSION
 
     @property
     def executable(self):
         """
         Returns the executable used in the unit.
 
         Returns:
              dict
         """
-        return {
-            "name": "vasp"
-        }
+        return {"name": "vasp"}
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/execution/scripting/shell.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/execution/scripting/shell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from exaparser.enums import *
+from exaparser.enums import SHELL_DEFAULT_VERSION
 from . import ScriptingExecutionUnit
 
 
 class ShellExecutionUnit(ScriptingExecutionUnit):
     """
     Shell unit parser class.
 
@@ -18,19 +18,15 @@
     def application(self):
         """
         Returns the application used in the unit.
 
         Returns:
              dict
         """
-        return {
-            "name": "shell",
-            "summary": "Shell Script",
-            "version": self.version
-        }
+        return {"name": "shell", "summary": "Shell Script", "version": self.version}
 
     @property
     def version(self):
         """
         Returns the application version used in the unit.
 
         Returns:
@@ -42,10 +38,8 @@
     def executable(self):
         """
         Returns the executable used in the unit.
 
         Returns:
              dict
         """
-        return {
-            "name": "sh"
-        }
+        return {"name": "sh"}
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from express.parsers.apps.espresso.settings import XML_DATA_FILE as ESPRESSO_XML_FILE
 from express.parsers.apps.vasp.settings import XML_DATA_FILE as VASP_XML_FILE
 
 from exaparser.utils import find_file, find_file_with_pattern
-from .shell import ShellExecutionUnit, ESPRESSO_INPUT_FILE_REGEX
+from exaparser.enums import ESPRESSO_INPUT_FILE_REGEX
+from .shell import ShellExecutionUnit
 from ..modeling import ModelingExecutionUnit
 
 
 class ShellWithResultsExecutionUnit(ShellExecutionUnit, ModelingExecutionUnit):
     """
     Shell unit parser class.
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/factory.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/factory.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/units/subworkflow.py` & `exaparser-2023.6.20.post0/exaparser/workflow/units/subworkflow.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,11 +18,9 @@
         """
         Returns the subworkflow unit in JSON format.
 
         Returns:
              dict
         """
         config = super(SubworkflowUnit, self).to_json()
-        config.update({
-            "_id": self.id
-        })
+        config.update({"_id": self.id})
         return config
```

### Comparing `exaparser-2023.6.16.post0/exaparser/workflow/workflow.py` & `exaparser-2023.6.20.post0/exaparser/workflow/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,9 +48,9 @@
              dict
         """
         return {
             "name": self.name,
             "properties": [],
             "units": [u.to_json() for u in self.units],
             "subworkflows": [u.to_json() for u in self.subworkflows],
-            "isMultiMaterial": True  # to let job have multiple materials
+            "isMultiMaterial": True,  # to let job have multiple materials
         }
```

### Comparing `exaparser-2023.6.16.post0/exaparser.egg-info/PKG-INFO` & `exaparser-2023.6.20.post0/exaparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exaparser
-Version: 2023.6.16.post0
+Version: 2023.6.20.post0
 Summary: Exabyte Parser
 Home-page: https://github.com/Exabyte-io/exaparser
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
```

### Comparing `exaparser-2023.6.16.post0/exaparser.egg-info/SOURCES.txt` & `exaparser-2023.6.20.post0/exaparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/requirements-dev.txt` & `exaparser-2023.6.20.post0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/requirements.txt` & `exaparser-2023.6.20.post0/requirements.txt`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/run-tests.sh` & `exaparser-2023.6.20.post0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/setup.cfg` & `exaparser-2023.6.20.post0/setup.cfg`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/__init__.py` & `exaparser-2023.6.20.post0/tests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         Notes:
             Based on: http://stackoverflow.com/a/23550280
 
         Args:
             expected (dict|list|tuple): expected complex object.
             actual (dict|list|tuple): actual complex object.
         """
-        is_root = '__trace' not in kwargs
-        trace = kwargs.pop('__trace', 'ROOT')
+        is_root = "__trace" not in kwargs
+        trace = kwargs.pop("__trace", "ROOT")
         try:
             if isinstance(expected, (int, float, complex)):
                 self.assertAlmostEqual(expected, actual, *args, **kwargs)
             elif isinstance(expected, (str)):
                 self.assertEqual(expected, actual)
             elif isinstance(expected, (list, tuple, np.ndarray)):
                 self.assertEqual(len(expected), len(actual))
@@ -40,12 +40,12 @@
                     v1, v2 = expected[index], actual[index]
                     self.assertDeepAlmostEqual(v1, v2, __trace=repr(index), *args, **kwargs)
             elif isinstance(expected, dict):
                 self.assertEqual(set(expected), set(actual))
                 for key in expected:
                     self.assertDeepAlmostEqual(expected[key], actual[key], __trace=repr(key), *args, **kwargs)
         except AssertionError as exc:
-            exc.__dict__.setdefault('traces', []).append(trace)
+            exc.__dict__.setdefault("traces", []).append(trace)
             if is_root:
-                trace = ' -> '.join(reversed(exc.traces))
+                trace = " -> ".join(reversed(exc.traces))
                 exc = AssertionError("%s\nTRACE: %s" % (str(exc), trace))
             raise exc
```

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/shell-job.json` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/shell-job.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/pw-scf.in` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/pw-scf.in`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/espresso/test-001/stdout` & `exaparser-2023.6.20.post0/tests/fixtures/espresso/test-001/stdout`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/shell-job.json` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/shell-job.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/CONTCAR` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/CONTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/DOSCAR` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/DOSCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/EIGENVAL` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/EIGENVAL`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/OSZICAR` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/OSZICAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/OUTCAR` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/OUTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/POTCAR` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/POTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/stdout` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/stdout`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/fixtures/vasp/test-001/vasprun.xml` & `exaparser-2023.6.20.post0/tests/fixtures/vasp/test-001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.6.16.post0/tests/integration/test_job.py` & `exaparser-2023.6.20.post0/tests/integration/test_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from exaparser.job import Job
 from exaparser.utils import read_json
 from tests.enums import FIXTURES_DIR
 from tests.integration import IntegrationTestBase
 
 
 class TestJobParser(IntegrationTestBase):
-
     def setUp(self):
         super(TestJobParser, self).setUp()
 
     def tearDown(self):
         super(TestJobParser, self).setUp()
 
     def _clean_job_config(self, config):
```

