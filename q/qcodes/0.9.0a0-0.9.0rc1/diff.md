# Comparing `tmp/qcodes-0.9.0a0.tar.gz` & `tmp/qcodes-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcodes-0.9.0a0.tar", last modified: Fri Dec  6 09:50:09 2019, max compression
+gzip compressed data, was "dist/qcodes-0.9.0rc1.tar", last modified: Tue Dec 10 09:11:20 2019, max compression
```

## Comparing `qcodes-0.9.0a0.tar` & `qcodes-0.9.0rc1.tar`

### file list

```diff
@@ -1,520 +1,520 @@
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/
--rw-r--r--   0 vsts      (1001) docker     (117)       49 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (117)     4940 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)     3383 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/
--rw-r--r--   0 vsts      (1001) docker     (117)     4068 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)      499 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/_version.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6949 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/actions.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/config/
--rw-r--r--   0 vsts      (1001) docker     (117)       83 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    15892 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/config/config.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2132 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/config/qcodesrc.json
--rw-r--r--   0 vsts      (1001) docker     (117)    13703 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/config/qcodesrc_schema.json
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/data/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    19667 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/data/data_array.py
--rw-r--r--   0 vsts      (1001) docker     (117)    26514 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/data/data_set.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13413 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/data/format.py
--rw-r--r--   0 vsts      (1001) docker     (117)    17385 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/data/gnuplot_format.py
--rw-r--r--   0 vsts      (1001) docker     (117)    23206 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/data/hdf5_format.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2474 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/data/hdf5_format_hickle.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8697 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/data/io.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6537 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/data/location.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dataset/
--rw-r--r--   0 vsts      (1001) docker     (117)      246 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13537 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/data_export.py
--rw-r--r--   0 vsts      (1001) docker     (117)    52509 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/data_set.py
--rw-r--r--   0 vsts      (1001) docker     (117)      673 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/database.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11193 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/database_extract_runs.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5864 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/database_fix_functions.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/
--rw-r--r--   0 vsts      (1001) docker     (117)      390 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20259 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/dependencies.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8943 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/param_spec.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2096 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/rundescriber.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/
--rw-r--r--   0 vsts      (1001) docker     (117)      255 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4721 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/converters.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4642 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3521 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/v0.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11617 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/experiment_container.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5647 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/guids.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2063 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/json_exporter.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4122 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/legacy_import.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dataset/linked_datasets/
--rw-r--r--   0 vsts      (1001) docker     (117)      103 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/linked_datasets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2201 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/linked_datasets/links.py
--rw-r--r--   0 vsts      (1001) docker     (117)    48869 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/measurements.py
--rw-r--r--   0 vsts      (1001) docker     (117)    30119 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/plotting.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/
--rw-r--r--   0 vsts      (1001) docker     (117)      553 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5564 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/connection.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10310 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/database.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/
--rw-r--r--   0 vsts      (1001) docker     (117)    11909 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8517 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/upgrade_2_to_3.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3450 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/upgrade_3_to_4.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1732 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/upgrade_5_to_6.py
--rw-r--r--   0 vsts      (1001) docker     (117)      422 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/version.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2241 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/initial_schema.py
--rw-r--r--   0 vsts      (1001) docker     (117)    57987 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/queries.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10296 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/query_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2969 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite/settings.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2998 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/dataset/sqlite_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dist/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dist/schemas/
--rw-r--r--   0 vsts      (1001) docker     (117)     8605 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dist/schemas/station-template.schema.json
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dist/tests/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/dist/tests/station/
--rw-r--r--   0 vsts      (1001) docker     (117)     1743 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/dist/tests/station/example.station.yaml
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    30848 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/base.py
--rw-r--r--   0 vsts      (1001) docker     (117)    34121 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/channel.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5351 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/function.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11138 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/group_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8643 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/ip.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3609 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/ip_to_visa.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument/mockers/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/mockers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7218 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/mockers/ami430.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4073 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/mockers/simulated_ats_api.py
--rw-r--r--   0 vsts      (1001) docker     (117)   100465 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/parameter.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument/sims/
--rw-r--r--   0 vsts      (1001) docker     (117)     2909 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/instrument/sims/AMI430.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      411 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/AimTTi_PL601P.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1324 2019-12-06 09:30:49.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Keithley_2450.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     4560 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Keithley_2600.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1474 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Keithley_s46.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      974 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Keysight_33xxx.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     2540 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Keysight_34465A.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      286 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Keysight_N6705B.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     2632 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument/sims/MercuryiPS.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      462 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/RSHMC804x.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1098 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/RTO_1000.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1195 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Rigol_DS1074Z.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1821 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Tektronix_AWG5014C.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      498 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Tektronix_AWG5208.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      884 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Tektronix_AWG70000A.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     2209 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/Tektronix_DPO7200xx.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)        5 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)      749 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (117)      403 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument/sims/dummy.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1186 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sims/keysight_34980A.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1568 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/instrument/sims/keysight_b1500.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     3760 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument/sims/keysight_b220x.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     3332 2019-12-06 09:30:34.000000 qcodes-0.9.0a0/qcodes/instrument/sims/lakeshore_model336.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      238 2019-12-06 09:30:34.000000 qcodes-0.9.0a0/qcodes/instrument/sims/lakeshore_model372.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)      760 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument/sims/stahl.yaml
--rw-r--r--   0 vsts      (1001) docker     (117)     1550 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/specialized_parameters.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10744 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/sweep_values.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9750 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument/visa.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Advantech/
--rw-r--r--   0 vsts      (1001) docker     (117)    11541 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Advantech/PCIE_1751.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Advantech/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AimTTi/
--rw-r--r--   0 vsts      (1001) docker     (117)    11233 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AimTTi/AimTTi_PL601P_channels.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AimTTi/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/
--rw-r--r--   0 vsts      (1001) docker     (117)    39313 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS.py
--rw-r--r--   0 vsts      (1001) docker     (117)    19940 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS9360.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20635 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS9373.py
--rw-r--r--   0 vsts      (1001) docker     (117)    15557 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS9870.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5628 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS_acquisition_controllers.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    21452 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ats_api.py
--rw-r--r--   0 vsts      (1001) docker     (117)    19645 2019-12-06 09:30:49.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/constants.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6840 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/dll_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3506 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1306 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Gentec/
--rw-r--r--   0 vsts      (1001) docker     (117)     2284 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Gentec/Gentec_Maestro.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Gentec/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/HP/
--rw-r--r--   0 vsts      (1001) docker     (117)     3825 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/HP/HP8133A.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10044 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/HP/HP8753D.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4913 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/HP/HP_83650A.py
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/HP/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Harvard/
--rw-r--r--   0 vsts      (1001) docker     (117)    22513 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Harvard/Decadac.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Harvard/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/
--rw-r--r--   0 vsts      (1001) docker     (117)    22847 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Infiniium.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14767 2019-12-06 09:30:49.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/KeysightAgilent_33XXX.py
--rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34410A_submodules.py
--rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34460A.py
--rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34460A_submodules.py
--rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34461A.py
--rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34461A_submodules.py
--rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34465A.py
--rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34465A_submodules.py
--rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34470A.py
--rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_34470A_submodules.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4553 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_B2962A.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7602 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_E8267D.py
--rw-r--r--   0 vsts      (1001) docker     (117)      172 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_N5183B.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3202 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_N6705B.py
--rw-r--r--   0 vsts      (1001) docker     (117)      795 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/M3201A.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2285 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/M3300A.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2114 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/N51x1.py
--rw-r--r--   0 vsts      (1001) docker     (117)      321 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/N5230C.py
--rw-r--r--   0 vsts      (1001) docker     (117)      510 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/N5245A.py
--rw-r--r--   0 vsts      (1001) docker     (117)    21557 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/N52xx.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/
--rw-r--r--   0 vsts      (1001) docker     (117)    33374 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/SD_AWG.py
--rw-r--r--   0 vsts      (1001) docker     (117)    29763 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/SD_DIG.py
--rw-r--r--   0 vsts      (1001) docker     (117)    12587 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/SD_Module.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6499 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_34934a.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5629 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_34980a.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5798 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_34980a_submodules.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14899 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_b220x.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/
--rw-r--r--   0 vsts      (1001) docker     (117)    10473 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7335 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_module.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3673 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_sampling_measurement.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11761 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1517A.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14487 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1520A.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1031 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1530A.py
--rw-r--r--   0 vsts      (1001) docker     (117)      802 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    19247 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/constants.py
--rw-r--r--   0 vsts      (1001) docker     (117)   125319 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/message_builder.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/
--rw-r--r--   0 vsts      (1001) docker     (117)    32800 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA.py
--rw-r--r--   0 vsts      (1001) docker     (117)    39082 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA_submodules.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1955 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/error_handling.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/
--rw-r--r--   0 vsts      (1001) docker     (117)    17591 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/Model_325.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6925 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/Model_336.py
--rw-r--r--   0 vsts      (1001) docker     (117)    12493 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/Model_372.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    22641 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/lakeshore_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/
--rw-r--r--   0 vsts      (1001) docker     (117)     3662 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/Base_SPDT.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3313 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/RC_SP4T.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2693 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/RC_SPDT.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1506 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/RUDAT_13G_90.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7136 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/USBHIDMixin.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3341 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/USB_SPDT.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Newport/
--rw-r--r--   0 vsts      (1001) docker     (117)    13764 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Newport/AG_UC8.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Newport/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QDev/
--rw-r--r--   0 vsts      (1001) docker     (117)    25083 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QDev/QDac.py
--rw-r--r--   0 vsts      (1001) docker     (117)    28339 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QDev/QDac_channels.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QDev/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/
--rw-r--r--   0 vsts      (1001) docker     (117)     1897 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/D4.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5545 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/D5a.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3011 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/F1d.py
--rw-r--r--   0 vsts      (1001) docker     (117)    27895 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/IVVI.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2846 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/M2j.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3537 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/S5i.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/
--rw-r--r--   0 vsts      (1001) docker     (117)    17110 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/DynaCool.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6219 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/commandhandler.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3106 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/server.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/
--rw-r--r--   0 vsts      (1001) docker     (117)    55986 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/M4i.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/py_header/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/py_header/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    64337 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/py_header/regs.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1913 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/py_header/spcerr.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7523 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/pyspcm.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/ZI/
--rw-r--r--   0 vsts      (1001) docker     (117)    14633 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/ZI/ZIHDAWG8.py
--rw-r--r--   0 vsts      (1001) docker     (117)   107591 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/ZI/ZIUHFLI.py
--rw-r--r--   0 vsts      (1001) docker     (117)       22 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/ZI/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)       36 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/
--rw-r--r--   0 vsts      (1001) docker     (117)     5968 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/Agilent_34400A.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3848 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/E8267C.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2909 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/E8527D.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5313 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/HP33210A.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/american_magnetics/
--rw-r--r--   0 vsts      (1001) docker     (117)    30099 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/american_magnetics/AMI430.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/american_magnetics/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/basel/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/basel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1719 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/basel/sp983c.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2735 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/devices.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/ithaco/
--rw-r--r--   0 vsts      (1001) docker     (117)     4098 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/ithaco/Ithaco_1211.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/ithaco/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/keysight/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/keysight/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/
--rw-r--r--   0 vsts      (1001) docker     (117)     9939 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/ILM200.py
--rw-r--r--   0 vsts      (1001) docker     (117)    29064 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/IPS120.py
--rw-r--r--   0 vsts      (1001) docker     (117)    22912 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/MercuryiPS_VISA.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    17938 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/kelvinox.py
--rw-r--r--   0 vsts      (1001) docker     (117)    17551 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/mercuryiPS.py
--rw-r--r--   0 vsts      (1001) docker     (117)    15677 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/triton.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/
--rw-r--r--   0 vsts      (1001) docker     (117)    12277 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DG1062.py
--rw-r--r--   0 vsts      (1001) docker     (117)    25200 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DG4000.py
--rw-r--r--   0 vsts      (1001) docker     (117)      662 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DP821.py
--rw-r--r--   0 vsts      (1001) docker     (117)      742 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DP831.py
--rw-r--r--   0 vsts      (1001) docker     (117)      734 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DP832.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7912 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DS1074Z.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10680 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DS4000.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/private/
--rw-r--r--   0 vsts      (1001) docker     (117)     6797 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/private/DP8xx.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/private/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/
--rw-r--r--   0 vsts      (1001) docker     (117)      476 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/HMC8041.py
--rw-r--r--   0 vsts      (1001) docker     (117)      476 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/HMC8042.py
--rw-r--r--   0 vsts      (1001) docker     (117)      476 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/HMC8043.py
--rw-r--r--   0 vsts      (1001) docker     (117)       76 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/RTE1000.py
--rw-r--r--   0 vsts      (1001) docker     (117)    34359 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/RTO1000.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6864 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/SGS100A.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9651 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/SMR40.py
--rw-r--r--   0 vsts      (1001) docker     (117)    23296 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/ZNB.py
--rw-r--r--   0 vsts      (1001) docker     (117)       66 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/ZNB20.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/private/
--rw-r--r--   0 vsts      (1001) docker     (117)     4185 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/private/HMC804x.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/private/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/signal_hound/
--rw-r--r--   0 vsts      (1001) docker     (117)    32885 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/signal_hound/USB_SA124B.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/signal_hound/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stahl/
--rw-r--r--   0 vsts      (1001) docker     (117)       25 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stahl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6989 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stahl/stahl.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/
--rw-r--r--   0 vsts      (1001) docker     (117)     7442 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SG384.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14978 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SIM928.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4092 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR560.py
--rw-r--r--   0 vsts      (1001) docker     (117)    26945 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR830.py
--rw-r--r--   0 vsts      (1001) docker     (117)      364 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR860.py
--rw-r--r--   0 vsts      (1001) docker     (117)      362 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR865.py
--rw-r--r--   0 vsts      (1001) docker     (117)      413 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR865A.py
--rw-r--r--   0 vsts      (1001) docker     (117)    44303 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR86x.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/
--rw-r--r--   0 vsts      (1001) docker     (117)    78297 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG5014.py
--rw-r--r--   0 vsts      (1001) docker     (117)    23171 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG520.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4893 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG5200.py
--rw-r--r--   0 vsts      (1001) docker     (117)      559 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG5208.py
--rw-r--r--   0 vsts      (1001) docker     (117)    54677 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG70000A.py
--rw-r--r--   0 vsts      (1001) docker     (117)      641 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG70002A.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20399 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWGFileParser.py
--rw-r--r--   0 vsts      (1001) docker     (117)    28076 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/DPO7200xx.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7518 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2000.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6188 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2400.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14366 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2450.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8430 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2600.py
--rw-r--r--   0 vsts      (1001) docker     (117)    29081 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2600_channels.py
--rw-r--r--   0 vsts      (1001) docker     (117)    12320 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2700.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9610 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_6500.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6487 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_s46.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13837 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/TPS2012.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2936 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/test.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/weinschel/
--rw-r--r--   0 vsts      (1001) docker     (117)      694 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/weinschel/Weinschel_8320.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/weinschel/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/yokogawa/
--rw-r--r--   0 vsts      (1001) docker     (117)    20860 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/yokogawa/GS200.py
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/instrument_drivers/yokogawa/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/logger/
--rw-r--r--   0 vsts      (1001) docker     (117)      760 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/logger/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5391 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/logger/instrument_logger.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5946 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/logger/log_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (117)    12243 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/logger/logger.py
--rw-r--r--   0 vsts      (1001) docker     (117)    36640 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/loops.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/math/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/math/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13089 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/math/field_vector.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6380 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/measure.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/monitor/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/monitor/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/monitor/dist/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/monitor/dist/css/
--rw-r--r--   0 vsts      (1001) docker     (117)     1934 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/monitor/dist/css/main.0963d6b9.css
--rw-r--r--   0 vsts      (1001) docker     (117)   103614 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/monitor/dist/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (117)      355 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/monitor/dist/index.html
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/monitor/dist/js/
--rw-r--r--   0 vsts      (1001) docker     (117)    82828 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/monitor/dist/js/main.b221ee88.js
--rw-r--r--   0 vsts      (1001) docker     (117)       69 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/monitor/dist/webpack-assets.json
--rw-r--r--   0 vsts      (1001) docker     (117)     9167 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/monitor/monitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/plots/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/plots/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11916 2019-12-06 09:30:44.000000 qcodes-0.9.0a0/qcodes/plots/base.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5243 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/plots/colors.py
--rw-r--r--   0 vsts      (1001) docker     (117)    24767 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/plots/pyqtgraph.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20762 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/plots/qcmatplotlib.py
--rw-r--r--   0 vsts      (1001) docker     (117)      128 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/py.typed
--rw-r--r--   0 vsts      (1001) docker     (117)    25821 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/station.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4241 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/common.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1314 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4601 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/data_mocks.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/dataset/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8131 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/dataset_fixtures.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/
--rw-r--r--   0 vsts      (1001) docker     (117)     1507 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/dac_ch1_set.dat
--rw-r--r--   0 vsts      (1001) docker     (117)     8934 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/snapshot.json
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/
--rw-r--r--   0 vsts      (1001) docker     (117)      339 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/dac_ch1_set_dac_ch2_set.dat
--rw-r--r--   0 vsts      (1001) docker     (117)    11004 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/snapshot.json
--rw-r--r--   0 vsts      (1001) docker     (117)     5217 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/helper_functions.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3300 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/interdeps_fixtures.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3934 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/temporary_databases.py
--rw-r--r--   0 vsts      (1001) docker     (117)    33497 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_database_creation_and_upgrading.py
--rw-r--r--   0 vsts      (1001) docker     (117)    30539 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_database_extract_runs.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3887 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_datasaver.py
--rw-r--r--   0 vsts      (1001) docker     (117)    47793 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_dataset_basic.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11612 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_dataset_loading.py
--rw-r--r--   0 vsts      (1001) docker     (117)    16391 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_dependencies.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3472 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_descriptions.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11581 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_experiment_container.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4347 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_fix_functions.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7558 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_guids.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3623 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_links.py
--rw-r--r--   0 vsts      (1001) docker     (117)    84729 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_measurement_context_manager.py
--rw-r--r--   0 vsts      (1001) docker     (117)      563 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9969 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_paramspec.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8908 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_plotting.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3964 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_snapshot.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14496 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_sqlite_base.py
--rw-r--r--   0 vsts      (1001) docker     (117)    12506 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_sqlite_connection.py
--rw-r--r--   0 vsts      (1001) docker     (117)      354 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_sqlitesettings.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5058 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_string_data.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7343 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/dataset/test_subscribing.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1308 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/dataset_generators.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/drivers/
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/
--rw-r--r--   0 vsts      (1001) docker     (117)       61 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6901 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/test_alazar_api.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1004 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/test_alazar_buffer.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1783 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/test_dll_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (117)        2 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/drivers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/drivers/auxiliary_files/
--rw-r--r--   0 vsts      (1001) docker     (117)        2 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/drivers/auxiliary_files/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5711 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/drivers/auxiliary_files/awgSeqDataSets.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5965 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2211 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500_module.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5655 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1517a_smu.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5974 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1520a_cmu.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4483 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_sampling_measurement.py
--rw-r--r--   0 vsts      (1001) docker     (117)    25573 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/test_MessageBuilder.py
--rw-r--r--   0 vsts      (1001) docker     (117)      633 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/test_commandList.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3334 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_Agilent_E8527D.py
--rw-r--r--   0 vsts      (1001) docker     (117)      544 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_AimTTi_PL601P.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4574 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_Keithley_2450.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1579 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_Keysight_33XXX.py
--rw-r--r--   0 vsts      (1001) docker     (117)    21098 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_Keysight_M3201A.py
--rw-r--r--   0 vsts      (1001) docker     (117)      834 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_Keysight_N6705B.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4642 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_MercuryiPS.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1811 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_Rigol_DS1074Z.py
--rw-r--r--   0 vsts      (1001) docker     (117)    33918 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_ami430.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5897 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_keithley_26xx.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5012 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_keithley_s46.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2302 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_34465a.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4070 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_34934a.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2105 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_34980a.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7980 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_b220x.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14332 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_lakeshore.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8183 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_lakeshore_336.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1612 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_lakeshore_file_parser.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1928 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_m2j.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1427 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_rohdeschwarz_HMC804x.py
--rw-r--r--   0 vsts      (1001) docker     (117)      779 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_rto_1000.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2751 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_stahl.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1503 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_AWG5014C.py
--rw-r--r--   0 vsts      (1001) docker     (117)      915 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_AWG5208.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7074 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_AWG70000A.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2102 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_dpo7200xx.py
--rw-r--r--   0 vsts      (1001) docker     (117)      993 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_weinchel.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10419 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/drivers/test_zihdawg8.py
--rw-r--r--   0 vsts      (1001) docker     (117)    18860 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/instrument_mocks.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9770 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_autoloadable_channels.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20547 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_channels.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9740 2019-12-06 09:30:32.000000 qcodes-0.9.0a0/qcodes/tests/test_combined_loop.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5910 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_combined_par.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3839 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_command.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13354 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (117)    20158 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_data.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7878 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_delegate_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6048 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_deprecate.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5719 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/test_field_vector.py
--rw-r--r--   0 vsts      (1001) docker     (117)    16127 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_format.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1696 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_generic_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3228 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_group_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13846 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/test_hdf5formatter.py
--rw-r--r--   0 vsts      (1001) docker     (117)    28191 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (117)      723 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_installation_info.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11195 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_instrument.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1518 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_json.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4786 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_location_provider.py
--rw-r--r--   0 vsts      (1001) docker     (117)     9511 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_logger.py
--rw-r--r--   0 vsts      (1001) docker     (117)    19907 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_loop.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3344 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_measure.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3515 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4800 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_monitor.py
--rw-r--r--   0 vsts      (1001) docker     (117)    66546 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (117)    19657 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_parameter_with_setpoints.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2498 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/tests/test_plot_utils.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2278 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_plots.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2599 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_qcmatplotlib_functions.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3351 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_snapshot.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1149 2019-12-06 09:31:02.000000 qcodes-0.9.0a0/qcodes/tests/test_specialized_parameters.py
--rw-r--r--   0 vsts      (1001) docker     (117)    22989 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_station.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5164 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_sweep_values.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1548 2019-12-06 09:30:45.000000 qcodes-0.9.0a0/qcodes/tests/test_testutils.py
--rw-r--r--   0 vsts      (1001) docker     (117)      856 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/tests/test_threading.py
--rw-r--r--   0 vsts      (1001) docker     (117)    27593 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_validators.py
--rw-r--r--   0 vsts      (1001) docker     (117)     5293 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/tests/test_visa.py
--rw-r--r--   0 vsts      (1001) docker     (117)      867 2019-12-06 09:30:58.000000 qcodes-0.9.0a0/qcodes/tests/test_wrong_address.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes/utils/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-06 09:27:26.000000 qcodes-0.9.0a0/qcodes/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7480 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/command.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2042 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/delaykeyboardinterrupt.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3584 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/deprecate.py
--rw-r--r--   0 vsts      (1001) docker     (117)    27362 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2041 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/installation.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2347 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/installation_info.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2443 2019-12-06 09:30:39.000000 qcodes-0.9.0a0/qcodes/utils/log_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6279 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/magic.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4651 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/metadata.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11481 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/plotting.py
--rw-r--r--   0 vsts      (1001) docker     (117)    16002 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/slack.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2346 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/threading.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1078 2019-12-06 09:30:49.000000 qcodes-0.9.0a0/qcodes/utils/types.py
--rw-r--r--   0 vsts      (1001) docker     (117)    32886 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/validators.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2750 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/utils/zmq_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (117)       92 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/qcodes/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (117)     4940 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)    19016 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-12-06 09:30:05.000000 qcodes-0.9.0a0/qcodes.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (117)      365 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        7 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/qcodes.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (117)      294 2019-12-06 09:50:09.000000 qcodes-0.9.0a0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (117)     3969 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/setup.py
--rw-r--r--   0 vsts      (1001) docker     (117)    68611 2019-12-06 09:31:07.000000 qcodes-0.9.0a0/versioneer.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/
+-rw-r--r--   0 vsts      (1001) docker     (117)       49 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (117)     4941 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (117)     3383 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/
+-rw-r--r--   0 vsts      (1001) docker     (117)     4214 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      500 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6949 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/actions.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/config/
+-rw-r--r--   0 vsts      (1001) docker     (117)       83 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    15892 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/config/config.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2191 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/config/qcodesrc.json
+-rw-r--r--   0 vsts      (1001) docker     (117)    14086 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/config/qcodesrc_schema.json
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/data/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    19667 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/data/data_array.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    26514 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/data/data_set.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13413 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/data/format.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    17385 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/data/gnuplot_format.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    23206 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/data/hdf5_format.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2474 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/data/hdf5_format_hickle.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8697 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/data/io.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6537 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/data/location.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (117)      246 2019-12-10 08:51:40.000000 qcodes-0.9.0rc1/qcodes/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13537 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/data_export.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    52509 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/data_set.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      673 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/database.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11193 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/database_extract_runs.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5864 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/database_fix_functions.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/
+-rw-r--r--   0 vsts      (1001) docker     (117)      390 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20259 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/dependencies.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8943 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/param_spec.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2096 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/rundescriber.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/
+-rw-r--r--   0 vsts      (1001) docker     (117)      255 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4721 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/converters.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4642 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3521 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/v0.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11617 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/experiment_container.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5647 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/guids.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2063 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/json_exporter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4122 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/legacy_import.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dataset/linked_datasets/
+-rw-r--r--   0 vsts      (1001) docker     (117)      103 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/linked_datasets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2201 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/linked_datasets/links.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    48869 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/measurements.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    30119 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/plotting.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/
+-rw-r--r--   0 vsts      (1001) docker     (117)      553 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5564 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/connection.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10310 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/database.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/
+-rw-r--r--   0 vsts      (1001) docker     (117)    11909 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8517 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/upgrade_2_to_3.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3450 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/upgrade_3_to_4.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1732 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/upgrade_5_to_6.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      422 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/version.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2241 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/initial_schema.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    57987 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/queries.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10296 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/query_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2969 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2998 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/dataset/sqlite_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dist/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dist/schemas/
+-rw-r--r--   0 vsts      (1001) docker     (117)     8605 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dist/schemas/station-template.schema.json
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dist/tests/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/dist/tests/station/
+-rw-r--r--   0 vsts      (1001) docker     (117)     1743 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/dist/tests/station/example.station.yaml
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    30848 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/base.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    34121 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/channel.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5351 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/function.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11138 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/group_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8643 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/ip.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3609 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/ip_to_visa.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument/mockers/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/mockers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7218 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/mockers/ami430.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4073 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/mockers/simulated_ats_api.py
+-rw-r--r--   0 vsts      (1001) docker     (117)   100465 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/parameter.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/
+-rw-r--r--   0 vsts      (1001) docker     (117)     2909 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/AMI430.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      411 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/AimTTi_PL601P.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1324 2019-12-10 08:51:27.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Keithley_2450.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     4560 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Keithley_2600.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1474 2019-12-10 08:51:40.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Keithley_s46.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      974 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Keysight_33xxx.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     2540 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Keysight_34465A.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      286 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Keysight_N6705B.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     2632 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/MercuryiPS.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      462 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/RSHMC804x.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1098 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/RTO_1000.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1195 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Rigol_DS1074Z.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1821 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Tektronix_AWG5014C.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      498 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Tektronix_AWG5208.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      884 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Tektronix_AWG70000A.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     2209 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/Tektronix_DPO7200xx.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)        5 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      749 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      403 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/dummy.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1186 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/keysight_34980A.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1568 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/keysight_b1500.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     3760 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/keysight_b220x.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     3332 2019-12-10 08:51:12.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/lakeshore_model336.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      238 2019-12-10 08:51:12.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/lakeshore_model372.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)      760 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument/sims/stahl.yaml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1550 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/specialized_parameters.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10744 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/sweep_values.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9750 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument/visa.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Advantech/
+-rw-r--r--   0 vsts      (1001) docker     (117)    11541 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Advantech/PCIE_1751.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Advantech/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AimTTi/
+-rw-r--r--   0 vsts      (1001) docker     (117)    11233 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AimTTi/AimTTi_PL601P_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AimTTi/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/
+-rw-r--r--   0 vsts      (1001) docker     (117)    39313 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    19940 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS9360.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20635 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS9373.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    15557 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS9870.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5628 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS_acquisition_controllers.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    21452 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ats_api.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    19645 2019-12-10 08:51:27.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6840 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/dll_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3506 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1306 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Gentec/
+-rw-r--r--   0 vsts      (1001) docker     (117)     2284 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Gentec/Gentec_Maestro.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Gentec/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/
+-rw-r--r--   0 vsts      (1001) docker     (117)     3825 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/HP8133A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10044 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/HP8753D.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4913 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/HP_83650A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Harvard/
+-rw-r--r--   0 vsts      (1001) docker     (117)    22513 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Harvard/Decadac.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Harvard/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/
+-rw-r--r--   0 vsts      (1001) docker     (117)    23523 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Infiniium.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14767 2019-12-10 08:51:27.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/KeysightAgilent_33XXX.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34410A_submodules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34460A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34460A_submodules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34461A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34461A_submodules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34465A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34465A_submodules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      315 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34470A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      327 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_34470A_submodules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4553 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_B2962A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7602 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_E8267D.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      172 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_N5183B.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3202 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_N6705B.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      795 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/M3201A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2285 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/M3300A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2114 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/N51x1.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      321 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/N5230C.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      510 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/N5245A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    21557 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/N52xx.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/
+-rw-r--r--   0 vsts      (1001) docker     (117)    33374 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/SD_AWG.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    29763 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/SD_DIG.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    12587 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/SD_Module.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6499 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_34934a.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5629 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_34980a.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5798 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_34980a_submodules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14899 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_b220x.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/
+-rw-r--r--   0 vsts      (1001) docker     (117)    10473 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7335 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_module.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3673 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_sampling_measurement.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11761 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1517A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14487 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1520A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1031 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1530A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      802 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    19247 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (117)   125319 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/message_builder.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/
+-rw-r--r--   0 vsts      (1001) docker     (117)    32800 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    39082 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA_submodules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1955 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/error_handling.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/
+-rw-r--r--   0 vsts      (1001) docker     (117)    17591 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/Model_325.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6925 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/Model_336.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    12493 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/Model_372.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    22641 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/lakeshore_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/
+-rw-r--r--   0 vsts      (1001) docker     (117)     3662 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/Base_SPDT.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3313 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/RC_SP4T.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2693 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/RC_SPDT.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1506 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/RUDAT_13G_90.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7136 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/USBHIDMixin.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3341 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/USB_SPDT.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Newport/
+-rw-r--r--   0 vsts      (1001) docker     (117)    13764 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Newport/AG_UC8.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Newport/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QDev/
+-rw-r--r--   0 vsts      (1001) docker     (117)    25083 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QDev/QDac.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    28339 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QDev/QDac_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QDev/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/
+-rw-r--r--   0 vsts      (1001) docker     (117)     1897 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/D4.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5545 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/D5a.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3011 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/F1d.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    27895 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/IVVI.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2846 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/M2j.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3537 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/S5i.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/
+-rw-r--r--   0 vsts      (1001) docker     (117)    17110 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/DynaCool.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6219 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/commandhandler.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3106 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/server.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/
+-rw-r--r--   0 vsts      (1001) docker     (117)    55986 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/M4i.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/py_header/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/py_header/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    64337 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/py_header/regs.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1913 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/py_header/spcerr.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7523 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/pyspcm.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/ZI/
+-rw-r--r--   0 vsts      (1001) docker     (117)    14633 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/ZI/ZIHDAWG8.py
+-rw-r--r--   0 vsts      (1001) docker     (117)   107591 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/ZI/ZIUHFLI.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       22 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/ZI/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       36 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/
+-rw-r--r--   0 vsts      (1001) docker     (117)     5968 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/Agilent_34400A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3848 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/E8267C.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2909 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/E8527D.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5313 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/HP33210A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/american_magnetics/
+-rw-r--r--   0 vsts      (1001) docker     (117)    30099 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/american_magnetics/AMI430.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/american_magnetics/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/basel/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/basel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1719 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/basel/sp983c.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2735 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/devices.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/ithaco/
+-rw-r--r--   0 vsts      (1001) docker     (117)     4098 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/ithaco/Ithaco_1211.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/ithaco/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/keysight/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/keysight/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/
+-rw-r--r--   0 vsts      (1001) docker     (117)     9939 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/ILM200.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    29064 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/IPS120.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    22912 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/MercuryiPS_VISA.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    17938 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/kelvinox.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    17551 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/mercuryiPS.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    15677 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/triton.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/
+-rw-r--r--   0 vsts      (1001) docker     (117)    12277 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DG1062.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    25200 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DG4000.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      662 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DP821.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      742 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DP831.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      734 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DP832.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7912 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DS1074Z.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10680 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DS4000.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/private/
+-rw-r--r--   0 vsts      (1001) docker     (117)     6797 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/private/DP8xx.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/private/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/
+-rw-r--r--   0 vsts      (1001) docker     (117)      476 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/HMC8041.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      476 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/HMC8042.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      476 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/HMC8043.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       76 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/RTE1000.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    34359 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/RTO1000.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6864 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/SGS100A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9651 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/SMR40.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    23296 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/ZNB.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       66 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/ZNB20.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/private/
+-rw-r--r--   0 vsts      (1001) docker     (117)     4185 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/private/HMC804x.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/private/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/signal_hound/
+-rw-r--r--   0 vsts      (1001) docker     (117)    32885 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/signal_hound/USB_SA124B.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/signal_hound/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stahl/
+-rw-r--r--   0 vsts      (1001) docker     (117)       25 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stahl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6989 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stahl/stahl.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/
+-rw-r--r--   0 vsts      (1001) docker     (117)     7442 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SG384.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14978 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SIM928.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4092 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR560.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    26945 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR830.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      364 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR860.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      362 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR865.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      413 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR865A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    44303 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR86x.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/
+-rw-r--r--   0 vsts      (1001) docker     (117)    78297 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG5014.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    23171 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG520.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4893 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG5200.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      559 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG5208.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    54677 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG70000A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      641 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG70002A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20399 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWGFileParser.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    28076 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/DPO7200xx.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7518 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2000.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6188 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2400.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14366 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2450.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8430 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2600.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    29081 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2600_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    12320 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2700.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9610 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_6500.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6487 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_s46.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13837 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/TPS2012.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2936 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/test.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/weinschel/
+-rw-r--r--   0 vsts      (1001) docker     (117)      694 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/weinschel/Weinschel_8320.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/weinschel/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/yokogawa/
+-rw-r--r--   0 vsts      (1001) docker     (117)    20860 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/yokogawa/GS200.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/instrument_drivers/yokogawa/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/logger/
+-rw-r--r--   0 vsts      (1001) docker     (117)      760 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/logger/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5391 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/logger/instrument_logger.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5946 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/logger/log_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13991 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/logger/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    36640 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/loops.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/math/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/math/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13089 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/math/field_vector.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6380 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/measure.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/monitor/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/monitor/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/css/
+-rw-r--r--   0 vsts      (1001) docker     (117)     1934 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/css/main.0963d6b9.css
+-rw-r--r--   0 vsts      (1001) docker     (117)   103614 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (117)      355 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/index.html
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/js/
+-rw-r--r--   0 vsts      (1001) docker     (117)    82828 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/js/main.b221ee88.js
+-rw-r--r--   0 vsts      (1001) docker     (117)       69 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/monitor/dist/webpack-assets.json
+-rw-r--r--   0 vsts      (1001) docker     (117)     9167 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/monitor/monitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/plots/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/plots/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11916 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/plots/base.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5243 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/plots/colors.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    24767 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/plots/pyqtgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20762 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/plots/qcmatplotlib.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      128 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (117)    25821 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/station.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4241 2019-12-10 08:51:22.000000 qcodes-0.9.0rc1/qcodes/tests/common.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1314 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4601 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/data_mocks.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8131 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/dataset_fixtures.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/
+-rw-r--r--   0 vsts      (1001) docker     (117)     1507 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/dac_ch1_set.dat
+-rw-r--r--   0 vsts      (1001) docker     (117)     8934 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/snapshot.json
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/
+-rw-r--r--   0 vsts      (1001) docker     (117)      339 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/dac_ch1_set_dac_ch2_set.dat
+-rw-r--r--   0 vsts      (1001) docker     (117)    11004 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/snapshot.json
+-rw-r--r--   0 vsts      (1001) docker     (117)     5217 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/helper_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3300 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/interdeps_fixtures.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3934 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/temporary_databases.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    33497 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_database_creation_and_upgrading.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    30539 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_database_extract_runs.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3887 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_datasaver.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    47793 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_dataset_basic.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11612 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_dataset_loading.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    16391 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_dependencies.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3472 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_descriptions.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11581 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_experiment_container.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4347 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_fix_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7558 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_guids.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3623 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_links.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    84729 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_measurement_context_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      563 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9969 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_paramspec.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8908 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_plotting.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3964 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_snapshot.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14496 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_sqlite_base.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    12506 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_sqlite_connection.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      354 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_sqlitesettings.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5058 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_string_data.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7343 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/dataset/test_subscribing.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1308 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/dataset_generators.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/
+-rw-r--r--   0 vsts      (1001) docker     (117)       61 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6901 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/test_alazar_api.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1004 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/test_alazar_buffer.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1783 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/test_dll_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (117)        2 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/auxiliary_files/
+-rw-r--r--   0 vsts      (1001) docker     (117)        2 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/auxiliary_files/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5711 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/auxiliary_files/awgSeqDataSets.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5965 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2211 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500_module.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5655 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1517a_smu.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5974 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1520a_cmu.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4483 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_sampling_measurement.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    25573 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/test_MessageBuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      633 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/test_commandList.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3334 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_Agilent_E8527D.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      544 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_AimTTi_PL601P.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4574 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keithley_2450.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1579 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keysight_33XXX.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    21098 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keysight_M3201A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      834 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keysight_N6705B.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4642 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_MercuryiPS.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1811 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_Rigol_DS1074Z.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    33918 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_ami430.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5897 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_keithley_26xx.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5012 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_keithley_s46.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2302 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_34465a.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4070 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_34934a.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2105 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_34980a.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7980 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_b220x.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    14332 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_lakeshore.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8183 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_lakeshore_336.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1612 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_lakeshore_file_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1928 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_m2j.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1427 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_rohdeschwarz_HMC804x.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      779 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_rto_1000.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2751 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_stahl.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1503 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_AWG5014C.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      915 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_AWG5208.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7074 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_AWG70000A.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2102 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_dpo7200xx.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      993 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_weinchel.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10419 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/drivers/test_zihdawg8.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    18860 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/instrument_mocks.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9770 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_autoloadable_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20547 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9740 2019-12-10 08:51:09.000000 qcodes-0.9.0rc1/qcodes/tests/test_combined_loop.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5910 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_combined_par.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3839 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_command.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13354 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    20158 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_data.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7878 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_delegate_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6048 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_deprecate.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5719 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/test_field_vector.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    16127 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_format.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1696 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_generic_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3228 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_group_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13846 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/test_hdf5formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    28191 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      723 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_installation_info.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11195 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_instrument.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1518 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_json.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4786 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_location_provider.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     9511 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_logger.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    19907 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_loop.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3344 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_measure.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3515 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4800 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    66546 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    19657 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_parameter_with_setpoints.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2498 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/tests/test_plot_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2278 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_plots.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2599 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_qcmatplotlib_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3351 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_snapshot.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1149 2019-12-10 08:51:41.000000 qcodes-0.9.0rc1/qcodes/tests/test_specialized_parameters.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    22989 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_station.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5164 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_sweep_values.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1548 2019-12-10 08:51:23.000000 qcodes-0.9.0rc1/qcodes/tests/test_testutils.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      856 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/tests/test_threading.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    27593 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     5293 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/tests/test_visa.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      867 2019-12-10 08:51:36.000000 qcodes-0.9.0rc1/qcodes/tests/test_wrong_address.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes/utils/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2019-12-10 08:47:58.000000 qcodes-0.9.0rc1/qcodes/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     7480 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/command.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2042 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/delaykeyboardinterrupt.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3584 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/deprecate.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    27366 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2041 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/installation.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2347 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/installation_info.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2443 2019-12-10 08:51:17.000000 qcodes-0.9.0rc1/qcodes/utils/log_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6279 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/magic.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4651 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11481 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/plotting.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    16002 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/slack.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2346 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/threading.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1078 2019-12-10 08:51:27.000000 qcodes-0.9.0rc1/qcodes/utils/types.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    32886 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/validators.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2750 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/utils/zmq_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (117)       92 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/qcodes/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (117)     4941 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (117)    19016 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)        1 2019-12-10 08:50:45.000000 qcodes-0.9.0rc1/qcodes.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (117)      365 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)        7 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/qcodes.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)      294 2019-12-10 09:11:20.000000 qcodes-0.9.0rc1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (117)     3969 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    68611 2019-12-10 08:51:45.000000 qcodes-0.9.0rc1/versioneer.py
```

### Comparing `qcodes-0.9.0a0/PKG-INFO` & `qcodes-0.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcodes
-Version: 0.9.0a0
+Version: 0.9.0rc1
 Summary: Python-based data acquisition framework developed by the Copenhagen / Delft / Sydney / Microsoft quantum computing consortium
 Home-page: https://github.com/QCoDeS/Qcodes
 Maintainer: Jens H Nielsen
 Maintainer-email: Jens.Nielsen@microsoft.com
 License: MIT
 Description: QCoDeS |Build Status Azure| |Build Status Travis| |DOCS| |DOI|
         ==============================================================
```

### Comparing `qcodes-0.9.0a0/README.rst` & `qcodes-0.9.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/__init__.py` & `qcodes-0.9.0rc1/qcodes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """Set up the main qcodes namespace."""
 
 # flake8: noqa (we don't need the "<...> imported but unused" error)
 
 # config
 
 from qcodes.config import Config
+from qcodes.logger import start_all_logging
+from qcodes.logger.logger import conditionally_start_all_logging
 from qcodes.utils.helpers import add_to_spyder_UMR_excludelist
 from .version import __version__
 
+config: Config = Config()
+
+conditionally_start_all_logging()
+
 # we dont want spyder to reload qcodes as this will overwrite the default station
 # instrument list and running monitor
 add_to_spyder_UMR_excludelist('qcodes')
-config: Config = Config()
+
 
 from qcodes.version import __version__
 
 plotlib = config.gui.plotlib
 if plotlib in {'QT', 'all'}:
     try:
         from qcodes.plots.pyqtgraph import QtPlot
```

### Comparing `qcodes-0.9.0a0/qcodes/actions.py` & `qcodes-0.9.0rc1/qcodes/actions.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/config/config.py` & `qcodes-0.9.0rc1/qcodes/config/config.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/config/qcodesrc.json` & `qcodes-0.9.0rc1/qcodes/config/qcodesrc.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'logger'": "{'start_logging_on_import': 'if_telemetry_set_up'}"}*

```diff
@@ -19,15 +19,16 @@
         "pyqtmaxplots": 100
     },
     "logger": {
         "console_level": "WARNING",
         "file_level": "INFO",
         "logger_levels": {
             "pyvisa": "INFO"
-        }
+        },
+        "start_logging_on_import": "if_telemetry_set_up"
     },
     "plotting": {
         "auto_color_scale": {
             "color_over": "#a1c4fc",
             "color_under": "#017000",
             "cutoff_percentile": [
                 0.5,
```

### Comparing `qcodes-0.9.0a0/qcodes/config/qcodesrc_schema.json` & `qcodes-0.9.0rc1/qcodes/config/qcodesrc_schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999826388888889%*

 * *Differences: {"'properties'": "{'logger': {'properties': {'start_logging_on_import': OrderedDict([('type', "*

 * *                 "'string'), ('enum', ['always', 'never', 'if_telemetry_set_up']), ('description', "*

 * *                 '"whether to call `start_all_logging` on qcodes import time. Valid values are '*

 * *                 '\'always\', \'never\', \'if_telemetry_set_up\'."), (\'default\', '*

 * *                 "'if_telemetry_set_up')])}}}"}*

```diff
@@ -149,14 +149,24 @@
                     "additionalProperties": {
                         "type": "string"
                     },
                     "default": {
                         "pyvisa": "INFO"
                     },
                     "type": "object"
+                },
+                "start_logging_on_import": {
+                    "default": "if_telemetry_set_up",
+                    "description": "whether to call `start_all_logging` on qcodes import time. Valid values are 'always', 'never', 'if_telemetry_set_up'.",
+                    "enum": [
+                        "always",
+                        "never",
+                        "if_telemetry_set_up"
+                    ],
+                    "type": "string"
                 }
             },
             "required": [
                 "console_level",
                 "file_level"
             ],
             "type": "object"
```

### Comparing `qcodes-0.9.0a0/qcodes/data/data_array.py` & `qcodes-0.9.0rc1/qcodes/data/data_array.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/data/data_set.py` & `qcodes-0.9.0rc1/qcodes/data/data_set.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/data/format.py` & `qcodes-0.9.0rc1/qcodes/data/format.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/data/gnuplot_format.py` & `qcodes-0.9.0rc1/qcodes/data/gnuplot_format.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/data/hdf5_format.py` & `qcodes-0.9.0rc1/qcodes/data/hdf5_format.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/data/hdf5_format_hickle.py` & `qcodes-0.9.0rc1/qcodes/data/hdf5_format_hickle.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/data/io.py` & `qcodes-0.9.0rc1/qcodes/data/io.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/data/location.py` & `qcodes-0.9.0rc1/qcodes/data/location.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/data_export.py` & `qcodes-0.9.0rc1/qcodes/dataset/data_export.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/data_set.py` & `qcodes-0.9.0rc1/qcodes/dataset/data_set.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/database.py` & `qcodes-0.9.0rc1/qcodes/dataset/database.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/database_extract_runs.py` & `qcodes-0.9.0rc1/qcodes/dataset/database_extract_runs.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/database_fix_functions.py` & `qcodes-0.9.0rc1/qcodes/dataset/database_fix_functions.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/descriptions/dependencies.py` & `qcodes-0.9.0rc1/qcodes/dataset/descriptions/dependencies.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/descriptions/param_spec.py` & `qcodes-0.9.0rc1/qcodes/dataset/descriptions/param_spec.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/descriptions/rundescriber.py` & `qcodes-0.9.0rc1/qcodes/dataset/descriptions/rundescriber.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/converters.py` & `qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/converters.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/serialization.py` & `qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/serialization.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/descriptions/versioning/v0.py` & `qcodes-0.9.0rc1/qcodes/dataset/descriptions/versioning/v0.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/experiment_container.py` & `qcodes-0.9.0rc1/qcodes/dataset/experiment_container.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/guids.py` & `qcodes-0.9.0rc1/qcodes/dataset/guids.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/json_exporter.py` & `qcodes-0.9.0rc1/qcodes/dataset/json_exporter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/legacy_import.py` & `qcodes-0.9.0rc1/qcodes/dataset/legacy_import.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/linked_datasets/links.py` & `qcodes-0.9.0rc1/qcodes/dataset/linked_datasets/links.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/measurements.py` & `qcodes-0.9.0rc1/qcodes/dataset/measurements.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/plotting.py` & `qcodes-0.9.0rc1/qcodes/dataset/plotting.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/__init__.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/connection.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/connection.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/database.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/__init__.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/__init__.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/upgrade_2_to_3.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/upgrade_2_to_3.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/upgrade_3_to_4.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/upgrade_3_to_4.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/db_upgrades/upgrade_5_to_6.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/db_upgrades/upgrade_5_to_6.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/initial_schema.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/initial_schema.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/queries.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/queries.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/query_helpers.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/query_helpers.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite/settings.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite/settings.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dataset/sqlite_base.py` & `qcodes-0.9.0rc1/qcodes/dataset/sqlite_base.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dist/schemas/station-template.schema.json` & `qcodes-0.9.0rc1/qcodes/dist/schemas/station-template.schema.json`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/dist/tests/station/example.station.yaml` & `qcodes-0.9.0rc1/qcodes/dist/tests/station/example.station.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/base.py` & `qcodes-0.9.0rc1/qcodes/instrument/base.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/channel.py` & `qcodes-0.9.0rc1/qcodes/instrument/channel.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/function.py` & `qcodes-0.9.0rc1/qcodes/instrument/function.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/group_parameter.py` & `qcodes-0.9.0rc1/qcodes/instrument/group_parameter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/ip.py` & `qcodes-0.9.0rc1/qcodes/instrument/ip.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/ip_to_visa.py` & `qcodes-0.9.0rc1/qcodes/instrument/ip_to_visa.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/mockers/ami430.py` & `qcodes-0.9.0rc1/qcodes/instrument/mockers/ami430.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/mockers/simulated_ats_api.py` & `qcodes-0.9.0rc1/qcodes/instrument/mockers/simulated_ats_api.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/parameter.py` & `qcodes-0.9.0rc1/qcodes/instrument/parameter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/AMI430.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/AMI430.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Keithley_2450.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Keithley_2450.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Keithley_2600.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Keithley_2600.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Keithley_s46.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Keithley_s46.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Keysight_33xxx.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Keysight_33xxx.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Keysight_34465A.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Keysight_34465A.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/MercuryiPS.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/MercuryiPS.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/RTO_1000.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/RTO_1000.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Rigol_DS1074Z.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Rigol_DS1074Z.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Tektronix_AWG5014C.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Tektronix_AWG5014C.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Tektronix_AWG70000A.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Tektronix_AWG70000A.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/Tektronix_DPO7200xx.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/Tektronix_DPO7200xx.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/dummy.py` & `qcodes-0.9.0rc1/qcodes/instrument/sims/dummy.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/keysight_34980A.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/keysight_34980A.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/keysight_b1500.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/keysight_b1500.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/keysight_b220x.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/keysight_b220x.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/lakeshore_model336.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/lakeshore_model336.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sims/stahl.yaml` & `qcodes-0.9.0rc1/qcodes/instrument/sims/stahl.yaml`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/specialized_parameters.py` & `qcodes-0.9.0rc1/qcodes/instrument/specialized_parameters.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/sweep_values.py` & `qcodes-0.9.0rc1/qcodes/instrument/sweep_values.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument/visa.py` & `qcodes-0.9.0rc1/qcodes/instrument/visa.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Advantech/PCIE_1751.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Advantech/PCIE_1751.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AimTTi/AimTTi_PL601P_channels.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AimTTi/AimTTi_PL601P_channels.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS9360.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS9360.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS9373.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS9373.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS9870.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS9870.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ATS_acquisition_controllers.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ATS_acquisition_controllers.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/ats_api.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/ats_api.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/constants.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/constants.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/dll_wrapper.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/dll_wrapper.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/helpers.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/helpers.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/AlazarTech/utils.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/AlazarTech/utils.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Gentec/Gentec_Maestro.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Gentec/Gentec_Maestro.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/HP/HP8133A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/HP8133A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/HP/HP8753D.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/HP8753D.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/HP/HP_83650A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/HP/HP_83650A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Harvard/Decadac.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Harvard/Decadac.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Infiniium.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Infiniium.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,14 +523,23 @@
 
         # time of the first point
         self.add_parameter('waveform_xorigin',
                             get_cmd='WAVeform:XORigin?',
                             unit='s',
                             get_parser=float
                             )
+
+        self.add_parameter('data_format',
+                           set_cmd='SAV:WAV:FORM {}',
+                           val_mapping={'csv': 'CSV',
+                                        'binary': 'BIN',
+                                        'asciixy': 'ASC'},
+                           docstring=("Set the format for saving "
+                                      "files using save_data function")
+                           )
         # Channels
         channels = ChannelList(self, "Channels", InfiniiumChannel,
                                 snapshotable=False)
 
         for i in range(1,5):
             channel = InfiniiumChannel(self, 'chan{}'.format(i), i)
             channels.append(channel)
@@ -548,7 +557,14 @@
     def _cmd_and_invalidate_call(self, cmd: str, val) -> None:
         """
         executes command and sets trace_ready status to false
         any command that effects the number of setpoints should invalidate the trace
         """
         self.trace_ready = False
         self.write(cmd.format(val))
+
+    def save_data(self, filename):
+        """
+        Saves the channels currently shown on oscilloscope screen to a USB.
+        Must set data_format parameter prior to calling this
+        """
+        self.write(f'SAV:WAV "{filename}"')
```

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/KeysightAgilent_33XXX.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/KeysightAgilent_33XXX.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_B2962A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_B2962A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_E8267D.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_E8267D.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/Keysight_N6705B.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/Keysight_N6705B.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/M3201A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/M3201A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/M3300A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/M3300A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/N51x1.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/N51x1.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/N52xx.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/N52xx.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/SD_AWG.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/SD_AWG.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/SD_DIG.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/SD_DIG.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/SD_common/SD_Module.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/SD_common/SD_Module.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_34934a.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_34934a.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_34980a.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_34980a.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_34980a_submodules.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_34980a_submodules.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysight_b220x.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysight_b220x.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_module.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_module.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_sampling_measurement.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1500_sampling_measurement.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1517A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1517A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1520A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1520A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1530A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/KeysightB1530A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/__init__.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/__init__.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/constants.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/constants.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/keysightb1500/message_builder.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/keysightb1500/message_builder.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA_submodules.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/Keysight_344xxA_submodules.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Keysight/private/error_handling.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Keysight/private/error_handling.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/Model_325.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/Model_325.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/Model_336.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/Model_336.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/Model_372.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/Model_372.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Lakeshore/lakeshore_base.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Lakeshore/lakeshore_base.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/Base_SPDT.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/Base_SPDT.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/RC_SP4T.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/RC_SP4T.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/RC_SPDT.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/RC_SPDT.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/RUDAT_13G_90.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/RUDAT_13G_90.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/USBHIDMixin.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/USBHIDMixin.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Minicircuits/USB_SPDT.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Minicircuits/USB_SPDT.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Newport/AG_UC8.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Newport/AG_UC8.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QDev/QDac.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QDev/QDac.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QDev/QDac_channels.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QDev/QDac_channels.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/D4.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/D4.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/D5a.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/D5a.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/F1d.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/F1d.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/IVVI.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/IVVI.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/M2j.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/M2j.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuTech/S5i.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuTech/S5i.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/DynaCool.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/DynaCool.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/commandhandler.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/commandhandler.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/server.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/QuantumDesign/DynaCoolPPMS/private/server.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/M4i.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/M4i.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/py_header/regs.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/py_header/regs.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/py_header/spcerr.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/py_header/spcerr.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/Spectrum/pyspcm.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/Spectrum/pyspcm.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/ZI/ZIHDAWG8.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/ZI/ZIHDAWG8.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/ZI/ZIUHFLI.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/ZI/ZIUHFLI.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/Agilent_34400A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/Agilent_34400A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/E8267C.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/E8267C.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/E8527D.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/E8527D.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/agilent/HP33210A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/agilent/HP33210A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/american_magnetics/AMI430.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/american_magnetics/AMI430.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/basel/sp983c.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/basel/sp983c.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/devices.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/devices.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/ithaco/Ithaco_1211.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/ithaco/Ithaco_1211.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/ILM200.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/ILM200.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/IPS120.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/IPS120.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/MercuryiPS_VISA.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/MercuryiPS_VISA.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/kelvinox.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/kelvinox.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/mercuryiPS.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/mercuryiPS.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/oxford/triton.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/oxford/triton.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DG1062.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DG1062.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DG4000.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DG4000.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DP821.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DP821.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DP831.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DP831.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DP832.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DP832.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DS1074Z.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DS1074Z.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/DS4000.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/DS4000.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rigol/private/DP8xx.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rigol/private/DP8xx.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/RTO1000.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/RTO1000.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/SGS100A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/SGS100A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/SMR40.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/SMR40.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/ZNB.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/ZNB.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/rohde_schwarz/private/HMC804x.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/rohde_schwarz/private/HMC804x.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/signal_hound/USB_SA124B.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/signal_hound/USB_SA124B.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/stahl/stahl.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/stahl/stahl.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SG384.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SG384.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SIM928.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SIM928.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR560.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR560.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR830.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR830.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/stanford_research/SR86x.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/stanford_research/SR86x.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG5014.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG5014.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG520.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG520.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG5200.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG5200.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG5208.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG5208.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG70000A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG70000A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWG70002A.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWG70002A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/AWGFileParser.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/AWGFileParser.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/DPO7200xx.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/DPO7200xx.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2000.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2000.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2400.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2400.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2450.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2450.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2600.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2600.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2600_channels.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2600_channels.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_2700.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_2700.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_6500.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_6500.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/Keithley_s46.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/Keithley_s46.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/tektronix/TPS2012.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/tektronix/TPS2012.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/test.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/test.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/weinschel/Weinschel_8320.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/weinschel/Weinschel_8320.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/instrument_drivers/yokogawa/GS200.py` & `qcodes-0.9.0rc1/qcodes/instrument_drivers/yokogawa/GS200.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/logger/__init__.py` & `qcodes-0.9.0rc1/qcodes/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/logger/instrument_logger.py` & `qcodes-0.9.0rc1/qcodes/logger/instrument_logger.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/logger/log_analysis.py` & `qcodes-0.9.0rc1/qcodes/logger/log_analysis.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/logger/logger.py` & `qcodes-0.9.0rc1/qcodes/logger/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -289,14 +289,64 @@
     """
     Starts python log module logging and ipython command history logging.
     """
     start_command_history_logger()
     start_logger()
 
 
+def conditionally_start_all_logging() -> None:
+    """Start logging if qcodesrc.json setup for it and in tool environment.
+
+    This function will start logging if the session is not being executed by
+    a tool such as pytest and under the following conditions depending on the
+    qcodes configuration of ``config.logger.start_logging_on_import``:
+
+    For ``never``:
+
+        don't start logging automatically
+
+    For ``always``:
+
+        Always start logging when not in test environment
+
+    For ``if_telemetry_set_up``:
+
+        Start logging if the GUID components and the instrumentation key for
+        telemetry are set up, and not in a test environment.
+    """
+    def start_logging_on_import() -> bool:
+        config = qc.config
+        if config.logger.start_logging_on_import == 'always':
+            return True
+        elif config.logger.start_logging_on_import == 'never':
+            return False
+        elif config.logger.start_logging_on_import == 'if_telemetry_set_up':
+            return (
+                config.GUID_components.location != 0 and
+                config.GUID_components.work_station != 0 and
+                config.telemetry.instrumentation_key != \
+                    "00000000-0000-0000-0000-000000000000"
+            )
+        else:
+            raise RuntimeError('Error in qcodesrc validation.')
+
+    def running_in_test_or_tool() -> bool:
+        import sys
+        tools = (
+            'pytest.py',
+            'pytest',
+            '_jb_pytest_runner.py',  # Jetbrains Pycharm
+            'testlauncher.py'        # VSCode
+        )
+        return any(sys.argv[0].endswith(tool) for tool in tools)
+
+    if start_logging_on_import() and not running_in_test_or_tool():
+        start_all_logging()
+
+
 @contextmanager
 def handler_level(level: LevelType,
                   handler: Union[logging.Handler,
                                  Sequence[logging.Handler]]):
     """
     Context manager to temporarily change the level of handlers.
```

### Comparing `qcodes-0.9.0a0/qcodes/loops.py` & `qcodes-0.9.0rc1/qcodes/loops.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/math/field_vector.py` & `qcodes-0.9.0rc1/qcodes/math/field_vector.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/measure.py` & `qcodes-0.9.0rc1/qcodes/measure.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/monitor/dist/css/main.0963d6b9.css` & `qcodes-0.9.0rc1/qcodes/monitor/dist/css/main.0963d6b9.css`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/monitor/dist/favicon.ico` & `qcodes-0.9.0rc1/qcodes/monitor/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/monitor/dist/js/main.b221ee88.js` & `qcodes-0.9.0rc1/qcodes/monitor/dist/js/main.b221ee88.js`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/monitor/monitor.py` & `qcodes-0.9.0rc1/qcodes/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/plots/base.py` & `qcodes-0.9.0rc1/qcodes/plots/base.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/plots/colors.py` & `qcodes-0.9.0rc1/qcodes/plots/colors.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/plots/pyqtgraph.py` & `qcodes-0.9.0rc1/qcodes/plots/pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/plots/qcmatplotlib.py` & `qcodes-0.9.0rc1/qcodes/plots/qcmatplotlib.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/station.py` & `qcodes-0.9.0rc1/qcodes/station.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/common.py` & `qcodes-0.9.0rc1/qcodes/tests/common.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/conftest.py` & `qcodes-0.9.0rc1/qcodes/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/data_mocks.py` & `qcodes-0.9.0rc1/qcodes/tests/data_mocks.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/dataset_fixtures.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/dac_ch1_set.dat` & `qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/dac_ch1_set.dat`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/snapshot.json` & `qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#001_testsweep_15-42-57/snapshot.json`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/snapshot.json` & `qcodes-0.9.0rc1/qcodes/tests/dataset/fixtures/2018-01-17/#002_2D_test_15-43-14/snapshot.json`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/helper_functions.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/interdeps_fixtures.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/interdeps_fixtures.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/temporary_databases.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/temporary_databases.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_database_creation_and_upgrading.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_database_creation_and_upgrading.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_database_extract_runs.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_database_extract_runs.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_datasaver.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_datasaver.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_dataset_basic.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_dataset_basic.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_dataset_loading.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_dataset_loading.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_dependencies.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_descriptions.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_descriptions.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_experiment_container.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_experiment_container.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_fix_functions.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_fix_functions.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_guids.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_guids.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_links.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_links.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_measurement_context_manager.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_measurement_context_manager.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_metadata.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_metadata.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_paramspec.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_paramspec.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_plotting.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_plotting.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_snapshot.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_sqlite_base.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_sqlite_base.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_sqlite_connection.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_string_data.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_string_data.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset/test_subscribing.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset/test_subscribing.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/dataset_generators.py` & `qcodes-0.9.0rc1/qcodes/tests/dataset_generators.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/test_alazar_api.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/test_alazar_api.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/test_alazar_buffer.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/test_alazar_buffer.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/AlazarTech/test_dll_wrapper.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/AlazarTech/test_dll_wrapper.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/auxiliary_files/awgSeqDataSets.xsd` & `qcodes-0.9.0rc1/qcodes/tests/drivers/auxiliary_files/awgSeqDataSets.xsd`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500_module.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1500_module.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1517a_smu.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1517a_smu.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1520a_cmu.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_b1520a_cmu.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_sampling_measurement.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/b1500_driver_tests/test_sampling_measurement.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/test_MessageBuilder.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/test_MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/keysight_b1500/test_commandList.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/keysight_b1500/test_commandList.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_Agilent_E8527D.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_Agilent_E8527D.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_AimTTi_PL601P.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_AimTTi_PL601P.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_Keithley_2450.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keithley_2450.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_Keysight_33XXX.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keysight_33XXX.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_Keysight_M3201A.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keysight_M3201A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_Keysight_N6705B.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_Keysight_N6705B.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_MercuryiPS.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_MercuryiPS.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_Rigol_DS1074Z.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_Rigol_DS1074Z.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_ami430.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_ami430.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_keithley_26xx.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_keithley_26xx.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_keithley_s46.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_keithley_s46.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_34465a.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_34465a.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_34934a.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_34934a.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_34980a.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_34980a.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_keysight_b220x.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_keysight_b220x.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_lakeshore.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_lakeshore.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_lakeshore_336.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_lakeshore_336.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_lakeshore_file_parser.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_lakeshore_file_parser.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_m2j.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_m2j.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_rohdeschwarz_HMC804x.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_rohdeschwarz_HMC804x.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_rto_1000.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_rto_1000.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_stahl.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_stahl.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_AWG5014C.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_AWG5014C.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_AWG5208.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_AWG5208.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_AWG70000A.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_AWG70000A.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_tektronix_dpo7200xx.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_tektronix_dpo7200xx.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_weinchel.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_weinchel.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/drivers/test_zihdawg8.py` & `qcodes-0.9.0rc1/qcodes/tests/drivers/test_zihdawg8.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/instrument_mocks.py` & `qcodes-0.9.0rc1/qcodes/tests/instrument_mocks.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_autoloadable_channels.py` & `qcodes-0.9.0rc1/qcodes/tests/test_autoloadable_channels.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_channels.py` & `qcodes-0.9.0rc1/qcodes/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_combined_loop.py` & `qcodes-0.9.0rc1/qcodes/tests/test_combined_loop.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_combined_par.py` & `qcodes-0.9.0rc1/qcodes/tests/test_combined_par.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_command.py` & `qcodes-0.9.0rc1/qcodes/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_config.py` & `qcodes-0.9.0rc1/qcodes/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_data.py` & `qcodes-0.9.0rc1/qcodes/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_delegate_parameter.py` & `qcodes-0.9.0rc1/qcodes/tests/test_delegate_parameter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_deprecate.py` & `qcodes-0.9.0rc1/qcodes/tests/test_deprecate.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_field_vector.py` & `qcodes-0.9.0rc1/qcodes/tests/test_field_vector.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_format.py` & `qcodes-0.9.0rc1/qcodes/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_generic_formatter.py` & `qcodes-0.9.0rc1/qcodes/tests/test_generic_formatter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_group_parameter.py` & `qcodes-0.9.0rc1/qcodes/tests/test_group_parameter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_hdf5formatter.py` & `qcodes-0.9.0rc1/qcodes/tests/test_hdf5formatter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_helpers.py` & `qcodes-0.9.0rc1/qcodes/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_installation_info.py` & `qcodes-0.9.0rc1/qcodes/tests/test_installation_info.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_instrument.py` & `qcodes-0.9.0rc1/qcodes/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_json.py` & `qcodes-0.9.0rc1/qcodes/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_location_provider.py` & `qcodes-0.9.0rc1/qcodes/tests/test_location_provider.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_logger.py` & `qcodes-0.9.0rc1/qcodes/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_loop.py` & `qcodes-0.9.0rc1/qcodes/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_measure.py` & `qcodes-0.9.0rc1/qcodes/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_metadata.py` & `qcodes-0.9.0rc1/qcodes/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_monitor.py` & `qcodes-0.9.0rc1/qcodes/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_parameter.py` & `qcodes-0.9.0rc1/qcodes/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_parameter_with_setpoints.py` & `qcodes-0.9.0rc1/qcodes/tests/test_parameter_with_setpoints.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_plot_utils.py` & `qcodes-0.9.0rc1/qcodes/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_plots.py` & `qcodes-0.9.0rc1/qcodes/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_qcmatplotlib_functions.py` & `qcodes-0.9.0rc1/qcodes/tests/test_qcmatplotlib_functions.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_snapshot.py` & `qcodes-0.9.0rc1/qcodes/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_specialized_parameters.py` & `qcodes-0.9.0rc1/qcodes/tests/test_specialized_parameters.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_station.py` & `qcodes-0.9.0rc1/qcodes/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_sweep_values.py` & `qcodes-0.9.0rc1/qcodes/tests/test_sweep_values.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_testutils.py` & `qcodes-0.9.0rc1/qcodes/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_threading.py` & `qcodes-0.9.0rc1/qcodes/tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_validators.py` & `qcodes-0.9.0rc1/qcodes/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_visa.py` & `qcodes-0.9.0rc1/qcodes/tests/test_visa.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/tests/test_wrong_address.py` & `qcodes-0.9.0rc1/qcodes/tests/test_wrong_address.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/command.py` & `qcodes-0.9.0rc1/qcodes/utils/command.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/delaykeyboardinterrupt.py` & `qcodes-0.9.0rc1/qcodes/utils/delaykeyboardinterrupt.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/deprecate.py` & `qcodes-0.9.0rc1/qcodes/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/helpers.py` & `qcodes-0.9.0rc1/qcodes/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from asyncio import iscoroutinefunction
 from inspect import signature
 from functools import partial
 from collections import OrderedDict
 
 import numpy as np
 
-import qcodes
 from qcodes.utils.deprecate import deprecate
 
 
 QCODES_USER_PATH_ENV = 'QCODES_USER_PATH'
 
 
 _tprint_times: Dict[str, float] = {}
@@ -746,14 +745,15 @@
 
 def get_qcodes_path(*subfolder: str) -> str:
     """
     Return full file path of the QCoDeS module. Additional arguments will be
     appended as subfolder.
 
     """
+    import qcodes
     path = os.sep.join(qcodes.__file__.split(os.sep)[:-1])
     return os.path.join(path, *subfolder) + os.sep
 
 
 def get_qcodes_user_path(*file_parts: str) -> str:
     """
     Get ``~/.qcodes`` path or if defined the path defined in the
```

### Comparing `qcodes-0.9.0a0/qcodes/utils/installation.py` & `qcodes-0.9.0rc1/qcodes/utils/installation.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/installation_info.py` & `qcodes-0.9.0rc1/qcodes/utils/installation_info.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/log_analysis.py` & `qcodes-0.9.0rc1/qcodes/utils/log_analysis.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/magic.py` & `qcodes-0.9.0rc1/qcodes/utils/magic.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/metadata.py` & `qcodes-0.9.0rc1/qcodes/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/plotting.py` & `qcodes-0.9.0rc1/qcodes/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/slack.py` & `qcodes-0.9.0rc1/qcodes/utils/slack.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/threading.py` & `qcodes-0.9.0rc1/qcodes/utils/threading.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/types.py` & `qcodes-0.9.0rc1/qcodes/utils/types.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/validators.py` & `qcodes-0.9.0rc1/qcodes/utils/validators.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes/utils/zmq_helpers.py` & `qcodes-0.9.0rc1/qcodes/utils/zmq_helpers.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/qcodes.egg-info/PKG-INFO` & `qcodes-0.9.0rc1/qcodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcodes
-Version: 0.9.0a0
+Version: 0.9.0rc1
 Summary: Python-based data acquisition framework developed by the Copenhagen / Delft / Sydney / Microsoft quantum computing consortium
 Home-page: https://github.com/QCoDeS/Qcodes
 Maintainer: Jens H Nielsen
 Maintainer-email: Jens.Nielsen@microsoft.com
 License: MIT
 Description: QCoDeS |Build Status Azure| |Build Status Travis| |DOCS| |DOI|
         ==============================================================
```

### Comparing `qcodes-0.9.0a0/qcodes.egg-info/SOURCES.txt` & `qcodes-0.9.0rc1/qcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/setup.py` & `qcodes-0.9.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `qcodes-0.9.0a0/versioneer.py` & `qcodes-0.9.0rc1/versioneer.py`

 * *Files identical despite different names*

