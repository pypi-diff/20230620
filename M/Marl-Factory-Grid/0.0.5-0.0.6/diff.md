# Comparing `tmp/Marl-Factory-Grid-0.0.5.tar.gz` & `tmp/Marl-Factory-Grid-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Marl-Factory-Grid-0.0.5.tar", last modified: Mon Jun 19 14:33:05 2023, max compression
+gzip compressed data, was "Marl-Factory-Grid-0.0.6.tar", last modified: Tue Jun 20 08:27:49 2023, max compression
```

## Comparing `Marl-Factory-Grid-0.0.5.tar` & `Marl-Factory-Grid-0.0.6.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.937193 Marl-Factory-Grid-0.0.5/
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.917194 Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4116 2023-06-19 14:33:05.000000 Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4192 2023-06-19 14:33:05.000000 Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 14:33:05.000000 Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 14:33:05.000000 Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-19 14:33:05.000000 Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4116 2023-06-19 14:33:05.937193 Marl-Factory-Grid-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.917194 Marl-Factory-Grid-0.0.5/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.917194 Marl-Factory-Grid-0.0.5/algorithms/marl/
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8658 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/base_ac.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/iac.py
--rw-rw-rw-   0 root         (0) root         (0)     3145 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/mappo.py
--rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/networks.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/seac.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/marl/snac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.921193 Marl-Factory-Grid-0.0.5/algorithms/static/
--rw-rw-rw-   0 root         (0) root         (0)     5296 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/static/TSP_base_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/static/TSP_dirt_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/static/TSP_item_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/static/TSP_target_agent.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/static/random_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2679 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/algorithms/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.921193 Marl-Factory-Grid-0.0.5/environment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.921193 Marl-Factory-Grid-0.0.5/environment/assets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.921193 Marl-Factory-Grid-0.0.5/environment/assets/agent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/adversary.png
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/agent.png
--rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/agent_collision.png
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/idle.png
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/invalid.png
--rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/move.png
--rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/agent/valid.png
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/assets/wall.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.925193 Marl-Factory-Grid-0.0.5/environment/entity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2302 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/entity/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/entity/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/entity/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3330 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/entity/object.py
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/entity/util.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/entity/wall_floor.py
--rw-rw-rw-   0 root         (0) root         (0)     6881 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.925193 Marl-Factory-Grid-0.0.5/environment/groups/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/agents.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/env_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/global_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2940 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3884 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/groups/wall_n_floors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.925193 Marl-Factory-Grid-0.0.5/environment/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/logging/envmonitor.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/logging/recorder.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.925193 Marl-Factory-Grid-0.0.5/environment/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5146 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10740 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/level_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    12457 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/observation_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/render.py
--rw-rw-rw-   0 root         (0) root         (0)     5759 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/states.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/environment/utils/utility_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.925193 Marl-Factory-Grid-0.0.5/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.925193 Marl-Factory-Grid-0.0.5/modules/_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/_template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/_template/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/_template/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.929193 Marl-Factory-Grid-0.0.5/modules/batteries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/batteries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/batteries/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/batteries/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/batteries/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/batteries/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/batteries/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/batteries/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.929193 Marl-Factory-Grid-0.0.5/modules/clean_up/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/dirtpiles.png
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/rule_done_on_all_clean.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/rule_respawn.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/clean_up/rule_smear_on_move.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.929193 Marl-Factory-Grid-0.0.5/modules/destinations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/destinations.png
--rw-rw-rw-   0 root         (0) root         (0)     1735 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3650 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/destinations/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.933193 Marl-Factory-Grid-0.0.5/modules/doors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/door_closed.png
--rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/door_open.png
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/doors/rule_door_auto_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.933193 Marl-Factory-Grid-0.0.5/modules/items/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1621 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.933193 Marl-Factory-Grid-0.0.5/modules/items/assets/
--rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/assets/charge_pod.png
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/assets/dropofflocations.png
--rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/assets/items.png
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2014 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     3065 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/items/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.933193 Marl-Factory-Grid-0.0.5/modules/levels/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/levels/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/levels/large.txt
--rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/levels/large_qquad.txt
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/levels/rooms.txt
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/levels/shelves.txt
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/levels/simple.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.933193 Marl-Factory-Grid-0.0.5/modules/machines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/machines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/machines/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/machines/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/machines/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/machines/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/modules/machines/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.933193 Marl-Factory-Grid-0.0.5/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8628 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/plotting/compare_runs.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/plotting/plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.933193 Marl-Factory-Grid-0.0.5/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/quickstart/all_test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/quickstart/default_config.yaml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 14:33:05.937193 Marl-Factory-Grid-0.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 14:33:05.937193 Marl-Factory-Grid-0.0.5/studies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23919 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/e_1.py
--rw-rw-rw-   0 root         (0) root         (0)    10156 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/e_1_mix.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/normalization_study.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/playground_file.py
--rw-rw-rw-   0 root         (0) root         (0)    12396 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/single_run_with_export.py
--rw-rw-rw-   0 root         (0) root         (0)     7417 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/test.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-19 14:32:52.000000 Marl-Factory-Grid-0.0.5/studies/viz_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.548525 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.548525 Marl-Factory-Grid-0.0.6/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/algorithms/marl/
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8658 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/base_ac.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/iac.py
+-rw-rw-rw-   0 root         (0) root         (0)     3145 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/mappo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/networks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/seac.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/snac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/algorithms/static/
+-rw-rw-rw-   0 root         (0) root         (0)     5296 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_base_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_dirt_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_item_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_target_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/random_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/assets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/assets/agent/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/adversary.png
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/agent.png
+-rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/agent_collision.png
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/idle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/invalid.png
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/move.png
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/valid.png
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/wall.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/entity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3330 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/wall_floor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6881 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/groups/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/agents.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/env_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/global_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2940 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3884 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/wall_n_floors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/logging/envmonitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5475 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/logging/recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/environment/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10740 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/level_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    12457 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/observation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/render.py
+-rw-rw-rw-   0 root         (0) root         (0)     5759 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     3565 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/states.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/utility_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/_template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/_template/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/_template/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/batteries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/clean_up/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/dirtpiles.png
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rule_done_on_all_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rule_respawn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rule_smear_on_move.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/destinations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/destinations.png
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3650 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/doors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/door_closed.png
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/door_open.png
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/rule_door_auto_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/items/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1621 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/items/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/assets/charge_pod.png
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/assets/dropofflocations.png
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/assets/items.png
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2014 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/levels/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/large.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/large_qquad.txt
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/rooms.txt
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/shelves.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/simple.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/modules/machines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8628 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/plotting/compare_runs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/plotting/plotting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/quickstart/all_test_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/quickstart/default_config.yaml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/studies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23919 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/e_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    10156 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/e_1_mix.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/normalization_study.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/playground_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    12396 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/single_run_with_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     7417 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/viz_policy.py
```

### Comparing `Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/PKG-INFO` & `Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Factory-Grid-0.0.5/Marl_Factory_Grid.egg-info/SOURCES.txt` & `Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/PKG-INFO` & `Marl-Factory-Grid-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Factory-Grid-0.0.5/README.md` & `Marl-Factory-Grid-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/base_ac.py` & `Marl-Factory-Grid-0.0.6/algorithms/marl/base_ac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/example_config.yaml` & `Marl-Factory-Grid-0.0.6/algorithms/marl/example_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/iac.py` & `Marl-Factory-Grid-0.0.6/algorithms/marl/iac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/mappo.py` & `Marl-Factory-Grid-0.0.6/algorithms/marl/mappo.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/memory.py` & `Marl-Factory-Grid-0.0.6/algorithms/marl/memory.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/networks.py` & `Marl-Factory-Grid-0.0.6/algorithms/marl/networks.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/seac.py` & `Marl-Factory-Grid-0.0.6/algorithms/marl/seac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/marl/snac.py` & `Marl-Factory-Grid-0.0.6/algorithms/marl/snac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/static/TSP_base_agent.py` & `Marl-Factory-Grid-0.0.6/algorithms/static/TSP_base_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/static/TSP_dirt_agent.py` & `Marl-Factory-Grid-0.0.6/algorithms/static/TSP_dirt_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/static/TSP_item_agent.py` & `Marl-Factory-Grid-0.0.6/algorithms/static/TSP_item_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/static/TSP_target_agent.py` & `Marl-Factory-Grid-0.0.6/algorithms/static/TSP_target_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/algorithms/utils.py` & `Marl-Factory-Grid-0.0.6/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/actions.py` & `Marl-Factory-Grid-0.0.6/environment/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/agent/adversary.png` & `Marl-Factory-Grid-0.0.6/environment/assets/agent/adversary.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/agent/agent.png` & `Marl-Factory-Grid-0.0.6/environment/assets/agent/agent.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/agent/agent_collision.png` & `Marl-Factory-Grid-0.0.6/environment/assets/agent/agent_collision.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/agent/idle.png` & `Marl-Factory-Grid-0.0.6/environment/assets/agent/idle.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/agent/invalid.png` & `Marl-Factory-Grid-0.0.6/environment/assets/agent/invalid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/agent/move.png` & `Marl-Factory-Grid-0.0.6/environment/assets/agent/move.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/agent/valid.png` & `Marl-Factory-Grid-0.0.6/environment/assets/agent/valid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/assets/wall.png` & `Marl-Factory-Grid-0.0.6/environment/assets/wall.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/constants.py` & `Marl-Factory-Grid-0.0.6/environment/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/entity/agent.py` & `Marl-Factory-Grid-0.0.6/environment/entity/agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/entity/entity.py` & `Marl-Factory-Grid-0.0.6/environment/entity/entity.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/entity/object.py` & `Marl-Factory-Grid-0.0.6/environment/entity/object.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/entity/util.py` & `Marl-Factory-Grid-0.0.6/environment/entity/util.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/entity/wall_floor.py` & `Marl-Factory-Grid-0.0.6/environment/entity/wall_floor.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/factory.py` & `Marl-Factory-Grid-0.0.6/environment/factory.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/groups/agents.py` & `Marl-Factory-Grid-0.0.6/environment/groups/agents.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/groups/env_objects.py` & `Marl-Factory-Grid-0.0.6/environment/groups/env_objects.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/groups/global_entities.py` & `Marl-Factory-Grid-0.0.6/environment/groups/global_entities.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/groups/mixins.py` & `Marl-Factory-Grid-0.0.6/environment/groups/mixins.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/groups/objects.py` & `Marl-Factory-Grid-0.0.6/environment/groups/objects.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/groups/utils.py` & `Marl-Factory-Grid-0.0.6/environment/groups/utils.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/groups/wall_n_floors.py` & `Marl-Factory-Grid-0.0.6/environment/groups/wall_n_floors.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/logging/envmonitor.py` & `Marl-Factory-Grid-0.0.6/environment/logging/envmonitor.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/logging/recorder.py` & `Marl-Factory-Grid-0.0.6/environment/logging/recorder.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/rules.py` & `Marl-Factory-Grid-0.0.6/environment/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/config_parser.py` & `Marl-Factory-Grid-0.0.6/environment/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/helpers.py` & `Marl-Factory-Grid-0.0.6/environment/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/level_parser.py` & `Marl-Factory-Grid-0.0.6/environment/utils/level_parser.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/observation_builder.py` & `Marl-Factory-Grid-0.0.6/environment/utils/observation_builder.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/renderer.py` & `Marl-Factory-Grid-0.0.6/environment/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/results.py` & `Marl-Factory-Grid-0.0.6/environment/utils/results.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/states.py` & `Marl-Factory-Grid-0.0.6/environment/utils/states.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/environment/utils/utility_classes.py` & `Marl-Factory-Grid-0.0.6/environment/utils/utility_classes.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/_template/rules.py` & `Marl-Factory-Grid-0.0.6/modules/_template/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/batteries/actions.py` & `Marl-Factory-Grid-0.0.6/modules/batteries/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/batteries/constants.py` & `Marl-Factory-Grid-0.0.6/modules/batteries/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/batteries/entitites.py` & `Marl-Factory-Grid-0.0.6/modules/batteries/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/batteries/groups.py` & `Marl-Factory-Grid-0.0.6/modules/batteries/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/batteries/rules.py` & `Marl-Factory-Grid-0.0.6/modules/batteries/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/clean_up/actions.py` & `Marl-Factory-Grid-0.0.6/modules/clean_up/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/clean_up/dirtpiles.png` & `Marl-Factory-Grid-0.0.6/modules/clean_up/dirtpiles.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/clean_up/entitites.py` & `Marl-Factory-Grid-0.0.6/modules/clean_up/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/clean_up/groups.py` & `Marl-Factory-Grid-0.0.6/modules/clean_up/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/clean_up/rule_done_on_all_clean.py` & `Marl-Factory-Grid-0.0.6/modules/clean_up/rule_done_on_all_clean.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/clean_up/rule_respawn.py` & `Marl-Factory-Grid-0.0.6/modules/clean_up/rule_respawn.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/clean_up/rule_smear_on_move.py` & `Marl-Factory-Grid-0.0.6/modules/clean_up/rule_smear_on_move.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/destinations/actions.py` & `Marl-Factory-Grid-0.0.6/modules/destinations/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/destinations/destinations.png` & `Marl-Factory-Grid-0.0.6/modules/destinations/destinations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/destinations/entitites.py` & `Marl-Factory-Grid-0.0.6/modules/destinations/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/destinations/groups.py` & `Marl-Factory-Grid-0.0.6/modules/destinations/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/destinations/rules.py` & `Marl-Factory-Grid-0.0.6/modules/destinations/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/doors/actions.py` & `Marl-Factory-Grid-0.0.6/modules/doors/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/doors/constants.py` & `Marl-Factory-Grid-0.0.6/modules/doors/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/doors/door_closed.png` & `Marl-Factory-Grid-0.0.6/modules/doors/door_closed.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/doors/door_open.png` & `Marl-Factory-Grid-0.0.6/modules/doors/door_open.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/doors/entitites.py` & `Marl-Factory-Grid-0.0.6/modules/doors/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/doors/groups.py` & `Marl-Factory-Grid-0.0.6/modules/doors/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/doors/rule_door_auto_close.py` & `Marl-Factory-Grid-0.0.6/modules/doors/rule_door_auto_close.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/items/actions.py` & `Marl-Factory-Grid-0.0.6/modules/items/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/items/assets/charge_pod.png` & `Marl-Factory-Grid-0.0.6/modules/items/assets/charge_pod.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/items/assets/dropofflocations.png` & `Marl-Factory-Grid-0.0.6/modules/items/assets/dropofflocations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/items/assets/items.png` & `Marl-Factory-Grid-0.0.6/modules/items/assets/items.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/items/entitites.py` & `Marl-Factory-Grid-0.0.6/modules/items/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/items/groups.py` & `Marl-Factory-Grid-0.0.6/modules/items/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/items/rules.py` & `Marl-Factory-Grid-0.0.6/modules/items/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/machines/entitites.py` & `Marl-Factory-Grid-0.0.6/modules/machines/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/modules/machines/rules.py` & `Marl-Factory-Grid-0.0.6/modules/machines/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/plotting/compare_runs.py` & `Marl-Factory-Grid-0.0.6/plotting/compare_runs.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/plotting/plotting.py` & `Marl-Factory-Grid-0.0.6/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/quickstart/all_test_config.yaml` & `Marl-Factory-Grid-0.0.6/quickstart/all_test_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/quickstart/default_config.yaml` & `Marl-Factory-Grid-0.0.6/quickstart/default_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/setup.py` & `Marl-Factory-Grid-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='Marl-Factory-Grid',
-      version='0.0.5',
+      version='0.0.6',
       description='A framework to research MARL agents in various setings.',
       author='Steffen Illium',
       author_email='steffen.illium@ifi.lmu.de',
       url='https://github.com/illiumst/marl-factory-grid/import',
       license='MIT',
       keywords=[
             'artificial intelligence',
             'pytorch',
             'multiagent reinforcement learning',
             'simulation',
             'emergence',
             'gymnasium',
-            'environment',
-
+            'environment'
       ],
       classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
             'Topic :: Scientific/Engineering :: Artificial Intelligence',
             'License :: OSI Approved :: MIT License',
             'Programming Language :: Python :: 3.11',
```

### Comparing `Marl-Factory-Grid-0.0.5/studies/e_1.py` & `Marl-Factory-Grid-0.0.6/studies/e_1.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/studies/e_1_mix.py` & `Marl-Factory-Grid-0.0.6/studies/e_1_mix.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/studies/normalization_study.py` & `Marl-Factory-Grid-0.0.6/studies/normalization_study.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/studies/playground_file.py` & `Marl-Factory-Grid-0.0.6/studies/playground_file.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/studies/single_run_with_export.py` & `Marl-Factory-Grid-0.0.6/studies/single_run_with_export.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/studies/test.py` & `Marl-Factory-Grid-0.0.6/studies/test.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.5/studies/viz_policy.py` & `Marl-Factory-Grid-0.0.6/studies/viz_policy.py`

 * *Files identical despite different names*

