# Comparing `tmp/skelebot-1.9.0.tar.gz` & `tmp/skelebot-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skelebot-1.9.0.tar", last modified: Fri Nov 15 21:50:16 2019, max compression
+gzip compressed data, was "dist/skelebot-1.9.1.tar", last modified: Thu Nov 21 15:20:58 2019, max compression
```

## Comparing `skelebot-1.9.0.tar` & `skelebot-1.9.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:16.000000 skelebot-1.9.0/
--rw-r--r--   0 seanshookman   (502) staff       (20)      205 2019-11-15 21:50:16.000000 skelebot-1.9.0/PKG-INFO
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:16.000000 skelebot-1.9.0/test/
--rw-r--r--   0 seanshookman   (502) staff       (20)     1210 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_objects_arg_validate.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1280 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_systems_generators_dockerignore.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2050 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_components_prime.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     3688 2019-10-17 19:53:34.000000 skelebot-1.9.0/test/test_skelebot_main.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1752 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_objects_job_validate.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1352 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_components_dexec.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1333 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_components_plugin.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1752 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_components_kerberos.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     5121 2019-11-15 20:14:46.000000 skelebot-1.9.0/test/test_systems_execution_executor.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     3293 2019-11-06 21:34:43.000000 skelebot-1.9.0/test/test_systems_execution_commandBuilder.py
--rw-r--r--   0 seanshookman   (502) staff       (20)    13925 2019-11-07 15:28:52.000000 skelebot-1.9.0/test/test_systems_generators_dockerfile.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2018 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_components_registry.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     8094 2019-10-16 19:44:33.000000 skelebot-1.9.0/test/test_systems_execution_docker.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1427 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_objects_param_validate.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2599 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_components_jupyter.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     7750 2019-11-11 22:38:44.000000 skelebot-1.9.0/test/test_systems_generators_yaml.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1288 2019-10-02 16:47:47.000000 skelebot-1.9.0/test/test_systems_generators_readme.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     9421 2019-11-15 21:14:13.000000 skelebot-1.9.0/test/test_components_artifactory.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     6182 2019-11-07 15:28:52.000000 skelebot-1.9.0/test/test_systems_scaffolding_scaffolder.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2382 2019-11-07 15:28:52.000000 skelebot-1.9.0/test/test_objects_config_validate.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     3478 2019-11-11 17:13:44.000000 skelebot-1.9.0/test/test_systems_parsing_skeleParser.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2606 2019-11-06 22:10:00.000000 skelebot-1.9.0/test/test_components_bump.py
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/
--rw-r--r--   0 seanshookman   (502) staff       (20)     1400 2019-11-15 20:14:46.000000 skelebot-1.9.0/skelebot/skelebot.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      125 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/__init__.py
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/objects/
--rw-r--r--   0 seanshookman   (502) staff       (20)     1699 2019-08-14 20:57:52.000000 skelebot-1.9.0/skelebot/objects/skeleYaml.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1424 2019-11-15 21:14:13.000000 skelebot-1.9.0/skelebot/objects/semver.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     6983 2019-11-07 15:28:52.000000 skelebot-1.9.0/skelebot/objects/config.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2374 2019-08-14 20:57:52.000000 skelebot-1.9.0/skelebot/objects/job.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      119 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/objects/__init__.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1131 2019-08-14 20:57:52.000000 skelebot-1.9.0/skelebot/objects/param.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      763 2019-08-14 20:57:52.000000 skelebot-1.9.0/skelebot/objects/arg.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2056 2019-08-23 18:13:23.000000 skelebot-1.9.0/skelebot/objects/component.py
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/components/
--rw-r--r--   0 seanshookman   (502) staff       (20)     1354 2019-09-05 14:37:39.000000 skelebot-1.9.0/skelebot/components/prime.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     3226 2019-11-11 22:38:44.000000 skelebot-1.9.0/skelebot/components/componentFactory.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1884 2019-10-02 16:25:23.000000 skelebot-1.9.0/skelebot/components/registry.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     8496 2019-11-15 21:14:13.000000 skelebot-1.9.0/skelebot/components/artifactory.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      171 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/components/__init__.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1420 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/components/dexec.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1752 2019-11-06 22:10:15.000000 skelebot-1.9.0/skelebot/components/bump.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1755 2019-08-14 20:57:52.000000 skelebot-1.9.0/skelebot/components/kerberos.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1679 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/components/plugin.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2097 2019-10-22 15:41:10.000000 skelebot-1.9.0/skelebot/components/jupyter.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     1241 2019-11-11 22:38:44.000000 skelebot-1.9.0/skelebot/common.py
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/systems/
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/systems/scaffolding/
--rw-r--r--   0 seanshookman   (502) staff       (20)      119 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/scaffolding/__init__.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2792 2019-08-28 18:42:04.000000 skelebot-1.9.0/skelebot/systems/scaffolding/scaffolder.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      536 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/scaffolding/prompt.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      154 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/__init__.py
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/systems/execution/
--rw-r--r--   0 seanshookman   (502) staff       (20)     2301 2019-11-06 21:58:19.000000 skelebot-1.9.0/skelebot/systems/execution/commandBuilder.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      123 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/execution/__init__.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     3640 2019-11-07 15:45:17.000000 skelebot-1.9.0/skelebot/systems/execution/docker.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2283 2019-11-15 20:14:46.000000 skelebot-1.9.0/skelebot/systems/execution/executor.py
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/systems/generators/
--rw-r--r--   0 seanshookman   (502) staff       (20)      869 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/generators/readme.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      815 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/generators/dockerignore.py
--rw-r--r--   0 seanshookman   (502) staff       (20)      137 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/generators/__init__.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     2327 2019-10-16 19:44:33.000000 skelebot-1.9.0/skelebot/systems/generators/yaml.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     6905 2019-11-07 15:28:52.000000 skelebot-1.9.0/skelebot/systems/generators/dockerfile.py
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot/systems/parsing/
--rw-r--r--   0 seanshookman   (502) staff       (20)       91 2019-08-06 20:25:26.000000 skelebot-1.9.0/skelebot/systems/parsing/__init__.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     5290 2019-11-15 20:14:46.000000 skelebot-1.9.0/skelebot/systems/parsing/skeleParser.py
--rw-r--r--   0 seanshookman   (502) staff       (20)     5453 2019-11-15 20:14:46.000000 skelebot-1.9.0/README.md
--rw-r--r--   0 seanshookman   (502) staff       (20)      638 2019-10-16 19:44:33.000000 skelebot-1.9.0/setup.py
--rw-r--r--   0 seanshookman   (502) staff       (20)       63 2019-11-15 21:50:16.000000 skelebot-1.9.0/setup.cfg
-drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot.egg-info/
--rw-r--r--   0 seanshookman   (502) staff       (20)      205 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot.egg-info/PKG-INFO
--rw-r--r--   0 seanshookman   (502) staff       (20)        1 2019-07-30 20:57:47.000000 skelebot-1.9.0/skelebot.egg-info/not-zip-safe
--rw-r--r--   0 seanshookman   (502) staff       (20)     2233 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot.egg-info/SOURCES.txt
--rw-r--r--   0 seanshookman   (502) staff       (20)       44 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot.egg-info/entry_points.txt
--rw-r--r--   0 seanshookman   (502) staff       (20)      111 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot.egg-info/requires.txt
--rw-r--r--   0 seanshookman   (502) staff       (20)        9 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot.egg-info/top_level.txt
--rw-r--r--   0 seanshookman   (502) staff       (20)        1 2019-11-15 21:50:15.000000 skelebot-1.9.0/skelebot.egg-info/dependency_links.txt
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:58.000000 skelebot-1.9.1/
+-rw-r--r--   0 seanshookman   (502) staff       (20)      205 2019-11-21 15:20:58.000000 skelebot-1.9.1/PKG-INFO
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:58.000000 skelebot-1.9.1/test/
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1210 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_objects_arg_validate.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1280 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_systems_generators_dockerignore.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2050 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_components_prime.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     3688 2019-10-17 19:53:34.000000 skelebot-1.9.1/test/test_skelebot_main.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1752 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_objects_job_validate.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1352 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_components_dexec.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1333 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_components_plugin.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1752 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_components_kerberos.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     5121 2019-11-15 20:14:46.000000 skelebot-1.9.1/test/test_systems_execution_executor.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     3293 2019-11-06 21:34:43.000000 skelebot-1.9.1/test/test_systems_execution_commandBuilder.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)    13925 2019-11-07 15:28:52.000000 skelebot-1.9.1/test/test_systems_generators_dockerfile.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2664 2019-11-20 20:04:52.000000 skelebot-1.9.1/test/test_components_registry.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     9417 2019-11-20 20:04:52.000000 skelebot-1.9.1/test/test_systems_execution_docker.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1427 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_objects_param_validate.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2599 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_components_jupyter.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     7750 2019-11-11 22:38:44.000000 skelebot-1.9.1/test/test_systems_generators_yaml.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1288 2019-10-02 16:47:47.000000 skelebot-1.9.1/test/test_systems_generators_readme.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     9421 2019-11-15 21:14:13.000000 skelebot-1.9.1/test/test_components_artifactory.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     6182 2019-11-07 15:28:52.000000 skelebot-1.9.1/test/test_systems_scaffolding_scaffolder.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2382 2019-11-07 15:28:52.000000 skelebot-1.9.1/test/test_objects_config_validate.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     3478 2019-11-11 17:13:44.000000 skelebot-1.9.1/test/test_systems_parsing_skeleParser.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2606 2019-11-06 22:10:00.000000 skelebot-1.9.1/test/test_components_bump.py
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1400 2019-11-15 20:14:46.000000 skelebot-1.9.1/skelebot/skelebot.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      125 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/__init__.py
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/objects/
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1699 2019-08-14 20:57:52.000000 skelebot-1.9.1/skelebot/objects/skeleYaml.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1424 2019-11-15 21:14:13.000000 skelebot-1.9.1/skelebot/objects/semver.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     6983 2019-11-07 15:28:52.000000 skelebot-1.9.1/skelebot/objects/config.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2374 2019-08-14 20:57:52.000000 skelebot-1.9.1/skelebot/objects/job.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      119 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/objects/__init__.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1131 2019-08-14 20:57:52.000000 skelebot-1.9.1/skelebot/objects/param.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      763 2019-08-14 20:57:52.000000 skelebot-1.9.1/skelebot/objects/arg.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2056 2019-08-23 18:13:23.000000 skelebot-1.9.1/skelebot/objects/component.py
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/components/
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1354 2019-11-19 22:16:35.000000 skelebot-1.9.1/skelebot/components/prime.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     3226 2019-11-11 22:38:44.000000 skelebot-1.9.1/skelebot/components/componentFactory.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2010 2019-11-20 20:04:52.000000 skelebot-1.9.1/skelebot/components/registry.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     8496 2019-11-15 21:14:13.000000 skelebot-1.9.1/skelebot/components/artifactory.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      171 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/components/__init__.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1420 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/components/dexec.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1752 2019-11-06 22:10:15.000000 skelebot-1.9.1/skelebot/components/bump.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1755 2019-08-14 20:57:52.000000 skelebot-1.9.1/skelebot/components/kerberos.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1679 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/components/plugin.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2097 2019-10-22 15:41:10.000000 skelebot-1.9.1/skelebot/components/jupyter.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     1241 2019-11-11 22:38:44.000000 skelebot-1.9.1/skelebot/common.py
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/systems/
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/systems/scaffolding/
+-rw-r--r--   0 seanshookman   (502) staff       (20)      119 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/scaffolding/__init__.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2792 2019-08-28 18:42:04.000000 skelebot-1.9.1/skelebot/systems/scaffolding/scaffolder.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      536 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/scaffolding/prompt.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      154 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/__init__.py
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/systems/execution/
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2301 2019-11-06 21:58:19.000000 skelebot-1.9.1/skelebot/systems/execution/commandBuilder.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      123 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/execution/__init__.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     3521 2019-11-20 20:04:52.000000 skelebot-1.9.1/skelebot/systems/execution/docker.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2283 2019-11-15 20:14:46.000000 skelebot-1.9.1/skelebot/systems/execution/executor.py
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/systems/generators/
+-rw-r--r--   0 seanshookman   (502) staff       (20)      869 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/generators/readme.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      815 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/generators/dockerignore.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)      137 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/generators/__init__.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2327 2019-10-16 19:44:33.000000 skelebot-1.9.1/skelebot/systems/generators/yaml.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     6905 2019-11-07 15:28:52.000000 skelebot-1.9.1/skelebot/systems/generators/dockerfile.py
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot/systems/parsing/
+-rw-r--r--   0 seanshookman   (502) staff       (20)       91 2019-08-06 20:25:26.000000 skelebot-1.9.1/skelebot/systems/parsing/__init__.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     5290 2019-11-18 15:54:08.000000 skelebot-1.9.1/skelebot/systems/parsing/skeleParser.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)     5453 2019-11-15 20:14:46.000000 skelebot-1.9.1/README.md
+-rw-r--r--   0 seanshookman   (502) staff       (20)      638 2019-10-16 19:44:33.000000 skelebot-1.9.1/setup.py
+-rw-r--r--   0 seanshookman   (502) staff       (20)       63 2019-11-21 15:20:58.000000 skelebot-1.9.1/setup.cfg
+drwxr-xr-x   0 seanshookman   (502) staff       (20)        0 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot.egg-info/
+-rw-r--r--   0 seanshookman   (502) staff       (20)      205 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot.egg-info/PKG-INFO
+-rw-r--r--   0 seanshookman   (502) staff       (20)        1 2019-07-30 20:57:47.000000 skelebot-1.9.1/skelebot.egg-info/not-zip-safe
+-rw-r--r--   0 seanshookman   (502) staff       (20)     2233 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot.egg-info/SOURCES.txt
+-rw-r--r--   0 seanshookman   (502) staff       (20)       44 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot.egg-info/entry_points.txt
+-rw-r--r--   0 seanshookman   (502) staff       (20)      111 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot.egg-info/requires.txt
+-rw-r--r--   0 seanshookman   (502) staff       (20)        9 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot.egg-info/top_level.txt
+-rw-r--r--   0 seanshookman   (502) staff       (20)        1 2019-11-21 15:20:57.000000 skelebot-1.9.1/skelebot.egg-info/dependency_links.txt
```

### Comparing `skelebot-1.9.0/test/test_objects_arg_validate.py` & `skelebot-1.9.1/test/test_objects_arg_validate.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_generators_dockerignore.py` & `skelebot-1.9.1/test/test_systems_generators_dockerignore.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_prime.py` & `skelebot-1.9.1/test/test_components_prime.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_skelebot_main.py` & `skelebot-1.9.1/test/test_skelebot_main.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_objects_job_validate.py` & `skelebot-1.9.1/test/test_objects_job_validate.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_dexec.py` & `skelebot-1.9.1/test/test_components_dexec.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_plugin.py` & `skelebot-1.9.1/test/test_components_plugin.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_kerberos.py` & `skelebot-1.9.1/test/test_components_kerberos.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_execution_executor.py` & `skelebot-1.9.1/test/test_systems_execution_executor.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_execution_commandBuilder.py` & `skelebot-1.9.1/test/test_systems_execution_commandBuilder.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_generators_dockerfile.py` & `skelebot-1.9.1/test/test_systems_generators_dockerfile.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_registry.py` & `skelebot-1.9.1/test/test_components_registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,22 +25,36 @@
         self.assertNotEqual(subparsers.choices["publish"], None)
 
     @mock.patch('skelebot.components.registry.docker')
     def test_execute(self, mock_docker):
         mock_docker.build.return_value = 0
 
         config = sb.objects.config.Config(language="R")
-        args = argparse.Namespace()
+        args = argparse.Namespace(tags=None)
 
         registry = sb.components.registry.Registry(host="docker.io", port=88, user="skelebot")
         registry.execute(config, args)
 
         mock_docker.login.assert_called_with("docker.io")
         mock_docker.build.assert_called_with(config)
-        mock_docker.push.assert_called_with(config, "docker.io", 88, "skelebot")
+        mock_docker.push.assert_called_with(config, "docker.io", 88, "skelebot", tags=None)
+
+    @mock.patch('skelebot.components.registry.docker')
+    def test_execute_tags(self, mock_docker):
+        mock_docker.build.return_value = 0
+
+        config = sb.objects.config.Config(language="R")
+        args = argparse.Namespace(tags=["test", "dev", "stage"])
+
+        registry = sb.components.registry.Registry(host="docker.io", port=88, user="skelebot")
+        registry.execute(config, args)
+
+        mock_docker.login.assert_called_with("docker.io")
+        mock_docker.build.assert_called_with(config)
+        mock_docker.push.assert_called_with(config, "docker.io", 88, "skelebot", tags=['test', 'dev', 'stage'])
 
     def test_validate_valid(self):
         try:
             sb.components.registry.Registry.validate(self.registry)
         except:
             self.fail("Validation Raised Exception Unexpectedly")
```

### Comparing `skelebot-1.9.0/test/test_systems_execution_docker.py` & `skelebot-1.9.1/test/test_systems_execution_docker.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,27 +63,52 @@
         mock_system.assert_any_call("docker tag test docker.io:8888/skelebot/test:latest")
         mock_system.assert_any_call("docker push docker.io:8888/skelebot/test:6.6.6")
         mock_system.assert_any_call("docker push docker.io:8888/skelebot/test:latest")
 
     @mock.patch('os.path.expanduser')
     @mock.patch('os.system')
     @mock.patch('os.getcwd')
+    def test_push_tags(self, mock_getcwd, mock_system, mock_expanduser):
+        host = "docker.io"
+        port = 8888
+        user = "skelebot"
+        folderPath = "{path}/test/files".format(path=self.path)
+
+        mock_expanduser.return_value = "{path}/test/plugins".format(path=self.path)
+        mock_getcwd.return_value = folderPath
+        mock_system.return_value = 0
+
+        config = sb.systems.generators.yaml.loadConfig()
+        sb.systems.execution.docker.push(config, host, port, user, tags=["DEV", "STG"])
+
+        mock_system.assert_any_call("docker tag test docker.io:8888/skelebot/test:6.6.6")
+        mock_system.assert_any_call("docker push docker.io:8888/skelebot/test:6.6.6")
+        mock_system.assert_any_call("docker tag test docker.io:8888/skelebot/test:latest")
+        mock_system.assert_any_call("docker push docker.io:8888/skelebot/test:latest")
+        mock_system.assert_any_call("docker tag test docker.io:8888/skelebot/test:DEV")
+        mock_system.assert_any_call("docker push docker.io:8888/skelebot/test:DEV")
+        mock_system.assert_any_call("docker tag test docker.io:8888/skelebot/test:STG")
+        mock_system.assert_any_call("docker push docker.io:8888/skelebot/test:STG")
+
+    @mock.patch('os.path.expanduser')
+    @mock.patch('os.system')
+    @mock.patch('os.getcwd')
     def test_push_error(self, mock_getcwd, mock_system, mock_expanduser):
         host = "docker.io"
         port = 8888
         user = "skelebot"
         folderPath = "{path}/test/files".format(path=self.path)
 
         mock_expanduser.return_value = "{path}/test/plugins".format(path=self.path)
         mock_getcwd.return_value = folderPath
         mock_system.return_value = 1
 
         config = sb.systems.generators.yaml.loadConfig()
 
-        with self.assertRaisesRegex(Exception, "Docker Push Failed"):
+        with self.assertRaisesRegex(Exception, "Docker Command Failed"):
             sb.systems.execution.docker.push(config, host, port, user)
 
     @mock.patch('os.path.expanduser')
     @mock.patch('os.remove')
     @mock.patch('os.system')
     @mock.patch('os.getcwd')
     def test_build_ephemeral(self, mock_getcwd, mock_system, mock_remove, mock_expanduser):
```

### Comparing `skelebot-1.9.0/test/test_objects_param_validate.py` & `skelebot-1.9.1/test/test_objects_param_validate.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_jupyter.py` & `skelebot-1.9.1/test/test_components_jupyter.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_generators_yaml.py` & `skelebot-1.9.1/test/test_systems_generators_yaml.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_generators_readme.py` & `skelebot-1.9.1/test/test_systems_generators_readme.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_artifactory.py` & `skelebot-1.9.1/test/test_components_artifactory.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_scaffolding_scaffolder.py` & `skelebot-1.9.1/test/test_systems_scaffolding_scaffolder.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_objects_config_validate.py` & `skelebot-1.9.1/test/test_objects_config_validate.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_systems_parsing_skeleParser.py` & `skelebot-1.9.1/test/test_systems_parsing_skeleParser.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/test/test_components_bump.py` & `skelebot-1.9.1/test/test_components_bump.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/skelebot.py` & `skelebot-1.9.1/skelebot/skelebot.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/objects/skeleYaml.py` & `skelebot-1.9.1/skelebot/objects/skeleYaml.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/objects/semver.py` & `skelebot-1.9.1/skelebot/objects/semver.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/objects/config.py` & `skelebot-1.9.1/skelebot/objects/config.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/objects/job.py` & `skelebot-1.9.1/skelebot/objects/job.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/objects/param.py` & `skelebot-1.9.1/skelebot/objects/param.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/objects/arg.py` & `skelebot-1.9.1/skelebot/objects/arg.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/objects/component.py` & `skelebot-1.9.1/skelebot/objects/component.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/prime.py` & `skelebot-1.9.1/skelebot/components/prime.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/componentFactory.py` & `skelebot-1.9.1/skelebot/components/componentFactory.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/registry.py` & `skelebot-1.9.1/skelebot/components/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,22 +37,23 @@
         SkeleParser Hook
 
         Adds a parser for the publish command to allow the user to login and push the project's
         Docker image to the defined registry, or Docker Hub, if one is not defined.
         """
 
         helpMessage = "Publish your versioned Docker Image to the registry"
-        subparsers.add_parser("publish", help=helpMessage)
+        registryParser = subparsers.add_parser("publish", help=helpMessage)
+        registryParser.add_argument("-t", "--tags", nargs='*', help="Additional image tags")
 
         return subparsers
 
     def execute(self, config, args):
         """
         Execution Hook
 
         Executes when the publish command is provided and prompts for username and password before
         building the project's Docker Image and pushing it to the defined registry.
         """
 
         docker.login(self.host)
         docker.build(config)
-        docker.push(config, self.host, self.port, self.user)
+        docker.push(config, self.host, self.port, self.user, tags=args.tags)
```

### Comparing `skelebot-1.9.0/skelebot/components/artifactory.py` & `skelebot-1.9.1/skelebot/components/artifactory.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/dexec.py` & `skelebot-1.9.1/skelebot/components/dexec.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/bump.py` & `skelebot-1.9.1/skelebot/components/bump.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/kerberos.py` & `skelebot-1.9.1/skelebot/components/kerberos.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/plugin.py` & `skelebot-1.9.1/skelebot/components/plugin.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/components/jupyter.py` & `skelebot-1.9.1/skelebot/components/jupyter.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/common.py` & `skelebot-1.9.1/skelebot/common.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/scaffolding/scaffolder.py` & `skelebot-1.9.1/skelebot/systems/scaffolding/scaffolder.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/scaffolding/prompt.py` & `skelebot-1.9.1/skelebot/systems/scaffolding/prompt.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/execution/commandBuilder.py` & `skelebot-1.9.1/skelebot/systems/execution/commandBuilder.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/execution/docker.py` & `skelebot-1.9.1/skelebot/systems/execution/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 from ...systems.generators import dockerfile
 from ...systems.generators import dockerignore
 
 LOGIN_CMD = "docker login {}"
 BUILD_CMD = "docker build -t {image} ."
 RUN_CMD = "docker run --name {image}-{jobName} --rm {params} {image} /bin/bash -c \"{command}\""
 SAVE_CMD = "docker save -o {filename} {image}"
-TAG_CMD = "docker tag {src} {image}:{version}"
-PUSH_CMD = "docker push {image}:{version}"
+TAG_CMD = "docker tag {src} {image}:{tag}"
+PUSH_CMD = "docker push {image}:{tag}"
+
+def execute(cmd):
+    status = os.system(cmd)
+    if (status != 0):
+        raise Exception("Docker Command Failed")
 
 def login(host=None):
     """Login to the given Docker Host"""
 
     host = host if host is not None else ""
     loginCMD = LOGIN_CMD.format(host)
 
@@ -75,26 +80,22 @@
     return os.system(runCMD)
 
 def save(config, filename="image.img"):
     """Save the Image File to the disk"""
 
     return os.system(SAVE_CMD.format(image=config.getImageName(), filename=filename))
 
-def push(config, host=None, port=None, user=None):
+def push(config, host=None, port=None, user=None, tags=None):
     """Tag with version and latest and push the project Image to the provided Docker Image Host"""
 
     imageName = config.getImageName()
     port = ":{port}".format(port=port) if port is not None else ""
     host = "{host}{port}/".format(host=host, port=port) if host is not None else ""
     user = "{user}/".format(user=user) if user is not None else ""
     image = "{host}{user}{name}".format(host=host, port=port, user=user, name=imageName)
 
-    status = os.system(TAG_CMD.format(src=imageName, image=image, version=config.version))
-    if (status == 0):
-        status = os.system(TAG_CMD.format(src=imageName, image=image, version="latest"))
-    if (status == 0):
-        status = os.system(PUSH_CMD.format(image=image, version=config.version))
-    if (status == 0):
-        status = os.system(PUSH_CMD.format(image=image, version="latest"))
+    tags = [] if tags is None else tags
+    tags = tags + [config.version, "latest"]
 
-    if (status != 0):
-        raise Exception("Docker Push Failed")
+    for tag in tags:
+        execute(TAG_CMD.format(src=imageName, image=image, tag=tag))
+        execute(PUSH_CMD.format(image=image, tag=tag))
```

### Comparing `skelebot-1.9.0/skelebot/systems/execution/executor.py` & `skelebot-1.9.1/skelebot/systems/execution/executor.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/generators/readme.py` & `skelebot-1.9.1/skelebot/systems/generators/readme.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/generators/dockerignore.py` & `skelebot-1.9.1/skelebot/systems/generators/dockerignore.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/generators/yaml.py` & `skelebot-1.9.1/skelebot/systems/generators/yaml.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/generators/dockerfile.py` & `skelebot-1.9.1/skelebot/systems/generators/dockerfile.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot/systems/parsing/skeleParser.py` & `skelebot-1.9.1/skelebot/systems/parsing/skeleParser.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/README.md` & `skelebot-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/setup.py` & `skelebot-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `skelebot-1.9.0/skelebot.egg-info/SOURCES.txt` & `skelebot-1.9.1/skelebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

