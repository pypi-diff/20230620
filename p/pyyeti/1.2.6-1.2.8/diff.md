# Comparing `tmp/pyyeti-1.2.6.tar.gz` & `tmp/pyyeti-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyeti-1.2.6.tar", last modified: Sat May 20 21:53:54 2023, max compression
+gzip compressed data, was "pyyeti-1.2.8.tar", last modified: Mon Jun 19 22:33:01 2023, max compression
```

## Comparing `pyyeti-1.2.6.tar` & `pyyeti-1.2.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.474276 pyyeti-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-20 21:53:38.000000 pyyeti-1.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-20 21:53:38.000000 pyyeti-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-20 21:53:54.474276 pyyeti-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-20 21:53:38.000000 pyyeti-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.470275 pyyeti-1.2.6/pyyeti/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   106717 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.470275 pyyeti-1.2.6/pyyeti/cla/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/_magpct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/_rptext1.py
--rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/_rptpct1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/_rpttab1.py
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    50972 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/dr_def.py
--rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/dr_event.py
--rw-r--r--   0 runner    (1001) docker     (123)   111221 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/dr_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/dr_results_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cla/rel_disp_dtm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/column_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/cyclecount.py
--rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/datacursor.py
--rw-r--r--   0 runner    (1001) docker     (123)   124529 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    49094 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/era.py
--rw-r--r--   0 runner    (1001) docker     (123)    42901 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/expmint.py
--rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/fdepsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/frclim.py
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/guitools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/locate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.474276 pyyeti-1.2.6/pyyeti/nastran/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/nastran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131608 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/nastran/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)   136601 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/nastran/n2p.py
--rw-r--r--   0 runner    (1001) docker     (123)   120906 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/nastran/op2.py
--rw-r--r--   0 runner    (1001) docker     (123)    91322 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/nastran/op4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.474276 pyyeti-1.2.6/pyyeti/ode/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/_base_ode_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/freqdirect.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/frf_mode_participation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/solvecdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/solveexp1.py
--rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/solveexp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/solvenewmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    69128 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ode/solveunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/pp.py
--rw-r--r--   0 runner    (1001) docker     (123)    42978 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/psd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.474276 pyyeti-1.2.6/pyyeti/rainflow/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/rainflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/rainflow/c_rain.c
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/rainflow/py_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)    74708 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/srs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ssmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    56785 2023-05-20 21:53:38.000000 pyyeti-1.2.6/pyyeti/ytools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.470275 pyyeti-1.2.6/pyyeti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-20 21:53:54.000000 pyyeti-1.2.6/pyyeti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-20 21:53:54.000000 pyyeti-1.2.6/pyyeti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 21:53:54.000000 pyyeti-1.2.6/pyyeti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-20 21:53:54.000000 pyyeti-1.2.6/pyyeti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 21:53:54.000000 pyyeti-1.2.6/pyyeti.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.474276 pyyeti-1.2.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-05-20 21:53:38.000000 pyyeti-1.2.6/scripts/lsop2
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-05-20 21:53:38.000000 pyyeti-1.2.6/scripts/lsop4
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-20 21:53:54.474276 pyyeti-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-20 21:53:38.000000 pyyeti-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.466276 pyyeti-1.2.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.474276 pyyeti-1.2.6/tests/nas2cam_csuper/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nas2cam_csuper/inboard.asm
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nas2cam_csuper/inboard.op4
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nas2cam_csuper/inboard.pch
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nas2cam_csuper/nas2cam.op2
--rw-r--r--   0 runner    (1001) docker     (123)   147552 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nas2cam_csuper/nas2cam.op4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:53:54.474276 pyyeti-1.2.6/tests/nastran_drm12/
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nastran_drm12/drm12.op2
--rw-r--r--   0 runner    (1001) docker     (123)    77852 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nastran_drm12/drm12.op4
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nastran_drm12/inboard_nas2cam.op2
--rw-r--r--   0 runner    (1001) docker     (123)    51624 2023-05-20 21:53:38.000000 pyyeti-1.2.6/tests/nastran_drm12/inboard_nas2cam.op4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-19 22:32:39.000000 pyyeti-1.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-19 22:32:39.000000 pyyeti-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-19 22:33:01.885629 pyyeti-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-19 22:32:39.000000 pyyeti-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.881629 pyyeti-1.2.8/pyyeti/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106717 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/cla/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_magpct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_rptext1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_rptpct1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_rpttab1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50944 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111221 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/dr_results_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cla/rel_disp_dtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/column_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/cyclecount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/datacursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124529 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69230 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/era.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42901 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/expmint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29531 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/fdepsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/frclim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/guitools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/locate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/nastran/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131608 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136601 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/n2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120906 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/op2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91322 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/nastran/op4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/_base_ode_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/freqdirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/frf_mode_participation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solvecdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solveexp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solveexp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solvenewmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69302 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ode/solveunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42978 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/psd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/pyyeti/rainflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/rainflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/rainflow/c_rain.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/rainflow/py_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74708 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/srs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ssmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56785 2023-06-19 22:32:39.000000 pyyeti-1.2.8/pyyeti/ytools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.881629 pyyeti-1.2.8/pyyeti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 22:33:01.000000 pyyeti-1.2.8/pyyeti.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-06-19 22:32:39.000000 pyyeti-1.2.8/scripts/lsop2
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-06-19 22:32:39.000000 pyyeti-1.2.8/scripts/lsop4
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-19 22:33:01.889629 pyyeti-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-19 22:32:39.000000 pyyeti-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.881629 pyyeti-1.2.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/tests/nas2cam_csuper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/inboard.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/inboard.op4
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/inboard.pch
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op2
+-rw-r--r--   0 runner    (1001) docker     (123)   147552 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:33:01.885629 pyyeti-1.2.8/tests/nastran_drm12/
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/drm12.op2
+-rw-r--r--   0 runner    (1001) docker     (123)    77852 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/drm12.op4
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op2
+-rw-r--r--   0 runner    (1001) docker     (123)    51624 2023-06-19 22:32:39.000000 pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op4
```

### Comparing `pyyeti-1.2.6/LICENSE.txt` & `pyyeti-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/PKG-INFO` & `pyyeti-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.2.6
+Version: 1.2.8
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.2.6 Summary: Tools mostly related
+Metadata-Version: 2.1 Name: pyyeti Version: 1.2.8 Summary: Tools mostly related
 to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
 Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: C
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `pyyeti-1.2.6/README.md` & `pyyeti-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/__init__.py` & `pyyeti-1.2.8/pyyeti/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cb.py` & `pyyeti-1.2.8/pyyeti/cb.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/_magpct.py` & `pyyeti-1.2.8/pyyeti/cla/_magpct.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/_rptext1.py` & `pyyeti-1.2.8/pyyeti/cla/_rptext1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/_rptpct1.py` & `pyyeti-1.2.8/pyyeti/cla/_rptpct1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/_rpttab1.py` & `pyyeti-1.2.8/pyyeti/cla/_rpttab1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/_utilities.py` & `pyyeti-1.2.8/pyyeti/cla/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/dr_def.py` & `pyyeti-1.2.8/pyyeti/cla/dr_def.py`

 * *Files 1% similar despite different names*

```diff
@@ -689,19 +689,19 @@
         :func:`DR_Event.set_dr_order` can be used to modify the final
         order. That routine uses the more general
         :func:`.pyyeti.ytools.reorder_dict` to reorder the
         categories.
 
         **Entering partition vectors.** The `histpv`, `srspv` and
         `ignorepv` inputs are all handled similarly. They can be input
-        as either an index or boolean style partition vector. If input
-        as 'all', they are reset internally to ``slice(len(labels))``.
-        They can also be entered as a slice directly. The stored
-        versions are either a slice or an index vector (uses 0-offset
-        for standard Python indexing).
+        as an index or boolean style partition vector, as a slice, or
+        as "all". If input as 'all', they are reset internally to
+        ``slice(len(labels))``. The stored versions are either a slice
+        or an index vector (uses 0-offset for standard Python
+        indexing).
 
         **`drfunc`, `drfile` notes.** If `drfunc` is a valid Python
         identifier (called "Type 2" above), then `drfile` must contain
         the appropriate data recovery function(s) named ``name`` and,
         optionally, ``name_psd``. For a typical data recovery
         category, only one data recovery function would be
         needed. Here are some examples:
```

### Comparing `pyyeti-1.2.6/pyyeti/cla/dr_event.py` & `pyyeti-1.2.8/pyyeti/cla/dr_event.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/dr_results.py` & `pyyeti-1.2.8/pyyeti/cla/dr_results.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/dr_results_plots.py` & `pyyeti-1.2.8/pyyeti/cla/dr_results_plots.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cla/rel_disp_dtm.py` & `pyyeti-1.2.8/pyyeti/cla/rel_disp_dtm.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/column_plotter.py` & `pyyeti-1.2.8/pyyeti/column_plotter.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/cyclecount.py` & `pyyeti-1.2.8/pyyeti/cyclecount.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,39 +49,41 @@
         `rf` is returned.
     use_pandas : bool; optional
         If True, this routine will return pandas DataFrames
 
     Returns
     -------
     rf : pandas DataFrame or 2d ndarray
-
         n x 3 matrix with the rainflow cycle count information with
         the index going from 0 to n-1 and the columns being ['amp',
         'mean', 'count']:
 
             - amp is the cycle amplitude (half the peak-to-peak range)
             - mean is mean of the cycle
             - count is either 0.5 or 1.0 depending on whether it's
               half or full cycle
 
     os : pandas DataFrame or 2d ndarray
-
         Only returned if `getoffsets` is True. n x 2 matrix of cycle
         offsets with index going from 0 to n-1 and the columns being
         ['start', 'stop']:
 
             - start is the offset into `peaks` for start of cycle
             - stop is the offset into `peaks` for end of cycle
 
     Notes
     -----
     This algorithm is derived from reference [#cc1]_. This routine is
-    a wrapper for either the :func:`pyyeti.rainflow.c_rain` or
-    :func:`pyyeti.rainflow.py_rain` routines. Note that the C version
-    is *much* faster (the algorithms are the same).
+    a wrapper for either the C version
+    (:func:`pyyeti.rainflow.c_rain`) or the Python version
+    (:func:`pyyeti.rainflow.py_rain`) of the algorithm. Both versions
+    give identical results. They also run in comparable times if
+    :func:`numba.jit` is available (if ``import numba`` works). If
+    :func:`numba.jit` is not available, the C version is *much*
+    faster.
 
     References
     ----------
     .. [#cc1] "Standard Practices for Cycle Counting in Fatigue
            Analysis", ASTM E 1049 - 85 (Reapproved 2005).
 
     Examples
@@ -240,15 +242,14 @@
 
         # expand to full size:
         PV = np.zeros(y.size, bool)  # non-uniques are not peaks
         PV[u] = pv
         # [ True, False, False,  True, False,  True, False, False]
         return PV
 
-
 else:
 
     def findap(y, tol=1e-6):
         """
         Find alternating local maximum and minimum points in a vector.
 
         Parameters
@@ -491,15 +492,14 @@
         for v in x[1:]:
             if v > mx:
                 mx = v
             elif v < mn:
                 mn = v
         return mx, mn
 
-
 else:
 
     def maxmin(x):
         return x.max(), x.min()
 
 
 def binify(
@@ -700,17 +700,17 @@
     meanbins : 1d ndarray
         Boundaries of mean-value bins used; length = # of bins + 1.
         Only returned if `retbins` is True.
 
     Notes
     -----
     Steps:
-      1.  calls :func:`findap` to find all local minima and maxima:
+      1.  Calls :func:`findap` to find all local minima and maxima:
           ``peaks = sig[findap(sig)]``
-      2.  calls :func:`rainflow` to do the cycle counting:
+      2.  Calls :func:`rainflow` to do the cycle counting:
           ``rf = rainflow(peaks)``
       3.  Summarizes the rainflow counting by putting the counts in
           bins. For each mean value bin (i'th):
 
           a. `rf` is filtered down to only those rows where the mean
              value falls in the mean-bin (call this subset of `rf`
              `rffilt`).
```

### Comparing `pyyeti-1.2.6/pyyeti/datacursor.py` & `pyyeti-1.2.8/pyyeti/datacursor.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/dsp.py` & `pyyeti-1.2.8/pyyeti/dsp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/era.py` & `pyyeti-1.2.8/pyyeti/era.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,28 +3,48 @@
 The Eigensystem Realization Algorithm
 
 Identify mode shapes, frequencies, and damping from free-decay
 measurement data.
 """
 # Python ERA class written by Natalie Hintz and Tim Widrick.
 
+import sys
 import re
 import numpy as np
 import scipy.linalg as la
-from pyyeti import ode, dsp
+from scipy import signal, fft
+from pyyeti import ode, dsp, writer
 import matplotlib.pyplot as plt
 import numbers
 from warnings import warn
 
 
 def _string_to_ints(string):
     """
     Convert "1, 2 5" to np.array([0, 1, 4])
     """
-    return np.array([int(i) - 1 for i in re.split("[, ]+", string)])
+    ints = []
+    for substring in re.split("[, ]+", string):
+        if "-" in substring:
+            a, b = substring.split("-")
+            ints += list(range(int(a), int(b) + 1))
+        else:
+            ints.append(int(substring))
+    return np.array(ints) - 1
+    # return np.array([int(i) - 1 for i in re.split("[, ]+", string)])
+
+
+def _string_to_ints2(string):
+    """
+    Convert Python expression to ndarray or "1, 2 5" to np.array([0,
+    1, 4])
+    """
+    if string[0].isdigit():
+        return _string_to_ints(string)
+    return np.atleast_1d(eval(string)).astype(int) - 1
 
 
 class ERA:
     """
     Implements the Eigensystem Realization Algorithm (ERA).
 
     ERA follows minimum realization theory to identify modal
@@ -101,33 +121,66 @@
         Jupyter notebook at the top of the tutorial.
 
     Mode indicators:
 
         =========  ===================================================
         Indicator  Description
         =========  ===================================================
-           MSV     Normalized mode singular value. The MSV value
+          MSV      Normalized mode singular value. The MSV value
                    ranges from 0.0 to 1.0 for each mode and is a
                    measure of contribution to the response. Larger
                    values represent larger contribution.
           EMAC     Extended modal amplitude coherence. The EMAC value
                    ranges from 0.0 to 1.0 for each mode and is a
-                   temporal measure indicating the importance of the
+                   temporal measure indicating the consistency of the
                    mode over time to the fit. Higher values indicate
-                   more importance. From experience, the EMAC is
-                   superior to the MAC value (see below). For more
-                   information, see [#era2]_.
-           MPC     Modal phase collinearity. The MPC value ranges from
+                   higher consistency, meaning that the mode decays as
+                   expected. The EMAC is computed based on both
+                   observability (outputs) and controllability
+                   (inputs). From experience, the EMAC is superior to
+                   the MAC value (see below). For more information,
+                   see [#era2]_. See also `EMACO`.
+          EMACO    EMAC from just observability, as opposed to both
+                   observability and controllability. Reference
+                   [#era3]_ argues that this is more reliable than
+                   EMAC because there are typically more response
+                   measurements (observability side) than inputs
+                   (controllability side). This means we are relying
+                   on the mode shape matrix C, which is typically
+                   supported by many measurements, and not relying on
+                   the mode participation factors matrix B, which may
+                   be more sensitive to the particular excitation. As
+                   pointed out in [#era3]_, temporal consistency based
+                   on B is highly dependent on the choice of input
+                   locations, which may be too few for reliable
+                   results.
+
+                   .. note::
+                        Note: this algorithm does not use the equation
+                        in [#era3]_, which is a simple average of all
+                        EMAC values for a mode across all
+                        outputs. Instead, it uses a weighted average
+                        where the weighting factor for each output is
+                        the modeshape coefficient for that output (as
+                        done in [#era2]_).
+
+          MPC      Modal phase collinearity. The MPC value ranges from
                    0.0 to 1.0 for each mode and is a spatial measure
                    indicating whether or not the different response
                    locations for a mode are in phase. Higher values
                    indicate more "in-phase" measurements. Only useful
                    if there are multiple outputs (MPC is 1.0 for
-                   single output).
-           MAC     Modal amplitude coherence. The MAC value ranges
+                   single output). MPC will be 1.0 for a mode that is
+                   100% real (this happens when the real mode
+                   diagonalizes the damping). MPC is directly related
+                   to the "Modal Complexity Factor" (MCF): ``MPC = 1 -
+                   MCF``.
+          CMIO     Consistent mode indicator based on observability.
+                   ``CMIO = EMACO * MPC`` for each mode.
+          MAC      Modal amplitude coherence. The MAC value ranges
                    from 0.0 to 1.0 for each mode and is a temporal
                    measure indicating the importance of the mode over
                    time to the fit. Higher values indicate more
                    importance. The MAC value for a mode is the dot
                    product of two vectors:
 
                      1. The ideal, reconstructed time history for a
@@ -146,14 +199,19 @@
                Kingdom: Prentice Hall, 1994.
 
     .. [#era2] Richard S. Pappa, Kenny B. Elliott, Axel Schenk. "A
                Consistent-Mode Indicator for the Eigensystem
                Realization Algorithm", NASA Technical Memorandum
                107607, April 1992.
 
+    .. [#era3] Yun, G. J., Lee, S. G., & Shang, S. "An improved mode
+               accuracy indicator for Eigensystem Realization Analysis
+               (ERA) techniques", KSCE Journal of Civil Engineering,
+               16, 377-387, March 2012.
+
     Examples
     --------
     The following example demonstrates ERA by comparing to a known
     system.
 
     .. plot::
         :context: close-figs
@@ -228,113 +286,118 @@
         is a very good exercise to experiment with using each of them
         with this problem.
 
         >>> era_fit = era.ERA(
         ...     sol.v,
         ...     sr=1 / dt,
         ...     auto=True,
-        ...     input_labels=["x", "y", "z"],
-        ...     FFT=True,
-        ...     FFT_range=30.0,
         ... )
         <BLANKLINE>
         Current fit includes all modes:
-          Mode   Freq. (Hz)     Zeta        MSV      EMAC       MPC       MAC
-          --------------------------------------------------------------------
-        *    1     1.33603     0.02000    *0.817    *1.000    *1.000    *1.000
-        *    2     7.39083     0.07500    *0.839    *1.000    *1.000    *1.000
-        *    3    13.79671     0.05000    *1.000    *1.000    *1.000    *1.000
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+        *    1     1.3360    2.0000  *0.817  *1.000  *1.000  *1.000  *1.000  *1.000
+        *    2     7.3908    7.5000  *0.839  *1.000  *1.000  *1.000  *1.000  *1.000
+        *    3    13.7967    5.0000  *1.000  *1.000  *1.000  *1.000  *1.000  *1.000
         <BLANKLINE>
         Auto-selected modes fit:
-          Mode   Freq. (Hz)     Zeta        MSV      EMAC       MPC       MAC
-          --------------------------------------------------------------------
-             1     1.33603     0.02000     0.817     1.000     1.000     1.000
-             2     7.39083     0.07500     0.839     1.000     1.000     1.000
-             3    13.79671     0.05000     1.000     1.000     1.000     1.000
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+             1     1.3360    2.0000   0.817   1.000   1.000   1.000   1.000   1.000
+             2     7.3908    7.5000   0.839   1.000   1.000   1.000   1.000   1.000
+             3    13.7967    5.0000   1.000   1.000   1.000   1.000   1.000   1.000
 
-        Compare frequencies and damping:
+        Compare frequencies, damping, mode shapes:
 
         >>> np.allclose(era_fit.freqs_hz, freq_hz)
         True
         >>> np.allclose(era_fit.zeta, zeta)
         True
+        >>> era_fit.phi / phi  # modes will be scaled differently
+        array([[ 1.38989, -1.02337, -1.34712],
+               [ 1.38989, -1.02337, -1.34712],
+               [ 1.38989, -1.02337, -1.34712]])
 
     .. plot::
         :context: close-figs
 
         For demonstration, add some noise to the signal and rerun
         ERA. Note that while this example works out nicely for our
         known system, it will often be necessary to run ERA multiple
         times with different parameters and different response data
         selections to gain confidence in which modes are real.
 
+        For this run, we'll also add some labels and some FFT plots up
+        to 30.0 Hz.
+
         >>> np.random.seed(1)  # for repeatability
         >>> era_fit = era.ERA(
         ...     sol.v + 0.05 * np.random.randn(*sol.v.shape),
         ...     sr=1 / dt,
         ...     auto=True,
         ...     input_labels=["x", "y", "z"],
         ...     FFT=True,
         ...     FFT_range=30.0,
         ... )
         <BLANKLINE>
         Current fit includes all modes:
-          Mode   Freq. (Hz)     Zeta        MSV      EMAC       MPC       MAC
-          --------------------------------------------------------------------
-             1     0.73875     1.28293     0.256     0.013    *1.000    *1.000
-        *    2     1.37239     0.02610    *0.833    *0.927    *0.990    *1.000
-             3     4.61109     0.08532     0.268     0.098     0.588    *1.000
-             4     6.48926     0.58299     0.257     0.000     0.549    *1.000
-        *    5     7.39420     0.07075    *0.853    *0.955    *0.994    *1.000
-             6     9.54517     0.02778     0.203     0.124     0.007    *1.000
-             7    11.60875     0.02303     0.275     0.000    *0.825    *1.000
-        *    8    13.84752     0.05013    *1.000    *0.698    *0.997    *1.000
-             9    15.56279     0.01595     0.248     0.384     0.476    *1.000
-            10    17.63534    -0.01207     0.151     0.192     0.105    *1.000
-            11    20.28144     0.00245     0.264    *0.669    *0.952    *1.000
-            12    21.84685     0.02069     0.208     0.176     0.376    *1.000
-            13    24.08700     0.02537     0.258     0.141     0.584    *1.000
-            14    26.42550     0.01341     0.258     0.083     0.394    *1.000
-            15    28.37983     0.03076     0.232     0.001    *0.827    *1.000
-            16    29.67884     0.02676     0.279     0.036     0.116    *1.000
-            17    32.23488     0.01671     0.216     0.000     0.696    *1.000
-            18    34.27749     0.00929     0.296     0.204    *0.844    *1.000
-            19    36.09656     0.01530     0.274    *0.855     0.631    *1.000
-            20    38.51809     0.01280     0.232     0.179     0.129    *1.000
-            21    40.13913     0.03768     0.224     0.000     0.370    *1.000
-            22    42.11085     0.00934     0.247     0.001    *0.790    *1.000
-            23    44.01415     0.02820     0.264     0.000     0.189    *1.000
-            24    46.19429     0.01336     0.290     0.000     0.254    *1.000
-            25    48.18869     0.01835     0.252     0.162     0.041    *1.000
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+        *    1     1.3529    1.2530  *0.808  *0.890  *0.903  *0.998  *0.901  *1.000
+             2     4.1838   31.8458   0.212   0.025   0.055  *0.698   0.039  *0.880
+        *    3     7.3880    7.0198  *0.847  *0.832  *0.890  *0.989  *0.880  *1.000
+             4     9.6646    5.1517   0.190   0.017   0.057   0.018   0.001  *0.979
+             5    11.6655    2.5487   0.234   0.035   0.057  *0.519   0.030  *0.988
+        *    6    13.8372    5.1240  *1.000  *0.655  *0.682  *0.998  *0.681  *1.000
+             7    15.6667    6.0264   0.207   0.010   0.032   0.019   0.001  *0.897
+             8    17.3887    3.1272   0.157   0.000   0.001   0.457   0.000   0.679
+             9    20.5904    1.0665   0.203   0.317  *0.660  *0.850  *0.561  *0.929
+            10    24.3082    3.0689   0.203   0.024   0.093   0.187   0.017  *0.965
+            11    26.4615    2.0703   0.252   0.080   0.345   0.361   0.124  *0.958
+            12    29.5931    3.8058   0.244   0.031   0.150  *0.687   0.103  *0.967
+            13    34.2570    0.4488   0.260  *0.445   0.471  *0.864  *0.407  *0.992
+            14    36.0289    1.0712   0.246  *0.380   0.447  *0.763   0.341  *0.985
+            15    41.8090    1.3177   0.231   0.044   0.073   0.431   0.032  *0.904
+            16    44.3820    3.9816   0.207   0.004   0.035  *0.539   0.019  *0.878
+            17    47.1949    2.6987   0.221   0.001   0.003  *0.511   0.001  *0.961
+            18    48.7638    0.9036   0.171   0.000   0.000  *0.652   0.000  *0.912
         <BLANKLINE>
         Auto-selected modes fit:
-          Mode   Freq. (Hz)     Zeta        MSV      EMAC       MPC       MAC
-          --------------------------------------------------------------------
-             1     1.37239     0.02610     0.833     0.871     0.990     1.000
-             2     7.39420     0.07075     0.853     0.787     0.994     1.000
-             3    13.84752     0.05013     1.000     0.665     0.997     1.000
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+             1     1.3529    1.2530   0.808   0.890   0.903   0.998   0.901   1.000
+             2     7.3880    7.0198   0.847   0.832   0.890   0.989   0.880   1.000
+             3    13.8372    5.1240   1.000   0.655   0.682   0.998   0.681   1.000
     """
 
     def __init__(
         self,
         resp,
         sr,
         *,
-        svd_tol=0.01,
+        svd_tol=0.05,
         auto=False,
+        alpha=None,
+        beta=None,
         MSV_lower_limit=0.35,
-        EMAC_lower_limit=0.5,
-        MPC_lower_limit=0.7,
-        MAC_lower_limit=0.0,
+        EMAC_lower_limit=0.35,
+        EMACO_lower_limit=0.5,
+        MPC_lower_limit=0.5,
+        CMIO_lower_limit=0.35,
+        MAC_lower_limit=0.75,
+        all_lower_limits=None,
         damp_range=(0.001, 0.999),
+        freq_range=None,
         t0=0.0,
+        verbose=True,
         show_plot=True,
         input_labels=None,
         FFT=False,
         FFT_range=None,
+        figure_label="ERA Fit",
     ):
         """
         Instantiates a :class:`ERA` solver.
 
         Parameters
         ----------
         resp : 1d, 2d, or 3d ndarray
@@ -362,182 +425,231 @@
             recommended to try multiple values of `svd_tol`. The
             secondary control is the selection of modes which can be
             interactive (if `auto` is False) or automatic according to
             the parameters below.
         auto : boolean; optional
             Enables automatic selection of true modes. The default is
             False.
+        alpha, beta : integers or None; optional
+            Number of block rows and block columns to use for the
+            Hankel matrix, respectively. If both are None, the Hankel
+            matrix is made roughly square in terms of blocks. If both
+            are set, `alpha` is given precedence over `beta` if there
+            is not enough data to support both settings.
+
+            .. note::
+                 The maximum number of modes that can be detected is
+                 equal to the minimum dimension of the Hankel matrix
+                 divided by 2. So, be careful not to limit either
+                 `alpha` or `beta` too low.
+
         MSV_lower_limit : scalar; optional
             The lower limit for the normalized "mode singular value"
             for modes to be selected when `auto` is True. The MSV
-            value ranges from 0.0 to 1.0 for each mode and is a
-            measure of contribution to the response. Larger values
-            represent larger contribution.
+            value ranges from 0.0 to 1.0 for each mode.
         EMAC_lower_limit : scalar; optional
             The lower limit for the "extended modal amplitude
             coherence" value for modes to be selected when `auto` is
-            True. The EMAC value ranges from 0.0 to 1.0 for each mode
-            and is a temporal measure indicating the importance of the
-            mode over time to the fit. Higher values indicate more
-            importance. From experience, the EMAC is superior to the
-            MAC value (see below). For more information, see [#era2]_.
+            True. The EMAC value ranges from 0.0 to 1.0 for each mode.
+        EMACO_lower_limit : scalar; optional
+            The lower limit for the "extended modal amplitude
+            coherence from observability" value for modes to be
+            selected when `auto` is True. The EMACO value ranges from
+            0.0 to 1.0 for each mode.
         MPC_lower_limit : scalar; optional
             The lower limit for the "modal phase collinearity" value
             for modes to be selected when `auto` is True. The MPC
-            value ranges from 0.0 to 1.0 for each mode and is a
-            spatial measure indicating whether or not the different
-            response locations for a mode are in phase. Higher values
-            indicate more "in-phase" measurements.
+            value ranges from 0.0 to 1.0 for each mode.
+        CMIO_lower_limit : scalar; optional
+            The lower limit for the "consistent mode indicator from
+            observability" value for modes to be selected when `auto`
+            is True. The CMIO value ranges from 0.0 to 1.0 for each
+            mode.
         MAC_lower_limit : scalar; optional
             The lower limit for the "modal amplitude coherence" value
             for modes to be selected when `auto` is True. The MAC
-            value ranges from 0.0 to 1.0 for each mode and is a
-            temporal measure indicating the importance of the mode
-            over time to the fit. Higher values indicate more
-            importance. The MAC value for a mode is the dot product of
-            two vectors:
-
-                1. The ideal, reconstructed time history for a mode
-                2. The time history extracted from the input data for
-                   the mode after discarding noisy data via singular
-                   value decomposition
-
+            value ranges from 0.0 to 1.0 for each mode.
+        all_lower_limits : scalar or None; optional
+            If not None, it sets all the indicator lower limit
+            values and any other lower limit settings are quietly
+            ignored.
         damp_range : 2-tuple; optional
             Specifies the range (inclusive) of acceptable damping
             values for automatic selection.
+        freq_range : 2-tuple or None; optional
+            Specifies the range (inclusive) of acceptable frequencies
+            (in Hz) values for automatic selection. If None (the
+            default), ``freq_range = (0, sr/2)``.
         t0 : scalar; optional
             The initial time value in `resp`. Only used for plotting.
+        verbose : bool; optional
+            If True, print tables showing frequencies and
+            indicators. Ignored (treated as True) if `auto` is False.
         show_plot : boolean; optional
             If True, show plot of ERA fit (with or without FFT). The
             default is True.
         input_labels : list or None; optional
             List of data labels for each input signal to ERA.
         FFT : boolean; optional
             Enables display of FFT plot of input data. The default is
             False.
         FFT_range : scalar or list; optional
             Limits displayed frequency range of FFT plot. A scalar
             value or list with one term will act as a maximum
             cutoff. A pair of values will act as minimum and maximum
             cutoffs, respectively. The default is None.
+        figure_label : string; optional
+            Label to use for opening figures. Handy for comparing
+            different ERA fits side-by-side.
 
         Notes
         -----
         The class instance is populated with the following members
         (equation numbers are from Chapter 5 of reference [#era1]_):
 
         ================  ============================================
         Member            Description
         ================  ============================================
-        resp              impulse response data
-        resp_era          final ERA fit to the impulse response data
-        n_outputs         number of outputs
-        n_tsteps          number of time-steps
-        n_inputs          number of inputs
-        sr                sample rate
-        t0                initial time value in `resp` (for plotting)
+        resp              Impulse response data
+        resp_era          Final ERA fit to the impulse response data
+        n_outputs         Number of outputs
+        n_tsteps          Number of time-steps
+        n_inputs          Number of inputs
+        sr                Sample rate
+        t0                Initial time value in `resp` (for plotting)
         time              `resp` time vector used for plotting;
                           created from `sr` and `t0`
-        svd_tol           singular value tolerance
-        auto              automatic or interactive method of
+        svd_tol           Singular value tolerance
+        auto              Automatic or interactive method of
                           identifying true modes
-        show_plot         if True, plots are made
-        input_labels      create a legend for approximated fit plot
-        MSV_lower_limit   normalized MSV lower limit for auto-
-                          selecting modes
-        EMAC_lower_limit  EMAC lower limit for auto-selecting modes
-        MPC_lower_limit   MPC lower limit for auto-selecting modes
-        MAC_lower_limit   MAC lower limit for auto-selecting modes
-        damp_range        range of acceptable damping values for
+        show_plot         If True, plots are made
+        input_labels      Create a legend for approximated fit plot
+        lower_limits      Dict of lower limits for each indicator for
+                          auto-selecting modes
+        damp_range        Range of acceptable damping values for
+                          automatic selection
+        freq_range        Range of acceptable frequencies (Hz) for
                           automatic selection
-        FFT               produces an FFT plot of input data for
+        FFT               Produces an FFT plot of input data for
                           comparison to detected modes
-        FFT_range         frequency cutoff(s) for FFT plot
-        H_0               the H(0) generalized Hankel matrix (eq 5.24)
-        H_1               the H(1) generalized Hankel matrix (eq 5.24)
-        alpha             number of block rows (time-steps) in H
-        beta              number of block columns (time-steps) in H
+        FFT_range         Frequency cutoff(s) for FFT plot
+        figure_label      Label for figure windows
+        H_0               The H(0) generalized Hankel matrix (eq 5.24)
+        H_1               The H(1) generalized Hankel matrix (eq 5.24)
+        alpha             Number of block rows (time-steps) in H
+        beta              Number of block columns (time-steps) in H
         A_hat             ERA state-space "A" matrix, (eq 5.34)
         B_hat             ERA state-space "B" matrix, (eq 5.34)
         C_hat             ERA state-space "C" matrix, (eq 5.34)
-        A_modal           ERA modal state-space "A" matrix
+        A_modal           ERA modal state-space "A" matrix (complex
+                          eigenvalues on diagonal)
         B_modal           ERA modal state-space "B" matrix
-        C_modal           ERA modal state-space "C" matrix
-        eigs              complex eigenvalues of `A_hat` (discrete)
-        eigs_continuous   continuous version of `eigs`; ln(eigs) * sr
-        psi               complex eigenvectors of `A_hat`
-        psi_inv           inverse of `psi`
-        freqs             mode pair frequencies (rad/sec)
-        freqs_hz          mode pair frequencies (Hz)
-        zeta              mode pair percent critical damping
-        MSV               MSV values for each mode pair (eq 5.50)
-        EMAC              EMAC values for each mode pair ([#era2]_)
-        MPC               MPC values for each mode pair ([#era2]_)
-        MAC               MAC values for each mode pair (eq 5.49)
+        C_modal           ERA modal state-space "C" matrix (complex
+                          mode-shapes)
+        eigs              Complex eigenvalues of `A_hat` (discrete)
+        eigs_continuous   Continuous version of `eigs`; ln(eigs) * sr
+        psi               Complex eigenvectors of `A_hat`
+        psi_inv           Inverse of `psi`
+        freqs             Real mode frequencies (rad/sec)
+        freqs_hz          Real mode frequencies (Hz)
+        zeta              Real mode percent critical damping
+        phi               Real mode shapes (from `C_modal`); see also
+                          the MPC results for how "real" each mode is
+        indicators        Dict of all indicator values for each mode
+                          pair
         ================  ============================================
         """
         self.resp = np.atleast_3d(resp)
         # 1d --> (1, n_tsteps, 1)
         # 2d --> (n_outputs, n_tsteps, 1)
         # 3d --> (n_outputs, n_tsteps, n_inputs)
         self.n_outputs, self.n_tsteps, self.n_inputs = self.resp.shape
 
         self.sr = sr
         self.svd_tol = svd_tol
         self.auto = auto
-        self.MSV_lower_limit = MSV_lower_limit
-        self.EMAC_lower_limit = EMAC_lower_limit
-        self.MPC_lower_limit = MPC_lower_limit
-        self.MAC_lower_limit = MAC_lower_limit
+        self.lower_limits = {
+            "MSV": MSV_lower_limit,
+            "EMAC": EMAC_lower_limit,
+            "EMACO": EMACO_lower_limit,
+            "MPC": MPC_lower_limit,
+            "CMIO": CMIO_lower_limit,
+            "MAC": MAC_lower_limit,
+        }
+
+        if all_lower_limits is not None:
+            for key in self.lower_limits:
+                self.lower_limits[key] = all_lower_limits
+
         self.damp_range = damp_range
+        if freq_range is None:
+            freq_range = (0.0, sr / 2)
+        self.freq_range = freq_range
+        self.verbose = verbose
         self.show_plot = show_plot
         self.input_labels = input_labels
         self.FFT = FFT
         self.FFT_range = FFT_range
         self.t0 = t0
+        self.figure_label = figure_label
 
-        self._H_generate()
+        self._H_generate(alpha, beta)
         self._state_space()
         self._conv_2_modal()
         self._mode_select()
 
-    def _H_generate(self):
+    def _H_generate(self, alpha, beta):
         """
         Given Markov parameters, will generate the system's generalized
         Hankel matrix and time-shifted generalized Hankel matrix.
         """
         # Determining the alpha and beta parameters in order to
         # maximize coverage of data in Hankel matrices
-        alpha = self.n_tsteps // 2
-        beta = self.n_tsteps - alpha
+        if alpha is None:
+            if beta is None:
+                alpha = self.n_tsteps // 2
+                beta = self.n_tsteps - alpha
+            else:
+                beta = min(beta, self.n_tsteps - 2)
+                alpha = self.n_tsteps - beta
+        else:
+            alpha = min(alpha, self.n_tsteps - 2)
+            beta_max = self.n_tsteps - alpha
+            if beta is None:
+                beta = beta_max
+            else:
+                beta = min(beta, beta_max)
+
         H_dim = (alpha * self.n_outputs, beta * self.n_inputs)
 
         # Forming Hankel matrices
-        self.H_0 = np.empty(H_dim)
-        self.H_1 = np.empty(H_dim)
+        H_0 = np.empty(H_dim)
+        H_1 = np.empty(H_dim)
 
         # Reshaping Markov parameters into form Y = [Y0, Y1, Y2, ..., Yn]
         # Each Y[i] is of shape m x r
         Markov = self.resp.reshape(self.n_outputs, -1)
         rows = np.arange(self.n_outputs)
         cols = np.arange(beta * self.n_inputs)
 
         for _ in range(alpha):
             # Using block indexing to fill Hankel matrices with Markov
             # parameters
-            self.H_0[rows] = Markov[:, cols]
-            self.H_1[rows] = Markov[:, cols + self.n_inputs]  # Time shift
+            H_0[rows] = Markov[:, cols]
+            H_1[rows] = Markov[:, cols + self.n_inputs]  # Time shift
             # Advancing row and column indices
             rows += self.n_outputs
             cols += self.n_inputs
 
+        self.H_0 = H_0
+        self.H_1 = H_1
         self.alpha = alpha
         self.beta = beta
 
-    def _state_space(self):
+    def _state_space(self, pre_set_n=None):
         """
         This function computes a state-space representation of a system
         given the block Hankel matrix which is decomposed using
         Singular Value Decomposition (SVD) and used to find the
         state-space matrices.
 
         Notes
@@ -547,32 +659,35 @@
         system order value, it will be altered to become even to
         ensure there are an even number of singular values.
         """
 
         # Decomposing H_0 using SVD
         R, sigma, ST = np.linalg.svd(self.H_0)  # eq 5.30, #era1
 
-        # svd_tol can be treated as a selection of modes (if greater
-        # than 1) or svd_tol can be set as a numeric boundary to sort
-        # through non-significant singular values
-        if self.svd_tol >= 1:
-            n = int(self.svd_tol)
-            if n > sigma.size:
-                n = sigma.size
-                warn(
-                    f"`svd_tol` ({n}) is greater than number of singular values"
-                    f" ({sigma.size}).",
-                    RuntimeWarning,
-                )
-        else:
-            n = np.argwhere(sigma / sigma[0] >= self.svd_tol).size
+        if pre_set_n is None:
+            # svd_tol can be treated as a selection of modes (if greater
+            # than 1) or svd_tol can be set as a numeric boundary to sort
+            # through non-significant singular values
+            if self.svd_tol >= 1:
+                n = int(self.svd_tol)
+                if n > sigma.size:
+                    n = sigma.size
+                    warn(
+                        f"`svd_tol` ({n}) is greater than number of singular values"
+                        f" ({sigma.size}).",
+                        RuntimeWarning,
+                    )
+            else:
+                n = np.argwhere(sigma / sigma[0] >= self.svd_tol).size
 
-        # Ensures that number of pairs remains even
-        if n % 2 != 0:
-            n += 1
+            # Ensures that number of pairs remains even
+            if n % 2 != 0:
+                n += 1
+        else:
+            n = pre_set_n
 
         # Reshaping R, sigma, ST, accordingly
         R = R[:, :n]
         sigma_sqrt = np.sqrt(sigma[:n])
         ST = ST[:n, :]
 
         # Recovering P and Q matrices: eq 5.35, #era1
@@ -584,87 +699,124 @@
         self.B_hat = self.Q[:, : self.n_inputs]
         self.A_hat = (R / sigma_sqrt).T @ self.H_1 @ (ST.T / sigma_sqrt)
 
     def _form_modal_realization(self):
         # Compute modal space state-space matrices
         self.A_modal = np.diag(self.eigs)
 
-        # include all modes for the EMAC calculation
+        # include all time for the EMAC calculation
         self.B_modal_all = self.psi_inv @ self.Q
         self.C_modal_all = self.P @ self.psi
 
         self.B_modal = self.B_modal_all[:, : self.n_inputs]
         self.C_modal = self.C_modal_all[: self.n_outputs]
 
+        # form estimate of real mode shapes:
+        phi = self.C_modal[:, ::2]
+        rows = np.abs(phi).argmax(axis=0)
+        cols = np.arange(phi.shape[1])
+        phi_scaled = phi / phi[rows, cols]
+        self.phi = phi_scaled.real
+
         # Calculate indicators:
         self._MSV()
         self._EMAC()
         self._MPC()
         self._MAC()
 
+        # also calculate the EMACO and CMIO from ref 3:
+        # self.EMACO = self.EMACo.mean(axis=1)
+        self.CMIO = self.EMACO * self.MPC
+
+        self.indicators = {
+            "MSV": self.MSV,
+            "EMAC": self.EMAC,
+            "EMACO": self.EMACO,
+            "MPC": self.MPC,
+            "CMIO": self.CMIO,
+            "MAC": self.MAC,
+        }
+
     def _conv_2_modal(self):
         """
         This routine converts the system realization problem into
         modal space.
         """
         # Generating eigenvalues and matrix of eigenvectors
-        self.eigs, self.psi = la.eig(self.A_hat)
+        eigs, psi = la.eig(self.A_hat)
 
         # Retrieving sorted index of eigenvalues based on magnitude of
         # imaginary components
         #  - Using a stable sorter to allow for preservation of
         #    overdamped modes (in case they're consecutive; if not,
         #    see the special note in the documentation for class ERA)
-        i = np.argsort(abs(self.eigs.imag), kind="stable")
-        self.eigs = self.eigs[i]
-        self.psi = self.psi[:, i]
-
-        self.eigs_continuous = np.log(self.eigs) * self.sr
-        self.freqs, self.zeta = ode.get_freq_damping(
-            self.eigs_continuous, suppress_warning=True
-        )
+        i = np.argsort(abs(eigs.imag), kind="stable")
+        eigs = eigs[i]
+        psi = psi[:, i]
+
+        eigs_continuous = np.log(eigs) * self.sr
+        freqs, zeta = ode.get_freq_damping(eigs_continuous, suppress_warning=True)
 
         # Finding the order of increasing frequency
-        index = np.argsort(self.freqs, kind="stable")
+        index = np.argsort(freqs, kind="stable")
 
         # Locating overdamped modes and putting them first:
-        pv = self.zeta[index] >= 1.0
+        pv = zeta[index] >= 1.0
         index = np.concatenate((index[pv], index[~pv]))
 
         # Ordering frequencies and damping accordingly
-        self.freqs = self.freqs[index]
-        self.zeta = self.zeta[index]
+        self.freqs = freqs[index]
+        self.zeta = zeta[index]
 
         # Deriving ordered indexing for mode pairs
         index_pairs = np.empty(index.size * 2, dtype=int)
         for i in range(index.size):
             index_pairs[2 * i] = index[i] * 2
             index_pairs[2 * i + 1] = index[i] * 2 + 1
 
         # Re-ordering eigenvalues and eigenvectors
-        self.eigs = self.eigs[index_pairs]
-        self.psi = self.psi[:, index_pairs]
+        self.eigs = eigs[index_pairs]
+        self.eigs_continuous = eigs_continuous[index_pairs]
+        self.psi = psi[:, index_pairs]
 
         # Deriving the frequencies in Hz
         self.freqs_hz = self.freqs / (2 * np.pi)
 
         # Recovering inverse of eigenvector matrix
         self.psi_inv = np.linalg.inv(self.psi)
 
         self._form_modal_realization()
 
+    def _remove_noise(self):
+        """
+        Replace input response history with current ERA fit
+        """
+        self.resp = self.resp_era
+        self._H_generate()
+        self._state_space()
+        self._conv_2_modal()
+
     def _remove_fit(self):
         """
         Remove current ERA fit from the input response history
         """
         self.resp = self.resp - self.resp_era
         self._H_generate()
         self._state_space()
         self._conv_2_modal()
 
+    def _remove_fit2(self, n_modes):
+        """
+        Remove current ERA fit from the input response history
+        """
+        self.resp = self.resp - self.resp_era
+        self._H_generate()
+        self._state_space(self.A_hat.shape[0] - 2 * n_modes)
+        self._conv_2_modal()
+
     def _MSV(self):
         """
         This routine calculates the normalized Mode Singular Values (MSV)
         of each detected mode.
         """
         A_m, B_m, C_m = self.A_modal, self.B_modal, self.C_modal
         lamd = np.diag(A_m)
@@ -813,24 +965,33 @@
         )
 
         # total EMAC:
         B_modal = self.B_modal
         C_modal = self.C_modal
         n = B_modal.shape[0]
         EMAC = np.empty(n // 2)
+        EMACO = np.empty(n // 2)
         for i, j in enumerate(range(0, n - 1, 2)):
             c2 = abs(C_modal[:, j]) ** 2
             b2 = abs(B_modal[j, :]) ** 2
-            num = (EMACo[i] @ c2) * (b2 @ EMACi[i])
-            den = c2.sum() * b2.sum()
+
+            # just based on observability (outputs)
+            num = EMACo[i] @ c2
+            den = c2.sum()
+            EMACO[i] = num / den
+
+            # include controllability (inputs)
+            num *= b2 @ EMACi[i]
+            den *= b2.sum()
             EMAC[i] = num / den
 
         self.EMACo = EMACo
         self.EMACi = EMACi
         self.EMAC = EMAC
+        self.EMACO = EMACO
 
     def _MPC(self):
         """
         This routine calculates the Modal Phase Colinearity for each
         detected mode.
         """
         C = self.C_modal
@@ -838,24 +999,23 @@
         MPC = np.empty(n // 2)
         for i, j in enumerate(range(0, n - 1, 2)):
             re = C[:, j].real
             im = C[:, j].imag
             Sxx = re @ re
             Syy = im @ im
             Sxy = re @ im
-            # om = la.eigh([[Sxx, Sxy], [Sxy, Syy]], eigvals_only=True)
-            # lam1 = om[1]
-            # lam2 = om[0]
-
-            # from pyyeti.ytools._calc_covariance_sine_cosine:
-            term = np.sqrt((Syy - Sxx) ** 2 + 4 * Sxy ** 2)
-            lam1 = (Sxx + Syy + term) / 2
-            lam2 = (Sxx + Syy - term) / 2
-
-            MPC[i] = (2 * lam1 / (lam1 + lam2) - 1) ** 2
+            # Can solve for eigenvalues with `la.eigh`:
+            #  om = la.eigh([[Sxx, Sxy], [Sxy, Syy]], eigvals_only=True)
+            #  lam1 = om[1]
+            #  lam2 = om[0]
+            # and then use the equations in the reference ...
+            # Or, since this is just 2x2, we can solve by hand (see
+            # eqns in pyyeti.ytools._calc_covariance_sine_cosine, then
+            # simplify the final eqn by hand)
+            MPC[i] = ((Syy - Sxx) ** 2 + 4 * Sxy**2) / (Sxx + Syy) ** 2
 
         self.MPC = MPC
 
     def _trim_2_selected_modes(self, selected_modes, saved_model=False):
         """
         This function extracts selected modes and arranges them to be
         presented without excluded modes. It recalculates the modal
@@ -867,33 +1027,36 @@
         if len(selected_modes) == 0:
             raise RuntimeError("No modes selected")
 
         if saved_model:
             freq = self._saved["freqs_hz"]
             zeta = self._saved["zeta"]
             eigs = self._saved["eigs"]
+            eigs_continuous = self._saved["eigs_continuous"]
             psi = self._saved["psi"]
             psi_inv = self._saved["psi_inv"]
         else:
             freq = self.freqs_hz
             zeta = self.zeta
             eigs = self.eigs
+            eigs_continuous = self.eigs_continuous
             psi = self.psi
             psi_inv = self.psi_inv
 
         # Identifying position of modal pairs
         self.selected_mode_pairs = []
         for i in selected_modes:
             self.selected_mode_pairs.append(2 * i)
             self.selected_mode_pairs.append(2 * i + 1)
 
         # Extracting reduced data
         self.freqs_hz = freq[selected_modes]
         self.zeta = zeta[selected_modes]
         self.eigs = eigs[self.selected_mode_pairs]
+        self.eigs_continuous = eigs_continuous[self.selected_mode_pairs]
         self.psi = psi[:, self.selected_mode_pairs]
         self.psi_inv = psi_inv[self.selected_mode_pairs, :]
 
         self._form_modal_realization()
 
     def _compute_era_fit(self, A, B, C):
         """
@@ -948,15 +1111,15 @@
 
         y = self.resp_era
         if not hasattr(self, "time"):
             self.time = np.arange(0, self.n_tsteps) / self.sr + self.t0
 
         # plot each input in its own window
         for j in range(self.n_inputs):
-            fig = plt.figure(f"ERA Fit, input {j}", clear=True)
+            fig = plt.figure(f"{self.figure_label}, input {j}", clear=True)
 
             if self.FFT:
                 ax1 = fig.add_subplot(211)
                 ax2 = fig.add_subplot(212)
             else:
                 ax1 = fig.add_subplot(111)
 
@@ -1028,131 +1191,118 @@
                 ax2.set_ylabel("Magnitude")
                 ax2.set_title("Magnitude of Frequency Responses of Data")
 
             fig.tight_layout()
             fig.canvas.draw()
         plt.show()
 
-    def _mode_print(self, title, freq, zeta, msv, emac, mpc, mac, mark):
+    @staticmethod
+    def _get_head_frm(which):
+        headers = [
+            " ",
+            "Mode",
+            "Freq (Hz)",
+            "% Damp",
+            *which,
+        ]
+        n_indicators = len(which)
+        widths = [1, 4, 9, 8] + [6] * n_indicators
+        formats = ["{}", "{:4}", "{:9.4f}", "{:8.4f}"] + n_indicators * ["{}{:5.3f}"]
+        head, frm = writer.formheader(headers, widths, formats, sep=(0, 1, 2), just="c")
+        # delete 1st underline:
+        head = "\n".join([" " + line[1:] for line in head.split("\n")])[:-2]
+        return head, frm
+
+    def _get_stars(self, mark, which, dct):
+        """
+        Return dict of lists to highlight auto-selected modes; one #
+        modes length list for each indicator
+        """
+        stars = {}
+        if mark:
+            all_star = True
+            for indicator in which:
+                good_modes = (
+                    dct["indicators"][indicator] >= self.lower_limits[indicator]
+                )
+                stars[indicator] = ["*" if j else " " for j in good_modes]
+                all_star = good_modes & all_star
+            all_star = all_star & (
+                (self.damp_range[0] <= dct["zeta"])
+                & (dct["zeta"] <= self.damp_range[1])
+            )
+            all_star = all_star & (
+                (self.freq_range[0] <= dct["freqs_hz"])
+                & (dct["freqs_hz"] <= self.freq_range[1])
+            )
+            rec_keep = all_star.nonzero()[0]
+            all_star = ["*" if j else " " for j in all_star]
+        else:
+            all_star = [" "] * (len(dct["eigs"]) // 2)
+            for indicator in which:
+                stars[indicator] = all_star
+            rec_keep = []
+        return stars, all_star, rec_keep
+
+    def _mode_print(self, title, dct, mark):
         """
         This function prints a table of descriptive data for each mode
         of interest.
 
         Parameters
         ----------
         title : string
             Title for table
-        freq : 1d ndarray
-            Array of modal frequencies, in Hz.
-        zeta : 1d ndarray
-            Array of modal damping.
-        msv : 2d ndarray
-            Array of MSV values corresponding with each mode.
-        emac : 2d ndarray
-            Array of EMAC values corresponding with each mode.
-        mpc : 2d ndarray
-            Array of MPC values corresponding with each mode.
-        mac : 2d ndarray
-            Array of MAC values corresponding with each mode.
+        dct : dict
+            Contains "freq", "zeta", "indicators", "eigs", etc
         mark : boolean
             If True, mark "good" modes with an asterisk ("*")
         """
         # Prints table of model data
-        print(f"\n{title}:")
-        print("  Mode   Freq. (Hz)     Zeta        MSV      EMAC       MPC       MAC")
-        print("  --------------------------------------------------------------------")
-        self.rec_keep = []
-        n = mac.shape[0]
-        for i in range(n):
-            if mark:
-                stars = []
-                for indicator, limit in (
-                    (msv, self.MSV_lower_limit),
-                    (emac, self.EMAC_lower_limit),
-                    (mpc, self.MPC_lower_limit),
-                    (mac, self.MAC_lower_limit),
-                ):
-                    if indicator[i] >= limit:
-                        stars.append("*")
-                    else:
-                        stars.append(" ")
-
-                if stars.count("*") == 4 and (
-                    self.damp_range[0] <= zeta[i] <= self.damp_range[1]
-                ):
-                    main_star = "*"
-                    self.rec_keep.append(i)
-                else:
-                    main_star = " "
-            else:
-                main_star = " "
-                stars = "    "
+        which = [
+            "MSV",
+            "EMAC",
+            "EMACO",
+            "MPC",
+            "CMIO",
+            "MAC",
+        ]
 
-            print(
-                ("{} {:4}  {:10.5f}  {:10.5f}" + "    {}{:{w}.{p}f}" * 4).format(
-                    main_star,
-                    i + 1,
-                    freq[i],
-                    zeta[i],
-                    stars[0],
-                    msv[i],
-                    stars[1],
-                    emac[i],
-                    stars[2],
-                    mpc[i],
-                    stars[3],
-                    mac[i],
-                    w=5,
-                    p=3,
-                )
-            )
+        head, frm = self._get_head_frm(which)
+        stars, all_star, self.rec_keep = self._get_stars(mark, which, dct)
+
+        n = len(dct["eigs"]) // 2
+        args = [all_star, np.arange(1, n + 1), dct["freqs_hz"], 100 * dct["zeta"]]
+        for indicator in which:
+            args.append(stars[indicator])
+            args.append(dct["indicators"][indicator])
+
+        if not self.auto or self.verbose:
+            print(f"\n{title}:")
+            print(head)
+            writer.vecwrite(sys.stdout, frm, *args)
 
     def _show_model(self, title, *, mark, saved_model=False):
-        if saved_model:
-            self._mode_print(
-                title,
-                self._saved["freqs_hz"],
-                self._saved["zeta"],
-                self._saved["MSV"],
-                self._saved["EMAC"],
-                self._saved["MPC"],
-                self._saved["MAC"],
-                mark,
-            )
-            self._compute_era_fit(
-                self._saved["A_modal"], self._saved["B_modal"], self._saved["C_modal"]
-            )
-        else:
-            self._mode_print(
-                title,
-                self.freqs_hz,
-                self.zeta,
-                self.MSV,
-                self.EMAC,
-                self.MPC,
-                self.MAC,
-                mark,
-            )
-            self._compute_era_fit(self.A_modal, self.B_modal, self.C_modal)
+        dct = self._saved if saved_model else self.__dict__
+        self._mode_print(title, dct, mark)
+        self._compute_era_fit(dct["A_modal"], dct["B_modal"], dct["C_modal"])
 
     def _save_model_data(self):
         """
         Saves model data so looping can return to beginning
         """
         names = (
             "freqs_hz",
             "zeta",
-            "MSV",
-            "EMAC",
-            "MPC",
-            "MAC",
+            "indicators",
             "A_modal",
             "B_modal",
             "C_modal",
             "eigs",
+            "eigs_continuous",
             "psi",
             "psi_inv",
         )
         self._saved = {name: getattr(self, name) for name in names}
 
     def _mode_select(self):
         """
@@ -1164,37 +1314,47 @@
         Notes
         -----
         Prompts user to select modes of interest. Recommended modes
         (determined from indicator values) will be marked with an *
         symbol.
         """
         self._show_model("Current fit includes all modes", mark=True)
+        self._save_model_data()
 
         # Runs interactive version of mode selection process
         if not self.auto:
-            self._save_model_data()
             done = "s"  # "s" for "select different modes"
             while done == "s":
                 input_string = (
                     input(
-                        "\nSelect modes for ERA fit (to keep or remove):\n"
-                        "\t- <Enter> or '*' to keep marked modes\n"
-                        "\t- 'a' to keep all modes\n"
-                        "\t- mode #s separated by space and/or comma (eg: 1, 2, 5)\n"
+                        "\nSelect modes for ERA fit (to keep or remove) [*]:\n"
+                        "\t* = keep marked modes\n"
+                        "\ta = keep all modes\n"
+                        "\tn = remove noise (via `svd_tol` setting; experimental)\n\n"
+                        "\tor: mode #s separated by space and/or comma (eg: 1, 2, 5-8),"
+                        " or\n\t    array_like Python expression\n"
                     )
                     .strip(", ")
                     .lower()
                 )
 
                 if input_string in ("*", ""):
                     selected_modes = np.array(self.rec_keep)
                 elif input_string == "a":
                     selected_modes = np.arange(len(self._saved["freqs_hz"]))
+                elif input_string == "n":
+                    self._remove_noise()
+                    self._show_model(
+                        "Fit with all modes after removing noise", mark=True
+                    )
+                    self._save_model_data()
+                    done = "s"
+                    continue
                 else:
-                    selected_modes = _string_to_ints(input_string)
+                    selected_modes = _string_to_ints2(input_string)
 
                 # Reducing model using selected modes
                 self._trim_2_selected_modes(selected_modes, saved_model=True)
                 self._show_model("Reduced model fit", mark=False)
 
                 done = input(
                     "\nDone? (d/s/r) [D]:\n"
@@ -1205,17 +1365,342 @@
                 ).lower()
 
                 if done == "s":
                     # restart mode selection:
                     self._show_model("Current fit", mark=True, saved_model=True)
                 elif done == "r":
                     # remove current fit, then restart mode selection:
-                    self._remove_fit()
+                    # self._remove_fit()
+                    self._remove_fit2(len(selected_modes))
                     self._show_model("Model data after removing fit", mark=True)
                     self._save_model_data()
                     done = "s"
 
         else:
             # automatically keep recommended modes
             selected_modes = np.array(self.rec_keep, dtype=int)
             self._trim_2_selected_modes(selected_modes)
             self._show_model("Auto-selected modes fit", mark=False)
+
+
+def NExT(
+    resp,
+    sr,
+    *,
+    ref_channels="all",
+    lag_start=1,
+    lag_stop,
+    domain="time",
+    nperseg=None,
+    window="hann",
+    nfft=None,
+    noverlap=None,
+):
+    """
+    Use NExT method to prepare measurement data for :class:`ERA`
+
+    **BETA**
+
+    This routine uses the "Natural Excitation Technique" to process
+    response measurements into free-decay-like signals using
+    cross-correlations. This can be done in either the time-domain or
+    the frequency-domain. The resulting signals can then be input to
+    ERA (the Eigensystem Realization Algorithm) for system
+    identification. See references [#nxt1]_ and [#nxt2]_.
+
+    Parameters
+    ----------
+    resp : 1d or 2d ndarray
+        The response signal(s) to process. If 2d, each row is a response
+        measurement. This data is expected to represent ambient
+        vibration responses over a significant period of time. Longer
+        measurements will result in more accurate results.
+    sr : scalar
+        Sample rate at which `resp` was sampled.
+    ref_channels : integer, integer array_like, or "all"; optional
+        If integer or integer array_like, specifies row(s) of `resp`
+        to use as the reference channel(s) for the cross-correlations
+        (starts at 0). Set to "all" to use all rows as reference (the
+        default). Note that the auto-correlation of each reference
+        channel will be included in the output.
+    lag_start : integer; optional
+        Cross-correlation lag for start of decay. This routine will
+        compute auto-correlations, and for those, any noise present in
+        the signal will be included in the 0 lag term. Specifically,
+        the noise will be squared and summed, as if it is perfectly
+        correlated. Therefore, the default `lag_start` is set to 1 to
+        avoid including perfectly correlated noise in the decay
+        signal.
+    lag_stop : integer
+        Cross-correlation lag for end of decay. It is recommended to
+        set this to the minimum viable value based on the lowest
+        frequency you are interested in for the current run. For
+        example, an initial value for `lag_stop` might be computed
+        such that the decay will have time for one full cycle of the
+        estimated lowest frequency (in Hz)::
+
+            lag_stop = lag_start + sr / lowest_est_freq
+
+        .. note::
+
+            `lag_stop` must be less than ``nperseg / 2`` if `domain`
+            is "frequency". This is due to the symmetric nature of the
+            cross-correlations. This shouldn't be much of a
+            restriction however, as the `lag_stop` value will
+            typically be considerably less than this for good results.
+
+    domain : string
+        Either "time" or "frequency" to specify how this routine is to
+        compute the cross-correlations. If "time",
+        :func:`scipy.signal.correlate` is used to compute the
+        correlations using the entire time history for each
+        cross-correlation. If "frequency", :func:`scipy.fft.ifft` and
+        :func:`scipy.signal.csd` are used together to compute the
+        correlations, along with looping and windowing and
+        averaging. If `domain` is "frequency", see the inputs
+        `nperseg`, `window`, `nfft`, and `noverlap`.
+    nperseg : integer
+        Required if `domain` is "frequency". Specifies the window size
+        to pass to :func:`scipy.signal.csd`. If `nperseg` is too
+        small, the damping for the lower frequency modes will likely
+        be inflated. In order to get any benefit that might come from
+        averaging multiple windows, a reasonable initial setting for
+        this value might be to choose the first power-of-2 less than N
+        / 2 where N is the number of time-steps. That would result in
+        the largest power-of-2 size window size (for fast processing)
+        while still giving you 3 windows to average.
+    window, nfft, noverlap : optional
+        These inputs are only used if `domain` is "frequency". The are
+        all passed to :func:`scipy.signal.csd`.
+
+    Returns
+    -------
+    3d ndarray
+        Decay-like responses shaped as expected by :class:`ERA`:
+        ``n_channels x n_decay_tsteps x n_ref_channels``. :class:`ERA`
+        will interpret the number of reference channels as the number
+        of inputs.
+
+    References
+    ----------
+    .. [#nxt1] James, G.H., Carne, T.G., and Lauffer, J.P. "The
+               Natural Excitation Technique (NExT) for Modal Parameter
+               Extraction From Operating Wind Turbines", Sandia
+               National Laboratories, Albuquerque, NM and Livermore,
+               CA, SAND92-1666 (1993).
+
+    .. [#nxt2] James, G.H., Carne, T.G., and Lauffer, J.P. "The
+               Natural Excitation Technique (NExT) for Modal Parameter
+               Extraction from Operating Structures", Modal Analysis
+               10:260–277 (1995).
+
+    Examples
+    --------
+    To generate synthetic ambient vibrations of a simple structure,
+    the same system that was demoed in :class:`ERA` is excited by
+    random forces over 100 seconds. The responses are fed into NExT
+    and then into :class:`ERA`.
+
+    .. plot::
+        :context: close-figs
+
+        We have the following mass, damping and stiffness matrices
+        (note that the damping has been specially defined to be
+        diagonalized by the modes):
+
+        >>> import numpy as np
+        >>> import scipy.linalg as la
+        >>> from pyyeti import era, ode
+        >>> np.set_printoptions(precision=5, suppress=True)
+        >>>
+        >>> M = np.identity(3)
+        >>>
+        >>> K = np.array(
+        ...     [
+        ...         [4185.1498, 576.6947, 3646.8923],
+        ...         [576.6947, 2104.9252, -28.0450],
+        ...         [3646.8923, -28.0450, 3451.5583],
+        ...     ]
+        ... )
+        >>>
+        >>> D = np.array(
+        ...     [
+        ...         [4.96765646, 0.97182432, 4.0162425],
+        ...         [0.97182432, 6.71403672, -0.86138453],
+        ...         [4.0162425, -0.86138453, 4.28850828],
+        ...     ]
+        ... )
+
+        Since we have the system matrices, we can determine the
+        frequencies and damping using the eigensolution.
+
+        >>> (w2, phi) = la.eigh(K, M)
+        >>> omega = np.sqrt(w2)
+        >>> freq_hz = omega / (2 * np.pi)
+        >>> freq_hz
+        array([  1.33603,   7.39083,  13.79671])
+        >>> modal_damping = phi.T @ D @ phi
+        >>> modal_damping
+        array([[ 0.33578, -0.     , -0.     ],
+               [-0.     ,  6.9657 ,  0.     ],
+               [-0.     ,  0.     ,  8.66873]])
+        >>> zeta = np.diag(modal_damping) / (2 * omega)
+        >>> zeta
+        array([ 0.02 ,  0.075,  0.05 ])
+
+        Simulate ambient vibrations over 100 seconds:
+
+        >>> dt = 0.01
+        >>> t = np.arange(0, 100, dt)
+        >>> n = len(t)
+        >>> sr = 1 / dt
+        >>> np.random.seed(1)  # for repeatability
+        >>> F = np.random.randn(3, len(t))
+        >>> ts = ode.SolveUnc(M, D, K, dt)
+        >>> sol = ts.tsolve(force=F)
+
+        Use the time-domain method of NExT and call :class:`ERA` to
+        get estimates of frequency, damping, and mode-shapes. We'll
+        use a `lag_stop` of 75 (from sr / lowest_freq = 100 / 1.33 ~=
+        75).
+
+        >>> era_fit = era.ERA(
+        ...     era.NExT(sol.a, sr, lag_stop=75),
+        ...     sr=1 / dt,
+        ...     auto=True,
+        ...     input_labels=["x", "y", "z"],
+        ...     figure_label="Time Domain ERA Fit",
+        ... )
+        <BLANKLINE>
+        Current fit includes all modes:
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+        *    1     1.3258    2.4155  *0.676  *0.996  *0.998  *1.000  *0.998  *1.000
+        *    2     7.5586    7.0610  *0.656  *0.715  *0.844  *1.000  *0.843  *1.000
+        *    3    13.8643    4.6710  *1.000  *0.721  *0.852  *1.000  *0.852  *1.000
+        <BLANKLINE>
+        Auto-selected modes fit:
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+             1     1.3258    2.4155   0.676   0.996   0.998   1.000   0.998   1.000
+             2     7.5586    7.0610   0.656   0.715   0.844   1.000   0.843   1.000
+             3    13.8643    4.6710   1.000   0.721   0.852   1.000   0.852   1.000
+
+    .. plot::
+        :context: close-figs
+
+        That seemed to work out pretty well! Now we'll try the
+        frequency-domain method of NExT (the increased `svd_tol` gave
+        slightly better results in this case):
+
+        >>> era_fit = era.ERA(
+        ...     era.NExT(
+        ...         sol.a,
+        ...         sr,
+        ...         lag_stop=75,
+        ...         domain="frequency",
+        ...         nperseg=4096,
+        ...     ),
+        ...     sr=1 / dt,
+        ...     svd_tol=0.1,
+        ...     auto=True,
+        ...     input_labels=["x", "y", "z"],
+        ...     figure_label="Frequency Domain ERA Fit",
+        ... )
+        <BLANKLINE>
+        Current fit includes all modes:
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+        *    1     1.3231    2.1499  *0.691  *0.993  *0.997  *1.000  *0.997  *1.000
+        *    2     7.5231    7.1348  *0.626  *0.640  *0.801  *0.997  *0.798  *0.999
+        *    3    13.9075    4.2107  *1.000  *0.684  *0.813  *1.000  *0.813  *0.999
+        <BLANKLINE>
+        Auto-selected modes fit:
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+             1     1.3231    2.1499   0.691   0.993   0.997   1.000   0.997   1.000
+             2     7.5231    7.1348   0.626   0.640   0.801   0.997   0.798   0.999
+             3    13.9075    4.2107   1.000   0.684   0.813   1.000   0.813   0.999
+
+    .. plot::
+        :context: close-figs
+
+        Both of the above examples used all channels as reference
+        channels. The next example uses just the first measurement as
+        the reference channel (which also means that the only
+        auto-correlation that will be included will be for the first
+        measurement):
+
+        >>> era_fit = era.ERA(
+        ...     era.NExT(sol.a, sr, lag_stop=75, ref_channels=0),
+        ...     sr=1 / dt,
+        ...     auto=True,
+        ...     input_labels=["x", "y", "z"],
+        ...     figure_label="Time Domain ERA Fit",
+        ... )
+        <BLANKLINE>
+        Current fit includes all modes:
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+        *    1     1.3455    1.8899  *0.881  *0.992  *0.992  *1.000  *0.992  *1.000
+             2     7.4679    4.5610   0.238  *0.785  *0.873  *0.978  *0.854  *0.998
+        *    3    13.8546    4.9336  *1.000  *0.893  *0.924  *0.999  *0.923  *1.000
+             4    14.5075   -3.7478   0.246  *0.440  *0.604   0.226   0.137  *0.982
+        <BLANKLINE>
+        Auto-selected modes fit:
+          Mode  Freq (Hz)   % Damp    MSV     EMAC   EMACO    MPC     CMIO    MAC
+          ----  ---------  --------  ------  ------  ------  ------  ------  ------
+             1     1.3455    1.8899   0.881   0.992   0.992   1.000   0.992   1.000
+             2    13.8546    4.9336   1.000   0.893   0.924   0.999   0.923   1.000
+
+        All three modes were identified, but the 7.4 Hz mode was not
+        auto-selected because the MSV indicator was too low. To
+        successfully auto-select it, we could either lower the MSV
+        value, use a different reference channel, or add more
+        reference channels.
+    """
+    resp = np.atleast_2d(resp)
+    n = resp.shape[1]
+
+    if ref_channels == "all":
+        ref_channels = np.arange(0, resp.shape[0])
+    else:
+        ref_channels = np.atleast_1d(ref_channels)
+
+    # compute cross-correlation functions
+    xc = []
+    if domain == "time":
+        for ref in resp[ref_channels]:
+            xc_ref = []
+            for sig in resp:
+                corr = signal.correlate(ref, sig, mode="same")[n // 2 :]
+                xc_ref.append(corr[lag_start : lag_stop + 1])
+            xc.append(xc_ref)
+    elif domain == "frequency":
+        # csd will scale values down by window.sum() ** 2 ... we don't
+        # need or necessarily want that, so scaling up by nperseg ** 2
+        # is reasonable
+        sc = nperseg**2
+        for ref in resp[ref_channels]:
+            xc_ref = []
+            for sig in resp:
+                f, csd = signal.csd(
+                    ref,
+                    sig,
+                    fs=sr,
+                    window=window,
+                    nperseg=nperseg,
+                    nfft=nfft,
+                    noverlap=noverlap,
+                    scaling="spectrum",
+                    return_onesided=False,
+                )
+                corr = fft.ifft(csd).real * sc
+                xc_ref.append(corr[lag_start : lag_stop + 1])
+            xc.append(xc_ref)
+    else:
+        raise ValueError(
+            "invalid value for `domain`; must be either 'time' or 'frequency'"
+        )
+
+    # put reference channels last instead of first for ERA:
+    return np.moveaxis(xc, 0, -1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyyeti-1.2.6/pyyeti/expmint.py` & `pyyeti-1.2.8/pyyeti/expmint.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/fdepsd.py` & `pyyeti-1.2.8/pyyeti/fdepsd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/frclim.py` & `pyyeti-1.2.8/pyyeti/frclim.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/guitools.py` & `pyyeti-1.2.8/pyyeti/guitools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/locate.py` & `pyyeti-1.2.8/pyyeti/locate.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/nastran/bulk.py` & `pyyeti-1.2.8/pyyeti/nastran/bulk.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/nastran/n2p.py` & `pyyeti-1.2.8/pyyeti/nastran/n2p.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/nastran/op2.py` & `pyyeti-1.2.8/pyyeti/nastran/op2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/nastran/op4.py` & `pyyeti-1.2.8/pyyeti/nastran/op4.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/__init__.py` & `pyyeti-1.2.8/pyyeti/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/_base_ode_class.py` & `pyyeti-1.2.8/pyyeti/ode/_base_ode_class.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/_utilities.py` & `pyyeti-1.2.8/pyyeti/ode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/freqdirect.py` & `pyyeti-1.2.8/pyyeti/ode/freqdirect.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/frf_mode_participation.py` & `pyyeti-1.2.8/pyyeti/ode/frf_mode_participation.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/solvecdf.py` & `pyyeti-1.2.8/pyyeti/ode/solvecdf.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/solveexp1.py` & `pyyeti-1.2.8/pyyeti/ode/solveexp1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/solveexp2.py` & `pyyeti-1.2.8/pyyeti/ode/solveexp2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/solvenewmark.py` & `pyyeti-1.2.8/pyyeti/ode/solvenewmark.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ode/solveunc.py` & `pyyeti-1.2.8/pyyeti/ode/solveunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -757,17 +757,20 @@
                0    same as "" (no rigid-body is included)
                1    same as "av"
                2    same as "dva" (all rigid-body responses included)
             ======  =================================================
 
         rf_disp_only : bool; optional
             This option specifies how to handle the velocity and
-            acceleration terms for residual-flexibility modes. If
-            True, they are set to zero. If False, they are computed
-            from the normal frequency-domain relationships::
+            acceleration terms for residual-flexibility modes. (The
+            displacements for these modes is always computed
+            statically.) If True, the velocities and accelerations are
+            set to zero. If False, the default and generally
+            recommended setting, they are computed from the normal
+            frequency-domain relationships::
 
                 velocity = i * omega * displacement
                 acceleration = -omega ** 2 * displacement
 
         Returns
         -------
         A SimpleNamespace with the members:
@@ -1820,15 +1823,15 @@
                 a[rb] = a_rb
 
     def _solve_freq_unc(self, d, v, a, force, freq, incrb):
         """Solve the uncoupled equations for
         :func:`SolveUnc.fsolve`"""
         # convert frequency in Hz to radian/sec:
         freqw = 2 * np.pi * freq
-        freqw2 = freqw ** 2
+        freqw2 = freqw**2
 
         # solve rigid-body and elastic parts separately
         # - residual-flexibility part was already solved in _init_dva
 
         # solve rigid-body part:
         self._solve_freq_rb(d, v, a, force, freqw, freqw2, incrb, True)
 
@@ -1851,15 +1854,15 @@
             a[el] = d[el] * -(freqw2)
             v[el] = d[el] * (1j * freqw)
 
     def _solve_freq_coup(self, d, v, a, force, freq, incrb):
         """Solve the coupled equations for :func:`SolveUnc.fsolve`"""
         # convert frequency in Hz to radian/sec:
         freqw = 2 * np.pi * freq
-        freqw2 = freqw ** 2
+        freqw2 = freqw**2
 
         # solve rigid-body and elastic parts separately
         # - residual-flexibility part was already solved in _init_dva
 
         # solve rigid-body part:
         self._solve_freq_rb(d, v, a, force, freqw, freqw2, incrb, False)
```

### Comparing `pyyeti-1.2.6/pyyeti/pp.py` & `pyyeti-1.2.8/pyyeti/pp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/psd.py` & `pyyeti-1.2.8/pyyeti/psd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/rainflow/c_rain.c` & `pyyeti-1.2.8/pyyeti/rainflow/c_rain.c`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/rainflow/py_rain.py` & `pyyeti-1.2.8/pyyeti/rainflow/py_rain.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/srs.py` & `pyyeti-1.2.8/pyyeti/srs.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ssmodel.py` & `pyyeti-1.2.8/pyyeti/ssmodel.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/stats.py` & `pyyeti-1.2.8/pyyeti/stats.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/writer.py` & `pyyeti-1.2.8/pyyeti/writer.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti/ytools.py` & `pyyeti-1.2.8/pyyeti/ytools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/pyyeti.egg-info/PKG-INFO` & `pyyeti-1.2.8/pyyeti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.2.6
+Version: 1.2.8
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.2.6 Summary: Tools mostly related
+Metadata-Version: 2.1 Name: pyyeti Version: 1.2.8 Summary: Tools mostly related
 to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
 Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: C
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `pyyeti-1.2.6/pyyeti.egg-info/SOURCES.txt` & `pyyeti-1.2.8/pyyeti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/scripts/lsop2` & `pyyeti-1.2.8/scripts/lsop2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/setup.py` & `pyyeti-1.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         )
     else:
         kw = {}
 
     install_requires = check_dependencies()
     setup(
         name="pyyeti",
-        version="1.2.6",
+        version="1.2.8",
         url="http://github.com/twmacro/pyyeti/",
         license="BSD",
         author="Tim Widrick",
         install_requires=install_requires,
         author_email="twmacro@gmail.com",
         description=("Tools mostly related to structural dynamics"),
         long_description=long_description,
```

### Comparing `pyyeti-1.2.6/tests/nas2cam_csuper/inboard.asm` & `pyyeti-1.2.8/tests/nas2cam_csuper/inboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nas2cam_csuper/inboard.op4` & `pyyeti-1.2.8/tests/nas2cam_csuper/inboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nas2cam_csuper/inboard.pch` & `pyyeti-1.2.8/tests/nas2cam_csuper/inboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nas2cam_csuper/nas2cam.op2` & `pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nas2cam_csuper/nas2cam.op4` & `pyyeti-1.2.8/tests/nas2cam_csuper/nas2cam.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nastran_drm12/drm12.op2` & `pyyeti-1.2.8/tests/nastran_drm12/drm12.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nastran_drm12/drm12.op4` & `pyyeti-1.2.8/tests/nastran_drm12/drm12.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nastran_drm12/inboard_nas2cam.op2` & `pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.2.6/tests/nastran_drm12/inboard_nas2cam.op4` & `pyyeti-1.2.8/tests/nastran_drm12/inboard_nas2cam.op4`

 * *Files identical despite different names*

