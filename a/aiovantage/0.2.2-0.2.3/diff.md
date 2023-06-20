# Comparing `tmp/aiovantage-0.2.2.tar.gz` & `tmp/aiovantage-0.2.3.tar.gz`

## Comparing `aiovantage-0.2.2.tar` & `aiovantage-0.2.3.tar`

### file list

```diff
@@ -1,135 +1,136 @@
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiovantage-0.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aiovantage-0.2.2/TODO
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.github/dependabot.yml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/dump_system.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/monitor_all.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/control_load.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.2.2/examples/tasks/run_task.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/query.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/client.py
--rw-r--r--   0        0        0    10260 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/connection.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/errors.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/response.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/client.py
--rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/connection.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/errors.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/config_client/objects/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aiovantage-0.2.2/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aiovantage-0.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.2.2/LICENSE
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 aiovantage-0.2.2/README.md
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 aiovantage-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aiovantage-0.2.3/TODO
+-rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 aiovantage-0.2.3/clienttest.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/dump_system.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/monitor_all.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/tasks/run_task.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0    18922 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/client.py
+-rw-r--r--   0        0        0    10260 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/connection.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/errors.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/response.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/client.py
+-rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/connection.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/errors.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 aiovantage-0.2.3/README.md
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 aiovantage-0.2.3/PKG-INFO
```

### Comparing `aiovantage-0.2.2/CONTRIBUTING.md` & `aiovantage-0.2.3/CONTRIBUTING.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 
 ## Publishing
 
 Commit `src/aiovantage/__about.py` to source control.
 
 ```console
 $ git add src/aiovantage/__about__.py
-$ git commit -m "Preparing for release"
+$ git commit -m "Preparing release `hatch version`"
 ```
 
 Tag the release
 
 ```console
 $ git tag `hatch version`
 $ git push && git push --tags
 ```
 
 Publish the release to PyPi
 
 ```console
 $ hatch publish
-```
+```
```

### Comparing `aiovantage-0.2.2/examples/dump_system.py` & `aiovantage-0.2.3/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/monitor_all.py` & `aiovantage-0.2.3/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/areas/dump_areas.py` & `aiovantage-0.2.3/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.2.3/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/blinds/dump_blinds.py` & `aiovantage-0.2.3/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/blinds/monitor_blinds.py` & `aiovantage-0.2.3/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/buttons/dump_buttons.py` & `aiovantage-0.2.3/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/buttons/monitor_buttons.py` & `aiovantage-0.2.3/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/command_client/event_log.py` & `aiovantage-0.2.3/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/command_client/status_load.py` & `aiovantage-0.2.3/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/config_client/dump_objects.py` & `aiovantage-0.2.3/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/config_client/get_version.py` & `aiovantage-0.2.3/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.2.3/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.2.3/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/gmem/dump_gmem.py` & `aiovantage-0.2.3/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/gmem/monitor_gmem.py` & `aiovantage-0.2.3/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/gmem/set_gmem.py` & `aiovantage-0.2.3/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/load_groups/dump_load_groups.py` & `aiovantage-0.2.3/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/loads/control_load.py` & `aiovantage-0.2.3/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/loads/dump_loads.py` & `aiovantage-0.2.3/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/loads/monitor_loads.py` & `aiovantage-0.2.3/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/loads/poll_on_loads.py` & `aiovantage-0.2.3/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/loads/toggle_load.py` & `aiovantage-0.2.3/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.2.3/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.2.3/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.2.3/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.2.3/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/stations/dump_stations.py` & `aiovantage-0.2.3/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/tasks/dump_tasks.py` & `aiovantage-0.2.3/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/examples/tasks/run_task.py` & `aiovantage-0.2.3/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/__init__.py` & `aiovantage-0.2.3/src/aiovantage/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/query.py` & `aiovantage-0.2.3/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/README.md` & `aiovantage-0.2.3/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/__init__.py` & `aiovantage-0.2.3/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/client.py` & `aiovantage-0.2.3/src/aiovantage/command_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
             def filter_fn(event: Event) -> bool:
                 return event["tag"] == event_filter
 
         elif isinstance(event_filter, Iterable):
 
             def filter_fn(event: Event) -> bool:
-                return event["tag"] in event_filter  # type: ignore[operator]
+                return event["tag"] in event_filter
 
         else:
             filter_fn = event_filter
 
         # Add the subscription
         subscription: EventSubscription = (callback, filter_fn)
         self._subscriptions.append(subscription)
@@ -279,33 +279,30 @@
 
         # Support both a single object id and a list of object ids
         if isinstance(object_ids, int):
             object_ids = (object_ids,)
 
         # Filter recived status events by id
         def event_filter(event: Event) -> bool:
-            return (
-                event["tag"] == EventType.STATUS
-                and event["id"] in object_ids  # type: ignore[operator]
-            )
+            return event["tag"] == EventType.STATUS and event["id"] in object_ids
 
         # Add the subscription to the list
         remove_subscription = self.subscribe(callback, event_filter)
 
         # Ask the controller to start sending status events for these objects
         conn = await self.connection()
         for object_id in object_ids:
             self._subscribed_objects[object_id] += 1
             if self._subscribed_objects[object_id] == 1:
                 await conn.command("ADDSTATUS", object_id)
 
         # Return an unsubscribe callback
         async def unsubscribe() -> None:
             with suppress(ClientConnectionError):
-                for object_id in object_ids:  # type: ignore[union-attr]
+                for object_id in object_ids:
                     self._subscribed_objects[object_id] -= 1
                     if self._subscribed_objects[object_id] == 0:
                         await conn.command("DELSTATUS", object_id)
 
             remove_subscription()
 
         return unsubscribe
@@ -329,16 +326,21 @@
         # Support both a single log type and a list of log types
         if isinstance(log_types, str):
             log_types = (log_types,)
 
         # Add the subscription to the list
         remove_subscription = self.subscribe(callback, EventType.EVENT_LOG)
 
-        # Ask the controller to start sending event logs for these types
+        # Get the connection
         conn = await self.connection()
+
+        # Enable the event log
+        await conn.command("ELAGG ON")
+
+        # Ask the controller to start sending event logs for these types
         for log_type in log_types:
             self._subscribed_event_logs[log_type] += 1
             if self._subscribed_event_logs[log_type] == 1:
                 await conn.command("ELENABLE", log_type, "ON")
                 await conn.command("ELLOG", log_type, "ON")
 
         # Return an unsubscribe callback
```

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/connection.py` & `aiovantage-0.2.3/src/aiovantage/command_client/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/errors.py` & `aiovantage-0.2.3/src/aiovantage/command_client/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/events.py` & `aiovantage-0.2.3/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/response.py` & `aiovantage-0.2.3/src/aiovantage/command_client/response.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/utils.py` & `aiovantage-0.2.3/src/aiovantage/command_client/utils.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/README.md` & `aiovantage-0.2.3/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/__init__.py` & `aiovantage-0.2.3/src/aiovantage/config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/client.py` & `aiovantage-0.2.3/src/aiovantage/config_client/client.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/connection.py` & `aiovantage-0.2.3/src/aiovantage/config_client/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/helpers.py` & `aiovantage-0.2.3/src/aiovantage/config_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.2.3/src/aiovantage/config_client/xml_dataclass.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/methods/types.py` & `aiovantage-0.2.3/src/aiovantage/config_client/methods/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.2.3/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/methods/login/login.py` & `aiovantage-0.2.3/src/aiovantage/config_client/methods/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/config_client/objects/system_object.py` & `aiovantage-0.2.3/src/aiovantage/config_client/objects/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/base.py` & `aiovantage-0.2.3/src/aiovantage/controllers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 self._id_subscriptions[vid].append(subscription)
 
         # Return a function to unsubscribe
         def unsubscribe() -> None:
             if id_filter is None:
                 self._subscriptions.remove(subscription)
             else:
-                for vid in id_filter:  # type: ignore[union-attr]
+                for vid in id_filter:
                     if vid not in self._id_subscriptions:
                         continue
                     self._id_subscriptions[vid].remove(subscription)
 
         return unsubscribe
 
     def emit(
```

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.2.3/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/blinds.py` & `aiovantage-0.2.3/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/buttons.py` & `aiovantage-0.2.3/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.2.3/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/gmem.py` & `aiovantage-0.2.3/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.2.3/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/loads.py` & `aiovantage-0.2.3/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.2.3/src/aiovantage/controllers/omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.2.3/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/src/aiovantage/controllers/tasks.py` & `aiovantage-0.2.3/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/LICENSE` & `aiovantage-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/README.md` & `aiovantage-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.2/pyproject.toml` & `aiovantage-0.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 Source = "https://github.com/loopj/aiovantage"
 
 [tool.hatch.version]
 path = "src/aiovantage/__about__.py"
 
 [tool.hatch.envs.lint]
 dependencies = [
-  "black>=23.3.0",
-  "mypy>=1.3.0",
-  "ruff>=0.0.272",
+  "black==23.3.0",
+  "mypy==1.4.0",
+  "ruff==0.0.272",
 ]
 
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:.}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
```

### Comparing `aiovantage-0.2.2/PKG-INFO` & `aiovantage-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.2.2
+Version: 0.2.3
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
```

