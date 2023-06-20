# Comparing `tmp/siriuspy-2.76.0.tar.gz` & `tmp/siriuspy-2.76.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.76.0.tar", last modified: Fri Jun 16 14:01:11 2023, max compression
+gzip compressed data, was "siriuspy-2.76.1.tar", last modified: Tue Jun 20 14:19:46 2023, max compression
```

## Comparing `siriuspy-2.76.0.tar` & `siriuspy-2.76.1.tar`

### file list

```diff
@@ -1,395 +1,395 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-06-16 14:01:00.000000 siriuspy-2.76.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-16 14:01:00.000000 siriuspy-2.76.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-16 14:01:11.822934 siriuspy-2.76.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-06-16 14:01:00.000000 siriuspy-2.76.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-16 14:01:00.000000 siriuspy-2.76.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:01:11.822934 siriuspy-2.76.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-06-16 14:01:00.000000 siriuspy-2.76.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.786934 siriuspy-2.76.0/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.786934 siriuspy-2.76.0/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.794934 siriuspy-2.76.0/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.794934 siriuspy-2.76.0/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.794934 siriuspy-2.76.0/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/blctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    41443 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    12885 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    16522 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    51761 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)     9798 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    21226 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    29992 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/dvfimgproc/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7611 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    15404 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/meas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20125 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    79298 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7475 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13812 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/test_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    34134 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    46519 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    39936 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.786934 siriuspy-2.76.0/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10089 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.874279 siriuspy-2.76.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-06-20 14:19:38.000000 siriuspy-2.76.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-20 14:19:38.000000 siriuspy-2.76.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-20 14:19:46.870279 siriuspy-2.76.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-06-20 14:19:38.000000 siriuspy-2.76.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-20 14:19:38.000000 siriuspy-2.76.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 14:19:46.874279 siriuspy-2.76.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-06-20 14:19:38.000000 siriuspy-2.76.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/blctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41475 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16522 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51622 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21325 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/dvfimgproc/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7611 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15404 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/meas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20125 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79363 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7475 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13812 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/test_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.850279 siriuspy-2.76.1/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.850279 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.850279 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.854279 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.854279 siriuspy-2.76.1/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46519 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39936 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10089 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.76.0/LICENSE` & `siriuspy-2.76.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/PKG-INFO` & `siriuspy-2.76.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.76.0
+Version: 2.76.1
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.76.0/README.md` & `siriuspy-2.76.1/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/setup.py` & `siriuspy-2.76.1/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/__init__.py` & `siriuspy-2.76.1/siriuspy/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/bsmp/commands.py` & `siriuspy-2.76.1/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/bsmp/constants.py` & `siriuspy-2.76.1/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/bsmp/entities.py` & `siriuspy-2.76.1/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/bsmp/exceptions.py` & `siriuspy-2.76.1/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/bsmp/serial.py` & `siriuspy-2.76.1/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/bsmp/types.py` & `siriuspy-2.76.1/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/callbacks.py` & `siriuspy-2.76.1/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientarch/client.py` & `siriuspy-2.76.1/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientarch/devices.py` & `siriuspy-2.76.1/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientarch/exceptions.py` & `siriuspy-2.76.1/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientarch/pvarch.py` & `siriuspy-2.76.1/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientarch/time.py` & `siriuspy-2.76.1/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/global_config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/clientweb/implementation.py` & `siriuspy-2.76.1/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/csdev.py` & `siriuspy-2.76.1/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/currinfo/csdev.py` & `siriuspy-2.76.1/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.76.1/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/currinfo/main.py` & `siriuspy-2.76.1/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/cycle/__init__.py` & `siriuspy-2.76.1/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.76.1/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/cycle/conn.py` & `siriuspy-2.76.1/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.76.1/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.76.1/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/cycle/main.py` & `siriuspy-2.76.1/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/cycle/util.py` & `siriuspy-2.76.1/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/__init__.py` & `siriuspy-2.76.1/siriuspy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/bbb.py` & `siriuspy-2.76.1/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/blctrl.py` & `siriuspy-2.76.1/siriuspy/devices/blctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/bpm.py` & `siriuspy-2.76.1/siriuspy/devices/bpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,29 +77,29 @@
         'XYPosCal-Sel', 'XYPosCal-Sts',
         'SUMPosCal-Sel', 'SUMPosCal-Sts',
         'QPosCal-Sel', 'QPosCal-Sts',
         )
 
     CONV_NM2UM = 1e-3  # [nm] --> [um]
 
-    def __init__(self, devname, auto_mon=True, ispost_mortem=False):
+    def __init__(self, devname, auto_monitor_mon=True, ispost_mortem=False):
         """."""
         # call base class constructor
         if not _BPMSearch.is_valid_devname(devname):
             raise ValueError(devname + ' is not a valid BPM or PBPM name.')
 
         self._ispost_mortem = ispost_mortem
         properties = {self.get_propname(p) for p in BPM._properties}
 
         if _BPMSearch.is_photon_bpm(devname):
             properties -= {'RFFEAtt-SP', 'RFFEAtt-RB'}
         properties = list(properties)
 
         super().__init__(
-            devname, properties=properties, auto_mon=auto_mon)
+            devname, properties=properties, auto_monitor_mon=auto_monitor_mon)
         self.csdata = _csbpm
 
     def __str__(self):
         """."""
         stg = '################### Summary Status ###################\n'
         stg += 'asyn:\n'
         stg += f'    Enabled: {_csbpm.EnblTyp._fields[self.asyn_state]:s}\n'
@@ -908,15 +908,15 @@
             raise ValueError('Wrong value for devname')
 
         devname = _PVName(devname)
         bpm_names = _BPMSearch.get_names(
             filters={'sec': devname.sec, 'dev': devname.dev})
         self._ispost_mortem = ispost_mortem
         devs = [
-            BPM(dev, auto_mon=False, ispost_mortem=ispost_mortem)
+            BPM(dev, auto_monitor_mon=False, ispost_mortem=ispost_mortem)
             for dev in bpm_names]
 
         super().__init__(devname, devs)
         self._bpm_names = bpm_names
         self._csbpm = devs[0].csdata
         self._initial_timestamps = None
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/currinfo.py` & `siriuspy-2.76.1/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/dcct.py` & `siriuspy-2.76.1/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/device.py` & `siriuspy-2.76.1/siriuspy/devices/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,41 @@
 from ..namesys import SiriusPVName as _SiriusPVName
 
 _DEF_TIMEOUT = 10  # s
 _TINY_INTERVAL = 0.050  # s
 
 
 class Device:
-    """Epics Device."""
+    """Epics Device.
+
+    Parameters
+    ----------
+        devname: str
+            Device name, to be used as PVs prefix.
+        properties: (tuple, list)
+            List of properties, to be used as last part of the PV names.
+        auto_monitor: bool, optional
+            Whether to automatically monitor PVs for changes. Used for PVs
+            that do not end with '-Mon' or 'Data'. Defaults to True.
+        auto_monitor_mon: bool, optional
+            Whether to automatically monitor '-Mon' or 'Data' PVs for changes.
+            Defaults to False (to avoid overloading the client). Set to False
+            when using PV.get_timevars() to know when a PV has been updated.
+    """
 
     CONNECTION_TIMEOUT = _CONN_TIMEOUT
     GET_TIMEOUT = _GET_TIMEOUT
     _properties = ()
 
-    def __init__(self, devname, properties, auto_mon=False):
-        """."""
+    def __init__(
+            self, devname, properties, auto_monitor=True,
+            auto_monitor_mon=False):
         self._properties = properties[:]
-        self._auto_mon = auto_mon
+        self._auto_monitor = auto_monitor
+        self._auto_monitor_mon = auto_monitor_mon
         self._devname, self._pvs = self._create_pvs(devname)
 
     @property
     def devname(self):
         """Return device name."""
         return self._devname
 
@@ -79,15 +96,23 @@
                 set_.add(pvobj.pvname)
         return set_
 
     def set_auto_monitor(self, pvname, value):
         """Set auto_monitor state of individual PVs."""
         if pvname not in self._pvs:
             return False
-        self._pvs[pvname].auto_monitor = int(value)
+        pvobj = self._pvs[pvname]
+        try:
+            # TODO verify need of int
+            pvobj.auto_monitor = int(value)
+        except (_ChannelAccessGetFailure, _CASeverityException):
+            # exceptions raised in a Virtual Circuit Disconnect (192)
+            # event. If the PV IOC goes down, for example.
+            print('Could not set auto_monitor of {}'.format(pvobj.pvname))
+            return False
         return True
 
     def update(self):
         """Update device properties."""
         for pvobj in self._pvs.values():
             pvobj.get()
 
@@ -147,17 +172,17 @@
     def _create_pvs(self, devname):
         if devname:
             devname = _SiriusPVName(devname)
 
         pvs = dict()
         for propty in self._properties:
             pvname = self._get_pvname(devname, propty)
-            # avoid keeping auto_monitor enabled for -Mon PVs as they usually
-            # have a high update rate which can generate a lot of CPU load
-            auto_monitor = self._auto_mon and not pvname.endswith('-Mon')
+            auto_monitor = self._auto_monitor
+            if pvname.endswith(('-Mon', 'Data')):
+                auto_monitor = self._auto_monitor_mon
             in_sim = _Simulation.pv_check(pvname)
             pvclass = _PVSim if in_sim else _PV
             pvs[propty] = pvclass(
                 pvname, auto_monitor=auto_monitor,
                 connection_timeout=Device.CONNECTION_TIMEOUT)
         return devname, pvs
 
@@ -207,19 +232,19 @@
         elif 0 <= int(value) < len(enums):
             self[propty] = value
 
 
 class ProptyDevice(Device):
     """Device with a prefix property name."""
 
-    def __init__(self, devname, propty_prefix, properties):
+    def __init__(self, devname, propty_prefix, properties, **kwargs):
         """."""
         self._propty_prefix = propty_prefix
         # call base class constructor
-        super().__init__(devname, properties=properties)
+        super().__init__(devname, properties=properties, **kwargs)
 
     def _get_pvname(self, devname, propty):
         if devname:
             func = devname.substitute
             pvname = func(propty=self._propty_prefix + propty)
         else:
             pvname = self._propty_prefix + propty
@@ -248,20 +273,20 @@
 
 class DeviceApp(Device):
     """Application Device.
 
     This kind of device groups properties of other devices.
     """
 
-    def __init__(self, properties, devname=None, auto_mon=False):
+    def __init__(self, properties, devname=None, **kwargs):
         """."""
         self._devname_app = devname
 
         # call base class constructor
-        super().__init__(None, properties=properties, auto_mon=auto_mon)
+        super().__init__(None, properties=properties, **kwargs)
 
     @property
     def devname(self):
         """Return application device name."""
         return self._devname_app
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/dvf.py` & `siriuspy-2.76.1/siriuspy/devices/dvf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/egun.py` & `siriuspy-2.76.1/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/energy.py` & `siriuspy-2.76.1/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/fofb.py` & `siriuspy-2.76.1/siriuspy/devices/fofb.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     def __init__(self, devname):
         """Init."""
         # check if device exists
         if devname not in self.DEVICES:
             raise NotImplementedError(devname)
 
         # call base class constructor
-        super().__init__(devname, properties=FOFBCtrlRef._properties)
+        super().__init__(
+            devname, properties=FOFBCtrlRef._properties, auto_monitor_mon=True)
 
     @property
     def refx(self):
         """Reference orbit X."""
         return self['RefOrbX-RB']
 
     @refx.setter
@@ -164,20 +165,17 @@
         """Init."""
         self.dccname = dccname
 
         properties = _DCCDevice._properties
         if 'FMC' in self.dccname:
             properties += _DCCDevice._properties_fmc
 
-        super().__init__(devname, dccname, properties=properties)
-        prop2automon = [
-            'BPMCnt-Mon', 'LinkPartnerCH0-Mon', 'LinkPartnerCH1-Mon',
-            'LinkPartnerCH2-Mon', 'LinkPartnerCH3-Mon']
-        for prop in prop2automon:
-            self.set_auto_monitor(prop, True)
+        super().__init__(
+            devname, dccname, properties=properties,
+            auto_monitor_mon=True)
 
     @property
     def bpm_id(self):
         """BPM Id."""
         return self['BPMId-RB']
 
     @bpm_id.setter
@@ -713,15 +711,15 @@
         """Init."""
         if not psnames:
             chn = _PSSearch.get_psnames({'sec': 'SI', 'dev': 'FCH'})
             cvn = _PSSearch.get_psnames({'sec': 'SI', 'dev': 'FCV'})
             psnames = chn + cvn
         self._psnames = psnames
         self._psdevs = [PowerSupplyFC(psn) for psn in self._psnames]
-        self._psconv = [StrengthConv(psn, 'Ref-Mon', auto_mon=True)
+        self._psconv = [StrengthConv(psn, 'Ref-Mon', auto_monitor_mon=True)
                         for psn in self._psnames]
         super().__init__('SI-Glob:PS-FCHV', self._psdevs + self._psconv)
 
     @property
     def psnames(self):
         """PS name list."""
         return list(self._psnames)
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/ict.py` & `siriuspy-2.76.1/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/idff.py` & `siriuspy-2.76.1/siriuspy/devices/idff.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,18 +230,20 @@
             pparameter=pparameter_value, kparameter=kparameter_value)
         return polarization, pparameter_value, kparameter_value
 
     def _create_devices(self, devname):
         param_auto_mon = False
         devpp = _Device(
             devname=devname,
-            properties=(self._pparametername, ), auto_mon=param_auto_mon)
+            properties=(self._pparametername, ),
+            auto_monitor_mon=param_auto_mon)
         devkp = _Device(
             devname=devname,
-            properties=(self._kparametername, ), auto_mon=param_auto_mon)
+            properties=(self._kparametername, ),
+            auto_monitor_mon=param_auto_mon)
         devsch = [_PowerSupplyFBP(devname=dev) for dev in self.chnames]
         devscv = [_PowerSupplyFBP(devname=dev) for dev in self.cvnames]
         devsqs = [_PowerSupplyFBP(devname=dev) for dev in self.qsnames]
 
         return devpp, devkp, devsch, devscv, devsqs
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/ids.py` & `siriuspy-2.76.1/siriuspy/devices/ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         devname = _SiriusPVName(devname)
 
         # check if device exists
         if devname not in APU.DEVICES.ALL:
             raise NotImplementedError(devname)
 
         # call base class constructor
-        super().__init__(devname, properties=APU._properties, auto_mon=True)
+        super().__init__(
+            devname, properties=APU._properties, auto_monitor_mon=True)
 
     @property
     def phase(self):
         """Return APU phase [mm]."""
         return self['Phase-Mon']
 
     @phase.setter
@@ -132,26 +133,26 @@
         'Phase-SP', 'Phase-RB', 'Phase-Mon',
         'PhaseSpeed-SP', 'PhaseSpeed-RB', 'PhaseSpeed-Mon',
         'MaxPhaseSpeed-SP', 'MaxPhaseSpeed-RB',
         'StopPhase-Cmd', 'ChangePhase-Cmd',
         'Log-Mon',
         )
 
-
-    def __init__(self, devname, properties=None, auto_mon=True):
+    def __init__(self, devname, properties=None, auto_monitor_mon=True):
         """."""
         devname = _SiriusPVName(devname)
 
         # check if device exists
         if devname not in self.DEVICES.ALL:
             raise NotImplementedError(devname)
 
         # call base class constructor
         properties = properties or self._properties + self._properties_papu
-        super().__init__(devname, properties=properties, auto_mon=auto_mon)
+        super().__init__(
+            devname, properties=properties, auto_monitor_mon=auto_monitor_mon)
 
     @property
     def period_length(self):
         """Return ID period length [mm]."""
         return self['PeriodLength-Cte']
 
     @property
@@ -454,15 +455,16 @@
         devname = _SiriusPVName(devname)
 
         # check if device exists
         if devname not in EPU.DEVICES.ALL:
             raise NotImplementedError(devname)
 
         # call base class constructor
-        super().__init__(devname, properties=self._properties, auto_mon=True)
+        super().__init__(
+            devname, properties=self._properties, auto_monitor_mon=True)
 
     @property
     def status(self):
         """ID status."""
         return self['Status-Mon']
 
     # --- gap speeds ----
@@ -692,8 +694,9 @@
         devname = _SiriusPVName(devname)
 
         # check if device exists
         if devname not in WIG.DEVICES.ALL:
             raise NotImplementedError(devname)
 
         # call base class constructor
-        super().__init__(devname, properties=WIG._properties, auto_mon=True)
+        super().__init__(
+            devname, properties=WIG._properties, auto_monitor_mon=True)
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/injctrl.py` & `siriuspy-2.76.1/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/injsys.py` & `siriuspy-2.76.1/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/lienergy.py` & `siriuspy-2.76.1/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/lillrf.py` & `siriuspy-2.76.1/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/machshift.py` & `siriuspy-2.76.1/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/modltr.py` & `siriuspy-2.76.1/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.76.1/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/posang.py` & `siriuspy-2.76.1/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/psconv.py` & `siriuspy-2.76.1/siriuspy/devices/psconv.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,24 +14,25 @@
         # devices which are mapped to more than one device
         'BO-Fam:PS-B-1': ('BO-Fam:PS-B-1', 'BO-Fam:PS-B-2'),
         'BO-Fam:PS-B-2': ('BO-Fam:PS-B-1', 'BO-Fam:PS-B-2'),
         'SI-Fam:PS-B1B2-1': ('SI-Fam:PS-B1B2-1', 'SI-Fam:PS-B1B2-2'),
         'SI-Fam:PS-B1B2-2': ('SI-Fam:PS-B1B2-1', 'SI-Fam:PS-B1B2-2'),
         }
 
-    def __init__(self, devname, propty, auto_mon=False):
+    def __init__(self, devname, propty, auto_monitor_mon=False):
         """."""
         devname = _SiriusPVName(devname)
 
         # get devnames
         devnames = PSProperty._get_devnames(devname)
 
         # call base class constructor
         super().__init__(
-            devnames=devnames, propty_sync=[propty], auto_mon=auto_mon)
+            devnames=devnames, propty_sync=[propty],
+            auto_monitor_mon=auto_monitor_mon)
 
     @property
     def property_sync(self):
         """Return sole synchonized property name of device."""
         return self.properties_sync[0]
 
     @property
@@ -74,27 +75,27 @@
             return PSProperty._ps2devs[devname]
         return (devname, )
 
 
 class StrengthConv(_Devices):
     """Strength Converter."""
 
-    # TODO: Test changing default value of auto_mon to see if conversion
-    # IOCs are improved.
+    # TODO: Test changing default value of auto_monitor_mon
+    # to see if conversion IOCs are improved.
 
-    def __init__(self, devname, proptype, auto_mon=False):
+    def __init__(self, devname, proptype, auto_monitor_mon=False):
         """."""
         devname = _SiriusPVName(devname)
 
         # get pwrsupply normalized
         self._norm_mag = self._create_normalizer(devname)
 
         # get devices that provide normalization current for strengths
         self._dev_dip, self._dev_fam = \
-            self._get_devices(devname, proptype, auto_mon)
+            self._get_devices(devname, proptype, auto_monitor_mon)
         if self._dev_fam:
             devices = (self._dev_dip, self._dev_fam)
         elif self._dev_dip:
             devices = (self._dev_dip, )
         else:
             devices = ()
 
@@ -180,37 +181,37 @@
             norm_mag = _NormalizerFactory.create('SI-Fam:MA-B1B2')
         else:
             maname = psname.replace(':PS', ':MA').replace(':PU', ':PM')
             norm_mag = _NormalizerFactory.create(maname)
         return norm_mag
 
     @staticmethod
-    def _get_devices(devname, proptype, auto_mon):
+    def _get_devices(devname, proptype, auto_monitor_mon):
         # is dipole?
         if StrengthConv._get_dev_if_dipole(devname):
             return None, None
 
         # is insertion device?
         if StrengthConv._get_dev_if_id(devname):
             return None, None
 
         # is trim?
         status, dev_dip, dev_fam = \
-            StrengthConv._get_dev_if_trim(devname, proptype, auto_mon)
+            StrengthConv._get_dev_if_trim(devname, proptype, auto_monitor_mon)
         if status:
             return dev_dip, dev_fam
 
         # is booster ps?
         status, dev_dip = StrengthConv._get_dev_if_booster(
-            devname, proptype, auto_mon)
+            devname, proptype, auto_monitor_mon)
         if status:
             return dev_dip, None
 
         # is others
-        return StrengthConv._get_dev_others(devname, proptype, auto_mon), None
+        return StrengthConv._get_dev_others(devname, proptype, auto_monitor_mon), None
 
     @staticmethod
     def _get_dev_if_dipole(devname):
         if devname.dev in {'B', 'B1B2'}:
             # dipoles need no connectors
             return True
         return False
@@ -219,60 +220,74 @@
     def _get_dev_if_id(devname):
         if devname.dis == 'ID':
             # insertion devices need no connectors
             return True
         return False
 
     @staticmethod
-    def _get_dev_if_trim(devname, proptype, auto_mon):
+    def _get_dev_if_trim(devname, proptype, auto_monitor_mon):
         if StrengthConv._is_trim(devname):
             # trims need dipole and family connectors
             dev_dip = PSProperty(
-                'SI-Fam:PS-B1B2-1', 'Energy' + proptype, auto_mon)
+                'SI-Fam:PS-B1B2-1', 'Energy' + proptype,
+                auto_monitor_mon=auto_monitor_mon)
             devname = devname.substitute(sub='Fam')
-            dev_fam = PSProperty(devname, 'KL' + proptype, auto_mon)
+            dev_fam = PSProperty(
+                devname, 'KL' + proptype, auto_monitor_mon=auto_monitor_mon)
             return True, dev_dip, dev_fam
         return False, None, None
 
     @staticmethod
-    def _get_dev_if_booster(devname, proptype, auto_mon):
+    def _get_dev_if_booster(devname, proptype, auto_monitor_mon):
         if devname.startswith('BO'):
             if devname.dev == 'InjKckr':
                 # BO injection kicker uses TB dipole normalizer
                 dev_dip = PSProperty(
-                    'TB-Fam:PS-B', 'Energy' + proptype, auto_mon)
+                    'TB-Fam:PS-B', 'Energy' + proptype,
+                    auto_monitor_mon=auto_monitor_mon)
             elif devname.dev == 'EjeKckr':
                 # BO ejection kicker uses TS dipole normalizer
                 dev_dip = PSProperty(
-                    'TS-Fam:PS-B', 'Energy' + proptype, auto_mon)
+                    'TS-Fam:PS-B', 'Energy' + proptype,
+                    auto_monitor_mon=auto_monitor_mon)
             else:
                 # other BO ps use BO dipoles as normalizer
                 dev_dip = PSProperty(
-                    'BO-Fam:PS-B-1', 'Energy' + proptype, auto_mon)
+                    'BO-Fam:PS-B-1', 'Energy' + proptype,
+                    auto_monitor_mon=auto_monitor_mon)
             return True, dev_dip
         return False, None
 
     @staticmethod
-    def _get_dev_others(devname, proptype, auto_mon):
+    def _get_dev_others(devname, proptype, auto_monitor_mon):
         if devname.startswith('LI'):
-            return PSProperty('TB-Fam:PS-B', 'Energy' + proptype, auto_mon)
+            return PSProperty(
+                'TB-Fam:PS-B', 'Energy' + proptype,
+                auto_monitor_mon=auto_monitor_mon)
         if devname.startswith('TB'):
             # all TB ps other than dipoles need dipole connectors
-            return PSProperty('TB-Fam:PS-B', 'Energy' + proptype, auto_mon)
+            return PSProperty(
+                'TB-Fam:PS-B', 'Energy' + proptype,
+                auto_monitor_mon=auto_monitor_mon)
         elif devname.startswith('TS'):
             # all TS ps use TS dipole
-            return PSProperty('TS-Fam:PS-B', 'Energy' + proptype, auto_mon)
+            return PSProperty(
+                'TS-Fam:PS-B', 'Energy' + proptype,
+                auto_monitor_mon=auto_monitor_mon)
         elif devname.startswith('SI'):
             if devname.dev in {'InjDpKckr', 'InjNLKckr'}:
                 # SI injection ps use TS dipole
-                return PSProperty('TS-Fam:PS-B', 'Energy' + proptype, auto_mon)
+                return PSProperty(
+                    'TS-Fam:PS-B', 'Energy' + proptype,
+                    auto_monitor_mon=auto_monitor_mon)
             else:
                 # other SI ps use SI dipole
                 return PSProperty(
-                    'SI-Fam:PS-B1B2-1', 'Energy' + proptype, auto_mon)
+                    'SI-Fam:PS-B1B2-1', 'Energy' + proptype,
+                    auto_monitor_mon=auto_monitor_mon)
         return None
 
     @staticmethod
     def _is_trim(psname):
         check = (psname.sec == 'SI')
         check &= (psname.sub != 'Fam')
         check &= 'QS' not in psname.dev
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/pssofb.py` & `siriuspy-2.76.1/siriuspy/devices/pssofb.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     _properties = (
         _curr_sp,
         _curr_rb,
         _curr_refmon,
         _curr_mon)
 
-    def __init__(self, devname, auto_mon=False):
+    def __init__(self, devname, auto_monitor_mon=False):
         """."""
         self._devname_orig = _SiriusPVName(devname)
         self._sec = self._devname_orig.sec
 
         # check if device exists and is a SOFB corrector
         if devname not in PSNamesSOFB.get_psnames_ch(self._sec) and \
                 devname not in PSNamesSOFB.get_psnames_cv(self._sec):
@@ -67,15 +67,16 @@
         # get bbbname and linked bsmp devices
         self._bbbname = _PSSearch.conv_psname_2_bbbname(devname)
         self._bsmpdevs = _PSSearch.conv_bbbname_2_bsmps(self._bbbname)
 
         # call base class constructor
         devname = self._bsmpdevs[0][0]
         super().__init__(
-            devname, properties=PSCorrSOFB._properties, auto_mon=auto_mon)
+            devname, properties=PSCorrSOFB._properties,
+            auto_monitor_mon=auto_monitor_mon)
 
         # get sofb indices
         self._sofb_indices, self._idx_corr = self._get_sofb_indices()
 
     @property
     def devname(self):
         """Device name."""
@@ -190,26 +191,27 @@
     class DEVICES:
         """."""
 
         BO = 'BO'
         SI = 'SI'
         ALL = (BO, SI)
 
-    def __init__(self, devname, auto_mon=False, dipoleoff=False):
+    def __init__(self, devname, auto_monitor_mon=False, dipoleoff=False):
         """."""
         # check if device exists
         if devname not in PSApplySOFB.DEVICES.ALL:
             raise NotImplementedError(devname)
 
         # get devices
-        devices = PSApplySOFB._get_pscorrsofb_devices(devname, auto_mon)
+        devices = PSApplySOFB._get_pscorrsofb_devices(
+            devname, auto_monitor_mon)
 
         # strengthconv dictionaries
         self._pstype_2_index, self._pstype_2_sconv = \
-            self._get_strenconv(devname, auto_mon)
+            self._get_strenconv(devname, auto_monitor_mon)
 
         # add StrengthConv devices
         devices += self._pstype_2_sconv.values()
 
         # call base class constructor
         super().__init__(devname, devices=devices)
 
@@ -348,44 +350,45 @@
                     strengths=value[idcs], strengths_dipole=3.0)
             else:
                 curr = sconv.conv_strength_2_current(strengths=value[idcs])
             current[index[idcs]] = curr
         return current
 
     @staticmethod
-    def _get_pscorrsofb_devices(devname, auto_mon):
+    def _get_pscorrsofb_devices(devname, auto_monitor_mon):
         psnames = PSNamesSOFB.get_psnames_ch(devname) + \
             PSNamesSOFB.get_psnames_cv(devname)
         devices = dict()
         all_devices = list()
         for psname in psnames:
             if psname in all_devices:
                 continue
-            sofb_corr = PSCorrSOFB(psname, auto_mon)
+            sofb_corr = PSCorrSOFB(psname, auto_monitor_mon)
             all_devices += [dev[0] for dev in sofb_corr.bsmpdevs]
             devname = sofb_corr.devname_first_udc
             if devname not in devices:
                 devices[devname] = sofb_corr
         return list(devices.values())
 
-    def _get_strenconv(self, devname, auto_mon):
+    def _get_strenconv(self, devname, auto_monitor_mon):
         # 1. create pstype to StrengthConv dictionary.
         # 2. create pstype to corrector index dictionnary.
         pstype_2_index = dict()
         pstype_2_sconv = dict()
         psnames = PSNamesSOFB.get_psnames_ch(devname) + \
             PSNamesSOFB.get_psnames_cv(devname)
         for i, psname in enumerate(psnames):
             pstype = _PSSearch.conv_psname_2_pstype(psname)
             if pstype not in pstype_2_index:
                 pstype_2_index[pstype] = []
             pstype_2_index[pstype].append(i)
             if pstype not in pstype_2_sconv:
                 sconv = _StrengthConv(
-                    psname, PSApplySOFB._dipole_propty, auto_mon)
+                    psname, PSApplySOFB._dipole_propty,
+                    auto_monitor_mon=auto_monitor_mon)
                 pstype_2_sconv[pstype] = sconv
 
         # convert index to numpy array
         for pstype in pstype_2_index:
             pstype_2_index[pstype] = _np.asarray(pstype_2_index[pstype])
 
         return pstype_2_index, pstype_2_sconv
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/pstesters.py` & `siriuspy-2.76.1/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/pwrsupply.py` & `siriuspy-2.76.1/siriuspy/devices/pwrsupply.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     )
     _properties_pulsed_kckr = _properties_pulsed_sept + ('Intlk8-Mon', )
     _properties_pulsed_nlkckr = _properties_pulsed_kckr + (
         'CCoilHVoltage-SP', 'CCoilHVoltage-RB', 'CCoilHVoltage-Mon',
         'CCoilVVoltage-SP', 'CCoilVVoltage-RB', 'CCoilVVoltage-Mon',
     )
 
-    def __init__(self, devname):
+    def __init__(self, devname, auto_monitor_mon=False):
         """."""
         devname = _SiriusPVName(devname)
 
         # check if device exists
         if devname not in _PSSearch.get_psnames():
             raise NotImplementedError(devname)
 
@@ -92,15 +92,16 @@
         # set attributes
         (self._strength_sp_propty,
          self._strength_rb_propty,
          self._strength_mon_propty,
          properties) = self._set_attributes_properties(devname)
 
         # call base class constructor
-        super().__init__(devname, properties=properties)
+        super().__init__(
+            devname, properties=properties, auto_monitor_mon=auto_monitor_mon)
 
         # private attribute with strength setpoint pv object
         self._strength_sp_pv = self.pv_object(self._strength_sp_propty)
 
     @property
     def pstype(self):
         """Return type of magnet(s) excited by power supply device."""
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/rf.py` & `siriuspy-2.76.1/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/screen.py` & `siriuspy-2.76.1/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/sofb.py` & `siriuspy-2.76.1/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/syncd.py` & `siriuspy-2.76.1/siriuspy/devices/syncd.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 
 
 class DevicesSync(_DeviceApp):
     """Synchronized devices."""
 
     def __init__(
             self, devnames, propty_sync, propty_async=None,
-            devname=None, auto_mon=False):
+            devname=None, auto_monitor_mon=False):
         """."""
         self._devnames = [_SiriusPVName(dev) for dev in devnames]
         self._props_sync = list(propty_sync)
         self._props_async = [] if propty_async is None else propty_async
 
         # get properties
         properties, self._prop2prop = self._get_properties()
 
         # call base class constructor
-        super().__init__(properties, devname, auto_mon)
+        super().__init__(
+            properties, devname, auto_monitor_mon=auto_monitor_mon)
 
     @property
     def devnames(self):
         """Return device names."""
         return self._devnames
 
     @property
```

### Comparing `siriuspy-2.76.0/siriuspy/devices/timing.py` & `siriuspy-2.76.1/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/devices/tune.py` & `siriuspy-2.76.1/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.76.1/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.76.1/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.76.1/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.76.1/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.76.1/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/app.py` & `siriuspy-2.76.1/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.76.1/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.76.1/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.76.1/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.76.1/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.76.1/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.76.1/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.76.1/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.76.1/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.76.1/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/pvs.py` & `siriuspy-2.76.1/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.76.1/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.76.1/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.76.1/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/dvfimgproc/csdev.py` & `siriuspy-2.76.1/siriuspy/dvfimgproc/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/dvfimgproc/main.py` & `siriuspy-2.76.1/siriuspy/dvfimgproc/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/dvfimgproc/meas.py` & `siriuspy-2.76.1/siriuspy/dvfimgproc/meas.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/envars.py` & `siriuspy-2.76.1/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/epics/multiproc.py` & `siriuspy-2.76.1/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/epics/properties.py` & `siriuspy-2.76.1/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/epics/pv_fake.py` & `siriuspy-2.76.1/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.76.1/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/fofb/csdev.py` & `siriuspy-2.76.1/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/fofb/main.py` & `siriuspy-2.76.1/siriuspy/fofb/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,37 +101,37 @@
         }
         self._kick_mon = {}
         size = len(self._corrs_dev.psdevs)
         for propty in self._propty2kickpvs:
             self._kick_mon[propty] = _np.zeros(size, dtype=float)
             for idx, pso in enumerate(self._corrs_dev.psdevs):
                 pvo = pso.pv_object(propty)
-                pvo.auto_monitor = _epics.dbr.DBE_VALUE
+                pvo.set_auto_monitor(True)
                 pvo.add_callback(
-                    _part(self._update_kick_array, ps_index=idx))
+                    _part(self._update_kick_array, ps_index=idx),
+                    with_ctrlvars=False)
 
         self._rf_dev = _RFGen()
 
         self._llfofb_dev = _FamFOFBCtrls()
 
         self._intlk_pvs = list()
         self._intlk_values = dict()
         for dev in self._llfofb_dev.ctrlrefdevs.values():
             pvo = dev.pv_object('LoopIntlk-Mon')
             self._intlk_values[pvo.pvname] = 0
-            pvo.auto_monitor = True
-            pvo.add_callback(self._callback_loopintlk)
+            pvo.add_callback(
+                self._callback_loopintlk, with_ctrlvars=False)
             self._intlk_pvs.append(pvo)
 
         self._corrs_dev.wait_for_connection(self._const.DEF_TIMEWAIT)
 
         self._auxbpm = _Device(
             'SI-01M1:DI-BPM',
-            properties=('INFOFOFBRate-RB', 'INFOMONITRate-RB'),
-            auto_mon=False)
+            properties=('INFOFOFBRate-RB', 'INFOMONITRate-RB'))
 
         havebeam_pvname = _PVName(
             'SI-Glob:AP-CurrInfo:StoredEBeam-Mon').substitute(
                 prefix=_vaca_prefix)
         self._havebeam_pv = _PV(
             havebeam_pvname, connection_timeout=0.05,
             callback=self._callback_havebeam)
@@ -271,37 +271,38 @@
             'MeasRespMatWait-SP': self._meas_respmat_wait,
             'MeasRespMatWait-RB': self._meas_respmat_wait,
         }
         for pvn, val in pvn2vals.items():
             self.run_callbacks(pvn, val)
 
         # load autosave data
+        # enable lists
+        for dev in ['bpmx', 'bpmy', 'ch', 'cv', 'rf']:
+            okl = self._load_enbllist(dev)
+            pvn = f'{dev.upper()}EnblList-SP' if dev != 'rf' else 'UseRF-Sel'
+            enb = self._enable_lists[dev]
+            pvv = enb if dev != 'rf' else bool(enb)
+            self.run_callbacks(pvn, pvv)
+            if not okl:
+                self.run_callbacks(
+                    pvn.replace('SP', 'RB').replace('Sel', 'Sts'), pvv)
+        self._update_fofbctrl_sync_enbllist()
         # matrix
         okm = self._load_respmat()
         self.run_callbacks('RespMat-SP', list(self._respmat.ravel()))
         if not okm:
             self.run_callbacks('RespMat-RB', list(self._respmat.ravel()))
         # ref orbits
         okr = self._load_reforbit()
         for plan in ['x', 'y']:
             pvn = f'RefOrb{plan.upper()}-SP'
             pvv = getattr(self, f'_reforb_{plan}')
             self.run_callbacks(pvn, pvv)
             if not okr:
                 self.run_callbacks(pvn.replace('SP', 'RB'), pvv)
-        # enable lists
-        for dev in ['bpmx', 'bpmy', 'ch', 'cv', 'rf']:
-            okl = self._load_enbllist(dev)
-            pvn = f'{dev.upper()}EnblList-SP' if dev != 'rf' else 'UseRF-Sel'
-            enb = self._enable_lists[dev]
-            pvv = enb if dev != 'rf' else bool(enb)
-            self.run_callbacks(pvn, pvv)
-            if not okl:
-                self.run_callbacks(
-                    pvn.replace('SP', 'RB').replace('Sel', 'Sts'), pvv)
         self._update_log('Started.')
         self._init = True
 
     @property
     def pvs_database(self):
         """Return pvs_database."""
         return self._pvs_database
@@ -1121,22 +1122,23 @@
         bkup = self._enable_lists[device]
         new = _np.array(value, dtype=bool)
         if bkup.size != new.size:
             self._update_log(
                 'ERR: Wrong {0:s} EnblList size.'.format(device.upper()))
             return False
 
-        # check if matrix is invertible
         self._enable_lists[device] = new
-        if not self._calc_matrices():
-            self._enable_lists[device] = bkup
-            return False
 
         # do not set enable lists and save to file in initialization
         if self._init:
+            # check if matrix is invertible
+            if not self._calc_matrices():
+                self._enable_lists[device] = bkup
+                return False
+
             # handle devices enable configuration
             self._thread_enbllist = _epics.ca.CAThread(
                 target=self._handle_devices_enblconfig, args=[device, ],
                 daemon=True)
             self._thread_enbllist.start()
 
             # save to autosave files
```

### Comparing `siriuspy-2.76.0/siriuspy/idff/config.py` & `siriuspy-2.76.1/siriuspy/idff/config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/idff/csdev.py` & `siriuspy-2.76.1/siriuspy/idff/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/idff/main.py` & `siriuspy-2.76.1/siriuspy/idff/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.76.1/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/injctrl/csdev.py` & `siriuspy-2.76.1/siriuspy/injctrl/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/injctrl/main.py` & `siriuspy-2.76.1/siriuspy/injctrl/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/machshift/csdev.py` & `siriuspy-2.76.1/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/machshift/macreport.py` & `siriuspy-2.76.1/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/machshift/macschedule.py` & `siriuspy-2.76.1/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/machshift/main.py` & `siriuspy-2.76.1/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/machshift/test_macreport.py` & `siriuspy-2.76.1/siriuspy/machshift/test_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/machshift/utils.py` & `siriuspy-2.76.1/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/magnet/data.py` & `siriuspy-2.76.1/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/magnet/excdata.py` & `siriuspy-2.76.1/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/magnet/factory.py` & `siriuspy-2.76.1/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/magnet/normalizer.py` & `siriuspy-2.76.1/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/magnet/util.py` & `siriuspy-2.76.1/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/meas/csdev.py` & `siriuspy-2.76.1/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.76.1/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/meas/liemit/main.py` & `siriuspy-2.76.1/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.76.1/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/meas/lienergy/main.py` & `siriuspy-2.76.1/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/meas/util.py` & `siriuspy-2.76.1/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/namesys/implementation.py` & `siriuspy-2.76.1/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/optics/lattice_survey.py` & `siriuspy-2.76.1/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/opticscorr/base.py` & `siriuspy-2.76.1/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/opticscorr/chrom.py` & `siriuspy-2.76.1/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/opticscorr/csdev.py` & `siriuspy-2.76.1/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.76.1/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/opticscorr/tune.py` & `siriuspy-2.76.1/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/opticscorr/utils.py` & `siriuspy-2.76.1/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.76.1/siriuspy/oscilloscope/keysight.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.76.1/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/posang/csdev.py` & `siriuspy-2.76.1/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/posang/main.py` & `siriuspy-2.76.1/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/posang/utils.py` & `siriuspy-2.76.1/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/data.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/factory.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/pssofb.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             pstype = _PSSearch.conv_psname_2_pstype(psname)
             if pstype not in pstype_2_index:
                 pstype_2_index[pstype] = []
             pstype_2_index[pstype].append(i)
             if pstype not in pstype_2_sconv:
                 # sconv = _NormFact.create(psname.replace(':PS', ':MA'))
                 sconv = _StrengthConv(
-                    psname, UnitConverter.DIPOLE_PROPTY, auto_mon=True)
+                    psname, UnitConverter.DIPOLE_PROPTY, auto_monitor_mon=True)
                 pstype_2_sconv[pstype] = sconv
 
         # convert index to numpy array
         for pstype in pstype_2_index:
             pstype_2_index[pstype] = _np.asarray(pstype_2_index[pstype])
 
         # wait for connection
```

### Comparing `siriuspy-2.76.0/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.76.1/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/conn.py` & `siriuspy-2.76.1/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/magnet.py` & `siriuspy-2.76.1/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/ramp.py` & `siriuspy-2.76.1/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.76.1/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.76.1/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/testwfm.py` & `siriuspy-2.76.1/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/util.py` & `siriuspy-2.76.1/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/ramp/waveform.py` & `siriuspy-2.76.1/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/search/bpms_search.py` & `siriuspy-2.76.1/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/search/hl_time_search.py` & `siriuspy-2.76.1/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/search/id_search.py` & `siriuspy-2.76.1/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/search/ioc_search.py` & `siriuspy-2.76.1/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/search/ll_time_search.py` & `siriuspy-2.76.1/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/search/ma_search.py` & `siriuspy-2.76.1/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/search/ps_search.py` & `siriuspy-2.76.1/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/simul/simfactory.py` & `siriuspy-2.76.1/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/simul/simps.py` & `siriuspy-2.76.1/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/simul/simpv.py` & `siriuspy-2.76.1/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/simul/simulation.py` & `siriuspy-2.76.1/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/simul/simulator.py` & `siriuspy-2.76.1/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/base_class.py` & `siriuspy-2.76.1/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/bpms.py` & `siriuspy-2.76.1/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/correctors.py` & `siriuspy-2.76.1/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/csdev.py` & `siriuspy-2.76.1/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/main.py` & `siriuspy-2.76.1/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/matrix.py` & `siriuspy-2.76.1/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/orbit.py` & `siriuspy-2.76.1/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/sofb/utils.py` & `siriuspy-2.76.1/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/stabinfo/csdev.py` & `siriuspy-2.76.1/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/stabinfo/main.py` & `siriuspy-2.76.1/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/thread.py` & `siriuspy-2.76.1/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/timesys/csdev.py` & `siriuspy-2.76.1/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/timesys/hl_classes.py` & `siriuspy-2.76.1/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/timesys/ll_classes.py` & `siriuspy-2.76.1/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/timesys/plot_network.py` & `siriuspy-2.76.1/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/timesys/static_table.py` & `siriuspy-2.76.1/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy/util.py` & `siriuspy-2.76.1/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.76.1/siriuspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.76.0
+Version: 2.76.1
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.76.0/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.76.1/siriuspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/bsmp/test_bsmp.py` & `siriuspy-2.76.1/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/bsmp/test_commands.py` & `siriuspy-2.76.1/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/bsmp/test_entities.py` & `siriuspy-2.76.1/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/bsmp/test_serial.py` & `siriuspy-2.76.1/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/bsmp/test_types.py` & `siriuspy-2.76.1/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.76.1/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/clientweb/test_implementation.py` & `siriuspy-2.76.1/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.76.1/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/currinfo/test_csdev.py` & `siriuspy-2.76.1/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/currinfo/test_main.py` & `siriuspy-2.76.1/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/magnet/test_factory.py` & `siriuspy-2.76.1/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/magnet/tests_normalizer.py` & `siriuspy-2.76.1/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/mock_servweb.py` & `siriuspy-2.76.1/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/namesys/test_implementation.py` & `siriuspy-2.76.1/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/opticscorr/test_chrom.py` & `siriuspy-2.76.1/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/opticscorr/test_csdev.py` & `siriuspy-2.76.1/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.76.1/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/opticscorr/test_tune.py` & `siriuspy-2.76.1/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/opticscorr/test_utils.py` & `siriuspy-2.76.1/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/posang/test_csdev.py` & `siriuspy-2.76.1/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/posang/test_main.py` & `siriuspy-2.76.1/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/pwrsupply/db.py` & `siriuspy-2.76.1/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.76.1/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.76.1/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/pwrsupply/test_csdev.py` & `siriuspy-2.76.1/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/pwrsupply/test_data.py` & `siriuspy-2.76.1/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/pwrsupply/test_siggen.py` & `siriuspy-2.76.1/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/pwrsupply/variables.py` & `siriuspy-2.76.1/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/ramp/test_magnet.py` & `siriuspy-2.76.1/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/ramp/test_waveform.py` & `siriuspy-2.76.1/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/search/test_hl_time_search.py` & `siriuspy-2.76.1/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/search/test_init.py` & `siriuspy-2.76.1/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/search/test_ll_time_search.py` & `siriuspy-2.76.1/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/search/test_ma_search.py` & `siriuspy-2.76.1/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/search/test_ps_search.py` & `siriuspy-2.76.1/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/test_callbacks.py` & `siriuspy-2.76.1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/test_csdev.py` & `siriuspy-2.76.1/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/test_envars.py` & `siriuspy-2.76.1/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/test_util.py` & `siriuspy-2.76.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/timesys/test_csdev.py` & `siriuspy-2.76.1/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.0/tests/timesys/test_plot_network.py` & `siriuspy-2.76.1/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

