# Comparing `tmp/idspy_dictionaries-33801.1.0.tar.gz` & `tmp/idspy_dictionaries-33801.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idspy_dictionaries-33801.1.0.tar", last modified: Tue Jun 20 13:57:46 2023, max compression
+gzip compressed data, was "idspy_dictionaries-33801.1.1.tar", last modified: Tue Jun 20 16:41:23 2023, max compression
```

## Comparing `idspy_dictionaries-33801.1.0.tar` & `idspy_dictionaries-33801.1.1.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:46.130711 idspy_dictionaries-33801.1.0/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-20 13:57:15.000000 idspy_dictionaries-33801.1.0/LICENSE
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4120 2023-06-20 13:57:46.117050 idspy_dictionaries-33801.1.0/PKG-INFO
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:26.443757 idspy_dictionaries-33801.1.0/idspy_dictionaries/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      130 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      845 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/dataclasses_idsschema.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:27.018645 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_amns_data/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      958 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_amns_data/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    19611 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_amns_data/idspy_amns_data.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:27.270764 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_barometry/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      592 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_barometry/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8905 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_barometry/idspy_barometry.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:27.529618 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bolometer/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      802 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bolometer/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16697 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bolometer/idspy_bolometer.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:27.822248 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bremsstrahlung_visible/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      758 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bremsstrahlung_visible/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    11593 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bremsstrahlung_visible/idspy_bremsstrahlung_visible.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:28.089915 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_calorimetry/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      720 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_calorimetry/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12256 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_calorimetry/idspy_calorimetry.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:28.357669 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_ir/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      620 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_ir/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10829 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_ir/idspy_camera_ir.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:28.652244 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_visible/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1108 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_visible/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    21567 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_visible/idspy_camera_visible.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:28.938716 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_x_rays/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      912 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_x_rays/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    25243 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_x_rays/idspy_camera_x_rays.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:29.208635 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_charge_exchange/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1216 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_charge_exchange/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    28154 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_charge_exchange/idspy_charge_exchange.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:29.501691 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_coils_non_axisymmetric/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      720 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_coils_non_axisymmetric/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12988 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_coils_non_axisymmetric/idspy_coils_non_axisymmetric.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:29.751468 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_controllers/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      784 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_controllers/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12028 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_controllers/idspy_controllers.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:30.002259 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_instant_changes/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1478 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_instant_changes/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    51393 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_instant_changes/idspy_core_instant_changes.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:30.252335 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_profiles/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1424 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_profiles/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    55609 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_profiles/idspy_core_profiles.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:30.537829 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_sources/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2552 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_sources/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    40543 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_sources/idspy_core_sources.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:30.814768 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_transport/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1942 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_transport/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    33952 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_transport/idspy_core_transport.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:31.058703 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_cryostat/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      750 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_cryostat/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12517 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_cryostat/idspy_cryostat.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:31.317494 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_description/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      586 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_description/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     9045 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_description/idspy_dataset_description.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:31.604891 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_fair/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      388 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_fair/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5631 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_fair/idspy_dataset_fair.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:31.876436 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_disruption/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      796 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_disruption/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16728 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_disruption/idspy_disruption.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:32.141771 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distribution_sources/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2578 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distribution_sources/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    40856 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distribution_sources/idspy_distribution_sources.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:32.432448 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distributions/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5422 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distributions/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    96977 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distributions/idspy_distributions.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:32.723736 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_divertors/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      740 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_divertors/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    18690 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_divertors/idspy_divertors.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:33.013181 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ec_launchers/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      694 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ec_launchers/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    11557 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ec_launchers/idspy_ec_launchers.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:33.273246 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ece/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1138 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ece/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    23610 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ece/idspy_ece.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:33.538015 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_profiles/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2840 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_profiles/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    90170 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_profiles/idspy_edge_profiles.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:33.814132 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_sources/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2602 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_sources/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    43261 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_sources/idspy_edge_sources.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:34.080860 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_transport/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2570 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_transport/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    46579 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_transport/idspy_edge_transport.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:34.351640 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_em_coupling/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      434 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_em_coupling/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     9888 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_em_coupling/idspy_em_coupling.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:34.612352 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_equilibrium/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3268 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_equilibrium/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    80102 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_equilibrium/idspy_equilibrium.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:34.912009 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_injection/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      826 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_injection/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12812 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_injection/idspy_gas_injection.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:35.182952 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_pumping/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      652 2023-06-20 13:57:01.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_pumping/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8507 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_pumping/idspy_gas_pumping.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:35.468721 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gyrokinetics/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      946 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gyrokinetics/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    33346 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gyrokinetics/idspy_gyrokinetics.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:35.742647 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_hard_x_rays/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      916 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_hard_x_rays/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24735 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_hard_x_rays/idspy_hard_x_rays.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:36.006481 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ic_antennas/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1372 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ic_antennas/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24317 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ic_antennas/idspy_ic_antennas.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:36.286547 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_interferometer/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      770 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_interferometer/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13160 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_interferometer/idspy_interferometer.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:36.572695 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_iron_core/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      852 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_iron_core/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    14416 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_iron_core/idspy_iron_core.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:36.855034 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_langmuir_probes/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1266 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_langmuir_probes/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    27365 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_langmuir_probes/idspy_langmuir_probes.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:37.143078 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_lh_antennas/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      846 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_lh_antennas/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16299 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_lh_antennas/idspy_lh_antennas.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:37.440064 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_magnetics/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1050 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_magnetics/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    23005 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_magnetics/idspy_magnetics.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:37.713023 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1296 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    22596 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd/idspy_mhd.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:37.987685 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd_linear/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1294 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd_linear/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24665 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd_linear/idspy_mhd_linear.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:38.276649 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mse/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      804 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mse/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16481 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mse/idspy_mse.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:38.512404 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_nbi/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1146 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_nbi/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    23567 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_nbi/idspy_nbi.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:38.782072 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_neutron_diagnostic/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2292 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_neutron_diagnostic/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    34968 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_neutron_diagnostic/idspy_neutron_diagnostic.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:39.066260 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ntms/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1000 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ntms/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    15856 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ntms/idspy_ntms.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:39.335734 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pellets/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1104 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pellets/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16561 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pellets/idspy_pellets.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:39.605810 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_active/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1024 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_active/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24972 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_active/idspy_pf_active.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:39.895843 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_passive/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      862 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_passive/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    14800 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_passive/idspy_pf_passive.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:40.153360 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_plasma_initiation/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      764 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_plasma_initiation/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12253 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_plasma_initiation/idspy_plasma_initiation.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:40.420154 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_polarimeter/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      746 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_polarimeter/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12286 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_polarimeter/idspy_polarimeter.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:40.670977 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pulse_schedule/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2058 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pulse_schedule/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    36247 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pulse_schedule/idspy_pulse_schedule.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:40.964527 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_radiation/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2508 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_radiation/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    40908 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_radiation/idspy_radiation.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:41.253474 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_real_time_data/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      602 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_real_time_data/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8692 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_real_time_data/idspy_real_time_data.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:41.525805 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_reflectometer_profile/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      770 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_reflectometer_profile/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13294 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_reflectometer_profile/idspy_reflectometer_profile.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:41.759825 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_refractometer/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      842 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_refractometer/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13754 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_refractometer/idspy_refractometer.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:41.993867 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_sawteeth/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      604 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_sawteeth/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    19903 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_sawteeth/idspy_sawteeth.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:42.240163 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_soft_x_rays/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      882 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_soft_x_rays/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    21956 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_soft_x_rays/idspy_soft_x_rays.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:42.527310 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_mass/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      510 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_mass/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8302 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_mass/idspy_spectrometer_mass.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:42.818235 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_uv/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1368 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_uv/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    28458 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_uv/idspy_spectrometer_uv.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:43.111477 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_visible/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2118 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_visible/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    41496 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_visible/idspy_spectrometer_visible.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:43.418184 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_x_ray_crystal/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1538 2023-06-20 13:57:02.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_x_ray_crystal/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    43341 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_x_ray_crystal/idspy_spectrometer_x_ray_crystal.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:43.656606 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_summary/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3556 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_summary/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)   105114 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_summary/idspy_summary.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:43.952226 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_temporary/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2548 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_temporary/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    26436 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_temporary/idspy_temporary.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:44.243136 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_tf/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1500 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_tf/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    26876 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_tf/idspy_tf.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:44.529436 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_thomson_scattering/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      796 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_thomson_scattering/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12032 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_thomson_scattering/idspy_thomson_scattering.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:44.814336 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_transport_solver_numerics/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3906 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_transport_solver_numerics/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    68017 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_transport_solver_numerics/idspy_transport_solver_numerics.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:45.107118 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_turbulence/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      860 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_turbulence/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13208 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_turbulence/idspy_turbulence.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:45.416638 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_wall/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4040 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_wall/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    71648 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_wall/idspy_wall.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:45.688493 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_waves/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3844 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_waves/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    73060 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_waves/idspy_waves.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:45.975584 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_workflow/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      596 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_workflow/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10034 2023-06-20 13:57:03.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_workflow/idspy_workflow.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 13:57:26.805064 idspy_dictionaries-33801.1.0/idspy_dictionaries.egg-info/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4120 2023-06-20 13:57:18.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries.egg-info/PKG-INFO
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7685 2023-06-20 13:57:24.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries.egg-info/SOURCES.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-20 13:57:18.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries.egg-info/dependency_links.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       19 2023-06-20 13:57:18.000000 idspy_dictionaries-33801.1.0/idspy_dictionaries.egg-info/top_level.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      822 2023-06-20 13:57:15.000000 idspy_dictionaries-33801.1.0/pyproject.toml
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-20 13:57:46.135635 idspy_dictionaries-33801.1.0/setup.cfg
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-20 13:57:15.000000 idspy_dictionaries-33801.1.0/setup.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:23.271189 idspy_dictionaries-33801.1.1/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-20 16:40:51.000000 idspy_dictionaries-33801.1.1/LICENSE
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4589 2023-06-20 16:41:23.256067 idspy_dictionaries-33801.1.1/PKG-INFO
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:03.000508 idspy_dictionaries-33801.1.1/idspy_dictionaries/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      130 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      845 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/dataclasses_idsschema.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:03.689121 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_amns_data/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      958 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_amns_data/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    19611 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_amns_data/idspy_amns_data.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:03.961031 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_barometry/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      592 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_barometry/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8905 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_barometry/idspy_barometry.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:04.210267 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bolometer/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      802 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bolometer/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16697 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bolometer/idspy_bolometer.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:04.436978 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bremsstrahlung_visible/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      758 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bremsstrahlung_visible/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    11593 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bremsstrahlung_visible/idspy_bremsstrahlung_visible.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:04.711677 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_calorimetry/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      720 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_calorimetry/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12256 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_calorimetry/idspy_calorimetry.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:05.008236 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_ir/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      620 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_ir/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10829 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_ir/idspy_camera_ir.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:05.211133 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_visible/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1108 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_visible/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    21567 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_visible/idspy_camera_visible.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:05.427158 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_x_rays/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      912 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_x_rays/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    25243 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_x_rays/idspy_camera_x_rays.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:05.689337 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_charge_exchange/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1216 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_charge_exchange/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    28154 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_charge_exchange/idspy_charge_exchange.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:05.984680 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_coils_non_axisymmetric/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      720 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_coils_non_axisymmetric/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12988 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_coils_non_axisymmetric/idspy_coils_non_axisymmetric.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:06.298774 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_controllers/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      784 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_controllers/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12028 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_controllers/idspy_controllers.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:06.596699 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_instant_changes/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1478 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_instant_changes/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    51393 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_instant_changes/idspy_core_instant_changes.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:06.907885 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_profiles/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1424 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_profiles/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    55609 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_profiles/idspy_core_profiles.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:07.188867 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_sources/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2552 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_sources/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    40543 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_sources/idspy_core_sources.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:07.495784 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_transport/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1942 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_transport/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    33952 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_transport/idspy_core_transport.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:07.803636 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_cryostat/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      750 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_cryostat/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12517 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_cryostat/idspy_cryostat.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:08.103820 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_description/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      586 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_description/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     9045 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_description/idspy_dataset_description.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:08.408702 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_fair/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      388 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_fair/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5631 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_fair/idspy_dataset_fair.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:08.711616 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_disruption/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      796 2023-06-20 16:40:36.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_disruption/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16728 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_disruption/idspy_disruption.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:08.992477 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distribution_sources/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2578 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distribution_sources/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    40856 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distribution_sources/idspy_distribution_sources.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:09.291621 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distributions/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5422 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distributions/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    96977 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distributions/idspy_distributions.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:09.556122 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_divertors/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      740 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_divertors/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    18690 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_divertors/idspy_divertors.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:09.832680 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ec_launchers/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      694 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ec_launchers/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    11557 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ec_launchers/idspy_ec_launchers.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:10.107966 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ece/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1138 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ece/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    23610 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ece/idspy_ece.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:10.408051 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_profiles/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2840 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_profiles/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    90170 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_profiles/idspy_edge_profiles.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:10.701876 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_sources/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2602 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_sources/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    43261 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_sources/idspy_edge_sources.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:11.015397 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_transport/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2570 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_transport/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    46579 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_transport/idspy_edge_transport.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:11.318909 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_em_coupling/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      434 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_em_coupling/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     9888 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_em_coupling/idspy_em_coupling.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:11.601359 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_equilibrium/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3268 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_equilibrium/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    80102 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_equilibrium/idspy_equilibrium.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:11.896013 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_injection/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      826 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_injection/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12812 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_injection/idspy_gas_injection.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:12.182743 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_pumping/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      652 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_pumping/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8507 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_pumping/idspy_gas_pumping.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:12.476650 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gyrokinetics/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      946 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gyrokinetics/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    33346 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gyrokinetics/idspy_gyrokinetics.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:12.759242 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_hard_x_rays/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      916 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_hard_x_rays/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24735 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_hard_x_rays/idspy_hard_x_rays.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:13.052357 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ic_antennas/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1372 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ic_antennas/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24317 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ic_antennas/idspy_ic_antennas.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:13.353807 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_interferometer/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      770 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_interferometer/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13160 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_interferometer/idspy_interferometer.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:13.647709 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_iron_core/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      852 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_iron_core/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    14416 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_iron_core/idspy_iron_core.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:13.914986 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_langmuir_probes/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1266 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_langmuir_probes/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    27365 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_langmuir_probes/idspy_langmuir_probes.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:14.195185 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_lh_antennas/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      846 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_lh_antennas/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16299 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_lh_antennas/idspy_lh_antennas.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:14.478345 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_magnetics/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1050 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_magnetics/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    23005 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_magnetics/idspy_magnetics.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:14.682834 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1296 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    22596 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd/idspy_mhd.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:14.925753 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd_linear/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1294 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd_linear/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24665 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd_linear/idspy_mhd_linear.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:15.204687 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mse/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      804 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mse/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16481 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mse/idspy_mse.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:15.474298 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_nbi/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1146 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_nbi/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    23567 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_nbi/idspy_nbi.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:15.752284 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_neutron_diagnostic/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2292 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_neutron_diagnostic/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    34968 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_neutron_diagnostic/idspy_neutron_diagnostic.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:16.038562 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ntms/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1000 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ntms/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    15856 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ntms/idspy_ntms.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:16.323188 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pellets/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1104 2023-06-20 16:40:37.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pellets/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    16561 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pellets/idspy_pellets.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:16.618323 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_active/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1024 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_active/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    24972 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_active/idspy_pf_active.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:16.901476 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_passive/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      862 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_passive/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    14800 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_passive/idspy_pf_passive.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:17.211956 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_plasma_initiation/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      764 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_plasma_initiation/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12253 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_plasma_initiation/idspy_plasma_initiation.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:17.513100 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_polarimeter/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      746 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_polarimeter/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12286 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_polarimeter/idspy_polarimeter.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:17.784953 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pulse_schedule/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2058 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pulse_schedule/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    36247 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pulse_schedule/idspy_pulse_schedule.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:18.073754 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_radiation/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2508 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_radiation/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    40908 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_radiation/idspy_radiation.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:18.360190 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_real_time_data/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      602 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_real_time_data/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8692 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_real_time_data/idspy_real_time_data.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:18.655297 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_reflectometer_profile/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      770 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_reflectometer_profile/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13294 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_reflectometer_profile/idspy_reflectometer_profile.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:18.931821 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_refractometer/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      842 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_refractometer/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13754 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_refractometer/idspy_refractometer.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:19.221004 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_sawteeth/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      604 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_sawteeth/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    19903 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_sawteeth/idspy_sawteeth.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:19.511895 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_soft_x_rays/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      882 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_soft_x_rays/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    21956 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_soft_x_rays/idspy_soft_x_rays.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:19.735581 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_mass/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      510 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_mass/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8302 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_mass/idspy_spectrometer_mass.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:19.992679 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_uv/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1368 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_uv/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    28458 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_uv/idspy_spectrometer_uv.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:20.280675 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_visible/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2118 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_visible/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    41496 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_visible/idspy_spectrometer_visible.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:20.575886 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_x_ray_crystal/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1538 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_x_ray_crystal/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    43341 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_x_ray_crystal/idspy_spectrometer_x_ray_crystal.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:20.872859 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_summary/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3556 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_summary/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)   105114 2023-06-20 16:40:39.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_summary/idspy_summary.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:21.129037 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_temporary/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2548 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_temporary/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    26436 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_temporary/idspy_temporary.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:21.414608 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_tf/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1500 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_tf/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    26876 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_tf/idspy_tf.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:21.687629 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_thomson_scattering/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      796 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_thomson_scattering/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    12032 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_thomson_scattering/idspy_thomson_scattering.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:21.945838 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_transport_solver_numerics/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3906 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_transport_solver_numerics/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    68017 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_transport_solver_numerics/idspy_transport_solver_numerics.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:22.223511 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_turbulence/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      860 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_turbulence/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    13208 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_turbulence/idspy_turbulence.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:22.514962 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_wall/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4040 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_wall/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    71648 2023-06-20 16:40:39.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_wall/idspy_wall.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:22.807199 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_waves/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     3844 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_waves/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    73060 2023-06-20 16:40:39.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_waves/idspy_waves.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:23.118208 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_workflow/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      596 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_workflow/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10034 2023-06-20 16:40:38.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_workflow/idspy_workflow.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 16:41:03.414486 idspy_dictionaries-33801.1.1/idspy_dictionaries.egg-info/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4589 2023-06-20 16:40:54.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries.egg-info/PKG-INFO
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7685 2023-06-20 16:41:00.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries.egg-info/SOURCES.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-20 16:40:54.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries.egg-info/dependency_links.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       19 2023-06-20 16:40:54.000000 idspy_dictionaries-33801.1.1/idspy_dictionaries.egg-info/top_level.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1080 2023-06-20 16:40:51.000000 idspy_dictionaries-33801.1.1/pyproject.toml
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-20 16:41:23.276241 idspy_dictionaries-33801.1.1/setup.cfg
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-20 16:40:51.000000 idspy_dictionaries-33801.1.1/setup.py
```

### Comparing `idspy_dictionaries-33801.1.0/LICENSE` & `idspy_dictionaries-33801.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idspy_dictionaries-33801.1.0/PKG-INFO` & `idspy_dictionaries-33801.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idspy_dictionaries
-Version: 33801.1.0
+Version: 33801.1.1
 Summary: IMAS Data Dictionaries converted to Python Dataclass used in the IMAS-GK/IDSPy project
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
@@ -33,30 +33,37 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://gitlab.com/gkdb/imas-gk
 Project-URL: Bug Tracker, https://gitlab.com/gkdb/imas-gk/-/issues
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 IDSPy_Dictionaries
 ==================
 
 IMAS Data Dictionaries converted to Python Dataclass used in the  IDSPy suite.
 
 Prerequisites
 =============
 
-To use this script, you need to have Python **3.10** or later installed. You can download Python from https://www.python.org/downloads/.
+To use this script, you need to have Python **3.9** or later installed. You can download Python from https://www.python.org/downloads/.
+Please note that Python at least **3.10** is recommended.
 
 Installation
 ============
 
 To install the necessary packages, run the following command:
 
 .. code-block:: console
@@ -73,23 +80,25 @@
    from idspy_dictionaries import ids_gyrokinetics # or any other available IDS
    new_ids = ids_gyrokinetics.Gyrokinetics()
 
 FAQ
 ===
 
 **Q:** What is the minimum required version of Python to run this script?
-  **A:** The minimum recommended version of Python is 3.10. It can be used with Python >= 3.8
+  **A:** The  recommended version of Python is 3.10. It can be used with Python >= 3.9
           but there is no support in that case.
 
 **Q:** Can I add new members to the dataclasses?
   **A:** This option is not possible to be sure that the dataclasses follow the IMAS conventions.
 
 **Q:** Is the package compatible with pydantic and/or attrs?
   **A:** Short answer, no ;)
 
-**Q:** I would really like to use python <3.10 is it really impossible?
+**Q:** I would really like to use python <3.9 is it really impossible?
   **A:** IDSPy_dictionaries used mainly python dataclasses and the slot property which had been added in python 3.10 only.
          The main reason to use __slots__ is to avoid addition of members in the IDS and remains fully compliant with IMAS.
-         A version of the package had been published "as it is" without the slots dependency and is available through pip.
+         A version of the package had been published "as it is" without the slots dependency but need at least python 3.9.
+         The way dataclasses are generated with the associated fields, at the opposite, is not compatible at all with python 3.8.
+
 
 **Q:** Can I load all the dictionaries at once?
   **A:** For performances reasons, it's not possible right now.
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/dataclasses_idsschema.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/dataclasses_idsschema.py`

 * *Files identical despite different names*

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_amns_data/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_amns_data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_amns_data.idspy_amns_data import (
     AmnsData,
     AmnsDataCoordinateSystem,
     AmnsDataCoordinateSystemCoordinate,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_amns_data/idspy_amns_data.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_amns_data/idspy_amns_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_barometry/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_barometry/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_barometry.idspy_barometry import (
     Barometry,
     BarometryGauge,
     Code,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_barometry/idspy_barometry.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_barometry/idspy_barometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bolometer/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bolometer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_bolometer.idspy_bolometer import (
     Bolometer,
     BolometerChannel,
     Code,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bolometer/idspy_bolometer.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bolometer/idspy_bolometer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bremsstrahlung_visible/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bremsstrahlung_visible/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_bremsstrahlung_visible.idspy_bremsstrahlung_visible import (
     BremsstrahlungChannel,
     BremsstrahlungVisible,
     Code,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_bremsstrahlung_visible/idspy_bremsstrahlung_visible.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_bremsstrahlung_visible/idspy_bremsstrahlung_visible.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_calorimetry/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_calorimetry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_calorimetry.idspy_calorimetry import (
     Calorimetry,
     CalorimetryCoolingLoop,
     CalorimetryGroup,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_calorimetry/idspy_calorimetry.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_calorimetry/idspy_calorimetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_ir/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_ir/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_camera_ir.idspy_camera_ir import (
     CameraIr,
     CameraIrCalibration,
     CameraIrFrame,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_ir/idspy_camera_ir.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_ir/idspy_camera_ir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_visible/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_visible/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_camera_visible.idspy_camera_visible import (
     CameraVisible,
     CameraVisibleChannel,
     CameraVisibleDetector,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_visible/idspy_camera_visible.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_visible/idspy_camera_visible.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_x_rays/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_x_rays/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_camera_x_rays.idspy_camera_x_rays import (
     CameraGeometry,
     CameraXRays,
     CameraXRaysFrame,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_camera_x_rays/idspy_camera_x_rays.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_camera_x_rays/idspy_camera_x_rays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_charge_exchange/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_charge_exchange/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_charge_exchange.idspy_charge_exchange import (
     ChargeExchange,
     ChargeExchangeChannel,
     ChargeExchangeChannelBes,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_charge_exchange/idspy_charge_exchange.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_charge_exchange/idspy_charge_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_coils_non_axisymmetric/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_coils_non_axisymmetric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_coils_non_axisymmetric.idspy_coils_non_axisymmetric import (
     Code,
     Coil,
     CoilConductor,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_coils_non_axisymmetric/idspy_coils_non_axisymmetric.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_coils_non_axisymmetric/idspy_coils_non_axisymmetric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_controllers/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_controllers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_controllers.idspy_controllers import (
     Code,
     Controllers,
     ControllersLinearController,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_controllers/idspy_controllers.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_controllers/idspy_controllers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_instant_changes/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_instant_changes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_core_instant_changes.idspy_core_instant_changes import (
     BTorVacuum1,
     Code,
     CoreInstantChanges,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_instant_changes/idspy_core_instant_changes.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_instant_changes/idspy_core_instant_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_profiles/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_profiles/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_core_profiles.idspy_core_profiles import (
     BTorVacuum1,
     Code,
     CoreProfileIons,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_profiles/idspy_core_profiles.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_profiles/idspy_core_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_sources/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_sources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_core_sources.idspy_core_sources import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_sources/idspy_core_sources.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_sources/idspy_core_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_transport/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_transport/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_core_transport.idspy_core_transport import (
     BTorVacuum1,
     Code,
     CodeWithTimebase,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_core_transport/idspy_core_transport.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_core_transport/idspy_core_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_cryostat/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_cryostat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_cryostat.idspy_cryostat import (
     Code,
     Cryostat,
     Cryostat2D,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_cryostat/idspy_cryostat.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_cryostat/idspy_cryostat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_description/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_description/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_dataset_description.idspy_dataset_description import (
     DataEntry,
     DatasetDescription,
     DatasetDescriptionEpochTime,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_description/idspy_dataset_description.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_description/idspy_dataset_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_dataset_fair/idspy_dataset_fair.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_dataset_fair/idspy_dataset_fair.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_disruption/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_disruption/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_disruption.idspy_disruption import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_disruption/idspy_disruption.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_disruption/idspy_disruption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distribution_sources/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distribution_sources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_distribution_sources.idspy_distribution_sources import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distribution_sources/idspy_distribution_sources.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distribution_sources/idspy_distribution_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distributions/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distributions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_distributions.idspy_distributions import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_distributions/idspy_distributions.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_distributions/idspy_distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_divertors/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_divertors/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_divertors.idspy_divertors import (
     Code,
     Divertor,
     DivertorTarget,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_divertors/idspy_divertors.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_divertors/idspy_divertors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ec_launchers/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ec_launchers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_ec_launchers.idspy_ec_launchers import (
     Code,
     EcLaunchers,
     EcLaunchersBeam,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ec_launchers/idspy_ec_launchers.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ec_launchers/idspy_ec_launchers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ece/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ece/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_ece.idspy_ece import (
     Code,
     Ece,
     EceChannel,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ece/idspy_ece.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ece/idspy_ece.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_profiles/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_profiles/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_edge_profiles.idspy_edge_profiles import (
     BTorVacuum1,
     Code,
     EdgeProfileIons,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_profiles/idspy_edge_profiles.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_profiles/idspy_edge_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 2320 5f5f 7665 7273 696f 6e5f 5f3d 2022  # __version__= "
-00000010: 3033 3338 3031 2e31 2e30 220a 2320 5f5f  033801.1.0".# __
+00000010: 3033 3338 3031 2e31 2e31 220a 2320 5f5f  033801.1.1".# __
 00000020: 7665 7273 696f 6e5f 6461 7461 5f64 6963  version_data_dic
 00000030: 7469 6f6e 6172 795f 5f3d 2022 332e 3338  tionary__= "3.38
 00000040: 2e31 220a 2320 5f5f 6769 745f 7665 7273  .1".# __git_vers
 00000050: 696f 6e5f 6861 7368 5f5f 3d20 2264 6436  ion_hash__= "dd6
 00000060: 3835 3462 3464 3037 3334 3832 3831 3061  854b4d073482810a
 00000070: 3233 3833 3965 3665 3531 3338 3663 3766  23839e6e51386c7f
 00000080: 3230 6664 3322 0a23 200a 6672 6f6d 202e  20fd3".# .from .
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_sources/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_sources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_edge_sources.idspy_edge_sources import (
     Code,
     DistributionSpecies,
     EdgeSources,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_sources/idspy_edge_sources.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_sources/idspy_edge_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_transport/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_transport/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_edge_transport.idspy_edge_transport import (
     Code,
     CodeWithTimebase,
     EdgeTransport,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_edge_transport/idspy_edge_transport.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_edge_transport/idspy_edge_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_em_coupling/idspy_em_coupling.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_em_coupling/idspy_em_coupling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_equilibrium/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_equilibrium/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_equilibrium.idspy_equilibrium import (
     BTorVacuum1,
     Code,
     Equilibrium,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_equilibrium/idspy_equilibrium.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_equilibrium/idspy_equilibrium.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_injection/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_injection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_gas_injection.idspy_gas_injection import (
     Code,
     GasInjection,
     GasInjectionPipe,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_injection/idspy_gas_injection.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_injection/idspy_gas_injection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_pumping/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_pumping/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_gas_pumping.idspy_gas_pumping import (
     Code,
     GasPumping,
     GasPumpingDuct,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gas_pumping/idspy_gas_pumping.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gas_pumping/idspy_gas_pumping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gyrokinetics/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gyrokinetics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_gyrokinetics.idspy_gyrokinetics import (
     Code,
     CodePartialConstant,
     EntryTag,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_gyrokinetics/idspy_gyrokinetics.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_gyrokinetics/idspy_gyrokinetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_hard_x_rays/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_hard_x_rays/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_hard_x_rays.idspy_hard_x_rays import (
     Code,
     DetectorAperture,
     DetectorEnergyBand,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_hard_x_rays/idspy_hard_x_rays.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_hard_x_rays/idspy_hard_x_rays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ic_antennas/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ic_antennas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_ic_antennas.idspy_ic_antennas import (
     AnnulusStatic,
     ArcsOfCircleStatic,
     Code,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ic_antennas/idspy_ic_antennas.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ic_antennas/idspy_ic_antennas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_interferometer/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_interferometer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_interferometer.idspy_interferometer import (
     Code,
     IdsProperties,
     IdsProvenance,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_interferometer/idspy_interferometer.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_interferometer/idspy_interferometer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_iron_core/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_iron_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_iron_core.idspy_iron_core import (
     AnnulusStatic,
     ArcsOfCircleStatic,
     Code,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_iron_core/idspy_iron_core.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_iron_core/idspy_iron_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_langmuir_probes/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_langmuir_probes/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_langmuir_probes.idspy_langmuir_probes import (
     Code,
     DataEntry,
     IdentifierStatic,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_langmuir_probes/idspy_langmuir_probes.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_langmuir_probes/idspy_langmuir_probes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_lh_antennas/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_lh_antennas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_lh_antennas.idspy_lh_antennas import (
     Code,
     IdsProperties,
     IdsProvenance,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_lh_antennas/idspy_lh_antennas.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_lh_antennas/idspy_lh_antennas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_magnetics/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_magnetics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_magnetics.idspy_magnetics import (
     Code,
     IdentifierStatic,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_magnetics/idspy_magnetics.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_magnetics/idspy_magnetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_mhd.idspy_mhd import (
     Code,
     GenericGridAos3Root,
     GenericGridDynamicGridSubset,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd/idspy_mhd.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd/idspy_mhd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd_linear/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd_linear/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_mhd_linear.idspy_mhd_linear import (
     BTorVacuum1,
     Code,
     Complex1DMhdAlfvenSpectrum,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mhd_linear/idspy_mhd_linear.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mhd_linear/idspy_mhd_linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mse/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_mse.idspy_mse import (
     Code,
     DetectorAperture,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_mse/idspy_mse.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_mse/idspy_mse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_nbi/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_nbi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_nbi.idspy_nbi import (
     Code,
     DetectorAperture,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_nbi/idspy_nbi.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_nbi/idspy_nbi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_neutron_diagnostic/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_neutron_diagnostic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_neutron_diagnostic.idspy_neutron_diagnostic import (
     Code,
     DetectorAperture,
     DetectorEnergyBand,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_neutron_diagnostic/idspy_neutron_diagnostic.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_neutron_diagnostic/idspy_neutron_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ntms/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ntms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_ntms.idspy_ntms import (
     BTorVacuum1,
     Code,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_ntms/idspy_ntms.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_ntms/idspy_ntms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pellets/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pellets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_pellets.idspy_pellets import (
     Code,
     IdentifierDynamicAos3,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pellets/idspy_pellets.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pellets/idspy_pellets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_active/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_active/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_pf_active.idspy_pf_active import (
     AnnulusStatic,
     ArcsOfCircleStatic,
     Code,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_active/idspy_pf_active.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_active/idspy_pf_active.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_passive/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_passive/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_pf_passive.idspy_pf_passive import (
     AnnulusStatic,
     ArcsOfCircleStatic,
     Code,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pf_passive/idspy_pf_passive.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pf_passive/idspy_pf_passive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_plasma_initiation/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_plasma_initiation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_plasma_initiation.idspy_plasma_initiation import (
     Code,
     EquilibriumProfiles2DGrid,
     IdentifierDynamicAos3,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_plasma_initiation/idspy_plasma_initiation.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_plasma_initiation/idspy_plasma_initiation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_polarimeter/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_polarimeter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_polarimeter.idspy_polarimeter import (
     Code,
     IdsProperties,
     IdsProvenance,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_polarimeter/idspy_polarimeter.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_polarimeter/idspy_polarimeter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pulse_schedule/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pulse_schedule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_pulse_schedule.idspy_pulse_schedule import (
     Code,
     GasMixtureConstant,
     Identifier,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_pulse_schedule/idspy_pulse_schedule.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_pulse_schedule/idspy_pulse_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_radiation/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_radiation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_radiation.idspy_radiation import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_radiation/idspy_radiation.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_radiation/idspy_radiation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_real_time_data/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_real_time_data/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_real_time_data.idspy_real_time_data import (
     Code,
     IdsProperties,
     IdsProvenance,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_real_time_data/idspy_real_time_data.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_real_time_data/idspy_real_time_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_reflectometer_profile/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_reflectometer_profile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_reflectometer_profile.idspy_reflectometer_profile import (
     Code,
     IdsProperties,
     IdsProvenance,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_reflectometer_profile/idspy_reflectometer_profile.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_reflectometer_profile/idspy_reflectometer_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_refractometer/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_refractometer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_refractometer.idspy_refractometer import (
     Code,
     Identifier,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_refractometer/idspy_refractometer.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_refractometer/idspy_refractometer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_sawteeth/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_sawteeth/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_sawteeth.idspy_sawteeth import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_sawteeth/idspy_sawteeth.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_sawteeth/idspy_sawteeth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_soft_x_rays/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_soft_x_rays/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_soft_x_rays.idspy_soft_x_rays import (
     Code,
     DetectorAperture,
     DetectorEnergyBand,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_soft_x_rays/idspy_soft_x_rays.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_soft_x_rays/idspy_soft_x_rays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_mass/idspy_spectrometer_mass.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_mass/idspy_spectrometer_mass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_uv/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_uv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_spectrometer_uv.idspy_spectrometer_uv import (
     Code,
     DetectorAperture,
     Identifier,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_uv/idspy_spectrometer_uv.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_uv/idspy_spectrometer_uv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_visible/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_visible/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_spectrometer_visible.idspy_spectrometer_visible import (
     Code,
     DetectorAperture,
     DetectorImage,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_visible/idspy_spectrometer_visible.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_visible/idspy_spectrometer_visible.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_x_ray_crystal/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_x_ray_crystal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_spectrometer_x_ray_crystal.idspy_spectrometer_x_ray_crystal import (
     CameraGeometry,
     Code,
     CurvedObject,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_spectrometer_x_ray_crystal/idspy_spectrometer_x_ray_crystal.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_spectrometer_x_ray_crystal/idspy_spectrometer_x_ray_crystal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_summary/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_summary/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_summary.idspy_summary import (
     Code,
     EntryTag,
     IdentifierStatic,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_summary/idspy_summary.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_summary/idspy_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_temporary/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_temporary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_temporary.idspy_temporary import (
     Code,
     Identifier,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_temporary/idspy_temporary.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_temporary/idspy_temporary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_tf/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_tf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_tf.idspy_tf import (
     Code,
     DeltaRzphi1DStatic,
     GenericGridDynamic,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_tf/idspy_tf.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_tf/idspy_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_thomson_scattering/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_thomson_scattering/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_thomson_scattering.idspy_thomson_scattering import (
     Code,
     DataEntry,
     IdentifierStatic,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_thomson_scattering/idspy_thomson_scattering.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_thomson_scattering/idspy_thomson_scattering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_transport_solver_numerics/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_transport_solver_numerics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_transport_solver_numerics.idspy_transport_solver_numerics import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_transport_solver_numerics/idspy_transport_solver_numerics.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_transport_solver_numerics/idspy_transport_solver_numerics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_turbulence/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_turbulence/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_turbulence.idspy_turbulence import (
     Code,
     Identifier,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_turbulence/idspy_turbulence.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_turbulence/idspy_turbulence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_wall/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_wall/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_wall.idspy_wall import (
     Code,
     GenericGridAos3Root,
     GenericGridDynamicGridSubset,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_wall/idspy_wall.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_wall/idspy_wall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_waves/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_waves/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_waves.idspy_waves import (
     BTorVacuum1,
     Code,
     CoreRadialGrid,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_waves/idspy_waves.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_waves/idspy_waves.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Dict, Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_workflow/__init__.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_workflow/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from idspy_dictionaries.ids_workflow.idspy_workflow import (
     Code,
     CodeConstant,
     IdsProperties,
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries/ids_workflow/idspy_workflow.py` & `idspy_dictionaries-33801.1.1/idspy_dictionaries/ids_workflow/idspy_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# __version__= "033801.1.0"
+# __version__= "033801.1.1"
 # __version_data_dictionary__= "3.38.1"
 # __git_version_hash__= "dd6854b4d073482810a23839e6e51386c7f20fd3"
 # 
 from ..dataclasses_idsschema import _IDSPYDD_USE_SLOTS,IdsBaseClass
 from dataclasses import dataclass, field
 from numpy import ndarray
 from typing import Optional
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries.egg-info/PKG-INFO` & `idspy_dictionaries-33801.1.1/idspy_dictionaries.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idspy-dictionaries
-Version: 33801.1.0
+Version: 33801.1.1
 Summary: IMAS Data Dictionaries converted to Python Dataclass used in the IMAS-GK/IDSPy project
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
@@ -33,30 +33,37 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://gitlab.com/gkdb/imas-gk
 Project-URL: Bug Tracker, https://gitlab.com/gkdb/imas-gk/-/issues
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 IDSPy_Dictionaries
 ==================
 
 IMAS Data Dictionaries converted to Python Dataclass used in the  IDSPy suite.
 
 Prerequisites
 =============
 
-To use this script, you need to have Python **3.10** or later installed. You can download Python from https://www.python.org/downloads/.
+To use this script, you need to have Python **3.9** or later installed. You can download Python from https://www.python.org/downloads/.
+Please note that Python at least **3.10** is recommended.
 
 Installation
 ============
 
 To install the necessary packages, run the following command:
 
 .. code-block:: console
@@ -73,23 +80,25 @@
    from idspy_dictionaries import ids_gyrokinetics # or any other available IDS
    new_ids = ids_gyrokinetics.Gyrokinetics()
 
 FAQ
 ===
 
 **Q:** What is the minimum required version of Python to run this script?
-  **A:** The minimum recommended version of Python is 3.10. It can be used with Python >= 3.8
+  **A:** The  recommended version of Python is 3.10. It can be used with Python >= 3.9
           but there is no support in that case.
 
 **Q:** Can I add new members to the dataclasses?
   **A:** This option is not possible to be sure that the dataclasses follow the IMAS conventions.
 
 **Q:** Is the package compatible with pydantic and/or attrs?
   **A:** Short answer, no ;)
 
-**Q:** I would really like to use python <3.10 is it really impossible?
+**Q:** I would really like to use python <3.9 is it really impossible?
   **A:** IDSPy_dictionaries used mainly python dataclasses and the slot property which had been added in python 3.10 only.
          The main reason to use __slots__ is to avoid addition of members in the IDS and remains fully compliant with IMAS.
-         A version of the package had been published "as it is" without the slots dependency and is available through pip.
+         A version of the package had been published "as it is" without the slots dependency but need at least python 3.9.
+         The way dataclasses are generated with the associated fields, at the opposite, is not compatible at all with python 3.8.
+
 
 **Q:** Can I load all the dictionaries at once?
   **A:** For performances reasons, it's not possible right now.
```

### Comparing `idspy_dictionaries-33801.1.0/idspy_dictionaries.egg-info/SOURCES.txt` & `idspy_dictionaries-33801.1.1/idspy_dictionaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idspy_dictionaries-33801.1.0/pyproject.toml` & `idspy_dictionaries-33801.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,32 @@
     "setuptools>=61.0.0",
     "wheel",
 ]
 # build-backend = "setuptools.build_meta"
 
 [project]
 name = "idspy_dictionaries"
-version = "033801.1.0"
+version = "033801.1.1"
 description = "IMAS Data Dictionaries converted to Python Dataclass used in the IMAS-GK/IDSPy project"
 authors = [
   { name = "Guillaume Fuhr", email = "guillaume.fuhr@univ-amu.fr" },
 ]
 license = { file = "LICENSE" }
 readme = "README.rst"
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    'Development Status :: 4 - Beta',
+    'Environment :: Console',
+    'Intended Audience :: Science/Research',
+    'License :: OSI Approved :: MIT License',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Topic :: Scientific/Engineering'
 ]
 requires-python = ">=3.10"
 
 dependencies = []
 
 [project.urls]
 "Homepage" = "https://gitlab.com/gkdb/imas-gk"
```

