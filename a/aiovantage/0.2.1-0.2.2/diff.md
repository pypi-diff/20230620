# Comparing `tmp/aiovantage-0.2.1.tar.gz` & `tmp/aiovantage-0.2.2.tar.gz`

## Comparing `aiovantage-0.2.1.tar` & `aiovantage-0.2.2.tar`

### file list

```diff
@@ -1,134 +1,135 @@
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiovantage-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 aiovantage-0.2.1/TODO
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/dump_system.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/monitor_all.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/control_load.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.2.1/examples/tasks/run_task.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/query.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/client.py
--rw-r--r--   0        0        0    10260 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/connection.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/errors.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/response.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/client.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/errors.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/config_client/objects/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aiovantage-0.2.1/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aiovantage-0.2.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.2.1/LICENSE
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 aiovantage-0.2.1/README.md
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 aiovantage-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 aiovantage-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiovantage-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aiovantage-0.2.2/TODO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/dump_system.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/monitor_all.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/tasks/run_task.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/client.py
+-rw-r--r--   0        0        0    10260 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/connection.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/errors.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/response.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/client.py
+-rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/connection.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/errors.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 aiovantage-0.2.2/README.md
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 aiovantage-0.2.2/PKG-INFO
```

### Comparing `aiovantage-0.2.1/CONTRIBUTING.md` & `aiovantage-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/dump_system.py` & `aiovantage-0.2.2/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/monitor_all.py` & `aiovantage-0.2.2/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/areas/dump_areas.py` & `aiovantage-0.2.2/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.2.2/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/blinds/dump_blinds.py` & `aiovantage-0.2.2/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/blinds/monitor_blinds.py` & `aiovantage-0.2.2/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/buttons/dump_buttons.py` & `aiovantage-0.2.2/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/buttons/monitor_buttons.py` & `aiovantage-0.2.2/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/command_client/event_log.py` & `aiovantage-0.2.2/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/command_client/status_load.py` & `aiovantage-0.2.2/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/config_client/dump_objects.py` & `aiovantage-0.2.2/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/config_client/get_version.py` & `aiovantage-0.2.2/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.2.2/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.2.2/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/gmem/dump_gmem.py` & `aiovantage-0.2.2/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/gmem/monitor_gmem.py` & `aiovantage-0.2.2/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/gmem/set_gmem.py` & `aiovantage-0.2.2/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/load_groups/dump_load_groups.py` & `aiovantage-0.2.2/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/loads/control_load.py` & `aiovantage-0.2.2/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/loads/dump_loads.py` & `aiovantage-0.2.2/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/loads/monitor_loads.py` & `aiovantage-0.2.2/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/loads/poll_on_loads.py` & `aiovantage-0.2.2/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/loads/toggle_load.py` & `aiovantage-0.2.2/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.2.2/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.2.2/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.2.2/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.2.2/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/stations/dump_stations.py` & `aiovantage-0.2.2/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/tasks/dump_tasks.py` & `aiovantage-0.2.2/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/examples/tasks/run_task.py` & `aiovantage-0.2.2/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/__init__.py` & `aiovantage-0.2.2/src/aiovantage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         config_port: Optional[int] = None,
         command_port: Optional[int] = None,
     ) -> None:
         """Initialize the Vantage instance."""
 
         # Set up config and command clients
         self._config_client = ConfigClient(
-            host, username, password, use_ssl=use_ssl, port=config_port
+            host, username, password, ssl=use_ssl, port=config_port
         )
 
         self._command_client = CommandClient(
             host, username, password, ssl=use_ssl, port=command_port
         )
 
         # Set up controllers
```

### Comparing `aiovantage-0.2.1/src/aiovantage/query.py` & `aiovantage-0.2.2/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/README.md` & `aiovantage-0.2.2/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/__init__.py` & `aiovantage-0.2.2/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/client.py` & `aiovantage-0.2.2/src/aiovantage/command_client/client.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/connection.py` & `aiovantage-0.2.2/src/aiovantage/command_client/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/errors.py` & `aiovantage-0.2.2/src/aiovantage/command_client/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/events.py` & `aiovantage-0.2.2/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/response.py` & `aiovantage-0.2.2/src/aiovantage/command_client/response.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/utils.py` & `aiovantage-0.2.2/src/aiovantage/command_client/utils.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/README.md` & `aiovantage-0.2.2/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/__init__.py` & `aiovantage-0.2.2/src/aiovantage/config_client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,23 @@
 this port has been opened by the firewall on the controller.
 
 The service is discoverable via mDNS as `_aci._tcp.local` and/or
 `_secure_aci._tcp.local`.
 """
 
 from .client import ConfigClient
-from .errors import ClientConnectionError, ClientError, ClientTimeoutError
+from .connection import ConfigConnection
+from .errors import (
+    ClientConnectionError,
+    ClientError,
+    ClientTimeoutError,
+    LoginFailedError,
+)
 
 __all__ = [
     "ConfigClient",
+    "ConfigConnection",
     "ClientConnectionError",
     "ClientError",
     "ClientTimeoutError",
+    "LoginFailedError",
 ]
```

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/client.py` & `aiovantage-0.2.2/src/aiovantage/config_client/connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,76 @@
 """Client for the Vantage Application Communication Interface (ACI) service."""
 
 import asyncio
 import logging
-import ssl
+from ssl import CERT_NONE, SSLContext, create_default_context
 from types import TracebackType
-from typing import Any, Optional, Tuple, Type, Union
+from typing import Any, Optional, Type, Union
 from xml.etree import ElementTree
 
 from typing_extensions import Self
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.handlers import XmlEventHandler
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from .errors import ClientConnectionError, ClientTimeoutError
 from .methods import Call, Method, Return
-from .methods.login import Login
 
-# Type alias for connections
-Connection = Tuple[asyncio.StreamReader, asyncio.StreamWriter]
 
-
-class ConfigClient:
-    """Client for the Vantage Application Communication Interface (ACI) service.
-
-    This client handles connecting to the ACI service, authenticating, and the
-    serialization/deserialization of XML requests and responses.
-    """
+class ConfigConnection:
+    """A connection to the Vantage ACI service."""
 
     def __init__(
         self,
         host: str,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-        *,
-        use_ssl: Union[ssl.SSLContext, bool] = True,
         port: Optional[int] = None,
-        conn_timeout: float = 5,
-        read_timeout: float = 60,
-    ):
-        """Initialize the ConfigClient instance.
+        *,
+        ssl: Union[SSLContext, bool] = True,
+        conn_timeout: Optional[float] = 5,
+        read_timeout: Optional[float] = 30,
+    ) -> None:
+        """Create a connection to the Vantage ACI service.
 
         Args:
-            host: The hostname or IP address of the ACI service.
-            username: The username to use when authenticating with the ACI service.
-            password: The password to use when authenticating with the ACI service.
-            use_ssl: Whether to use SSL when connecting to the ACI service.
-            port: The port to use when connecting to the ACI service.
-            conn_timeout: The timeout to use when connecting.
-            read_timeout: The timeout to use when making requests.
+            host: The hostname or IP address of the Vantage host.
+            port: The port to connect to. Defaults to 3010 if SSL is enabled, else 3001.
+            ssl: Whether to use SSL for the connection. If True, a default SSL context
+                will be created. If False, SSL will not be used. If a SSLContext is
+                provided, it will be used.
+            conn_timeout: The timeout for establishing a connection, in seconds.
+            read_timeout: The timeout for reading a response, in seconds.
         """
 
         self._host = host
-        self._username = username
-        self._password = password
-        self._ssl_context = None
-        self._logger = logging.getLogger(__name__)
-        self._connection: Optional[Connection] = None
         self._conn_timeout = conn_timeout
         self._read_timeout = read_timeout
+        self._reader: Optional[asyncio.StreamReader] = None
+        self._writer: Optional[asyncio.StreamWriter] = None
         self._lock = asyncio.Lock()
+        self._logger = logging.getLogger(__name__)
 
-        # Set up SSL context
-        if use_ssl is True:
+        # Set up the SSL context
+        self._ssl: Optional[SSLContext]
+        if ssl is True:
             # We don't have a local issuer certificate to check against, and we'll be
             # connecting to an IP address so we can't check the hostname
-            self._ssl_context = ssl.create_default_context()
-            self._ssl_context.check_hostname = False
-            self._ssl_context.verify_mode = ssl.CERT_NONE
-        elif isinstance(use_ssl, ssl.SSLContext):
-            self._ssl_context = use_ssl
+            self._ssl = create_default_context()
+            self._ssl.check_hostname = False
+            self._ssl.verify_mode = CERT_NONE
+        elif isinstance(ssl, SSLContext):
+            self._ssl = ssl
+        else:
+            self._ssl = None
 
-        # Set up port
+        # Set up the port
+        self._port: int
         if port is None:
-            self._port = 2010 if use_ssl else 2001
+            self._port = 2010 if ssl else 2001
         else:
             self._port = port
 
         # Set up XML parser and serializer
         self._parser = XmlParser(
             config=ParserConfig(fail_on_unknown_properties=False),
             handler=XmlEventHandler,
@@ -86,73 +78,106 @@
 
         self._serializer = XmlSerializer(
             config=SerializerConfig(xml_declaration=False),
         )
 
     async def __aenter__(self) -> Self:
         """Return context manager."""
+        await self.open()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        traceback: Optional[TracebackType],
     ) -> None:
         """Exit context manager."""
         self.close()
         if exc_val:
             raise exc_val
 
-    def close(self) -> None:
-        """Close any open connections to the ACI service."""
+    async def open(self) -> None:
+        """Open a connection to the Vantage ACI service."""
 
-        # Check if connection is already closed
-        if self._connection is None or self._connection[1].is_closing():
+        # If we're already connected, do nothing
+        if self._writer is not None and not self._writer.is_closing():
             return
 
-        # Close the connection
-        _, writer = self._connection
-        writer.close()
+        # Create the connection
+        try:
+            self._reader, self._writer = await asyncio.wait_for(
+                asyncio.open_connection(
+                    self._host,
+                    self._port,
+                    ssl=self._ssl,
+                    limit=2**20,
+                ),
+                timeout=self._conn_timeout,
+            )
+        except asyncio.TimeoutError as exc:
+            raise ClientTimeoutError(
+                f"Timed out connecting to {self._host}:{self._port}"
+            ) from exc
+        except OSError as exc:
+            raise ClientConnectionError(
+                f"Failed to connect to {self._host}:{self._port}"
+            ) from exc
+
+    def close(self) -> None:
+        """Close the connection to the Vantage ACI service."""
+
+        if self._writer is not None and not self._writer.is_closing():
+            self._writer.close()
+            self._writer = None
 
-        self._logger.debug("Connection closed")
+    @property
+    def closed(self) -> bool:
+        """Whether the connection is closed."""
+
+        return self._writer is None or self._writer.is_closing()
 
     async def raw_request(self, interface: str, payload: str) -> str:
         """Send a plaintext request to the ACI service.
 
         Args:
             interface: The interface to send the request to
             payload: The request payload string to send
 
         Returns:
             The response payload string
         """
 
-        async with self._lock:
-            # Get a connection
-            reader, writer = await self._get_connection()
+        # Make sure we're connected
+        if self._reader is None or self._writer is None or self._writer.is_closing():
+            raise ClientConnectionError("Not connected to Vantage ACI service")
 
+        async with self._lock:
             try:
                 # Send the request
                 request = f"<{interface}>{payload}</{interface}>"
-                writer.write(request.encode())
-                await writer.drain()
+                self._logger.debug(request)
+                self._writer.write(request.encode())
+                await self._writer.drain()
 
                 # Fetch the response
                 end_bytes = f"</{interface}>\n".encode()
                 data = await asyncio.wait_for(
-                    reader.readuntil(end_bytes), timeout=self._read_timeout
+                    self._reader.readuntil(end_bytes), timeout=self._read_timeout
                 )
 
             except asyncio.TimeoutError as err:
                 raise ClientTimeoutError from err
             except (OSError, asyncio.IncompleteReadError) as err:
                 raise ClientConnectionError from err
 
-            return data.decode()
+            response = data.decode()
+            self._logger.debug(response)
+
+            return response
 
     async def request(
         self, method_cls: Type[Method[Call, Return]], params: Any = None
     ) -> Return:
         """Marshall a request, send it to the ACI service, and yield a parsed object.
 
         Args:
@@ -165,76 +190,29 @@
 
         # Build the method object
         method = method_cls()
         method.call = params
 
         # Render the method object to XML with xsdata
         request = self._serializer.render(method)
-        self._logger.debug(request)
-
         response = await self.raw_request(method.interface, request)
-        self._logger.debug(response)
 
         # Parse the XML doc
         tree = ElementTree.fromstring(response)
 
         # Extract the method element from XML doc
         method_el = tree.find(f"{method_cls.__name__}")
         if method_el is None:
             raise ValueError(
                 f"Response from {method_cls.interface} did not contain a "
                 f"<{method_cls.__name__}> element"
             )
 
         # Parse the method element with xsdata
         method = self._parser.parse(method_el, method_cls)
-        if not method.return_value:
+        if method.return_value is None or method.return_value == "":
             raise TypeError(
                 f"Response from {method_cls.interface}.{method_cls.__name__}"
-                f"did not contain a return value"
+                f" did not contain a return value"
             )
 
         return method.return_value
-
-    async def _get_connection(self) -> Connection:
-        """Get a connection to the ACI service, authenticating if necessary."""
-
-        # If we already have a connection, return it
-        if self._connection is not None and not self._connection[1].is_closing():
-            return self._connection
-
-        try:
-            # Otherwise, open a new connection
-            connection = await asyncio.wait_for(
-                asyncio.open_connection(
-                    self._host,
-                    self._port,
-                    ssl=self._ssl_context,
-                    limit=2**20,
-                ),
-                timeout=self._conn_timeout,
-            )
-            self._connection = connection
-            self._logger.info("Connected")
-
-            # Login if we have a username and password
-            await self._login()
-
-        except asyncio.TimeoutError as err:
-            raise ClientTimeoutError from err
-        except OSError as err:
-            raise ClientConnectionError from err
-
-        return connection
-
-    async def _login(self) -> None:
-        # Authenticate if necessary
-
-        if self._username is None or self._password is None:
-            return
-
-        params = Login.Params(user=self._username, password=self._password)
-        success = await self.request(Login, params)
-        if not success:
-            raise PermissionError("Authentication failed, bad username or password")
-
-        self._logger.info("Login successful")
```

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/helpers.py` & `aiovantage-0.2.2/src/aiovantage/config_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.2.2/src/aiovantage/config_client/xml_dataclass.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/methods/types.py` & `aiovantage-0.2.2/src/aiovantage/config_client/methods/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.2.2/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/methods/login/login.py` & `aiovantage-0.2.2/src/aiovantage/config_client/methods/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/config_client/objects/system_object.py` & `aiovantage-0.2.2/src/aiovantage/config_client/objects/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/base.py` & `aiovantage-0.2.2/src/aiovantage/controllers/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.2.2/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/blinds.py` & `aiovantage-0.2.2/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/buttons.py` & `aiovantage-0.2.2/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.2.2/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/gmem.py` & `aiovantage-0.2.2/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.2.2/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/loads.py` & `aiovantage-0.2.2/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.2.2/src/aiovantage/controllers/omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.2.2/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/src/aiovantage/controllers/tasks.py` & `aiovantage-0.2.2/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/LICENSE` & `aiovantage-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/README.md` & `aiovantage-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.1/pyproject.toml` & `aiovantage-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -56,20 +56,18 @@
 ]
 
 [tool.mypy]
 strict = true
 
 [tool.black]
 target-version = ["py38"]
-# line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py38"
-# line-length = 120
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
```

### Comparing `aiovantage-0.2.1/PKG-INFO` & `aiovantage-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
```

