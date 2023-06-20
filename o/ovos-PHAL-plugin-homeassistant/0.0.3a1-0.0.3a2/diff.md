# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.3a1.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.3a1.tar", last modified: Sat Jun 10 02:06:04 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.3a2.tar", last modified: Tue Jun 20 16:52:42 2023, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1.tar` & `ovos-PHAL-plugin-homeassistant-0.0.3a2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35653 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/code/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.700117 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/icon/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:06:04.704117 ovos-PHAL-plugin-homeassistant-0.0.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-10 02:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.321889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28135 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.329889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.329889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.329889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.321889 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,28 @@
             "ovos-PHAL-plugin-homeassistant": {
                 "host": "https://someurl.toinstance",
                 "api_key": "api key from the instance"
             }
         }
    ```
 
+The config also takes an optional property, `brightness_increment`, which is the amount to increment/decrement the brightness of a light when the brightness up/down commands are sent. The default value is 10 and represents a percentage, e.g. 10%.
+
+Sample config:
+
+```json
+        "PHAL": {
+            "ovos-PHAL-plugin-homeassistant": {
+                "host": "https://someurl.toinstance",
+                "api_key": "api key from the instance",
+                "brightness_increment": 5
+            }
+        }
+```
+
 ### Usage
 
 The plugin provides a GUI interface for Home Assistant Instances. It also provides an API for other plugins or skills to user.
 
 The plugin is in early development, so there are some features that are not yet implemented. It currently supports the following entities:
 - Media Player
 - Light
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import uuid
-import asyncio
 from copy import deepcopy
 from os.path import dirname, join
 from typing import Optional
 
-from pfzy import fuzzy_match
 from ovos_utils.log import LOG
 from ovos_bus_client import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.gui import GUIInterface
+from ovos_utils.parse import match_one
 from ovos_PHAL_plugin_homeassistant.logic.connector import HomeAssistantRESTConnector, HomeAssistantWSConnector
 from ovos_PHAL_plugin_homeassistant.logic.device import (HomeAssistantSensor,
                                                          HomeAssistantBinarySensor,
                                                          HomeAssistantLight, HomeAssistantAutomation,
                                                          HomeAssistantMediaPlayer, HomeAssistantScene,
                                                          HomeAssistantVacuum, HomeAssistantSwitch,
                                                          HomeAssistantClimate, HomeAssistantCamera)
@@ -55,14 +54,15 @@
         self.bus = bus
         self.gui = GUIInterface(bus=self.bus, skill_id=self.name,
                                 config=self.config_core.get('gui'))
         self.integrator = Integrator(self.bus, self.gui)
         self.instance_available = False
         self.use_ws = False
         self.device_types = SUPPORTED_DEVICES
+        self.brightness_increment = self.get_brightness_increment()
 
         # BUS API FOR HOME ASSISTANT
         self.bus.on("ovos.phal.plugin.homeassistant.get.devices",
                     self.handle_get_devices)
         self.bus.on("ovos.phal.plugin.homeassistant.get.device",
                     self.handle_get_device)
         self.bus.on("ovos.phal.plugin.homeassistant.device.turn_on",
@@ -109,14 +109,22 @@
         # LISTEN FOR OAUTH RESPONSE
         self.bus.on("oauth.app.host.info.response", self.handle_oauth_host_info)
         self.bus.on("oauth.generate.qr.response", self.handle_qr_oauth_response)
         self.bus.on(f"oauth.token.response.{self.munged_id}", self.handle_token_oauth_response)
 
         self.init_configuration()
 
+    def get_brightness_increment(self) -> int:
+        """ Get the brightness increment from the config
+
+            Returns:
+                int: The brightness increment
+        """
+        return self.config.get("brightness_increment", 10)
+
 # SETUP INSTANCE SUPPORT
     def validate_instance_connection(self, host, api_key):
         """ Validate the connection to the Home Assistant instance
 
             Args:
                 host (str): The Home Assistant instance URL
                 api_key (str): The Home Assistant API key
@@ -343,14 +351,15 @@
         device_id = message.data.get("device_id", None)
         if device_id is not None:
             LOG.debug(f"Device ID provided in bus message: {device_id}")
             return self._return_device_response(message, device_id)
 
         # Device ID not provided, usually VUI
         device = message.data.get("device")
+        device_result = match_one(device, self.registered_device_names)
         device_result = self.fuzzy_match_name(
                             self.registered_devices,
                             device,
                             self.registered_device_names
                         )
         LOG.debug(f"No device ID, found device result: {device_result or 'None'}")
         if device_result:
@@ -533,36 +542,36 @@
 
         Args:
             message (Message): The message object
         """
         device_id, spoken_device = self._gather_device_id(message)
         for device in self.registered_devices:
             if device.device_id == device_id:
-                brightness = device.increase_brightness()
+                device.increase_brightness(self.brightness_increment)
                 return self.bus.emit(message.response(data={
                     "device": spoken_device,
-                    "brightness": get_percentage_brightness_from_ha_value(brightness)
+                    "brightness": get_percentage_brightness_from_ha_value(device.get_brightness())
                     }))
         response = "Device id not provided"
         LOG.error(response)
         return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
 
     def handle_decrease_light_brightness(self, message):
         """ Handle the decrease light brightness message
 
         Args:
             message (Message): The message object
         """
         device_id, spoken_device = self._gather_device_id(message)
         for device in self.registered_devices:
             if device.device_id == device_id:
-                brightness = device.decrease_brightness()
+                brightness = device.decrease_brightness(self.brightness_increment)
                 return self.bus.emit(message.response(data={
                     "device": spoken_device,
-                    "brightness": get_percentage_brightness_from_ha_value(brightness)
+                    "brightness": get_percentage_brightness_from_ha_value(device.get_brightness())
                     }))
         response = "Device id not provided"
         LOG.error(response)
         return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
 
     def handle_get_device_display_model(self, message):
         """ Handle the get device display model message
@@ -739,15 +748,15 @@
         """ Handle the start oauth flow message
 
             Args:
                 message (Message): The message object
         """
         instance = message.data.get("instance", None)
         if instance:
-            self.temporary_instance = instance
+            self.temporary_instance = instance.lower()
             self.request_host_info_from_oauth()
 
     def oauth_register(self):
         """ Register the phal plugin with the oauth service """
         host = self.temporary_instance.replace("ws://", "http://").replace("wss://", "https://")
         auth_endpoint = f"{host}/auth/authorize"
         token_endpoint = f"{host}/auth/token"
@@ -811,18 +820,14 @@
         self.bus.emit(Message("ovos.phal.plugin.homeassistant.device.state.updated"))
 
 # UTILS
     def fuzzy_match_name(self, devices_list, spoken_name, device_names) -> Optional[str]:
         """Given a list of device names, fuzzy match the spoken name to the most likely one.
         Returns the device id of the most likely match or None if no match is found.
         """
-        # https://github.com/kazhala/pfzy/issues/1 fuzzy_match mutates its haystack
-        device_names_haystack = deepcopy(device_names)
-        try:
-            result = asyncio.run(fuzzy_match(spoken_name, device_names_haystack))
-            if result:
-                return devices_list[device_names.index(result[0].get("value"))].device_id
-            else:
-                return None
-        except TypeError:
-            LOG.error(f"Failed to fuzzy match device name {spoken_name}", exc_info=True)
+        device, score = match_one(spoken_name, device_names)
+        if score > 0.75:
+            return devices_list[device_names.index(device)].device_id
+        else:
+            LOG.info(f"Device name '{spoken_name}' not found, closest match is '{device}' with confidence score {score}")
+            LOG.info(f"Score of {score} is too low, returning None")
             return None
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/connector.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/connector.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/device.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -275,29 +275,23 @@
         Args:
             brightness (int): The brightness to set the light to.
         """
         LOG.debug(f"Setting brightness to {brightness}")
         self.call_function("turn_on", {"brightness": brightness})
         self.update_device()
 
-    def increase_brightness(self) -> int:
-        """Increase the brightness of the light by 10%."""
-        current_brightness = self.get_brightness()
-        bumped_value = min(current_brightness + current_brightness * 0.1, 255)
-        LOG.debug(f"Setting brightness to {bumped_value}")
-        self.call_function("turn_on", {"brightness": bumped_value})
+    def increase_brightness(self, brightness_increment: int = 10) -> int:
+        """Increase the brightness of the light by the brightness increment."""
+        bumped_value = self.call_function("turn_on", {"brightness_step_pct": brightness_increment})
         self.update_device()
         return bumped_value
 
-    def decrease_brightness(self) -> int:
-        """Decrease the brightness of the light by 10%."""
-        current_brightness = self.get_brightness()
-        decreased_value = max(current_brightness - current_brightness * 0.1, 0)
-        LOG.debug(f"Setting brightness to {decreased_value}")
-        self.call_function("turn_on", {"brightness": decreased_value})
+    def decrease_brightness(self, brightness_increment: int = 10) -> int:
+        """Decrease the brightness of the light by the brightness increment."""
+        decreased_value = self.call_function("turn_on", {"brightness_step_pct": -brightness_increment})
         self.update_device()
         return decreased_value
 
     def set_color(self, color):
         """Set the color of the light.
 
         Args:
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/integration.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/integration.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/socketclient.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/socketclient.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/logic/utils.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/code/helper.js` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/code/helper.js`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a1/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a2/setup.py`

 * *Files identical despite different names*

